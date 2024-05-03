# Comparing `tmp/mypy_boto3_datasync-1.34.91.tar.gz` & `tmp/mypy_boto3_datasync-1.34.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_datasync-1.34.91.tar", last modified: Wed Apr 24 19:19:04 2024, max compression
+gzip compressed data, was "mypy_boto3_datasync-1.34.98.tar", last modified: Fri May  3 19:32:42 2024, max compression
```

## Comparing `mypy_boto3_datasync-1.34.91.tar` & `mypy_boto3_datasync-1.34.98.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:04.979908 mypy_boto3_datasync-1.34.91/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 19:17:54.000000 mypy_boto3_datasync-1.34.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-04-24 19:19:04.979908 mypy_boto3_datasync-1.34.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-04-24 19:17:54.000000 mypy_boto3_datasync-1.34.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:04.979908 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-24 19:17:54.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-24 19:17:54.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-24 19:17:54.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48576 2024-04-24 19:17:54.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    48573 2024-04-24 19:17:54.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-04-24 19:17:55.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-04-24 19:17:55.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-04-24 19:17:55.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-04-24 19:17:55.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:17:54.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    53925 2024-04-24 19:17:56.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    53925 2024-04-24 19:17:55.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-24 19:17:54.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:04.979908 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-04-24 19:19:04.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-24 19:19:04.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:19:04.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:19:04.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 19:19:04.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 19:19:04.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:19:04.979908 mypy_boto3_datasync-1.34.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-24 19:17:54.000000 mypy_boto3_datasync-1.34.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:42.377290 mypy_boto3_datasync-1.34.98/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 19:32:00.000000 mypy_boto3_datasync-1.34.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-05-03 19:32:42.377290 mypy_boto3_datasync-1.34.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-05-03 19:32:00.000000 mypy_boto3_datasync-1.34.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:42.377290 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-03 19:32:00.000000 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-03 19:32:00.000000 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-03 19:32:00.000000 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48578 2024-05-03 19:32:00.000000 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48575 2024-05-03 19:32:00.000000 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-05-03 19:32:01.000000 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-05-03 19:32:00.000000 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-05-03 19:32:00.000000 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-03 19:32:00.000000 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:00.000000 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    54597 2024-05-03 19:32:02.000000 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54597 2024-05-03 19:32:02.000000 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 19:32:00.000000 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:42.377290 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-05-03 19:32:42.000000 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-03 19:32:42.000000 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:32:42.000000 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:32:42.000000 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-03 19:32:42.000000 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 19:32:42.000000 mypy_boto3_datasync-1.34.98/mypy_boto3_datasync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:32:42.377290 mypy_boto3_datasync-1.34.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-03 19:32:00.000000 mypy_boto3_datasync-1.34.98/setup.py
```

### Comparing `mypy_boto3_datasync-1.34.91/LICENSE` & `mypy_boto3_datasync-1.34.98/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_datasync-1.34.91/PKG-INFO` & `mypy_boto3_datasync-1.34.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datasync
-Version: 1.34.91
-Summary: Type annotations for boto3.DataSync 1.34.91 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.98
+Summary: Type annotations for boto3.DataSync 1.34.98 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datasync.svg?color=blue)](https://pypi.org/project/mypy-boto3-datasync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datasync)](https://pepy.tech/project/mypy-boto3-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataSync 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[boto3.DataSync 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_datasync-1.34.91/README.md` & `mypy_boto3_datasync-1.34.98/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datasync.svg?color=blue)](https://pypi.org/project/mypy-boto3-datasync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datasync)](https://pepy.tech/project/mypy-boto3-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataSync 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[boto3.DataSync 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/__init__.py` & `mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/__init__.pyi` & `mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/__main__.py` & `mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DataSync 1.34.91\n"
-        "Version:         1.34.91\n"
-        "Builder version: 7.23.2\n"
+        "Type annotations for boto3.DataSync 1.34.98\n"
+        "Version:         1.34.98\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.91")
+    print("1.34.98")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/client.py` & `mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,29 +70,29 @@
     DescribeLocationSmbResponseTypeDef,
     DescribeStorageSystemResourceMetricsResponseTypeDef,
     DescribeStorageSystemResourcesResponseTypeDef,
     DescribeStorageSystemResponseTypeDef,
     DescribeTaskExecutionResponseTypeDef,
     DescribeTaskResponseTypeDef,
     DiscoveryServerConfigurationTypeDef,
-    Ec2ConfigTypeDef,
+    Ec2ConfigUnionTypeDef,
     FilterRuleTypeDef,
     FsxProtocolTypeDef,
     HdfsNameNodeTypeDef,
     ListAgentsResponseTypeDef,
     ListDiscoveryJobsResponseTypeDef,
     ListLocationsResponseTypeDef,
     ListStorageSystemsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTaskExecutionsResponseTypeDef,
     ListTasksResponseTypeDef,
     LocationFilterTypeDef,
     ManifestConfigTypeDef,
     NfsMountOptionsTypeDef,
-    OnPremConfigTypeDef,
+    OnPremConfigUnionTypeDef,
     OptionsTypeDef,
     QopConfigurationTypeDef,
     S3ConfigTypeDef,
     SmbMountOptionsTypeDef,
     StartDiscoveryJobResponseTypeDef,
     StartTaskExecutionResponseTypeDef,
     TagListEntryTypeDef,
@@ -222,15 +222,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_azure_blob)
         """
 
     def create_location_efs(
         self,
         *,
         EfsFilesystemArn: str,
-        Ec2Config: Ec2ConfigTypeDef,
+        Ec2Config: Ec2ConfigUnionTypeDef,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         AccessPointArn: str = ...,
         FileSystemAccessRoleArn: str = ...,
         InTransitEncryption: EfsInTransitEncryptionType = ...,
     ) -> CreateLocationEfsResponseTypeDef:
         """
@@ -331,15 +331,15 @@
         """
 
     def create_location_nfs(
         self,
         *,
         Subdirectory: str,
         ServerHostname: str,
-        OnPremConfig: OnPremConfigTypeDef,
+        OnPremConfig: OnPremConfigUnionTypeDef,
         MountOptions: NfsMountOptionsTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
     ) -> CreateLocationNfsResponseTypeDef:
         """
         Creates a transfer *location* for a Network File System (NFS) file server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_nfs)
@@ -906,15 +906,15 @@
         """
 
     def update_location_nfs(
         self,
         *,
         LocationArn: str,
         Subdirectory: str = ...,
-        OnPremConfig: OnPremConfigTypeDef = ...,
+        OnPremConfig: OnPremConfigUnionTypeDef = ...,
         MountOptions: NfsMountOptionsTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Modifies some configurations of the Network File System (NFS) transfer location
         that you're using with
         DataSync.
 
@@ -931,17 +931,16 @@
         Subdirectory: str = ...,
         AccessKey: str = ...,
         SecretKey: str = ...,
         AgentArns: Sequence[str] = ...,
         ServerCertificate: BlobTypeDef = ...,
     ) -> Dict[str, Any]:
         """
-        Updates some parameters of an existing object storage location that DataSync
-        accesses for a
-        transfer.
+        Updates some parameters of an existing DataSync location for an object storage
+        system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_object_storage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_location_object_storage)
         """
 
     def update_location_smb(
         self,
```

### Comparing `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/client.pyi` & `mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -70,29 +70,29 @@
     DescribeLocationSmbResponseTypeDef,
     DescribeStorageSystemResourceMetricsResponseTypeDef,
     DescribeStorageSystemResourcesResponseTypeDef,
     DescribeStorageSystemResponseTypeDef,
     DescribeTaskExecutionResponseTypeDef,
     DescribeTaskResponseTypeDef,
     DiscoveryServerConfigurationTypeDef,
-    Ec2ConfigTypeDef,
+    Ec2ConfigUnionTypeDef,
     FilterRuleTypeDef,
     FsxProtocolTypeDef,
     HdfsNameNodeTypeDef,
     ListAgentsResponseTypeDef,
     ListDiscoveryJobsResponseTypeDef,
     ListLocationsResponseTypeDef,
     ListStorageSystemsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTaskExecutionsResponseTypeDef,
     ListTasksResponseTypeDef,
     LocationFilterTypeDef,
     ManifestConfigTypeDef,
     NfsMountOptionsTypeDef,
-    OnPremConfigTypeDef,
+    OnPremConfigUnionTypeDef,
     OptionsTypeDef,
     QopConfigurationTypeDef,
     S3ConfigTypeDef,
     SmbMountOptionsTypeDef,
     StartDiscoveryJobResponseTypeDef,
     StartTaskExecutionResponseTypeDef,
     TagListEntryTypeDef,
@@ -219,15 +219,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_azure_blob)
         """
 
     def create_location_efs(
         self,
         *,
         EfsFilesystemArn: str,
-        Ec2Config: Ec2ConfigTypeDef,
+        Ec2Config: Ec2ConfigUnionTypeDef,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         AccessPointArn: str = ...,
         FileSystemAccessRoleArn: str = ...,
         InTransitEncryption: EfsInTransitEncryptionType = ...,
     ) -> CreateLocationEfsResponseTypeDef:
         """
@@ -328,15 +328,15 @@
         """
 
     def create_location_nfs(
         self,
         *,
         Subdirectory: str,
         ServerHostname: str,
-        OnPremConfig: OnPremConfigTypeDef,
+        OnPremConfig: OnPremConfigUnionTypeDef,
         MountOptions: NfsMountOptionsTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
     ) -> CreateLocationNfsResponseTypeDef:
         """
         Creates a transfer *location* for a Network File System (NFS) file server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_nfs)
@@ -903,15 +903,15 @@
         """
 
     def update_location_nfs(
         self,
         *,
         LocationArn: str,
         Subdirectory: str = ...,
-        OnPremConfig: OnPremConfigTypeDef = ...,
+        OnPremConfig: OnPremConfigUnionTypeDef = ...,
         MountOptions: NfsMountOptionsTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Modifies some configurations of the Network File System (NFS) transfer location
         that you're using with
         DataSync.
 
@@ -928,17 +928,16 @@
         Subdirectory: str = ...,
         AccessKey: str = ...,
         SecretKey: str = ...,
         AgentArns: Sequence[str] = ...,
         ServerCertificate: BlobTypeDef = ...,
     ) -> Dict[str, Any]:
         """
-        Updates some parameters of an existing object storage location that DataSync
-        accesses for a
-        transfer.
+        Updates some parameters of an existing DataSync location for an object storage
+        system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_object_storage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_location_object_storage)
         """
 
     def update_location_smb(
         self,
```

### Comparing `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/literals.py` & `mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/literals.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/literals.pyi` & `mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/paginator.py` & `mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/paginator.pyi` & `mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/type_defs.py` & `mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,20 +98,22 @@
     "DeleteLocationRequestRequestTypeDef",
     "DeleteTaskRequestRequestTypeDef",
     "DescribeAgentRequestRequestTypeDef",
     "PrivateLinkConfigTypeDef",
     "DescribeDiscoveryJobRequestRequestTypeDef",
     "DescribeLocationAzureBlobRequestRequestTypeDef",
     "DescribeLocationEfsRequestRequestTypeDef",
+    "Ec2ConfigOutputTypeDef",
     "DescribeLocationFsxLustreRequestRequestTypeDef",
     "DescribeLocationFsxOntapRequestRequestTypeDef",
     "DescribeLocationFsxOpenZfsRequestRequestTypeDef",
     "DescribeLocationFsxWindowsRequestRequestTypeDef",
     "DescribeLocationHdfsRequestRequestTypeDef",
     "DescribeLocationNfsRequestRequestTypeDef",
+    "OnPremConfigOutputTypeDef",
     "DescribeLocationObjectStorageRequestRequestTypeDef",
     "DescribeLocationS3RequestRequestTypeDef",
     "DescribeLocationSmbRequestRequestTypeDef",
     "DescribeStorageSystemRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "TimestampTypeDef",
     "DescribeStorageSystemResourcesRequestRequestTypeDef",
@@ -178,30 +180,32 @@
     "StartTaskExecutionResponseTypeDef",
     "AgentListEntryTypeDef",
     "CreateLocationAzureBlobRequestRequestTypeDef",
     "UpdateLocationAzureBlobRequestRequestTypeDef",
     "CreateLocationObjectStorageRequestRequestTypeDef",
     "UpdateLocationObjectStorageRequestRequestTypeDef",
     "CreateLocationEfsRequestRequestTypeDef",
-    "DescribeLocationEfsResponseTypeDef",
     "CreateLocationHdfsRequestRequestTypeDef",
     "DescribeLocationHdfsResponseTypeDef",
     "UpdateLocationHdfsRequestRequestTypeDef",
     "FsxProtocolNfsTypeDef",
     "CreateLocationNfsRequestRequestTypeDef",
-    "DescribeLocationNfsResponseTypeDef",
     "UpdateLocationNfsRequestRequestTypeDef",
     "CreateLocationS3RequestRequestTypeDef",
     "DescribeLocationS3ResponseTypeDef",
     "CreateLocationSmbRequestRequestTypeDef",
     "DescribeLocationSmbResponseTypeDef",
     "FsxProtocolSmbTypeDef",
     "UpdateLocationSmbRequestRequestTypeDef",
     "UpdateTaskExecutionRequestRequestTypeDef",
     "DescribeAgentResponseTypeDef",
+    "DescribeLocationEfsResponseTypeDef",
+    "Ec2ConfigUnionTypeDef",
+    "DescribeLocationNfsResponseTypeDef",
+    "OnPremConfigUnionTypeDef",
     "ListAgentsRequestListAgentsPaginateTypeDef",
     "ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef",
     "ListStorageSystemsRequestListStorageSystemsPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef",
     "DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef",
     "DescribeStorageSystemResourceMetricsRequestRequestTypeDef",
@@ -425,14 +429,21 @@
 )
 DescribeLocationEfsRequestRequestTypeDef = TypedDict(
     "DescribeLocationEfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
+Ec2ConfigOutputTypeDef = TypedDict(
+    "Ec2ConfigOutputTypeDef",
+    {
+        "SubnetArn": str,
+        "SecurityGroupArns": List[str],
+    },
+)
 DescribeLocationFsxLustreRequestRequestTypeDef = TypedDict(
     "DescribeLocationFsxLustreRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 DescribeLocationFsxOntapRequestRequestTypeDef = TypedDict(
@@ -461,14 +472,20 @@
 )
 DescribeLocationNfsRequestRequestTypeDef = TypedDict(
     "DescribeLocationNfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
+OnPremConfigOutputTypeDef = TypedDict(
+    "OnPremConfigOutputTypeDef",
+    {
+        "AgentArns": List[str],
+    },
+)
 DescribeLocationObjectStorageRequestRequestTypeDef = TypedDict(
     "DescribeLocationObjectStorageRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 DescribeLocationS3RequestRequestTypeDef = TypedDict(
@@ -1002,16 +1019,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagListEntryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 StartDiscoveryJobResponseTypeDef = TypedDict(
     "StartDiscoveryJobResponseTypeDef",
     {
         "DiscoveryJobArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1094,27 +1111,14 @@
         "Subdirectory": NotRequired[str],
         "Tags": NotRequired[Sequence[TagListEntryTypeDef]],
         "AccessPointArn": NotRequired[str],
         "FileSystemAccessRoleArn": NotRequired[str],
         "InTransitEncryption": NotRequired[EfsInTransitEncryptionType],
     },
 )
-DescribeLocationEfsResponseTypeDef = TypedDict(
-    "DescribeLocationEfsResponseTypeDef",
-    {
-        "LocationArn": str,
-        "LocationUri": str,
-        "Ec2Config": Ec2ConfigTypeDef,
-        "CreationTime": datetime,
-        "AccessPointArn": str,
-        "FileSystemAccessRoleArn": str,
-        "InTransitEncryption": EfsInTransitEncryptionType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 CreateLocationHdfsRequestRequestTypeDef = TypedDict(
     "CreateLocationHdfsRequestRequestTypeDef",
     {
         "NameNodes": Sequence[HdfsNameNodeTypeDef],
         "AuthenticationType": HdfsAuthenticationTypeType,
         "AgentArns": Sequence[str],
         "Subdirectory": NotRequired[str],
@@ -1177,25 +1181,14 @@
         "Subdirectory": str,
         "ServerHostname": str,
         "OnPremConfig": OnPremConfigTypeDef,
         "MountOptions": NotRequired[NfsMountOptionsTypeDef],
         "Tags": NotRequired[Sequence[TagListEntryTypeDef]],
     },
 )
-DescribeLocationNfsResponseTypeDef = TypedDict(
-    "DescribeLocationNfsResponseTypeDef",
-    {
-        "LocationArn": str,
-        "LocationUri": str,
-        "OnPremConfig": OnPremConfigTypeDef,
-        "MountOptions": NfsMountOptionsTypeDef,
-        "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 UpdateLocationNfsRequestRequestTypeDef = TypedDict(
     "UpdateLocationNfsRequestRequestTypeDef",
     {
         "LocationArn": str,
         "Subdirectory": NotRequired[str],
         "OnPremConfig": NotRequired[OnPremConfigTypeDef],
         "MountOptions": NotRequired[NfsMountOptionsTypeDef],
@@ -1288,14 +1281,40 @@
         "CreationTime": datetime,
         "EndpointType": EndpointTypeType,
         "PrivateLinkConfig": PrivateLinkConfigTypeDef,
         "Platform": PlatformTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DescribeLocationEfsResponseTypeDef = TypedDict(
+    "DescribeLocationEfsResponseTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "Ec2Config": Ec2ConfigOutputTypeDef,
+        "CreationTime": datetime,
+        "AccessPointArn": str,
+        "FileSystemAccessRoleArn": str,
+        "InTransitEncryption": EfsInTransitEncryptionType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+Ec2ConfigUnionTypeDef = Union[Ec2ConfigTypeDef, Ec2ConfigOutputTypeDef]
+DescribeLocationNfsResponseTypeDef = TypedDict(
+    "DescribeLocationNfsResponseTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "OnPremConfig": OnPremConfigOutputTypeDef,
+        "MountOptions": NfsMountOptionsTypeDef,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+OnPremConfigUnionTypeDef = Union[OnPremConfigTypeDef, OnPremConfigOutputTypeDef]
 ListAgentsRequestListAgentsPaginateTypeDef = TypedDict(
     "ListAgentsRequestListAgentsPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef = TypedDict(
@@ -1348,16 +1367,16 @@
         "NextToken": NotRequired[str],
     },
 )
 ListDiscoveryJobsResponseTypeDef = TypedDict(
     "ListDiscoveryJobsResponseTypeDef",
     {
         "DiscoveryJobs": List[DiscoveryJobListEntryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListLocationsRequestListLocationsPaginateTypeDef = TypedDict(
     "ListLocationsRequestListLocationsPaginateTypeDef",
     {
         "Filters": NotRequired[Sequence[LocationFilterTypeDef]],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -1371,32 +1390,32 @@
         "Filters": NotRequired[Sequence[LocationFilterTypeDef]],
     },
 )
 ListLocationsResponseTypeDef = TypedDict(
     "ListLocationsResponseTypeDef",
     {
         "Locations": List[LocationListEntryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListStorageSystemsResponseTypeDef = TypedDict(
     "ListStorageSystemsResponseTypeDef",
     {
         "StorageSystems": List[StorageSystemListEntryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTaskExecutionsResponseTypeDef = TypedDict(
     "ListTaskExecutionsResponseTypeDef",
     {
         "TaskExecutions": List[TaskExecutionListEntryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTasksRequestListTasksPaginateTypeDef = TypedDict(
     "ListTasksRequestListTasksPaginateTypeDef",
     {
         "Filters": NotRequired[Sequence[TaskFilterTypeDef]],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -1410,16 +1429,16 @@
         "Filters": NotRequired[Sequence[TaskFilterTypeDef]],
     },
 )
 ListTasksResponseTypeDef = TypedDict(
     "ListTasksResponseTypeDef",
     {
         "Tasks": List[TaskListEntryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 NetAppONTAPClusterTypeDef = TypedDict(
     "NetAppONTAPClusterTypeDef",
     {
         "CifsShareCount": NotRequired[int],
         "NfsExportedVolumes": NotRequired[int],
@@ -1503,16 +1522,16 @@
         "S3": S3ManifestConfigTypeDef,
     },
 )
 ListAgentsResponseTypeDef = TypedDict(
     "ListAgentsResponseTypeDef",
     {
         "Agents": List[AgentListEntryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 FsxProtocolTypeDef = TypedDict(
     "FsxProtocolTypeDef",
     {
         "NFS": NotRequired[FsxProtocolNfsTypeDef],
         "SMB": NotRequired[FsxProtocolSmbTypeDef],
@@ -1598,24 +1617,24 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeStorageSystemResourcesResponseTypeDef = TypedDict(
     "DescribeStorageSystemResourcesResponseTypeDef",
     {
         "ResourceDetails": ResourceDetailsTypeDef,
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeStorageSystemResourceMetricsResponseTypeDef = TypedDict(
     "DescribeStorageSystemResourceMetricsResponseTypeDef",
     {
         "Metrics": List[ResourceMetricsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateTaskRequestRequestTypeDef = TypedDict(
     "CreateTaskRequestRequestTypeDef",
     {
         "SourceLocationArn": str,
         "DestinationLocationArn": str,
```

### Comparing `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/type_defs.pyi` & `mypy_boto3_datasync-1.34.98/mypy_boto3_datasync/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -98,20 +98,22 @@
     "DeleteLocationRequestRequestTypeDef",
     "DeleteTaskRequestRequestTypeDef",
     "DescribeAgentRequestRequestTypeDef",
     "PrivateLinkConfigTypeDef",
     "DescribeDiscoveryJobRequestRequestTypeDef",
     "DescribeLocationAzureBlobRequestRequestTypeDef",
     "DescribeLocationEfsRequestRequestTypeDef",
+    "Ec2ConfigOutputTypeDef",
     "DescribeLocationFsxLustreRequestRequestTypeDef",
     "DescribeLocationFsxOntapRequestRequestTypeDef",
     "DescribeLocationFsxOpenZfsRequestRequestTypeDef",
     "DescribeLocationFsxWindowsRequestRequestTypeDef",
     "DescribeLocationHdfsRequestRequestTypeDef",
     "DescribeLocationNfsRequestRequestTypeDef",
+    "OnPremConfigOutputTypeDef",
     "DescribeLocationObjectStorageRequestRequestTypeDef",
     "DescribeLocationS3RequestRequestTypeDef",
     "DescribeLocationSmbRequestRequestTypeDef",
     "DescribeStorageSystemRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "TimestampTypeDef",
     "DescribeStorageSystemResourcesRequestRequestTypeDef",
@@ -178,30 +180,32 @@
     "StartTaskExecutionResponseTypeDef",
     "AgentListEntryTypeDef",
     "CreateLocationAzureBlobRequestRequestTypeDef",
     "UpdateLocationAzureBlobRequestRequestTypeDef",
     "CreateLocationObjectStorageRequestRequestTypeDef",
     "UpdateLocationObjectStorageRequestRequestTypeDef",
     "CreateLocationEfsRequestRequestTypeDef",
-    "DescribeLocationEfsResponseTypeDef",
     "CreateLocationHdfsRequestRequestTypeDef",
     "DescribeLocationHdfsResponseTypeDef",
     "UpdateLocationHdfsRequestRequestTypeDef",
     "FsxProtocolNfsTypeDef",
     "CreateLocationNfsRequestRequestTypeDef",
-    "DescribeLocationNfsResponseTypeDef",
     "UpdateLocationNfsRequestRequestTypeDef",
     "CreateLocationS3RequestRequestTypeDef",
     "DescribeLocationS3ResponseTypeDef",
     "CreateLocationSmbRequestRequestTypeDef",
     "DescribeLocationSmbResponseTypeDef",
     "FsxProtocolSmbTypeDef",
     "UpdateLocationSmbRequestRequestTypeDef",
     "UpdateTaskExecutionRequestRequestTypeDef",
     "DescribeAgentResponseTypeDef",
+    "DescribeLocationEfsResponseTypeDef",
+    "Ec2ConfigUnionTypeDef",
+    "DescribeLocationNfsResponseTypeDef",
+    "OnPremConfigUnionTypeDef",
     "ListAgentsRequestListAgentsPaginateTypeDef",
     "ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef",
     "ListStorageSystemsRequestListStorageSystemsPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef",
     "DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef",
     "DescribeStorageSystemResourceMetricsRequestRequestTypeDef",
@@ -425,14 +429,21 @@
 )
 DescribeLocationEfsRequestRequestTypeDef = TypedDict(
     "DescribeLocationEfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
+Ec2ConfigOutputTypeDef = TypedDict(
+    "Ec2ConfigOutputTypeDef",
+    {
+        "SubnetArn": str,
+        "SecurityGroupArns": List[str],
+    },
+)
 DescribeLocationFsxLustreRequestRequestTypeDef = TypedDict(
     "DescribeLocationFsxLustreRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 DescribeLocationFsxOntapRequestRequestTypeDef = TypedDict(
@@ -461,14 +472,20 @@
 )
 DescribeLocationNfsRequestRequestTypeDef = TypedDict(
     "DescribeLocationNfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
+OnPremConfigOutputTypeDef = TypedDict(
+    "OnPremConfigOutputTypeDef",
+    {
+        "AgentArns": List[str],
+    },
+)
 DescribeLocationObjectStorageRequestRequestTypeDef = TypedDict(
     "DescribeLocationObjectStorageRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 DescribeLocationS3RequestRequestTypeDef = TypedDict(
@@ -1002,16 +1019,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagListEntryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 StartDiscoveryJobResponseTypeDef = TypedDict(
     "StartDiscoveryJobResponseTypeDef",
     {
         "DiscoveryJobArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1094,27 +1111,14 @@
         "Subdirectory": NotRequired[str],
         "Tags": NotRequired[Sequence[TagListEntryTypeDef]],
         "AccessPointArn": NotRequired[str],
         "FileSystemAccessRoleArn": NotRequired[str],
         "InTransitEncryption": NotRequired[EfsInTransitEncryptionType],
     },
 )
-DescribeLocationEfsResponseTypeDef = TypedDict(
-    "DescribeLocationEfsResponseTypeDef",
-    {
-        "LocationArn": str,
-        "LocationUri": str,
-        "Ec2Config": Ec2ConfigTypeDef,
-        "CreationTime": datetime,
-        "AccessPointArn": str,
-        "FileSystemAccessRoleArn": str,
-        "InTransitEncryption": EfsInTransitEncryptionType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 CreateLocationHdfsRequestRequestTypeDef = TypedDict(
     "CreateLocationHdfsRequestRequestTypeDef",
     {
         "NameNodes": Sequence[HdfsNameNodeTypeDef],
         "AuthenticationType": HdfsAuthenticationTypeType,
         "AgentArns": Sequence[str],
         "Subdirectory": NotRequired[str],
@@ -1177,25 +1181,14 @@
         "Subdirectory": str,
         "ServerHostname": str,
         "OnPremConfig": OnPremConfigTypeDef,
         "MountOptions": NotRequired[NfsMountOptionsTypeDef],
         "Tags": NotRequired[Sequence[TagListEntryTypeDef]],
     },
 )
-DescribeLocationNfsResponseTypeDef = TypedDict(
-    "DescribeLocationNfsResponseTypeDef",
-    {
-        "LocationArn": str,
-        "LocationUri": str,
-        "OnPremConfig": OnPremConfigTypeDef,
-        "MountOptions": NfsMountOptionsTypeDef,
-        "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 UpdateLocationNfsRequestRequestTypeDef = TypedDict(
     "UpdateLocationNfsRequestRequestTypeDef",
     {
         "LocationArn": str,
         "Subdirectory": NotRequired[str],
         "OnPremConfig": NotRequired[OnPremConfigTypeDef],
         "MountOptions": NotRequired[NfsMountOptionsTypeDef],
@@ -1288,14 +1281,40 @@
         "CreationTime": datetime,
         "EndpointType": EndpointTypeType,
         "PrivateLinkConfig": PrivateLinkConfigTypeDef,
         "Platform": PlatformTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DescribeLocationEfsResponseTypeDef = TypedDict(
+    "DescribeLocationEfsResponseTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "Ec2Config": Ec2ConfigOutputTypeDef,
+        "CreationTime": datetime,
+        "AccessPointArn": str,
+        "FileSystemAccessRoleArn": str,
+        "InTransitEncryption": EfsInTransitEncryptionType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+Ec2ConfigUnionTypeDef = Union[Ec2ConfigTypeDef, Ec2ConfigOutputTypeDef]
+DescribeLocationNfsResponseTypeDef = TypedDict(
+    "DescribeLocationNfsResponseTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "OnPremConfig": OnPremConfigOutputTypeDef,
+        "MountOptions": NfsMountOptionsTypeDef,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+OnPremConfigUnionTypeDef = Union[OnPremConfigTypeDef, OnPremConfigOutputTypeDef]
 ListAgentsRequestListAgentsPaginateTypeDef = TypedDict(
     "ListAgentsRequestListAgentsPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef = TypedDict(
@@ -1348,16 +1367,16 @@
         "NextToken": NotRequired[str],
     },
 )
 ListDiscoveryJobsResponseTypeDef = TypedDict(
     "ListDiscoveryJobsResponseTypeDef",
     {
         "DiscoveryJobs": List[DiscoveryJobListEntryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListLocationsRequestListLocationsPaginateTypeDef = TypedDict(
     "ListLocationsRequestListLocationsPaginateTypeDef",
     {
         "Filters": NotRequired[Sequence[LocationFilterTypeDef]],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -1371,32 +1390,32 @@
         "Filters": NotRequired[Sequence[LocationFilterTypeDef]],
     },
 )
 ListLocationsResponseTypeDef = TypedDict(
     "ListLocationsResponseTypeDef",
     {
         "Locations": List[LocationListEntryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListStorageSystemsResponseTypeDef = TypedDict(
     "ListStorageSystemsResponseTypeDef",
     {
         "StorageSystems": List[StorageSystemListEntryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTaskExecutionsResponseTypeDef = TypedDict(
     "ListTaskExecutionsResponseTypeDef",
     {
         "TaskExecutions": List[TaskExecutionListEntryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTasksRequestListTasksPaginateTypeDef = TypedDict(
     "ListTasksRequestListTasksPaginateTypeDef",
     {
         "Filters": NotRequired[Sequence[TaskFilterTypeDef]],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -1410,16 +1429,16 @@
         "Filters": NotRequired[Sequence[TaskFilterTypeDef]],
     },
 )
 ListTasksResponseTypeDef = TypedDict(
     "ListTasksResponseTypeDef",
     {
         "Tasks": List[TaskListEntryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 NetAppONTAPClusterTypeDef = TypedDict(
     "NetAppONTAPClusterTypeDef",
     {
         "CifsShareCount": NotRequired[int],
         "NfsExportedVolumes": NotRequired[int],
@@ -1503,16 +1522,16 @@
         "S3": S3ManifestConfigTypeDef,
     },
 )
 ListAgentsResponseTypeDef = TypedDict(
     "ListAgentsResponseTypeDef",
     {
         "Agents": List[AgentListEntryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 FsxProtocolTypeDef = TypedDict(
     "FsxProtocolTypeDef",
     {
         "NFS": NotRequired[FsxProtocolNfsTypeDef],
         "SMB": NotRequired[FsxProtocolSmbTypeDef],
@@ -1598,24 +1617,24 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeStorageSystemResourcesResponseTypeDef = TypedDict(
     "DescribeStorageSystemResourcesResponseTypeDef",
     {
         "ResourceDetails": ResourceDetailsTypeDef,
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeStorageSystemResourceMetricsResponseTypeDef = TypedDict(
     "DescribeStorageSystemResourceMetricsResponseTypeDef",
     {
         "Metrics": List[ResourceMetricsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateTaskRequestRequestTypeDef = TypedDict(
     "CreateTaskRequestRequestTypeDef",
     {
         "SourceLocationArn": str,
         "DestinationLocationArn": str,
```

### Comparing `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync.egg-info/PKG-INFO` & `mypy_boto3_datasync-1.34.98/mypy_boto3_datasync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datasync
-Version: 1.34.91
-Summary: Type annotations for boto3.DataSync 1.34.91 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.98
+Summary: Type annotations for boto3.DataSync 1.34.98 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datasync.svg?color=blue)](https://pypi.org/project/mypy-boto3-datasync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datasync)](https://pepy.tech/project/mypy-boto3-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataSync 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[boto3.DataSync 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync.egg-info/SOURCES.txt` & `mypy_boto3_datasync-1.34.98/mypy_boto3_datasync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_datasync-1.34.91/setup.py` & `mypy_boto3_datasync-1.34.98/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-datasync",
-    version="1.34.91",
+    version="1.34.98",
     packages=["mypy_boto3_datasync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.DataSync 1.34.91 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.DataSync 1.34.98 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```


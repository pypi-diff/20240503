# Comparing `tmp/deepset_cloud_sdk-1.0.0.tar.gz` & `tmp/deepset_cloud_sdk-1.0.1.tar.gz`

## Comparing `deepset_cloud_sdk-1.0.0.tar` & `deepset_cloud_sdk-1.0.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/mkdocs.yml
--rw-r--r--   0        0        0   475761 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/assets/cli.gif
--rw-r--r--   0        0        0    48074 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/assets/logo.png
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/README.md
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/__about__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/__init__.py
--rw-r--r--   0        0        0    12518 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/cli.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/models.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_api/config.py
--rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_api/deepset_cloud_api.py
--rw-r--r--   0        0        0    10801 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_api/files.py
--rw-r--r--   0        0        0    10389 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_api/upload_sessions.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_s3/__init__.py
--rw-r--r--   0        0        0    11656 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_s3/upload.py
--rw-r--r--   0        0        0    31216 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_service/files_service.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_utils/__init__.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_utils/datetime.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/workflows/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/workflows/async_client/__init__.py
--rw-r--r--   0        0        0    10241 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/workflows/async_client/files.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/workflows/sync_client/__init__.py
--rw-r--r--   0        0        0    10049 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/workflows/sync_client/files.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/workflows/sync_client/utils.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/index.md
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/upload_files.md
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/_images/favicon.svg
--rw-r--r--   0        0        0    15589 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/_images/white-logo.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/_pydoc/__init__.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/_pydoc/renderers.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/_pydoc/requirements.txt
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/_pydoc/config/async_client.yml
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/_pydoc/config/cli.yml
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/_pydoc/config/sync_client.yml
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/_stylesheets/extra.css
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/examples/cli/README.md
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/examples/data/example.pdf
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/examples/data/example.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/examples/data/example.txt.meta.json
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/examples/sdk/README.md
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/examples/sdk/upload.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/test-upload/example.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/test-upload/example.txt.meta.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/test-upload/example2.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/test-upload/example2.txt.meta.json
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/.gitignore
--rw-r--r--   0        0        0    10241 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/LICENSE
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/README.md
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/mkdocs.yml
+-rw-r--r--   0        0        0   475761 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/assets/cli.gif
+-rw-r--r--   0        0        0    48074 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/assets/logo.png
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/README.md
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/__about__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/__init__.py
+-rw-r--r--   0        0        0    12518 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/cli.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/models.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_api/config.py
+-rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_api/deepset_cloud_api.py
+-rw-r--r--   0        0        0    10801 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_api/files.py
+-rw-r--r--   0        0        0    10389 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_api/upload_sessions.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_s3/__init__.py
+-rw-r--r--   0        0        0    11656 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_s3/upload.py
+-rw-r--r--   0        0        0    31123 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_service/files_service.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_utils/__init__.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_utils/datetime.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/workflows/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/workflows/async_client/__init__.py
+-rw-r--r--   0        0        0    10241 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/workflows/async_client/files.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/workflows/sync_client/__init__.py
+-rw-r--r--   0        0        0    10049 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/workflows/sync_client/files.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/workflows/sync_client/utils.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/index.md
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/upload_files.md
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/_images/favicon.svg
+-rw-r--r--   0        0        0    15589 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/_images/white-logo.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/_pydoc/__init__.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/_pydoc/renderers.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/_pydoc/requirements.txt
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/_pydoc/config/async_client.yml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/_pydoc/config/cli.yml
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/_pydoc/config/sync_client.yml
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/_stylesheets/extra.css
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/examples/cli/README.md
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/examples/data/example.pdf
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/examples/data/example.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/examples/data/example.txt.meta.json
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/examples/sdk/README.md
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/examples/sdk/upload.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/test-upload/example.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/test-upload/example.txt.meta.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/test-upload/example2.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/test-upload/example2.txt.meta.json
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/.gitignore
+-rw-r--r--   0        0        0    10241 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/README.md
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/PKG-INFO
```

### Comparing `deepset_cloud_sdk-1.0.0/.pre-commit-config.yaml` & `deepset_cloud_sdk-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/CONTRIBUTING.md` & `deepset_cloud_sdk-1.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/mkdocs.yml` & `deepset_cloud_sdk-1.0.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/assets/cli.gif` & `deepset_cloud_sdk-1.0.1/assets/cli.gif`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/assets/logo.png` & `deepset_cloud_sdk-1.0.1/assets/logo.png`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/README.md` & `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/README.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/cli.py` & `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_api/config.py` & `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_api/config.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_api/deepset_cloud_api.py` & `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_api/deepset_cloud_api.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_api/files.py` & `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_api/files.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_api/upload_sessions.py` & `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_api/upload_sessions.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_s3/upload.py` & `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_s3/upload.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_service/files_service.py` & `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_service/files_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for all file-related operations."""
+
 from __future__ import annotations
 
 import asyncio
 import json
 import os
 import time
 from collections import defaultdict
@@ -31,14 +32,15 @@
 )
 from deepset_cloud_sdk._s3.upload import S3, S3UploadResult, S3UploadSummary
 from deepset_cloud_sdk.models import DeepsetCloudFile
 
 logger = structlog.get_logger(__name__)
 
 SUPPORTED_TYPE_SUFFIXES = [".csv", ".docx", ".html", ".json", ".md", ".txt", ".pdf", ".pptx", ".xlsx", ".xml"]
+META_SUFFIX = ".meta.json"
 DIRECT_UPLOAD_THRESHOLD = 20
 
 
 class FilesService:
     """Service for all file-related operations."""
 
     def __init__(self, upload_sessions: UploadSessionsAPI, files: FilesAPI, s3: S3):
@@ -193,19 +195,19 @@
         """
         if len(file_paths) <= DIRECT_UPLOAD_THRESHOLD:
             logger.info("Uploading files to deepset Cloud.", file_paths=file_paths)
             _coroutines = []
             _raw_files = [
                 path
                 for path in file_paths
-                if path.suffix.lower() in SUPPORTED_TYPE_SUFFIXES and not path.name.endswith(".meta.json")
+                if path.suffix in SUPPORTED_TYPE_SUFFIXES and not path.name.endswith(META_SUFFIX)
             ]
             for file_path in _raw_files:
                 meta: Dict[str, Any] = {}
-                meta_path = Path(str(file_path) + ".meta.json")
+                meta_path = Path(str(file_path) + META_SUFFIX)
                 if meta_path in file_paths:
                     with meta_path.open("r") as meta_file:
                         meta = json.loads(meta_file.read())
 
                 _coroutines.append(
                     self._wrapped_direct_upload_path(
                         workspace_name=workspace_name, file_path=file_path, meta=meta, write_mode=write_mode
@@ -236,15 +238,15 @@
                 successful_uploads=upload_summary.successful_upload_count,
                 failed_uploads=upload_summary.failed_upload_count,
                 failed=upload_summary.failed,
             )
 
         # wait for ingestion to finish
         if blocking:
-            total_files = len(list(filter(lambda x: not os.path.basename(x).endswith(".meta.json"), file_paths)))
+            total_files = len(list(filter(lambda x: not os.path.basename(x).endswith(META_SUFFIX), file_paths)))
             await self._wait_for_finished(
                 workspace_name=workspace_name,
                 session_id=upload_session.session_id,
                 total_files=total_files,
                 timeout_s=timeout_s,
                 show_progress=show_progress,
             )
@@ -278,32 +280,32 @@
         It also validates if there are metadata files mapped to not existing raw files.
 
         :param file_paths: A list of paths to upload.
         :raises ValueError: If the file paths are invalid.
         """
         logger.info("Validating file paths and metadata.")
         for file_path in file_paths:
-            if file_path.suffix.lower() not in SUPPORTED_TYPE_SUFFIXES:
+            if file_path.suffix not in SUPPORTED_TYPE_SUFFIXES:
                 raise ValueError(
                     f"Invalid file extension: {file_path.suffix}. Refer to the list of supported file types in `SUPPORTED_TYPE_SUFFIXES`. "
                     "Metadata files should have the `.meta.json` extension."
                 )
         meta_file_names = list(
             map(
                 lambda fp: os.path.basename(fp),
-                [file_path for file_path in file_paths if str(file_path).lower().endswith(".meta.json")],
+                [file_path for file_path in file_paths if str(file_path).endswith(META_SUFFIX)],
             )
         )
         file_names = list(map(lambda fp: os.path.basename(fp), file_paths))
-        file_name_set = set(filter(lambda fn: not fn.lower().endswith(".meta.json"), file_names))
+        file_name_set = set(filter(lambda fn: not fn.endswith(META_SUFFIX), file_names))
 
         not_mapped_meta_files = [
             meta_file_name
             for meta_file_name in meta_file_names
-            if meta_file_name.lower().split(".meta.json")[0] not in file_name_set
+            if meta_file_name.split(META_SUFFIX)[0] not in file_name_set
         ]
 
         if len(not_mapped_meta_files) > 0:
             raise ValueError(
                 f"Metadata files without corresponding files were found: {not_mapped_meta_files}. "
                 "Make sure each metadata file has a corresponding file. "
                 "Map the files using file names like this: '<file_name>' and '<file_name>.meta.json'. "
@@ -337,15 +339,15 @@
         :param desired_file_types: A list of desired file types.
         :return: A list of desired file types that can be processed by deepset Cloud.
         """
         if not desired_file_types:
             return SUPPORTED_TYPE_SUFFIXES
 
         desired_types_processed: Set[str] = {
-            str(file_type).lower() if str(file_type).startswith(".") else f".{str(file_type).lower()}"
+            str(file_type) if str(file_type).startswith(".") else f".{str(file_type)}"
             for file_type in desired_file_types
         }
         allowed_types: Set[str] = {
             file_type for file_type in SUPPORTED_TYPE_SUFFIXES if file_type in desired_types_processed
         }
 
         return list(allowed_types)
@@ -358,22 +360,19 @@
         desired_file_types: Optional[List[str]] = None,
     ) -> List[Path]:
         all_files = FilesService._get_file_paths(paths, recursive=recursive)
 
         allowed_file_types: List[str] = FilesService._get_allowed_file_types(desired_file_types)
         allowed_meta_types: Tuple = tuple(f"{file_type}.meta.json" for file_type in allowed_file_types)
 
-        meta_file_path = [
-            path for path in all_files if path.is_file() and str(path).lower().endswith(allowed_meta_types)
-        ]
+        meta_file_path = [path for path in all_files if path.is_file() and str(path).endswith(allowed_meta_types)]
         file_paths = [
             path
             for path in all_files
-            if path.is_file()
-            and (path.suffix.lower() in allowed_file_types and not str(path).lower().endswith(".meta.json"))
+            if path.is_file() and (path.suffix in allowed_file_types and not str(path).endswith(META_SUFFIX))
         ]
         combined_paths = meta_file_path + file_paths
 
         combined_paths = FilesService._remove_duplicates(combined_paths)
         if len(combined_paths) < len(all_files):
             logger.warning(
                 "Skipping files with unsupported file format.",
```

### Comparing `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/workflows/async_client/files.py` & `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/workflows/async_client/files.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/workflows/sync_client/files.py` & `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/workflows/sync_client/files.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/workflows/sync_client/utils.py` & `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/workflows/sync_client/utils.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/docs/index.md` & `deepset_cloud_sdk-1.0.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/docs/upload_files.md` & `deepset_cloud_sdk-1.0.1/docs/upload_files.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/docs/_images/favicon.svg` & `deepset_cloud_sdk-1.0.1/docs/_images/favicon.svg`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/docs/_images/white-logo.svg` & `deepset_cloud_sdk-1.0.1/docs/_images/white-logo.svg`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/docs/_pydoc/renderers.py` & `deepset_cloud_sdk-1.0.1/docs/_pydoc/renderers.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/docs/_pydoc/config/async_client.yml` & `deepset_cloud_sdk-1.0.1/docs/_pydoc/config/async_client.yml`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/docs/_pydoc/config/cli.yml` & `deepset_cloud_sdk-1.0.1/docs/_pydoc/config/cli.yml`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/docs/_pydoc/config/sync_client.yml` & `deepset_cloud_sdk-1.0.1/docs/_pydoc/config/sync_client.yml`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/docs/examples/cli/README.md` & `deepset_cloud_sdk-1.0.1/docs/examples/cli/README.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/docs/examples/data/example.pdf` & `deepset_cloud_sdk-1.0.1/docs/examples/data/example.pdf`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/docs/examples/sdk/README.md` & `deepset_cloud_sdk-1.0.1/docs/examples/sdk/README.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/docs/examples/sdk/upload.py` & `deepset_cloud_sdk-1.0.1/docs/examples/sdk/upload.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/.gitignore` & `deepset_cloud_sdk-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/LICENSE` & `deepset_cloud_sdk-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/README.md` & `deepset_cloud_sdk-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/pyproject.toml` & `deepset_cloud_sdk-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.0/PKG-INFO` & `deepset_cloud_sdk-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deepset-cloud-sdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: deepset Cloud SDK
 Project-URL: Documentation, https://github.com/deepset-ai/deepset-cloud-sdk#readme
 Project-URL: Issues, https://github.com/deepset-ai/deepset-cloud-sdk/issues
 Project-URL: Source, https://github.com/deepset-ai/deepset-cloud-sdk
 Author-email: deepset <rohan.janjua@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: deepset-cloud-sdk Version: 1.0.0 Summary: deepset
+Metadata-Version: 2.3 Name: deepset-cloud-sdk Version: 1.0.1 Summary: deepset
 Cloud SDK Project-URL: Documentation, https://github.com/deepset-ai/deepset-
 cloud-sdk#readme Project-URL: Issues, https://github.com/deepset-ai/deepset-
 cloud-sdk/issues Project-URL: Source, https://github.com/deepset-ai/deepset-
 cloud-sdk Author-email: deepset
 deepset.ai> License-Expression: Apache-2.0 License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```


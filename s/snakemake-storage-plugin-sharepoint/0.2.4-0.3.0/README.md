# Comparing `tmp/snakemake_storage_plugin_sharepoint-0.2.4.tar.gz` & `tmp/snakemake_storage_plugin_sharepoint-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_storage_plugin_sharepoint-0.2.4.tar", max compression
+gzip compressed data, was "snakemake_storage_plugin_sharepoint-0.3.0.tar", max compression
```

## Comparing `snakemake_storage_plugin_sharepoint-0.2.4.tar` & `snakemake_storage_plugin_sharepoint-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1058 2024-04-30 20:32:51.687547 snakemake_storage_plugin_sharepoint-0.2.4/LICENSE
--rw-r--r--   0        0        0      119 2024-04-30 20:32:51.687547 snakemake_storage_plugin_sharepoint-0.2.4/README.md
--rw-r--r--   0        0        0      958 2024-04-30 20:32:51.687547 snakemake_storage_plugin_sharepoint-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      322 2024-04-30 20:32:51.687547 snakemake_storage_plugin_sharepoint-0.2.4/snakemake_storage_plugin_sharepoint/__init__.py
--rw-r--r--   0        0        0     6810 2024-04-30 20:32:51.687547 snakemake_storage_plugin_sharepoint-0.2.4/snakemake_storage_plugin_sharepoint/object.py
--rw-r--r--   0        0        0     2561 2024-04-30 20:32:51.687547 snakemake_storage_plugin_sharepoint-0.2.4/snakemake_storage_plugin_sharepoint/provider.py
--rw-r--r--   0        0        0     4367 2024-04-30 20:32:51.687547 snakemake_storage_plugin_sharepoint-0.2.4/snakemake_storage_plugin_sharepoint/settings.py
--rw-r--r--   0        0        0     1087 1970-01-01 00:00:00.000000 snakemake_storage_plugin_sharepoint-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-03 18:54:45.799045 snakemake_storage_plugin_sharepoint-0.3.0/LICENSE
+-rw-r--r--   0        0        0      292 2024-05-03 18:54:45.799045 snakemake_storage_plugin_sharepoint-0.3.0/README.md
+-rw-r--r--   0        0        0      958 2024-05-03 18:54:45.799045 snakemake_storage_plugin_sharepoint-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      322 2024-05-03 18:54:45.799045 snakemake_storage_plugin_sharepoint-0.3.0/snakemake_storage_plugin_sharepoint/__init__.py
+-rw-r--r--   0        0        0     7364 2024-05-03 18:54:45.799045 snakemake_storage_plugin_sharepoint-0.3.0/snakemake_storage_plugin_sharepoint/object.py
+-rw-r--r--   0        0        0     4023 2024-05-03 18:54:45.799045 snakemake_storage_plugin_sharepoint-0.3.0/snakemake_storage_plugin_sharepoint/provider.py
+-rw-r--r--   0        0        0     4190 2024-05-03 18:54:45.799045 snakemake_storage_plugin_sharepoint-0.3.0/snakemake_storage_plugin_sharepoint/settings.py
+-rw-r--r--   0        0        0     1260 1970-01-01 00:00:00.000000 snakemake_storage_plugin_sharepoint-0.3.0/PKG-INFO
```

### Comparing `snakemake_storage_plugin_sharepoint-0.2.4/LICENSE` & `snakemake_storage_plugin_sharepoint-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_storage_plugin_sharepoint-0.2.4/pyproject.toml` & `snakemake_storage_plugin_sharepoint-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakemake-storage-plugin-sharepoint"
-version = "0.2.4"
+version = "0.3.0"
 description = "Snakemake storage plugin for reading and writing files on Microsoft SharePoint."
 authors = [
     "Hugo Lapre <hugo.lapre@brabantwater.nl>",
 ]
 readme = "README.md"
 repository = "https://github.com/Hugovdberg/snakemake-storage-plugin-sharepoint"
 documentation = "https://snakemake.github.io/snakemake-plugin-catalog/plugins/storage/sharepoint.html"
```

### Comparing `snakemake_storage_plugin_sharepoint-0.2.4/snakemake_storage_plugin_sharepoint/object.py` & `snakemake_storage_plugin_sharepoint-0.3.0/snakemake_storage_plugin_sharepoint/object.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from snakemake_interface_common.exceptions import WorkflowError
 from snakemake_interface_common.logging import get_logger
 from snakemake_interface_storage_plugins.io import IOCacheStorageInterface, Mtime
 from snakemake_interface_storage_plugins.storage_object import (
     StorageObjectRead,
     StorageObjectWrite,
 )
+from snakemake_interface_storage_plugins.storage_provider import StorageProviderBase
 
 if TYPE_CHECKING:
     from .provider import StorageProvider
 
 __all__ = ["StorageObject"]
 
 HTTPVerb = Literal["GET", "POST", "HEAD"]
@@ -38,14 +39,41 @@
     UPLOAD_FILE_URL = (
         "{site_url}/_api/web/GetFolderByServerRelativeUrl('{folder}')/"
         "Files/add(url='{filename}',overwrite={overwrite})"
     )
     if TYPE_CHECKING:
         provider: StorageProvider
 
+    def __init__(
+        self,
+        query: str,
+        keep_local: bool,
+        retrieve: bool,
+        provider: StorageProviderBase,
+    ):
+        self.allow_overwrite: bool
+        self.site_url: str
+        self.site_netloc: str
+        self.library: str
+        self.filepath: str
+        super().__init__(query, keep_local, retrieve, provider)
+
+    def __post_init__(self):
+        if (site_url := self.provider.settings.site_url) is None:
+            raise WorkflowError("No site URL specified")
+        parsed_site = urlparse(site_url)
+        self.site_url = site_url.rstrip("/")
+        self.site_netloc = parsed_site.netloc
+
+        parsed_query = urlparse(self.query)
+        self.library = parsed_query.netloc
+        self.filepath = parsed_query.path.lstrip("/")
+
+        self.allow_overwrite = self.provider.settings.allow_overwrite or False
+
     async def inventory(self, cache: IOCacheStorageInterface):
         """From this file, try to find as much existence and modification date
         information as possible. Only retrieve that information that comes for free
         given the current object.
         """
         with self.httpr(self.GET_FILE_URL) as r:
             name = str(self.local_path())
@@ -57,48 +85,39 @@
     def get_inventory_parent(self) -> Optional[str]:
         return None
 
     def cleanup(self):
         pass
 
     def exists(self) -> bool:
-        with self.httpr(self.GET_FILE_URL) as r:
+        with self.httpr(self.GET_FILE_URL, "GET") as r:
             return FileInfo(r).exists()
 
     def mtime(self) -> float:
-        with self.httpr(self.GET_FILE_URL) as r:
+        with self.httpr(self.GET_FILE_URL, "GET") as r:
             return FileInfo(r).last_modified()
 
     def size(self) -> int:
-        with self.httpr(self.GET_FILE_URL) as r:
+        with self.httpr(self.GET_FILE_URL, "GET") as r:
             return FileInfo(r).size()
 
     def retrieve_object(self):
         self.local_path().parent.mkdir(parents=True, exist_ok=True)
         with (
             self.httpr(self.DOWNLOAD_FILE_URL, stream=True) as r,
             self.local_path().open("wb") as fh,
         ):
             for chunk in r.iter_content():
                 fh.write(chunk)
 
-    @property
-    def _full_query(self) -> str:
-        if (site_url := self.provider.settings.site_url) is None:
-            raise WorkflowError("No site URL specified")
-        if (library := self.provider.settings.library) is None:
-            raise WorkflowError("No library specified")
-        return "/".join([site_url, library, self.query])
-
     # The type: ignore is necessary because the return type is not compatible with the
     # base class:
     # https://github.com/snakemake/snakemake-interface-storage-plugins/pull/48
     def local_suffix(self) -> str:  # type: ignore
-        parsed = urlparse(self._full_query)
-        return f"{parsed.netloc}/{parsed.path}"
+        return "/".join([self.site_netloc, self.library, self.filepath])
 
     def store_object(self):
         with self.httpr(self.DIGEST_URL, "POST") as r:
             try:
                 r.raise_for_status()
             except requests.HTTPError as e:
                 raise WorkflowError(
@@ -132,20 +151,20 @@
         **kwargs: Any,
     ) -> Generator[requests.Response, Any, None]:
         _headers = {
             "Content-Type": "application/json; odata=verbose",
             "Accept": "application/json; odata=verbose",
         }
         _url = url.format(
-            site_url=self.provider.settings.site_url,
-            folder=self.provider.settings.library,
-            filename=self.query,
-            overwrite=str(self.provider.settings.allow_overwrite).lower(),
+            site_url=self.site_url,
+            folder=self.library,
+            filename=self.filepath,
+            overwrite=str(self.allow_overwrite).lower(),
         )
-        logger.debug(f"Requesting {verb!r} to {_url}")
+        logger.debug(f"Requesting HTTP {verb!r} {_url}")
         logger.debug(f"Authenticating with {self.provider.settings.auth}")
         if headers is not None:
             _headers.update(headers)
         r = None
         try:
             match verb.upper():
                 case "GET":
```

### Comparing `snakemake_storage_plugin_sharepoint-0.2.4/snakemake_storage_plugin_sharepoint/settings.py` & `snakemake_storage_plugin_sharepoint-0.3.0/snakemake_storage_plugin_sharepoint/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,20 +106,14 @@
     site_url: Optional[str] = dataclasses.field(
         default=None,
         metadata={
             "help": "The URL of the SharePoint site.",
             "env_var": True,
         },
     )
-    library: Optional[str] = dataclasses.field(
-        default=None,
-        metadata={
-            "help": "The folder in the SharePoint site to work with.",
-        },
-    )
     allow_overwrite: bool = dataclasses.field(
         default=False,
         metadata={
             "help": "Allow overwriting files in the SharePoint site.",
         },
     )
     upload_timeout: int = dataclasses.field(
```

### Comparing `snakemake_storage_plugin_sharepoint-0.2.4/PKG-INFO` & `snakemake_storage_plugin_sharepoint-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-storage-plugin-sharepoint
-Version: 0.2.4
+Version: 0.3.0
 Summary: Snakemake storage plugin for reading and writing files on Microsoft SharePoint.
 Home-page: https://github.com/Hugovdberg/snakemake-storage-plugin-sharepoint
 License: MIT
 Keywords: snakemake,plugin,storage,sharepoint
 Author: Hugo Lapre
 Author-email: hugo.lapre@brabantwater.nl
 Requires-Python: >=3.11,<4.0
@@ -16,9 +16,12 @@
 Requires-Dist: snakemake-interface-storage-plugins (>=3.0.0,<4.0.0)
 Project-URL: Documentation, https://snakemake.github.io/snakemake-plugin-catalog/plugins/storage/sharepoint.html
 Project-URL: Repository, https://github.com/Hugovdberg/snakemake-storage-plugin-sharepoint
 Description-Content-Type: text/markdown
 
 # snakemake-storage-plugin-sharepoint
 
-Snakemake storage plugin for reading and writing files on Microsoft SharePoint.
+[Snakemake](https://snakemake.github.io/) storage plugin for reading and writing files
+on Microsoft SharePoint sites.
+Documentation is on the snakemake plugin catalog:
+https://snakemake.github.io/snakemake-plugin-catalog/plugins/storage/sharepoint.html
```


# Comparing `tmp/servicex-3.0.0a8.tar.gz` & `tmp/servicex-3.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicex-3.0.0a8.tar", max compression
+gzip compressed data, was "servicex-3.0.0a9.tar", max compression
```

## Comparing `servicex-3.0.0a8.tar` & `servicex-3.0.0a9.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     1499 2024-01-11 20:52:16.718673 servicex-3.0.0a8/LICENSE
--rw-r--r--   0        0        0     4890 2024-01-11 20:52:16.718673 servicex-3.0.0a8/README.md
--rw-r--r--   0        0        0     1246 2024-01-11 20:53:13.699017 servicex-3.0.0a8/pyproject.toml
--rw-r--r--   0        0        0     2212 2024-01-11 20:52:16.718673 servicex-3.0.0a8/servicex/__init__.py
--rw-r--r--   0        0        0       96 2024-01-11 20:52:16.718673 servicex-3.0.0a8/servicex/_version.py
--rw-r--r--   0        0        0     1535 2024-01-11 20:52:16.718673 servicex-3.0.0a8/servicex/app/__init__.py
--rw-r--r--   0        0        0     3350 2024-01-11 20:52:16.718673 servicex-3.0.0a8/servicex/app/cache.py
--rw-r--r--   0        0        0     1776 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/app/cli_options.py
--rw-r--r--   0        0        0     2489 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/app/codegen.py
--rw-r--r--   0        0        0     2295 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/app/main.py
--rw-r--r--   0        0        0     5420 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/app/transforms.py
--rw-r--r--   0        0        0     5311 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/configuration.py
--rw-r--r--   0        0        0     1602 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/databinder/__init__.py
--rw-r--r--   0        0        0     2113 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/databinder/databinder.py
--rw-r--r--   0        0        0    10671 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/databinder/databinder_configuration.py
--rw-r--r--   0        0        0     3487 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/databinder/databinder_deliver.py
--rw-r--r--   0        0        0     3571 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/databinder/databinder_outputs.py
--rw-r--r--   0        0        0     5585 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/databinder/databinder_requests.py
--rw-r--r--   0        0        0    19978 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/dataset.py
--rw-r--r--   0        0        0     3803 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/dataset_group.py
--rw-r--r--   0        0        0     3403 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/dataset_identifier.py
--rw-r--r--   0        0        0     8271 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/expandable_progress.py
--rw-r--r--   0        0        0     1535 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/func_adl/__init__.py
--rw-r--r--   0        0        0    12499 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/func_adl/func_adl_dataset.py
--rw-r--r--   0        0        0     2438 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/func_adl/func_adl_dataset_group.py
--rw-r--r--   0        0        0     4013 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/func_adl/util.py
--rw-r--r--   0        0        0     4563 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/minio_adapter.py
--rw-r--r--   0        0        0     5232 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/models.py
--rw-r--r--   0        0        0     3344 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/python_dataset.py
--rw-r--r--   0        0        0     5189 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/query_cache.py
--rw-r--r--   0        0        0     5542 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/servicex_adapter.py
--rw-r--r--   0        0        0     8352 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/servicex_client.py
--rw-r--r--   0        0        0     1685 2024-01-11 20:52:16.722673 servicex-3.0.0a8/servicex/types.py
--rw-r--r--   0        0        0     6337 1970-01-01 00:00:00.000000 servicex-3.0.0a8/setup.py
--rw-r--r--   0        0        0     6194 1970-01-01 00:00:00.000000 servicex-3.0.0a8/PKG-INFO
+-rw-r--r--   0        0        0     1499 2024-03-15 14:28:05.978814 servicex-3.0.0a9/LICENSE
+-rw-r--r--   0        0        0     4890 2024-03-15 14:28:05.978814 servicex-3.0.0a9/README.md
+-rw-r--r--   0        0        0     1246 2024-03-15 14:28:57.710561 servicex-3.0.0a9/pyproject.toml
+-rw-r--r--   0        0        0     2420 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/__init__.py
+-rw-r--r--   0        0        0       96 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/_version.py
+-rw-r--r--   0        0        0     1535 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/app/__init__.py
+-rw-r--r--   0        0        0     3350 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/app/cache.py
+-rw-r--r--   0        0        0     1776 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/app/cli_options.py
+-rw-r--r--   0        0        0     2489 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/app/codegen.py
+-rw-r--r--   0        0        0     2295 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/app/main.py
+-rw-r--r--   0        0        0     5420 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/app/transforms.py
+-rw-r--r--   0        0        0     5410 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/configuration.py
+-rw-r--r--   0        0        0     1602 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/databinder/__init__.py
+-rw-r--r--   0        0        0     2113 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/databinder/databinder.py
+-rw-r--r--   0        0        0    10671 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/databinder/databinder_configuration.py
+-rw-r--r--   0        0        0     3487 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/databinder/databinder_deliver.py
+-rw-r--r--   0        0        0     3571 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/databinder/databinder_outputs.py
+-rw-r--r--   0        0        0     5585 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/databinder/databinder_requests.py
+-rw-r--r--   0        0        0     6264 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/databinder_models.py
+-rw-r--r--   0        0        0     3835 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/dataset_group.py
+-rw-r--r--   0        0        0     3403 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/dataset_identifier.py
+-rw-r--r--   0        0        0     8271 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/expandable_progress.py
+-rw-r--r--   0        0        0     1535 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/func_adl/__init__.py
+-rw-r--r--   0        0        0    12484 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/func_adl/func_adl_dataset.py
+-rw-r--r--   0        0        0     2438 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/func_adl/func_adl_dataset_group.py
+-rw-r--r--   0        0        0     4013 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/func_adl/util.py
+-rw-r--r--   0        0        0     4563 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/minio_adapter.py
+-rw-r--r--   0        0        0     5232 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/models.py
+-rw-r--r--   0        0        0     3334 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/python_dataset.py
+-rw-r--r--   0        0        0    19972 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/query.py
+-rw-r--r--   0        0        0     5189 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/query_cache.py
+-rw-r--r--   0        0        0     5542 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/servicex_adapter.py
+-rw-r--r--   0        0        0    10917 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/servicex_client.py
+-rw-r--r--   0        0        0     1685 2024-03-15 14:28:05.982814 servicex-3.0.0a9/servicex/types.py
+-rw-r--r--   0        0        0     6337 1970-01-01 00:00:00.000000 servicex-3.0.0a9/setup.py
+-rw-r--r--   0        0        0     6194 1970-01-01 00:00:00.000000 servicex-3.0.0a9/PKG-INFO
```

### Comparing `servicex-3.0.0a8/LICENSE` & `servicex-3.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/README.md` & `servicex-3.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/pyproject.toml` & `servicex-3.0.0a9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servicex"
-version = "3.0.0-alpha.8"
+version = "3.0.0-alpha.9"
 description = ""
 authors = [
     "Ben Galewsky <bengal1@illinois.edu>",
     "Gordon Watts <gwatts@uw.edu>",
 ]
 readme = "README.md"
 packages = [{ include = "servicex" }]
```

### Comparing `servicex-3.0.0a8/servicex/__init__.py` & `servicex-3.0.0a9/servicex/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,34 +21,39 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-from servicex import dataset
 from servicex import dataset_group
 from servicex import models
 from servicex import servicex_client
 from servicex import dataset_identifier
-
-from .servicex_client import ServiceXClient
-from .dataset import Dataset
+from servicex.databinder_models import Sample, General, Definition, ServiceXSpec
+from servicex.func_adl.func_adl_dataset import FuncADLQuery
+from servicex.servicex_client import ServiceXClient, deliver
+from .query import Query
 from .models import ResultFormat, ResultDestination
 from .dataset_group import DatasetGroup
 from .dataset_identifier import RucioDatasetIdentifier, FileListDataset
 
 
 __all__ = [
     "ServiceXClient",
-    "Dataset",
+    "Query",
     "DatasetGroup",
     "ResultFormat",
     "ResultDestination",
     "servicex_client",
-    "dataset",
     "dataset_group",
     "models",
     "dataset_identifier",
     "RucioDatasetIdentifier",
     "FileListDataset",
+    "FuncADLQuery",
+    "Sample",
+    "General",
+    "Definition",
+    "ServiceXSpec",
+    "deliver"
 ]
```

### Comparing `servicex-3.0.0a8/servicex/app/__init__.py` & `servicex-3.0.0a9/servicex/app/__init__.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/app/cache.py` & `servicex-3.0.0a9/servicex/app/cache.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/app/cli_options.py` & `servicex-3.0.0a9/servicex/app/cli_options.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/app/codegen.py` & `servicex-3.0.0a9/servicex/app/codegen.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/app/main.py` & `servicex-3.0.0a9/servicex/app/main.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/app/transforms.py` & `servicex-3.0.0a9/servicex/app/transforms.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/configuration.py` & `servicex-3.0.0a9/servicex/configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,16 +51,17 @@
     def expand_cache_path(cls, v):
         """
         Expand the cache path to a full path, and create it if it doesn't exist.
         Expand ${USER} to be the user name on the system. Works for windows, too.
         :param v:
         :return:
         """
+        # create a folder inside the tmp directory if not specified in cache_path
         if not v:
-            v = "/tmp"
+            v = "/tmp/servicex_${USER}"
 
         s_path = os.path.expanduser(v)
 
         # If they have tried to use the USER or UserName as an expansion, and it has failed, then
         # translate it to maintain harmony across platforms.
         if "${USER}" in s_path and "UserName" in os.environ:
             s_path = s_path.replace("${USER}", os.environ["UserName"])
```

### Comparing `servicex-3.0.0a8/servicex/databinder/__init__.py` & `servicex-3.0.0a9/servicex/databinder/__init__.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/databinder/databinder.py` & `servicex-3.0.0a9/servicex/databinder/databinder.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/databinder/databinder_configuration.py` & `servicex-3.0.0a9/servicex/databinder/databinder_configuration.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/databinder/databinder_deliver.py` & `servicex-3.0.0a9/servicex/databinder/databinder_deliver.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/databinder/databinder_outputs.py` & `servicex-3.0.0a9/servicex/databinder/databinder_outputs.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/databinder/databinder_requests.py` & `servicex-3.0.0a9/servicex/databinder/databinder_requests.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/dataset.py` & `servicex-3.0.0a9/servicex/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 from servicex.servicex_adapter import ServiceXAdapter
 
 from make_it_sync import make_sync
 
 ProgressIndicators = Union[Progress, ExpandableProgress]
 
 
-class Dataset(ABC):
+class Query(ABC):
     def __init__(
         self,
         dataset_identifier: DID,
         title: str,
         codegen: str,
         sx_adapter: ServiceXAdapter,
         config: Configuration,
@@ -91,15 +91,15 @@
         :param servicex_polling_interval: How many seconds between polling for
                                           transform status?
         :param minio_polling_interval:  How many seconds between polling the minio bucket
                                         for new files?
         :param result_format:
         :param ignore_cache:  If true, ignore the cache and always submit a new transform
         """
-        super(Dataset, self).__init__()
+        super(Query, self).__init__()
         self.servicex = sx_adapter
         self.configuration = config
         self.cache = query_cache
 
         self.dataset_identifier = dataset_identifier
         self.codegen = codegen
         self.title = title
@@ -138,15 +138,15 @@
             result_format=self.result_format,  # type: ignore
             selection=self.generate_selection_string(),
         )  # type: ignore
         # Transfer the DID into the transform request
         self.dataset_identifier.populate_transform_request(sx_request)
         return sx_request
 
-    def set_title(self, title: str) -> Dataset:
+    def set_title(self, title: str) -> Query:
         self.title = title
         return self
 
     def set_result_format(self, result_format: ResultFormat):
         r"""
         Set the result format - required at constructor time or as part of the query
         chain of methods
```

### Comparing `servicex-3.0.0a8/servicex/dataset_group.py` & `servicex-3.0.0a9/servicex/dataset_group.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,22 +26,22 @@
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 import asyncio
 from typing import List, Optional, Union
 
 from rich.progress import Progress
 
-from servicex.dataset import Dataset
+from servicex.query import Query
 from servicex.expandable_progress import ExpandableProgress
-from servicex.func_adl.func_adl_dataset import FuncADLDataset
+from servicex.func_adl.func_adl_dataset import FuncADLQuery
 from servicex.models import TransformedResults, ResultFormat
 from make_it_sync import make_sync
 
 
-DatasetGroupMember = Union[Dataset, FuncADLDataset]
+DatasetGroupMember = Union[Query, FuncADLQuery]
 
 
 class DatasetGroup:
     def __init__(self, datasets: List[DatasetGroupMember]):
         r"""
         A group of datasets that are to be transformed together. This is a convenience
         class to allow you to submit multiple datasets to a ServiceX instance and
@@ -83,7 +83,9 @@
                              ) -> List[TransformedResults]:
         with ExpandableProgress(display_progress, provided_progress) as progress:
             self.tasks = [
                 d.as_files_async(provided_progress=progress)
                 for d in self.datasets
             ]
             return await asyncio.gather(*self.tasks)
+
+    as_files = make_sync(as_files_async)
```

### Comparing `servicex-3.0.0a8/servicex/dataset_identifier.py` & `servicex-3.0.0a9/servicex/dataset_identifier.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/expandable_progress.py` & `servicex-3.0.0a9/servicex/expandable_progress.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/func_adl/__init__.py` & `servicex-3.0.0a9/servicex/func_adl/__init__.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/func_adl/func_adl_dataset.py` & `servicex-3.0.0a9/servicex/func_adl/func_adl_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,25 +42,25 @@
     Dict,
 )
 from qastle import python_ast_to_text_ast
 
 from func_adl import EventDataset, find_EventDataset
 from func_adl.object_stream import S
 from servicex.configuration import Configuration
-from servicex.dataset import Dataset
+from servicex.query import Query
 from servicex.func_adl.util import has_tuple
 from servicex.models import ResultFormat
 from servicex.query_cache import QueryCache
 from servicex.servicex_adapter import ServiceXAdapter
 from servicex.types import DID
 
 T = TypeVar("T")
 
 
-class FuncADLDataset(Dataset, EventDataset[T]):
+class FuncADLQuery(Query, EventDataset[T]):
     r"""
     ServiceX Dataset class that uses func_adl query syntax.
     """
     # These are methods that are translated locally
     _execute_locally = ["ResultPandasDF", "ResultAwkwardArray"]
 
     async def execute_result_async(
@@ -69,25 +69,25 @@
         pass
 
     def check_data_format_request(self, f_name: str):
         pass
 
     def __init__(
         self,
-        dataset_identifier: DID,
+        dataset_identifier: DID = None,
         sx_adapter: ServiceXAdapter = None,
         title: str = "ServiceX Client",
         codegen: str = None,
         config: Configuration = None,
         query_cache: QueryCache = None,
         result_format: Optional[ResultFormat] = None,
         item_type: Type = Any,
         ignore_cache: bool = False,
     ):
-        Dataset.__init__(
+        Query.__init__(
             self,
             dataset_identifier=dataset_identifier,
             title=title,
             codegen=codegen,
             sx_adapter=sx_adapter,
             config=config,
             query_cache=query_cache,
@@ -118,15 +118,15 @@
             else:
                 setattr(obj, attr, copy.deepcopy(value, memo))
 
         return obj
 
     def SelectMany(
         self, func: Union[str, ast.Lambda, Callable[[T], Iterable[S]]]
-    ) -> FuncADLDataset[S]:
+    ) -> FuncADLQuery[S]:
         r"""
         Given the current stream's object type is an array or other iterable, return
         the items in this objects type, one-by-one. This has the effect of flattening a
         nested array.
 
         Arguments:
 
@@ -138,15 +138,15 @@
 
         Notes:
             - The function can be a `lambda`, the name of a one-line function, a string that
               contains a lambda definition, or a python `ast` of type `ast.Lambda`.
         """
         return super().SelectMany(func)
 
-    def Select(self, f: Union[str, ast.Lambda, Callable[[T], S]]) -> FuncADLDataset[S]:
+    def Select(self, f: Union[str, ast.Lambda, Callable[[T], S]]) -> FuncADLQuery[S]:
         r"""
         Apply a transformation function to each object in the stream, yielding a new type of
         object. There is a one-to-one correspondence between the input objects and output objects.
 
         Arguments:
             f:      selection function (lambda)
 
@@ -164,15 +164,15 @@
         if self.provided_qastle:
             return self.provided_qastle
         else:
             return self.generate_qastle(self.query_ast)
 
     def Where(
         self, filter: Union[str, ast.Lambda, Callable[[T], bool]]
-    ) -> FuncADLDataset[T]:
+    ) -> FuncADLQuery[T]:
         r"""
         Filter the object stream, allowing only items for which `filter` evaluates as true through.
 
         Arguments:
 
             filter      A filter lambda that returns True/False.
 
@@ -183,25 +183,25 @@
         Notes:
             - The function can be a `lambda`, the name of a one-line function, a string that
               contains a lambda definition, or a python `ast` of type `ast.Lambda`.
         """
 
         return super().Where(filter)
 
-    def MetaData(self, metadata: Dict[str, Any]) -> FuncADLDataset[T]:
+    def MetaData(self, metadata: Dict[str, Any]) -> FuncADLQuery[T]:
         r"""Add metadata to the current object stream. The metadata is an arbitrary set of string
         key-value pairs. The backend must be able to properly interpret the metadata.
 
         Returns:
             The Dataset with the MetaData operator applied
         """
 
         return super().MetaData(metadata)
 
-    def QMetaData(self, metadata: Dict[str, Any]) -> FuncADLDataset[T]:
+    def QMetaData(self, metadata: Dict[str, Any]) -> FuncADLQuery[T]:
         r"""Add query metadata to the current object stream.
 
         - Metadata is never transmitted to any back end
         - Metadata is per-query, not per sample.
 
         Warnings are issued if metadata is overwriting metadata.
 
@@ -209,15 +209,15 @@
             metadata (Dict[str, Any]): Metadata to be used later
 
         Returns:
             The Dataset with the QMetaData operator applied
         """
         return super().QMetaData(metadata)
 
-    def set_tree(self, tree_name: str) -> FuncADLDataset[T]:
+    def set_tree(self, tree_name: str) -> FuncADLQuery[T]:
         r"""Set the tree name for the query.
         Args:
             tree_name (str): Name of the tree to use for the query
 
         Returns:
             The Dataset with the tree appended to the first call object
         """
```

### Comparing `servicex-3.0.0a8/servicex/func_adl/func_adl_dataset_group.py` & `servicex-3.0.0a9/servicex/func_adl/func_adl_dataset_group.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/func_adl/util.py` & `servicex-3.0.0a9/servicex/func_adl/util.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/minio_adapter.py` & `servicex-3.0.0a9/servicex/minio_adapter.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/models.py` & `servicex-3.0.0a9/servicex/models.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/python_dataset.py` & `servicex-3.0.0a9/servicex/python_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,22 +26,22 @@
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 import inspect
 import typing
 from base64 import b64encode
 
 from servicex.configuration import Configuration
-from servicex.dataset import Dataset
+from servicex.query import Query
 from servicex.models import ResultFormat
 from servicex.query_cache import QueryCache
 from servicex.servicex_adapter import ServiceXAdapter
 from servicex.types import DID
 
 
-class PythonDataset(Dataset):
+class PythonQuery(Query):
 
     def __init__(self, dataset_identifier: DID,
                  sx_adapter: ServiceXAdapter = None,
                  title: str = "ServiceX Client",
                  codegen: str = None,
                  config: Configuration = None,
                  query_cache: QueryCache = None,
@@ -55,15 +55,15 @@
                          config=config,
                          query_cache=query_cache,
                          result_format=result_format,
                          ignore_cache=ignore_cache)
 
         self.python_function = None
 
-    def with_uproot_function(self, f: typing.Union[str, typing.Callable]) -> Dataset:
+    def with_uproot_function(self, f: typing.Union[str, typing.Callable]) -> Query:
         self.python_function = f
         return self
 
     def generate_selection_string(self) -> str:
         if not self.python_function:
             raise ValueError("You must provide a python function using with_uproot_function")
```

### Comparing `servicex-3.0.0a8/servicex/query_cache.py` & `servicex-3.0.0a9/servicex/query_cache.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/servicex_adapter.py` & `servicex-3.0.0a9/servicex/servicex_adapter.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/servicex/types.py` & `servicex-3.0.0a9/servicex/types.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a8/setup.py` & `servicex-3.0.0a9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             'fastparquet>=2023.4.0,<2024.0.0']}
 
 entry_points = \
 {'console_scripts': ['servicex = servicex.app.main:app']}
 
 setup_kwargs = {
     'name': 'servicex',
-    'version': '3.0.0a8',
+    'version': '3.0.0a9',
     'description': '',
     'long_description': "# servicex_client\nPython SDK and CLI Client for ServiceX\n\n## Configuration\nThe client relies on a YAML file to obtain the URLs of different servicex\ndeployments, as well as tokens to authenticate with the service. The file \nshould be named `.servicex` and the format of this file is as follows:\n```yaml\napi_endpoints:\n  - endpoint: http://localhost:5000\n    name: localhost\n\n  - endpoint: https://servicex-release-testing-4.servicex.ssl-hep.org\n    name: testing4\n    token: ...\n\ndefault_endpoint: testing4\n\ncache_path: /tmp/ServiceX_Client/cache-dir\nshortened_downloaded_filename: true\n\n```\nThe `default_endpoint` will be used if otherwise not specified. The cache \ndatabase and downloaded files will be stored in the directory specified by \n`cache_path`.\n\nThe `shortened_downloaded_filename` property controls whether downloaded files\nwill have their names shortened for convenience. Setting to false preserves\nthe full filename from the dataset.\n`\n\nThe library will search for this file in the current working directory and then\nstart looking in parent directories until a file is found.\n\n## Command Line Interface\nWhen installed, the client provides a new command in your shell, `servicex`.\nThis command uses a series of subcommands to work with various functions of\nserviceX.\n\nCommon command line arguments:\n\n| Flag | Long Flag | What it does                                         |\n|------|-----------|------------------------------------------------------|\n| -u   | --url     | The url of the serviceX ingress                      |\n| -b   | --backend | Named backend from the .servicex file endpoints list |\n\nIf neither url nor backend are specified then the client will attempt to use the\n`default_endpoint` value to determine who to talk to.\n\n### codegens \nThis command will list the code generators deployed.\n\n### transforms\nThese commands interact with transforms that have been run\n\n#### list\nList transforms associated with the current user. Add the `--complete` flag to\nonly show transforms that have completed.\n\n#### files\nList the files along with their size generated by a transform. Specify the \ntransform request id with the `-t` or `--transform-id` flag\n\n#### download\nDownload the files from a transform to a local directory. Specify the transform\nrequest id with `-t` and the directory to download to with `-d`. Defaults to\ndownloading files to the current working directory.\n\n### cache\nThese commands allow you to work with the query cache maintained by the serviceX\nclient.\n\n#### list\nShow all of the cached transforms along with the run time, code generator, and \nnumber of resulting files\n\n#### delete\nDelete a specific transform from the cache. Provide the transform request ID \nwith the `-t` or `--transform-id` arg.\n\n#### clear\nClear all of the transforms from the cache. Add `-y` to force the operation \nwithout confirming with the console.\n\n## Python SDK\nEntry to the SDK starts with constructing an instance of ServiceXClient.  The \nconstructor accepts `backend` argument to specify a named backend from the\n`.servicex` file, or `url` for the direct URL to a serviceX server. With the \nURL option you can't provide a token from `.servicex` so it must either be an\nunsecured endpoint, or the token must be provided via the WLCG standard of a \nfile pointed to by `BEARER_TOKEN_FILE` environment variable.\n\nWith an instance of ServiceXClient you can \n- List the code generators deployed with the ServiceX instance\n- List the transformers that have been run\n- Get the current status of a specific transform\n\n### Create a Dataset Instance to Run Transforms\nThe ServiceX client also can create a `Dataset` instance that \nallows you to specify a query, provide a dataset identifier,\nand retrieve the results of the resulting transform request.\n\nThere are two types of datasets\n- func_adl_dataset\n- Python Function dataset\n\n### Dataset Identifiers\nBefore we get too deeply into the dataset classes, we should look\nat how to specify a dataset.\n- RucioDatasetIdentifier - for retrieving data files registered with Rucio\n- FileListDataset - A list of URIs for accessing files using xRootd\n\n### FuncADL Dataset\nThis dataset is controlled by the func_adl language. The dataset\nsupports the `Select`, `SelectMany`, `Where`, `MetaData`, and `QMetaData` \noperators from func_adl.\n\n\n### Datasets\nThis is the abstract class for requesting data from ServiceX. You have to \nspecify the dataset identifier you want data from and provide some sort of \nselection query. You can set the result format with the `set_result_format` \noperator (it's also a factory method arg for the dataset).\n\nOperators that cause the client to interact with the server: These terminal \noperators will call out to the serviceX server and process results. They\nare all implemented as asynchronous coroutines, but they also come with \nsynchronous versions to make it easy to do easy things.\n\n\n#### \n\n",
     'author': 'Ben Galewsky',
     'author_email': 'bengal1@illinois.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `servicex-3.0.0a8/PKG-INFO` & `servicex-3.0.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicex
-Version: 3.0.0a8
+Version: 3.0.0a9
 Summary: 
 Author: Ben Galewsky
 Author-email: bengal1@illinois.edu
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


# Comparing `tmp/model_registry-0.1.2.tar.gz` & `tmp/model_registry-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_registry-0.1.2.tar", max compression
+gzip compressed data, was "model_registry-0.2.0a1.tar", max compression
```

## Comparing `model_registry-0.1.2.tar` & `model_registry-0.2.0a1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     3347 2024-03-05 09:53:27.492853 model_registry-0.1.2/README.md
--rw-r--r--   0        0        0     2247 2024-03-05 09:53:27.496853 model_registry-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      142 2024-03-05 09:53:27.496853 model_registry-0.1.2/src/model_registry/__init__.py
--rw-r--r--   0        0        0     9447 2024-03-05 09:53:27.496853 model_registry-0.1.2/src/model_registry/_client.py
--rw-r--r--   0        0        0    12269 2024-03-05 09:53:27.496853 model_registry-0.1.2/src/model_registry/core.py
--rw-r--r--   0        0        0      535 2024-03-05 09:53:27.496853 model_registry-0.1.2/src/model_registry/exceptions.py
--rw-r--r--   0        0        0      178 2024-03-05 09:53:27.496853 model_registry-0.1.2/src/model_registry/store/__init__.py
--rw-r--r--   0        0        0      347 2024-03-05 09:53:27.496853 model_registry-0.1.2/src/model_registry/store/base.py
--rw-r--r--   0        0        0    11047 2024-03-05 09:53:27.496853 model_registry-0.1.2/src/model_registry/store/wrapper.py
--rw-r--r--   0        0        0      503 2024-03-05 09:53:27.496853 model_registry-0.1.2/src/model_registry/types/__init__.py
--rw-r--r--   0        0        0     4386 2024-03-05 09:53:27.496853 model_registry-0.1.2/src/model_registry/types/artifacts.py
--rw-r--r--   0        0        0     5831 2024-03-05 09:53:27.496853 model_registry-0.1.2/src/model_registry/types/base.py
--rw-r--r--   0        0        0     4302 2024-03-05 09:53:27.496853 model_registry-0.1.2/src/model_registry/types/contexts.py
--rw-r--r--   0        0        0     1266 2024-03-05 09:53:27.496853 model_registry-0.1.2/src/model_registry/types/options.py
--rw-r--r--   0        0        0     4156 1970-01-01 00:00:00.000000 model_registry-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3938 2024-05-03 07:28:51.288530 model_registry-0.2.0a1/README.md
+-rw-r--r--   0        0        0     2249 2024-05-03 07:28:51.288530 model_registry-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0      142 2024-05-03 07:28:51.288530 model_registry-0.2.0a1/src/model_registry/__init__.py
+-rw-r--r--   0        0        0     9350 2024-05-03 07:28:51.288530 model_registry-0.2.0a1/src/model_registry/_client.py
+-rw-r--r--   0        0        0     3540 2024-05-03 07:28:51.288530 model_registry-0.2.0a1/src/model_registry/_utils.py
+-rw-r--r--   0        0        0    12220 2024-05-03 07:28:51.288530 model_registry-0.2.0a1/src/model_registry/core.py
+-rw-r--r--   0        0        0      624 2024-05-03 07:28:51.288530 model_registry-0.2.0a1/src/model_registry/exceptions.py
+-rw-r--r--   0        0        0      178 2024-05-03 07:28:51.292530 model_registry-0.2.0a1/src/model_registry/store/__init__.py
+-rw-r--r--   0        0        0      347 2024-05-03 07:28:51.292530 model_registry-0.2.0a1/src/model_registry/store/base.py
+-rw-r--r--   0        0        0    11616 2024-05-03 07:28:51.292530 model_registry-0.2.0a1/src/model_registry/store/wrapper.py
+-rw-r--r--   0        0        0      503 2024-05-03 07:28:51.292530 model_registry-0.2.0a1/src/model_registry/types/__init__.py
+-rw-r--r--   0        0        0     4386 2024-05-03 07:28:51.292530 model_registry-0.2.0a1/src/model_registry/types/artifacts.py
+-rw-r--r--   0        0        0     5831 2024-05-03 07:28:51.292530 model_registry-0.2.0a1/src/model_registry/types/base.py
+-rw-r--r--   0        0        0     4302 2024-05-03 07:28:51.292530 model_registry-0.2.0a1/src/model_registry/types/contexts.py
+-rw-r--r--   0        0        0     1266 2024-05-03 07:28:51.292530 model_registry-0.2.0a1/src/model_registry/types/options.py
+-rw-r--r--   0        0        0     2405 2024-05-03 07:28:51.292530 model_registry-0.2.0a1/src/model_registry/utils.py
+-rw-r--r--   0        0        0     4749 1970-01-01 00:00:00.000000 model_registry-0.2.0a1/PKG-INFO
```

### Comparing `model_registry-0.1.2/README.md` & `model_registry-0.2.0a1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: model-registry
+Version: 0.2.0a1
+Summary: Client for Kubeflow Model Registry
+Home-page: https://github.com/kubeflow/model-registry
+License: Apache-2.0
+Author: Isabella Basso do Amaral
+Author-email: idoamara@redhat.com
+Requires-Python: >=3.9,<3.11
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Provides-Extra: hf
+Requires-Dist: attrs (>=21.0,<22.0)
+Requires-Dist: huggingface-hub (>=0.20.1,<0.21.0) ; extra == "hf"
+Requires-Dist: ml-metadata (>=1.14.0,<2.0.0)
+Requires-Dist: typing-extensions (>=4.8,<5.0)
+Project-URL: Issues, https://github.com/kubeflow/model-registry/issues
+Description-Content-Type: text/markdown
+
 # Model Registry Python Client
 
 [![Python](https://img.shields.io/badge/python%20-3.9%7C3.10-blue)](https://github.com/kubeflow/model-registry)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](../../../LICENSE)
 
 This library provides a high level interface for interacting with a model registry server.
 
@@ -10,20 +31,20 @@
 ```py
 from model_registry import ModelRegistry
 
 registry = ModelRegistry(server_address="server-address", port=9090, author="author")
 
 model = registry.register_model(
     "my-model",  # model name
-    "s3://path/to/model",  # model URI
+    "https://storage-place.my-company.com",  # model URI
     version="2.0.0",
     description="lorem ipsum",
     model_format_name="onnx",
     model_format_version="1",
-    storage_key="aws-connection-path",
+    storage_key="my-data-connection",
     storage_path="path/to/model",
     metadata={
         # can be one of the following types
         "int_key": 1,
         "bool_key": False,
         "float_key": 3.14,
         "str_key": "str_value",
@@ -33,18 +54,41 @@
 model = registry.get_registered_model("my-model")
 
 version = registry.get_model_version("my-model", "v2.0")
 
 experiment = registry.get_model_artifact("my-model", "v2.0")
 ```
 
-### Default values for metadata
+### Importing from S3
+
+When registering models stored on S3-compatible object storage, you should use `utils.s3_uri_from` to build an
+unambiguous URI for your artifact.
+
+```py
+from model_registry import ModelRegistry, utils
+
+registry = ModelRegistry(server_address="server-address", port=9090, author="author")
 
-If not supplied, `metadata` values defaults to a predefined set of conventional values.
-Reference the technical documentation in the pydoc of the client.
+model = registry.register_model(
+    "my-model",  # model name
+    uri=utils.s3_uri_from("path/to/model", "my-bucket"),
+    version="2.0.0",
+    description="lorem ipsum",
+    model_format_name="onnx",
+    model_format_version="1",
+    storage_key="my-data-connection",
+    metadata={
+        # can be one of the following types
+        "int_key": 1,
+        "bool_key": False,
+        "float_key": 3.14,
+        "str_key": "str_value",
+    }
+)
+```
 
 ### Importing from Hugging Face Hub
 
 To import models from Hugging Face Hub, start by installing the `huggingface-hub` package, either directly or as an
 extra (available as `model-registry[hf]`).
 Models can be imported with
 
@@ -96,7 +140,8 @@
 
 ```sh
 poetry install
 poetry run pytest -v
 ```
 
 <!-- github-only -->
+
```

### Comparing `model_registry-0.1.2/pyproject.toml` & `model_registry-0.2.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "model-registry"
-version = "0.1.2"
+version = "0.2.0a1"
 description = "Client for Kubeflow Model Registry"
 authors = ["Isabella Basso do Amaral <idoamara@redhat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/kubeflow/model-registry"
 
 [tool.poetry.urls]
```

### Comparing `model_registry-0.1.2/src/model_registry/_client.py` & `model_registry-0.2.0a1/src/model_registry/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Standard client for the model registry."""
+
 from __future__ import annotations
 
-import os
 from typing import get_args
 from warnings import warn
 
 from .core import ModelRegistryAPIClient
 from .exceptions import StoreException
 from .store import ScalarType
 from .types import ModelArtifact, ModelVersion, RegisteredModel
@@ -71,24 +71,30 @@
         self,
         name: str,
         uri: str,
         *,
         model_format_name: str,
         model_format_version: str,
         version: str,
-        author: str | None = None,
-        description: str | None = None,
         storage_key: str | None = None,
         storage_path: str | None = None,
         service_account_name: str | None = None,
+        author: str | None = None,
+        description: str | None = None,
         metadata: dict[str, ScalarType] | None = None,
     ) -> RegisteredModel:
         """Register a model.
 
-        Either `storage_key` and `storage_path`, or `service_account_name` must be provided.
+        This registers a model in the model registry. The model is not downloaded, and has to be stored prior to
+        registration.
+
+        Most models can be registered using their URI, along with optional connection-specific parameters, `storage_key`
+        and `storage_path` or, simply a `service_account_name`.
+        URI builder utilities are recommended when referring to specialized storage; for example `utils.s3_uri_from`
+        helper when using S3 object storage data connections.
 
         Args:
             name: Name of the model.
             uri: URI of the model.
 
         Keyword Args:
             version: Version of the model. Has to be unique.
@@ -106,41 +112,28 @@
         """
         rm = self._register_model(name)
         mv = self._register_new_version(
             rm,
             version,
             author or self._author,
             description=description,
-            metadata=metadata or self.default_metadata(),
+            metadata=metadata or {},
         )
         self._register_model_artifact(
             mv,
             uri,
             model_format_name=model_format_name,
             model_format_version=model_format_version,
             storage_key=storage_key,
             storage_path=storage_path,
             service_account_name=service_account_name,
         )
 
         return rm
 
-    def default_metadata(self) -> dict[str, ScalarType]:
-        """Default metadata valorisations.
-
-        When not explicitly supplied by the end users, these valorisations will be used
-        by default.
-
-        Returns:
-            default metadata valorisations.
-        """
-        return {
-            key: os.environ[key] for key in ["AWS_S3_ENDPOINT", "AWS_S3_BUCKET", "AWS_DEFAULT_REGION"] if key in os.environ
-        }
-
     def register_hf_model(
         self,
         repo: str,
         path: str,
         *,
         version: str,
         model_format_name: str,
@@ -198,15 +191,14 @@
                 )
             else:
                 model_author = model_info.author
         else:
             model_author = author
         source_uri = hf_hub_url(repo, path, revision=git_ref)
         metadata = {
-            **self.default_metadata(),
             "repo": repo,
             "source_uri": source_uri,
             "model_origin": "huggingface_hub",
             "model_author": model_author,
         }
         # card_data is the new field, but let's use the old one for backwards compatibility.
         if card_data := model_info.cardData:
```

### Comparing `model_registry-0.1.2/src/model_registry/core.py` & `model_registry-0.2.0a1/src/model_registry/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Client for the model registry."""
-from __future__ import annotations
 
-from collections.abc import Sequence
+from __future__ import annotations
 
 from ml_metadata.proto import MetadataStoreClientConfig
 
 from .exceptions import StoreException
 from .store import MLMDStore, ProtoType
 from .types import ListOptions, ModelArtifact, ModelVersion, RegisteredModel
 from .types.base import ProtoBase
@@ -126,15 +125,15 @@
         if proto_rm is not None:
             return RegisteredModel.unmap(proto_rm)
 
         return None
 
     def get_registered_models(
         self, options: ListOptions | None = None
-    ) -> Sequence[RegisteredModel]:
+    ) -> list[RegisteredModel]:
         """Fetch registered models.
 
         Args:
             options: Options for listing registered models.
 
         Returns:
             Registered models.
@@ -190,15 +189,15 @@
         if proto_mv is not None:
             return ModelVersion.unmap(proto_mv)
 
         return None
 
     def get_model_versions(
         self, registered_model_id: str, options: ListOptions | None = None
-    ) -> Sequence[ModelVersion]:
+    ) -> list[ModelVersion]:
         """Fetch model versions by registered model ID.
 
         Args:
             registered_model_id: Registered model ID.
             options: Options for listing model versions.
 
         Returns:
@@ -340,15 +339,15 @@
 
         return None
 
     def get_model_artifacts(
         self,
         model_version_id: str | None = None,
         options: ListOptions | None = None,
-    ) -> Sequence[ModelArtifact]:
+    ) -> list[ModelArtifact]:
         """Fetches model artifacts.
 
         Args:
             model_version_id: ID of the associated model version.
             options: Options for listing model artifacts.
 
         Returns:
```

### Comparing `model_registry-0.1.2/src/model_registry/exceptions.py` & `model_registry-0.2.0a1/src/model_registry/exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """Exceptions for the model registry."""
 
 
 class StoreException(Exception):
     """Storage related error."""
 
 
+class MissingMetadata(Exception):
+    """Not enough metadata to complete operation."""
+
+
 class UnsupportedTypeException(StoreException):
     """Raised when an unsupported type is encountered."""
 
 
 class TypeNotFoundException(StoreException):
     """Raised when a type cannot be found."""
```

### Comparing `model_registry-0.1.2/src/model_registry/store/wrapper.py` & `model_registry-0.2.0a1/src/model_registry/store/wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,15 +120,15 @@
             raise StoreException(msg) from e
         except errors.NotFoundError as e:
             msg = f"Context type {context.type} does not exist"
             raise TypeNotFoundException(msg) from e
 
     def _filter_type(
         self, type_name: str, protos: Sequence[ProtoType]
-    ) -> Sequence[ProtoType]:
+    ) -> list[ProtoType]:
         return [proto for proto in protos if proto.type == type_name]
 
     def get_context(
         self,
         ctx_type_name: str,
         id: int | None = None,
         name: str | None = None,
@@ -164,25 +164,28 @@
 
         contexts = self._filter_type(ctx_type_name, contexts)
         if contexts:
             return contexts[0]
 
         return None
 
-    def get_contexts(
-        self, ctx_type_name: str, options: ListOptions
-    ) -> Sequence[Context]:
+    def get_contexts(self, ctx_type_name: str, options: ListOptions) -> list[Context]:
         """Get contexts from the store.
 
         Args:
             ctx_type_name: Name of the context type.
             options: List options.
 
         Returns:
             Contexts.
+
+        Raises:
+            TypeNotFoundException: If the type doesn't exist.
+            ServerException: If there was an error getting the type.
+            StoreException: Invalid arguments.
         """
         # TODO: should we make options optional?
         # if options is not None:
         try:
             contexts = self._mlmd_store.get_contexts(options)
         except errors.InvalidArgumentError as e:
             msg = f"Invalid arguments for get_contexts: {e}"
@@ -191,17 +194,19 @@
             msg = "Couldn't get contexts from MLMD store"
             raise ServerException(msg) from e
 
         contexts = self._filter_type(ctx_type_name, contexts)
         # else:
         #     contexts = self._mlmd_store.get_contexts_by_type(ctx_type_name)
 
-        if not contexts:
+        if not contexts and ctx_type_name not in [
+            t.name for t in self._mlmd_store.get_context_types()
+        ]:
             msg = f"Context type {ctx_type_name} does not exist"
-            raise StoreException(msg)
+            raise TypeNotFoundException(msg)
 
         return contexts
 
     def put_context_parent(self, parent_id: int, child_id: int):
         """Put a parent-child relationship between two contexts.
 
         Args:
@@ -305,34 +310,39 @@
             raise ServerException(msg) from e
         artifacts = self._filter_type(art_type_name, artifacts)
         if artifacts:
             return artifacts[0]
 
         return None
 
-    def get_artifacts(
-        self, art_type_name: str, options: ListOptions
-    ) -> Sequence[Artifact]:
+    def get_artifacts(self, art_type_name: str, options: ListOptions) -> list[Artifact]:
         """Get artifacts from the store.
 
         Args:
             art_type_name: Name of the artifact type.
             options: List options.
 
         Returns:
             Artifacts.
+
+        Raises:
+            TypeNotFoundException: If the type doesn't exist.
+            ServerException: If there was an error getting the type.
+            StoreException: Invalid arguments.
         """
         try:
             artifacts = self._mlmd_store.get_artifacts(options)
         except errors.InvalidArgumentError as e:
             msg = f"Invalid arguments for get_artifacts: {e}"
             raise StoreException(msg) from e
         except errors.InternalError as e:
             msg = "Couldn't get artifacts from MLMD store"
             raise ServerException(msg) from e
 
         artifacts = self._filter_type(art_type_name, artifacts)
-        if not artifacts:
+        if not artifacts and art_type_name not in [
+            t.name for t in self._mlmd_store.get_artifact_types()
+        ]:
             msg = f"Artifact type {art_type_name} does not exist"
-            raise StoreException(msg)
+            raise TypeNotFoundException(msg)
 
         return artifacts
```

### Comparing `model_registry-0.1.2/src/model_registry/types/artifacts.py` & `model_registry-0.2.0a1/src/model_registry/types/artifacts.py`

 * *Files identical despite different names*

### Comparing `model_registry-0.1.2/src/model_registry/types/base.py` & `model_registry-0.2.0a1/src/model_registry/types/base.py`

 * *Files identical despite different names*

### Comparing `model_registry-0.1.2/src/model_registry/types/contexts.py` & `model_registry-0.2.0a1/src/model_registry/types/contexts.py`

 * *Files identical despite different names*

### Comparing `model_registry-0.1.2/src/model_registry/types/options.py` & `model_registry-0.2.0a1/src/model_registry/types/options.py`

 * *Files identical despite different names*


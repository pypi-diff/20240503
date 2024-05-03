# Comparing `tmp/garden_ai-1.0.9.tar.gz` & `tmp/garden_ai-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garden_ai-1.0.9.tar", max compression
+gzip compressed data, was "garden_ai-2.0.0.tar", max compression
```

## Comparing `garden_ai-1.0.9.tar` & `garden_ai-2.0.0.tar`

### file list

```diff
@@ -1,63 +1,44 @@
--rw-r--r--   0        0        0     1078 2024-03-26 16:19:12.307627 garden_ai-1.0.9/LICENSE
--rw-r--r--   0        0        0      797 2024-03-26 16:19:12.307627 garden_ai-1.0.9/README.md
--rw-r--r--   0        0        0      531 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/__init__.py
--rw-r--r--   0        0        0       54 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/__main__.py
--rw-r--r--   0        0        0      180 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/_version.py
--rw-r--r--   0        0        0        0 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/app/__init__.py
--rw-r--r--   0        0        0      905 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/app/completion.py
--rw-r--r--   0        0        0     2501 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/app/console.py
--rw-r--r--   0        0        0     2840 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/app/docker.py
--rw-r--r--   0        0        0     7963 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/app/entrypoint.py
--rw-r--r--   0        0        0    16506 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/app/garden.py
--rw-r--r--   0        0        0     1936 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/app/main.py
--rw-r--r--   0        0        0    23044 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/app/notebook.py
--rw-r--r--   0        0        0     3280 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/backend_client.py
--rw-r--r--   0        0        0      655 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/base_image_dockerfiles/Dockerfile_jupyter_3.10
--rw-r--r--   0        0        0      655 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/base_image_dockerfiles/Dockerfile_jupyter_3.11
--rw-r--r--   0        0        0      653 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/base_image_dockerfiles/Dockerfile_jupyter_3.8
--rw-r--r--   0        0        0      653 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/base_image_dockerfiles/Dockerfile_jupyter_3.9
--rw-r--r--   0        0        0     2120 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/base_image_dockerfiles/Dockerfile_jupyter_all_3.10
--rw-r--r--   0        0        0     1966 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/base_image_dockerfiles/Dockerfile_jupyter_all_3.8
--rw-r--r--   0        0        0      812 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/base_image_dockerfiles/Dockerfile_jupyter_sklearn_3.10
--rw-r--r--   0        0        0      812 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/base_image_dockerfiles/Dockerfile_jupyter_sklearn_3.11
--rw-r--r--   0        0        0      810 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/base_image_dockerfiles/Dockerfile_jupyter_sklearn_3.8
--rw-r--r--   0        0        0      810 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/base_image_dockerfiles/Dockerfile_jupyter_sklearn_3.9
--rw-r--r--   0        0        0     1114 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/base_image_dockerfiles/Dockerfile_jupyter_tf_3.10
--rw-r--r--   0        0        0     1114 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/base_image_dockerfiles/Dockerfile_jupyter_tf_3.11
--rw-r--r--   0        0        0     1161 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/base_image_dockerfiles/Dockerfile_jupyter_tf_3.8
--rw-r--r--   0        0        0     1112 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/base_image_dockerfiles/Dockerfile_jupyter_tf_3.9
--rw-r--r--   0        0        0     1239 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/base_image_dockerfiles/Dockerfile_jupyter_torch_3.10
--rw-r--r--   0        0        0     1239 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/base_image_dockerfiles/Dockerfile_jupyter_torch_3.11
--rw-r--r--   0        0        0     1237 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/base_image_dockerfiles/Dockerfile_jupyter_torch_3.8
--rw-r--r--   0        0        0     1237 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/base_image_dockerfiles/Dockerfile_jupyter_torch_3.9
--rw-r--r--   0        0        0     6110 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/base_image_dockerfiles/build_push_images.sh
--rw-r--r--   0        0        0    24810 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/client.py
--rw-r--r--   0        0        0     3795 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/constants.py
--rw-r--r--   0        0        0    18611 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/containers.py
--rw-r--r--   0        0        0     9394 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/datacite.py
--rw-r--r--   0        0        0    13354 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/entrypoints.py
--rw-r--r--   0        0        0     1068 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/garden_file_adapter.py
--rw-r--r--   0        0        0    18186 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/gardens.py
--rw-r--r--   0        0        0        0 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/globus_search/__init__.py
--rw-r--r--   0        0        0     1409 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/globus_search/garden_search.py
--rw-r--r--   0        0        0     6461 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/local_data.py
--rw-r--r--   0        0        0     2030 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/mlmodel.py
--rw-r--r--   0        0        0      107 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/model_connectors/__init__.py
--rw-r--r--   0        0        0     2449 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/model_connectors/github_conn.py
--rw-r--r--   0        0        0     1712 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/model_connectors/hugging_face.py
--rw-r--r--   0        0        0     8060 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/notebook_metadata.py
--rw-r--r--   0        0        0     2426 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/notebook_templates/debug.ipynb
--rw-r--r--   0        0        0     1203 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/notebook_templates/empty.ipynb
--rw-r--r--   0        0        0     7498 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/notebook_templates/sklearn.ipynb
--rw-r--r--   0        0        0     7405 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/notebook_templates/tensorflow.ipynb
--rw-r--r--   0        0        0     7620 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/notebook_templates/torch.ipynb
--rw-r--r--   0        0        0    10258 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/notebook_templates/tutorial.ipynb
--rw-r--r--   0        0        0     3491 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/scripts/save_session_and_metadata.py
--rw-r--r--   0        0        0        0 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/utils/__init__.py
--rw-r--r--   0        0        0     3394 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/utils/_meta.py
--rw-r--r--   0        0        0      628 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/utils/dois.py
--rw-r--r--   0        0        0     1684 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/utils/interactive_cli.py
--rw-r--r--   0        0        0     2769 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/utils/misc.py
--rw-r--r--   0        0        0     1854 2024-03-26 16:19:12.315626 garden_ai-1.0.9/garden_ai/utils/notebooks.py
--rw-r--r--   0        0        0     2544 2024-03-26 16:19:34.687435 garden_ai-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     2581 1970-01-01 00:00:00.000000 garden_ai-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-03 16:58:19.319971 garden_ai-2.0.0/LICENSE
+-rw-r--r--   0        0        0      797 2024-05-03 16:58:19.319971 garden_ai-2.0.0/README.md
+-rw-r--r--   0        0        0      537 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/__init__.py
+-rw-r--r--   0        0        0       54 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/__main__.py
+-rw-r--r--   0        0        0      180 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/_version.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/app/__init__.py
+-rw-r--r--   0        0        0      905 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/app/completion.py
+-rw-r--r--   0        0        0     2501 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/app/console.py
+-rw-r--r--   0        0        0     2840 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/app/docker.py
+-rw-r--r--   0        0        0     7963 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/app/entrypoint.py
+-rw-r--r--   0        0        0    16504 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/app/garden.py
+-rw-r--r--   0        0        0     1936 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/app/main.py
+-rw-r--r--   0        0        0    22960 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/app/notebook.py
+-rw-r--r--   0        0        0     3280 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/backend_client.py
+-rw-r--r--   0        0        0    24960 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/client.py
+-rw-r--r--   0        0        0     3970 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/constants.py
+-rw-r--r--   0        0        0    18666 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/containers.py
+-rw-r--r--   0        0        0     9394 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/datacite.py
+-rw-r--r--   0        0        0    13997 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/entrypoints.py
+-rw-r--r--   0        0        0     1068 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/garden_file_adapter.py
+-rw-r--r--   0        0        0    18186 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/gardens.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/globus_search/__init__.py
+-rw-r--r--   0        0        0     1409 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/globus_search/garden_search.py
+-rw-r--r--   0        0        0     6461 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/local_data.py
+-rw-r--r--   0        0        0     3270 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/mlmodel.py
+-rw-r--r--   0        0        0      107 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/model_connectors/__init__.py
+-rw-r--r--   0        0        0     2449 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/model_connectors/github_conn.py
+-rw-r--r--   0        0        0     1712 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/model_connectors/hugging_face.py
+-rw-r--r--   0        0        0     8060 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/notebook_metadata.py
+-rw-r--r--   0        0        0     2423 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/notebook_templates/debug.ipynb
+-rw-r--r--   0        0        0     1200 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/notebook_templates/empty.ipynb
+-rw-r--r--   0        0        0     7490 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/notebook_templates/sklearn.ipynb
+-rw-r--r--   0        0        0     7405 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/notebook_templates/tensorflow.ipynb
+-rw-r--r--   0        0        0     7612 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/notebook_templates/torch.ipynb
+-rw-r--r--   0        0        0    10250 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/notebook_templates/tutorial.ipynb
+-rw-r--r--   0        0        0     3495 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/scripts/save_session_and_metadata.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/utils/__init__.py
+-rw-r--r--   0        0        0     3394 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/utils/_meta.py
+-rw-r--r--   0        0        0      628 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/utils/dois.py
+-rw-r--r--   0        0        0     1684 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/utils/interactive_cli.py
+-rw-r--r--   0        0        0     2769 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/utils/misc.py
+-rw-r--r--   0        0        0     1854 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/utils/notebooks.py
+-rw-r--r--   0        0        0     2545 2024-05-03 16:58:30.431993 garden_ai-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2583 1970-01-01 00:00:00.000000 garden_ai-2.0.0/PKG-INFO
```

### Comparing `garden_ai-1.0.9/LICENSE` & `garden_ai-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/README.md` & `garden_ai-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/garden_ai/__init__.py` & `garden_ai-2.0.0/garden_ai/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from ._version import __version__  # noqa  # type: ignore
-from .constants import GardenConstants
 from .client import GardenClient
-from .gardens import Garden, PublishedGarden
+from .constants import GardenConstants
 from .entrypoints import (
     EntrypointMetadata,
     RegisteredEntrypoint,
+    entrypoint_test,
     garden_entrypoint,
     garden_step,
-    entrypoint_test,
 )
+from .gardens import Garden, PublishedGarden
+from .mlmodel import DatasetConnection
 
 __all__ = [
     "GardenConstants",
     "GardenClient",
     "Garden",
     "PublishedGarden",
     "EntrypointMetadata",
     "RegisteredEntrypoint",
     "garden_entrypoint",
     "garden_step",
     "entrypoint_test",
+    "DatasetConnection",
 ]
```

### Comparing `garden_ai-1.0.9/garden_ai/app/completion.py` & `garden_ai-2.0.0/garden_ai/app/completion.py`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/garden_ai/app/console.py` & `garden_ai-2.0.0/garden_ai/app/console.py`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/garden_ai/app/docker.py` & `garden_ai-2.0.0/garden_ai/app/docker.py`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/garden_ai/app/entrypoint.py` & `garden_ai-2.0.0/garden_ai/app/entrypoint.py`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/garden_ai/app/garden.py` & `garden_ai-2.0.0/garden_ai/app/garden.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         "--description",
         help=(
             "A brief summary of the Garden and/or its purpose, to aid discovery by other Gardeners."
         ),
         rich_help_panel="Recommended",
     ),
     tags: List[str] = typer.Option(
-        None,
+        [],
         "--tag",
         help="Add a tag, keyword, key phrase or other classification pertaining to the Garden.",
         rich_help_panel="Recommended",
     ),
     verbose: bool = typer.Option(
         False, help="If true, pretty-print Garden's metadata when created."
     ),
```

### Comparing `garden_ai-1.0.9/garden_ai/app/main.py` & `garden_ai-2.0.0/garden_ai/app/main.py`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/garden_ai/app/notebook.py` & `garden_ai-2.0.0/garden_ai/app/notebook.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
             "To see all the available Garden base images, use 'garden-ai notebook list-premade-images'"
         ),
     ),
     requirements_path: Optional[Path] = typer.Option(
         None,
         "--requirements",
         help=(
-            "Path to a requirements.txt or a conda environment.yml containing "
+            "Path to a requirements.txt containing "
             "additional dependencies to install in the base image."
         ),
     ),
     custom_image_uri: Optional[str] = typer.Option(
         None,
         "--custom-image",
         help=(
@@ -312,15 +312,15 @@
             "Path to a .ipynb notebook whose remote environment will be approximated for debugging."
         ),
     ),
     requirements_path: Optional[Path] = typer.Option(
         None,
         "--requirements",
         help=(
-            "Path to a requirements.txt or a conda environment.yml containing "
+            "Path to a requirements.txt containing "
             "additional dependencies to install in the base image."
         ),
     ),
 ):
     """Open the debugging notebook in a pre-prepared container.
 
     Changes to the notebook file will NOT persist after the container shuts down.
@@ -328,15 +328,15 @@
     """
 
     with DockerClientSession(verbose=True) as docker_client:
         base_image_uri = (
             _get_base_image_uri(
                 base_image_name=None, custom_image_uri=None, notebook_path=path
             )
-            or "gardenai/base:python-3.10-jupyter"
+            or "gardenai/base:python-3.10-base"
         )
 
         # Validate and read requirements file.
         if requirements_path:
             _validate_requirements_path(requirements_path)
             requirements_data = read_requirements_data(requirements_path)
         else:
@@ -416,15 +416,15 @@
         writable=True,
         readable=True,
     ),
     requirements_path: Optional[Path] = typer.Option(
         None,
         "--requirements",
         help=(
-            "Path to a requirements.txt or a conda environment.yml containing "
+            "Path to a requirements.txt containing "
             "additional dependencies to install in the base image."
         ),
     ),
     base_image_name: Optional[str] = typer.Option(
         None,
         "--base-image",
         help=(
```

### Comparing `garden_ai-1.0.9/garden_ai/backend_client.py` & `garden_ai-2.0.0/garden_ai/backend_client.py`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/garden_ai/client.py` & `garden_ai-2.0.0/garden_ai/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pathlib import Path
 from typing import List, Union
 from uuid import UUID
 
 import typer
 from globus_compute_sdk import Client
 from globus_compute_sdk.sdk.login_manager.tokenstore import get_token_storage_adapter
+from globus_compute_sdk.sdk.login_manager import ComputeScopes
 from globus_compute_sdk.serialize.concretes import DillCodeTextInspect
 from globus_sdk import (
     AuthAPIError,
     AuthLoginClient,
     ClientCredentialsAuthorizer,
     ConfidentialAppAuthClient,
     GroupsClient,
@@ -23,30 +24,29 @@
     SearchClient,
 )
 from globus_sdk.scopes import ScopeBuilder
 from globus_sdk.tokenstorage import SimpleJSONFileAdapter
 from rich import print
 from rich.prompt import Prompt
 
-from garden_ai import GardenConstants, local_data
+from garden_ai import local_data
+from garden_ai.constants import GardenConstants
 from garden_ai.backend_client import BackendClient
 from garden_ai.garden_file_adapter import GardenFileAdapter
 from garden_ai.gardens import Garden, PublishedGarden
 from garden_ai.globus_search import garden_search
 from garden_ai.local_data import GardenNotFoundException, EntrypointNotFoundException
 from garden_ai.entrypoints import (
     Paper,
     RegisteredEntrypoint,
     Repository,
 )
 from garden_ai.utils._meta import make_function_to_register
 from garden_ai.utils.misc import extract_email_from_globus_jwt
 
-COMPUTE_RESOURCE_SERVER_NAME = "funcx_service"
-
 logger = logging.getLogger()
 
 
 class AuthException(Exception):
     pass
 
 
@@ -105,15 +105,15 @@
             self.groups_authorizer = self._create_authorizer(
                 GroupsClient.scopes.resource_server
             )
             self.search_authorizer = self._create_authorizer(
                 SearchClient.scopes.resource_server
             )
             self.compute_authorizer = self._create_authorizer(
-                COMPUTE_RESOURCE_SERVER_NAME
+                ComputeScopes.resource_server
             )
             self.search_client = (
                 SearchClient(authorizer=self.search_authorizer)
                 if not search_client
                 else search_client
             )
             self.garden_authorizer = self._create_authorizer(
@@ -164,18 +164,20 @@
         )
 
     def _do_login_flow(self):
         self.auth_client.oauth2_start_flow(
             requested_scopes=[
                 AuthLoginClient.scopes.openid,
                 AuthLoginClient.scopes.email,
+                AuthLoginClient.scopes.manage_projects,
                 GroupsClient.scopes.view_my_groups_and_memberships,
                 SearchClient.scopes.all,
                 GardenClient.scopes.test_scope,
-                Client.FUNCX_SCOPE,
+                GardenClient.scopes.action_all,
+                ComputeScopes.all,
             ],
             refresh_tokens=True,
         )
         authorize_url = self.auth_client.oauth2_get_authorize_url()
 
         try:
             __IPYTHON__  # Check if running in notebook. '__IPYTHON__' is defined if in one.
```

### Comparing `garden_ai-1.0.9/garden_ai/constants.py` & `garden_ai-2.0.0/garden_ai/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,39 +2,44 @@
 from dotenv import load_dotenv
 import pathlib
 
 # get env file from project root
 dotenv_path = pathlib.Path(f"{__file__}/../..").resolve() / ".env.shared"
 load_dotenv(str(dotenv_path), override=False)
 
-_PROD_ENDPOINT = "https://nu3cetwc84.execute-api.us-east-1.amazonaws.com/garden_prod"
-_DEV_ENDPOINT = "https://y0ipq1bueb.execute-api.us-east-1.amazonaws.com/garden_dev"
+_PROD_ENDPOINT = "https://api.thegardens.ai"
+_DEV_ENDPOINT = "https://api-dev.thegardens.ai"
+_LOCAL_ENDPOINT = "http://localhost:5500"
 
 _DEV_SEARCH_INDEX = "58e4df29-4492-4e7d-9317-b27eba62a911"
 _PROD_SEARCH_INDEX = "813d4556-cbd4-4ba9-97f2-a7155f70682f"
 
 _PROD_ECR_REPO = "public.ecr.aws/x2v7f8j4/garden-containers-prod"
 _DEV_ECR_REPO = "public.ecr.aws/x2v7f8j4/garden-containers-dev"
 
 
 class GardenConstants:
     GARDEN_TEST_EMAIL = "garden-test-runner@email.com"
     GARDEN_DIR = os.path.expanduser("~/.garden")
     GARDEN_KEY_STORE = os.path.join(GARDEN_DIR, "tokens.json")
     URL_ENV_VAR_NAME = "GARDEN_MODELS"
     GARDEN_ENDPOINT = (
-        _DEV_ENDPOINT if os.environ.get("GARDEN_ENV") == "dev" else _PROD_ENDPOINT
+        _LOCAL_ENDPOINT
+        if os.environ.get("GARDEN_ENV") == "local"
+        else _DEV_ENDPOINT if os.environ.get("GARDEN_ENV") == "dev" else _PROD_ENDPOINT
     )
     GARDEN_INDEX_UUID = (
         _DEV_SEARCH_INDEX
-        if os.environ.get("GARDEN_ENV") == "dev"
+        if os.environ.get("GARDEN_ENV") in ("dev", "local")
         else _PROD_SEARCH_INDEX
     )
     GARDEN_ECR_REPO = (
-        _DEV_ECR_REPO if os.environ.get("GARDEN_ENV") == "dev" else _PROD_ECR_REPO
+        _DEV_ECR_REPO
+        if os.environ.get("GARDEN_ENV") in ("dev", "local")
+        else _PROD_ECR_REPO
     )
 
     DEMO_ENDPOINT = "6ed5d749-abc3-4c83-bcad-80837b3d126f"
 
     # Constants for picking a port to start a Jupyter notebook on
     DEFAULT_JUPYTER_PORT = 9188
     MAX_JUPYTER_PORTS_TO_ATTEMPT = 10
@@ -55,31 +60,34 @@
             "10.26311/s8hf-3v65",
             "10.26311/aefd-p769",
             "10.26311/cd31-az33",
         ]
     )
 
     PREMADE_IMAGES = {
-        "3.8-base": "gardenai/base:python-3.8-jupyter",
-        "3.9-base": "gardenai/base:python-3.9-jupyter",
-        "3.10-base": "gardenai/base:python-3.10-jupyter",
-        "3.11-base": "gardenai/base:python-3.11-jupyter",
-        "3.8-sklearn": "gardenai/base:python-3.8-jupyter-sklearn",
-        "3.9-sklearn": "gardenai/base:python-3.9-jupyter-sklearn",
-        "3.10-sklearn": "gardenai/base:python-3.10-jupyter-sklearn",
-        "3.11-sklearn": "gardenai/base:python-3.11-jupyter-sklearn",
-        "3.8-tensorflow": "gardenai/base:python-3.8-jupyter-tf",
-        "3.9-tensorflow": "gardenai/base:python-3.9-jupyter-tf",
-        "3.10-tensorflow": "gardenai/base:python-3.10-jupyter-tf",
-        "3.11-tensorflow": "gardenai/base:python-3.11-jupyter-tf",
-        "3.8-torch": "gardenai/base:python-3.8-jupyter-torch",
-        "3.9-torch": "gardenai/base:python-3.9-jupyter-torch",
-        "3.10-torch": "gardenai/base:python-3.10-jupyter-torch",
-        "3.11-torch": "gardenai/base:python-3.11-jupyter-torch",
-        "3.10-all-extras": "gardenai/base:python-3.10-jupyter-all",
+        "3.8-base": "gardenai/base:python-3.8-base",
+        "3.9-base": "gardenai/base:python-3.9-base",
+        "3.10-base": "gardenai/base:python-3.10-base",
+        "3.11-base": "gardenai/base:python-3.11-base",
+        "3.8-sklearn": "gardenai/base:python-3.8-sklearn",
+        "3.9-sklearn": "gardenai/base:python-3.9-sklearn",
+        "3.10-sklearn": "gardenai/base:python-3.10-sklearn",
+        "3.11-sklearn": "gardenai/base:python-3.11-sklearn",
+        "3.8-tensorflow": "gardenai/base:python-3.8-tensorflow",
+        "3.9-tensorflow": "gardenai/base:python-3.9-tensorflow",
+        "3.10-tensorflow": "gardenai/base:python-3.10-tensorflow",
+        "3.11-tensorflow": "gardenai/base:python-3.11-tensorflow",
+        "3.8-torch": "gardenai/base:python-3.8-torch",
+        "3.9-torch": "gardenai/base:python-3.9-torch",
+        "3.10-torch": "gardenai/base:python-3.10-torch",
+        "3.11-torch": "gardenai/base:python-3.11-torch",
+        "3.8-all-extras": "gardenai/base:python-3.8-all",
+        "3.9-all-extras": "gardenai/base:python-3.9-all",
+        "3.10-all-extras": "gardenai/base:python-3.10-all",
+        "3.11-all-extras": "gardenai/base:python-3.11-all",
     }
 
     IMAGES_TO_FLAVOR = {
         "3.8-base": "empty.ipynb",
         "3.9-base": "empty.ipynb",
         "3.10-base": "empty.ipynb",
         "3.11-base": "empty.ipynb",
```

### Comparing `garden_ai-1.0.9/garden_ai/containers.py` & `garden_ai-2.0.0/garden_ai/containers.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,27 +435,28 @@
     Raises:
         DockerPreBuildFailure: If the build fails.
     """
 
     # always install garden first
     dockerfile_content = f"""
     FROM {base_image}
-    RUN pip install garden-ai
+    WORKDIR /garden
+    RUN pip install --no-cache-dir --upgrade garden-ai
     """
     with TemporaryDirectory() as temp_dir:
         temp_dir_path = pathlib.Path(temp_dir)
 
         # append to Dockerfile based on whether dependencies are provided
         if requirements_data is not None:
             requirements_path = save_requirements_data(temp_dir_path, requirements_data)
             if requirements_path is not None:
                 if requirements_path.suffix == ".txt":  # pip
                     dockerfile_content += f"""
                     COPY {requirements_path.name} /garden/{requirements_path.name}
-                    RUN pip install -r /garden/{requirements_path.name}
+                    RUN pip install --upgrade -r /garden/{requirements_path.name}
                     """
                 else:  # conda
                     # nb: installs directly into base environment instead of isolating from image's already-installed packages
                     dockerfile_content += f"""
                     COPY {requirements_path.name} /garden/{requirements_path.name}
                     RUN conda env update --name base --file /garden/{requirements_path.name} && conda clean -afy
                     """
```

### Comparing `garden_ai-1.0.9/garden_ai/datacite.py` & `garden_ai-2.0.0/garden_ai/datacite.py`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/garden_ai/entrypoints.py` & `garden_ai-2.0.0/garden_ai/entrypoints.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     DataciteSchema,
     Description,
     Identifier,
     Subject,
     Title,
     Types,
 )
-from garden_ai.mlmodel import ModelMetadata
+from garden_ai.mlmodel import ModelMetadata, DatasetConnection
 from garden_ai.utils.misc import JSON
 
 
 logger = logging.getLogger()
 
 
 class Repository(BaseModel):
@@ -104,28 +104,30 @@
         Otherwise we will generate a DOI for you.
         title: A short title that describes the entrypoint.
         description: A longer free text description of this entrypoint.
         authors: A list of the authors of this entrypoint. You need at least one.
         short_name: This will be the name of the Python method that people call to invoke your entrypoint.
         year: When did you make this entrypoint? (Defaults to current year)
         tags: Helpful tags
-        repositories: List of related code repositories, like GitHub or GitLab repos.
-        papers: List of related papers, like a paper that describes the model you are publishing here.
+        repositories: List of related code repositories (``Repository``), like GitHub or GitLab repos.
+        papers: List of related papers, like a paper (``Paper``) that describes the model you are publishing here.
+        datasets: List of related datasets (``DatasetConnection``) that is related to the entrypoint you are publishing.
     """
 
     doi: Optional[str] = Field(None)
     title: str = Field(...)
     authors: List[str] = Field(...)
     short_name: Optional[str] = Field(None)
     description: Optional[str] = Field(None)
     year: str = Field(default_factory=lambda: str(datetime.now().year))
     tags: List[str] = Field(default_factory=list, unique_items=True)
     models: List[ModelMetadata] = Field(default_factory=list)
     repositories: List[Repository] = Field(default_factory=list)
     papers: List[Paper] = Field(default_factory=list)
+    datasets: List[DatasetConnection] = Field(default_factory=list)
     # The PrivateAttrs below are used internally for publishing.
     _test_functions: List[str] = PrivateAttr(default_factory=list)
     _target_garden_doi: Optional[str] = PrivateAttr(None)
     _as_step: Optional[Step] = PrivateAttr(None)
 
 
 class RegisteredEntrypoint(EntrypointMetadata):
@@ -271,19 +273,28 @@
         """
         return self.doi in GardenConstants.DLHUB_DOIS
 
 
 def garden_entrypoint(
     metadata: EntrypointMetadata,
     garden_doi: str = None,
-    model_connectors=None,
+    model_connectors: Optional[List] = None,
+    datasets: Optional[List[DatasetConnection]] = None,
 ):
     def decorate(func):
+        if datasets:
+            # datasets explicitly connected to entrypoint by decorator
+            metadata.datasets += datasets
         if model_connectors:
-            metadata.models += [connector.metadata for connector in model_connectors]
+            for connector in model_connectors:
+                model_meta: ModelMetadata = connector.metadata
+                metadata.models += [model_meta]
+                # datasets implicitly connected from model metadata
+                metadata.datasets += model_meta.datasets
+
         metadata._as_step = Step(
             function_text=inspect.getsource(func),
             function_name=func.__name__,
             description="Top level entrypoint function",
         )
         metadata._target_garden_doi = garden_doi
         # let func carry its own metadata
```

### Comparing `garden_ai-1.0.9/garden_ai/garden_file_adapter.py` & `garden_ai-2.0.0/garden_ai/garden_file_adapter.py`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/garden_ai/gardens.py` & `garden_ai-2.0.0/garden_ai/gardens.py`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/garden_ai/globus_search/garden_search.py` & `garden_ai-2.0.0/garden_ai/globus_search/garden_search.py`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/garden_ai/local_data.py` & `garden_ai-2.0.0/garden_ai/local_data.py`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/garden_ai/mlmodel.py` & `garden_ai-2.0.0/garden_ai/mlmodel.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,38 +7,74 @@
 class ModelRepository(Enum):
     HUGGING_FACE = "Hugging Face"
     GITHUB = "GitHub"
 
 
 class DatasetConnection(BaseModel):
     """
-    The ``DataSetConnection`` class represents all the metadata we want to \
-    publically expose about the datasets that can be utilized with this model.
+    The ``DatasetConnection`` class represents metadata of external datasets \
+    which publishers want to highlight as related to their Entrypoint. This \
+    metadata (if provided) will be displayed with the Entrypoint as "related \
+    work".
+
+    These can be linked to an Entrypoint directly in the `EntrypointMetadata` or \
+    via the ``@garden_entrypoint`` decorator with the `datasets` kwarg.
+
+    Example:
+
+        ```python
+        my_relevant_dataset = DatasetConnection(
+            title="Benchmark Dataset for Locating Atoms in STEM images",
+            doi="10.18126/e73h-3w6n",
+            url="https://foundry-ml.org/#/datasets/10.18126%2Fe73h-3w6n",
+            repository="foundry",
+        )
+        my_metadata = EntrypointMetadata(
+            title="...",
+            # etc
+        )
+
+        @garden_entrypoint(metadata=my_metadata, datasets=[my_relevant_dataset])
+        def my_entrypoint(*args, **kwargs):
+            ...
+
+        ```
+
 
     Attributes:
         title (str):
             A short and descriptive name of the dataset.
         doi (str):
             A digital identifier to the dataset.
         url (str):
             Location where the dataset can be accessed. If using foundry \
             dataset, both url and DOI must be provided.
         repository (str):
-            The public repository where the dataset is hosted
+            The public repository where the dataset is hosted (e.g. "foundry", "github")
         data_type (str):
             Optional, the type of file of dataset.
 
     """
 
     title: str = Field(...)
     doi: Optional[str] = Field(None)
     url: str = Field(...)
     data_type: Optional[str] = Field(None)
     repository: str = Field(...)
 
+    @validator("repository")
+    def check_foundry(cls, v, values, **kwargs):
+        v = v.lower()  # case-insensitive
+        if "url" in values and "doi" in values:
+            if v == "foundry" and (values["url"] is None or values["doi"] is None):
+                raise ValueError(
+                    "For a Foundry repository, both url and doi must be provided"
+                )
+        return v
+
 
 class ModelMetadata(BaseModel):
     """
     The ``ModelMetadata`` class represents metadata about an ML model published  \
     on a public model repository used in an Entrypoint.
 
     Attributes:
```

### Comparing `garden_ai-1.0.9/garden_ai/model_connectors/github_conn.py` & `garden_ai-2.0.0/garden_ai/model_connectors/github_conn.py`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/garden_ai/model_connectors/hugging_face.py` & `garden_ai-2.0.0/garden_ai/model_connectors/hugging_face.py`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/garden_ai/notebook_metadata.py` & `garden_ai-2.0.0/garden_ai/notebook_metadata.py`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/garden_ai/notebook_templates/debug.ipynb` & `garden_ai-2.0.0/garden_ai/notebook_templates/debug.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997395833333333%*

 * *Differences: {"'cells'": "{0: {'metadata': {'garden_metadata': {'NOTEBOOK_BASE_IMAGE_URI': "*

 * *            "'gardenai/base:python-3.9-base'}}}}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "garden_metadata": {
-                    "NOTEBOOK_BASE_IMAGE_URI": "gardenai/base:python-3.9-jupyter"
+                    "NOTEBOOK_BASE_IMAGE_URI": "gardenai/base:python-3.9-base"
                 },
                 "tags": [
                     "garden_metadata_cell"
                 ]
             },
             "outputs": [],
             "source": [
```

### Comparing `garden_ai-1.0.9/garden_ai/notebook_templates/empty.ipynb` & `garden_ai-2.0.0/garden_ai/notebook_templates/empty.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99921875%*

 * *Differences: {"'cells'": "{0: {'metadata': {'garden_metadata': {'NOTEBOOK_BASE_IMAGE_URI': "*

 * *            "'gardenai/base:python-3.9-base'}}}}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "garden_metadata": {
-                    "NOTEBOOK_BASE_IMAGE_URI": "gardenai/base:python-3.9-jupyter"
+                    "NOTEBOOK_BASE_IMAGE_URI": "gardenai/base:python-3.9-base"
                 },
                 "tags": [
                     "garden_metadata_cell"
                 ]
             },
             "outputs": [],
             "source": [
```

### Comparing `garden_ai-1.0.9/garden_ai/notebook_templates/sklearn.ipynb` & `garden_ai-2.0.0/garden_ai/notebook_templates/sklearn.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998883928571429%*

 * *Differences: {"'cells'": "{0: {'metadata': {'garden_metadata': {'NOTEBOOK_BASE_IMAGE_URI': "*

 * *            "'gardenai/base:python-3.9-sklearn'}}}}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "garden_metadata": {
-                    "NOTEBOOK_BASE_IMAGE_URI": "gardenai/base:python-3.9-jupyter-sklearn"
+                    "NOTEBOOK_BASE_IMAGE_URI": "gardenai/base:python-3.9-sklearn"
                 },
                 "tags": [
                     "garden_metadata_cell"
                 ]
             },
             "outputs": [],
             "source": [
```

### Comparing `garden_ai-1.0.9/garden_ai/notebook_templates/tensorflow.ipynb` & `garden_ai-2.0.0/garden_ai/notebook_templates/tensorflow.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998883928571429%*

 * *Differences: {"'cells'": "{0: {'metadata': {'garden_metadata': {'NOTEBOOK_BASE_IMAGE_URI': "*

 * *            "'gardenai/base:python-3.9-tensorflow'}}}}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "garden_metadata": {
-                    "NOTEBOOK_BASE_IMAGE_URI": "gardenai/base:python-3.9-jupyter-tf"
+                    "NOTEBOOK_BASE_IMAGE_URI": "gardenai/base:python-3.9-tensorflow"
                 },
                 "tags": [
                     "garden_metadata_cell"
                 ]
             },
             "outputs": [],
             "source": [
```

### Comparing `garden_ai-1.0.9/garden_ai/notebook_templates/torch.ipynb` & `garden_ai-2.0.0/garden_ai/notebook_templates/torch.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998958333333333%*

 * *Differences: {"'cells'": "{0: {'metadata': {'garden_metadata': {'NOTEBOOK_BASE_IMAGE_URI': "*

 * *            "'gardenai/base:python-3.9-torch'}}}}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "garden_metadata": {
-                    "NOTEBOOK_BASE_IMAGE_URI": "gardenai/base:python-3.9-jupyter-torch"
+                    "NOTEBOOK_BASE_IMAGE_URI": "gardenai/base:python-3.9-torch"
                 },
                 "tags": [
                     "garden_metadata_cell"
                 ]
             },
             "outputs": [],
             "source": [
```

### Comparing `garden_ai-1.0.9/garden_ai/notebook_templates/tutorial.ipynb` & `garden_ai-2.0.0/garden_ai/notebook_templates/tutorial.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999131944444444%*

 * *Differences: {"'cells'": "{0: {'metadata': {'garden_metadata': {'NOTEBOOK_BASE_IMAGE_URI': "*

 * *            "'gardenai/base:python-3.10-sklearn'}}}}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "garden_metadata": {
-                    "NOTEBOOK_BASE_IMAGE_URI": "gardenai/base:python-3.10-jupyter-sklearn"
+                    "NOTEBOOK_BASE_IMAGE_URI": "gardenai/base:python-3.10-sklearn"
                 },
                 "tags": [
                     "garden_metadata_cell"
                 ]
             },
             "outputs": [],
             "source": [
```

### Comparing `garden_ai-1.0.9/garden_ai/scripts/save_session_and_metadata.py` & `garden_ai-2.0.0/garden_ai/scripts/save_session_and_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             "To ensure compatibility with Globus Compute endpoints, Garden needs "
             f"dill version {required_dill_version} when running python version "
             f"{'.'.join(map(str, python_version[:2]))}. However, this environment "
             f"has dill version {dill_version} installed, possibly due to other "
             "packages installed from within your notebook. \n\nIf you are installing "
             "dependencies from a cell of your notebook, try specifying them in a "
             "requirements file with the `--requirements` flag from the command line "
-            "instead try again. "
+            "instead and try again. "
         )
         raise EnvironmentError(message)
 
 
 if __name__ == "__main__":
     import dill  # type: ignore
```

### Comparing `garden_ai-1.0.9/garden_ai/utils/_meta.py` & `garden_ai-2.0.0/garden_ai/utils/_meta.py`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/garden_ai/utils/dois.py` & `garden_ai-2.0.0/garden_ai/utils/dois.py`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/garden_ai/utils/interactive_cli.py` & `garden_ai-2.0.0/garden_ai/utils/interactive_cli.py`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/garden_ai/utils/misc.py` & `garden_ai-2.0.0/garden_ai/utils/misc.py`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/garden_ai/utils/notebooks.py` & `garden_ai-2.0.0/garden_ai/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `garden_ai-1.0.9/pyproject.toml` & `garden_ai-2.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "garden-ai"
-version = "1.0.9" # placeholder
+version = "2.0.0" # placeholder
 description = "Garden: tools to simplify access to scientific AI advances."
 # note to contributors: feel free to add yourselves to this list 🌱
 maintainers = [
   "Globus Labs <labs@globus.org>",
   "Owen Price Skelly",
   "Will Engler",
   "Ben Blaiszik",
@@ -29,20 +29,20 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 dill = [ # same constraints as globus compute
 # https://github.com/funcx-faas/funcX/blob/369807addb855e1964d55bada67c0a374ba44896/compute_sdk/setup.py#L17
      {version = "0.3.5.1", python = "<3.11"},
      {version = "0.3.6", python= ">=3.11"}
 ]
-cryptography = "^41.0.6"
+cryptography = "^42.0.0"
 requests = "^2.20.0"
 gitpython = "^3.1.35"
 globus-sdk = "^3.34.0"
 pydantic = "^1.10.13"
-typer = { extras = ["all"], version = "^0.7.0" }
+typer = { extras = ["all"], version = "^0.12.3" }
 jinja2 = "^3.1.2"
 huggingface-hub = "0.18.0"
 pyyaml = "^6.0"
 packaging = "^23.0"
 globus-compute-sdk = "^2.2.0"
 tabulate = "^0.9.0"
 types-tabulate = "^0.9.0.3"
```

### Comparing `garden_ai-1.0.9/PKG-INFO` & `garden_ai-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garden-ai
-Version: 1.0.9
+Version: 2.0.0
 Summary: Garden: tools to simplify access to scientific AI advances.
 Home-page: https://thegardens.ai
 License: MIT
 Author: Garden Team
 Author-email: labs@globus.org
 Maintainer: Globus Labs
 Maintainer-email: labs@globus.org
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.29,<2.0)
 Requires-Dist: boto3-stubs (>=1.29,<2.0)
-Requires-Dist: cryptography (>=41.0.6,<42.0.0)
+Requires-Dist: cryptography (>=42.0.0,<43.0.0)
 Requires-Dist: dill (==0.3.5.1) ; python_version < "3.11"
 Requires-Dist: dill (==0.3.6) ; python_version >= "3.11"
 Requires-Dist: docker (>=6.1.3,<7.0.0)
 Requires-Dist: gitpython (>=3.1.35,<4.0.0)
 Requires-Dist: globus-compute-sdk (>=2.2.0,<3.0.0)
 Requires-Dist: globus-sdk (>=3.34.0,<4.0.0)
 Requires-Dist: huggingface-hub (==0.18.0)
@@ -32,15 +32,15 @@
 Requires-Dist: nbformat (>=5.9.2,<6.0.0)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pydantic (>=1.10.13,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.20.0,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
-Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Requires-Dist: typer[all] (>=0.12.3,<0.13.0)
 Requires-Dist: types-tabulate (>=0.9.0.3,<0.10.0.0)
 Project-URL: Documentation, https://garden-ai.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Garden-AI/garden
 Description-Content-Type: text/markdown
 
 # Garden
```


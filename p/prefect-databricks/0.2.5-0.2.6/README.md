# Comparing `tmp/prefect_databricks-0.2.5.tar.gz` & `tmp/prefect_databricks-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_databricks-0.2.5.tar", last modified: Fri Apr 26 15:03:56 2024, max compression
+gzip compressed data, was "prefect_databricks-0.2.6.tar", last modified: Fri May  3 16:56:44 2024, max compression
```

## Comparing `prefect_databricks-0.2.5.tar` & `prefect_databricks-0.2.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.199693 prefect_databricks-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-04-26 15:03:56.199693 prefect_databricks-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.195693 prefect_databricks-0.2.5/prefect_databricks/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/prefect_databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:03:55.000000 prefect_databricks-0.2.5/prefect_databricks/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/prefect_databricks/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    18357 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/prefect_databricks/flows.py
--rw-r--r--   0 runner    (1001) docker     (127)    81198 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/prefect_databricks/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.195693 prefect_databricks-0.2.5/prefect_databricks/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/prefect_databricks/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   168341 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/prefect_databricks/models/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/prefect_databricks/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.195693 prefect_databricks-0.2.5/prefect_databricks/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)   178999 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/prefect_databricks/schemas/jobs-2.1-aws.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.195693 prefect_databricks-0.2.5/prefect_databricks/schemas/original/
--rw-r--r--   0 runner    (1001) docker     (127)   178843 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/prefect_databricks/schemas/original/jobs-2.1-aws.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.199693 prefect_databricks-0.2.5/prefect_databricks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-04-26 15:03:55.000000 prefect_databricks-0.2.5/prefect_databricks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-26 15:03:56.000000 prefect_databricks-0.2.5/prefect_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:03:55.000000 prefect_databricks-0.2.5/prefect_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 15:03:55.000000 prefect_databricks-0.2.5/prefect_databricks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-26 15:03:55.000000 prefect_databricks-0.2.5/prefect_databricks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 15:03:55.000000 prefect_databricks-0.2.5/prefect_databricks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:03:56.199693 prefect_databricks-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.199693 prefect_databricks-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/tests/mock_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    13619 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/tests/test_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/tests/test_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:44.963230 prefect_databricks-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-03 16:56:44.963230 prefect_databricks-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:44.959230 prefect_databricks-0.2.6/prefect_databricks/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/prefect_databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 16:56:44.000000 prefect_databricks-0.2.6/prefect_databricks/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/prefect_databricks/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19110 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/prefect_databricks/flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81198 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/prefect_databricks/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:44.959230 prefect_databricks-0.2.6/prefect_databricks/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/prefect_databricks/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   168341 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/prefect_databricks/models/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/prefect_databricks/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:44.959230 prefect_databricks-0.2.6/prefect_databricks/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)   178999 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/prefect_databricks/schemas/jobs-2.1-aws.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:44.959230 prefect_databricks-0.2.6/prefect_databricks/schemas/original/
+-rw-r--r--   0 runner    (1001) docker     (127)   178843 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/prefect_databricks/schemas/original/jobs-2.1-aws.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:44.963230 prefect_databricks-0.2.6/prefect_databricks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-03 16:56:44.000000 prefect_databricks-0.2.6/prefect_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-03 16:56:44.000000 prefect_databricks-0.2.6/prefect_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:56:44.000000 prefect_databricks-0.2.6/prefect_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 16:56:44.000000 prefect_databricks-0.2.6/prefect_databricks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-03 16:56:44.000000 prefect_databricks-0.2.6/prefect_databricks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-03 16:56:44.000000 prefect_databricks-0.2.6/prefect_databricks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:56:44.963230 prefect_databricks-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:44.963230 prefect_databricks-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/tests/mock_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13610 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/tests/test_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/tests/test_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/tests/test_version.py
```

### Comparing `prefect_databricks-0.2.5/LICENSE` & `prefect_databricks-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.5/PKG-INFO` & `prefect_databricks-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-databricks
-Version: 0.2.5
+Version: 0.2.6
 Summary: Prefect integrations with Databricks
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-databricks
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `prefect_databricks-0.2.5/README.md` & `prefect_databricks-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.5/prefect_databricks/credentials.py` & `prefect_databricks-0.2.6/prefect_databricks/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.5/prefect_databricks/flows.py` & `prefect_databricks-0.2.6/prefect_databricks/flows.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Module containing flows for interacting with Databricks
 """
 
 import asyncio
 from logging import Logger
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 from prefect import flow, get_run_logger
 from prefect_databricks import DatabricksCredentials
 from prefect_databricks.jobs import (
     jobs_runs_get,
     jobs_runs_get_output,
     jobs_runs_submit,
@@ -17,14 +17,17 @@
     AccessControlRequest,
     GitSource,
     RunLifeCycleState,
     RunResultState,
     RunSubmitTaskSettings,
 )
 
+JobMetadata = Dict[str, Any]
+NotebookOutput = Dict[str, Any]
+
 
 class DatabricksJobTerminated(Exception):
     """Raised when Databricks jobs runs submit terminates"""
 
 
 class DatabricksJobSkipped(Exception):
     """Raised when Databricks jobs runs submit skips"""
@@ -61,16 +64,17 @@
     run_name: Optional[str] = None,
     max_wait_seconds: int = 900,
     poll_frequency_seconds: int = 10,
     git_source: Optional[GitSource] = None,
     timeout_seconds: Optional[int] = None,
     idempotency_token: Optional[str] = None,
     access_control_list: Optional[List[AccessControlRequest]] = None,
+    return_metadata: bool = False,
     **jobs_runs_submit_kwargs: Dict[str, Any],
-) -> Dict:
+) -> Union[NotebookOutput, Tuple[NotebookOutput, JobMetadata]]:
     """
     Flow that triggers a job run and waits for the triggered run to complete.
 
     Args:
         databricks_credentials:
             Credentials to use for authentication with Databricks.
         tasks: Tasks to run, e.g.
@@ -174,18 +178,24 @@
             jobs](https://kb.databricks.com/jobs/jobs-idempotency.html),
             e.g. `8f018174-4792-40d5-bcbc-3e6a527352c8`.
         access_control_list:
             List of permissions to set on the job.
         max_wait_seconds: Maximum number of seconds to wait for the entire flow to complete.
         poll_frequency_seconds: Number of seconds to wait in between checks for
             run completion.
+        return_metadata: When True, method will return a tuple of notebook output as well as
+            job run metadata; by default though, the method only returns notebook output
         **jobs_runs_submit_kwargs: Additional keyword arguments to pass to `jobs_runs_submit`.
 
     Returns:
-        A dictionary of task keys to its corresponding notebook output.
+        Either a dict or a tuple (depends on `return_metadata`) comprised of
+        * task_notebook_outputs: dictionary of task keys to its corresponding notebook output;
+          this is the only object returned by default from this method
+        * jobs_runs_metadata: dictionary containing IDs of the jobs runs tasks; this is only
+          returned if `return_metadata=True`.
 
     Examples:
         Submit jobs runs and wait.
         ```python
         from prefect import flow
         from prefect_databricks import DatabricksCredentials
         from prefect_databricks.flows import jobs_runs_submit_and_wait_for_completion
@@ -286,14 +296,16 @@
                 task_run_notebook_output = task_run_output.get("notebook_output", {})
                 task_notebook_outputs[task_key] = task_run_notebook_output
             logger.info(
                 "Databricks Jobs Runs Submit (%s ID %s) completed successfully!",
                 run_name,
                 multi_task_jobs_runs_id,
             )
+            if return_metadata:
+                return task_notebook_outputs, jobs_runs_metadata
             return task_notebook_outputs
         else:
             raise DatabricksJobTerminated(
                 f"Databricks Jobs Runs Submit "
                 f"({run_name} ID {multi_task_jobs_runs_id}) "
                 f"terminated with result state, {jobs_runs_result_state}: "
                 f"{jobs_runs_state_message}"
```

### Comparing `prefect_databricks-0.2.5/prefect_databricks/jobs.py` & `prefect_databricks-0.2.6/prefect_databricks/jobs.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.5/prefect_databricks/models/jobs.py` & `prefect_databricks-0.2.6/prefect_databricks/models/jobs.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.5/prefect_databricks/rest.py` & `prefect_databricks-0.2.6/prefect_databricks/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,21 @@
 
 from prefect._internal.pydantic import HAS_PYDANTIC_V2
 from prefect._internal.pydantic._compat import model_dump
 
 if HAS_PYDANTIC_V2:
     from pydantic import BaseModel as V2BaseModel
     from pydantic.v1 import BaseModel
+
+    MODELS = (BaseModel, V2BaseModel)
 else:
     from pydantic import BaseModel
 
+    MODELS = BaseModel
+
 from prefect import task
 
 if TYPE_CHECKING:
     from prefect_databricks import DatabricksCredentials
 
 
 class HTTPMethod(Enum):
@@ -50,15 +54,15 @@
         Serialized version of object.
     """
     if isinstance(obj, list):
         return [serialize_model(o) for o in obj]
     elif isinstance(obj, Dict):
         return {k: serialize_model(v) for k, v in obj.items()}
 
-    if isinstance(obj, (BaseModel, V2BaseModel)):
+    if isinstance(obj, MODELS):
         return model_dump(obj, mode="json")
     elif isinstance(obj, Enum):
         return obj.value
     return obj
 
 
 def strip_kwargs(**kwargs: Dict) -> Dict:
```

### Comparing `prefect_databricks-0.2.5/prefect_databricks/schemas/jobs-2.1-aws.yaml` & `prefect_databricks-0.2.6/prefect_databricks/schemas/jobs-2.1-aws.yaml`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.5/prefect_databricks/schemas/original/jobs-2.1-aws.yaml` & `prefect_databricks-0.2.6/prefect_databricks/schemas/original/jobs-2.1-aws.yaml`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.5/prefect_databricks.egg-info/PKG-INFO` & `prefect_databricks-0.2.6/prefect_databricks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-databricks
-Version: 0.2.5
+Version: 0.2.6
 Summary: Prefect integrations with Databricks
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-databricks
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `prefect_databricks-0.2.5/prefect_databricks.egg-info/SOURCES.txt` & `prefect_databricks-0.2.6/prefect_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.5/pyproject.toml` & `prefect_databricks-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.5/tests/mock_schema.yaml` & `prefect_databricks-0.2.6/tests/mock_schema.yaml`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.5/tests/test_block_standards.py` & `prefect_databricks-0.2.6/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.5/tests/test_flows.py` & `prefect_databricks-0.2.6/tests/test_flows.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,50 +107,48 @@
             },
         )
 
 
 class TestJobsRunsSubmitAndWaitForCompletion:
     @pytest.mark.respx(assert_all_called=True)
     async def test_run_success(self, common_mocks, respx_mock, databricks_credentials):
+        json = {
+            "state": {
+                "life_cycle_state": "TERMINATED",
+                "state_message": "",
+                "result_state": "SUCCESS",
+            },
+            "tasks": [{"run_id": 36260, "task_key": "prefect-task"}],
+        }
         respx_mock.get(
             "https://dbc-abcdefgh-123d.cloud.databricks.com/api/2.1/jobs/runs/get?run_id=36108",  # noqa
             headers={"Authorization": "Bearer testing_token"},
-        ).mock(
-            return_value=Response(
-                200,
-                json={
-                    "state": {
-                        "life_cycle_state": "TERMINATED",
-                        "state_message": "",
-                        "result_state": "SUCCESS",
-                    },
-                    "tasks": [{"run_id": 36260, "task_key": "prefect-task"}],
-                },
-            )
-        )
+        ).mock(return_value=Response(200, json=json))
 
         respx_mock.get(
             "https://dbc-abcdefgh-123d.cloud.databricks.com/api/2.1/jobs/runs/get-output",  # noqa
             headers={"Authorization": "Bearer testing_token"},
         ).mock(return_value=Response(200, json={"notebook_output": {"cell": "output"}}))
 
-        result = await jobs_runs_submit_and_wait_for_completion(
+        result, jobs_runs_metadata = await jobs_runs_submit_and_wait_for_completion(
             databricks_credentials=databricks_credentials,
             run_name="prefect-job",
+            return_metadata=True,
             tasks=[
                 {
                     "notebook_task": {
                         "notebook_path": "path",
                         "base_parameters": {"param": "a"},
                     },
                     "task_key": "key",
                 }
             ],
         )
         assert result == {"prefect-task": {"cell": "output"}}
+        assert jobs_runs_metadata == json
 
     @pytest.mark.respx(assert_all_called=True)
     async def test_run_non_notebook_success(
         self, common_mocks, respx_mock, databricks_credentials
     ):
         respx_mock.get(
             "https://dbc-abcdefgh-123d.cloud.databricks.com/api/2.1/jobs/runs/get?run_id=36108",  # noqa
```

### Comparing `prefect_databricks-0.2.5/tests/test_generate.py` & `prefect_databricks-0.2.6/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.5/tests/test_jobs.py` & `prefect_databricks-0.2.6/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.5/tests/test_rest.py` & `prefect_databricks-0.2.6/tests/test_rest.py`

 * *Files identical despite different names*


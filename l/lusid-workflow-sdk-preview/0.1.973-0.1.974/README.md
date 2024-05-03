# Comparing `tmp/lusid-workflow-sdk-preview-0.1.973.tar.gz` & `tmp/lusid-workflow-sdk-preview-0.1.974.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-workflow-sdk-preview-0.1.973.tar", last modified: Thu May  2 21:24:12 2024, max compression
+gzip compressed data, was "dist/lusid-workflow-sdk-preview-0.1.974.tar", last modified: Fri May  3 16:00:13 2024, max compression
```

## Comparing `lusid-workflow-sdk-preview-0.1.973.tar` & `lusid-workflow-sdk-preview-0.1.974.tar`

### file list

```diff
@@ -1,99 +1,106 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/
--rw-r--r--   0 root         (0) root         (0)       49 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      353 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9995 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/
--rw-r--r--   0 root         (0) root         (0)     6528 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api/
--rw-r--r--   0 root         (0) root         (0)      341 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6826 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    57864 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api/task_definitions_api.py
--rw-r--r--   0 root         (0) root         (0)    42809 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api/tasks_api.py
--rw-r--r--   0 root         (0) root         (0)    62480 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api/workers_api.py
--rw-r--r--   0 root         (0) root         (0)    27758 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16610 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5094 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/
--rw-r--r--   0 root         (0) root         (0)     5369 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7209 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     8972 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     8262 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/action_definition.py
--rw-r--r--   0 root         (0) root         (0)     6409 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/action_definition_response.py
--rw-r--r--   0 root         (0) root         (0)    12100 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/action_details.py
--rw-r--r--   0 root         (0) root         (0)    10733 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/action_details_response.py
--rw-r--r--   0 root         (0) root         (0)     7222 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)    10122 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_child_task_configuration.py
--rw-r--r--   0 root         (0) root         (0)     6232 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_child_tasks_action.py
--rw-r--r--   0 root         (0) root         (0)     5895 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_child_tasks_action_response.py
--rw-r--r--   0 root         (0) root         (0)    13450 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_task_definition_request.py
--rw-r--r--   0 root         (0) root         (0)     7821 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_task_request.py
--rw-r--r--   0 root         (0) root         (0)     9176 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_worker_request.py
--rw-r--r--   0 root         (0) root         (0)     6852 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/deleted_entity_response.py
--rw-r--r--   0 root         (0) root         (0)     4368 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/fail.py
--rw-r--r--   0 root         (0) root         (0)     4239 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/fail_response.py
--rw-r--r--   0 root         (0) root         (0)     5622 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/field_mapping.py
--rw-r--r--   0 root         (0) root         (0)     6800 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/get_worker_result_response.py
--rw-r--r--   0 root         (0) root         (0)     5878 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/health_check.py
--rw-r--r--   0 root         (0) root         (0)     5112 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/health_check_response.py
--rw-r--r--   0 root         (0) root         (0)     8000 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9489 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     5984 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/initial_state.py
--rw-r--r--   0 root         (0) root         (0)     6416 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/link.py
--rw-r--r--   0 root         (0) root         (0)     6165 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/luminesce_view.py
--rw-r--r--   0 root         (0) root         (0)     5113 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/luminesce_view_response.py
--rw-r--r--   0 root         (0) root         (0)     9530 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10695 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     7295 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/paged_resource_list_of_task.py
--rw-r--r--   0 root         (0) root         (0)     7575 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/paged_resource_list_of_task_definition.py
--rw-r--r--   0 root         (0) root         (0)     7351 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/paged_resource_list_of_worker.py
--rw-r--r--   0 root         (0) root         (0)     9076 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/parameter.py
--rw-r--r--   0 root         (0) root         (0)     5767 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/parameter_value.py
--rw-r--r--   0 root         (0) root         (0)     4822 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7735 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7175 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/resource_list_of_task.py
--rw-r--r--   0 root         (0) root         (0)     7211 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/result_field.py
--rw-r--r--   0 root         (0) root         (0)     4985 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/result_matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    11562 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/resultant_child_task_configuration.py
--rw-r--r--   0 root         (0) root         (0)    10386 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/run_worker_action.py
--rw-r--r--   0 root         (0) root         (0)    10247 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/run_worker_action_response.py
--rw-r--r--   0 root         (0) root         (0)     4435 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/run_worker_request.py
--rw-r--r--   0 root         (0) root         (0)     5179 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/run_worker_response.py
--rw-r--r--   0 root         (0) root         (0)     5383 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/scheduler_job.py
--rw-r--r--   0 root         (0) root         (0)     5119 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/scheduler_job_response.py
--rw-r--r--   0 root         (0) root         (0)     4377 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/sleep.py
--rw-r--r--   0 root         (0) root         (0)     4441 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/sleep_response.py
--rw-r--r--   0 root         (0) root         (0)    11504 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/stack.py
--rw-r--r--   0 root         (0) root         (0)    19688 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task.py
--rw-r--r--   0 root         (0) root         (0)    14093 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_definition.py
--rw-r--r--   0 root         (0) root         (0)     4386 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_definition_version.py
--rw-r--r--   0 root         (0) root         (0)     6387 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_field_definition.py
--rw-r--r--   0 root         (0) root         (0)     5243 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_instance_field.py
--rw-r--r--   0 root         (0) root         (0)     4944 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_state_definition.py
--rw-r--r--   0 root         (0) root         (0)     9826 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_summary.py
--rw-r--r--   0 root         (0) root         (0)    12376 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_transition_definition.py
--rw-r--r--   0 root         (0) root         (0)     6067 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/transition_trigger_definition.py
--rw-r--r--   0 root         (0) root         (0)     6451 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/trigger_parent_task_action.py
--rw-r--r--   0 root         (0) root         (0)     5348 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/trigger_parent_task_action_response.py
--rw-r--r--   0 root         (0) root         (0)     4440 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/trigger_schema.py
--rw-r--r--   0 root         (0) root         (0)    12546 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/update_task_definition_request.py
--rw-r--r--   0 root         (0) root         (0)     6427 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/update_task_request.py
--rw-r--r--   0 root         (0) root         (0)     8188 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/update_worker_request.py
--rw-r--r--   0 root         (0) root         (0)    11105 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/version_info.py
--rw-r--r--   0 root         (0) root         (0)    11171 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/worker.py
--rw-r--r--   0 root         (0) root         (0)     8585 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/worker_configuration.py
--rw-r--r--   0 root         (0) root         (0)     7048 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/worker_configuration_response.py
--rw-r--r--   0 root         (0) root         (0)     8967 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/worker_status_triggers.py
--rw-r--r--   0 root         (0) root         (0)    13551 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/utilities/
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3924 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2237 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:00:13.000000 lusid-workflow-sdk-preview-0.1.974/
+-rw-r--r--   0 root         (0) root         (0)       49 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      353 2024-05-03 16:00:13.000000 lusid-workflow-sdk-preview-0.1.974/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11324 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:00:13.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/
+-rw-r--r--   0 root         (0) root         (0)     7091 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:00:13.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/api/
+-rw-r--r--   0 root         (0) root         (0)      408 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6826 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    47852 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/api/event_handlers_api.py
+-rw-r--r--   0 root         (0) root         (0)    57864 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/api/task_definitions_api.py
+-rw-r--r--   0 root         (0) root         (0)    42809 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/api/tasks_api.py
+-rw-r--r--   0 root         (0) root         (0)    62480 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/api/workers_api.py
+-rw-r--r--   0 root         (0) root         (0)    27758 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16610 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5094 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:00:13.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/
+-rw-r--r--   0 root         (0) root         (0)     5865 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7209 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     8972 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     8262 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/action_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6409 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/action_definition_response.py
+-rw-r--r--   0 root         (0) root         (0)    12100 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/action_details.py
+-rw-r--r--   0 root         (0) root         (0)    10733 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/action_details_response.py
+-rw-r--r--   0 root         (0) root         (0)     7222 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)    10122 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/create_child_task_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     6232 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/create_child_tasks_action.py
+-rw-r--r--   0 root         (0) root         (0)     5895 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/create_child_tasks_action_response.py
+-rw-r--r--   0 root         (0) root         (0)    14189 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/create_event_handler_request.py
+-rw-r--r--   0 root         (0) root         (0)    13450 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/create_task_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     7821 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/create_task_request.py
+-rw-r--r--   0 root         (0) root         (0)     9176 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/create_worker_request.py
+-rw-r--r--   0 root         (0) root         (0)     6852 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/deleted_entity_response.py
+-rw-r--r--   0 root         (0) root         (0)    14474 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/event_handler.py
+-rw-r--r--   0 root         (0) root         (0)     4883 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/event_handler_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     6798 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/event_matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)     4368 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/fail.py
+-rw-r--r--   0 root         (0) root         (0)     4239 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/fail_response.py
+-rw-r--r--   0 root         (0) root         (0)     5622 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/field_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     6800 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/get_worker_result_response.py
+-rw-r--r--   0 root         (0) root         (0)     5878 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/health_check.py
+-rw-r--r--   0 root         (0) root         (0)     5112 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/health_check_response.py
+-rw-r--r--   0 root         (0) root         (0)     8000 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9489 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     5984 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/initial_state.py
+-rw-r--r--   0 root         (0) root         (0)     6416 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     6165 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/luminesce_view.py
+-rw-r--r--   0 root         (0) root         (0)     5113 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/luminesce_view_response.py
+-rw-r--r--   0 root         (0) root         (0)     9530 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10695 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     7519 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/paged_resource_list_of_event_handler.py
+-rw-r--r--   0 root         (0) root         (0)     7295 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/paged_resource_list_of_task.py
+-rw-r--r--   0 root         (0) root         (0)     7575 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/paged_resource_list_of_task_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/paged_resource_list_of_worker.py
+-rw-r--r--   0 root         (0) root         (0)     9076 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/parameter.py
+-rw-r--r--   0 root         (0) root         (0)     5767 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/parameter_value.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7735 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7175 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/resource_list_of_task.py
+-rw-r--r--   0 root         (0) root         (0)     7211 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/result_field.py
+-rw-r--r--   0 root         (0) root         (0)     4985 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/result_matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    11562 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/resultant_child_task_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    10386 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/run_worker_action.py
+-rw-r--r--   0 root         (0) root         (0)    10247 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/run_worker_action_response.py
+-rw-r--r--   0 root         (0) root         (0)     4435 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/run_worker_request.py
+-rw-r--r--   0 root         (0) root         (0)     5179 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/run_worker_response.py
+-rw-r--r--   0 root         (0) root         (0)     5383 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/scheduler_job.py
+-rw-r--r--   0 root         (0) root         (0)     5119 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/scheduler_job_response.py
+-rw-r--r--   0 root         (0) root         (0)     4377 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/sleep.py
+-rw-r--r--   0 root         (0) root         (0)     4441 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/sleep_response.py
+-rw-r--r--   0 root         (0) root         (0)    11504 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/stack.py
+-rw-r--r--   0 root         (0) root         (0)    19688 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/task.py
+-rw-r--r--   0 root         (0) root         (0)    14093 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/task_definition.py
+-rw-r--r--   0 root         (0) root         (0)     4386 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/task_definition_version.py
+-rw-r--r--   0 root         (0) root         (0)     6387 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/task_field_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5243 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/task_instance_field.py
+-rw-r--r--   0 root         (0) root         (0)     4944 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/task_state_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9826 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/task_summary.py
+-rw-r--r--   0 root         (0) root         (0)    12376 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/task_transition_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6067 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/transition_trigger_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6451 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/trigger_parent_task_action.py
+-rw-r--r--   0 root         (0) root         (0)     5348 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/trigger_parent_task_action_response.py
+-rw-r--r--   0 root         (0) root         (0)     4440 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/trigger_schema.py
+-rw-r--r--   0 root         (0) root         (0)    13293 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/update_event_handler_request.py
+-rw-r--r--   0 root         (0) root         (0)    12546 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/update_task_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     6427 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/update_task_request.py
+-rw-r--r--   0 root         (0) root         (0)     8188 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/update_worker_request.py
+-rw-r--r--   0 root         (0) root         (0)    11105 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/version_info.py
+-rw-r--r--   0 root         (0) root         (0)    11171 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/worker.py
+-rw-r--r--   0 root         (0) root         (0)     8585 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/worker_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     7048 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/worker_configuration_response.py
+-rw-r--r--   0 root         (0) root         (0)     8967 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/worker_status_triggers.py
+-rw-r--r--   0 root         (0) root         (0)    13551 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:00:13.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/utilities/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:00:13.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2024-05-03 16:00:13.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4269 2024-05-03 16:00:13.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 16:00:13.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2024-05-03 16:00:13.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-03 16:00:13.000000 lusid-workflow-sdk-preview-0.1.974/lusid_workflow_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 16:00:13.000000 lusid-workflow-sdk-preview-0.1.974/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2237 2024-05-03 15:59:39.000000 lusid-workflow-sdk-preview-0.1.974/setup.py
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/README.md` & `lusid-workflow-sdk-preview-0.1.974/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-workflow-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.973
-- Package version: 0.1.973
+- API version: 0.1.974
+- Package version: 0.1.974
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -88,14 +88,19 @@
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://www.lusid.com/workflow*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | [EXPERIMENTAL] ListAccessControlledResources: Get resources available for access control
+*EventHandlersApi* | [**create_event_handler**](docs/EventHandlersApi.md#create_event_handler) | **POST** /api/eventhandlers | [EXPERIMENTAL] CreateEventHandler: Create a new Event Handler
+*EventHandlersApi* | [**delete_event_handler**](docs/EventHandlersApi.md#delete_event_handler) | **DELETE** /api/eventhandlers/{scope}/{code} | [EXPERIMENTAL] DeleteEventHandler: Delete an Event Handler
+*EventHandlersApi* | [**get_event_handler**](docs/EventHandlersApi.md#get_event_handler) | **GET** /api/eventhandlers/{scope}/{code} | [EXPERIMENTAL] GetEventHandler: Get an Event Handler
+*EventHandlersApi* | [**list_event_handlers**](docs/EventHandlersApi.md#list_event_handlers) | **GET** /api/eventhandlers | [EXPERIMENTAL] ListEventHandlers: List Event Handlers
+*EventHandlersApi* | [**update_event_handler**](docs/EventHandlersApi.md#update_event_handler) | **PUT** /api/eventhandlers/{scope}/{code} | [EXPERIMENTAL] UpdateEventHandler: Update an existing Task Definition
 *TaskDefinitionsApi* | [**create_task_definition**](docs/TaskDefinitionsApi.md#create_task_definition) | **POST** /api/taskdefinitions | [EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition
 *TaskDefinitionsApi* | [**delete_task_definition**](docs/TaskDefinitionsApi.md#delete_task_definition) | **DELETE** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] DeleteTaskDefinition: Delete a Task Definition
 *TaskDefinitionsApi* | [**get_task_definition**](docs/TaskDefinitionsApi.md#get_task_definition) | **GET** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] GetTaskDefinition: Get a Task Definition
 *TaskDefinitionsApi* | [**list_task_definitions**](docs/TaskDefinitionsApi.md#list_task_definitions) | **GET** /api/taskdefinitions | [EXPERIMENTAL] ListTaskDefinitions: List Task Definitions
 *TaskDefinitionsApi* | [**list_tasks_for_task_definition**](docs/TaskDefinitionsApi.md#list_tasks_for_task_definition) | **GET** /api/taskdefinitions/{scope}/{code}/tasks | [EXPERIMENTAL] ListTasksForTaskDefinition: List Tasks for a Task Definition
 *TaskDefinitionsApi* | [**update_task_definition**](docs/TaskDefinitionsApi.md#update_task_definition) | **PUT** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] UpdateTaskDefinition: Update an existing Task Definition
 *TasksApi* | [**create_task**](docs/TasksApi.md#create_task) | **POST** /api/tasks | [EXPERIMENTAL] CreateTask: Create a new Task
@@ -120,32 +125,37 @@
  - [ActionDefinitionResponse](docs/ActionDefinitionResponse.md)
  - [ActionDetails](docs/ActionDetails.md)
  - [ActionDetailsResponse](docs/ActionDetailsResponse.md)
  - [ActionId](docs/ActionId.md)
  - [CreateChildTaskConfiguration](docs/CreateChildTaskConfiguration.md)
  - [CreateChildTasksAction](docs/CreateChildTasksAction.md)
  - [CreateChildTasksActionResponse](docs/CreateChildTasksActionResponse.md)
+ - [CreateEventHandlerRequest](docs/CreateEventHandlerRequest.md)
  - [CreateTaskDefinitionRequest](docs/CreateTaskDefinitionRequest.md)
  - [CreateTaskRequest](docs/CreateTaskRequest.md)
  - [CreateWorkerRequest](docs/CreateWorkerRequest.md)
  - [DeletedEntityResponse](docs/DeletedEntityResponse.md)
+ - [EventHandler](docs/EventHandler.md)
+ - [EventHandlerMapping](docs/EventHandlerMapping.md)
+ - [EventMatchingPattern](docs/EventMatchingPattern.md)
  - [Fail](docs/Fail.md)
  - [FailResponse](docs/FailResponse.md)
  - [FieldMapping](docs/FieldMapping.md)
  - [GetWorkerResultResponse](docs/GetWorkerResultResponse.md)
  - [HealthCheck](docs/HealthCheck.md)
  - [HealthCheckResponse](docs/HealthCheckResponse.md)
  - [IdSelectorDefinition](docs/IdSelectorDefinition.md)
  - [IdentifierPartSchema](docs/IdentifierPartSchema.md)
  - [InitialState](docs/InitialState.md)
  - [Link](docs/Link.md)
  - [LuminesceView](docs/LuminesceView.md)
  - [LuminesceViewResponse](docs/LuminesceViewResponse.md)
  - [LusidProblemDetails](docs/LusidProblemDetails.md)
  - [LusidValidationProblemDetails](docs/LusidValidationProblemDetails.md)
+ - [PagedResourceListOfEventHandler](docs/PagedResourceListOfEventHandler.md)
  - [PagedResourceListOfTask](docs/PagedResourceListOfTask.md)
  - [PagedResourceListOfTaskDefinition](docs/PagedResourceListOfTaskDefinition.md)
  - [PagedResourceListOfWorker](docs/PagedResourceListOfWorker.md)
  - [Parameter](docs/Parameter.md)
  - [ParameterValue](docs/ParameterValue.md)
  - [ResourceId](docs/ResourceId.md)
  - [ResourceListOfAccessControlledResource](docs/ResourceListOfAccessControlledResource.md)
@@ -170,14 +180,15 @@
  - [TaskStateDefinition](docs/TaskStateDefinition.md)
  - [TaskSummary](docs/TaskSummary.md)
  - [TaskTransitionDefinition](docs/TaskTransitionDefinition.md)
  - [TransitionTriggerDefinition](docs/TransitionTriggerDefinition.md)
  - [TriggerParentTaskAction](docs/TriggerParentTaskAction.md)
  - [TriggerParentTaskActionResponse](docs/TriggerParentTaskActionResponse.md)
  - [TriggerSchema](docs/TriggerSchema.md)
+ - [UpdateEventHandlerRequest](docs/UpdateEventHandlerRequest.md)
  - [UpdateTaskDefinitionRequest](docs/UpdateTaskDefinitionRequest.md)
  - [UpdateTaskRequest](docs/UpdateTaskRequest.md)
  - [UpdateWorkerRequest](docs/UpdateWorkerRequest.md)
  - [VersionInfo](docs/VersionInfo.md)
  - [Worker](docs/Worker.md)
  - [WorkerConfiguration](docs/WorkerConfiguration.md)
  - [WorkerConfigurationResponse](docs/WorkerConfigurationResponse.md)
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/__init__.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,69 +1,57 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.973"
-
-# import apis into sdk package
-from lusid_workflow.api.application_metadata_api import ApplicationMetadataApi
-from lusid_workflow.api.task_definitions_api import TaskDefinitionsApi
-from lusid_workflow.api.tasks_api import TasksApi
-from lusid_workflow.api.workers_api import WorkersApi
-
-# import ApiClient
-from lusid_workflow.api_client import ApiClient
-from lusid_workflow.configuration import Configuration
-from lusid_workflow.exceptions import OpenApiException
-from lusid_workflow.exceptions import ApiTypeError
-from lusid_workflow.exceptions import ApiValueError
-from lusid_workflow.exceptions import ApiKeyError
-from lusid_workflow.exceptions import ApiException
-# import models into sdk package
+# import models into model package
 from lusid_workflow.models.access_controlled_action import AccessControlledAction
 from lusid_workflow.models.access_controlled_resource import AccessControlledResource
 from lusid_workflow.models.action_definition import ActionDefinition
 from lusid_workflow.models.action_definition_response import ActionDefinitionResponse
 from lusid_workflow.models.action_details import ActionDetails
 from lusid_workflow.models.action_details_response import ActionDetailsResponse
 from lusid_workflow.models.action_id import ActionId
 from lusid_workflow.models.create_child_task_configuration import CreateChildTaskConfiguration
 from lusid_workflow.models.create_child_tasks_action import CreateChildTasksAction
 from lusid_workflow.models.create_child_tasks_action_response import CreateChildTasksActionResponse
+from lusid_workflow.models.create_event_handler_request import CreateEventHandlerRequest
 from lusid_workflow.models.create_task_definition_request import CreateTaskDefinitionRequest
 from lusid_workflow.models.create_task_request import CreateTaskRequest
 from lusid_workflow.models.create_worker_request import CreateWorkerRequest
 from lusid_workflow.models.deleted_entity_response import DeletedEntityResponse
+from lusid_workflow.models.event_handler import EventHandler
+from lusid_workflow.models.event_handler_mapping import EventHandlerMapping
+from lusid_workflow.models.event_matching_pattern import EventMatchingPattern
 from lusid_workflow.models.fail import Fail
 from lusid_workflow.models.fail_response import FailResponse
 from lusid_workflow.models.field_mapping import FieldMapping
 from lusid_workflow.models.get_worker_result_response import GetWorkerResultResponse
 from lusid_workflow.models.health_check import HealthCheck
 from lusid_workflow.models.health_check_response import HealthCheckResponse
 from lusid_workflow.models.id_selector_definition import IdSelectorDefinition
 from lusid_workflow.models.identifier_part_schema import IdentifierPartSchema
 from lusid_workflow.models.initial_state import InitialState
 from lusid_workflow.models.link import Link
 from lusid_workflow.models.luminesce_view import LuminesceView
 from lusid_workflow.models.luminesce_view_response import LuminesceViewResponse
 from lusid_workflow.models.lusid_problem_details import LusidProblemDetails
 from lusid_workflow.models.lusid_validation_problem_details import LusidValidationProblemDetails
+from lusid_workflow.models.paged_resource_list_of_event_handler import PagedResourceListOfEventHandler
 from lusid_workflow.models.paged_resource_list_of_task import PagedResourceListOfTask
 from lusid_workflow.models.paged_resource_list_of_task_definition import PagedResourceListOfTaskDefinition
 from lusid_workflow.models.paged_resource_list_of_worker import PagedResourceListOfWorker
 from lusid_workflow.models.parameter import Parameter
 from lusid_workflow.models.parameter_value import ParameterValue
 from lusid_workflow.models.resource_id import ResourceId
 from lusid_workflow.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
@@ -88,24 +76,16 @@
 from lusid_workflow.models.task_state_definition import TaskStateDefinition
 from lusid_workflow.models.task_summary import TaskSummary
 from lusid_workflow.models.task_transition_definition import TaskTransitionDefinition
 from lusid_workflow.models.transition_trigger_definition import TransitionTriggerDefinition
 from lusid_workflow.models.trigger_parent_task_action import TriggerParentTaskAction
 from lusid_workflow.models.trigger_parent_task_action_response import TriggerParentTaskActionResponse
 from lusid_workflow.models.trigger_schema import TriggerSchema
+from lusid_workflow.models.update_event_handler_request import UpdateEventHandlerRequest
 from lusid_workflow.models.update_task_definition_request import UpdateTaskDefinitionRequest
 from lusid_workflow.models.update_task_request import UpdateTaskRequest
 from lusid_workflow.models.update_worker_request import UpdateWorkerRequest
 from lusid_workflow.models.version_info import VersionInfo
 from lusid_workflow.models.worker import Worker
 from lusid_workflow.models.worker_configuration import WorkerConfiguration
 from lusid_workflow.models.worker_configuration_response import WorkerConfigurationResponse
 from lusid_workflow.models.worker_status_triggers import WorkerStatusTriggers
-
-# import utilities into sdk package
-from fbnsdkutilities.utilities.api_client_builder import ApiClientBuilder
-from fbnsdkutilities.utilities.api_configuration import ApiConfiguration
-from fbnsdkutilities.utilities.api_configuration_loader import ApiConfigurationLoader
-from fbnsdkutilities.utilities.refreshing_token import RefreshingToken
-
-# import tcp utilities
-from fbnsdkutilities.tcp.tcp_keep_alive_probes import TCPKeepAlivePoolManager, TCPKeepAliveProxyManager
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api/application_metadata_api.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/api/application_metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.973'
+        header_params['X-LUSID-SDK-Version'] = '0.1.974'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api/task_definitions_api.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/api/task_definitions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -159,15 +159,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.973'
+        header_params['X-LUSID-SDK-Version'] = '0.1.974'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "TaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -328,15 +328,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.973'
+        header_params['X-LUSID-SDK-Version'] = '0.1.974'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -505,15 +505,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.973'
+        header_params['X-LUSID-SDK-Version'] = '0.1.974'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "TaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -681,15 +681,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.973'
+        header_params['X-LUSID-SDK-Version'] = '0.1.974'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfTaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -858,15 +858,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.973'
+        header_params['X-LUSID-SDK-Version'] = '0.1.974'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfTask",
             400: "LusidValidationProblemDetails",
@@ -1042,15 +1042,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.973'
+        header_params['X-LUSID-SDK-Version'] = '0.1.974'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "TaskDefinition",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api/tasks_api.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/api/tasks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -173,15 +173,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.973'
+        header_params['X-LUSID-SDK-Version'] = '0.1.974'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Task",
             400: "LusidValidationProblemDetails",
@@ -323,15 +323,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.973'
+        header_params['X-LUSID-SDK-Version'] = '0.1.974'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -481,15 +481,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.973'
+        header_params['X-LUSID-SDK-Version'] = '0.1.974'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Task",
             400: "LusidValidationProblemDetails",
@@ -657,15 +657,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.973'
+        header_params['X-LUSID-SDK-Version'] = '0.1.974'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfTask",
             400: "LusidValidationProblemDetails",
@@ -833,15 +833,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.973'
+        header_params['X-LUSID-SDK-Version'] = '0.1.974'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Task",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api/workers_api.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/api/workers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -163,15 +163,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.973'
+        header_params['X-LUSID-SDK-Version'] = '0.1.974'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Worker",
             400: "LusidValidationProblemDetails",
@@ -334,15 +334,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.973'
+        header_params['X-LUSID-SDK-Version'] = '0.1.974'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -513,15 +513,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.973'
+        header_params['X-LUSID-SDK-Version'] = '0.1.974'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Worker",
             400: "LusidValidationProblemDetails",
@@ -655,15 +655,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.973'
+        header_params['X-LUSID-SDK-Version'] = '0.1.974'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "GetWorkerResultResponse",
             400: "LusidValidationProblemDetails",
@@ -815,15 +815,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.973'
+        header_params['X-LUSID-SDK-Version'] = '0.1.974'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfWorker",
             400: "LusidValidationProblemDetails",
@@ -1005,15 +1005,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.973'
+        header_params['X-LUSID-SDK-Version'] = '0.1.974'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "RunWorkerResponse",
             400: "LusidValidationProblemDetails",
@@ -1190,15 +1190,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.973'
+        header_params['X-LUSID-SDK-Version'] = '0.1.974'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Worker",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api_client.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.973/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.974/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/configuration.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.973\n"\
-               "SDK Package Version: 0.1.973".\
+               "Version of the API: 0.1.974\n"\
+               "SDK Package Version: 0.1.974".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/exceptions.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/__init__.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,75 @@
 # coding: utf-8
 
 # flake8: noqa
+
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-# import models into model package
+__version__ = "0.1.974"
+
+# import apis into sdk package
+from lusid_workflow.api.application_metadata_api import ApplicationMetadataApi
+from lusid_workflow.api.event_handlers_api import EventHandlersApi
+from lusid_workflow.api.task_definitions_api import TaskDefinitionsApi
+from lusid_workflow.api.tasks_api import TasksApi
+from lusid_workflow.api.workers_api import WorkersApi
+
+# import ApiClient
+from lusid_workflow.api_client import ApiClient
+from lusid_workflow.configuration import Configuration
+from lusid_workflow.exceptions import OpenApiException
+from lusid_workflow.exceptions import ApiTypeError
+from lusid_workflow.exceptions import ApiValueError
+from lusid_workflow.exceptions import ApiKeyError
+from lusid_workflow.exceptions import ApiException
+# import models into sdk package
 from lusid_workflow.models.access_controlled_action import AccessControlledAction
 from lusid_workflow.models.access_controlled_resource import AccessControlledResource
 from lusid_workflow.models.action_definition import ActionDefinition
 from lusid_workflow.models.action_definition_response import ActionDefinitionResponse
 from lusid_workflow.models.action_details import ActionDetails
 from lusid_workflow.models.action_details_response import ActionDetailsResponse
 from lusid_workflow.models.action_id import ActionId
 from lusid_workflow.models.create_child_task_configuration import CreateChildTaskConfiguration
 from lusid_workflow.models.create_child_tasks_action import CreateChildTasksAction
 from lusid_workflow.models.create_child_tasks_action_response import CreateChildTasksActionResponse
+from lusid_workflow.models.create_event_handler_request import CreateEventHandlerRequest
 from lusid_workflow.models.create_task_definition_request import CreateTaskDefinitionRequest
 from lusid_workflow.models.create_task_request import CreateTaskRequest
 from lusid_workflow.models.create_worker_request import CreateWorkerRequest
 from lusid_workflow.models.deleted_entity_response import DeletedEntityResponse
+from lusid_workflow.models.event_handler import EventHandler
+from lusid_workflow.models.event_handler_mapping import EventHandlerMapping
+from lusid_workflow.models.event_matching_pattern import EventMatchingPattern
 from lusid_workflow.models.fail import Fail
 from lusid_workflow.models.fail_response import FailResponse
 from lusid_workflow.models.field_mapping import FieldMapping
 from lusid_workflow.models.get_worker_result_response import GetWorkerResultResponse
 from lusid_workflow.models.health_check import HealthCheck
 from lusid_workflow.models.health_check_response import HealthCheckResponse
 from lusid_workflow.models.id_selector_definition import IdSelectorDefinition
 from lusid_workflow.models.identifier_part_schema import IdentifierPartSchema
 from lusid_workflow.models.initial_state import InitialState
 from lusid_workflow.models.link import Link
 from lusid_workflow.models.luminesce_view import LuminesceView
 from lusid_workflow.models.luminesce_view_response import LuminesceViewResponse
 from lusid_workflow.models.lusid_problem_details import LusidProblemDetails
 from lusid_workflow.models.lusid_validation_problem_details import LusidValidationProblemDetails
+from lusid_workflow.models.paged_resource_list_of_event_handler import PagedResourceListOfEventHandler
 from lusid_workflow.models.paged_resource_list_of_task import PagedResourceListOfTask
 from lusid_workflow.models.paged_resource_list_of_task_definition import PagedResourceListOfTaskDefinition
 from lusid_workflow.models.paged_resource_list_of_worker import PagedResourceListOfWorker
 from lusid_workflow.models.parameter import Parameter
 from lusid_workflow.models.parameter_value import ParameterValue
 from lusid_workflow.models.resource_id import ResourceId
 from lusid_workflow.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
@@ -71,15 +94,25 @@
 from lusid_workflow.models.task_state_definition import TaskStateDefinition
 from lusid_workflow.models.task_summary import TaskSummary
 from lusid_workflow.models.task_transition_definition import TaskTransitionDefinition
 from lusid_workflow.models.transition_trigger_definition import TransitionTriggerDefinition
 from lusid_workflow.models.trigger_parent_task_action import TriggerParentTaskAction
 from lusid_workflow.models.trigger_parent_task_action_response import TriggerParentTaskActionResponse
 from lusid_workflow.models.trigger_schema import TriggerSchema
+from lusid_workflow.models.update_event_handler_request import UpdateEventHandlerRequest
 from lusid_workflow.models.update_task_definition_request import UpdateTaskDefinitionRequest
 from lusid_workflow.models.update_task_request import UpdateTaskRequest
 from lusid_workflow.models.update_worker_request import UpdateWorkerRequest
 from lusid_workflow.models.version_info import VersionInfo
 from lusid_workflow.models.worker import Worker
 from lusid_workflow.models.worker_configuration import WorkerConfiguration
 from lusid_workflow.models.worker_configuration_response import WorkerConfigurationResponse
 from lusid_workflow.models.worker_status_triggers import WorkerStatusTriggers
+
+# import utilities into sdk package
+from fbnsdkutilities.utilities.api_client_builder import ApiClientBuilder
+from fbnsdkutilities.utilities.api_configuration import ApiConfiguration
+from fbnsdkutilities.utilities.api_configuration_loader import ApiConfigurationLoader
+from fbnsdkutilities.utilities.refreshing_token import RefreshingToken
+
+# import tcp utilities
+from fbnsdkutilities.tcp.tcp_keep_alive_probes import TCPKeepAlivePoolManager, TCPKeepAliveProxyManager
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/access_controlled_action.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/access_controlled_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/access_controlled_resource.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/action_definition.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/action_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/action_definition_response.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/action_definition_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/action_details.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/action_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/action_details_response.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/action_details_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/action_id.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/action_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_child_task_configuration.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/create_child_task_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_child_tasks_action.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/create_child_tasks_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_child_tasks_action_response.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/create_child_tasks_action_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_task_definition_request.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/create_task_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_task_request.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/create_task_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_worker_request.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/create_worker_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/deleted_entity_response.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/deleted_entity_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/fail.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/fail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/fail_response.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/fail_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/field_mapping.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/field_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/get_worker_result_response.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/get_worker_result_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/health_check.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/health_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/health_check_response.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/health_check_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/id_selector_definition.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/id_selector_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/identifier_part_schema.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/identifier_part_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/initial_state.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/initial_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/link.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/luminesce_view.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/luminesce_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/luminesce_view_response.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/luminesce_view_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/lusid_problem_details.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/lusid_validation_problem_details.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/paged_resource_list_of_task.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/paged_resource_list_of_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/paged_resource_list_of_task_definition.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/paged_resource_list_of_task_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/paged_resource_list_of_worker.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/paged_resource_list_of_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/parameter.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/parameter_value.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/parameter_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/resource_id.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/resource_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/resource_list_of_access_controlled_resource.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/resource_list_of_access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/resource_list_of_task.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/resource_list_of_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/result_field.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/result_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/result_matching_pattern.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/result_matching_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/resultant_child_task_configuration.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/resultant_child_task_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/run_worker_action.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/run_worker_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/run_worker_action_response.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/run_worker_action_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/run_worker_request.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/run_worker_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/run_worker_response.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/run_worker_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/scheduler_job.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/scheduler_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/scheduler_job_response.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/scheduler_job_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/sleep.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/sleep.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/sleep_response.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/sleep_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/stack.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_definition.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/task_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_definition_version.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/task_definition_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_field_definition.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/task_field_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_instance_field.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/task_instance_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_state_definition.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/task_state_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_summary.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/task_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_transition_definition.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/task_transition_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/transition_trigger_definition.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/transition_trigger_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/trigger_parent_task_action.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/trigger_parent_task_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/trigger_parent_task_action_response.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/trigger_parent_task_action_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/trigger_schema.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/trigger_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/update_task_definition_request.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/update_task_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/update_task_request.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/update_task_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/update_worker_request.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/update_worker_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/version_info.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/version_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/worker.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/worker_configuration.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/worker_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/worker_configuration_response.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/worker_configuration_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/worker_status_triggers.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/models/worker_status_triggers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/rest.py` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.973
+    The version of the OpenAPI document: 0.1.974
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/utilities/config_keys.json` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-workflow-sdk-preview-0.1.973/lusid_workflow_sdk_preview.egg-info/SOURCES.txt` & `lusid-workflow-sdk-preview-0.1.974/lusid_workflow_sdk_preview.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,46 +5,52 @@
 lusid_workflow/__version__.py
 lusid_workflow/api_client.py
 lusid_workflow/configuration.py
 lusid_workflow/exceptions.py
 lusid_workflow/rest.py
 lusid_workflow/api/__init__.py
 lusid_workflow/api/application_metadata_api.py
+lusid_workflow/api/event_handlers_api.py
 lusid_workflow/api/task_definitions_api.py
 lusid_workflow/api/tasks_api.py
 lusid_workflow/api/workers_api.py
 lusid_workflow/models/__init__.py
 lusid_workflow/models/access_controlled_action.py
 lusid_workflow/models/access_controlled_resource.py
 lusid_workflow/models/action_definition.py
 lusid_workflow/models/action_definition_response.py
 lusid_workflow/models/action_details.py
 lusid_workflow/models/action_details_response.py
 lusid_workflow/models/action_id.py
 lusid_workflow/models/create_child_task_configuration.py
 lusid_workflow/models/create_child_tasks_action.py
 lusid_workflow/models/create_child_tasks_action_response.py
+lusid_workflow/models/create_event_handler_request.py
 lusid_workflow/models/create_task_definition_request.py
 lusid_workflow/models/create_task_request.py
 lusid_workflow/models/create_worker_request.py
 lusid_workflow/models/deleted_entity_response.py
+lusid_workflow/models/event_handler.py
+lusid_workflow/models/event_handler_mapping.py
+lusid_workflow/models/event_matching_pattern.py
 lusid_workflow/models/fail.py
 lusid_workflow/models/fail_response.py
 lusid_workflow/models/field_mapping.py
 lusid_workflow/models/get_worker_result_response.py
 lusid_workflow/models/health_check.py
 lusid_workflow/models/health_check_response.py
 lusid_workflow/models/id_selector_definition.py
 lusid_workflow/models/identifier_part_schema.py
 lusid_workflow/models/initial_state.py
 lusid_workflow/models/link.py
 lusid_workflow/models/luminesce_view.py
 lusid_workflow/models/luminesce_view_response.py
 lusid_workflow/models/lusid_problem_details.py
 lusid_workflow/models/lusid_validation_problem_details.py
+lusid_workflow/models/paged_resource_list_of_event_handler.py
 lusid_workflow/models/paged_resource_list_of_task.py
 lusid_workflow/models/paged_resource_list_of_task_definition.py
 lusid_workflow/models/paged_resource_list_of_worker.py
 lusid_workflow/models/parameter.py
 lusid_workflow/models/parameter_value.py
 lusid_workflow/models/resource_id.py
 lusid_workflow/models/resource_list_of_access_controlled_resource.py
@@ -69,14 +75,15 @@
 lusid_workflow/models/task_state_definition.py
 lusid_workflow/models/task_summary.py
 lusid_workflow/models/task_transition_definition.py
 lusid_workflow/models/transition_trigger_definition.py
 lusid_workflow/models/trigger_parent_task_action.py
 lusid_workflow/models/trigger_parent_task_action_response.py
 lusid_workflow/models/trigger_schema.py
+lusid_workflow/models/update_event_handler_request.py
 lusid_workflow/models/update_task_definition_request.py
 lusid_workflow/models/update_task_request.py
 lusid_workflow/models/update_worker_request.py
 lusid_workflow/models/version_info.py
 lusid_workflow/models/worker.py
 lusid_workflow/models/worker_configuration.py
 lusid_workflow/models/worker_configuration_response.py
```

### Comparing `lusid-workflow-sdk-preview-0.1.973/setup.py` & `lusid-workflow-sdk-preview-0.1.974/setup.py`

 * *Files identical despite different names*


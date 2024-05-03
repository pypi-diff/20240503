# Comparing `tmp/forloop_modules-1.0.2.tar.gz` & `tmp/forloop_modules-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forloop_modules-1.0.2.tar", last modified: Thu Apr 18 13:46:39 2024, max compression
+gzip compressed data, was "forloop_modules-1.1.0.tar", last modified: Fri May  3 13:08:48 2024, max compression
```

## Comparing `forloop_modules-1.0.2.tar` & `forloop_modules-1.1.0.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.487948 forloop_modules-1.0.2/
--rw-rw-rw-   0        0        0     1525 2024-02-22 17:34:45.000000 forloop_modules-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      658 2024-04-18 13:46:39.487948 forloop_modules-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      155 2024-02-22 17:34:45.000000 forloop_modules-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.095402 forloop_modules-1.0.2/forloop_modules/
--rw-rw-rw-   0        0        0      179 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.128244 forloop_modules-1.0.2/forloop_modules/errors/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/errors/__init__.py
--rw-rw-rw-   0        0        0     1670 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/errors/errors.py
--rw-rw-rw-   0        0        0     9860 2024-03-12 11:46:28.000000 forloop_modules-1.0.2/forloop_modules/flog.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.237142 forloop_modules-1.0.2/forloop_modules/function_handlers/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/__init__.py
--rw-rw-rw-   0        0        0     6781 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/api_endpoint_handlers.py
--rw-rw-rw-   0        0        0    22200 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/api_handlers.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.286309 forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/__init__.py
--rw-rw-rw-   0        0        0    17835 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py
--rw-rw-rw-   0        0        0      807 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py
--rw-rw-rw-   0        0        0     2061 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/data_types_validation.py
--rw-rw-rw-   0        0        0     1047 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/docs.py
--rw-rw-rw-   0        0        0     1940 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py
--rw-rw-rw-   0        0        0     7504 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/form_dict_list.py
--rw-rw-rw-   0        0        0     2169 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py
--rw-rw-rw-   0        0        0    22515 2024-04-18 13:45:44.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/browser_handlers.py
--rw-rw-rw-   0        0        0   204411 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/cleaning_handlers.py
--rw-rw-rw-   0        0        0    12258 2024-03-21 12:02:54.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/control_flow_handlers.py
--rw-rw-rw-   0        0        0    46277 2024-03-21 12:02:54.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/data_handlers.py
--rw-rw-rw-   0        0        0    72995 2024-04-08 16:56:40.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/database_handlers.py
--rw-rw-rw-   0        0        0    30031 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/datetime_handlers.py
--rw-rw-rw-   0        0        0    14696 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/file_managment_handlers.py
--rw-rw-rw-   0        0        0    83412 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/integration_handlers.py
--rw-rw-rw-   0        0        0    27439 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/mapping_handlers.py
--rw-rw-rw-   0        0        0    14152 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/model_handlers.py
--rw-rw-rw-   0        0        0     2778 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/orchestration_handlers.py
--rw-rw-rw-   0        0        0    16250 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/rpa_handlers.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.322744 forloop_modules-1.0.2/forloop_modules/function_handlers/transformations/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/transformations/__init__.py
--rw-rw-rw-   0        0        0    14097 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/transformations/basic_transforms.py
--rw-rw-rw-   0        0        0    10448 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/transformations/imputation.py
--rw-rw-rw-   0        0        0     4092 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/transformations/outliers.py
--rw-rw-rw-   0        0        0    58900 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/variable_handlers.py
--rw-rw-rw-   0        0        0   103324 2024-03-12 11:46:28.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/webscraping_handlers.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.369957 forloop_modules-1.0.2/forloop_modules/globals/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/globals/__init__.py
--rw-rw-rw-   0        0        0     5145 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/globals/active_entity_tracker.py
--rw-rw-rw-   0        0        0     1871 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/globals/database_utilities_handler.py
--rw-rw-rw-   0        0        0     5482 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/globals/db_connection.py
--rw-rw-rw-   0        0        0     8030 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/globals/dbtables_loader_popups.py
--rw-rw-rw-   0        0        0      223 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/globals/docs_categories.py
--rw-rw-rw-   0        0        0    17317 2024-03-14 09:29:03.000000 forloop_modules-1.0.2/forloop_modules/globals/local_variable_handler.py
--rw-rw-rw-   0        0        0    32107 2024-04-18 13:45:44.000000 forloop_modules-1.0.2/forloop_modules/globals/scraping_utilities_handler.py
--rw-rw-rw-   0        0        0     9133 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/globals/variable_handler.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.385548 forloop_modules-1.0.2/forloop_modules/integrations/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/integrations/__init__.py
--rw-rw-rw-   0        0        0     2082 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/integrations/slack_integration.py
--rw-rw-rw-   0        0        0     3580 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/integrations/testing_check_slack_notifications.py
--rw-rw-rw-   0        0        0    14244 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/node_detail_form.py
--rw-rw-rw-   0        0        0    10856 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/pipeline_function_handlers.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.408708 forloop_modules-1.0.2/forloop_modules/queries/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/queries/__init__.py
--rw-rw-rw-   0        0        0     2888 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/queries/context_request_backend_auxiliary_functions.py
--rw-rw-rw-   0        0        0    22387 2024-04-08 16:56:40.000000 forloop_modules-1.0.2/forloop_modules/queries/db_model_templates.py
--rw-rw-rw-   0        0        0    41165 2024-03-21 12:02:54.000000 forloop_modules-1.0.2/forloop_modules/queries/node_context_requests_backend.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.414719 forloop_modules-1.0.2/forloop_modules/redis/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/redis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.421414 forloop_modules-1.0.2/forloop_modules/redis/config/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/redis/config/__init__.py
--rw-rw-rw-   0        0        0     2108 2024-04-08 16:56:40.000000 forloop_modules-1.0.2/forloop_modules/redis/config/config.py
--rw-rw-rw-   0        0        0     6223 2024-04-08 16:56:40.000000 forloop_modules-1.0.2/forloop_modules/redis/redis_connection.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.480239 forloop_modules-1.0.2/forloop_modules/utils/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/utils/__init__.py
--rw-rw-rw-   0        0        0     5587 2024-04-08 16:56:40.000000 forloop_modules-1.0.2/forloop_modules/utils/definitions.py
--rw-rw-rw-   0        0        0     1024 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/utils/encryption.py
--rw-rw-rw-   0        0        0     3393 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/utils/pandas_operations.py
--rw-rw-rw-   0        0        0     3545 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/utils/pickle_serializer.py
--rw-rw-rw-   0        0        0     3190 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/utils/script_utils.py
--rw-rw-rw-   0        0        0     1622 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/utils/str_helpers.py
--rw-rw-rw-   0        0        0      856 2024-04-08 16:56:40.000000 forloop_modules-1.0.2/forloop_modules/utils/synchronization_flags.py
--rw-rw-rw-   0        0        0     4570 2024-04-08 16:56:40.000000 forloop_modules-1.0.2/forloop_modules/utils/url_template_builder.py
--rw-rw-rw-   0        0        0     3558 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/utils/various.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.119575 forloop_modules-1.0.2/forloop_modules.egg-info/
--rw-rw-rw-   0        0        0      658 2024-04-18 13:46:38.000000 forloop_modules-1.0.2/forloop_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3493 2024-04-18 13:46:39.000000 forloop_modules-1.0.2/forloop_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 13:46:38.000000 forloop_modules-1.0.2/forloop_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-18 13:46:38.000000 forloop_modules-1.0.2/forloop_modules.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 13:46:39.487948 forloop_modules-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      786 2024-04-18 13:46:17.000000 forloop_modules-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.486697 forloop_modules-1.0.2/tests/
--rw-rw-rw-   0        0        0        0 2024-02-22 17:34:45.000000 forloop_modules-1.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0     3316 2024-04-08 16:56:40.000000 forloop_modules-1.0.2/tests/test_url_template_builder.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:08:48.545177 forloop_modules-1.1.0/
+-rw-rw-rw-   0        0        0     1525 2024-02-22 17:34:45.000000 forloop_modules-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      658 2024-05-03 13:08:48.544177 forloop_modules-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2024-02-22 17:34:45.000000 forloop_modules-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 13:08:48.453185 forloop_modules-1.1.0/forloop_modules/
+-rw-rw-rw-   0        0        0      179 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:08:48.467197 forloop_modules-1.1.0/forloop_modules/errors/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/errors/__init__.py
+-rw-rw-rw-   0        0        0     1670 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/errors/errors.py
+-rw-rw-rw-   0        0        0     9860 2024-03-12 11:46:28.000000 forloop_modules-1.1.0/forloop_modules/flog.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:08:48.501239 forloop_modules-1.1.0/forloop_modules/function_handlers/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/__init__.py
+-rw-rw-rw-   0        0        0     6781 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/api_endpoint_handlers.py
+-rw-rw-rw-   0        0        0    22200 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/api_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:08:48.516643 forloop_modules-1.1.0/forloop_modules/function_handlers/auxilliary/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/auxilliary/__init__.py
+-rw-rw-rw-   0        0        0    17835 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py
+-rw-rw-rw-   0        0        0      807 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py
+-rw-rw-rw-   0        0        0     2061 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/auxilliary/data_types_validation.py
+-rw-rw-rw-   0        0        0     1047 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/auxilliary/docs.py
+-rw-rw-rw-   0        0        0     1940 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py
+-rw-rw-rw-   0        0        0     7933 2024-05-03 13:07:28.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/auxilliary/form_dict_list.py
+-rw-rw-rw-   0        0        0     2169 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py
+-rw-rw-rw-   0        0        0    25173 2024-05-03 13:07:28.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/browser_handlers.py
+-rw-rw-rw-   0        0        0   204411 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/cleaning_handlers.py
+-rw-rw-rw-   0        0        0    12258 2024-03-21 12:02:54.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/control_flow_handlers.py
+-rw-rw-rw-   0        0        0    46277 2024-03-21 12:02:54.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/data_handlers.py
+-rw-rw-rw-   0        0        0    72995 2024-04-08 16:56:40.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/database_handlers.py
+-rw-rw-rw-   0        0        0    30031 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/datetime_handlers.py
+-rw-rw-rw-   0        0        0    14696 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/file_managment_handlers.py
+-rw-rw-rw-   0        0        0    83412 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/integration_handlers.py
+-rw-rw-rw-   0        0        0    27439 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/mapping_handlers.py
+-rw-rw-rw-   0        0        0    14152 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/model_handlers.py
+-rw-rw-rw-   0        0        0     2778 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/orchestration_handlers.py
+-rw-rw-rw-   0        0        0    16250 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/rpa_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:08:48.519641 forloop_modules-1.1.0/forloop_modules/function_handlers/transformations/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/transformations/__init__.py
+-rw-rw-rw-   0        0        0    14097 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/transformations/basic_transforms.py
+-rw-rw-rw-   0        0        0    10448 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/transformations/imputation.py
+-rw-rw-rw-   0        0        0     4092 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/transformations/outliers.py
+-rw-rw-rw-   0        0        0    58900 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/variable_handlers.py
+-rw-rw-rw-   0        0        0   103383 2024-05-03 13:07:28.000000 forloop_modules-1.1.0/forloop_modules/function_handlers/webscraping_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:08:48.525656 forloop_modules-1.1.0/forloop_modules/globals/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/globals/__init__.py
+-rw-rw-rw-   0        0        0     5162 2024-05-03 13:07:28.000000 forloop_modules-1.1.0/forloop_modules/globals/active_entity_tracker.py
+-rw-rw-rw-   0        0        0     1871 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/globals/database_utilities_handler.py
+-rw-rw-rw-   0        0        0     6522 2024-05-03 13:07:28.000000 forloop_modules-1.1.0/forloop_modules/globals/db_connection.py
+-rw-rw-rw-   0        0        0     8030 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/globals/dbtables_loader_popups.py
+-rw-rw-rw-   0        0        0      223 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/globals/docs_categories.py
+-rw-rw-rw-   0        0        0    19056 2024-05-03 13:07:28.000000 forloop_modules-1.1.0/forloop_modules/globals/local_variable_handler.py
+-rw-rw-rw-   0        0        0    33215 2024-05-03 13:07:28.000000 forloop_modules-1.1.0/forloop_modules/globals/scraping_utilities_handler.py
+-rw-rw-rw-   0        0        0     9133 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/globals/variable_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:08:48.528648 forloop_modules-1.1.0/forloop_modules/integrations/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/integrations/__init__.py
+-rw-rw-rw-   0        0        0     2082 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/integrations/slack_integration.py
+-rw-rw-rw-   0        0        0     3580 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/integrations/testing_check_slack_notifications.py
+-rw-rw-rw-   0        0        0    14244 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/node_detail_form.py
+-rw-rw-rw-   0        0        0    10856 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/pipeline_function_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:08:48.530649 forloop_modules-1.1.0/forloop_modules/queries/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/queries/__init__.py
+-rw-rw-rw-   0        0        0     2888 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/queries/context_request_backend_auxiliary_functions.py
+-rw-rw-rw-   0        0        0    21775 2024-05-03 13:07:28.000000 forloop_modules-1.1.0/forloop_modules/queries/db_model_templates.py
+-rw-rw-rw-   0        0        0    42399 2024-05-03 13:07:28.000000 forloop_modules-1.1.0/forloop_modules/queries/node_context_requests_backend.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:08:48.532648 forloop_modules-1.1.0/forloop_modules/redis/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/redis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:08:48.533648 forloop_modules-1.1.0/forloop_modules/redis/config/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/redis/config/__init__.py
+-rw-rw-rw-   0        0        0     2108 2024-04-08 16:56:40.000000 forloop_modules-1.1.0/forloop_modules/redis/config/config.py
+-rw-rw-rw-   0        0        0     6223 2024-04-08 16:56:40.000000 forloop_modules-1.1.0/forloop_modules/redis/redis_connection.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:08:48.542178 forloop_modules-1.1.0/forloop_modules/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/utils/__init__.py
+-rw-rw-rw-   0        0        0     5587 2024-04-08 16:56:40.000000 forloop_modules-1.1.0/forloop_modules/utils/definitions.py
+-rw-rw-rw-   0        0        0     1024 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/utils/encryption.py
+-rw-rw-rw-   0        0        0     3393 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/utils/pandas_operations.py
+-rw-rw-rw-   0        0        0     3545 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/utils/pickle_serializer.py
+-rw-rw-rw-   0        0        0     3190 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/utils/script_utils.py
+-rw-rw-rw-   0        0        0     2021 2024-05-03 13:07:28.000000 forloop_modules-1.1.0/forloop_modules/utils/sse_parser.py
+-rw-rw-rw-   0        0        0     1622 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/utils/str_helpers.py
+-rw-rw-rw-   0        0        0      856 2024-04-08 16:56:40.000000 forloop_modules-1.1.0/forloop_modules/utils/synchronization_flags.py
+-rw-rw-rw-   0        0        0     4570 2024-04-08 16:56:40.000000 forloop_modules-1.1.0/forloop_modules/utils/url_template_builder.py
+-rw-rw-rw-   0        0        0     3558 2024-02-29 13:17:45.000000 forloop_modules-1.1.0/forloop_modules/utils/various.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:08:48.466199 forloop_modules-1.1.0/forloop_modules.egg-info/
+-rw-rw-rw-   0        0        0      658 2024-05-03 13:08:48.000000 forloop_modules-1.1.0/forloop_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3529 2024-05-03 13:08:48.000000 forloop_modules-1.1.0/forloop_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 13:08:48.000000 forloop_modules-1.1.0/forloop_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-03 13:08:48.000000 forloop_modules-1.1.0/forloop_modules.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 13:08:48.545177 forloop_modules-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      786 2024-05-03 13:07:55.000000 forloop_modules-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:08:48.544177 forloop_modules-1.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-22 17:34:45.000000 forloop_modules-1.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     3316 2024-04-08 16:56:40.000000 forloop_modules-1.1.0/tests/test_url_template_builder.py
```

### Comparing `forloop_modules-1.0.2/LICENSE` & `forloop_modules-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/PKG-INFO` & `forloop_modules-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forloop_modules
-Version: 1.0.2
+Version: 1.1.0
 Summary: This package contains open source modules and integrations within Forloop.ai platform
 Home-page: https://github.com/ForloopAI/forloop_modules
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forloop_modules-1.0.2/forloop_modules/errors/errors.py` & `forloop_modules-1.1.0/forloop_modules/errors/errors.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/flog.py` & `forloop_modules-1.1.0/forloop_modules/flog.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/api_endpoint_handlers.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/api_endpoint_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/api_handlers.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/api_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/data_types_validation.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/auxilliary/data_types_validation.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/docs.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/auxilliary/docs.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/form_dict_list.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/auxilliary/form_dict_list.py`

 * *Files 22% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             text (str): text of the element
             row (int): row number of the element - specified only if it's not first element on the same row
         """
         key = "Label"
         value = text
         self.insert_element_to_form_dict_list(key, value, row)
 
-    def entry(self, name, text, category=None, input_types=None, required=None, type='text', file_types=None, show_info=None, row=None):
+    def entry(self, name, text, category=None, input_types=None, required=None, type='text', file_types=None, show_info=None, desktop_only=False, row=None):
         """
         Entry is a text element with a name and a text
         args:
             name (str): name of the element
             text (str): text of the element
             category (str): category of the element
             input_types (str): input types of the element
@@ -74,93 +74,103 @@
             type (str): One of 'text', 'file', 'password' - changes entry behaviour
             row (int): row number of the element - specified only if it's not first element on the same row
         """
         if file_types is None:
             file_types = [("all files", "*")]
 
         key = "Entry"
-        value = {"name": name, "text": text, "category": category, "input_types": input_types, "required": required, "type": type, "file_types": file_types, "show_info": show_info}
+        value = {
+            "name": name,
+            "text": text,
+            "category": category,
+            "input_types": input_types,
+            "required": required,
+            "type": type,
+            "file_types": file_types,
+            "show_info": show_info,
+            'desktop_only': desktop_only,
+        }
 
         if required:
             if "Label" in self[-1].keys():
                 self[-1]["Label"] = self[-1]["Label"] + "*"
 
         self.insert_element_to_form_dict_list(key, value, row)
 
-    def combobox(self, name, options, multiselect_indices=None, default=None, show_info=None, row=None):
+    def combobox(self, name, options, multiselect_indices=None, default=None, show_info=None, desktop_only=False, row=None):
         """
         Combobox is a dropdown list with options
 
         Args:
             name (str): name of the element
             options (list): list of options
             multiselect_indices (dict, optional): Enables multiselect mode. Defaults to None.
             default (str, optional): Default option. Defaults to None.
             row (int, optional): Row number of the element - specified only if it's not first element on the same row. Defaults to None.
         """
         key = "Combobox"
-        value = {"name": name, "options": options, "default": default, "multiselect_indices": multiselect_indices, "show_info":show_info}
+        value = {"name": name, "options": options, "default": default, "multiselect_indices": multiselect_indices, "show_info":show_info, 'desktop_only': desktop_only}
         self.insert_element_to_form_dict_list(key, value, row)
 
-    def comboentry(self, name, text, options, show_info=None, row=None):
+    def comboentry(self, name, text, options, show_info=None, desktop_only=False, row=None):
         """
         Comboentry is a dropdown list with options and a text field
         
         Args:
             name (str): name of the element
             text (str): text of the element
             options (list): list of options
             row (int): row number of the element - specified only if it's not first element on the same row
         """
         key = "ComboEntry"
-        value = {"name": name, "text": text, "options": options, "show_info": show_info}
+        value = {"name": name, "text": text, "options": options, "show_info": show_info, 'desktop_only': desktop_only}
         self.insert_element_to_form_dict_list(key, value, row)
 
-    def button(self, function, function_args, text, focused: bool = False, enforce_required: bool = None, frontend_implementation=False, name=None, row=None):
+    def button(self, function, function_args, text, focused: bool = False, enforce_required: bool = None, frontend_implementation=False, name=None, desktop_only=False, row=None):
         """
         Button is a button with a function and arguments
 
         Args:
             function (function): function to be called when button is pressed
             function_args (list): list of arguments for the function
             text (str): text of the button
             focused (bool, optional): If True, button will be executed after Enter push. Defaults to False.
             enforce_required (bool, optional): If True, button will check whether compulsory elements are filled. Defaults to True.
             row (int): row number of the element - specified only if it's not first element on the same row
         """    
         key = "Button"
-        value = {"name": name, "function": function, "function_args": function_args, "text": text, "focused": focused, "enforce_required": enforce_required, "frontend_implementation": frontend_implementation}
+        value = {"name": name, "function": function, "function_args": function_args, "text": text, "focused": focused, "enforce_required": enforce_required, "frontend_implementation": frontend_implementation, 'desktop_only': desktop_only}
         self.insert_element_to_form_dict_list(key, value, row)
 
-    def button_image(self, image, x_size, y_size, x_offset, function, function_args=None, row=None):
+    def button_image(self, image, x_size, y_size, x_offset, function, function_args=None, desktop_only=False, row=None):
         """
         Button is an image with or without function and arguments
 
         Args:
             image (str): path to image (relative to src/png)
             function (function): function to be called when button is pressed
             function_args (list): list of arguments for the function
             x_size (int): width of image
             y_size (int): height of the button
             x_offset (int): offset on x-axis
             row (int): row number of the element - specified only if it's not first element on the same row
         """
 
         key = "ButtonImage"
-        value = {"image": image, "function": function, "function_args": function_args, "x_size": x_size, "y_size": y_size, "x_offset": x_offset}
+        value = {"image": image, "function": function, "function_args": function_args, "x_size": x_size, "y_size": y_size, "x_offset": x_offset, 'desktop_only': desktop_only}
         self.insert_element_to_form_dict_list(key, value, row)
 
-    def checkbox(self, name, bool_value: bool = False, row=None):
+    def checkbox(self, name, bool_value: bool = False, desktop_only=False, row=None):
         """
         CheckBox is an element for storing True/False values
 
         Args:
             name (str): name of the element
             bool_value (bool, optional): if True, checkbox is selected. Default False.
             row (int): row number of the element - specified only if it's not first element on the same row
         """
         key = "Checkbox"
-        value = {"name": name, "bool_value": bool_value}
+        value = {"name": name, "bool_value": bool_value, 'desktop_only': desktop_only}
         self.insert_element_to_form_dict_list(key, value, row)
```

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/browser_handlers.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/browser_handlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from io import BytesIO
 import base64
 from pathlib import Path
 from typing import Union
 
 from PIL import Image
 
 import forloop_modules.queries.node_context_requests_backend as ncrb
+from forloop_modules.errors.errors import CriticalPipelineError
 from forloop_modules.flog import flog
 from forloop_modules.function_handlers.auxilliary.abstract_function_handler import (
     AbstractFunctionHandler,
 )
 from forloop_modules.function_handlers.auxilliary.form_dict_list import FormDictList
 from forloop_modules.function_handlers.auxilliary.node_type_categories_manager import ntcm
 from forloop_modules.globals.active_entity_tracker import aet
@@ -26,16 +28,23 @@
         self.fn_name = "Find Similar Items"
         self.type_category = ntcm.categories.webscraping
         self.docs_category = DocsCategories.webscraping_and_rpa
         super().__init__()
 
     def make_form_dict_list(self, node_detail_form=None):
         fdl = FormDictList()
+        fdl.entry(name="elements", text="Elements", input_types=["list"], row=1)
+
         return fdl
 
+    def execute(self, node_detail_form):
+        elements = node_detail_form.get_chosen_value_by_name("elements", variable_handler)
+
+        self.direct_execute(elements)
+
     def direct_execute_old(self, elements: list[dict]):
         # Get XPaths of selected elements
         xpaths = [x['xpath'] for x in elements]
         common_xpath_part, xpaths_leftovers = suh.cut_xpaths_to_common_part(xpaths)
         # Find optimal siblings level (index of XPath)
         generalized_common_xpath_parts, optimal_xpath_index = suh.get_generalized_xpaths(
             common_xpath_part
@@ -108,15 +117,15 @@
         # new_elements_positions after scanning of generalized elements in suh.get_generalized_xpaths
         try:
             new_elements_positions = suh.update_webpage_elements(  # noqa
                 refresh_browser_view_elements=False
             )
         except:
             flog.error('Error while loading elements positions!')
-            new_elements_positions = []  # noqa
+            # new_elements_positions = []  # noqa
 
         # api_user_flow_step=APIUserFlowStep(user_uid="1", step_identifier="WebExtractor_FindSimilarItems", step_data=str(len(new_elements_positions)), timestamp_utc=datetime.datetime.now())
         # acm.new_user_flow_step(api_user_flow_step)
 
         import difflib
 
         def extract_shared_prefix_and_suffix_from_strings_and_substring(string, substring):
@@ -186,27 +195,27 @@
 
             #     print(is_at_least_one_leftover_contained, xpaths_leftovers)
 
             #     if is_generalized_common_xpath_part_contained and is_at_least_one_leftover_contained:
             #         matching_elements.append(element_position["xpath"])
 
             suh.matching_elements_groups = matching_elements_groups
-            message = "Selected elements XPATHs " + str(selected_elements_xpaths_new)
+            # message = "Selected elements XPATHs " + str(selected_elements_xpaths_new)
         except Exception as e:
             print(e)
             matching_elements = []
             matching_elements_groups = {}
             suh.matching_elements_groups = matching_elements_groups
-            message = "Selected elements XPATHs " + str(
-                selected_elements_xpaths_new
-            ) + ", Error occured in finding matching elements"
+            # message = "Selected elements XPATHs " + str(
+            #     selected_elements_xpaths_new
+            # ) + ", Error occured in finding matching elements"
 
         data = {
-            "message": message,
-            "ok": True,
+            # "message": message,
+            # "ok": True,
             "elements_generalized_xpaths": elements_generalized_xpaths,
             "similar_items_xpaths": matching_elements,
             "similar_items_xpath_groups": matching_elements_groups,
         }
         redis_action_key = redis_config.SCRAPING_ACTION_KEY_TEMPLATE.format(
             pipeline_uid=aet.active_pipeline_uid
         )
@@ -219,16 +228,23 @@
         self.icon_type = "ConvertToScrapingNodes"
         self.fn_name = "Convert To Scraping Nodes"
         self.type_category = ntcm.categories.webscraping
         super().__init__()
 
     def make_form_dict_list(self, node_detail_form=None):
         fdl = FormDictList()
+        fdl.entry(name="xpaths", text="", input_types=["str", "list"], row=1)
+
         return fdl
 
+    def execute(self, node_detail_form):
+        xpaths = node_detail_form.get_chosen_value_by_name("xpaths", variable_handler)
+
+        self.direct_execute(xpaths)
+
     def direct_execute(self, xpaths: list[Union[str, list[str]]]):
         columns = [f"column_{i}" for i, _ in enumerate(xpaths)]
 
         variable_handler.create_variable("xpaths_ExtractXPathsToDf", xpaths)
         variable_handler.create_variable("columns_ExtractXPathsToDf", columns)
         ncrb.new_node(
             pos=[300, 300], typ="ExtractXPathsToDf", params_dict={
@@ -251,14 +267,17 @@
 
         super().__init__()
 
     def make_form_dict_list(self, node_detail_form=None):
         fdl = FormDictList()
         return fdl
 
+    def execute(self, node_detail_form):
+        self.direct_execute()
+
     def direct_execute(self):
         suh.refresh_browser_view()
         redis_action_key = redis_config.SCRAPING_ACTION_KEY_TEMPLATE.format(
             pipeline_uid=aet.active_pipeline_uid
         )
         kv_redis.set(redis_action_key, suh.screenshot_string)
 
@@ -271,28 +290,54 @@
         self.fn_name = "Scan browser webpage"
         self.type_category = ntcm.categories.webscraping
 
         super().__init__()
 
     def make_form_dict_list(self, node_detail_form=None):
         fdl = FormDictList()
+        fdl.entry(name="url", text="", input_types=["str"], row=1)
+        fdl.entry(
+            name="incl_tables", text="Include tables", input_types=["bool"], row=2
+        )
+        fdl.entry(
+            name="incl_bullets", text="Include bullets", input_types=["bool"], row=3
+        )
+        fdl.entry(
+            name="incl_texts", text="Include texts", input_types=["bool"], row=4
+        )
+        fdl.entry(
+            name="incl_headlines", text="Include headlines", input_types=["bool"], row=5
+        )
+        fdl.entry(
+            name="incl_links", text="Include links", input_types=["bool"], row=6
+        )
+        fdl.entry(
+            name="incl_images", text="Include images", input_types=["bool"], row=7
+        )
+        fdl.entry(
+            name="incl_buttons", text="Include buttons", input_types=["bool"], row=8
+        )
+        fdl.entry(name="xpath", text="By XPath", input_types=["str"], row=9)
+
         return fdl
 
-    def direct_execute_old(
-        self, incl_tables, incl_bullets, incl_texts, incl_headlines, incl_links, incl_images,
-        incl_buttons, by_xpath, context_xpath=''
-    ):
-        suh.scan_web_page(
-            incl_tables, incl_bullets, incl_texts, incl_headlines, incl_links, incl_images,
-            incl_buttons, by_xpath, context_xpath, refresh_bv_elements=False
-        )
-        redis_action_key = redis_config.SCRAPING_ACTION_KEY_TEMPLATE.format(
-            pipeline_uid=aet.active_pipeline_uid
+    def execute(self, node_detail_form):
+        url = node_detail_form.get_chosen_value_by_name("url", variable_handler)
+        incl_tables = node_detail_form.get_chosen_value_by_name("incl_tables", variable_handler)
+        incl_bullets = node_detail_form.get_chosen_value_by_name("incl_bullets", variable_handler)
+        incl_texts = node_detail_form.get_chosen_value_by_name("incl_texts", variable_handler)
+        incl_headlines = node_detail_form.get_chosen_value_by_name("incl_headlines", variable_handler)
+        incl_links = node_detail_form.get_chosen_value_by_name("incl_links", variable_handler)
+        incl_images = node_detail_form.get_chosen_value_by_name("incl_images", variable_handler)
+        incl_buttons = node_detail_form.get_chosen_value_by_name("incl_buttons", variable_handler)
+        xpath = node_detail_form.get_chosen_value_by_name("xpath", variable_handler)
+
+        self.direct_execute(
+            url, incl_tables, incl_bullets, incl_texts, incl_headlines, incl_links, incl_images, incl_buttons, xpath
         )
-        kv_redis.set(redis_action_key, suh.webpage_elements)
 
     def direct_execute(
         self, url: str, incl_tables, incl_bullets, incl_texts, incl_headlines, incl_links,
         incl_images, incl_buttons, xpath
     ):
         scraping_options = {
             'incl_tables': incl_tables,
@@ -361,29 +406,31 @@
         # request_thread=slack_notif.UnblockingFunctionThread(slack_notif.send_slack_notification, api_scan_webpage.url, user_email=api_scan_webpage.email)
         # request_thread.start()
 
         #slack_notif.send_slack_notification(api_scan_webpage.url,user_email=api_scan_webpage.email)  #2 seconds
         # e_time = time.perf_counter() - start_time #12.5s
 
         suh.webscraping_client.load_website(url, timeout=30)
-        elements = suh.scan_web_page_API(output_folder, scraping_options)  #9 seconds
-        # with open(output_folder / "website.png", "rb") as file:
+        elements, screenshot_base64 = suh.scan_web_page_API(output_folder, scraping_options)  #9 seconds
+
+        # # Convert PNG file to WEBP
+        # img = Image.open(output_folder / "website.png")
+        # img.save(output_folder / "website.webp", quality=85)
+        # (output_folder / "website.png").unlink()
+        # with open(output_folder / "website.webp", "rb") as file:
         #     screenshot = file.read()
         #     screenshot = base64.b64encode(screenshot).decode("utf-8")
 
-        # Convert to WEBP
-        img = Image.open(output_folder / "website.png")
-        webp_filename = url
-        for char in r'<>:"/\|?*':
-            webp_filename = webp_filename.replace(char, '_')
-        webp_filename += ".webp"
-        img.save(output_folder / webp_filename, quality=85)
-        with open(output_folder / webp_filename, "rb") as file:
-            screenshot = file.read()
-            screenshot = base64.b64encode(screenshot).decode("utf-8")
+        # Convert Base64 to WEBP
+        png_img_data = BytesIO(base64.b64decode(screenshot_base64))
+        webp_img_data = BytesIO()
+        Image.open(png_img_data).save(webp_img_data, 'WEBP', quality=70)
+        webp_img_data.seek(0)
+        screenshot = base64.b64encode(webp_img_data.getvalue()).decode("utf-8")
+
 
         # f_time = time.perf_counter() - start_time #21.5s
         # request_thread.join()
 
         # i_time = time.perf_counter() - start_time #???s
 
         # ncm.elements_positions_temp=elements #temp storage TODO: should be done for users or send via API
@@ -460,19 +507,29 @@
     def __init__(self):
         self.icon_type = "FilterWebpageElementsWithAI"
         self.fn_name = "Filter webpage elements with AI"
         self.type_category = ntcm.categories.webscraping
         super().__init__()
 
     def make_form_dict_list(self, node_detail_form=None):
-        return FormDictList()
+        fdl = FormDictList()
+        fdl.entry(name="elements", text="Elements", input_types=["list"], row=1)
+        fdl.entry(name="objective", text="Objective", input_types=["str"], row=2)
+
+        return fdl
+
+    def execute(self, node_detail_form):
+        elements = node_detail_form.get_chosen_value_by_name("elements", variable_handler)
+        objective = node_detail_form.get_chosen_value_by_name("objective", variable_handler)
+
+        self.direct_execute(elements, objective)
 
     def direct_execute(self, elements, objective):
         response = ncrb.filter_webpage_elements_based_on_objective(elements=elements, objective=objective)
-            
+
         if response.status_code in [200, 201]:
             result = response.json()
             redis_action_key = redis_config.SCRAPING_ACTION_KEY_TEMPLATE.format(pipeline_uid=aet.active_pipeline_uid)
             kv_redis.set(redis_action_key, result)
         else:
             raise CriticalPipelineError(response.reason)
```

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/cleaning_handlers.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/cleaning_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/control_flow_handlers.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/control_flow_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/data_handlers.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/data_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/database_handlers.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/database_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/datetime_handlers.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/datetime_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/file_managment_handlers.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/file_managment_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/integration_handlers.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/integration_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/mapping_handlers.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/mapping_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/model_handlers.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/model_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/orchestration_handlers.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/orchestration_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/rpa_handlers.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/rpa_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/transformations/basic_transforms.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/transformations/basic_transforms.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/transformations/imputation.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/transformations/imputation.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/transformations/outliers.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/transformations/outliers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/variable_handlers.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/variable_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/function_handlers/webscraping_handlers.py` & `forloop_modules-1.1.0/forloop_modules/function_handlers/webscraping_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,17 +72,17 @@
         )
 
     def make_form_dict_list(self, node_detail_form=None):
         fdl = FormDictList()
 
         fdl.label(self.fn_name)
         fdl.label("Show browser:")
-        fdl.checkbox(name="in_browser", bool_value=True, row=1)
+        fdl.checkbox(name="in_browser", bool_value=False, row=1, desktop_only=True)
         fdl.label("Driver:")
-        fdl.combobox(name="driver", options=['Firefox', 'Chrome'], default='Firefox', show_info=True, row=2)
+        fdl.combobox(name="driver", options=['Firefox', 'Chrome'], default='Firefox', show_info=True, row=2, desktop_only=True)
 
         return fdl
 
     def execute(self, node_detail_form):
         in_browser = node_detail_form.get_chosen_value_by_name("in_browser", variable_handler)
         driver = node_detail_form.get_chosen_value_by_name("driver", variable_handler)
 
@@ -245,15 +245,15 @@
     def make_form_dict_list(self, node_detail_form=None):
         fdl = FormDictList()
 
         fdl.label(self.fn_name)
         fdl.label("URL")
         fdl.entry(name="url", text="", input_types=["str"], required=True, show_info=True, row=1)
         fdl.label("Take screenshot")
-        fdl.checkbox(name="take_screenshot", bool_value=True, row=2)
+        fdl.checkbox(name="take_screenshot", bool_value=False, row=2, desktop_only=True)
         fdl.label("Screenshot will be shown in Browser View", row=3)
 
         return fdl
 
     def execute(self, node_detail_form):
         url = node_detail_form.get_chosen_value_by_name("url", variable_handler)
         take_screenshot = node_detail_form.get_chosen_value_by_name("take_screenshot", variable_handler)
```

### Comparing `forloop_modules-1.0.2/forloop_modules/globals/active_entity_tracker.py` & `forloop_modules-1.1.0/forloop_modules/globals/active_entity_tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,11 +105,11 @@
 
     def set_project_and_pipeline_uid(
         self, project_uid: Optional[str] = None, pipeline_uid: Optional[str] = None
     ) -> None:
         self.project_uid = project_uid if project_uid is not None else self.project_uid
         self.active_pipeline_uid = pipeline_uid if pipeline_uid is not None else self.active_pipeline_uid
 
-    def set_pipeline_job_uid(self, pipeline_job_uid: str) -> None:
+    def set_pipeline_job_uid(self, pipeline_job_uid: Optional[str] = None) -> None:
         self.active_pipeline_job_uid = pipeline_job_uid
 
 aet=ActiveEntityTracker()
```

### Comparing `forloop_modules-1.0.2/forloop_modules/globals/database_utilities_handler.py` & `forloop_modules-1.1.0/forloop_modules/globals/database_utilities_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/globals/db_connection.py` & `forloop_modules-1.1.0/forloop_modules/globals/db_connection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,57 @@
-import dbhydra.dbhydra_core as dh
-import forloop_modules.flog as flog
+from typing import Literal, Optional, Union
 
 from pydantic import BaseModel
-from typing import Literal, Union, Optional
+
+import dbhydra.dbhydra_core as dh
+import forloop_modules.flog as flog
+from forloop_modules.redis.redis_connection import (
+    create_redis_key_for_project_db_private_key,
+    kv_redis,
+)
+from forloop_modules.utils.encryption import (
+    convert_base64_private_key_to_rsa_private_key,
+    decrypt_text,
+)
 
 DbDialect = Literal["MySQL", "SQL Server", "PostgreSQL", "Xlsx structure", "MongoDB", "BigQuery"]
 DBInstance = Union[dh.MysqlDb, dh.SqlServerDb, dh.PostgresDb, dh.XlsxDB, dh.MongoDb, dh.BigQueryDb]
 
+
 class DbDetails(BaseModel):
     DB_SERVER: str
     DB_PASSWORD: str
     DB_PORT: int
     DB_USERNAME: str
     DB_DATABASE: str
     LOCALLY: bool
     DIALECT: DbDialect
-    
+
     def __getitem__(self, key):
         return getattr(self, key)
 
+
 class DbConnection:
     def __init__(self, db_details: Union[DbDetails, dict], is_stored: bool = False):
-        self.db_details = db_details.model_dump() if isinstance(db_details, DbDetails) else db_details
+        self.db_details = db_details.model_dump(
+        ) if isinstance(db_details, DbDetails) else db_details
         self.server = db_details["DB_SERVER"]
         self.database = db_details["DB_DATABASE"]
         self.is_stored = is_stored
         self.is_valid_db_connection: bool = False
-        
+
         # Assigned after testing the connection
         self.db_instance: Optional[DBInstance] = None
         self.is_connected: bool = False
         self.table_dict: Optional[dict] = None
         self.foreign_keys: Optional[list] = None
 
         # TODO: This should not be here. Examine the code and delete it everywhere.
         self.images = []  # icons covering this DbConnection
 
-
     def create_new_db(self):
         if self.db_details["DIALECT"] == "MySQL":
             dh.MysqlDb(db_details=self.db_details).create_new_db()
             return True
         return False
 
     # def _store_db_details_if_valid(self):
@@ -84,24 +95,24 @@
             else:
                 return False
 
             self.is_valid_db_connection = True
             # self._store_db_details_if_valid()
             return True
         except Exception:
-            self.db_instance=None
+            self.db_instance = None
             self.is_valid_db_connection = False
             flog.error("Database Connection Failed!")
 
             return False
 
     def test_database_connection(self) -> bool:
         """
         Test connection to database
-        if connected successfully, get database tables
+        if connected successfully, get database tables.
         """
         is_connected = self._test_connection_dbhydra_db()
 
         if is_connected:
             self.get_table_dict_and_fk()
 
         return is_connected
@@ -110,23 +121,49 @@
         with self.db_instance.connect_to_db():
             self.table_dict = self.db_instance.generate_table_dict()
             if self.db_details["DIALECT"] == "SQL Server":
                 self.foreign_keys = self.db_instance.get_foreign_keys_columns()
             else:
                 self.foreign_keys = []
         return (self.table_dict, self.foreign_keys)
-    
+
     def get_db_table(self, db_table_name: str):
         if self.table_dict is None:
             return
-        
+
         for table_name, table in self.table_dict.items():
             if table_name == db_table_name:
                 return table
-            
+
+
 def create_db_details_from_database_dict(db_dict: dict):
-    db_details = DbDetails(DB_SERVER=db_dict["server"], DB_PASSWORD=db_dict["password"], DB_PORT=db_dict["port"],
-                           DB_USERNAME=db_dict["username"], DB_DATABASE=db_dict["database_name"], LOCALLY=False,
-                           DIALECT=db_dict["dialect"])
-    
+    db_details = DbDetails(
+        DB_SERVER=db_dict["server"],
+        DB_PASSWORD=db_dict["password"],
+        DB_PORT=db_dict["port"],
+        DB_USERNAME=db_dict["username"],
+        DB_DATABASE=db_dict["database"],
+        LOCALLY=False,
+        DIALECT=db_dict["dialect"],
+    )
+
     return db_details
-    
+
+
+def decrypt_db_details(database: dict) -> DbDetails:
+    """Decrypt the password of the database using the private key stored in Redis."""
+    redis_key = create_redis_key_for_project_db_private_key(project_uid=database['project_uid'])
+    private_key_base64 = kv_redis.get(redis_key)
+
+    if private_key_base64 is not None:
+        private_key = convert_base64_private_key_to_rsa_private_key(
+            private_key_base64=private_key_base64
+        )
+
+        encrypted_password = database["password"]
+        decrypted_password = decrypt_text(text=encrypted_password, private_key=private_key)
+
+        database["password"] = decrypted_password
+
+        return create_db_details_from_database_dict(db_dict=database)
+    else:
+        raise ValueError("Private key not found in Redis.")
```

### Comparing `forloop_modules-1.0.2/forloop_modules/globals/dbtables_loader_popups.py` & `forloop_modules-1.1.0/forloop_modules/globals/dbtables_loader_popups.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/globals/local_variable_handler.py` & `forloop_modules-1.1.0/forloop_modules/globals/local_variable_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-
-
 IS_EXECUTION_CORE=True
 
 #if IS_EXECUTION_CORE:
 #    from src.core.variable_handler import variable_handler
 
 import json
 import pandas as pd
-import ast 
+import ast
 import inspect
 
-from typing import Dict, Set, Any, Literal
+from typing import Dict, Set, Any, Literal, Optional
 from dataclasses import dataclass, field
 
 import forloop_modules.flog as flog
 
 #from src.df_column_category_predictor import classify_df_column_categories, DataFrameColumnCategoryAnalysis
 
 from forloop_modules.redis.config.config import redis_config
@@ -78,32 +76,34 @@
     def handler_mode(self):
         return self._handler_mode
 
     @handler_mode.setter
     def handler_mode(self, value: Any) -> None:
         raise AttributeError("Use `change_variable_mode` method to change the mode of LocalVariableHandler.")
 
-    def change_mode(self, mode: Literal["initial_variable", "variable"]) -> None:
+    def change_variable_mode(self, mode: Literal["initial_variable", "variable"]) -> None:
         """Change state specifying on which type of variable is the handler currently operating."""
         if mode not in ["variable", "initial_variable"]:
             raise ValueError(f"Variable mode `{mode}` is not supported.")
         self._handler_mode = mode
+        self.variables.clear()
+
 
     def _set_up_unique_varname(self, name: str) -> str:
         i = 2
 
         if not name:
             name = 'untitled1'
             # If untitled_i already exists -> try untitled_i+1
             while self._is_varname_duplicated(name):
                 name = f'untitled{i}'
                 i += 1
         elif " " in name:
             name = "_".join(name.split())
-        
+
         return name
 
     def _is_varname_duplicated(self, name: str) -> bool:
         # names = [x.value for x in self.variables.values()]#self.stored_variable_df['Name'].tolist()  # All current variables' names
         names = list(self.variables.keys())
         checker = name in names
         return checker
@@ -121,15 +121,15 @@
             value.attrs["name"] = local_variable.name
 
             variable = self.get_variable_by_name(name)
             local_variable = LocalVariable(variable["uid"], variable["name"], value, variable["is_result"])  # TODO: Remove when PrototypeJobs are implemented
             return local_variable
         else:
             return local_variable
-        
+
     def get_int_to_str_col_name_mapping(self, df: pd.DataFrame) -> dict[int, str]:
         """
         find columns whose name type is int and create mapping between their int name and its string form
         :param df:
         :type df:
         :return:
         :rtype:
@@ -144,15 +144,15 @@
     def new_file(self, path):
         # TODO is temporary until workflow for files is introduced
         name, *suffix = path.split(".")
         suffix = ".".join(suffix)
         name = path.split("/")[-1]
         file = File(path, name)  # suffix
         file_variable = self.create_file(file)
-    
+
     def create_file(self, file: File, project_uid=None):
         # TODO is temporary until workflow for files is introduced
 
         # TODO: NEVER USED, NOT TESTED (NCRB + LOCAL VARIABLE CALL WITH 4 PARAMETERS INSTEAD OF 2)
         response = ncrb.get_variable_by_name(file.file_name)
         result = json.loads(response.content)
         uid = result["uid"]
@@ -168,33 +168,33 @@
         self.dataframe_scan_analyses_records[name] = DataFrameWizardScanAnalysis()
         value = value.rename(columns=self.get_int_to_str_col_name_mapping(value))
         # self.dataframe_column_category_predictions[name] = classify_df_column_categories(value)
         value.attrs["name"] = name
 
         return value
 
-    def new_variable(self, name, value, additional_params: dict = None, project_uid=None):
+    def new_variable(self, name, value, is_result: Optional[bool] = None, additional_params: dict = None, project_uid=None):
         if additional_params is None:
             additional_params = {}
 
         name = self._set_up_unique_varname(name)
 
         if isinstance(value, pd.DataFrame):
             value = self.process_dataframe_variable_on_initialization(name, value)
 
         if name in self.variables.keys():
-            variable = self.update_variable(name, value, additional_params)
+            variable = self.update_variable(name, value, is_result, additional_params)
             is_new_variable=False
         else:
-            variable=self.create_variable(name, value, additional_params)
+            variable=self.create_variable(name, value, is_result, additional_params)
             is_new_variable=True
 
         return variable, is_new_variable
 
-    def create_variable(self, name, value, additional_params: dict = None, project_uid=None):
+    def create_variable(self, name, value, is_result: Optional[bool] = None, additional_params: dict = None, project_uid=None):
         #self.variable_uid_project_uid_dict[variable.uid]=project_uid #is used in API call
         if additional_params is None:
             additional_params = {}
 
         if self.handler_mode == "initial_variable":
             ncrb_fn = ncrb.new_initial_variable
         elif self.handler_mode == "variable":
@@ -210,15 +210,16 @@
             else:
                 data_dict={}
                 data_dict[name]=value
                 folder=".//file_transfer"
                 save_data_dict_to_pickle_folder(data_dict,folder,clean_existing_folder=False)
             #TODO: FILE TRANSFER MISSING
 
-            response = ncrb_fn(name=name, value="", type=type(value).__name__)
+            optional_args = {"is_result": is_result} if is_result is not None else {}
+            response = ncrb_fn(name=name, value="", type=type(value).__name__, **optional_args)
 
         result = response.json()
         self.create_local_variable(
             result["uid"], result["name"], result["value"], result["is_result"],
             result["type"]
         )  # TODO: Remove when PrototypeJobs are implemented
         return result
@@ -232,72 +233,73 @@
             if isinstance(value, pd.DataFrame):
                 value = self.process_dataframe_variable_on_initialization(name, value)
 
         variable=LocalVariable(uid, name, value, is_result) # TODO: Remove when PrototypeJobs are implemented
         self.variables[name]=variable
         return(variable)
 
-    def update_variable(self, name, value, additional_params: dict = None, project_uid=None):
+    def update_variable(self, name, value, is_result: Optional[bool] = None, additional_params: dict = None, project_uid=None):
         if additional_params is None:
             additional_params = {}
 
         if self.handler_mode == "initial_variable":
-            ncrb_fn = ncrb.update_initial_variable_by_uid
+            ncrb_update_by_uid_fn = ncrb.update_initial_variable_by_uid
         elif self.handler_mode == "variable":
-            ncrb_fn = ncrb.update_variable_by_uid
+            ncrb_update_by_uid_fn = ncrb.update_variable_by_uid
 
         variable = None
         try: # Function to run even if no variable is found
             variable = self.get_variable_by_name(name)
         except Exception:
             flog.warning(f"Variable '{name}' was not found in LocalVariableHandler.")
 
         if variable is not None:
+            is_result = is_result if is_result is not None else variable["is_result"]
             ncrb_fn_kwargs = {
                 "variable_uid": variable["uid"],
                 "name": name,
                 "value": value,
-                "is_result": variable["is_result"]  # TODO: Remove when PrototypeJobs are implemented
+                "is_result": is_result  # TODO: Remove when PrototypeJobs are implemented
             }
 
             if is_value_serializable(value):
-                response = ncrb_fn(**ncrb_fn_kwargs)
+                response = ncrb_update_by_uid_fn(**ncrb_fn_kwargs)
             else:
                 ncrb_fn_kwargs.update(value="")
 
                 if is_value_redis_compatible(value):
                     kv_redis.set(self.get_variable_redis_name(name), value, additional_params)
                 else:
                     data_dict={}
                     data_dict[name]=value
                     folder=".//file_transfer"
                     save_data_dict_to_pickle_folder(data_dict,folder,clean_existing_folder=False)
-                response = ncrb_fn(type=type(value).__name__, **ncrb_fn_kwargs)
+                response = ncrb_update_by_uid_fn(type=type(value).__name__, **ncrb_fn_kwargs)
 
             result = response.json()
             self.update_local_variable(
                 result["name"], result["value"], result["is_result"], result["type"]
             )  # TODO: Remove when PrototypeJobs are implemented
             return result
 
-        
+
         #else:
         #    self.variables.pop(name)
         #    self.create_variable(name, value)
-            
+
         #variable=self.variables[name]
         #self.variables[name].value=value #Update
         #return(variable)
-    
+
     def update_local_variable(self, name, value, is_result: bool, type=None):
         if type in JSON_SERIALIZABLE_TYPES_AS_STRINGS and type != "str":
             value=ast.literal_eval(str(value))
         elif type in REDIS_STORED_TYPES_AS_STRINGS:
             value = kv_redis.get(self.get_variable_redis_name(name))
-        
+
         variable=self.variables[name]
         self.variables[name].value=value #Update
         self.variables[name].is_result = is_result  # TODO: Remove when PrototypeJobs are implemented
 
         return(variable)
 
     def delete_variable(self, var_name: str):
@@ -309,14 +311,45 @@
         elif self.handler_mode == "variable":
             ncrb_delete_by_uid = ncrb.delete_variable_by_uid
 
         variable = self.get_variable_by_name(var_name)
         ncrb_delete_by_uid(variable["uid"])
         self.delete_local_variable(var_name)
 
+
+    def save_variables_as_initial_variables(self):
+        """Save all currently loaded Variables as InitialVariables."""
+        if not self._handler_mode == "variable":
+            raise AttributeError(
+                "LocalVariableHandler must be in 'variable' mode to resave results."
+            )
+
+        for variable in self.variables.values():
+            if is_value_serializable(variable.value):
+                ncrb.new_initial_variable(name=variable.name, value=variable.value)
+            else:
+                value = kv_redis.get(self.get_variable_redis_name(variable.name))
+                if is_value_redis_compatible(variable.value):
+                    kv_redis.set(f'stored_initial_variable_{variable.name}', value)
+                else:
+                    data_dict = {}
+                    data_dict[variable.name] = variable.value
+                    folder = ".//file_transfer"
+                    save_data_dict_to_pickle_folder(data_dict, folder, clean_existing_folder=False)
+                #TODO: FILE TRANSFER MISSING
+
+                optional_args = (
+                    {"is_result": variable.is_result} if variable.is_result is not None else {}
+                )
+                ncrb.new_initial_variable(
+                    name=variable.name, value="", type=type(variable.value).__name__,
+                    **optional_args
+                )
+
+
     def delete_local_variable(self, var_name:str):
         self.variables.pop(var_name)
 
     def get_variable_by_name(self, name: str) -> dict:
         """Get Variable/InitialVariable uid based on its name and the pipeline it's assigned to."""
         if self.handler_mode == "initial_variable":
             ncrb_get_by_name_fn = ncrb.get_initial_variable_by_name
@@ -326,30 +359,30 @@
         response = ncrb_get_by_name_fn(name)
         response.raise_for_status()
         return response.json()
 
     @property
     def last_active_dataframe_node_uid(self):
         return self._last_active_dataframe_node_uid
-    
+
     # temporary until cyclic import of ncrb in cleaning handlers is resolved
     @last_active_dataframe_node_uid.setter
     def last_active_dataframe_node_uid(self, node_uid:int):
         self._last_active_dataframe_node_uid = node_uid
-    
+
     #   TODO: fix dependencies
     #def update_data_in_variable_explorer(self, glc): #TODO Dominik: Refactor out, shouldnt be here
     #    self.is_refresh_needed = False
     #    if hasattr(glc, "variable_explorer"):
-            
+
     #        glc.variable_explorer.update_data(self.stored_variable_df)
 
-        # stored_variables_list = [[x.name, x.typ, x.size, x.value] for x in self.values()]
-        # stored_variable_df = pd.DataFrame(stored_variables_list, columns=["Name", "Type", "Size", "Value"])
-        # glc.variable_explorer.update_data(stored_variable_df)
+    # stored_variables_list = [[x.name, x.typ, x.size, x.value] for x in self.values()]
+    # stored_variable_df = pd.DataFrame(stored_variables_list, columns=["Name", "Type", "Size", "Value"])
+    # glc.variable_explorer.update_data(stored_variable_df)
 
 
     def populate_df_analysis_record(self, name, empty_rows, duplicated_rows, empty_columns, id_columns, result):
         df_analysis = DataFrameWizardScanAnalysis()
         df_analysis.is_analyzed = True
         df_analysis.empty_rows = empty_rows
         df_analysis.duplicated_rows = duplicated_rows
```

### Comparing `forloop_modules-1.0.2/forloop_modules/globals/scraping_utilities_handler.py` & `forloop_modules-1.1.0/forloop_modules/globals/scraping_utilities_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import re
 import forloop_modules.flog as flog
 import numpy as np
 import time
 import configparser
 from contextlib import suppress
 from itertools import product
+import uuid
+from typing import Optional
 
 import forloop_modules.queries.node_context_requests_backend as ncrb #questionable import - potential problems - should be rather called from pfh
 
 from pathlib import Path
 from docrawl.docrawl_client import DocrawlClient
 from docrawl.elements import ElementType
 
@@ -71,15 +73,18 @@
     Ideally webpage_elements should be only used in SUH (BE), while browser_view_elements and
     browser_view_selected_elements should be used in BrowserView (FE)
 
     Also note, that redis communication should be performed here, not in BrowserView
 
     """
 
-    def __init__(self):
+    def __init__(self, uid: Optional[str] = None, init_docrawl = False):
+        if not init_docrawl:
+            return
+
         self.webpage_elements = []
         self.browser_view_elements = []
         self.browser_view_selected_elements = []
         self.browser_view_selected_element_groups = []
 
         # Used for refreshing image in BrowserView
         self.is_screenshot_updated = False
@@ -90,46 +95,42 @@
         self.are_all_elements_selected = False
 
         self._is_browser_active = None
 
         # TODO: for now hardcoded, user_id, project_id and pipeline_id should be passed later
         # All kv_redis scraping keys should be stored only here to avoid
         
-        if synchronization_flags.IS_MODULE_MAIN_INITIALIZED:
-            redis_key_prefix="FORLOOP_MAIN_DOCRAWL_"
-        elif synchronization_flags.IS_MODULE_FORLOOP_FASTAPI_INITIALIZED:
-            redis_key_prefix="FORLOOP_FASTAPI_DOCRAWL_"
-        elif synchronization_flags.IS_MODULE_EXECUTION_CORE_INITIALIZED:
-            redis_key_prefix="FORLOOP_EXECUTION_CORE_DOCRAWL_"
+        # if synchronization_flags.IS_MODULE_MAIN_INITIALIZED:
+        #     redis_key_prefix="FORLOOP_MAIN_DOCRAWL_"
+        # elif synchronization_flags.IS_MODULE_FORLOOP_FASTAPI_INITIALIZED:
+        #     redis_key_prefix="FORLOOP_FASTAPI_DOCRAWL_"
+        # elif synchronization_flags.IS_MODULE_EXECUTION_CORE_INITIALIZED:
+        #     redis_key_prefix="FORLOOP_EXECUTION_CORE_DOCRAWL_"
+        # else:
+        #     redis_key_prefix = None
+
+        if uid is not None:
+            redis_key_prefix = f'docrawl:{uid}'
         else:
-            redis_key_prefix = None
-            
-        
-        
-        self._scraping_data_redis_key_prefix = redis_key_prefix #older approach: 'test_user:test_project:test_pipeline:scraping'
+            redis_key_prefix = f'docrawl:{str(uuid.uuid4())[:8]}'
+
+        self._scraping_data_redis_key_prefix = redis_key_prefix
         self._kv_redis_key_browser_meta_data = f'{self._scraping_data_redis_key_prefix}:browser_meta_data'
         self._kv_redis_key_screenshot = f'{self._scraping_data_redis_key_prefix}:screenshot'
         self._kv_redis_key_elements = f'{self._scraping_data_redis_key_prefix}:elements'
 
         kv_redis_keys = {
             'browser_meta_data': self._kv_redis_key_browser_meta_data,
             'screenshot': self._kv_redis_key_screenshot,
             'elements': self._kv_redis_key_elements,
         }
 
         # For now DocrawlClient should follow singleton pattern, meaning it should be initialised only once and here
-        
-        
-        
-        if redis_key_prefix is not None:
-            redis_key_prefix="" # to be deprecated
-            self.webscraping_client = DocrawlClient(kv_redis=kv_redis, kv_redis_keys=kv_redis_keys, number_of_spawn_browsers=1, redis_key_prefix=redis_key_prefix)
-            
-            
-            
+        self.webscraping_client = DocrawlClient(kv_redis=kv_redis, kv_redis_keys=kv_redis_keys, number_of_spawn_browsers=1, redis_key_prefix=redis_key_prefix)
+
         try:
             config = configparser.ConfigParser()
             config.read(Path(__file__).parent.parent.parent.absolute() / 'config' / 'scraping_conf.ini')
     
             self.scraperapi_key = config['PROXY']['SCRAPERAPI_KEY']
             self.scrapingbee_key = config['PROXY']['SCRPABINGBEE_KEY']
         except KeyError:
@@ -623,15 +624,16 @@
         
         generate_folder_structure("tmp")
         generate_folder_structure("tmp/screenshots")
         generate_folder_structure("tmp/scraped_data")
 
         xpath = self.detect_cookies_xpath_preparation()
     
-        self.webscraping_client.take_png_screenshot(str(Path(output_folder, 'website.png'))) #needs to run before the scanner so there is enough time for the parallel thread
+        # self.webscraping_client.take_png_screenshot(str(Path(output_folder, 'website.png'))) #needs to run before the scanner so there is enough time for the parallel thread
+        self.webscraping_client.take_screenshot()
         self.webscraping_client.scan_web_page(**scraping_options, timeout = 60) #Duration: ~3s
         
     
         webpage_elements = self.update_webpage_elements(refresh_browser_view_elements=False) #Duration: ~ 0s
 
         cookies_elements, rest_elements = [], []
 
@@ -644,32 +646,33 @@
 
         if cookies_elements:
             flog.warning('Cookies popup was found')
             button_xpath = cookies_elements[0]['xpath']
 
             # Close cookies popup
             self.webscraping_client.click_xpath(button_xpath)
-            self.webscraping_client.take_png_screenshot(str(Path(output_folder, 'website.png'))) #TODO: The scanning finishes before the screenshot thread - need to either 1) refresh screenshot multiple times in FE (optimal), or 2) run this not in thread when cookies detected
+            # self.webscraping_client.take_png_screenshot(str(Path(output_folder, 'website.png'))) #TODO: The scanning finishes before the screenshot thread - need to either 1) refresh screenshot multiple times in FE (optimal), or 2) run this not in thread when cookies detected
+            self.webscraping_client.take_screenshot()
 
 
         # [::-1] needed to ensure that FE rectangles are not overlapped (bigger elements do not cover smaller)
-        return rest_elements[::-1]
+        return rest_elements[::-1], self.webscraping_client.get_browser_screenshot()
 
     def scan_web_page(self, incl_tables, incl_bullets, incl_texts, incl_headlines, incl_links, incl_images,
                       incl_buttons, by_xpath, context_xpath='', refresh_bv_elements=True):
         by_xpath = self.check_xpath_apostrophes(by_xpath)
 
         self.webscraping_client.scan_web_page(incl_tables, incl_bullets, incl_texts, incl_headlines,
                                        incl_links, incl_images, incl_buttons, by_xpath, context_xpath=context_xpath)
 
         # Load coordinates of elements on page
         webpage_elements = self.update_webpage_elements(refresh_browser_view_elements=refresh_bv_elements)
 
         return webpage_elements
-    
+
     def find_nth_substring_occurence(self, string, substring, n):
         #TODO: potentially could hit recursive limit
         if (n == 1) or n == 0:
             return string.find(substring)
         else:
             return string.find(substring, self.find_nth_substring_occurence(string, substring, n - 1) + 1)
 
@@ -758,10 +761,21 @@
     
             self.browser_view_elements = rest_of_browser_view_elements + [new_elem]
             self.reset_browser_view_selected_elements()
     
             flog.warning(self.browser_view_elements)
 
 
+# HACK: Without passing `init_docrawl=True`, `suh` variable acts as uninitialized, empty proxy.
+# This is necessary as the whole codebase imports `suh` from this file.
 
+# On the other hand, if `docrawl` gets initialized here, ExecCore workers are failing to spin up
+# their own event loops on which their `docrawl` instances relies. This is due to the fact that when
+# workers are spawned from the parent process, `docrawl` is already initialized (alongside with it's
+# event loop). The spawned process inherits `docrawls` event loop state without the actual event
+# loop thread running. This leads to the inconsistent state in every worker.
+
+# `suh` must only be used inside of processes which have `docrawl` event loop initialized -
+# currently it means only  `ExecutionCore` workers. As long as the process WILL NOT spawn child
+# processes, it is safe to initialize `docrawl` in it.
 suh = ScrapingUtilitiesHandler()
```

### Comparing `forloop_modules-1.0.2/forloop_modules/globals/variable_handler.py` & `forloop_modules-1.1.0/forloop_modules/globals/variable_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/integrations/slack_integration.py` & `forloop_modules-1.1.0/forloop_modules/integrations/slack_integration.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/integrations/testing_check_slack_notifications.py` & `forloop_modules-1.1.0/forloop_modules/integrations/testing_check_slack_notifications.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/node_detail_form.py` & `forloop_modules-1.1.0/forloop_modules/node_detail_form.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/pipeline_function_handlers.py` & `forloop_modules-1.1.0/forloop_modules/pipeline_function_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/queries/context_request_backend_auxiliary_functions.py` & `forloop_modules-1.1.0/forloop_modules/queries/context_request_backend_auxiliary_functions.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/queries/db_model_templates.py` & `forloop_modules-1.1.0/forloop_modules/queries/db_model_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -387,14 +387,15 @@
     name: str = ""
     value: Any = "" # strings, bytes, numbers, tuples, lists, dicts, sets, booleans, and None (anything evaluatable by ast.literal_eval)
     type: Optional[str] = None # Type can be enforced or autoinferred
     size: Optional[int] = None
     is_result: bool = False
     pipeline_uid: str = "0"
     project_uid: str = "0" # TODO: Is this necessary? Node is indirectly linked to a project via pipeline
+    pipeline_job_uid: str = "0"
 
     @field_validator("name", "value")
     @classmethod
     def check_for_single_quote_mark(cls, value: str) -> str:
         """
         HACK: Current DBHydra's implementation of INSERT method will remove any ' mark from the
         variable while inserting a record - even if this ' mark is a part of the inserted string.
@@ -655,45 +656,18 @@
     sheet_name: str
     email: str
 
 class APIEmail(BaseModel):
     email: Optional[str] = ""
     #email: str #Jakub branch
 
-class WebpageData(BaseModel):
+class APIDataFrame(BaseModel):
     columns: list[str]
     values: list[list[Any]]
 
-class APINewDbTable(BaseModel):
-    server: str
-    database_name: str
-    port: int
-    table_name: str
-    username: str
-    password: str
-    dialect: Literal["MySQL"] # TODO: Enable other dialects like PostgreSQL
-    data: WebpageData
-    # columns: list[str]
-    # elements: list[dict]
-    
-class APIDbDataPreview(BaseModel):
-    server: str
-    database_name: str
-    port: int
-    table_name: str
-    username: str
-    password: str
-    dialect: Literal["MySQL"] # TODO: Enable other dialects like PostgreSQL
-    data: WebpageData
-    # elements: list[dict]
-
-class APIUrl(BaseModel):
-    url: Optional[str]=""
-
-
 class APIToggleStatus(BaseModel):
     status: bool = False
 
 
 class APIButtonName(BaseModel):
     button_name:str=""
```

### Comparing `forloop_modules-1.0.2/forloop_modules/queries/node_context_requests_backend.py` & `forloop_modules-1.1.0/forloop_modules/queries/node_context_requests_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #### GLC, GOM dependencies forbidden !!!
 """In this file all functions should have response-like return value"""
 
 import requests
 import json
 from inspect import Parameter, Signature
 from pydantic import BaseModel
-from typing import Optional, Any
+from typing import Optional, Any, Generator
 import sys
-
 from pathlib import Path
-
+import httpx
 import forloop_modules.flog as flog
+import json
 
+from forloop_modules.utils.sse_parser import SSEParser
 from forloop_modules.globals.active_entity_tracker import aet
 
 from forloop_modules.queries.db_model_templates import APIProject, APITrigger, APIDataset, APIDbTable, APIScript, APIFile, APIDatabase, APIPipeline, APIEdge, APIVariable, APIPopup, APIInitialVariable
 
 if sys.platform == "darwin":  # MAC OS
     config_path = 'config/server_config_remote.ini'
 else:
@@ -112,14 +113,17 @@
     def new(*args,model_attribute_names_without_uid=model_attribute_names_without_uid, **kwargs):
         payload = {
             param: arg
             for param, arg in zip(model_attribute_names_without_uid, args)
         }
         payload.update(kwargs)
         set_stored_project_uid_and_pipeline_uid_to_factory_payload(payload)
+        if issubclass(model, APIVariable):
+            payload["pipeline_job_uid"] = aet.active_pipeline_job_uid
+
         #flog.info(f'New {resource_name} payload: {payload}')
         resource_url = f'{BASE_API}/{resource_name}'
 
         response = requests.post(resource_url, json=payload)
         #flog.info(f'New {resource_name} response: {response.text}')
         if not response.ok:
             flog.error(response.json())
@@ -141,14 +145,16 @@
     def update(uid, *args, model_attribute_names_without_uid=model_attribute_names_without_uid, **kwargs):
         payload = {
             param: arg
             for param, arg in zip(model_attribute_names_without_uid, args)
         }
         payload.update(kwargs)
         set_stored_project_uid_and_pipeline_uid_to_factory_payload(payload)
+        if issubclass(model, APIVariable):
+            payload["pipeline_job_uid"] = aet.active_pipeline_job_uid
 
         #flog.info(f'Update {resource_name} payload: {payload}')
         resource_url = f'{BASE_API}/{resource_name}/{uid}'
 
         response = requests.put(resource_url, json=payload)
         #flog.info(f'Update {resource_name} response: {response.text}')
         if not response.ok:
@@ -577,27 +583,29 @@
     response.raise_for_status()
     return response
 
 
 def update_variable_by_uid(variable_uid: str, name: str, value: Any, is_result: bool = None, type = None, size: Optional[int] = None):
     project_uid = aet.project_uid
     pipeline_uid = aet.active_pipeline_uid
-    
+    pipeline_job_uid = aet.active_pipeline_job_uid
+
     if type is None:
         for std_type in [str,int,list,dict,float,bool]:
             if isinstance(value,std_type):
                 type=std_type.__name__
                 
     payload = {
         "name": name,
         "value": value,
         "type": type,
         "size": size,
         "project_uid": project_uid,
-        "pipeline_uid": pipeline_uid
+        "pipeline_uid": pipeline_uid,
+        "pipeline_job_uid": pipeline_job_uid
         }
     if is_result is not None:
         payload["is_result"] = is_result
 
     response=requests.put(f"{BASE_API}/variables/{variable_uid}",json=payload)
     result=json.loads(response.content.decode('utf-8'))
     return(response)
@@ -618,14 +626,38 @@
     
 #     response = requests.put(url, json=payload)
 #     flog.info(f'Updated Variable response: {response.text}')
 
 #     return response
 
 
+def get_job_variables():
+    job_uid = aet.active_pipeline_job_uid
+    url = f'{BASE_API}/jobs/{job_uid}/variables'
+    response = requests.get(url)
+    response.raise_for_status()
+    return response
+
+def cancel_pipeline_job():
+    job_uid = aet.active_pipeline_job_uid
+    url = f'{BASE_API}/jobs/{job_uid}/cancel'
+    response = requests.post(url)
+    response.raise_for_status()
+    return response
+
+def consume_execution_stream(job_uid: str) -> Generator[dict, None, None]:
+    """Run in a separate thread as this is a blocking operation."""
+    url = f'{BASE_API}/jobs/{job_uid}/execution_stream'
+
+    with (httpx.Client(timeout=300) as client):
+        sse_handler = SSEParser(client)
+        for message in sse_handler.stream("GET", url, as_dict=True):
+            yield from message
+
+
 ##### INITIAL VARIABLES #####
 
 
 def get_initial_variable_by_name(uid: str):
     pipeline_uid = aet.active_pipeline_uid
     url = f'{BASE_API}/initial_variables?name={uid}&pipeline_uid={pipeline_uid}'
 
@@ -1302,22 +1334,23 @@
            }
     url = f'{BASE_API}/finalize_pipeline'
     response=requests.post(url=url,json=payload)
     print(json.loads(response.content))
     return response
 
 
-
 def pipeline_direct_execute(pipeline_uid):
-    payload={"pipeline_uid":pipeline_uid,}
+    payload = {"pipeline_uid": pipeline_uid}
     url = f'{BASE_API}/pipelines/{pipeline_uid}/direct_execute'
-    response=requests.post(url=url,json=payload)
-    print(json.loads(response.content))
+    response = requests.post(url=url, json=payload)
+    response.raise_for_status()
+
     return response
 
+
 def filter_webpage_elements_based_on_objective(elements: list[dict], objective: str):
     payload = {
         "elements": elements,
         "objective": objective
     }
     
     url = f'{BASE_API}/filter_webpage_elements_based_on_objective'
```

### Comparing `forloop_modules-1.0.2/forloop_modules/redis/config/config.py` & `forloop_modules-1.1.0/forloop_modules/redis/config/config.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/redis/redis_connection.py` & `forloop_modules-1.1.0/forloop_modules/redis/redis_connection.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/utils/definitions.py` & `forloop_modules-1.1.0/forloop_modules/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/utils/encryption.py` & `forloop_modules-1.1.0/forloop_modules/utils/encryption.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/utils/pandas_operations.py` & `forloop_modules-1.1.0/forloop_modules/utils/pandas_operations.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/utils/pickle_serializer.py` & `forloop_modules-1.1.0/forloop_modules/utils/pickle_serializer.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/utils/script_utils.py` & `forloop_modules-1.1.0/forloop_modules/utils/script_utils.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/utils/str_helpers.py` & `forloop_modules-1.1.0/forloop_modules/utils/str_helpers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/utils/synchronization_flags.py` & `forloop_modules-1.1.0/forloop_modules/utils/synchronization_flags.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/utils/url_template_builder.py` & `forloop_modules-1.1.0/forloop_modules/utils/url_template_builder.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules/utils/various.py` & `forloop_modules-1.1.0/forloop_modules/utils/various.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.2/forloop_modules.egg-info/PKG-INFO` & `forloop_modules-1.1.0/forloop_modules.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forloop-modules
-Version: 1.0.2
+Version: 1.1.0
 Summary: This package contains open source modules and integrations within Forloop.ai platform
 Home-page: https://github.com/ForloopAI/forloop_modules
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forloop_modules-1.0.2/forloop_modules.egg-info/SOURCES.txt` & `forloop_modules-1.1.0/forloop_modules.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -62,13 +62,14 @@
 forloop_modules/redis/config/config.py
 forloop_modules/utils/__init__.py
 forloop_modules/utils/definitions.py
 forloop_modules/utils/encryption.py
 forloop_modules/utils/pandas_operations.py
 forloop_modules/utils/pickle_serializer.py
 forloop_modules/utils/script_utils.py
+forloop_modules/utils/sse_parser.py
 forloop_modules/utils/str_helpers.py
 forloop_modules/utils/synchronization_flags.py
 forloop_modules/utils/url_template_builder.py
 forloop_modules/utils/various.py
 tests/__init__.py
 tests/test_url_template_builder.py
```

### Comparing `forloop_modules-1.0.2/setup.py` & `forloop_modules-1.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='forloop_modules',
-    version='1.0.2',
+    version='1.1.0',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='This package contains open source modules and integrations within Forloop.ai platform',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/ForloopAI/forloop_modules',
     packages=setuptools.find_packages(),
```

### Comparing `forloop_modules-1.0.2/tests/test_url_template_builder.py` & `forloop_modules-1.1.0/tests/test_url_template_builder.py`

 * *Files identical despite different names*


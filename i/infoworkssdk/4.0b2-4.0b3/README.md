# Comparing `tmp/infoworkssdk-4.0b2.tar.gz` & `tmp/infoworkssdk-4.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infoworkssdk-4.0b2.tar", last modified: Wed Oct  4 06:10:27 2023, max compression
+gzip compressed data, was "infoworkssdk-4.0b3.tar", last modified: Fri Oct  6 13:26:04 2023, max compression
```

## Comparing `infoworkssdk-4.0b2.tar` & `infoworkssdk-4.0b3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-04 06:10:27.801448 infoworkssdk-4.0b2/
--rw-r--r--   0 infoworks   (501) staff       (20)    35149 2022-12-08 16:36:18.000000 infoworkssdk-4.0b2/LICENSE
--rw-r--r--   0 infoworks   (501) staff       (20)     2441 2023-10-04 06:10:27.801247 infoworkssdk-4.0b2/PKG-INFO
--rw-r--r--   0 infoworks   (501) staff       (20)     1806 2023-01-25 13:55:47.000000 infoworkssdk-4.0b2/README.md
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-04 06:10:27.761215 infoworkssdk-4.0b2/infoworks/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-4.0b2/infoworks/__init__.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-04 06:10:27.761911 infoworkssdk-4.0b2/infoworks/core/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-4.0b2/infoworks/core/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)     3057 2023-04-11 06:44:19.000000 infoworkssdk-4.0b2/infoworks/core/iw_authentication.py
--rw-r--r--   0 infoworks   (501) staff       (20)     1234 2023-06-01 10:05:48.000000 infoworkssdk-4.0b2/infoworks/error.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-04 06:10:27.781625 infoworkssdk-4.0b2/infoworks/sdk/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-4.0b2/infoworks/sdk/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)   113698 2023-10-03 13:33:30.000000 infoworkssdk-4.0b2/infoworks/sdk/admin_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)    11222 2023-04-11 06:44:19.000000 infoworkssdk-4.0b2/infoworks/sdk/base_client.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-04 06:10:27.782321 infoworkssdk-4.0b2/infoworks/sdk/cicd/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-18 15:08:53.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)      544 2022-12-19 09:22:58.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/cicd_response.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-04 06:10:27.791249 infoworkssdk-4.0b2/infoworks/sdk/cicd/download_configurations/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-18 15:08:53.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/download_configurations/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)     5276 2023-08-08 15:52:16.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/download_configurations/get_all_configs_from_domain.py
--rw-r--r--   0 infoworks   (501) staff       (20)     7337 2023-08-08 15:52:16.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/download_configurations/get_entity_configuration_lineage.py
--rw-r--r--   0 infoworks   (501) staff       (20)     3791 2023-10-03 13:33:30.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/download_configurations/get_pipeline_configuration.py
--rw-r--r--   0 infoworks   (501) staff       (20)     2368 2023-08-08 15:52:16.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/download_configurations/get_source_configuration.py
--rw-r--r--   0 infoworks   (501) staff       (20)     2441 2023-08-08 15:52:16.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py
--rw-r--r--   0 infoworks   (501) staff       (20)      987 2022-12-18 15:08:53.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/download_configurations/lineage.py
--rw-r--r--   0 infoworks   (501) staff       (20)    37501 2023-10-03 13:33:30.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/download_configurations/utils.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-04 06:10:27.798736 infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-18 15:08:53.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)    14064 2023-08-08 16:16:36.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/cdata_source.py
--rw-r--r--   0 infoworks   (501) staff       (20)    21776 2023-08-18 09:17:19.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/csv_source.py
--rw-r--r--   0 infoworks   (501) staff       (20)    13654 2023-08-08 16:16:36.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/domains.py
--rw-r--r--   0 infoworks   (501) staff       (20)      185 2023-05-15 06:02:14.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/local_configurations.py
--rw-r--r--   0 infoworks   (501) staff       (20)      517 2022-12-18 15:08:53.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/misc.py
--rw-r--r--   0 infoworks   (501) staff       (20)     7857 2023-08-08 16:16:36.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/pipeline_group.py
--rw-r--r--   0 infoworks   (501) staff       (20)    24801 2023-08-18 09:17:19.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/pipelines.py
--rw-r--r--   0 infoworks   (501) staff       (20)    27544 2023-10-04 06:03:07.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/rdbms_source.py
--rw-r--r--   0 infoworks   (501) staff       (20)    13060 2023-08-08 16:16:36.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/salesforce_source.py
--rw-r--r--   0 infoworks   (501) staff       (20)     2445 2023-08-18 09:17:19.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/update_configurations.py
--rw-r--r--   0 infoworks   (501) staff       (20)    14896 2023-08-08 15:52:16.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/workflow.py
--rw-r--r--   0 infoworks   (501) staff       (20)    23700 2023-08-18 09:17:19.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py
--rw-r--r--   0 infoworks   (501) staff       (20)    30204 2023-10-03 13:33:30.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/wrappersource.py
--rw-r--r--   0 infoworks   (501) staff       (20)    12333 2023-08-08 15:52:16.000000 infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py
--rw-r--r--   0 infoworks   (501) staff       (20)     1729 2023-08-08 16:16:36.000000 infoworkssdk-4.0b2/infoworks/sdk/client.py
--rw-r--r--   0 infoworks   (501) staff       (20)    34243 2023-08-18 09:17:19.000000 infoworkssdk-4.0b2/infoworks/sdk/domain_client.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-04 06:10:27.799156 infoworkssdk-4.0b2/infoworks/sdk/ejson/
--rw-r--r--   0 infoworks   (501) staff       (20)     4435 2022-12-08 16:36:18.000000 infoworkssdk-4.0b2/infoworks/sdk/ejson/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)      547 2023-01-23 12:36:52.000000 infoworkssdk-4.0b2/infoworks/sdk/generic_response.py
--rw-r--r--   0 infoworks   (501) staff       (20)    53262 2023-04-11 06:43:28.000000 infoworkssdk-4.0b2/infoworks/sdk/jobmetrics.py
--rw-r--r--   0 infoworks   (501) staff       (20)    32292 2023-06-20 05:05:38.000000 infoworkssdk-4.0b2/infoworks/sdk/jobs_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)      487 2023-01-10 05:44:03.000000 infoworkssdk-4.0b2/infoworks/sdk/jobs_response.py
--rw-r--r--   0 infoworks   (501) staff       (20)     2216 2023-05-08 06:08:31.000000 infoworkssdk-4.0b2/infoworks/sdk/local_configurations.py
--rw-r--r--   0 infoworks   (501) staff       (20)    66574 2023-10-03 13:33:30.000000 infoworkssdk-4.0b2/infoworks/sdk/pipeline_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)    47632 2023-08-18 09:17:19.000000 infoworkssdk-4.0b2/infoworks/sdk/pipeline_group_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)      593 2022-12-08 16:35:08.000000 infoworkssdk-4.0b2/infoworks/sdk/pipeline_response.py
--rw-r--r--   0 infoworks   (501) staff       (20)    72307 2023-07-18 06:17:15.000000 infoworkssdk-4.0b2/infoworks/sdk/replicator_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)   193543 2023-08-25 14:58:31.000000 infoworkssdk-4.0b2/infoworks/sdk/source_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)      584 2022-12-08 16:35:08.000000 infoworkssdk-4.0b2/infoworks/sdk/source_response.py
--rw-r--r--   0 infoworks   (501) staff       (20)    83469 2023-08-18 09:17:19.000000 infoworkssdk-4.0b2/infoworks/sdk/url_builder.py
--rw-r--r--   0 infoworks   (501) staff       (20)     4479 2022-12-08 16:35:08.000000 infoworkssdk-4.0b2/infoworks/sdk/utils.py
--rw-r--r--   0 infoworks   (501) staff       (20)    67499 2023-08-18 09:17:19.000000 infoworkssdk-4.0b2/infoworks/sdk/workflow_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)      594 2022-12-08 16:35:08.000000 infoworkssdk-4.0b2/infoworks/sdk/workflow_response.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-04 06:10:27.800881 infoworkssdk-4.0b2/infoworkssdk.egg-info/
--rw-r--r--   0 infoworks   (501) staff       (20)     2441 2023-10-04 06:10:27.000000 infoworkssdk-4.0b2/infoworkssdk.egg-info/PKG-INFO
--rw-r--r--   0 infoworks   (501) staff       (20)     2425 2023-10-04 06:10:27.000000 infoworkssdk-4.0b2/infoworkssdk.egg-info/SOURCES.txt
--rw-r--r--   0 infoworks   (501) staff       (20)        1 2023-10-04 06:10:27.000000 infoworkssdk-4.0b2/infoworkssdk.egg-info/dependency_links.txt
--rw-r--r--   0 infoworks   (501) staff       (20)       45 2023-10-04 06:10:27.000000 infoworkssdk-4.0b2/infoworkssdk.egg-info/requires.txt
--rw-r--r--   0 infoworks   (501) staff       (20)       10 2023-10-04 06:10:27.000000 infoworkssdk-4.0b2/infoworkssdk.egg-info/top_level.txt
--rw-r--r--   0 infoworks   (501) staff       (20)       38 2023-10-04 06:10:27.801522 infoworkssdk-4.0b2/setup.cfg
--rw-r--r--   0 infoworks   (501) staff       (20)      907 2023-10-04 06:09:43.000000 infoworkssdk-4.0b2/setup.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-06 13:26:04.508104 infoworkssdk-4.0b3/
+-rw-r--r--   0 infoworks   (501) staff       (20)    35149 2022-12-08 16:36:18.000000 infoworkssdk-4.0b3/LICENSE
+-rw-r--r--   0 infoworks   (501) staff       (20)     2441 2023-10-06 13:26:04.507946 infoworkssdk-4.0b3/PKG-INFO
+-rw-r--r--   0 infoworks   (501) staff       (20)     1806 2023-01-25 13:55:47.000000 infoworkssdk-4.0b3/README.md
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-06 13:26:04.476524 infoworkssdk-4.0b3/infoworks/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-4.0b3/infoworks/__init__.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-06 13:26:04.477156 infoworkssdk-4.0b3/infoworks/core/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-4.0b3/infoworks/core/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     3057 2023-04-11 06:44:19.000000 infoworkssdk-4.0b3/infoworks/core/iw_authentication.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     1234 2023-06-01 10:05:48.000000 infoworkssdk-4.0b3/infoworks/error.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-06 13:26:04.494209 infoworkssdk-4.0b3/infoworks/sdk/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-4.0b3/infoworks/sdk/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)   113698 2023-10-03 13:33:30.000000 infoworkssdk-4.0b3/infoworks/sdk/admin_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    11222 2023-04-11 06:44:19.000000 infoworkssdk-4.0b3/infoworks/sdk/base_client.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-06 13:26:04.494753 infoworkssdk-4.0b3/infoworks/sdk/cicd/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-18 15:08:53.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      544 2022-12-19 09:22:58.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/cicd_response.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-06 13:26:04.498949 infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-18 15:08:53.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     5276 2023-08-08 15:52:16.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/get_all_configs_from_domain.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     7337 2023-08-08 15:52:16.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/get_entity_configuration_lineage.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     3791 2023-10-03 13:33:30.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/get_pipeline_configuration.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     2368 2023-08-08 15:52:16.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/get_source_configuration.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     2441 2023-08-08 15:52:16.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      987 2022-12-18 15:08:53.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/lineage.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    37501 2023-10-03 13:33:30.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/utils.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-06 13:26:04.506388 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-18 15:08:53.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    14064 2023-08-08 16:16:36.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/cdata_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    21776 2023-08-18 09:17:19.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/csv_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    13654 2023-08-08 16:16:36.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/domains.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      185 2023-05-15 06:02:14.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/local_configurations.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      517 2022-12-18 15:08:53.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/misc.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     7857 2023-08-08 16:16:36.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/pipeline_group.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    24801 2023-08-18 09:17:19.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/pipelines.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    28163 2023-10-06 13:25:32.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/rdbms_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    13060 2023-08-08 16:16:36.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/salesforce_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     2445 2023-08-18 09:17:19.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/update_configurations.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    14896 2023-08-08 15:52:16.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/workflow.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    23700 2023-08-18 09:17:19.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    30204 2023-10-03 13:33:30.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/wrappersource.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    12333 2023-08-08 15:52:16.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     1729 2023-08-08 16:16:36.000000 infoworkssdk-4.0b3/infoworks/sdk/client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    34243 2023-08-18 09:17:19.000000 infoworkssdk-4.0b3/infoworks/sdk/domain_client.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-06 13:26:04.506720 infoworkssdk-4.0b3/infoworks/sdk/ejson/
+-rw-r--r--   0 infoworks   (501) staff       (20)     4435 2022-12-08 16:36:18.000000 infoworkssdk-4.0b3/infoworks/sdk/ejson/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      547 2023-01-23 12:36:52.000000 infoworkssdk-4.0b3/infoworks/sdk/generic_response.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    53262 2023-04-11 06:43:28.000000 infoworkssdk-4.0b3/infoworks/sdk/jobmetrics.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    32292 2023-06-20 05:05:38.000000 infoworkssdk-4.0b3/infoworks/sdk/jobs_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      487 2023-01-10 05:44:03.000000 infoworkssdk-4.0b3/infoworks/sdk/jobs_response.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     2216 2023-05-08 06:08:31.000000 infoworkssdk-4.0b3/infoworks/sdk/local_configurations.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    66566 2023-10-06 13:25:32.000000 infoworkssdk-4.0b3/infoworks/sdk/pipeline_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    47632 2023-08-18 09:17:19.000000 infoworkssdk-4.0b3/infoworks/sdk/pipeline_group_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      593 2022-12-08 16:35:08.000000 infoworkssdk-4.0b3/infoworks/sdk/pipeline_response.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    72307 2023-07-18 06:17:15.000000 infoworkssdk-4.0b3/infoworks/sdk/replicator_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)   193543 2023-08-25 14:58:31.000000 infoworkssdk-4.0b3/infoworks/sdk/source_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      584 2022-12-08 16:35:08.000000 infoworkssdk-4.0b3/infoworks/sdk/source_response.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    83469 2023-08-18 09:17:19.000000 infoworkssdk-4.0b3/infoworks/sdk/url_builder.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     4479 2022-12-08 16:35:08.000000 infoworkssdk-4.0b3/infoworks/sdk/utils.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    67499 2023-08-18 09:17:19.000000 infoworkssdk-4.0b3/infoworks/sdk/workflow_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      594 2022-12-08 16:35:08.000000 infoworkssdk-4.0b3/infoworks/sdk/workflow_response.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-06 13:26:04.507675 infoworkssdk-4.0b3/infoworkssdk.egg-info/
+-rw-r--r--   0 infoworks   (501) staff       (20)     2441 2023-10-06 13:26:04.000000 infoworkssdk-4.0b3/infoworkssdk.egg-info/PKG-INFO
+-rw-r--r--   0 infoworks   (501) staff       (20)     2425 2023-10-06 13:26:04.000000 infoworkssdk-4.0b3/infoworkssdk.egg-info/SOURCES.txt
+-rw-r--r--   0 infoworks   (501) staff       (20)        1 2023-10-06 13:26:04.000000 infoworkssdk-4.0b3/infoworkssdk.egg-info/dependency_links.txt
+-rw-r--r--   0 infoworks   (501) staff       (20)       45 2023-10-06 13:26:04.000000 infoworkssdk-4.0b3/infoworkssdk.egg-info/requires.txt
+-rw-r--r--   0 infoworks   (501) staff       (20)       10 2023-10-06 13:26:04.000000 infoworkssdk-4.0b3/infoworkssdk.egg-info/top_level.txt
+-rw-r--r--   0 infoworks   (501) staff       (20)       38 2023-10-06 13:26:04.508195 infoworkssdk-4.0b3/setup.cfg
+-rw-r--r--   0 infoworks   (501) staff       (20)      907 2023-10-06 13:25:24.000000 infoworkssdk-4.0b3/setup.py
```

### Comparing `infoworkssdk-4.0b2/LICENSE` & `infoworkssdk-4.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/PKG-INFO` & `infoworkssdk-4.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infoworkssdk
-Version: 4.0b2
+Version: 4.0b3
 Summary: A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.34 onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-3.0
 Home-page: https://github.com/Infoworks/InfoworksPythonSDK
 Author: Infoworks CE Team
 Author-email: abhishek.raviprasad@infoworks.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `infoworkssdk-4.0b2/README.md` & `infoworkssdk-4.0b3/README.md`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/core/iw_authentication.py` & `infoworkssdk-4.0b3/infoworks/core/iw_authentication.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/error.py` & `infoworkssdk-4.0b3/infoworks/error.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/admin_client.py` & `infoworkssdk-4.0b3/infoworks/sdk/admin_client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/base_client.py` & `infoworkssdk-4.0b3/infoworks/sdk/base_client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/cicd_response.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/cicd_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/download_configurations/get_all_configs_from_domain.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/get_all_configs_from_domain.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/download_configurations/get_entity_configuration_lineage.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/get_entity_configuration_lineage.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/download_configurations/get_pipeline_configuration.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/get_pipeline_configuration.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/download_configurations/get_source_configuration.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/get_source_configuration.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/download_configurations/lineage.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/lineage.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/download_configurations/utils.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/utils.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/cdata_source.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/cdata_source.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/csv_source.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/csv_source.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/domains.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/domains.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/misc.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/misc.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/pipeline_group.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/pipeline_group.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/pipelines.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/pipelines.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/rdbms_source.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/rdbms_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,34 +269,39 @@
         if len(tables_already_added_in_source) > 0:
             for table in tables:
                 if table["configuration"].get("schema_name_at_source",
                                               table["configuration"].get("catalog_name", "")) + "." + \
                         table["configuration"][
                             "name"] not in tables_already_added_in_source:
                     temp = {"table_name": table["configuration"]["name"],
-                            "table_type": table["table_type"].upper(),
+                            "table_type": table.get("table_type","TABLE").upper(),
                             "target_table_name": table["configuration"]["configuration"]["target_table_name"],
                             "target_schema_name": table["configuration"]["configuration"]["target_schema_name"]}
                     if table["configuration"].get("catalog_name", "") != "":
                         temp["catalog_name"] = table["configuration"]["catalog_name"]
                     if table["configuration"].get("schema_name_at_source", "") != "":
                         temp["schema_name"] = table["configuration"]["schema_name_at_source"]
+                    if table["configuration"].get("configuration", {}).get("configuration", {}).get("target_database_name","") != "":
+                        temp["target_database_name"] = table["configuration"]["configuration"]["target_database_name"]
                     tables_list.append(copy.deepcopy(temp))
                     src_client_obj.logger.info(
                         f"Adding table {temp['table_name']} to source {source_id} config payload")
         else:
             for table in tables:
                 temp = {"table_name": table["configuration"]["name"],
-                        "table_type": table["table_type"].upper(),
+                        "table_type": table.get("table_type","TABLE").upper(),
                         "target_table_name": table["configuration"]["configuration"]["target_table_name"],
                         "target_schema_name": table["configuration"]["configuration"]["target_schema_name"]}
                 if table["configuration"].get("catalog_name", "") != "":
                     temp["catalog_name"] = table["configuration"]["catalog_name"]
                 if table["configuration"].get("schema_name_at_source", "") != "":
                     temp["schema_name"] = table["configuration"]["schema_name_at_source"]
+                if table["configuration"].get("configuration", {}).get("configuration", {}).get("target_database_name",
+                                                                                                "") != "":
+                    temp["target_database_name"] = table["configuration"]["configuration"]["target_database_name"]
                 tables_list.append(copy.deepcopy(temp))
                 src_client_obj.logger.info(f"Adding table {temp['table_name']} to source {source_id} config payload")
         if len(tables_list) > 0:
             response = src_client_obj.add_tables_to_source(source_id, tables_list)
             return SourceResponse.parse_result(status=response["result"]["status"].upper(), source_id=source_id,
                                                response=response)
         else:
```

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/salesforce_source.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/salesforce_source.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/update_configurations.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/update_configurations.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/workflow.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/workflow.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/wrappersource.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/wrappersource.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py` & `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/client.py` & `infoworkssdk-4.0b3/infoworks/sdk/client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/domain_client.py` & `infoworkssdk-4.0b3/infoworks/sdk/domain_client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/ejson/__init__.py` & `infoworkssdk-4.0b3/infoworks/sdk/ejson/__init__.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/generic_response.py` & `infoworkssdk-4.0b3/infoworks/sdk/generic_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/jobmetrics.py` & `infoworkssdk-4.0b3/infoworks/sdk/jobmetrics.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/jobs_client.py` & `infoworkssdk-4.0b3/infoworks/sdk/jobs_client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/local_configurations.py` & `infoworkssdk-4.0b3/infoworks/sdk/local_configurations.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/pipeline_client.py` & `infoworkssdk-4.0b3/infoworks/sdk/pipeline_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,19 +387,18 @@
         :param pipeline_version_id: id of the pipeline version that has to be deleted
         :type pipeline_version_id: String
         :return: response dict
         """
         try:
             if None in {pipeline_id, pipeline_version_id, domain_id}:
                 raise Exception(f"pipeline_id, pipeline_version_id, domain_id cannot be None")
-            response = IWUtils.ejson_deserialize(self.call_api("GET", url_builder.delete_pipeline_version_url(
+            response = IWUtils.ejson_deserialize(self.call_api("DELETE", url_builder.delete_pipeline_version_url(
                 self.client_config, domain_id, pipeline_id, pipeline_version_id), IWUtils.get_default_header_for_v3(
                 self.client_config['bearer_token'])).content)
-            result = response.get('result', {})
-            if result.get('id', None) is None:
+            if response.get("message","")!="Successfully removed Pipeline Version":
                 self.logger.error('Failed to delete the pipeline version')
                 return PipelineResponse.parse_result(status=Response.Status.FAILED,
                                                      error_code=ErrorCode.USER_ERROR,
                                                      error_desc='Failed to delete the pipeline version',
                                                      response=response)
             pipeline_version_id = str(pipeline_version_id)
             self.logger.info(
```

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/pipeline_group_client.py` & `infoworkssdk-4.0b3/infoworks/sdk/pipeline_group_client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/pipeline_response.py` & `infoworkssdk-4.0b3/infoworks/sdk/pipeline_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/replicator_client.py` & `infoworkssdk-4.0b3/infoworks/sdk/replicator_client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/source_client.py` & `infoworkssdk-4.0b3/infoworks/sdk/source_client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/source_response.py` & `infoworkssdk-4.0b3/infoworks/sdk/source_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/url_builder.py` & `infoworkssdk-4.0b3/infoworks/sdk/url_builder.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/utils.py` & `infoworkssdk-4.0b3/infoworks/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/workflow_client.py` & `infoworkssdk-4.0b3/infoworks/sdk/workflow_client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworks/sdk/workflow_response.py` & `infoworkssdk-4.0b3/infoworks/sdk/workflow_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/infoworkssdk.egg-info/PKG-INFO` & `infoworkssdk-4.0b3/infoworkssdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infoworkssdk
-Version: 4.0b2
+Version: 4.0b3
 Summary: A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.34 onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-3.0
 Home-page: https://github.com/Infoworks/InfoworksPythonSDK
 Author: Infoworks CE Team
 Author-email: abhishek.raviprasad@infoworks.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `infoworkssdk-4.0b2/infoworkssdk.egg-info/SOURCES.txt` & `infoworkssdk-4.0b3/infoworkssdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b2/setup.py` & `infoworkssdk-4.0b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="infoworkssdk",
-    version="4.0.beta2",
+    version="4.0.beta3",
     author="Infoworks CE Team",
     author_email="abhishek.raviprasad@infoworks.io",
     description="A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.34 onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-3.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Infoworks/InfoworksPythonSDK",
     packages=setuptools.find_packages(),
```


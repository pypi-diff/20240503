# Comparing `tmp/data-repo-client-2.55.0.tar.gz` & `tmp/data-repo-client-2.56.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/jade-data-repo/jade-data-repo/data-repo-client/dist/.tmp-dt08r6jo/data-repo-client-2.55.0.tar", last modified: Tue Apr 30 22:29:24 2024, max compression
+gzip compressed data, was "/home/runner/work/jade-data-repo/jade-data-repo/data-repo-client/dist/.tmp-jufd9l36/data-repo-client-2.56.0.tar", last modified: Fri May  3 14:33:27 2024, max compression
```

## Comparing `data-repo-client-2.55.0.tar` & `data-repo-client-2.56.0.tar`

### file list

```diff
@@ -1,388 +1,388 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:29:24.000000 data-repo-client-2.55.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-30 22:29:24.000000 data-repo-client-2.55.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    43849 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:29:24.000000 data-repo-client-2.55.0/data_repo_client/
--rw-r--r--   0 runner    (1001) docker     (127)    17319 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:29:24.000000 data-repo-client-2.55.0/data_repo_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/api/admin_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/api/configs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    41290 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/api/data_repository_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   261657 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/api/datasets_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22542 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/api/duos_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17614 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/api/journal_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    47273 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/api/profiles_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/api/register_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   470715 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/api/repository_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    47274 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/api/resources_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    31737 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   163156 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/api/snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/api/unauthenticated_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/api/upgrade_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27140 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:29:24.000000 data-repo-client-2.55.0/data_repo_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)    15980 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/access_info_big_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/access_info_big_query_model_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/access_info_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/access_info_parquet_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/access_info_parquet_model_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/add_auth_domain_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/asset_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/billing_profile_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/billing_profile_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/bulk_load_array_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/bulk_load_array_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/bulk_load_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/bulk_load_file_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/bulk_load_file_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/bulk_load_history_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/bulk_load_history_model_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/bulk_load_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/bulk_load_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/cloud_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/column_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/column_statistics_double_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/column_statistics_double_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/column_statistics_int_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/column_statistics_int_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/column_statistics_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/column_statistics_text_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/column_statistics_text_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/column_statistics_text_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/config_enable_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/config_fault_counted_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/config_fault_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/config_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/config_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/config_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/config_parameter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/data_deletion_gcs_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/data_deletion_json_array_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/data_deletion_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/data_deletion_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/dataset_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    22250 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/dataset_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/dataset_request_access_include_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21943 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/dataset_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/dataset_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/dataset_schema_column_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/dataset_schema_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/dataset_schema_update_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/dataset_specification_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/dataset_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/date_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/delete_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/directory_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/drs_access_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/drs_access_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/drs_alias_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/drs_authorizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/drs_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/drs_contents_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/drs_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/drs_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/drs_passport_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/drs_service_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/duos_firecloud_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/duos_firecloud_groups_sync_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/enumerate_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/enumerate_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/enumerate_snapshot_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/enumerate_snapshot_access_request_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/enumerate_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/enumerate_sort_by_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/error_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/file_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/file_load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/file_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/iam_resource_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/inaccessible_workspace_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    28228 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/ingest_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/ingest_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/int_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/job_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/journal_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/policy_member_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/policy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/query_column_statistics_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/query_data_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/relationship_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/relationship_term_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/repository_configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/repository_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/repository_status_model_systems.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/resource_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/resource_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/sam_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12433 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_access_request_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_access_request_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_count_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_count_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_count_response_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_criteria_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_dataset_concept_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_domain_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_domain_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_domain_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_domain_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_feature_value_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_get_concepts_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_parent_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_list_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_list_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_list_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_range_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_range_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_range_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_range_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_export_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_export_response_model_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_ids_and_roles_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_link_duos_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    21041 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_preview_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_request_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_request_contents_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_request_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_request_row_id_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_request_row_id_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_retrieve_include_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_source_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19078 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/snapshot_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/sql_sort_direction_asc_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/sql_sort_direction_desc_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/storage_resource_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/table_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/tag_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/tag_count_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/tag_update_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/transaction_close_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/transaction_create_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/transaction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/unlock_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/upgrade_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/upgrade_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/user_status_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/data_repo_client/models/workspace_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/data_repo_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:29:24.000000 data-repo-client-2.55.0/data_repo_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-30 22:29:24.000000 data-repo-client-2.55.0/data_repo_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17311 2024-04-30 22:29:24.000000 data-repo-client-2.55.0/data_repo_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 22:29:24.000000 data-repo-client-2.55.0/data_repo_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 22:29:24.000000 data-repo-client-2.55.0/data_repo_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 22:29:24.000000 data-repo-client-2.55.0/data_repo_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 22:29:24.000000 data-repo-client-2.55.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:29:24.000000 data-repo-client-2.55.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_access_info_big_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_access_info_big_query_model_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_access_info_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_access_info_parquet_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_access_info_parquet_model_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_add_auth_domain_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/test/test_admin_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_asset_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_billing_profile_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_billing_profile_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_bulk_load_array_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_bulk_load_array_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_bulk_load_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_bulk_load_file_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_bulk_load_file_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_bulk_load_history_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_bulk_load_history_model_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_bulk_load_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_bulk_load_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_cloud_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_column_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_column_statistics_double_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_column_statistics_double_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_column_statistics_int_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_column_statistics_int_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_column_statistics_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_column_statistics_text_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_column_statistics_text_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_column_statistics_text_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_config_enable_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_config_fault_counted_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_config_fault_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_config_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_config_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_config_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_config_parameter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/test/test_configs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_data_deletion_gcs_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_data_deletion_json_array_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_data_deletion_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_data_deletion_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/test/test_data_repository_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_dataset_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_dataset_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_dataset_request_access_include_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_dataset_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_dataset_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_dataset_schema_column_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_dataset_schema_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_dataset_schema_update_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_dataset_specification_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_dataset_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/test/test_datasets_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_date_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_delete_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_directory_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_drs_access_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_drs_access_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_drs_alias_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_drs_authorizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_drs_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_drs_contents_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_drs_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_drs_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_drs_passport_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_drs_service_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/test/test_duos_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_duos_firecloud_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_duos_firecloud_groups_sync_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_enumerate_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_enumerate_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_enumerate_snapshot_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_enumerate_snapshot_access_request_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_enumerate_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_enumerate_sort_by_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_error_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_file_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_file_load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_file_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_iam_resource_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_inaccessible_workspace_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_ingest_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_ingest_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_int_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_job_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/test/test_jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/test/test_journal_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_journal_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_policy_member_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_policy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/test/test_profiles_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_query_column_statistics_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_query_data_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/test/test_register_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_relationship_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_relationship_term_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/test/test_repository_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_repository_configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_repository_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_repository_status_model_systems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_resource_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_resource_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/test/test_resources_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_sam_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/test/test_search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_access_request_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_access_request_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_count_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_count_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_count_response_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_criteria_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_dataset_concept_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_domain_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_domain_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_domain_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_domain_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_feature_value_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_get_concept_hierarchy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_get_concepts_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_parent_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_program_data_list_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_program_data_list_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_program_data_list_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_program_data_list_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_program_data_list_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_program_data_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_program_data_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_program_data_range_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_program_data_range_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_program_data_range_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_program_data_range_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_builder_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_export_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_export_response_model_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_export_response_model_format_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_export_response_model_format_parquet_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_export_response_model_format_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_ids_and_roles_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_link_duos_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_preview_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_request_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_request_contents_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_request_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_request_row_id_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_request_row_id_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_retrieve_include_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_source_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_snapshot_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/test/test_snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_sql_sort_direction_asc_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_sql_sort_direction_desc_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_storage_resource_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_table_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_tag_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_tag_count_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_tag_update_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_transaction_close_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_transaction_create_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_transaction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/test/test_unauthenticated_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_unlock_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-30 22:29:21.000000 data-repo-client-2.55.0/test/test_upgrade_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_upgrade_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_upgrade_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_user_status_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-30 22:29:20.000000 data-repo-client-2.55.0/test/test_workspace_policy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:27.000000 data-repo-client-2.56.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-03 14:33:27.000000 data-repo-client-2.56.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    43829 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:27.000000 data-repo-client-2.56.0/data_repo_client/
+-rw-r--r--   0 runner    (1001) docker     (127)    17295 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:27.000000 data-repo-client-2.56.0/data_repo_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/api/admin_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/api/configs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41290 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/api/data_repository_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   250524 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/api/datasets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22542 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/api/duos_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17614 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/api/journal_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47273 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/api/profiles_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/api/register_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   470715 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/api/repository_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47274 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/api/resources_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31737 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11578 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/api/snapshot_access_request_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   163156 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/api/snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/api/unauthenticated_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/api/upgrade_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27140 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:27.000000 data-repo-client-2.56.0/data_repo_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    15870 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/access_info_big_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/access_info_big_query_model_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/access_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/access_info_parquet_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/access_info_parquet_model_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/add_auth_domain_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/asset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/asset_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/billing_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/billing_profile_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/billing_profile_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/bulk_load_array_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/bulk_load_array_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/bulk_load_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/bulk_load_file_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/bulk_load_file_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/bulk_load_history_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/bulk_load_history_model_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/bulk_load_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/bulk_load_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/cloud_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/column_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/column_statistics_double_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/column_statistics_double_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/column_statistics_int_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/column_statistics_int_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/column_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/column_statistics_text_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/column_statistics_text_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/column_statistics_text_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/config_enable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/config_fault_counted_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/config_fault_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/config_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/config_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/config_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/config_parameter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/data_deletion_gcs_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/data_deletion_json_array_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/data_deletion_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/data_deletion_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/dataset_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22250 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/dataset_patch_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/dataset_request_access_include_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21943 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/dataset_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/dataset_request_model_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/dataset_schema_column_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/dataset_schema_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/dataset_schema_update_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/dataset_specification_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/dataset_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/date_partition_options_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/delete_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/directory_detail_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/drs_access_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/drs_access_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/drs_alias_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/drs_authorizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/drs_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/drs_contents_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/drs_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/drs_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/drs_passport_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/data_repo_client/models/drs_service_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/duos_firecloud_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/duos_firecloud_groups_sync_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/enumerate_billing_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/enumerate_dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/enumerate_snapshot_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/enumerate_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/enumerate_sort_by_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/error_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/file_detail_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/file_load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/file_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/iam_resource_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/inaccessible_workspace_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28228 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/ingest_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/ingest_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/int_partition_options_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/job_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/journal_entry_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/policy_member_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/policy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/query_column_statistics_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/query_data_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/relationship_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/relationship_term_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/repository_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/repository_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/repository_status_model_systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/resource_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/resource_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/sam_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12433 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_access_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_access_request_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_count_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_count_response_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_criteria_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_dataset_concept_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_domain_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_domain_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_domain_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_domain_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_feature_value_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_get_concepts_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_parent_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_list_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_list_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_range_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_range_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_range_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_range_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_export_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_export_response_model_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_ids_and_roles_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_link_duos_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21041 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_patch_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_preview_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_request_asset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_request_contents_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_request_model_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_request_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_request_row_id_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_request_row_id_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_retrieve_include_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19078 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/snapshot_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/sql_sort_direction_asc_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/sql_sort_direction_desc_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/storage_resource_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/table_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/tag_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/tag_count_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/tag_update_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/transaction_close_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/transaction_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/transaction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/unlock_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/upgrade_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/upgrade_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/user_status_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/models/workspace_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/data_repo_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:27.000000 data-repo-client-2.56.0/data_repo_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-03 14:33:27.000000 data-repo-client-2.56.0/data_repo_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17286 2024-05-03 14:33:27.000000 data-repo-client-2.56.0/data_repo_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:33:27.000000 data-repo-client-2.56.0/data_repo_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 14:33:27.000000 data-repo-client-2.56.0/data_repo_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 14:33:27.000000 data-repo-client-2.56.0/data_repo_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-03 14:33:27.000000 data-repo-client-2.56.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:27.000000 data-repo-client-2.56.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_access_info_big_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_access_info_big_query_model_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_access_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_access_info_parquet_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_access_info_parquet_model_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_add_auth_domain_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_admin_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_asset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_asset_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_billing_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_billing_profile_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_billing_profile_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_bulk_load_array_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_bulk_load_array_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_bulk_load_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_bulk_load_file_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_bulk_load_file_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_bulk_load_history_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_bulk_load_history_model_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_bulk_load_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_bulk_load_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_cloud_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_column_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_column_statistics_double_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_column_statistics_double_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_column_statistics_int_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_column_statistics_int_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_column_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_column_statistics_text_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_column_statistics_text_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_column_statistics_text_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_config_enable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_config_fault_counted_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_config_fault_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_config_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_config_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_config_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_config_parameter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_configs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_data_deletion_gcs_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_data_deletion_json_array_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_data_deletion_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_data_deletion_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_data_repository_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_dataset_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_dataset_patch_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_dataset_request_access_include_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_dataset_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_dataset_request_model_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_dataset_schema_column_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_dataset_schema_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_dataset_schema_update_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_dataset_specification_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_dataset_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_datasets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_date_partition_options_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_delete_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_directory_detail_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_drs_access_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_drs_access_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_drs_alias_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_drs_authorizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_drs_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_drs_contents_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_drs_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_drs_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_drs_passport_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-03 14:33:20.000000 data-repo-client-2.56.0/test/test_drs_service_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_duos_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_duos_firecloud_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_duos_firecloud_groups_sync_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_enumerate_billing_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_enumerate_dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_enumerate_snapshot_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_enumerate_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_enumerate_sort_by_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_error_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_file_detail_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_file_load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_file_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_iam_resource_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_inaccessible_workspace_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_ingest_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_ingest_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_int_partition_options_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_job_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_journal_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_journal_entry_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_policy_member_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_policy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_profiles_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_query_column_statistics_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_query_data_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_register_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_relationship_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_relationship_term_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_repository_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_repository_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_repository_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_repository_status_model_systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_resource_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_resource_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_resources_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_sam_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_access_request_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_access_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_access_request_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_count_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_count_response_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_criteria_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_dataset_concept_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_domain_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_domain_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_domain_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_domain_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_feature_value_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_get_concept_hierarchy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_get_concepts_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_parent_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_program_data_list_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_program_data_list_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_program_data_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_program_data_list_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_program_data_list_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_program_data_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_program_data_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_program_data_range_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_program_data_range_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_program_data_range_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_program_data_range_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_builder_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_export_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_export_response_model_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_export_response_model_format_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_export_response_model_format_parquet_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_export_response_model_format_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_ids_and_roles_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_link_duos_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_patch_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_preview_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_request_asset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_request_contents_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_request_model_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_request_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_request_row_id_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_request_row_id_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_retrieve_include_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshot_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_sql_sort_direction_asc_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_sql_sort_direction_desc_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_storage_resource_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_table_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_tag_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_tag_count_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_tag_update_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_transaction_close_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_transaction_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_transaction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_unauthenticated_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_unlock_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_upgrade_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_upgrade_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_upgrade_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_user_status_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-03 14:33:21.000000 data-repo-client-2.56.0/test/test_workspace_policy_model.py
```

### Comparing `data-repo-client-2.55.0/PKG-INFO` & `data-repo-client-2.56.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-repo-client
-Version: 2.55.0
+Version: 2.56.0
 Summary: Data Repository API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,Data Repository API
```

### Comparing `data-repo-client-2.55.0/README.md` & `data-repo-client-2.56.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1.0
-- Package version: 2.55.0
+- Package version: 2.56.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -105,34 +105,34 @@
 ------------ | ------------- | ------------- | -------------
 *DataRepositoryServiceApi* | [**get_access_url**](docs/DataRepositoryServiceApi.md#get_access_url) | **GET** /ga4gh/drs/v1/objects/{object_id}/access/{access_id} | Get a URL for fetching bytes.
 *DataRepositoryServiceApi* | [**get_object**](docs/DataRepositoryServiceApi.md#get_object) | **GET** /ga4gh/drs/v1/objects/{object_id} | Get info about an &#x60;Object&#x60;.
 *DataRepositoryServiceApi* | [**get_service_info**](docs/DataRepositoryServiceApi.md#get_service_info) | **GET** /ga4gh/drs/v1/service-info | Get information about this implementation.
 *DataRepositoryServiceApi* | [**options_object**](docs/DataRepositoryServiceApi.md#options_object) | **OPTIONS** /ga4gh/drs/v1/objects/{object_id} | Get Authorization info about a DRS Object.
 *DataRepositoryServiceApi* | [**post_access_url**](docs/DataRepositoryServiceApi.md#post_access_url) | **POST** /ga4gh/drs/v1/objects/{object_id}/access/{access_id} | Get a URL for fetching bytes through POST&#39;ing a Passport
 *DataRepositoryServiceApi* | [**post_object**](docs/DataRepositoryServiceApi.md#post_object) | **POST** /ga4gh/drs/v1/objects/{object_id} | Get info about a DrsObject through POST&#39;ing a Passport.
+*SnapshotAccessRequestApi* | [**create_snapshot_access_request**](docs/SnapshotAccessRequestApi.md#create_snapshot_access_request) | **POST** /api/repository/v1/snapshotAccessRequests | 
+*SnapshotAccessRequestApi* | [**enumerate_snapshot_access_requests**](docs/SnapshotAccessRequestApi.md#enumerate_snapshot_access_requests) | **GET** /api/repository/v1/snapshotAccessRequests | 
 *AdminApi* | [**register_drs_aliases**](docs/AdminApi.md#register_drs_aliases) | **POST** /api/repository/v1/admin/register-drs-aliases | 
 *ConfigsApi* | [**get_config**](docs/ConfigsApi.md#get_config) | **GET** /api/repository/v1/configs/{name} | 
 *ConfigsApi* | [**get_config_list**](docs/ConfigsApi.md#get_config_list) | **GET** /api/repository/v1/configs | 
 *ConfigsApi* | [**reset_config**](docs/ConfigsApi.md#reset_config) | **PUT** /api/repository/v1/configs/reset | 
 *ConfigsApi* | [**set_config_list**](docs/ConfigsApi.md#set_config_list) | **PUT** /api/repository/v1/configs | 
 *ConfigsApi* | [**set_fault**](docs/ConfigsApi.md#set_fault) | **PUT** /api/repository/v1/configs/{name} | 
 *DatasetsApi* | [**add_dataset_asset_specifications**](docs/DatasetsApi.md#add_dataset_asset_specifications) | **POST** /api/repository/v1/datasets/{id}/assets | 
 *DatasetsApi* | [**add_dataset_policy_member**](docs/DatasetsApi.md#add_dataset_policy_member) | **POST** /api/repository/v1/datasets/{id}/policies/{policyName}/members | 
 *DatasetsApi* | [**apply_dataset_data_deletion**](docs/DatasetsApi.md#apply_dataset_data_deletion) | **POST** /api/repository/v1/datasets/{id}/deletes | 
 *DatasetsApi* | [**bulk_file_load**](docs/DatasetsApi.md#bulk_file_load) | **POST** /api/repository/v1/datasets/{id}/files/bulk | 
 *DatasetsApi* | [**bulk_file_load_array**](docs/DatasetsApi.md#bulk_file_load_array) | **POST** /api/repository/v1/datasets/{id}/files/bulk/array | 
 *DatasetsApi* | [**bulk_file_results_delete**](docs/DatasetsApi.md#bulk_file_results_delete) | **DELETE** /api/repository/v1/datasets/{id}/files/bulk/{loadTag} | 
 *DatasetsApi* | [**close_transaction**](docs/DatasetsApi.md#close_transaction) | **POST** /api/repository/v1/datasets/{id}/transactions/{transactionId} | 
 *DatasetsApi* | [**create_dataset**](docs/DatasetsApi.md#create_dataset) | **POST** /api/repository/v1/datasets | 
-*DatasetsApi* | [**create_snapshot_request**](docs/DatasetsApi.md#create_snapshot_request) | **POST** /api/repository/v1/datasets/{id}/snapshotRequests | 
 *DatasetsApi* | [**delete_dataset**](docs/DatasetsApi.md#delete_dataset) | **DELETE** /api/repository/v1/datasets/{id} | 
 *DatasetsApi* | [**delete_dataset_policy_member**](docs/DatasetsApi.md#delete_dataset_policy_member) | **DELETE** /api/repository/v1/datasets/{id}/policies/{policyName}/members/{memberEmail} | 
 *DatasetsApi* | [**delete_file**](docs/DatasetsApi.md#delete_file) | **DELETE** /api/repository/v1/datasets/{id}/files/{fileid} | 
 *DatasetsApi* | [**enumerate_datasets**](docs/DatasetsApi.md#enumerate_datasets) | **GET** /api/repository/v1/datasets | 
-*DatasetsApi* | [**enumerate_snapshot_requests**](docs/DatasetsApi.md#enumerate_snapshot_requests) | **GET** /api/repository/v1/datasets/{id}/snapshotRequests | 
 *DatasetsApi* | [**enumerate_transactions**](docs/DatasetsApi.md#enumerate_transactions) | **GET** /api/repository/v1/datasets/{id}/transactions | 
 *DatasetsApi* | [**get_concept_hierarchy**](docs/DatasetsApi.md#get_concept_hierarchy) | **GET** /api/repository/v1/datasets/{id}/snapshotBuilder/conceptHierarchy/{conceptId} | 
 *DatasetsApi* | [**get_concepts**](docs/DatasetsApi.md#get_concepts) | **GET** /api/repository/v1/datasets/{id}/snapshotBuilder/concepts/{conceptId} | 
 *DatasetsApi* | [**get_dataset_tags**](docs/DatasetsApi.md#get_dataset_tags) | **GET** /api/repository/v1/datasets/tags | 
 *DatasetsApi* | [**get_load_history_for_load_tag**](docs/DatasetsApi.md#get_load_history_for_load_tag) | **GET** /api/repository/v1/datasets/{id}/files/bulk/{loadTag} | 
 *DatasetsApi* | [**get_snapshot_builder_count**](docs/DatasetsApi.md#get_snapshot_builder_count) | **POST** /api/repository/v1/datasets/{id}/snapshotBuilder/count | 
 *DatasetsApi* | [**ingest_dataset**](docs/DatasetsApi.md#ingest_dataset) | **POST** /api/repository/v1/datasets/{id}/ingest | 
@@ -369,15 +369,14 @@
  - [DirectoryDetailModel](docs/DirectoryDetailModel.md)
  - [DrsAliasModel](docs/DrsAliasModel.md)
  - [DuosFirecloudGroupModel](docs/DuosFirecloudGroupModel.md)
  - [DuosFirecloudGroupsSyncResponse](docs/DuosFirecloudGroupsSyncResponse.md)
  - [EnumerateBillingProfileModel](docs/EnumerateBillingProfileModel.md)
  - [EnumerateDatasetModel](docs/EnumerateDatasetModel.md)
  - [EnumerateSnapshotAccessRequest](docs/EnumerateSnapshotAccessRequest.md)
- - [EnumerateSnapshotAccessRequestItem](docs/EnumerateSnapshotAccessRequestItem.md)
  - [EnumerateSnapshotModel](docs/EnumerateSnapshotModel.md)
  - [EnumerateSortByParam](docs/EnumerateSortByParam.md)
  - [ErrorModel](docs/ErrorModel.md)
  - [FileDetailModel](docs/FileDetailModel.md)
  - [FileLoadModel](docs/FileLoadModel.md)
  - [FileModel](docs/FileModel.md)
  - [FileModelType](docs/FileModelType.md)
```

### Comparing `data-repo-client-2.55.0/data_repo_client/__init__.py` & `data-repo-client-2.56.0/data_repo_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,19 @@
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "2.55.0"
+__version__ = "2.56.0"
 
 # import apis into sdk package
 from data_repo_client.api.data_repository_service_api import DataRepositoryServiceApi
+from data_repo_client.api.snapshot_access_request_api import SnapshotAccessRequestApi
 from data_repo_client.api.admin_api import AdminApi
 from data_repo_client.api.configs_api import ConfigsApi
 from data_repo_client.api.datasets_api import DatasetsApi
 from data_repo_client.api.duos_api import DuosApi
 from data_repo_client.api.jobs_api import JobsApi
 from data_repo_client.api.journal_api import JournalApi
 from data_repo_client.api.profiles_api import ProfilesApi
@@ -108,15 +109,14 @@
 from data_repo_client.models.directory_detail_model import DirectoryDetailModel
 from data_repo_client.models.drs_alias_model import DrsAliasModel
 from data_repo_client.models.duos_firecloud_group_model import DuosFirecloudGroupModel
 from data_repo_client.models.duos_firecloud_groups_sync_response import DuosFirecloudGroupsSyncResponse
 from data_repo_client.models.enumerate_billing_profile_model import EnumerateBillingProfileModel
 from data_repo_client.models.enumerate_dataset_model import EnumerateDatasetModel
 from data_repo_client.models.enumerate_snapshot_access_request import EnumerateSnapshotAccessRequest
-from data_repo_client.models.enumerate_snapshot_access_request_item import EnumerateSnapshotAccessRequestItem
 from data_repo_client.models.enumerate_snapshot_model import EnumerateSnapshotModel
 from data_repo_client.models.enumerate_sort_by_param import EnumerateSortByParam
 from data_repo_client.models.error_model import ErrorModel
 from data_repo_client.models.file_detail_model import FileDetailModel
 from data_repo_client.models.file_load_model import FileLoadModel
 from data_repo_client.models.file_model import FileModel
 from data_repo_client.models.file_model_type import FileModelType
```

### Comparing `data-repo-client-2.55.0/data_repo_client/api/__init__.py` & `data-repo-client-2.56.0/data_repo_client/api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import absolute_import
 
 # flake8: noqa
 
 # import apis into api package
 from data_repo_client.api.data_repository_service_api import DataRepositoryServiceApi
+from data_repo_client.api.snapshot_access_request_api import SnapshotAccessRequestApi
 from data_repo_client.api.admin_api import AdminApi
 from data_repo_client.api.configs_api import ConfigsApi
 from data_repo_client.api.datasets_api import DatasetsApi
 from data_repo_client.api.duos_api import DuosApi
 from data_repo_client.api.jobs_api import JobsApi
 from data_repo_client.api.journal_api import JournalApi
 from data_repo_client.api.profiles_api import ProfilesApi
```

### Comparing `data-repo-client-2.55.0/data_repo_client/api/admin_api.py` & `data-repo-client-2.56.0/data_repo_client/api/admin_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/api/configs_api.py` & `data-repo-client-2.56.0/data_repo_client/api/configs_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/api/data_repository_service_api.py` & `data-repo-client-2.56.0/data_repo_client/api/data_repository_service_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/api/datasets_api.py` & `data-repo-client-2.56.0/data_repo_client/api/datasets_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1030,137 +1030,14 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def create_snapshot_request(self, id, **kwargs):  # noqa: E501
-        """create_snapshot_request  # noqa: E501
-
-        As a researcher, create a snapshot request for a dataset, given a set of criteria and required concept sets and values.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.create_snapshot_request(id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param str id: A UUID to used to identify an object in the repository (required)
-        :param SnapshotAccessRequest snapshot_access_request: Description of the snapshot being requested.
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: SnapshotAccessRequestResponse
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.create_snapshot_request_with_http_info(id, **kwargs)  # noqa: E501
-
-    def create_snapshot_request_with_http_info(self, id, **kwargs):  # noqa: E501
-        """create_snapshot_request  # noqa: E501
-
-        As a researcher, create a snapshot request for a dataset, given a set of criteria and required concept sets and values.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.create_snapshot_request_with_http_info(id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param str id: A UUID to used to identify an object in the repository (required)
-        :param SnapshotAccessRequest snapshot_access_request: Description of the snapshot being requested.
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: tuple(SnapshotAccessRequestResponse, status_code(int), headers(HTTPHeaderDict))
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'id',
-            'snapshot_access_request'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method create_snapshot_request" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `create_snapshot_request`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        if 'snapshot_access_request' in local_var_params:
-            body_params = local_var_params['snapshot_access_request']
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['oidc']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/snapshotRequests', 'POST',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='SnapshotAccessRequestResponse',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
     def delete_dataset(self, id, **kwargs):  # noqa: E501
         """delete_dataset  # noqa: E501
 
         Delete a dataset by id  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.delete_dataset(id, async_req=True)
@@ -1663,128 +1540,14 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def enumerate_snapshot_requests(self, id, **kwargs):  # noqa: E501
-        """enumerate_snapshot_requests  # noqa: E501
-
-        As an admin for this dataset, view all snapshot requests for this dataset.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.enumerate_snapshot_requests(id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param str id: A UUID to used to identify an object in the repository (required)
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: EnumerateSnapshotAccessRequest
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.enumerate_snapshot_requests_with_http_info(id, **kwargs)  # noqa: E501
-
-    def enumerate_snapshot_requests_with_http_info(self, id, **kwargs):  # noqa: E501
-        """enumerate_snapshot_requests  # noqa: E501
-
-        As an admin for this dataset, view all snapshot requests for this dataset.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.enumerate_snapshot_requests_with_http_info(id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param str id: A UUID to used to identify an object in the repository (required)
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: tuple(EnumerateSnapshotAccessRequest, status_code(int), headers(HTTPHeaderDict))
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'id'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method enumerate_snapshot_requests" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `enumerate_snapshot_requests`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['oidc']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/snapshotRequests', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='EnumerateSnapshotAccessRequest',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
     def enumerate_transactions(self, id, **kwargs):  # noqa: E501
         """enumerate_transactions  # noqa: E501
 
         Lists transactions on the dataset  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.enumerate_transactions(id, async_req=True)
```

### Comparing `data-repo-client-2.55.0/data_repo_client/api/duos_api.py` & `data-repo-client-2.56.0/data_repo_client/api/duos_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/api/jobs_api.py` & `data-repo-client-2.56.0/data_repo_client/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/api/journal_api.py` & `data-repo-client-2.56.0/data_repo_client/api/journal_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/api/profiles_api.py` & `data-repo-client-2.56.0/data_repo_client/api/profiles_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/api/register_api.py` & `data-repo-client-2.56.0/data_repo_client/api/register_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/api/repository_api.py` & `data-repo-client-2.56.0/data_repo_client/api/repository_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/api/resources_api.py` & `data-repo-client-2.56.0/data_repo_client/api/resources_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/api/search_api.py` & `data-repo-client-2.56.0/data_repo_client/api/search_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/api/snapshots_api.py` & `data-repo-client-2.56.0/data_repo_client/api/snapshots_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/api/unauthenticated_api.py` & `data-repo-client-2.56.0/data_repo_client/api/unauthenticated_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/api/upgrade_api.py` & `data-repo-client-2.56.0/data_repo_client/api/upgrade_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/api_client.py` & `data-repo-client-2.56.0/data_repo_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.55.0/python'
+        self.user_agent = 'OpenAPI-Generator/2.56.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `data-repo-client-2.55.0/data_repo_client/configuration.py` & `data-repo-client-2.56.0/data_repo_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1.0\n"\
-               "SDK Package Version: 2.55.0".\
+               "SDK Package Version: 2.56.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `data-repo-client-2.55.0/data_repo_client/exceptions.py` & `data-repo-client-2.56.0/data_repo_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/__init__.py` & `data-repo-client-2.56.0/data_repo_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,14 @@
 from data_repo_client.models.directory_detail_model import DirectoryDetailModel
 from data_repo_client.models.drs_alias_model import DrsAliasModel
 from data_repo_client.models.duos_firecloud_group_model import DuosFirecloudGroupModel
 from data_repo_client.models.duos_firecloud_groups_sync_response import DuosFirecloudGroupsSyncResponse
 from data_repo_client.models.enumerate_billing_profile_model import EnumerateBillingProfileModel
 from data_repo_client.models.enumerate_dataset_model import EnumerateDatasetModel
 from data_repo_client.models.enumerate_snapshot_access_request import EnumerateSnapshotAccessRequest
-from data_repo_client.models.enumerate_snapshot_access_request_item import EnumerateSnapshotAccessRequestItem
 from data_repo_client.models.enumerate_snapshot_model import EnumerateSnapshotModel
 from data_repo_client.models.enumerate_sort_by_param import EnumerateSortByParam
 from data_repo_client.models.error_model import ErrorModel
 from data_repo_client.models.file_detail_model import FileDetailModel
 from data_repo_client.models.file_load_model import FileLoadModel
 from data_repo_client.models.file_model import FileModel
 from data_repo_client.models.file_model_type import FileModelType
```

### Comparing `data-repo-client-2.55.0/data_repo_client/models/access_info_big_query_model.py` & `data-repo-client-2.56.0/data_repo_client/models/access_info_big_query_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/access_info_big_query_model_table.py` & `data-repo-client-2.56.0/data_repo_client/models/access_info_big_query_model_table.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/access_info_model.py` & `data-repo-client-2.56.0/data_repo_client/models/access_info_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/access_info_parquet_model.py` & `data-repo-client-2.56.0/data_repo_client/models/access_info_parquet_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/access_info_parquet_model_table.py` & `data-repo-client-2.56.0/data_repo_client/models/access_info_parquet_model_table.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/add_auth_domain_response_model.py` & `data-repo-client-2.56.0/data_repo_client/models/add_auth_domain_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/asset_model.py` & `data-repo-client-2.56.0/data_repo_client/models/asset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/asset_table_model.py` & `data-repo-client-2.56.0/data_repo_client/models/asset_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/billing_profile_model.py` & `data-repo-client-2.56.0/data_repo_client/models/billing_profile_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/billing_profile_request_model.py` & `data-repo-client-2.56.0/data_repo_client/models/billing_profile_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/billing_profile_update_model.py` & `data-repo-client-2.56.0/data_repo_client/models/billing_profile_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/bulk_load_array_request_model.py` & `data-repo-client-2.56.0/data_repo_client/models/bulk_load_array_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/bulk_load_array_result_model.py` & `data-repo-client-2.56.0/data_repo_client/models/bulk_load_array_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/bulk_load_file_model.py` & `data-repo-client-2.56.0/data_repo_client/models/bulk_load_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/bulk_load_file_result_model.py` & `data-repo-client-2.56.0/data_repo_client/models/bulk_load_file_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/bulk_load_file_state.py` & `data-repo-client-2.56.0/data_repo_client/models/bulk_load_file_state.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/bulk_load_history_model.py` & `data-repo-client-2.56.0/data_repo_client/models/bulk_load_history_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/bulk_load_history_model_list.py` & `data-repo-client-2.56.0/data_repo_client/models/bulk_load_history_model_list.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/bulk_load_request_model.py` & `data-repo-client-2.56.0/data_repo_client/models/bulk_load_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/bulk_load_result_model.py` & `data-repo-client-2.56.0/data_repo_client/models/bulk_load_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/cloud_platform.py` & `data-repo-client-2.56.0/data_repo_client/models/cloud_platform.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/column_model.py` & `data-repo-client-2.56.0/data_repo_client/models/column_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/column_statistics_double_model.py` & `data-repo-client-2.56.0/data_repo_client/models/column_statistics_double_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/column_statistics_double_model_all_of.py` & `data-repo-client-2.56.0/data_repo_client/models/column_statistics_double_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/column_statistics_int_model.py` & `data-repo-client-2.56.0/data_repo_client/models/column_statistics_int_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/column_statistics_int_model_all_of.py` & `data-repo-client-2.56.0/data_repo_client/models/column_statistics_int_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/column_statistics_model.py` & `data-repo-client-2.56.0/data_repo_client/models/column_statistics_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/column_statistics_text_model.py` & `data-repo-client-2.56.0/data_repo_client/models/column_statistics_text_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/column_statistics_text_model_all_of.py` & `data-repo-client-2.56.0/data_repo_client/models/column_statistics_text_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/column_statistics_text_value.py` & `data-repo-client-2.56.0/data_repo_client/models/column_statistics_text_value.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/config_enable_model.py` & `data-repo-client-2.56.0/data_repo_client/models/config_enable_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/config_fault_counted_model.py` & `data-repo-client-2.56.0/data_repo_client/models/config_fault_counted_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/config_fault_model.py` & `data-repo-client-2.56.0/data_repo_client/models/config_fault_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/config_group_model.py` & `data-repo-client-2.56.0/data_repo_client/models/config_group_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/config_list_model.py` & `data-repo-client-2.56.0/data_repo_client/models/config_list_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/config_model.py` & `data-repo-client-2.56.0/data_repo_client/models/config_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/config_parameter_model.py` & `data-repo-client-2.56.0/data_repo_client/models/config_parameter_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/data_deletion_gcs_file_model.py` & `data-repo-client-2.56.0/data_repo_client/models/data_deletion_gcs_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/data_deletion_json_array_model.py` & `data-repo-client-2.56.0/data_repo_client/models/data_deletion_json_array_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/data_deletion_request.py` & `data-repo-client-2.56.0/data_repo_client/models/data_deletion_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/data_deletion_table_model.py` & `data-repo-client-2.56.0/data_repo_client/models/data_deletion_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/dataset_data_model.py` & `data-repo-client-2.56.0/data_repo_client/models/dataset_data_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/dataset_model.py` & `data-repo-client-2.56.0/data_repo_client/models/dataset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/dataset_patch_request_model.py` & `data-repo-client-2.56.0/data_repo_client/models/dataset_patch_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/dataset_request_access_include_model.py` & `data-repo-client-2.56.0/data_repo_client/models/dataset_request_access_include_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/dataset_request_model.py` & `data-repo-client-2.56.0/data_repo_client/models/dataset_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/dataset_request_model_policies.py` & `data-repo-client-2.56.0/data_repo_client/models/dataset_request_model_policies.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/dataset_schema_column_update_model.py` & `data-repo-client-2.56.0/data_repo_client/models/dataset_schema_column_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/dataset_schema_update_model.py` & `data-repo-client-2.56.0/data_repo_client/models/dataset_schema_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/dataset_schema_update_model_changes.py` & `data-repo-client-2.56.0/data_repo_client/models/dataset_schema_update_model_changes.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/dataset_specification_model.py` & `data-repo-client-2.56.0/data_repo_client/models/dataset_specification_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/dataset_summary_model.py` & `data-repo-client-2.56.0/data_repo_client/models/dataset_summary_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/date_partition_options_model.py` & `data-repo-client-2.56.0/data_repo_client/models/date_partition_options_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/delete_response_model.py` & `data-repo-client-2.56.0/data_repo_client/models/delete_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/directory_detail_model.py` & `data-repo-client-2.56.0/data_repo_client/models/directory_detail_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/drs_access_method.py` & `data-repo-client-2.56.0/data_repo_client/models/drs_access_method.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/drs_access_url.py` & `data-repo-client-2.56.0/data_repo_client/models/drs_access_url.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/drs_alias_model.py` & `data-repo-client-2.56.0/data_repo_client/models/drs_alias_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/drs_authorizations.py` & `data-repo-client-2.56.0/data_repo_client/models/drs_authorizations.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/drs_checksum.py` & `data-repo-client-2.56.0/data_repo_client/models/drs_checksum.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/drs_contents_object.py` & `data-repo-client-2.56.0/data_repo_client/models/drs_contents_object.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/drs_error.py` & `data-repo-client-2.56.0/data_repo_client/models/drs_error.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/drs_object.py` & `data-repo-client-2.56.0/data_repo_client/models/drs_object.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/drs_passport_request_model.py` & `data-repo-client-2.56.0/data_repo_client/models/drs_passport_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/drs_service_info.py` & `data-repo-client-2.56.0/data_repo_client/models/drs_service_info.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/duos_firecloud_group_model.py` & `data-repo-client-2.56.0/data_repo_client/models/duos_firecloud_group_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/duos_firecloud_groups_sync_response.py` & `data-repo-client-2.56.0/data_repo_client/models/duos_firecloud_groups_sync_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/enumerate_billing_profile_model.py` & `data-repo-client-2.56.0/data_repo_client/models/enumerate_billing_profile_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/enumerate_dataset_model.py` & `data-repo-client-2.56.0/data_repo_client/models/enumerate_dataset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/enumerate_snapshot_access_request.py` & `data-repo-client-2.56.0/data_repo_client/models/enumerate_snapshot_access_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'items': 'list[EnumerateSnapshotAccessRequestItem]'
+        'items': 'list[SnapshotAccessRequestResponse]'
     }
 
     attribute_map = {
         'items': 'items'
     }
 
     def __init__(self, items=None, local_vars_configuration=None):  # noqa: E501
@@ -54,25 +54,25 @@
 
     @property
     def items(self):
         """Gets the items of this EnumerateSnapshotAccessRequest.  # noqa: E501
 
 
         :return: The items of this EnumerateSnapshotAccessRequest.  # noqa: E501
-        :rtype: list[EnumerateSnapshotAccessRequestItem]
+        :rtype: list[SnapshotAccessRequestResponse]
         """
         return self._items
 
     @items.setter
     def items(self, items):
         """Sets the items of this EnumerateSnapshotAccessRequest.
 
 
         :param items: The items of this EnumerateSnapshotAccessRequest.  # noqa: E501
-        :type: list[EnumerateSnapshotAccessRequestItem]
+        :type: list[SnapshotAccessRequestResponse]
         """
 
         self._items = items
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `data-repo-client-2.55.0/data_repo_client/models/enumerate_snapshot_access_request_item.py` & `data-repo-client-2.56.0/data_repo_client/models/job_model.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class EnumerateSnapshotAccessRequestItem(object):
+class JobModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -30,190 +30,234 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'id': 'str',
-        'status': 'SnapshotAccessRequestStatus',
-        'created_date': 'str',
-        'name': 'str',
-        'research_purpose': 'str',
-        'created_by': 'str'
+        'description': 'str',
+        'job_status': 'str',
+        'status_code': 'int',
+        'submitted': 'str',
+        'completed': 'str',
+        'class_name': 'str'
     }
 
     attribute_map = {
         'id': 'id',
-        'status': 'status',
-        'created_date': 'createdDate',
-        'name': 'name',
-        'research_purpose': 'researchPurpose',
-        'created_by': 'createdBy'
+        'description': 'description',
+        'job_status': 'job_status',
+        'status_code': 'status_code',
+        'submitted': 'submitted',
+        'completed': 'completed',
+        'class_name': 'class_name'
     }
 
-    def __init__(self, id=None, status=None, created_date=None, name=None, research_purpose=None, created_by=None, local_vars_configuration=None):  # noqa: E501
-        """EnumerateSnapshotAccessRequestItem - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, id=None, description=None, job_status=None, status_code=None, submitted=None, completed=None, class_name=None, local_vars_configuration=None):  # noqa: E501
+        """JobModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
-        self._status = None
-        self._created_date = None
-        self._name = None
-        self._research_purpose = None
-        self._created_by = None
+        self._description = None
+        self._job_status = None
+        self._status_code = None
+        self._submitted = None
+        self._completed = None
+        self._class_name = None
         self.discriminator = None
 
         self.id = id
-        self.status = status
-        self.created_date = created_date
-        self.name = name
-        self.research_purpose = research_purpose
-        self.created_by = created_by
+        if description is not None:
+            self.description = description
+        self.job_status = job_status
+        self.status_code = status_code
+        if submitted is not None:
+            self.submitted = submitted
+        if completed is not None:
+            self.completed = completed
+        if class_name is not None:
+            self.class_name = class_name
 
     @property
     def id(self):
-        """Gets the id of this EnumerateSnapshotAccessRequestItem.  # noqa: E501
+        """Gets the id of this JobModel.  # noqa: E501
 
-        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
+        Unique identifier for flights, jobs, etc.   # noqa: E501
 
-        :return: The id of this EnumerateSnapshotAccessRequestItem.  # noqa: E501
+        :return: The id of this JobModel.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this EnumerateSnapshotAccessRequestItem.
+        """Sets the id of this JobModel.
 
-        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
+        Unique identifier for flights, jobs, etc.   # noqa: E501
 
-        :param id: The id of this EnumerateSnapshotAccessRequestItem.  # noqa: E501
+        :param id: The id of this JobModel.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
             raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                id is not None and not re.search(r'[A-Za-z0-9_\\-]{22}', id)):  # noqa: E501
+            raise ValueError(r"Invalid value for `id`, must be a follow pattern or equal to `/[A-Za-z0-9_\\-]{22}/`")  # noqa: E501
 
         self._id = id
 
     @property
-    def status(self):
-        """Gets the status of this EnumerateSnapshotAccessRequestItem.  # noqa: E501
+    def description(self):
+        """Gets the description of this JobModel.  # noqa: E501
 
+        Description of the job's flight from description flight input parameter  # noqa: E501
 
-        :return: The status of this EnumerateSnapshotAccessRequestItem.  # noqa: E501
-        :rtype: SnapshotAccessRequestStatus
+        :return: The description of this JobModel.  # noqa: E501
+        :rtype: str
         """
-        return self._status
+        return self._description
 
-    @status.setter
-    def status(self, status):
-        """Sets the status of this EnumerateSnapshotAccessRequestItem.
+    @description.setter
+    def description(self, description):
+        """Sets the description of this JobModel.
 
+        Description of the job's flight from description flight input parameter  # noqa: E501
 
-        :param status: The status of this EnumerateSnapshotAccessRequestItem.  # noqa: E501
-        :type: SnapshotAccessRequestStatus
+        :param description: The description of this JobModel.  # noqa: E501
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and status is None:  # noqa: E501
-            raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
 
-        self._status = status
+        self._description = description
 
     @property
-    def created_date(self):
-        """Gets the created_date of this EnumerateSnapshotAccessRequestItem.  # noqa: E501
+    def job_status(self):
+        """Gets the job_status of this JobModel.  # noqa: E501
 
+        Status of job  # noqa: E501
 
-        :return: The created_date of this EnumerateSnapshotAccessRequestItem.  # noqa: E501
+        :return: The job_status of this JobModel.  # noqa: E501
         :rtype: str
         """
-        return self._created_date
+        return self._job_status
 
-    @created_date.setter
-    def created_date(self, created_date):
-        """Sets the created_date of this EnumerateSnapshotAccessRequestItem.
+    @job_status.setter
+    def job_status(self, job_status):
+        """Sets the job_status of this JobModel.
 
+        Status of job  # noqa: E501
 
-        :param created_date: The created_date of this EnumerateSnapshotAccessRequestItem.  # noqa: E501
+        :param job_status: The job_status of this JobModel.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and created_date is None:  # noqa: E501
-            raise ValueError("Invalid value for `created_date`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and job_status is None:  # noqa: E501
+            raise ValueError("Invalid value for `job_status`, must not be `None`")  # noqa: E501
+        allowed_values = ["running", "succeeded", "failed"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and job_status not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `job_status` ({0}), must be one of {1}"  # noqa: E501
+                .format(job_status, allowed_values)
+            )
+
+        self._job_status = job_status
+
+    @property
+    def status_code(self):
+        """Gets the status_code of this JobModel.  # noqa: E501
+
+        HTTP code  # noqa: E501
+
+        :return: The status_code of this JobModel.  # noqa: E501
+        :rtype: int
+        """
+        return self._status_code
+
+    @status_code.setter
+    def status_code(self, status_code):
+        """Sets the status_code of this JobModel.
+
+        HTTP code  # noqa: E501
+
+        :param status_code: The status_code of this JobModel.  # noqa: E501
+        :type: int
+        """
+        if self.local_vars_configuration.client_side_validation and status_code is None:  # noqa: E501
+            raise ValueError("Invalid value for `status_code`, must not be `None`")  # noqa: E501
 
-        self._created_date = created_date
+        self._status_code = status_code
 
     @property
-    def name(self):
-        """Gets the name of this EnumerateSnapshotAccessRequestItem.  # noqa: E501
+    def submitted(self):
+        """Gets the submitted of this JobModel.  # noqa: E501
 
+        Timestamp when the flight was created  # noqa: E501
 
-        :return: The name of this EnumerateSnapshotAccessRequestItem.  # noqa: E501
+        :return: The submitted of this JobModel.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._submitted
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this EnumerateSnapshotAccessRequestItem.
+    @submitted.setter
+    def submitted(self, submitted):
+        """Sets the submitted of this JobModel.
 
+        Timestamp when the flight was created  # noqa: E501
 
-        :param name: The name of this EnumerateSnapshotAccessRequestItem.  # noqa: E501
+        :param submitted: The submitted of this JobModel.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._submitted = submitted
 
     @property
-    def research_purpose(self):
-        """Gets the research_purpose of this EnumerateSnapshotAccessRequestItem.  # noqa: E501
+    def completed(self):
+        """Gets the completed of this JobModel.  # noqa: E501
 
+        Timestamp when the flight was completed; not present if not complete  # noqa: E501
 
-        :return: The research_purpose of this EnumerateSnapshotAccessRequestItem.  # noqa: E501
+        :return: The completed of this JobModel.  # noqa: E501
         :rtype: str
         """
-        return self._research_purpose
+        return self._completed
 
-    @research_purpose.setter
-    def research_purpose(self, research_purpose):
-        """Sets the research_purpose of this EnumerateSnapshotAccessRequestItem.
+    @completed.setter
+    def completed(self, completed):
+        """Sets the completed of this JobModel.
 
+        Timestamp when the flight was completed; not present if not complete  # noqa: E501
 
-        :param research_purpose: The research_purpose of this EnumerateSnapshotAccessRequestItem.  # noqa: E501
+        :param completed: The completed of this JobModel.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and research_purpose is None:  # noqa: E501
-            raise ValueError("Invalid value for `research_purpose`, must not be `None`")  # noqa: E501
 
-        self._research_purpose = research_purpose
+        self._completed = completed
 
     @property
-    def created_by(self):
-        """Gets the created_by of this EnumerateSnapshotAccessRequestItem.  # noqa: E501
+    def class_name(self):
+        """Gets the class_name of this JobModel.  # noqa: E501
 
+        Class name of the flight  # noqa: E501
 
-        :return: The created_by of this EnumerateSnapshotAccessRequestItem.  # noqa: E501
+        :return: The class_name of this JobModel.  # noqa: E501
         :rtype: str
         """
-        return self._created_by
+        return self._class_name
 
-    @created_by.setter
-    def created_by(self, created_by):
-        """Sets the created_by of this EnumerateSnapshotAccessRequestItem.
+    @class_name.setter
+    def class_name(self, class_name):
+        """Sets the class_name of this JobModel.
 
+        Class name of the flight  # noqa: E501
 
-        :param created_by: The created_by of this EnumerateSnapshotAccessRequestItem.  # noqa: E501
+        :param class_name: The class_name of this JobModel.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and created_by is None:  # noqa: E501
-            raise ValueError("Invalid value for `created_by`, must not be `None`")  # noqa: E501
 
-        self._created_by = created_by
+        self._class_name = class_name
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -241,18 +285,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, EnumerateSnapshotAccessRequestItem):
+        if not isinstance(other, JobModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, EnumerateSnapshotAccessRequestItem):
+        if not isinstance(other, JobModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-2.55.0/data_repo_client/models/enumerate_snapshot_model.py` & `data-repo-client-2.56.0/data_repo_client/models/enumerate_snapshot_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/enumerate_sort_by_param.py` & `data-repo-client-2.56.0/data_repo_client/models/enumerate_sort_by_param.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/error_model.py` & `data-repo-client-2.56.0/data_repo_client/models/error_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/file_detail_model.py` & `data-repo-client-2.56.0/data_repo_client/models/file_detail_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/file_load_model.py` & `data-repo-client-2.56.0/data_repo_client/models/file_load_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/file_model.py` & `data-repo-client-2.56.0/data_repo_client/models/file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/file_model_type.py` & `data-repo-client-2.56.0/data_repo_client/models/file_model_type.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/iam_resource_type_enum.py` & `data-repo-client-2.56.0/data_repo_client/models/iam_resource_type_enum.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,16 +29,17 @@
     allowed enum values
     """
     DATASET = "DATASET"
     DATASNAPSHOT = "DATASNAPSHOT"
     SPEND_PROFILE = "SPEND_PROFILE"
     DATAREPO = "DATAREPO"
     WORKSPACE = "WORKSPACE"
+    SNAPSHOT_BUILDER_REQUEST = "SNAPSHOT_BUILDER_REQUEST"
 
-    allowable_values = [DATASET, DATASNAPSHOT, SPEND_PROFILE, DATAREPO, WORKSPACE]  # noqa: E501
+    allowable_values = [DATASET, DATASNAPSHOT, SPEND_PROFILE, DATAREPO, WORKSPACE, SNAPSHOT_BUILDER_REQUEST]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `data-repo-client-2.55.0/data_repo_client/models/inaccessible_workspace_policy_model.py` & `data-repo-client-2.56.0/data_repo_client/models/inaccessible_workspace_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/ingest_request_model.py` & `data-repo-client-2.56.0/data_repo_client/models/ingest_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/ingest_response_model.py` & `data-repo-client-2.56.0/data_repo_client/models/ingest_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/int_partition_options_model.py` & `data-repo-client-2.56.0/data_repo_client/models/int_partition_options_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/job_model.py` & `data-repo-client-2.56.0/data_repo_client/models/transaction_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class JobModel(object):
+class TransactionModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -30,234 +30,257 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'id': 'str',
+        'status': 'str',
+        'lock': 'str',
         'description': 'str',
-        'job_status': 'str',
-        'status_code': 'int',
-        'submitted': 'str',
-        'completed': 'str',
-        'class_name': 'str'
+        'created_at': 'str',
+        'created_by': 'str',
+        'terminated_at': 'str',
+        'terminated_by': 'str'
     }
 
     attribute_map = {
         'id': 'id',
+        'status': 'status',
+        'lock': 'lock',
         'description': 'description',
-        'job_status': 'job_status',
-        'status_code': 'status_code',
-        'submitted': 'submitted',
-        'completed': 'completed',
-        'class_name': 'class_name'
+        'created_at': 'created_at',
+        'created_by': 'created_by',
+        'terminated_at': 'terminated_at',
+        'terminated_by': 'terminated_by'
     }
 
-    def __init__(self, id=None, description=None, job_status=None, status_code=None, submitted=None, completed=None, class_name=None, local_vars_configuration=None):  # noqa: E501
-        """JobModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, id=None, status=None, lock=None, description=None, created_at=None, created_by=None, terminated_at=None, terminated_by=None, local_vars_configuration=None):  # noqa: E501
+        """TransactionModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
+        self._status = None
+        self._lock = None
         self._description = None
-        self._job_status = None
-        self._status_code = None
-        self._submitted = None
-        self._completed = None
-        self._class_name = None
+        self._created_at = None
+        self._created_by = None
+        self._terminated_at = None
+        self._terminated_by = None
         self.discriminator = None
 
         self.id = id
+        if status is not None:
+            self.status = status
+        if lock is not None:
+            self.lock = lock
         if description is not None:
             self.description = description
-        self.job_status = job_status
-        self.status_code = status_code
-        if submitted is not None:
-            self.submitted = submitted
-        if completed is not None:
-            self.completed = completed
-        if class_name is not None:
-            self.class_name = class_name
+        self.created_at = created_at
+        self.created_by = created_by
+        if terminated_at is not None:
+            self.terminated_at = terminated_at
+        if terminated_by is not None:
+            self.terminated_by = terminated_by
 
     @property
     def id(self):
-        """Gets the id of this JobModel.  # noqa: E501
+        """Gets the id of this TransactionModel.  # noqa: E501
 
-        Unique identifier for flights, jobs, etc.   # noqa: E501
+        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
 
-        :return: The id of this JobModel.  # noqa: E501
+        :return: The id of this TransactionModel.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this JobModel.
+        """Sets the id of this TransactionModel.
 
-        Unique identifier for flights, jobs, etc.   # noqa: E501
+        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
 
-        :param id: The id of this JobModel.  # noqa: E501
+        :param id: The id of this TransactionModel.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
             raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                id is not None and not re.search(r'[A-Za-z0-9_\\-]{22}', id)):  # noqa: E501
-            raise ValueError(r"Invalid value for `id`, must be a follow pattern or equal to `/[A-Za-z0-9_\\-]{22}/`")  # noqa: E501
 
         self._id = id
 
     @property
-    def description(self):
-        """Gets the description of this JobModel.  # noqa: E501
+    def status(self):
+        """Gets the status of this TransactionModel.  # noqa: E501
 
-        Description of the job's flight from description flight input parameter  # noqa: E501
 
-        :return: The description of this JobModel.  # noqa: E501
+        :return: The status of this TransactionModel.  # noqa: E501
         :rtype: str
         """
-        return self._description
+        return self._status
 
-    @description.setter
-    def description(self, description):
-        """Sets the description of this JobModel.
+    @status.setter
+    def status(self, status):
+        """Sets the status of this TransactionModel.
 
-        Description of the job's flight from description flight input parameter  # noqa: E501
 
-        :param description: The description of this JobModel.  # noqa: E501
+        :param status: The status of this TransactionModel.  # noqa: E501
         :type: str
         """
+        allowed_values = ["active", "committed", "rolled_back"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and status not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `status` ({0}), must be one of {1}"  # noqa: E501
+                .format(status, allowed_values)
+            )
 
-        self._description = description
+        self._status = status
 
     @property
-    def job_status(self):
-        """Gets the job_status of this JobModel.  # noqa: E501
+    def lock(self):
+        """Gets the lock of this TransactionModel.  # noqa: E501
 
-        Status of job  # noqa: E501
+        the id of the flight that is locking the transaction or empty if the transaction is not locked  # noqa: E501
 
-        :return: The job_status of this JobModel.  # noqa: E501
+        :return: The lock of this TransactionModel.  # noqa: E501
         :rtype: str
         """
-        return self._job_status
+        return self._lock
 
-    @job_status.setter
-    def job_status(self, job_status):
-        """Sets the job_status of this JobModel.
+    @lock.setter
+    def lock(self, lock):
+        """Sets the lock of this TransactionModel.
 
-        Status of job  # noqa: E501
+        the id of the flight that is locking the transaction or empty if the transaction is not locked  # noqa: E501
 
-        :param job_status: The job_status of this JobModel.  # noqa: E501
+        :param lock: The lock of this TransactionModel.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and job_status is None:  # noqa: E501
-            raise ValueError("Invalid value for `job_status`, must not be `None`")  # noqa: E501
-        allowed_values = ["running", "succeeded", "failed"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and job_status not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `job_status` ({0}), must be one of {1}"  # noqa: E501
-                .format(job_status, allowed_values)
-            )
 
-        self._job_status = job_status
+        self._lock = lock
+
+    @property
+    def description(self):
+        """Gets the description of this TransactionModel.  # noqa: E501
+
+        the transaction's description, if one was specified  # noqa: E501
+
+        :return: The description of this TransactionModel.  # noqa: E501
+        :rtype: str
+        """
+        return self._description
+
+    @description.setter
+    def description(self, description):
+        """Sets the description of this TransactionModel.
+
+        the transaction's description, if one was specified  # noqa: E501
+
+        :param description: The description of this TransactionModel.  # noqa: E501
+        :type: str
+        """
+
+        self._description = description
 
     @property
-    def status_code(self):
-        """Gets the status_code of this JobModel.  # noqa: E501
+    def created_at(self):
+        """Gets the created_at of this TransactionModel.  # noqa: E501
 
-        HTTP code  # noqa: E501
+        timestamp of transaction creation in RFC3339  # noqa: E501
 
-        :return: The status_code of this JobModel.  # noqa: E501
-        :rtype: int
+        :return: The created_at of this TransactionModel.  # noqa: E501
+        :rtype: str
         """
-        return self._status_code
+        return self._created_at
 
-    @status_code.setter
-    def status_code(self, status_code):
-        """Sets the status_code of this JobModel.
+    @created_at.setter
+    def created_at(self, created_at):
+        """Sets the created_at of this TransactionModel.
 
-        HTTP code  # noqa: E501
+        timestamp of transaction creation in RFC3339  # noqa: E501
 
-        :param status_code: The status_code of this JobModel.  # noqa: E501
-        :type: int
+        :param created_at: The created_at of this TransactionModel.  # noqa: E501
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and status_code is None:  # noqa: E501
-            raise ValueError("Invalid value for `status_code`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and created_at is None:  # noqa: E501
+            raise ValueError("Invalid value for `created_at`, must not be `None`")  # noqa: E501
 
-        self._status_code = status_code
+        self._created_at = created_at
 
     @property
-    def submitted(self):
-        """Gets the submitted of this JobModel.  # noqa: E501
+    def created_by(self):
+        """Gets the created_by of this TransactionModel.  # noqa: E501
 
-        Timestamp when the flight was created  # noqa: E501
+        the creator of the transaction  # noqa: E501
 
-        :return: The submitted of this JobModel.  # noqa: E501
+        :return: The created_by of this TransactionModel.  # noqa: E501
         :rtype: str
         """
-        return self._submitted
+        return self._created_by
 
-    @submitted.setter
-    def submitted(self, submitted):
-        """Sets the submitted of this JobModel.
+    @created_by.setter
+    def created_by(self, created_by):
+        """Sets the created_by of this TransactionModel.
 
-        Timestamp when the flight was created  # noqa: E501
+        the creator of the transaction  # noqa: E501
 
-        :param submitted: The submitted of this JobModel.  # noqa: E501
+        :param created_by: The created_by of this TransactionModel.  # noqa: E501
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and created_by is None:  # noqa: E501
+            raise ValueError("Invalid value for `created_by`, must not be `None`")  # noqa: E501
 
-        self._submitted = submitted
+        self._created_by = created_by
 
     @property
-    def completed(self):
-        """Gets the completed of this JobModel.  # noqa: E501
+    def terminated_at(self):
+        """Gets the terminated_at of this TransactionModel.  # noqa: E501
 
-        Timestamp when the flight was completed; not present if not complete  # noqa: E501
+        timestamp of transaction creation in RFC3339  # noqa: E501
 
-        :return: The completed of this JobModel.  # noqa: E501
+        :return: The terminated_at of this TransactionModel.  # noqa: E501
         :rtype: str
         """
-        return self._completed
+        return self._terminated_at
 
-    @completed.setter
-    def completed(self, completed):
-        """Sets the completed of this JobModel.
+    @terminated_at.setter
+    def terminated_at(self, terminated_at):
+        """Sets the terminated_at of this TransactionModel.
 
-        Timestamp when the flight was completed; not present if not complete  # noqa: E501
+        timestamp of transaction creation in RFC3339  # noqa: E501
 
-        :param completed: The completed of this JobModel.  # noqa: E501
+        :param terminated_at: The terminated_at of this TransactionModel.  # noqa: E501
         :type: str
         """
 
-        self._completed = completed
+        self._terminated_at = terminated_at
 
     @property
-    def class_name(self):
-        """Gets the class_name of this JobModel.  # noqa: E501
+    def terminated_by(self):
+        """Gets the terminated_by of this TransactionModel.  # noqa: E501
 
-        Class name of the flight  # noqa: E501
+        the creator of the transaction  # noqa: E501
 
-        :return: The class_name of this JobModel.  # noqa: E501
+        :return: The terminated_by of this TransactionModel.  # noqa: E501
         :rtype: str
         """
-        return self._class_name
+        return self._terminated_by
 
-    @class_name.setter
-    def class_name(self, class_name):
-        """Sets the class_name of this JobModel.
+    @terminated_by.setter
+    def terminated_by(self, terminated_by):
+        """Sets the terminated_by of this TransactionModel.
 
-        Class name of the flight  # noqa: E501
+        the creator of the transaction  # noqa: E501
 
-        :param class_name: The class_name of this JobModel.  # noqa: E501
+        :param terminated_by: The terminated_by of this TransactionModel.  # noqa: E501
         :type: str
         """
 
-        self._class_name = class_name
+        self._terminated_by = terminated_by
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -285,18 +308,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, JobModel):
+        if not isinstance(other, TransactionModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, JobModel):
+        if not isinstance(other, TransactionModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-2.55.0/data_repo_client/models/journal_entry_model.py` & `data-repo-client-2.56.0/data_repo_client/models/journal_entry_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/policy_member_request.py` & `data-repo-client-2.56.0/data_repo_client/models/policy_member_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/policy_model.py` & `data-repo-client-2.56.0/data_repo_client/models/policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/policy_response.py` & `data-repo-client-2.56.0/data_repo_client/models/policy_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/query_column_statistics_request_model.py` & `data-repo-client-2.56.0/data_repo_client/models/query_column_statistics_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/query_data_request_model.py` & `data-repo-client-2.56.0/data_repo_client/models/query_data_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/relationship_model.py` & `data-repo-client-2.56.0/data_repo_client/models/relationship_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/relationship_term_model.py` & `data-repo-client-2.56.0/data_repo_client/models/relationship_term_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/repository_configuration_model.py` & `data-repo-client-2.56.0/data_repo_client/models/repository_configuration_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/repository_status_model.py` & `data-repo-client-2.56.0/data_repo_client/models/repository_status_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/repository_status_model_systems.py` & `data-repo-client-2.56.0/data_repo_client/models/repository_status_model_systems.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/resource_locks.py` & `data-repo-client-2.56.0/data_repo_client/models/resource_locks.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/resource_policy_model.py` & `data-repo-client-2.56.0/data_repo_client/models/resource_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/sam_policy_model.py` & `data-repo-client-2.56.0/data_repo_client/models/sam_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_access_request.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_access_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,44 +29,70 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'source_snapshot_id': 'str',
         'name': 'str',
         'research_purpose_statement': 'str',
         'dataset_request': 'SnapshotBuilderRequest'
     }
 
     attribute_map = {
+        'source_snapshot_id': 'sourceSnapshotId',
         'name': 'name',
         'research_purpose_statement': 'researchPurposeStatement',
         'dataset_request': 'datasetRequest'
     }
 
-    def __init__(self, name=None, research_purpose_statement=None, dataset_request=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, source_snapshot_id=None, name=None, research_purpose_statement=None, dataset_request=None, local_vars_configuration=None):  # noqa: E501
         """SnapshotAccessRequest - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._source_snapshot_id = None
         self._name = None
         self._research_purpose_statement = None
         self._dataset_request = None
         self.discriminator = None
 
+        if source_snapshot_id is not None:
+            self.source_snapshot_id = source_snapshot_id
         if name is not None:
             self.name = name
         if research_purpose_statement is not None:
             self.research_purpose_statement = research_purpose_statement
         if dataset_request is not None:
             self.dataset_request = dataset_request
 
     @property
+    def source_snapshot_id(self):
+        """Gets the source_snapshot_id of this SnapshotAccessRequest.  # noqa: E501
+
+
+        :return: The source_snapshot_id of this SnapshotAccessRequest.  # noqa: E501
+        :rtype: str
+        """
+        return self._source_snapshot_id
+
+    @source_snapshot_id.setter
+    def source_snapshot_id(self, source_snapshot_id):
+        """Sets the source_snapshot_id of this SnapshotAccessRequest.
+
+
+        :param source_snapshot_id: The source_snapshot_id of this SnapshotAccessRequest.  # noqa: E501
+        :type: str
+        """
+
+        self._source_snapshot_id = source_snapshot_id
+
+    @property
     def name(self):
         """Gets the name of this SnapshotAccessRequest.  # noqa: E501
 
 
         :return: The name of this SnapshotAccessRequest.  # noqa: E501
         :rtype: str
         """
```

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_access_request_response.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_access_request_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_access_request_status.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_access_request_status.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_cohort.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_cohort.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_concept.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_concept.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_count_request.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_count_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_count_response.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_count_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_count_response_result.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_count_response_result.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_criteria.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_criteria_group.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_criteria_group.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_dataset_concept_set.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_dataset_concept_set.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_domain_criteria.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_domain_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_domain_criteria_all_of.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_domain_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_domain_option.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_domain_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_domain_option_all_of.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_domain_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_feature_value_group.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_feature_value_group.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_get_concepts_response.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_get_concepts_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_option.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_parent_concept.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_parent_concept.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_list_criteria.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_list_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_list_item.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_list_item.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_list_option.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_list_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_option.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_option_all_of.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_range_criteria.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_range_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_range_criteria_all_of.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_range_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_range_option.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_range_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_program_data_range_option_all_of.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_program_data_range_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_request.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_builder_settings.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_builder_settings.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_export_response_model.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_export_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_export_response_model_format.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_export_response_model_format.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_ids_and_roles_model.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_ids_and_roles_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_link_duos_dataset_response.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_link_duos_dataset_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_model.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_patch_request_model.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_patch_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_preview_model.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_preview_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_request_asset_model.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_request_asset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_request_contents_model.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_request_contents_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_request_model.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_request_model_policies.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_request_model_policies.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_request_query_model.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_request_query_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_request_row_id_model.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_request_row_id_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_request_row_id_table_model.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_request_row_id_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_retrieve_include_model.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_retrieve_include_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_source_model.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_source_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/snapshot_summary_model.py` & `data-repo-client-2.56.0/data_repo_client/models/snapshot_summary_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/sql_sort_direction_asc_default.py` & `data-repo-client-2.56.0/data_repo_client/models/sql_sort_direction_asc_default.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/sql_sort_direction_desc_default.py` & `data-repo-client-2.56.0/data_repo_client/models/sql_sort_direction_desc_default.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/storage_resource_model.py` & `data-repo-client-2.56.0/data_repo_client/models/storage_resource_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/table_data_type.py` & `data-repo-client-2.56.0/data_repo_client/models/table_data_type.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/table_model.py` & `data-repo-client-2.56.0/data_repo_client/models/table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/tag_count.py` & `data-repo-client-2.56.0/data_repo_client/models/tag_count.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/tag_count_result_model.py` & `data-repo-client-2.56.0/data_repo_client/models/tag_count_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/tag_update_request_model.py` & `data-repo-client-2.56.0/data_repo_client/models/tag_update_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/transaction_close_model.py` & `data-repo-client-2.56.0/data_repo_client/models/transaction_close_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/transaction_create_model.py` & `data-repo-client-2.56.0/data_repo_client/models/transaction_create_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/unlock_resource_request.py` & `data-repo-client-2.56.0/data_repo_client/models/unlock_resource_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/upgrade_model.py` & `data-repo-client-2.56.0/data_repo_client/models/upgrade_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/upgrade_response_model.py` & `data-repo-client-2.56.0/data_repo_client/models/upgrade_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/user_status_info.py` & `data-repo-client-2.56.0/data_repo_client/models/user_status_info.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/models/workspace_policy_model.py` & `data-repo-client-2.56.0/data_repo_client/models/workspace_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client/rest.py` & `data-repo-client-2.56.0/data_repo_client/rest.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/data_repo_client.egg-info/PKG-INFO` & `data-repo-client-2.56.0/data_repo_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-repo-client
-Version: 2.55.0
+Version: 2.56.0
 Summary: Data Repository API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,Data Repository API
```

### Comparing `data-repo-client-2.55.0/data_repo_client.egg-info/SOURCES.txt` & `data-repo-client-2.56.0/data_repo_client.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 data_repo_client/api/jobs_api.py
 data_repo_client/api/journal_api.py
 data_repo_client/api/profiles_api.py
 data_repo_client/api/register_api.py
 data_repo_client/api/repository_api.py
 data_repo_client/api/resources_api.py
 data_repo_client/api/search_api.py
+data_repo_client/api/snapshot_access_request_api.py
 data_repo_client/api/snapshots_api.py
 data_repo_client/api/unauthenticated_api.py
 data_repo_client/api/upgrade_api.py
 data_repo_client/models/__init__.py
 data_repo_client/models/access_info_big_query_model.py
 data_repo_client/models/access_info_big_query_model_table.py
 data_repo_client/models/access_info_model.py
@@ -94,15 +95,14 @@
 data_repo_client/models/drs_passport_request_model.py
 data_repo_client/models/drs_service_info.py
 data_repo_client/models/duos_firecloud_group_model.py
 data_repo_client/models/duos_firecloud_groups_sync_response.py
 data_repo_client/models/enumerate_billing_profile_model.py
 data_repo_client/models/enumerate_dataset_model.py
 data_repo_client/models/enumerate_snapshot_access_request.py
-data_repo_client/models/enumerate_snapshot_access_request_item.py
 data_repo_client/models/enumerate_snapshot_model.py
 data_repo_client/models/enumerate_sort_by_param.py
 data_repo_client/models/error_model.py
 data_repo_client/models/file_detail_model.py
 data_repo_client/models/file_load_model.py
 data_repo_client/models/file_model.py
 data_repo_client/models/file_model_type.py
@@ -267,15 +267,14 @@
 test/test_drs_service_info.py
 test/test_duos_api.py
 test/test_duos_firecloud_group_model.py
 test/test_duos_firecloud_groups_sync_response.py
 test/test_enumerate_billing_profile_model.py
 test/test_enumerate_dataset_model.py
 test/test_enumerate_snapshot_access_request.py
-test/test_enumerate_snapshot_access_request_item.py
 test/test_enumerate_snapshot_model.py
 test/test_enumerate_sort_by_param.py
 test/test_error_model.py
 test/test_file_detail_model.py
 test/test_file_load_model.py
 test/test_file_model.py
 test/test_file_model_type.py
@@ -303,14 +302,15 @@
 test/test_repository_status_model_systems.py
 test/test_resource_locks.py
 test/test_resource_policy_model.py
 test/test_resources_api.py
 test/test_sam_policy_model.py
 test/test_search_api.py
 test/test_snapshot_access_request.py
+test/test_snapshot_access_request_api.py
 test/test_snapshot_access_request_response.py
 test/test_snapshot_access_request_status.py
 test/test_snapshot_builder_cohort.py
 test/test_snapshot_builder_concept.py
 test/test_snapshot_builder_count_request.py
 test/test_snapshot_builder_count_response.py
 test/test_snapshot_builder_count_response_result.py
```

### Comparing `data-repo-client-2.55.0/setup.py` & `data-repo-client-2.56.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "data-repo-client"
-VERSION = "2.55.0"
+VERSION = "2.56.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `data-repo-client-2.55.0/test/test_access_info_big_query_model.py` & `data-repo-client-2.56.0/test/test_access_info_big_query_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_access_info_big_query_model_table.py` & `data-repo-client-2.56.0/test/test_access_info_big_query_model_table.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_access_info_model.py` & `data-repo-client-2.56.0/test/test_access_info_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_access_info_parquet_model.py` & `data-repo-client-2.56.0/test/test_access_info_parquet_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_access_info_parquet_model_table.py` & `data-repo-client-2.56.0/test/test_access_info_parquet_model_table.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_add_auth_domain_response_model.py` & `data-repo-client-2.56.0/test/test_add_auth_domain_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_admin_api.py` & `data-repo-client-2.56.0/test/test_admin_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_asset_model.py` & `data-repo-client-2.56.0/test/test_asset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_asset_table_model.py` & `data-repo-client-2.56.0/test/test_asset_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_billing_profile_model.py` & `data-repo-client-2.56.0/test/test_billing_profile_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_billing_profile_request_model.py` & `data-repo-client-2.56.0/test/test_billing_profile_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_billing_profile_update_model.py` & `data-repo-client-2.56.0/test/test_billing_profile_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_bulk_load_array_request_model.py` & `data-repo-client-2.56.0/test/test_bulk_load_array_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_bulk_load_array_result_model.py` & `data-repo-client-2.56.0/test/test_bulk_load_array_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_bulk_load_file_model.py` & `data-repo-client-2.56.0/test/test_bulk_load_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_bulk_load_file_result_model.py` & `data-repo-client-2.56.0/test/test_bulk_load_file_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_bulk_load_file_state.py` & `data-repo-client-2.56.0/test/test_bulk_load_file_state.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_bulk_load_history_model.py` & `data-repo-client-2.56.0/test/test_bulk_load_history_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_bulk_load_history_model_list.py` & `data-repo-client-2.56.0/test/test_bulk_load_history_model_list.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_bulk_load_request_model.py` & `data-repo-client-2.56.0/test/test_bulk_load_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_bulk_load_result_model.py` & `data-repo-client-2.56.0/test/test_bulk_load_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_cloud_platform.py` & `data-repo-client-2.56.0/test/test_cloud_platform.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_column_model.py` & `data-repo-client-2.56.0/test/test_column_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_column_statistics_double_model.py` & `data-repo-client-2.56.0/test/test_column_statistics_double_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_column_statistics_double_model_all_of.py` & `data-repo-client-2.56.0/test/test_column_statistics_double_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_column_statistics_int_model.py` & `data-repo-client-2.56.0/test/test_column_statistics_int_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_column_statistics_int_model_all_of.py` & `data-repo-client-2.56.0/test/test_column_statistics_int_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_column_statistics_model.py` & `data-repo-client-2.56.0/test/test_column_statistics_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_column_statistics_text_model.py` & `data-repo-client-2.56.0/test/test_column_statistics_text_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_column_statistics_text_model_all_of.py` & `data-repo-client-2.56.0/test/test_column_statistics_text_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_column_statistics_text_value.py` & `data-repo-client-2.56.0/test/test_column_statistics_text_value.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_config_enable_model.py` & `data-repo-client-2.56.0/test/test_config_enable_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_config_fault_counted_model.py` & `data-repo-client-2.56.0/test/test_config_fault_counted_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_config_fault_model.py` & `data-repo-client-2.56.0/test/test_config_fault_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_config_group_model.py` & `data-repo-client-2.56.0/test/test_config_group_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_config_list_model.py` & `data-repo-client-2.56.0/test/test_config_list_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_config_model.py` & `data-repo-client-2.56.0/test/test_config_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_config_parameter_model.py` & `data-repo-client-2.56.0/test/test_config_parameter_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_configs_api.py` & `data-repo-client-2.56.0/test/test_configs_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_data_deletion_gcs_file_model.py` & `data-repo-client-2.56.0/test/test_data_deletion_gcs_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_data_deletion_json_array_model.py` & `data-repo-client-2.56.0/test/test_data_deletion_json_array_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_data_deletion_request.py` & `data-repo-client-2.56.0/test/test_data_deletion_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_data_deletion_table_model.py` & `data-repo-client-2.56.0/test/test_data_deletion_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_data_repository_service_api.py` & `data-repo-client-2.56.0/test/test_data_repository_service_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_dataset_data_model.py` & `data-repo-client-2.56.0/test/test_dataset_data_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_dataset_model.py` & `data-repo-client-2.56.0/test/test_dataset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_dataset_patch_request_model.py` & `data-repo-client-2.56.0/test/test_dataset_patch_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_dataset_request_access_include_model.py` & `data-repo-client-2.56.0/test/test_dataset_request_access_include_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_dataset_request_model.py` & `data-repo-client-2.56.0/test/test_dataset_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_dataset_request_model_policies.py` & `data-repo-client-2.56.0/test/test_dataset_request_model_policies.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_dataset_schema_column_update_model.py` & `data-repo-client-2.56.0/test/test_dataset_schema_column_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_dataset_schema_update_model.py` & `data-repo-client-2.56.0/test/test_dataset_schema_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_dataset_schema_update_model_changes.py` & `data-repo-client-2.56.0/test/test_dataset_schema_update_model_changes.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_dataset_specification_model.py` & `data-repo-client-2.56.0/test/test_dataset_specification_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_dataset_summary_model.py` & `data-repo-client-2.56.0/test/test_dataset_summary_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_datasets_api.py` & `data-repo-client-2.56.0/test/test_datasets_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,20 +72,14 @@
 
     def test_create_dataset(self):
         """Test case for create_dataset
 
         """
         pass
 
-    def test_create_snapshot_request(self):
-        """Test case for create_snapshot_request
-
-        """
-        pass
-
     def test_delete_dataset(self):
         """Test case for delete_dataset
 
         """
         pass
 
     def test_delete_dataset_policy_member(self):
@@ -102,20 +96,14 @@
 
     def test_enumerate_datasets(self):
         """Test case for enumerate_datasets
 
         """
         pass
 
-    def test_enumerate_snapshot_requests(self):
-        """Test case for enumerate_snapshot_requests
-
-        """
-        pass
-
     def test_enumerate_transactions(self):
         """Test case for enumerate_transactions
 
         """
         pass
 
     def test_get_concept_hierarchy(self):
```

### Comparing `data-repo-client-2.55.0/test/test_date_partition_options_model.py` & `data-repo-client-2.56.0/test/test_date_partition_options_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_delete_response_model.py` & `data-repo-client-2.56.0/test/test_delete_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_directory_detail_model.py` & `data-repo-client-2.56.0/test/test_directory_detail_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_drs_access_method.py` & `data-repo-client-2.56.0/test/test_drs_access_method.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_drs_access_url.py` & `data-repo-client-2.56.0/test/test_drs_access_url.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_drs_alias_model.py` & `data-repo-client-2.56.0/test/test_drs_alias_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_drs_authorizations.py` & `data-repo-client-2.56.0/test/test_drs_authorizations.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_drs_checksum.py` & `data-repo-client-2.56.0/test/test_drs_checksum.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_drs_contents_object.py` & `data-repo-client-2.56.0/test/test_drs_contents_object.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_drs_error.py` & `data-repo-client-2.56.0/test/test_drs_error.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_drs_object.py` & `data-repo-client-2.56.0/test/test_drs_object.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_drs_passport_request_model.py` & `data-repo-client-2.56.0/test/test_drs_passport_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_drs_service_info.py` & `data-repo-client-2.56.0/test/test_drs_service_info.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_duos_api.py` & `data-repo-client-2.56.0/test/test_duos_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_duos_firecloud_group_model.py` & `data-repo-client-2.56.0/test/test_duos_firecloud_group_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_duos_firecloud_groups_sync_response.py` & `data-repo-client-2.56.0/test/test_duos_firecloud_groups_sync_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_enumerate_billing_profile_model.py` & `data-repo-client-2.56.0/test/test_enumerate_billing_profile_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_enumerate_dataset_model.py` & `data-repo-client-2.56.0/test/test_enumerate_dataset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_enumerate_snapshot_access_request.py` & `data-repo-client-2.56.0/test/test_snapshot_request_asset_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,49 +12,48 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.enumerate_snapshot_access_request import EnumerateSnapshotAccessRequest  # noqa: E501
+from data_repo_client.models.snapshot_request_asset_model import SnapshotRequestAssetModel  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestEnumerateSnapshotAccessRequest(unittest.TestCase):
-    """EnumerateSnapshotAccessRequest unit test stubs"""
+class TestSnapshotRequestAssetModel(unittest.TestCase):
+    """SnapshotRequestAssetModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test EnumerateSnapshotAccessRequest
+        """Test SnapshotRequestAssetModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.enumerate_snapshot_access_request.EnumerateSnapshotAccessRequest()  # noqa: E501
+        # model = data_repo_client.models.snapshot_request_asset_model.SnapshotRequestAssetModel()  # noqa: E501
         if include_optional :
-            return EnumerateSnapshotAccessRequest(
-                items = [
-                    data_repo_client.models.enumerate_snapshot_access_request_item.EnumerateSnapshotAccessRequestItem(
-                        id = '0', 
-                        status = 'SUBMITTED', 
-                        created_date = '0', 
-                        name = '0', 
-                        research_purpose = '0', 
-                        created_by = '0', )
+            return SnapshotRequestAssetModel(
+                asset_name = 'a', 
+                root_values = [
+                    '0'
                     ]
             )
         else :
-            return EnumerateSnapshotAccessRequest(
+            return SnapshotRequestAssetModel(
+                asset_name = 'a',
+                root_values = [
+                    '0'
+                    ],
         )
 
-    def testEnumerateSnapshotAccessRequest(self):
-        """Test EnumerateSnapshotAccessRequest"""
+    def testSnapshotRequestAssetModel(self):
+        """Test SnapshotRequestAssetModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.55.0/test/test_enumerate_snapshot_access_request_item.py` & `data-repo-client-2.56.0/test/test_snapshot_preview_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,52 +12,45 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.enumerate_snapshot_access_request_item import EnumerateSnapshotAccessRequestItem  # noqa: E501
+from data_repo_client.models.snapshot_preview_model import SnapshotPreviewModel  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestEnumerateSnapshotAccessRequestItem(unittest.TestCase):
-    """EnumerateSnapshotAccessRequestItem unit test stubs"""
+class TestSnapshotPreviewModel(unittest.TestCase):
+    """SnapshotPreviewModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test EnumerateSnapshotAccessRequestItem
+        """Test SnapshotPreviewModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.enumerate_snapshot_access_request_item.EnumerateSnapshotAccessRequestItem()  # noqa: E501
+        # model = data_repo_client.models.snapshot_preview_model.SnapshotPreviewModel()  # noqa: E501
         if include_optional :
-            return EnumerateSnapshotAccessRequestItem(
-                id = '0', 
-                status = 'SUBMITTED', 
-                created_date = '0', 
-                name = '0', 
-                research_purpose = '0', 
-                created_by = '0'
+            return SnapshotPreviewModel(
+                result = [
+                    None
+                    ], 
+                total_row_count = 56, 
+                filtered_row_count = 56
             )
         else :
-            return EnumerateSnapshotAccessRequestItem(
-                id = '0',
-                status = 'SUBMITTED',
-                created_date = '0',
-                name = '0',
-                research_purpose = '0',
-                created_by = '0',
+            return SnapshotPreviewModel(
         )
 
-    def testEnumerateSnapshotAccessRequestItem(self):
-        """Test EnumerateSnapshotAccessRequestItem"""
+    def testSnapshotPreviewModel(self):
+        """Test SnapshotPreviewModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.55.0/test/test_enumerate_snapshot_model.py` & `data-repo-client-2.56.0/test/test_enumerate_snapshot_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_enumerate_sort_by_param.py` & `data-repo-client-2.56.0/test/test_enumerate_sort_by_param.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_error_model.py` & `data-repo-client-2.56.0/test/test_error_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_file_detail_model.py` & `data-repo-client-2.56.0/test/test_file_detail_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_file_load_model.py` & `data-repo-client-2.56.0/test/test_file_load_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_file_model.py` & `data-repo-client-2.56.0/test/test_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_file_model_type.py` & `data-repo-client-2.56.0/test/test_file_model_type.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_iam_resource_type_enum.py` & `data-repo-client-2.56.0/test/test_iam_resource_type_enum.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_inaccessible_workspace_policy_model.py` & `data-repo-client-2.56.0/test/test_inaccessible_workspace_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_ingest_request_model.py` & `data-repo-client-2.56.0/test/test_ingest_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_ingest_response_model.py` & `data-repo-client-2.56.0/test/test_ingest_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_int_partition_options_model.py` & `data-repo-client-2.56.0/test/test_int_partition_options_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_job_model.py` & `data-repo-client-2.56.0/test/test_job_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_jobs_api.py` & `data-repo-client-2.56.0/test/test_jobs_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_journal_api.py` & `data-repo-client-2.56.0/test/test_journal_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_journal_entry_model.py` & `data-repo-client-2.56.0/test/test_journal_entry_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_policy_member_request.py` & `data-repo-client-2.56.0/test/test_policy_member_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_policy_model.py` & `data-repo-client-2.56.0/test/test_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_policy_response.py` & `data-repo-client-2.56.0/test/test_policy_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_profiles_api.py` & `data-repo-client-2.56.0/test/test_profiles_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_query_column_statistics_request_model.py` & `data-repo-client-2.56.0/test/test_query_column_statistics_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_query_data_request_model.py` & `data-repo-client-2.56.0/test/test_query_data_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_register_api.py` & `data-repo-client-2.56.0/test/test_register_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_relationship_model.py` & `data-repo-client-2.56.0/test/test_relationship_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_relationship_term_model.py` & `data-repo-client-2.56.0/test/test_relationship_term_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_repository_api.py` & `data-repo-client-2.56.0/test/test_repository_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_repository_configuration_model.py` & `data-repo-client-2.56.0/test/test_repository_configuration_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_repository_status_model.py` & `data-repo-client-2.56.0/test/test_repository_status_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_repository_status_model_systems.py` & `data-repo-client-2.56.0/test/test_repository_status_model_systems.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_resource_locks.py` & `data-repo-client-2.56.0/test/test_resource_locks.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_resource_policy_model.py` & `data-repo-client-2.56.0/test/test_resource_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_resources_api.py` & `data-repo-client-2.56.0/test/test_resources_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_sam_policy_model.py` & `data-repo-client-2.56.0/test/test_sam_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_search_api.py` & `data-repo-client-2.56.0/test/test_search_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_access_request.py` & `data-repo-client-2.56.0/test/test_snapshot_access_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         """Test SnapshotAccessRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = data_repo_client.models.snapshot_access_request.SnapshotAccessRequest()  # noqa: E501
         if include_optional :
             return SnapshotAccessRequest(
+                source_snapshot_id = '0', 
                 name = '0', 
                 research_purpose_statement = '0', 
                 dataset_request = data_repo_client.models.snapshot_builder_request.SnapshotBuilderRequest(
                     cohorts = [
                         data_repo_client.models.snapshot_builder_cohort.SnapshotBuilderCohort(
                             name = '0', 
                             criteria_groups = [
```

### Comparing `data-repo-client-2.55.0/test/test_snapshot_access_request_response.py` & `data-repo-client-2.56.0/test/test_snapshot_access_request_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_access_request_status.py` & `data-repo-client-2.56.0/test/test_snapshot_access_request_status.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_cohort.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_cohort.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_concept.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_concept.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_count_request.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_count_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_count_response.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_count_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_count_response_result.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_count_response_result.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_criteria.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_criteria_group.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_criteria_group.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_dataset_concept_set.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_dataset_concept_set.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_domain_criteria.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_domain_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_domain_criteria_all_of.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_domain_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_domain_option.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_domain_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_domain_option_all_of.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_domain_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_feature_value_group.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_feature_value_group.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_get_concept_hierarchy_response.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_get_concept_hierarchy_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_get_concepts_response.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_get_concepts_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_option.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_parent_concept.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_parent_concept.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_program_data_list_criteria.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_program_data_list_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_program_data_list_criteria_all_of.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_program_data_list_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_program_data_list_item.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_program_data_list_item.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_program_data_list_option.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_program_data_list_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_program_data_list_option_all_of.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_program_data_list_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_program_data_option.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_program_data_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_program_data_option_all_of.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_program_data_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_program_data_range_criteria.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_program_data_range_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_program_data_range_criteria_all_of.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_program_data_range_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_program_data_range_option.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_program_data_range_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_program_data_range_option_all_of.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_program_data_range_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_request.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_builder_settings.py` & `data-repo-client-2.56.0/test/test_snapshot_builder_settings.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_export_response_model.py` & `data-repo-client-2.56.0/test/test_snapshot_export_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_export_response_model_format.py` & `data-repo-client-2.56.0/test/test_snapshot_export_response_model_format.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_export_response_model_format_parquet.py` & `data-repo-client-2.56.0/test/test_snapshot_export_response_model_format_parquet.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_export_response_model_format_parquet_location.py` & `data-repo-client-2.56.0/test/test_snapshot_export_response_model_format_parquet_location.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py` & `data-repo-client-2.56.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_export_response_model_format_workspace.py` & `data-repo-client-2.56.0/test/test_snapshot_export_response_model_format_workspace.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_ids_and_roles_model.py` & `data-repo-client-2.56.0/test/test_snapshot_ids_and_roles_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_link_duos_dataset_response.py` & `data-repo-client-2.56.0/test/test_snapshot_link_duos_dataset_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_model.py` & `data-repo-client-2.56.0/test/test_snapshot_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_patch_request_model.py` & `data-repo-client-2.56.0/test/test_snapshot_patch_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_preview_model.py` & `data-repo-client-2.56.0/test/test_tag_update_request_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,45 +12,46 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.snapshot_preview_model import SnapshotPreviewModel  # noqa: E501
+from data_repo_client.models.tag_update_request_model import TagUpdateRequestModel  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestSnapshotPreviewModel(unittest.TestCase):
-    """SnapshotPreviewModel unit test stubs"""
+class TestTagUpdateRequestModel(unittest.TestCase):
+    """TagUpdateRequestModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SnapshotPreviewModel
+        """Test TagUpdateRequestModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.snapshot_preview_model.SnapshotPreviewModel()  # noqa: E501
+        # model = data_repo_client.models.tag_update_request_model.TagUpdateRequestModel()  # noqa: E501
         if include_optional :
-            return SnapshotPreviewModel(
-                result = [
-                    None
+            return TagUpdateRequestModel(
+                add = [
+                    'a-resource-tag'
                     ], 
-                total_row_count = 56, 
-                filtered_row_count = 56
+                remove = [
+                    'a-resource-tag'
+                    ]
             )
         else :
-            return SnapshotPreviewModel(
+            return TagUpdateRequestModel(
         )
 
-    def testSnapshotPreviewModel(self):
-        """Test SnapshotPreviewModel"""
+    def testTagUpdateRequestModel(self):
+        """Test TagUpdateRequestModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.55.0/test/test_snapshot_request_asset_model.py` & `data-repo-client-2.56.0/test/test_snapshot_request_row_id_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,48 +12,60 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.snapshot_request_asset_model import SnapshotRequestAssetModel  # noqa: E501
+from data_repo_client.models.snapshot_request_row_id_model import SnapshotRequestRowIdModel  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestSnapshotRequestAssetModel(unittest.TestCase):
-    """SnapshotRequestAssetModel unit test stubs"""
+class TestSnapshotRequestRowIdModel(unittest.TestCase):
+    """SnapshotRequestRowIdModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SnapshotRequestAssetModel
+        """Test SnapshotRequestRowIdModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.snapshot_request_asset_model.SnapshotRequestAssetModel()  # noqa: E501
+        # model = data_repo_client.models.snapshot_request_row_id_model.SnapshotRequestRowIdModel()  # noqa: E501
         if include_optional :
-            return SnapshotRequestAssetModel(
-                asset_name = 'a', 
-                root_values = [
-                    '0'
+            return SnapshotRequestRowIdModel(
+                tables = [
+                    data_repo_client.models.snapshot_request_row_id_table_model.SnapshotRequestRowIdTableModel(
+                        table_name = 'a', 
+                        columns = [
+                            'a'
+                            ], 
+                        row_ids = [
+                            '0'
+                            ], )
                     ]
             )
         else :
-            return SnapshotRequestAssetModel(
-                asset_name = 'a',
-                root_values = [
-                    '0'
+            return SnapshotRequestRowIdModel(
+                tables = [
+                    data_repo_client.models.snapshot_request_row_id_table_model.SnapshotRequestRowIdTableModel(
+                        table_name = 'a', 
+                        columns = [
+                            'a'
+                            ], 
+                        row_ids = [
+                            '0'
+                            ], )
                     ],
         )
 
-    def testSnapshotRequestAssetModel(self):
-        """Test SnapshotRequestAssetModel"""
+    def testSnapshotRequestRowIdModel(self):
+        """Test SnapshotRequestRowIdModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.55.0/test/test_snapshot_request_contents_model.py` & `data-repo-client-2.56.0/test/test_snapshot_request_contents_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_request_model.py` & `data-repo-client-2.56.0/test/test_snapshot_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_request_model_policies.py` & `data-repo-client-2.56.0/test/test_snapshot_request_model_policies.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_request_query_model.py` & `data-repo-client-2.56.0/test/test_snapshot_request_query_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_request_row_id_model.py` & `data-repo-client-2.56.0/test/test_snapshot_request_row_id_table_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,60 +12,54 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.snapshot_request_row_id_model import SnapshotRequestRowIdModel  # noqa: E501
+from data_repo_client.models.snapshot_request_row_id_table_model import SnapshotRequestRowIdTableModel  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestSnapshotRequestRowIdModel(unittest.TestCase):
-    """SnapshotRequestRowIdModel unit test stubs"""
+class TestSnapshotRequestRowIdTableModel(unittest.TestCase):
+    """SnapshotRequestRowIdTableModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SnapshotRequestRowIdModel
+        """Test SnapshotRequestRowIdTableModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.snapshot_request_row_id_model.SnapshotRequestRowIdModel()  # noqa: E501
+        # model = data_repo_client.models.snapshot_request_row_id_table_model.SnapshotRequestRowIdTableModel()  # noqa: E501
         if include_optional :
-            return SnapshotRequestRowIdModel(
-                tables = [
-                    data_repo_client.models.snapshot_request_row_id_table_model.SnapshotRequestRowIdTableModel(
-                        table_name = 'a', 
-                        columns = [
-                            'a'
-                            ], 
-                        row_ids = [
-                            '0'
-                            ], )
+            return SnapshotRequestRowIdTableModel(
+                table_name = 'a', 
+                columns = [
+                    'a'
+                    ], 
+                row_ids = [
+                    '0'
                     ]
             )
         else :
-            return SnapshotRequestRowIdModel(
-                tables = [
-                    data_repo_client.models.snapshot_request_row_id_table_model.SnapshotRequestRowIdTableModel(
-                        table_name = 'a', 
-                        columns = [
-                            'a'
-                            ], 
-                        row_ids = [
-                            '0'
-                            ], )
+            return SnapshotRequestRowIdTableModel(
+                table_name = 'a',
+                columns = [
+                    'a'
+                    ],
+                row_ids = [
+                    '0'
                     ],
         )
 
-    def testSnapshotRequestRowIdModel(self):
-        """Test SnapshotRequestRowIdModel"""
+    def testSnapshotRequestRowIdTableModel(self):
+        """Test SnapshotRequestRowIdTableModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.55.0/test/test_snapshot_request_row_id_table_model.py` & `data-repo-client-2.56.0/test/test_transaction_create_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,54 +12,41 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.snapshot_request_row_id_table_model import SnapshotRequestRowIdTableModel  # noqa: E501
+from data_repo_client.models.transaction_create_model import TransactionCreateModel  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestSnapshotRequestRowIdTableModel(unittest.TestCase):
-    """SnapshotRequestRowIdTableModel unit test stubs"""
+class TestTransactionCreateModel(unittest.TestCase):
+    """TransactionCreateModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SnapshotRequestRowIdTableModel
+        """Test TransactionCreateModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.snapshot_request_row_id_table_model.SnapshotRequestRowIdTableModel()  # noqa: E501
+        # model = data_repo_client.models.transaction_create_model.TransactionCreateModel()  # noqa: E501
         if include_optional :
-            return SnapshotRequestRowIdTableModel(
-                table_name = 'a', 
-                columns = [
-                    'a'
-                    ], 
-                row_ids = [
-                    '0'
-                    ]
+            return TransactionCreateModel(
+                description = '0'
             )
         else :
-            return SnapshotRequestRowIdTableModel(
-                table_name = 'a',
-                columns = [
-                    'a'
-                    ],
-                row_ids = [
-                    '0'
-                    ],
+            return TransactionCreateModel(
         )
 
-    def testSnapshotRequestRowIdTableModel(self):
-        """Test SnapshotRequestRowIdTableModel"""
+    def testTransactionCreateModel(self):
+        """Test TransactionCreateModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.55.0/test/test_snapshot_retrieve_include_model.py` & `data-repo-client-2.56.0/test/test_snapshot_retrieve_include_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_source_model.py` & `data-repo-client-2.56.0/test/test_snapshot_source_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshot_summary_model.py` & `data-repo-client-2.56.0/test/test_snapshot_summary_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_snapshots_api.py` & `data-repo-client-2.56.0/test/test_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_sql_sort_direction_asc_default.py` & `data-repo-client-2.56.0/test/test_sql_sort_direction_asc_default.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_sql_sort_direction_desc_default.py` & `data-repo-client-2.56.0/test/test_sql_sort_direction_desc_default.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_storage_resource_model.py` & `data-repo-client-2.56.0/test/test_storage_resource_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_table_data_type.py` & `data-repo-client-2.56.0/test/test_table_data_type.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_table_model.py` & `data-repo-client-2.56.0/test/test_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_tag_count.py` & `data-repo-client-2.56.0/test/test_tag_count.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_tag_count_result_model.py` & `data-repo-client-2.56.0/test/test_tag_count_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_tag_update_request_model.py` & `data-repo-client-2.56.0/test/test_unlock_resource_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,46 +12,43 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.tag_update_request_model import TagUpdateRequestModel  # noqa: E501
+from data_repo_client.models.unlock_resource_request import UnlockResourceRequest  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestTagUpdateRequestModel(unittest.TestCase):
-    """TagUpdateRequestModel unit test stubs"""
+class TestUnlockResourceRequest(unittest.TestCase):
+    """UnlockResourceRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test TagUpdateRequestModel
+        """Test UnlockResourceRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.tag_update_request_model.TagUpdateRequestModel()  # noqa: E501
+        # model = data_repo_client.models.unlock_resource_request.UnlockResourceRequest()  # noqa: E501
         if include_optional :
-            return TagUpdateRequestModel(
-                add = [
-                    'a-resource-tag'
-                    ], 
-                remove = [
-                    'a-resource-tag'
-                    ]
+            return UnlockResourceRequest(
+                lock_name = '0', 
+                force_unlock = True
             )
         else :
-            return TagUpdateRequestModel(
+            return UnlockResourceRequest(
+                lock_name = '0',
         )
 
-    def testTagUpdateRequestModel(self):
-        """Test TagUpdateRequestModel"""
+    def testUnlockResourceRequest(self):
+        """Test UnlockResourceRequest"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.55.0/test/test_transaction_close_model.py` & `data-repo-client-2.56.0/test/test_transaction_close_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_transaction_create_model.py` & `data-repo-client-2.56.0/test/test_transaction_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,41 +12,51 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.transaction_create_model import TransactionCreateModel  # noqa: E501
+from data_repo_client.models.transaction_model import TransactionModel  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestTransactionCreateModel(unittest.TestCase):
-    """TransactionCreateModel unit test stubs"""
+class TestTransactionModel(unittest.TestCase):
+    """TransactionModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test TransactionCreateModel
+        """Test TransactionModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.transaction_create_model.TransactionCreateModel()  # noqa: E501
+        # model = data_repo_client.models.transaction_model.TransactionModel()  # noqa: E501
         if include_optional :
-            return TransactionCreateModel(
-                description = '0'
+            return TransactionModel(
+                id = '0', 
+                status = 'active', 
+                lock = '0', 
+                description = '0', 
+                created_at = '0', 
+                created_by = '0', 
+                terminated_at = '0', 
+                terminated_by = '0'
             )
         else :
-            return TransactionCreateModel(
+            return TransactionModel(
+                id = '0',
+                created_at = '0',
+                created_by = '0',
         )
 
-    def testTransactionCreateModel(self):
-        """Test TransactionCreateModel"""
+    def testTransactionModel(self):
+        """Test TransactionModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.55.0/test/test_transaction_model.py` & `data-repo-client-2.56.0/test/test_user_status_info.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,51 +12,46 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.transaction_model import TransactionModel  # noqa: E501
+from data_repo_client.models.user_status_info import UserStatusInfo  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestTransactionModel(unittest.TestCase):
-    """TransactionModel unit test stubs"""
+class TestUserStatusInfo(unittest.TestCase):
+    """UserStatusInfo unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test TransactionModel
+        """Test UserStatusInfo
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.transaction_model.TransactionModel()  # noqa: E501
+        # model = data_repo_client.models.user_status_info.UserStatusInfo()  # noqa: E501
         if include_optional :
-            return TransactionModel(
-                id = '0', 
-                status = 'active', 
-                lock = '0', 
-                description = '0', 
-                created_at = '0', 
-                created_by = '0', 
-                terminated_at = '0', 
-                terminated_by = '0'
+            return UserStatusInfo(
+                user_subject_id = '0', 
+                user_email = '0', 
+                enabled = True
             )
         else :
-            return TransactionModel(
-                id = '0',
-                created_at = '0',
-                created_by = '0',
+            return UserStatusInfo(
+                user_subject_id = '0',
+                user_email = '0',
+                enabled = True,
         )
 
-    def testTransactionModel(self):
-        """Test TransactionModel"""
+    def testUserStatusInfo(self):
+        """Test UserStatusInfo"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.55.0/test/test_unauthenticated_api.py` & `data-repo-client-2.56.0/test/test_unauthenticated_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_unlock_resource_request.py` & `data-repo-client-2.56.0/test/test_workspace_policy_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,43 +12,51 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.unlock_resource_request import UnlockResourceRequest  # noqa: E501
+from data_repo_client.models.workspace_policy_model import WorkspacePolicyModel  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestUnlockResourceRequest(unittest.TestCase):
-    """UnlockResourceRequest unit test stubs"""
+class TestWorkspacePolicyModel(unittest.TestCase):
+    """WorkspacePolicyModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test UnlockResourceRequest
+        """Test WorkspacePolicyModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.unlock_resource_request.UnlockResourceRequest()  # noqa: E501
+        # model = data_repo_client.models.workspace_policy_model.WorkspacePolicyModel()  # noqa: E501
         if include_optional :
-            return UnlockResourceRequest(
-                lock_name = '0', 
-                force_unlock = True
+            return WorkspacePolicyModel(
+                workspace_id = '0', 
+                workspace_name = '0', 
+                workspace_namespace = '0', 
+                workspace_link = '0', 
+                workspace_policies = [
+                    data_repo_client.models.policy_model.PolicyModel(
+                        name = '0', 
+                        members = [
+                            '0'
+                            ], )
+                    ]
             )
         else :
-            return UnlockResourceRequest(
-                lock_name = '0',
+            return WorkspacePolicyModel(
         )
 
-    def testUnlockResourceRequest(self):
-        """Test UnlockResourceRequest"""
+    def testWorkspacePolicyModel(self):
+        """Test WorkspacePolicyModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.55.0/test/test_upgrade_api.py` & `data-repo-client-2.56.0/test/test_upgrade_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_upgrade_model.py` & `data-repo-client-2.56.0/test/test_upgrade_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.55.0/test/test_upgrade_response_model.py` & `data-repo-client-2.56.0/test/test_upgrade_response_model.py`

 * *Files identical despite different names*


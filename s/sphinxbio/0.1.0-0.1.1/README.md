# Comparing `tmp/sphinxbio-0.1.0.tar.gz` & `tmp/sphinxbio-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxbio-0.1.0.tar", max compression
+gzip compressed data, was "sphinxbio-0.1.1.tar", max compression
```

## Comparing `sphinxbio-0.1.0.tar` & `sphinxbio-0.1.1.tar`

### file list

```diff
@@ -1,197 +1,200 @@
--rw-r--r--   0        0        0      392 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/README.md
--rw-r--r--   0        0        0      636 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3706 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/__init__.py
--rw-r--r--   0        0        0      157 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/analyses/__init__.py
--rw-r--r--   0        0        0     9847 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/analyses/client.py
--rw-r--r--   0        0        0      191 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/analyses/types/__init__.py
--rw-r--r--   0        0        0     1878 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/analyses/types/analysis.py
--rw-r--r--   0        0        0     1938 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/analyses/types/paginated_analyses.py
--rw-r--r--   0        0        0      241 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/analysis_templates/__init__.py
--rw-r--r--   0        0        0    15859 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/analysis_templates/client.py
--rw-r--r--   0        0        0      331 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/analysis_templates/types/__init__.py
--rw-r--r--   0        0        0     1678 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/analysis_templates/types/analysis_template.py
--rw-r--r--   0        0        0     1232 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/analysis_templates/types/create_analysis_template.py
--rw-r--r--   0        0        0     1951 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/analysis_templates/types/paginated_analysis_templates.py
--rw-r--r--   0        0        0      227 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/annotations/__init__.py
--rw-r--r--   0        0        0    14188 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/annotations/client.py
--rw-r--r--   0        0        0      308 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/annotations/types/__init__.py
--rw-r--r--   0        0        0     1654 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/annotations/types/annotation.py
--rw-r--r--   0        0        0     1153 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/annotations/types/annotations_pagination_params.py
--rw-r--r--   0        0        0     1785 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/annotations/types/paginated_annotations.py
--rw-r--r--   0        0        0     8359 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/base_client.py
--rw-r--r--   0        0        0      205 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/campaigns/__init__.py
--rw-r--r--   0        0        0    21376 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/campaigns/client.py
--rw-r--r--   0        0        0      275 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/campaigns/types/__init__.py
--rw-r--r--   0        0        0      977 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/campaigns/types/create_campaign.py
--rw-r--r--   0        0        0     1746 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/campaigns/types/paginated_campaigns.py
--rw-r--r--   0        0        0      985 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/campaigns/types/update_campaign.py
--rw-r--r--   0        0        0     2207 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/client.py
--rw-r--r--   0        0        0      853 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/core/api_error.py
--rw-r--r--   0        0        0     2633 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/core/request_options.py
--rw-r--r--   0        0        0      227 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/dataset_schemas/__init__.py
--rw-r--r--   0        0        0    15735 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/dataset_schemas/client.py
--rw-r--r--   0        0        0      310 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/dataset_schemas/types/__init__.py
--rw-r--r--   0        0        0     1002 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/dataset_schemas/types/dataset_schema.py
--rw-r--r--   0        0        0     1452 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/dataset_schemas/types/paginated_dataset_schemas.py
--rw-r--r--   0        0        0     1249 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/dataset_schemas/types/register_dataset_schema.py
--rw-r--r--   0        0        0      242 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/datasets/__init__.py
--rw-r--r--   0        0        0    17200 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/datasets/client.py
--rw-r--r--   0        0        0      144 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/datasets/errors/__init__.py
--rw-r--r--   0        0        0      227 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/datasets/errors/non_csv_file_error.py
--rw-r--r--   0        0        0      247 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/datasets/types/__init__.py
--rw-r--r--   0        0        0     1607 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/datasets/types/create_dataset.py
--rw-r--r--   0        0        0     2128 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/datasets/types/dataset.py
--rw-r--r--   0        0        0     2118 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/datasets/types/paginated_datasets.py
--rw-r--r--   0        0        0      249 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/entities/__init__.py
--rw-r--r--   0        0        0    25656 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/entities/client.py
--rw-r--r--   0        0        0      353 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/entities/types/__init__.py
--rw-r--r--   0        0        0     1499 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/entities/types/create_entity.py
--rw-r--r--   0        0        0     1150 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/entities/types/entities_pagination_params.py
--rw-r--r--   0        0        0     2149 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/entities/types/paginated_entities.py
--rw-r--r--   0        0        0     1003 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/entities/types/update_entity.py
--rw-r--r--   0        0        0      245 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/environment.py
--rw-r--r--   0        0        0      518 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/errors/__init__.py
--rw-r--r--   0        0        0      551 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/errors/errors/__init__.py
--rw-r--r--   0        0        0      307 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/errors/errors/archived_object_error.py
--rw-r--r--   0        0        0      319 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/errors/errors/invalid_staged_file_error.py
--rw-r--r--   0        0        0      219 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/errors/errors/not_authenticated_error.py
--rw-r--r--   0        0        0      216 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/errors/errors/not_authorized_error.py
--rw-r--r--   0        0        0      307 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/errors/errors/object_not_found_error.py
--rw-r--r--   0        0        0      206 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/errors/errors/redirect.py
--rw-r--r--   0        0        0      238 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/errors/types/__init__.py
--rw-r--r--   0        0        0     1011 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/errors/types/invalid_staged_file_body.py
--rw-r--r--   0        0        0     1140 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/errors/types/object_not_found_body.py
--rw-r--r--   0        0        0      830 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/external_tasks/__init__.py
--rw-r--r--   0        0        0     5117 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/external_tasks/client.py
--rw-r--r--   0        0        0      218 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/external_tasks/errors/__init__.py
--rw-r--r--   0        0        0      216 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/external_tasks/errors/invalid_task_content.py
--rw-r--r--   0        0        0      213 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/external_tasks/errors/invalid_task_type.py
--rw-r--r--   0        0        0      908 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/external_tasks/types/__init__.py
--rw-r--r--   0        0        0      957 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/external_tasks/types/create_dataset_task_result.py
--rw-r--r--   0        0        0      833 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/external_tasks/types/failed_task_response.py
--rw-r--r--   0        0        0     1129 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/external_tasks/types/initial_task_response.py
--rw-r--r--   0        0        0      821 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/external_tasks/types/processing_task_response.py
--rw-r--r--   0        0        0      897 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/external_tasks/types/success_task_response.py
--rw-r--r--   0        0        0      519 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/external_tasks/types/sucess_task_result.py
--rw-r--r--   0        0        0       78 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/external_tasks/types/task_id.py
--rw-r--r--   0        0        0     1132 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/external_tasks/types/task_response.py
--rw-r--r--   0        0        0      215 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/files/__init__.py
--rw-r--r--   0        0        0    20231 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/files/client.py
--rw-r--r--   0        0        0      301 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/files/types/__init__.py
--rw-r--r--   0        0        0     1300 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/files/types/create_file.py
--rw-r--r--   0        0        0     1116 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/files/types/download_file_response.py
--rw-r--r--   0        0        0     1687 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/files/types/file.py
--rw-r--r--   0        0        0     2402 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/files/types/paginated_files.py
--rw-r--r--   0        0        0      225 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/filters/__init__.py
--rw-r--r--   0        0        0      308 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/filters/types/__init__.py
--rw-r--r--   0        0        0      923 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/filters/types/created_filter_params.py
--rw-r--r--   0        0        0      198 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/filters/types/datetime_filter_enum.py
--rw-r--r--   0        0        0      923 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/filters/types/updated_filter_params.py
--rw-r--r--   0        0        0      195 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/pagination/__init__.py
--rw-r--r--   0        0        0      260 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/pagination/types/__init__.py
--rw-r--r--   0        0        0      995 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/pagination/types/paginated_response.py
--rw-r--r--   0        0        0     1068 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/pagination/types/pagination_params.py
--rw-r--r--   0        0        0      194 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/pagination/types/sort_enum.py
--rw-r--r--   0        0        0      143 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/plots/__init__.py
--rw-r--r--   0        0        0     9691 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/plots/client.py
--rw-r--r--   0        0        0      170 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/plots/types/__init__.py
--rw-r--r--   0        0        0     1870 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/plots/types/paginated_plots.py
--rw-r--r--   0        0        0     1762 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/plots/types/plot.py
--rw-r--r--   0        0        0     3554 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/shared/__init__.py
--rw-r--r--   0        0        0      254 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/shared/campaign/__init__.py
--rw-r--r--   0        0        0      175 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/shared/campaign/errors/__init__.py
--rw-r--r--   0        0        0      224 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/shared/campaign/errors/campaign_does_not_exist_error.py
--rw-r--r--   0        0        0      235 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/shared/campaign/types/__init__.py
--rw-r--r--   0        0        0     1485 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/shared/campaign/types/campaign.py
--rw-r--r--   0        0        0       82 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/shared/campaign/types/campaign_id.py
--rw-r--r--   0        0        0      842 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/shared/campaign/types/campaign_summary.py
--rw-r--r--   0        0        0      115 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/shared/creator/__init__.py
--rw-r--r--   0        0        0      117 2024-05-02 22:51:32.694858 sphinxbio-0.1.0/src/sphinxbio/shared/creator/types/__init__.py
--rw-r--r--   0        0        0      877 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/creator/types/creator.py
--rw-r--r--   0        0        0      373 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/dataset/__init__.py
--rw-r--r--   0        0        0      507 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/dataset/types/__init__.py
--rw-r--r--   0        0        0     1346 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/dataset/types/dataset_base.py
--rw-r--r--   0        0        0     1054 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/dataset/types/dataset_creator_summary.py
--rw-r--r--   0        0        0       81 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/dataset/types/dataset_id.py
--rw-r--r--   0        0        0     1112 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/dataset/types/dataset_node_summary.py
--rw-r--r--   0        0        0       87 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/dataset/types/dataset_record_id.py
--rw-r--r--   0        0        0      172 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/dataset/types/uploadable_file_types.py
--rw-r--r--   0        0        0     1557 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/__init__.py
--rw-r--r--   0        0        0     2017 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/__init__.py
--rw-r--r--   0        0        0      982 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/amino_acid_sequence.py
--rw-r--r--   0        0        0     1066 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/amino_acid_structure.py
--rw-r--r--   0        0        0      914 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/cell_line.py
--rw-r--r--   0        0        0      939 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/chemical_molecule.py
--rw-r--r--   0        0        0      913 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/control.py
--rw-r--r--   0        0        0     1007 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/create_amino_acid_sequence.py
--rw-r--r--   0        0        0     1002 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/create_amino_acid_structure.py
--rw-r--r--   0        0        0      956 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/create_chemical.py
--rw-r--r--   0        0        0      938 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/create_control.py
--rw-r--r--   0        0        0     1038 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/create_entities_request.py
--rw-r--r--   0        0        0     1855 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/create_entity.py
--rw-r--r--   0        0        0     1036 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/create_entity_base.py
--rw-r--r--   0        0        0      961 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/create_rna_sequence.py
--rw-r--r--   0        0        0      936 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/dna_sequence.py
--rw-r--r--   0        0        0     2965 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/entity.py
--rw-r--r--   0        0        0     1500 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/entity_base.py
--rw-r--r--   0        0        0       80 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/entity_id.py
--rw-r--r--   0        0        0      272 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/entity_types_enum.py
--rw-r--r--   0        0        0      936 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/rna_sequence.py
--rw-r--r--   0        0        0      443 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/filter/__init__.py
--rw-r--r--   0        0        0      208 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/filter/errors/__init__.py
--rw-r--r--   0        0        0      210 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/filter/errors/filter_error.py
--rw-r--r--   0        0        0      218 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/filter/errors/filter_operator_error.py
--rw-r--r--   0        0        0      461 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/filter/types/__init__.py
--rw-r--r--   0        0        0     1039 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/filter/types/composable_filter.py
--rw-r--r--   0        0        0      805 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/filter/types/filter.py
--rw-r--r--   0        0        0      151 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/filter/types/filter_join_enum.py
--rw-r--r--   0        0        0      421 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/filter/types/filter_operator_enum.py
--rw-r--r--   0        0        0      935 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/filter/types/leaf_filter.py
--rw-r--r--   0        0        0      115 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/hit_types/__init__.py
--rw-r--r--   0        0        0      118 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/hit_types/types/__init__.py
--rw-r--r--   0        0        0      879 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/hit_types/types/hit_type.py
--rw-r--r--   0        0        0      139 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/outliers/__init__.py
--rw-r--r--   0        0        0      164 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/outliers/types/__init__.py
--rw-r--r--   0        0        0     1402 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/outliers/types/outlier.py
--rw-r--r--   0        0        0       81 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/outliers/types/outlier_id.py
--rw-r--r--   0        0        0      435 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/sharing/__init__.py
--rw-r--r--   0        0        0      568 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/sharing/types/__init__.py
--rw-r--r--   0        0        0     1163 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/sharing/types/base_share_permission.py
--rw-r--r--   0        0        0      833 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/sharing/types/invite_user_by_email.py
--rw-r--r--   0        0        0      467 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/sharing/types/invite_user_object.py
--rw-r--r--   0        0        0      180 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/sharing/types/permission_access_scope_enum.py
--rw-r--r--   0        0        0      191 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/sharing/types/permission_action_level_enum.py
--rw-r--r--   0        0        0      109 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/sort/__init__.py
--rw-r--r--   0        0        0      108 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/sort/types/__init__.py
--rw-r--r--   0        0        0      836 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/sort/types/sort.py
--rw-r--r--   0        0        0      131 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/tag/__init__.py
--rw-r--r--   0        0        0      152 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/tag/types/__init__.py
--rw-r--r--   0        0        0      860 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/tag/types/create_tag.py
--rw-r--r--   0        0        0      830 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/tag/types/tag.py
--rw-r--r--   0        0        0      134 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/validation/__init__.py
--rw-r--r--   0        0        0      146 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/validation/errors/__init__.py
--rw-r--r--   0        0        0      215 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/validation/errors/invalid_name_error.py
--rw-r--r--   0        0        0      217 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/workflow/__init__.py
--rw-r--r--   0        0        0      304 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/workflow/types/__init__.py
--rw-r--r--   0        0        0     1058 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/workflow/types/create_workflow.py
--rw-r--r--   0        0        0     1233 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/workflow/types/workflow_base.py
--rw-r--r--   0        0        0       82 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/workflow/types/workflow_id.py
--rw-r--r--   0        0        0      271 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/shared/workflow/types/workflow_names.py
--rw-r--r--   0        0        0      169 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/sort/__init__.py
--rw-r--r--   0        0        0      211 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/sort/types/__init__.py
--rw-r--r--   0        0        0      170 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/sort/types/datetime_column_enum.py
--rw-r--r--   0        0        0      918 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/sort/types/sortable_types.py
--rw-r--r--   0        0        0      175 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/storage/__init__.py
--rw-r--r--   0        0        0     5638 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/storage/client.py
--rw-r--r--   0        0        0      220 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/storage/types/__init__.py
--rw-r--r--   0        0        0      864 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/storage/types/presigned_response.py
--rw-r--r--   0        0        0     1045 2024-05-02 22:51:32.698858 sphinxbio-0.1.0/src/sphinxbio/storage/types/upload_url_response.py
--rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 sphinxbio-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      392 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/README.md
+-rw-r--r--   0        0        0      671 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/cli/__init__.py
+-rw-r--r--   0        0        0      874 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/cli/entrypoint.py
+-rw-r--r--   0        0        0     1310 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/cli/utils.py
+-rw-r--r--   0        0        0     3706 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/sphinxbio/__init__.py
+-rw-r--r--   0        0        0      157 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/sphinxbio/analyses/__init__.py
+-rw-r--r--   0        0        0     9847 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/sphinxbio/analyses/client.py
+-rw-r--r--   0        0        0      191 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/sphinxbio/analyses/types/__init__.py
+-rw-r--r--   0        0        0     1878 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/sphinxbio/analyses/types/analysis.py
+-rw-r--r--   0        0        0     1938 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/sphinxbio/analyses/types/paginated_analyses.py
+-rw-r--r--   0        0        0      241 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/sphinxbio/analysis_templates/__init__.py
+-rw-r--r--   0        0        0    15859 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/sphinxbio/analysis_templates/client.py
+-rw-r--r--   0        0        0      331 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/sphinxbio/analysis_templates/types/__init__.py
+-rw-r--r--   0        0        0     1678 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/sphinxbio/analysis_templates/types/analysis_template.py
+-rw-r--r--   0        0        0     1232 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/sphinxbio/analysis_templates/types/create_analysis_template.py
+-rw-r--r--   0        0        0     1951 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/sphinxbio/analysis_templates/types/paginated_analysis_templates.py
+-rw-r--r--   0        0        0      227 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/sphinxbio/annotations/__init__.py
+-rw-r--r--   0        0        0    14188 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/sphinxbio/annotations/client.py
+-rw-r--r--   0        0        0      308 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/sphinxbio/annotations/types/__init__.py
+-rw-r--r--   0        0        0     1654 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/sphinxbio/annotations/types/annotation.py
+-rw-r--r--   0        0        0     1153 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/sphinxbio/annotations/types/annotations_pagination_params.py
+-rw-r--r--   0        0        0     1785 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/sphinxbio/annotations/types/paginated_annotations.py
+-rw-r--r--   0        0        0     8359 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/sphinxbio/base_client.py
+-rw-r--r--   0        0        0      205 2024-05-02 23:11:48.591474 sphinxbio-0.1.1/src/sphinxbio/campaigns/__init__.py
+-rw-r--r--   0        0        0    21376 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/campaigns/client.py
+-rw-r--r--   0        0        0      275 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/campaigns/types/__init__.py
+-rw-r--r--   0        0        0      977 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/campaigns/types/create_campaign.py
+-rw-r--r--   0        0        0     1746 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/campaigns/types/paginated_campaigns.py
+-rw-r--r--   0        0        0      985 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/campaigns/types/update_campaign.py
+-rw-r--r--   0        0        0     2207 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/client.py
+-rw-r--r--   0        0        0      853 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/core/api_error.py
+-rw-r--r--   0        0        0     2633 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/core/request_options.py
+-rw-r--r--   0        0        0      227 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/dataset_schemas/__init__.py
+-rw-r--r--   0        0        0    15735 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/dataset_schemas/client.py
+-rw-r--r--   0        0        0      310 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/dataset_schemas/types/__init__.py
+-rw-r--r--   0        0        0     1002 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/dataset_schemas/types/dataset_schema.py
+-rw-r--r--   0        0        0     1452 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/dataset_schemas/types/paginated_dataset_schemas.py
+-rw-r--r--   0        0        0     1249 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/dataset_schemas/types/register_dataset_schema.py
+-rw-r--r--   0        0        0      242 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/datasets/__init__.py
+-rw-r--r--   0        0        0    17200 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/datasets/client.py
+-rw-r--r--   0        0        0      144 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/datasets/errors/__init__.py
+-rw-r--r--   0        0        0      227 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/datasets/errors/non_csv_file_error.py
+-rw-r--r--   0        0        0      247 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/datasets/types/__init__.py
+-rw-r--r--   0        0        0     1607 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/datasets/types/create_dataset.py
+-rw-r--r--   0        0        0     2128 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/datasets/types/dataset.py
+-rw-r--r--   0        0        0     2118 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/datasets/types/paginated_datasets.py
+-rw-r--r--   0        0        0      249 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/entities/__init__.py
+-rw-r--r--   0        0        0    25656 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/entities/client.py
+-rw-r--r--   0        0        0      353 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/entities/types/__init__.py
+-rw-r--r--   0        0        0     1499 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/entities/types/create_entity.py
+-rw-r--r--   0        0        0     1150 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/entities/types/entities_pagination_params.py
+-rw-r--r--   0        0        0     2149 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/entities/types/paginated_entities.py
+-rw-r--r--   0        0        0     1003 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/entities/types/update_entity.py
+-rw-r--r--   0        0        0      245 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/environment.py
+-rw-r--r--   0        0        0      518 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/errors/__init__.py
+-rw-r--r--   0        0        0      551 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/errors/errors/__init__.py
+-rw-r--r--   0        0        0      307 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/errors/errors/archived_object_error.py
+-rw-r--r--   0        0        0      319 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/errors/errors/invalid_staged_file_error.py
+-rw-r--r--   0        0        0      219 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/errors/errors/not_authenticated_error.py
+-rw-r--r--   0        0        0      216 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/errors/errors/not_authorized_error.py
+-rw-r--r--   0        0        0      307 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/errors/errors/object_not_found_error.py
+-rw-r--r--   0        0        0      206 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/errors/errors/redirect.py
+-rw-r--r--   0        0        0      238 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/errors/types/__init__.py
+-rw-r--r--   0        0        0     1011 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/errors/types/invalid_staged_file_body.py
+-rw-r--r--   0        0        0     1140 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/errors/types/object_not_found_body.py
+-rw-r--r--   0        0        0      830 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/external_tasks/__init__.py
+-rw-r--r--   0        0        0     5117 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/external_tasks/client.py
+-rw-r--r--   0        0        0      218 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/external_tasks/errors/__init__.py
+-rw-r--r--   0        0        0      216 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/external_tasks/errors/invalid_task_content.py
+-rw-r--r--   0        0        0      213 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/external_tasks/errors/invalid_task_type.py
+-rw-r--r--   0        0        0      908 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/external_tasks/types/__init__.py
+-rw-r--r--   0        0        0      957 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/external_tasks/types/create_dataset_task_result.py
+-rw-r--r--   0        0        0      833 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/external_tasks/types/failed_task_response.py
+-rw-r--r--   0        0        0     1129 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/external_tasks/types/initial_task_response.py
+-rw-r--r--   0        0        0      821 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/external_tasks/types/processing_task_response.py
+-rw-r--r--   0        0        0      897 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/external_tasks/types/success_task_response.py
+-rw-r--r--   0        0        0      519 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/external_tasks/types/sucess_task_result.py
+-rw-r--r--   0        0        0       78 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/external_tasks/types/task_id.py
+-rw-r--r--   0        0        0     1132 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/external_tasks/types/task_response.py
+-rw-r--r--   0        0        0      215 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/files/__init__.py
+-rw-r--r--   0        0        0    20231 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/files/client.py
+-rw-r--r--   0        0        0      301 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/files/types/__init__.py
+-rw-r--r--   0        0        0     1300 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/files/types/create_file.py
+-rw-r--r--   0        0        0     1116 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/files/types/download_file_response.py
+-rw-r--r--   0        0        0     1687 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/files/types/file.py
+-rw-r--r--   0        0        0     2402 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/files/types/paginated_files.py
+-rw-r--r--   0        0        0      225 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/filters/__init__.py
+-rw-r--r--   0        0        0      308 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/filters/types/__init__.py
+-rw-r--r--   0        0        0      923 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/filters/types/created_filter_params.py
+-rw-r--r--   0        0        0      198 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/filters/types/datetime_filter_enum.py
+-rw-r--r--   0        0        0      923 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/filters/types/updated_filter_params.py
+-rw-r--r--   0        0        0      195 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/pagination/__init__.py
+-rw-r--r--   0        0        0      260 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/pagination/types/__init__.py
+-rw-r--r--   0        0        0      995 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/pagination/types/paginated_response.py
+-rw-r--r--   0        0        0     1068 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/pagination/types/pagination_params.py
+-rw-r--r--   0        0        0      194 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/pagination/types/sort_enum.py
+-rw-r--r--   0        0        0      143 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/plots/__init__.py
+-rw-r--r--   0        0        0     9691 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/plots/client.py
+-rw-r--r--   0        0        0      170 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/plots/types/__init__.py
+-rw-r--r--   0        0        0     1870 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/plots/types/paginated_plots.py
+-rw-r--r--   0        0        0     1762 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/plots/types/plot.py
+-rw-r--r--   0        0        0     3554 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/__init__.py
+-rw-r--r--   0        0        0      254 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/campaign/__init__.py
+-rw-r--r--   0        0        0      175 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/campaign/errors/__init__.py
+-rw-r--r--   0        0        0      224 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/campaign/errors/campaign_does_not_exist_error.py
+-rw-r--r--   0        0        0      235 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/campaign/types/__init__.py
+-rw-r--r--   0        0        0     1485 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/campaign/types/campaign.py
+-rw-r--r--   0        0        0       82 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/campaign/types/campaign_id.py
+-rw-r--r--   0        0        0      842 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/campaign/types/campaign_summary.py
+-rw-r--r--   0        0        0      115 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/creator/__init__.py
+-rw-r--r--   0        0        0      117 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/creator/types/__init__.py
+-rw-r--r--   0        0        0      877 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/creator/types/creator.py
+-rw-r--r--   0        0        0      373 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/dataset/__init__.py
+-rw-r--r--   0        0        0      507 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/dataset/types/__init__.py
+-rw-r--r--   0        0        0     1346 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/dataset/types/dataset_base.py
+-rw-r--r--   0        0        0     1054 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/dataset/types/dataset_creator_summary.py
+-rw-r--r--   0        0        0       81 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/dataset/types/dataset_id.py
+-rw-r--r--   0        0        0     1112 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/dataset/types/dataset_node_summary.py
+-rw-r--r--   0        0        0       87 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/dataset/types/dataset_record_id.py
+-rw-r--r--   0        0        0      172 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/dataset/types/uploadable_file_types.py
+-rw-r--r--   0        0        0     1557 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/__init__.py
+-rw-r--r--   0        0        0     2017 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/__init__.py
+-rw-r--r--   0        0        0      982 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/amino_acid_sequence.py
+-rw-r--r--   0        0        0     1066 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/amino_acid_structure.py
+-rw-r--r--   0        0        0      914 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/cell_line.py
+-rw-r--r--   0        0        0      939 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/chemical_molecule.py
+-rw-r--r--   0        0        0      913 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/control.py
+-rw-r--r--   0        0        0     1007 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/create_amino_acid_sequence.py
+-rw-r--r--   0        0        0     1002 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/create_amino_acid_structure.py
+-rw-r--r--   0        0        0      956 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/create_chemical.py
+-rw-r--r--   0        0        0      938 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/create_control.py
+-rw-r--r--   0        0        0     1038 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/create_entities_request.py
+-rw-r--r--   0        0        0     1855 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/create_entity.py
+-rw-r--r--   0        0        0     1036 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/create_entity_base.py
+-rw-r--r--   0        0        0      961 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/create_rna_sequence.py
+-rw-r--r--   0        0        0      936 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/dna_sequence.py
+-rw-r--r--   0        0        0     2965 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/entity.py
+-rw-r--r--   0        0        0     1500 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/entity_base.py
+-rw-r--r--   0        0        0       80 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/entity_id.py
+-rw-r--r--   0        0        0      272 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/entity_types_enum.py
+-rw-r--r--   0        0        0      936 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/rna_sequence.py
+-rw-r--r--   0        0        0      443 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/filter/__init__.py
+-rw-r--r--   0        0        0      208 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/filter/errors/__init__.py
+-rw-r--r--   0        0        0      210 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/filter/errors/filter_error.py
+-rw-r--r--   0        0        0      218 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/filter/errors/filter_operator_error.py
+-rw-r--r--   0        0        0      461 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/filter/types/__init__.py
+-rw-r--r--   0        0        0     1039 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/filter/types/composable_filter.py
+-rw-r--r--   0        0        0      805 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/filter/types/filter.py
+-rw-r--r--   0        0        0      151 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/filter/types/filter_join_enum.py
+-rw-r--r--   0        0        0      421 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/filter/types/filter_operator_enum.py
+-rw-r--r--   0        0        0      935 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/filter/types/leaf_filter.py
+-rw-r--r--   0        0        0      115 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/hit_types/__init__.py
+-rw-r--r--   0        0        0      118 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/hit_types/types/__init__.py
+-rw-r--r--   0        0        0      879 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/hit_types/types/hit_type.py
+-rw-r--r--   0        0        0      139 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/outliers/__init__.py
+-rw-r--r--   0        0        0      164 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/outliers/types/__init__.py
+-rw-r--r--   0        0        0     1402 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/outliers/types/outlier.py
+-rw-r--r--   0        0        0       81 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/outliers/types/outlier_id.py
+-rw-r--r--   0        0        0      435 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/sharing/__init__.py
+-rw-r--r--   0        0        0      568 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/sharing/types/__init__.py
+-rw-r--r--   0        0        0     1163 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/sharing/types/base_share_permission.py
+-rw-r--r--   0        0        0      833 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/sharing/types/invite_user_by_email.py
+-rw-r--r--   0        0        0      467 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/sharing/types/invite_user_object.py
+-rw-r--r--   0        0        0      180 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/sharing/types/permission_access_scope_enum.py
+-rw-r--r--   0        0        0      191 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/sharing/types/permission_action_level_enum.py
+-rw-r--r--   0        0        0      109 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/sort/__init__.py
+-rw-r--r--   0        0        0      108 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/sort/types/__init__.py
+-rw-r--r--   0        0        0      836 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/sort/types/sort.py
+-rw-r--r--   0        0        0      131 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/tag/__init__.py
+-rw-r--r--   0        0        0      152 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/tag/types/__init__.py
+-rw-r--r--   0        0        0      860 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/tag/types/create_tag.py
+-rw-r--r--   0        0        0      830 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/tag/types/tag.py
+-rw-r--r--   0        0        0      134 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/validation/__init__.py
+-rw-r--r--   0        0        0      146 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/validation/errors/__init__.py
+-rw-r--r--   0        0        0      215 2024-05-02 23:11:48.595474 sphinxbio-0.1.1/src/sphinxbio/shared/validation/errors/invalid_name_error.py
+-rw-r--r--   0        0        0      217 2024-05-02 23:11:48.599474 sphinxbio-0.1.1/src/sphinxbio/shared/workflow/__init__.py
+-rw-r--r--   0        0        0      304 2024-05-02 23:11:48.599474 sphinxbio-0.1.1/src/sphinxbio/shared/workflow/types/__init__.py
+-rw-r--r--   0        0        0     1058 2024-05-02 23:11:48.599474 sphinxbio-0.1.1/src/sphinxbio/shared/workflow/types/create_workflow.py
+-rw-r--r--   0        0        0     1233 2024-05-02 23:11:48.599474 sphinxbio-0.1.1/src/sphinxbio/shared/workflow/types/workflow_base.py
+-rw-r--r--   0        0        0       82 2024-05-02 23:11:48.599474 sphinxbio-0.1.1/src/sphinxbio/shared/workflow/types/workflow_id.py
+-rw-r--r--   0        0        0      271 2024-05-02 23:11:48.599474 sphinxbio-0.1.1/src/sphinxbio/shared/workflow/types/workflow_names.py
+-rw-r--r--   0        0        0      169 2024-05-02 23:11:48.599474 sphinxbio-0.1.1/src/sphinxbio/sort/__init__.py
+-rw-r--r--   0        0        0      211 2024-05-02 23:11:48.599474 sphinxbio-0.1.1/src/sphinxbio/sort/types/__init__.py
+-rw-r--r--   0        0        0      170 2024-05-02 23:11:48.599474 sphinxbio-0.1.1/src/sphinxbio/sort/types/datetime_column_enum.py
+-rw-r--r--   0        0        0      918 2024-05-02 23:11:48.599474 sphinxbio-0.1.1/src/sphinxbio/sort/types/sortable_types.py
+-rw-r--r--   0        0        0      175 2024-05-02 23:11:48.599474 sphinxbio-0.1.1/src/sphinxbio/storage/__init__.py
+-rw-r--r--   0        0        0     5638 2024-05-02 23:11:48.599474 sphinxbio-0.1.1/src/sphinxbio/storage/client.py
+-rw-r--r--   0        0        0      220 2024-05-02 23:11:48.599474 sphinxbio-0.1.1/src/sphinxbio/storage/types/__init__.py
+-rw-r--r--   0        0        0      864 2024-05-02 23:11:48.599474 sphinxbio-0.1.1/src/sphinxbio/storage/types/presigned_response.py
+-rw-r--r--   0        0        0     1045 2024-05-02 23:11:48.599474 sphinxbio-0.1.1/src/sphinxbio/storage/types/upload_url_response.py
+-rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 sphinxbio-0.1.1/PKG-INFO
```

### Comparing `sphinxbio-0.1.0/pyproject.toml` & `sphinxbio-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "sphinxbio"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
-    { include = "sphinxbio", from = "src"}
+    { include = "sphinxbio", from = "src"},
+    { include = "cli", from = "src"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = ">=0.21.2"
 pydantic = "2.7.1"
 ipykernel = "^6.29.4"
@@ -21,15 +22,15 @@
 pytest = "^7.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-sb = "src.cli.entrypoint:cli"
+sb = "cli.entrypoint:cli"
 
 
 [tool.mypy]
 plugins = ["pydantic.mypy"]
 
 [[tool.mypy.overrides]]
 module = [
```

### Comparing `sphinxbio-0.1.0/src/sphinxbio/__init__.py` & `sphinxbio-0.1.1/src/sphinxbio/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/analyses/client.py` & `sphinxbio-0.1.1/src/sphinxbio/analyses/client.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/analyses/types/analysis.py` & `sphinxbio-0.1.1/src/sphinxbio/analyses/types/analysis.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/analyses/types/paginated_analyses.py` & `sphinxbio-0.1.1/src/sphinxbio/analyses/types/paginated_analyses.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/analysis_templates/client.py` & `sphinxbio-0.1.1/src/sphinxbio/analysis_templates/client.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/analysis_templates/types/analysis_template.py` & `sphinxbio-0.1.1/src/sphinxbio/analysis_templates/types/analysis_template.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/analysis_templates/types/create_analysis_template.py` & `sphinxbio-0.1.1/src/sphinxbio/analysis_templates/types/create_analysis_template.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/analysis_templates/types/paginated_analysis_templates.py` & `sphinxbio-0.1.1/src/sphinxbio/analysis_templates/types/paginated_analysis_templates.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/annotations/client.py` & `sphinxbio-0.1.1/src/sphinxbio/annotations/client.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/annotations/types/annotation.py` & `sphinxbio-0.1.1/src/sphinxbio/annotations/types/annotation.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/annotations/types/annotations_pagination_params.py` & `sphinxbio-0.1.1/src/sphinxbio/annotations/types/annotations_pagination_params.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/annotations/types/paginated_annotations.py` & `sphinxbio-0.1.1/src/sphinxbio/annotations/types/paginated_annotations.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/base_client.py` & `sphinxbio-0.1.1/src/sphinxbio/base_client.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/campaigns/client.py` & `sphinxbio-0.1.1/src/sphinxbio/campaigns/client.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/campaigns/types/create_campaign.py` & `sphinxbio-0.1.1/src/sphinxbio/campaigns/types/create_campaign.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/campaigns/types/paginated_campaigns.py` & `sphinxbio-0.1.1/src/sphinxbio/campaigns/types/paginated_campaigns.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/campaigns/types/update_campaign.py` & `sphinxbio-0.1.1/src/sphinxbio/campaigns/types/update_campaign.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/client.py` & `sphinxbio-0.1.1/src/sphinxbio/client.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/core/__init__.py` & `sphinxbio-0.1.1/src/sphinxbio/core/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/core/client_wrapper.py` & `sphinxbio-0.1.1/src/sphinxbio/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/core/datetime_utils.py` & `sphinxbio-0.1.1/src/sphinxbio/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/core/file.py` & `sphinxbio-0.1.1/src/sphinxbio/core/file.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/core/http_client.py` & `sphinxbio-0.1.1/src/sphinxbio/core/http_client.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/core/jsonable_encoder.py` & `sphinxbio-0.1.1/src/sphinxbio/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/core/request_options.py` & `sphinxbio-0.1.1/src/sphinxbio/core/request_options.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/dataset_schemas/client.py` & `sphinxbio-0.1.1/src/sphinxbio/dataset_schemas/client.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/dataset_schemas/types/dataset_schema.py` & `sphinxbio-0.1.1/src/sphinxbio/dataset_schemas/types/dataset_schema.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/dataset_schemas/types/paginated_dataset_schemas.py` & `sphinxbio-0.1.1/src/sphinxbio/dataset_schemas/types/paginated_dataset_schemas.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/dataset_schemas/types/register_dataset_schema.py` & `sphinxbio-0.1.1/src/sphinxbio/dataset_schemas/types/register_dataset_schema.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/datasets/client.py` & `sphinxbio-0.1.1/src/sphinxbio/datasets/client.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/datasets/types/create_dataset.py` & `sphinxbio-0.1.1/src/sphinxbio/datasets/types/create_dataset.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/datasets/types/dataset.py` & `sphinxbio-0.1.1/src/sphinxbio/datasets/types/dataset.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/datasets/types/paginated_datasets.py` & `sphinxbio-0.1.1/src/sphinxbio/datasets/types/paginated_datasets.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/entities/client.py` & `sphinxbio-0.1.1/src/sphinxbio/entities/client.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/entities/types/create_entity.py` & `sphinxbio-0.1.1/src/sphinxbio/entities/types/create_entity.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/entities/types/entities_pagination_params.py` & `sphinxbio-0.1.1/src/sphinxbio/entities/types/entities_pagination_params.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/entities/types/paginated_entities.py` & `sphinxbio-0.1.1/src/sphinxbio/entities/types/paginated_entities.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/entities/types/update_entity.py` & `sphinxbio-0.1.1/src/sphinxbio/entities/types/update_entity.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/errors/__init__.py` & `sphinxbio-0.1.1/src/sphinxbio/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/errors/errors/__init__.py` & `sphinxbio-0.1.1/src/sphinxbio/errors/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/errors/types/invalid_staged_file_body.py` & `sphinxbio-0.1.1/src/sphinxbio/errors/types/invalid_staged_file_body.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/errors/types/object_not_found_body.py` & `sphinxbio-0.1.1/src/sphinxbio/errors/types/object_not_found_body.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/external_tasks/__init__.py` & `sphinxbio-0.1.1/src/sphinxbio/external_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/external_tasks/client.py` & `sphinxbio-0.1.1/src/sphinxbio/external_tasks/client.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/external_tasks/types/__init__.py` & `sphinxbio-0.1.1/src/sphinxbio/external_tasks/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/external_tasks/types/create_dataset_task_result.py` & `sphinxbio-0.1.1/src/sphinxbio/external_tasks/types/create_dataset_task_result.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/external_tasks/types/failed_task_response.py` & `sphinxbio-0.1.1/src/sphinxbio/external_tasks/types/failed_task_response.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/external_tasks/types/initial_task_response.py` & `sphinxbio-0.1.1/src/sphinxbio/external_tasks/types/initial_task_response.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/external_tasks/types/processing_task_response.py` & `sphinxbio-0.1.1/src/sphinxbio/external_tasks/types/processing_task_response.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/external_tasks/types/success_task_response.py` & `sphinxbio-0.1.1/src/sphinxbio/external_tasks/types/success_task_response.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/external_tasks/types/sucess_task_result.py` & `sphinxbio-0.1.1/src/sphinxbio/external_tasks/types/sucess_task_result.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/external_tasks/types/task_response.py` & `sphinxbio-0.1.1/src/sphinxbio/external_tasks/types/task_response.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/files/client.py` & `sphinxbio-0.1.1/src/sphinxbio/files/client.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/files/types/create_file.py` & `sphinxbio-0.1.1/src/sphinxbio/files/types/create_file.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/files/types/download_file_response.py` & `sphinxbio-0.1.1/src/sphinxbio/files/types/download_file_response.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/files/types/file.py` & `sphinxbio-0.1.1/src/sphinxbio/files/types/file.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/files/types/paginated_files.py` & `sphinxbio-0.1.1/src/sphinxbio/files/types/paginated_files.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/filters/types/created_filter_params.py` & `sphinxbio-0.1.1/src/sphinxbio/filters/types/created_filter_params.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/filters/types/updated_filter_params.py` & `sphinxbio-0.1.1/src/sphinxbio/filters/types/updated_filter_params.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/pagination/types/paginated_response.py` & `sphinxbio-0.1.1/src/sphinxbio/pagination/types/paginated_response.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/pagination/types/pagination_params.py` & `sphinxbio-0.1.1/src/sphinxbio/pagination/types/pagination_params.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/plots/client.py` & `sphinxbio-0.1.1/src/sphinxbio/plots/client.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/plots/types/paginated_plots.py` & `sphinxbio-0.1.1/src/sphinxbio/plots/types/paginated_plots.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/plots/types/plot.py` & `sphinxbio-0.1.1/src/sphinxbio/plots/types/plot.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/__init__.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/campaign/types/campaign.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/campaign/types/campaign.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/campaign/types/campaign_summary.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/campaign/types/campaign_summary.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/creator/types/creator.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/creator/types/creator.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/dataset/types/dataset_base.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/dataset/types/dataset_base.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/dataset/types/dataset_creator_summary.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/dataset/types/dataset_creator_summary.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/dataset/types/dataset_node_summary.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/dataset/types/dataset_node_summary.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/entity/__init__.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/__init__.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/amino_acid_sequence.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/amino_acid_sequence.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/amino_acid_structure.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/amino_acid_structure.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/cell_line.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/cell_line.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/chemical_molecule.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/chemical_molecule.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/control.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/control.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/create_amino_acid_sequence.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/create_amino_acid_sequence.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/create_amino_acid_structure.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/create_amino_acid_structure.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/create_chemical.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/create_chemical.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/create_control.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/create_control.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/create_entities_request.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/create_entities_request.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/create_entity.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/create_entity.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/create_entity_base.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/create_entity_base.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/create_rna_sequence.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/create_rna_sequence.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/dna_sequence.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/dna_sequence.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/entity.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/entity.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/entity_base.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/entity_base.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/entity/types/rna_sequence.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/entity/types/rna_sequence.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/filter/types/composable_filter.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/filter/types/composable_filter.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/filter/types/filter.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/filter/types/filter.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/filter/types/leaf_filter.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/filter/types/leaf_filter.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/hit_types/types/hit_type.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/hit_types/types/hit_type.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/outliers/types/outlier.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/outliers/types/outlier.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/sharing/types/__init__.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/sharing/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/sharing/types/base_share_permission.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/sharing/types/base_share_permission.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/sharing/types/invite_user_by_email.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/sharing/types/invite_user_by_email.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/sort/types/sort.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/sort/types/sort.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/tag/types/create_tag.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/tag/types/create_tag.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/tag/types/tag.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/tag/types/tag.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/workflow/types/create_workflow.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/workflow/types/create_workflow.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/shared/workflow/types/workflow_base.py` & `sphinxbio-0.1.1/src/sphinxbio/shared/workflow/types/workflow_base.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/sort/types/sortable_types.py` & `sphinxbio-0.1.1/src/sphinxbio/sort/types/sortable_types.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/storage/client.py` & `sphinxbio-0.1.1/src/sphinxbio/storage/client.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/storage/types/presigned_response.py` & `sphinxbio-0.1.1/src/sphinxbio/storage/types/presigned_response.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/src/sphinxbio/storage/types/upload_url_response.py` & `sphinxbio-0.1.1/src/sphinxbio/storage/types/upload_url_response.py`

 * *Files identical despite different names*

### Comparing `sphinxbio-0.1.0/PKG-INFO` & `sphinxbio-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxbio
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


# Comparing `tmp/trycourier-6.0.3.tar.gz` & `tmp/trycourier-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trycourier-6.0.3.tar", max compression
+gzip compressed data, was "trycourier-6.0.4.tar", max compression
```

## Comparing `trycourier-6.0.3.tar` & `trycourier-6.0.4.tar`

### file list

```diff
@@ -1,366 +1,366 @@
--rw-r--r--   0        0        0     1063 2024-05-01 02:48:53.976418 trycourier-6.0.3/LICENSE
--rw-r--r--   0        0        0     5507 2024-05-01 02:48:53.976418 trycourier-6.0.3/README.md
--rw-r--r--   0        0        0      595 2024-05-01 02:48:53.976418 trycourier-6.0.3/pyproject.toml
--rw-r--r--   0        0        0    14108 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/__init__.py
--rw-r--r--   0        0        0      751 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/__init__.py
--rw-r--r--   0        0        0    28202 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/client.py
--rw-r--r--   0        0        0     1100 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/__init__.py
--rw-r--r--   0        0        0     1199 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/audience.py
--rw-r--r--   0        0        0      971 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/audience_list_response.py
--rw-r--r--   0        0        0      939 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/audience_member.py
--rw-r--r--   0        0        0     1052 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/audience_member_get_response.py
--rw-r--r--   0        0        0      996 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/audience_member_list_response.py
--rw-r--r--   0        0        0      901 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/audience_update_response.py
--rw-r--r--   0        0        0      971 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/base_filter_config.py
--rw-r--r--   0        0        0      386 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/comparison_operator.py
--rw-r--r--   0        0        0      249 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/filter.py
--rw-r--r--   0        0        0      255 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/filter_config.py
--rw-r--r--   0        0        0      152 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/logical_operator.py
--rw-r--r--   0        0        0     1191 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/nested_filter_config.py
--rw-r--r--   0        0        0      240 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/operator.py
--rw-r--r--   0        0        0     1252 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/single_filter_config.py
--rw-r--r--   0        0        0      299 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audit_events/__init__.py
--rw-r--r--   0        0        0    10417 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audit_events/client.py
--rw-r--r--   0        0        0      453 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audit_events/types/__init__.py
--rw-r--r--   0        0        0      905 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audit_events/types/actor.py
--rw-r--r--   0        0        0     1164 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audit_events/types/audit_event.py
--rw-r--r--   0        0        0      988 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audit_events/types/get_audit_event_params.py
--rw-r--r--   0        0        0      886 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audit_events/types/list_audit_events_params.py
--rw-r--r--   0        0        0      983 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audit_events/types/list_audit_events_response.py
--rw-r--r--   0        0        0      906 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audit_events/types/target.py
--rw-r--r--   0        0        0      137 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/auth_tokens/__init__.py
--rw-r--r--   0        0        0     7229 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/auth_tokens/client.py
--rw-r--r--   0        0        0      152 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/auth_tokens/types/__init__.py
--rw-r--r--   0        0        0      882 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/auth_tokens/types/issue_token_response.py
--rw-r--r--   0        0        0     1847 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/__init__.py
--rw-r--r--   0        0        0    16885 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/client.py
--rw-r--r--   0        0        0     2836 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/__init__.py
--rw-r--r--   0        0        0      962 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/accessor_type.py
--rw-r--r--   0        0        0      988 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation.py
--rw-r--r--   0        0        0     1054 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_ad_hoc_invoke_params.py
--rw-r--r--   0        0        0      138 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_add_to_batch_max_items_type.py
--rw-r--r--   0        0        0     1954 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_add_to_batch_retain.py
--rw-r--r--   0        0        0      192 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_add_to_batch_retain_type.py
--rw-r--r--   0        0        0      178 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_add_to_batch_scope.py
--rw-r--r--   0        0        0     3128 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_add_to_batch_step.py
--rw-r--r--   0        0        0     1355 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_add_to_digest_step.py
--rw-r--r--   0        0        0     1048 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_cancel_step.py
--rw-r--r--   0        0        0     1331 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_delay_step.py
--rw-r--r--   0        0        0     1784 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_fetch_data_step.py
--rw-r--r--   0        0        0     1186 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_fetch_data_webhook.py
--rw-r--r--   0        0        0      171 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_fetch_data_webhook_method.py
--rw-r--r--   0        0        0     1108 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_invoke_params.py
--rw-r--r--   0        0        0      978 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_invoke_response.py
--rw-r--r--   0        0        0     1015 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_invoke_step.py
--rw-r--r--   0        0        0     1056 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_invoke_template_params.py
--rw-r--r--   0        0        0     1088 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_run_context.py
--rw-r--r--   0        0        0     1262 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_send_list_step.py
--rw-r--r--   0        0        0     1295 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_send_step.py
--rw-r--r--   0        0        0     1030 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_step.py
--rw-r--r--   0        0        0     1102 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_step_option.py
--rw-r--r--   0        0        0     1052 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_throttle_on_throttle.py
--rw-r--r--   0        0        0      176 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_throttle_scope.py
--rw-r--r--   0        0        0     2301 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_throttle_step.py
--rw-r--r--   0        0        0     1039 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_update_profile_step.py
--rw-r--r--   0        0        0     1058 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_v_2_send_step.py
--rw-r--r--   0        0        0      184 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/merge_algorithm.py
--rw-r--r--   0        0        0      101 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/profile.py
--rw-r--r--   0        0        0      419 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/__init__.py
--rw-r--r--   0        0        0    29995 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/client.py
--rw-r--r--   0        0        0      579 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/types/__init__.py
--rw-r--r--   0        0        0     1716 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/types/brand.py
--rw-r--r--   0        0        0      962 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/types/brand_colors.py
--rw-r--r--   0        0        0      963 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/types/brand_get_all_response.py
--rw-r--r--   0        0        0     1120 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/types/brand_parameters.py
--rw-r--r--   0        0        0     1052 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/types/brand_settings.py
--rw-r--r--   0        0        0      907 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/types/brand_snippet.py
--rw-r--r--   0        0        0      915 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/types/brand_snippets.py
--rw-r--r--   0        0        0      958 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/types/brands_response.py
--rw-r--r--   0        0        0     1059 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/__init__.py
--rw-r--r--   0        0        0    30912 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/client.py
--rw-r--r--   0        0        0     1603 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/__init__.py
--rw-r--r--   0        0        0      975 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_create_job_response.py
--rw-r--r--   0        0        0      970 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_get_job_params.py
--rw-r--r--   0        0        0      899 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_get_job_response.py
--rw-r--r--   0        0        0     1015 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_get_job_users_params.py
--rw-r--r--   0        0        0     1022 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_get_job_users_response.py
--rw-r--r--   0        0        0      883 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_ingest_error.py
--rw-r--r--   0        0        0      955 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_ingest_users_params.py
--rw-r--r--   0        0        0      975 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_ingest_users_response.py
--rw-r--r--   0        0        0      184 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_job_status.py
--rw-r--r--   0        0        0      173 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_job_user_status.py
--rw-r--r--   0        0        0     1161 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_message_user_response.py
--rw-r--r--   0        0        0     1512 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_content_message.py
--rw-r--r--   0        0        0     1096 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_message.py
--rw-r--r--   0        0        0     1218 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_message_user.py
--rw-r--r--   0        0        0     1672 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_message_v_1.py
--rw-r--r--   0        0        0      310 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_message_v_2.py
--rw-r--r--   0        0        0     1165 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_template_message.py
--rw-r--r--   0        0        0     1046 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/job_details.py
--rw-r--r--   0        0        0    17491 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/client.py
--rw-r--r--   0        0        0     1127 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/__init__.py
--rw-r--r--   0        0        0      527 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/errors/__init__.py
--rw-r--r--   0        0        0      289 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/errors/already_exists_error.py
--rw-r--r--   0        0        0      277 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/errors/bad_request_error.py
--rw-r--r--   0        0        0      268 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/errors/conflict_error.py
--rw-r--r--   0        0        0      298 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/errors/message_not_found_error.py
--rw-r--r--   0        0        0      269 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/errors/not_found_error.py
--rw-r--r--   0        0        0      297 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/errors/payment_required_error.py
--rw-r--r--   0        0        0     1207 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/__init__.py
--rw-r--r--   0        0        0      988 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/already_exists.py
--rw-r--r--   0        0        0      985 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/bad_request.py
--rw-r--r--   0        0        0      939 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/base_error.py
--rw-r--r--   0        0        0      213 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/channel_classification.py
--rw-r--r--   0        0        0      935 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/channel_preference.py
--rw-r--r--   0        0        0      983 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/conflict.py
--rw-r--r--   0        0        0      876 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/email.py
--rw-r--r--   0        0        0      990 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/message_not_found.py
--rw-r--r--   0        0        0      983 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/not_found.py
--rw-r--r--   0        0        0     1137 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/notification_preference_details.py
--rw-r--r--   0        0        0      230 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/notification_preferences.py
--rw-r--r--   0        0        0      886 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/paging.py
--rw-r--r--   0        0        0      988 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/payment_required.py
--rw-r--r--   0        0        0      177 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/preference_status.py
--rw-r--r--   0        0        0     1038 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/recipient_preferences.py
--rw-r--r--   0        0        0      883 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/rule.py
--rw-r--r--   0        0        0     1353 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/user_tenant_association.py
--rw-r--r--   0        0        0      853 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/core/api_error.py
--rw-r--r--   0        0        0     2088 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/core/request_options.py
--rw-r--r--   0        0        0      159 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/environment.py
--rw-r--r--   0        0        0      413 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/lists/__init__.py
--rw-r--r--   0        0        0    69860 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/lists/client.py
--rw-r--r--   0        0        0      569 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/lists/types/__init__.py
--rw-r--r--   0        0        0      937 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/lists/types/list.py
--rw-r--r--   0        0        0      957 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/lists/types/list_get_all_response.py
--rw-r--r--   0        0        0     1032 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/lists/types/list_get_subscriptions_response.py
--rw-r--r--   0        0        0      986 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/lists/types/list_put_params.py
--rw-r--r--   0        0        0     1166 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/lists/types/list_subscription_recipient.py
--rw-r--r--   0        0        0     1125 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/lists/types/put_subscriptions_recipient.py
--rw-r--r--   0        0        0      527 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/__init__.py
--rw-r--r--   0        0        0    41212 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/client.py
--rw-r--r--   0        0        0      747 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/types/__init__.py
--rw-r--r--   0        0        0     1157 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/types/list_messages_response.py
--rw-r--r--   0        0        0     2811 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/types/message_details.py
--rw-r--r--   0        0        0      932 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/types/message_history_response.py
--rw-r--r--   0        0        0      357 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/types/message_status.py
--rw-r--r--   0        0        0      233 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/types/reason.py
--rw-r--r--   0        0        0     1234 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/types/render_output.py
--rw-r--r--   0        0        0     1022 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/types/render_output_response.py
--rw-r--r--   0        0        0     1050 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/types/rendered_message_block.py
--rw-r--r--   0        0        0     1499 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/types/rendered_message_content.py
--rw-r--r--   0        0        0      985 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/__init__.py
--rw-r--r--   0        0        0    45003 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/client.py
--rw-r--r--   0        0        0     1463 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/__init__.py
--rw-r--r--   0        0        0      943 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/base_check.py
--rw-r--r--   0        0        0      229 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/block_type.py
--rw-r--r--   0        0        0      947 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/check.py
--rw-r--r--   0        0        0      168 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/check_status.py
--rw-r--r--   0        0        0     1127 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/message_routing.py
--rw-r--r--   0        0        0      183 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/message_routing_channel.py
--rw-r--r--   0        0        0      161 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/message_routing_method.py
--rw-r--r--   0        0        0      941 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/notification.py
--rw-r--r--   0        0        0     1216 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/notification_block.py
--rw-r--r--   0        0        0     1151 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/notification_channel.py
--rw-r--r--   0        0        0      931 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/notification_channel_content.py
--rw-r--r--   0        0        0      224 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/notification_content.py
--rw-r--r--   0        0        0      935 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/notification_content_hierarchy.py
--rw-r--r--   0        0        0     1139 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/notification_get_content_response.py
--rw-r--r--   0        0        0      989 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/notification_list_response.py
--rw-r--r--   0        0        0      908 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/submission_checks_get_response.py
--rw-r--r--   0        0        0      912 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/submission_checks_replace_response.py
--rw-r--r--   0        0        0     1877 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/__init__.py
--rw-r--r--   0        0        0    43043 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/client.py
--rw-r--r--   0        0        0     2897 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/__init__.py
--rw-r--r--   0        0        0      947 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/address.py
--rw-r--r--   0        0        0     1015 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/airship_profile.py
--rw-r--r--   0        0        0      867 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/airship_profile_audience.py
--rw-r--r--   0        0        0      893 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/delete_list_subscription_response.py
--rw-r--r--   0        0        0      104 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/device_type.py
--rw-r--r--   0        0        0      232 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/discord.py
--rw-r--r--   0        0        0      193 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/expo.py
--rw-r--r--   0        0        0     1348 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/get_list_subscriptions_list.py
--rw-r--r--   0        0        0     1092 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/get_list_subscriptions_response.py
--rw-r--r--   0        0        0     1036 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/intercom.py
--rw-r--r--   0        0        0      854 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/intercom_recipient.py
--rw-r--r--   0        0        0      883 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/merge_profile_response.py
--rw-r--r--   0        0        0      566 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/ms_teams.py
--rw-r--r--   0        0        0      886 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/ms_teams_base_properties.py
--rw-r--r--   0        0        0      895 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/multiple_tokens.py
--rw-r--r--   0        0        0      986 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/profile_get_parameters.py
--rw-r--r--   0        0        0     1019 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/profile_get_response.py
--rw-r--r--   0        0        0      885 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/replace_profile_response.py
--rw-r--r--   0        0        0      859 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/send_direct_message.py
--rw-r--r--   0        0        0      858 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/send_to_channel.py
--rw-r--r--   0        0        0     1005 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/send_to_ms_teams_channel_id.py
--rw-r--r--   0        0        0     1026 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/send_to_ms_teams_channel_name.py
--rw-r--r--   0        0        0     1015 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/send_to_ms_teams_conversation_id.py
--rw-r--r--   0        0        0      996 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/send_to_ms_teams_email.py
--rw-r--r--   0        0        0      999 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/send_to_ms_teams_user_id.py
--rw-r--r--   0        0        0      991 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/send_to_slack_channel.py
--rw-r--r--   0        0        0      987 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/send_to_slack_email.py
--rw-r--r--   0        0        0      990 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/send_to_slack_user_id.py
--rw-r--r--   0        0        0      316 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/slack.py
--rw-r--r--   0        0        0      866 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/slack_base_properties.py
--rw-r--r--   0        0        0      935 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/snooze_rule.py
--rw-r--r--   0        0        0      148 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/snooze_rule_type.py
--rw-r--r--   0        0        0      992 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/subscribe_to_lists_request.py
--rw-r--r--   0        0        0     1123 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/subscribe_to_lists_request_list_object.py
--rw-r--r--   0        0        0      887 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/subscribe_to_lists_response.py
--rw-r--r--   0        0        0      845 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/token.py
--rw-r--r--   0        0        0     2026 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/user_profile.py
--rw-r--r--   0        0        0        0 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/py.typed
--rw-r--r--   0        0        0     4101 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/__init__.py
--rw-r--r--   0        0        0     6149 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/__init__.py
--rw-r--r--   0        0        0      122 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/attachment.py
--rw-r--r--   0        0        0     1031 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/audience_filter.py
--rw-r--r--   0        0        0     1201 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/audience_recipient.py
--rw-r--r--   0        0        0     2961 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/base_message.py
--rw-r--r--   0        0        0     1039 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/base_message_send_to.py
--rw-r--r--   0        0        0      856 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/base_social_presence.py
--rw-r--r--   0        0        0     1366 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/brand_settings_email.py
--rw-r--r--   0        0        0     1637 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/brand_settings_in_app.py
--rw-r--r--   0        0        0     1367 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/brand_settings_social_presence.py
--rw-r--r--   0        0        0     1308 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/brand_template.py
--rw-r--r--   0        0        0     1201 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/brand_template_override.py
--rw-r--r--   0        0        0     2359 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/channel.py
--rw-r--r--   0        0        0      898 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/channel_metadata.py
--rw-r--r--   0        0        0      174 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/channel_source.py
--rw-r--r--   0        0        0      252 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/content.py
--rw-r--r--   0        0        0     1546 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/content_message.py
--rw-r--r--   0        0        0      183 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/criteria.py
--rw-r--r--   0        0        0      933 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/delay.py
--rw-r--r--   0        0        0     2131 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_action_node.py
--rw-r--r--   0        0        0     1126 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_base_node.py
--rw-r--r--   0        0        0     2524 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_channel_node.py
--rw-r--r--   0        0        0     1056 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_content.py
--rw-r--r--   0        0        0     1180 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_content_sugar.py
--rw-r--r--   0        0        0     1178 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_divider_node.py
--rw-r--r--   0        0        0     1449 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_group_node.py
--rw-r--r--   0        0        0     1689 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_image_node.py
--rw-r--r--   0        0        0     1384 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_meta_node.py
--rw-r--r--   0        0        0     8164 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_node.py
--rw-r--r--   0        0        0     1697 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_quote_node.py
--rw-r--r--   0        0        0     2459 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_text_node.py
--rw-r--r--   0        0        0     1063 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/email_footer.py
--rw-r--r--   0        0        0     1023 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/email_head.py
--rw-r--r--   0        0        0     1141 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/email_header.py
--rw-r--r--   0        0        0      119 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/expires_in_type.py
--rw-r--r--   0        0        0     1257 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/expiry.py
--rw-r--r--   0        0        0      160 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/i_action_button_style.py
--rw-r--r--   0        0        0      169 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/i_alignment.py
--rw-r--r--   0        0        0      160 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/i_preferences.py
--rw-r--r--   0        0        0     1139 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/i_profile_preferences.py
--rw-r--r--   0        0        0      909 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/icons.py
--rw-r--r--   0        0        0      172 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/in_app_placement.py
--rw-r--r--   0        0        0      886 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/invalid_list_pattern_recipient.py
--rw-r--r--   0        0        0      884 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/invalid_list_recipient.py
--rw-r--r--   0        0        0      884 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/invalid_user_recipient.py
--rw-r--r--   0        0        0     1027 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/list_filter.py
--rw-r--r--   0        0        0     1122 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/list_pattern_recipient.py
--rw-r--r--   0        0        0      848 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/list_pattern_recipient_type.py
--rw-r--r--   0        0        0     1185 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/list_recipient.py
--rw-r--r--   0        0        0      841 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/list_recipient_type.py
--rw-r--r--   0        0        0      848 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/locale.py
--rw-r--r--   0        0        0      160 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/locales.py
--rw-r--r--   0        0        0      906 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/logo.py
--rw-r--r--   0        0        0      227 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/message.py
--rw-r--r--   0        0        0     1502 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/message_channel_email_override.py
--rw-r--r--   0        0        0      154 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/message_channels.py
--rw-r--r--   0        0        0     1123 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/message_context.py
--rw-r--r--   0        0        0      123 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/message_data.py
--rw-r--r--   0        0        0     1723 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/message_metadata.py
--rw-r--r--   0        0        0      196 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/message_providers.py
--rw-r--r--   0        0        0     1477 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/message_providers_type.py
--rw-r--r--   0        0        0      181 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/message_recipient.py
--rw-r--r--   0        0        0      891 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/metadata.py
--rw-r--r--   0        0        0      910 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/ms_teams_recipient.py
--rw-r--r--   0        0        0      193 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/override.py
--rw-r--r--   0        0        0     1258 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/preference.py
--rw-r--r--   0        0        0      990 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/preferences.py
--rw-r--r--   0        0        0      583 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/recipient.py
--rw-r--r--   0        0        0      125 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/recipient_data.py
--rw-r--r--   0        0        0     1462 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/routing.py
--rw-r--r--   0        0        0      289 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/routing_channel.py
--rw-r--r--   0        0        0      154 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/routing_method.py
--rw-r--r--   0        0        0     1279 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/routing_strategy_channel.py
--rw-r--r--   0        0        0     1135 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/routing_strategy_provider.py
--rw-r--r--   0        0        0      175 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/rule_type.py
--rw-r--r--   0        0        0      898 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/slack_recipient.py
--rw-r--r--   0        0        0     1212 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/template_message.py
--rw-r--r--   0        0        0      160 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/text_align.py
--rw-r--r--   0        0        0      164 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/text_style.py
--rw-r--r--   0        0        0     1114 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/timeout.py
--rw-r--r--   0        0        0      916 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/timeouts.py
--rw-r--r--   0        0        0      856 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/tracking_override.py
--rw-r--r--   0        0        0     2035 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/user_recipient.py
--rw-r--r--   0        0        0      841 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/user_recipient_type.py
--rw-r--r--   0        0        0     1029 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/utm.py
--rw-r--r--   0        0        0     1101 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/widget_background.py
--rw-r--r--   0        0        0      411 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/templates/__init__.py
--rw-r--r--   0        0        0     5852 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/templates/client.py
--rw-r--r--   0        0        0      564 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/templates/types/__init__.py
--rw-r--r--   0        0        0       89 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/templates/types/channel_identifier.py
--rw-r--r--   0        0        0     1091 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/templates/types/list_templates_response.py
--rw-r--r--   0        0        0     1781 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/templates/types/notification_templates.py
--rw-r--r--   0        0        0     1351 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/templates/types/routing_strategy.py
--rw-r--r--   0        0        0      162 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/templates/types/routing_strategy_method.py
--rw-r--r--   0        0        0      889 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/templates/types/tag.py
--rw-r--r--   0        0        0      992 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/templates/types/tag_data.py
--rw-r--r--   0        0        0      449 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/tenants/__init__.py
--rw-r--r--   0        0        0    30865 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/tenants/client.py
--rw-r--r--   0        0        0      624 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/tenants/types/__init__.py
--rw-r--r--   0        0        0      959 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/tenants/types/default_preferences.py
--rw-r--r--   0        0        0     1737 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/tenants/types/list_users_for_tenant_response.py
--rw-r--r--   0        0        0     1005 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/tenants/types/subscription_topic.py
--rw-r--r--   0        0        0      184 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/tenants/types/subscription_topic_status.py
--rw-r--r--   0        0        0      110 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/tenants/types/template_property.py
--rw-r--r--   0        0        0     1904 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/tenants/types/tenant.py
--rw-r--r--   0        0        0     1698 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/tenants/types/tenant_list_response.py
--rw-r--r--   0        0        0       65 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/translations/__init__.py
--rw-r--r--   0        0        0    11268 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/translations/client.py
--rw-r--r--   0        0        0      155 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/types/__init__.py
--rw-r--r--   0        0        0     1592 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/types/send_message_response.py
--rw-r--r--   0        0        0     1354 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/__init__.py
--rw-r--r--   0        0        0     1067 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/client.py
--rw-r--r--   0        0        0      409 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/preferences/__init__.py
--rw-r--r--   0        0        0    18445 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/preferences/client.py
--rw-r--r--   0        0        0      561 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/preferences/types/__init__.py
--rw-r--r--   0        0        0     1345 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/preferences/types/topic_preference.py
--rw-r--r--   0        0        0     1276 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/preferences/types/topic_preference_update.py
--rw-r--r--   0        0        0      926 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/preferences/types/user_preferences_get_response.py
--rw-r--r--   0        0        0     1090 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/preferences/types/user_preferences_list_response.py
--rw-r--r--   0        0        0      873 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/preferences/types/user_preferences_update_response.py
--rw-r--r--   0        0        0      229 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tenants/__init__.py
--rw-r--r--   0        0        0    28780 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tenants/client.py
--rw-r--r--   0        0        0      308 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tenants/types/__init__.py
--rw-r--r--   0        0        0     1397 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tenants/types/add_user_to_single_tenants_params_profile.py
--rw-r--r--   0        0        0     1740 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tenants/types/list_tenants_for_user_response.py
--rw-r--r--   0        0        0      765 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/__init__.py
--rw-r--r--   0        0        0    29460 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/client.py
--rw-r--r--   0        0        0     1135 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/__init__.py
--rw-r--r--   0        0        0      878 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/delete_user_token_opts.py
--rw-r--r--   0        0        0     1576 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/device.py
--rw-r--r--   0        0        0      117 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/expiry_date.py
--rw-r--r--   0        0        0      161 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/get_all_tokens_response.py
--rw-r--r--   0        0        0      875 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/get_user_token_opts.py
--rw-r--r--   0        0        0     1160 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/get_user_token_response.py
--rw-r--r--   0        0        0      861 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/get_user_tokens_opts.py
--rw-r--r--   0        0        0      183 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/patch_op.py
--rw-r--r--   0        0        0     1158 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/patch_operation.py
--rw-r--r--   0        0        0      928 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/patch_user_token_opts.py
--rw-r--r--   0        0        0      179 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/provider_key.py
--rw-r--r--   0        0        0      915 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/put_user_token_opts.py
--rw-r--r--   0        0        0      930 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/put_user_tokens_opts.py
--rw-r--r--   0        0        0      177 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/token_status.py
--rw-r--r--   0        0        0     1387 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/tracking.py
--rw-r--r--   0        0        0     1790 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/user_token.py
--rw-r--r--   0        0        0       78 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/version.py
--rw-r--r--   0        0        0     6000 1970-01-01 00:00:00.000000 trycourier-6.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-03 19:18:39.362366 trycourier-6.0.4/LICENSE
+-rw-r--r--   0        0        0     5507 2024-05-03 19:18:39.362366 trycourier-6.0.4/README.md
+-rw-r--r--   0        0        0      595 2024-05-03 19:18:39.362366 trycourier-6.0.4/pyproject.toml
+-rw-r--r--   0        0        0    14108 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/__init__.py
+-rw-r--r--   0        0        0      751 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audiences/__init__.py
+-rw-r--r--   0        0        0    28202 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audiences/client.py
+-rw-r--r--   0        0        0     1100 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audiences/types/__init__.py
+-rw-r--r--   0        0        0     1199 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audiences/types/audience.py
+-rw-r--r--   0        0        0      971 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audiences/types/audience_list_response.py
+-rw-r--r--   0        0        0      939 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audiences/types/audience_member.py
+-rw-r--r--   0        0        0     1052 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audiences/types/audience_member_get_response.py
+-rw-r--r--   0        0        0      996 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audiences/types/audience_member_list_response.py
+-rw-r--r--   0        0        0      901 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audiences/types/audience_update_response.py
+-rw-r--r--   0        0        0      971 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audiences/types/base_filter_config.py
+-rw-r--r--   0        0        0      386 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audiences/types/comparison_operator.py
+-rw-r--r--   0        0        0      249 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audiences/types/filter.py
+-rw-r--r--   0        0        0      255 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audiences/types/filter_config.py
+-rw-r--r--   0        0        0      152 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audiences/types/logical_operator.py
+-rw-r--r--   0        0        0     1191 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audiences/types/nested_filter_config.py
+-rw-r--r--   0        0        0      240 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audiences/types/operator.py
+-rw-r--r--   0        0        0     1252 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audiences/types/single_filter_config.py
+-rw-r--r--   0        0        0      299 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audit_events/__init__.py
+-rw-r--r--   0        0        0    10417 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audit_events/client.py
+-rw-r--r--   0        0        0      453 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audit_events/types/__init__.py
+-rw-r--r--   0        0        0      905 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audit_events/types/actor.py
+-rw-r--r--   0        0        0     1164 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audit_events/types/audit_event.py
+-rw-r--r--   0        0        0      988 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audit_events/types/get_audit_event_params.py
+-rw-r--r--   0        0        0      886 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audit_events/types/list_audit_events_params.py
+-rw-r--r--   0        0        0      983 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audit_events/types/list_audit_events_response.py
+-rw-r--r--   0        0        0      906 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/audit_events/types/target.py
+-rw-r--r--   0        0        0      137 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/auth_tokens/__init__.py
+-rw-r--r--   0        0        0     7229 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/auth_tokens/client.py
+-rw-r--r--   0        0        0      152 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/auth_tokens/types/__init__.py
+-rw-r--r--   0        0        0      882 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/auth_tokens/types/issue_token_response.py
+-rw-r--r--   0        0        0     1847 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/__init__.py
+-rw-r--r--   0        0        0    16885 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/client.py
+-rw-r--r--   0        0        0     2836 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/__init__.py
+-rw-r--r--   0        0        0      962 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/accessor_type.py
+-rw-r--r--   0        0        0      988 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation.py
+-rw-r--r--   0        0        0     1054 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_ad_hoc_invoke_params.py
+-rw-r--r--   0        0        0      138 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_add_to_batch_max_items_type.py
+-rw-r--r--   0        0        0     1954 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_add_to_batch_retain.py
+-rw-r--r--   0        0        0      192 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_add_to_batch_retain_type.py
+-rw-r--r--   0        0        0      178 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_add_to_batch_scope.py
+-rw-r--r--   0        0        0     3128 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_add_to_batch_step.py
+-rw-r--r--   0        0        0     1355 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_add_to_digest_step.py
+-rw-r--r--   0        0        0     1048 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_cancel_step.py
+-rw-r--r--   0        0        0     1331 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_delay_step.py
+-rw-r--r--   0        0        0     1784 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_fetch_data_step.py
+-rw-r--r--   0        0        0     1186 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_fetch_data_webhook.py
+-rw-r--r--   0        0        0      171 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_fetch_data_webhook_method.py
+-rw-r--r--   0        0        0     1108 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_invoke_params.py
+-rw-r--r--   0        0        0      978 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_invoke_response.py
+-rw-r--r--   0        0        0     1015 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_invoke_step.py
+-rw-r--r--   0        0        0     1056 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_invoke_template_params.py
+-rw-r--r--   0        0        0     1088 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_run_context.py
+-rw-r--r--   0        0        0     1262 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_send_list_step.py
+-rw-r--r--   0        0        0     1295 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_send_step.py
+-rw-r--r--   0        0        0     1030 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_step.py
+-rw-r--r--   0        0        0     1102 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_step_option.py
+-rw-r--r--   0        0        0     1052 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_throttle_on_throttle.py
+-rw-r--r--   0        0        0      176 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_throttle_scope.py
+-rw-r--r--   0        0        0     2301 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_throttle_step.py
+-rw-r--r--   0        0        0     1039 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_update_profile_step.py
+-rw-r--r--   0        0        0     1058 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/automation_v_2_send_step.py
+-rw-r--r--   0        0        0      184 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/merge_algorithm.py
+-rw-r--r--   0        0        0      101 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/automations/types/profile.py
+-rw-r--r--   0        0        0      419 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/brands/__init__.py
+-rw-r--r--   0        0        0    29995 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/brands/client.py
+-rw-r--r--   0        0        0      579 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/brands/types/__init__.py
+-rw-r--r--   0        0        0     1716 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/brands/types/brand.py
+-rw-r--r--   0        0        0      962 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/brands/types/brand_colors.py
+-rw-r--r--   0        0        0      963 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/brands/types/brand_get_all_response.py
+-rw-r--r--   0        0        0     1120 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/brands/types/brand_parameters.py
+-rw-r--r--   0        0        0     1052 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/brands/types/brand_settings.py
+-rw-r--r--   0        0        0      907 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/brands/types/brand_snippet.py
+-rw-r--r--   0        0        0      915 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/brands/types/brand_snippets.py
+-rw-r--r--   0        0        0      958 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/brands/types/brands_response.py
+-rw-r--r--   0        0        0     1059 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/bulk/__init__.py
+-rw-r--r--   0        0        0    30912 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/bulk/client.py
+-rw-r--r--   0        0        0     1603 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/bulk/types/__init__.py
+-rw-r--r--   0        0        0      975 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/bulk/types/bulk_create_job_response.py
+-rw-r--r--   0        0        0      970 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/bulk/types/bulk_get_job_params.py
+-rw-r--r--   0        0        0      899 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/bulk/types/bulk_get_job_response.py
+-rw-r--r--   0        0        0     1015 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/bulk/types/bulk_get_job_users_params.py
+-rw-r--r--   0        0        0     1022 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/bulk/types/bulk_get_job_users_response.py
+-rw-r--r--   0        0        0      883 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/bulk/types/bulk_ingest_error.py
+-rw-r--r--   0        0        0      955 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/bulk/types/bulk_ingest_users_params.py
+-rw-r--r--   0        0        0      975 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/bulk/types/bulk_ingest_users_response.py
+-rw-r--r--   0        0        0      184 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/bulk/types/bulk_job_status.py
+-rw-r--r--   0        0        0      173 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/bulk/types/bulk_job_user_status.py
+-rw-r--r--   0        0        0     1161 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/bulk/types/bulk_message_user_response.py
+-rw-r--r--   0        0        0     1512 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/bulk/types/inbound_bulk_content_message.py
+-rw-r--r--   0        0        0     1096 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/bulk/types/inbound_bulk_message.py
+-rw-r--r--   0        0        0     1218 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/bulk/types/inbound_bulk_message_user.py
+-rw-r--r--   0        0        0     1672 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/bulk/types/inbound_bulk_message_v_1.py
+-rw-r--r--   0        0        0      310 2024-05-03 19:18:39.362366 trycourier-6.0.4/src/courier/bulk/types/inbound_bulk_message_v_2.py
+-rw-r--r--   0        0        0     1165 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/bulk/types/inbound_bulk_template_message.py
+-rw-r--r--   0        0        0     1046 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/bulk/types/job_details.py
+-rw-r--r--   0        0        0    17491 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/client.py
+-rw-r--r--   0        0        0     1127 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/__init__.py
+-rw-r--r--   0        0        0      527 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/errors/__init__.py
+-rw-r--r--   0        0        0      289 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/errors/already_exists_error.py
+-rw-r--r--   0        0        0      277 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/errors/bad_request_error.py
+-rw-r--r--   0        0        0      268 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/errors/conflict_error.py
+-rw-r--r--   0        0        0      298 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/errors/message_not_found_error.py
+-rw-r--r--   0        0        0      269 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/errors/not_found_error.py
+-rw-r--r--   0        0        0      297 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/errors/payment_required_error.py
+-rw-r--r--   0        0        0     1207 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/types/__init__.py
+-rw-r--r--   0        0        0      988 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/types/already_exists.py
+-rw-r--r--   0        0        0      985 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/types/bad_request.py
+-rw-r--r--   0        0        0      939 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/types/base_error.py
+-rw-r--r--   0        0        0      213 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/types/channel_classification.py
+-rw-r--r--   0        0        0      935 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/types/channel_preference.py
+-rw-r--r--   0        0        0      983 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/types/conflict.py
+-rw-r--r--   0        0        0      876 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/types/email.py
+-rw-r--r--   0        0        0      990 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/types/message_not_found.py
+-rw-r--r--   0        0        0      983 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/types/not_found.py
+-rw-r--r--   0        0        0     1137 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/types/notification_preference_details.py
+-rw-r--r--   0        0        0      230 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/types/notification_preferences.py
+-rw-r--r--   0        0        0      886 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/types/paging.py
+-rw-r--r--   0        0        0      988 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/types/payment_required.py
+-rw-r--r--   0        0        0      177 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/types/preference_status.py
+-rw-r--r--   0        0        0     1038 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/types/recipient_preferences.py
+-rw-r--r--   0        0        0      883 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/types/rule.py
+-rw-r--r--   0        0        0     1353 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/commons/types/user_tenant_association.py
+-rw-r--r--   0        0        0      853 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/core/api_error.py
+-rw-r--r--   0        0        0     2088 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/core/request_options.py
+-rw-r--r--   0        0        0      159 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/environment.py
+-rw-r--r--   0        0        0      413 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/lists/__init__.py
+-rw-r--r--   0        0        0    69860 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/lists/client.py
+-rw-r--r--   0        0        0      569 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/lists/types/__init__.py
+-rw-r--r--   0        0        0      937 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/lists/types/list.py
+-rw-r--r--   0        0        0      957 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/lists/types/list_get_all_response.py
+-rw-r--r--   0        0        0     1032 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/lists/types/list_get_subscriptions_response.py
+-rw-r--r--   0        0        0      986 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/lists/types/list_put_params.py
+-rw-r--r--   0        0        0     1166 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/lists/types/list_subscription_recipient.py
+-rw-r--r--   0        0        0     1125 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/lists/types/put_subscriptions_recipient.py
+-rw-r--r--   0        0        0      527 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/messages/__init__.py
+-rw-r--r--   0        0        0    41212 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/messages/client.py
+-rw-r--r--   0        0        0      747 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/messages/types/__init__.py
+-rw-r--r--   0        0        0     1157 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/messages/types/list_messages_response.py
+-rw-r--r--   0        0        0     2811 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/messages/types/message_details.py
+-rw-r--r--   0        0        0      932 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/messages/types/message_history_response.py
+-rw-r--r--   0        0        0      357 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/messages/types/message_status.py
+-rw-r--r--   0        0        0      233 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/messages/types/reason.py
+-rw-r--r--   0        0        0     1234 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/messages/types/render_output.py
+-rw-r--r--   0        0        0     1022 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/messages/types/render_output_response.py
+-rw-r--r--   0        0        0     1050 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/messages/types/rendered_message_block.py
+-rw-r--r--   0        0        0     1499 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/messages/types/rendered_message_content.py
+-rw-r--r--   0        0        0      985 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/notifications/__init__.py
+-rw-r--r--   0        0        0    45003 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/notifications/client.py
+-rw-r--r--   0        0        0     1463 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/notifications/types/__init__.py
+-rw-r--r--   0        0        0      943 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/notifications/types/base_check.py
+-rw-r--r--   0        0        0      229 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/notifications/types/block_type.py
+-rw-r--r--   0        0        0      947 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/notifications/types/check.py
+-rw-r--r--   0        0        0      168 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/notifications/types/check_status.py
+-rw-r--r--   0        0        0     1127 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/notifications/types/message_routing.py
+-rw-r--r--   0        0        0      183 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/notifications/types/message_routing_channel.py
+-rw-r--r--   0        0        0      161 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/notifications/types/message_routing_method.py
+-rw-r--r--   0        0        0      941 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/notifications/types/notification.py
+-rw-r--r--   0        0        0     1216 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/notifications/types/notification_block.py
+-rw-r--r--   0        0        0     1151 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/notifications/types/notification_channel.py
+-rw-r--r--   0        0        0      931 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/notifications/types/notification_channel_content.py
+-rw-r--r--   0        0        0      224 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/notifications/types/notification_content.py
+-rw-r--r--   0        0        0      935 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/notifications/types/notification_content_hierarchy.py
+-rw-r--r--   0        0        0     1139 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/notifications/types/notification_get_content_response.py
+-rw-r--r--   0        0        0      989 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/notifications/types/notification_list_response.py
+-rw-r--r--   0        0        0      908 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/notifications/types/submission_checks_get_response.py
+-rw-r--r--   0        0        0      912 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/notifications/types/submission_checks_replace_response.py
+-rw-r--r--   0        0        0     1877 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/__init__.py
+-rw-r--r--   0        0        0    43043 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/client.py
+-rw-r--r--   0        0        0     2897 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/__init__.py
+-rw-r--r--   0        0        0      947 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/address.py
+-rw-r--r--   0        0        0     1015 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/airship_profile.py
+-rw-r--r--   0        0        0      867 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/airship_profile_audience.py
+-rw-r--r--   0        0        0      893 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/delete_list_subscription_response.py
+-rw-r--r--   0        0        0      104 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/device_type.py
+-rw-r--r--   0        0        0      232 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/discord.py
+-rw-r--r--   0        0        0      193 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/expo.py
+-rw-r--r--   0        0        0     1348 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/get_list_subscriptions_list.py
+-rw-r--r--   0        0        0     1092 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/get_list_subscriptions_response.py
+-rw-r--r--   0        0        0     1036 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/intercom.py
+-rw-r--r--   0        0        0      854 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/intercom_recipient.py
+-rw-r--r--   0        0        0      883 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/merge_profile_response.py
+-rw-r--r--   0        0        0      566 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/ms_teams.py
+-rw-r--r--   0        0        0      886 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/ms_teams_base_properties.py
+-rw-r--r--   0        0        0      895 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/multiple_tokens.py
+-rw-r--r--   0        0        0      986 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/profile_get_parameters.py
+-rw-r--r--   0        0        0     1019 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/profile_get_response.py
+-rw-r--r--   0        0        0      885 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/replace_profile_response.py
+-rw-r--r--   0        0        0      859 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/send_direct_message.py
+-rw-r--r--   0        0        0      858 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/send_to_channel.py
+-rw-r--r--   0        0        0     1005 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/send_to_ms_teams_channel_id.py
+-rw-r--r--   0        0        0     1026 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/send_to_ms_teams_channel_name.py
+-rw-r--r--   0        0        0     1015 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/send_to_ms_teams_conversation_id.py
+-rw-r--r--   0        0        0      996 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/send_to_ms_teams_email.py
+-rw-r--r--   0        0        0      999 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/send_to_ms_teams_user_id.py
+-rw-r--r--   0        0        0      991 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/send_to_slack_channel.py
+-rw-r--r--   0        0        0      987 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/send_to_slack_email.py
+-rw-r--r--   0        0        0      990 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/send_to_slack_user_id.py
+-rw-r--r--   0        0        0      316 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/slack.py
+-rw-r--r--   0        0        0      866 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/slack_base_properties.py
+-rw-r--r--   0        0        0      935 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/snooze_rule.py
+-rw-r--r--   0        0        0      148 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/snooze_rule_type.py
+-rw-r--r--   0        0        0      992 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/subscribe_to_lists_request.py
+-rw-r--r--   0        0        0     1123 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/subscribe_to_lists_request_list_object.py
+-rw-r--r--   0        0        0      887 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/subscribe_to_lists_response.py
+-rw-r--r--   0        0        0      845 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/token.py
+-rw-r--r--   0        0        0     2026 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/profiles/types/user_profile.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/py.typed
+-rw-r--r--   0        0        0     4101 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/__init__.py
+-rw-r--r--   0        0        0     6149 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/__init__.py
+-rw-r--r--   0        0        0      122 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/attachment.py
+-rw-r--r--   0        0        0     1031 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/audience_filter.py
+-rw-r--r--   0        0        0     1201 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/audience_recipient.py
+-rw-r--r--   0        0        0     2961 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/base_message.py
+-rw-r--r--   0        0        0     1039 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/base_message_send_to.py
+-rw-r--r--   0        0        0      856 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/base_social_presence.py
+-rw-r--r--   0        0        0     1366 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/brand_settings_email.py
+-rw-r--r--   0        0        0     1637 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/brand_settings_in_app.py
+-rw-r--r--   0        0        0     1367 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/brand_settings_social_presence.py
+-rw-r--r--   0        0        0     1308 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/brand_template.py
+-rw-r--r--   0        0        0     1201 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/brand_template_override.py
+-rw-r--r--   0        0        0     2359 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/channel.py
+-rw-r--r--   0        0        0      898 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/channel_metadata.py
+-rw-r--r--   0        0        0      174 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/channel_source.py
+-rw-r--r--   0        0        0      252 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/content.py
+-rw-r--r--   0        0        0     1546 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/content_message.py
+-rw-r--r--   0        0        0      183 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/criteria.py
+-rw-r--r--   0        0        0      933 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/delay.py
+-rw-r--r--   0        0        0     2131 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/elemental_action_node.py
+-rw-r--r--   0        0        0     1126 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/elemental_base_node.py
+-rw-r--r--   0        0        0     2524 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/elemental_channel_node.py
+-rw-r--r--   0        0        0     1056 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/elemental_content.py
+-rw-r--r--   0        0        0     1180 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/elemental_content_sugar.py
+-rw-r--r--   0        0        0     1178 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/elemental_divider_node.py
+-rw-r--r--   0        0        0     1449 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/elemental_group_node.py
+-rw-r--r--   0        0        0     1689 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/elemental_image_node.py
+-rw-r--r--   0        0        0     1384 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/elemental_meta_node.py
+-rw-r--r--   0        0        0     8164 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/elemental_node.py
+-rw-r--r--   0        0        0     1697 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/elemental_quote_node.py
+-rw-r--r--   0        0        0     2459 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/elemental_text_node.py
+-rw-r--r--   0        0        0     1063 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/email_footer.py
+-rw-r--r--   0        0        0     1023 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/email_head.py
+-rw-r--r--   0        0        0     1141 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/email_header.py
+-rw-r--r--   0        0        0      119 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/expires_in_type.py
+-rw-r--r--   0        0        0     1257 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/expiry.py
+-rw-r--r--   0        0        0      160 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/i_action_button_style.py
+-rw-r--r--   0        0        0      169 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/i_alignment.py
+-rw-r--r--   0        0        0      160 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/i_preferences.py
+-rw-r--r--   0        0        0     1139 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/i_profile_preferences.py
+-rw-r--r--   0        0        0      909 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/icons.py
+-rw-r--r--   0        0        0      172 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/in_app_placement.py
+-rw-r--r--   0        0        0      886 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/invalid_list_pattern_recipient.py
+-rw-r--r--   0        0        0      884 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/invalid_list_recipient.py
+-rw-r--r--   0        0        0      884 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/invalid_user_recipient.py
+-rw-r--r--   0        0        0     1027 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/list_filter.py
+-rw-r--r--   0        0        0     1122 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/list_pattern_recipient.py
+-rw-r--r--   0        0        0      848 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/list_pattern_recipient_type.py
+-rw-r--r--   0        0        0     1185 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/list_recipient.py
+-rw-r--r--   0        0        0      841 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/list_recipient_type.py
+-rw-r--r--   0        0        0      848 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/locale.py
+-rw-r--r--   0        0        0      160 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/locales.py
+-rw-r--r--   0        0        0      906 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/logo.py
+-rw-r--r--   0        0        0      227 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/message.py
+-rw-r--r--   0        0        0     1502 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/message_channel_email_override.py
+-rw-r--r--   0        0        0      154 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/message_channels.py
+-rw-r--r--   0        0        0     1123 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/message_context.py
+-rw-r--r--   0        0        0      123 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/message_data.py
+-rw-r--r--   0        0        0     1723 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/message_metadata.py
+-rw-r--r--   0        0        0      196 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/message_providers.py
+-rw-r--r--   0        0        0     1477 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/message_providers_type.py
+-rw-r--r--   0        0        0      181 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/message_recipient.py
+-rw-r--r--   0        0        0      891 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/metadata.py
+-rw-r--r--   0        0        0      910 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/ms_teams_recipient.py
+-rw-r--r--   0        0        0      193 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/override.py
+-rw-r--r--   0        0        0     1258 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/preference.py
+-rw-r--r--   0        0        0      990 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/preferences.py
+-rw-r--r--   0        0        0      583 2024-05-03 19:18:39.366366 trycourier-6.0.4/src/courier/send/types/recipient.py
+-rw-r--r--   0        0        0      125 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/send/types/recipient_data.py
+-rw-r--r--   0        0        0     1462 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/send/types/routing.py
+-rw-r--r--   0        0        0      289 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/send/types/routing_channel.py
+-rw-r--r--   0        0        0      154 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/send/types/routing_method.py
+-rw-r--r--   0        0        0     1279 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/send/types/routing_strategy_channel.py
+-rw-r--r--   0        0        0     1135 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/send/types/routing_strategy_provider.py
+-rw-r--r--   0        0        0      175 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/send/types/rule_type.py
+-rw-r--r--   0        0        0      898 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/send/types/slack_recipient.py
+-rw-r--r--   0        0        0     1212 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/send/types/template_message.py
+-rw-r--r--   0        0        0      160 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/send/types/text_align.py
+-rw-r--r--   0        0        0      164 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/send/types/text_style.py
+-rw-r--r--   0        0        0     1114 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/send/types/timeout.py
+-rw-r--r--   0        0        0      916 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/send/types/timeouts.py
+-rw-r--r--   0        0        0      856 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/send/types/tracking_override.py
+-rw-r--r--   0        0        0     2035 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/send/types/user_recipient.py
+-rw-r--r--   0        0        0      841 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/send/types/user_recipient_type.py
+-rw-r--r--   0        0        0     1029 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/send/types/utm.py
+-rw-r--r--   0        0        0     1101 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/send/types/widget_background.py
+-rw-r--r--   0        0        0      411 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/templates/__init__.py
+-rw-r--r--   0        0        0     5852 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/templates/client.py
+-rw-r--r--   0        0        0      564 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/templates/types/__init__.py
+-rw-r--r--   0        0        0       89 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/templates/types/channel_identifier.py
+-rw-r--r--   0        0        0     1091 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/templates/types/list_templates_response.py
+-rw-r--r--   0        0        0     1781 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/templates/types/notification_templates.py
+-rw-r--r--   0        0        0     1351 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/templates/types/routing_strategy.py
+-rw-r--r--   0        0        0      162 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/templates/types/routing_strategy_method.py
+-rw-r--r--   0        0        0      889 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/templates/types/tag.py
+-rw-r--r--   0        0        0      992 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/templates/types/tag_data.py
+-rw-r--r--   0        0        0      449 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/tenants/__init__.py
+-rw-r--r--   0        0        0    30811 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/tenants/client.py
+-rw-r--r--   0        0        0      624 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/tenants/types/__init__.py
+-rw-r--r--   0        0        0      959 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/tenants/types/default_preferences.py
+-rw-r--r--   0        0        0     1737 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/tenants/types/list_users_for_tenant_response.py
+-rw-r--r--   0        0        0     1005 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/tenants/types/subscription_topic.py
+-rw-r--r--   0        0        0      184 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/tenants/types/subscription_topic_status.py
+-rw-r--r--   0        0        0      110 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/tenants/types/template_property.py
+-rw-r--r--   0        0        0     1868 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/tenants/types/tenant.py
+-rw-r--r--   0        0        0     1698 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/tenants/types/tenant_list_response.py
+-rw-r--r--   0        0        0       65 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/translations/__init__.py
+-rw-r--r--   0        0        0    11268 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/translations/client.py
+-rw-r--r--   0        0        0      155 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/types/__init__.py
+-rw-r--r--   0        0        0     1592 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/types/send_message_response.py
+-rw-r--r--   0        0        0     1354 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/__init__.py
+-rw-r--r--   0        0        0     1067 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/client.py
+-rw-r--r--   0        0        0      409 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/preferences/__init__.py
+-rw-r--r--   0        0        0    18445 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/preferences/client.py
+-rw-r--r--   0        0        0      561 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/preferences/types/__init__.py
+-rw-r--r--   0        0        0     1345 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/preferences/types/topic_preference.py
+-rw-r--r--   0        0        0     1276 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/preferences/types/topic_preference_update.py
+-rw-r--r--   0        0        0      926 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/preferences/types/user_preferences_get_response.py
+-rw-r--r--   0        0        0     1090 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/preferences/types/user_preferences_list_response.py
+-rw-r--r--   0        0        0      873 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/preferences/types/user_preferences_update_response.py
+-rw-r--r--   0        0        0      229 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tenants/__init__.py
+-rw-r--r--   0        0        0    28780 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tenants/client.py
+-rw-r--r--   0        0        0      308 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tenants/types/__init__.py
+-rw-r--r--   0        0        0     1397 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tenants/types/add_user_to_single_tenants_params_profile.py
+-rw-r--r--   0        0        0     1740 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tenants/types/list_tenants_for_user_response.py
+-rw-r--r--   0        0        0      765 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tokens/__init__.py
+-rw-r--r--   0        0        0    29460 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tokens/client.py
+-rw-r--r--   0        0        0     1135 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tokens/types/__init__.py
+-rw-r--r--   0        0        0      878 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tokens/types/delete_user_token_opts.py
+-rw-r--r--   0        0        0     1576 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tokens/types/device.py
+-rw-r--r--   0        0        0      117 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tokens/types/expiry_date.py
+-rw-r--r--   0        0        0      161 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tokens/types/get_all_tokens_response.py
+-rw-r--r--   0        0        0      875 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tokens/types/get_user_token_opts.py
+-rw-r--r--   0        0        0     1160 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tokens/types/get_user_token_response.py
+-rw-r--r--   0        0        0      861 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tokens/types/get_user_tokens_opts.py
+-rw-r--r--   0        0        0      183 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tokens/types/patch_op.py
+-rw-r--r--   0        0        0     1158 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tokens/types/patch_operation.py
+-rw-r--r--   0        0        0      928 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tokens/types/patch_user_token_opts.py
+-rw-r--r--   0        0        0      179 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tokens/types/provider_key.py
+-rw-r--r--   0        0        0      915 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tokens/types/put_user_token_opts.py
+-rw-r--r--   0        0        0      930 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tokens/types/put_user_tokens_opts.py
+-rw-r--r--   0        0        0      177 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tokens/types/token_status.py
+-rw-r--r--   0        0        0     1387 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tokens/types/tracking.py
+-rw-r--r--   0        0        0     1790 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/users/tokens/types/user_token.py
+-rw-r--r--   0        0        0       78 2024-05-03 19:18:39.370366 trycourier-6.0.4/src/courier/version.py
+-rw-r--r--   0        0        0     6000 1970-01-01 00:00:00.000000 trycourier-6.0.4/PKG-INFO
```

### Comparing `trycourier-6.0.3/LICENSE` & `trycourier-6.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/README.md` & `trycourier-6.0.4/README.md`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/pyproject.toml` & `trycourier-6.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trycourier"
-version = "v6.0.3"
+version = "v6.0.4"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "courier", from = "src"}
 ]
```

### Comparing `trycourier-6.0.3/src/courier/__init__.py` & `trycourier-6.0.4/src/courier/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/audiences/__init__.py` & `trycourier-6.0.4/src/courier/audiences/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/audiences/client.py` & `trycourier-6.0.4/src/courier/audiences/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/audiences/types/__init__.py` & `trycourier-6.0.4/src/courier/audiences/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/audiences/types/audience.py` & `trycourier-6.0.4/src/courier/audiences/types/audience.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/audiences/types/audience_list_response.py` & `trycourier-6.0.4/src/courier/audiences/types/audience_list_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/audiences/types/audience_member.py` & `trycourier-6.0.4/src/courier/audiences/types/audience_member.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/audiences/types/audience_member_get_response.py` & `trycourier-6.0.4/src/courier/audiences/types/audience_member_get_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/audiences/types/audience_member_list_response.py` & `trycourier-6.0.4/src/courier/audiences/types/audience_member_list_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/audiences/types/audience_update_response.py` & `trycourier-6.0.4/src/courier/audiences/types/audience_update_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/audiences/types/base_filter_config.py` & `trycourier-6.0.4/src/courier/audiences/types/base_filter_config.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/audiences/types/nested_filter_config.py` & `trycourier-6.0.4/src/courier/audiences/types/nested_filter_config.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/audiences/types/single_filter_config.py` & `trycourier-6.0.4/src/courier/audiences/types/single_filter_config.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/audit_events/client.py` & `trycourier-6.0.4/src/courier/audit_events/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/audit_events/types/actor.py` & `trycourier-6.0.4/src/courier/audit_events/types/actor.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/audit_events/types/audit_event.py` & `trycourier-6.0.4/src/courier/audit_events/types/audit_event.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/audit_events/types/get_audit_event_params.py` & `trycourier-6.0.4/src/courier/audit_events/types/get_audit_event_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/audit_events/types/list_audit_events_params.py` & `trycourier-6.0.4/src/courier/audit_events/types/list_audit_events_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/audit_events/types/list_audit_events_response.py` & `trycourier-6.0.4/src/courier/audit_events/types/list_audit_events_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/audit_events/types/target.py` & `trycourier-6.0.4/src/courier/audit_events/types/target.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/auth_tokens/client.py` & `trycourier-6.0.4/src/courier/auth_tokens/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/auth_tokens/types/issue_token_response.py` & `trycourier-6.0.4/src/courier/auth_tokens/types/issue_token_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/__init__.py` & `trycourier-6.0.4/src/courier/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/client.py` & `trycourier-6.0.4/src/courier/automations/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/__init__.py` & `trycourier-6.0.4/src/courier/automations/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/accessor_type.py` & `trycourier-6.0.4/src/courier/automations/types/accessor_type.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation.py` & `trycourier-6.0.4/src/courier/automations/types/automation.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_ad_hoc_invoke_params.py` & `trycourier-6.0.4/src/courier/automations/types/automation_ad_hoc_invoke_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_add_to_batch_retain.py` & `trycourier-6.0.4/src/courier/automations/types/automation_add_to_batch_retain.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_add_to_batch_step.py` & `trycourier-6.0.4/src/courier/automations/types/automation_add_to_batch_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_add_to_digest_step.py` & `trycourier-6.0.4/src/courier/automations/types/automation_add_to_digest_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_cancel_step.py` & `trycourier-6.0.4/src/courier/automations/types/automation_cancel_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_delay_step.py` & `trycourier-6.0.4/src/courier/automations/types/automation_delay_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_fetch_data_step.py` & `trycourier-6.0.4/src/courier/automations/types/automation_fetch_data_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_fetch_data_webhook.py` & `trycourier-6.0.4/src/courier/automations/types/automation_fetch_data_webhook.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_invoke_params.py` & `trycourier-6.0.4/src/courier/automations/types/automation_invoke_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_invoke_response.py` & `trycourier-6.0.4/src/courier/automations/types/automation_invoke_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_invoke_step.py` & `trycourier-6.0.4/src/courier/automations/types/automation_invoke_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_invoke_template_params.py` & `trycourier-6.0.4/src/courier/automations/types/automation_invoke_template_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_run_context.py` & `trycourier-6.0.4/src/courier/automations/types/automation_run_context.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_send_list_step.py` & `trycourier-6.0.4/src/courier/automations/types/automation_send_list_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_send_step.py` & `trycourier-6.0.4/src/courier/automations/types/automation_send_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_step.py` & `trycourier-6.0.4/src/courier/automations/types/automation_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_step_option.py` & `trycourier-6.0.4/src/courier/automations/types/automation_step_option.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_throttle_on_throttle.py` & `trycourier-6.0.4/src/courier/automations/types/automation_throttle_on_throttle.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_throttle_step.py` & `trycourier-6.0.4/src/courier/automations/types/automation_throttle_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_update_profile_step.py` & `trycourier-6.0.4/src/courier/automations/types/automation_update_profile_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/automations/types/automation_v_2_send_step.py` & `trycourier-6.0.4/src/courier/automations/types/automation_v_2_send_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/brands/client.py` & `trycourier-6.0.4/src/courier/brands/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/brands/types/__init__.py` & `trycourier-6.0.4/src/courier/brands/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/brands/types/brand.py` & `trycourier-6.0.4/src/courier/brands/types/brand.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/brands/types/brand_colors.py` & `trycourier-6.0.4/src/courier/brands/types/brand_colors.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/brands/types/brand_get_all_response.py` & `trycourier-6.0.4/src/courier/brands/types/brand_get_all_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/brands/types/brand_parameters.py` & `trycourier-6.0.4/src/courier/brands/types/brand_parameters.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/brands/types/brand_settings.py` & `trycourier-6.0.4/src/courier/brands/types/brand_settings.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/brands/types/brand_snippet.py` & `trycourier-6.0.4/src/courier/brands/types/brand_snippet.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/brands/types/brand_snippets.py` & `trycourier-6.0.4/src/courier/brands/types/brand_snippets.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/brands/types/brands_response.py` & `trycourier-6.0.4/src/courier/brands/types/brands_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/bulk/__init__.py` & `trycourier-6.0.4/src/courier/bulk/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/bulk/client.py` & `trycourier-6.0.4/src/courier/bulk/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/bulk/types/__init__.py` & `trycourier-6.0.4/src/courier/bulk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/bulk/types/bulk_create_job_response.py` & `trycourier-6.0.4/src/courier/bulk/types/bulk_create_job_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/bulk/types/bulk_get_job_params.py` & `trycourier-6.0.4/src/courier/bulk/types/bulk_get_job_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/bulk/types/bulk_get_job_response.py` & `trycourier-6.0.4/src/courier/bulk/types/bulk_get_job_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/bulk/types/bulk_get_job_users_params.py` & `trycourier-6.0.4/src/courier/bulk/types/bulk_get_job_users_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/bulk/types/bulk_get_job_users_response.py` & `trycourier-6.0.4/src/courier/bulk/types/bulk_get_job_users_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/bulk/types/bulk_ingest_error.py` & `trycourier-6.0.4/src/courier/bulk/types/bulk_ingest_error.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/bulk/types/bulk_ingest_users_params.py` & `trycourier-6.0.4/src/courier/bulk/types/bulk_ingest_users_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/bulk/types/bulk_ingest_users_response.py` & `trycourier-6.0.4/src/courier/bulk/types/bulk_ingest_users_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/bulk/types/bulk_message_user_response.py` & `trycourier-6.0.4/src/courier/bulk/types/bulk_message_user_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_content_message.py` & `trycourier-6.0.4/src/courier/bulk/types/inbound_bulk_content_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_message.py` & `trycourier-6.0.4/src/courier/bulk/types/inbound_bulk_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_message_user.py` & `trycourier-6.0.4/src/courier/bulk/types/inbound_bulk_message_user.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_message_v_1.py` & `trycourier-6.0.4/src/courier/bulk/types/inbound_bulk_message_v_1.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_template_message.py` & `trycourier-6.0.4/src/courier/bulk/types/inbound_bulk_template_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/bulk/types/job_details.py` & `trycourier-6.0.4/src/courier/bulk/types/job_details.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/client.py` & `trycourier-6.0.4/src/courier/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/commons/__init__.py` & `trycourier-6.0.4/src/courier/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/commons/errors/__init__.py` & `trycourier-6.0.4/src/courier/commons/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/commons/types/__init__.py` & `trycourier-6.0.4/src/courier/commons/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/commons/types/already_exists.py` & `trycourier-6.0.4/src/courier/commons/types/already_exists.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/commons/types/bad_request.py` & `trycourier-6.0.4/src/courier/commons/types/bad_request.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/commons/types/base_error.py` & `trycourier-6.0.4/src/courier/commons/types/base_error.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/commons/types/channel_preference.py` & `trycourier-6.0.4/src/courier/commons/types/channel_preference.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/commons/types/conflict.py` & `trycourier-6.0.4/src/courier/commons/types/conflict.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/commons/types/email.py` & `trycourier-6.0.4/src/courier/commons/types/email.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/commons/types/message_not_found.py` & `trycourier-6.0.4/src/courier/commons/types/message_not_found.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/commons/types/not_found.py` & `trycourier-6.0.4/src/courier/commons/types/not_found.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/commons/types/notification_preference_details.py` & `trycourier-6.0.4/src/courier/commons/types/notification_preference_details.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/commons/types/paging.py` & `trycourier-6.0.4/src/courier/commons/types/paging.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/commons/types/payment_required.py` & `trycourier-6.0.4/src/courier/commons/types/payment_required.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/commons/types/recipient_preferences.py` & `trycourier-6.0.4/src/courier/commons/types/recipient_preferences.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/commons/types/rule.py` & `trycourier-6.0.4/src/courier/commons/types/rule.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/commons/types/user_tenant_association.py` & `trycourier-6.0.4/src/courier/commons/types/user_tenant_association.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/core/__init__.py` & `trycourier-6.0.4/src/courier/core/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/core/client_wrapper.py` & `trycourier-6.0.4/src/courier/core/client_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "trycourier",
-            "X-Fern-SDK-Version": "v6.0.3",
+            "X-Fern-SDK-Version": "v6.0.4",
         }
         headers["Authorization"] = f"Bearer {self._get_authorization_token()}"
         return headers
 
     def _get_authorization_token(self) -> str:
         if isinstance(self._authorization_token, str):
             return self._authorization_token
```

### Comparing `trycourier-6.0.3/src/courier/core/datetime_utils.py` & `trycourier-6.0.4/src/courier/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/core/file.py` & `trycourier-6.0.4/src/courier/core/file.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/core/http_client.py` & `trycourier-6.0.4/src/courier/core/http_client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/core/jsonable_encoder.py` & `trycourier-6.0.4/src/courier/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/core/request_options.py` & `trycourier-6.0.4/src/courier/core/request_options.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/lists/client.py` & `trycourier-6.0.4/src/courier/lists/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/lists/types/__init__.py` & `trycourier-6.0.4/src/courier/lists/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/lists/types/list.py` & `trycourier-6.0.4/src/courier/lists/types/list.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/lists/types/list_get_all_response.py` & `trycourier-6.0.4/src/courier/lists/types/list_get_all_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/lists/types/list_get_subscriptions_response.py` & `trycourier-6.0.4/src/courier/lists/types/list_get_subscriptions_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/lists/types/list_put_params.py` & `trycourier-6.0.4/src/courier/lists/types/list_put_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/lists/types/list_subscription_recipient.py` & `trycourier-6.0.4/src/courier/lists/types/list_subscription_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/lists/types/put_subscriptions_recipient.py` & `trycourier-6.0.4/src/courier/lists/types/put_subscriptions_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/messages/__init__.py` & `trycourier-6.0.4/src/courier/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/messages/client.py` & `trycourier-6.0.4/src/courier/messages/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/messages/types/__init__.py` & `trycourier-6.0.4/src/courier/messages/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/messages/types/list_messages_response.py` & `trycourier-6.0.4/src/courier/messages/types/list_messages_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/messages/types/message_details.py` & `trycourier-6.0.4/src/courier/messages/types/message_details.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/messages/types/message_history_response.py` & `trycourier-6.0.4/src/courier/messages/types/message_history_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/messages/types/render_output.py` & `trycourier-6.0.4/src/courier/messages/types/render_output.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/messages/types/render_output_response.py` & `trycourier-6.0.4/src/courier/messages/types/render_output_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/messages/types/rendered_message_block.py` & `trycourier-6.0.4/src/courier/messages/types/rendered_message_block.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/messages/types/rendered_message_content.py` & `trycourier-6.0.4/src/courier/messages/types/rendered_message_content.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/notifications/__init__.py` & `trycourier-6.0.4/src/courier/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/notifications/client.py` & `trycourier-6.0.4/src/courier/notifications/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/notifications/types/__init__.py` & `trycourier-6.0.4/src/courier/notifications/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/notifications/types/base_check.py` & `trycourier-6.0.4/src/courier/notifications/types/base_check.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/notifications/types/check.py` & `trycourier-6.0.4/src/courier/notifications/types/check.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/notifications/types/message_routing.py` & `trycourier-6.0.4/src/courier/notifications/types/message_routing.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/notifications/types/notification.py` & `trycourier-6.0.4/src/courier/notifications/types/notification.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/notifications/types/notification_block.py` & `trycourier-6.0.4/src/courier/notifications/types/notification_block.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/notifications/types/notification_channel.py` & `trycourier-6.0.4/src/courier/notifications/types/notification_channel.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/notifications/types/notification_channel_content.py` & `trycourier-6.0.4/src/courier/notifications/types/notification_channel_content.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/notifications/types/notification_content_hierarchy.py` & `trycourier-6.0.4/src/courier/notifications/types/notification_content_hierarchy.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/notifications/types/notification_get_content_response.py` & `trycourier-6.0.4/src/courier/notifications/types/notification_get_content_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/notifications/types/notification_list_response.py` & `trycourier-6.0.4/src/courier/notifications/types/notification_list_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/notifications/types/submission_checks_get_response.py` & `trycourier-6.0.4/src/courier/notifications/types/submission_checks_get_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/notifications/types/submission_checks_replace_response.py` & `trycourier-6.0.4/src/courier/notifications/types/submission_checks_replace_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/__init__.py` & `trycourier-6.0.4/src/courier/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/client.py` & `trycourier-6.0.4/src/courier/profiles/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/__init__.py` & `trycourier-6.0.4/src/courier/profiles/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/address.py` & `trycourier-6.0.4/src/courier/profiles/types/address.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/airship_profile.py` & `trycourier-6.0.4/src/courier/profiles/types/airship_profile.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/airship_profile_audience.py` & `trycourier-6.0.4/src/courier/profiles/types/airship_profile_audience.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/delete_list_subscription_response.py` & `trycourier-6.0.4/src/courier/profiles/types/delete_list_subscription_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/get_list_subscriptions_list.py` & `trycourier-6.0.4/src/courier/profiles/types/get_list_subscriptions_list.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/get_list_subscriptions_response.py` & `trycourier-6.0.4/src/courier/profiles/types/get_list_subscriptions_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/intercom.py` & `trycourier-6.0.4/src/courier/profiles/types/intercom.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/intercom_recipient.py` & `trycourier-6.0.4/src/courier/profiles/types/intercom_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/merge_profile_response.py` & `trycourier-6.0.4/src/courier/profiles/types/merge_profile_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/ms_teams.py` & `trycourier-6.0.4/src/courier/profiles/types/ms_teams.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/ms_teams_base_properties.py` & `trycourier-6.0.4/src/courier/profiles/types/ms_teams_base_properties.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/multiple_tokens.py` & `trycourier-6.0.4/src/courier/profiles/types/multiple_tokens.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/profile_get_parameters.py` & `trycourier-6.0.4/src/courier/profiles/types/profile_get_parameters.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/profile_get_response.py` & `trycourier-6.0.4/src/courier/profiles/types/profile_get_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/replace_profile_response.py` & `trycourier-6.0.4/src/courier/profiles/types/replace_profile_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/send_direct_message.py` & `trycourier-6.0.4/src/courier/profiles/types/send_direct_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/send_to_channel.py` & `trycourier-6.0.4/src/courier/profiles/types/send_to_channel.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/send_to_ms_teams_channel_id.py` & `trycourier-6.0.4/src/courier/profiles/types/send_to_ms_teams_channel_id.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/send_to_ms_teams_channel_name.py` & `trycourier-6.0.4/src/courier/profiles/types/send_to_ms_teams_channel_name.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/send_to_ms_teams_conversation_id.py` & `trycourier-6.0.4/src/courier/profiles/types/send_to_ms_teams_conversation_id.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/send_to_ms_teams_email.py` & `trycourier-6.0.4/src/courier/profiles/types/send_to_ms_teams_email.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/send_to_ms_teams_user_id.py` & `trycourier-6.0.4/src/courier/profiles/types/send_to_ms_teams_user_id.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/send_to_slack_channel.py` & `trycourier-6.0.4/src/courier/profiles/types/send_to_slack_channel.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/send_to_slack_email.py` & `trycourier-6.0.4/src/courier/profiles/types/send_to_slack_email.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/send_to_slack_user_id.py` & `trycourier-6.0.4/src/courier/profiles/types/send_to_slack_user_id.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/slack_base_properties.py` & `trycourier-6.0.4/src/courier/profiles/types/slack_base_properties.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/snooze_rule.py` & `trycourier-6.0.4/src/courier/profiles/types/snooze_rule.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/subscribe_to_lists_request.py` & `trycourier-6.0.4/src/courier/profiles/types/subscribe_to_lists_request.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/subscribe_to_lists_request_list_object.py` & `trycourier-6.0.4/src/courier/profiles/types/subscribe_to_lists_request_list_object.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/subscribe_to_lists_response.py` & `trycourier-6.0.4/src/courier/profiles/types/subscribe_to_lists_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/token.py` & `trycourier-6.0.4/src/courier/profiles/types/token.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/profiles/types/user_profile.py` & `trycourier-6.0.4/src/courier/profiles/types/user_profile.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/__init__.py` & `trycourier-6.0.4/src/courier/send/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/__init__.py` & `trycourier-6.0.4/src/courier/send/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/audience_filter.py` & `trycourier-6.0.4/src/courier/send/types/audience_filter.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/audience_recipient.py` & `trycourier-6.0.4/src/courier/send/types/audience_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/base_message.py` & `trycourier-6.0.4/src/courier/send/types/base_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/base_message_send_to.py` & `trycourier-6.0.4/src/courier/send/types/base_message_send_to.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/base_social_presence.py` & `trycourier-6.0.4/src/courier/send/types/base_social_presence.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/brand_settings_email.py` & `trycourier-6.0.4/src/courier/send/types/brand_settings_email.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/brand_settings_in_app.py` & `trycourier-6.0.4/src/courier/send/types/brand_settings_in_app.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/brand_settings_social_presence.py` & `trycourier-6.0.4/src/courier/send/types/brand_settings_social_presence.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/brand_template.py` & `trycourier-6.0.4/src/courier/send/types/brand_template.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/brand_template_override.py` & `trycourier-6.0.4/src/courier/send/types/brand_template_override.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/channel.py` & `trycourier-6.0.4/src/courier/send/types/channel.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/channel_metadata.py` & `trycourier-6.0.4/src/courier/send/types/channel_metadata.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/content_message.py` & `trycourier-6.0.4/src/courier/send/types/content_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/delay.py` & `trycourier-6.0.4/src/courier/send/types/delay.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/elemental_action_node.py` & `trycourier-6.0.4/src/courier/send/types/elemental_action_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/elemental_base_node.py` & `trycourier-6.0.4/src/courier/send/types/elemental_base_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/elemental_channel_node.py` & `trycourier-6.0.4/src/courier/send/types/elemental_channel_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/elemental_content.py` & `trycourier-6.0.4/src/courier/send/types/elemental_content.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/elemental_content_sugar.py` & `trycourier-6.0.4/src/courier/send/types/elemental_content_sugar.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/elemental_divider_node.py` & `trycourier-6.0.4/src/courier/send/types/elemental_divider_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/elemental_group_node.py` & `trycourier-6.0.4/src/courier/send/types/elemental_group_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/elemental_image_node.py` & `trycourier-6.0.4/src/courier/send/types/elemental_image_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/elemental_meta_node.py` & `trycourier-6.0.4/src/courier/send/types/elemental_meta_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/elemental_node.py` & `trycourier-6.0.4/src/courier/send/types/elemental_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/elemental_quote_node.py` & `trycourier-6.0.4/src/courier/send/types/elemental_quote_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/elemental_text_node.py` & `trycourier-6.0.4/src/courier/send/types/elemental_text_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/email_footer.py` & `trycourier-6.0.4/src/courier/send/types/email_footer.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/email_head.py` & `trycourier-6.0.4/src/courier/send/types/email_head.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/email_header.py` & `trycourier-6.0.4/src/courier/send/types/email_header.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/expiry.py` & `trycourier-6.0.4/src/courier/send/types/expiry.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/i_profile_preferences.py` & `trycourier-6.0.4/src/courier/send/types/i_profile_preferences.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/icons.py` & `trycourier-6.0.4/src/courier/send/types/icons.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/invalid_list_pattern_recipient.py` & `trycourier-6.0.4/src/courier/send/types/invalid_list_pattern_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/invalid_list_recipient.py` & `trycourier-6.0.4/src/courier/send/types/invalid_list_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/invalid_user_recipient.py` & `trycourier-6.0.4/src/courier/send/types/invalid_user_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/list_filter.py` & `trycourier-6.0.4/src/courier/send/types/list_filter.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/list_pattern_recipient.py` & `trycourier-6.0.4/src/courier/send/types/list_pattern_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/list_pattern_recipient_type.py` & `trycourier-6.0.4/src/courier/send/types/list_pattern_recipient_type.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/list_recipient.py` & `trycourier-6.0.4/src/courier/send/types/list_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/list_recipient_type.py` & `trycourier-6.0.4/src/courier/send/types/list_recipient_type.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/locale.py` & `trycourier-6.0.4/src/courier/send/types/locale.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/logo.py` & `trycourier-6.0.4/src/courier/send/types/logo.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/message_channel_email_override.py` & `trycourier-6.0.4/src/courier/send/types/message_channel_email_override.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/message_context.py` & `trycourier-6.0.4/src/courier/send/types/message_context.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/message_metadata.py` & `trycourier-6.0.4/src/courier/send/types/message_metadata.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/message_providers_type.py` & `trycourier-6.0.4/src/courier/send/types/message_providers_type.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/metadata.py` & `trycourier-6.0.4/src/courier/send/types/metadata.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/ms_teams_recipient.py` & `trycourier-6.0.4/src/courier/send/types/ms_teams_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/preference.py` & `trycourier-6.0.4/src/courier/send/types/preference.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/preferences.py` & `trycourier-6.0.4/src/courier/send/types/preferences.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/recipient.py` & `trycourier-6.0.4/src/courier/send/types/recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/routing.py` & `trycourier-6.0.4/src/courier/send/types/routing.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/routing_strategy_channel.py` & `trycourier-6.0.4/src/courier/send/types/routing_strategy_channel.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/routing_strategy_provider.py` & `trycourier-6.0.4/src/courier/send/types/routing_strategy_provider.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/slack_recipient.py` & `trycourier-6.0.4/src/courier/send/types/slack_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/template_message.py` & `trycourier-6.0.4/src/courier/send/types/template_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/timeout.py` & `trycourier-6.0.4/src/courier/send/types/timeout.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/timeouts.py` & `trycourier-6.0.4/src/courier/send/types/timeouts.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/tracking_override.py` & `trycourier-6.0.4/src/courier/send/types/tracking_override.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/user_recipient.py` & `trycourier-6.0.4/src/courier/send/types/user_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/user_recipient_type.py` & `trycourier-6.0.4/src/courier/send/types/user_recipient_type.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/utm.py` & `trycourier-6.0.4/src/courier/send/types/utm.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/send/types/widget_background.py` & `trycourier-6.0.4/src/courier/send/types/widget_background.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/templates/client.py` & `trycourier-6.0.4/src/courier/templates/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/templates/types/__init__.py` & `trycourier-6.0.4/src/courier/templates/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/templates/types/list_templates_response.py` & `trycourier-6.0.4/src/courier/templates/types/list_templates_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/templates/types/notification_templates.py` & `trycourier-6.0.4/src/courier/templates/types/notification_templates.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/templates/types/routing_strategy.py` & `trycourier-6.0.4/src/courier/templates/types/routing_strategy.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/templates/types/tag.py` & `trycourier-6.0.4/src/courier/templates/types/tag.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/templates/types/tag_data.py` & `trycourier-6.0.4/src/courier/templates/types/tag_data.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/tenants/client.py` & `trycourier-6.0.4/src/courier/tenants/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from .types.default_preferences import DefaultPreferences
 from .types.list_users_for_tenant_response import ListUsersForTenantResponse
-from .types.template_property import TemplateProperty
 from .types.tenant import Tenant
 from .types.tenant_list_response import TenantListResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
@@ -29,15 +28,15 @@
     def create_or_replace(
         self,
         tenant_id: str,
         *,
         name: str,
         parent_tenant_id: typing.Optional[str] = OMIT,
         default_preferences: typing.Optional[DefaultPreferences] = OMIT,
-        properties: typing.Optional[typing.Sequence[TemplateProperty]] = OMIT,
+        properties: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         user_profile: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         brand_id: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> Tenant:
         """
         Parameters
         ----------
@@ -49,15 +48,15 @@
 
         parent_tenant_id : typing.Optional[str]
             Tenant's parent id (if any).
 
         default_preferences : typing.Optional[DefaultPreferences]
             Defines the preferences used for the tenant when the user hasn't specified their own.
 
-        properties : typing.Optional[typing.Sequence[TemplateProperty]]
+        properties : typing.Optional[typing.Dict[str, typing.Any]]
             Arbitrary properties accessible to a template.
 
         user_profile : typing.Optional[typing.Dict[str, typing.Any]]
             A user profile object merged with user profile on send.
 
         brand_id : typing.Optional[str]
             Brand to be used for the account when one is not specified by the send call.
@@ -80,15 +79,15 @@
         client.tenants.create_or_replace(
             tenant_id="string",
             name="string",
             parent_tenant_id="string",
             default_preferences=DefaultPreferences(
                 items=[SubscriptionTopic()],
             ),
-            properties=[{"key": "value"}],
+            properties={"string": {"key": "value"}},
             user_profile={"string": {"key": "value"}},
             brand_id="string",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if parent_tenant_id is not OMIT:
             _request["parent_tenant_id"] = parent_tenant_id
@@ -415,15 +414,15 @@
     async def create_or_replace(
         self,
         tenant_id: str,
         *,
         name: str,
         parent_tenant_id: typing.Optional[str] = OMIT,
         default_preferences: typing.Optional[DefaultPreferences] = OMIT,
-        properties: typing.Optional[typing.Sequence[TemplateProperty]] = OMIT,
+        properties: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         user_profile: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         brand_id: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> Tenant:
         """
         Parameters
         ----------
@@ -435,15 +434,15 @@
 
         parent_tenant_id : typing.Optional[str]
             Tenant's parent id (if any).
 
         default_preferences : typing.Optional[DefaultPreferences]
             Defines the preferences used for the tenant when the user hasn't specified their own.
 
-        properties : typing.Optional[typing.Sequence[TemplateProperty]]
+        properties : typing.Optional[typing.Dict[str, typing.Any]]
             Arbitrary properties accessible to a template.
 
         user_profile : typing.Optional[typing.Dict[str, typing.Any]]
             A user profile object merged with user profile on send.
 
         brand_id : typing.Optional[str]
             Brand to be used for the account when one is not specified by the send call.
@@ -466,15 +465,15 @@
         await client.tenants.create_or_replace(
             tenant_id="string",
             name="string",
             parent_tenant_id="string",
             default_preferences=DefaultPreferences(
                 items=[SubscriptionTopic()],
             ),
-            properties=[{"key": "value"}],
+            properties={"string": {"key": "value"}},
             user_profile={"string": {"key": "value"}},
             brand_id="string",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if parent_tenant_id is not OMIT:
             _request["parent_tenant_id"] = parent_tenant_id
```

### Comparing `trycourier-6.0.3/src/courier/tenants/types/__init__.py` & `trycourier-6.0.4/src/courier/tenants/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/tenants/types/default_preferences.py` & `trycourier-6.0.4/src/courier/tenants/types/default_preferences.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/tenants/types/list_users_for_tenant_response.py` & `trycourier-6.0.4/src/courier/tenants/types/list_users_for_tenant_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/tenants/types/subscription_topic.py` & `trycourier-6.0.4/src/courier/tenants/types/subscription_topic.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/tenants/types/tenant.py` & `trycourier-6.0.4/src/courier/tenants/types/tenant.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import pydantic_v1
 from .default_preferences import DefaultPreferences
-from .template_property import TemplateProperty
 
 
 class Tenant(pydantic_v1.BaseModel):
     id: str = pydantic_v1.Field()
     """
     Id of the tenant.
     """
@@ -26,15 +25,15 @@
     """
 
     default_preferences: typing.Optional[DefaultPreferences] = pydantic_v1.Field(default=None)
     """
     Defines the preferences used for the account when the user hasn't specified their own.
     """
 
-    properties: typing.Optional[TemplateProperty] = pydantic_v1.Field(default=None)
+    properties: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
     """
     Arbitrary properties accessible to a template.
     """
 
     user_profile: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
     """
     A user profile object merged with user profile on send.
```

### Comparing `trycourier-6.0.3/src/courier/tenants/types/tenant_list_response.py` & `trycourier-6.0.4/src/courier/tenants/types/tenant_list_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/translations/client.py` & `trycourier-6.0.4/src/courier/translations/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/types/send_message_response.py` & `trycourier-6.0.4/src/courier/types/send_message_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/__init__.py` & `trycourier-6.0.4/src/courier/users/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/client.py` & `trycourier-6.0.4/src/courier/users/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/preferences/client.py` & `trycourier-6.0.4/src/courier/users/preferences/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/preferences/types/__init__.py` & `trycourier-6.0.4/src/courier/users/preferences/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/preferences/types/topic_preference.py` & `trycourier-6.0.4/src/courier/users/preferences/types/topic_preference.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/preferences/types/topic_preference_update.py` & `trycourier-6.0.4/src/courier/users/preferences/types/topic_preference_update.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/preferences/types/user_preferences_get_response.py` & `trycourier-6.0.4/src/courier/users/preferences/types/user_preferences_get_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/preferences/types/user_preferences_list_response.py` & `trycourier-6.0.4/src/courier/users/preferences/types/user_preferences_list_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/preferences/types/user_preferences_update_response.py` & `trycourier-6.0.4/src/courier/users/preferences/types/user_preferences_update_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/tenants/client.py` & `trycourier-6.0.4/src/courier/users/tenants/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/tenants/types/add_user_to_single_tenants_params_profile.py` & `trycourier-6.0.4/src/courier/users/tenants/types/add_user_to_single_tenants_params_profile.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/tenants/types/list_tenants_for_user_response.py` & `trycourier-6.0.4/src/courier/users/tenants/types/list_tenants_for_user_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/tokens/__init__.py` & `trycourier-6.0.4/src/courier/users/tokens/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/tokens/client.py` & `trycourier-6.0.4/src/courier/users/tokens/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/tokens/types/__init__.py` & `trycourier-6.0.4/src/courier/users/tokens/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/tokens/types/delete_user_token_opts.py` & `trycourier-6.0.4/src/courier/users/tokens/types/delete_user_token_opts.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/tokens/types/device.py` & `trycourier-6.0.4/src/courier/users/tokens/types/device.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/tokens/types/get_user_token_opts.py` & `trycourier-6.0.4/src/courier/users/tokens/types/get_user_token_opts.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/tokens/types/get_user_token_response.py` & `trycourier-6.0.4/src/courier/users/tokens/types/get_user_token_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/tokens/types/get_user_tokens_opts.py` & `trycourier-6.0.4/src/courier/users/tokens/types/get_user_tokens_opts.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/tokens/types/patch_operation.py` & `trycourier-6.0.4/src/courier/users/tokens/types/patch_operation.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/tokens/types/patch_user_token_opts.py` & `trycourier-6.0.4/src/courier/users/tokens/types/patch_user_token_opts.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/tokens/types/put_user_token_opts.py` & `trycourier-6.0.4/src/courier/users/tokens/types/put_user_token_opts.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/tokens/types/put_user_tokens_opts.py` & `trycourier-6.0.4/src/courier/users/tokens/types/put_user_tokens_opts.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/tokens/types/tracking.py` & `trycourier-6.0.4/src/courier/users/tokens/types/tracking.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/src/courier/users/tokens/types/user_token.py` & `trycourier-6.0.4/src/courier/users/tokens/types/user_token.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.3/PKG-INFO` & `trycourier-6.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trycourier
-Version: 6.0.3
+Version: 6.0.4
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


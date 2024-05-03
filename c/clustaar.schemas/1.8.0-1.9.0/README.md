# Comparing `tmp/clustaar.schemas-1.8.0.tar.gz` & `tmp/clustaar_schemas-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clustaar.schemas-1.8.0.tar", last modified: Tue Mar 19 15:50:16 2024, max compression
+gzip compressed data, was "clustaar_schemas-1.9.0.tar", last modified: Fri May  3 16:14:37 2024, max compression
```

## Comparing `clustaar.schemas-1.8.0.tar` & `clustaar_schemas-1.9.0.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:16.100717 clustaar.schemas-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:16.080717 clustaar.schemas-1.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:16.084717 clustaar.schemas-1.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/.github/workflows/build_dev_package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/.github/workflows/build_package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/.github/workflows/launch_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-19 15:50:16.100717 clustaar.schemas-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:16.084717 clustaar.schemas-1.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7608 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:16.084717 clustaar.schemas-1.8.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-03-19 15:50:16.104717 clustaar.schemas-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:16.080717 clustaar.schemas-1.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:16.084717 clustaar.schemas-1.8.0/src/clustaar/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/src/clustaar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:16.088717 clustaar.schemas-1.8.0/src/clustaar/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/src/clustaar/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/src/clustaar/schemas/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/src/clustaar/schemas/custom_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/src/clustaar/schemas/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/src/clustaar/schemas/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/src/clustaar/schemas/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)    41282 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/src/clustaar/schemas/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/src/clustaar/schemas/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:16.100717 clustaar.schemas-1.8.0/src/clustaar.schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-19 15:50:16.000000 clustaar.schemas-1.8.0/src/clustaar.schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-03-19 15:50:16.000000 clustaar.schemas-1.8.0/src/clustaar.schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 15:50:16.000000 clustaar.schemas-1.8.0/src/clustaar.schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 15:50:16.000000 clustaar.schemas-1.8.0/src/clustaar.schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-19 15:50:16.000000 clustaar.schemas-1.8.0/src/clustaar.schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-19 15:50:16.000000 clustaar.schemas-1.8.0/src/clustaar.schemas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:16.088717 clustaar.schemas-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:16.088717 clustaar.schemas-1.8.0/tests/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:16.100717 clustaar.schemas-1.8.0/tests/schemas/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_ask_location_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_assign_intercom_conversation_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_close_iadvize_conversation_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_close_intercom_conversation_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_contain_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_create_user_request_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_create_zendesk_ticket_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_custom_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_customer_satisfaction_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_customer_satisfaction_callback_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_equals_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_flow_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_flow_connection_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_flow_connection_team_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_flow_connection_user_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_go_to_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_google_custom_search_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_is_greater_than_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_is_greater_than_or_equal_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_is_less_than_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_is_less_than_or_equal_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_is_logged_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_is_not_logged_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_is_not_set_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_is_number_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_is_offline_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_is_online_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_is_set_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_jump_to_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_legacy_reply_to_message_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_match_intent_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_match_regexp_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_open_url_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_pause_bot_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_predicate_message_getter.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_predicate_session_value_getter.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_predicate_user_attribute_getter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_send_ai_task_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_send_cards_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_send_choices_list_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_send_email_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_send_image_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_send_js_event_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_send_quick_replies_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_send_simple_cards_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_send_text_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_send_webhook_request_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_set_user_attribute_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_share_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_step_target.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_store_session_value_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_story_target.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_transfer_iadvize_conversation_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_url_loaded_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_video.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_wait_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_webhook_interlocutor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/v1/test_webhook_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:16.100717 clustaar.schemas-1.8.0/tests/schemas/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/validators/test_is_regexp.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/schemas/validators/test_object_id.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-19 15:50:00.000000 clustaar.schemas-1.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:14:37.238089 clustaar_schemas-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:14:37.218089 clustaar_schemas-1.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:14:37.222089 clustaar_schemas-1.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/.github/workflows/build_dev_package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/.github/workflows/build_package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/.github/workflows/launch_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-03 16:14:37.238089 clustaar_schemas-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:14:37.222089 clustaar_schemas-1.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7608 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:14:37.222089 clustaar_schemas-1.9.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-03 16:14:37.238089 clustaar_schemas-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:14:37.218089 clustaar_schemas-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:14:37.222089 clustaar_schemas-1.9.0/src/clustaar/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/src/clustaar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:14:37.226089 clustaar_schemas-1.9.0/src/clustaar/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/src/clustaar/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/src/clustaar/schemas/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/src/clustaar/schemas/custom_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/src/clustaar/schemas/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/src/clustaar/schemas/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/src/clustaar/schemas/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41601 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/src/clustaar/schemas/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/src/clustaar/schemas/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:14:37.238089 clustaar_schemas-1.9.0/src/clustaar.schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-03 16:14:37.000000 clustaar_schemas-1.9.0/src/clustaar.schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-03 16:14:37.000000 clustaar_schemas-1.9.0/src/clustaar.schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:14:37.000000 clustaar_schemas-1.9.0/src/clustaar.schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:14:37.000000 clustaar_schemas-1.9.0/src/clustaar.schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-03 16:14:37.000000 clustaar_schemas-1.9.0/src/clustaar.schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 16:14:37.000000 clustaar_schemas-1.9.0/src/clustaar.schemas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:14:37.226089 clustaar_schemas-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:14:37.226089 clustaar_schemas-1.9.0/tests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:14:37.238089 clustaar_schemas-1.9.0/tests/schemas/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_ask_location_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_assign_intercom_conversation_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_close_iadvize_conversation_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_close_intercom_conversation_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_contain_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_create_user_request_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_create_zendesk_ticket_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_custom_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_customer_satisfaction_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_customer_satisfaction_callback_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_equals_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_flow_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_flow_connection_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_flow_connection_team_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_flow_connection_user_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_go_to_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_google_custom_search_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_is_greater_than_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_is_greater_than_or_equal_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_is_less_than_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_is_less_than_or_equal_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_is_logged_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_is_not_logged_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_is_not_set_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_is_number_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_is_offline_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_is_online_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_is_set_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_jump_to_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_legacy_reply_to_message_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_match_intent_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_match_regexp_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_open_url_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_pause_bot_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_predicate_message_getter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_predicate_session_value_getter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_predicate_user_attribute_getter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_send_ai_task_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_send_cards_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_send_choices_list_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_send_email_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_send_image_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_send_js_event_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_send_quick_replies_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_send_simple_cards_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_send_text_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_send_webhook_request_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_set_user_attribute_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_share_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_step_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_store_session_value_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_story_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_transfer_iadvize_conversation_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_url_loaded_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_wait_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_webhook_interlocutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/v1/test_webhook_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:14:37.238089 clustaar_schemas-1.9.0/tests/schemas/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/validators/test_is_regexp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/schemas/validators/test_object_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-03 16:14:31.000000 clustaar_schemas-1.9.0/tox.ini
```

### Comparing `clustaar.schemas-1.8.0/.coveragerc` & `clustaar_schemas-1.9.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/.github/workflows/build_dev_package.yml` & `clustaar_schemas-1.9.0/.github/workflows/build_dev_package.yml`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/.github/workflows/build_package.yml` & `clustaar_schemas-1.9.0/.github/workflows/build_package.yml`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/.github/workflows/launch_tests.yml` & `clustaar_schemas-1.9.0/.github/workflows/launch_tests.yml`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/.gitignore` & `clustaar_schemas-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/LICENSE.txt` & `clustaar_schemas-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/PKG-INFO` & `clustaar_schemas-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustaar.schemas
-Version: 1.8.0
+Version: 1.9.0
 Summary: Clustaar objects schemas
 Home-page: https://github.com/Clustaar/clustaar.schemas
 Author: Aurélien
 Author-email: aurelien@clustaar.com
 License: mit
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `clustaar.schemas-1.8.0/docs/Makefile` & `clustaar_schemas-1.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/docs/conf.py` & `clustaar_schemas-1.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/docs/index.rst` & `clustaar_schemas-1.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/requirements.txt` & `clustaar_schemas-1.9.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/setup.cfg` & `clustaar_schemas-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/setup.py` & `clustaar_schemas-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/src/clustaar/schemas/constants.py` & `clustaar_schemas-1.9.0/src/clustaar/schemas/constants.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/src/clustaar/schemas/custom_schemas.py` & `clustaar_schemas-1.9.0/src/clustaar/schemas/custom_schemas.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/src/clustaar/schemas/fields.py` & `clustaar_schemas-1.9.0/src/clustaar/schemas/fields.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/src/clustaar/schemas/models.py` & `clustaar_schemas-1.9.0/src/clustaar/schemas/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 
 
 # Bot actions
 AskLocationAction = model("AskLocationAction", "message callback_action")
 StepTarget = model("StepTarget", "step_id name")
 StoryTarget = model("StoryTarget", "story_id name")
 GoToAction = model("GoToAction", "target session_values")
-LegacyReplyToMessageAction = model("LegacyReplyToMessageAction", "message")
+DocumentAttachment = model("name url")
+LegacyReplyToMessageAction = model("LegacyReplyToMessageAction", "message attachments")
 OpenURLAction = model("OpenURLAction", "url")
 ShareAction = model("ShareAction", "")
 SendImageAction = model("SendImageAction", "image_url alt")
 SendTextAction = model("SendTextAction", "alternatives text")
 SendJSEventAction = model("SendJSEventAction", "event payload")
 SendEmailAction = model(
     "SendEmailAction", "from_name from_email content subject recipient reply_to_name reply_to_email"
```

### Comparing `clustaar.schemas-1.8.0/src/clustaar/schemas/processors.py` & `clustaar_schemas-1.9.0/src/clustaar/schemas/processors.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/src/clustaar/schemas/v1.py` & `clustaar_schemas-1.9.0/src/clustaar/schemas/v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,21 +258,32 @@
             on="type", allow_none=True, schemas={"step": STEP_TARGET, "story": STORY_TARGET}
         ),
         "kind": f.String(validators=v.In(CUSTOMER_SATISFACTION_CHOICE_KINDS)),
     },
     name="customer_satisfaction_callback_action",
 )
 
+DOCUMENT_ATTACHMENT = Schema(
+    {
+        "name": f.String(),
+        "url": f.String(),
+    },
+    name="document_attachment",
+)
+
 LEGACY_REPLY_TO_MESSAGE_ACTION = Schema(
     {
         "type": f.Constant(value="legacy_reply_to_message_action", read_only=True),
         "message": f.String(
             validators=v.Length(min=1, max=SEND_TEXT_ACTION_MESSAGE_MAX_LENGTH),
             pre_load=[html_sanitize],
         ),
+        "attachments": f.List(
+            f.Object(DOCUMENT_ATTACHMENT), allow_none=True, ignore_if_null=True, optional=True
+        ),
     },
     name="legacy_reply_to_message_action",
 )
 
 OPEN_URL_ACTION = Schema(
     {
         "type": f.Constant(value="open_url_action", read_only=True),
@@ -1125,14 +1136,15 @@
     """
     mapper = Mapper()
     mappings = {
         AskLocationAction: ASK_LOCATION_ACTION,
         StepTarget: STEP_TARGET,
         StoryTarget: STORY_TARGET,
         GoToAction: GO_TO_ACTION,
+        DocumentAttachment: DOCUMENT_ATTACHMENT,
         LegacyReplyToMessageAction: LEGACY_REPLY_TO_MESSAGE_ACTION,
         OpenURLAction: OPEN_URL_ACTION,
         ShareAction: SHARE_ACTION,
         SendImageAction: SEND_IMAGE_ACTION,
         SendTextAction: SEND_TEXT_ACTION,
         SendJSEventAction: SEND_JS_EVENT_ACTION,
         SendEmailAction: SEND_EMAIL_ACTION,
```

### Comparing `clustaar.schemas-1.8.0/src/clustaar/schemas/validators.py` & `clustaar_schemas-1.9.0/src/clustaar/schemas/validators.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/src/clustaar.schemas.egg-info/PKG-INFO` & `clustaar_schemas-1.9.0/src/clustaar.schemas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustaar.schemas
-Version: 1.8.0
+Version: 1.9.0
 Summary: Clustaar objects schemas
 Home-page: https://github.com/Clustaar/clustaar.schemas
 Author: Aurélien
 Author-email: aurelien@clustaar.com
 License: mit
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `clustaar.schemas-1.8.0/src/clustaar.schemas.egg-info/SOURCES.txt` & `clustaar_schemas-1.9.0/src/clustaar.schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_ask_location_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_ask_location_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_assign_intercom_conversation_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_assign_intercom_conversation_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_audio.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_audio.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_close_iadvize_conversation_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_close_iadvize_conversation_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_close_intercom_conversation_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_close_intercom_conversation_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_contain_condition.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_contain_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_coordinates.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_create_user_request_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_create_user_request_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_create_zendesk_ticket_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_create_zendesk_ticket_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_custom_event.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_custom_event.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_customer_satisfaction_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_customer_satisfaction_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_customer_satisfaction_callback_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_customer_satisfaction_callback_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_equals_condition.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_equals_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_file.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_file.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_flow_connection.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_flow_connection.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_flow_connection_predicate.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_flow_connection_predicate.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_flow_connection_team_predicate.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_flow_connection_team_predicate.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_flow_connection_user_predicate.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_flow_connection_user_predicate.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_go_to_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_go_to_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_google_custom_search_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_google_custom_search_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_image.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_image.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_is_greater_than_condition.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_is_greater_than_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_is_greater_than_or_equal_condition.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_is_greater_than_or_equal_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_is_less_than_condition.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_is_less_than_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_is_less_than_or_equal_condition.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_is_less_than_or_equal_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_is_logged_condition.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_is_logged_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_is_not_logged_condition.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_is_not_logged_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_is_not_set_condition.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_is_not_set_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_is_number_condition.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_is_number_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_is_offline_condition.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_is_offline_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_is_online_condition.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_is_online_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_is_set_condition.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_is_set_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_jump_to_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_jump_to_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_legacy_reply_to_message_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_legacy_reply_to_message_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_match_intent_condition.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_match_intent_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_match_regexp_condition.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_match_regexp_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_message.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_message.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_open_url_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_open_url_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_pause_bot_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_pause_bot_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_predicate_message_getter.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_predicate_message_getter.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_predicate_session_value_getter.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_predicate_session_value_getter.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_predicate_user_attribute_getter.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_predicate_user_attribute_getter.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_send_ai_task_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_send_ai_task_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,11 +78,12 @@
         assert isinstance(predicate.value_getter, MessageGetter)
 
 
 class TestValidate:
     def test_validation(self, data, action, mapper):
         result = mapper.validate(data, SEND_AI_TASK_ACTION)
 
+
 class TestDump(object):
     def test_returns_a_dict(self, data, action, mapper):
         result = mapper.dump(action, SEND_AI_TASK_ACTION)
         assert result == data
```

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_send_cards_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_send_cards_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_send_choices_list_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_send_choices_list_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_send_email_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_send_email_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_send_image_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_send_image_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_send_js_event_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_send_js_event_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_send_quick_replies_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_send_quick_replies_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_send_simple_cards_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_send_simple_cards_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_send_text_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_send_text_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_send_webhook_request_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_send_webhook_request_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_set_user_attribute_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_set_user_attribute_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_share_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_share_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_step_target.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_step_target.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_store_session_value_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_store_session_value_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_story_target.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_story_target.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_transfer_iadvize_conversation_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_transfer_iadvize_conversation_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_url_loaded_event.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_url_loaded_event.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_video.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_video.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_wait_action.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_wait_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_webhook_interlocutor.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_webhook_interlocutor.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.8.0/tests/schemas/v1/test_webhook_request.py` & `clustaar_schemas-1.9.0/tests/schemas/v1/test_webhook_request.py`

 * *Files identical despite different names*


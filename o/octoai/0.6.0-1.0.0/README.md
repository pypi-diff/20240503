# Comparing `tmp/octoai-0.6.0.tar.gz` & `tmp/octoai-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octoai-0.6.0.tar", max compression
+gzip compressed data, was "octoai-1.0.0.tar", max compression
```

## Comparing `octoai-0.6.0.tar` & `octoai-1.0.0.tar`

### file list

```diff
@@ -1,125 +1,125 @@
--rw-r--r--   0        0        0     4922 2024-05-01 20:10:13.103144 octoai-0.6.0/README.md
--rw-r--r--   0        0        0      649 2024-05-01 20:10:13.103144 octoai-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      308 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/__init__.py
--rw-r--r--   0        0        0     2266 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/__init__.py
--rw-r--r--   0        0        0    36620 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/client.py
--rw-r--r--   0        0        0      170 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/errors/__init__.py
--rw-r--r--   0        0        0      314 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     2925 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/__init__.py
--rw-r--r--   0        0        0     2172 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/asset.py
--rw-r--r--   0        0        0      201 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/asset_type.py
--rw-r--r--   0        0        0      646 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/base_engine.py
--rw-r--r--   0        0        0      164 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/base_engine_type.py
--rw-r--r--   0        0        0     1241 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/checkpoint_data.py
--rw-r--r--   0        0        0      891 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/complete_asset_upload_response.py
--rw-r--r--   0        0        0     1257 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/create_asset_response.py
--rw-r--r--   0        0        0     1218 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/create_asset_response_transfer_api.py
--rw-r--r--   0        0        0     1870 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/data.py
--rw-r--r--   0        0        0      164 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/data_type.py
--rw-r--r--   0        0        0      986 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/delete_asset_response.py
--rw-r--r--   0        0        0     1133 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/file_data.py
--rw-r--r--   0        0        0      191 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/file_extension.py
--rw-r--r--   0        0        0      155 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/file_format.py
--rw-r--r--   0        0        0      181 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/file_structure.py
--rw-r--r--   0        0        0      955 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/http_validation_error.py
--rw-r--r--   0        0        0     1098 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/latent_data.py
--rw-r--r--   0        0        0     1137 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/list_assets_response.py
--rw-r--r--   0        0        0     1340 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/lora_data.py
--rw-r--r--   0        0        0     1096 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/no_transfer_api.py
--rw-r--r--   0        0        0     1003 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/presigned_url_transfer_api.py
--rw-r--r--   0        0        0     1128 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/retrieve_asset_response.py
--rw-r--r--   0        0        0     1241 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/retrieve_asset_response_transfer_api.py
--rw-r--r--   0        0        0      221 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/status.py
--rw-r--r--   0        0        0     1505 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/sts_transfer_api.py
--rw-r--r--   0        0        0     1370 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/textual_inversion_data.py
--rw-r--r--   0        0        0      163 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/transfer_api_type.py
--rw-r--r--   0        0        0     1234 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/vae_data.py
--rw-r--r--   0        0        0      974 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     5549 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/base_client.py
--rw-r--r--   0        0        0    13262 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/client.py
--rw-r--r--   0        0        0      853 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/core/api_error.py
--rw-r--r--   0        0        0     2224 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/core/request_options.py
--rw-r--r--   0        0        0      732 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/environment.py
--rw-r--r--   0        0        0     1032 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/__init__.py
--rw-r--r--   0        0        0    31006 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/client.py
--rw-r--r--   0        0        0      170 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/errors/__init__.py
--rw-r--r--   0        0        0      314 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     1266 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/types/__init__.py
--rw-r--r--   0        0        0      646 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/types/base_engine.py
--rw-r--r--   0        0        0      826 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/types/details.py
--rw-r--r--   0        0        0      955 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/types/http_validation_error.py
--rw-r--r--   0        0        0     1189 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/types/list_tunes_response.py
--rw-r--r--   0        0        0     1592 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/types/lora_tune.py
--rw-r--r--   0        0        0     1111 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/types/lora_tune_checkpoint.py
--rw-r--r--   0        0        0     1039 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/types/lora_tune_file.py
--rw-r--r--   0        0        0     1062 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/types/text_to_speech_latent_tune.py
--rw-r--r--   0        0        0     2273 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/fine_tuning/types/tune.py
--rw-r--r--   0        0        0      846 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/fine_tuning/types/tune_details.py
--rw-r--r--   0        0        0     1122 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/fine_tuning/types/tune_result.py
--rw-r--r--   0        0        0      192 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/fine_tuning/types/tune_status.py
--rw-r--r--   0        0        0      259 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/fine_tuning/types/tune_type.py
--rw-r--r--   0        0        0      974 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/fine_tuning/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/fine_tuning/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      838 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/__init__.py
--rw-r--r--   0        0        0   123904 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/client.py
--rw-r--r--   0        0        0      170 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/errors/__init__.py
--rw-r--r--   0        0        0      314 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     1115 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/__init__.py
--rw-r--r--   0        0        0      955 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/http_validation_error.py
--rw-r--r--   0        0        0      152 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/image_encoding.py
--rw-r--r--   0        0        0     1245 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/image_generation.py
--rw-r--r--   0        0        0     5332 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/image_generation_request.py
--rw-r--r--   0        0        0      162 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/image_generation_request_seed.py
--rw-r--r--   0        0        0     1205 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/image_generation_response.py
--rw-r--r--   0        0        0      514 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/scheduler.py
--rw-r--r--   0        0        0     1880 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/sdxl_styles.py
--rw-r--r--   0        0        0      974 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     1271 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/video_generation.py
--rw-r--r--   0        0        0      162 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/video_generation_request_seed.py
--rw-r--r--   0        0        0     1208 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/video_generation_response.py
--rw-r--r--   0        0        0        0 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/py.typed
--rw-r--r--   0        0        0     1528 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/__init__.py
--rw-r--r--   0        0        0    54677 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/client.py
--rw-r--r--   0        0        0      248 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/errors/__init__.py
--rw-r--r--   0        0        0      290 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/errors/internal_server_error.py
--rw-r--r--   0        0        0      314 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     2131 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/__init__.py
--rw-r--r--   0        0        0     1358 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/chat_completion_choice.py
--rw-r--r--   0        0        0     1684 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/chat_completion_chunk.py
--rw-r--r--   0        0        0     1133 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/chat_completion_chunk_choice.py
--rw-r--r--   0        0        0     1100 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/chat_completion_delta.py
--rw-r--r--   0        0        0     1066 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/chat_completion_request_ext.py
--rw-r--r--   0        0        0     1143 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/chat_completion_request_ext_vllm.py
--rw-r--r--   0        0        0     1688 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/chat_completion_response.py
--rw-r--r--   0        0        0     1054 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/chat_completion_response_format.py
--rw-r--r--   0        0        0      947 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/chat_fn_call.py
--rw-r--r--   0        0        0     1061 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/chat_message.py
--rw-r--r--   0        0        0     1045 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/completion_choice.py
--rw-r--r--   0        0        0     1429 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/completion_response.py
--rw-r--r--   0        0        0      163 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/create_chat_completion_request_function_call.py
--rw-r--r--   0        0        0      169 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/create_chat_completion_stream_request_function_call.py
--rw-r--r--   0        0        0     1265 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/error_response.py
--rw-r--r--   0        0        0      153 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/error_response_validation_errors_value.py
--rw-r--r--   0        0        0      189 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/finish_reason.py
--rw-r--r--   0        0        0      982 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/function.py
--rw-r--r--   0        0        0      955 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/http_validation_error.py
--rw-r--r--   0        0        0     1247 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/log_probs.py
--rw-r--r--   0        0        0      174 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/prompt.py
--rw-r--r--   0        0        0      123 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/stop.py
--rw-r--r--   0        0        0     1228 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/usage_stats.py
--rw-r--r--   0        0        0      974 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     7630 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/uploading_asset_library.py
--rw-r--r--   0        0        0     2799 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/util.py
--rw-r--r--   0        0        0       74 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/version.py
--rw-r--r--   0        0        0     5526 1970-01-01 00:00:00.000000 octoai-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     4922 2024-05-01 23:28:15.979270 octoai-1.0.0/README.md
+-rw-r--r--   0        0        0      649 2024-05-01 23:28:15.979270 octoai-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      308 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/__init__.py
+-rw-r--r--   0        0        0     2266 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/__init__.py
+-rw-r--r--   0        0        0    36620 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/client.py
+-rw-r--r--   0        0        0      170 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/errors/__init__.py
+-rw-r--r--   0        0        0      314 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0     2925 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/__init__.py
+-rw-r--r--   0        0        0     2172 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/asset.py
+-rw-r--r--   0        0        0      201 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/asset_type.py
+-rw-r--r--   0        0        0      646 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/base_engine.py
+-rw-r--r--   0        0        0      164 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/base_engine_type.py
+-rw-r--r--   0        0        0     1241 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/checkpoint_data.py
+-rw-r--r--   0        0        0      891 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/complete_asset_upload_response.py
+-rw-r--r--   0        0        0     1257 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/create_asset_response.py
+-rw-r--r--   0        0        0     1218 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/create_asset_response_transfer_api.py
+-rw-r--r--   0        0        0     1870 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/data.py
+-rw-r--r--   0        0        0      164 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/data_type.py
+-rw-r--r--   0        0        0      986 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/delete_asset_response.py
+-rw-r--r--   0        0        0     1133 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/file_data.py
+-rw-r--r--   0        0        0      191 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/file_extension.py
+-rw-r--r--   0        0        0      155 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/file_format.py
+-rw-r--r--   0        0        0      181 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/file_structure.py
+-rw-r--r--   0        0        0      955 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/http_validation_error.py
+-rw-r--r--   0        0        0     1098 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/latent_data.py
+-rw-r--r--   0        0        0     1137 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/list_assets_response.py
+-rw-r--r--   0        0        0     1340 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/lora_data.py
+-rw-r--r--   0        0        0     1096 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/no_transfer_api.py
+-rw-r--r--   0        0        0     1003 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/presigned_url_transfer_api.py
+-rw-r--r--   0        0        0     1128 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/retrieve_asset_response.py
+-rw-r--r--   0        0        0     1241 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/retrieve_asset_response_transfer_api.py
+-rw-r--r--   0        0        0      221 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/status.py
+-rw-r--r--   0        0        0     1505 2024-05-01 23:28:15.979270 octoai-1.0.0/src/octoai/asset_library/types/sts_transfer_api.py
+-rw-r--r--   0        0        0     1370 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/asset_library/types/textual_inversion_data.py
+-rw-r--r--   0        0        0      163 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/asset_library/types/transfer_api_type.py
+-rw-r--r--   0        0        0     1234 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/asset_library/types/vae_data.py
+-rw-r--r--   0        0        0      974 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/asset_library/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/asset_library/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     5549 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/base_client.py
+-rw-r--r--   0        0        0    13262 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/client.py
+-rw-r--r--   0        0        0      853 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/core/api_error.py
+-rw-r--r--   0        0        0     2224 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/core/request_options.py
+-rw-r--r--   0        0        0      732 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/environment.py
+-rw-r--r--   0        0        0     1032 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/fine_tuning/__init__.py
+-rw-r--r--   0        0        0    31006 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/fine_tuning/client.py
+-rw-r--r--   0        0        0      170 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/fine_tuning/errors/__init__.py
+-rw-r--r--   0        0        0      314 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/fine_tuning/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0     1266 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/fine_tuning/types/__init__.py
+-rw-r--r--   0        0        0      646 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/fine_tuning/types/base_engine.py
+-rw-r--r--   0        0        0      826 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/fine_tuning/types/details.py
+-rw-r--r--   0        0        0      955 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/fine_tuning/types/http_validation_error.py
+-rw-r--r--   0        0        0     1189 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/fine_tuning/types/list_tunes_response.py
+-rw-r--r--   0        0        0     1592 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/fine_tuning/types/lora_tune.py
+-rw-r--r--   0        0        0     1111 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/fine_tuning/types/lora_tune_checkpoint.py
+-rw-r--r--   0        0        0     1039 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/fine_tuning/types/lora_tune_file.py
+-rw-r--r--   0        0        0     1062 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/fine_tuning/types/text_to_speech_latent_tune.py
+-rw-r--r--   0        0        0     2273 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/fine_tuning/types/tune.py
+-rw-r--r--   0        0        0      846 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/fine_tuning/types/tune_details.py
+-rw-r--r--   0        0        0     1122 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/fine_tuning/types/tune_result.py
+-rw-r--r--   0        0        0      192 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/fine_tuning/types/tune_status.py
+-rw-r--r--   0        0        0      259 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/fine_tuning/types/tune_type.py
+-rw-r--r--   0        0        0      974 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/fine_tuning/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/fine_tuning/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      838 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/image_gen/__init__.py
+-rw-r--r--   0        0        0   123904 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/image_gen/client.py
+-rw-r--r--   0        0        0      170 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/image_gen/errors/__init__.py
+-rw-r--r--   0        0        0      314 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/image_gen/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0     1115 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/image_gen/types/__init__.py
+-rw-r--r--   0        0        0      955 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/image_gen/types/http_validation_error.py
+-rw-r--r--   0        0        0      152 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/image_gen/types/image_encoding.py
+-rw-r--r--   0        0        0     1245 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/image_gen/types/image_generation.py
+-rw-r--r--   0        0        0     5332 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/image_gen/types/image_generation_request.py
+-rw-r--r--   0        0        0      162 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/image_gen/types/image_generation_request_seed.py
+-rw-r--r--   0        0        0     1205 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/image_gen/types/image_generation_response.py
+-rw-r--r--   0        0        0      514 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/image_gen/types/scheduler.py
+-rw-r--r--   0        0        0     1880 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/image_gen/types/sdxl_styles.py
+-rw-r--r--   0        0        0      974 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/image_gen/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/image_gen/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     1271 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/image_gen/types/video_generation.py
+-rw-r--r--   0        0        0      162 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/image_gen/types/video_generation_request_seed.py
+-rw-r--r--   0        0        0     1208 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/image_gen/types/video_generation_response.py
+-rw-r--r--   0        0        0        0 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/py.typed
+-rw-r--r--   0        0        0     1528 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/__init__.py
+-rw-r--r--   0        0        0    54677 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/client.py
+-rw-r--r--   0        0        0      248 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/errors/__init__.py
+-rw-r--r--   0        0        0      290 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/errors/internal_server_error.py
+-rw-r--r--   0        0        0      314 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0     2131 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/__init__.py
+-rw-r--r--   0        0        0     1358 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/chat_completion_choice.py
+-rw-r--r--   0        0        0     1684 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/chat_completion_chunk.py
+-rw-r--r--   0        0        0     1133 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/chat_completion_chunk_choice.py
+-rw-r--r--   0        0        0     1100 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/chat_completion_delta.py
+-rw-r--r--   0        0        0     1066 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/chat_completion_request_ext.py
+-rw-r--r--   0        0        0     1143 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/chat_completion_request_ext_vllm.py
+-rw-r--r--   0        0        0     1688 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/chat_completion_response.py
+-rw-r--r--   0        0        0     1054 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/chat_completion_response_format.py
+-rw-r--r--   0        0        0      947 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/chat_fn_call.py
+-rw-r--r--   0        0        0     1061 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/chat_message.py
+-rw-r--r--   0        0        0     1045 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/completion_choice.py
+-rw-r--r--   0        0        0     1429 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/completion_response.py
+-rw-r--r--   0        0        0      163 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/create_chat_completion_request_function_call.py
+-rw-r--r--   0        0        0      169 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/create_chat_completion_stream_request_function_call.py
+-rw-r--r--   0        0        0     1265 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/error_response.py
+-rw-r--r--   0        0        0      153 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/error_response_validation_errors_value.py
+-rw-r--r--   0        0        0      189 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/finish_reason.py
+-rw-r--r--   0        0        0      982 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/function.py
+-rw-r--r--   0        0        0      955 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/http_validation_error.py
+-rw-r--r--   0        0        0     1247 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/log_probs.py
+-rw-r--r--   0        0        0      174 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/prompt.py
+-rw-r--r--   0        0        0      123 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/stop.py
+-rw-r--r--   0        0        0     1228 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/usage_stats.py
+-rw-r--r--   0        0        0      974 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/text_gen/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     7630 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/uploading_asset_library.py
+-rw-r--r--   0        0        0     2799 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/util.py
+-rw-r--r--   0        0        0       74 2024-05-01 23:28:15.983270 octoai-1.0.0/src/octoai/version.py
+-rw-r--r--   0        0        0     5526 1970-01-01 00:00:00.000000 octoai-1.0.0/PKG-INFO
```

### Comparing `octoai-0.6.0/README.md` & `octoai-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/pyproject.toml` & `octoai-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "octoai"
-version = "0.6.0"
+version = "1.0.0"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "octoai", from = "src"}
 ]
```

### Comparing `octoai-0.6.0/src/octoai/asset_library/__init__.py` & `octoai-1.0.0/src/octoai/asset_library/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/client.py` & `octoai-1.0.0/src/octoai/asset_library/client.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/__init__.py` & `octoai-1.0.0/src/octoai/asset_library/types/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/asset.py` & `octoai-1.0.0/src/octoai/asset_library/types/asset.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/base_engine.py` & `octoai-1.0.0/src/octoai/asset_library/types/base_engine.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/checkpoint_data.py` & `octoai-1.0.0/src/octoai/asset_library/types/checkpoint_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/complete_asset_upload_response.py` & `octoai-1.0.0/src/octoai/asset_library/types/complete_asset_upload_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/create_asset_response.py` & `octoai-1.0.0/src/octoai/asset_library/types/create_asset_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/create_asset_response_transfer_api.py` & `octoai-1.0.0/src/octoai/asset_library/types/create_asset_response_transfer_api.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/data.py` & `octoai-1.0.0/src/octoai/asset_library/types/data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/delete_asset_response.py` & `octoai-1.0.0/src/octoai/asset_library/types/delete_asset_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/file_data.py` & `octoai-1.0.0/src/octoai/asset_library/types/file_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/http_validation_error.py` & `octoai-1.0.0/src/octoai/asset_library/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/latent_data.py` & `octoai-1.0.0/src/octoai/asset_library/types/latent_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/list_assets_response.py` & `octoai-1.0.0/src/octoai/asset_library/types/list_assets_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/lora_data.py` & `octoai-1.0.0/src/octoai/asset_library/types/lora_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/no_transfer_api.py` & `octoai-1.0.0/src/octoai/asset_library/types/no_transfer_api.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/presigned_url_transfer_api.py` & `octoai-1.0.0/src/octoai/asset_library/types/presigned_url_transfer_api.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/retrieve_asset_response.py` & `octoai-1.0.0/src/octoai/asset_library/types/retrieve_asset_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/retrieve_asset_response_transfer_api.py` & `octoai-1.0.0/src/octoai/asset_library/types/retrieve_asset_response_transfer_api.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/sts_transfer_api.py` & `octoai-1.0.0/src/octoai/asset_library/types/sts_transfer_api.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/textual_inversion_data.py` & `octoai-1.0.0/src/octoai/asset_library/types/textual_inversion_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/vae_data.py` & `octoai-1.0.0/src/octoai/asset_library/types/vae_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/asset_library/types/validation_error.py` & `octoai-1.0.0/src/octoai/asset_library/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/base_client.py` & `octoai-1.0.0/src/octoai/base_client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -65,16 +65,16 @@
             else httpx.Client(timeout=_defaulted_timeout, follow_redirects=follow_redirects)
             if follow_redirects is not None
             else httpx.Client(timeout=_defaulted_timeout),
             timeout=_defaulted_timeout,
         )
         self.asset_library = AssetLibraryClient(client_wrapper=self._client_wrapper)
         self.fine_tuning = FineTuningClient(client_wrapper=self._client_wrapper)
-        self.image_gen = ImageGenClient(client_wrapper=self._client_wrapper)
         self.text_gen = TextGenClient(client_wrapper=self._client_wrapper)
+        self.image_gen = ImageGenClient(client_wrapper=self._client_wrapper)
 
 
 class AsyncBaseOctoAI:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
     Parameters
@@ -125,9 +125,9 @@
             else httpx.AsyncClient(timeout=_defaulted_timeout, follow_redirects=follow_redirects)
             if follow_redirects is not None
             else httpx.AsyncClient(timeout=_defaulted_timeout),
             timeout=_defaulted_timeout,
         )
         self.asset_library = AsyncAssetLibraryClient(client_wrapper=self._client_wrapper)
         self.fine_tuning = AsyncFineTuningClient(client_wrapper=self._client_wrapper)
-        self.image_gen = AsyncImageGenClient(client_wrapper=self._client_wrapper)
         self.text_gen = AsyncTextGenClient(client_wrapper=self._client_wrapper)
+        self.image_gen = AsyncImageGenClient(client_wrapper=self._client_wrapper)
```

### Comparing `octoai-0.6.0/src/octoai/client.py` & `octoai-1.0.0/src/octoai/client.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/core/__init__.py` & `octoai-1.0.0/src/octoai/core/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/core/client_wrapper.py` & `octoai-1.0.0/src/octoai/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self._environment = environment
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "octoai",
-            "X-Fern-SDK-Version": "0.6.0",
+            "X-Fern-SDK-Version": "1.0.0",
         }
         api_key = self._get_api_key()
         if api_key is not None:
             headers["Authorization"] = f"Bearer {api_key}"
         return headers
 
     def _get_api_key(self) -> typing.Optional[str]:
```

### Comparing `octoai-0.6.0/src/octoai/core/datetime_utils.py` & `octoai-1.0.0/src/octoai/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/core/file.py` & `octoai-1.0.0/src/octoai/core/file.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/core/http_client.py` & `octoai-1.0.0/src/octoai/core/http_client.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/core/jsonable_encoder.py` & `octoai-1.0.0/src/octoai/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/core/request_options.py` & `octoai-1.0.0/src/octoai/core/request_options.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/environment.py` & `octoai-1.0.0/src/octoai/environment.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/fine_tuning/__init__.py` & `octoai-1.0.0/src/octoai/fine_tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/fine_tuning/client.py` & `octoai-1.0.0/src/octoai/fine_tuning/client.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/fine_tuning/types/__init__.py` & `octoai-1.0.0/src/octoai/fine_tuning/types/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/fine_tuning/types/base_engine.py` & `octoai-1.0.0/src/octoai/fine_tuning/types/base_engine.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/fine_tuning/types/details.py` & `octoai-1.0.0/src/octoai/fine_tuning/types/details.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/fine_tuning/types/http_validation_error.py` & `octoai-1.0.0/src/octoai/fine_tuning/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/fine_tuning/types/list_tunes_response.py` & `octoai-1.0.0/src/octoai/fine_tuning/types/list_tunes_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/fine_tuning/types/lora_tune.py` & `octoai-1.0.0/src/octoai/fine_tuning/types/lora_tune.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/fine_tuning/types/lora_tune_checkpoint.py` & `octoai-1.0.0/src/octoai/fine_tuning/types/lora_tune_checkpoint.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/fine_tuning/types/lora_tune_file.py` & `octoai-1.0.0/src/octoai/fine_tuning/types/lora_tune_file.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/fine_tuning/types/text_to_speech_latent_tune.py` & `octoai-1.0.0/src/octoai/fine_tuning/types/text_to_speech_latent_tune.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/fine_tuning/types/tune.py` & `octoai-1.0.0/src/octoai/fine_tuning/types/tune.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/fine_tuning/types/tune_details.py` & `octoai-1.0.0/src/octoai/fine_tuning/types/tune_details.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/fine_tuning/types/tune_result.py` & `octoai-1.0.0/src/octoai/fine_tuning/types/tune_result.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/fine_tuning/types/validation_error.py` & `octoai-1.0.0/src/octoai/fine_tuning/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/image_gen/__init__.py` & `octoai-1.0.0/src/octoai/image_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/image_gen/client.py` & `octoai-1.0.0/src/octoai/image_gen/client.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/image_gen/types/__init__.py` & `octoai-1.0.0/src/octoai/image_gen/types/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/image_gen/types/http_validation_error.py` & `octoai-1.0.0/src/octoai/image_gen/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/image_gen/types/image_generation.py` & `octoai-1.0.0/src/octoai/image_gen/types/image_generation.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/image_gen/types/image_generation_request.py` & `octoai-1.0.0/src/octoai/image_gen/types/image_generation_request.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/image_gen/types/image_generation_response.py` & `octoai-1.0.0/src/octoai/image_gen/types/image_generation_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/image_gen/types/scheduler.py` & `octoai-1.0.0/src/octoai/image_gen/types/scheduler.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/image_gen/types/sdxl_styles.py` & `octoai-1.0.0/src/octoai/image_gen/types/sdxl_styles.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/image_gen/types/validation_error.py` & `octoai-1.0.0/src/octoai/image_gen/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/image_gen/types/video_generation.py` & `octoai-1.0.0/src/octoai/image_gen/types/video_generation.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/image_gen/types/video_generation_response.py` & `octoai-1.0.0/src/octoai/image_gen/types/video_generation_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/__init__.py` & `octoai-1.0.0/src/octoai/text_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/client.py` & `octoai-1.0.0/src/octoai/text_gen/client.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/types/__init__.py` & `octoai-1.0.0/src/octoai/text_gen/types/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/types/chat_completion_choice.py` & `octoai-1.0.0/src/octoai/text_gen/types/chat_completion_choice.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/types/chat_completion_chunk.py` & `octoai-1.0.0/src/octoai/text_gen/types/chat_completion_chunk.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/types/chat_completion_chunk_choice.py` & `octoai-1.0.0/src/octoai/text_gen/types/chat_completion_chunk_choice.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/types/chat_completion_delta.py` & `octoai-1.0.0/src/octoai/text_gen/types/chat_completion_delta.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/types/chat_completion_request_ext.py` & `octoai-1.0.0/src/octoai/text_gen/types/chat_completion_request_ext.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/types/chat_completion_request_ext_vllm.py` & `octoai-1.0.0/src/octoai/text_gen/types/chat_completion_request_ext_vllm.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/types/chat_completion_response.py` & `octoai-1.0.0/src/octoai/text_gen/types/chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/types/chat_completion_response_format.py` & `octoai-1.0.0/src/octoai/text_gen/types/chat_completion_response_format.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/types/chat_fn_call.py` & `octoai-1.0.0/src/octoai/text_gen/types/chat_fn_call.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/types/chat_message.py` & `octoai-1.0.0/src/octoai/text_gen/types/chat_message.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/types/completion_choice.py` & `octoai-1.0.0/src/octoai/text_gen/types/completion_choice.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/types/completion_response.py` & `octoai-1.0.0/src/octoai/text_gen/types/completion_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/types/error_response.py` & `octoai-1.0.0/src/octoai/text_gen/types/error_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/types/function.py` & `octoai-1.0.0/src/octoai/text_gen/types/function.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/types/http_validation_error.py` & `octoai-1.0.0/src/octoai/text_gen/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/types/log_probs.py` & `octoai-1.0.0/src/octoai/text_gen/types/log_probs.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/types/usage_stats.py` & `octoai-1.0.0/src/octoai/text_gen/types/usage_stats.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/text_gen/types/validation_error.py` & `octoai-1.0.0/src/octoai/text_gen/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/uploading_asset_library.py` & `octoai-1.0.0/src/octoai/uploading_asset_library.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/src/octoai/util.py` & `octoai-1.0.0/src/octoai/util.py`

 * *Files identical despite different names*

### Comparing `octoai-0.6.0/PKG-INFO` & `octoai-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoai
-Version: 0.6.0
+Version: 1.0.0
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


# Comparing `tmp/aladdinsdk-0.0.1a4.post0.tar.gz` & `tmp/aladdinsdk-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aladdinsdk-0.0.1a4.post0.tar", last modified: Thu May  2 22:50:34 2024, max compression
+gzip compressed data, was "aladdinsdk-2.0.0a1.tar", last modified: Fri May  3 21:50:03 2024, max compression
```

## Comparing `aladdinsdk-0.0.1a4.post0.tar` & `aladdinsdk-2.0.0a1.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.537735 aladdinsdk-0.0.1a4.post0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    42553 2024-05-02 22:50:34.537735 aladdinsdk-0.0.1a4.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    41618 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.485736 aladdinsdk-0.0.1a4.post0/aladdinsdk/
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.485736 aladdinsdk-0.0.1a4.post0/aladdinsdk/adc/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/adc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21917 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/adc/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.485736 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26142 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.489735 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/codegen_allow_list.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.477736 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.477736 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.477736 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.477736 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.489735 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.489735 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30917 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api/default_token_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30281 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17107 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.489735 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/any.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/rpc_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/token_api_generate_authorization_url400_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_authorization_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_check_token_exists_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)    41125 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/swagger.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.477736 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.477736 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.477736 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.477736 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.493735 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.493735 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   123450 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api/default_train_journey_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30448 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17260 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.517735 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/any.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_region.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_train_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/expand_expand_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/rpc_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_journey_api_cancel_longrunning_operation_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_journey_api_get_longrunning_operation400_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_station_train_station_facilities_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_station_train_station_summary_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_train_summary_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_create_train_journeys_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_create_train_journeys_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_delete_train_journeys_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_delete_train_journeys_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_update_train_journeys_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_update_train_journeys_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_control_train_journey_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_create_train_journey_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_create_train_journey_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_delete_train_journey_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_filter_train_journeys_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_filter_train_journeys_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_follow_train_journey_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_list_train_journeys_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_longrunning_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_simulate_train_journey_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_train_journey.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_train_journey_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_update_train_journey_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_update_train_journey_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)   173990 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/swagger.json
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/api/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.517735 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.517735 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/authentication/adc.py
--rw-r--r--   0 runner    (1001) docker     (127)    23017 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/authentication/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.517735 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/authentication/basicauth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/authentication/basicauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/authentication/basicauth/basicauthutil.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.521735 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/authentication/oauth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/authentication/oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/authentication/oauth/oauth_token_cred_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/authentication/oauth/oauth_url_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/authentication/oauth/okta_sidecar_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.521735 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/blkutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/blkutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/blkutils/blkutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.521735 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/datatransformation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/datatransformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/datatransformation/json_to_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.525735 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/error/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/error/asdkerrors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/error/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.525735 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/error/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/error/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/error/handlers/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/error/handlers/adc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/error/handlers/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/error/handlers/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.529735 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/error/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/error/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/error/notifications/email_notifications_for_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.529735 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/exports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/exports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/exports/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/exports/export_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/exports/export_excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/exports/export_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/exports/export_pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.529735 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/exports/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/exports/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/exports/utils/data_parse_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/exports/utils/validate_file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/exports/utils/write_file_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.533735 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/metrics/domain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.533735 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/notifications/email_notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.533735 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/retry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/retry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/retry/adc_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/retry/api_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/retry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.533735 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/secrets/fsutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/common/secrets/keyringutil.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.533735 aladdinsdk-0.0.1a4.post0/aladdinsdk/config/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/config/asdkconf.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/config/internal_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/config/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.533735 aladdinsdk-0.0.1a4.post0/aladdinsdk/config/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/config/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24947 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk/config/utils/user_settings_file_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.537735 aladdinsdk-0.0.1a4.post0/aladdinsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42553 2024-05-02 22:50:34.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9706 2024-05-02 22:50:34.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 22:50:34.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-02 22:50:34.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-02 22:50:34.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 22:50:34.000000 aladdinsdk-0.0.1a4.post0/aladdinsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-02 22:50:34.541735 aladdinsdk-0.0.1a4.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:34.537735 aladdinsdk-0.0.1a4.post0/test/
--rw-r--r--   0 runner    (1001) docker     (127)    34511 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/test/test_adc.py
--rw-r--r--   0 runner    (1001) docker     (127)    44103 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    19299 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/test/test_common_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    16163 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/test/test_common_authentication_adc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15890 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/test/test_common_authentication_oauth_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/test/test_common_authentication_okta_sidecar_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/test/test_common_blkutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17941 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/test/test_common_datatransformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/test/test_common_datatransformation_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/test/test_common_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/test/test_common_error_notifications_email.py
--rw-r--r--   0 runner    (1001) docker     (127)    26531 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/test/test_common_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/test/test_common_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/test/test_common_notifications_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/test/test_common_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/test/test_common_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27929 2024-05-02 22:49:39.000000 aladdinsdk-0.0.1a4.post0/test/test_user_settings_file_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.433616 aladdinsdk-2.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    42547 2024-05-03 21:50:03.433616 aladdinsdk-2.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    41618 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.401616 aladdinsdk-2.0.0a1/aladdinsdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.401616 aladdinsdk-2.0.0a1/aladdinsdk/adc/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/adc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21917 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/adc/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.405616 aladdinsdk-2.0.0a1/aladdinsdk/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26142 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.405616 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/codegen_allow_list.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.393616 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.393616 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.393616 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.393616 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.405616 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.405616 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30917 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api/default_token_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30281 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17107 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.409616 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/any.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/rpc_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/token_api_generate_authorization_url400_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_authorization_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_check_token_exists_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41125 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/swagger.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.393616 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.393616 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.393616 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.393616 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.409616 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.409616 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   123450 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api/default_train_journey_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30448 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17260 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.417616 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/any.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_train_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/expand_expand_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/rpc_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_journey_api_cancel_longrunning_operation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_journey_api_get_longrunning_operation400_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_station_train_station_facilities_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_station_train_station_summary_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_train_summary_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_create_train_journeys_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_create_train_journeys_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_delete_train_journeys_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_delete_train_journeys_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_update_train_journeys_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_update_train_journeys_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_control_train_journey_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_create_train_journey_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_create_train_journey_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_delete_train_journey_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_filter_train_journeys_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_filter_train_journeys_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_follow_train_journey_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_list_train_journeys_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_longrunning_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_simulate_train_journey_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_train_journey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_train_journey_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_update_train_journey_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_update_train_journey_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)   173990 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/swagger.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/api/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.417616 aladdinsdk-2.0.0a1/aladdinsdk/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.417616 aladdinsdk-2.0.0a1/aladdinsdk/common/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/authentication/adc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23017 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/authentication/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.417616 aladdinsdk-2.0.0a1/aladdinsdk/common/authentication/basicauth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/authentication/basicauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/authentication/basicauth/basicauthutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.421616 aladdinsdk-2.0.0a1/aladdinsdk/common/authentication/oauth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/authentication/oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/authentication/oauth/oauth_token_cred_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/authentication/oauth/oauth_url_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/authentication/oauth/okta_sidecar_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.421616 aladdinsdk-2.0.0a1/aladdinsdk/common/blkutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/blkutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/blkutils/blkutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.421616 aladdinsdk-2.0.0a1/aladdinsdk/common/datatransformation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/datatransformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/datatransformation/json_to_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.421616 aladdinsdk-2.0.0a1/aladdinsdk/common/error/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/error/asdkerrors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/error/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.421616 aladdinsdk-2.0.0a1/aladdinsdk/common/error/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/error/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/error/handlers/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/error/handlers/adc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/error/handlers/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/error/handlers/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.421616 aladdinsdk-2.0.0a1/aladdinsdk/common/error/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/error/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/error/notifications/email_notifications_for_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.421616 aladdinsdk-2.0.0a1/aladdinsdk/common/exports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/exports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/exports/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/exports/export_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/exports/export_excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/exports/export_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/exports/export_pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.425616 aladdinsdk-2.0.0a1/aladdinsdk/common/exports/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/exports/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/exports/utils/data_parse_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/exports/utils/validate_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/exports/utils/write_file_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.425616 aladdinsdk-2.0.0a1/aladdinsdk/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/metrics/domain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.425616 aladdinsdk-2.0.0a1/aladdinsdk/common/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/notifications/email_notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.425616 aladdinsdk-2.0.0a1/aladdinsdk/common/retry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/retry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/retry/adc_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/retry/api_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/retry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.425616 aladdinsdk-2.0.0a1/aladdinsdk/common/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/secrets/fsutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/common/secrets/keyringutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.425616 aladdinsdk-2.0.0a1/aladdinsdk/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/config/asdkconf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/config/internal_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/config/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.429616 aladdinsdk-2.0.0a1/aladdinsdk/config/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/config/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24947 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/aladdinsdk/config/utils/user_settings_file_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.433616 aladdinsdk-2.0.0a1/aladdinsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42547 2024-05-03 21:50:03.000000 aladdinsdk-2.0.0a1/aladdinsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9706 2024-05-03 21:50:03.000000 aladdinsdk-2.0.0a1/aladdinsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 21:50:03.000000 aladdinsdk-2.0.0a1/aladdinsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-03 21:50:03.000000 aladdinsdk-2.0.0a1/aladdinsdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-03 21:50:03.000000 aladdinsdk-2.0.0a1/aladdinsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 21:50:03.000000 aladdinsdk-2.0.0a1/aladdinsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-03 21:50:03.433616 aladdinsdk-2.0.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:50:03.429616 aladdinsdk-2.0.0a1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    34511 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/test/test_adc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44103 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19299 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/test/test_common_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16163 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/test/test_common_authentication_adc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15890 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/test/test_common_authentication_oauth_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/test/test_common_authentication_okta_sidecar_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/test/test_common_blkutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17941 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/test/test_common_datatransformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/test/test_common_datatransformation_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/test/test_common_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/test/test_common_error_notifications_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26531 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/test/test_common_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/test/test_common_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/test/test_common_notifications_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/test/test_common_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/test/test_common_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27929 2024-05-03 21:49:12.000000 aladdinsdk-2.0.0a1/test/test_user_settings_file_util.py
```

### Comparing `aladdinsdk-0.0.1a4.post0/LICENSE` & `aladdinsdk-2.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/PKG-INFO` & `aladdinsdk-2.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aladdinsdk
-Version: 0.0.1a4.post0
+Version: 2.0.0a1
 Summary: AladdinSDK
 Author-email: Vedant Naik <naik.vedant@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `aladdinsdk-0.0.1a4.post0/README.md` & `aladdinsdk-2.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/__init__.py` & `aladdinsdk-2.0.0a1/aladdinsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/adc/client.py` & `aladdinsdk-2.0.0a1/aladdinsdk/adc/client.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/client.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/client.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/codegen_allow_list.yaml` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/codegen_allow_list.yaml`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/__init__.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api/default_token_api.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api/default_token_api.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api_client.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api_client.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api_response.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/configuration.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/configuration.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/exceptions.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/exceptions.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/__init__.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/any.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/any.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/rpc_status.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/rpc_status.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/token_api_generate_authorization_url400_response.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/token_api_generate_authorization_url400_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_authorization_url.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_authorization_url.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_check_token_exists_response.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_check_token_exists_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_token.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_token.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/rest.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/rest.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/swagger.json` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/swagger.json`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/__init__.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api/default_train_journey_api.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api/default_train_journey_api.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api_client.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api_client.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api_response.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/configuration.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/configuration.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/exceptions.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/exceptions.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/__init__.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/any.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/any.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_operator.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_operator.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_region.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_region.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_size.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_size.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_train_type.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_train_type.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/expand_expand_mask.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/expand_expand_mask.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/rpc_status.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/rpc_status.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_journey_api_cancel_longrunning_operation_request.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_journey_api_cancel_longrunning_operation_request.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_journey_api_get_longrunning_operation400_response.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_journey_api_get_longrunning_operation400_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_station_train_station_facilities_slice.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_station_train_station_facilities_slice.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_station_train_station_summary_slice.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_station_train_station_summary_slice.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_train_summary_slice.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_train_summary_slice.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_create_train_journeys_request.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_create_train_journeys_request.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_create_train_journeys_response.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_create_train_journeys_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_delete_train_journeys_request.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_delete_train_journeys_request.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_delete_train_journeys_response.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_delete_train_journeys_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_update_train_journeys_request.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_update_train_journeys_request.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_update_train_journeys_response.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_update_train_journeys_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_control_train_journey_response.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_control_train_journey_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_create_train_journey_request.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_create_train_journey_request.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_create_train_journey_result.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_create_train_journey_result.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_delete_train_journey_result.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_delete_train_journey_result.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_filter_train_journeys_request.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_filter_train_journeys_request.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_filter_train_journeys_response.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_filter_train_journeys_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_follow_train_journey_response.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_follow_train_journey_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_list_train_journeys_response.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_list_train_journeys_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_longrunning_operation.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_longrunning_operation.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_simulate_train_journey_response.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_simulate_train_journey_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_train_journey.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_train_journey.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_train_journey_query.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_train_journey_query.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_update_train_journey_request.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_update_train_journey_request.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_update_train_journey_result.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_update_train_journey_result.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/rest.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/rest.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/swagger.json` & `aladdinsdk-2.0.0a1/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/swagger.json`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/api/registry.py` & `aladdinsdk-2.0.0a1/aladdinsdk/api/registry.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/authentication/adc.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/authentication/adc.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/authentication/api.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/authentication/api.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/authentication/basicauth/basicauthutil.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/authentication/basicauth/basicauthutil.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/authentication/oauth/oauth_token_cred_client.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/authentication/oauth/oauth_token_cred_client.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/authentication/oauth/oauth_url_client.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/authentication/oauth/oauth_url_client.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/authentication/oauth/okta_sidecar_client.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/authentication/oauth/okta_sidecar_client.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/blkutils/blkutils.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/blkutils/blkutils.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/datatransformation/json_to_pandas.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/datatransformation/json_to_pandas.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/error/asdkerrors.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/error/asdkerrors.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/error/handler.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/error/handler.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/error/handlers/abstract.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/error/handlers/abstract.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/error/handlers/adc.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/error/handlers/adc.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/error/handlers/api.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/error/handlers/api.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/error/handlers/internal.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/error/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/error/notifications/email_notifications_for_errors.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/error/notifications/email_notifications_for_errors.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/exports/export.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/exports/export.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/exports/export_csv.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/exports/export_csv.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/exports/export_excel.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/exports/export_excel.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/exports/export_json.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/exports/export_json.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/exports/export_pickle.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/exports/export_pickle.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/exports/utils/data_parse_util.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/exports/utils/data_parse_util.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/exports/utils/validate_file_util.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/exports/utils/validate_file_util.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/exports/utils/write_file_util.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/exports/utils/write_file_util.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/metrics/domain.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/metrics/domain.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/notifications/email_notifications.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/notifications/email_notifications.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/retry/adc_retry.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/retry/adc_retry.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/retry/api_retry.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/retry/api_retry.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/retry/utils.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/retry/utils.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/secrets/fsutil.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/secrets/fsutil.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/common/secrets/keyringutil.py` & `aladdinsdk-2.0.0a1/aladdinsdk/common/secrets/keyringutil.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/config/asdkconf.py` & `aladdinsdk-2.0.0a1/aladdinsdk/config/asdkconf.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/config/internal_settings.py` & `aladdinsdk-2.0.0a1/aladdinsdk/config/internal_settings.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/config/user_settings.py` & `aladdinsdk-2.0.0a1/aladdinsdk/config/user_settings.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk/config/utils/user_settings_file_util.py` & `aladdinsdk-2.0.0a1/aladdinsdk/config/utils/user_settings_file_util.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk.egg-info/PKG-INFO` & `aladdinsdk-2.0.0a1/aladdinsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aladdinsdk
-Version: 0.0.1a4.post0
+Version: 2.0.0a1
 Summary: AladdinSDK
 Author-email: Vedant Naik <naik.vedant@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `aladdinsdk-0.0.1a4.post0/aladdinsdk.egg-info/SOURCES.txt` & `aladdinsdk-2.0.0a1/aladdinsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/pyproject.toml` & `aladdinsdk-2.0.0a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "setuptools-git-versioning"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools-git-versioning]
 enabled = true
-dev_template = "{tag}.post{ccount}"
-dirty_template = "{tag}.post{ccount}"
+dev_template = "{tag}"
+dirty_template = "{tag}"
 
 [project]
 name = "aladdinsdk"
 authors = [
   { name="Vedant Naik", email="naik.vedant@gmail.com" },
 ]
 description = "AladdinSDK"
```

### Comparing `aladdinsdk-0.0.1a4.post0/test/test_adc.py` & `aladdinsdk-2.0.0a1/test/test_adc.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/test/test_api.py` & `aladdinsdk-2.0.0a1/test/test_api.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/test/test_common_authentication.py` & `aladdinsdk-2.0.0a1/test/test_common_authentication.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/test/test_common_authentication_adc.py` & `aladdinsdk-2.0.0a1/test/test_common_authentication_adc.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/test/test_common_authentication_oauth_client.py` & `aladdinsdk-2.0.0a1/test/test_common_authentication_oauth_client.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/test/test_common_authentication_okta_sidecar_client.py` & `aladdinsdk-2.0.0a1/test/test_common_authentication_okta_sidecar_client.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/test/test_common_blkutils.py` & `aladdinsdk-2.0.0a1/test/test_common_blkutils.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/test/test_common_datatransformation.py` & `aladdinsdk-2.0.0a1/test/test_common_datatransformation.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/test/test_common_datatransformation_options.py` & `aladdinsdk-2.0.0a1/test/test_common_datatransformation_options.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/test/test_common_error_handling.py` & `aladdinsdk-2.0.0a1/test/test_common_error_handling.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/test/test_common_error_notifications_email.py` & `aladdinsdk-2.0.0a1/test/test_common_error_notifications_email.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/test/test_common_exports.py` & `aladdinsdk-2.0.0a1/test/test_common_exports.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/test/test_common_metrics.py` & `aladdinsdk-2.0.0a1/test/test_common_metrics.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/test/test_common_notifications_email.py` & `aladdinsdk-2.0.0a1/test/test_common_notifications_email.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/test/test_common_retry.py` & `aladdinsdk-2.0.0a1/test/test_common_retry.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/test/test_common_secrets.py` & `aladdinsdk-2.0.0a1/test/test_common_secrets.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/test/test_config.py` & `aladdinsdk-2.0.0a1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a4.post0/test/test_user_settings_file_util.py` & `aladdinsdk-2.0.0a1/test/test_user_settings_file_util.py`

 * *Files identical despite different names*


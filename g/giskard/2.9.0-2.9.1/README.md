# Comparing `tmp/giskard-2.9.0.tar.gz` & `tmp/giskard-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giskard-2.9.0.tar", last modified: Mon Apr  8 14:07:36 2024, max compression
+gzip compressed data, was "giskard-2.9.1.tar", last modified: Tue Apr  9 11:06:06 2024, max compression
```

## Comparing `giskard-2.9.0.tar` & `giskard-2.9.1.tar`

### file list

```diff
@@ -1,338 +1,338 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.594685 giskard-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-04-08 14:07:05.000000 giskard-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-08 14:07:36.594685 giskard-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-04-08 14:07:05.000000 giskard-2.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.554685 giskard-2.9.0/giskard/
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.554685 giskard-2.9.0/giskard/client/
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/client/dtos.py
--rw-r--r--   0 runner    (1001) docker     (127)    19627 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/client/giskard_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/client/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/client/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/client/python_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.554685 giskard-2.9.0/giskard/commands/
--rw-r--r--   0 runner    (1001) docker     (127)    18864 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/commands/cli_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/commands/cli_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.554685 giskard-2.9.0/giskard/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17335 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/core/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/core/dataset_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/core/kwargs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14327 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/core/model_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/core/savable.py
--rw-r--r--   0 runner    (1001) docker     (127)    36960 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/core/suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/core/test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/core/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.554685 giskard-2.9.0/giskard/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.554685 giskard-2.9.0/giskard/datasets/base/
--rw-r--r--   0 runner    (1001) docker     (127)    31942 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/datasets/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.558686 giskard-2.9.0/giskard/datasets/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/datasets/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/datasets/metadata/indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/datasets/metadata/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/datasets/metadata/text_metadata_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.558686 giskard-2.9.0/giskard/demo/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/demo/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/demo/llm_ipcc_climate_change.py
--rw-r--r--   0 runner    (1001) docker     (127)    60302 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/demo/titanic.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/demo/titanic_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.558686 giskard-2.9.0/giskard/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/exceptions/IllegalArgumentError.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/exceptions/giskard_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.558686 giskard-2.9.0/giskard/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/functions/slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/functions/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.558686 giskard-2.9.0/giskard/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/integrations/avid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.558686 giskard-2.9.0/giskard/integrations/mlflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/integrations/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/integrations/mlflow/evaluation_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/integrations/mlflow/giskard_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/integrations/mlflow/giskard_evaluator_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.558686 giskard-2.9.0/giskard/integrations/wandb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/integrations/wandb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/integrations/wandb/wandb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.558686 giskard-2.9.0/giskard/llm/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.562686 giskard-2.9.0/giskard/llm/client/
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/client/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/client/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/client/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.562686 giskard-2.9.0/giskard/llm/evaluators/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/evaluators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/evaluators/coherency.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/evaluators/correctness.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/evaluators/plausibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/evaluators/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/evaluators/string_matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.562686 giskard-2.9.0/giskard/llm/generators/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/generators/adversarial.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/generators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/generators/implausible.py
--rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/generators/sycophancy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.562686 giskard-2.9.0/giskard/llm/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/loaders/prompt_injections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.562686 giskard-2.9.0/giskard/ml_worker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.562686 giskard-2.9.0/giskard/ml_worker/bridge/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/bridge/data_encryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/bridge/error.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/bridge/service_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/ml_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.562686 giskard-2.9.0/giskard/ml_worker/stomp/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/stomp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8374 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/stomp/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/stomp/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/stomp/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/stomp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.562686 giskard-2.9.0/giskard/ml_worker/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/utils/network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.566686 giskard-2.9.0/giskard/ml_worker/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/websocket/action.py
--rw-r--r--   0 runner    (1001) docker     (127)    30302 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/websocket/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)    14327 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/websocket/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.566686 giskard-2.9.0/giskard/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/_precooked.py
--rw-r--r--   0 runner    (1001) docker     (127)    11544 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/automodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.566686 giskard-2.9.0/giskard/models/base/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25786 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/base/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/base/model_prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/base/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    14149 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/base/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.566686 giskard-2.9.0/giskard/models/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/cache/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/catboost.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    10285 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/model_explanation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/shap_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/path_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.566686 giskard-2.9.0/giskard/push/
--rw-r--r--   0 runner    (1001) docker     (127)    18662 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/push/contribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/push/perturbation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/push/prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.570685 giskard-2.9.0/giskard/push/push_test_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)    10518 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/push/push_test_catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/push/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.570685 giskard-2.9.0/giskard/rag/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11505 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/knowledge_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/knowledge_base_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.570685 giskard-2.9.0/giskard/rag/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/metrics/correctness.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/metrics/ragas_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.570685 giskard-2.9.0/giskard/rag/question_generators/
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/complex_questions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/conversational_questions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/distracting_questions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/double_questions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/oos_questions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/question_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/simple_questions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/situational_questions.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/recommendation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16390 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/testset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/testset_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.574685 giskard-2.9.0/giskard/registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/registry/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/registry/decorators_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/registry/giskard_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/registry/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/registry/slicing_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/registry/transformation_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/registry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.574685 giskard-2.9.0/giskard/scanner/
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.574685 giskard-2.9.0/giskard/scanner/calibration/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/calibration/overconfidence_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/calibration/underconfidence_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.574685 giskard-2.9.0/giskard/scanner/common/
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/common/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/common/loss_based_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.574685 giskard-2.9.0/giskard/scanner/correlation/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/correlation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/correlation/spurious_correlation_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.574685 giskard-2.9.0/giskard/scanner/data_leakage/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/data_leakage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/data_leakage/data_leakage_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    14180 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/issues.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.578685 giskard-2.9.0/giskard/scanner/llm/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/llm_basic_sycophancy_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/llm_chars_injection_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/llm_faithfulness_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/llm_harmful_content_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/llm_implausible_output_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/llm_information_disclosure_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/llm_output_formatting_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/llm_prompt_injection_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/llm_stereotypes_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.578685 giskard-2.9.0/giskard/scanner/performance/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/performance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/performance/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15765 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/performance/performance_bias_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    11476 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.578685 giskard-2.9.0/giskard/scanner/robustness/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/robustness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/robustness/base_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)   497222 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/robustness/entity_swap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/robustness/ethical_bias_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    19432 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/robustness/nationalities.json
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/robustness/text_perturbation_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    15828 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/robustness/text_transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.578685 giskard-2.9.0/giskard/scanner/stochasticity/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/stochasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/stochasticity/stochasticity_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.550686 giskard-2.9.0/giskard/scanner/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.578685 giskard-2.9.0/giskard/scanner/templates/static/
--rw-r--r--   0 runner    (1001) docker     (127)    19904 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/templates/static/external.js
--rw-r--r--   0 runner    (1001) docker     (127)    65083 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/templates/static/internal.js
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/templates/static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.582685 giskard-2.9.0/giskard/slicing/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/bruteforce_slicer.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/category_slicer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/multiscale_slicer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/opt_slicer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10625 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/slice_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/stop_words.py
--rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/text_slicer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/tree_slicer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.582685 giskard-2.9.0/giskard/testing/
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.582685 giskard-2.9.0/giskard/testing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7480 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13877 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/data_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/debug_slicing_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    36651 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/drift.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.582685 giskard-2.9.0/giskard/testing/tests/llm/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/llm/correctness.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/llm/ground_truth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/llm/hallucination.py
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/llm/injections.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/llm/output_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)    33910 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/metamorphic.py
--rw-r--r--   0 runner    (1001) docker     (127)    32522 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)    22600 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/statistic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.582685 giskard-2.9.0/giskard/testing/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/utils/stat_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.586686 giskard-2.9.0/giskard/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/utils/analytics_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/utils/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/utils/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/utils/environment_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/utils/sentry.py
--rw-r--r--   0 runner    (1001) docker     (127)    17016 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/utils/worker_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.586686 giskard-2.9.0/giskard/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/custom_jinja.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.550686 giskard-2.9.0/giskard/visualization/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.586686 giskard-2.9.0/giskard/visualization/templates/rag_report/
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/rag_report/rag_report.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.586686 giskard-2.9.0/giskard/visualization/templates/rag_report/static/
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/rag_report/static/internal.js
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/rag_report/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.550686 giskard-2.9.0/giskard/visualization/templates/scan_report/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.586686 giskard-2.9.0/giskard/visualization/templates/scan_report/html/
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/html/_code_snippet.html
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/html/_issue.html
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/html/_issues_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/html/_main_content.html
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/html/_tab_header.html
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/html/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/html/full.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.586686 giskard-2.9.0/giskard/visualization/templates/scan_report/html/static/
--rw-r--r--   0 runner    (1001) docker     (127)    19904 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/html/static/external.js
--rw-r--r--   0 runner    (1001) docker     (127)    65083 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/html/static/internal.js
--rw-r--r--   0 runner    (1001) docker     (127)    13753 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/html/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.586686 giskard-2.9.0/giskard/visualization/templates/scan_report/markdown/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/markdown/github.md
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/markdown/huggingface.md
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/markdown/summary.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.586686 giskard-2.9.0/giskard/visualization/templates/suite_results/
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/suite_results/_suite_results_cards.html
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/suite_results/_suite_results_header.html
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/suite_results/suite_results.html
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.590685 giskard-2.9.0/giskard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-08 14:07:36.000000 giskard-2.9.0/giskard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10058 2024-04-08 14:07:36.000000 giskard-2.9.0/giskard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:07:36.000000 giskard-2.9.0/giskard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-08 14:07:36.000000 giskard-2.9.0/giskard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-08 14:07:36.000000 giskard-2.9.0/giskard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 14:07:36.000000 giskard-2.9.0/giskard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-04-08 14:07:17.000000 giskard-2.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 14:07:36.594685 giskard-2.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.590685 giskard-2.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_artifact_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_custom_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14783 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_data_drift.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_data_processing_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_import_giskard.py
--rw-r--r--   0 runner    (1001) docker     (127)    10771 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_metamorphic_direction.py
--rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_metamorphic_invariance.py
--rw-r--r--   0 runner    (1001) docker     (127)    14070 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_performance.py
--rw-r--r--   0 runner    (1001) docker     (127)    15728 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_programmatic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_project_uploads.py
--rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_push.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_statistical.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_worker_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.568241 giskard-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-04-09 11:05:26.000000 giskard-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-09 11:06:06.568241 giskard-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-04-09 11:05:26.000000 giskard-2.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.524241 giskard-2.9.1/giskard/
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.528241 giskard-2.9.1/giskard/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/client/dtos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19694 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/client/giskard_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/client/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/client/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/client/python_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.528241 giskard-2.9.1/giskard/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)    18864 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/commands/cli_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/commands/cli_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.528241 giskard-2.9.1/giskard/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17335 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/core/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/core/dataset_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/core/kwargs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14327 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/core/model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/core/savable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36960 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/core/suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/core/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/core/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.528241 giskard-2.9.1/giskard/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.528241 giskard-2.9.1/giskard/datasets/base/
+-rw-r--r--   0 runner    (1001) docker     (127)    31942 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/datasets/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.528241 giskard-2.9.1/giskard/datasets/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/datasets/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/datasets/metadata/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/datasets/metadata/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/datasets/metadata/text_metadata_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.532241 giskard-2.9.1/giskard/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/demo/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/demo/llm_ipcc_climate_change.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60302 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/demo/titanic.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/demo/titanic_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.532241 giskard-2.9.1/giskard/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/exceptions/IllegalArgumentError.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/exceptions/giskard_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.532241 giskard-2.9.1/giskard/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/functions/slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/functions/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.532241 giskard-2.9.1/giskard/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/integrations/avid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.532241 giskard-2.9.1/giskard/integrations/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/integrations/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/integrations/mlflow/evaluation_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/integrations/mlflow/giskard_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/integrations/mlflow/giskard_evaluator_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.532241 giskard-2.9.1/giskard/integrations/wandb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/integrations/wandb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/integrations/wandb/wandb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.532241 giskard-2.9.1/giskard/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.532241 giskard-2.9.1/giskard/llm/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/client/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/client/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.536241 giskard-2.9.1/giskard/llm/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/evaluators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/evaluators/coherency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/evaluators/correctness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/evaluators/plausibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/evaluators/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/evaluators/string_matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.536241 giskard-2.9.1/giskard/llm/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/generators/adversarial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/generators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/generators/implausible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/generators/sycophancy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.536241 giskard-2.9.1/giskard/llm/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/loaders/prompt_injections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/llm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.536241 giskard-2.9.1/giskard/ml_worker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/ml_worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.536241 giskard-2.9.1/giskard/ml_worker/bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/ml_worker/bridge/data_encryptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/ml_worker/bridge/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/ml_worker/bridge/service_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/ml_worker/ml_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.536241 giskard-2.9.1/giskard/ml_worker/stomp/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/ml_worker/stomp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8374 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/ml_worker/stomp/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/ml_worker/stomp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/ml_worker/stomp/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/ml_worker/stomp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.536241 giskard-2.9.1/giskard/ml_worker/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/ml_worker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/ml_worker/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/ml_worker/utils/network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.536241 giskard-2.9.1/giskard/ml_worker/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/ml_worker/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/ml_worker/websocket/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30302 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/ml_worker/websocket/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14327 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/ml_worker/websocket/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.540241 giskard-2.9.1/giskard/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/models/_precooked.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11544 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/models/automodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.540241 giskard-2.9.1/giskard/models/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25786 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/models/base/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/models/base/model_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/models/base/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14149 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/models/base/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.540241 giskard-2.9.1/giskard/models/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/models/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/models/cache/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/models/catboost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/models/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10285 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/models/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/models/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/models/model_explanation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/models/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/models/shap_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/models/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/models/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/path_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.540241 giskard-2.9.1/giskard/push/
+-rw-r--r--   0 runner    (1001) docker     (127)    18662 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/push/contribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/push/perturbation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/push/prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.540241 giskard-2.9.1/giskard/push/push_test_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)    10518 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/push/push_test_catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/push/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.544241 giskard-2.9.1/giskard/rag/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11505 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/knowledge_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/knowledge_base_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.544241 giskard-2.9.1/giskard/rag/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/metrics/correctness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/metrics/ragas_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.544241 giskard-2.9.1/giskard/rag/question_generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/question_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/question_generators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/question_generators/complex_questions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/question_generators/conversational_questions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/question_generators/distracting_questions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/question_generators/double_questions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/question_generators/oos_questions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/question_generators/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/question_generators/question_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/question_generators/simple_questions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/question_generators/situational_questions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/question_generators/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16390 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/testset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/rag/testset_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.544241 giskard-2.9.1/giskard/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/registry/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/registry/decorators_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/registry/giskard_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/registry/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/registry/slicing_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/registry/transformation_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/registry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.548241 giskard-2.9.1/giskard/scanner/
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.548241 giskard-2.9.1/giskard/scanner/calibration/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/calibration/overconfidence_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/calibration/underconfidence_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.548241 giskard-2.9.1/giskard/scanner/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/common/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/common/loss_based_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.548241 giskard-2.9.1/giskard/scanner/correlation/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/correlation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/correlation/spurious_correlation_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.548241 giskard-2.9.1/giskard/scanner/data_leakage/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/data_leakage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/data_leakage/data_leakage_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14180 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/issues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.548241 giskard-2.9.1/giskard/scanner/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/llm/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/llm/llm_basic_sycophancy_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/llm/llm_chars_injection_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/llm/llm_faithfulness_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/llm/llm_harmful_content_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/llm/llm_implausible_output_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/llm/llm_information_disclosure_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/llm/llm_output_formatting_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/llm/llm_prompt_injection_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/llm/llm_stereotypes_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.552241 giskard-2.9.1/giskard/scanner/performance/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/performance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/performance/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15765 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/performance/performance_bias_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11476 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.552241 giskard-2.9.1/giskard/scanner/robustness/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/robustness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/robustness/base_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)   497222 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/robustness/entity_swap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/robustness/ethical_bias_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19432 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/robustness/nationalities.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/robustness/text_perturbation_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15828 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/robustness/text_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.552241 giskard-2.9.1/giskard/scanner/stochasticity/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/stochasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/stochasticity/stochasticity_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.524241 giskard-2.9.1/giskard/scanner/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.552241 giskard-2.9.1/giskard/scanner/templates/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    19904 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/templates/static/external.js
+-rw-r--r--   0 runner    (1001) docker     (127)    65083 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/templates/static/internal.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/scanner/templates/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.556241 giskard-2.9.1/giskard/slicing/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/slicing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/slicing/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/slicing/bruteforce_slicer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/slicing/category_slicer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/slicing/multiscale_slicer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/slicing/opt_slicer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10625 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/slicing/slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/slicing/slice_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/slicing/stop_words.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/slicing/text_slicer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/slicing/tree_slicer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/slicing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.556241 giskard-2.9.1/giskard/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.556241 giskard-2.9.1/giskard/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/testing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7480 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/testing/tests/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13877 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/testing/tests/data_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/testing/tests/debug_slicing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36651 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/testing/tests/drift.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.556241 giskard-2.9.1/giskard/testing/tests/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/testing/tests/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/testing/tests/llm/correctness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/testing/tests/llm/ground_truth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/testing/tests/llm/hallucination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/testing/tests/llm/injections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/testing/tests/llm/output_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33910 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/testing/tests/metamorphic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32522 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/testing/tests/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22600 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/testing/tests/statistic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.556241 giskard-2.9.1/giskard/testing/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/testing/utils/stat_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/testing/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.560241 giskard-2.9.1/giskard/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/utils/analytics_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/utils/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/utils/environment_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/utils/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17016 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/utils/worker_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.560241 giskard-2.9.1/giskard/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/custom_jinja.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.524241 giskard-2.9.1/giskard/visualization/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.560241 giskard-2.9.1/giskard/visualization/templates/rag_report/
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/templates/rag_report/rag_report.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.560241 giskard-2.9.1/giskard/visualization/templates/rag_report/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/templates/rag_report/static/internal.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/templates/rag_report/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.524241 giskard-2.9.1/giskard/visualization/templates/scan_report/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.560241 giskard-2.9.1/giskard/visualization/templates/scan_report/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/templates/scan_report/html/_code_snippet.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/templates/scan_report/html/_issue.html
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/templates/scan_report/html/_issues_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/templates/scan_report/html/_main_content.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/templates/scan_report/html/_tab_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/templates/scan_report/html/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/templates/scan_report/html/full.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.560241 giskard-2.9.1/giskard/visualization/templates/scan_report/html/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    19904 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/templates/scan_report/html/static/external.js
+-rw-r--r--   0 runner    (1001) docker     (127)    65083 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/templates/scan_report/html/static/internal.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13753 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/templates/scan_report/html/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.560241 giskard-2.9.1/giskard/visualization/templates/scan_report/markdown/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/templates/scan_report/markdown/github.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/templates/scan_report/markdown/huggingface.md
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/templates/scan_report/markdown/summary.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.560241 giskard-2.9.1/giskard/visualization/templates/suite_results/
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/templates/suite_results/_suite_results_cards.html
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/templates/suite_results/_suite_results_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/templates/suite_results/suite_results.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-09 11:05:26.000000 giskard-2.9.1/giskard/visualization/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.564241 giskard-2.9.1/giskard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-09 11:06:06.000000 giskard-2.9.1/giskard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10058 2024-04-09 11:06:06.000000 giskard-2.9.1/giskard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:06:06.000000 giskard-2.9.1/giskard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-09 11:06:06.000000 giskard-2.9.1/giskard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-09 11:06:06.000000 giskard-2.9.1/giskard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 11:06:06.000000 giskard-2.9.1/giskard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-04-09 11:05:41.000000 giskard-2.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:06:06.568241 giskard-2.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:06.564241 giskard-2.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-04-09 11:05:26.000000 giskard-2.9.1/tests/test_artifact_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-09 11:05:26.000000 giskard-2.9.1/tests/test_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14783 2024-04-09 11:05:26.000000 giskard-2.9.1/tests/test_data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-09 11:05:26.000000 giskard-2.9.1/tests/test_data_processing_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-04-09 11:05:26.000000 giskard-2.9.1/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-09 11:05:26.000000 giskard-2.9.1/tests/test_import_giskard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10771 2024-04-09 11:05:26.000000 giskard-2.9.1/tests/test_metamorphic_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-04-09 11:05:26.000000 giskard-2.9.1/tests/test_metamorphic_invariance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14070 2024-04-09 11:05:26.000000 giskard-2.9.1/tests/test_performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15728 2024-04-09 11:05:26.000000 giskard-2.9.1/tests/test_programmatic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-09 11:05:26.000000 giskard-2.9.1/tests/test_project_uploads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-04-09 11:05:26.000000 giskard-2.9.1/tests/test_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-09 11:05:26.000000 giskard-2.9.1/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-09 11:05:26.000000 giskard-2.9.1/tests/test_statistical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-09 11:05:26.000000 giskard-2.9.1/tests/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-04-09 11:05:26.000000 giskard-2.9.1/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-09 11:05:26.000000 giskard-2.9.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-04-09 11:05:26.000000 giskard-2.9.1/tests/test_worker_pool.py
```

### Comparing `giskard-2.9.0/LICENSE` & `giskard-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/PKG-INFO` & `giskard-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giskard
-Version: 2.9.0
+Version: 2.9.1
 Summary: The testing framework dedicated to ML models, from tabular to LLMs
 Author-email: Giskard AI <hello@giskard.ai>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://giskard.ai
 Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues
 Project-URL: Documentation, https://docs.giskard.ai/
```

### Comparing `giskard-2.9.0/README.md` & `giskard-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/__init__.py` & `giskard-2.9.1/giskard/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/cli.py` & `giskard-2.9.1/giskard/cli.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/cli_utils.py` & `giskard-2.9.1/giskard/cli_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/client/dtos.py` & `giskard-2.9.1/giskard/client/dtos.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/client/giskard_client.py` & `giskard-2.9.1/giskard/client/giskard_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,21 +134,22 @@
 
     # Java, js, h2 and postgres use UTF-16 surrogate pairs to calculate str length while python count characters
     if original_len > len(json[field]):
         logger.warning(f"Field '{field} exceeded the limit of {limit} characters and has been truncated")
 
 
 class GiskardClient:
-    def __init__(self, url: str, key: str, hf_token: str = None):
+    def __init__(self, url: str, key: str, hf_token: str = None, verify_ssl: bool = True):
         self.host_url = url
         self.key = key
         self.hf_token = hf_token
         base_url = urljoin(url, "/api/v2/")
 
         self._session = sessions.BaseUrlSession(base_url=base_url)
+        self._session.verify = verify_ssl
 
         adapter = ErrorHandlingAdapter()
 
         self._session.mount(url, adapter)
 
         self._session.auth = BearerAuth(key)
```

### Comparing `giskard-2.9.0/giskard/client/io_utils.py` & `giskard-2.9.1/giskard/client/io_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/client/project.py` & `giskard-2.9.1/giskard/client/project.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/client/python_utils.py` & `giskard-2.9.1/giskard/client/python_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/commands/cli_hub.py` & `giskard-2.9.1/giskard/commands/cli_hub.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/commands/cli_worker.py` & `giskard-2.9.1/giskard/commands/cli_worker.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/core/core.py` & `giskard-2.9.1/giskard/core/core.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/core/dataset_validation.py` & `giskard-2.9.1/giskard/core/dataset_validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/core/errors.py` & `giskard-2.9.1/giskard/core/errors.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/core/kwargs_utils.py` & `giskard-2.9.1/giskard/core/kwargs_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/core/model_validation.py` & `giskard-2.9.1/giskard/core/model_validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/core/savable.py` & `giskard-2.9.1/giskard/core/savable.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/core/suite.py` & `giskard-2.9.1/giskard/core/suite.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/core/test_result.py` & `giskard-2.9.1/giskard/core/test_result.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/core/validation.py` & `giskard-2.9.1/giskard/core/validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/datasets/__init__.py` & `giskard-2.9.1/giskard/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/datasets/base/__init__.py` & `giskard-2.9.1/giskard/datasets/base/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/datasets/metadata/indexing.py` & `giskard-2.9.1/giskard/datasets/metadata/indexing.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/datasets/metadata/registry.py` & `giskard-2.9.1/giskard/datasets/metadata/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/datasets/metadata/text_metadata_provider.py` & `giskard-2.9.1/giskard/datasets/metadata/text_metadata_provider.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/demo/__init__.py` & `giskard-2.9.1/giskard/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/demo/linear_regression.py` & `giskard-2.9.1/giskard/demo/linear_regression.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/demo/llm_ipcc_climate_change.py` & `giskard-2.9.1/giskard/demo/llm_ipcc_climate_change.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/demo/titanic.csv` & `giskard-2.9.1/giskard/demo/titanic.csv`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/demo/titanic_classification.py` & `giskard-2.9.1/giskard/demo/titanic_classification.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/exceptions/giskard_exception.py` & `giskard-2.9.1/giskard/exceptions/giskard_exception.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/functions/slicing.py` & `giskard-2.9.1/giskard/functions/slicing.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/functions/transformation.py` & `giskard-2.9.1/giskard/functions/transformation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/integrations/avid.py` & `giskard-2.9.1/giskard/integrations/avid.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/integrations/mlflow/evaluation_artifacts.py` & `giskard-2.9.1/giskard/integrations/mlflow/evaluation_artifacts.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/integrations/mlflow/giskard_evaluator.py` & `giskard-2.9.1/giskard/integrations/mlflow/giskard_evaluator.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/integrations/mlflow/giskard_evaluator_utils.py` & `giskard-2.9.1/giskard/integrations/mlflow/giskard_evaluator_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/integrations/wandb/wandb_utils.py` & `giskard-2.9.1/giskard/integrations/wandb/wandb_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/llm/client/__init__.py` & `giskard-2.9.1/giskard/llm/client/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/llm/client/base.py` & `giskard-2.9.1/giskard/llm/client/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/llm/client/logger.py` & `giskard-2.9.1/giskard/llm/client/logger.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/llm/client/openai.py` & `giskard-2.9.1/giskard/llm/client/openai.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/llm/evaluators/base.py` & `giskard-2.9.1/giskard/llm/evaluators/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/llm/evaluators/coherency.py` & `giskard-2.9.1/giskard/llm/evaluators/coherency.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/llm/evaluators/correctness.py` & `giskard-2.9.1/giskard/llm/evaluators/correctness.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/llm/evaluators/plausibility.py` & `giskard-2.9.1/giskard/llm/evaluators/plausibility.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/llm/evaluators/requirements.py` & `giskard-2.9.1/giskard/llm/evaluators/requirements.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/llm/evaluators/string_matcher.py` & `giskard-2.9.1/giskard/llm/evaluators/string_matcher.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/llm/generators/adversarial.py` & `giskard-2.9.1/giskard/llm/generators/adversarial.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/llm/generators/base.py` & `giskard-2.9.1/giskard/llm/generators/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/llm/generators/implausible.py` & `giskard-2.9.1/giskard/llm/generators/implausible.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/llm/generators/sycophancy.py` & `giskard-2.9.1/giskard/llm/generators/sycophancy.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/llm/loaders/prompt_injections.py` & `giskard-2.9.1/giskard/llm/loaders/prompt_injections.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/llm/testcase.py` & `giskard-2.9.1/giskard/llm/testcase.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/llm/utils.py` & `giskard-2.9.1/giskard/llm/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/ml_worker/bridge/data_encryptor.py` & `giskard-2.9.1/giskard/ml_worker/bridge/data_encryptor.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/ml_worker/ml_worker.py` & `giskard-2.9.1/giskard/ml_worker/ml_worker.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/ml_worker/stomp/client.py` & `giskard-2.9.1/giskard/ml_worker/stomp/client.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/ml_worker/stomp/constants.py` & `giskard-2.9.1/giskard/ml_worker/stomp/constants.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/ml_worker/stomp/parsing.py` & `giskard-2.9.1/giskard/ml_worker/stomp/parsing.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/ml_worker/stomp/utils.py` & `giskard-2.9.1/giskard/ml_worker/stomp/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/ml_worker/utils/cache.py` & `giskard-2.9.1/giskard/ml_worker/utils/cache.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/ml_worker/utils/network.py` & `giskard-2.9.1/giskard/ml_worker/utils/network.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/ml_worker/websocket/__init__.py` & `giskard-2.9.1/giskard/ml_worker/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/ml_worker/websocket/action.py` & `giskard-2.9.1/giskard/ml_worker/websocket/action.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/ml_worker/websocket/listener.py` & `giskard-2.9.1/giskard/ml_worker/websocket/listener.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/ml_worker/websocket/utils.py` & `giskard-2.9.1/giskard/ml_worker/websocket/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/models/__init__.py` & `giskard-2.9.1/giskard/models/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/models/_precooked.py` & `giskard-2.9.1/giskard/models/_precooked.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/models/automodel.py` & `giskard-2.9.1/giskard/models/automodel.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/models/base/model.py` & `giskard-2.9.1/giskard/models/base/model.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/models/base/model_prediction.py` & `giskard-2.9.1/giskard/models/base/model_prediction.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/models/base/serialization.py` & `giskard-2.9.1/giskard/models/base/serialization.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/models/base/wrapper.py` & `giskard-2.9.1/giskard/models/base/wrapper.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/models/cache/__init__.py` & `giskard-2.9.1/giskard/models/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/models/cache/cache.py` & `giskard-2.9.1/giskard/models/cache/cache.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/models/catboost.py` & `giskard-2.9.1/giskard/models/catboost.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/models/function.py` & `giskard-2.9.1/giskard/models/function.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/models/huggingface.py` & `giskard-2.9.1/giskard/models/huggingface.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/models/langchain.py` & `giskard-2.9.1/giskard/models/langchain.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/models/model_explanation.py` & `giskard-2.9.1/giskard/models/model_explanation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/models/pytorch.py` & `giskard-2.9.1/giskard/models/pytorch.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/models/shap_result.py` & `giskard-2.9.1/giskard/models/shap_result.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/models/sklearn.py` & `giskard-2.9.1/giskard/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/models/tensorflow.py` & `giskard-2.9.1/giskard/models/tensorflow.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/models/utils.py` & `giskard-2.9.1/giskard/models/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/push/__init__.py` & `giskard-2.9.1/giskard/push/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/push/contribution.py` & `giskard-2.9.1/giskard/push/contribution.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/push/perturbation.py` & `giskard-2.9.1/giskard/push/perturbation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/push/prediction.py` & `giskard-2.9.1/giskard/push/prediction.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/push/push_test_catalog/catalog.py` & `giskard-2.9.1/giskard/push/push_test_catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/push/utils.py` & `giskard-2.9.1/giskard/push/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/evaluate.py` & `giskard-2.9.1/giskard/rag/evaluate.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/knowledge_base.py` & `giskard-2.9.1/giskard/rag/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/knowledge_base_plots.py` & `giskard-2.9.1/giskard/rag/knowledge_base_plots.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/metrics/base.py` & `giskard-2.9.1/giskard/rag/metrics/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/metrics/correctness.py` & `giskard-2.9.1/giskard/rag/metrics/correctness.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/metrics/ragas_metrics.py` & `giskard-2.9.1/giskard/rag/metrics/ragas_metrics.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/question_generators/__init__.py` & `giskard-2.9.1/giskard/rag/question_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/question_generators/base.py` & `giskard-2.9.1/giskard/rag/question_generators/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/question_generators/complex_questions.py` & `giskard-2.9.1/giskard/rag/question_generators/complex_questions.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/question_generators/conversational_questions.py` & `giskard-2.9.1/giskard/rag/question_generators/conversational_questions.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/question_generators/distracting_questions.py` & `giskard-2.9.1/giskard/rag/question_generators/distracting_questions.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/question_generators/double_questions.py` & `giskard-2.9.1/giskard/rag/question_generators/double_questions.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/question_generators/oos_questions.py` & `giskard-2.9.1/giskard/rag/question_generators/oos_questions.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/question_generators/prompt.py` & `giskard-2.9.1/giskard/rag/question_generators/prompt.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/question_generators/question_types.py` & `giskard-2.9.1/giskard/rag/question_generators/question_types.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/question_generators/simple_questions.py` & `giskard-2.9.1/giskard/rag/question_generators/simple_questions.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/question_generators/situational_questions.py` & `giskard-2.9.1/giskard/rag/question_generators/situational_questions.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/recommendation.py` & `giskard-2.9.1/giskard/rag/recommendation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/report.py` & `giskard-2.9.1/giskard/rag/report.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/testset.py` & `giskard-2.9.1/giskard/rag/testset.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/rag/testset_generation.py` & `giskard-2.9.1/giskard/rag/testset_generation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/registry/decorators.py` & `giskard-2.9.1/giskard/registry/decorators.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/registry/decorators_utils.py` & `giskard-2.9.1/giskard/registry/decorators_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/registry/giskard_test.py` & `giskard-2.9.1/giskard/registry/giskard_test.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/registry/registry.py` & `giskard-2.9.1/giskard/registry/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/registry/slicing_function.py` & `giskard-2.9.1/giskard/registry/slicing_function.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/registry/transformation_function.py` & `giskard-2.9.1/giskard/registry/transformation_function.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/registry/utils.py` & `giskard-2.9.1/giskard/registry/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/__init__.py` & `giskard-2.9.1/giskard/scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/calibration/overconfidence_detector.py` & `giskard-2.9.1/giskard/scanner/calibration/overconfidence_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/calibration/underconfidence_detector.py` & `giskard-2.9.1/giskard/scanner/calibration/underconfidence_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/common/examples.py` & `giskard-2.9.1/giskard/scanner/common/examples.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/common/loss_based_detector.py` & `giskard-2.9.1/giskard/scanner/common/loss_based_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/common/utils.py` & `giskard-2.9.1/giskard/scanner/common/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/correlation/spurious_correlation_detector.py` & `giskard-2.9.1/giskard/scanner/correlation/spurious_correlation_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/data_leakage/data_leakage_detector.py` & `giskard-2.9.1/giskard/scanner/data_leakage/data_leakage_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/decorators.py` & `giskard-2.9.1/giskard/scanner/decorators.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/issues.py` & `giskard-2.9.1/giskard/scanner/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/llm/__init__.py` & `giskard-2.9.1/giskard/scanner/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/llm/base.py` & `giskard-2.9.1/giskard/scanner/llm/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/llm/llm_basic_sycophancy_detector.py` & `giskard-2.9.1/giskard/scanner/llm/llm_basic_sycophancy_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/llm/llm_chars_injection_detector.py` & `giskard-2.9.1/giskard/scanner/llm/llm_chars_injection_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/llm/llm_faithfulness_detector.py` & `giskard-2.9.1/giskard/scanner/llm/llm_faithfulness_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/llm/llm_harmful_content_detector.py` & `giskard-2.9.1/giskard/scanner/llm/llm_harmful_content_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/llm/llm_implausible_output_detector.py` & `giskard-2.9.1/giskard/scanner/llm/llm_implausible_output_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/llm/llm_information_disclosure_detector.py` & `giskard-2.9.1/giskard/scanner/llm/llm_information_disclosure_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/llm/llm_output_formatting_detector.py` & `giskard-2.9.1/giskard/scanner/llm/llm_output_formatting_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/llm/llm_prompt_injection_detector.py` & `giskard-2.9.1/giskard/scanner/llm/llm_prompt_injection_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/llm/llm_stereotypes_detector.py` & `giskard-2.9.1/giskard/scanner/llm/llm_stereotypes_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/performance/__init__.py` & `giskard-2.9.1/giskard/scanner/performance/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/performance/metrics.py` & `giskard-2.9.1/giskard/scanner/performance/metrics.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/performance/performance_bias_detector.py` & `giskard-2.9.1/giskard/scanner/performance/performance_bias_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/registry.py` & `giskard-2.9.1/giskard/scanner/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/report.py` & `giskard-2.9.1/giskard/scanner/report.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/robustness/__init__.py` & `giskard-2.9.1/giskard/scanner/robustness/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/robustness/base_detector.py` & `giskard-2.9.1/giskard/scanner/robustness/base_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/robustness/entity_swap.py` & `giskard-2.9.1/giskard/scanner/robustness/entity_swap.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/robustness/ethical_bias_detector.py` & `giskard-2.9.1/giskard/scanner/robustness/ethical_bias_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/robustness/nationalities.json` & `giskard-2.9.1/giskard/scanner/robustness/nationalities.json`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/robustness/text_perturbation_detector.py` & `giskard-2.9.1/giskard/scanner/robustness/text_perturbation_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/robustness/text_transformations.py` & `giskard-2.9.1/giskard/scanner/robustness/text_transformations.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/scanner.py` & `giskard-2.9.1/giskard/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/stochasticity/stochasticity_detector.py` & `giskard-2.9.1/giskard/scanner/stochasticity/stochasticity_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/templates/static/external.js` & `giskard-2.9.1/giskard/scanner/templates/static/external.js`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/templates/static/internal.js` & `giskard-2.9.1/giskard/scanner/templates/static/internal.js`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/scanner/templates/static/style.css` & `giskard-2.9.1/giskard/scanner/templates/static/style.css`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/settings.py` & `giskard-2.9.1/giskard/settings.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/slicing/base.py` & `giskard-2.9.1/giskard/slicing/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/slicing/bruteforce_slicer.py` & `giskard-2.9.1/giskard/slicing/bruteforce_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/slicing/category_slicer.py` & `giskard-2.9.1/giskard/slicing/category_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/slicing/multiscale_slicer.py` & `giskard-2.9.1/giskard/slicing/multiscale_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/slicing/opt_slicer.py` & `giskard-2.9.1/giskard/slicing/opt_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/slicing/slice.py` & `giskard-2.9.1/giskard/slicing/slice.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/slicing/slice_finder.py` & `giskard-2.9.1/giskard/slicing/slice_finder.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/slicing/stop_words.py` & `giskard-2.9.1/giskard/slicing/stop_words.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/slicing/text_slicer.py` & `giskard-2.9.1/giskard/slicing/text_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/slicing/tree_slicer.py` & `giskard-2.9.1/giskard/slicing/tree_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/slicing/utils.py` & `giskard-2.9.1/giskard/slicing/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/testing/__init__.py` & `giskard-2.9.1/giskard/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/testing/tests/calibration.py` & `giskard-2.9.1/giskard/testing/tests/calibration.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/testing/tests/data_quality.py` & `giskard-2.9.1/giskard/testing/tests/data_quality.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/testing/tests/debug_slicing_functions.py` & `giskard-2.9.1/giskard/testing/tests/debug_slicing_functions.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/testing/tests/drift.py` & `giskard-2.9.1/giskard/testing/tests/drift.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/testing/tests/llm/__init__.py` & `giskard-2.9.1/giskard/testing/tests/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/testing/tests/llm/correctness.py` & `giskard-2.9.1/giskard/testing/tests/llm/correctness.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/testing/tests/llm/ground_truth.py` & `giskard-2.9.1/giskard/testing/tests/llm/ground_truth.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/testing/tests/llm/hallucination.py` & `giskard-2.9.1/giskard/testing/tests/llm/hallucination.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/testing/tests/llm/injections.py` & `giskard-2.9.1/giskard/testing/tests/llm/injections.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/testing/tests/llm/output_requirements.py` & `giskard-2.9.1/giskard/testing/tests/llm/output_requirements.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/testing/tests/metamorphic.py` & `giskard-2.9.1/giskard/testing/tests/metamorphic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/testing/tests/performance.py` & `giskard-2.9.1/giskard/testing/tests/performance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/testing/tests/statistic.py` & `giskard-2.9.1/giskard/testing/tests/statistic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/testing/utils/stat_utils.py` & `giskard-2.9.1/giskard/testing/utils/stat_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/testing/utils/utils.py` & `giskard-2.9.1/giskard/testing/utils/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/utils/__init__.py` & `giskard-2.9.1/giskard/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/utils/analytics_collector.py` & `giskard-2.9.1/giskard/utils/analytics_collector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/utils/artifacts.py` & `giskard-2.9.1/giskard/utils/artifacts.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/utils/display.py` & `giskard-2.9.1/giskard/utils/display.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/utils/environment_detector.py` & `giskard-2.9.1/giskard/utils/environment_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/utils/logging_utils.py` & `giskard-2.9.1/giskard/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/utils/sentry.py` & `giskard-2.9.1/giskard/utils/sentry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/utils/worker_pool.py` & `giskard-2.9.1/giskard/utils/worker_pool.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/visualization/custom_jinja.py` & `giskard-2.9.1/giskard/visualization/custom_jinja.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/visualization/templates/rag_report/rag_report.html` & `giskard-2.9.1/giskard/visualization/templates/rag_report/rag_report.html`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/visualization/templates/rag_report/static/internal.js` & `giskard-2.9.1/giskard/visualization/templates/rag_report/static/internal.js`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/visualization/templates/rag_report/static/style.css` & `giskard-2.9.1/giskard/visualization/templates/rag_report/static/style.css`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/visualization/templates/scan_report/html/_code_snippet.html` & `giskard-2.9.1/giskard/visualization/templates/scan_report/html/_code_snippet.html`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/visualization/templates/scan_report/html/_issue.html` & `giskard-2.9.1/giskard/visualization/templates/scan_report/html/_issue.html`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/visualization/templates/scan_report/html/_main_content.html` & `giskard-2.9.1/giskard/visualization/templates/scan_report/html/_main_content.html`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/visualization/templates/scan_report/html/_tab_header.html` & `giskard-2.9.1/giskard/visualization/templates/scan_report/html/_tab_header.html`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/visualization/templates/scan_report/html/full.html` & `giskard-2.9.1/giskard/visualization/templates/scan_report/html/full.html`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/visualization/templates/scan_report/html/static/external.js` & `giskard-2.9.1/giskard/visualization/templates/scan_report/html/static/external.js`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/visualization/templates/scan_report/html/static/internal.js` & `giskard-2.9.1/giskard/visualization/templates/scan_report/html/static/internal.js`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/visualization/templates/scan_report/html/static/style.css` & `giskard-2.9.1/giskard/visualization/templates/scan_report/html/static/style.css`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/visualization/templates/scan_report/markdown/github.md` & `giskard-2.9.1/giskard/visualization/templates/scan_report/markdown/github.md`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/visualization/templates/scan_report/markdown/huggingface.md` & `giskard-2.9.1/giskard/visualization/templates/scan_report/markdown/huggingface.md`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/visualization/templates/scan_report/markdown/summary.md` & `giskard-2.9.1/giskard/visualization/templates/scan_report/markdown/summary.md`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/visualization/templates/suite_results/_suite_results_cards.html` & `giskard-2.9.1/giskard/visualization/templates/suite_results/_suite_results_cards.html`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/visualization/templates/suite_results/_suite_results_header.html` & `giskard-2.9.1/giskard/visualization/templates/suite_results/_suite_results_header.html`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/visualization/templates/suite_results/suite_results.html` & `giskard-2.9.1/giskard/visualization/templates/suite_results/suite_results.html`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard/visualization/widget.py` & `giskard-2.9.1/giskard/visualization/widget.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard.egg-info/PKG-INFO` & `giskard-2.9.1/giskard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giskard
-Version: 2.9.0
+Version: 2.9.1
 Summary: The testing framework dedicated to ML models, from tabular to LLMs
 Author-email: Giskard AI <hello@giskard.ai>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://giskard.ai
 Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues
 Project-URL: Documentation, https://docs.giskard.ai/
```

### Comparing `giskard-2.9.0/giskard.egg-info/SOURCES.txt` & `giskard-2.9.1/giskard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/giskard.egg-info/requires.txt` & `giskard-2.9.1/giskard.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/pyproject.toml` & `giskard-2.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 "Twitter" = "https://twitter.com/giskard_ai"
 
 
 [project]
 name = "giskard"
 readme = "README.md"
 license = { text = "Apache Software License 2.0" }
-version = "2.9.0"
+version = "2.9.1"
 description = "The testing framework dedicated to ML models, from tabular to LLMs"
 authors = [{ name = "Giskard AI", email = "hello@giskard.ai" }]
 keywords = ["Artificial Intelligence", "Machine Learning", "Quality", "MLOps"]
 
 # Pypi classifiers: https://pypi.org/classifiers/
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `giskard-2.9.0/tests/test_artifact_download.py` & `giskard-2.9.1/tests/test_artifact_download.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/tests/test_custom_model.py` & `giskard-2.9.1/tests/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/tests/test_data_drift.py` & `giskard-2.9.1/tests/test_data_drift.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/tests/test_data_processing_pipeline.py` & `giskard-2.9.1/tests/test_data_processing_pipeline.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/tests/test_dataset.py` & `giskard-2.9.1/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/tests/test_import_giskard.py` & `giskard-2.9.1/tests/test_import_giskard.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/tests/test_metamorphic_direction.py` & `giskard-2.9.1/tests/test_metamorphic_direction.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/tests/test_metamorphic_invariance.py` & `giskard-2.9.1/tests/test_metamorphic_invariance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/tests/test_performance.py` & `giskard-2.9.1/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/tests/test_programmatic.py` & `giskard-2.9.1/tests/test_programmatic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/tests/test_project_uploads.py` & `giskard-2.9.1/tests/test_project_uploads.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/tests/test_push.py` & `giskard-2.9.1/tests/test_push.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/tests/test_settings.py` & `giskard-2.9.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/tests/test_statistical.py` & `giskard-2.9.1/tests/test_statistical.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/tests/test_suite.py` & `giskard-2.9.1/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/tests/test_upload.py` & `giskard-2.9.1/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `giskard-2.9.0/tests/test_worker_pool.py` & `giskard-2.9.1/tests/test_worker_pool.py`

 * *Files identical despite different names*


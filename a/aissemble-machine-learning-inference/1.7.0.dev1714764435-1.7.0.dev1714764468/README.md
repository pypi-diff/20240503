# Comparing `tmp/aissemble_machine_learning_inference-1.7.0.dev1714764435.tar.gz` & `tmp/aissemble_machine_learning_inference-1.7.0.dev1714764468.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_machine_learning_inference-1.7.0.dev1714764435.tar", max compression
+gzip compressed data, was "aissemble_machine_learning_inference-1.7.0.dev1714764468.tar", max compression
```

## Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435.tar` & `aissemble_machine_learning_inference-1.7.0.dev1714764468.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     9580 2024-05-03 19:26:48.671276 aissemble_machine_learning_inference-1.7.0.dev1714764435/LICENSE
--rw-r--r--   0        0        0     1893 2024-05-03 19:27:15.424261 aissemble_machine_learning_inference-1.7.0.dev1714764435/pyproject.toml
--rw-r--r--   0        0        0      208 2024-05-03 19:26:48.623276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 19:26:48.551276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/__init__.py.tmp
--rw-r--r--   0        0        0      208 2024-05-03 19:26:48.622276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 19:26:44.805278 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/__init__.py.tmp
--rw-r--r--   0        0        0     1460 2024-05-03 19:26:48.622276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/date_as_seconds_since_epoch_base.py
--rw-r--r--   0        0        0     1252 2024-05-03 19:26:48.550276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/date_as_seconds_since_epoch_base.py.tmp
--rw-r--r--   0        0        0     1768 2024-05-03 19:26:48.614276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/event_category_base.py
--rw-r--r--   0        0        0     1560 2024-05-03 19:26:48.538276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/event_category_base.py.tmp
--rw-r--r--   0        0        0     1661 2024-05-03 19:26:48.612276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/event_kind_base.py
--rw-r--r--   0        0        0     1453 2024-05-03 19:26:48.535276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/event_kind_base.py.tmp
--rw-r--r--   0        0        0     1642 2024-05-03 19:26:48.616276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/event_outcome_base.py
--rw-r--r--   0        0        0     1434 2024-05-03 19:26:48.541276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/event_outcome_base.py.tmp
--rw-r--r--   0        0        0     1680 2024-05-03 19:26:48.618276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/ip_address_base.py
--rw-r--r--   0        0        0     1472 2024-05-03 19:26:48.544276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/ip_address_base.py.tmp
--rw-r--r--   0        0        0     1586 2024-05-03 19:26:48.619276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/port_base.py
--rw-r--r--   0        0        0     1378 2024-05-03 19:26:48.547276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/port_base.py.tmp
--rw-r--r--   0        0        0      208 2024-05-03 19:26:48.607276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 19:26:48.530276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/__init__.py.tmp
--rw-r--r--   0        0        0      208 2024-05-03 19:26:48.610276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/grpc/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 19:26:48.570276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/grpc/__init__.py.tmp
--rw-r--r--   0        0        0      208 2024-05-03 19:26:48.610276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 19:26:48.532276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/__init__.py.tmp
--rw-r--r--   0        0        0     1640 2024-05-03 19:27:11.004263 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/inference_payload_definition_pb2.py
--rw-r--r--   0        0        0     1217 2024-05-03 19:27:11.004263 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/inference_payload_definition_pb2_grpc.py
--rw-r--r--   0        0        0     5696 2024-05-03 19:26:48.610276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_grpc_base.py
--rw-r--r--   0        0        0     5487 2024-05-03 19:26:48.531276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_grpc_base.py.tmp
--rw-r--r--   0        0        0     2931 2024-05-03 19:27:11.004263 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_pb2.py
--rw-r--r--   0        0        0     6582 2024-05-03 19:27:11.004263 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_pb2_grpc.py
--rw-r--r--   0        0        0      208 2024-05-03 19:26:48.604276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/rest/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 19:26:48.528276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/rest/__init__.py.tmp
--rw-r--r--   0        0        0     2366 2024-05-03 19:26:48.607276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/rest/inference_payload_definition.py
--rw-r--r--   0        0        0     2158 2024-05-03 19:26:48.529276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/rest/inference_payload_definition.py.tmp
--rw-r--r--   0        0        0      208 2024-05-03 19:26:48.598276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/record/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 19:26:44.771278 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/record/__init__.py.tmp
--rw-r--r--   0        0        0     3006 2024-05-03 19:26:48.601276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_base.py
--rw-r--r--   0        0        0     2798 2024-05-03 19:26:48.562276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_base.py.tmp
--rw-r--r--   0        0        0     2910 2024-05-03 19:26:48.596276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_field.py
--rw-r--r--   0        0        0     2702 2024-05-03 19:26:48.526276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_field.py.tmp
--rw-r--r--   0        0        0     6369 2024-05-03 19:26:48.604276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/record/event_log_entry_base.py
--rw-r--r--   0        0        0     6161 2024-05-03 19:26:48.567276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/record/event_log_entry_base.py.tmp
--rw-r--r--   0        0        0     2902 2024-05-03 19:26:48.598276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/record/event_log_entry_field.py
--rw-r--r--   0        0        0     2694 2024-05-03 19:26:48.527276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/record/event_log_entry_field.py.tmp
--rw-r--r--   0        0        0      208 2024-05-03 19:26:48.627276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/validation/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 19:26:48.557276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/validation/__init__.py.tmp
--rw-r--r--   0        0        0     1456 2024-05-03 19:26:48.624276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/validation/inference_message_definition_base.py
--rw-r--r--   0        0        0     1247 2024-05-03 19:26:48.553276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/validation/inference_message_definition_base.py.tmp
--rw-r--r--   0        0        0     1748 2024-05-03 19:26:48.627276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/validation/inference_payload_definition_base.py
--rw-r--r--   0        0        0     1540 2024-05-03 19:26:48.556276 aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/validation/inference_payload_definition_base.py.tmp
--rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 aissemble_machine_learning_inference-1.7.0.dev1714764435/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-03 19:27:19.703858 aissemble_machine_learning_inference-1.7.0.dev1714764468/LICENSE
+-rw-r--r--   0        0        0     1893 2024-05-03 19:27:49.223059 aissemble_machine_learning_inference-1.7.0.dev1714764468/pyproject.toml
+-rw-r--r--   0        0        0      208 2024-05-03 19:27:19.613861 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:27:19.473865 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/__init__.py.tmp
+-rw-r--r--   0        0        0      208 2024-05-03 19:27:19.613861 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:27:14.973984 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/__init__.py.tmp
+-rw-r--r--   0        0        0     1460 2024-05-03 19:27:19.613861 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/date_as_seconds_since_epoch_base.py
+-rw-r--r--   0        0        0     1252 2024-05-03 19:27:19.473865 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/date_as_seconds_since_epoch_base.py.tmp
+-rw-r--r--   0        0        0     1768 2024-05-03 19:27:19.583862 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/event_category_base.py
+-rw-r--r--   0        0        0     1560 2024-05-03 19:27:19.453865 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/event_category_base.py.tmp
+-rw-r--r--   0        0        0     1661 2024-05-03 19:27:19.583862 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/event_kind_base.py
+-rw-r--r--   0        0        0     1453 2024-05-03 19:27:19.443865 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/event_kind_base.py.tmp
+-rw-r--r--   0        0        0     1642 2024-05-03 19:27:19.593861 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/event_outcome_base.py
+-rw-r--r--   0        0        0     1434 2024-05-03 19:27:19.453865 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/event_outcome_base.py.tmp
+-rw-r--r--   0        0        0     1680 2024-05-03 19:27:19.603861 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/ip_address_base.py
+-rw-r--r--   0        0        0     1472 2024-05-03 19:27:19.463865 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/ip_address_base.py.tmp
+-rw-r--r--   0        0        0     1586 2024-05-03 19:27:19.603861 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/port_base.py
+-rw-r--r--   0        0        0     1378 2024-05-03 19:27:19.463865 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/port_base.py.tmp
+-rw-r--r--   0        0        0      208 2024-05-03 19:27:19.573862 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:27:19.443865 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/__init__.py.tmp
+-rw-r--r--   0        0        0      208 2024-05-03 19:27:19.573862 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/grpc/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:27:19.503864 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/grpc/__init__.py.tmp
+-rw-r--r--   0        0        0      208 2024-05-03 19:27:19.573862 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:27:19.443865 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/__init__.py.tmp
+-rw-r--r--   0        0        0     1640 2024-05-03 19:27:44.003209 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/inference_payload_definition_pb2.py
+-rw-r--r--   0        0        0     1217 2024-05-03 19:27:44.003209 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/inference_payload_definition_pb2_grpc.py
+-rw-r--r--   0        0        0     5696 2024-05-03 19:27:19.573862 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_grpc_base.py
+-rw-r--r--   0        0        0     5487 2024-05-03 19:27:19.443865 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_grpc_base.py.tmp
+-rw-r--r--   0        0        0     2931 2024-05-03 19:27:44.003209 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_pb2.py
+-rw-r--r--   0        0        0     6582 2024-05-03 19:27:44.003209 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_pb2_grpc.py
+-rw-r--r--   0        0        0      208 2024-05-03 19:27:19.563862 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/rest/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:27:19.433866 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/rest/__init__.py.tmp
+-rw-r--r--   0        0        0     2366 2024-05-03 19:27:19.563862 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/rest/inference_payload_definition.py
+-rw-r--r--   0        0        0     2158 2024-05-03 19:27:19.443865 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/rest/inference_payload_definition.py.tmp
+-rw-r--r--   0        0        0      208 2024-05-03 19:27:19.553862 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/record/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:27:14.933985 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/record/__init__.py.tmp
+-rw-r--r--   0        0        0     3006 2024-05-03 19:27:19.563862 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_base.py
+-rw-r--r--   0        0        0     2798 2024-05-03 19:27:19.493864 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_base.py.tmp
+-rw-r--r--   0        0        0     2910 2024-05-03 19:27:19.553862 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_field.py
+-rw-r--r--   0        0        0     2702 2024-05-03 19:27:19.433866 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_field.py.tmp
+-rw-r--r--   0        0        0     6369 2024-05-03 19:27:19.563862 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/record/event_log_entry_base.py
+-rw-r--r--   0        0        0     6161 2024-05-03 19:27:19.503864 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/record/event_log_entry_base.py.tmp
+-rw-r--r--   0        0        0     2902 2024-05-03 19:27:19.553862 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/record/event_log_entry_field.py
+-rw-r--r--   0        0        0     2694 2024-05-03 19:27:19.433866 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/record/event_log_entry_field.py.tmp
+-rw-r--r--   0        0        0      208 2024-05-03 19:27:19.623861 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/validation/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:27:19.483864 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/validation/__init__.py.tmp
+-rw-r--r--   0        0        0     1456 2024-05-03 19:27:19.613861 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/validation/inference_message_definition_base.py
+-rw-r--r--   0        0        0     1247 2024-05-03 19:27:19.473865 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/validation/inference_message_definition_base.py.tmp
+-rw-r--r--   0        0        0     1748 2024-05-03 19:27:19.623861 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/validation/inference_payload_definition_base.py
+-rw-r--r--   0        0        0     1540 2024-05-03 19:27:19.483864 aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/validation/inference_payload_definition_base.py.tmp
+-rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 aissemble_machine_learning_inference-1.7.0.dev1714764468/PKG-INFO
```

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/LICENSE` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/pyproject.toml` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GENERATED STUB - PLEASE ***DO*** MODIFY
 # Originally generated from templates/inference/pyproject.toml.vm.
 
 [tool.poetry]
 name = "aissemble-machine-learning-inference"
-version = "1.7.0.dev1714764435"
+version = "1.7.0.dev1714764468"
 description = "Machine Learning Inference Test Module"
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 
 # Ensure that generated code is included in package archives
 include = ["src/aissemble_machine_learning_inference/generated/**/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/date_as_seconds_since_epoch_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/date_as_seconds_since_epoch_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/date_as_seconds_since_epoch_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/date_as_seconds_since_epoch_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/event_category_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/event_category_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/event_category_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/event_category_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/event_kind_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/event_kind_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/event_kind_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/event_kind_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/event_outcome_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/event_outcome_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/event_outcome_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/event_outcome_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/ip_address_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/ip_address_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/ip_address_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/ip_address_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/port_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/port_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/dictionary/port_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/dictionary/port_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/inference_payload_definition_pb2.py` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/inference_payload_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/inference_payload_definition_pb2_grpc.py` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/inference_payload_definition_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_grpc_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_grpc_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_grpc_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_grpc_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_pb2.py` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_pb2.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_pb2_grpc.py` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/rest/inference_payload_definition.py` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/rest/inference_payload_definition.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/inference/rest/inference_payload_definition.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/inference/rest/inference_payload_definition.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_field.py` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_field.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_field.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_field.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/record/event_log_entry_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/record/event_log_entry_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/record/event_log_entry_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/record/event_log_entry_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/record/event_log_entry_field.py` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/record/event_log_entry_field.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/record/event_log_entry_field.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/record/event_log_entry_field.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/validation/inference_message_definition_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/validation/inference_message_definition_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/validation/inference_message_definition_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/validation/inference_message_definition_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/validation/inference_payload_definition_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/validation/inference_payload_definition_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/src/aissemble_machine_learning_inference/generated/validation/inference_payload_definition_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/src/aissemble_machine_learning_inference/generated/validation/inference_payload_definition_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1714764435/PKG-INFO` & `aissemble_machine_learning_inference-1.7.0.dev1714764468/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-machine-learning-inference
-Version: 1.7.0.dev1714764435
+Version: 1.7.0.dev1714764468
 Summary: Machine Learning Inference Test Module
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aissemble-extensions-encryption-vault-python (==1.7.0.*)
```


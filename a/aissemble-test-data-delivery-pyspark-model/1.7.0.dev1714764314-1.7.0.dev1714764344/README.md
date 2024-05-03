# Comparing `tmp/aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314.tar.gz` & `tmp/aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314.tar", max compression
+gzip compressed data, was "aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344.tar", max compression
```

## Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314.tar` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344.tar`

### file list

```diff
@@ -1,142 +1,142 @@
--rw-r--r--   0        0        0     9580 2024-05-03 19:24:49.888342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/LICENSE
--rw-r--r--   0        0        0     1815 2024-05-03 19:25:14.436327 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/pyproject.toml
--rw-r--r--   0        0        0      202 2024-05-03 19:24:49.744342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 19:24:48.839343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/__init__.py.tmp
--rw-r--r--   0        0        0      202 2024-05-03 19:24:49.716342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 19:24:43.864346 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/__init__.py.tmp
--rw-r--r--   0        0        0     1871 2024-05-03 19:24:49.712342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/decimal_with_validation_base.py
--rw-r--r--   0        0        0     1669 2024-05-03 19:24:48.765343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/decimal_with_validation_base.py.tmp
--rw-r--r--   0        0        0     1805 2024-05-03 19:24:49.714342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/float_with_validation_base.py
--rw-r--r--   0        0        0     1603 2024-05-03 19:24:48.768343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/float_with_validation_base.py.tmp
--rw-r--r--   0        0        0     1738 2024-05-03 19:24:49.710342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/integer_with_validation_base.py
--rw-r--r--   0        0        0     1536 2024-05-03 19:24:48.762343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/integer_with_validation_base.py.tmp
--rw-r--r--   0        0        0     2355 2024-05-03 19:24:49.708342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/string_with_validation_base.py
--rw-r--r--   0        0        0     2153 2024-05-03 19:24:48.760343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/string_with_validation_base.py.tmp
--rw-r--r--   0        0        0     1259 2024-05-03 19:24:49.716342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/type_with_policies_base.py
--rw-r--r--   0        0        0     1057 2024-05-03 19:24:48.770343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/type_with_policies_base.py.tmp
--rw-r--r--   0        0        0     1004 2024-05-03 19:24:49.744342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/environment_base.py
--rw-r--r--   0        0        0      802 2024-05-03 19:24:48.835343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/environment_base.py.tmp
--rw-r--r--   0        0        0     4694 2024-05-03 19:24:49.742342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/pipeline/pipeline_base.py
--rw-r--r--   0        0        0     4492 2024-05-03 19:24:48.800343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/pipeline/pipeline_base.py.tmp
--rw-r--r--   0        0        0      202 2024-05-03 19:24:49.573342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 19:24:43.474346 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/__init__.py.tmp
--rw-r--r--   0        0        0     2265 2024-05-03 19:24:49.578343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/binary_record_base.py
--rw-r--r--   0        0        0     2063 2024-05-03 19:24:48.809343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/binary_record_base.py.tmp
--rw-r--r--   0        0        0     2749 2024-05-03 19:24:49.566342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/binary_record_field.py
--rw-r--r--   0        0        0     2547 2024-05-03 19:24:48.736343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/binary_record_field.py.tmp
--rw-r--r--   0        0        0     2216 2024-05-03 19:24:49.580342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/custom_record_base.py
--rw-r--r--   0        0        0     2014 2024-05-03 19:24:48.812343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/custom_record_base.py.tmp
--rw-r--r--   0        0        0     2749 2024-05-03 19:24:49.568343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/custom_record_field.py
--rw-r--r--   0        0        0     2547 2024-05-03 19:24:48.738343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/custom_record_field.py.tmp
--rw-r--r--   0        0        0     5062 2024-05-03 19:24:49.584343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_policies_base.py
--rw-r--r--   0        0        0     4860 2024-05-03 19:24:48.821343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_policies_base.py.tmp
--rw-r--r--   0        0        0     3193 2024-05-03 19:24:49.572342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_policies_field.py
--rw-r--r--   0        0        0     2991 2024-05-03 19:24:48.741343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_policies_field.py.tmp
--rw-r--r--   0        0        0     4112 2024-05-03 19:24:49.582342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_type_coercion_validation_base.py
--rw-r--r--   0        0        0     3910 2024-05-03 19:24:48.817343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_type_coercion_validation_base.py.tmp
--rw-r--r--   0        0        0     2958 2024-05-03 19:24:49.570342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_type_coercion_validation_field.py
--rw-r--r--   0        0        0     2756 2024-05-03 19:24:48.739343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_type_coercion_validation_field.py.tmp
--rw-r--r--   0        0        0     8070 2024-05-03 19:24:49.576342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_validation_base.py
--rw-r--r--   0        0        0     7868 2024-05-03 19:24:48.806343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_validation_base.py.tmp
--rw-r--r--   0        0        0     3046 2024-05-03 19:24:49.564342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_validation_field.py
--rw-r--r--   0        0        0     2844 2024-05-03 19:24:48.734343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_validation_field.py.tmp
--rw-r--r--   0        0        0      202 2024-05-03 19:24:49.717342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 19:24:43.467347 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/__init__.py.tmp
--rw-r--r--   0        0        0     3615 2024-05-03 19:24:49.733342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/binary_record_schema_base.py
--rw-r--r--   0        0        0     3412 2024-05-03 19:24:48.787343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/binary_record_schema_base.py.tmp
--rw-r--r--   0        0        0     3615 2024-05-03 19:24:49.735342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/custom_record_schema_base.py
--rw-r--r--   0        0        0     3412 2024-05-03 19:24:48.790343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/custom_record_schema_base.py.tmp
--rw-r--r--   0        0        0     4937 2024-05-03 19:24:49.739342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_policies_schema_base.py
--rw-r--r--   0        0        0     4734 2024-05-03 19:24:48.797343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_policies_schema_base.py.tmp
--rw-r--r--   0        0        0     5102 2024-05-03 19:24:49.737342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_type_coercion_validation_schema_base.py
--rw-r--r--   0        0        0     4899 2024-05-03 19:24:48.793343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_type_coercion_validation_schema_base.py.tmp
--rw-r--r--   0        0        0     8844 2024-05-03 19:24:49.719342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_validation_schema_base.py
--rw-r--r--   0        0        0     8641 2024-05-03 19:24:48.784343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_validation_schema_base.py.tmp
--rw-r--r--   0        0        0      202 2024-05-03 19:24:49.604343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 19:24:48.750343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/__init__.py.tmp
--rw-r--r--   0        0        0     9634 2024-05-03 19:24:49.604343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/abstract_data_action.py
--rw-r--r--   0        0        0     9555 2024-05-03 19:24:48.748343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/abstract_data_action.py.tmp
--rw-r--r--   0        0        0      664 2024-05-03 19:24:49.606342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/abstract_pipeline_step.py
--rw-r--r--   0        0        0      462 2024-05-03 19:24:48.837343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/abstract_pipeline_step.py.tmp
--rw-r--r--   0        0        0     4370 2024-05-03 19:24:49.622342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/delta_lake_persistence_async_base.py
--rw-r--r--   0        0        0     4168 2024-05-03 19:24:48.874343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/delta_lake_persistence_async_base.py.tmp
--rw-r--r--   0        0        0     4255 2024-05-03 19:24:49.666342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/delta_lake_persistence_base.py
--rw-r--r--   0        0        0     4053 2024-05-03 19:24:49.020343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/delta_lake_persistence_base.py.tmp
--rw-r--r--   0        0        0     4309 2024-05-03 19:24:49.629342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/elasticsearch_persistence_async_base.py
--rw-r--r--   0        0        0     4107 2024-05-03 19:24:48.893343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/elasticsearch_persistence_async_base.py.tmp
--rw-r--r--   0        0        0     4194 2024-05-03 19:24:49.674342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/elasticsearch_persistence_base.py
--rw-r--r--   0        0        0     3992 2024-05-03 19:24:49.036343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/elasticsearch_persistence_base.py.tmp
--rw-r--r--   0        0        0     3988 2024-05-03 19:24:49.619342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/hive_persistence_async_base.py
--rw-r--r--   0        0        0     3786 2024-05-03 19:24:48.868343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/hive_persistence_async_base.py.tmp
--rw-r--r--   0        0        0     3873 2024-05-03 19:24:49.664342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/hive_persistence_base.py
--rw-r--r--   0        0        0     3671 2024-05-03 19:24:49.014343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/hive_persistence_base.py.tmp
--rw-r--r--   0        0        0     8044 2024-05-03 19:24:49.610342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_outbound_async_base.py
--rw-r--r--   0        0        0     7842 2024-05-03 19:24:48.846343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_outbound_async_base.py.tmp
--rw-r--r--   0        0        0     7813 2024-05-03 19:24:49.655342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_outbound_base.py
--rw-r--r--   0        0        0     7611 2024-05-03 19:24:48.994343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_outbound_base.py.tmp
--rw-r--r--   0        0        0     7488 2024-05-03 19:24:49.615342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_void_outbound_async_base.py
--rw-r--r--   0        0        0     7286 2024-05-03 19:24:48.856343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_void_outbound_async_base.py.tmp
--rw-r--r--   0        0        0     7233 2024-05-03 19:24:49.660342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_void_outbound_base.py
--rw-r--r--   0        0        0     7031 2024-05-03 19:24:49.003343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_void_outbound_base.py.tmp
--rw-r--r--   0        0        0    10587 2024-05-03 19:24:49.617342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_messaging_outbound_async_base.py
--rw-r--r--   0        0        0    10385 2024-05-03 19:24:48.862343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_messaging_outbound_async_base.py.tmp
--rw-r--r--   0        0        0    10014 2024-05-03 19:24:49.662342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_messaging_outbound_base.py
--rw-r--r--   0        0        0     9812 2024-05-03 19:24:49.008343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_messaging_outbound_base.py.tmp
--rw-r--r--   0        0        0     9835 2024-05-03 19:24:49.643342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_outbound_async_base.py
--rw-r--r--   0        0        0     9633 2024-05-03 19:24:48.919343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_outbound_async_base.py.tmp
--rw-r--r--   0        0        0     9298 2024-05-03 19:24:49.686342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_outbound_base.py
--rw-r--r--   0        0        0     9096 2024-05-03 19:24:49.059343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_outbound_base.py.tmp
--rw-r--r--   0        0        0     9845 2024-05-03 19:24:49.640342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_void_outbound_async_base.py
--rw-r--r--   0        0        0     9643 2024-05-03 19:24:48.913343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_void_outbound_async_base.py.tmp
--rw-r--r--   0        0        0     9307 2024-05-03 19:24:49.683342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_void_outbound_base.py
--rw-r--r--   0        0        0     9105 2024-05-03 19:24:49.054343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_void_outbound_base.py.tmp
--rw-r--r--   0        0        0    10532 2024-05-03 19:24:49.649342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_collection_type_async_base.py
--rw-r--r--   0        0        0    10330 2024-05-03 19:24:48.932343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_collection_type_async_base.py.tmp
--rw-r--r--   0        0        0     9994 2024-05-03 19:24:49.700342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_collection_type_base.py
--rw-r--r--   0        0        0     9792 2024-05-03 19:24:49.075343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_collection_type_base.py.tmp
--rw-r--r--   0        0        0     7517 2024-05-03 19:24:49.651342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_record_type_async_base.py
--rw-r--r--   0        0        0     7315 2024-05-03 19:24:48.938343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_record_type_async_base.py.tmp
--rw-r--r--   0        0        0     7406 2024-05-03 19:24:49.703342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_record_type_base.py
--rw-r--r--   0        0        0     7204 2024-05-03 19:24:49.081343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_record_type_base.py.tmp
--rw-r--r--   0        0        0     7591 2024-05-03 19:24:49.647342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_types_async_base.py
--rw-r--r--   0        0        0     7389 2024-05-03 19:24:48.926343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_types_async_base.py.tmp
--rw-r--r--   0        0        0     7480 2024-05-03 19:24:49.692342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_types_base.py
--rw-r--r--   0        0        0     7278 2024-05-03 19:24:49.070343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_types_base.py.tmp
--rw-r--r--   0        0        0     3709 2024-05-03 19:24:49.706342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_outbound_with_custom_types_base.py
--rw-r--r--   0        0        0     3507 2024-05-03 19:24:49.085343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_outbound_with_custom_types_base.py.tmp
--rw-r--r--   0        0        0     4318 2024-05-03 19:24:49.631343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/neo4_j_persistence_async_base.py
--rw-r--r--   0        0        0     4116 2024-05-03 19:24:48.898343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/neo4_j_persistence_async_base.py.tmp
--rw-r--r--   0        0        0     4203 2024-05-03 19:24:49.676342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/neo4_j_persistence_base.py
--rw-r--r--   0        0        0     4001 2024-05-03 19:24:49.041343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/neo4_j_persistence_base.py.tmp
--rw-r--r--   0        0        0     3976 2024-05-03 19:24:49.689342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/persist_with_custom_types_base.py
--rw-r--r--   0        0        0     3774 2024-05-03 19:24:49.065343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/persist_with_custom_types_base.py.tmp
--rw-r--r--   0        0        0     4578 2024-05-03 19:24:49.627342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/postgres_persistence_async_base.py
--rw-r--r--   0        0        0     4376 2024-05-03 19:24:48.887343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/postgres_persistence_async_base.py.tmp
--rw-r--r--   0        0        0     4463 2024-05-03 19:24:49.668342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/postgres_persistence_base.py
--rw-r--r--   0        0        0     4261 2024-05-03 19:24:49.025343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/postgres_persistence_base.py.tmp
--rw-r--r--   0        0        0     4892 2024-05-03 19:24:49.624343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/rdbms_persistence_async_base.py
--rw-r--r--   0        0        0     4690 2024-05-03 19:24:48.881343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/rdbms_persistence_async_base.py.tmp
--rw-r--r--   0        0        0     4777 2024-05-03 19:24:49.670342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/rdbms_persistence_base.py
--rw-r--r--   0        0        0     4575 2024-05-03 19:24:49.031343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/rdbms_persistence_base.py.tmp
--rw-r--r--   0        0        0     4366 2024-05-03 19:24:49.612342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_messaging_outbound_async_base.py
--rw-r--r--   0        0        0     4164 2024-05-03 19:24:48.850343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_messaging_outbound_async_base.py.tmp
--rw-r--r--   0        0        0     4226 2024-05-03 19:24:49.657343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_messaging_outbound_base.py
--rw-r--r--   0        0        0     4024 2024-05-03 19:24:48.998343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_messaging_outbound_base.py.tmp
--rw-r--r--   0        0        0     3760 2024-05-03 19:24:49.635342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_native_outbound_async_base.py
--rw-r--r--   0        0        0     3558 2024-05-03 19:24:48.907343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_native_outbound_async_base.py.tmp
--rw-r--r--   0        0        0     3656 2024-05-03 19:24:49.681342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_native_outbound_base.py
--rw-r--r--   0        0        0     3454 2024-05-03 19:24:49.049343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_native_outbound_base.py.tmp
--rw-r--r--   0        0        0     3617 2024-05-03 19:24:49.633342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_outbound_async_base.py
--rw-r--r--   0        0        0     3415 2024-05-03 19:24:48.903343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_outbound_async_base.py.tmp
--rw-r--r--   0        0        0     3512 2024-05-03 19:24:49.678342 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_outbound_base.py
--rw-r--r--   0        0        0     3310 2024-05-03 19:24:49.045343 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_outbound_base.py.tmp
--rw-r--r--   0        0        0      265 2024-05-03 19:16:24.523693 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/resources/config/messaging.properties
--rw-r--r--   0        0        0     1225 2024-05-03 19:16:24.523693 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/resources/dictionaries/PysparkDataDeliveryDictionary.json
--rw-r--r--   0        0        0      263 2024-05-03 19:16:24.523693 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/resources/krausening/base/messaging.properties
--rw-r--r--   0        0        0     6893 2024-05-03 19:16:24.523693 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/resources/pipelines/PysparkDataDeliveryPatterns.json
--rw-r--r--   0        0        0      352 2024-05-03 19:16:24.523693 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/resources/records/BinaryRecord.json
--rw-r--r--   0        0        0      313 2024-05-03 19:16:24.523693 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/resources/records/CustomRecord.json
--rw-r--r--   0        0        0      936 2024-05-03 19:16:24.523693 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/resources/records/RecordWithPolicies.json
--rw-r--r--   0        0        0      543 2024-05-03 19:16:24.524693 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/resources/records/RecordWithTypeCoercionValidation.json
--rw-r--r--   0        0        0     1139 2024-05-03 19:16:24.524693 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/resources/records/RecordWithValidation.json
--rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-03 19:25:18.617077 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/LICENSE
+-rw-r--r--   0        0        0     1815 2024-05-03 19:25:45.286378 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/pyproject.toml
+-rw-r--r--   0        0        0      202 2024-05-03 19:25:18.467081 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:25:17.597104 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/__init__.py.tmp
+-rw-r--r--   0        0        0      202 2024-05-03 19:25:18.447081 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:25:12.337242 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/__init__.py.tmp
+-rw-r--r--   0        0        0     1871 2024-05-03 19:25:18.437082 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/decimal_with_validation_base.py
+-rw-r--r--   0        0        0     1669 2024-05-03 19:25:17.497106 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/decimal_with_validation_base.py.tmp
+-rw-r--r--   0        0        0     1805 2024-05-03 19:25:18.437082 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/float_with_validation_base.py
+-rw-r--r--   0        0        0     1603 2024-05-03 19:25:17.497106 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/float_with_validation_base.py.tmp
+-rw-r--r--   0        0        0     1738 2024-05-03 19:25:18.437082 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/integer_with_validation_base.py
+-rw-r--r--   0        0        0     1536 2024-05-03 19:25:17.487107 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/integer_with_validation_base.py.tmp
+-rw-r--r--   0        0        0     2355 2024-05-03 19:25:18.427082 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/string_with_validation_base.py
+-rw-r--r--   0        0        0     2153 2024-05-03 19:25:17.487107 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/string_with_validation_base.py.tmp
+-rw-r--r--   0        0        0     1259 2024-05-03 19:25:18.447081 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/type_with_policies_base.py
+-rw-r--r--   0        0        0     1057 2024-05-03 19:25:17.497106 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/type_with_policies_base.py.tmp
+-rw-r--r--   0        0        0     1004 2024-05-03 19:25:18.467081 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/environment_base.py
+-rw-r--r--   0        0        0      802 2024-05-03 19:25:17.587104 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/environment_base.py.tmp
+-rw-r--r--   0        0        0     4694 2024-05-03 19:25:18.457081 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/pipeline/pipeline_base.py
+-rw-r--r--   0        0        0     4492 2024-05-03 19:25:17.557105 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/pipeline/pipeline_base.py.tmp
+-rw-r--r--   0        0        0      202 2024-05-03 19:25:18.277086 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:25:12.057249 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/__init__.py.tmp
+-rw-r--r--   0        0        0     2265 2024-05-03 19:25:18.287086 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/binary_record_base.py
+-rw-r--r--   0        0        0     2063 2024-05-03 19:25:17.567104 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/binary_record_base.py.tmp
+-rw-r--r--   0        0        0     2749 2024-05-03 19:25:18.267086 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/binary_record_field.py
+-rw-r--r--   0        0        0     2547 2024-05-03 19:25:17.437108 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/binary_record_field.py.tmp
+-rw-r--r--   0        0        0     2216 2024-05-03 19:25:18.287086 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/custom_record_base.py
+-rw-r--r--   0        0        0     2014 2024-05-03 19:25:17.567104 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/custom_record_base.py.tmp
+-rw-r--r--   0        0        0     2749 2024-05-03 19:25:18.267086 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/custom_record_field.py
+-rw-r--r--   0        0        0     2547 2024-05-03 19:25:17.447108 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/custom_record_field.py.tmp
+-rw-r--r--   0        0        0     5062 2024-05-03 19:25:18.297085 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_policies_base.py
+-rw-r--r--   0        0        0     4860 2024-05-03 19:25:17.577104 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_policies_base.py.tmp
+-rw-r--r--   0        0        0     3193 2024-05-03 19:25:18.277086 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_policies_field.py
+-rw-r--r--   0        0        0     2991 2024-05-03 19:25:17.447108 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_policies_field.py.tmp
+-rw-r--r--   0        0        0     4112 2024-05-03 19:25:18.287086 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_type_coercion_validation_base.py
+-rw-r--r--   0        0        0     3910 2024-05-03 19:25:17.567104 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_type_coercion_validation_base.py.tmp
+-rw-r--r--   0        0        0     2958 2024-05-03 19:25:18.277086 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_type_coercion_validation_field.py
+-rw-r--r--   0        0        0     2756 2024-05-03 19:25:17.447108 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_type_coercion_validation_field.py.tmp
+-rw-r--r--   0        0        0     8070 2024-05-03 19:25:18.277086 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_validation_base.py
+-rw-r--r--   0        0        0     7868 2024-05-03 19:25:17.557105 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_validation_base.py.tmp
+-rw-r--r--   0        0        0     3046 2024-05-03 19:25:18.267086 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_validation_field.py
+-rw-r--r--   0        0        0     2844 2024-05-03 19:25:17.437108 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_validation_field.py.tmp
+-rw-r--r--   0        0        0      202 2024-05-03 19:25:18.447081 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:25:12.047249 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/__init__.py.tmp
+-rw-r--r--   0        0        0     3615 2024-05-03 19:25:18.447081 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/binary_record_schema_base.py
+-rw-r--r--   0        0        0     3412 2024-05-03 19:25:17.527106 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/binary_record_schema_base.py.tmp
+-rw-r--r--   0        0        0     3615 2024-05-03 19:25:18.447081 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/custom_record_schema_base.py
+-rw-r--r--   0        0        0     3412 2024-05-03 19:25:17.537105 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/custom_record_schema_base.py.tmp
+-rw-r--r--   0        0        0     4937 2024-05-03 19:25:18.457081 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_policies_schema_base.py
+-rw-r--r--   0        0        0     4734 2024-05-03 19:25:17.547105 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_policies_schema_base.py.tmp
+-rw-r--r--   0        0        0     5102 2024-05-03 19:25:18.457081 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_type_coercion_validation_schema_base.py
+-rw-r--r--   0        0        0     4899 2024-05-03 19:25:17.537105 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_type_coercion_validation_schema_base.py.tmp
+-rw-r--r--   0        0        0     8844 2024-05-03 19:25:18.447081 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_validation_schema_base.py
+-rw-r--r--   0        0        0     8641 2024-05-03 19:25:17.527106 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_validation_schema_base.py.tmp
+-rw-r--r--   0        0        0      202 2024-05-03 19:25:18.297085 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:25:17.467107 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/__init__.py.tmp
+-rw-r--r--   0        0        0     9634 2024-05-03 19:25:18.297085 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/abstract_data_action.py
+-rw-r--r--   0        0        0     9555 2024-05-03 19:25:17.467107 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/abstract_data_action.py.tmp
+-rw-r--r--   0        0        0      664 2024-05-03 19:25:18.297085 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/abstract_pipeline_step.py
+-rw-r--r--   0        0        0      462 2024-05-03 19:25:17.597104 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/abstract_pipeline_step.py.tmp
+-rw-r--r--   0        0        0     4370 2024-05-03 19:25:18.327085 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/delta_lake_persistence_async_base.py
+-rw-r--r--   0        0        0     4168 2024-05-03 19:25:17.627103 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/delta_lake_persistence_async_base.py.tmp
+-rw-r--r--   0        0        0     4255 2024-05-03 19:25:18.387083 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/delta_lake_persistence_base.py
+-rw-r--r--   0        0        0     4053 2024-05-03 19:25:17.757099 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/delta_lake_persistence_base.py.tmp
+-rw-r--r--   0        0        0     4309 2024-05-03 19:25:18.337084 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/elasticsearch_persistence_async_base.py
+-rw-r--r--   0        0        0     4107 2024-05-03 19:25:17.647102 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/elasticsearch_persistence_async_base.py.tmp
+-rw-r--r--   0        0        0     4194 2024-05-03 19:25:18.397083 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/elasticsearch_persistence_base.py
+-rw-r--r--   0        0        0     3992 2024-05-03 19:25:17.767099 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/elasticsearch_persistence_base.py.tmp
+-rw-r--r--   0        0        0     3988 2024-05-03 19:25:18.327085 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/hive_persistence_async_base.py
+-rw-r--r--   0        0        0     3786 2024-05-03 19:25:17.627103 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/hive_persistence_async_base.py.tmp
+-rw-r--r--   0        0        0     3873 2024-05-03 19:25:18.387083 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/hive_persistence_base.py
+-rw-r--r--   0        0        0     3671 2024-05-03 19:25:17.747100 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/hive_persistence_base.py.tmp
+-rw-r--r--   0        0        0     8044 2024-05-03 19:25:18.307085 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_outbound_async_base.py
+-rw-r--r--   0        0        0     7842 2024-05-03 19:25:17.607103 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_outbound_async_base.py.tmp
+-rw-r--r--   0        0        0     7813 2024-05-03 19:25:18.367084 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_outbound_base.py
+-rw-r--r--   0        0        0     7611 2024-05-03 19:25:17.727100 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_outbound_base.py.tmp
+-rw-r--r--   0        0        0     7488 2024-05-03 19:25:18.307085 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_void_outbound_async_base.py
+-rw-r--r--   0        0        0     7286 2024-05-03 19:25:17.617103 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_void_outbound_async_base.py.tmp
+-rw-r--r--   0        0        0     7233 2024-05-03 19:25:18.377083 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_void_outbound_base.py
+-rw-r--r--   0        0        0     7031 2024-05-03 19:25:17.737100 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_void_outbound_base.py.tmp
+-rw-r--r--   0        0        0    10587 2024-05-03 19:25:18.317085 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_messaging_outbound_async_base.py
+-rw-r--r--   0        0        0    10385 2024-05-03 19:25:17.617103 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_messaging_outbound_async_base.py.tmp
+-rw-r--r--   0        0        0    10014 2024-05-03 19:25:18.377083 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_messaging_outbound_base.py
+-rw-r--r--   0        0        0     9812 2024-05-03 19:25:17.747100 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_messaging_outbound_base.py.tmp
+-rw-r--r--   0        0        0     9835 2024-05-03 19:25:18.357084 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_outbound_async_base.py
+-rw-r--r--   0        0        0     9633 2024-05-03 19:25:17.667102 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_outbound_async_base.py.tmp
+-rw-r--r--   0        0        0     9298 2024-05-03 19:25:18.417082 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_outbound_base.py
+-rw-r--r--   0        0        0     9096 2024-05-03 19:25:17.787099 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_outbound_base.py.tmp
+-rw-r--r--   0        0        0     9845 2024-05-03 19:25:18.347084 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_void_outbound_async_base.py
+-rw-r--r--   0        0        0     9643 2024-05-03 19:25:17.667102 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_void_outbound_async_base.py.tmp
+-rw-r--r--   0        0        0     9307 2024-05-03 19:25:18.407082 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_void_outbound_base.py
+-rw-r--r--   0        0        0     9105 2024-05-03 19:25:17.787099 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_void_outbound_base.py.tmp
+-rw-r--r--   0        0        0    10532 2024-05-03 19:25:18.367084 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_collection_type_async_base.py
+-rw-r--r--   0        0        0    10330 2024-05-03 19:25:17.677102 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_collection_type_async_base.py.tmp
+-rw-r--r--   0        0        0     9994 2024-05-03 19:25:18.427082 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_collection_type_base.py
+-rw-r--r--   0        0        0     9792 2024-05-03 19:25:17.807098 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_collection_type_base.py.tmp
+-rw-r--r--   0        0        0     7517 2024-05-03 19:25:18.367084 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_record_type_async_base.py
+-rw-r--r--   0        0        0     7315 2024-05-03 19:25:17.687101 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_record_type_async_base.py.tmp
+-rw-r--r--   0        0        0     7406 2024-05-03 19:25:18.427082 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_record_type_base.py
+-rw-r--r--   0        0        0     7204 2024-05-03 19:25:17.807098 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_record_type_base.py.tmp
+-rw-r--r--   0        0        0     7591 2024-05-03 19:25:18.357084 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_types_async_base.py
+-rw-r--r--   0        0        0     7389 2024-05-03 19:25:17.677102 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_types_async_base.py.tmp
+-rw-r--r--   0        0        0     7480 2024-05-03 19:25:18.417082 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_types_base.py
+-rw-r--r--   0        0        0     7278 2024-05-03 19:25:17.797098 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_types_base.py.tmp
+-rw-r--r--   0        0        0     3709 2024-05-03 19:25:18.427082 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_outbound_with_custom_types_base.py
+-rw-r--r--   0        0        0     3507 2024-05-03 19:25:17.817098 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_outbound_with_custom_types_base.py.tmp
+-rw-r--r--   0        0        0     4318 2024-05-03 19:25:18.337084 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/neo4_j_persistence_async_base.py
+-rw-r--r--   0        0        0     4116 2024-05-03 19:25:17.657102 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/neo4_j_persistence_async_base.py.tmp
+-rw-r--r--   0        0        0     4203 2024-05-03 19:25:18.397083 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/neo4_j_persistence_base.py
+-rw-r--r--   0        0        0     4001 2024-05-03 19:25:17.777099 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/neo4_j_persistence_base.py.tmp
+-rw-r--r--   0        0        0     3976 2024-05-03 19:25:18.417082 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/persist_with_custom_types_base.py
+-rw-r--r--   0        0        0     3774 2024-05-03 19:25:17.797098 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/persist_with_custom_types_base.py.tmp
+-rw-r--r--   0        0        0     4578 2024-05-03 19:25:18.337084 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/postgres_persistence_async_base.py
+-rw-r--r--   0        0        0     4376 2024-05-03 19:25:17.637103 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/postgres_persistence_async_base.py.tmp
+-rw-r--r--   0        0        0     4463 2024-05-03 19:25:18.387083 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/postgres_persistence_base.py
+-rw-r--r--   0        0        0     4261 2024-05-03 19:25:17.757099 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/postgres_persistence_base.py.tmp
+-rw-r--r--   0        0        0     4892 2024-05-03 19:25:18.337084 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/rdbms_persistence_async_base.py
+-rw-r--r--   0        0        0     4690 2024-05-03 19:25:17.637103 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/rdbms_persistence_async_base.py.tmp
+-rw-r--r--   0        0        0     4777 2024-05-03 19:25:18.397083 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/rdbms_persistence_base.py
+-rw-r--r--   0        0        0     4575 2024-05-03 19:25:17.767099 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/rdbms_persistence_base.py.tmp
+-rw-r--r--   0        0        0     4366 2024-05-03 19:25:18.307085 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_messaging_outbound_async_base.py
+-rw-r--r--   0        0        0     4164 2024-05-03 19:25:17.607103 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_messaging_outbound_async_base.py.tmp
+-rw-r--r--   0        0        0     4226 2024-05-03 19:25:18.377083 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_messaging_outbound_base.py
+-rw-r--r--   0        0        0     4024 2024-05-03 19:25:17.737100 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_messaging_outbound_base.py.tmp
+-rw-r--r--   0        0        0     3760 2024-05-03 19:25:18.347084 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_native_outbound_async_base.py
+-rw-r--r--   0        0        0     3558 2024-05-03 19:25:17.657102 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_native_outbound_async_base.py.tmp
+-rw-r--r--   0        0        0     3656 2024-05-03 19:25:18.407082 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_native_outbound_base.py
+-rw-r--r--   0        0        0     3454 2024-05-03 19:25:17.777099 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_native_outbound_base.py.tmp
+-rw-r--r--   0        0        0     3617 2024-05-03 19:25:18.347084 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_outbound_async_base.py
+-rw-r--r--   0        0        0     3415 2024-05-03 19:25:17.657102 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_outbound_async_base.py.tmp
+-rw-r--r--   0        0        0     3512 2024-05-03 19:25:18.407082 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_outbound_base.py
+-rw-r--r--   0        0        0     3310 2024-05-03 19:25:17.777099 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_outbound_base.py.tmp
+-rw-r--r--   0        0        0      265 2024-05-03 19:16:24.721112 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/resources/config/messaging.properties
+-rw-r--r--   0        0        0     1225 2024-05-03 19:16:24.721112 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/resources/dictionaries/PysparkDataDeliveryDictionary.json
+-rw-r--r--   0        0        0      263 2024-05-03 19:16:24.721112 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/resources/krausening/base/messaging.properties
+-rw-r--r--   0        0        0     6893 2024-05-03 19:16:24.721112 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/resources/pipelines/PysparkDataDeliveryPatterns.json
+-rw-r--r--   0        0        0      352 2024-05-03 19:16:24.721112 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/resources/records/BinaryRecord.json
+-rw-r--r--   0        0        0      313 2024-05-03 19:16:24.721112 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/resources/records/CustomRecord.json
+-rw-r--r--   0        0        0      936 2024-05-03 19:16:24.721112 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/resources/records/RecordWithPolicies.json
+-rw-r--r--   0        0        0      543 2024-05-03 19:16:24.721112 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/resources/records/RecordWithTypeCoercionValidation.json
+-rw-r--r--   0        0        0     1139 2024-05-03 19:16:24.721112 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/resources/records/RecordWithValidation.json
+-rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/PKG-INFO
```

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/LICENSE` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/pyproject.toml` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # GENERATED STUB - PLEASE ***DO*** MODIFY
 
 [tool.poetry]
 name = "aissemble-test-data-delivery-pyspark-model"
-version = "1.7.0.dev1714764314"
+version = "1.7.0.dev1714764344"
 description = "Pyspark test module"
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 
 # Ensure that generated code is included in package archives
 include = ["src/aissemble_test_data_delivery_pyspark_model/generated/**/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/decimal_with_validation_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/decimal_with_validation_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/decimal_with_validation_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/decimal_with_validation_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/float_with_validation_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/float_with_validation_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/float_with_validation_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/float_with_validation_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/integer_with_validation_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/integer_with_validation_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/integer_with_validation_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/integer_with_validation_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/string_with_validation_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/string_with_validation_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/string_with_validation_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/string_with_validation_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/type_with_policies_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/type_with_policies_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/type_with_policies_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/dictionary/type_with_policies_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/environment_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/environment_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/environment_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/environment_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/pipeline/pipeline_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/pipeline/pipeline_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/pipeline/pipeline_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/pipeline/pipeline_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/binary_record_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/binary_record_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/binary_record_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/binary_record_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/binary_record_field.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/binary_record_field.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/binary_record_field.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/binary_record_field.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/custom_record_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/custom_record_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/custom_record_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/custom_record_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/custom_record_field.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/custom_record_field.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/custom_record_field.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/custom_record_field.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_policies_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_policies_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_policies_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_policies_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_policies_field.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_policies_field.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_policies_field.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_policies_field.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_type_coercion_validation_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_type_coercion_validation_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_type_coercion_validation_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_type_coercion_validation_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_type_coercion_validation_field.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_type_coercion_validation_field.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_type_coercion_validation_field.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_type_coercion_validation_field.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_validation_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_validation_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_validation_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_validation_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_validation_field.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_validation_field.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_validation_field.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/record/record_with_validation_field.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/binary_record_schema_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/binary_record_schema_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/binary_record_schema_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/binary_record_schema_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/custom_record_schema_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/custom_record_schema_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/custom_record_schema_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/custom_record_schema_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_policies_schema_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_policies_schema_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_policies_schema_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_policies_schema_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_type_coercion_validation_schema_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_type_coercion_validation_schema_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_type_coercion_validation_schema_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_type_coercion_validation_schema_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_validation_schema_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_validation_schema_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_validation_schema_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/schema/record_with_validation_schema_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/abstract_data_action.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/abstract_data_action.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/abstract_data_action.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/abstract_data_action.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/abstract_pipeline_step.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/abstract_pipeline_step.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/delta_lake_persistence_async_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/delta_lake_persistence_async_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/delta_lake_persistence_async_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/delta_lake_persistence_async_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/delta_lake_persistence_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/delta_lake_persistence_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/delta_lake_persistence_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/delta_lake_persistence_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/elasticsearch_persistence_async_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/elasticsearch_persistence_async_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/elasticsearch_persistence_async_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/elasticsearch_persistence_async_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/elasticsearch_persistence_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/elasticsearch_persistence_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/elasticsearch_persistence_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/elasticsearch_persistence_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/hive_persistence_async_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/hive_persistence_async_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/hive_persistence_async_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/hive_persistence_async_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/hive_persistence_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/hive_persistence_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/hive_persistence_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/hive_persistence_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_outbound_async_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_outbound_async_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_outbound_async_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_outbound_async_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_outbound_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_outbound_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_outbound_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_outbound_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_void_outbound_async_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_void_outbound_async_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_void_outbound_async_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_void_outbound_async_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_void_outbound_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_void_outbound_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_void_outbound_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/messaging_inbound_and_void_outbound_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_messaging_outbound_async_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_messaging_outbound_async_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_messaging_outbound_async_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_messaging_outbound_async_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_messaging_outbound_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_messaging_outbound_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_messaging_outbound_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_messaging_outbound_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_outbound_async_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_outbound_async_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_outbound_async_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_outbound_async_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_outbound_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_outbound_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_outbound_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_outbound_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_void_outbound_async_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_void_outbound_async_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_void_outbound_async_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_void_outbound_async_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_void_outbound_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_void_outbound_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_void_outbound_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_and_void_outbound_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_collection_type_async_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_collection_type_async_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_collection_type_async_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_collection_type_async_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_collection_type_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_collection_type_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_collection_type_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_collection_type_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_record_type_async_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_record_type_async_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_record_type_async_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_record_type_async_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_record_type_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_record_type_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_record_type_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_record_type_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_types_async_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_types_async_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_types_async_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_types_async_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_types_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_types_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_types_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_inbound_with_custom_types_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_outbound_with_custom_types_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_outbound_with_custom_types_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_outbound_with_custom_types_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/native_outbound_with_custom_types_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/neo4_j_persistence_async_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/neo4_j_persistence_async_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/neo4_j_persistence_async_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/neo4_j_persistence_async_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/neo4_j_persistence_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/neo4_j_persistence_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/neo4_j_persistence_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/neo4_j_persistence_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/persist_with_custom_types_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/persist_with_custom_types_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/persist_with_custom_types_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/persist_with_custom_types_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/postgres_persistence_async_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/postgres_persistence_async_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/postgres_persistence_async_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/postgres_persistence_async_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/postgres_persistence_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/postgres_persistence_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/postgres_persistence_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/postgres_persistence_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/rdbms_persistence_async_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/rdbms_persistence_async_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/rdbms_persistence_async_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/rdbms_persistence_async_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/rdbms_persistence_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/rdbms_persistence_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/rdbms_persistence_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/rdbms_persistence_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_messaging_outbound_async_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_messaging_outbound_async_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_messaging_outbound_async_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_messaging_outbound_async_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_messaging_outbound_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_messaging_outbound_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_messaging_outbound_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_messaging_outbound_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_native_outbound_async_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_native_outbound_async_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_native_outbound_async_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_native_outbound_async_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_native_outbound_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_native_outbound_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_native_outbound_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_native_outbound_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_outbound_async_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_outbound_async_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_outbound_async_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_outbound_async_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_outbound_base.py` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_outbound_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_outbound_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/generated/step/void_inbound_and_outbound_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/resources/dictionaries/PysparkDataDeliveryDictionary.json` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/resources/dictionaries/PysparkDataDeliveryDictionary.json`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/resources/pipelines/PysparkDataDeliveryPatterns.json` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/resources/pipelines/PysparkDataDeliveryPatterns.json`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/resources/records/RecordWithPolicies.json` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/resources/records/RecordWithPolicies.json`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/resources/records/RecordWithTypeCoercionValidation.json` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/resources/records/RecordWithTypeCoercionValidation.json`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/src/aissemble_test_data_delivery_pyspark_model/resources/records/RecordWithValidation.json` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/src/aissemble_test_data_delivery_pyspark_model/resources/records/RecordWithValidation.json`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764314/PKG-INFO` & `aissemble_test_data_delivery_pyspark_model-1.7.0.dev1714764344/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-test-data-delivery-pyspark-model
-Version: 1.7.0.dev1714764314
+Version: 1.7.0.dev1714764344
 Summary: Pyspark test module
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aissemble-extensions-data-delivery-spark-py (==1.7.0.*)
```


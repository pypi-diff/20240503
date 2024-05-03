# Comparing `tmp/opperai-0.4.0.tar.gz` & `tmp/opperai-0.5.0.tar.gz`

## Comparing `opperai-0.4.0.tar` & `opperai-0.5.0.tar`

### file list

```diff
@@ -1,85 +1,83 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 opperai-0.4.0/pytest.ini
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.4.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/__init__.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/_client.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/_http_clients.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/functions/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/functions/_async_functions.py
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/functions/_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/functions/decorator/__init__.py
--rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/functions/decorator/_decorator.py
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/functions/decorator/_schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/indexes/__init__.py
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/indexes/_async_indexes.py
--rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/indexes/_indexes.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/spans/__init__.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/spans/_async_spans.py
--rw-r--r--   0        0        0     4876 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/spans/_decorator.py
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/spans/_spans.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/types/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/types/exceptions.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/types/indexes.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/types/spans.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/types/validators.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/utils/__init__.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/test_async_functions.py
--rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/test_async_indexes.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/test_async_spans.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/test_decorator.py
--rw-r--r--   0        0        0     8184 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/test_functions.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/test_indexes.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/test_spans.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/test_trace_decorator.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/test_types.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml
--rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_id.yaml
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_path.yaml
--rw-r--r--   0        0        0     9714 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml
--rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_spans/test_save_feedback.yaml
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml
--rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml
--rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml
--rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml
--rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml
--rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_get.yaml
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml
--rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml
--rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_upload_file.yaml
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 opperai-0.4.0/.gitignore
--rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 opperai-0.4.0/LICENSE
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 opperai-0.4.0/README.md
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 opperai-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 opperai-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 opperai-0.5.0/pytest.ini
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.5.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/__init__.py
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/_client.py
+-rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/functions.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/indexes.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/spans.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/core/_http_clients.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/core/functions/__init__.py
+-rw-r--r--   0        0        0     6556 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/core/functions/_async_functions.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/core/functions/_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/core/functions/decorator/__init__.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/core/functions/decorator/_decorator.py
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/core/functions/decorator/_schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/core/indexes/__init__.py
+-rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/core/indexes/_async_indexes.py
+-rw-r--r--   0        0        0     5077 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/core/indexes/_indexes.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/core/spans/__init__.py
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/core/spans/_async_spans.py
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/core/spans/_decorator.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/core/spans/_spans.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/core/utils/__init__.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/types/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/types/exceptions.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/types/indexes.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/types/spans.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opperai-0.5.0/src/opperai/types/validators.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/test_async_functions.py
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/test_async_indexes.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/test_async_spans.py
+-rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/test_decorator.py
+-rw-r--r--   0        0        0     8185 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/test_functions.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/test_indexes.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/test_spans.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/test_trace_decorator.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/test_types.py
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml
+-rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml
+-rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.5.0/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 opperai-0.5.0/.gitignore
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 opperai-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 opperai-0.5.0/README.md
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 opperai-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 opperai-0.5.0/PKG-INFO
```

### Comparing `opperai-0.4.0/.github/workflows/publish.yml` & `opperai-0.5.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `opperai-0.4.0/src/opperai/_client.py` & `opperai-0.5.0/src/opperai/_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 
-from ._http_clients import _async_http_client, _http_client
-from .functions._async_functions import AsyncFunctions
-from .functions._functions import Functions
-from .indexes._async_indexes import AsyncIndexes
-from .indexes._indexes import Indexes
-from .spans._async_spans import AsyncSpans
-from .spans._spans import Spans
+from opperai.core.functions._async_functions import AsyncFunctions
+from opperai.core.functions._functions import Functions
+from opperai.core.indexes._async_indexes import AsyncIndexes
+from opperai.core.indexes._indexes import Indexes
+from opperai.core.spans._async_spans import AsyncSpans
+from opperai.core.spans._spans import Spans
+
+from .core._http_clients import _async_http_client, _http_client
 
 DEFAULT_API_URL = "https://api.opper.ai"
 DEFAULT_TIMEOUT = 120
 
 
 class AsyncClient:
     _instance = None
```

### Comparing `opperai-0.4.0/src/opperai/_http_clients.py` & `opperai-0.5.0/src/opperai/core/_http_clients.py`

 * *Files identical despite different names*

### Comparing `opperai-0.4.0/src/opperai/functions/_async_functions.py` & `opperai-0.5.0/src/opperai/core/functions/_async_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,62 @@
+from http import HTTPStatus
 from typing import Generator, Optional
 
-from opperai._http_clients import _async_http_client
-from opperai.spans import get_current_span_id
+from opperai.core._http_clients import _async_http_client
+from opperai.core.spans import get_current_span_id
 from opperai.types import (
     ChatPayload,
     Function,
     FunctionResponse,
     StreamingChunk,
     validate_id_xor_path,
 )
-from http import HTTPStatus
 from opperai.types.exceptions import APIError, RateLimitError, StructuredGenerationError
 
 
 class AsyncFunctions:
     def __init__(self, http_client: _async_http_client, default_model: str = None):
         self.http_client = http_client
         self.default_model = default_model
 
+    async def create(
+        self, function: Function, update: bool = True, **kwargs
+    ) -> Function:
+        fn = await self.get(path=function.path)
+        if fn is None:
+            return await self._create(function, **kwargs)
+        elif update:
+            function.id = fn.id
+            return await self.update(function, **kwargs)
+        return fn
+
     async def _create(self, function: Function, **kwargs) -> Function:
         if not function.model and self.default_model:
             function.model = self.default_model
         response = await self.http_client.do_request(
             "POST",
-            "/api/v1/functions",
+            "/v1/functions",
             json={**function.model_dump(), **kwargs},
         )
         if response.status_code != HTTPStatus.OK:
             raise APIError(
-                f"Failed to create function {function.path} with status {response.status_code}"
+                f"Failed to create function {function.path} with status {response.status_code}: {response.text}"
             )
 
         return Function.model_validate(response.json())
 
     async def update(self, function: Function, **kwargs) -> Function:
         response = await self.http_client.do_request(
-            "POST",
-            f"/api/v1/functions/{function.id}",
+            "PATCH",
+            f"/v1/functions/{function.id}",
             json={**function.model_dump(), **kwargs},
         )
         if response.status_code != HTTPStatus.OK:
             raise APIError(
-                f"Failed to update function {function.path} with status {response.status_code}"
+                f"Failed to update function {function.path} with status {response.status_code}: {response.text}"
             )
 
         return Function.model_validate(response.json())
 
     @validate_id_xor_path
     async def get(self, id: str = None, path: str = None) -> Optional[Function]:
         if path is not None:
@@ -53,74 +64,78 @@
                 raise ValueError("Only one of id or path should be provided")
             return await self._get_by_path(path)
         elif id is not None:
             return await self._get_by_id(id)
         else:
             return None
 
-    async def _get_by_path(self, function_path: str) -> Function:
+    async def _get_by_path(self, function_path: str) -> Optional[Function]:
         response = await self.http_client.do_request(
             "GET",
-            f"/api/v1/functions/by_path/{function_path}",
+            f"/v1/functions/by_path/{function_path}",
         )
         if response.status_code == HTTPStatus.NOT_FOUND:
             return None
         if response.status_code != HTTPStatus.OK:
             raise APIError(
                 f"Failed to get function {function_path} with status {response.status_code}"
             )
 
         return Function.model_validate(response.json())
 
-    async def _get_by_id(self, function_id: str) -> Function:
+    async def _get_by_id(self, function_id: str) -> Optional[Function]:
         response = await self.http_client.do_request(
             "GET",
-            f"/api/v1/functions/{function_id}",
+            f"/v1/functions/{function_id}",
         )
         if response.status_code == HTTPStatus.NOT_FOUND:
             return None
         if response.status_code != HTTPStatus.OK:
             raise APIError(
                 f"Failed to get function {function_id} with status {response.status_code}"
             )
 
         return Function.model_validate(response.json())
 
-    async def create(
-        self, function: Function, update: bool = True, **kwargs
-    ) -> Function:
-        fn = await self.get(path=function.path)
-        if fn is None:
-            return await self._create(function, **kwargs)
-        elif update:
-            function.id = fn.id
-            return await self.update(function, **kwargs)
-        return fn
-
     @validate_id_xor_path
     async def delete(self, id: str = None, path: str = None):
         if path is not None:
             try:
                 await self._delete_by_path(path)
             except APIError:
                 pass
         elif id is not None:
-            fn = await self.get(id=id)
-            if fn:
-                await self._delete_by_path(fn.path)
+            try:
+                await self._delete_by_id(id)
+            except APIError:
+                pass
+
+        return True
+
+    async def _delete_by_id(self, id: str):
+        response = await self.http_client.do_request(
+            "DELETE",
+            f"/v1/functions/{id}",
+        )
+        if response.status_code != HTTPStatus.NO_CONTENT:
+            raise APIError(
+                f"Failed to delete function {id} with status {response.status_code}"
+            )
+        return True
 
     async def _delete_by_path(self, function_path: str):
         response = await self.http_client.do_request(
             "DELETE",
-            f"/api/v1/functions/by_path/{function_path}",
+            f"/v1/functions/by_path/{function_path}",
         )
-        if response.status_code != HTTPStatus.OK:
+        if response.status_code != HTTPStatus.NO_CONTENT:
             raise APIError(
                 f"Failed to delete function {function_path} with status {response.status_code}"
             )
+        return True
 
     async def chat(
         self, function_path, data: ChatPayload, stream=False, **kwargs
     ) -> FunctionResponse:
         if data.parent_span_uuid is None:
             data.parent_span_uuid = get_current_span_id()
         if stream:
@@ -154,13 +169,15 @@
         )
         async for item in gen:
             yield StreamingChunk(**item)
 
     async def flush_cache(self, id: int) -> None:
         response = await self.http_client.do_request(
             "DELETE",
-            f"/api/v1/functions/{id}/cache",
+            f"/v1/functions/{id}/cache",
         )
         if response.status_code != HTTPStatus.NO_CONTENT:
             raise APIError(
                 f"Failed to flush cache for function with id={id} with status {response.status_code}"
             )
+
+        return True
```

### Comparing `opperai-0.4.0/src/opperai/functions/_functions.py` & `opperai-0.5.0/src/opperai/core/functions/_functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,20 @@
+from http import HTTPStatus
 from typing import Generator, Optional
 
-from opperai._http_clients import _http_client
-from opperai.spans import get_current_span_id
+from opperai.core._http_clients import _http_client
+from opperai.core.spans import get_current_span_id
 from opperai.types import (
     ChatPayload,
     Function,
     FunctionResponse,
     StreamingChunk,
     validate_id_xor_path,
 )
-from http import HTTPStatus
-from opperai.types.exceptions import (
-    APIError,
-    RateLimitError,
-    StructuredGenerationError,
-)
+from opperai.types.exceptions import APIError, RateLimitError, StructuredGenerationError
 
 
 class Functions:
     def __init__(self, http_client: _http_client, default_model: str = None):
         self.http_client = http_client
         self.default_model = default_model
 
@@ -33,28 +29,28 @@
             return fn
 
     def _create(self, function: Function, **kwargs) -> Function:
         if not function.model and self.default_model:
             function.model = self.default_model
         response = self.http_client.do_request(
             "POST",
-            "/api/v1/functions",
+            "/v1/functions",
             json={**function.model_dump(), **kwargs},
         )
         if response.status_code != HTTPStatus.OK:
             raise APIError(
                 f"Failed to create function {function.path} with status {response.status_code}: {response.text}"
             )
 
         return Function.model_validate(response.json())
 
     def update(self, function: Function, **kwargs) -> Function:
         response = self.http_client.do_request(
-            "POST",
-            f"/api/v1/functions/{function.id}",
+            "PATCH",
+            f"/v1/functions/{function.id}",
             json={**function.model_dump(), **kwargs},
         )
         if response.status_code != HTTPStatus.OK:
             raise APIError(
                 f"Failed to update function `{function.path}` with status {response.status_code}: {response.text}"
             )
 
@@ -70,29 +66,29 @@
             return self._get_by_id(id)
         else:
             return None
 
     def _get_by_path(self, function_path: str) -> Optional[Function]:
         response = self.http_client.do_request(
             "GET",
-            f"/api/v1/functions/by_path/{function_path}",
+            f"/v1/functions/by_path/{function_path}",
         )
         if response.status_code == HTTPStatus.NOT_FOUND:
             return None
         if response.status_code != HTTPStatus.OK:
             raise APIError(
                 f"Failed to get function {function_path} with status {response.status_code}"
             )
 
         return Function.model_validate(response.json())
 
     def _get_by_id(self, function_id: str) -> Optional[Function]:
         response = self.http_client.do_request(
             "GET",
-            f"/api/v1/functions/{function_id}",
+            f"/v1/functions/{function_id}",
         )
         if response.status_code == HTTPStatus.NOT_FOUND:
             return None
         if response.status_code != HTTPStatus.OK:
             raise APIError(
                 f"Failed to get function {function_id} with status {response.status_code}"
             )
@@ -103,24 +99,38 @@
     def delete(self, id: str = None, path: str = None) -> bool:
         if path is not None:
             try:
                 return self._delete_by_path(path)
             except APIError:
                 pass
         elif id is not None:
-            fn = self.get(id=id)
-            if fn:
-                return self._delete_by_path(fn.path)
+            try:
+                return self._delete_by_id(id)
+            except APIError:
+                pass
+
+        return True
+
+    def _delete_by_id(self, id: str) -> bool:
+        response = self.http_client.do_request(
+            "DELETE",
+            f"/v1/functions/{id}",
+        )
+        if response.status_code != HTTPStatus.NO_CONTENT:
+            raise APIError(
+                f"Failed to delete function {id} with status {response.status_code}"
+            )
+        return True
 
     def _delete_by_path(self, function_path: str) -> bool:
         response = self.http_client.do_request(
             "DELETE",
-            f"/api/v1/functions/by_path/{function_path}",
+            f"/v1/functions/by_path/{function_path}",
         )
-        if response.status_code != HTTPStatus.OK:
+        if response.status_code != HTTPStatus.NO_CONTENT:
             raise APIError(
                 f"Failed to delete function {function_path} with status {response.status_code}"
             )
         return True
 
     def chat(
         self, function_path, data: ChatPayload, stream=False, **kwargs
@@ -147,28 +157,27 @@
         raise APIError(
             f"Failed to run function {function_path} with status {response.status_code}"
         )
 
     def _chat_stream(
         self, function_path, data: ChatPayload, **kwargs
     ) -> Generator[StreamingChunk, None, None]:
-        serialized_data = data.model_dump()
         gen = self.http_client.stream(
             "POST",
             f"/v1/chat/{function_path}",
-            json={**serialized_data, **kwargs},
+            json={**data.model_dump(), **kwargs},
             params={"stream": "True"},
         )
         for item in gen:
             yield StreamingChunk(**item)
 
     def flush_cache(self, id: int) -> bool:
         response = self.http_client.do_request(
             "DELETE",
-            f"/api/v1/functions/{id}/cache",
+            f"/v1/functions/{id}/cache",
         )
         if response.status_code != HTTPStatus.NO_CONTENT:
             raise APIError(
                 f"Failed to flush cache for function with id={id} with status {response.status_code}"
             )
 
         return True
```

### Comparing `opperai-0.4.0/src/opperai/functions/decorator/_decorator.py` & `opperai-0.5.0/src/opperai/core/functions/decorator/_decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 import inspect
 import json
 import os
 import threading
 from functools import wraps
 from typing import List, get_args, get_origin, get_type_hints
 
-from pydantic import BaseModel
-
-from opperai import AsyncClient, Client
-from opperai.spans import _current_span_id
+from opperai._client import AsyncClient, Client
+from opperai.core.spans import get_current_span_id
+from opperai.core.utils import convert_function_call_to_json
 from opperai.types import CacheConfiguration, ChatPayload, Function, Message
+from pydantic import BaseModel
 
-from ...utils import convert_function_call_to_json
 from ._schemas import get_output_schema
 
 _thread_local = threading.local()
 
 
 @contextlib.contextmanager
 def span_id_context():
@@ -90,15 +89,15 @@
             setup_done = True
 
         @wraps(func)
         async def async_wrapper(*args, **kwargs):
             setup()
             input = convert_function_call_to_json(func, *args, **kwargs)
             payload = ChatPayload(
-                parent_span_uuid=_current_span_id.get(),
+                parent_span_uuid=get_current_span_id(),
                 messages=[
                     Message(role="user", content=json.dumps(input, cls=json_encoder))
                 ],
             )
 
             response = await c.functions.chat(func_path, payload)
             answer = response.json_payload
@@ -117,15 +116,15 @@
                     answer = [get_args(return_type)[0](**item) for item in answer]
             return answer
 
         def sync_wrapper(*args, **kwargs):
             setup()
             input = convert_function_call_to_json(func, *args, **kwargs)
             payload = ChatPayload(
-                parent_span_uuid=_current_span_id.get(),
+                parent_span_uuid=get_current_span_id(),
                 messages=[
                     Message(role="user", content=json.dumps(input, cls=json_encoder))
                 ],
             )
             response = c.functions.chat(func_path, payload)
             answer = response.json_payload
             _thread_local.span_id = response.span_id
```

### Comparing `opperai-0.4.0/src/opperai/functions/decorator/_schemas.py` & `opperai-0.5.0/src/opperai/core/functions/decorator/_schemas.py`

 * *Files identical despite different names*

### Comparing `opperai-0.4.0/src/opperai/indexes/_async_indexes.py` & `opperai-0.5.0/src/opperai/core/indexes/_async_indexes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Optional
 
-from opperai._http_clients import _async_http_client
+from opperai.core._http_clients import _async_http_client
 from opperai.types.exceptions import APIError
 from opperai.types.indexes import (
     Document,
     Filter,
     Index,
     RetrievalResponse,
 )
```

### Comparing `opperai-0.4.0/src/opperai/indexes/_indexes.py` & `opperai-0.5.0/src/opperai/core/indexes/_indexes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import List, Optional
 
-from opperai._http_clients import _http_client
+from pydantic import BaseModel
+
+from opperai.core._http_clients import _http_client
 from opperai.types.exceptions import APIError
 from opperai.types.indexes import (
     Document,
-    Document,
     Filter,
     Index,
     RetrievalResponse,
 )
-from pydantic import BaseModel
 
 
 class RetrieveQuery(BaseModel):
     q: str
     k: int
     filters: Optional[List[Filter]]
```

### Comparing `opperai-0.4.0/src/opperai/spans/_async_spans.py` & `opperai-0.5.0/src/opperai/core/spans/_async_spans.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from typing import Any, Dict
 from uuid import UUID
 
-from opperai._http_clients import _async_http_client
+from opperai.core._http_clients import _async_http_client
+from opperai.core.utils import DateTimeEncoder
 from opperai.types.exceptions import APIError
 from opperai.types.spans import Span, SpanMetric
-from opperai.utils import DateTimeEncoder
 
 
 class AsyncSpans:
     def __init__(self, http_client: _async_http_client):
         self.http_client = http_client
 
     async def create(self, span: Span, **kwargs) -> Span:
```

### Comparing `opperai-0.4.0/src/opperai/spans/_decorator.py` & `opperai-0.5.0/src/opperai/core/spans/_decorator.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import json
 import os
 from contextlib import contextmanager
 from functools import wraps
 from typing import Callable, Optional
 from uuid import uuid4
 
-from opperai import Client
-from opperai.spans import _current_span_id
+from opperai._client import Client
+from opperai.core.spans import _current_span_id
+from opperai.core.utils import convert_function_call_to_json
 from opperai.types.spans import Span
-from opperai.utils import convert_function_call_to_json
 
 
 class SpanContext:
     def __init__(self, client: Client, span_uuid: str):
         self.client = client
         self.span_uuid = span_uuid
         self.output = None
```

### Comparing `opperai-0.4.0/src/opperai/spans/_spans.py` & `opperai-0.5.0/src/opperai/core/spans/_spans.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 from http import HTTPStatus
 from typing import Any, Dict
 from uuid import UUID
 
-from opperai._http_clients import _http_client
+from opperai.core._http_clients import _http_client
+from opperai.core.utils import DateTimeEncoder
 from opperai.types.exceptions import APIError
 from opperai.types.spans import Span, SpanMetric
-from opperai.utils import DateTimeEncoder
 
 
 class Spans:
     def __init__(self, http_client: _http_client):
         self.http_client = http_client
 
     def create(self, span: Span, **kwargs) -> str:
```

### Comparing `opperai-0.4.0/src/opperai/types/__init__.py` & `opperai-0.5.0/src/opperai/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # ruff: noqa: F401
 from typing import Any, Dict, List, Optional, Union
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
 
+from .indexes import Document
 from .spans import SpanMetric
 from .validators import validate_id_xor_path
 
 
 class Message(BaseModel):
     role: str
     content: str
```

### Comparing `opperai-0.4.0/src/opperai/types/indexes.py` & `opperai-0.5.0/src/opperai/types/indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.4.0/src/opperai/types/spans.py` & `opperai-0.5.0/src/opperai/types/spans.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 from typing import Optional
 from uuid import UUID
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel
 
 
 class Span(BaseModel):
     uuid: Optional[UUID] = None
     project: Optional[str] = None
     name: Optional[str] = None
     input: Optional[str] = None
@@ -18,9 +18,9 @@
     meta: Optional[dict] = None
     evaluations: Optional[dict] = None
     score: Optional[int] = None
 
 
 class SpanMetric(BaseModel):
     dimension: Optional[str] = None
-    score: Optional[float] = Field(None, ge=0, le=1)
+    value: Optional[float] = None
     comment: Optional[str] = None
```

### Comparing `opperai-0.4.0/src/opperai/types/validators.py` & `opperai-0.5.0/src/opperai/types/validators.py`

 * *Files identical despite different names*

### Comparing `opperai-0.4.0/src/opperai/utils/__init__.py` & `opperai-0.5.0/src/opperai/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `opperai-0.4.0/tests/conftest.py` & `opperai-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `opperai-0.4.0/tests/test_async_functions.py` & `opperai-0.5.0/tests/test_async_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.4.0/tests/test_async_indexes.py` & `opperai-0.5.0/tests/test_async_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.4.0/tests/test_async_spans.py` & `opperai-0.5.0/tests/test_async_spans.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,9 +71,9 @@
             name="name",
             input="input",
             start_time=datetime(2021, 1, 1, 0, 0, 0, 0),
         ),
         aclient,
     ) as _span:
         await aclient.spans.save_metric(
-            _span.uuid, SpanMetric(dimension="dim", score=0.5, comment="comment")
+            _span.uuid, SpanMetric(dimension="dim", value=0.5, comment="comment")
         )
```

### Comparing `opperai-0.4.0/tests/test_decorator.py` & `opperai-0.5.0/tests/test_decorator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from typing import Dict, List, Optional, Union
 from unittest.mock import MagicMock, patch
 
 import pytest
 from jsonschema import validate
 from opperai import fn
-from opperai.functions.decorator._schemas import type_to_json_schema
-from opperai.utils import (
-    convert_function_call_to_json,
-)
+from opperai.core.functions.decorator._schemas import type_to_json_schema
+from opperai.core.utils import convert_function_call_to_json
 from pydantic import BaseModel
 
 
-@patch("opperai._http_clients._http_client.do_request")
+@patch("opperai.core._http_clients._http_client.do_request")
 def test_decorator(mock_do_request):
     mock_do_request.side_effect = [
         MagicMock(status_code=404),
         MagicMock(
             status_code=200,
             json=lambda: {
                 "id": 1,
@@ -46,15 +44,15 @@
     def translate_list(text: str, target_languages: List[str]) -> List[str]:
         """Translate text to a list of target languages."""
 
     assert translate("Hello", "es") == "Hola"
     assert translate_list("Hello", ["es", "fr"]) == ["Hola", "Bonjour"]
 
 
-@patch("opperai._http_clients._http_client.do_request")
+@patch("opperai.core._http_clients._http_client.do_request")
 def test_decorator_supply_model(mock_do_request):
     mock_do_request.side_effect = [
         MagicMock(status_code=404),
         MagicMock(
             status_code=200,
             json=lambda: {
                 "id": 1,
```

### Comparing `opperai-0.4.0/tests/test_functions.py` & `opperai-0.5.0/tests/test_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from opperai import Client
-from opperai.types import CacheConfiguration, ChatPayload, Function, Message
 from contextlib import contextmanager
+
 import pytest
+from opperai import Client
+from opperai.types import CacheConfiguration, ChatPayload, Function, Message
 from opperai.types.exceptions import StructuredGenerationError
 
 
 @contextmanager
 def _function(desc: Function, c: Client):
     function = c.functions.create(desc)
     yield function
```

### Comparing `opperai-0.4.0/tests/test_indexes.py` & `opperai-0.5.0/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.4.0/tests/test_spans.py` & `opperai-0.5.0/tests/test_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.4.0/tests/test_trace_decorator.py` & `opperai-0.5.0/tests/test_trace_decorator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,14 @@
-import os
 import uuid
 from unittest.mock import MagicMock, patch
-from datetime import datetime
 
-from uuid import uuid4
-from opperai.types.spans import Span
-from opperai import Client
+from opperai import Client, trace
 
-from opperai import trace
 
-
-@patch("opperai._http_clients._http_client.do_request")
+@patch("opperai.core._http_clients._http_client.do_request")
 def test_decorator(mock_do_request):
     mock_do_request.side_effect = [
         MagicMock(status_code=200, json=lambda: {"uuid": str(uuid.uuid4())}),
         MagicMock(status_code=200, json=lambda: {"uuid": str(uuid.uuid4())}),
     ]
 
     @trace(client=Client(api_key="temporary", api_url="temporary"))
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,157 +1,144 @@
 interactions:
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_async_chat
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_sync_chat_stream
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:17:38 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_async_chat", "description": "Translate
+    body: '{"id": null, "path": "test/sdk/test_sync_chat_stream", "description": "Translate
       to French", "input_schema": null, "out_schema": null, "instructions": "Translate
       to French", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
       null, "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '299'
+      - '305'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/api/v1/functions
+    uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":48,"path":"test/sdk/test_async_chat","description":"Translate
+      string: '{"id":27,"path":"test/sdk/test_sync_chat_stream","description":"Translate
         to French","input_schema":null,"out_schema":null,"instructions":"Translate
-        to French","few_shot":false,"few_shot_count":2,"dataset_uuid":"7223ad03-9f13-433d-a2c7-27052da2195d","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+        to French","few_shot":false,"few_shot_count":2,"dataset_uuid":"1f6ce832-10cd-4541-b338-3c0f02996a49","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '400'
+      - '406'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:17:38 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
+    body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      content-length:
-      - '78'
-      content-type:
-      - application/json
-      user-agent:
-      - python-httpx/0.27.0
-    method: POST
-    uri: http://localhost:8000/v1/chat/test/sdk/test_async_chat
+    method: GET
+    uri: http://localhost:8000/v1/functions/27
   response:
     body:
-      string: '{"span_id":"84b5d901-47f0-4abd-8cf4-d5dc18800756","message":"Bonjour","json_payload":null,"error":null,"context":null,"cached":false}'
+      string: '{"id":27,"path":"test/sdk/test_sync_chat_stream","description":"Translate
+        to French","input_schema":null,"out_schema":null,"instructions":"Translate
+        to French","few_shot":false,"few_shot_count":2,"dataset_uuid":"1f6ce832-10cd-4541-b338-3c0f02996a49","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '133'
+      - '484'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:17:38 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: ''
+    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
     headers:
       accept:
-      - '*/*'
-      accept-encoding:
-      - gzip, deflate
+      - text/event-stream
+      cache-control:
+      - no-store
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/48
+      content-length:
+      - '78'
+      content-type:
+      - application/json
+    method: POST
+    uri: http://localhost:8000/v1/chat/test/sdk/test_sync_chat_stream?stream=True
   response:
     body:
-      string: '{"id":48,"path":"test/sdk/test_async_chat","description":"Translate
-        to French","input_schema":null,"dataset_uuid":"7223ad03-9f13-433d-a2c7-27052da2195d","out_schema":null,"instructions":"Translate
-        to French","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: "data: {\"span_id\": \"0199c47d-b130-4346-a06c-bbdce9e53e18\"}\r\n\r\ndata:
+        {\"delta\": \"Bonjour\"}\r\n\r\n"
     headers:
-      content-length:
-      - '383'
+      Transfer-Encoding:
+      - chunked
+      cache-control:
+      - no-cache
+      connection:
+      - keep-alive
       content-type:
-      - application/json
+      - text/event-stream; charset=utf-8
       date:
-      - Thu, 11 Apr 2024 16:23:55 GMT
+      - Thu, 02 May 2024 09:17:38 GMT
       server:
       - uvicorn
+      x-accel-buffering:
+      - 'no'
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_async_chat
+    uri: http://localhost:8000/v1/functions/27
   response:
     body:
-      string: '{"detail":"Function and associated generations deleted successfully"}'
+      string: ''
     headers:
-      content-length:
-      - '69'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:55 GMT
+      - Thu, 02 May 2024 09:17:39 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 204
+      message: No Content
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,166 +1,130 @@
 interactions:
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_async_chat_stream
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:55 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_async_chat_stream", "description":
-      "Translate to French", "input_schema": null, "out_schema": null, "instructions":
-      "Translate to French", "model": null, "index_ids": [], "use_semantic_search":
-      null, "few_shot": null, "few_shot_count": null, "cache_configuration": null}'
+    body: '{"id": null, "path": "test/sdk/test_get", "description": "Test function",
+      "input_schema": null, "out_schema": null, "instructions": "Do something", "model":
+      null, "index_ids": [], "use_semantic_search": null, "few_shot": null, "few_shot_count":
+      null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '306'
+      - '279'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/api/v1/functions
+    uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":49,"path":"test/sdk/test_async_chat_stream","description":"Translate
-        to French","input_schema":null,"out_schema":null,"instructions":"Translate
-        to French","few_shot":false,"few_shot_count":2,"dataset_uuid":"0fca4d22-aae7-4ed5-a0a8-0dbde51959f9","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"id":68,"path":"test/sdk/test_get","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
+        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"0499d814-14f6-46cc-afd3-f8405b14c4d0","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '407'
+      - '380'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:55 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
+    body: ''
     headers:
       accept:
-      - text/event-stream
-      accept-encoding:
-      - gzip, deflate
-      cache-control:
-      - no-store
+      - '*/*'
       connection:
       - keep-alive
-      content-length:
-      - '78'
-      content-type:
-      - application/json
-      user-agent:
-      - python-httpx/0.27.0
-    method: POST
-    uri: http://localhost:8000/v1/chat/test/sdk/test_async_chat_stream?stream=True
+    method: GET
+    uri: http://localhost:8000/v1/functions/68
   response:
     body:
-      string: "data: {\"span_id\": \"7e5513a3-70a8-4442-a901-e7bb280e1834\"}\r\n\r\ndata:
-        {\"delta\": \"Bonjour\"}\r\n\r\n"
+      string: '{"id":68,"path":"test/sdk/test_get","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
+        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"0499d814-14f6-46cc-afd3-f8405b14c4d0","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
-      Transfer-Encoding:
-      - chunked
-      cache-control:
-      - no-cache
-      connection:
-      - keep-alive
+      content-length:
+      - '458'
       content-type:
-      - text/event-stream; charset=utf-8
+      - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:55 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
-      x-accel-buffering:
-      - 'no'
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/49
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get
   response:
     body:
-      string: '{"id":49,"path":"test/sdk/test_async_chat_stream","description":"Translate
-        to French","input_schema":null,"dataset_uuid":"0fca4d22-aae7-4ed5-a0a8-0dbde51959f9","out_schema":null,"instructions":"Translate
-        to French","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '{"id":68,"path":"test/sdk/test_get","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
+        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"0499d814-14f6-46cc-afd3-f8405b14c4d0","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '390'
+      - '458'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:59 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_async_chat_stream
+    uri: http://localhost:8000/v1/functions/68
   response:
     body:
-      string: '{"detail":"Function and associated generations deleted successfully"}'
+      string: ''
     headers:
-      content-length:
-      - '69'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:59 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 204
+      message: No Content
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,124 +1,133 @@
 interactions:
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_create_function_async
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_chat
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:17:37 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_create_function_async", "description":
-      "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
-      something", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
+    body: '{"id": null, "path": "test/sdk/test_chat", "description": "Translate to
+      French", "input_schema": null, "out_schema": null, "instructions": "Translate
+      to French", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
       null, "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '297'
+      - '293'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/api/v1/functions
+    uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":42,"path":"test/sdk/test_create_function_async","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"8bb86025-9c91-4930-8f26-ac97cc7fb9a2","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"id":26,"path":"test/sdk/test_chat","description":"Translate to French","input_schema":null,"out_schema":null,"instructions":"Translate
+        to French","few_shot":false,"few_shot_count":2,"dataset_uuid":"6b3d0427-baac-4be2-ad81-6b15bfbec58a","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '398'
+      - '394'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:17:37 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/42
+    uri: http://localhost:8000/v1/functions/26
   response:
     body:
-      string: '{"id":42,"path":"test/sdk/test_create_function_async","description":"Test
-        function","input_schema":null,"dataset_uuid":"8bb86025-9c91-4930-8f26-ac97cc7fb9a2","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '{"id":26,"path":"test/sdk/test_chat","description":"Translate to French","input_schema":null,"out_schema":null,"instructions":"Translate
+        to French","few_shot":false,"few_shot_count":2,"dataset_uuid":"6b3d0427-baac-4be2-ad81-6b15bfbec58a","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '381'
+      - '472'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:17:37 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: ''
+    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: DELETE
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_create_function_async
+      content-length:
+      - '78'
+      content-type:
+      - application/json
+    method: POST
+    uri: http://localhost:8000/v1/chat/test/sdk/test_chat
   response:
     body:
-      string: '{"detail":"Function and associated generations deleted successfully"}'
+      string: '{"span_id":"41f52b87-85c1-4495-a89a-a4b24d983f33","message":"Bonjour","json_payload":null,"error":null,"context":null,"cached":false}'
     headers:
       content-length:
-      - '69'
+      - '133'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:17:37 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
+- request:
+    body: ''
+    headers:
+      accept:
+      - '*/*'
+      connection:
+      - keep-alive
+    method: DELETE
+    uri: http://localhost:8000/v1/functions/26
+  response:
+    body:
+      string: ''
+    headers:
+      content-type:
+      - application/json
+      date:
+      - Thu, 02 May 2024 09:17:38 GMT
+      server:
+      - uvicorn
+    status:
+      code: 204
+      message: No Content
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,152 +1,105 @@
 interactions:
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get_by_path
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:22:31 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_delete_function", "description": "Test
+    body: '{"id": null, "path": "test/sdk/test_get_by_path", "description": "Test
       function", "input_schema": null, "out_schema": null, "instructions": "Do something",
       "model": null, "index_ids": [], "use_semantic_search": null, "few_shot": null,
       "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '291'
+      - '287'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/api/v1/functions
+    uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":47,"path":"test/sdk/test_delete_function","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"f3529aba-20a8-407b-9f68-b6eca214d9d6","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"id":58,"path":"test/sdk/test_get_by_path","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
+        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"02d0f301-270e-4014-be08-c3cfc2017d18","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '392'
+      - '388'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:22:31 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/47
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get_by_path
   response:
     body:
-      string: '{"id":47,"path":"test/sdk/test_delete_function","description":"Test
-        function","input_schema":null,"dataset_uuid":"f3529aba-20a8-407b-9f68-b6eca214d9d6","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '{"id":58,"path":"test/sdk/test_get_by_path","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
+        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"02d0f301-270e-4014-be08-c3cfc2017d18","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '375'
+      - '466'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:22:31 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function
+    uri: http://localhost:8000/v1/functions/58
   response:
     body:
-      string: '{"detail":"Function and associated generations deleted successfully"}'
+      string: ''
     headers:
-      content-length:
-      - '69'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:22:31 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
-- request:
-    body: ''
-    headers:
-      accept:
-      - '*/*'
-      accept-encoding:
-      - gzip, deflate
-      connection:
-      - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/47
-  response:
-    body:
-      string: '{"detail":"Function not found"}'
-    headers:
-      content-length:
-      - '31'
-      content-type:
-      - application/json
-      date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
-      server:
-      - uvicorn
-    status:
-      code: 404
-      message: Not Found
+      code: 204
+      message: No Content
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_id.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,209 +1,141 @@
 interactions:
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_id
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_create_function_with_cache_async
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Mon, 08 Apr 2024 13:34:13 GMT
+      - Thu, 02 May 2024 10:52:29 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_delete_function_by_id", "description":
-      "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
-      something", "model": null, "index_ids": null, "use_semantic_search": null, "few_shot":
-      null, "few_shot_count": null, "cache_configuration": null}'
+    body: '{"id": null, "path": "test/sdk/test_create_function_with_cache_async",
+      "description": "Test function", "input_schema": null, "out_schema": null, "instructions":
+      "Do something", "model": null, "index_ids": [], "use_semantic_search": null,
+      "few_shot": null, "few_shot_count": null, "cache_configuration": {"exact_match_cache_ttl":
+      10, "semantic_cache_threshold": null, "semantic_cache_ttl": null}}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '299'
+      - '395'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/api/v1/functions
+    uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":117}'
+      string: '{"id":73,"path":"test/sdk/test_create_function_with_cache_async","description":"Test
+        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"8628e6fd-7519-4f50-9298-3f8da3db4f33","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '10'
+      - '409'
       content-type:
       - application/json
       date:
-      - Mon, 08 Apr 2024 13:34:13 GMT
+      - Thu, 02 May 2024 10:52:29 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: ''
+    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/117
-  response:
-    body:
-      string: '{"id":117,"path":"test/sdk/test_delete_function_by_id","description":"Test
-        function","input_schema":null,"dataset_uuid":"7984e90d-798e-4b1a-b54b-4701878c96d2","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
-    headers:
       content-length:
-      - '382'
+      - '78'
       content-type:
       - application/json
-      date:
-      - Mon, 08 Apr 2024 13:34:13 GMT
-      server:
-      - uvicorn
-    status:
-      code: 200
-      message: OK
-- request:
-    body: ''
-    headers:
-      accept:
-      - '*/*'
-      accept-encoding:
-      - gzip, deflate
-      connection:
-      - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/117
+    method: POST
+    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache_async
   response:
     body:
-      string: '{"id":117,"path":"test/sdk/test_delete_function_by_id","description":"Test
-        function","input_schema":null,"dataset_uuid":"7984e90d-798e-4b1a-b54b-4701878c96d2","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '{"span_id":"1fc4ce18-b522-4015-bbb3-a84a39c79af4","message":"Hello!
+        How can I assist you today? If you have any questions or need information
+        on a topic, feel free to ask.","json_payload":null,"error":null,"context":null,"cached":false}'
     headers:
       content-length:
-      - '382'
+      - '236'
       content-type:
       - application/json
       date:
-      - Mon, 08 Apr 2024 13:34:13 GMT
+      - Thu, 02 May 2024 10:52:30 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: ''
+    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: DELETE
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_id
-  response:
-    body:
-      string: '{"detail":"Function and associated generations deleted successfully"}'
-    headers:
       content-length:
-      - '69'
+      - '78'
       content-type:
       - application/json
-      date:
-      - Mon, 08 Apr 2024 13:34:13 GMT
-      server:
-      - uvicorn
-    status:
-      code: 200
-      message: OK
-- request:
-    body: ''
-    headers:
-      accept:
-      - '*/*'
-      accept-encoding:
-      - gzip, deflate
-      connection:
-      - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/117
+    method: POST
+    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache_async
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"span_id":"9688cdc4-261e-4fe1-8df1-0a2282dd3186","message":"Hello!
+        How can I assist you today? If you have any questions or need information
+        on a topic, feel free to ask.","json_payload":null,"error":null,"context":null,"cached":true}'
     headers:
       content-length:
-      - '31'
+      - '235'
       content-type:
       - application/json
       date:
-      - Mon, 08 Apr 2024 13:34:13 GMT
+      - Thu, 02 May 2024 10:52:32 GMT
       server:
       - uvicorn
     status:
-      code: 404
-      message: Not Found
+      code: 200
+      message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/117
+    method: DELETE
+    uri: http://localhost:8000/v1/functions/73
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: ''
     headers:
-      content-length:
-      - '31'
       content-type:
       - application/json
       date:
-      - Mon, 08 Apr 2024 13:34:13 GMT
+      - Thu, 02 May 2024 10:52:32 GMT
       server:
       - uvicorn
     status:
-      code: 404
-      message: Not Found
+      code: 204
+      message: No Content
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_path.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,179 +1,141 @@
 interactions:
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_path
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_create_function_with_cache
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Mon, 08 Apr 2024 13:34:13 GMT
+      - Thu, 02 May 2024 09:17:39 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_delete_function_by_path", "description":
+    body: '{"id": null, "path": "test/sdk/test_create_function_with_cache", "description":
       "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
-      something", "model": null, "index_ids": null, "use_semantic_search": null, "few_shot":
-      null, "few_shot_count": null, "cache_configuration": null}'
+      something", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
+      null, "few_shot_count": null, "cache_configuration": {"exact_match_cache_ttl":
+      10, "semantic_cache_threshold": null, "semantic_cache_ttl": null}}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '301'
+      - '389'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/api/v1/functions
+    uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":118}'
+      string: '{"id":28,"path":"test/sdk/test_create_function_with_cache","description":"Test
+        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"0ddeb3de-617d-4442-afc5-e51c05c833af","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '10'
+      - '403'
       content-type:
       - application/json
       date:
-      - Mon, 08 Apr 2024 13:34:13 GMT
+      - Thu, 02 May 2024 09:17:39 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: ''
+    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/118
-  response:
-    body:
-      string: '{"id":118,"path":"test/sdk/test_delete_function_by_path","description":"Test
-        function","input_schema":null,"dataset_uuid":"98cf36c4-3b86-4952-abb8-dd418620b5c5","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
-    headers:
       content-length:
-      - '384'
+      - '78'
       content-type:
       - application/json
-      date:
-      - Mon, 08 Apr 2024 13:34:13 GMT
-      server:
-      - uvicorn
-    status:
-      code: 200
-      message: OK
-- request:
-    body: ''
-    headers:
-      accept:
-      - '*/*'
-      accept-encoding:
-      - gzip, deflate
-      connection:
-      - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: DELETE
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_path
+    method: POST
+    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache
   response:
     body:
-      string: '{"detail":"Function and associated generations deleted successfully"}'
+      string: '{"span_id":"ca79b63e-76d3-4962-91bb-83d4e6de549b","message":"Hello!
+        How can I assist you today? If you have any questions or need information
+        on a topic, feel free to ask.","json_payload":null,"error":null,"context":null,"cached":false}'
     headers:
       content-length:
-      - '69'
+      - '236'
       content-type:
       - application/json
       date:
-      - Mon, 08 Apr 2024 13:34:13 GMT
+      - Thu, 02 May 2024 09:17:39 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: ''
+    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_path
+      content-length:
+      - '78'
+      content-type:
+      - application/json
+    method: POST
+    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"span_id":"0794f09f-22e3-4a1a-8ebf-ad03922d636f","message":"Hello!
+        How can I assist you today? If you have any questions or need information
+        on a topic, feel free to ask.","json_payload":null,"error":null,"context":null,"cached":true}'
     headers:
       content-length:
-      - '31'
+      - '235'
       content-type:
       - application/json
       date:
-      - Mon, 08 Apr 2024 13:34:13 GMT
+      - Thu, 02 May 2024 09:17:41 GMT
       server:
       - uvicorn
     status:
-      code: 404
-      message: Not Found
+      code: 200
+      message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/118
+    method: DELETE
+    uri: http://localhost:8000/v1/functions/28
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: ''
     headers:
-      content-length:
-      - '31'
       content-type:
       - application/json
       date:
-      - Mon, 08 Apr 2024 13:34:13 GMT
+      - Thu, 02 May 2024 09:17:42 GMT
       server:
       - uvicorn
     status:
-      code: 404
-      message: Not Found
+      code: 204
+      message: No Content
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,181 +1,167 @@
 interactions:
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_get
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_update_function
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"id":23,"path":"test/sdk/test_update_function","description":"Test
+        function","input_schema":null,"out_schema":null,"instructions":"Do something
+        else","few_shot":false,"few_shot_count":2,"dataset_uuid":"22a1b039-cf65-441a-81b4-6306625067b9","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":2,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '31'
+      - '475'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:17:37 GMT
       server:
       - uvicorn
     status:
-      code: 404
-      message: Not Found
+      code: 200
+      message: OK
 - request:
-    body: '{"id": null, "path": "test/sdk/test_get", "description": "Test function",
-      "input_schema": null, "out_schema": null, "instructions": "Do something", "model":
-      null, "index_ids": [], "use_semantic_search": null, "few_shot": null, "few_shot_count":
-      null, "cache_configuration": null}'
+    body: '{"id": 23, "path": "test/sdk/test_update_function", "description": "Test
+      function", "input_schema": null, "out_schema": null, "instructions": "Do something",
+      "model": null, "index_ids": [], "use_semantic_search": null, "few_shot": null,
+      "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '279'
+      - '289'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
-    method: POST
-    uri: http://localhost:8000/api/v1/functions
+    method: PATCH
+    uri: http://localhost:8000/v1/functions/23
   response:
     body:
-      string: '{"id":45,"path":"test/sdk/test_get","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
-        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"1acd2324-dad7-47a4-a48e-f59bc054eda8","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"id":23,"path":"test/sdk/test_update_function","description":"Test
+        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"22a1b039-cf65-441a-81b4-6306625067b9","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":3,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '380'
+      - '470'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:17:37 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/45
+    uri: http://localhost:8000/v1/functions/23
   response:
     body:
-      string: '{"id":45,"path":"test/sdk/test_get","description":"Test function","input_schema":null,"dataset_uuid":"1acd2324-dad7-47a4-a48e-f59bc054eda8","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '{"id":23,"path":"test/sdk/test_update_function","description":"Test
+        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"22a1b039-cf65-441a-81b4-6306625067b9","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":3,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '363'
+      - '470'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:17:37 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: ''
+    body: '{"id": 23, "path": "test/sdk/test_update_function", "description": "Test
+      function", "input_schema": null, "out_schema": null, "instructions": "Do something
+      else", "model": "azure/gpt4-eu", "index_ids": [], "use_semantic_search": false,
+      "few_shot": false, "few_shot_count": 2, "cache_configuration": {"exact_match_cache_ttl":
+      0, "semantic_cache_threshold": 0.95, "semantic_cache_ttl": 0}}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_get
+      content-length:
+      - '387'
+      content-type:
+      - application/json
+    method: PATCH
+    uri: http://localhost:8000/v1/functions/23
   response:
     body:
-      string: '{"id":45,"path":"test/sdk/test_get","description":"Test function","input_schema":null,"dataset_uuid":"1acd2324-dad7-47a4-a48e-f59bc054eda8","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '{"id":23,"path":"test/sdk/test_update_function","description":"Test
+        function","input_schema":null,"out_schema":null,"instructions":"Do something
+        else","few_shot":false,"few_shot_count":2,"dataset_uuid":"22a1b039-cf65-441a-81b4-6306625067b9","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":4,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '363'
+      - '475'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:17:37 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/45
+    uri: http://localhost:8000/v1/functions/23
   response:
     body:
-      string: '{"id":45,"path":"test/sdk/test_get","description":"Test function","input_schema":null,"dataset_uuid":"1acd2324-dad7-47a4-a48e-f59bc054eda8","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '{"id":23,"path":"test/sdk/test_update_function","description":"Test
+        function","input_schema":null,"out_schema":null,"instructions":"Do something
+        else","few_shot":false,"few_shot_count":2,"dataset_uuid":"22a1b039-cf65-441a-81b4-6306625067b9","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":4,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '363'
+      - '475'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:17:37 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_get
+    uri: http://localhost:8000/v1/functions/23
   response:
     body:
-      string: '{"detail":"Function and associated generations deleted successfully"}'
+      string: ''
     headers:
-      content-length:
-      - '69'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:17:37 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 204
+      message: No Content
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,152 +1,105 @@
 interactions:
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_get_by_id
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get_by_id
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
     body: '{"id": null, "path": "test/sdk/test_get_by_id", "description": "Test function",
       "input_schema": null, "out_schema": null, "instructions": "Do something", "model":
       null, "index_ids": [], "use_semantic_search": null, "few_shot": null, "few_shot_count":
       null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
       - '285'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/api/v1/functions
+    uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":43,"path":"test/sdk/test_get_by_id","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
-        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"69bf17eb-e694-4b0d-823e-55898260c1ef","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"id":66,"path":"test/sdk/test_get_by_id","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
+        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"50969b89-33ce-4a1b-9676-1667695aa78e","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
       - '386'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/43
+    uri: http://localhost:8000/v1/functions/66
   response:
     body:
-      string: '{"id":43,"path":"test/sdk/test_get_by_id","description":"Test function","input_schema":null,"dataset_uuid":"69bf17eb-e694-4b0d-823e-55898260c1ef","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '{"id":66,"path":"test/sdk/test_get_by_id","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
+        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"50969b89-33ce-4a1b-9676-1667695aa78e","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '369'
+      - '464'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/43
-  response:
-    body:
-      string: '{"id":43,"path":"test/sdk/test_get_by_id","description":"Test function","input_schema":null,"dataset_uuid":"69bf17eb-e694-4b0d-823e-55898260c1ef","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
-    headers:
-      content-length:
-      - '369'
-      content-type:
-      - application/json
-      date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
-      server:
-      - uvicorn
-    status:
-      code: 200
-      message: OK
-- request:
-    body: ''
-    headers:
-      accept:
-      - '*/*'
-      accept-encoding:
-      - gzip, deflate
-      connection:
-      - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_get_by_id
+    uri: http://localhost:8000/v1/functions/66
   response:
     body:
-      string: '{"detail":"Function and associated generations deleted successfully"}'
+      string: ''
     headers:
-      content-length:
-      - '69'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 204
+      message: No Content
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,152 +1,181 @@
 interactions:
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_get_by_path
+    uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '[]'
     headers:
       content-length:
-      - '31'
+      - '2'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:18:07 GMT
       server:
       - uvicorn
     status:
-      code: 404
-      message: Not Found
+      code: 200
+      message: OK
 - request:
-    body: '{"id": null, "path": "test/sdk/test_get_by_path", "description": "Test
-      function", "input_schema": null, "out_schema": null, "instructions": "Do something",
-      "model": null, "index_ids": [], "use_semantic_search": null, "few_shot": null,
-      "few_shot_count": null, "cache_configuration": null}'
+    body: '{"name": "test_list_indexes"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '287'
+      - '29'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/api/v1/functions
+    uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":44,"path":"test/sdk/test_get_by_path","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
-        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"3c605946-0432-463c-9038-c736877877aa","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"id":6,"name":"test_list_indexes","files":[],"created_at":"2024-05-02T09:18:07.426246Z"}'
     headers:
       content-length:
-      - '388'
+      - '89'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:18:07 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_get_by_path
+    uri: http://localhost:8000/v1/indexes
+  response:
+    body:
+      string: '[{"id":6,"org_id":1,"org_name":null,"name":"test_list_indexes","created_by":"Mattias
+        Lundell","created_at":"2024-05-02T09:18:07.426246Z","updated_at":"2024-05-02T09:18:07.426246Z","count":0}]'
+    headers:
+      content-length:
+      - '191'
+      content-type:
+      - application/json
+      date:
+      - Thu, 02 May 2024 09:18:07 GMT
+      server:
+      - uvicorn
+    status:
+      code: 200
+      message: OK
+- request:
+    body: '{"name": "test_list_indexes_2"}'
+    headers:
+      accept:
+      - '*/*'
+      connection:
+      - keep-alive
+      content-length:
+      - '31'
+      content-type:
+      - application/json
+    method: POST
+    uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":44,"path":"test/sdk/test_get_by_path","description":"Test function","input_schema":null,"dataset_uuid":"3c605946-0432-463c-9038-c736877877aa","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '{"id":7,"name":"test_list_indexes_2","files":[],"created_at":"2024-05-02T09:18:07.459416Z"}'
     headers:
       content-length:
-      - '371'
+      - '91'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:18:07 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/44
+    uri: http://localhost:8000/v1/indexes
+  response:
+    body:
+      string: '[{"id":6,"org_id":1,"org_name":null,"name":"test_list_indexes","created_by":"Mattias
+        Lundell","created_at":"2024-05-02T09:18:07.426246Z","updated_at":"2024-05-02T09:18:07.426246Z","count":0},{"id":7,"org_id":1,"org_name":null,"name":"test_list_indexes_2","created_by":"Mattias
+        Lundell","created_at":"2024-05-02T09:18:07.459416Z","updated_at":"2024-05-02T09:18:07.459416Z","count":0}]'
+    headers:
+      content-length:
+      - '383'
+      content-type:
+      - application/json
+      date:
+      - Thu, 02 May 2024 09:18:07 GMT
+      server:
+      - uvicorn
+    status:
+      code: 200
+      message: OK
+- request:
+    body: ''
+    headers:
+      accept:
+      - '*/*'
+      connection:
+      - keep-alive
+    method: DELETE
+    uri: http://localhost:8000/v1/indexes/7
   response:
     body:
-      string: '{"id":44,"path":"test/sdk/test_get_by_path","description":"Test function","input_schema":null,"dataset_uuid":"3c605946-0432-463c-9038-c736877877aa","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: 'true'
     headers:
       content-length:
-      - '371'
+      - '4'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:18:07 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_get_by_path
+    uri: http://localhost:8000/v1/indexes/6
   response:
     body:
-      string: '{"detail":"Function and associated generations deleted successfully"}'
+      string: 'true'
     headers:
       content-length:
-      - '69'
+      - '4'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 09:18:07 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,161 +1,118 @@
 interactions:
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_update_function
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_failed_structured_generation
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 10:46:24 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_update_function", "description": "Test
-      function", "input_schema": null, "out_schema": null, "instructions": "Do something",
-      "model": null, "index_ids": [], "use_semantic_search": null, "few_shot": null,
-      "few_shot_count": null, "cache_configuration": null}'
+    body: '{"id": null, "path": "test/sdk/test_failed_structured_generation", "description":
+      "test structured generation exception", "input_schema": null, "out_schema":
+      {"type": "object", "properties": {"universityName": {"type": "string"}, "location":
+      {"type": "string"}, "departments": {"type": "array", "items": {"type": "object",
+      "properties": {"departmentName": {"type": "string"}, "head": {"type": "string"},
+      "courses": {"type": "array", "items": {"type": "object", "properties": {"courseId":
+      {"type": "string"}, "courseName": {"type": "string"}, "credits": {"type": "integer",
+      "minimum": 1, "maximum": 10}}, "required": ["courseId", "courseName", "credits"]}}},
+      "required": ["departmentName", "head", "courses"]}}}, "required": ["universityName",
+      "location", "departments"]}, "instructions": "You translate the incoming text
+      to french", "model": "mistral/mistral-tiny-eu", "index_ids": [], "use_semantic_search":
+      null, "few_shot": null, "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '291'
+      - '985'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/api/v1/functions
+    uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":46,"path":"test/sdk/test_update_function","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"a12f84b0-1d8d-4e01-b9f1-1a285dc99b74","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"id":64,"path":"test/sdk/test_failed_structured_generation","description":"test
+        structured generation exception","input_schema":null,"out_schema":null,"instructions":"You
+        translate the incoming text to french","few_shot":false,"few_shot_count":2,"dataset_uuid":"ab9dbbaf-e647-4b5b-a69c-e3e768e2f11d","use_semantic_search":false,"model":"mistral/mistral-tiny-eu","language_model_id":4,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '392'
+      - '467'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 10:46:24 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"id": 46, "path": "test/sdk/test_update_function", "description": "Test
-      function", "input_schema": null, "out_schema": null, "instructions": "Do something
-      else", "model": "azure/gpt4-eu", "index_ids": [], "use_semantic_search": false,
-      "few_shot": false, "few_shot_count": 2, "cache_configuration": null}'
+    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '304'
+      - '78'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/api/v1/functions/46
+    uri: http://localhost:8000/v1/chat/test/sdk/test_failed_structured_generation
   response:
     body:
-      string: '{"id":46,"path":"test/sdk/test_update_function","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something
-        else","few_shot":false,"few_shot_count":2,"dataset_uuid":"a12f84b0-1d8d-4e01-b9f1-1a285dc99b74","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":2,"cache_configuration":null}'
+      string: '{"detail":"Structured generation failed, could not generate response
+        matching the schema."}'
     headers:
       content-length:
-      - '397'
+      - '91'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 10:46:24 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 400
+      message: Bad Request
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/46
-  response:
-    body:
-      string: '{"id":46,"path":"test/sdk/test_update_function","description":"Test
-        function","input_schema":null,"dataset_uuid":"a12f84b0-1d8d-4e01-b9f1-1a285dc99b74","out_schema":null,"instructions":"Do
-        something else","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":2,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
-    headers:
-      content-length:
-      - '380'
-      content-type:
-      - application/json
-      date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
-      server:
-      - uvicorn
-    status:
-      code: 200
-      message: OK
-- request:
-    body: ''
-    headers:
-      accept:
-      - '*/*'
-      accept-encoding:
-      - gzip, deflate
-      connection:
-      - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_update_function
+    uri: http://localhost:8000/v1/functions/64
   response:
     body:
-      string: '{"detail":"Function and associated generations deleted successfully"}'
+      string: ''
     headers:
-      content-length:
-      - '69'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:23:54 GMT
+      - Thu, 02 May 2024 10:46:45 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 204
+      message: No Content
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,83 @@
 interactions:
 - request:
-    body: '{"name": "test_create_index"}'
+    body: '{"name": "test_index_document"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '29'
+      - '31'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":250,"name":"test_create_index","files":[],"created_at":"2024-04-11T16:25:34.062134Z"}'
+      string: '{"id":28,"name":"test_index_document","files":[],"created_at":"2024-05-02T10:54:43.552742Z"}'
     headers:
       content-length:
+      - '92'
+      content-type:
+      - application/json
+      date:
+      - Thu, 02 May 2024 10:54:43 GMT
+      server:
+      - uvicorn
+    status:
+      code: 200
+      message: OK
+- request:
+    body: '{"id": null, "uuid": null, "key": null, "content": "Hello", "metadata":
+      {"source": "test"}}'
+    headers:
+      accept:
+      - '*/*'
+      connection:
+      - keep-alive
+      content-length:
       - '91'
       content-type:
       - application/json
+    method: POST
+    uri: http://localhost:8000/v1/indexes/28/index
+  response:
+    body:
+      string: '{"id":12,"uuid":"a36fd9f3-051f-4bb0-b2bb-d85ed56f44a3","key":"a36fd9f3-051f-4bb0-b2bb-d85ed56f44a3"}'
+    headers:
+      content-length:
+      - '100'
+      content-type:
+      - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 10:54:43 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/250
+    uri: http://localhost:8000/v1/indexes/28
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 10:54:43 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,118 +1,78 @@
 interactions:
 - request:
-    body: '{"name": "test_delete_index"}'
+    body: '{"name": "test_get_by_id"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '29'
+      - '26'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":251,"name":"test_delete_index","files":[],"created_at":"2024-04-11T16:25:34.116650Z"}'
+      string: '{"id":4,"name":"test_get_by_id","files":[],"created_at":"2024-05-02T09:18:07.341181Z"}'
     headers:
       content-length:
-      - '91'
+      - '86'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 09:18:07 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: DELETE
-    uri: http://localhost:8000/v1/indexes/251
+    method: GET
+    uri: http://localhost:8000/v1/indexes/4
   response:
     body:
-      string: 'true'
+      string: '{"id":4,"name":"test_get_by_id","files":[],"created_at":"2024-05-02T09:18:07.341181Z"}'
     headers:
       content-length:
-      - '4'
+      - '86'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 09:18:07 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
-      connection:
-      - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/v1/indexes/251
-  response:
-    body:
-      string: '{"detail":"Index not found"}'
-    headers:
-      content-length:
-      - '28'
-      content-type:
-      - application/json
-      date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
-      server:
-      - uvicorn
-    status:
-      code: 404
-      message: Not Found
-- request:
-    body: ''
-    headers:
-      accept:
-      - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/251
+    uri: http://localhost:8000/v1/indexes/4
   response:
     body:
-      string: '{"detail":"Index not found"}'
+      string: 'true'
     headers:
       content-length:
-      - '28'
+      - '4'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 09:18:07 GMT
       server:
       - uvicorn
     status:
-      code: 404
-      message: Not Found
+      code: 200
+      message: OK
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,90 +1,79 @@
 interactions:
 - request:
-    body: '{"name": "test_get_by_id"}'
+    body: '{"name": "test_get_by_name"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '26'
+      - '28'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":252,"name":"test_get_by_id","files":[],"created_at":"2024-04-11T16:25:34.175974Z"}'
+      string: '{"id":25,"name":"test_get_by_name","files":[],"created_at":"2024-05-02T10:54:43.459696Z"}'
     headers:
       content-length:
-      - '88'
+      - '89'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 10:54:43 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/v1/indexes/252
+    uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":252,"name":"test_get_by_id","files":[],"created_at":"2024-04-11T16:25:34.175974Z"}'
+      string: '[{"id":25,"org_id":1,"org_name":null,"name":"test_get_by_name","created_by":"Mattias
+        Lundell","created_at":"2024-05-02T10:54:43.459696Z","updated_at":"2024-05-02T10:54:43.459696Z","count":0}]'
     headers:
       content-length:
-      - '88'
+      - '191'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 10:54:43 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/252
+    uri: http://localhost:8000/v1/indexes/25
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 10:54:43 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 interactions:
 - request:
-    body: '{"name": "test_get_by_name"}'
+    body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
+    method: GET
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_delete_function
+  response:
+    body:
+      string: '{"detail":"Function not found"}'
+    headers:
       content-length:
-      - '28'
+      - '31'
+      content-type:
+      - application/json
+      date:
+      - Thu, 02 May 2024 10:52:28 GMT
+      server:
+      - uvicorn
+    status:
+      code: 404
+      message: Not Found
+- request:
+    body: '{"id": null, "path": "test/sdk/test_delete_function", "description": "Test
+      function", "input_schema": null, "out_schema": null, "instructions": "Do something",
+      "model": null, "index_ids": [], "use_semantic_search": null, "few_shot": null,
+      "few_shot_count": null, "cache_configuration": null}'
+    headers:
+      accept:
+      - '*/*'
+      connection:
+      - keep-alive
+      content-length:
+      - '291'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/v1/indexes
+    uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":253,"name":"test_get_by_name","files":[],"created_at":"2024-04-11T16:25:34.227196Z"}'
+      string: '{"id":70,"path":"test/sdk/test_delete_function","description":"Test
+        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"a40bf43d-a236-4b34-9095-9a4e73330f65","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '90'
+      - '392'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/v1/indexes
+    method: DELETE
+    uri: http://localhost:8000/v1/functions/70
   response:
     body:
-      string: '[{"id":253,"org_id":1,"org_name":null,"name":"test_get_by_name","created_by":"Mattias
-        Lundell","created_at":"2024-04-11T16:25:34.227196Z","updated_at":"2024-04-11T16:25:34.227196Z","count":0}]'
+      string: ''
     headers:
-      content-length:
-      - '192'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 204
+      message: No Content
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: DELETE
-    uri: http://localhost:8000/v1/indexes/253
+    method: GET
+    uri: http://localhost:8000/v1/functions/70
   response:
     body:
-      string: 'true'
+      string: '{"detail":"Function not found"}'
     headers:
       content-length:
-      - '4'
+      - '31'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 404
+      message: Not Found
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,79 @@
 interactions:
 - request:
-    body: '{"name": "test_index_document"}'
+    body: '{"uuid": "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133", "project": "project",
+      "name": "name", "input": "input", "start_time": "2021-01-01T00:00:00"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '31'
-      content-type:
-      - application/json
-      user-agent:
-      - python-httpx/0.27.0
+      - '141'
     method: POST
-    uri: http://localhost:8000/v1/indexes
+    uri: http://localhost:8000/v1/spans
   response:
     body:
-      string: '{"id":256,"name":"test_index_document","files":[],"created_at":"2024-04-11T16:25:34.330325Z"}'
+      string: '{"uuid":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133"}'
     headers:
       content-length:
-      - '93'
+      - '47'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 13:23:01 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"id": null, "uuid": null, "key": null, "content": "Hello", "metadata":
-      {"source": "test"}}'
+    body: '{"dimension": "dim", "value": 0.5, "comment": "comment"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '91'
+      - '56'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/v1/indexes/256/index
+    uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133/metrics
   response:
     body:
-      string: '{"id":85,"uuid":"5704e3d5-545b-468a-83af-0fd744b634e9","key":"5704e3d5-545b-468a-83af-0fd744b634e9"}'
+      string: '{"id":"0bf87615-d886-405b-a696-e10e9eacf787","span_id":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133","dimension":"dim","value":null,"comment":"comment","updated_at":null,"created_at":"2024-05-02T13:23:02.650064Z"}'
     headers:
       content-length:
-      - '100'
+      - '206'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 13:23:01 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/256
+    uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133
   response:
     body:
-      string: 'true'
+      string: ''
     headers:
-      content-length:
-      - '4'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 13:23:01 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 204
+      message: No Content
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,209 +1,181 @@
 interactions:
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
     uri: http://localhost:8000/v1/indexes
   response:
     body:
       string: '[]'
     headers:
       content-length:
       - '2'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 10:54:43 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"name": "test_list_indexes"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
       - '29'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":254,"name":"test_list_indexes","files":[],"created_at":"2024-04-11T16:25:34.267484Z"}'
+      string: '{"id":26,"name":"test_list_indexes","files":[],"created_at":"2024-05-02T10:54:43.494792Z"}'
     headers:
       content-length:
-      - '91'
+      - '90'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 10:54:43 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '[{"id":254,"org_id":1,"org_name":null,"name":"test_list_indexes","created_by":"Mattias
-        Lundell","created_at":"2024-04-11T16:25:34.267484Z","updated_at":"2024-04-11T16:25:34.267484Z","count":0}]'
+      string: '[{"id":26,"org_id":1,"org_name":null,"name":"test_list_indexes","created_by":"Mattias
+        Lundell","created_at":"2024-05-02T10:54:43.494792Z","updated_at":"2024-05-02T10:54:43.494792Z","count":0}]'
     headers:
       content-length:
-      - '193'
+      - '192'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 10:54:43 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"name": "test_list_indexes_2"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
       - '31'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":255,"name":"test_list_indexes_2","files":[],"created_at":"2024-04-11T16:25:34.286601Z"}'
+      string: '{"id":27,"name":"test_list_indexes_2","files":[],"created_at":"2024-05-02T10:54:43.512887Z"}'
     headers:
       content-length:
-      - '93'
+      - '92'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 10:54:43 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '[{"id":254,"org_id":1,"org_name":null,"name":"test_list_indexes","created_by":"Mattias
-        Lundell","created_at":"2024-04-11T16:25:34.267484Z","updated_at":"2024-04-11T16:25:34.267484Z","count":0},{"id":255,"org_id":1,"org_name":null,"name":"test_list_indexes_2","created_by":"Mattias
-        Lundell","created_at":"2024-04-11T16:25:34.286601Z","updated_at":"2024-04-11T16:25:34.286601Z","count":0}]'
+      string: '[{"id":26,"org_id":1,"org_name":null,"name":"test_list_indexes","created_by":"Mattias
+        Lundell","created_at":"2024-05-02T10:54:43.494792Z","updated_at":"2024-05-02T10:54:43.494792Z","count":0},{"id":27,"org_id":1,"org_name":null,"name":"test_list_indexes_2","created_by":"Mattias
+        Lundell","created_at":"2024-05-02T10:54:43.512887Z","updated_at":"2024-05-02T10:54:43.512887Z","count":0}]'
     headers:
       content-length:
-      - '387'
+      - '385'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 10:54:43 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/255
+    uri: http://localhost:8000/v1/indexes/27
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 10:54:43 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/254
+    uri: http://localhost:8000/v1/indexes/26
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 10:54:43 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,127 +1,80 @@
 interactions:
 - request:
-    body: '{"name": "test_retrieve_document"}'
-    headers:
-      accept:
-      - '*/*'
-      accept-encoding:
-      - gzip, deflate
-      connection:
-      - keep-alive
-      content-length:
-      - '34'
-      content-type:
-      - application/json
-      user-agent:
-      - python-httpx/0.27.0
-    method: POST
-    uri: http://localhost:8000/v1/indexes
-  response:
-    body:
-      string: '{"id":257,"name":"test_retrieve_document","files":[],"created_at":"2024-04-11T16:25:34.538913Z"}'
-    headers:
-      content-length:
-      - '96'
-      content-type:
-      - application/json
-      date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
-      server:
-      - uvicorn
-    status:
-      code: 200
-      message: OK
-- request:
-    body: '{"id": null, "uuid": null, "key": null, "content": "Hello", "metadata":
-      {"source": "test"}}'
+    body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      content-length:
-      - '91'
-      content-type:
-      - application/json
-      user-agent:
-      - python-httpx/0.27.0
-    method: POST
-    uri: http://localhost:8000/v1/indexes/257/index
+    method: GET
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_create_function_async
   response:
     body:
-      string: '{"id":86,"uuid":"8320bd18-12da-4104-8f09-cfdb4b10e8e3","key":"8320bd18-12da-4104-8f09-cfdb4b10e8e3"}'
+      string: '{"detail":"Function not found"}'
     headers:
       content-length:
-      - '100'
+      - '31'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 404
+      message: Not Found
 - request:
-    body: '{"q": "Hello", "k": 1, "filters": null}'
+    body: '{"id": null, "path": "test/sdk/test_create_function_async", "description":
+      "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
+      something", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
+      null, "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '39'
+      - '297'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/v1/indexes/257/query
+    uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '[{"uuid":"060d77ca-09e7-4436-96cb-29ab17a8b160","content":"Hello","metadata":{"source":"test"},"document_id":null,"score":29.458036422729492,"source_uuids":["060d77ca-09e7-4436-96cb-29ab17a8b160"]}]'
+      string: '{"id":65,"path":"test/sdk/test_create_function_async","description":"Test
+        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"b10c086d-6e04-4517-b577-8387939018d8","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '198'
+      - '398'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/257
+    uri: http://localhost:8000/v1/functions/65
   response:
     body:
-      string: 'true'
+      string: ''
     headers:
-      content-length:
-      - '4'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 204
+      message: No Content
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,128 +1,111 @@
 interactions:
 - request:
-    body: '{"name": "test_retrieve_filters"}'
+    body: '{"name": "test_retrieve_document"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '33'
+      - '34'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":258,"name":"test_retrieve_filters","files":[],"created_at":"2024-04-11T16:25:35.076324Z"}'
+      string: '{"id":29,"name":"test_retrieve_document","files":[],"created_at":"2024-05-02T10:54:43.991266Z"}'
     headers:
       content-length:
       - '95'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 10:54:43 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"id": null, "uuid": null, "key": null, "content": "Bonjour", "metadata":
+    body: '{"id": null, "uuid": null, "key": null, "content": "Hello", "metadata":
       {"source": "test"}}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '93'
+      - '91'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/v1/indexes/258/index
+    uri: http://localhost:8000/v1/indexes/29/index
   response:
     body:
-      string: '{"id":87,"uuid":"76d4c277-5262-4a26-9a5a-89948aa0e9fd","key":"76d4c277-5262-4a26-9a5a-89948aa0e9fd"}'
+      string: '{"id":13,"uuid":"ae40747e-b6a3-4649-ab53-d59cf77b3828","key":"ae40747e-b6a3-4649-ab53-d59cf77b3828"}'
     headers:
       content-length:
       - '100'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:33 GMT
+      - Thu, 02 May 2024 10:54:43 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"q": "test", "k": 1, "filters": [{"key": "source", "operation": "=", "value":
-      "test"}]}'
+    body: '{"q": "Hello", "k": 1, "filters": null}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '88'
+      - '39'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/v1/indexes/258/query
+    uri: http://localhost:8000/v1/indexes/29/query
   response:
     body:
-      string: '[{"uuid":"b72145ad-99e9-4a56-b410-f6d54c9979f5","content":"Bonjour","metadata":{"source":"test"},"document_id":null,"score":4.736573219299316,"source_uuids":["b72145ad-99e9-4a56-b410-f6d54c9979f5"]}]'
+      string: '[{"uuid":"fc3499e7-a601-4256-9a84-ecf7b8cc7458","content":"Hello","metadata":{"source":"test"},"document_id":null,"score":29.458036422729492,"source_uuids":["fc3499e7-a601-4256-9a84-ecf7b8cc7458"]}]'
     headers:
       content-length:
-      - '199'
+      - '198'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:35 GMT
+      - Thu, 02 May 2024 10:54:43 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/258
+    uri: http://localhost:8000/v1/indexes/29
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:25:35 GMT
+      - Thu, 02 May 2024 10:54:43 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,179 +1,155 @@
 interactions:
 - request:
-    body: '{"uuid": "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112", "project": "project",
+    body: '{"uuid": "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b", "project": "project",
       "name": "name", "input": "input", "start_time": "2021-01-01T00:00:00"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
       - '141'
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/v1/spans
   response:
     body:
-      string: '{"uuid":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112"}'
+      string: '{"uuid":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b"}'
     headers:
       content-length:
       - '47'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:06 GMT
+      - Thu, 02 May 2024 10:52:26 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"uuid": "cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12", "project": "project",
+    body: '{"uuid": "cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c3c4c3c", "project": "project",
       "name": "name", "input": "input", "start_time": "2021-01-01T00:00:00", "parent_uuid":
-      "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112"}'
+      "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
       - '196'
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/v1/spans
   response:
     body:
-      string: '{"uuid":"cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12"}'
+      string: '{"uuid":"cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c3c4c3c"}'
     headers:
       content-length:
       - '47'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:06 GMT
+      - Thu, 02 May 2024 10:52:26 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"uuid": "cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12", "output": "output", "end_time":
+    body: '{"uuid": "cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c3c4c3c", "output": "output", "end_time":
       "2021-12-01T00:00:00"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
       - '103'
-      user-agent:
-      - python-httpx/0.27.0
     method: PUT
-    uri: http://localhost:8000/v1/spans/cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12
+    uri: http://localhost:8000/v1/spans/cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c3c4c3c
   response:
     body:
-      string: '{"uuid":"cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12"}'
+      string: '{"uuid":"cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c3c4c3c"}'
     headers:
       content-length:
       - '47'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:06 GMT
+      - Thu, 02 May 2024 10:52:26 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"uuid": "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112", "output": "output", "end_time":
+    body: '{"uuid": "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b", "output": "output", "end_time":
       "2022-01-01T00:00:00"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
       - '103'
-      user-agent:
-      - python-httpx/0.27.0
     method: PUT
-    uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112
+    uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b
   response:
     body:
-      string: '{"uuid":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112"}'
+      string: '{"uuid":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b"}'
     headers:
       content-length:
       - '47'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:06 GMT
+      - Thu, 02 May 2024 10:52:26 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/v1/spans/cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12
+    uri: http://localhost:8000/v1/spans/cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c3c4c3c
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:06 GMT
+      - Thu, 02 May 2024 10:52:26 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112
+    uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:06 GMT
+      - Thu, 02 May 2024 10:52:26 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_spans/test_save_feedback.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,91 +1,111 @@
 interactions:
 - request:
-    body: '{"uuid": "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133", "project": "project",
-      "name": "name", "input": "input", "start_time": "2021-01-01T00:00:00"}'
+    body: '{"name": "test_retrieve_document"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '141'
-      user-agent:
-      - python-httpx/0.27.0
+      - '34'
+      content-type:
+      - application/json
     method: POST
-    uri: http://localhost:8000/v1/spans
+    uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"uuid":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133"}'
+      string: '{"id":9,"name":"test_retrieve_document","files":[],"created_at":"2024-05-02T09:18:07.817552Z"}'
     headers:
       content-length:
-      - '47'
+      - '94'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:06 GMT
+      - Thu, 02 May 2024 09:18:07 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"dimension": "dim", "score": 0.5, "comment": "comment"}'
+    body: '{"id": null, "uuid": null, "key": null, "content": "Hello", "metadata":
+      {"source": "test"}}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '56'
+      - '91'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133/feedbacks
+    uri: http://localhost:8000/v1/indexes/9/index
   response:
     body:
-      string: '{"id":"7e8b094c-9b6c-4c43-a3c8-dfc162531da4","span_id":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133","dimension":"dim","score":0.5,"comment":"comment","updated_at":null,"created_at":"2024-04-11T16:26:07.306703Z"}'
+      string: '{"id":7,"uuid":"4c7e92b0-950a-402e-8152-959b4b8bae86","key":"4c7e92b0-950a-402e-8152-959b4b8bae86"}'
     headers:
       content-length:
-      - '205'
+      - '99'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:06 GMT
+      - Thu, 02 May 2024 09:18:07 GMT
+      server:
+      - uvicorn
+    status:
+      code: 200
+      message: OK
+- request:
+    body: '{"q": "Hello", "k": 1, "filters": null}'
+    headers:
+      accept:
+      - '*/*'
+      connection:
+      - keep-alive
+      content-length:
+      - '39'
+      content-type:
+      - application/json
+    method: POST
+    uri: http://localhost:8000/v1/indexes/9/query
+  response:
+    body:
+      string: '[{"uuid":"b6542583-f101-4af0-bde6-5a6f9cb54793","content":"Hello","metadata":{"source":"test"},"document_id":null,"score":29.458036422729492,"source_uuids":["b6542583-f101-4af0-bde6-5a6f9cb54793"]}]'
+    headers:
+      content-length:
+      - '198'
+      content-type:
+      - application/json
+      date:
+      - Thu, 02 May 2024 09:18:07 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133
+    uri: http://localhost:8000/v1/indexes/9
   response:
     body:
-      string: ''
+      string: 'true'
     headers:
+      content-length:
+      - '4'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:06 GMT
+      - Thu, 02 May 2024 09:18:08 GMT
       server:
       - uvicorn
     status:
-      code: 204
-      message: No Content
+      code: 200
+      message: OK
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,79 @@
 interactions:
 - request:
-    body: '{"uuid": "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133", "project": "project",
-      "name": "name", "input": "input", "start_time": "2021-01-01T00:00:00"}'
+    body: '{"name": "test_get_by_name"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '141'
-      user-agent:
-      - python-httpx/0.27.0
+      - '28'
+      content-type:
+      - application/json
     method: POST
-    uri: http://localhost:8000/v1/spans
+    uri: http://localhost:8000/v1/indexes
   response:
-    content: '{"uuid":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133"}'
+    body:
+      string: '{"id":5,"name":"test_get_by_name","files":[],"created_at":"2024-05-02T09:18:07.379419Z"}'
     headers:
       content-length:
-      - '47'
+      - '88'
       content-type:
       - application/json
       date:
-      - Tue, 30 Apr 2024 18:57:37 GMT
+      - Thu, 02 May 2024 09:18:07 GMT
       server:
       - uvicorn
-    http_version: HTTP/1.1
-    status_code: 200
+    status:
+      code: 200
+      message: OK
 - request:
-    body: '{"dimension": "dim", "score": 0.5, "comment": "comment"}'
+    body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      content-length:
-      - '56'
-      content-type:
-      - application/json
-      user-agent:
-      - python-httpx/0.27.0
-    method: POST
-    uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133/metrics
+    method: GET
+    uri: http://localhost:8000/v1/indexes
   response:
-    content: '{"id":"75f72199-87ed-4b71-9513-5ade7c94c40d","span_id":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133","dimension":"dim","score":0.5,"comment":"comment","updated_at":null,"created_at":"2024-04-30T18:57:38.088687Z"}'
+    body:
+      string: '[{"id":5,"org_id":1,"org_name":null,"name":"test_get_by_name","created_by":"Mattias
+        Lundell","created_at":"2024-05-02T09:18:07.379419Z","updated_at":"2024-05-02T09:18:07.379419Z","count":0}]'
     headers:
       content-length:
-      - '205'
+      - '190'
       content-type:
       - application/json
       date:
-      - Tue, 30 Apr 2024 18:57:37 GMT
+      - Thu, 02 May 2024 09:18:07 GMT
       server:
       - uvicorn
-    http_version: HTTP/1.1
-    status_code: 200
+    status:
+      code: 200
+      message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133
+    uri: http://localhost:8000/v1/indexes/5
   response:
-    content: ''
+    body:
+      string: 'true'
     headers:
+      content-length:
+      - '4'
       content-type:
       - application/json
       date:
-      - Tue, 30 Apr 2024 18:57:37 GMT
+      - Thu, 02 May 2024 09:18:07 GMT
       server:
       - uvicorn
-    http_version: HTTP/1.1
-    status_code: 204
+    status:
+      code: 200
+      message: OK
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,124 +1,105 @@
 interactions:
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_create_function
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get_by_path
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:06 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_create_function", "description": "Test
+    body: '{"id": null, "path": "test/sdk/test_get_by_path", "description": "Test
       function", "input_schema": null, "out_schema": null, "instructions": "Do something",
       "model": null, "index_ids": [], "use_semantic_search": null, "few_shot": null,
       "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '291'
+      - '287'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/api/v1/functions
+    uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":52,"path":"test/sdk/test_create_function","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"5c2ded91-dd84-4161-ae5d-269130628be4","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"id":67,"path":"test/sdk/test_get_by_path","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
+        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"4e22a996-0444-41b2-8921-3aaaf20f0af8","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '392'
+      - '388'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:06 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/52
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get_by_path
   response:
     body:
-      string: '{"id":52,"path":"test/sdk/test_create_function","description":"Test
-        function","input_schema":null,"dataset_uuid":"5c2ded91-dd84-4161-ae5d-269130628be4","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '{"id":67,"path":"test/sdk/test_get_by_path","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
+        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"4e22a996-0444-41b2-8921-3aaaf20f0af8","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '375'
+      - '466'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:06 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_create_function
+    uri: http://localhost:8000/v1/functions/67
   response:
     body:
-      string: '{"detail":"Function and associated generations deleted successfully"}'
+      string: ''
     headers:
-      content-length:
-      - '69'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:06 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 204
+      message: No Content
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,193 +1,105 @@
 interactions:
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_create_function_with_cache
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get_by_id
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:17 GMT
+      - Thu, 02 May 2024 09:22:31 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_create_function_with_cache", "description":
-      "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
-      something", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
-      null, "few_shot_count": null, "cache_configuration": {"exact_match_cache_ttl":
-      10, "semantic_cache_threshold": null, "semantic_cache_ttl": null}}'
+    body: '{"id": null, "path": "test/sdk/test_get_by_id", "description": "Test function",
+      "input_schema": null, "out_schema": null, "instructions": "Do something", "model":
+      null, "index_ids": [], "use_semantic_search": null, "few_shot": null, "few_shot_count":
+      null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '389'
+      - '285'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/api/v1/functions
+    uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":60,"path":"test/sdk/test_create_function_with_cache","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"0492231a-3b8d-4fab-ad8e-19f8be5d8597","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"id":57,"path":"test/sdk/test_get_by_id","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
+        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"7ce0a1d8-d7bb-4323-8703-95974c257844","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '403'
-      content-type:
-      - application/json
-      date:
-      - Thu, 11 Apr 2024 16:26:17 GMT
-      server:
-      - uvicorn
-    status:
-      code: 200
-      message: OK
-- request:
-    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
-    headers:
-      accept:
-      - '*/*'
-      accept-encoding:
-      - gzip, deflate
-      connection:
-      - keep-alive
-      content-length:
-      - '78'
-      content-type:
-      - application/json
-      user-agent:
-      - python-httpx/0.27.0
-    method: POST
-    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache
-  response:
-    body:
-      string: '{"span_id":"621f54fb-902c-4898-9cf2-c421b5129e26","message":"Hello!
-        How can I assist you today? If you have any questions or need information
-        on a particular topic, feel free to ask.","json_payload":null,"error":null,"context":null,"cached":false}'
-    headers:
-      content-length:
-      - '247'
-      content-type:
-      - application/json
-      date:
-      - Thu, 11 Apr 2024 16:26:17 GMT
-      server:
-      - uvicorn
-    status:
-      code: 200
-      message: OK
-- request:
-    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
-    headers:
-      accept:
-      - '*/*'
-      accept-encoding:
-      - gzip, deflate
-      connection:
-      - keep-alive
-      content-length:
-      - '78'
-      content-type:
-      - application/json
-      user-agent:
-      - python-httpx/0.27.0
-    method: POST
-    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache
-  response:
-    body:
-      string: '{"span_id":"b6d774b9-7cc6-4a01-8dd2-846d1fdd331a","message":"Hello!
-        How can I assist you today? If you have any questions or need information
-        on a particular topic, feel free to ask.","json_payload":null,"error":null,"context":null,"cached":true}'
-    headers:
-      content-length:
-      - '246'
+      - '386'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:21 GMT
+      - Thu, 02 May 2024 09:22:31 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/60
+    uri: http://localhost:8000/v1/functions/57
   response:
     body:
-      string: '{"id":60,"path":"test/sdk/test_create_function_with_cache","description":"Test
-        function","input_schema":null,"dataset_uuid":"0492231a-3b8d-4fab-ad8e-19f8be5d8597","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '{"id":57,"path":"test/sdk/test_get_by_id","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
+        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"7ce0a1d8-d7bb-4323-8703-95974c257844","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '386'
+      - '464'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:21 GMT
+      - Thu, 02 May 2024 09:22:31 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_create_function_with_cache
+    uri: http://localhost:8000/v1/functions/57
   response:
     body:
-      string: '{"detail":"Function and associated generations deleted successfully"}'
+      string: ''
     headers:
-      content-length:
-      - '69'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:21 GMT
+      - Thu, 02 May 2024 09:22:31 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 204
+      message: No Content
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,152 +1,109 @@
 interactions:
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_id
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_async_chat
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:07 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_delete_function_by_id", "description":
-      "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
-      something", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
+    body: '{"id": null, "path": "test/sdk/test_async_chat", "description": "Translate
+      to French", "input_schema": null, "out_schema": null, "instructions": "Translate
+      to French", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
       null, "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '297'
+      - '299'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/api/v1/functions
+    uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":56,"path":"test/sdk/test_delete_function_by_id","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"87e5ce5e-db28-4dc0-b860-045fd6ce9e7e","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"id":71,"path":"test/sdk/test_async_chat","description":"Translate
+        to French","input_schema":null,"out_schema":null,"instructions":"Translate
+        to French","few_shot":false,"few_shot_count":2,"dataset_uuid":"05a07dc3-f0a2-4a31-8283-b85ad16b8653","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '398'
+      - '400'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:07 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: ''
+    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/56
-  response:
-    body:
-      string: '{"id":56,"path":"test/sdk/test_delete_function_by_id","description":"Test
-        function","input_schema":null,"dataset_uuid":"87e5ce5e-db28-4dc0-b860-045fd6ce9e7e","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
-    headers:
       content-length:
-      - '381'
+      - '78'
       content-type:
       - application/json
-      date:
-      - Thu, 11 Apr 2024 16:26:07 GMT
-      server:
-      - uvicorn
-    status:
-      code: 200
-      message: OK
-- request:
-    body: ''
-    headers:
-      accept:
-      - '*/*'
-      accept-encoding:
-      - gzip, deflate
-      connection:
-      - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: DELETE
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_id
+    method: POST
+    uri: http://localhost:8000/v1/chat/test/sdk/test_async_chat
   response:
     body:
-      string: '{"detail":"Function and associated generations deleted successfully"}'
+      string: '{"span_id":"7099623e-78b8-450d-887c-2028f018caed","message":"Bonjour","json_payload":null,"error":null,"context":null,"cached":false}'
     headers:
       content-length:
-      - '69'
+      - '133'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:07 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/56
+    method: DELETE
+    uri: http://localhost:8000/v1/functions/71
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: ''
     headers:
-      content-length:
-      - '31'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:07 GMT
+      - Thu, 02 May 2024 10:52:29 GMT
       server:
       - uvicorn
     status:
-      code: 404
-      message: Not Found
+      code: 204
+      message: No Content
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,122 +1,113 @@
 interactions:
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_path
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_update_function
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:07 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_delete_function_by_path", "description":
-      "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
-      something", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
-      null, "few_shot_count": null, "cache_configuration": null}'
+    body: '{"id": null, "path": "test/sdk/test_update_function", "description": "Test
+      function", "input_schema": null, "out_schema": null, "instructions": "Do something",
+      "model": null, "index_ids": [], "use_semantic_search": null, "few_shot": null,
+      "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '299'
+      - '291'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/api/v1/functions
+    uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":57,"path":"test/sdk/test_delete_function_by_path","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"3b2d8017-5f8a-40ec-8077-ce3ce9fcc3a7","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"id":69,"path":"test/sdk/test_update_function","description":"Test
+        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"dd72b71a-ca0d-45bc-bf60-29651f5fffcf","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '400'
+      - '392'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:07 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: ''
+    body: '{"id": 69, "path": "test/sdk/test_update_function", "description": "Test
+      function", "input_schema": null, "out_schema": null, "instructions": "Do something
+      else", "model": "azure/gpt4-eu", "index_ids": [], "use_semantic_search": false,
+      "few_shot": false, "few_shot_count": 2, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: DELETE
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_path
+      content-length:
+      - '304'
+      content-type:
+      - application/json
+    method: PATCH
+    uri: http://localhost:8000/v1/functions/69
   response:
     body:
-      string: '{"detail":"Function and associated generations deleted successfully"}'
+      string: '{"id":69,"path":"test/sdk/test_update_function","description":"Test
+        function","input_schema":null,"out_schema":null,"instructions":"Do something
+        else","few_shot":false,"few_shot_count":2,"dataset_uuid":"dd72b71a-ca0d-45bc-bf60-29651f5fffcf","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":2,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '69'
+      - '475'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:07 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_path
+    method: DELETE
+    uri: http://localhost:8000/v1/functions/69
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: ''
     headers:
-      content-length:
-      - '31'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:07 GMT
+      - Thu, 02 May 2024 10:52:28 GMT
       server:
       - uvicorn
     status:
-      code: 404
-      message: Not Found
+      code: 204
+      message: No Content
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_get.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,180 +1,155 @@
 interactions:
 - request:
-    body: ''
+    body: '{"uuid": "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112", "project": "project",
+      "name": "name", "input": "input", "start_time": "2021-01-01T00:00:00"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_get
+      content-length:
+      - '141'
+    method: POST
+    uri: http://localhost:8000/v1/spans
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"uuid":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112"}'
     headers:
       content-length:
-      - '31'
+      - '47'
       content-type:
       - application/json
       date:
-      - Mon, 08 Apr 2024 13:45:34 GMT
+      - Thu, 02 May 2024 10:52:26 GMT
       server:
       - uvicorn
     status:
-      code: 404
-      message: Not Found
+      code: 200
+      message: OK
 - request:
-    body: '{"id": null, "path": "test/sdk/test_get", "description": "Test function",
-      "input_schema": null, "out_schema": null, "instructions": "Do something", "model":
-      null, "index_ids": null, "use_semantic_search": null, "few_shot": null, "few_shot_count":
-      null, "cache_configuration": null}'
+    body: '{"uuid": "cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12", "project": "project",
+      "name": "name", "input": "input", "start_time": "2021-01-01T00:00:00", "parent_uuid":
+      "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '281'
-      content-type:
-      - application/json
-      user-agent:
-      - python-httpx/0.27.0
+      - '196'
     method: POST
-    uri: http://localhost:8000/api/v1/functions
+    uri: http://localhost:8000/v1/spans
   response:
     body:
-      string: '{"id":123}'
+      string: '{"uuid":"cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12"}'
     headers:
       content-length:
-      - '10'
+      - '47'
       content-type:
       - application/json
       date:
-      - Mon, 08 Apr 2024 13:45:34 GMT
+      - Thu, 02 May 2024 10:52:26 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: ''
+    body: '{"uuid": "cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12", "output": "output", "end_time":
+      "2021-12-01T00:00:00"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/123
+      content-length:
+      - '103'
+    method: PUT
+    uri: http://localhost:8000/v1/spans/cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12
   response:
     body:
-      string: '{"id":123,"path":"test/sdk/test_get","description":"Test function","input_schema":null,"dataset_uuid":"b6188ef1-3393-4ca6-8f86-e2433422dab8","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '{"uuid":"cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12"}'
     headers:
       content-length:
-      - '364'
+      - '47'
       content-type:
       - application/json
       date:
-      - Mon, 08 Apr 2024 13:45:34 GMT
+      - Thu, 02 May 2024 10:52:26 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: ''
+    body: '{"uuid": "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112", "output": "output", "end_time":
+      "2022-01-01T00:00:00"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_get
+      content-length:
+      - '103'
+    method: PUT
+    uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112
   response:
     body:
-      string: '{"id":123,"path":"test/sdk/test_get","description":"Test function","input_schema":null,"dataset_uuid":"b6188ef1-3393-4ca6-8f86-e2433422dab8","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '{"uuid":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112"}'
     headers:
       content-length:
-      - '364'
+      - '47'
       content-type:
       - application/json
       date:
-      - Mon, 08 Apr 2024 13:45:34 GMT
+      - Thu, 02 May 2024 10:52:26 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/123
+    method: DELETE
+    uri: http://localhost:8000/v1/spans/cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12
   response:
     body:
-      string: '{"id":123,"path":"test/sdk/test_get","description":"Test function","input_schema":null,"dataset_uuid":"b6188ef1-3393-4ca6-8f86-e2433422dab8","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: ''
     headers:
-      content-length:
-      - '364'
       content-type:
       - application/json
       date:
-      - Mon, 08 Apr 2024 13:45:34 GMT
+      - Thu, 02 May 2024 10:52:26 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 204
+      message: No Content
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_get
+    uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112
   response:
     body:
-      string: '{"detail":"Function and associated generations deleted successfully"}'
+      string: ''
     headers:
-      content-length:
-      - '69'
       content-type:
       - application/json
       date:
-      - Mon, 08 Apr 2024 13:45:34 GMT
+      - Thu, 02 May 2024 10:52:26 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 204
+      message: No Content
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,152 +1,118 @@
 interactions:
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_get_by_id
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_failed_structured_generation
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:06 GMT
+      - Thu, 02 May 2024 09:17:50 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_get_by_id", "description": "Test function",
-      "input_schema": null, "out_schema": null, "instructions": "Do something", "model":
-      null, "index_ids": [], "use_semantic_search": null, "few_shot": null, "few_shot_count":
-      null, "cache_configuration": null}'
+    body: '{"id": null, "path": "test/sdk/test_failed_structured_generation", "description":
+      "test structured generation exception", "input_schema": null, "out_schema":
+      {"type": "object", "properties": {"universityName": {"type": "string"}, "location":
+      {"type": "string"}, "departments": {"type": "array", "items": {"type": "object",
+      "properties": {"departmentName": {"type": "string"}, "head": {"type": "string"},
+      "courses": {"type": "array", "items": {"type": "object", "properties": {"courseId":
+      {"type": "string"}, "courseName": {"type": "string"}, "credits": {"type": "integer",
+      "minimum": 1, "maximum": 10}}, "required": ["courseId", "courseName", "credits"]}}},
+      "required": ["departmentName", "head", "courses"]}}}, "required": ["universityName",
+      "location", "departments"]}, "instructions": "You translate the incoming text
+      to french", "model": "mistral/mistral-tiny-eu", "index_ids": [], "use_semantic_search":
+      null, "few_shot": null, "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '285'
+      - '985'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/api/v1/functions
+    uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":53,"path":"test/sdk/test_get_by_id","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
-        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"d6742964-f102-4c1d-8b64-070d80089353","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"id":30,"path":"test/sdk/test_failed_structured_generation","description":"test
+        structured generation exception","input_schema":null,"out_schema":null,"instructions":"You
+        translate the incoming text to french","few_shot":false,"few_shot_count":2,"dataset_uuid":"b6e23402-8fcf-49d0-9a30-3ada2f0b5742","use_semantic_search":false,"model":"mistral/mistral-tiny-eu","language_model_id":4,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '386'
+      - '467'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:06 GMT
+      - Thu, 02 May 2024 09:17:50 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: ''
+    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/53
-  response:
-    body:
-      string: '{"id":53,"path":"test/sdk/test_get_by_id","description":"Test function","input_schema":null,"dataset_uuid":"d6742964-f102-4c1d-8b64-070d80089353","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
-    headers:
       content-length:
-      - '369'
+      - '78'
       content-type:
       - application/json
-      date:
-      - Thu, 11 Apr 2024 16:26:06 GMT
-      server:
-      - uvicorn
-    status:
-      code: 200
-      message: OK
-- request:
-    body: ''
-    headers:
-      accept:
-      - '*/*'
-      accept-encoding:
-      - gzip, deflate
-      connection:
-      - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/53
+    method: POST
+    uri: http://localhost:8000/v1/chat/test/sdk/test_failed_structured_generation
   response:
     body:
-      string: '{"id":53,"path":"test/sdk/test_get_by_id","description":"Test function","input_schema":null,"dataset_uuid":"d6742964-f102-4c1d-8b64-070d80089353","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '{"detail":"Structured generation failed, could not generate response
+        matching the schema."}'
     headers:
       content-length:
-      - '369'
+      - '91'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:06 GMT
+      - Thu, 02 May 2024 09:17:50 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 400
+      message: Bad Request
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_get_by_id
+    uri: http://localhost:8000/v1/functions/30
   response:
     body:
-      string: '{"detail":"Function and associated generations deleted successfully"}'
+      string: ''
     headers:
-      content-length:
-      - '69'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:06 GMT
+      - Thu, 02 May 2024 09:18:06 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 204
+      message: No Content
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,78 @@
 interactions:
 - request:
-    body: '{"name": "test_create_index"}'
+    body: '{"name": "test_get_by_id"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '29'
+      - '26'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":259,"name":"test_create_index","files":[],"created_at":"2024-04-11T16:26:34.227488Z"}'
+      string: '{"id":24,"name":"test_get_by_id","files":[],"created_at":"2024-05-02T10:54:43.425668Z"}'
     headers:
       content-length:
-      - '91'
+      - '87'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:33 GMT
+      - Thu, 02 May 2024 10:54:43 GMT
+      server:
+      - uvicorn
+    status:
+      code: 200
+      message: OK
+- request:
+    body: ''
+    headers:
+      accept:
+      - '*/*'
+      connection:
+      - keep-alive
+    method: GET
+    uri: http://localhost:8000/v1/indexes/24
+  response:
+    body:
+      string: '{"id":24,"name":"test_get_by_id","files":[],"created_at":"2024-05-02T10:54:43.425668Z"}'
+    headers:
+      content-length:
+      - '87'
+      content-type:
+      - application/json
+      date:
+      - Thu, 02 May 2024 10:54:43 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/259
+    uri: http://localhost:8000/v1/indexes/24
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:33 GMT
+      - Thu, 02 May 2024 10:54:43 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,90 +1,83 @@
 interactions:
 - request:
-    body: '{"name": "test_delete_index"}'
+    body: '{"name": "test_index_document"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '29'
+      - '31'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":260,"name":"test_delete_index","files":[],"created_at":"2024-04-11T16:26:34.258026Z"}'
+      string: '{"id":8,"name":"test_index_document","files":[],"created_at":"2024-05-02T09:18:07.509002Z"}'
     headers:
       content-length:
       - '91'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:34 GMT
+      - Thu, 02 May 2024 09:18:07 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: ''
+    body: '{"id": null, "uuid": null, "key": null, "content": "Hello", "metadata":
+      {"source": "test"}}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: DELETE
-    uri: http://localhost:8000/v1/indexes/260
+      content-length:
+      - '91'
+      content-type:
+      - application/json
+    method: POST
+    uri: http://localhost:8000/v1/indexes/8/index
   response:
     body:
-      string: 'true'
+      string: '{"id":6,"uuid":"5b1ffc8c-d713-48a4-a3a5-2d6cfe8fc571","key":"5b1ffc8c-d713-48a4-a3a5-2d6cfe8fc571"}'
     headers:
       content-length:
-      - '4'
+      - '99'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:34 GMT
+      - Thu, 02 May 2024 09:18:07 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/v1/indexes/260
+    method: DELETE
+    uri: http://localhost:8000/v1/indexes/8
   response:
     body:
-      string: '{"detail":"Index not found"}'
+      string: 'true'
     headers:
       content-length:
-      - '28'
+      - '4'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:34 GMT
+      - Thu, 02 May 2024 09:18:07 GMT
       server:
       - uvicorn
     status:
-      code: 404
-      message: Not Found
+      code: 200
+      message: OK
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,112 @@
 interactions:
 - request:
-    body: '{"name": "test_index_document"}'
+    body: '{"name": "test_retrieve_filters"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '31'
+      - '33'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":265,"name":"test_index_document","files":[],"created_at":"2024-04-11T16:26:34.415078Z"}'
+      string: '{"id":30,"name":"test_retrieve_filters","files":[],"created_at":"2024-05-02T10:54:44.462991Z"}'
     headers:
       content-length:
-      - '93'
+      - '94'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:34 GMT
+      - Thu, 02 May 2024 10:54:44 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"id": null, "uuid": null, "key": null, "content": "Hello", "metadata":
+    body: '{"id": null, "uuid": null, "key": null, "content": "Bonjour", "metadata":
       {"source": "test"}}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '91'
+      - '93'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/v1/indexes/265/index
+    uri: http://localhost:8000/v1/indexes/30/index
   response:
     body:
-      string: '{"id":88,"uuid":"3b6e706f-e531-4e30-a5bd-59d395e1f51b","key":"3b6e706f-e531-4e30-a5bd-59d395e1f51b"}'
+      string: '{"id":14,"uuid":"a8008a30-6a5e-4ab4-8ad0-eee61bc32eaa","key":"a8008a30-6a5e-4ab4-8ad0-eee61bc32eaa"}'
     headers:
       content-length:
       - '100'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:34 GMT
+      - Thu, 02 May 2024 10:54:44 GMT
+      server:
+      - uvicorn
+    status:
+      code: 200
+      message: OK
+- request:
+    body: '{"q": "test", "k": 1, "filters": [{"key": "source", "operation": "=", "value":
+      "test"}]}'
+    headers:
+      accept:
+      - '*/*'
+      connection:
+      - keep-alive
+      content-length:
+      - '88'
+      content-type:
+      - application/json
+    method: POST
+    uri: http://localhost:8000/v1/indexes/30/query
+  response:
+    body:
+      string: '[{"uuid":"366fdf32-fba0-453c-ae3e-e3b6ce29289d","content":"Bonjour","metadata":{"source":"test"},"document_id":null,"score":4.736573219299316,"source_uuids":["366fdf32-fba0-453c-ae3e-e3b6ce29289d"]}]'
+    headers:
+      content-length:
+      - '199'
+      content-type:
+      - application/json
+      date:
+      - Thu, 02 May 2024 10:54:44 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/265
+    uri: http://localhost:8000/v1/indexes/30
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:34 GMT
+      - Thu, 02 May 2024 10:54:44 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,209 +1,193 @@
 interactions:
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/v1/indexes
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_create_function_with_cache_async_flush
   response:
     body:
-      string: '[]'
+      string: '{"detail":"Function not found"}'
     headers:
       content-length:
-      - '2'
+      - '31'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:34 GMT
+      - Thu, 02 May 2024 10:52:32 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 404
+      message: Not Found
 - request:
-    body: '{"name": "test_list_indexes"}'
+    body: '{"id": null, "path": "test/sdk/test_create_function_with_cache_async_flush",
+      "description": "Test function", "input_schema": null, "out_schema": null, "instructions":
+      "Do something", "model": null, "index_ids": [], "use_semantic_search": null,
+      "few_shot": null, "few_shot_count": null, "cache_configuration": {"exact_match_cache_ttl":
+      10, "semantic_cache_threshold": null, "semantic_cache_ttl": null}}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '29'
+      - '401'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/v1/indexes
+    uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":263,"name":"test_list_indexes","files":[],"created_at":"2024-04-11T16:26:34.358515Z"}'
+      string: '{"id":74,"path":"test/sdk/test_create_function_with_cache_async_flush","description":"Test
+        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"f755d0c0-8430-4052-8072-00a160c38fa8","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '91'
+      - '415'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:34 GMT
+      - Thu, 02 May 2024 10:52:32 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: ''
+    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/v1/indexes
+      content-length:
+      - '78'
+      content-type:
+      - application/json
+    method: POST
+    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache_async_flush
   response:
     body:
-      string: '[{"id":263,"org_id":1,"org_name":null,"name":"test_list_indexes","created_by":"Mattias
-        Lundell","created_at":"2024-04-11T16:26:34.358515Z","updated_at":"2024-04-11T16:26:34.358515Z","count":0}]'
+      string: '{"span_id":"08b7c1c3-b5bb-4304-97b7-2722aef33a1b","message":"Hello!
+        How can I assist you today? If you have any questions or need information
+        on a particular topic, feel free to ask.","json_payload":null,"error":null,"context":null,"cached":false}'
     headers:
       content-length:
-      - '193'
+      - '247'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:34 GMT
+      - Thu, 02 May 2024 10:52:32 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"name": "test_list_indexes_2"}'
+    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '31'
+      - '78'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/v1/indexes
+    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache_async_flush
   response:
     body:
-      string: '{"id":264,"name":"test_list_indexes_2","files":[],"created_at":"2024-04-11T16:26:34.376310Z"}'
+      string: '{"span_id":"d95bbcac-602b-49af-aaef-47002e271e28","message":"Hello!
+        How can I assist you today? If you have any questions or need information
+        on a particular topic, feel free to ask.","json_payload":null,"error":null,"context":null,"cached":true}'
     headers:
       content-length:
-      - '93'
+      - '246'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:34 GMT
+      - Thu, 02 May 2024 10:52:34 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/v1/indexes
+    method: DELETE
+    uri: http://localhost:8000/v1/functions/74/cache
   response:
     body:
-      string: '[{"id":263,"org_id":1,"org_name":null,"name":"test_list_indexes","created_by":"Mattias
-        Lundell","created_at":"2024-04-11T16:26:34.358515Z","updated_at":"2024-04-11T16:26:34.358515Z","count":0},{"id":264,"org_id":1,"org_name":null,"name":"test_list_indexes_2","created_by":"Mattias
-        Lundell","created_at":"2024-04-11T16:26:34.376310Z","updated_at":"2024-04-11T16:26:34.376310Z","count":0}]'
+      string: ''
     headers:
-      content-length:
-      - '387'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:34 GMT
+      - Thu, 02 May 2024 10:52:34 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 204
+      message: No Content
 - request:
-    body: ''
+    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: DELETE
-    uri: http://localhost:8000/v1/indexes/264
+      content-length:
+      - '78'
+      content-type:
+      - application/json
+    method: POST
+    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache_async_flush
   response:
     body:
-      string: 'true'
+      string: '{"span_id":"0041a12d-1433-4d75-988d-03e346f715b4","message":"Hello!
+        How can I assist you today? If you have any questions or need information
+        on a specific topic, feel free to ask.","json_payload":null,"error":null,"context":null,"cached":false}'
     headers:
       content-length:
-      - '4'
+      - '245'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:34 GMT
+      - Thu, 02 May 2024 10:52:34 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/263
+    uri: http://localhost:8000/v1/functions/74
   response:
     body:
-      string: 'true'
+      string: ''
     headers:
-      content-length:
-      - '4'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:34 GMT
+      - Thu, 02 May 2024 10:52:36 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 204
+      message: No Content
 version: 1
```

### Comparing `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml` & `opperai-0.5.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,127 +1,112 @@
 interactions:
 - request:
-    body: '{"name": "test_retrieve_document"}'
+    body: '{"name": "test_retrieve_filters"}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '34'
+      - '33'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":266,"name":"test_retrieve_document","files":[],"created_at":"2024-04-11T16:26:34.595843Z"}'
+      string: '{"id":10,"name":"test_retrieve_filters","files":[],"created_at":"2024-05-02T09:18:08.481814Z"}'
     headers:
       content-length:
-      - '96'
+      - '94'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:34 GMT
+      - Thu, 02 May 2024 09:18:08 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"id": null, "uuid": null, "key": null, "content": "Hello", "metadata":
+    body: '{"id": null, "uuid": null, "key": null, "content": "Bonjour", "metadata":
       {"source": "test"}}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '91'
+      - '93'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/v1/indexes/266/index
+    uri: http://localhost:8000/v1/indexes/10/index
   response:
     body:
-      string: '{"id":89,"uuid":"152d502b-f3d3-4f12-9871-9469bbb319cd","key":"152d502b-f3d3-4f12-9871-9469bbb319cd"}'
+      string: '{"id":8,"uuid":"1ed107f4-29d9-40de-8b3a-550a61efe1d4","key":"1ed107f4-29d9-40de-8b3a-550a61efe1d4"}'
     headers:
       content-length:
-      - '100'
+      - '99'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:34 GMT
+      - Thu, 02 May 2024 09:18:08 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"q": "Hello", "k": 1, "filters": null}'
+    body: '{"q": "test", "k": 1, "filters": [{"key": "source", "operation": "=", "value":
+      "test"}]}'
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '39'
+      - '88'
       content-type:
       - application/json
-      user-agent:
-      - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/v1/indexes/266/query
+    uri: http://localhost:8000/v1/indexes/10/query
   response:
     body:
-      string: '[{"uuid":"0a6f9f4e-18be-4e84-8afd-77c4fbbe4279","content":"Hello","metadata":{"source":"test"},"document_id":null,"score":29.458036422729492,"source_uuids":["0a6f9f4e-18be-4e84-8afd-77c4fbbe4279"]}]'
+      string: '[{"uuid":"9c9adf6d-f446-4cb2-b701-602b211f9491","content":"Bonjour","metadata":{"source":"test"},"document_id":null,"score":4.736573219299316,"source_uuids":["9c9adf6d-f446-4cb2-b701-602b211f9491"]}]'
     headers:
       content-length:
-      - '198'
+      - '199'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:34 GMT
+      - Thu, 02 May 2024 09:18:08 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
-      accept-encoding:
-      - gzip, deflate
       connection:
       - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/266
+    uri: http://localhost:8000/v1/indexes/10
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 11 Apr 2024 16:26:34 GMT
+      - Thu, 02 May 2024 09:18:08 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.4.0/LICENSE` & `opperai-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opperai-0.4.0/README.md` & `opperai-0.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,24 @@
 
 ## Install
 
 ```bash
 pip install opperai
 ```
 
+## Configuration
+
+### Environment variable
+
+- `OPPER_API_KEY` environment variable is read by the SDK if no `api_key` is provided to the `Client` object. 
+- `OPPER_PROJECT` is attached to traces and can be used for filtering in the Opper UI.
+- `OPPER_DEFAULT_MODEL` will define the model used by functions created with the `fn` decorator
+
+When using the `fn` decorator the SDK client is automatically initialized with the `OPPER_API_KEY` environment variable.
+
 ## Using the `fn` decorator
 
 ```python
 from opperai import fn
 
 @fn()
 def translate(text: str, target_language: str) -> str:
@@ -110,15 +120,10 @@
 ## Retrieval
 
 ```python
 client.indexes.retrieve(index_id=42, "Who is the president of the USA?", 3)
 
 ```
 
-## Configuration
-
-### Environment variable
-
-The `OPPER_API_KEY` environment variable is read by the SDK if no `api_key` is provided to the `Client` object. 
-`OPPER_PROJECT` is attached to traces and can be used for filtering in the Opper UI.
+# Examples
 
-When using the `fn` decorator the SDK client is automatically initialized with the `OPPER_API_KEY` environment variable.
+See examples in our [documentation](https://docs.opper.ai)
```

### Comparing `opperai-0.4.0/pyproject.toml` & `opperai-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "opperai"
-version = "0.4.0"
+version = "0.5.0"
 description = "Opper Python client"
 authors = [
   {name = "Opper", email = "opper@opper.ai"},
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `opperai-0.4.0/PKG-INFO` & `opperai-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: opperai
-Version: 0.4.0
+Version: 0.5.0
 Summary: Opper Python client
 Project-URL: Homepage, https://opper.ai
 Project-URL: Documentation, https://docs.opper.ai
 Project-URL: Platform, https://platform.opper.ai
 Author-email: Opper <opper@opper.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -25,14 +25,24 @@
 
 ## Install
 
 ```bash
 pip install opperai
 ```
 
+## Configuration
+
+### Environment variable
+
+- `OPPER_API_KEY` environment variable is read by the SDK if no `api_key` is provided to the `Client` object. 
+- `OPPER_PROJECT` is attached to traces and can be used for filtering in the Opper UI.
+- `OPPER_DEFAULT_MODEL` will define the model used by functions created with the `fn` decorator
+
+When using the `fn` decorator the SDK client is automatically initialized with the `OPPER_API_KEY` environment variable.
+
 ## Using the `fn` decorator
 
 ```python
 from opperai import fn
 
 @fn()
 def translate(text: str, target_language: str) -> str:
@@ -133,15 +143,10 @@
 ## Retrieval
 
 ```python
 client.indexes.retrieve(index_id=42, "Who is the president of the USA?", 3)
 
 ```
 
-## Configuration
-
-### Environment variable
-
-The `OPPER_API_KEY` environment variable is read by the SDK if no `api_key` is provided to the `Client` object. 
-`OPPER_PROJECT` is attached to traces and can be used for filtering in the Opper UI.
+# Examples
 
-When using the `fn` decorator the SDK client is automatically initialized with the `OPPER_API_KEY` environment variable.
+See examples in our [documentation](https://docs.opper.ai)
```


# Comparing `tmp/th2_data_services-2.0.0.dev8934542107.tar.gz` & `tmp/th2_data_services-2.0.0.dev8934901680.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "th2_data_services-2.0.0.dev8934542107.tar", last modified: Fri May  3 05:30:18 2024, max compression
+gzip compressed data, was "th2_data_services-2.0.0.dev8934901680.tar", last modified: Fri May  3 06:16:27 2024, max compression
```

## Comparing `th2_data_services-2.0.0.dev8934542107.tar` & `th2_data_services-2.0.0.dev8934901680.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.773842 th2_data_services-2.0.0.dev8934542107/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-05-03 05:30:18.773842 th2_data_services-2.0.0.dev8934542107/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    35047 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-03 05:30:04.000000 th2_data_services-2.0.0.dev8934542107/package_info.json
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 05:30:18.773842 th2_data_services-2.0.0.dev8934542107/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.765842 th2_data_services-2.0.0.dev8934542107/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.765842 th2_data_services-2.0.0.dev8934542107/th2_data_services/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/_internal/perf_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.765842 th2_data_services-2.0.0.dev8934542107/th2_data_services/config/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    41868 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.765842 th2_data_services-2.0.0.dev8934542107/th2_data_services/dummy/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/dummy/data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.765842 th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/etc_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    26246 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/parent_event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.769842 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.769842 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/utils/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.769842 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/_is_sorted_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    16455 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/aggregation_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/az_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/categorizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/decode_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.769842 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/totals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/json_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.769842 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/message_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/message_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/message_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/message_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22242 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/path_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/perfect_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/script_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/sse_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.773842 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/stream_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/stream_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/stream_utils/stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/total_category_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.773842 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/viewer_structs/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/viewer_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/viewer_structs/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.765842 th2_data_services-2.0.0.dev8934542107/th2_data_services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-05-03 05:30:18.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-03 05:30:18.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 05:30:18.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-03 05:30:18.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 05:30:18.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:16:27.967967 th2_data_services-2.0.0.dev8934901680/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-05-03 06:16:27.967967 th2_data_services-2.0.0.dev8934901680/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    35047 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-03 06:16:19.000000 th2_data_services-2.0.0.dev8934901680/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 06:16:27.967967 th2_data_services-2.0.0.dev8934901680/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:16:27.959967 th2_data_services-2.0.0.dev8934901680/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:16:27.959967 th2_data_services-2.0.0.dev8934901680/th2_data_services/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/_internal/perf_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:16:27.959967 th2_data_services-2.0.0.dev8934901680/th2_data_services/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41868 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:16:27.959967 th2_data_services-2.0.0.dev8934901680/th2_data_services/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/dummy/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:16:27.959967 th2_data_services-2.0.0.dev8934901680/th2_data_services/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/event_tree/etc_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/event_tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26246 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/event_tree/event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/event_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/event_tree/parent_event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:16:27.959967 th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:16:27.959967 th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/utils/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:16:27.963967 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/_is_sorted_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16455 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/aggregation_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/az_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/categorizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/decode_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:16:27.963967 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/event_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/event_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/event_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/event_utils/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/event_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/event_utils/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/event_utils/totals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/json_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:16:27.963967 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/message_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/message_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/message_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/message_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22097 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/path_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/perfect_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/script_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/sse_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:16:27.963967 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/stream_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/stream_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/stream_utils/stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/total_category_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:16:27.963967 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/viewer_structs/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/viewer_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-05-03 06:15:01.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/viewer_structs/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:16:27.959967 th2_data_services-2.0.0.dev8934901680/th2_data_services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-05-03 06:16:27.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-03 06:16:27.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 06:16:27.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-03 06:16:27.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 06:16:27.000000 th2_data_services-2.0.0.dev8934901680/th2_data_services.egg-info/top_level.txt
```

### Comparing `th2_data_services-2.0.0.dev8934542107/LICENSE` & `th2_data_services-2.0.0.dev8934901680/LICENSE`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/PKG-INFO` & `th2_data_services-2.0.0.dev8934901680/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 325f  : 2.1.Name: th2_
 00000020: 6461 7461 5f73 6572 7669 6365 730a 5665  data_services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3839 3334 3534 3231 3037 0a53 756d 6d61  8934542107.Summa
+00000040: 3839 3334 3930 3136 3830 0a53 756d 6d61  8934901680.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev8934542107/README.md` & `th2_data_services-2.0.0.dev8934901680/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/setup.py` & `th2_data_services-2.0.0.dev8934901680/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/_internal/__init__.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/_internal/perf_tests.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/_internal/perf_tests.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/config/__init__.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/config/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/config/config.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/config/config.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/data.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/data.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/dummy/__init__.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/dummy/data_source.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/dummy/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/__init__.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/etc_driver.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/event_tree/etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/event_tree.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/event_tree/event_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/event_tree_collection.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/event_tree/event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/exceptions.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/event_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/parent_event_tree_collection.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/event_tree/parent_event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/exceptions.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/__init__.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/adapter.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/command.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/data_source.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/source_api.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/struct.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/stub_builder.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/utils/__init__.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/utils/converter.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/utils/converter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/utils/resolver.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/interfaces/utils/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/_is_sorted_result.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/_is_sorted_result.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/_json.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/_json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/_types.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/_types.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/aggregation_classes.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/aggregation_classes.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/az_tree.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/az_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/categorizers.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/categorizers.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/category.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/category.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/converters.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/converters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/decode_error_handler.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/decode_error_handler.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/display.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/__init__.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/event_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/display.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/event_utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/event_utils.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/event_utils/event_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/frequencies.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/event_utils/totals.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,166 +8,192 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from deprecated.classic import deprecated
+from typing import Callable, Dict, Iterable, List
+from collections import defaultdict
 
-from th2_data_services.utils import misc_utils
-from typing import Callable, Iterable, List, Literal, Optional
+from deprecated.classic import deprecated
 
 from th2_data_services.utils._types import Th2Event
-from th2_data_services.utils.aggregation_classes import FrequencyCategoryTable
-from th2_data_services.config import options
+from th2_data_services.utils.aggregation_classes import CategoryTotal, TotalCategoryTable
+from th2_data_services.utils.total_category_calculator import TotalCategoryCalculator
 from th2_data_services.utils.category import Category
 
+from th2_data_services.config import options
+
+
+"""
+These functions return how many events were in some category.
+"""
 
+
+# USEFUL
 # STREAMING
+# TODO - NOT-READY -- event["successful"] should be updated by resolver
+# categorizer - expects that it will return str
+# def get_category_totals(
+#     events: Iterable[Th2Event], categorizer: Callable[[Dict], str], ignore_status: bool = False
+# ) -> StatsTotal:
+#     """Returns dictionary quantities of events for different categories.
+#
+#     Args:
+#         events (List[Dict]): TH2-Events
+#         categorizer (Callable): Categorizer function
+#         ignore_status (bool): Concatenate status string, defaults to False.
+#
+#     Returns:
+#         Dict[str, int]
+#
+#     Example:
+#         >>> get_category_totals(events=events,
+#                                 categorizer=lambda e: e["eventType"])
+#             defaultdict(<class 'int'>, {'Service event [ok]': 9531, 'Info [ok]': 469})
+#         >>> get_category_totals(events=events,
+#                                 categorizer=lambda e: e["eventType"],
+#                                 ignore_status=True)
+#             defaultdict(<class 'int'>, {'Service event': 9531, 'Info': 469})
+#     """
+#     event_categories = defaultdict(int)
+#     for event in events:
+#         category = categorizer(event)
+#         if not ignore_status:
+#             status = " [ok]" if options.EVENT_FIELDS_RESOLVER.get_status(event) else " [fail]"
+#             category += status
+#         event_categories[category] += 1
+#
+#     return CategoryTotal(event_categories)
+
+# TODO - we have categorizer and Category now
+#   It's a good idea to unite them
 @deprecated(
-    reason='Use "get_category_frequencies2" instead. \n'
-    "We want to have unification in functions.\n"
-    "Tell DS team if you dont agree or have some ideas."
+    reason='Use "get_category_totals2" instead. \n'
+    "It provides more advantages. \n"
+    "Make sure, it has another interface.\n"
+    "Example:\n"
+    '  metrics = [Category("date", lambda m: m["eventType"])] \n '
+    '  totals.get_category_totals2(events, metrics).sort_by("date")'
 )
-def get_category_frequencies(
-    events: Iterable[Th2Event],
-    categories: List[str],
-    categorizer: Callable,
-    aggregation_level: str = "seconds",
-    object_expander=None,
-) -> FrequencyCategoryTable:
-    """Returns event frequencies based on event category.
+def get_category_totals(
+    events: Iterable[Th2Event], categorizer: Callable[[Dict], str], ignore_status: bool = False
+) -> CategoryTotal:
+    """Returns dictionary quantities of events for different categories.
 
     Args:
-        events (Iterable[Th2Event]): TH2-Events
-        categories (List[str]): Event Categories
-        categorizer (Callable): Categorizer Method
-        aggregation_level (Optional, str): Aggregation Level
+        events (List[Dict]): TH2-Events
+        categorizer (Callable): Categorizer function
+        ignore_status (bool): Concatenate status string, defaults to False.
 
     Returns:
-        List[List[str]]
+        Dict[str, int]
 
     Example:
-        >>> get_category_frequencies(events=events,
-                                     categories=["Info", "ModelMatrix"],
-                                     categorizer=lambda e: e["eventType"],
-                                     aggregation_level="seconds" # Optional
-                                     )
-        [
-            ['timestamp', 'Info', 'ModelMatrix'],
-            ['2022-03-16T02:00:00', 4, 0],
-            ['2022-03-16T02:00:31', 1, 0],
-            ['2022-03-16T02:00:32', 4, 0],
-            ...
-        ]
-
+        >>> get_category_totals(events=events,
+                                categorizer=lambda e: e["eventType"])
+            defaultdict(<class 'int'>, {'Service event [ok]': 9531, 'Info [ok]': 469})
+        >>> get_category_totals(events=events,
+                                categorizer=lambda e: e["eventType"],
+                                ignore_status=True)
+            defaultdict(<class 'int'>, {'Service event': 9531, 'Info': 469})
     """
-    return misc_utils.get_objects_frequencies2(
-        events,
-        categories,
-        categorizer,
-        # TODO -- we shouldn't know internal structure!!! - epochSeconds
-        lambda e: options.EVENT_FIELDS_RESOLVER.get_start_timestamp(e)["epochSecond"],
-        aggregation_level=aggregation_level,
-        object_expander=object_expander,
-    )
+    event_categories = defaultdict(int)
+    for event in events:
+        category = categorizer(event)
+        if not ignore_status:
+            status = " [ok]" if options.EVENT_FIELDS_RESOLVER.get_status(event) else " [fail]"
+            category += status
+        event_categories[category] += 1
+
+    return CategoryTotal(event_categories)
 
 
-# Doesn't use category name now. Category values are table header.
-def get_category_frequencies2(
+# TODO - it will be renamed to get_category_totals before release
+def get_category_totals2(
     events: Iterable[Th2Event],
-    category: Category,
-    aggregation_level: str = "seconds",
-    filter_: Optional[Callable] = None,
-    gap_mode: Literal[1, 2, 3] = 1,
-    zero_anchor: bool = False,
-    include_total: bool = False,
-) -> FrequencyCategoryTable:
-    """Returns event frequencies based on event category.
+    categories: List[Category],
+    # order=None
+) -> TotalCategoryTable:
+    """More advanced totals with multiple columns.
+
+    Examples:
+        metrics = [
+            Category('date', lambda m: Th2TimestampConverter.to_datetime(m['startTimestamp']).date()) ]
+        totals.get_category_totals2(events, metrics).sort_by('date')
 
-    For more info please see: https://github.com/th2-net/th2-data-services/blob/dev_2.0.0/documentation/frequencies.md
+    Args:
+        events:
+        categories:
+
+    Returns:
+        TotalCategoryTable
+    """
+    # if order is None:
+    #     order = [metrics]
+    # else:
+    #     order = [order]
+    if isinstance(categories, Category):
+        categories = [categories]
+
+    ctc = TotalCategoryCalculator(categories, [categories])
+    ctc.handle_objects(events)
+    tct = ctc.get_table(categories)
+    return tct
+
+
+def get_attached_messages_totals(events: Iterable[Th2Event]) -> CategoryTotal:
+    # USEFUL
+    # STREAMING
+    # TODO - NOT-READY -- event["attachedMessageIds"] should be updated by resolver
+    """Returns dictionary quantities of messages attached to events for each stream.
 
     Args:
-        events (Iterable[Th2Event]): TH2-Events
-        category: The name of the category doesn't make sence.
-            Used just for unification to use general Category class.
-        aggregation_level (Optional, str): Aggregation Level
-        filter_: Event filter function
-        gap_mode:
-            1 - Every range starts with actual event timestamp,
-            2 - Ranges are split equally,
-            3 - Same as 2, but filled with empty ranges in between
-        zero_anchor: If False anchor used is first timestamp from event, if True anchor is 0
-        include_total: Will add Total column if True.
+        events (List[Dict]): TH2-Events
 
     Returns:
-        List[List[str]]
+        Dict[str, int]
 
     Example:
-        >>> get_category_frequencies(events=events,
-                                     categories=["Info", "ModelMatrix"],
-                                     categorizer=lambda e: e["eventType"],
-                                     aggregation_level="seconds" # Optional
-                                     )
-        [
-            ['timestamp', 'Info', 'ModelMatrix'],
-            ['2022-03-16T02:00:00', 4, 0],
-            ['2022-03-16T02:00:31', 1, 0],
-            ['2022-03-16T02:00:32', 4, 0],
-            ...
-        ]
-
+        >>> get_attached_messages_totals(events=events)
+            defaultdict(<class 'int'>, {'envtn2_msfix5:first': 25262,
+                                        'envtn2_jpmfix1:second': 1702, ...)
     """
-    return misc_utils.get_objects_frequencies2(
-        events,
-        categories=[],
-        categorizer=category.get_func,
-        # TODO -- we shouldn't know internal structure!!! - epochSeconds
-        timestamp_function=lambda e: options.EVENT_FIELDS_RESOLVER.get_start_timestamp(e)[
-            "epochSecond"
-        ],
-        aggregation_level=aggregation_level,
-        objects_filter=filter_,
-        gap_mode=gap_mode,
-        zero_anchor=zero_anchor,
-        include_total=include_total,
-    )
-
-
-# STREAMING
-# TODO - slava
-#   Do we really need it? Why user cannot just use this one line?
-#   Maybe better to have prepared list of categorizers? e.g. in form of Adapters.
-#   get_category_frequencies(events, types_list, EventCategorizer.type)
-#   or idea to creat class TypeFrequences
-#   GetFrequences.by_type_category
-#   GetFrequences.by_name_category
-#   GetFrequences.by_category
-#    OR maybe better to separate them to modules
-#    utils.frequencies.
-def get_type_frequencies(
-    events: Iterable[Th2Event], types: List[str], aggregation_level="seconds"
-) -> FrequencyCategoryTable:
-    """Returns event frequencies based on event type.
+    streams = defaultdict(int)
+    for event in events:
+        for message_id in options.EVENT_FIELDS_RESOLVER.get_attached_messages_ids(event):
+            key = message_id[: message_id.rindex(":")]
+            streams[key] += 1
+
+    return CategoryTotal(streams)
+
+
+def get_type_totals(events: Iterable[Th2Event]) -> CategoryTotal:
+    # TODO - USEFULL ??? Do we need ignore status??
+    # partly the same as get_category_totals and WO ignore status
+    # Because it's the same we can you get_category_totals inside
+    #
+    # STREAMING
+    # TODO - NOT-READY -- event["successful"] should be updated by resolver
+    """Returns dictionary quantities of events for different event types.
 
     Args:
-        events (Iterable[Th2Event]): TH2-Events
-        types (List[str]): Event Types
-        aggregation_level (Optional, str): Aggregation Level
+        events (List[Dict]): TH2-Events
 
     Returns:
-        List[List[str]]: List Of Frequency Lists
+        Dict[str, int]
 
     Example:
-        >>> get_type_frequencies(events=events, types=["Info", "ModelMatrix"])
-        [
-            ['timestamp', 'Info', 'ModelMatrix'],
-            ['2022-03-16T02:00:00', 4, 0],
-            ['2022-03-16T02:00:31', 1, 0],
-            ['2022-03-16T02:00:32', 4, 0],
-            ...
-        ]
+        >>> get_type_totals(events=events)
+            {
+                "eventType eventStatus": count,
+                ...
+            }
     """
-    return get_category_frequencies(
-        events, types, lambda e: options.EVENT_FIELDS_RESOLVER.get_type(e), aggregation_level
-    )
+    event_types = defaultdict(int)
+    for event in events:
+        status = " [ok]" if options.EVENT_FIELDS_RESOLVER.get_status(event) else " [fail] "
+        event_type = options.EVENT_FIELDS_RESOLVER.get_type(event) + status
+        event_types[event_type] += 1
+
+    return CategoryTotal(event_types)
```

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/select.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/event_utils/select.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/experimental.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/experimental.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/json_tree.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/json_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/message_utils/__init__.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/message_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/message_utils/frequencies.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/message_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/message_utils/message_utils.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/message_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/misc_utils.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/misc_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from collections import defaultdict
-from typing import Any, Callable, Dict, Iterable, List, Tuple
+from typing import Any, Callable, Dict, Iterable, List, Tuple, Literal
 from datetime import datetime, timezone
 
 from deprecated.classic import deprecated
 
 from th2_data_services.utils._types import Th2Event
 
 # TODO - we have special converters for it in ds-2.0 (ProtobufTimestampConverter)
@@ -122,73 +122,73 @@
     objects_stream: Iterable[Th2Event],
     categories: List[str],  # TODO - can be None to collect all values or []
     categorizer: Callable,
     timestamp_function: Callable,
     aggregation_level: str = "seconds",
     object_expander: Callable = None,
     objects_filter: Callable = None,
-    gap_mode: int = 1,
+    gap_mode: Literal[1, 2, 3] = 1,
     zero_anchor: bool = False,
-    include_total: bool = False,
+    include_total: bool = True,
 ) -> FrequencyCategoryTable:
     # TODO - used by both messages and events get_category_frequencies
     """Returns objects frequencies based on categorizer.
 
     Returns timestamps in UTC format.
 
     For more info please see: https://github.com/th2-net/th2-data-services/blob/dev_2.0.0/documentation/frequencies.md
 
     Args:
         objects_stream: Objects stream
-        categories: Categories list
+        categories: Categories list.
+            Provide [] or None to collect all possible values.
         categorizer: Categorizer function
         timestamp_function: Timestamp function
         aggregation_level: Aggregation level
         object_expander: Object expander function
         objects_filter: Object filter function
-        gap_mode: 1 - Every range starts with actual message timestamp, 2 - Ranges are split equally, 3 - Same as 2, but filled with empty ranges in between
+        gap_mode:
+            1 - Every range starts with actual message timestamp,
+            2 - Ranges are split equally,
+            3 - Same as 2, but filled with empty ranges in between
         zero_anchor: If False anchor used is first timestamp from message, if True anchor is 0
         include_total: Will add Total column if True.
 
     Returns:
         List[List]
 
     Examples:
         It'll return the table like this.
-        +--------+---------------------+-------------------+------------+---------------+---------+
-        |        | timestamp           | ExecutionReport   | NewOrder   | OrderCancel   |   Total |
-        +========+=====================+===================+============+===============+=========+
-        |        | 2023-08-13T08:53:05 | 1                 | 1          | 2             |       4 |
-        +--------+---------------------+-------------------+------------+---------------+---------+
-        |        | 2023-08-14T08:53:05 | 1                 | 1          | 2             |       4 |
-        +--------+---------------------+-------------------+------------+---------------+---------+
-        |        | 2023-08-15T08:53:05 | 0                 | 1          | 2             |       3 |
-        +--------+---------------------+-------------------+------------+---------------+---------+
-        |        | 2023-08-16T08:53:05 | 0                 | 1          | 1             |       2 |
-        +--------+---------------------+-------------------+------------+---------------+---------+
-        |        | 2023-08-17T08:53:05 | 1                 | 0          | 1             |       2 |
-        +--------+---------------------+-------------------+------------+---------------+---------+
-        |        | 2023-08-18T08:53:05 | 0                 | 1          | 0             |       1 |
-        +--------+---------------------+-------------------+------------+---------------+---------+
-        |        | 2023-08-19T08:53:05 | 1                 | 0          | 1             |       2 |
-        +--------+---------------------+-------------------+------------+---------------+---------+
-        |        | 2023-08-20T08:53:05 | 0                 | 1          | 1             |       2 |
-        +--------+---------------------+-------------------+------------+---------------+---------+
-        |        | 2023-08-21T08:53:05 | 1                 | 2          | 0             |       3 |
-        +--------+---------------------+-------------------+------------+---------------+---------+
-        |        | 2023-08-22T08:53:05 | 1                 | 0          | 0             |       1 |
-        +--------+---------------------+-------------------+------------+---------------+---------+
-        |        | 2023-08-23T08:53:05 | 0                 | 4          | 1             |       5 |
-        +--------+---------------------+-------------------+------------+---------------+---------+
-        |        | 2023-08-24T08:53:05 | 0                 | 1          | 0             |       1 |
-        +--------+---------------------+-------------------+------------+---------------+---------+
-        | count  |                     |                   |            |               |      12 |
-        +--------+---------------------+-------------------+------------+---------------+---------+
-        | totals |                     | 6                 | 13         | 11            |      30 |
-        +--------+---------------------+-------------------+------------+---------------+---------+
+        +--------+-------------------+-----------------+-------------------+------------+---------------+---------+
+        |        | timestamp_start   | timestamp_end   | ExecutionReport   | NewOrder   | OrderCancel   |   Total |
+        +========+===================+=================+===================+============+===============+=========+
+        |        | 2023-08-13        | 2023-08-14      | 1                 | 1          | 2             |       4 |
+        +--------+-------------------+-----------------+-------------------+------------+---------------+---------+
+        |        | 2023-08-14        | 2023-08-15      | 1                 | 1          | 2             |       4 |
+        +--------+-------------------+-----------------+-------------------+------------+---------------+---------+
+        |        | 2023-08-16        | 2023-08-17      | 0                 | 2          | 3             |       5 |
+        +--------+-------------------+-----------------+-------------------+------------+---------------+---------+
+        |        | 2023-08-17        | 2023-08-18      | 1                 | 0          | 1             |       2 |
+        +--------+-------------------+-----------------+-------------------+------------+---------------+---------+
+        |        | 2023-08-19        | 2023-08-20      | 1                 | 1          | 0             |       2 |
+        +--------+-------------------+-----------------+-------------------+------------+---------------+---------+
+        |        | 2023-08-20        | 2023-08-21      | 0                 | 0          | 2             |       2 |
+        +--------+-------------------+-----------------+-------------------+------------+---------------+---------+
+        |        | 2023-08-21        | 2023-08-22      | 1                 | 3          | 0             |       4 |
+        +--------+-------------------+-----------------+-------------------+------------+---------------+---------+
+        |        | 2023-08-22        | 2023-08-23      | 1                 | 0          | 0             |       1 |
+        +--------+-------------------+-----------------+-------------------+------------+---------------+---------+
+        |        | 2023-08-23        | 2023-08-24      | 0                 | 3          | 0             |       3 |
+        +--------+-------------------+-----------------+-------------------+------------+---------------+---------+
+        |        | 2023-08-24        | 2023-08-25      | 0                 | 2          | 1             |       3 |
+        +--------+-------------------+-----------------+-------------------+------------+---------------+---------+
+        | count  |                   |                 |                   |            |               |      10 |
+        +--------+-------------------+-----------------+-------------------+------------+---------------+---------+
+        | totals |                   |                 | 6                 | 13         | 11            |      30 |
+        +--------+-------------------+-----------------+-------------------+------------+---------------+---------+
     """
     if gap_mode == 1 and zero_anchor:
         raise Exception("gap_mode=1 and zero_anchor=True are not supported together")
     TOTAL_FIELD = "Total"
     frequencies = {}
     anchor = 0
     categories_set = set()
@@ -241,19 +241,21 @@
                         frequencies[epoch][category] = 0
                     frequencies[epoch][category] += 1
                     if include_total:
                         if TOTAL_FIELD not in frequencies[epoch]:
                             frequencies[epoch][TOTAL_FIELD] = 0
                         frequencies[epoch][TOTAL_FIELD] += 1
 
+    sorted_categories = sorted(categories_set)
+
     header = ["timestamp_start", "timestamp_end"]
     if categories:
         header.extend(categories)
     else:
-        header.extend(categories_set)
+        header.extend(sorted_categories)
 
     if include_total:
         header.append(TOTAL_FIELD)
 
     results = [header]
     timestamps = list(sorted(frequencies.keys()))
     # Expected that timestamp is seconds.
@@ -277,30 +279,24 @@
         et_string = _round_timestamp_string_aggregation(
             timestamp + _time_str_to_seconds(aggregation_level), aggregation_level
         )
         line = [st_string, et_string]
         if categories:
             line.extend(frequencies[timestamp].values())
         else:
-            for category in categories_set:
+            for category in sorted_categories:
                 line.append(frequencies[timestamp][category]) if category in frequencies[
                     timestamp
                 ] else line.append(0)
             if include_total:
                 line.append(sum(line[2:]))
 
         results.append(line)
 
     r = FrequencyCategoryTable(header=header, rows=results[1:])
-    if not categories and include_total:
-        # Put TOTAL_FIELD in the end of the header.
-        categories_names = categories_set.copy()
-        sorted_categories_names = ["timestamp_start", "timestamp_end"] + sorted(categories_names)
-        sorted_categories_names.append(TOTAL_FIELD)
-        r = r.change_columns_order(sorted_categories_names)
 
     return r
 
 
 # STREAMABLE (?)
 def analyze_stream_sequence(
     stream: Iterable[Th2Event],
```

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/path_utils.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/perfect_table.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/perfect_table.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/script_report_utils.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/script_report_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/sse_client.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/stream_utils/__init__.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/stream_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/stream_utils/stream_utils.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/stream_utils/stream_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/time.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/time.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/total_category_calculator.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/total_category_calculator.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/viewer_structs/__init__.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/viewer_structs/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/viewer_structs/verification.py` & `th2_data_services-2.0.0.dev8934901680/th2_data_services/utils/viewer_structs/verification.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services.egg-info/PKG-INFO` & `th2_data_services-2.0.0.dev8934901680/th2_data_services.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 322d  : 2.1.Name: th2-
 00000020: 6461 7461 2d73 6572 7669 6365 730a 5665  data-services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3839 3334 3534 3231 3037 0a53 756d 6d61  8934542107.Summa
+00000040: 3839 3334 3930 3136 3830 0a53 756d 6d61  8934901680.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services.egg-info/SOURCES.txt` & `th2_data_services-2.0.0.dev8934901680/th2_data_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8934542107/th2_data_services.egg-info/requires.txt` & `th2_data_services-2.0.0.dev8934901680/th2_data_services.egg-info/requires.txt`

 * *Files identical despite different names*


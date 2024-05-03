# Comparing `tmp/th2_data_services-2.0.0.dev8831728420.tar.gz` & `tmp/th2_data_services-2.0.0.dev8934542107.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services-2.0.0.dev8831728420.tar", last modified: Thu Apr 25 11:29:41 2024, max compression
+gzip compressed data, was "th2_data_services-2.0.0.dev8934542107.tar", last modified: Fri May  3 05:30:18 2024, max compression
```

## Comparing `th2_data_services-2.0.0.dev8831728420.tar` & `th2_data_services-2.0.0.dev8934542107.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:29:41.000000 th2_data_services-2.0.0.dev8831728420/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-04-25 11:29:41.000000 th2_data_services-2.0.0.dev8831728420/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    35047 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-25 11:29:31.000000 th2_data_services-2.0.0.dev8831728420/package_info.json
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 11:29:41.000000 th2_data_services-2.0.0.dev8831728420/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:29:41.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:29:41.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/_internal/perf_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:29:41.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/config/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    41868 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:29:41.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/dummy/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/dummy/data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:29:41.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/event_tree/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/event_tree/etc_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/event_tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    26246 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/event_tree/event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/event_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/event_tree/parent_event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:29:41.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:29:41.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/utils/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:29:41.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/_is_sorted_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    16455 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/aggregation_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/az_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/categorizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/decode_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:29:41.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/event_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/event_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/event_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/event_utils/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/event_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/event_utils/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/event_utils/totals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/json_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:29:41.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/message_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/message_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/message_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/message_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22242 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/path_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/perfect_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/script_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/sse_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:29:41.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/stream_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/stream_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/stream_utils/stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/total_category_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:29:41.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/viewer_structs/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/viewer_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-04-25 11:28:21.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/viewer_structs/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:29:41.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-04-25 11:29:40.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-25 11:29:41.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 11:29:40.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-25 11:29:40.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 11:29:40.000000 th2_data_services-2.0.0.dev8831728420/th2_data_services.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.773842 th2_data_services-2.0.0.dev8934542107/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-05-03 05:30:18.773842 th2_data_services-2.0.0.dev8934542107/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    35047 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-03 05:30:04.000000 th2_data_services-2.0.0.dev8934542107/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 05:30:18.773842 th2_data_services-2.0.0.dev8934542107/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.765842 th2_data_services-2.0.0.dev8934542107/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.765842 th2_data_services-2.0.0.dev8934542107/th2_data_services/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/_internal/perf_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.765842 th2_data_services-2.0.0.dev8934542107/th2_data_services/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41868 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.765842 th2_data_services-2.0.0.dev8934542107/th2_data_services/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/dummy/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.765842 th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/etc_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26246 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/parent_event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.769842 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.769842 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/utils/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.769842 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/_is_sorted_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16455 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/aggregation_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/az_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/categorizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/decode_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.769842 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/totals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/json_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.769842 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/message_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/message_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/message_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/message_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22242 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/path_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/perfect_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/script_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/sse_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.773842 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/stream_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/stream_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/stream_utils/stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/total_category_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.773842 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/viewer_structs/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/viewer_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-05-03 05:29:05.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/viewer_structs/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:30:18.765842 th2_data_services-2.0.0.dev8934542107/th2_data_services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-05-03 05:30:18.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-03 05:30:18.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 05:30:18.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-03 05:30:18.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 05:30:18.000000 th2_data_services-2.0.0.dev8934542107/th2_data_services.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `th2_data_services-2.0.0.dev8831728420/PKG-INFO` & `th2_data_services-2.0.0.dev8934542107/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 325f  : 2.1.Name: th2_
 00000020: 6461 7461 5f73 6572 7669 6365 730a 5665  data_services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3838 3331 3732 3834 3230 0a53 756d 6d61  8831728420.Summa
+00000040: 3839 3334 3534 3231 3037 0a53 756d 6d61  8934542107.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
@@ -2636,15 +2636,15 @@
 0000a4b0: 2020 2020 2020 2d20 5b67 6574 5f73 7461        - [get_sta
 0000a4c0: 7274 6564 5f65 7861 6d70 6c65 2e70 795d  rted_example.py]
 0000a4d0: 2865 7861 6d70 6c65 732f 6765 745f 7374  (examples/get_st
 0000a4e0: 6172 7465 645f 6578 616d 706c 652e 7079  arted_example.py
 0000a4f0: 290a 2020 2020 2020 2020 0a50 6c61 7466  ).        .Platf
 0000a500: 6f72 6d3a 2055 4e4b 4e4f 574e 0a52 6571  orm: UNKNOWN.Req
 0000a510: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
-0000a520: 332e 370a 4465 7363 7269 7074 696f 6e2d  3.7.Description-
+0000a520: 332e 380a 4465 7363 7269 7074 696f 6e2d  3.8.Description-
 0000a530: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
 0000a540: 7874 2f6d 6172 6b64 6f77 6e0a 5072 6f76  xt/markdown.Prov
 0000a550: 6964 6573 2d45 7874 7261 3a20 7264 700a  ides-Extra: rdp.
 0000a560: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
 0000a570: 7264 7035 0a50 726f 7669 6465 732d 4578  rdp5.Provides-Ex
 0000a580: 7472 613a 2072 6470 360a 5072 6f76 6964  tra: rdp6.Provid
 0000a590: 6573 2d45 7874 7261 3a20 6c77 6470 0a50  es-Extra: lwdp.P
```

### Comparing `th2_data_services-2.0.0.dev8831728420/README.md` & `th2_data_services-2.0.0.dev8934542107/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/setup.py` & `th2_data_services-2.0.0.dev8934542107/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,13 +73,13 @@
     description=package_name,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="TH2-devs",
     author_email="th2-devs@exactprosystems.com",
     url="https://github.com/th2-net/th2-data-services",
     license="Apache License 2.0",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=requirements,
     packages=find_namespace_packages(include=["th2_data_services", "th2_data_services.*"]),
     extras_require=CORE_EXTRAS_DEPENDENCIES,
     include_package_data=True,
 )
```

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/_internal/__init__.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/_internal/perf_tests.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/_internal/perf_tests.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/config/__init__.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/config/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/config/config.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/config/config.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/data.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/data.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/dummy/__init__.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/dummy/data_source.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/dummy/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/event_tree/__init__.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/event_tree/etc_driver.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/event_tree/event_tree.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/event_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/event_tree/event_tree_collection.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/event_tree/exceptions.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/event_tree/parent_event_tree_collection.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/event_tree/parent_event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/exceptions.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/__init__.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/adapter.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/command.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/data_source.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/source_api.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/struct.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/stub_builder.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/utils/__init__.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/utils/converter.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/utils/converter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/interfaces/utils/resolver.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/interfaces/utils/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/_is_sorted_result.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/_is_sorted_result.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/_json.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/_json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/_types.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/_types.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/aggregation_classes.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/aggregation_classes.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/az_tree.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/az_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/categorizers.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/categorizers.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/category.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/category.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/converters.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/converters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/decode_error_handler.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/decode_error_handler.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/display.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/event_utils/__init__.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/event_utils/display.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/event_utils/event_utils.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/event_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/event_utils/frequencies.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/event_utils/select.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/select.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/event_utils/totals.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/event_utils/totals.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/experimental.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/experimental.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/json_tree.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/json_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/message_utils/__init__.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/message_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/message_utils/frequencies.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/message_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/message_utils/message_utils.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/message_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/misc_utils.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/path_utils.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/perfect_table.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/perfect_table.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/script_report_utils.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/script_report_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/sse_client.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/stream_utils/__init__.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/stream_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/stream_utils/stream_utils.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/stream_utils/stream_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/time.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/time.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/total_category_calculator.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/total_category_calculator.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/viewer_structs/__init__.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/viewer_structs/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services/utils/viewer_structs/verification.py` & `th2_data_services-2.0.0.dev8934542107/th2_data_services/utils/viewer_structs/verification.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services.egg-info/PKG-INFO` & `th2_data_services-2.0.0.dev8934542107/th2_data_services.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 322d  : 2.1.Name: th2-
 00000020: 6461 7461 2d73 6572 7669 6365 730a 5665  data-services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3838 3331 3732 3834 3230 0a53 756d 6d61  8831728420.Summa
+00000040: 3839 3334 3534 3231 3037 0a53 756d 6d61  8934542107.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
@@ -2636,15 +2636,15 @@
 0000a4b0: 2020 2020 2020 2d20 5b67 6574 5f73 7461        - [get_sta
 0000a4c0: 7274 6564 5f65 7861 6d70 6c65 2e70 795d  rted_example.py]
 0000a4d0: 2865 7861 6d70 6c65 732f 6765 745f 7374  (examples/get_st
 0000a4e0: 6172 7465 645f 6578 616d 706c 652e 7079  arted_example.py
 0000a4f0: 290a 2020 2020 2020 2020 0a50 6c61 7466  ).        .Platf
 0000a500: 6f72 6d3a 2055 4e4b 4e4f 574e 0a52 6571  orm: UNKNOWN.Req
 0000a510: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
-0000a520: 332e 370a 4465 7363 7269 7074 696f 6e2d  3.7.Description-
+0000a520: 332e 380a 4465 7363 7269 7074 696f 6e2d  3.8.Description-
 0000a530: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
 0000a540: 7874 2f6d 6172 6b64 6f77 6e0a 5072 6f76  xt/markdown.Prov
 0000a550: 6964 6573 2d45 7874 7261 3a20 7264 700a  ides-Extra: rdp.
 0000a560: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
 0000a570: 7264 7035 0a50 726f 7669 6465 732d 4578  rdp5.Provides-Ex
 0000a580: 7472 613a 2072 6470 360a 5072 6f76 6964  tra: rdp6.Provid
 0000a590: 6573 2d45 7874 7261 3a20 6c77 6470 0a50  es-Extra: lwdp.P
```

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services.egg-info/SOURCES.txt` & `th2_data_services-2.0.0.dev8934542107/th2_data_services.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 package_info.json
 requirements.txt
 setup.py
 th2_data_services/data.py
 th2_data_services/exceptions.py
```

### Comparing `th2_data_services-2.0.0.dev8831728420/th2_data_services.egg-info/requires.txt` & `th2_data_services-2.0.0.dev8934542107/th2_data_services.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 deprecated
 flatdict~=4.0
-orjson
+orjson<4,>=3.10
 prettytable
 requests~=2.28
 sseclient-py~=1.7
 tabulate
 treelib==1.6.1
 urllib3~=1.26
 wheel>=0.38.1
```


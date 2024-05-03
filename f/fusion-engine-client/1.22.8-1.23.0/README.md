# Comparing `tmp/fusion-engine-client-1.22.8.tar.gz` & `tmp/fusion_engine_client-1.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-engine-client-1.22.8.tar", last modified: Tue Mar 19 14:21:19 2024, max compression
+gzip compressed data, was "fusion_engine_client-1.23.0.tar", last modified: Fri May  3 21:02:55 2024, max compression
```

## Comparing `fusion-engine-client-1.22.8.tar` & `fusion_engine_client-1.23.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:21:19.784439 fusion-engine-client-1.22.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-03-19 14:21:19.780439 fusion-engine-client-1.22.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14885 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:21:19.772439 fusion-engine-client-1.22.8/fusion_engine_client/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:21:19.772439 fusion-engine-client-1.22.8/fusion_engine_client/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/analysis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   128047 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/analysis/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/analysis/attitude.py
--rw-r--r--   0 runner    (1001) docker     (127)    47884 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/analysis/data_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:21:19.776439 fusion-engine-client-1.22.8/fusion_engine_client/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/applications/import_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      313 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/applications/p1_display.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4443 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/applications/p1_extract.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6809 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/applications/p1_lband_extract.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14784 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/applications/p1_print.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:21:19.776439 fusion-engine-client-1.22.8/fusion_engine_client/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62160 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/messages/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    27101 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/messages/control.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/messages/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    26909 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/messages/defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/messages/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/messages/fault_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/messages/gnss_corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/messages/measurement_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    50308 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/messages/measurements.py
--rw-r--r--   0 runner    (1001) docker     (127)    15264 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/messages/ros.py
--rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/messages/signal_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    35603 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/messages/solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/messages/timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:21:19.780439 fusion-engine-client-1.22.8/fusion_engine_client/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17531 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/parsers/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/parsers/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/parsers/fast_indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24420 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/parsers/file_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    28048 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/parsers/mixed_log_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:21:19.780439 fusion-engine-client-1.22.8/fusion_engine_client/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/utils/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/utils/bin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9043 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/utils/construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/utils/enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24918 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/utils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/utils/time_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/fusion_engine_client/utils/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:21:19.780439 fusion-engine-client-1.22.8/fusion_engine_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-03-19 14:21:19.000000 fusion-engine-client-1.22.8/fusion_engine_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-19 14:21:19.000000 fusion-engine-client-1.22.8/fusion_engine_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 14:21:19.000000 fusion-engine-client-1.22.8/fusion_engine_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-19 14:21:19.000000 fusion-engine-client-1.22.8/fusion_engine_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-19 14:21:19.000000 fusion-engine-client-1.22.8/fusion_engine_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-19 14:21:19.000000 fusion-engine-client-1.22.8/fusion_engine_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 14:21:19.784439 fusion-engine-client-1.22.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:21:19.780439 fusion-engine-client-1.22.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/tests/test_construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19673 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/tests/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/tests/test_enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/tests/test_file_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/tests/test_message_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/tests/test_mixed_log_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13200 2024-03-19 14:20:42.000000 fusion-engine-client-1.22.8/tests/test_time_range.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:55.513875 fusion_engine_client-1.23.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-03 21:02:55.513875 fusion_engine_client-1.23.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14885 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:55.501875 fusion_engine_client-1.23.0/fusion_engine_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:55.505875 fusion_engine_client-1.23.0/fusion_engine_client/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/analysis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   128047 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/analysis/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/analysis/attitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47884 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/analysis/data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:55.505875 fusion_engine_client-1.23.0/fusion_engine_client/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/applications/import_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      313 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/applications/p1_display.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4443 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/applications/p1_extract.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6809 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/applications/p1_lband_extract.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16262 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/applications/p1_print.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:55.509875 fusion_engine_client-1.23.0/fusion_engine_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62152 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27163 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29659 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/fault_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/gnss_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/measurement_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50308 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15264 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/ros.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10215 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/signal_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35603 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:55.509875 fusion_engine_client-1.23.0/fusion_engine_client/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17531 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/parsers/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/parsers/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/parsers/fast_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24420 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/parsers/file_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28048 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/parsers/mixed_log_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:55.509875 fusion_engine_client-1.23.0/fusion_engine_client/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/utils/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/utils/bin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/utils/construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/utils/enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24918 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/utils/numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/utils/time_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/utils/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:55.513875 fusion_engine_client-1.23.0/fusion_engine_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-03 21:02:55.000000 fusion_engine_client-1.23.0/fusion_engine_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-03 21:02:55.000000 fusion_engine_client-1.23.0/fusion_engine_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 21:02:55.000000 fusion_engine_client-1.23.0/fusion_engine_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-03 21:02:55.000000 fusion_engine_client-1.23.0/fusion_engine_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-03 21:02:55.000000 fusion_engine_client-1.23.0/fusion_engine_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 21:02:55.000000 fusion_engine_client-1.23.0/fusion_engine_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 21:02:55.513875 fusion_engine_client-1.23.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:55.513875 fusion_engine_client-1.23.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/tests/test_construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19673 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/tests/test_enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/tests/test_file_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/tests/test_message_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/tests/test_mixed_log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13200 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/tests/test_time_range.py
```

### Comparing `fusion-engine-client-1.22.8/PKG-INFO` & `fusion_engine_client-1.23.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.22.8
+Version: 1.23.0
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
-Download-URL: https://github.com/PointOneNav/fusion-engine-client/archive/refs/tags/v1.22.8.tar.gz
+Download-URL: https://github.com/PointOneNav/fusion-engine-client/archive/refs/tags/v1.23.0.tar.gz
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
@@ -23,24 +23,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: scipy>=1.5.0
-Requires-Dist: palettable>=3.3.0
 Requires-Dist: numpy>=1.16.0
+Requires-Dist: pymap3d>=2.4.3
 Requires-Dist: aenum>=3.1.1
 Requires-Dist: p1-gpstime>=0.6.3.dev1
-Requires-Dist: pymap3d>=2.4.3
-Requires-Dist: plotly>=4.0.0
-Requires-Dist: colorama>=0.4.4
 Requires-Dist: packaging>=21.0.0
+Requires-Dist: palettable>=3.3.0
+Requires-Dist: colorama>=0.4.4
+Requires-Dist: scipy>=1.5.0
 Requires-Dist: construct>=2.10.0
+Requires-Dist: plotly>=4.0.0
 Requires-Dist: argparse-formatter>=1.4
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: display
 Provides-Extra: tools
 
 Point One FusionEngine protocol support for real-time interaction and control, plus post-processing data analysis tools.
```

### Comparing `fusion-engine-client-1.22.8/README.md` & `fusion_engine_client-1.23.0/README.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/analysis/analyzer.py` & `fusion_engine_client-1.23.0/fusion_engine_client/analysis/analyzer.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/analysis/attitude.py` & `fusion_engine_client-1.23.0/fusion_engine_client/analysis/attitude.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/analysis/data_loader.py` & `fusion_engine_client-1.23.0/fusion_engine_client/analysis/data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/applications/import_utils.py` & `fusion_engine_client-1.23.0/fusion_engine_client/applications/import_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/applications/p1_extract.py` & `fusion_engine_client-1.23.0/fusion_engine_client/applications/p1_extract.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/applications/p1_lband_extract.py` & `fusion_engine_client-1.23.0/fusion_engine_client/applications/p1_lband_extract.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/applications/p1_print.py` & `fusion_engine_client-1.23.0/fusion_engine_client/applications/p1_print.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,21 +15,38 @@
 from ..utils.log import locate_log, DEFAULT_LOG_BASE_DIR
 from ..utils.time_range import TimeRange
 from ..utils.trace import HighlightFormatter, BrokenPipeStreamHandler
 
 _logger = logging.getLogger('point_one.fusion_engine.applications.print_contents')
 
 
-def print_message(header, contents, offset_bytes, format='pretty', bytes=None):
+def add_print_format_argument(parser, *arg_names):
+    parser.add_argument(
+        *arg_names,
+        choices=['binary', 'pretty', 'pretty-binary', 'pretty-binary-payload',
+                 'oneline', 'oneline-detailed', 'oneline-binary', 'oneline-binary-payload'],
+        default='pretty',
+        help="Specify the format used to print the message contents:\n"
+             "- Print the binary representation of each message on a single line, but no other details\n"
+             "- pretty - Print the message contents in a human-readable format (default)\n"
+             "- pretty-binary - Use `pretty` format, but include the binary representation of each message\n"
+             "- pretty-binary-payload - Like `pretty-binary`, but exclude the message header from the binary\n"
+             "- oneline - Print a summary of each message on a single line\n"
+             "- oneline-detailed - Print a one-line summary, including message offset details\n"
+             "- oneline-binary - Use `oneline-detailed` format, but include the binary representation of each message\n"
+             "- oneline-binary-payload - Like `oneline-binary`, but exclude the message header from the binary")
+
+
+def print_message(header, contents, offset_bytes=None, format='pretty', bytes=None):
     if format == 'binary':
         if bytes is None:
             raise ValueError('No data provided for binary format.')
         parts = []
     elif isinstance(contents, MessagePayload):
-        if format in ('oneline', 'oneline-binary', 'oneline-detailed'):
+        if format.startswith('oneline'):
             # The repr string should always start with the message type, then other contents:
             #   [POSE (10000), p1_time=12.029 sec, gps_time=2249:528920.500 (1360724120.500 sec), ...]
             # We want to reformat and insert the additional details as follows for consistency:
             #   POSE (10000) [sequence=10, ... p1_time=12.029 sec, gps_time=2249:528920.500 (1360724120.500 sec), ...]
             message_str = repr(contents).split('\n')[0]
             message_str = message_str.replace('[', '', 1)
             break_idx = message_str.find(',')
@@ -39,33 +56,38 @@
                 message_str = message_str.rstrip(']')
             parts = [message_str]
         else:
             parts = str(contents).split('\n')
     else:
         parts = [f'{header.get_type_string()} (unsupported)']
 
-    if format in ('pretty', 'pretty-binary', 'oneline-detailed', 'oneline-binary'):
-        details = 'sequence=%d, size=%d B, offset=%d B (0x%x)' %\
-                  (header.sequence_number, header.get_message_size(), offset_bytes, offset_bytes)
+    if format != 'oneline':
+        details = 'sequence=%d, size=%d B' % (header.sequence_number, header.get_message_size())
+        if offset_bytes is not None:
+            details += ', offset=%d B (0x%x)' % (offset_bytes, offset_bytes)
 
         idx = parts[0].find('[')
         if idx < 0:
             parts[0] += f' [{details}]'
         else:
             parts[0] = f'{parts[0][:(idx + 1)]}{details}, {parts[0][(idx + 1):]}'
 
     if bytes is None:
         pass
     elif format == 'binary':
         byte_string = bytes_to_hex(bytes, bytes_per_row=-1, bytes_per_col=2).replace('\n', '\n  ')
         parts.insert(1, byte_string)
-    elif format == 'pretty-binary':
+    elif format == 'pretty-binary' or format == 'pretty-binary-payload':
+        if format.endswith('-payload'):
+            bytes = bytes[MessageHeader.calcsize():]
         byte_string = '    ' + bytes_to_hex(bytes, bytes_per_row=16, bytes_per_col=2).replace('\n', '\n    ')
         parts.insert(1, "  Binary:\n%s" % byte_string)
-    elif format == 'oneline-binary':
+    elif format == 'oneline-binary' or format == 'oneline-binary-payload':
+        if format.endswith('-payload'):
+            bytes = bytes[MessageHeader.calcsize():]
         byte_string = '  ' + bytes_to_hex(bytes, bytes_per_row=16, bytes_per_col=2).replace('\n', '\n  ')
         parts.insert(1, byte_string)
 
     _logger.info('\n'.join(parts))
 
 
 def main():
@@ -75,39 +97,37 @@
 other types of data.
 """)
 
     parser.add_argument(
         '--absolute-time', '--abs', action=ExtendedBooleanAction,
         help="Interpret the timestamps in --time as absolute P1 times. Otherwise, treat them as relative to the first "
              "message in the file. Ignored if --time contains a type specifier.")
-    parser.add_argument(
-        '-f', '--format', choices=['binary', 'pretty', 'pretty-binary', 'oneline', 'oneline-detailed',
-                                   'oneline-binary'],
-        default='pretty',
-        help="Specify the format used to print the message contents:\n"
-             "- Print the binary representation of each message on a single line, but no other details\n"
-             "- pretty - Print the message contents in a human-readable format (default)\n"
-             "- pretty-binary - Use `pretty` format, but include the binary representation of each message\n"
-             "- oneline - Print a summary of each message on a single line\n"
-             "- oneline-detailed - Print a one-line summary, including message offset details\n"
-             "- oneline-binary - Use `oneline-detailed` format, but include the binary representation of each message")
-    parser.add_argument(
-        '-s', '--summary', action='store_true',
-        help="Print a summary of the messages in the file.")
+    add_print_format_argument(parser, '-f', '--format', '--display-format')
     parser.add_argument(
         '-m', '--message-type', type=str, action='append',
         help="An optional list of class names corresponding with the message types to be displayed. May be specified "
              "multiple times (-m Pose -m PoseAux), or as a comma-separated list (-m Pose,PoseAux). All matches are"
              "case-insensitive.\n"
              "\n"
              "If a partial name is specified, the best match will be returned. Use the wildcard '*' to match multiple "
              "message types.\n"
              "\n"
              "Supported types:\n%s" % '\n'.join(['- %s' % c for c in message_type_by_name.keys()]))
     parser.add_argument(
+        '-n', '--max', type=int, default=None,
+        help="Print up to a maximum of N messages. If --message-type is specified, only count messages matching the "
+             "specified type(s).")
+    parser.add_argument(
+        '-s', '--summary', action='store_true',
+        help="Print a summary of the messages in the file.")
+    parser.add_argument(
+        '--skip', type=int, default=0,
+        help="Skip the first N messages in the log. If --message-type is specified, only count messages matching the "
+             "specified type(s).")
+    parser.add_argument(
         '-t', '--time', type=str, metavar='[START][:END][:{rel,abs}]',
         help="The desired time range to be analyzed. Both start and end may be omitted to read from beginning or to "
              "the end of the file. By default, timestamps are treated as relative to the first message in the file, "
              "unless an 'abs' type is specified or --absolute-time is set.")
     parser.add_argument('-v', '--verbose', action='count', default=0,
                         help="Print verbose/trace debugging messages.")
 
@@ -191,25 +211,31 @@
     newest_p1_message_type = None
 
     first_system_time_sec = None
     last_system_time_sec = None
     newest_system_time_sec = None
     newest_system_message_type = None
 
+    total_decoded_messages = 0
     total_messages = 0
     bytes_decoded = 0
 
-    def create_stats_entry(): return {'count': 1}
+    def create_stats_entry(): return {'count': 0}
     message_stats = defaultdict(create_stats_entry)
     try:
         for header, message, data, offset_bytes in reader:
-            bytes_decoded += len(data)
+            total_decoded_messages += 1
+            if total_decoded_messages <= options.skip:
+                continue
+            elif options.max is not None and (total_decoded_messages - options.skip) > options.max:
+                break
 
             # Update the data summary in summary mode, or print the message contents otherwise.
             total_messages += 1
+            bytes_decoded += len(data)
             if options.summary:
                 entry = message_stats[header.message_type]
                 entry['count'] += 1
 
                 if message is not None:
                     p1_time = message.get_p1_time()
                     if p1_time is not None:
@@ -238,15 +264,15 @@
                             first_system_time_sec = system_time_sec
                             last_system_time_sec = system_time_sec
                             newest_system_time_sec = system_time_sec
                             newest_system_message_type = header.message_type
                         else:
                             # We allow a small tolerance to account for normal latency between measurements and computed
                             # data like pose solutions, as well as latency between different types of measurements.
-                            dt_sec = newest_system_time_sec - system_time_sec
+                            dt_sec = system_time_sec - newest_system_time_sec
                             if dt_sec < -0.2:
                                 _logger.warning(
                                     'Backwards/restarted system time detected after %s (%s). [new_message=%s, '
                                     'new_system_time=%s, offset=%d B]' %
                                     (system_time_to_str(newest_system_time_sec, is_seconds=True),
                                      str(newest_system_message_type), header.get_type_string(),
                                      system_time_to_str(system_time_sec, is_seconds=True),
@@ -275,15 +301,20 @@
         _logger.info('Selected data size: %d B' % bytes_decoded)
         _logger.info('')
 
         format_string = '| {:<50} | {:>5} | {:>8} |'
         _logger.info(format_string.format('Message Name', 'Type', 'Count'))
         _logger.info(format_string.format('-' * 50, '-' * 5, '-' * 8))
         for type, info in sorted(message_stats.items(), key=lambda x: int(x[0])):
-            name = message_type_to_class[type].__name__ if type in message_type_to_class else "Unknown"
+            if type in message_type_to_class:
+                name = message_type_to_class[type].__name__
+            elif type.is_unrecognized():
+                name = str(type)
+            else:
+                name = f'Unsupported ({str(type)})'
             _logger.info(format_string.format(name, int(type), info['count']))
         _logger.info(format_string.format('-' * 50, '-' * 5, '-' * 8))
         _logger.info(format_string.format('Total', '', total_messages))
     elif total_messages == 0:
         _logger.warning('No valid FusionEngine messages found.')
```

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/messages/configuration.py` & `fusion_engine_client-1.23.0/fusion_engine_client/messages/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -432,63 +432,63 @@
         """
         def __new__(cls, *args, **kwargs):
             # Check if the user specified a single SatelliteType or a list of values, and convert to a mask.
             if len(args) == 1:
                 # SatelliteTypeMaskVal(SatelliteType.GPS)
                 # SatelliteTypeMaskVal('GPS')
                 if isinstance(args[0], SatelliteType) or isinstance(args[0], str):
-                    args = (SatelliteTypeMask.to_bit_mask(args),)
+                    args = (SatelliteTypeMask.to_bitmask(args),)
                 # SatelliteTypeMaskVal([SatelliteType.GPS, SatelliteType.GALILEO])
                 # SatelliteTypeMaskVal(['GPS', 'GALILEO'])
                 elif isinstance(args[0], Iterable):
-                    args = (SatelliteTypeMask.to_bit_mask(args[0])),
+                    args = (SatelliteTypeMask.to_bitmask(args[0])),
                 # SatelliteTypeMaskVal(bit_mask)
                 else:
                     pass
             # Check if the user specified one or more SatelliteTypes values, and convert to a mask:
             #   SatelliteTypeMaskVal(SatelliteType.GPS, SatelliteType.GALILEO)
             #   SatelliteTypeMaskVal('GPS', 'GALILEO')
             elif len(args) > 1:
-                args = (SatelliteTypeMask.to_bit_mask(args),)
+                args = (SatelliteTypeMask.to_bitmask(args),)
 
             return super().__new__(cls, *args, **kwargs)
 
         def __repr__(self):
             return f'{self.__class__.__name__}(value=0x{self.value:02x} ' \
-                   f'({SatelliteTypeMask.bit_mask_to_string(self.value)}))'
+                   f'({SatelliteTypeMask.bitmask_to_string(self.value)}))'
 
     class FrequencyBandMaskVal(IntegerVal):
         """!
         @brief Bitmask specifying enabled @ref FrequencyBand%s.
         """
         def __new__(cls, *args, **kwargs):
             # Check if the user specified a single FrequencyBand or a list of values, and convert to a mask.
             if len(args) == 1:
                 # FrequencyBandMaskVal(FrequencyBand.L1)
                 # FrequencyBandMaskVal('L1')
                 if isinstance(args[0], FrequencyBand) or isinstance(args[0], str):
-                    args = (FrequencyBandMask.to_bit_mask(args),)
+                    args = (FrequencyBandMask.to_bitmask(args),)
                 # FrequencyBandMaskVal([FrequencyBand.L1, FrequencyBand.L5])
                 # FrequencyBandMaskVal(['L1', 'L5'])
                 elif isinstance(args[0], Iterable):
-                    args = (FrequencyBandMask.to_bit_mask(args[0])),
+                    args = (FrequencyBandMask.to_bitmask(args[0])),
                 # FrequencyBandMaskVal(bit_mask)
                 else:
                     pass
             # Check if the user specified one or more FrequencyBands values, and convert to a mask:
             #   FrequencyBandMaskVal(FrequencyBand.L1, FrequencyBand.L5)
             #   FrequencyBandMaskVal('L1', 'L5')
             elif len(args) > 1:
-                args = (FrequencyBandMask.to_bit_mask(args),)
+                args = (FrequencyBandMask.to_bitmask(args),)
 
             return super().__new__(cls, *args, **kwargs)
 
         def __repr__(self):
             return f'{self.__class__.__name__}(value=0x{self.value:02x} ' \
-                   f'({FrequencyBandMask.bit_mask_to_string(self.value)}))'
+                   f'({FrequencyBandMask.bitmask_to_string(self.value)}))'
 
     class CoarseOrientation(NamedTuple):
         """!
         @brief The orientation of a device with respect to the vehicle body axes.
         """
         ## The direction of the device +x axis relative to the vehicle body axes.
         x_direction: Direction = Direction.FORWARD
```

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/messages/control.py` & `fusion_engine_client-1.23.0/fusion_engine_client/messages/control.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,14 +438,17 @@
 
 class DeviceType(IntEnum):
     UNKNOWN = 0
     ATLAS = 1
     LG69T_AM = 2
     LG69T_AP = 3
     LG69T_AH = 4
+    NEXAR_BEAM2K = 5,
+    SSR_LG69T = 6,
+    SSR_DESKTOP = 7,
 
 
 class DeviceIDMessage(MessagePayload):
     """!
     @brief Device identifiers.
     """
     MESSAGE_TYPE = MessageType.DEVICE_ID
```

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/messages/defs.py` & `fusion_engine_client-1.23.0/fusion_engine_client/messages/defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import inspect
 import re
 import struct
 import sys
-from typing import Dict, List, Optional, Set, Type, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Set, Type, Union
 from zlib import crc32
 
 import numpy as np
 
 from .measurement_details import *
 from .signal_defs import *
 from .timestamp import *
 from ..utils import trace as logging
+from ..utils.construct_utils import construct_message_to_string
 from ..utils.enum_utils import IntEnum
 
 _logger = logging.getLogger('point_one.fusion_engine.messages.defs')
 
 if sys.version_info >= (3, 9):
     def _remove_suffix(s, suffix):
         return s.removesuffix(suffix)
@@ -534,18 +535,34 @@
         @param obj The object to be tested.
 
         @return `True` if obj is a class type that is derived from @ref MessagePayload.
         """
         return inspect.isclass(obj) and issubclass(obj, MessagePayload)
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
-        raise NotImplementedError('pack() not implemented.')
+        construct = getattr(self.__class__, 'Construct', None)
+        if construct is not None:
+            values = vars(self)
+            packed_data = construct.build(values)
+            return PackedDataToBuffer(packed_data, buffer, offset, return_buffer)
+        else:
+            raise NotImplementedError('pack() not implemented.')
 
     def unpack(self, buffer: bytes, offset: int = 0, message_version: int = _UNSPECIFIED_VERSION) -> int:
-        raise NotImplementedError('unpack() not implemented.')
+        construct = getattr(self.__class__, 'Construct', None)
+        if construct is not None:
+            parsed = construct.parse(buffer[offset:])
+            self.__dict__.update(parsed)
+            del self.__dict__['_io']
+            return parsed._io.tell()
+        else:
+            raise NotImplementedError('unpack() not implemented.')
+
+    def calcsize(self) -> int:
+        raise NotImplementedError('calcsize() not implemented.')
 
     def get_p1_time(self) -> Timestamp:
         measurement_details = getattr(self, 'details', None)
         if isinstance(measurement_details, MeasurementDetails):
             if measurement_details.measurement_time_source == SystemTimeSource.P1_TIME:
                 return measurement_details.measurement_time
             else:
@@ -582,15 +599,27 @@
             result += f', system_time={system_time_sec:.3f} sec'
 
         result += ']'
 
         return result
 
     def __str__(self):
-        return repr(self)
+        construct = getattr(self.__class__, 'Construct', None)
+        if construct is not None:
+            return self._construct_str_impl()
+        else:
+            return repr(self)
+
+    def _construct_str_impl(self, **kwargs):
+        if 'title' not in kwargs:
+            title = self.__class__.__name__
+            if hasattr(self, 'p1_time'):
+                title += f' @ {self.p1_time}'
+            kwargs['title'] = title
+        return construct_message_to_string(message=self, **kwargs)
 
     @classmethod
     def pack_values(cls, format: Union[str, struct.Struct], buffer: bytes, offset: int = 0, *args):
         """!
         @brief Serialize data into a byte stream.
 
         This is a convenience packing function for consistency with @ref unpack_values(). It behaves similarly to a
@@ -682,14 +711,55 @@
                     value_idx += 1
             else:
                 args[arg_idx] = values[value_idx]
                 value_idx += 1
 
         return size
 
+    @classmethod
+    def to_numpy(cls, messages: Sequence['MessagePayload']):
+        return cls._message_to_numpy(messages)
+
+    @classmethod
+    def _message_to_numpy(cls,
+                          messages: Sequence['MessagePayload'],
+                          fields: Optional[Sequence[str]] = None,
+                          value_to_array: Optional[Dict[str, Callable[[List[Any]], np.ndarray]]] = None) -> \
+            Dict[str, np.ndarray]:
+        if fields is None:
+            if len(messages) > 0:
+                fields = sorted(messages[0].__dict__.keys())
+            elif cls is not MessagePayload:
+                instance = cls()
+                fields = sorted(instance.__dict__.keys())
+            else:
+                raise RuntimeError('Cannot infer message fields.')
+
+        if len(messages) == 0:
+            return {f: np.array(()) for f in fields}
+
+        if value_to_array is None:
+            value_to_array = {}
+
+        def _generic_value_to_array(values):
+            if isinstance(values[0], np.ndarray) and len(values[0]) > 1:
+                return np.array(values).T
+            elif isinstance(values[0], Timestamp):
+                return np.array([float(v) for v in values])
+            else:
+                return np.array(values)
+
+        result = {}
+        for field in fields:
+            to_array = value_to_array.get(field, _generic_value_to_array)
+            values = [getattr(m, field) for m in messages]
+            result[field] = to_array(values)
+
+        return result
+
 
 def PackedDataToBuffer(packed_data: bytes, buffer: Optional[bytes] = None, offset: int = 0,
                        return_buffer: bool = True) -> (bytes, int):
     if buffer is None:
         buffer = packed_data
     else:
         buffer[offset:(offset + len(packed_data))] = packed_data
```

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/messages/device.py` & `fusion_engine_client-1.23.0/fusion_engine_client/messages/device.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/messages/fault_control.py` & `fusion_engine_client-1.23.0/fusion_engine_client/messages/fault_control.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/messages/gnss_corrections.py` & `fusion_engine_client-1.23.0/fusion_engine_client/messages/gnss_corrections.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/messages/measurement_details.py` & `fusion_engine_client-1.23.0/fusion_engine_client/messages/measurement_details.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/messages/measurements.py` & `fusion_engine_client-1.23.0/fusion_engine_client/messages/measurements.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/messages/ros.py` & `fusion_engine_client-1.23.0/fusion_engine_client/messages/ros.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/messages/signal_defs.py` & `fusion_engine_client-1.23.0/fusion_engine_client/messages/signal_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from typing import List, Union
 
 import numpy as np
 
-from ..utils.enum_utils import IntEnum
+from ..utils.enum_utils import IntEnum, enum_bitmask
 
 
 class SatelliteType(IntEnum):
     UNKNOWN = 0
     GPS = 1
     GLONASS = 2
     LEO = 3
@@ -31,94 +31,35 @@
     SatelliteType.SBAS: 'S',
     SatelliteType.IRNSS: 'I'
 }
 
 SatelliteTypeCharReverse = {v: k for k, v in SatelliteTypeChar.items()}
 
 
-class SatelliteTypeMask(IntEnum):
-    GPS = (1 << SatelliteType.GPS)
-    GLONASS = (1 << SatelliteType.GLONASS)
-    LEO = (1 << SatelliteType.LEO)
-    GALILEO = (1 << SatelliteType.GALILEO)
-    BEIDOU = (1 << SatelliteType.BEIDOU)
-    QZSS = (1 << SatelliteType.QZSS)
-    MIXED = (1 << SatelliteType.MIXED)
-    SBAS = (1 << SatelliteType.SBAS)
-    IRNSS = (1 << SatelliteType.IRNSS)
-
+@enum_bitmask(SatelliteType)
+class SatelliteTypeMask:
     ALL = 0xFFFFFFFF
 
-    @classmethod
-    def to_bit_mask(cls, systems: List[Union[SatelliteType, str]]):
-        mask = 0
-        for system in systems:
-            if isinstance(system, str):
-                mask |= getattr(cls, system.upper())
-            else:
-                mask |= (1 << int(system))
-        return mask
-
-    @classmethod
-    def bit_mask_to_systems(cls, mask: int):
-        systems = []
-        for system in SatelliteType:
-            if (mask & (1 << int(system))) != 0:
-                systems.append(system)
-        return systems
-
-    @classmethod
-    def bit_mask_to_string(cls, mask: int):
-        systems = cls.bit_mask_to_systems(mask)
-        return ', '.join(str(s) for s in systems)
-
 
 class SignalType(IntEnum):
     UNKNOWN = 0
 
 
 class FrequencyBand(IntEnum):
     UNKNOWN = 0
     L1 = 1
     L2 = 2
     L5 = 5
     L6 = 6
 
 
-class FrequencyBandMask(IntEnum):
-    L1 = (1 << FrequencyBand.L1)
-    L2 = (1 << FrequencyBand.L2)
-    L5 = (1 << FrequencyBand.L5)
-    L6 = (1 << FrequencyBand.L6)
-
+@enum_bitmask(FrequencyBand)
+class FrequencyBandMask:
     ALL = 0xFFFFFFFF
 
-    @classmethod
-    def to_bit_mask(cls, frequencies: List[Union[FrequencyBand, str]]):
-        mask = 0
-        for freq in frequencies:
-            if isinstance(freq, str):
-                mask |= getattr(cls, freq.upper())
-            else:
-                mask |= (1 << int(freq))
-        return mask
-
-    @classmethod
-    def bit_mask_to_systems(cls, mask: int):
-        frequencies = []
-        for freq in FrequencyBand:
-            if (mask & (1 << int(freq))) != 0:
-                frequencies.append(freq)
-        return frequencies
-
-    @classmethod
-    def bit_mask_to_string(cls, mask: int):
-        systems = cls.bit_mask_to_systems(mask)
-        return ', '.join(str(s) for s in systems)
-
 
 _SHORT_FORMAT = re.compile(r'([%s])(\d+)(?:\s+(\w+))?' % ''.join(SatelliteTypeCharReverse.keys()))
 _LONG_FORMAT = re.compile(r'(\w+)(?:\s+(\w+))(?:\s+PRN\s+(\d+))?')
 
 
 def decode_signal_id(signal_id):
     """!
```

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/messages/solution.py` & `fusion_engine_client-1.23.0/fusion_engine_client/messages/solution.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/messages/timestamp.py` & `fusion_engine_client-1.23.0/fusion_engine_client/messages/timestamp.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     def get_week_tow(self) -> (int, float):
         if self.is_gps():
             week = int(self.seconds / SECONDS_PER_WEEK)
             tow_sec = self.seconds - week * SECONDS_PER_WEEK
             return week, tow_sec
         else:
-            return np.nan, np.nan
+            return -1, np.nan
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = False) -> (bytes, int):
         if math.isnan(self.seconds):
             int_part = Timestamp._INVALID
             frac_part_ns = Timestamp._INVALID
         else:
             int_part = int(self.seconds)
@@ -145,18 +145,21 @@
         return not math.isnan(self.seconds)
 
     def __float__(self):
         return self.seconds
 
     def __str__(self):
         if self.is_gps():
-            return 'GPS: %d:%.3f (%.3f sec)' % (*self.get_week_tow(), self.seconds)
+            return 'GPS: %s' % self.to_gps_str()
         else:
             return 'P1: %.3f sec' % self.seconds
 
+    def to_gps_str(self):
+        return '%d:%.3f (%.3f sec)' % (*self.get_week_tow(), self.seconds)
+
 
 def system_time_to_str(system_time, is_seconds=False):
     if system_time is None:
         return 'None'
 
     if is_seconds:
         system_time_sec = system_time
```

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/parsers/decoder.py` & `fusion_engine_client-1.23.0/fusion_engine_client/parsers/decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/parsers/encoder.py` & `fusion_engine_client-1.23.0/fusion_engine_client/parsers/encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/parsers/fast_indexer.py` & `fusion_engine_client-1.23.0/fusion_engine_client/parsers/fast_indexer.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,23 +20,30 @@
 _READ_SIZE_BYTES = 80 * 1024
 
 _PREAMBLE = struct.unpack('<H', MessageHeader.SYNC)
 
 _logger = logging.getLogger('point_one.fusion_engine.parsers.fast_indexer')
 
 
-def _search_blocks_for_fe(input_path: str, block_starts: List[int]):
+def _search_blocks_for_fe(input_path: str, thread_idx: int, block_starts: List[int]):
     """!
     @brief Search the specified portions of the file for the start offsets of valid FE messages.
 
     @param input_path The path to the file to be read.
     @param block_starts The blocks of data to search for FE messages in.
 
     @return The raw index data corresponding to this thread's data blocks.
     """
+    if len(block_starts) == 0:
+        _logger.trace(f'Skipping search thread {thread_idx}. [num_blocks={len(block_starts)}]', depth=2)
+        return np.array([], dtype=FileIndex._RAW_DTYPE)
+    else:
+        _logger.trace(f'Starting search thread {thread_idx}. '
+                      f'[num_blocks={len(block_starts)}, first={block_starts[0]} B, last={block_starts[-1]} B]',
+                      depth=2)
     header = MessageHeader()
     message_end = 0
     num_syncs = 0
     # Data corresponding to raw values in FileIndex._RAW_DTYPE.
     raw_list: List[Tuple[int, int, int]] = []
     with open(input_path, 'rb') as fd:
         for i in range(len(block_starts)):
@@ -67,14 +74,15 @@
             # Load the potential sync words for the even offsets.
             np_data[0::2] = np.frombuffer(data, dtype=np.uint16, count=word_count)
             # Load the potential sync words for the odd offsets ([AA 31 2E AA] shifted over one byte).
             np_data[1::2] = np.frombuffer(data[1:], dtype=np.uint16, count=word_count)
             # This is lot faster then doing this check in raw Python due to numpy optimizations.
             sync_matches = np.where(np_data == _PREAMBLE)[0]
 
+            _logger.trace(f'Thread {thread_idx}, block {i}: {len(sync_matches)} matches', depth=2)
             num_syncs += len(sync_matches)
 
             # To do the CRC check and find a p1_time the full message needs to be parsed. This
             # section is not particularly optimized. The chance of the preamble appearing in data
             # is relatively low, so this code is in a much less hot path then the preamble sync above.
             for i in sync_matches:
                 absolute_offset = i + block_offset
@@ -101,18 +109,22 @@
                                                MessageHeader.calcsize(), message_version=header.message_version)
                                 p1_time = payload.get_p1_time()
                         except BaseException:
                             pass
                     # Convert the Timestamp to an integer.
                     p1_time_raw = Timestamp._INVALID if math.isnan(p1_time.seconds) else int(p1_time.seconds)
                     message_end = absolute_offset + header.get_message_size()
+                    if _logger.isEnabledFor(logging.getTraceLevel(depth=3)):
+                        _logger.trace(f'Thread {thread_idx}, block {i}: message={header.message_type.to_string()}, '
+                                      f'file_offset={absolute_offset} B, p1_time={p1_time}',
+                                      depth=3)
                     raw_list.append((p1_time_raw, int(header.message_type), absolute_offset))
                 except BaseException:
                     pass
-    _logger.trace(f'{num_syncs} sync with {len(raw_list)} valid FE.')
+    _logger.trace(f'Thread {thread_idx}: {num_syncs} sync with {len(raw_list)} valid FE.')
     # Return the index data for this section of the file.
     return np.array(raw_list, dtype=FileIndex._RAW_DTYPE)
 
 
 def fast_generate_index(
         input_path: str,
         force_reindex=False,
@@ -152,26 +164,27 @@
         except ValueError as e:
             _logger.warning(f'Couldn\'t load cache "{index_path}": {str(e)}.')
 
     _logger.info(f'Indexing file "{input_path}". This may take a few seconds.')
     _logger.debug(f'Using Threads: {num_threads}')
 
     # These are the args passed to the _search_blocks_for_fe instances.
-    args: list[Tuple[str, List[int]]] = []
+    args: list[Tuple[str, int, List[int]]] = []
     # Allocate which blocks of bytes will be processed by each thread.
     num_blocks = math.ceil(file_size / _READ_SIZE_BYTES)
     # Each thread will process at least blocks_per_thread blocks. If the number
     # doesn't divide evenly, distribute the remainder.
     blocks_per_thread, blocks_remainder = divmod(num_blocks, num_threads)
     byte_offset = 0
     for i in range(num_threads):
         blocks = blocks_per_thread
         if i < blocks_remainder:
             blocks += 1
-        args.append((input_path, list(range(byte_offset, byte_offset + blocks * _READ_SIZE_BYTES, _READ_SIZE_BYTES))))
+        args.append((input_path, i,
+                     list(range(byte_offset, byte_offset + blocks * _READ_SIZE_BYTES, _READ_SIZE_BYTES))))
         byte_offset += blocks * _READ_SIZE_BYTES
 
     _logger.debug(f'Reads/thread: {blocks_per_thread}')
 
     # Create a threadpool.
     with Pool(num_threads) as p:
         # Kick off the threads to process with their args. Then concatenate their returned data.
```

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/parsers/file_index.py` & `fusion_engine_client-1.23.0/fusion_engine_client/parsers/file_index.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/parsers/mixed_log_reader.py` & `fusion_engine_client-1.23.0/fusion_engine_client/parsers/mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/utils/argument_parser.py` & `fusion_engine_client-1.23.0/fusion_engine_client/utils/argument_parser.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/utils/bin_utils.py` & `fusion_engine_client-1.23.0/fusion_engine_client/utils/bin_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/utils/construct_utils.py` & `fusion_engine_client-1.23.0/fusion_engine_client/utils/construct_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from functools import reduce
 import math
 import re
 from typing import Optional
 
-from construct import Adapter, Enum, Struct
+from construct import Adapter, Array, Enum, Float64l, Float32l, FormatField, Struct
+import numpy as np
 
 from .enum_utils import IntEnum
 
 
 class FixedPointAdapter(Adapter):
     def __init__(self, scale, *args, invalid=None):
         super().__init__(*args)
@@ -28,14 +30,59 @@
     def _encode(self, obj, context, path):
         if math.isnan(obj) and self.invalid is not None:
             return self.invalid
         else:
             return int(round(obj / self.scale))
 
 
+class NumpyAdapter(Adapter):
+    def __init__(self, shape, dtype=None, construct_type=Float64l):
+        if dtype is None:
+            if construct_type is Float64l or construct_type is Float32l:
+                dtype = float
+            elif isinstance(construct_type, FormatField) and construct_type.fmtstr[1].lower() in 'bhlq':
+                dtype = int
+            else:
+                raise ValueError(f"Unable to infer numpy dtype from construct type {repr(construct_type)}.")
+
+        if construct_type is None:
+            if dtype is float or dtype is np.float:
+                # Assuming all floats are transmitted as 64-bit little endian by default.
+                construct_type = Float64l
+            else:
+                raise ValueError(f"Unable to infer serialized data type from numpy dtype {repr(dtype)}.")
+
+        if isinstance(shape, int):
+            shape = (shape,)
+
+        num_elements = reduce(lambda x, y: x * y, shape)
+        super().__init__(subcon=Array(num_elements, construct_type))
+
+        self.shape = shape
+        self.dtype = dtype
+
+    def _decode(self, obj, context, path):
+        return np.array(obj, dtype=self.dtype).reshape(self.shape)
+
+    def _encode(self, obj, context, path):
+        # Multi-dimensional arrays will be flattened an row-major order:
+        #   [[1, 2, 3],
+        #    [4, 5, 6]]
+        # becomes
+        #   [1, 2, 3, 4, 5, 6]
+        if isinstance(obj, np.ndarray):
+            return obj.astype(self.dtype).flatten().tolist()
+        else:
+            # Handle the case where the user passes in a list or tuple instead of a numpy array.
+            if len(self.shape) == 1:
+                return obj
+            else:
+                return np.array(obj, shape=self.shape, dtype=self.dtype).flatten().tolist()
+
+
 class NamedTupleAdapter(Adapter):
     """!
     @brief Adapter for automatically converting between construct streams and
            NamedTuples with corresponding fields.
 
     Usage Example:
     ```{.py}
```

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/utils/log.py` & `fusion_engine_client-1.23.0/fusion_engine_client/utils/log.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/utils/numpy_utils.py` & `fusion_engine_client-1.23.0/fusion_engine_client/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/utils/time_range.py` & `fusion_engine_client-1.23.0/fusion_engine_client/utils/time_range.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client/utils/trace.py` & `fusion_engine_client-1.23.0/fusion_engine_client/utils/trace.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client.egg-info/PKG-INFO` & `fusion_engine_client-1.23.0/fusion_engine_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.22.8
+Version: 1.23.0
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
-Download-URL: https://github.com/PointOneNav/fusion-engine-client/archive/refs/tags/v1.22.8.tar.gz
+Download-URL: https://github.com/PointOneNav/fusion-engine-client/archive/refs/tags/v1.23.0.tar.gz
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
@@ -23,24 +23,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: scipy>=1.5.0
-Requires-Dist: palettable>=3.3.0
 Requires-Dist: numpy>=1.16.0
+Requires-Dist: pymap3d>=2.4.3
 Requires-Dist: aenum>=3.1.1
 Requires-Dist: p1-gpstime>=0.6.3.dev1
-Requires-Dist: pymap3d>=2.4.3
-Requires-Dist: plotly>=4.0.0
-Requires-Dist: colorama>=0.4.4
 Requires-Dist: packaging>=21.0.0
+Requires-Dist: palettable>=3.3.0
+Requires-Dist: colorama>=0.4.4
+Requires-Dist: scipy>=1.5.0
 Requires-Dist: construct>=2.10.0
+Requires-Dist: plotly>=4.0.0
 Requires-Dist: argparse-formatter>=1.4
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: display
 Provides-Extra: tools
 
 Point One FusionEngine protocol support for real-time interaction and control, plus post-processing data analysis tools.
```

### Comparing `fusion-engine-client-1.22.8/fusion_engine_client.egg-info/SOURCES.txt` & `fusion_engine_client-1.23.0/fusion_engine_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/setup.py` & `fusion_engine_client-1.23.0/setup.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/tests/test_config.py` & `fusion_engine_client-1.23.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/tests/test_data_loader.py` & `fusion_engine_client-1.23.0/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/tests/test_decoder.py` & `fusion_engine_client-1.23.0/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/tests/test_encoder.py` & `fusion_engine_client-1.23.0/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/tests/test_file_index.py` & `fusion_engine_client-1.23.0/tests/test_file_index.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/tests/test_mixed_log_reader.py` & `fusion_engine_client-1.23.0/tests/test_mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.22.8/tests/test_time_range.py` & `fusion_engine_client-1.23.0/tests/test_time_range.py`

 * *Files identical despite different names*


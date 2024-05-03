# Comparing `tmp/darshan-3.4.4.0.tar.gz` & `tmp/darshan-3.4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "darshan-3.4.4.0.tar", last modified: Tue Aug  8 00:12:28 2023, max compression
+gzip compressed data, was "darshan-3.4.5.0.tar", last modified: Fri May  3 16:28:05 2024, max compression
```

## Comparing `darshan-3.4.4.0.tar` & `darshan-3.4.5.0.tar`

### file list

```diff
@@ -1,156 +1,154 @@
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.302298 darshan-3.4.4.0/
--rw-rw-r--   0 shane     (1000) shane     (1000)      213 2022-10-26 18:33:05.000000 darshan-3.4.4.0/MANIFEST.in
--rw-rw-r--   0 shane     (1000) shane     (1000)     2830 2023-08-08 00:12:28.302298 darshan-3.4.4.0/PKG-INFO
--rw-rw-r--   0 shane     (1000) shane     (1000)     2115 2023-08-01 19:58:29.000000 darshan-3.4.4.0/README.rst
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.174293 darshan-3.4.4.0/darshan/
--rw-rw-r--   0 shane     (1000) shane     (1000)     1221 2023-08-07 22:14:06.000000 darshan-3.4.4.0/darshan/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)       64 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/__main__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.178293 darshan-3.4.4.0/darshan/backend/
--rw-rw-r--   0 shane     (1000) shane     (1000)      227 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/backend/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     6193 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/backend/api_def_c.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     3694 2022-05-04 14:43:41.000000 darshan-3.4.4.0/darshan/backend/apmpi.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1928 2022-05-04 14:43:41.000000 darshan-3.4.4.0/darshan/backend/apss.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2305 2022-05-04 14:43:41.000000 darshan-3.4.4.0/darshan/backend/apxc.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    22874 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/backend/cffi_backend.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.182293 darshan-3.4.4.0/darshan/cli/
--rw-rw-r--   0 shane     (1000) shane     (1000)     5545 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/cli/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)       73 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/cli/__main__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2313 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/cli/base.html
--rw-rw-r--   0 shane     (1000) shane     (1000)      966 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/cli/info.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1028 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/cli/name_records.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     7563 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/cli/style.css
--rw-rw-r--   0 shane     (1000) shane     (1000)    29267 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/cli/summary.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      920 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/cli/to_json.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.182293 darshan-3.4.4.0/darshan/datatypes/
--rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/datatypes/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     3814 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/datatypes/heatmap.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     7635 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/discover_darshan.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.182293 darshan-3.4.4.0/darshan/examples/
--rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/__init__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.182293 darshan-3.4.4.0/darshan/examples/darshan-graph/
--rw-rw-r--   0 shane     (1000) shane     (1000)      279 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/darshan-graph/Makefile
--rw-rw-r--   0 shane     (1000) shane     (1000)     1676 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/darshan-graph/app.c
--rw-rw-r--   0 shane     (1000) shane     (1000)     3882 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/darshan-graph/app_rw_mpiio.c
--rw-rw-r--   0 shane     (1000) shane     (1000)     2498 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_readAB_writeC_id71326_7-31-5658-2037904274838284930_55623.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1070 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_read_id71317_7-31-5657-2037904274838284930_55623.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1079 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_read_id71344_7-31-5658-2037904274838284930_55623.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1068 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_write_id71296_7-31-5657-2037904274838284930_55623.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1069 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_write_id71303_7-31-5657-2037904274838284930_55623.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1072 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_write_id71310_7-31-5657-2037904274838284930_55623.darshan
--rwxrwxr-x   0 shane     (1000) shane     (1000)      717 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/darshan-graph/run.sh
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.214294 darshan-3.4.4.0/darshan/examples/example_logs/
--rw-rw-r--   0 shane     (1000) shane     (1000)      286 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/example_logs/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    98998 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/example_logs/dxt.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)    11472 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/example_logs/example.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     3967 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/example_logs/ior_hdf5_example.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)    16073 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/example_logs/noposix.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)   459650 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/example_logs/sample-badost.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1992 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/example_logs/shane_macsio_id29959_5-22-32552-7035573431850780836_1590156158.darshan
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.218294 darshan-3.4.4.0/darshan/examples/tutorial/
--rw-rw-r--   0 shane     (1000) shane     (1000)      103 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/tutorial/hello.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      216 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/tutorial/plot.py
--rwxrwxr-x   0 shane     (1000) shane     (1000)      596 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/tutorial/tojson.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.218294 darshan-3.4.4.0/darshan/experimental/
--rw-rw-r--   0 shane     (1000) shane     (1000)      134 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/__init__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.222295 darshan-3.4.4.0/darshan/experimental/aggregators/
--rw-rw-r--   0 shane     (1000) shane     (1000)      407 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/aggregators/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     4560 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/aggregators/agg_ioops.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2950 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/aggregators/create_dxttimeline.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1749 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/aggregators/create_sankey.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1335 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/aggregators/create_time_summary.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     5726 2022-11-02 17:48:53.000000 darshan-3.4.4.0/darshan/experimental/aggregators/create_timeline.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1476 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/aggregators/mod_agg_iohist.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      637 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/aggregators/name_records_summary.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     6951 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/aggregators/print_module_records.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1211 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/aggregators/records_as_dict.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      516 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/aggregators/summarize.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.226295 darshan-3.4.4.0/darshan/experimental/operations/
--rw-rw-r--   0 shane     (1000) shane     (1000)     2303 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/operations/filter.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2405 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/operations/merge.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     3187 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/operations/reduce.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.238295 darshan-3.4.4.0/darshan/experimental/plots/
--rw-rw-r--   0 shane     (1000) shane     (1000)      251 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/plots/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    26333 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/plots/data_access_by_filesystem.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    14559 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/plots/heatmap_handling.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2765 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/plots/plot_access_histogram.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     4340 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/experimental/plots/plot_common_access_table.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    14759 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/plots/plot_dxt_heatmap.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     4145 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/experimental/plots/plot_dxt_heatmap2.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     6297 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/plots/plot_io_cost.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     6638 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/plots/plot_opcounts.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1982 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/plots/plot_posix_access_pattern.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     5204 2022-12-19 21:37:30.000000 darshan-3.4.4.0/darshan/experimental/plots/plot_posix_io_pattern.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.238295 darshan-3.4.4.0/darshan/experimental/transforms/
--rw-rw-r--   0 shane     (1000) shane     (1000)     5626 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/transforms/dxt2png.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.242295 darshan-3.4.4.0/darshan/lib/
--rw-rw-r--   0 shane     (1000) shane     (1000)     3741 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/lib/accum.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2901 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/log_utils.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    35880 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/report.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.254296 darshan-3.4.4.0/darshan/tests/
--rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      533 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/conftest.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.294297 darshan-3.4.4.0/darshan/tests/input/
--rw-rw-r--   0 shane     (1000) shane     (1000)      313 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/input/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/input/match_dotout.dot
--rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/input/match_jsonout.json
--rw-rw-r--   0 shane     (1000) shane     (1000)    16073 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/input/noposix.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1441 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/input/noposixopens.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)   459650 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/input/sample-badost.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     6631 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/input/sample-dxt-simple.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)    10717 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/input/sample-goodost.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)    11472 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/input/sample.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)    11523 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/tests/test_cffi_misc.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    32921 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/tests/test_data_access_by_filesystem.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      567 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/test_error.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    22010 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/tests/test_heatmap_handling.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     8314 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/tests/test_lib_accum.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2064 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/test_log_utils.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1653 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/test_moddxt.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1116 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/test_modmpiio.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1107 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/test_modposix.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1144 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/test_modstdio.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     8550 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/tests/test_plot_common_access_table.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    16837 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/tests/test_plot_dxt_heatmap.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    13048 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/tests/test_plot_exp_common.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    10752 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/tests/test_plot_io_cost.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    24120 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/tests/test_report.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      563 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/test_report_copy.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    25957 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/tests/test_summary.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.174293 darshan-3.4.4.0/darshan.egg-info/
--rw-rw-r--   0 shane     (1000) shane     (1000)     2830 2023-08-08 00:12:28.000000 darshan-3.4.4.0/darshan.egg-info/PKG-INFO
--rw-rw-r--   0 shane     (1000) shane     (1000)     5035 2023-08-08 00:12:28.000000 darshan-3.4.4.0/darshan.egg-info/SOURCES.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)        1 2023-08-08 00:12:28.000000 darshan-3.4.4.0/darshan.egg-info/dependency_links.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)        1 2023-08-08 00:12:28.000000 darshan-3.4.4.0/darshan.egg-info/not-zip-safe
--rw-rw-r--   0 shane     (1000) shane     (1000)       51 2023-08-08 00:12:28.000000 darshan-3.4.4.0/darshan.egg-info/requires.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)        8 2023-08-08 00:12:28.000000 darshan-3.4.4.0/darshan.egg-info/top_level.txt
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.298298 darshan-3.4.4.0/docs/
--rw-rw-r--   0 shane     (1000) shane     (1000)      610 2022-10-26 18:33:05.000000 darshan-3.4.4.0/docs/Makefile
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.170292 darshan-3.4.4.0/docs/api/
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.302298 darshan-3.4.4.0/docs/api/pydarshan/
--rw-rw-r--   0 shane     (1000) shane     (1000)      951 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.backend.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      740 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.cli.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      328 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.datatypes.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      179 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.examples.example_logs.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      227 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.examples.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)     2573 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.experimental.aggregators.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)     2015 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.experimental.plots.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      272 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.experimental.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      742 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      147 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.tests.input.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)     3341 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.tests.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)       62 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/modules.rst
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.170292 darshan-3.4.4.0/docs/build/
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.170292 darshan-3.4.4.0/docs/build/html/
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.302298 darshan-3.4.4.0/docs/build/html/_static/
--rw-rw-r--   0 shane     (1000) shane     (1000)      286 2023-08-05 14:28:56.000000 darshan-3.4.4.0/docs/build/html/_static/file.png
--rw-rw-r--   0 shane     (1000) shane     (1000)       90 2023-08-05 14:28:56.000000 darshan-3.4.4.0/docs/build/html/_static/minus.png
--rw-rw-r--   0 shane     (1000) shane     (1000)       90 2023-08-05 14:28:56.000000 darshan-3.4.4.0/docs/build/html/_static/plus.png
--rwxrwxr-x   0 shane     (1000) shane     (1000)     5230 2022-10-26 18:33:05.000000 darshan-3.4.4.0/docs/conf.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      669 2023-08-01 19:58:29.000000 darshan-3.4.4.0/docs/index.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)     2097 2023-08-01 19:58:29.000000 darshan-3.4.4.0/docs/install.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      771 2022-10-26 18:33:05.000000 darshan-3.4.4.0/docs/make.bat
--rw-rw-r--   0 shane     (1000) shane     (1000)       27 2022-12-01 18:54:58.000000 darshan-3.4.4.0/docs/readme.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)     3682 2023-08-01 19:58:29.000000 darshan-3.4.4.0/docs/usage.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)     1353 2023-08-01 19:58:29.000000 darshan-3.4.4.0/pyproject.toml
--rw-rw-r--   0 shane     (1000) shane     (1000)      480 2023-08-08 00:12:28.302298 darshan-3.4.4.0/setup.cfg
--rw-rw-r--   0 shane     (1000) shane     (1000)     2850 2023-08-07 22:14:06.000000 darshan-3.4.4.0/setup.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.280857 darshan-3.4.5.0/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      213 2024-05-03 14:54:04.000000 darshan-3.4.5.0/MANIFEST.in
+-rw-r--r--   0 shane     (1000) shane     (1000)     3433 2024-05-03 16:28:05.280857 darshan-3.4.5.0/PKG-INFO
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2115 2024-05-03 14:54:04.000000 darshan-3.4.5.0/README.rst
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.232855 darshan-3.4.5.0/darshan/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1221 2024-05-03 16:24:16.000000 darshan-3.4.5.0/darshan/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)       64 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/__main__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.236855 darshan-3.4.5.0/darshan/backend/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      227 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/backend/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     6193 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/backend/api_def_c.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3694 2022-05-04 14:43:41.000000 darshan-3.4.5.0/darshan/backend/apmpi.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1928 2022-05-04 14:43:41.000000 darshan-3.4.5.0/darshan/backend/apss.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2305 2022-05-04 14:43:41.000000 darshan-3.4.5.0/darshan/backend/apxc.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    22874 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/backend/cffi_backend.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.240855 darshan-3.4.5.0/darshan/cli/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     5545 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/cli/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)       73 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/cli/__main__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2313 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/cli/base.html
+-rw-rw-r--   0 shane     (1000) shane     (1000)      966 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/cli/info.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1028 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/cli/name_records.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     7563 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/cli/style.css
+-rw-rw-r--   0 shane     (1000) shane     (1000)    29267 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/cli/summary.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      920 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/cli/to_json.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.240855 darshan-3.4.5.0/darshan/datatypes/
+-rw-rw-r--   0 shane     (1000) shane     (1000)        0 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/datatypes/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3814 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/datatypes/heatmap.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     7635 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/discover_darshan.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.240855 darshan-3.4.5.0/darshan/examples/
+-rw-rw-r--   0 shane     (1000) shane     (1000)        0 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/__init__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.244855 darshan-3.4.5.0/darshan/examples/darshan-graph/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      279 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/darshan-graph/Makefile
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1676 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/darshan-graph/app.c
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3882 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/darshan-graph/app_rw_mpiio.c
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2498 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/darshan-graph/pq_app_readAB_writeC_id71326_7-31-5658-2037904274838284930_55623.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1070 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/darshan-graph/pq_app_read_id71317_7-31-5657-2037904274838284930_55623.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1079 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/darshan-graph/pq_app_read_id71344_7-31-5658-2037904274838284930_55623.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1068 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/darshan-graph/pq_app_write_id71296_7-31-5657-2037904274838284930_55623.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1069 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/darshan-graph/pq_app_write_id71303_7-31-5657-2037904274838284930_55623.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1072 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/darshan-graph/pq_app_write_id71310_7-31-5657-2037904274838284930_55623.darshan
+-rwxrwxr-x   0 shane     (1000) shane     (1000)      717 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/darshan-graph/run.sh
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.248856 darshan-3.4.5.0/darshan/examples/example_logs/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      286 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/example_logs/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    98998 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/example_logs/dxt.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)    11472 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/example_logs/example.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3967 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/example_logs/ior_hdf5_example.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)    16073 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/example_logs/noposix.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)   459650 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/example_logs/sample-badost.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1992 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/example_logs/shane_macsio_id29959_5-22-32552-7035573431850780836_1590156158.darshan
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.252856 darshan-3.4.5.0/darshan/examples/tutorial/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      103 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/tutorial/hello.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      216 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/tutorial/plot.py
+-rwxrwxr-x   0 shane     (1000) shane     (1000)      596 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/examples/tutorial/tojson.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.252856 darshan-3.4.5.0/darshan/experimental/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      134 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/__init__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.252856 darshan-3.4.5.0/darshan/experimental/aggregators/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      407 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/aggregators/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     4560 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/aggregators/agg_ioops.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2950 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/aggregators/create_dxttimeline.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1749 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/aggregators/create_sankey.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1335 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/aggregators/create_time_summary.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     5726 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/aggregators/create_timeline.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1476 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/aggregators/mod_agg_iohist.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      637 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/aggregators/name_records_summary.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     6951 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/aggregators/print_module_records.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1211 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/aggregators/records_as_dict.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      516 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/aggregators/summarize.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.256856 darshan-3.4.5.0/darshan/experimental/operations/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2303 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/operations/filter.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2405 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/operations/merge.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3187 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/operations/reduce.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.260856 darshan-3.4.5.0/darshan/experimental/plots/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      251 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/plots/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    26353 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/plots/data_access_by_filesystem.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    14559 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/plots/heatmap_handling.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2765 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/plots/plot_access_histogram.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     4340 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/plots/plot_common_access_table.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    14759 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/plots/plot_dxt_heatmap.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     4145 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/plots/plot_dxt_heatmap2.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     6296 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/plots/plot_io_cost.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     6638 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/plots/plot_opcounts.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1982 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/plots/plot_posix_access_pattern.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.260856 darshan-3.4.5.0/darshan/experimental/transforms/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     5626 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/experimental/transforms/dxt2png.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.260856 darshan-3.4.5.0/darshan/lib/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3741 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/lib/accum.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2901 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/log_utils.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    35880 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/report.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.268856 darshan-3.4.5.0/darshan/tests/
+-rw-rw-r--   0 shane     (1000) shane     (1000)        0 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      533 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/conftest.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.272857 darshan-3.4.5.0/darshan/tests/input/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      313 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/input/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)        0 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/input/match_dotout.dot
+-rw-rw-r--   0 shane     (1000) shane     (1000)        0 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/input/match_jsonout.json
+-rw-rw-r--   0 shane     (1000) shane     (1000)    16073 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/input/noposix.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1441 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/input/noposixopens.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)   459650 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/input/sample-badost.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     6631 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/input/sample-dxt-simple.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)    10717 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/input/sample-goodost.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)    11472 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/input/sample.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)    11523 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/test_cffi_misc.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    32921 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/test_data_access_by_filesystem.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      567 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/test_error.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    22010 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/test_heatmap_handling.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     8314 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/test_lib_accum.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2064 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/test_log_utils.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1653 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/test_moddxt.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1116 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/test_modmpiio.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1107 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/test_modposix.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1144 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/test_modstdio.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     8550 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/test_plot_common_access_table.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    16837 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/test_plot_dxt_heatmap.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    13048 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/test_plot_exp_common.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    10752 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/test_plot_io_cost.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    24120 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/test_report.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      563 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/test_report_copy.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    26119 2024-05-03 14:54:04.000000 darshan-3.4.5.0/darshan/tests/test_summary.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.280857 darshan-3.4.5.0/darshan.egg-info/
+-rw-r--r--   0 shane     (1000) shane     (1000)     3433 2024-05-03 16:28:05.000000 darshan-3.4.5.0/darshan.egg-info/PKG-INFO
+-rw-rw-r--   0 shane     (1000) shane     (1000)     4943 2024-05-03 16:28:05.000000 darshan-3.4.5.0/darshan.egg-info/SOURCES.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)        1 2024-05-03 16:28:05.000000 darshan-3.4.5.0/darshan.egg-info/dependency_links.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)      152 2024-05-03 16:28:05.000000 darshan-3.4.5.0/darshan.egg-info/requires.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)        8 2024-05-03 16:28:05.000000 darshan-3.4.5.0/darshan.egg-info/top_level.txt
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.276857 darshan-3.4.5.0/docs/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      610 2024-05-03 14:54:04.000000 darshan-3.4.5.0/docs/Makefile
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.228855 darshan-3.4.5.0/docs/api/
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.276857 darshan-3.4.5.0/docs/api/pydarshan/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      501 2024-05-03 16:22:46.000000 darshan-3.4.5.0/docs/api/pydarshan/darshan.backend.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      740 2024-05-03 16:22:46.000000 darshan-3.4.5.0/docs/api/pydarshan/darshan.cli.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      328 2024-05-03 16:22:46.000000 darshan-3.4.5.0/docs/api/pydarshan/darshan.datatypes.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      179 2024-05-03 16:22:46.000000 darshan-3.4.5.0/docs/api/pydarshan/darshan.examples.example_logs.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      227 2024-05-03 16:22:46.000000 darshan-3.4.5.0/docs/api/pydarshan/darshan.examples.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2573 2024-05-03 16:22:46.000000 darshan-3.4.5.0/docs/api/pydarshan/darshan.experimental.aggregators.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2266 2024-05-03 16:22:46.000000 darshan-3.4.5.0/docs/api/pydarshan/darshan.experimental.plots.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      272 2024-05-03 16:22:46.000000 darshan-3.4.5.0/docs/api/pydarshan/darshan.experimental.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      742 2024-05-03 16:22:46.000000 darshan-3.4.5.0/docs/api/pydarshan/darshan.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      147 2024-05-03 16:22:46.000000 darshan-3.4.5.0/docs/api/pydarshan/darshan.tests.input.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3518 2024-05-03 16:22:46.000000 darshan-3.4.5.0/docs/api/pydarshan/darshan.tests.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)       62 2024-05-03 16:22:46.000000 darshan-3.4.5.0/docs/api/pydarshan/modules.rst
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.228855 darshan-3.4.5.0/docs/build/
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.228855 darshan-3.4.5.0/docs/build/html/
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-05-03 16:28:05.276857 darshan-3.4.5.0/docs/build/html/_static/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      286 2024-05-03 16:22:35.000000 darshan-3.4.5.0/docs/build/html/_static/file.png
+-rw-rw-r--   0 shane     (1000) shane     (1000)       90 2024-05-03 16:22:35.000000 darshan-3.4.5.0/docs/build/html/_static/minus.png
+-rw-rw-r--   0 shane     (1000) shane     (1000)       90 2024-05-03 16:22:35.000000 darshan-3.4.5.0/docs/build/html/_static/plus.png
+-rwxrwxr-x   0 shane     (1000) shane     (1000)     5230 2024-05-03 14:54:04.000000 darshan-3.4.5.0/docs/conf.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      669 2024-05-03 14:54:04.000000 darshan-3.4.5.0/docs/index.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2097 2024-05-03 14:54:04.000000 darshan-3.4.5.0/docs/install.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      771 2024-05-03 14:54:04.000000 darshan-3.4.5.0/docs/make.bat
+-rw-rw-r--   0 shane     (1000) shane     (1000)       27 2024-05-03 14:54:04.000000 darshan-3.4.5.0/docs/readme.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3682 2024-05-03 14:54:04.000000 darshan-3.4.5.0/docs/usage.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3315 2024-05-03 14:53:20.000000 darshan-3.4.5.0/pyproject.toml
+-rw-rw-r--   0 shane     (1000) shane     (1000)       38 2024-05-03 16:28:05.280857 darshan-3.4.5.0/setup.cfg
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1312 2024-05-03 14:54:04.000000 darshan-3.4.5.0/setup.py
```

### Comparing `darshan-3.4.4.0/PKG-INFO` & `darshan-3.4.5.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: darshan
-Version: 3.4.4.0
-Summary: Python tools to interact with darshan log records of HPC applications.
-Home-page: https://www.mcs.anl.gov/research/projects/darshan/
-Author: 
-Author-email: 
-Keywords: darshan
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-
 =======================
 PyDarshan Documentation
 =======================
 
 Python utilities to interact with `Darshan <https://www.mcs.anl.gov/research/projects/darshan/>`__
 log records of HPC applications.
```

### Comparing `darshan-3.4.4.0/darshan/__init__.py` & `darshan-3.4.5.0/darshan/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 PyDarshan provides direct log access for reading binary Darshan logs.
 PyDarshan also provides a suite of analysis utilities.
 """
 
-__version__ = '3.4.4.0'
-__darshanutil_version__ = '3.4.4'
+__version__ = '3.4.5.0'
+__darshanutil_version__ = '3.4.5'
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 options = {} # type: ignore
```

### Comparing `darshan-3.4.4.0/darshan/backend/api_def_c.py` & `darshan-3.4.5.0/darshan/backend/api_def_c.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/backend/apmpi.py` & `darshan-3.4.5.0/darshan/backend/apmpi.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/backend/apss.py` & `darshan-3.4.5.0/darshan/backend/apss.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/backend/apxc.py` & `darshan-3.4.5.0/darshan/backend/apxc.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/backend/cffi_backend.py` & `darshan-3.4.5.0/darshan/backend/cffi_backend.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/cli/__init__.py` & `darshan-3.4.5.0/darshan/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/cli/base.html` & `darshan-3.4.5.0/darshan/cli/base.html`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/cli/info.py` & `darshan-3.4.5.0/darshan/cli/info.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/cli/name_records.py` & `darshan-3.4.5.0/darshan/cli/name_records.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/cli/style.css` & `darshan-3.4.5.0/darshan/cli/style.css`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/cli/summary.py` & `darshan-3.4.5.0/darshan/cli/summary.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/cli/to_json.py` & `darshan-3.4.5.0/darshan/cli/to_json.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/datatypes/heatmap.py` & `darshan-3.4.5.0/darshan/datatypes/heatmap.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/discover_darshan.py` & `darshan-3.4.5.0/darshan/discover_darshan.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/examples/darshan-graph/app.c` & `darshan-3.4.5.0/darshan/examples/darshan-graph/app.c`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/examples/darshan-graph/app_rw_mpiio.c` & `darshan-3.4.5.0/darshan/examples/darshan-graph/app_rw_mpiio.c`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_readAB_writeC_id71326_7-31-5658-2037904274838284930_55623.darshan` & `darshan-3.4.5.0/darshan/examples/darshan-graph/pq_app_readAB_writeC_id71326_7-31-5658-2037904274838284930_55623.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_read_id71317_7-31-5657-2037904274838284930_55623.darshan` & `darshan-3.4.5.0/darshan/examples/darshan-graph/pq_app_read_id71317_7-31-5657-2037904274838284930_55623.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_read_id71344_7-31-5658-2037904274838284930_55623.darshan` & `darshan-3.4.5.0/darshan/examples/darshan-graph/pq_app_read_id71344_7-31-5658-2037904274838284930_55623.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_write_id71296_7-31-5657-2037904274838284930_55623.darshan` & `darshan-3.4.5.0/darshan/examples/darshan-graph/pq_app_write_id71296_7-31-5657-2037904274838284930_55623.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_write_id71303_7-31-5657-2037904274838284930_55623.darshan` & `darshan-3.4.5.0/darshan/examples/darshan-graph/pq_app_write_id71303_7-31-5657-2037904274838284930_55623.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_write_id71310_7-31-5657-2037904274838284930_55623.darshan` & `darshan-3.4.5.0/darshan/examples/darshan-graph/pq_app_write_id71310_7-31-5657-2037904274838284930_55623.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/examples/darshan-graph/run.sh` & `darshan-3.4.5.0/darshan/examples/darshan-graph/run.sh`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/examples/example_logs/dxt.darshan` & `darshan-3.4.5.0/darshan/examples/example_logs/dxt.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/examples/example_logs/example.darshan` & `darshan-3.4.5.0/darshan/examples/example_logs/example.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/examples/example_logs/ior_hdf5_example.darshan` & `darshan-3.4.5.0/darshan/examples/example_logs/ior_hdf5_example.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/examples/example_logs/noposix.darshan` & `darshan-3.4.5.0/darshan/examples/example_logs/noposix.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/examples/example_logs/sample-badost.darshan` & `darshan-3.4.5.0/darshan/examples/example_logs/sample-badost.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/examples/example_logs/shane_macsio_id29959_5-22-32552-7035573431850780836_1590156158.darshan` & `darshan-3.4.5.0/darshan/examples/example_logs/shane_macsio_id29959_5-22-32552-7035573431850780836_1590156158.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/examples/tutorial/tojson.py` & `darshan-3.4.5.0/darshan/examples/tutorial/tojson.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/aggregators/agg_ioops.py` & `darshan-3.4.5.0/darshan/experimental/aggregators/agg_ioops.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/aggregators/create_dxttimeline.py` & `darshan-3.4.5.0/darshan/experimental/aggregators/create_dxttimeline.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/aggregators/create_sankey.py` & `darshan-3.4.5.0/darshan/experimental/aggregators/create_sankey.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/aggregators/create_time_summary.py` & `darshan-3.4.5.0/darshan/experimental/aggregators/create_time_summary.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/aggregators/create_timeline.py` & `darshan-3.4.5.0/darshan/experimental/aggregators/create_timeline.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/aggregators/mod_agg_iohist.py` & `darshan-3.4.5.0/darshan/experimental/aggregators/mod_agg_iohist.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/aggregators/name_records_summary.py` & `darshan-3.4.5.0/darshan/experimental/aggregators/name_records_summary.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/aggregators/print_module_records.py` & `darshan-3.4.5.0/darshan/experimental/aggregators/print_module_records.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/aggregators/records_as_dict.py` & `darshan-3.4.5.0/darshan/experimental/aggregators/records_as_dict.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/aggregators/summarize.py` & `darshan-3.4.5.0/darshan/experimental/aggregators/summarize.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/operations/filter.py` & `darshan-3.4.5.0/darshan/experimental/operations/filter.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/operations/merge.py` & `darshan-3.4.5.0/darshan/experimental/operations/merge.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/operations/reduce.py` & `darshan-3.4.5.0/darshan/experimental/operations/reduce.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/plots/data_access_by_filesystem.py` & `darshan-3.4.5.0/darshan/experimental/plots/data_access_by_filesystem.py`

 * *Files 0% similar despite different names*

```diff
@@ -673,18 +673,18 @@
     sort_inds = (bytes_rd_series + bytes_wr_series).argsort()[::-1]
     if num_cats is None:
         height = len(file_rd_series)
     else:
         height = num_cats
 
     plot_data(fig,
-              file_rd_series[sort_inds],
-              file_wr_series[sort_inds],
-              bytes_rd_series[sort_inds],
-              bytes_wr_series[sort_inds],
+              file_rd_series.iloc[sort_inds],
+              file_wr_series.iloc[sort_inds],
+              bytes_rd_series.iloc[sort_inds],
+              bytes_wr_series.iloc[sort_inds],
               filesystem_roots,
               num_cats=num_cats)
 
     # at least this much height seems to
     # produce a decent aspect ratio
     if height < 16:
         height = 16
```

### Comparing `darshan-3.4.4.0/darshan/experimental/plots/heatmap_handling.py` & `darshan-3.4.5.0/darshan/experimental/plots/heatmap_handling.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/plots/plot_access_histogram.py` & `darshan-3.4.5.0/darshan/experimental/plots/plot_access_histogram.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/plots/plot_common_access_table.py` & `darshan-3.4.5.0/darshan/experimental/plots/plot_common_access_table.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/plots/plot_dxt_heatmap.py` & `darshan-3.4.5.0/darshan/experimental/plots/plot_dxt_heatmap.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/plots/plot_dxt_heatmap2.py` & `darshan-3.4.5.0/darshan/experimental/plots/plot_dxt_heatmap2.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/plots/plot_io_cost.py` & `darshan-3.4.5.0/darshan/experimental/plots/plot_io_cost.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
     # values on both sides of the bar graph
     n_ticks = len(ax_norm.get_yticks())
     yticks = np.linspace(0, runtime, n_ticks)
     ax_raw.set_yticks(yticks)
     # add the legend and appropriate labels
     ax_raw.set_ylabel("Runtime (s)")
     handles, labels = ax_raw.get_legend_handles_labels()
-    ax_norm.legend(handles[::-1], labels[::-1], loc="upper left", bbox_to_anchor=(1.22, 1.02))
+    ax_raw.legend(handles[::-1], labels[::-1], loc="upper left", bbox_to_anchor=(1.22, 1.02))
     ax_norm.set_ylabel("Runtime (%)")
     # rotate the xticklabels so they don't overlap
     for ax in [ax_raw, ax_norm]:
         for label in ax.get_xticklabels():
             label.set_rotation(90)
     # adjust the figure to reduce white space
     io_cost_fig.subplots_adjust(right=0.59)
```

### Comparing `darshan-3.4.4.0/darshan/experimental/plots/plot_opcounts.py` & `darshan-3.4.5.0/darshan/experimental/plots/plot_opcounts.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/plots/plot_posix_access_pattern.py` & `darshan-3.4.5.0/darshan/experimental/plots/plot_posix_access_pattern.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/experimental/transforms/dxt2png.py` & `darshan-3.4.5.0/darshan/experimental/transforms/dxt2png.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/lib/accum.py` & `darshan-3.4.5.0/darshan/lib/accum.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/log_utils.py` & `darshan-3.4.5.0/darshan/log_utils.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/report.py` & `darshan-3.4.5.0/darshan/report.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/conftest.py` & `darshan-3.4.5.0/darshan/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/input/noposix.darshan` & `darshan-3.4.5.0/darshan/tests/input/noposix.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/input/noposixopens.darshan` & `darshan-3.4.5.0/darshan/tests/input/noposixopens.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/input/sample-badost.darshan` & `darshan-3.4.5.0/darshan/tests/input/sample-badost.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/input/sample-dxt-simple.darshan` & `darshan-3.4.5.0/darshan/tests/input/sample-dxt-simple.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/input/sample-goodost.darshan` & `darshan-3.4.5.0/darshan/tests/input/sample-goodost.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/input/sample.darshan` & `darshan-3.4.5.0/darshan/tests/input/sample.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/test_cffi_misc.py` & `darshan-3.4.5.0/darshan/tests/test_cffi_misc.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/test_data_access_by_filesystem.py` & `darshan-3.4.5.0/darshan/tests/test_data_access_by_filesystem.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/test_error.py` & `darshan-3.4.5.0/darshan/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/test_heatmap_handling.py` & `darshan-3.4.5.0/darshan/tests/test_heatmap_handling.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/test_lib_accum.py` & `darshan-3.4.5.0/darshan/tests/test_lib_accum.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/test_log_utils.py` & `darshan-3.4.5.0/darshan/tests/test_log_utils.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/test_moddxt.py` & `darshan-3.4.5.0/darshan/tests/test_moddxt.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/test_modmpiio.py` & `darshan-3.4.5.0/darshan/tests/test_modmpiio.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/test_modposix.py` & `darshan-3.4.5.0/darshan/tests/test_modposix.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/test_modstdio.py` & `darshan-3.4.5.0/darshan/tests/test_modstdio.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/test_plot_common_access_table.py` & `darshan-3.4.5.0/darshan/tests/test_plot_common_access_table.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/test_plot_dxt_heatmap.py` & `darshan-3.4.5.0/darshan/tests/test_plot_dxt_heatmap.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/test_plot_exp_common.py` & `darshan-3.4.5.0/darshan/tests/test_plot_exp_common.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/test_plot_io_cost.py` & `darshan-3.4.5.0/darshan/tests/test_plot_io_cost.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/test_report.py` & `darshan-3.4.5.0/darshan/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/test_report_copy.py` & `darshan-3.4.5.0/darshan/tests/test_report_copy.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/darshan/tests/test_summary.py` & `darshan-3.4.5.0/darshan/tests/test_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import io
 import re
 import os
 import pytest
 import argparse
 from unittest import mock
 from datetime import datetime
 
@@ -385,15 +386,15 @@
         if not has_lxml:
             pytest.skip("Test requires lxml")
 
         log_path = get_log_path(log_path)
         # generate the report data
         R = summary.ReportData(log_path=log_path)
         # convert the metadata table back to a pandas dataframe
-        actual_metadata_df = pd.read_html(R.metadata_table, index_col=0)[0]
+        actual_metadata_df = pd.read_html(io.StringIO(R.metadata_table), index_col=0)[0]
         # correct index and columns attributes after
         # `index_col` removed the first column
         actual_metadata_df.index.names = [None]
         actual_metadata_df.columns = [0]
 
         # check the metadata dataframes
         assert_frame_equal(actual_metadata_df, expected_df)
@@ -499,15 +500,15 @@
 
         log_path = get_log_path(log_path)
         # collect the report data
         R = summary.ReportData(log_path=log_path)
         # check that number of unicode warning symbols matches expected partial flag count
         assert R.module_table.count("&#x26A0;") == expected_partial_flags
         # convert the module table back to a pandas dataframe
-        actual_mod_df = pd.read_html(R.module_table, index_col=0)[0]
+        actual_mod_df = pd.read_html(io.StringIO(R.module_table), index_col=0)[0]
         # correct index and columns attributes after
         # `index_col` removed the first column
         actual_mod_df.index.names = [None]
         actual_mod_df.columns = [0, 1]
 
         # verify the number of modules in the report is equal to
         # the number of rows in the module table, including the 3 rows
@@ -517,16 +518,18 @@
 
         expected_df.rename(index=lambda s: s + " Module Data" if "ver=" in s else s, inplace=True)
 
         # add new column for partial flags
         expected_df[1] = np.nan
         flag = "\u26A0 Module data incomplete due to runtime memory or record count limits"
         if "partial_data_stdio.darshan" in log_path:
+            expected_df[[1]] = expected_df[[1]].astype(object)
             expected_df.iloc[5, 1] = flag
         if "partial_data_dxt.darshan" in log_path:
+            expected_df[[1]] = expected_df[[1]].astype(object)
             expected_df.iloc[6:, 1] = flag
 
         # check the module dataframes
         assert_frame_equal(actual_mod_df, expected_df)
 
     @pytest.mark.parametrize(
         "logname, expected_cmd",
```

### Comparing `darshan-3.4.4.0/darshan.egg-info/PKG-INFO` & `darshan-3.4.5.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 Metadata-Version: 2.1
 Name: darshan
-Version: 3.4.4.0
-Summary: Python tools to interact with darshan log records of HPC applications.
-Home-page: https://www.mcs.anl.gov/research/projects/darshan/
-Author: 
-Author-email: 
-Keywords: darshan
+Version: 3.4.5.0
+Summary: Python tools to interact with Darshan log records of HPC applications.
+Project-URL: homepage, https://www.mcs.anl.gov/research/projects/darshan/
+Project-URL: repository, https://github.com/darshan-hpc/darshan
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Requires-Dist: cffi
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: mako
+Requires-Dist: humanize
+Provides-Extra: test
+Requires-Dist: packaging; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: lxml; extra == "test"
+Requires-Dist: matplotlib; extra == "test"
+Requires-Dist: importlib_resources; python_version < "3.9" and extra == "test"
+Requires-Dist: humanize; extra == "test"
 
 =======================
 PyDarshan Documentation
 =======================
 
 Python utilities to interact with `Darshan <https://www.mcs.anl.gov/research/projects/darshan/>`__
 log records of HPC applications.
```

### Comparing `darshan-3.4.4.0/darshan.egg-info/SOURCES.txt` & `darshan-3.4.5.0/darshan.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
 setup.py
 darshan/__init__.py
 darshan/__main__.py
 darshan/discover_darshan.py
 darshan/log_utils.py
 darshan/report.py
 darshan.egg-info/PKG-INFO
 darshan.egg-info/SOURCES.txt
 darshan.egg-info/dependency_links.txt
-darshan.egg-info/not-zip-safe
 darshan.egg-info/requires.txt
 darshan.egg-info/top_level.txt
 darshan/backend/__init__.py
 darshan/backend/api_def_c.py
 darshan/backend/apmpi.py
 darshan/backend/apss.py
 darshan/backend/apxc.py
@@ -72,15 +70,14 @@
 darshan/experimental/plots/plot_access_histogram.py
 darshan/experimental/plots/plot_common_access_table.py
 darshan/experimental/plots/plot_dxt_heatmap.py
 darshan/experimental/plots/plot_dxt_heatmap2.py
 darshan/experimental/plots/plot_io_cost.py
 darshan/experimental/plots/plot_opcounts.py
 darshan/experimental/plots/plot_posix_access_pattern.py
-darshan/experimental/plots/plot_posix_io_pattern.py
 darshan/experimental/transforms/dxt2png.py
 darshan/lib/accum.py
 darshan/tests/__init__.py
 darshan/tests/conftest.py
 darshan/tests/test_cffi_misc.py
 darshan/tests/test_data_access_by_filesystem.py
 darshan/tests/test_error.py
```

### Comparing `darshan-3.4.4.0/docs/Makefile` & `darshan-3.4.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/docs/api/pydarshan/darshan.backend.rst` & `darshan-3.4.5.0/docs/api/pydarshan/darshan.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,47 @@
-darshan.backend package
-=======================
+darshan package
+===============
 
-.. automodule:: darshan.backend
+.. automodule:: darshan
    :members:
    :undoc-members:
    :show-inheritance:
 
-Submodules
-----------
-
-darshan.backend.api\_def\_c module
-----------------------------------
+Subpackages
+-----------
 
-.. automodule:: darshan.backend.api_def_c
-   :members:
-   :undoc-members:
-   :show-inheritance:
+.. toctree::
+   :maxdepth: 4
 
-darshan.backend.apmpi module
-----------------------------
+   darshan.backend
+   darshan.cli
+   darshan.datatypes
+   darshan.examples
+   darshan.experimental
+   darshan.tests
 
-.. automodule:: darshan.backend.apmpi
-   :members:
-   :undoc-members:
-   :show-inheritance:
+Submodules
+----------
 
-darshan.backend.apss module
----------------------------
+darshan.discover\_darshan module
+--------------------------------
 
-.. automodule:: darshan.backend.apss
+.. automodule:: darshan.discover_darshan
    :members:
    :undoc-members:
    :show-inheritance:
 
-darshan.backend.apxc module
----------------------------
+darshan.log\_utils module
+-------------------------
 
-.. automodule:: darshan.backend.apxc
+.. automodule:: darshan.log_utils
    :members:
    :undoc-members:
    :show-inheritance:
 
-darshan.backend.cffi\_backend module
-------------------------------------
+darshan.report module
+---------------------
 
-.. automodule:: darshan.backend.cffi_backend
+.. automodule:: darshan.report
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `darshan-3.4.4.0/docs/api/pydarshan/darshan.cli.rst` & `darshan-3.4.5.0/docs/api/pydarshan/darshan.cli.rst`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/docs/api/pydarshan/darshan.experimental.aggregators.rst` & `darshan-3.4.5.0/docs/api/pydarshan/darshan.experimental.aggregators.rst`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/docs/api/pydarshan/darshan.experimental.plots.rst` & `darshan-3.4.5.0/docs/api/pydarshan/darshan.experimental.plots.rst`

 * *Files 7% similar despite different names*

```diff
@@ -68,7 +68,15 @@
 darshan.experimental.plots.plot\_opcounts module
 ------------------------------------------------
 
 .. automodule:: darshan.experimental.plots.plot_opcounts
    :members:
    :undoc-members:
    :show-inheritance:
+
+darshan.experimental.plots.plot\_posix\_access\_pattern module
+--------------------------------------------------------------
+
+.. automodule:: darshan.experimental.plots.plot_posix_access_pattern
+   :members:
+   :undoc-members:
+   :show-inheritance:
```

### Comparing `darshan-3.4.4.0/docs/api/pydarshan/darshan.tests.rst` & `darshan-3.4.5.0/docs/api/pydarshan/darshan.tests.rst`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,22 @@
 --------------------------------------------
 
 .. automodule:: darshan.tests.test_heatmap_handling
    :members:
    :undoc-members:
    :show-inheritance:
 
+darshan.tests.test\_lib\_accum module
+-------------------------------------
+
+.. automodule:: darshan.tests.test_lib_accum
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 darshan.tests.test\_log\_utils module
 -------------------------------------
 
 .. automodule:: darshan.tests.test_log_utils
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `darshan-3.4.4.0/docs/conf.py` & `darshan-3.4.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/docs/index.rst` & `darshan-3.4.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/docs/install.rst` & `darshan-3.4.5.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/docs/make.bat` & `darshan-3.4.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `darshan-3.4.4.0/docs/usage.rst` & `darshan-3.4.5.0/docs/usage.rst`

 * *Files identical despite different names*


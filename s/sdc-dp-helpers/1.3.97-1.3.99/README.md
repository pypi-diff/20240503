# Comparing `tmp/sdc_dp_helpers-1.3.97.tar.gz` & `tmp/sdc_dp_helpers-1.3.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdc_dp_helpers-1.3.97.tar", last modified: Wed Mar 13 07:07:58 2024, max compression
+gzip compressed data, was "sdc_dp_helpers-1.3.99.tar", last modified: Fri May  3 05:51:16 2024, max compression
```

## Comparing `sdc_dp_helpers-1.3.97.tar` & `sdc_dp_helpers-1.3.99.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.594902 sdc_dp_helpers-1.3.97/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-13 07:07:58.594902 sdc_dp_helpers-1.3.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.586902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.586902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/api_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/api_utilities/__init_.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/api_utilities/data_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20801 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/api_utilities/date_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/api_utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/api_utilities/file_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/api_utilities/retry_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/api_utilities/tracking_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.590902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/azure/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/azure/writers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/base_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/base_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12994 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/base_writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.590902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/facebook/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/facebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/facebook/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/facebook/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.590902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/falcon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/falcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/falcon/falcon_sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/falcon/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/falcon/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.590902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/ftp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/ftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/ftp/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/ftp/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.590902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_ads/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_ads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_ads/generate_refresh_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_ads/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_ads/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.590902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_analytics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_analytics/config_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17278 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_analytics/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_analytics/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_analytics/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.590902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_analytics_v4/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_analytics_v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_analytics_v4/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_analytics_v4/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.590902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_big_query/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_big_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_big_query/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_big_query/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.590902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_knowledge_graph/gkg_sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_knowledge_graph/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_knowledge_graph/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.590902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_knowledge_graph_v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_knowledge_graph_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_knowledge_graph_v1/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_knowledge_graph_v1/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.590902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_postmaster_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_postmaster_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_postmaster_tools/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_postmaster_tools/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.594902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_search_console/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_search_console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_search_console/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_search_console/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.594902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/onesignal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/onesignal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/onesignal/onesignal_sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/onesignal/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/onesignal/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.594902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/pyspark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/pyspark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/pyspark/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/pyspark/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.594902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/sailthru/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/sailthru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/sailthru/config_magagers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/sailthru/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/sailthru/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/sailthru/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.594902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/sftp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/sftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/sftp/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/sftp/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.594902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/webvitalize/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/webvitalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/webvitalize/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/webvitalize/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.594902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/xero/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/xero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/xero/config_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/xero/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/xero/writers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13559 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/xero/xero_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.594902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/xml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/xml/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/xml/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.594902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_crm/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_crm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22264 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_crm/bulk_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_crm/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_crm/records_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_crm/users_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_crm/writers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_crm/zoho_crm_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.594902 sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_recruit/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_recruit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_recruit/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_recruit/writers.py
--rw-r--r--   0 runner    (1001) docker     (127)    28830 2024-03-13 07:07:55.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_recruit/zoho_recruit_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 07:07:58.586902 sdc_dp_helpers-1.3.97/sdc_dp_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-13 07:07:58.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-03-13 07:07:58.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 07:07:58.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-13 07:07:58.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-13 07:07:58.000000 sdc_dp_helpers-1.3.97/sdc_dp_helpers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-13 07:07:58.594902 sdc_dp_helpers-1.3.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-03-13 07:07:57.000000 sdc_dp_helpers-1.3.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.287393 sdc_dp_helpers-1.3.99/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-03 05:51:16.287393 sdc_dp_helpers-1.3.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.271393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.271393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/api_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/api_utilities/__init_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/api_utilities/data_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20801 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/api_utilities/date_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/api_utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/api_utilities/file_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/api_utilities/retry_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/api_utilities/tracking_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.275393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/azure/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/azure/writers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/base_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/base_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12994 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/base_writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.275393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/facebook/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/facebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/facebook/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/facebook/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.275393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/falcon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/falcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/falcon/falcon_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/falcon/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/falcon/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.275393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/ftp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/ftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/ftp/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/ftp/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.275393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_ads/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_ads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_ads/generate_refresh_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_ads/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_ads/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.275393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_analytics/config_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17278 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_analytics/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_analytics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_analytics/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.275393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_analytics_v4/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_analytics_v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_analytics_v4/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_analytics_v4/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.279393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_big_query/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_big_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_big_query/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_big_query/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.279393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_knowledge_graph/gkg_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_knowledge_graph/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_knowledge_graph/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.279393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_knowledge_graph_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_knowledge_graph_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_knowledge_graph_v1/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_knowledge_graph_v1/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.279393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_postmaster_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_postmaster_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_postmaster_tools/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_postmaster_tools/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.279393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_search_console/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_search_console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_search_console/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_search_console/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.279393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/onesignal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/onesignal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/onesignal/onesignal_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/onesignal/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/onesignal/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.279393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/pyspark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/pyspark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/pyspark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/pyspark/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.279393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/sailthru/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/sailthru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/sailthru/config_magagers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/sailthru/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/sailthru/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/sailthru/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.283393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/sftp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/sftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/sftp/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/sftp/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.283393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/webvitalize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/webvitalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/webvitalize/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/webvitalize/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.283393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/xero/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/xero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/xero/config_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/xero/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/xero/writers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13559 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/xero/xero_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.283393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/xml/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/xml/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.283393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_crm/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_crm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22264 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_crm/bulk_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_crm/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_crm/records_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_crm/users_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_crm/writers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_crm/zoho_crm_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.283393 sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_recruit/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_recruit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_recruit/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_recruit/writers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28830 2024-05-03 05:51:11.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_recruit/zoho_recruit_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:51:16.271393 sdc_dp_helpers-1.3.99/sdc_dp_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-03 05:51:15.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-03 05:51:16.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 05:51:15.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-03 05:51:15.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 05:51:15.000000 sdc_dp_helpers-1.3.99/sdc_dp_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-03 05:51:16.287393 sdc_dp_helpers-1.3.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-03 05:51:14.000000 sdc_dp_helpers-1.3.99/setup.py
```

### Comparing `sdc_dp_helpers-1.3.97/README.md` & `sdc_dp_helpers-1.3.99/README.md`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/api_utilities/data_managers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/api_utilities/data_managers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/api_utilities/date_managers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/api_utilities/date_managers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/api_utilities/exceptions.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/api_utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/api_utilities/file_managers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/api_utilities/file_managers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/api_utilities/retry_managers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/api_utilities/retry_managers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/api_utilities/tracking_metadata.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/api_utilities/tracking_metadata.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/azure/readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/azure/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/azure/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/azure/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/base_readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/base_readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/base_writer.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/base_writer.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/base_writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/base_writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/facebook/readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/facebook/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/facebook/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/facebook/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/falcon/falcon_sdk.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/falcon/falcon_sdk.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/falcon/readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/falcon/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/falcon/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/falcon/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/ftp/readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/ftp/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/ftp/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/ftp/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_ads/generate_refresh_token.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_ads/generate_refresh_token.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_ads/readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_ads/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_ads/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_ads/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_analytics/config_managers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_analytics/config_managers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_analytics/readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_analytics/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_analytics/utils.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_analytics/utils.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_analytics/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_analytics/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_analytics_v4/readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_analytics_v4/readers.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,31 +8,34 @@
     DateRange,
     Dimension,
     Filter,
     FilterExpression,
     Metric,
     RunReportRequest,
 )
+from google.api_core import exceptions
 
 
 from sdc_dp_helpers.api_utilities.date_managers import date_range_iterator
 from sdc_dp_helpers.api_utilities.file_managers import load_file
 
 
 class GAV4Reader:
     """
     GOOGLE ANALYTICS V4 READERS CLASS
     """
+
     api_calls = 0
 
     def __init__(self, configs_file_path: str, service_account_file_path: str):
         self.configs = load_file(configs_file_path, fmt="yml")
         self.service_account_file_path = service_account_file_path
         self._client = self._get_client()
         self.dataset = []
+        self.errors: dict = {}
 
     def _get_client(self):
         client = BetaAnalyticsDataClient().from_service_account_json(
             self.service_account_file_path
         )
         return client
 
@@ -55,31 +58,31 @@
                 row_data[metric_headers[idx].name] = metric_value_key.value
 
             list_dataset.append(row_data)
             # print(row_data)
         return list_dataset
 
     @staticmethod
-    def build_multi_dimension_filter(config):
+    def build_multi_dimension_filter(config: dict):
+        """method to build the api query to run"""
         for field_name, value in config.items():
             in_list_filter = Filter.InListFilter(values=value)
             dimension_filter = FilterExpression(
                 filter=Filter(
                     field_name=field_name,
                     in_list_filter=in_list_filter,
                 )
             )
         return dimension_filter
 
     def _query_handler(self, property_id: str, start_date: str, end_date: str):
         """Runs a simple report on a Google Analytics 4 property."""
         # Explicitly use service account credentials by specifying
         # the private key file.
-        # query = self.build_query(property_id,date)
-        # request = RunReportRequest(**query)
+        response = None
         if self.configs.get("filters") is None:
             request = RunReportRequest(
                 property=f"properties/{property_id}",
                 dimensions=[Dimension(name=dim) for dim in self.configs["dimensions"]],
                 metrics=[Metric(name=metric) for metric in self.configs["metrics"]],
                 date_ranges=[DateRange(start_date=start_date, end_date=end_date)],
                 limit=self.configs.get("limit", 100000),
@@ -92,17 +95,24 @@
                 date_ranges=[DateRange(start_date=start_date, end_date=end_date)],
                 dimension_filter=self.build_multi_dimension_filter(
                     self.configs.get("filters")
                 ),
                 limit=self.configs.get("limit", 100000),
             )
         GAV4Reader.api_calls += 1
-        response = self._client.run_report(request)
+        try:
+            response = self._client.run_report(request)
+        except exceptions.InvalidArgument as error:
+            print(f"invalid parameters for property_id: {error.message}")
+            response = {"details": "invalid parameters"}
+            self.errors[property_id] = error.message
+        except Exception as error:
+            print(f"Number of api calls made before this error {GAV4Reader.api_calls}")
+            raise error
         return response
-        # [END analyticsdata_json_credentials_run_report]
 
     def run_query(self):
         """Controls the Flow of Query"""
         try:
             for property_id in self.configs["property_ids"]:
                 for start_date, end_date in date_range_iterator(
                     start_date=self.configs["start_date"],
@@ -112,20 +122,30 @@
                     time_format="%Y-%m-%d",
                 ):
                     payload = self._query_handler(
                         property_id=property_id,
                         start_date=start_date,
                         end_date=end_date,
                     )
-                    if payload:
-                        dataset: List[Dict] = self._normalize(payload, property_id)
-                        yield {
-                            "date": start_date,
-                            "property_id": property_id,
-                            "data": dataset,
-                        }
-                        self.dataset = dataset
+
+                    if (
+                        isinstance(payload, dict)
+                        and payload.get("details") == "invalid parameters"
+                    ):
+                        break
+                    if not payload:
+                        continue
+
+                    dataset: List[Dict] = self._normalize(payload, property_id)
+                    yield {
+                        "date": start_date,
+                        "property_id": property_id,
+                        "data": dataset,
+                    }
+                    self.dataset = dataset
+                if not self.dataset:
+                    print(f"no data for property_id {property_id}")
         except Exception as error:
             print(f"Number of api calls made before this error {GAV4Reader.api_calls}")
             raise error
         finally:
             print(f"Current number of api calls: {GAV4Reader.api_calls}")
```

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_analytics_v4/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_analytics_v4/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_big_query/readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_big_query/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_big_query/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_big_query/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_knowledge_graph/gkg_sdk.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_knowledge_graph/gkg_sdk.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_knowledge_graph/readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_knowledge_graph/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_knowledge_graph/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_knowledge_graph/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_knowledge_graph_v1/readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_knowledge_graph_v1/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_knowledge_graph_v1/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_knowledge_graph_v1/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_postmaster_tools/readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_postmaster_tools/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_postmaster_tools/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_postmaster_tools/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_search_console/readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_search_console/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/google_search_console/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/google_search_console/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/onesignal/onesignal_sdk.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/onesignal/onesignal_sdk.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/onesignal/readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/onesignal/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/onesignal/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/onesignal/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/pyspark/utils.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/pyspark/utils.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/pyspark/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/pyspark/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/sailthru/readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/sailthru/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/sailthru/utils.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/sailthru/utils.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/sailthru/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/sailthru/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/sftp/readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/sftp/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/sftp/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/sftp/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/webvitalize/readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/webvitalize/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/webvitalize/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/webvitalize/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/xero/readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/xero/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/xero/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/xero/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/xero/xero_sdk.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/xero/xero_sdk.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/xml/readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/xml/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/xml/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/xml/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_crm/bulk_endpoint.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_crm/bulk_endpoint.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_crm/readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_crm/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_crm/records_endpoint.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_crm/records_endpoint.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_crm/users_endpoint.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_crm/users_endpoint.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_crm/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_crm/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_crm/zoho_crm_sdk.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_crm/zoho_crm_sdk.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_recruit/readers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_recruit/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_recruit/writers.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_recruit/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers/zoho_recruit/zoho_recruit_sdk.py` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers/zoho_recruit/zoho_recruit_sdk.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/sdc_dp_helpers.egg-info/SOURCES.txt` & `sdc_dp_helpers-1.3.99/sdc_dp_helpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.97/setup.py` & `sdc_dp_helpers-1.3.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,19 +71,19 @@
         "paramiko",
         "google-cloud-enterpriseknowledgegraph>=0.3.3",
     ],
     extras_require={"pyspark": ["pyspark"]},
     cmdclass={"sdist_zip": sdistzip},
     description="A module for developing data pipelines from external api's and on ETL like services",
 
-    version="1.3.97",
+    version="1.3.99",
 
     url="http://github.com/RingierIMU/sdc-dataPipeline-helpers",
     author="Ringier South Africa",
     author_email="tools@ringier.co.za",
     keywords=[
         "pip",
         "datapipeline",
         "helpers",
     ],
-    download_url="https://github.com/RingierIMU/sdc-global-dataPipeline-helpers/archive/v1.3.97.zip",
+    download_url="https://github.com/RingierIMU/sdc-global-dataPipeline-helpers/archive/v1.3.99.zip",
 )
```


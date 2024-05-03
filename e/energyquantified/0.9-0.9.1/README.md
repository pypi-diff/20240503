# Comparing `tmp/energyquantified-0.9.tar.gz` & `tmp/energyquantified-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyquantified-0.9.tar", last modified: Thu Oct  6 13:39:34 2022, max compression
+gzip compressed data, was "energyquantified-0.9.1.tar", last modified: Fri Oct 21 12:36:06 2022, max compression
```

## Comparing `energyquantified-0.9.tar` & `energyquantified-0.9.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-06 13:39:34.614519 energyquantified-0.9/
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     4557 2022-10-06 13:39:34.614519 energyquantified-0.9/PKG-INFO
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     2609 2021-07-02 08:18:52.000000 energyquantified-0.9/README.md
-drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-06 13:39:34.590518 energyquantified-0.9/energyquantified/
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      524 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/__init__.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      327 2022-10-06 13:35:38.000000 energyquantified-0.9/energyquantified/__version__.py
-drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-06 13:39:34.594519 energyquantified-0.9/energyquantified/api/
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      433 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/api/__init__.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)    13955 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/api/base.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)    16756 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/api/instances.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     8068 2022-05-23 07:25:45.000000 energyquantified-0.9/energyquantified/api/metadata.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)    11120 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/api/ohlc.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     8224 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/api/period_instances.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     1683 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/api/periods.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)    23474 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/api/srmc.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     2619 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/api/timeseries.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)    10296 2021-10-11 12:30:54.000000 energyquantified-0.9/energyquantified/base.py
-drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-06 13:39:34.594519 energyquantified-0.9/energyquantified/data/
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      659 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/data/__init__.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     2906 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/data/base.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     4773 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/data/ohlc.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)    20714 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/data/periodseries.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     4565 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/data/srmc.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)    20259 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/data/timeseries.py
-drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-06 13:39:34.594519 energyquantified-0.9/energyquantified/exceptions/
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      260 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/exceptions/__init__.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     2148 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/exceptions/api.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      303 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/exceptions/client.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      245 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/exceptions/page.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      172 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/exceptions/parser.py
-drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-06 13:39:34.598518 energyquantified-0.9/energyquantified/http/
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      155 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/http/__init__.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     1673 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/http/rate_limiter.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     2052 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/http/retry.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     3093 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/http/session.py
-drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-06 13:39:34.598518 energyquantified-0.9/energyquantified/metadata/
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      647 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/metadata/__init__.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)    20628 2022-05-23 07:47:33.000000 energyquantified-0.9/energyquantified/metadata/area.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     7125 2022-04-13 09:54:29.000000 energyquantified-0.9/energyquantified/metadata/curve.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     1588 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/metadata/instance.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     7608 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/metadata/ohlc.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     5812 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/metadata/options.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     3604 2022-04-13 09:54:29.000000 energyquantified-0.9/energyquantified/metadata/place.py
-drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-06 13:39:34.610519 energyquantified-0.9/energyquantified/parser/
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)        0 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/parser/__init__.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     4969 2022-04-13 09:54:29.000000 energyquantified-0.9/energyquantified/parser/metadata.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     1595 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/parser/ohlc.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     2770 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/parser/periodseries.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     2618 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/parser/srmc.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     3719 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/parser/timeseries.py
-drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-06 13:39:34.614519 energyquantified-0.9/energyquantified/time/
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      518 2021-10-12 08:21:37.000000 energyquantified-0.9/energyquantified/time/__init__.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)    19766 2021-10-12 08:21:37.000000 energyquantified-0.9/energyquantified/time/_timezone_gas.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     6941 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/time/frequency.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     8112 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/time/helpers.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     8052 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/time/resolution.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      576 2021-10-12 08:21:37.000000 energyquantified-0.9/energyquantified/time/timezone.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     4005 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/time/utils.py
-drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-06 13:39:34.614519 energyquantified-0.9/energyquantified/utils/
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)       99 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/utils/__init__.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      471 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/utils/misc.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     5436 2021-07-02 08:18:52.000000 energyquantified-0.9/energyquantified/utils/page.py
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)    13224 2022-10-06 13:35:12.000000 energyquantified-0.9/energyquantified/utils/pandas.py
-drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-06 13:39:34.590518 energyquantified-0.9/energyquantified.egg-info/
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     4557 2022-10-06 13:39:34.000000 energyquantified-0.9/energyquantified.egg-info/PKG-INFO
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     1956 2022-10-06 13:39:34.000000 energyquantified-0.9/energyquantified.egg-info/SOURCES.txt
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)        1 2022-10-06 13:39:34.000000 energyquantified-0.9/energyquantified.egg-info/dependency_links.txt
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)       58 2022-10-06 13:39:34.000000 energyquantified-0.9/energyquantified.egg-info/requires.txt
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)       17 2022-10-06 13:39:34.000000 energyquantified-0.9/energyquantified.egg-info/top_level.txt
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)       38 2022-10-06 13:39:34.614519 energyquantified-0.9/setup.cfg
--rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     2091 2022-07-26 12:51:48.000000 energyquantified-0.9/setup.py
+drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-21 12:36:06.710825 energyquantified-0.9.1/
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     4559 2022-10-21 12:36:06.710825 energyquantified-0.9.1/PKG-INFO
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     2609 2021-07-02 08:18:52.000000 energyquantified-0.9.1/README.md
+drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-21 12:36:06.702825 energyquantified-0.9.1/energyquantified/
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      524 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/__init__.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      329 2022-10-21 12:32:04.000000 energyquantified-0.9.1/energyquantified/__version__.py
+drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-21 12:36:06.706825 energyquantified-0.9.1/energyquantified/api/
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      433 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/api/__init__.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)    13955 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/api/base.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)    16756 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/api/instances.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     8068 2022-05-23 07:25:45.000000 energyquantified-0.9.1/energyquantified/api/metadata.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)    11120 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/api/ohlc.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     8224 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/api/period_instances.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     1683 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/api/periods.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)    23474 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/api/srmc.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     2619 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/api/timeseries.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)    10296 2021-10-11 12:30:54.000000 energyquantified-0.9.1/energyquantified/base.py
+drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-21 12:36:06.706825 energyquantified-0.9.1/energyquantified/data/
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      659 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/data/__init__.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     2906 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/data/base.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     4773 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/data/ohlc.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)    20714 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/data/periodseries.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     4565 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/data/srmc.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)    20259 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/data/timeseries.py
+drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-21 12:36:06.706825 energyquantified-0.9.1/energyquantified/exceptions/
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      260 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/exceptions/__init__.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     2148 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/exceptions/api.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      303 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/exceptions/client.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      245 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/exceptions/page.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      172 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/exceptions/parser.py
+drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-21 12:36:06.706825 energyquantified-0.9.1/energyquantified/http/
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      155 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/http/__init__.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     1673 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/http/rate_limiter.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     2052 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/http/retry.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     3093 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/http/session.py
+drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-21 12:36:06.706825 energyquantified-0.9.1/energyquantified/metadata/
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      647 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/metadata/__init__.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)    20945 2022-10-21 12:13:03.000000 energyquantified-0.9.1/energyquantified/metadata/area.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     7125 2022-04-13 09:54:29.000000 energyquantified-0.9.1/energyquantified/metadata/curve.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     1588 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/metadata/instance.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     7608 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/metadata/ohlc.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     5812 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/metadata/options.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     3604 2022-04-13 09:54:29.000000 energyquantified-0.9.1/energyquantified/metadata/place.py
+drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-21 12:36:06.710825 energyquantified-0.9.1/energyquantified/parser/
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)        0 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/parser/__init__.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     4969 2022-04-13 09:54:29.000000 energyquantified-0.9.1/energyquantified/parser/metadata.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     1595 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/parser/ohlc.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     2770 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/parser/periodseries.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     2618 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/parser/srmc.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     3719 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/parser/timeseries.py
+drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-21 12:36:06.710825 energyquantified-0.9.1/energyquantified/time/
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      518 2021-10-12 08:21:37.000000 energyquantified-0.9.1/energyquantified/time/__init__.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)    19766 2021-10-12 08:21:37.000000 energyquantified-0.9.1/energyquantified/time/_timezone_gas.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     6941 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/time/frequency.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     8112 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/time/helpers.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     8052 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/time/resolution.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      576 2021-10-12 08:21:37.000000 energyquantified-0.9.1/energyquantified/time/timezone.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     4005 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/time/utils.py
+drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-21 12:36:06.710825 energyquantified-0.9.1/energyquantified/utils/
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)       99 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/utils/__init__.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)      471 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/utils/misc.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     5436 2021-07-02 08:18:52.000000 energyquantified-0.9.1/energyquantified/utils/page.py
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)    13224 2022-10-06 13:35:12.000000 energyquantified-0.9.1/energyquantified/utils/pandas.py
+drwxrwxr-x   0 jonmd     (1000) jonmd     (1000)        0 2022-10-21 12:36:06.702825 energyquantified-0.9.1/energyquantified.egg-info/
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     4559 2022-10-21 12:36:06.000000 energyquantified-0.9.1/energyquantified.egg-info/PKG-INFO
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     1956 2022-10-21 12:36:06.000000 energyquantified-0.9.1/energyquantified.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)        1 2022-10-21 12:36:06.000000 energyquantified-0.9.1/energyquantified.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)       58 2022-10-21 12:36:06.000000 energyquantified-0.9.1/energyquantified.egg-info/requires.txt
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)       17 2022-10-21 12:36:06.000000 energyquantified-0.9.1/energyquantified.egg-info/top_level.txt
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)       38 2022-10-21 12:36:06.710825 energyquantified-0.9.1/setup.cfg
+-rw-rw-r--   0 jonmd     (1000) jonmd     (1000)     2091 2022-07-26 12:51:48.000000 energyquantified-0.9.1/setup.py
```

### Comparing `energyquantified-0.9/PKG-INFO` & `energyquantified-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyquantified
-Version: 0.9
+Version: 0.9.1
 Summary: Energy Quantified Time series API client.
 Home-page: https://github.com/energyquantified/eq-python-client
 Author: Energy Quantified AS
 License: UNKNOWN
 Project-URL: Documentation, https://energyquantified-python.readthedocs.io
 Project-URL: Source, https://github.com/energyquantified/eq-python-client
 Description: # Energy Quantified Python Client
```

### Comparing `energyquantified-0.9/README.md` & `energyquantified-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/__init__.py` & `energyquantified-0.9.1/energyquantified/__init__.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/api/base.py` & `energyquantified-0.9.1/energyquantified/api/base.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/api/instances.py` & `energyquantified-0.9.1/energyquantified/api/instances.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/api/metadata.py` & `energyquantified-0.9.1/energyquantified/api/metadata.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/api/ohlc.py` & `energyquantified-0.9.1/energyquantified/api/ohlc.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/api/period_instances.py` & `energyquantified-0.9.1/energyquantified/api/period_instances.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/api/periods.py` & `energyquantified-0.9.1/energyquantified/api/periods.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/api/srmc.py` & `energyquantified-0.9.1/energyquantified/api/srmc.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/api/timeseries.py` & `energyquantified-0.9.1/energyquantified/api/timeseries.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/base.py` & `energyquantified-0.9.1/energyquantified/base.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/data/__init__.py` & `energyquantified-0.9.1/energyquantified/data/__init__.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/data/base.py` & `energyquantified-0.9.1/energyquantified/data/base.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/data/ohlc.py` & `energyquantified-0.9.1/energyquantified/data/ohlc.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/data/periodseries.py` & `energyquantified-0.9.1/energyquantified/data/periodseries.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/data/srmc.py` & `energyquantified-0.9.1/energyquantified/data/srmc.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/data/timeseries.py` & `energyquantified-0.9.1/energyquantified/data/timeseries.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/exceptions/api.py` & `energyquantified-0.9.1/energyquantified/exceptions/api.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/http/rate_limiter.py` & `energyquantified-0.9.1/energyquantified/http/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/http/retry.py` & `energyquantified-0.9.1/energyquantified/http/retry.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/http/session.py` & `energyquantified-0.9.1/energyquantified/http/session.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/metadata/__init__.py` & `energyquantified-0.9.1/energyquantified/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/metadata/area.py` & `energyquantified-0.9.1/energyquantified/metadata/area.py`

 * *Files 4% similar despite different names*

```diff
@@ -279,21 +279,23 @@
 
         :return: This border as a tuple of (source, sink, allocations)
         :rtype: tuple
         """
         return (self.source, self.sink, self.allocations)
 
     def __hash__(self):
-        return hash(self.as_tuple())
+        return hash((self.__class__,) + self.as_tuple())
 
     def __eq__(self, other):
-        return self.as_tuple() == other.as_tuple()
+        return isinstance(other, self.__class__) and self.as_tuple() == other.as_tuple()
 
     def __ne__(self, other):
-        return self.as_tuple() != other.as_tuple()
+        return (
+            not isinstance(other, self.__class__) or self.as_tuple() != other.as_tuple()
+        )
 
     def __repr__(self):
         return "<Border: %s – %s, allocations=%s>" % (
             self.source.tag,
             self.sink.tag,
             sorted(self.allocations),
         )
@@ -591,14 +593,18 @@
 RU_KGD = Area(tag="RU-KGD", name="Kaliningrad (Russia)", country=True, external=True)
 BY = Area(tag="BY", name="Belarus", country=True, external=True)
 UA = Area(tag="UA", name="Ukraine", country=True, external=True)
 MD = Area(tag="MD", name="Moldova", country=True, external=True)
 MT = Area(tag="MT", name="Malta", country=True, external=True)
 GE = Area(tag="GE", name="Georgia", country=True, external=True)
 
+MA = Area(tag="MA", name="Morocco", country=True, external=True)
+LY = Area(tag="LY", name="Libya", country=True, external=True)
+DZ = Area(tag="DZ", name="Algeria", country=True, external=True)
+
 
 ## Nordic borders
 
 NO1._add_borders((NO2, "I"), (NO3, "I"), (NO5, "I"), (SE3, "I"))
 NO2._add_borders((DE, "I"), (DK1, "I"), (GB, "I"), (NL, "I"), (NO1, "I"), (NO5, "I"))
 NO3._add_borders((NO1, "I"), (NO4, "I"), (NO5, "I"), (SE2, "I"))
 NO4._add_borders((FI, "N"), (NO3, "I"), (SE1, "I"), (SE2, "I"))
@@ -608,42 +614,40 @@
 SE2._add_borders((NO3, "I"), (NO4, "I"), (SE1, "I"), (SE3, "I"))
 SE3._add_borders((DK1, "I"), (FI, "I"), (NO1, "I"), (SE2, "I"), (SE4, "I"))
 SE4._add_borders((DE, "I"), (DK2, "I"), (LT, "I"), (PL, "I"), (SE3, "I"))
 
 DK1._add_borders((DE, "I"), (DK2, "I"), (NL, "I"), (NO2, "I"), (SE3, "I"))
 DK2._add_borders((DE, "I"), (DK1, "I"), (SE4, "I"))
 
-FI._add_borders((EE, "I"), (NO4, "N"), (RU, "E"), (SE1, "I"), (SE3, "I"))
+FI._add_borders((EE, "I"), (NO4, "N"), (RU, "N"), (SE1, "I"), (SE3, "I"))
 
 
 ## Baltic borders
 
 EE._add_borders((FI, "I"), (LV, "I"), (RU, "N"))
-LV._add_borders((EE, "I"), (LT, "I"), (RU, "E"))
-LT._add_borders((BY, "N"), (LV, "I"), (PL, "I"), (RU_KGD, "E"), (SE4, "I"))
+LV._add_borders((EE, "I"), (LT, "I"), (RU, "N"))
+LT._add_borders((BY, "N"), (LV, "I"), (PL, "I"), (RU_KGD, "N"), (SE4, "I"))
 
 
 ## Central Western Europe
 
 DE._add_borders(
     (AT, "F"),
     (BE, "F"),
     (CH, "E"),
-    (CZ, "EI"),
+    (CZ, "F"),
     (DK1, "I"),
     (DK2, "I"),
     (FR, "F"),
     (NL, "F"),
     (NO2, "I"),
-    (PL, "EI"),
+    (PL, "F"),
     (SE4, "I"),
 )
-AT._add_borders(
-    (CH, "E"), (CZ, "I"), (DE, "F"), (HU, "I"), (IT_NORD, "EI"), (SI, "EI")
-)
+AT._add_borders((CH, "E"), (CZ, "I"), (DE, "F"), (HU, "I"), (IT_NORD, "EI"), (SI, "F"))
 FR._add_borders((BE, "F"), (CH, "E"), (DE, "F"), (ES, "EI"), (GB, "E"), (IT_NORD, "EI"))
 FR_COR._add_borders((IT_SARD, "I"))
 NL._add_borders((BE, "F"), (DE, "F"), (DK1, "I"), (GB, "E"), (NO2, "I"))
 BE._add_borders((DE, "F"), (FR, "F"), (GB, "E"), (NL, "F"))
 CH._add_borders((AT, "E"), (DE, "E"), (FR, "E"), (IT_NORD, "E"))
 
 
@@ -652,18 +656,18 @@
 GB._add_borders((BE, "E"), (FR, "E"), (NL, "E"), (NIE, "I"), (IE, "I"), (NO2, "I"))
 NIE._add_borders((IE, "I"), (GB, "I"))
 IE._add_borders((NIE, "I"), (GB, "I"))
 
 
 ## Central Eastern Europe
 
-PL._add_borders((CZ, "EI"), (DE, "EI"), (LT, "I"), (SE4, "I"), (SK, "EI"), (UA, "E"))
-CZ._add_borders((AT, "I"), (DE, "EI"), (PL, "EI"), (SK, "EI"))
-HU._add_borders((AT, "I"), (HR, "E"), (RO, "EI"), (RS, "E"), (SK, "EI"), (UA, "E"))
-SK._add_borders((CZ, "EI"), (HU, "EI"), (PL, "EI"), (UA, "E"))
+PL._add_borders((CZ, "F"), (DE, "F"), (LT, "I"), (SE4, "I"), (SK, "F"), (UA, "E"))
+CZ._add_borders((AT, "I"), (DE, "F"), (PL, "F"), (SK, "F"))
+HU._add_borders((AT, "I"), (HR, "F"), (RO, "F"), (RS, "E"), (SI, "F"), (SK, "F"), (UA, "E"))
+SK._add_borders((CZ, "F"), (HU, "F"), (PL, "F"), (UA, "E"))
 
 
 ## Iberian Peninsula
 
 ES._add_borders((FR, "EI"), (PT, "I"))
 PT._add_borders((ES, "I"))
 
@@ -675,17 +679,17 @@
 IT_CSUD._add_borders((IT_CNOR, "I"), (IT_SARD, "I"), (IT_SUD, "I"), (ME, "E"))
 IT_SUD._add_borders((GR, "EI"), (IT_CSUD, "I"), (IT_CALA, "I"))
 IT_CALA._add_borders((IT_SUD, "I"), (IT_SICI, "I"))
 IT_SICI._add_borders((IT_CALA, "I"), (MT, "I"))
 IT_SARD._add_borders((FR_COR, "I"), (IT_CNOR, "I"), (IT_CSUD, "I"))
 
 
-SI._add_borders((AT, "EI"), (HR, "EI"), (IT_NORD, "EI"))
-RO._add_borders((BG, "E"), (HU, "EI"), (RS, "E"), (UA, "E"))
-HR._add_borders((BA, "E"), (HU, "E"), (RS, "E"), (SI, "EI"))
+SI._add_borders((AT, "F"), (HR, "EF"), (HU, "F"), (IT_NORD, "EI"))
+RO._add_borders((BG, "E"), (HU, "F"), (RS, "E"), (UA, "E"))
+HR._add_borders((BA, "E"), (HU, "F"), (RS, "E"), (SI, "EF"))
 BA._add_borders((HR, "E"), (ME, "E"), (RS, "E"))
 RS._add_borders(
     (BA, "E"),
     (BG, "E"),
     (HR, "E"),
     (HU, "E"),
     (ME, "E"),
@@ -704,13 +708,13 @@
 ## South-Eastern Europe
 
 TR._add_borders((BG, "E"), (GE, "E"), (GR, "E"))
 
 
 ## Others
 
-RU._add_borders((EE, "N"), (FI, "E"), (LV, "E"))
-RU_KGD._add_borders((LT, "E"))
+RU._add_borders((EE, "N"), (FI, "N"), (LV, "N"))
+RU_KGD._add_borders((LT, "N"))
 BY._add_borders((LT, "N"))
 UA._add_borders((HU, "E"), (PL, "E"), (RO, "E"), (SK, "E"))
 MT._add_borders((IT_SICI, "I"))
 GE._add_borders((TR, "E"))
```

### Comparing `energyquantified-0.9/energyquantified/metadata/curve.py` & `energyquantified-0.9.1/energyquantified/metadata/curve.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/metadata/instance.py` & `energyquantified-0.9.1/energyquantified/metadata/instance.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/metadata/ohlc.py` & `energyquantified-0.9.1/energyquantified/metadata/ohlc.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/metadata/options.py` & `energyquantified-0.9.1/energyquantified/metadata/options.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/metadata/place.py` & `energyquantified-0.9.1/energyquantified/metadata/place.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/parser/metadata.py` & `energyquantified-0.9.1/energyquantified/parser/metadata.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/parser/ohlc.py` & `energyquantified-0.9.1/energyquantified/parser/ohlc.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/parser/periodseries.py` & `energyquantified-0.9.1/energyquantified/parser/periodseries.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/parser/srmc.py` & `energyquantified-0.9.1/energyquantified/parser/srmc.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/parser/timeseries.py` & `energyquantified-0.9.1/energyquantified/parser/timeseries.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/time/__init__.py` & `energyquantified-0.9.1/energyquantified/time/__init__.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/time/_timezone_gas.py` & `energyquantified-0.9.1/energyquantified/time/_timezone_gas.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/time/frequency.py` & `energyquantified-0.9.1/energyquantified/time/frequency.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/time/helpers.py` & `energyquantified-0.9.1/energyquantified/time/helpers.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/time/resolution.py` & `energyquantified-0.9.1/energyquantified/time/resolution.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/time/timezone.py` & `energyquantified-0.9.1/energyquantified/time/timezone.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/time/utils.py` & `energyquantified-0.9.1/energyquantified/time/utils.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/utils/page.py` & `energyquantified-0.9.1/energyquantified/utils/page.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified/utils/pandas.py` & `energyquantified-0.9.1/energyquantified/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/energyquantified.egg-info/PKG-INFO` & `energyquantified-0.9.1/energyquantified.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyquantified
-Version: 0.9
+Version: 0.9.1
 Summary: Energy Quantified Time series API client.
 Home-page: https://github.com/energyquantified/eq-python-client
 Author: Energy Quantified AS
 License: UNKNOWN
 Project-URL: Documentation, https://energyquantified-python.readthedocs.io
 Project-URL: Source, https://github.com/energyquantified/eq-python-client
 Description: # Energy Quantified Python Client
```

### Comparing `energyquantified-0.9/energyquantified.egg-info/SOURCES.txt` & `energyquantified-0.9.1/energyquantified.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `energyquantified-0.9/setup.py` & `energyquantified-0.9.1/setup.py`

 * *Files identical despite different names*


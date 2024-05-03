# Comparing `tmp/moexalgo-2.0.0.tar.gz` & `tmp/moexalgo-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moexalgo-2.0.0.tar", last modified: Fri May  3 11:36:42 2024, max compression
+gzip compressed data, was "moexalgo-2.0.1.tar", last modified: Fri May  3 14:30:46 2024, max compression
```

## Comparing `moexalgo-2.0.0.tar` & `moexalgo-2.0.1.tar`

### file list

```diff
@@ -1,72 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.988378 moexalgo-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.976378 moexalgo-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.976378 moexalgo-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-03 11:36:38.000000 moexalgo-2.0.0/.github/workflows/python-publish_flow.yml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-03 11:36:38.000000 moexalgo-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-03 11:36:38.000000 moexalgo-2.0.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-03 11:36:38.000000 moexalgo-2.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-03 11:36:42.988378 moexalgo-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-03 11:36:38.000000 moexalgo-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.976378 moexalgo-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.980378 moexalgo-2.0.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.980378 moexalgo-2.0.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    48404 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/_static/newplot.png
--rw-r--r--   0 runner    (1001) docker     (127)    34177 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/_static/output_4_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/candels.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.currency.rst
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.futures.rst
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.indices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.market.rst
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.models.common.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.models.indices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.models.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.models.shares.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.rst
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.session.rst
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.stocks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.tickers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.984378 moexalgo-2.0.0/moexalgo/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 11:36:42.000000 moexalgo-2.0.0/moexalgo/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/candles.py
--rw-r--r--   0 runner    (1001) docker     (127)    13794 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/currency.py
--rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/futures.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/indices.py
--rw-r--r--   0 runner    (1001) docker     (127)    24493 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/market.py
--rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.984378 moexalgo-2.0.0/moexalgo/models/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/models/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/models/indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/models/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/models/shares.py
--rw-r--r--   0 runner    (1001) docker     (127)    13962 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    13607 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/stocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/tickers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.988378 moexalgo-2.0.0/moexalgo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-03 11:36:42.000000 moexalgo-2.0.0/moexalgo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-03 11:36:42.000000 moexalgo-2.0.0/moexalgo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:36:42.000000 moexalgo-2.0.0/moexalgo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 11:36:42.000000 moexalgo-2.0.0/moexalgo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 11:36:42.000000 moexalgo-2.0.0/moexalgo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-03 11:36:38.000000 moexalgo-2.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.984378 moexalgo-2.0.0/samples/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 11:36:38.000000 moexalgo-2.0.0/samples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-03 11:36:38.000000 moexalgo-2.0.0/samples/auth.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-05-03 11:36:38.000000 moexalgo-2.0.0/samples/download_algopack_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   157564 2024-05-03 11:36:38.000000 moexalgo-2.0.0/samples/quick_start.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:36:42.988378 moexalgo-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.988378 moexalgo-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 11:36:38.000000 moexalgo-2.0.0/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-03 11:36:38.000000 moexalgo-2.0.0/tests/test_currency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-03 11:36:38.000000 moexalgo-2.0.0/tests/test_futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-03 11:36:38.000000 moexalgo-2.0.0/tests/test_markets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-03 11:36:38.000000 moexalgo-2.0.0/tests/test_stocks.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:38.000000 moexalgo-2.0.0/tests/test_tickers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:30:46.565751 moexalgo-2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:30:46.553751 moexalgo-2.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:30:46.557751 moexalgo-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-03 14:30:41.000000 moexalgo-2.0.1/.github/workflows/python-publish_flow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-03 14:30:41.000000 moexalgo-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-03 14:30:41.000000 moexalgo-2.0.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-03 14:30:41.000000 moexalgo-2.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-03 14:30:46.565751 moexalgo-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-03 14:30:41.000000 moexalgo-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:30:46.557751 moexalgo-2.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:30:46.561751 moexalgo-2.0.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:30:46.561751 moexalgo-2.0.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    48404 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/source/_static/newplot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34177 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/source/_static/output_4_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/source/candels.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/source/moexalgo.currency.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/source/moexalgo.futures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/source/moexalgo.indices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/source/moexalgo.market.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/source/moexalgo.models.common.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/source/moexalgo.models.indices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/source/moexalgo.models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/source/moexalgo.models.shares.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/source/moexalgo.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/source/moexalgo.session.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/source/moexalgo.stocks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/source/moexalgo.tickers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-03 14:30:41.000000 moexalgo-2.0.1/docs/source/moexalgo.utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:30:46.561751 moexalgo-2.0.1/moexalgo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-03 14:30:41.000000 moexalgo-2.0.1/moexalgo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 14:30:46.000000 moexalgo-2.0.1/moexalgo/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-03 14:30:41.000000 moexalgo-2.0.1/moexalgo/candles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13794 2024-05-03 14:30:41.000000 moexalgo-2.0.1/moexalgo/currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-03 14:30:41.000000 moexalgo-2.0.1/moexalgo/futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-03 14:30:41.000000 moexalgo-2.0.1/moexalgo/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24499 2024-05-03 14:30:41.000000 moexalgo-2.0.1/moexalgo/market.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-05-03 14:30:41.000000 moexalgo-2.0.1/moexalgo/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:30:46.565751 moexalgo-2.0.1/moexalgo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-03 14:30:41.000000 moexalgo-2.0.1/moexalgo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-03 14:30:41.000000 moexalgo-2.0.1/moexalgo/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-03 14:30:41.000000 moexalgo-2.0.1/moexalgo/models/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-03 14:30:41.000000 moexalgo-2.0.1/moexalgo/models/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-05-03 14:30:41.000000 moexalgo-2.0.1/moexalgo/models/shares.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13976 2024-05-03 14:30:41.000000 moexalgo-2.0.1/moexalgo/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13607 2024-05-03 14:30:41.000000 moexalgo-2.0.1/moexalgo/stocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-03 14:30:41.000000 moexalgo-2.0.1/moexalgo/tickers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-03 14:30:41.000000 moexalgo-2.0.1/moexalgo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:30:46.565751 moexalgo-2.0.1/moexalgo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-03 14:30:46.000000 moexalgo-2.0.1/moexalgo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-03 14:30:46.000000 moexalgo-2.0.1/moexalgo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:30:46.000000 moexalgo-2.0.1/moexalgo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 14:30:46.000000 moexalgo-2.0.1/moexalgo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 14:30:46.000000 moexalgo-2.0.1/moexalgo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-03 14:30:41.000000 moexalgo-2.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:30:46.565751 moexalgo-2.0.1/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 14:30:41.000000 moexalgo-2.0.1/samples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-03 14:30:41.000000 moexalgo-2.0.1/samples/auth.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   138920 2024-05-03 14:30:41.000000 moexalgo-2.0.1/samples/quick_start.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 14:30:46.565751 moexalgo-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:30:46.565751 moexalgo-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 14:30:41.000000 moexalgo-2.0.1/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-03 14:30:41.000000 moexalgo-2.0.1/tests/test_currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-03 14:30:41.000000 moexalgo-2.0.1/tests/test_futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-03 14:30:41.000000 moexalgo-2.0.1/tests/test_markets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-03 14:30:41.000000 moexalgo-2.0.1/tests/test_stocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-03 14:30:41.000000 moexalgo-2.0.1/tests/test_tickers.py
```

### Comparing `moexalgo-2.0.0/.github/workflows/python-publish_flow.yml` & `moexalgo-2.0.1/.github/workflows/python-publish_flow.yml`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/.gitlab-ci.yml` & `moexalgo-2.0.1/.gitlab-ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # The Docker image that will be used to build your app
 .build_pypi:
   # Functions that should be executed before the build script is run
   before_script:
     - pip config set global.trusted-host "nexus-dev.tech.moex.com:443"
     - pip config set global.index "https://nexus-dev.tech.moex.com/repository/moex-pypi-static-group/pypi"
     - pip config set global.index-url "https://nexus-dev.tech.moex.com/repository/moex-pypi-static-group/simple"
+    - pip config set global.extra-index-url "https://nexus-dev.tech.moex.com/repository/mdata-pypi-static-group/simple"
     - pip config set global.no-cache-dir "false"
     - pip install sphinx sphinx_rtd_theme pandas httpx
 image: nexus-dev.tech.moex.com/moex-docker-static-group/python:3.10
 
 stages:
   - build
   - push
```

### Comparing `moexalgo-2.0.0/CHANGELOG.md` & `moexalgo-2.0.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/PKG-INFO` & `moexalgo-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moexalgo
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python lib for MOEX AlgoPack data
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Financial and Insurance Industry
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `moexalgo-2.0.0/README.md` & `moexalgo-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/docs/Makefile` & `moexalgo-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/docs/make.bat` & `moexalgo-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/docs/source/_static/newplot.png` & `moexalgo-2.0.1/docs/source/_static/newplot.png`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/docs/source/_static/output_4_0.png` & `moexalgo-2.0.1/docs/source/_static/output_4_0.png`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/docs/source/candels.rst` & `moexalgo-2.0.1/docs/source/candels.rst`

 * *Files 3% similar despite different names*

```diff
@@ -32,16 +32,14 @@
 Также, можно получить справочную информацию по инструментам, свечи и прочую торговую статистику
 
 Пример использования
 --------------------
 
 Быстрое знакомство с библиотекой moexalgo - `quick_start.ipynb <./../../../samples/quick_start.ipynb>`_
 
-Получение данных с использованием API - `download_algopack_data.ipynb <./../../../samples/download_algopack_data.ipynb>`_
-
 Пример авторизации - `auth.ipynb <./../../../samples/auth.ipynb>`_
 
 Для работы с библиотекой необходимо авторизоваться на https://passport.moex.com
 
 .. code:: python
 
     from moexalgo import session
```

### Comparing `moexalgo-2.0.0/docs/source/conf.py` & `moexalgo-2.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/moexalgo/__init__.py` & `moexalgo-2.0.1/moexalgo/__init__.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/moexalgo/candles.py` & `moexalgo-2.0.1/moexalgo/candles.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/moexalgo/currency.py` & `moexalgo-2.0.1/moexalgo/currency.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/moexalgo/futures.py` & `moexalgo-2.0.1/moexalgo/futures.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/moexalgo/indices.py` & `moexalgo-2.0.1/moexalgo/indices.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/moexalgo/market.py` & `moexalgo-2.0.1/moexalgo/market.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
         """
         self._ensure_loaded(cs)
         marketdata = self._values['marketdata'].get(secid)
         securities = self._values['securities'].get(secid)
         if securities or marketdata:
             return dict(securities=securities, marketdata=marketdata)
     
-    def _normalize_row(row: dict[str, dict], fields: tuple[str]) -> dict[str, dict]:
+    def _normalize_row(self, row: dict[str, dict], fields: tuple[str]) -> dict[str, dict]:
         """
         Нормализует строку данных о статистике инструмента.
 
         Parameters
         ----------
         row : Dict[str, Any]
             Строка данных о статистике инструмента.
```

### Comparing `moexalgo-2.0.0/moexalgo/metrics.py` & `moexalgo-2.0.1/moexalgo/metrics.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/moexalgo/models/common.py` & `moexalgo-2.0.1/moexalgo/models/common.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/moexalgo/models/indices.py` & `moexalgo-2.0.1/moexalgo/models/indices.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/moexalgo/models/metrics.py` & `moexalgo-2.0.1/moexalgo/models/metrics.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/moexalgo/models/shares.py` & `moexalgo-2.0.1/moexalgo/models/shares.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/moexalgo/session.py` & `moexalgo-2.0.1/moexalgo/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -451,11 +451,11 @@
         while True:
             options['start'] = start
             items = client.get_objects(path, lambda data: result_deserializer(data, section), **options)
             if metrics := items.get(section):
                 for item in metrics:
                     yield item
                     start += 1
-                    if (start - offset) >= limit:
+                    if (start - offset) >= limit or limit < -1:
                         return
             else:
                 return
```

### Comparing `moexalgo-2.0.0/moexalgo/stocks.py` & `moexalgo-2.0.1/moexalgo/stocks.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/moexalgo/tickers.py` & `moexalgo-2.0.1/moexalgo/tickers.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,17 +269,19 @@
             Если `True`, то возвращает `pd.DataFrame`, иначе итератор.
 
         Returns
         -------
         return : Union[iter, pd.DataFrame]
             Стакан лучших цен.
         """
+        if self._PATH.startswith('engines/currency/markets'):
+            raise NotImplementedError("OrderBook is not implemented for currencies")
         path = f'{self._PATH}/boards/{self._boardid}/securities/{self._secid}/orderbook'
         orderbook_it = data_gen(
             cs=cs, 
             path=path, 
             options={}, 
             offset=0, 
-            limit=1_000, 
+            limit=-1,
             section='orderbook'
         )
         return pandas_frame(orderbook_it) if use_dataframe else dataclass_it(orderbook_it)
```

### Comparing `moexalgo-2.0.0/moexalgo/utils.py` & `moexalgo-2.0.1/moexalgo/utils.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/moexalgo.egg-info/PKG-INFO` & `moexalgo-2.0.1/moexalgo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moexalgo
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python lib for MOEX AlgoPack data
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Financial and Insurance Industry
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `moexalgo-2.0.0/moexalgo.egg-info/SOURCES.txt` & `moexalgo-2.0.1/moexalgo.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 moexalgo/models/__init__.py
 moexalgo/models/common.py
 moexalgo/models/indices.py
 moexalgo/models/metrics.py
 moexalgo/models/shares.py
 samples/.gitignore
 samples/auth.ipynb
-samples/download_algopack_data.ipynb
 samples/quick_start.ipynb
 tests/.gitignore
 tests/test_currency.py
 tests/test_futures.py
 tests/test_markets.py
 tests/test_stocks.py
 tests/test_tickers.py
```

### Comparing `moexalgo-2.0.0/pyproject.toml` & `moexalgo-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/samples/auth.ipynb` & `moexalgo-2.0.1/samples/auth.ipynb`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/samples/quick_start.ipynb` & `moexalgo-2.0.1/samples/quick_start.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9753575562169312%*

 * *Differences: {"'cells'": "{0: {'id': '282a2812'}, 1: {'id': '654fd17c'}, 2: {'execution_count': 2, 'id': "*

 * *            "'d414f2d2', 'outputs': []}, 3: {'id': '9533a197'}, 4: {'id': '4227226a'}, 5: {'id': "*

 * *            "'870706be'}, 6: {'id': 'ec7ff97f'}, 7: {'id': 'a4d14605'}, 8: {'id': '80b3cb41'}, 9: "*

 * *            "{'id': '6633a470'}, 10: {'id': 'a6685ed3'}, 11: {'id': '6c0713d8'}, 12: {'id': "*

 * *            "'cc8ba94d'}, 13: {'id': 'e4e0a27d'}, 14: {'id': '70507055'}, 15: {'id': 'df00dcee'}, "*

 * *            "16: {'id': ' […]*

```diff
@@ -1,86 +1,75 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "e7fb060b-5f70-4a71-b182-69729d8860f0",
+            "id": "282a2812",
             "metadata": {},
             "source": [
                 "<h2 style=\"text-align: center;\"><b>Quick start with MOEXALGO!</b></h2>\n",
                 "\n",
                 "---\n",
                 "\n",
                 "---"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "7b15b329-fbef-4c01-924a-851807586047",
+            "id": "654fd17c",
             "metadata": {},
             "source": [
                 "<h3 style=\"text-align: center;\"><b>\u0410\u0432\u0442\u043e\u0440\u0438\u0437\u0430\u0446\u0438\u044f</b></h3>\n",
                 "\n",
                 "---\n",
                 "\n",
                 "\n",
                 "\u0414\u043b\u044f \u0434\u043e\u0441\u0442\u0443\u043f\u0430 \u043a \u0434\u0430\u043d\u043d\u044b\u043c \u043d\u0435\u043e\u0431\u0445\u043e\u0434\u0438\u043c\u043e \u0437\u0430\u0440\u0435\u0433\u0435\u0441\u0442\u0440\u0438\u0440\u043e\u0432\u0430\u0442\u044c\u0441\u044f \u043d\u0430 https://passport.moex.com \u0438 \u0441\u043e\u0445\u0440\u0430\u043d\u0438\u0442\u044c \u043b\u043e\u0433\u0438\u043d/\u043f\u0430\u0440\u043e\u043b\u044c."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
-            "id": "feb0dd72-17aa-4dc5-be1d-654a35038ce6",
+            "execution_count": 2,
+            "id": "d414f2d2",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:42:28.895519862Z",
                     "start_time": "2024-04-25T14:42:28.607667803Z"
                 }
             },
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "True"
-                        ]
-                    },
-                    "execution_count": 11,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
                 "from moexalgo import session, Market, Ticker, CandlePeriod\n",
                 "\n",
                 "username = \"\"\n",
                 "password = \"\"\n",
                 "session.authorize(username, password)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "baae8cba-ccfc-4395-a6aa-ca191b669219",
+            "id": "9533a197",
             "metadata": {},
             "source": [
                 "<h3 style=\"text-align: center;\"><b>C\u043f\u0438\u0441\u043e\u043a \u0434\u043e\u0441\u0442\u0443\u043f\u043d\u044b\u0445 \u0442\u0438\u043a\u0435\u0440\u043e\u0432</b></h3>\n",
                 "\n",
                 "---"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "5fd294e1",
+            "id": "4227226a",
             "metadata": {},
             "source": [
                 "**\u0410\u043a\u0446\u0438\u0438:**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
-            "id": "6f84b675-3b20-4a7d-b73f-60212e19df59",
+            "id": "870706be",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:42:28.896493355Z",
                     "start_time": "2024-04-25T14:42:28.807960517Z"
                 }
             },
             "outputs": [
@@ -292,24 +281,24 @@
             "source": [
                 "eq = Market('EQ')\n",
                 "eq.tickers()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "0a21cfbe",
+            "id": "ec7ff97f",
             "metadata": {},
             "source": [
                 "**\u0412\u0430\u043b\u044e\u0442\u0430:**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
-            "id": "247e22c1-bbec-44f6-b50a-997fed75b60f",
+            "id": "a4d14605",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:42:28.897308539Z",
                     "start_time": "2024-04-25T14:42:28.808487575Z"
                 }
             },
             "outputs": [
@@ -460,24 +449,24 @@
             "source": [
                 "fx = Market('FX')\n",
                 "fx.tickers()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "2f8c842a",
+            "id": "80b3cb41",
             "metadata": {},
             "source": [
                 "**\u0424\u044c\u044e\u0447\u0435\u0440\u0441\u044b:**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
-            "id": "33bac09c-c4b6-4da7-a7c4-af7e0a0a1d6c",
+            "id": "6633a470",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:42:28.897916761Z",
                     "start_time": "2024-04-25T14:42:28.827698088Z"
                 }
             },
             "outputs": [
@@ -616,26 +605,26 @@
             "source": [
                 "fo = Market('FO')\n",
                 "fo.tickers()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9d102986-1f11-4818-9fb5-59e32197244a",
+            "id": "a6685ed3",
             "metadata": {},
             "source": [
                 "<h3 style=\"text-align: center;\"><b>\u0420\u0430\u0431\u043e\u0442\u0430 \u0441 \u0442\u0438\u043a\u0435\u0440\u0430\u043c\u0438</b></h3>\n",
                 "\n",
                 "---"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 15,
-            "id": "087e2e29-c614-4475-b959-3c2316a37d62",
+            "id": "6c0713d8",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:42:28.898133972Z",
                     "start_time": "2024-04-25T14:42:28.841680773Z"
                 }
             },
             "outputs": [],
@@ -648,15 +637,15 @@
                 "\n",
                 "# \u0424\u044c\u044e\u0447\u0435\u0440\u0441\u043d\u044b\u0439 \u043a\u043e\u043d\u0442\u0440\u0430\u043a\u0442 \u0410\u0424\u041a \u0421\u0438\u0441\u0442\u0435\u043c\u0430\n",
                 "akm4 = Ticker('AKM4')"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "81a0047d",
+            "id": "cc8ba94d",
             "metadata": {},
             "source": [
                 "<h4 style=\"text-align: center;\"><b>Candles</b></h4>\n",
                 "\n",
                 "---\n",
                 "\n",
                 "\u041a\u043b\u0430\u0441\u0441\u0438\u0447\u0435\u0441\u043a\u0438\u0435 \u0441\u0432\u0435\u0447\u0438 *OHLCV*\n",
@@ -686,32 +675,32 @@
                 "    - '1d'\n",
                 "    - '1w'\n",
                 "    - '1m'\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "59bd6a3c-7bb4-4a54-877d-28d7dac97f1f",
+            "id": "e4e0a27d",
             "metadata": {},
             "source": [
                 "#### \u2757\ufe0f\u041e\u0433\u0440\u0430\u043d\u0438\u0447\u0435\u043d\u0438\u0435 \u043d\u0430 \u043a\u043e\u043b-\u0432\u043e \u043e\u0442\u0434\u0430\u0432\u0430\u0435\u043c\u044b\u0445 \u0441\u0432\u0435\u0447\u0435\u043a - 10 000\u2757\ufe0f"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c9f401e2",
+            "id": "70507055",
             "metadata": {},
             "source": [
                 "**\u0421\u0432\u0435\u0447\u0438 \u043f\u043e \u0430\u043a\u0446\u0438\u044f\u043c SBER \u0437\u0430 \u043f\u0435\u0440\u0438\u043e\u0434:**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 16,
-            "id": "080af71a-9a92-444f-b29a-04790c4d4bca",
+            "id": "df00dcee",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:42:29.413579258Z",
                     "start_time": "2024-04-25T14:42:28.883973651Z"
                 }
             },
             "outputs": [
@@ -829,24 +818,24 @@
             ],
             "source": [
                 "sber.candles(start='2023-10-10', end='2023-10-18', period='10min').head()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "b070cb90",
+            "id": "3ffc85a5",
             "metadata": {},
             "source": [
                 "**\u0421\u0432\u0435\u0447\u0438 \u043f\u043e \u043a\u0438\u0442\u0430\u0439\u0441\u043a\u043e\u043c\u0443 \u044e\u0430\u043d\u044e \u0437\u0430 \u043f\u0435\u0440\u0438\u043e\u0434:**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 17,
-            "id": "9455094f-cc7c-4797-8e46-730a286aa2c0",
+            "id": "eb476b26",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:42:30.519085304Z",
                     "start_time": "2024-04-25T14:42:29.359668644Z"
                 }
             },
             "outputs": [
@@ -964,24 +953,24 @@
             ],
             "source": [
                 "cny000000tod.candles(start='2023-10-10', end='2023-10-18', period=CandlePeriod.ONE_MINUTE).head()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "6c9bfc05",
+            "id": "767cacc8",
             "metadata": {},
             "source": [
                 "**\u0421\u0432\u0435\u0447\u0438 \u043f\u043e \u0444\u044c\u044e\u0447\u0435\u0440\u0441\u043d\u043e\u043c\u0443 \u043a\u043e\u043d\u0442\u0440\u0430\u043a\u0442\u0443 \u0437\u0430 \u043f\u0435\u0440\u0438\u043e\u0434:**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 18,
-            "id": "02948340-b572-4cb9-8eb7-ff86651f1b50",
+            "id": "1bbf5f6a",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:42:30.947025932Z",
                     "start_time": "2024-04-25T14:42:30.511966295Z"
                 }
             },
             "outputs": [
@@ -1099,34 +1088,34 @@
             ],
             "source": [
                 "akm4.candles(start='2024-04-23', end='2024-04-23', period=60).head()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e25982d8-5a96-4cf6-9189-5e4ed8d8e97b",
+            "id": "21ab49c1",
             "metadata": {},
             "source": [
                 "<h4 style=\"text-align: center;\"><b>OrderBook</b></h4>\n",
                 "\n",
                 "---"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "19f08a0e",
+            "id": "ac434e27",
             "metadata": {},
             "source": [
                 "**C\u0442\u0430\u043a\u0430\u043d \u0437\u0430\u044f\u0432\u043e\u043a \u043f\u043e \u0430\u043a\u0446\u0438\u044f\u043c SBER:**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 19,
-            "id": "bcd77e3e-568f-4683-938d-cb14386abee5",
+            "id": "e8368209",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:42:31.360407917Z",
                     "start_time": "2024-04-25T14:42:30.949803451Z"
                 }
             },
             "outputs": [
@@ -1440,604 +1429,87 @@
             "source": [
                 "sber = Ticker('SBER')\n",
                 "sber.orderbook()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "6a9faf41",
+            "id": "cd37d3ad",
             "metadata": {},
             "source": [
-                "**C\u0442\u0430\u043a\u0430\u043d \u0437\u0430\u044f\u0432\u043e\u043a \u043f\u043e \u043a\u0438\u0442\u0430\u0439\u0441\u043a\u043e\u043c\u0443 \u044e\u0430\u043d\u044e:**"
+                "**C\u0442\u0430\u043a\u0430\u043d \u0437\u0430\u044f\u0432\u043e\u043a \u043f\u043e \u0444\u044c\u044e\u0447\u0435\u0440\u0441\u043d\u043e\u043c\u0443 \u043a\u043e\u043d\u0442\u0440\u0430\u043a\u0442\u0443:**"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
-            "id": "97ef3ea0-387d-4e7b-a9e1-e18b0711ff2b",
+            "execution_count": 9,
+            "id": "13291c54",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2024-04-25T14:42:31.567879878Z",
-                    "start_time": "2024-04-25T14:42:31.361836812Z"
+                    "end_time": "2024-04-25T14:42:34.284639614Z",
+                    "start_time": "2024-04-25T14:42:31.570520197Z"
                 }
             },
-            "outputs": [
-                {
-                    "data": {
-                        "text/html": [
-                            "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
-                            "<table border=\"1\" class=\"dataframe\">\n",
-                            "  <thead>\n",
-                            "    <tr style=\"text-align: right;\">\n",
-                            "      <th></th>\n",
-                            "      <th>boardid</th>\n",
-                            "      <th>secid</th>\n",
-                            "      <th>buysell</th>\n",
-                            "      <th>price</th>\n",
-                            "      <th>quantity</th>\n",
-                            "      <th>seqnum</th>\n",
-                            "      <th>updatetime</th>\n",
-                            "      <th>decimals</th>\n",
-                            "    </tr>\n",
-                            "  </thead>\n",
-                            "  <tbody>\n",
-                            "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>CETS</td>\n",
-                            "      <td>CNY000000TOD</td>\n",
-                            "      <td>B</td>\n",
-                            "      <td>12.6625</td>\n",
-                            "      <td>400</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:26</td>\n",
-                            "      <td>5</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1</th>\n",
-                            "      <td>CETS</td>\n",
-                            "      <td>CNY000000TOD</td>\n",
-                            "      <td>B</td>\n",
-                            "      <td>12.6630</td>\n",
-                            "      <td>400</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:26</td>\n",
-                            "      <td>5</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2</th>\n",
-                            "      <td>CETS</td>\n",
-                            "      <td>CNY000000TOD</td>\n",
-                            "      <td>B</td>\n",
-                            "      <td>12.6635</td>\n",
-                            "      <td>400</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:26</td>\n",
-                            "      <td>5</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3</th>\n",
-                            "      <td>CETS</td>\n",
-                            "      <td>CNY000000TOD</td>\n",
-                            "      <td>B</td>\n",
-                            "      <td>12.6640</td>\n",
-                            "      <td>354</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:26</td>\n",
-                            "      <td>5</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>4</th>\n",
-                            "      <td>CETS</td>\n",
-                            "      <td>CNY000000TOD</td>\n",
-                            "      <td>B</td>\n",
-                            "      <td>12.6645</td>\n",
-                            "      <td>900</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:26</td>\n",
-                            "      <td>5</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>5</th>\n",
-                            "      <td>CETS</td>\n",
-                            "      <td>CNY000000TOD</td>\n",
-                            "      <td>B</td>\n",
-                            "      <td>12.6650</td>\n",
-                            "      <td>400</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:26</td>\n",
-                            "      <td>5</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>6</th>\n",
-                            "      <td>CETS</td>\n",
-                            "      <td>CNY000000TOD</td>\n",
-                            "      <td>B</td>\n",
-                            "      <td>12.6655</td>\n",
-                            "      <td>3900</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:26</td>\n",
-                            "      <td>5</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>7</th>\n",
-                            "      <td>CETS</td>\n",
-                            "      <td>CNY000000TOD</td>\n",
-                            "      <td>B</td>\n",
-                            "      <td>12.6660</td>\n",
-                            "      <td>400</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:26</td>\n",
-                            "      <td>5</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>8</th>\n",
-                            "      <td>CETS</td>\n",
-                            "      <td>CNY000000TOD</td>\n",
-                            "      <td>B</td>\n",
-                            "      <td>12.6665</td>\n",
-                            "      <td>4510</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:26</td>\n",
-                            "      <td>5</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>9</th>\n",
-                            "      <td>CETS</td>\n",
-                            "      <td>CNY000000TOD</td>\n",
-                            "      <td>B</td>\n",
-                            "      <td>12.6670</td>\n",
-                            "      <td>9</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:26</td>\n",
-                            "      <td>5</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>10</th>\n",
-                            "      <td>CETS</td>\n",
-                            "      <td>CNY000000TOD</td>\n",
-                            "      <td>S</td>\n",
-                            "      <td>12.6695</td>\n",
-                            "      <td>450</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:26</td>\n",
-                            "      <td>5</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>11</th>\n",
-                            "      <td>CETS</td>\n",
-                            "      <td>CNY000000TOD</td>\n",
-                            "      <td>S</td>\n",
-                            "      <td>12.6700</td>\n",
-                            "      <td>800</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:26</td>\n",
-                            "      <td>5</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>12</th>\n",
-                            "      <td>CETS</td>\n",
-                            "      <td>CNY000000TOD</td>\n",
-                            "      <td>S</td>\n",
-                            "      <td>12.6705</td>\n",
-                            "      <td>400</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:26</td>\n",
-                            "      <td>5</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>13</th>\n",
-                            "      <td>CETS</td>\n",
-                            "      <td>CNY000000TOD</td>\n",
-                            "      <td>S</td>\n",
-                            "      <td>12.6710</td>\n",
-                            "      <td>400</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:26</td>\n",
-                            "      <td>5</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>14</th>\n",
-                            "      <td>CETS</td>\n",
-                            "      <td>CNY000000TOD</td>\n",
-                            "      <td>S</td>\n",
-                            "      <td>12.6715</td>\n",
-                            "      <td>3900</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:26</td>\n",
-                            "      <td>5</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>15</th>\n",
-                            "      <td>CETS</td>\n",
-                            "      <td>CNY000000TOD</td>\n",
-                            "      <td>S</td>\n",
-                            "      <td>12.6720</td>\n",
-                            "      <td>1400</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:26</td>\n",
-                            "      <td>5</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>16</th>\n",
-                            "      <td>CETS</td>\n",
-                            "      <td>CNY000000TOD</td>\n",
-                            "      <td>S</td>\n",
-                            "      <td>12.6725</td>\n",
-                            "      <td>1900</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:26</td>\n",
-                            "      <td>5</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>17</th>\n",
-                            "      <td>CETS</td>\n",
-                            "      <td>CNY000000TOD</td>\n",
-                            "      <td>S</td>\n",
-                            "      <td>12.6730</td>\n",
-                            "      <td>2400</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:26</td>\n",
-                            "      <td>5</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>18</th>\n",
-                            "      <td>CETS</td>\n",
-                            "      <td>CNY000000TOD</td>\n",
-                            "      <td>S</td>\n",
-                            "      <td>12.6735</td>\n",
-                            "      <td>900</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:26</td>\n",
-                            "      <td>5</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>19</th>\n",
-                            "      <td>CETS</td>\n",
-                            "      <td>CNY000000TOD</td>\n",
-                            "      <td>S</td>\n",
-                            "      <td>12.6740</td>\n",
-                            "      <td>400</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:26</td>\n",
-                            "      <td>5</td>\n",
-                            "    </tr>\n",
-                            "  </tbody>\n",
-                            "</table>\n",
-                            "</div>"
-                        ],
-                        "text/plain": [
-                            "   boardid         secid buysell    price  quantity          seqnum  \\\n",
-                            "0     CETS  CNY000000TOD       B  12.6625       400  20240425174226   \n",
-                            "1     CETS  CNY000000TOD       B  12.6630       400  20240425174226   \n",
-                            "2     CETS  CNY000000TOD       B  12.6635       400  20240425174226   \n",
-                            "3     CETS  CNY000000TOD       B  12.6640       354  20240425174226   \n",
-                            "4     CETS  CNY000000TOD       B  12.6645       900  20240425174226   \n",
-                            "5     CETS  CNY000000TOD       B  12.6650       400  20240425174226   \n",
-                            "6     CETS  CNY000000TOD       B  12.6655      3900  20240425174226   \n",
-                            "7     CETS  CNY000000TOD       B  12.6660       400  20240425174226   \n",
-                            "8     CETS  CNY000000TOD       B  12.6665      4510  20240425174226   \n",
-                            "9     CETS  CNY000000TOD       B  12.6670         9  20240425174226   \n",
-                            "10    CETS  CNY000000TOD       S  12.6695       450  20240425174226   \n",
-                            "11    CETS  CNY000000TOD       S  12.6700       800  20240425174226   \n",
-                            "12    CETS  CNY000000TOD       S  12.6705       400  20240425174226   \n",
-                            "13    CETS  CNY000000TOD       S  12.6710       400  20240425174226   \n",
-                            "14    CETS  CNY000000TOD       S  12.6715      3900  20240425174226   \n",
-                            "15    CETS  CNY000000TOD       S  12.6720      1400  20240425174226   \n",
-                            "16    CETS  CNY000000TOD       S  12.6725      1900  20240425174226   \n",
-                            "17    CETS  CNY000000TOD       S  12.6730      2400  20240425174226   \n",
-                            "18    CETS  CNY000000TOD       S  12.6735       900  20240425174226   \n",
-                            "19    CETS  CNY000000TOD       S  12.6740       400  20240425174226   \n",
-                            "\n",
-                            "   updatetime  decimals  \n",
-                            "0    17:42:26         5  \n",
-                            "1    17:42:26         5  \n",
-                            "2    17:42:26         5  \n",
-                            "3    17:42:26         5  \n",
-                            "4    17:42:26         5  \n",
-                            "5    17:42:26         5  \n",
-                            "6    17:42:26         5  \n",
-                            "7    17:42:26         5  \n",
-                            "8    17:42:26         5  \n",
-                            "9    17:42:26         5  \n",
-                            "10   17:42:26         5  \n",
-                            "11   17:42:26         5  \n",
-                            "12   17:42:26         5  \n",
-                            "13   17:42:26         5  \n",
-                            "14   17:42:26         5  \n",
-                            "15   17:42:26         5  \n",
-                            "16   17:42:26         5  \n",
-                            "17   17:42:26         5  \n",
-                            "18   17:42:26         5  \n",
-                            "19   17:42:26         5  "
-                        ]
-                    },
-                    "execution_count": 20,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "cny000000tod = Ticker('CNY000000TOD')\n",
-                "cny000000tod.orderbook()"
+                "akm4 = Ticker('SiM4')\n",
+                "akm4.orderbook()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "7aa82d8f",
+            "id": "5e400569",
             "metadata": {},
             "source": [
-                "**C\u0442\u0430\u043a\u0430\u043d \u0437\u0430\u044f\u0432\u043e\u043a \u043f\u043e \u0444\u044c\u044e\u0447\u0435\u0440\u0441\u043d\u043e\u043c\u0443 \u043a\u043e\u043d\u0442\u0440\u0430\u043a\u0442\u0443:**"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 21,
-            "id": "2ce27ba7-b7ef-4014-b482-e1857c34c467",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-04-25T14:42:34.284639614Z",
-                    "start_time": "2024-04-25T14:42:31.570520197Z"
-                }
-            },
-            "outputs": [
-                {
-                    "data": {
-                        "text/html": [
-                            "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
-                            "<table border=\"1\" class=\"dataframe\">\n",
-                            "  <thead>\n",
-                            "    <tr style=\"text-align: right;\">\n",
-                            "      <th></th>\n",
-                            "      <th>boardid</th>\n",
-                            "      <th>secid</th>\n",
-                            "      <th>buysell</th>\n",
-                            "      <th>price</th>\n",
-                            "      <th>quantity</th>\n",
-                            "      <th>seqnum</th>\n",
-                            "      <th>updatetime</th>\n",
-                            "      <th>decimals</th>\n",
-                            "    </tr>\n",
-                            "  </thead>\n",
-                            "  <tbody>\n",
-                            "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>RFUD</td>\n",
-                            "      <td>AKM4</td>\n",
-                            "      <td>B</td>\n",
-                            "      <td>26200</td>\n",
-                            "      <td>8</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:25</td>\n",
-                            "      <td>0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1</th>\n",
-                            "      <td>RFUD</td>\n",
-                            "      <td>AKM4</td>\n",
-                            "      <td>B</td>\n",
-                            "      <td>26210</td>\n",
-                            "      <td>4</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:25</td>\n",
-                            "      <td>0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2</th>\n",
-                            "      <td>RFUD</td>\n",
-                            "      <td>AKM4</td>\n",
-                            "      <td>B</td>\n",
-                            "      <td>26217</td>\n",
-                            "      <td>11</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:25</td>\n",
-                            "      <td>0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3</th>\n",
-                            "      <td>RFUD</td>\n",
-                            "      <td>AKM4</td>\n",
-                            "      <td>B</td>\n",
-                            "      <td>26226</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:25</td>\n",
-                            "      <td>0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>4</th>\n",
-                            "      <td>RFUD</td>\n",
-                            "      <td>AKM4</td>\n",
-                            "      <td>B</td>\n",
-                            "      <td>26248</td>\n",
-                            "      <td>13</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:25</td>\n",
-                            "      <td>0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>...</th>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>995</th>\n",
-                            "      <td>RFUD</td>\n",
-                            "      <td>AKM4</td>\n",
-                            "      <td>S</td>\n",
-                            "      <td>26523</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:25</td>\n",
-                            "      <td>0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>996</th>\n",
-                            "      <td>RFUD</td>\n",
-                            "      <td>AKM4</td>\n",
-                            "      <td>S</td>\n",
-                            "      <td>26526</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:25</td>\n",
-                            "      <td>0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>997</th>\n",
-                            "      <td>RFUD</td>\n",
-                            "      <td>AKM4</td>\n",
-                            "      <td>S</td>\n",
-                            "      <td>26540</td>\n",
-                            "      <td>4</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:25</td>\n",
-                            "      <td>0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>998</th>\n",
-                            "      <td>RFUD</td>\n",
-                            "      <td>AKM4</td>\n",
-                            "      <td>S</td>\n",
-                            "      <td>26548</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:25</td>\n",
-                            "      <td>0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>999</th>\n",
-                            "      <td>RFUD</td>\n",
-                            "      <td>AKM4</td>\n",
-                            "      <td>S</td>\n",
-                            "      <td>26554</td>\n",
-                            "      <td>10</td>\n",
-                            "      <td>20240425174226</td>\n",
-                            "      <td>17:42:25</td>\n",
-                            "      <td>0</td>\n",
-                            "    </tr>\n",
-                            "  </tbody>\n",
-                            "</table>\n",
-                            "<p>1000 rows \u00d7 8 columns</p>\n",
-                            "</div>"
-                        ],
-                        "text/plain": [
-                            "    boardid secid buysell  price  quantity          seqnum updatetime  \\\n",
-                            "0      RFUD  AKM4       B  26200         8  20240425174226   17:42:25   \n",
-                            "1      RFUD  AKM4       B  26210         4  20240425174226   17:42:25   \n",
-                            "2      RFUD  AKM4       B  26217        11  20240425174226   17:42:25   \n",
-                            "3      RFUD  AKM4       B  26226         1  20240425174226   17:42:25   \n",
-                            "4      RFUD  AKM4       B  26248        13  20240425174226   17:42:25   \n",
-                            "..      ...   ...     ...    ...       ...             ...        ...   \n",
-                            "995    RFUD  AKM4       S  26523         1  20240425174226   17:42:25   \n",
-                            "996    RFUD  AKM4       S  26526         1  20240425174226   17:42:25   \n",
-                            "997    RFUD  AKM4       S  26540         4  20240425174226   17:42:25   \n",
-                            "998    RFUD  AKM4       S  26548         1  20240425174226   17:42:25   \n",
-                            "999    RFUD  AKM4       S  26554        10  20240425174226   17:42:25   \n",
-                            "\n",
-                            "     decimals  \n",
-                            "0           0  \n",
-                            "1           0  \n",
-                            "2           0  \n",
-                            "3           0  \n",
-                            "4           0  \n",
-                            "..        ...  \n",
-                            "995         0  \n",
-                            "996         0  \n",
-                            "997         0  \n",
-                            "998         0  \n",
-                            "999         0  \n",
-                            "\n",
-                            "[1000 rows x 8 columns]"
-                        ]
-                    },
-                    "execution_count": 21,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "akm4 = Ticker('AKM4')\n",
-                "akm4.orderbook()"
+                "#### \u0421\u0442\u0430\u043a\u0430\u043d\u044b \u043f\u043e \u0432\u0430\u043b\u044e\u0442\u043d\u043e\u043c\u0443 \u0440\u044b\u043d\u043a\u0443 \u043d\u0435 \u0434\u043e\u0441\u0442\u0443\u043f\u043d\u044b\u2757\ufe0f"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "45a4d857-eb6d-4cfa-ac45-966ea3eb4a4c",
+            "id": "b2094db2",
             "metadata": {},
             "source": [
                 "<h3 style=\"text-align: center;\"><b>\u041c\u0435\u0442\u0440\u0438\u043a\u0438 TradeStats, OrderStats, Obstats, HI2, FUTOI</b></h3>\n",
                 "\n",
                 "---"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "5a7ffe51-e559-40ca-bcf4-7fc8a1291b96",
+            "id": "e9acc0bc",
             "metadata": {},
             "source": [
                 "<h4 style=\"text-align: center;\"><b>Tradestats</b></h4>\n",
                 "\n",
                 "---\n",
                 "\n",
                 "\u0422\u043e\u0440\u0433\u043e\u0432\u0430\u044f \u0441\u0442\u0430\u0442\u0438\u0441\u0442\u0438\u043a\u0430 \u043d\u0430 \u043e\u0441\u043d\u043e\u0432\u0435 \u0441\u0434\u0435\u043b\u043e\u043a\n",
                 "\n",
                 "**\u0413\u0440\u0430\u043d\u0443\u043b\u044f\u0440\u043d\u043e\u0441\u0442\u044c \u0434\u0430\u043d\u043d\u044b\u0445:** 5 \u043c\u0438\u043d\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c36d43fe-90ac-4a20-82db-a30469a65a62",
+            "id": "638a453e",
             "metadata": {},
             "source": [
                 "\u041f\u0440\u0438\u043c\u0435\u0440 \u043f\u043e\u043b\u0443\u0447\u0435\u043d\u0438\u044f \u0434\u0430\u043d\u043d\u044b\u0445 TradeStats \u0437\u0430 \u043a\u043e\u043d\u043a\u0440\u0435\u0442\u043d\u044b\u0439 \u0434\u0435\u043d\u044c.\n",
                 "\n",
                 "**\u0420\u044b\u043d\u043e\u043a \u0430\u043a\u0446\u0438\u0439:**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e80feed0db5e49a",
+            "id": "9fd87818",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:42:40.358044715Z",
                     "start_time": "2024-04-25T14:42:34.287065417Z"
                 },
-                "collapsed": false,
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [
                 {
                     "data": {
@@ -2241,34 +1713,34 @@
             ],
             "source": [
                 "eq.tradestats(date='2023-10-10').head()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "3cebab2a",
+            "id": "e6a51e72",
             "metadata": {},
             "source": [
                 "_*\u0427\u0442\u043e\u0431\u044b \u043f\u043e\u043b\u0443\u0447\u0438\u0442\u044c \u0434\u0430\u043d\u043d\u044b\u0435 \u0437\u0430 \u043f\u0435\u0440\u0438\u043e\u0434, \u043d\u0443\u0436\u043d\u043e \u0437\u0430\u043f\u0443\u0441\u0442\u0438\u0442\u044c \u0446\u0438\u043a\u043b \u043f\u043e \u0434\u0430\u0442\u0430\u043c_"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "8c425b50-ad4a-44bf-afd4-a17a0447c137",
+            "id": "2f6fa876",
             "metadata": {},
             "source": [
                 "\u0410\u043d\u0430\u043b\u043e\u0433\u0438\u0447\u043d\u043e \u0434\u043b\u044f \u0434\u0440\u0443\u0433\u0438\u0445 \u0440\u044b\u043d\u043a\u043e\u0432.\n",
                 "\n",
                 "**\u0420\u044b\u043d\u043e\u043a \u0444\u044c\u044e\u0447\u0435\u0440\u0441\u043e\u0432:**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 23,
-            "id": "8c072daf-8363-4f0c-b131-97cb291ccca7",
+            "id": "8b20c2a6",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:42:45.749359746Z",
                     "start_time": "2024-04-25T14:42:40.361279440Z"
                 }
             },
             "outputs": [
@@ -2474,24 +1946,24 @@
             ],
             "source": [
                 "fo.tradestats(date='2024-04-22').head()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "76cdd0ec",
+            "id": "0a8c8470",
             "metadata": {},
             "source": [
                 "**\u0420\u044b\u043d\u043e\u043a \u0432\u0430\u043b\u044e\u0442:**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 24,
-            "id": "9553e7fe-3d80-4f8d-9bb0-a909c2b7d4a7",
+            "id": "c3b0bf6e",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:42:46.521657688Z",
                     "start_time": "2024-04-25T14:42:45.752206346Z"
                 }
             },
             "outputs": [
@@ -2697,24 +2169,24 @@
             ],
             "source": [
                 "fx.tradestats(date='2024-04-22').head()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "901c30fe-df5c-46a3-b6e5-e97312700113",
+            "id": "d383716b",
             "metadata": {},
             "source": [
                 "\u0414\u0430\u043d\u043d\u044b\u0435 TradeStats \u043f\u043e \u0430\u043a\u0446\u0438\u044f\u043c SBER \u0437\u0430 \u043f\u0435\u0440\u0438\u043e\u0434"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 25,
-            "id": "bbb7f59d-66c4-4e9d-a846-9c5ba0e19233",
+            "id": "8a501b23",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:42:46.928100831Z",
                     "start_time": "2024-04-25T14:42:46.474961267Z"
                 }
             },
             "outputs": [
@@ -2920,48 +2392,48 @@
             ],
             "source": [
                 "sber.tradestats(start='2023-10-10', end='2023-10-18').head()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "1aed8f1c-61c3-44c6-a25d-41c08a86a5aa",
+            "id": "d114c02f",
             "metadata": {},
             "source": [
                 "<h4 style=\"text-align: center;\"><b>Orderstats</b></h4>\n",
                 "\n",
                 "---\n",
                 "\n",
                 "\u0422\u043e\u0440\u0433\u043e\u0432\u0430\u044f \u0441\u0442\u0430\u0442\u0438\u0441\u0442\u0438\u043a\u0430 \u043d\u0430 \u043e\u0441\u043d\u043e\u0432\u0435 \u0437\u0430\u044f\u0432\u043e\u043a\n",
                 "\n",
                 "**\u0413\u0440\u0430\u043d\u0443\u043b\u044f\u0440\u043d\u043e\u0441\u0442\u044c \u0434\u0430\u043d\u043d\u044b\u0445:** 5 \u043c\u0438\u043d\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e64d6b53",
+            "id": "af4c6e63",
             "metadata": {},
             "source": [
                 "##### \u2757\ufe0f \u0414\u043b\u044f \u0440\u044b\u043d\u043a\u0430 \u0444\u044c\u044e\u0447\u0435\u0440\u0441\u043e\u0432 \u043d\u0435\u0442 \u043c\u0435\u0442\u0440\u0438\u043a\u0438 OrderStats \u2757\ufe0f"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "7d545542-2d11-4789-97d1-d7f687c022b2",
+            "id": "18d2ca76",
             "metadata": {},
             "source": [
                 "\u0414\u0430\u043d\u043d\u044b\u0435 OrderStats \u0437\u0430 \u0434\u0430\u0442\u0443 \u0437\u0430 \u043a\u043e\u043d\u043a\u0440\u0435\u0442\u043d\u044b\u0439 \u0434\u0435\u043d\u044c.\n",
                 "\n",
                 "**\u0420\u044b\u043d\u043e\u043a \u0430\u043a\u0446\u0438\u0439:**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 26,
-            "id": "5f963eea-c7c4-4fde-9de8-7f91a4d81479",
+            "id": "7ddf7eab",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:42:56.472053892Z",
                     "start_time": "2024-04-25T14:42:46.926808204Z"
                 }
             },
             "outputs": [
@@ -3174,32 +2646,32 @@
             ],
             "source": [
                 "eq.orderstats(date='2024-04-22').head()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "6f77c584",
+            "id": "07d0b41a",
             "metadata": {},
             "source": [
                 "_*\u0427\u0442\u043e\u0431\u044b \u043f\u043e\u043b\u0443\u0447\u0438\u0442\u044c \u0434\u0430\u043d\u043d\u044b\u0435 \u0437\u0430 \u043f\u0435\u0440\u0438\u043e\u0434, \u043d\u0443\u0436\u043d\u043e \u0437\u0430\u043f\u0443\u0441\u0442\u0438\u0442\u044c \u0446\u0438\u043a\u043b \u043f\u043e \u0434\u0430\u0442\u0430\u043c_"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "27544791",
+            "id": "5b421627",
             "metadata": {},
             "source": [
                 "**\u0420\u044b\u043d\u043e\u043a \u0432\u0430\u043b\u044e\u0442:**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 27,
-            "id": "2be8abd3-ad48-48fe-abf4-3dcf1e9cf4bd",
+            "id": "fa6dcf2e",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:42:57.148687224Z",
                     "start_time": "2024-04-25T14:42:56.427828288Z"
                 }
             },
             "outputs": [
@@ -3403,24 +2875,24 @@
             ],
             "source": [
                 "fx.orderstats(date='2024-04-22').head()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "b5d43d5e-1cc6-4145-beeb-9ff30876b55e",
+            "id": "c5ed36b4",
             "metadata": {},
             "source": [
                 "\u0414\u0430\u043d\u043d\u044b\u0435 OrderStats \u043f\u043e \u0430\u043a\u0446\u0438\u044f\u043c SBER \u0437\u0430 \u043f\u0435\u0440\u0438\u043e\u0434"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 28,
-            "id": "684e1cf5-bcfb-408e-a666-4ea10fb22b80",
+            "id": "89085e40",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:42:57.934018786Z",
                     "start_time": "2024-04-25T14:42:57.126349175Z"
                 }
             },
             "outputs": [
@@ -3633,40 +3105,40 @@
             ],
             "source": [
                 "sber.orderstats(start='2023-10-10', end='2023-10-18').head()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c3942ccd-1549-4ba8-8f8c-45a56c44c92f",
+            "id": "ea3cd151",
             "metadata": {},
             "source": [
                 "<h4 style=\"text-align: center;\"><b>OrderBookStats</b></h4>\n",
                 "\n",
                 "---\n",
                 "\n",
                 "\u0422\u043e\u0440\u0433\u043e\u0432\u0430\u044f \u0441\u0442\u0430\u0442\u0438\u0441\u0442\u0438\u043a\u0430 \u043d\u0430 \u043e\u0441\u043d\u043e\u0432\u0435 \u0441\u0442\u0430\u043a\u0430\u043d\u0430 \u0437\u0430\u044f\u0432\u043e\u043a\n",
                 "\n",
                 "**\u0413\u0440\u0430\u043d\u0443\u043b\u044f\u0440\u043d\u043e\u0441\u0442\u044c \u0434\u0430\u043d\u043d\u044b\u0445:** 5 \u043c\u0438\u043d\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "0ccff365-ee32-47f9-a590-fe73ff444d64",
+            "id": "e9541081",
             "metadata": {},
             "source": [
                 "\u0414\u0430\u043d\u043d\u044b\u0435 ObStats \u0437\u0430 \u0434\u0430\u0442\u0443 \u0437\u0430 \u043a\u043e\u043d\u043a\u0440\u0435\u0442\u043d\u044b\u0439 \u0434\u0435\u043d\u044c.\n",
                 "\n",
                 "**\u0420\u044b\u043d\u043e\u043a \u0430\u043a\u0446\u0438\u0439:**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 29,
-            "id": "974518bd-e257-46ad-b9ce-630453c5d4d0",
+            "id": "6c49f64e",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:43:06.646384370Z",
                     "start_time": "2024-04-25T14:42:57.936908629Z"
                 }
             },
             "outputs": [
@@ -3879,33 +3351,34 @@
             ],
             "source": [
                 "eq.obstats(date='2024-04-10').head()"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "4224a928",
             "metadata": {},
             "source": [
                 "_*\u0427\u0442\u043e\u0431\u044b \u043f\u043e\u043b\u0443\u0447\u0438\u0442\u044c \u0434\u0430\u043d\u043d\u044b\u0435 \u0437\u0430 \u043f\u0435\u0440\u0438\u043e\u0434, \u043d\u0443\u0436\u043d\u043e \u0437\u0430\u043f\u0443\u0441\u0442\u0438\u0442\u044c \u0446\u0438\u043a\u043b \u043f\u043e \u0434\u0430\u0442\u0430\u043c_"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a12cba02-c72b-484a-8766-38946071ac6f",
+            "id": "31f1d8e4",
             "metadata": {},
             "source": [
                 "\u0410\u043d\u0430\u043b\u043e\u0433\u0438\u0447\u043d\u043e \u0434\u043b\u044f \u0434\u0440\u0443\u0433\u0438\u0445 \u0440\u044b\u043d\u043a\u043e\u0432.\n",
                 "\n",
                 "**\u0420\u044b\u043d\u043e\u043a \u0432\u0430\u043b\u044e\u0442:**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 30,
-            "id": "8da25528-22dc-43d0-b7eb-4f9c41666b54",
+            "id": "36ccc469",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:43:07.456789957Z",
                     "start_time": "2024-04-25T14:43:06.648979985Z"
                 }
             },
             "outputs": [
@@ -4119,15 +3592,15 @@
             "source": [
                 "fx.obstats(date='2024-04-10').head()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 31,
-            "id": "dfebaddd-2c1c-46a2-85a4-e0f96a99b031",
+            "id": "792400e1",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:43:07.807169256Z",
                     "start_time": "2024-04-25T14:43:07.457480625Z"
                 }
             },
             "outputs": [
@@ -4172,24 +3645,24 @@
             ],
             "source": [
                 "fo.obstats(date='2024-04-10').head()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "f05daa81-e8e4-4c66-b476-2fc03d4da0cf",
+            "id": "b2b1d58c",
             "metadata": {},
             "source": [
                 "\u0414\u0430\u043d\u043d\u044b\u0435 OrderBookStats \u043f\u043e \u0430\u043a\u0446\u0438\u044f\u043c SBER \u0437\u0430 \u043f\u0435\u0440\u0438\u043e\u0434"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 32,
-            "id": "080dfada-a0f7-4a3d-92c9-4f2d95cd8031",
+            "id": "fc2596fa",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:43:08.255865202Z",
                     "start_time": "2024-04-25T14:43:07.814003668Z"
                 }
             },
             "outputs": [
@@ -4402,30 +3875,30 @@
             ],
             "source": [
                 "sber.obstats(start='2023-10-10', end='2023-10-18').head()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "6f73b380-de9f-4535-92eb-37cba24ec5de",
+            "id": "638d906d",
             "metadata": {},
             "source": [
                 "<h4 style=\"text-align: center;\"><b>HI2</b></h4>\n",
                 "\n",
                 "---\n",
                 "\n",
                 "\u0422\u043e\u0440\u0433\u043e\u0432\u0430\u044f \u0441\u0442\u0430\u0442\u0438\u0441\u0442\u0438\u043a\u0430 \u043d\u0430 \u043e\u0441\u043d\u043e\u0432\u0435 \u0438\u043d\u0434\u0435\u043a\u0441\u0430 \u0440\u044b\u043d\u043e\u0447\u043d\u043e\u0439 \u043a\u043e\u043d\u0446\u0435\u043d\u0442\u0440\u0430\u0446\u0438\u0438\n",
                 "\n",
                 "**\u0413\u0440\u0430\u043d\u0443\u043b\u044f\u0440\u043d\u043e\u0441\u0442\u044c \u0434\u0430\u043d\u043d\u044b\u0445:** 24 \u0447\u0430\u0441\u0430."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 33,
-            "id": "482c3450-04fc-4ab1-85f5-e113d13edb7f",
+            "id": "860181d1",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:43:08.651859321Z",
                     "start_time": "2024-04-25T14:43:08.246288928Z"
                 }
             },
             "outputs": [
@@ -4537,30 +4010,30 @@
             ],
             "source": [
                 "sber.hi2(start='2024-04-10', end='2024-04-18').head()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "757235ce-a4de-4a15-892f-136ec875eaa2",
+            "id": "368f706a",
             "metadata": {},
             "source": [
                 "<h4 style=\"text-align: center;\"><b>FUTOI</b></h4>\n",
                 "\n",
                 "---\n",
                 "\n",
                 "\u0422\u043e\u0440\u0433\u043e\u0432\u0430\u044f \u0441\u0442\u0430\u0442\u0438\u0441\u0442\u0438\u043a\u0430 \u043d\u0430 \u043e\u0441\u043d\u043e\u0432\u0435 \u043e\u0442\u043a\u0440\u044b\u0442\u044b\u0445 \u043f\u043e\u0437\u0438\u0446\u0438\u0439 \u043f\u043e \u0444\u044c\u044e\u0447\u0435\u0440\u0441\u043d\u044b\u043c \u043a\u043e\u043d\u0442\u0440\u0430\u043a\u0442\u0430\u043c \u0432 \u0440\u0430\u0437\u0440\u0435\u0437\u0435 \u0444\u0438\u0437. \u0438 \u044e\u0440. \u043b\u0438\u0446\n",
                 "\n",
                 "**\u0413\u0440\u0430\u043d\u0443\u043b\u044f\u0440\u043d\u043e\u0441\u0442\u044c \u0434\u0430\u043d\u043d\u044b\u0445:** 5 \u043c\u0438\u043d."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 34,
-            "id": "c9e42c88-ef11-457f-9a2a-87ed970db006",
+            "id": "fdf3baec",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-04-25T14:43:11.755100501Z",
                     "start_time": "2024-04-25T14:43:08.633532627Z"
                 }
             },
             "outputs": [
@@ -4703,27 +4176,27 @@
             "source": [
                 "fo.futoi(date=\"2024-04-08\").head()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "Python 3",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.6"
+            "version": "3.8.3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `moexalgo-2.0.0/tests/test_currency.py` & `moexalgo-2.0.1/tests/test_currency.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/tests/test_futures.py` & `moexalgo-2.0.1/tests/test_futures.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/tests/test_markets.py` & `moexalgo-2.0.1/tests/test_markets.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.0/tests/test_stocks.py` & `moexalgo-2.0.1/tests/test_stocks.py`

 * *Files identical despite different names*


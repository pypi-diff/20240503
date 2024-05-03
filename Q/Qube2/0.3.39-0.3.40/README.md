# Comparing `tmp/Qube2-0.3.39.tar.gz` & `tmp/Qube2-0.3.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Qube2-0.3.39.tar", last modified: Wed May  1 15:37:16 2024, max compression
+gzip compressed data, was "Qube2-0.3.40.tar", last modified: Fri May  3 11:45:15 2024, max compression
```

## Comparing `Qube2-0.3.39.tar` & `Qube2-0.3.40.tar`

### file list

```diff
@@ -1,233 +1,233 @@
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.148076 Qube2-0.3.39/
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1325 2024-01-09 18:52:45.000000 Qube2-0.3.39/LICENSE
--rw-r--r--   0 quant0    (1000) quant0    (1000)      226 2024-01-09 18:52:45.000000 Qube2-0.3.39/MANIFEST.in
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1210 2024-05-01 15:37:16.148076 Qube2-0.3.39/PKG-INFO
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.148076 Qube2-0.3.39/Qube2.egg-info/
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1210 2024-05-01 15:37:16.000000 Qube2-0.3.39/Qube2.egg-info/PKG-INFO
--rw-r--r--   0 quant0    (1000) quant0    (1000)     6304 2024-05-01 15:37:16.000000 Qube2-0.3.39/Qube2.egg-info/SOURCES.txt
--rw-r--r--   0 quant0    (1000) quant0    (1000)        1 2024-05-01 15:37:16.000000 Qube2-0.3.39/Qube2.egg-info/dependency_links.txt
--rw-r--r--   0 quant0    (1000) quant0    (1000)      270 2024-05-01 15:37:16.000000 Qube2-0.3.39/Qube2.egg-info/requires.txt
--rw-r--r--   0 quant0    (1000) quant0    (1000)        5 2024-05-01 15:37:16.000000 Qube2-0.3.39/Qube2.egg-info/top_level.txt
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1134 2024-01-09 18:52:45.000000 Qube2-0.3.39/README.md
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.136076 Qube2-0.3.39/bin/
--rw-r--r--   0 quant0    (1000) quant0    (1000)     5849 2024-01-09 18:52:45.000000 Qube2-0.3.39/bin/booster
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.136076 Qube2-0.3.39/qube/
--rw-r--r--   0 quant0    (1000) quant0    (1000)     7261 2024-05-01 15:36:56.000000 Qube2-0.3.39/qube/__init__.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.136076 Qube2-0.3.39/qube/booster/
--rw-r--r--   0 quant0    (1000) quant0    (1000)       22 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/booster/__init__.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.136076 Qube2-0.3.39/qube/booster/app/
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/booster/app/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    21047 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/booster/app/boo.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    20152 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/booster/app/reports.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     5511 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/booster/app/signal_viewer.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.136076 Qube2-0.3.39/qube/booster/app/templates/
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2559 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/booster/app/templates/detailed_report.html
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1627 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/booster/app/templates/experiment_chart_report.html
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2593 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/booster/app/templates/experiment_report.html
--rw-r--r--   0 quant0    (1000) quant0    (1000)      754 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/booster/app/templates/experiments_index.html
--rw-r--r--   0 quant0    (1000) quant0    (1000)      656 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/booster/app/templates/index.html
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2428 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/booster/app/templates/main_report.html
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2536 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/booster/app/templates/signals_viewer.html
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2511 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/booster/app/templates/tearsheet_report.html
--rw-r--r--   0 quant0    (1000) quant0    (1000)    16074 2024-05-01 15:36:56.000000 Qube2-0.3.39/qube/booster/boosterai.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    46792 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/booster/core.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.136076 Qube2-0.3.39/qube/booster/data/
--rw-r--r--   0 quant0    (1000) quant0    (1000)    13501 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/booster/data/markets.yml
--rw-r--r--   0 quant0    (1000) quant0    (1000)    14897 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/booster/simctrl.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     5984 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/booster/utils.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.136076 Qube2-0.3.39/qube/charting/
--rw-r--r--   0 quant0    (1000) quant0    (1000)       35 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/charting/__init__.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.140076 Qube2-0.3.39/qube/charting/highcharts/
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/charting/highcharts/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     9714 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/charting/highcharts/core.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2704 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/charting/highcharts/display.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    27021 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/charting/lookinglass.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    29533 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/charting/mpl_finance.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    18006 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/charting/plot_helpers.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.140076 Qube2-0.3.39/qube/configs/
--rw-r--r--   0 quant0    (1000) quant0    (1000)     3943 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/configs/Properties.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/configs/__init__.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.140076 Qube2-0.3.39/qube/configs/config-default/
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1388 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/configs/config-default/datasource.json
--rw-r--r--   0 quant0    (1000) quant0    (1000)    30265 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/configs/config-default/dukas_outlook.csv
--rw-r--r--   0 quant0    (1000) quant0    (1000)      399 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/configs/config-default/main-props.json
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.140076 Qube2-0.3.39/qube/configs/config-test/
--rw-r--r--   0 quant0    (1000) quant0    (1000)      720 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/configs/config-test/datasource.json
--rw-r--r--   0 quant0    (1000) quant0    (1000)    30265 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/configs/config-test/dukas_outlook.csv
--rw-r--r--   0 quant0    (1000) quant0    (1000)      348 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/configs/config-test/main-props.json
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.140076 Qube2-0.3.39/qube/datasource/
--rw-r--r--   0 quant0    (1000) quant0    (1000)     3025 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/datasource/CsvConnector.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    11829 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/datasource/DataSource.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2947 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/datasource/DataserverConnector.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)      731 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/datasource/DukasOutlookConnector.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1585 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/datasource/InMemoryDataSource.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    12102 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/datasource/KdbConnector.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2132 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/datasource/MongoConnector.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2040 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/datasource/YahooConnector.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)      318 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/datasource/__init__.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.140076 Qube2-0.3.39/qube/datasource/controllers/
--rw-r--r--   0 quant0    (1000) quant0    (1000)     7152 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/datasource/controllers/KdbServerController.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2592 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/datasource/controllers/MemcacheController.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     9283 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/datasource/controllers/MongoController.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/datasource/controllers/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     6343 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/datasource/controllers/kdb_utils.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    13096 2024-03-21 09:37:59.000000 Qube2-0.3.39/qube/datasource/loaders.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.140076 Qube2-0.3.39/qube/examples/
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/examples/__init__.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.140076 Qube2-0.3.39/qube/examples/booster/
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1166 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/examples/booster/test_portfolio_task.yml
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.140076 Qube2-0.3.39/qube/examples/learn/
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/examples/learn/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     4573 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/examples/learn/filters.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    12840 2024-04-28 09:52:57.000000 Qube2-0.3.39/qube/examples/learn/generators.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     4056 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/examples/learn/transformers.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.140076 Qube2-0.3.39/qube/examples/strategies/
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/examples/strategies/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    11151 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/examples/strategies/test_strategies.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     7825 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/examples/strategies/turtles.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.140076 Qube2-0.3.39/qube/learn/
--rw-r--r--   0 quant0    (1000) quant0    (1000)      488 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/learn/__init__.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.140076 Qube2-0.3.39/qube/learn/advanced/
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/learn/advanced/__init__.py
--rw-rw-r--   0 quant0    (1000) quant0    (1000)     9997 2024-03-25 15:09:12.000000 Qube2-0.3.39/qube/learn/advanced/labeling.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.140076 Qube2-0.3.39/qube/learn/core/
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/learn/core/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     9903 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/learn/core/base.py
--rw-rw-r--   0 quant0    (1000) quant0    (1000)     8250 2024-02-01 11:19:00.000000 Qube2-0.3.39/qube/learn/core/data_utils.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     7603 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/learn/core/metrics.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2838 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/learn/core/mlhelpers.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     4375 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/learn/core/operations.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     6278 2024-03-21 09:37:59.000000 Qube2-0.3.39/qube/learn/core/pickers.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)      499 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/learn/core/structs.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     3713 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/learn/core/utils.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.140076 Qube2-0.3.39/qube/portfolio/
--rw-r--r--   0 quant0    (1000) quant0    (1000)      426 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/portfolio/Instrument.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     6804 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/portfolio/PortfolioLogger.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    18942 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/portfolio/Position.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/portfolio/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     6437 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/portfolio/allocating.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)      480 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/portfolio/broker_constants.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    18671 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/portfolio/commissions.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     5030 2024-03-24 12:41:39.000000 Qube2-0.3.39/qube/portfolio/drawdown.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    28343 2024-03-24 14:11:27.000000 Qube2-0.3.39/qube/portfolio/performance.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.140076 Qube2-0.3.39/qube/portfolio/report_templates/
--rw-r--r--   0 quant0    (1000) quant0    (1000)      107 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/portfolio/report_templates/comparison_report.tpl
--rw-r--r--   0 quant0    (1000) quant0    (1000)     3562 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/portfolio/report_templates/old_report.tpl
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2452 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/portfolio/report_templates/optimizer_report.tpl
--rw-r--r--   0 quant0    (1000) quant0    (1000)      224 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/portfolio/report_templates/signal_statistics_report.tpl
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2794 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/portfolio/report_templates/simple_report.tpl
--rw-rw-r--   0 quant0    (1000) quant0    (1000)    15023 2024-03-26 13:47:54.000000 Qube2-0.3.39/qube/portfolio/reports.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     5074 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/portfolio/signals_analysis.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.140076 Qube2-0.3.39/qube/quantitative/
--rw-r--r--   0 quant0    (1000) quant0    (1000)      171 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/quantitative/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1783 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/quantitative/fast_ols.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.144076 Qube2-0.3.39/qube/quantitative/stats/
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/quantitative/stats/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    14152 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/quantitative/stats/cointegration.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     6593 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/quantitative/stats/ssa.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     9430 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/quantitative/stats/stats.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.144076 Qube2-0.3.39/qube/quantitative/ta/
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/quantitative/ta/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     4030 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/quantitative/ta/bands.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     6037 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/quantitative/ta/dtw.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    63739 2024-03-24 12:41:39.000000 Qube2-0.3.39/qube/quantitative/ta/indicators.py
--rw-rw-r--   0 quant0    (1000) quant0    (1000)     3983 2024-03-26 13:47:54.000000 Qube2-0.3.39/qube/quantitative/ta/kalman.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     3813 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/quantitative/ta/pewma.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.144076 Qube2-0.3.39/qube/quantitative/ta/swings/
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/quantitative/ta/swings/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     7087 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/quantitative/ta/swings/reversals.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    20699 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/quantitative/ta/swings/swings_splitter.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    16531 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/quantitative/tools.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     6798 2024-03-24 14:11:27.000000 Qube2-0.3.39/qube/qube_nb_magic_init.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.144076 Qube2-0.3.39/qube/series/
--rw-r--r--   0 quant0    (1000) quant0    (1000)      452 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/series/Bar.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    12186 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/series/BarSeries.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1594 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/series/DoubleSeries.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    23849 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/series/Indicators.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1325 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/series/Quote.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2653 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/series/Series.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/series/__init__.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.144076 Qube2-0.3.39/qube/simulator/
--rw-r--r--   0 quant0    (1000) quant0    (1000)     4555 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/simulator/Brokerage.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    26552 2024-03-24 13:44:39.000000 Qube2-0.3.39/qube/simulator/SignalTester.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)      113 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/simulator/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     3097 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/simulator/backtester.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    10392 2024-03-24 14:11:27.000000 Qube2-0.3.39/qube/simulator/core.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     7620 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/simulator/management.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    10776 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/simulator/multiproc.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    24085 2024-03-24 12:41:39.000000 Qube2-0.3.39/qube/simulator/multisim.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.144076 Qube2-0.3.39/qube/simulator/tracking/
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/simulator/tracking/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2925 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/simulator/tracking/sizers.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    48671 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/simulator/tracking/trackers.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    14604 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/simulator/tracking/trailings.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    31999 2024-04-28 09:52:57.000000 Qube2-0.3.39/qube/simulator/utils.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.144076 Qube2-0.3.39/qube/tests/
--rw-r--r--   0 quant0    (1000) quant0    (1000)     7527 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/DateUtils_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/__init__.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.144076 Qube2-0.3.39/qube/tests/booster/
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/booster/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     5246 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/booster/booster_test.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.144076 Qube2-0.3.39/qube/tests/data/
--rw-r--r--   0 quant0    (1000) quant0    (1000)    21024 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/data/EURUSD.csv
--rw-r--r--   0 quant0    (1000) quant0    (1000)     8509 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/data/FDI_test.csv
--rw-r--r--   0 quant0    (1000) quant0    (1000)      242 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/data/RM1.csv
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/data/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1389 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/data/test_mdf.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.144076 Qube2-0.3.39/qube/tests/datasource/
--rw-r--r--   0 quant0    (1000) quant0    (1000)     4448 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/datasource/DataSource_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2578 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/datasource/KdbConnector_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1092 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/datasource/MemcacheController_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1502 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/datasource/MongoConnector_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    10427 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/datasource/MongoController_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/datasource/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2392 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/ds_test_cfg.json
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.144076 Qube2-0.3.39/qube/tests/learn/
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/learn/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     9170 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/learn/base_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     5627 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/learn/scoring_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1091 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/ntp_test.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.144076 Qube2-0.3.39/qube/tests/portfolio/
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/portfolio/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2771 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/portfolio/commissions_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2089 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/portfolio/drawdown_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     4458 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/portfolio/portfolio_allocating_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     5449 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/portfolio/portfolio_performance_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1084 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/properties_test.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.144076 Qube2-0.3.39/qube/tests/quantitative/
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/quantitative/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    19445 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/quantitative/coint_test.csv
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2226 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/quantitative/cointegration_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1048 2024-03-24 12:41:39.000000 Qube2-0.3.39/qube/tests/quantitative/dtw_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     8038 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/quantitative/indicators_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1735 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/quantitative/kalman_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     2154 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/quantitative/tools_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)       43 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/qube_props_test.json
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.148076 Qube2-0.3.39/qube/tests/series/
--rw-r--r--   0 quant0    (1000) quant0    (1000)     4554 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/series/BarSeries_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     3144 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/series/Indicator_demo_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    20189 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/series/Indicator_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/series/__init__.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.148076 Qube2-0.3.39/qube/tests/simulator/
--rw-r--r--   0 quant0    (1000) quant0    (1000)    10368 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/simulator/Position_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/simulator/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    17897 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/simulator/signal_tester_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     4942 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/simulator/signal_tracker_cloning_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     5696 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/simulator/signal_tracker_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     4563 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/simulator/strategy_tester_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     3743 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/simulator/test_multiproc.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    12994 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/simulator/test_multisim.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    21502 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/simulator/trackers_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     4463 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/simulator/utilities.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    12172 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/simulator/utils_test.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1237 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/tests/utils_for_tests.py
-drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-01 15:37:16.148076 Qube2-0.3.39/qube/utils/
--rw-r--r--   0 quant0    (1000) quant0    (1000)     8591 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/utils/DateUtils.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1428 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/utils/QubeLogger.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/utils/__init__.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     5543 2024-03-24 12:41:39.000000 Qube2-0.3.39/qube/utils/nb_functions.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1890 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/utils/ntp.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1958 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/utils/ui_utils.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)    12709 2024-01-09 18:52:45.000000 Qube2-0.3.39/qube/utils/utils.py
--rw-r--r--   0 quant0    (1000) quant0    (1000)       38 2024-05-01 15:37:16.148076 Qube2-0.3.39/setup.cfg
--rw-r--r--   0 quant0    (1000) quant0    (1000)     1529 2024-01-09 19:23:40.000000 Qube2-0.3.39/setup.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.668714 Qube2-0.3.40/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1325 2024-01-09 18:52:45.000000 Qube2-0.3.40/LICENSE
+-rw-r--r--   0 quant0    (1000) quant0    (1000)      226 2024-01-09 18:52:45.000000 Qube2-0.3.40/MANIFEST.in
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1210 2024-05-03 11:45:15.668714 Qube2-0.3.40/PKG-INFO
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.668714 Qube2-0.3.40/Qube2.egg-info/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1210 2024-05-03 11:45:15.000000 Qube2-0.3.40/Qube2.egg-info/PKG-INFO
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     6304 2024-05-03 11:45:15.000000 Qube2-0.3.40/Qube2.egg-info/SOURCES.txt
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        1 2024-05-03 11:45:15.000000 Qube2-0.3.40/Qube2.egg-info/dependency_links.txt
+-rw-r--r--   0 quant0    (1000) quant0    (1000)      270 2024-05-03 11:45:15.000000 Qube2-0.3.40/Qube2.egg-info/requires.txt
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        5 2024-05-03 11:45:15.000000 Qube2-0.3.40/Qube2.egg-info/top_level.txt
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1134 2024-01-09 18:52:45.000000 Qube2-0.3.40/README.md
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.656715 Qube2-0.3.40/bin/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     5849 2024-01-09 18:52:45.000000 Qube2-0.3.40/bin/booster
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.656715 Qube2-0.3.40/qube/
+-rw-rw-r--   0 quant0    (1000) quant0    (1000)     7261 2024-05-03 11:44:00.000000 Qube2-0.3.40/qube/__init__.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.656715 Qube2-0.3.40/qube/booster/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)       22 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/booster/__init__.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.656715 Qube2-0.3.40/qube/booster/app/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/booster/app/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    21047 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/booster/app/boo.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    20152 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/booster/app/reports.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     5511 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/booster/app/signal_viewer.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.656715 Qube2-0.3.40/qube/booster/app/templates/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2559 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/booster/app/templates/detailed_report.html
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1627 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/booster/app/templates/experiment_chart_report.html
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2593 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/booster/app/templates/experiment_report.html
+-rw-r--r--   0 quant0    (1000) quant0    (1000)      754 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/booster/app/templates/experiments_index.html
+-rw-r--r--   0 quant0    (1000) quant0    (1000)      656 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/booster/app/templates/index.html
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2428 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/booster/app/templates/main_report.html
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2536 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/booster/app/templates/signals_viewer.html
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2511 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/booster/app/templates/tearsheet_report.html
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    16074 2024-05-01 15:36:56.000000 Qube2-0.3.40/qube/booster/boosterai.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    46792 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/booster/core.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.656715 Qube2-0.3.40/qube/booster/data/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    13501 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/booster/data/markets.yml
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    14897 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/booster/simctrl.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     5984 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/booster/utils.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.660714 Qube2-0.3.40/qube/charting/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)       35 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/charting/__init__.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.660714 Qube2-0.3.40/qube/charting/highcharts/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/charting/highcharts/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     9714 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/charting/highcharts/core.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2704 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/charting/highcharts/display.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    27021 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/charting/lookinglass.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    29533 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/charting/mpl_finance.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    18006 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/charting/plot_helpers.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.660714 Qube2-0.3.40/qube/configs/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     3943 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/configs/Properties.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/configs/__init__.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.660714 Qube2-0.3.40/qube/configs/config-default/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1388 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/configs/config-default/datasource.json
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    30265 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/configs/config-default/dukas_outlook.csv
+-rw-r--r--   0 quant0    (1000) quant0    (1000)      399 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/configs/config-default/main-props.json
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.660714 Qube2-0.3.40/qube/configs/config-test/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)      720 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/configs/config-test/datasource.json
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    30265 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/configs/config-test/dukas_outlook.csv
+-rw-r--r--   0 quant0    (1000) quant0    (1000)      348 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/configs/config-test/main-props.json
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.660714 Qube2-0.3.40/qube/datasource/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     3025 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/datasource/CsvConnector.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    11829 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/datasource/DataSource.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2947 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/datasource/DataserverConnector.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)      731 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/datasource/DukasOutlookConnector.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1585 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/datasource/InMemoryDataSource.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    12102 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/datasource/KdbConnector.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2132 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/datasource/MongoConnector.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2040 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/datasource/YahooConnector.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)      318 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/datasource/__init__.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.660714 Qube2-0.3.40/qube/datasource/controllers/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     7152 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/datasource/controllers/KdbServerController.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2592 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/datasource/controllers/MemcacheController.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     9283 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/datasource/controllers/MongoController.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/datasource/controllers/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     6343 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/datasource/controllers/kdb_utils.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    13096 2024-03-21 09:37:59.000000 Qube2-0.3.40/qube/datasource/loaders.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.660714 Qube2-0.3.40/qube/examples/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/examples/__init__.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.660714 Qube2-0.3.40/qube/examples/booster/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1166 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/examples/booster/test_portfolio_task.yml
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.660714 Qube2-0.3.40/qube/examples/learn/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/examples/learn/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     4573 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/examples/learn/filters.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    12840 2024-04-28 09:52:57.000000 Qube2-0.3.40/qube/examples/learn/generators.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     4056 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/examples/learn/transformers.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.660714 Qube2-0.3.40/qube/examples/strategies/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/examples/strategies/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    11151 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/examples/strategies/test_strategies.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     7825 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/examples/strategies/turtles.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.660714 Qube2-0.3.40/qube/learn/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)      488 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/learn/__init__.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.660714 Qube2-0.3.40/qube/learn/advanced/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/learn/advanced/__init__.py
+-rw-rw-r--   0 quant0    (1000) quant0    (1000)     9997 2024-03-25 15:09:12.000000 Qube2-0.3.40/qube/learn/advanced/labeling.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.660714 Qube2-0.3.40/qube/learn/core/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/learn/core/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     9903 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/learn/core/base.py
+-rw-rw-r--   0 quant0    (1000) quant0    (1000)     8250 2024-02-01 11:19:00.000000 Qube2-0.3.40/qube/learn/core/data_utils.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     7603 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/learn/core/metrics.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2838 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/learn/core/mlhelpers.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     4375 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/learn/core/operations.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     6278 2024-03-21 09:37:59.000000 Qube2-0.3.40/qube/learn/core/pickers.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)      499 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/learn/core/structs.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     3713 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/learn/core/utils.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.660714 Qube2-0.3.40/qube/portfolio/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)      426 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/portfolio/Instrument.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     6804 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/portfolio/PortfolioLogger.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    18942 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/portfolio/Position.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/portfolio/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     6437 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/portfolio/allocating.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)      480 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/portfolio/broker_constants.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    18671 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/portfolio/commissions.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     5030 2024-03-24 12:41:39.000000 Qube2-0.3.40/qube/portfolio/drawdown.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    28343 2024-03-24 14:11:27.000000 Qube2-0.3.40/qube/portfolio/performance.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.664714 Qube2-0.3.40/qube/portfolio/report_templates/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)      107 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/portfolio/report_templates/comparison_report.tpl
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     3562 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/portfolio/report_templates/old_report.tpl
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2452 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/portfolio/report_templates/optimizer_report.tpl
+-rw-r--r--   0 quant0    (1000) quant0    (1000)      224 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/portfolio/report_templates/signal_statistics_report.tpl
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2794 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/portfolio/report_templates/simple_report.tpl
+-rw-rw-r--   0 quant0    (1000) quant0    (1000)    15023 2024-03-26 13:47:54.000000 Qube2-0.3.40/qube/portfolio/reports.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     5074 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/portfolio/signals_analysis.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.664714 Qube2-0.3.40/qube/quantitative/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)      171 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/quantitative/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1783 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/quantitative/fast_ols.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.664714 Qube2-0.3.40/qube/quantitative/stats/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/quantitative/stats/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    14152 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/quantitative/stats/cointegration.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     6593 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/quantitative/stats/ssa.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     9430 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/quantitative/stats/stats.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.664714 Qube2-0.3.40/qube/quantitative/ta/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/quantitative/ta/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     4030 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/quantitative/ta/bands.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     6037 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/quantitative/ta/dtw.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    63739 2024-03-24 12:41:39.000000 Qube2-0.3.40/qube/quantitative/ta/indicators.py
+-rw-rw-r--   0 quant0    (1000) quant0    (1000)     3983 2024-03-26 13:47:54.000000 Qube2-0.3.40/qube/quantitative/ta/kalman.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     3813 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/quantitative/ta/pewma.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.664714 Qube2-0.3.40/qube/quantitative/ta/swings/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/quantitative/ta/swings/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     7087 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/quantitative/ta/swings/reversals.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    20699 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/quantitative/ta/swings/swings_splitter.py
+-rw-rw-r--   0 quant0    (1000) quant0    (1000)    16592 2024-05-03 11:44:00.000000 Qube2-0.3.40/qube/quantitative/tools.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     6798 2024-03-24 14:11:27.000000 Qube2-0.3.40/qube/qube_nb_magic_init.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.664714 Qube2-0.3.40/qube/series/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)      452 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/series/Bar.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    12186 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/series/BarSeries.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1594 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/series/DoubleSeries.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    23849 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/series/Indicators.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1325 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/series/Quote.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2653 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/series/Series.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/series/__init__.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.664714 Qube2-0.3.40/qube/simulator/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     4555 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/simulator/Brokerage.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    26552 2024-03-24 13:44:39.000000 Qube2-0.3.40/qube/simulator/SignalTester.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)      113 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/simulator/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     3097 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/simulator/backtester.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    10392 2024-03-24 14:11:27.000000 Qube2-0.3.40/qube/simulator/core.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     7620 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/simulator/management.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    10776 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/simulator/multiproc.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    24085 2024-03-24 12:41:39.000000 Qube2-0.3.40/qube/simulator/multisim.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.664714 Qube2-0.3.40/qube/simulator/tracking/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/simulator/tracking/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2925 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/simulator/tracking/sizers.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    48671 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/simulator/tracking/trackers.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    14604 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/simulator/tracking/trailings.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    31999 2024-04-28 09:52:57.000000 Qube2-0.3.40/qube/simulator/utils.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.664714 Qube2-0.3.40/qube/tests/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     7527 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/DateUtils_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/__init__.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.664714 Qube2-0.3.40/qube/tests/booster/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/booster/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     5246 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/booster/booster_test.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.664714 Qube2-0.3.40/qube/tests/data/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    21024 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/data/EURUSD.csv
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     8509 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/data/FDI_test.csv
+-rw-r--r--   0 quant0    (1000) quant0    (1000)      242 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/data/RM1.csv
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/data/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1389 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/data/test_mdf.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.664714 Qube2-0.3.40/qube/tests/datasource/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     4448 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/datasource/DataSource_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2578 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/datasource/KdbConnector_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1092 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/datasource/MemcacheController_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1502 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/datasource/MongoConnector_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    10427 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/datasource/MongoController_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/datasource/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2392 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/ds_test_cfg.json
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.664714 Qube2-0.3.40/qube/tests/learn/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/learn/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     9170 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/learn/base_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     5627 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/learn/scoring_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1091 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/ntp_test.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.664714 Qube2-0.3.40/qube/tests/portfolio/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/portfolio/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2771 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/portfolio/commissions_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2089 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/portfolio/drawdown_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     4458 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/portfolio/portfolio_allocating_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     5449 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/portfolio/portfolio_performance_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1084 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/properties_test.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.668714 Qube2-0.3.40/qube/tests/quantitative/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/quantitative/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    19445 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/quantitative/coint_test.csv
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2226 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/quantitative/cointegration_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1048 2024-03-24 12:41:39.000000 Qube2-0.3.40/qube/tests/quantitative/dtw_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     8038 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/quantitative/indicators_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1735 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/quantitative/kalman_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     2154 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/quantitative/tools_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)       43 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/qube_props_test.json
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.668714 Qube2-0.3.40/qube/tests/series/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     4554 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/series/BarSeries_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     3144 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/series/Indicator_demo_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    20189 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/series/Indicator_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/series/__init__.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.668714 Qube2-0.3.40/qube/tests/simulator/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    10368 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/simulator/Position_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/simulator/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    17897 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/simulator/signal_tester_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     4942 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/simulator/signal_tracker_cloning_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     5696 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/simulator/signal_tracker_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     4563 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/simulator/strategy_tester_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     3743 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/simulator/test_multiproc.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    12994 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/simulator/test_multisim.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    21502 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/simulator/trackers_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     4463 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/simulator/utilities.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    12172 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/simulator/utils_test.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1237 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/tests/utils_for_tests.py
+drwxr-xr-x   0 quant0    (1000) quant0    (1000)        0 2024-05-03 11:45:15.668714 Qube2-0.3.40/qube/utils/
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     8591 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/utils/DateUtils.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1428 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/utils/QubeLogger.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)        0 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/utils/__init__.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     5543 2024-03-24 12:41:39.000000 Qube2-0.3.40/qube/utils/nb_functions.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1890 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/utils/ntp.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1958 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/utils/ui_utils.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)    12709 2024-01-09 18:52:45.000000 Qube2-0.3.40/qube/utils/utils.py
+-rw-r--r--   0 quant0    (1000) quant0    (1000)       38 2024-05-03 11:45:15.668714 Qube2-0.3.40/setup.cfg
+-rw-r--r--   0 quant0    (1000) quant0    (1000)     1529 2024-01-09 19:23:40.000000 Qube2-0.3.40/setup.py
```

### Comparing `Qube2-0.3.39/LICENSE` & `Qube2-0.3.40/LICENSE`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/PKG-INFO` & `Qube2-0.3.40/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Qube2
-Version: 0.3.39
+Version: 0.3.40
 Summary: Qube
 Home-page: https://github.com/dmarienko/Qube
 Author: Dmitry Marienko
 Author-email: dmitry.ema@gmail.com
 Project-URL: Bug Tracker, https://github.com/dmarienko/Qube/issues
 Keywords: quantitative,backtesting,backtester,quantitative finance
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Qube2-0.3.39/Qube2.egg-info/PKG-INFO` & `Qube2-0.3.40/Qube2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Qube2
-Version: 0.3.39
+Version: 0.3.40
 Summary: Qube
 Home-page: https://github.com/dmarienko/Qube
 Author: Dmitry Marienko
 Author-email: dmitry.ema@gmail.com
 Project-URL: Bug Tracker, https://github.com/dmarienko/Qube/issues
 Keywords: quantitative,backtesting,backtester,quantitative finance
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Qube2-0.3.39/Qube2.egg-info/SOURCES.txt` & `Qube2-0.3.40/Qube2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/README.md` & `Qube2-0.3.40/README.md`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/bin/booster` & `Qube2-0.3.40/bin/booster`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/__init__.py` & `Qube2-0.3.40/qube/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from . import quantitative
 from . import charting
 from . import datasource
 from . import utils
 
-__version__ = '0.3.39'
+__version__ = '0.3.40'
 
 from qube.utils.utils import runtime_env
 from cycler import cycler
 
 # reload cython modules
 try:
     from qube.utils.utils import reload_pyx_module
```

### Comparing `Qube2-0.3.39/qube/booster/app/boo.py` & `Qube2-0.3.40/qube/booster/app/boo.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/booster/app/reports.py` & `Qube2-0.3.40/qube/booster/app/reports.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/booster/app/signal_viewer.py` & `Qube2-0.3.40/qube/booster/app/signal_viewer.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/booster/app/templates/detailed_report.html` & `Qube2-0.3.40/qube/booster/app/templates/detailed_report.html`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/booster/app/templates/experiment_chart_report.html` & `Qube2-0.3.40/qube/booster/app/templates/experiment_chart_report.html`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/booster/app/templates/experiment_report.html` & `Qube2-0.3.40/qube/booster/app/templates/experiment_report.html`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/booster/app/templates/experiments_index.html` & `Qube2-0.3.40/qube/booster/app/templates/experiments_index.html`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/booster/app/templates/index.html` & `Qube2-0.3.40/qube/booster/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/booster/app/templates/main_report.html` & `Qube2-0.3.40/qube/booster/app/templates/main_report.html`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/booster/app/templates/signals_viewer.html` & `Qube2-0.3.40/qube/booster/app/templates/signals_viewer.html`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/booster/app/templates/tearsheet_report.html` & `Qube2-0.3.40/qube/booster/app/templates/tearsheet_report.html`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/booster/boosterai.py` & `Qube2-0.3.40/qube/booster/boosterai.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/booster/core.py` & `Qube2-0.3.40/qube/booster/core.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/booster/data/markets.yml` & `Qube2-0.3.40/qube/booster/data/markets.yml`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/booster/simctrl.py` & `Qube2-0.3.40/qube/booster/simctrl.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/booster/utils.py` & `Qube2-0.3.40/qube/booster/utils.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/charting/highcharts/core.py` & `Qube2-0.3.40/qube/charting/highcharts/core.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/charting/highcharts/display.py` & `Qube2-0.3.40/qube/charting/highcharts/display.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/charting/lookinglass.py` & `Qube2-0.3.40/qube/charting/lookinglass.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/charting/mpl_finance.py` & `Qube2-0.3.40/qube/charting/mpl_finance.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/charting/plot_helpers.py` & `Qube2-0.3.40/qube/charting/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/configs/Properties.py` & `Qube2-0.3.40/qube/configs/Properties.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/configs/config-default/datasource.json` & `Qube2-0.3.40/qube/configs/config-default/datasource.json`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/configs/config-default/dukas_outlook.csv` & `Qube2-0.3.40/qube/configs/config-default/dukas_outlook.csv`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/configs/config-test/datasource.json` & `Qube2-0.3.40/qube/configs/config-test/datasource.json`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/configs/config-test/dukas_outlook.csv` & `Qube2-0.3.40/qube/configs/config-test/dukas_outlook.csv`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/datasource/CsvConnector.py` & `Qube2-0.3.40/qube/datasource/CsvConnector.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/datasource/DataSource.py` & `Qube2-0.3.40/qube/datasource/DataSource.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/datasource/DataserverConnector.py` & `Qube2-0.3.40/qube/datasource/DataserverConnector.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/datasource/DukasOutlookConnector.py` & `Qube2-0.3.40/qube/datasource/DukasOutlookConnector.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/datasource/InMemoryDataSource.py` & `Qube2-0.3.40/qube/datasource/InMemoryDataSource.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/datasource/KdbConnector.py` & `Qube2-0.3.40/qube/datasource/KdbConnector.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/datasource/MongoConnector.py` & `Qube2-0.3.40/qube/datasource/MongoConnector.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/datasource/YahooConnector.py` & `Qube2-0.3.40/qube/datasource/YahooConnector.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/datasource/controllers/KdbServerController.py` & `Qube2-0.3.40/qube/datasource/controllers/KdbServerController.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/datasource/controllers/MemcacheController.py` & `Qube2-0.3.40/qube/datasource/controllers/MemcacheController.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/datasource/controllers/MongoController.py` & `Qube2-0.3.40/qube/datasource/controllers/MongoController.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/datasource/controllers/kdb_utils.py` & `Qube2-0.3.40/qube/datasource/controllers/kdb_utils.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/datasource/loaders.py` & `Qube2-0.3.40/qube/datasource/loaders.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/examples/booster/test_portfolio_task.yml` & `Qube2-0.3.40/qube/examples/booster/test_portfolio_task.yml`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/examples/learn/filters.py` & `Qube2-0.3.40/qube/examples/learn/filters.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/examples/learn/generators.py` & `Qube2-0.3.40/qube/examples/learn/generators.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/examples/learn/transformers.py` & `Qube2-0.3.40/qube/examples/learn/transformers.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/examples/strategies/test_strategies.py` & `Qube2-0.3.40/qube/examples/strategies/test_strategies.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/examples/strategies/turtles.py` & `Qube2-0.3.40/qube/examples/strategies/turtles.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/learn/advanced/labeling.py` & `Qube2-0.3.40/qube/learn/advanced/labeling.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/learn/core/base.py` & `Qube2-0.3.40/qube/learn/core/base.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/learn/core/data_utils.py` & `Qube2-0.3.40/qube/learn/core/data_utils.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/learn/core/metrics.py` & `Qube2-0.3.40/qube/learn/core/metrics.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/learn/core/mlhelpers.py` & `Qube2-0.3.40/qube/learn/core/mlhelpers.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/learn/core/operations.py` & `Qube2-0.3.40/qube/learn/core/operations.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/learn/core/pickers.py` & `Qube2-0.3.40/qube/learn/core/pickers.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/learn/core/utils.py` & `Qube2-0.3.40/qube/learn/core/utils.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/portfolio/PortfolioLogger.py` & `Qube2-0.3.40/qube/portfolio/PortfolioLogger.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/portfolio/Position.py` & `Qube2-0.3.40/qube/portfolio/Position.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/portfolio/allocating.py` & `Qube2-0.3.40/qube/portfolio/allocating.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/portfolio/commissions.py` & `Qube2-0.3.40/qube/portfolio/commissions.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/portfolio/drawdown.py` & `Qube2-0.3.40/qube/portfolio/drawdown.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/portfolio/performance.py` & `Qube2-0.3.40/qube/portfolio/performance.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/portfolio/report_templates/old_report.tpl` & `Qube2-0.3.40/qube/portfolio/report_templates/old_report.tpl`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/portfolio/report_templates/optimizer_report.tpl` & `Qube2-0.3.40/qube/portfolio/report_templates/optimizer_report.tpl`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/portfolio/report_templates/simple_report.tpl` & `Qube2-0.3.40/qube/portfolio/report_templates/simple_report.tpl`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/portfolio/reports.py` & `Qube2-0.3.40/qube/portfolio/reports.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/portfolio/signals_analysis.py` & `Qube2-0.3.40/qube/portfolio/signals_analysis.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/quantitative/fast_ols.py` & `Qube2-0.3.40/qube/quantitative/fast_ols.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/quantitative/stats/cointegration.py` & `Qube2-0.3.40/qube/quantitative/stats/cointegration.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/quantitative/stats/ssa.py` & `Qube2-0.3.40/qube/quantitative/stats/ssa.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/quantitative/stats/stats.py` & `Qube2-0.3.40/qube/quantitative/stats/stats.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/quantitative/ta/bands.py` & `Qube2-0.3.40/qube/quantitative/ta/bands.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/quantitative/ta/dtw.py` & `Qube2-0.3.40/qube/quantitative/ta/dtw.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/quantitative/ta/indicators.py` & `Qube2-0.3.40/qube/quantitative/ta/indicators.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/quantitative/ta/kalman.py` & `Qube2-0.3.40/qube/quantitative/ta/kalman.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/quantitative/ta/pewma.py` & `Qube2-0.3.40/qube/quantitative/ta/pewma.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/quantitative/ta/swings/reversals.py` & `Qube2-0.3.40/qube/quantitative/ta/swings/reversals.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/quantitative/ta/swings/swings_splitter.py` & `Qube2-0.3.40/qube/quantitative/ta/swings/swings_splitter.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/quantitative/tools.py` & `Qube2-0.3.40/qube/quantitative/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -495,19 +495,20 @@
     values = np.array(sorted([(x.total_seconds()) for x in np.diff(times_index)]))
     diff = np.concatenate(([1], np.diff(values)))
     idx = np.concatenate((np.where(diff)[0], [len(values)]))
     freqs = dict(zip(values[idx[:-1]], np.diff(idx)))
     return timedelta(seconds=max(freqs, key=freqs.get))
 
 
-def continuous_periods(xs, cond):
+def continuous_periods(xs: pd.Series, cond) -> mstruct:
     """
     Detect continues periods on series xs based on condition cond
     """
     df = scols(xs, cond, keys=['_XS_', 'sig'])
     df['block'] = (df.sig.shift(1) != df.sig).astype(int).cumsum()
+    idx_col_name = xs.index.name
 
-    blk = df[df.sig].reset_index().groupby('block')['time'].apply(np.array)
+    blk = df[df.sig].reset_index().groupby('block')[idx_col_name].apply(np.array)
     starts = blk.apply(lambda x: x[0])
     ends = blk.apply(lambda x: x[-1])
     se_info = scols(starts, ends, keys=['start', 'end'])
     return mstruct(blocks=blk.reset_index(drop=True), periods=se_info)
```

### Comparing `Qube2-0.3.39/qube/qube_nb_magic_init.py` & `Qube2-0.3.40/qube/qube_nb_magic_init.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/series/BarSeries.py` & `Qube2-0.3.40/qube/series/BarSeries.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/series/DoubleSeries.py` & `Qube2-0.3.40/qube/series/DoubleSeries.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/series/Indicators.py` & `Qube2-0.3.40/qube/series/Indicators.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/series/Quote.py` & `Qube2-0.3.40/qube/series/Quote.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/series/Series.py` & `Qube2-0.3.40/qube/series/Series.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/simulator/Brokerage.py` & `Qube2-0.3.40/qube/simulator/Brokerage.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/simulator/SignalTester.py` & `Qube2-0.3.40/qube/simulator/SignalTester.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/simulator/backtester.py` & `Qube2-0.3.40/qube/simulator/backtester.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/simulator/core.py` & `Qube2-0.3.40/qube/simulator/core.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/simulator/management.py` & `Qube2-0.3.40/qube/simulator/management.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/simulator/multiproc.py` & `Qube2-0.3.40/qube/simulator/multiproc.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/simulator/multisim.py` & `Qube2-0.3.40/qube/simulator/multisim.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/simulator/tracking/sizers.py` & `Qube2-0.3.40/qube/simulator/tracking/sizers.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/simulator/tracking/trackers.py` & `Qube2-0.3.40/qube/simulator/tracking/trackers.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/simulator/tracking/trailings.py` & `Qube2-0.3.40/qube/simulator/tracking/trailings.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/simulator/utils.py` & `Qube2-0.3.40/qube/simulator/utils.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/DateUtils_test.py` & `Qube2-0.3.40/qube/tests/DateUtils_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/booster/booster_test.py` & `Qube2-0.3.40/qube/tests/booster/booster_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/data/EURUSD.csv` & `Qube2-0.3.40/qube/tests/data/EURUSD.csv`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/data/FDI_test.csv` & `Qube2-0.3.40/qube/tests/data/FDI_test.csv`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/data/test_mdf.py` & `Qube2-0.3.40/qube/tests/data/test_mdf.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/datasource/DataSource_test.py` & `Qube2-0.3.40/qube/tests/datasource/DataSource_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/datasource/KdbConnector_test.py` & `Qube2-0.3.40/qube/tests/datasource/KdbConnector_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/datasource/MemcacheController_test.py` & `Qube2-0.3.40/qube/tests/datasource/MemcacheController_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/datasource/MongoConnector_test.py` & `Qube2-0.3.40/qube/tests/datasource/MongoConnector_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/datasource/MongoController_test.py` & `Qube2-0.3.40/qube/tests/datasource/MongoController_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/ds_test_cfg.json` & `Qube2-0.3.40/qube/tests/ds_test_cfg.json`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/learn/base_test.py` & `Qube2-0.3.40/qube/tests/learn/base_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/learn/scoring_test.py` & `Qube2-0.3.40/qube/tests/learn/scoring_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/ntp_test.py` & `Qube2-0.3.40/qube/tests/ntp_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/portfolio/commissions_test.py` & `Qube2-0.3.40/qube/tests/portfolio/commissions_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/portfolio/drawdown_test.py` & `Qube2-0.3.40/qube/tests/portfolio/drawdown_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/portfolio/portfolio_allocating_test.py` & `Qube2-0.3.40/qube/tests/portfolio/portfolio_allocating_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/portfolio/portfolio_performance_test.py` & `Qube2-0.3.40/qube/tests/portfolio/portfolio_performance_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/properties_test.py` & `Qube2-0.3.40/qube/tests/properties_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/quantitative/coint_test.csv` & `Qube2-0.3.40/qube/tests/quantitative/coint_test.csv`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/quantitative/cointegration_test.py` & `Qube2-0.3.40/qube/tests/quantitative/cointegration_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/quantitative/dtw_test.py` & `Qube2-0.3.40/qube/tests/quantitative/dtw_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/quantitative/indicators_test.py` & `Qube2-0.3.40/qube/tests/quantitative/indicators_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/quantitative/kalman_test.py` & `Qube2-0.3.40/qube/tests/quantitative/kalman_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/quantitative/tools_test.py` & `Qube2-0.3.40/qube/tests/quantitative/tools_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/series/BarSeries_test.py` & `Qube2-0.3.40/qube/tests/series/BarSeries_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/series/Indicator_demo_test.py` & `Qube2-0.3.40/qube/tests/series/Indicator_demo_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/series/Indicator_test.py` & `Qube2-0.3.40/qube/tests/series/Indicator_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/simulator/Position_test.py` & `Qube2-0.3.40/qube/tests/simulator/Position_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/simulator/signal_tester_test.py` & `Qube2-0.3.40/qube/tests/simulator/signal_tester_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/simulator/signal_tracker_cloning_test.py` & `Qube2-0.3.40/qube/tests/simulator/signal_tracker_cloning_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/simulator/signal_tracker_test.py` & `Qube2-0.3.40/qube/tests/simulator/signal_tracker_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/simulator/strategy_tester_test.py` & `Qube2-0.3.40/qube/tests/simulator/strategy_tester_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/simulator/test_multiproc.py` & `Qube2-0.3.40/qube/tests/simulator/test_multiproc.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/simulator/test_multisim.py` & `Qube2-0.3.40/qube/tests/simulator/test_multisim.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/simulator/trackers_test.py` & `Qube2-0.3.40/qube/tests/simulator/trackers_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/simulator/utilities.py` & `Qube2-0.3.40/qube/tests/simulator/utilities.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/simulator/utils_test.py` & `Qube2-0.3.40/qube/tests/simulator/utils_test.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/tests/utils_for_tests.py` & `Qube2-0.3.40/qube/tests/utils_for_tests.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/utils/DateUtils.py` & `Qube2-0.3.40/qube/utils/DateUtils.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/utils/QubeLogger.py` & `Qube2-0.3.40/qube/utils/QubeLogger.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/utils/nb_functions.py` & `Qube2-0.3.40/qube/utils/nb_functions.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/utils/ntp.py` & `Qube2-0.3.40/qube/utils/ntp.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/utils/ui_utils.py` & `Qube2-0.3.40/qube/utils/ui_utils.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/qube/utils/utils.py` & `Qube2-0.3.40/qube/utils/utils.py`

 * *Files identical despite different names*

### Comparing `Qube2-0.3.39/setup.py` & `Qube2-0.3.40/setup.py`

 * *Files identical despite different names*


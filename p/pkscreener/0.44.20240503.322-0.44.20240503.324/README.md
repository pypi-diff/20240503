# Comparing `tmp/pkscreener-0.44.20240503.322.tar.gz` & `tmp/pkscreener-0.44.20240503.324.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240503.322.tar", last modified: Fri May  3 05:42:21 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240503.324.tar", last modified: Fri May  3 10:34:00 2024, max compression
```

## Comparing `pkscreener-0.44.20240503.322.tar` & `pkscreener-0.44.20240503.324.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 05:42:21.000875 pkscreener-0.44.20240503.322/
--rw-rw-rw-   0        0        0     1086 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-03 05:42:21.000875 pkscreener-0.44.20240503.322/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 05:42:20.985280 pkscreener-0.44.20240503.322/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 05:42:21.000875 pkscreener-0.44.20240503.322/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25810 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7496 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29461 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    22090 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    20814 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8124 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   119213 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    52127 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    82304 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-03 05:42:11.000000 pkscreener-0.44.20240503.322/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   123825 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/globals.py
--rw-rw-rw-   0        0        0      595 2024-05-03 05:38:10.000000 pkscreener-0.44.20240503.322/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    42912 2024-05-03 05:38:10.000000 pkscreener-0.44.20240503.322/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    26382 2024-05-03 05:38:10.000000 pkscreener-0.44.20240503.322/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-03 05:42:20.985280 pkscreener-0.44.20240503.322/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-03 05:42:20.000000 pkscreener-0.44.20240503.322/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-05-03 05:42:20.000000 pkscreener-0.44.20240503.322/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 05:42:20.000000 pkscreener-0.44.20240503.322/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-03 05:42:20.000000 pkscreener-0.44.20240503.322/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-03 05:42:20.000000 pkscreener-0.44.20240503.322/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-03 05:42:20.000000 pkscreener-0.44.20240503.322/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-03 05:42:21.000875 pkscreener-0.44.20240503.322/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-05-03 05:38:10.000000 pkscreener-0.44.20240503.322/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 10:34:00.867843 pkscreener-0.44.20240503.324/
+-rw-rw-rw-   0        0        0     1086 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-03 10:34:00.867843 pkscreener-0.44.20240503.324/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 10:34:00.852244 pkscreener-0.44.20240503.324/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 10:34:00.867843 pkscreener-0.44.20240503.324/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    25810 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7690 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29461 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    22090 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    20814 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8126 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   119213 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    52127 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    82304 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-03 10:33:51.000000 pkscreener-0.44.20240503.324/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   123825 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      595 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    42912 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    26382 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-03 10:34:00.852244 pkscreener-0.44.20240503.324/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-03 10:34:00.000000 pkscreener-0.44.20240503.324/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-05-03 10:34:00.000000 pkscreener-0.44.20240503.324/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 10:34:00.000000 pkscreener-0.44.20240503.324/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-03 10:34:00.000000 pkscreener-0.44.20240503.324/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-03 10:34:00.000000 pkscreener-0.44.20240503.324/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-03 10:34:00.000000 pkscreener-0.44.20240503.324/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-03 10:34:00.867843 pkscreener-0.44.20240503.324/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-05-03 10:29:30.000000 pkscreener-0.44.20240503.324/setup.py
```

### Comparing `pkscreener-0.44.20240503.322/LICENSE` & `pkscreener-0.44.20240503.324/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/LICENSE-Others` & `pkscreener-0.44.20240503.324/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/PKG-INFO` & `pkscreener-0.44.20240503.324/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240503.322
+Version: 0.44.20240503.324
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240503.322.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240503.324.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.319/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240503.322/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.319/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240503.322/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.319/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240503.322/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240503.322/README.md` & `pkscreener-0.44.20240503.324/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.319/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240503.322/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.319/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240503.322/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.319/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240503.322/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240503.322/pkscreener/__init__.py` & `pkscreener-0.44.20240503.324/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/MarketMonitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 """
 import sys
 import pandas as pd
 import numpy as np
 from PKDevTools.classes.Singleton import SingletonType, SingletonMixin
 from PKDevTools.classes.OutputControls import OutputControls
 from PKDevTools.classes.ColorText import colorText
-from pkscreener.classes import Utility
 
 class MarketMonitor(SingletonMixin, metaclass=SingletonType):
     def __init__(self,monitors=[], maxNumResultsPerRow=5,maxNumColsInEachResult=6,maxNumRowsInEachResult=10):
         super(MarketMonitor, self).__init__()
         if monitors is not None and len(monitors) > 0:
             self.monitors = monitors
             self.monitorIndex = 0
@@ -78,14 +77,17 @@
         highlightCols = []
         if screen_df is None or screen_df.empty:
             return
 
         screen_monitor_df = screen_df.copy()
         screen_monitor_df.reset_index(inplace=True)
         screen_monitor_df = screen_monitor_df[["Stock", "LTP", "%Chng","52Wk H","RSI/i","Volume"]].head(self.maxNumRowsInEachResult-1)
+        # Import Utility here since Utility has dependency on PKScheduler which in turn has dependency on 
+        # multiprocessing, which behaves erratically if imported at the top.
+        from pkscreener.classes import Utility
         screen_monitor_df.loc[:, "%Chng"] = screen_monitor_df.loc[:, "%Chng"].apply(
                     lambda x: Utility.tools.roundOff(str(x).split("% (")[0] + colorText.END,0)
                 )
         screen_monitor_df.loc[:, "52Wk H"] = screen_monitor_df.loc[:, "52Wk H"].apply(
             lambda x: Utility.tools.roundOff(x,0)
         )
         screen_monitor_df.loc[:, "Volume"] = screen_monitor_df.loc[:, "Volume"].apply(
```

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/PKScheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,33 +24,34 @@
 """
 import warnings
 import os
 import sys
 import time
 warnings.simplefilter("ignore", UserWarning,append=True)
 os.environ["PYTHONWARNINGS"]="ignore::UserWarning"
+
+def init_pool_processes(the_lock):
+    '''Initialize each process with a global variable lock.
+    '''
+    global lock
+    lock = the_lock
+
 import multiprocessing
 from multiprocessing import Lock
 
 # from time import sleep
 from concurrent.futures import ProcessPoolExecutor
 from rich.progress import Progress, BarColumn, TimeRemainingColumn, TimeElapsedColumn
 from rich.console import Console
 from rich.control import Control
 from rich.segment import ControlType
 from pkscreener.classes.PKTask import PKTask
 
 multiprocessing.freeze_support()
 
-def init_pool_processes(the_lock):
-    '''Initialize each process with a global variable lock.
-    '''
-    global lock
-    lock = the_lock
-
 # def long_running_fn(*args, **kwargs):
 #     len_of_task = random.randint(3, 20000)  # take some random length of time
 #     task = args[0]
 #     progress = task.progressStatusDict
 #     task_id = task.taskId
 #     for n in range(0, len_of_task):
 #         # sleep(1)  # sleep for a bit to simulate work
```

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/classes/keys.py` & `pkscreener-0.44.20240503.324/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/courbd.ttf` & `pkscreener-0.44.20240503.324/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/globals.py` & `pkscreener-0.44.20240503.324/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240503.324/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240503.324/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240503.324/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240503.324/pkscreener.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240503.322
+Version: 0.44.20240503.324
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240503.322.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240503.324.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.319/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240503.322/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.319/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240503.322/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.319/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240503.322/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240503.322/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240503.324/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.322/setup.py` & `pkscreener-0.44.20240503.324/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/pkscreener-0.44.20240502.318.tar.gz` & `tmp/pkscreener-0.44.20240503.322.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240502.318.tar", last modified: Thu May  2 12:49:51 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240503.322.tar", last modified: Fri May  3 05:42:21 2024, max compression
```

## Comparing `pkscreener-0.44.20240502.318.tar` & `pkscreener-0.44.20240503.322.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 12:49:51.615947 pkscreener-0.44.20240502.318/
--rw-rw-rw-   0        0        0     1086 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-02 12:49:51.615947 pkscreener-0.44.20240502.318/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 12:49:51.584700 pkscreener-0.44.20240502.318/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:49:51.600322 pkscreener-0.44.20240502.318/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25810 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7496 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29455 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    21093 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    20691 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8124 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   117763 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    52127 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    82304 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-02 12:49:42.000000 pkscreener-0.44.20240502.318/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   123422 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/globals.py
--rw-rw-rw-   0        0        0      595 2024-05-02 12:44:28.000000 pkscreener-0.44.20240502.318/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    42912 2024-05-02 12:44:28.000000 pkscreener-0.44.20240502.318/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    25897 2024-05-02 12:44:28.000000 pkscreener-0.44.20240502.318/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:49:51.600322 pkscreener-0.44.20240502.318/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-02 12:49:51.000000 pkscreener-0.44.20240502.318/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-05-02 12:49:51.000000 pkscreener-0.44.20240502.318/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 12:49:51.000000 pkscreener-0.44.20240502.318/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-02 12:49:51.000000 pkscreener-0.44.20240502.318/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-02 12:49:51.000000 pkscreener-0.44.20240502.318/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-02 12:49:51.000000 pkscreener-0.44.20240502.318/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-02 12:49:51.615947 pkscreener-0.44.20240502.318/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-05-02 12:44:28.000000 pkscreener-0.44.20240502.318/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 05:42:21.000875 pkscreener-0.44.20240503.322/
+-rw-rw-rw-   0        0        0     1086 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-03 05:42:21.000875 pkscreener-0.44.20240503.322/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 05:42:20.985280 pkscreener-0.44.20240503.322/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 05:42:21.000875 pkscreener-0.44.20240503.322/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    25810 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7496 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29461 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    22090 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    20814 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8124 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   119213 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    52127 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    82304 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-03 05:42:11.000000 pkscreener-0.44.20240503.322/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   123825 2024-05-03 05:38:09.000000 pkscreener-0.44.20240503.322/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      595 2024-05-03 05:38:10.000000 pkscreener-0.44.20240503.322/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    42912 2024-05-03 05:38:10.000000 pkscreener-0.44.20240503.322/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    26382 2024-05-03 05:38:10.000000 pkscreener-0.44.20240503.322/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-03 05:42:20.985280 pkscreener-0.44.20240503.322/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-03 05:42:20.000000 pkscreener-0.44.20240503.322/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-05-03 05:42:20.000000 pkscreener-0.44.20240503.322/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 05:42:20.000000 pkscreener-0.44.20240503.322/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-03 05:42:20.000000 pkscreener-0.44.20240503.322/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-03 05:42:20.000000 pkscreener-0.44.20240503.322/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-03 05:42:20.000000 pkscreener-0.44.20240503.322/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-03 05:42:21.000875 pkscreener-0.44.20240503.322/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-05-03 05:38:10.000000 pkscreener-0.44.20240503.322/setup.py
```

### Comparing `pkscreener-0.44.20240502.318/LICENSE` & `pkscreener-0.44.20240503.322/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/LICENSE-Others` & `pkscreener-0.44.20240503.322/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/PKG-INFO` & `pkscreener-0.44.20240503.322/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240502.318
+Version: 0.44.20240503.322
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240502.318.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240503.322.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.317/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.319/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.317/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.319/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.317/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.319/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240502.318/README.md` & `pkscreener-0.44.20240503.322/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.317/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.319/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.317/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.319/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.317/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.319/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240502.318/pkscreener/__init__.py` & `pkscreener-0.44.20240503.322/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/MenuOptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,15 @@
 # This Class manages application menus
 class menus:
     
     @staticmethod
     def allMenus(topLevel="X",index=12):
         menuOptions = [topLevel]
         indexOptions =[index]
-        scanOptions = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,23,24,25]
+        scanOptions = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,23,24,25,27,28]
         scanSubOptions = {
                             6:[1,2,3,4,5,6,{7:[1,2]},8,9],
                             7:[1,2,{3:[1,2]},4,5,{6:[1,3]},7],
                             # 21:[3,5,6,7,8,9]
                          }
         runOptions = []
         for menuOption in menuOptions:
```

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files 4% similar despite different names*

```diff
@@ -262,26 +262,30 @@
     def diffMorningCandleDataWithLatestDailyCandleData(screen_df,save_df, updatedCandleData, allDailyCandles,runOptionName=None):
         save_df.reset_index(inplace=True)
         screen_df.reset_index(inplace=True)
         save_df.drop(f"index", axis=1, inplace=True, errors="ignore")
         screen_df.drop(f"index", axis=1, inplace=True, errors="ignore")
         stocks = save_df["Stock"]
         eodLTPs = []
+        dayHighLTPs = []
         morningTimestamps = []
         sellTimestamps = []
+        dayHighTimestamps = []
         sellLTPs = []
         eodDiffs = []
+        dayHighDiffs = []
         sqrOffDiffs = []
         index = 0
         scrStats = ScreeningStatistics(PKMarketOpenCloseAnalyser.configManager, default_logger())
         for stock in stocks:
             try:
                 # Open, High, Low, Close, Adj Close, Volume. We need the 3rd index item: Close.
+                dayHighLTP = allDailyCandles[stock]["data"][-1][1]
                 endOfDayLTP = allDailyCandles[stock]["data"][-1][3]
-                morningLTP = updatedCandleData[stock]["data"][-1][3] #round(save_df["LTP"][index],2)
+                morningLTP = updatedCandleData[stock]["data"][-1][3] or round(save_df["LTP"][index],2)
                 morningTime = updatedCandleData[stock]["index"][-1].strftime("%H:%M")
                 morningTimestamps.append(morningTime)
                 morningCandles = PKMarketOpenCloseAnalyser.allIntradayCandles
                 df = pd.DataFrame(data=morningCandles[stock]["data"],
                                 columns=morningCandles[stock]["columns"],
                                 index=morningCandles[stock]["index"])
                 # try:
@@ -290,55 +294,64 @@
                 # except:
                 #     df = df[df.index >=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+PKMarketOpenCloseAnalyser.configManager.morninganalysiscandlenumber}:00+05:30', utc=True)]
                 #     pass
                 ts, row = scrStats.findMACDCrossover(df=df,
                                            afterTimestamp=updatedCandleData[stock]["index"][-1],
                                            nthCrossover=1,
                                            upDirection=True)
+                highTS, highRow = scrStats.findIntradayHighCrossover(df=df)
                 sellTimestamps.append(ts.strftime("%H:%M"))
+                dayHighTimestamps.append(highTS.strftime("%H:%M"))
                 sellLTPs.append(row["High"][-1])
                 eodLTPs.append(round(endOfDayLTP,2))
+                dayHighLTPs.append(round(dayHighLTP,2))
                 eodDiffs.append(round(endOfDayLTP - morningLTP,2))
+                dayHighDiffs.append(round(dayHighLTP - morningLTP,2))
                 sqrOffDiffs.append(round(row["High"][-1] - morningLTP,2))
                 index += 1
             except:
                 eodLTPs.append("0")
                 eodDiffs.append("0")
+                dayHighLTPs.append("0")
+                dayHighDiffs.append("0")
                 continue
-        diffColumns = ["AlertTime", "SqrOff", "SqrOffLTP", "SqrOffDiff", "EoDLTP", "EoDDiff"]
-        diffValues = [morningTimestamps, sellTimestamps, sellLTPs, sqrOffDiffs,eodLTPs, eodDiffs]
+        diffColumns = ["AlertTime", "SqrOff", "SqrOffLTP", "SqrOffDiff","DayHighTime","DayHigh","DayHighDiff", "EoDLTP", "EoDDiff"]
+        diffValues = [morningTimestamps, sellTimestamps, sellLTPs, sqrOffDiffs,dayHighTimestamps,dayHighLTPs, dayHighDiffs,eodLTPs, eodDiffs]
         for col in diffColumns:
             save_df[col] = diffValues[diffColumns.index(col)]
             screen_df.loc[:, col] = save_df.loc[:, col].apply(
-                lambda x: x if col in ["AlertTime", "SqrOff", "SqrOffLTP", "EoDLTP"] else ((colorText.GREEN if x >= 0 else colorText.FAIL) + str(x) + colorText.END)
+                lambda x: x if col in ["AlertTime", "SqrOff", "SqrOffLTP", "EoDLTP","DayHigh","DayHighTime"] else ((colorText.GREEN if x >= 0 else colorText.FAIL) + str(x) + colorText.END)
             )
 
         columns = save_df.columns
         lastIndex = len(save_df)
         for col in columns:
-            if col in ["Stock", "Pattern", "LTP", "SqrOffLTP","SqrOffDiff","AlertTime", "EoDLTP", "EoDDiff", "%Chng"]:
+            if col in ["Stock", "Pattern", "LTP", "SqrOffLTP","SqrOffDiff","DayHigh","DayHighDiff","AlertTime", "EoDLTP", "EoDDiff", "%Chng"]:
                 if col == "Stock":
                     save_df.loc[lastIndex,col] = "PORTFOLIO"
                 elif col == "Pattern":
                     save_df.loc[lastIndex,col] = runOptionName if runOptionName is not None else ""
-                elif col in ["LTP", "SqrOffLTP","SqrOffDiff", "EoDLTP", "EoDDiff"]:
+                elif col in ["LTP", "SqrOffLTP","SqrOffDiff", "EoDLTP", "EoDDiff","DayHigh","DayHighDiff"]:
                     save_df.loc[lastIndex,col] = round(sum(save_df[col].dropna(inplace=False).astype(float)),2)
                 elif col == "%Chng":
                     ltpSum = sum(save_df["LTP"].dropna(inplace=False).astype(float))
                     change_pct = sum(save_df["EoDDiff"].dropna(inplace=False).astype(float))*100/ltpSum
                     save_df.loc[lastIndex,col] = f"{round(2*change_pct,2)}%" # when summing above for LTP, the total of LTP gets summed up too. Hence *2 here.
             else:
                 save_df.loc[lastIndex,col] = ""
             screen_df.loc[lastIndex,col] = save_df.loc[lastIndex,col]
         eodDiff = save_df.loc[lastIndex,"EoDDiff"]
         sqrOffDiff = save_df.loc[lastIndex,"SqrOffDiff"]
+        dayHighDiff = save_df.loc[lastIndex,"DayHighDiff"]
         save_df.loc[lastIndex,"EoDDiff"] = str(eodDiff) + f'({round(100*2*eodDiff/ltpSum,2)}%)'
         save_df.loc[lastIndex,"SqrOffDiff"] = str(sqrOffDiff) + f'({round(100*2*sqrOffDiff/ltpSum,2)}%)'
+        save_df.loc[lastIndex,"DayHighDiff"] = str(dayHighDiff) + f'({round(100*2*dayHighDiff/ltpSum,2)}%)'
         screen_df.loc[lastIndex,"EoDDiff"] = (colorText.GREEN if eodDiff >= 0 else colorText.FAIL) + save_df.loc[lastIndex,"EoDDiff"] + colorText.END
         screen_df.loc[lastIndex,"SqrOffDiff"] = (colorText.GREEN if sqrOffDiff >= 0 else colorText.FAIL) + save_df.loc[lastIndex,"SqrOffDiff"] + colorText.END
+        screen_df.loc[lastIndex,"DayHighDiff"] = (colorText.GREEN if dayHighDiff >= 0 else colorText.FAIL) + save_df.loc[lastIndex,"DayHighDiff"] + colorText.END
         save_df.set_index("Stock", inplace=True)
         screen_df.set_index("Stock", inplace=True)
         PKMarketOpenCloseAnalyser.allIntradayCandles = None
         if 'index' in save_df.columns:
             save_df.drop('index', axis=1, inplace=True, errors="ignore")
         if 'index' in screen_df.columns:
             screen_df.drop('index', axis=1, inplace=True, errors="ignore")
```

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/PKScanRunner.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,15 +277,15 @@
                     screenResults,
                     saveResults,
                     backtest_df,
                     testing=testing,
                 )
 
         OutputControls().printOutput(colorText.END)
-        if userPassedArgs is not None and (userPassedArgs.monitor is None and "|" not in userPassedArgs.options):
+        if userPassedArgs is not None and (userPassedArgs.monitor is None and "|" not in userPassedArgs.options) and not userPassedArgs.options.upper().startswith("C"):
             # Don't terminate the multiprocessing clients if we're 
             # going to pipe the results from an earlier run
             # or we're running in monitoring mode
             PKScanRunner.terminateAllWorkers(consumers, tasks_queue, testing)
         return screenResults, saveResults,backtest_df,tasks_queue, results_queue, consumers, logging_queue
 
     def prepareToRunScan(menuOption,keyboardInterruptEvent, screenCounter, screenResultsCounter, stockDictPrimary,stockDictSecondary, items):
@@ -345,29 +345,30 @@
             sys.stdout.write(f"{round(time.time() - start_time)}.")
             worker.daemon = True
             worker.start()
         OutputControls().printOutput(f"Started all workers in {round(time.time() - start_time,4)}s")
         if OutputControls().enableMultipleLineOutput:
             sys.stdout.write("\x1b[1A")
 
-    def terminateAllWorkers(consumers, tasks_queue, testing):
+    def terminateAllWorkers(consumers, tasks_queue, testing=False):
         # Exit all processes. Without this, it threw error in next screening session
         for worker in consumers:
             try:
                 if testing: # pragma: no cover
                     if sys.platform.startswith("win"):
                         import signal
 
                         signal.signal(signal.SIGBREAK, PKScanRunner.shutdown)
                         sleep(1)
                     # worker.join()  # necessary so that the Process exists before the test suite exits (thus coverage is collected)
                 # else:
                 # try:
                     # while worker.is_alive():
                 worker.terminate()
+                default_logger().debug("Worker terminated!")
                 # except:
                 #     continue
             except OSError as e: # pragma: no cover
                 default_logger().debug(e, exc_info=True)
                 # if e.winerror == 5:
                 continue
```

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/ScreeningStatistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -745,14 +745,37 @@
             if filter not in [2,4]: # SqZ/All
                 return False
             screenDict["Pattern"] = f'{saved[0]}{colorText.BOLD}{colorText.WARN}TTM-SQZ{colorText.END}'
             saveDict["Pattern"] = f'{saved[1]}TTM-SQZ'
             return True
         return False
 
+    def findIntradayHighCrossover(self, df, afterTimestamp=None):
+        if df is None or len(df) == 0:
+            return False
+        data = df.copy()
+        data = data.fillna(0)
+        data = data.replace([np.inf, -np.inf], 0)
+        data = data[::-1]  # Reverse the dataframe so that its the oldest date first
+        diff_df = None
+        try:
+            # Let's only consider those candles that are after the alert issue-time in the mornings + 2 candles (for buy/sell)
+            diff_df = data[data.index >=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+self.configManager.morninganalysiscandlenumber + 2}:00+05:30').to_datetime64()]
+            # brokerSqrOfftime = pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 15:14:00+05:30').to_datetime64()
+        except:
+            diff_df = data[data.index >=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+self.configManager.morninganalysiscandlenumber + 2}:00+05:30', utc=True)]
+            # brokerSqrOfftime = pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 15:14:00+05:30', utc=True)
+            pass
+        dayHighAfterAlert = diff_df["High"].max()
+        highRow = diff_df[diff_df["High"] >= dayHighAfterAlert]
+        if highRow is not None and len(highRow) > 0:
+            highRow = highRow.tail(1)
+        return highRow.index[-1], highRow
+
+
     def findMACDCrossover(self, df, afterTimestamp=None, nthCrossover=1, upDirection=True, minRSI=60):
         if df is None or len(df) == 0:
             return False
         data = df.copy()
         data = data.fillna(0)
         data = data.replace([np.inf, -np.inf], 0)
         data = data[::-1]  # Reverse the dataframe so that its the oldest date first
```

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/classes/keys.py` & `pkscreener-0.44.20240503.322/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/courbd.ttf` & `pkscreener-0.44.20240503.322/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/globals.py` & `pkscreener-0.44.20240503.322/pkscreener/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -585,14 +585,16 @@
                 pass
             screenResults.sort_values(by=sortKey, ascending=ascending, inplace=True)
             saveResults.sort_values(by=sortKey, ascending=ascending, inplace=True)
         except Exception as e:
             default_logger().debug(e, exc_info=True)
             pass
         columnsToBeDeleted = ["MFI","FVDiff","ConfDMADifference","bbands_ulr_ratio_max5", "RSIi"]
+        if userPassedArgs is not None and userPassedArgs.options is not None and userPassedArgs.options.upper().startswith("C"):
+            columnsToBeDeleted.append("FairValue")
         for column in columnsToBeDeleted:
             if column in saveResults.columns:
                 saveResults.drop(column, axis=1, inplace=True, errors="ignore")
                 screenResults.drop(column, axis=1, inplace=True, errors="ignore")
         if "Stock" in screenResults.columns:
             screenResults.set_index("Stock", inplace=True)
         if "Stock" in saveResults.columns:
@@ -636,14 +638,19 @@
     options, menuOption, indexOption, executeOption = getTopLevelMenuChoices(
         options, False, False, defaultAnswer='Y'
     )
     listStockCodes = prepareStocksForScreening(testing=False, downloadOnly=False, listStockCodes=None,indexOption=indexOption)
     stockDictPrimary,stockDictSecondary = loadDatabaseOrFetch(downloadOnly=False, listStockCodes=listStockCodes, menuOption=menuOption,indexOption=indexOption)
     PKScanRunner.refreshDatabase(consumers,stockDictPrimary,stockDictSecondary)
 
+def closeWorkersAndExit():
+    global consumers, tasks_queue
+    if consumers is not None:
+        PKScanRunner.terminateAllWorkers(consumers, tasks_queue)
+    
 # @tracelog
 def main(userArgs=None,optionalFinalOutcome_df=None):
     global mp_manager, listStockCodes, screenResults, selectedChoice, defaultAnswer, menuChoiceHierarchy, screenCounter, screenResultsCounter, stockDictPrimary, stockDictSecondary, userPassedArgs, loadedStockData, keyboardInterruptEvent, loadCount, maLength, newlyListedOnly, keyboardInterruptEventFired,strategyFilter, elapsed_time, start_time
     selectedChoice = {"0": "", "1": "", "2": "", "3": "", "4": ""}
     elapsed_time = 0
     start_time = 0
     testing = False if userArgs is None else (userArgs.testbuild and userArgs.prodbuild)
@@ -1199,15 +1206,15 @@
                 actualHistoricalDuration = samplingDuration - fillerPlaceHolder
                 if actualHistoricalDuration >= 0:
                     progressbar()
         sys.stdout.write(f"\x1b[1A") # Replace the download progress bar and start writing on the same line
         if not keyboardInterruptEventFired:
             global tasks_queue, results_queue, consumers, logging_queue
             screenResults, saveResults, backtest_df, tasks_queue, results_queue, consumers,logging_queue = PKScanRunner.runScanWithParams(userPassedArgs,keyboardInterruptEvent,screenCounter,screenResultsCounter,stockDictPrimary,stockDictSecondary,testing, backtestPeriod, menuOption, samplingDuration, items,screenResults, saveResults, backtest_df,scanningCb=runScanners,tasks_queue=tasks_queue, results_queue=results_queue, consumers=consumers,logging_queue=logging_queue)
-            if userPassedArgs is not None and (userPassedArgs.monitor is None and "|" not in userPassedArgs.options):
+            if userPassedArgs is not None and (userPassedArgs.monitor is None and "|" not in userPassedArgs.options and not userPassedArgs.options.upper().startswith("C")):
                 tasks_queue = None
                 results_queue = None
                 consumers = None
             if menuOption in ["C"]:
                 runOptionName = PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)
                 PKMarketOpenCloseAnalyser.runOpenCloseAnalysis(stockDictPrimary,endOfdayCandles,screenResults, saveResults,runOptionName=runOptionName)
             if downloadOnly and menuOption in ["X"]:
```

### Comparing `pkscreener-0.44.20240502.318/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240503.322/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240503.322/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240503.322/pkscreener/pkscreenercli.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,15 +298,15 @@
                 + colorText.FAIL
                 + "[+] Neither ta-lib nor pandas_ta was located. You need at least one of them to continue! \n[+] Please follow instructions from README file under PKScreener repo: https://github.com/pkjmesra/PKScreener"
                 + colorText.END
             )
             input("Press any key to try anyway...")
 
 def runApplication():
-    from pkscreener.globals import main, sendQuickScanResult, sendGlobalMarketBarometer, updateMenuChoiceHierarchy, isInterrupted, refreshStockData
+    from pkscreener.globals import main, sendQuickScanResult, sendGlobalMarketBarometer, updateMenuChoiceHierarchy, isInterrupted, refreshStockData, closeWorkersAndExit
     # From a previous call to main with args, it may have been mutated.
     # Let's stock to the original args passed by user
     argsv = argParser.parse_known_args()
     args = argsv[0]
     if args.runintradayanalysis:
         from pkscreener.classes.MenuOptions import menus
         runOptions = menus.allMenus(topLevel="C", index=12)
@@ -323,21 +323,22 @@
                     break
             except Exception as e:
                 OutputControls().printOutput(e)
                 if args.log:
                     traceback.print_exc()
         if optionalFinalOutcome_df is not None:
             final_df = None
+            optionalFinalOutcome_df.drop('FairValue', axis=1, inplace=True, errors="ignore")
             df_grouped = optionalFinalOutcome_df.groupby("Stock")
             for stock, df_group in df_grouped:
                 if stock == "PORTFOLIO":
                     if final_df is None:
-                        final_df = df_group[["Pattern","LTP","SqrOffLTP","SqrOffDiff","EoDLTP","EoDDiff","%Chng"]]
+                        final_df = df_group[["Pattern","LTP","SqrOffLTP","SqrOffDiff","EoDLTP","EoDDiff","DayHigh","DayHighDiff","%Chng"]]
                     else:
-                        final_df = pd.concat([final_df, df_group[["Pattern","LTP","SqrOffLTP","SqrOffDiff","EoDLTP","EoDDiff","%Chng"]]], axis=0)
+                        final_df = pd.concat([final_df, df_group[["Pattern","LTP","SqrOffLTP","SqrOffDiff","EoDLTP","EoDDiff","DayHigh","DayHighDiff","%Chng"]]], axis=0)
             final_df.rename(
                 columns={
                     "LTP": "Morning Portfolio",
                     "SqrOffLTP": "SqrOff Portfolio",
                     "EoDLTP": "EoD Portfolio",
                     "%Chng": "EoD %Chng",
                     },
@@ -401,18 +402,20 @@
                     refreshStockData(args.options)
             try: 
                 results = None
                 plainResults = None
                 resultStocks = None
                 results, plainResults = main(userArgs=args)
                 if isInterrupted():
+                    closeWorkersAndExit()
                     sys.exit(0)
                 while pipeResults(plainResults,args):
                     results, plainResults = main(userArgs=args)
             except SystemExit:
+                closeWorkersAndExit()
                 sys.exit(0)
             except Exception as e:
                 default_logger().debug(e, exc_info=True)
                 # Probably user cancelled an operation by choosing a cancel sub-menu somewhere
                 pass
             if plainResults is not None and not plainResults.empty:
                 plainResults = plainResults[~plainResults.index.duplicated(keep='first')]
@@ -535,51 +538,57 @@
             + colorText.FAIL
             + "[+] Download ONLY mode! Stocks will not be screened!"
             + colorText.END
         )
         if args.intraday is None:
             configManager.toggleConfig(candleDuration="1d", clearCache=False)
         runApplication()
+        from pkscreener.globals import closeWorkersAndExit
+        closeWorkersAndExit()
         sys.exit(0)
     else:
         runApplicationForScreening()
 
 def runLoopOnScheduleOrStdApplication(hasCronInterval):
     if hasCronInterval:
         scheduleNextRun()
     else:
         runApplication()
 
 def runApplicationForScreening():
+    from pkscreener.globals import closeWorkersAndExit
     try:
         hasCronInterval = args.croninterval is not None and str(args.croninterval).isnumeric()
         shouldBreak = (args.exit and not hasCronInterval)or args.user is not None or args.testbuild
         runLoopOnScheduleOrStdApplication(hasCronInterval)
         while True:
             if shouldBreak:
                 break
             runLoopOnScheduleOrStdApplication(hasCronInterval)
         if args.v:
             disableSysOut(disable=False)
             return
+        closeWorkersAndExit()
         sys.exit(0)
     except SystemExit:
+        closeWorkersAndExit()
         sys.exit(0)
     except (RuntimeError, Exception) as e:  # pragma: no cover
         default_logger().debug(e, exc_info=True)
         if args.prodbuild:
             disableSysOut(disable=False)
         OutputControls().printOutput(
             f"{e}\n[+] An error occurred! Please run with '-l' option to collect the logs.\n[+] For example, 'pkscreener -l' and then contact the developer!"
         )
         if "RUNNER" in os.environ.keys() or ('PKDevTools_Default_Log_Level' in os.environ.keys() and os.environ["PKDevTools_Default_Log_Level"] != str(log.logging.NOTSET)):
             traceback.print_exc()
         if args.v:
             disableSysOut(disable=False)
             return
+        closeWorkersAndExit()
         sys.exit(0)
 
 
 def scheduleNextRun():
     sleepUntilNextExecution = not PKDateUtilities.isTradingTime()
     while sleepUntilNextExecution:
         OutputControls().printOutput(
```

### Comparing `pkscreener-0.44.20240502.318/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240503.322/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240502.318
+Version: 0.44.20240503.322
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240502.318.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240503.322.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.317/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.319/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.317/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.319/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.317/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.319/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240502.318/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240503.322/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.318/setup.py` & `pkscreener-0.44.20240503.322/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/pkscreener-0.44.20240502.317.tar.gz` & `tmp/pkscreener-0.44.20240502.318.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240502.317.tar", last modified: Thu May  2 07:26:48 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240502.318.tar", last modified: Thu May  2 12:49:51 2024, max compression
```

## Comparing `pkscreener-0.44.20240502.317.tar` & `pkscreener-0.44.20240502.318.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 07:26:48.451769 pkscreener-0.44.20240502.317/
--rw-rw-rw-   0        0        0     1086 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-02 07:26:48.451769 pkscreener-0.44.20240502.317/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 07:26:48.436155 pkscreener-0.44.20240502.317/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 07:26:48.436155 pkscreener-0.44.20240502.317/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25810 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7496 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29455 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    21093 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    20691 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8124 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   117763 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    52127 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    82304 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-02 07:26:39.000000 pkscreener-0.44.20240502.317/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   123195 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/globals.py
--rw-rw-rw-   0        0        0      595 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    42912 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    25897 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-02 07:26:48.436155 pkscreener-0.44.20240502.317/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-02 07:26:48.000000 pkscreener-0.44.20240502.317/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-05-02 07:26:48.000000 pkscreener-0.44.20240502.317/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 07:26:48.000000 pkscreener-0.44.20240502.317/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-02 07:26:48.000000 pkscreener-0.44.20240502.317/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-02 07:26:48.000000 pkscreener-0.44.20240502.317/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-02 07:26:48.000000 pkscreener-0.44.20240502.317/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-02 07:26:48.451769 pkscreener-0.44.20240502.317/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:49:51.615947 pkscreener-0.44.20240502.318/
+-rw-rw-rw-   0        0        0     1086 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-02 12:49:51.615947 pkscreener-0.44.20240502.318/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 12:49:51.584700 pkscreener-0.44.20240502.318/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:49:51.600322 pkscreener-0.44.20240502.318/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    25810 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7496 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29455 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    21093 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    20691 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8124 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   117763 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    52127 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    82304 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-02 12:49:42.000000 pkscreener-0.44.20240502.318/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   123422 2024-05-02 12:44:27.000000 pkscreener-0.44.20240502.318/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      595 2024-05-02 12:44:28.000000 pkscreener-0.44.20240502.318/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    42912 2024-05-02 12:44:28.000000 pkscreener-0.44.20240502.318/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    25897 2024-05-02 12:44:28.000000 pkscreener-0.44.20240502.318/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:49:51.600322 pkscreener-0.44.20240502.318/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-02 12:49:51.000000 pkscreener-0.44.20240502.318/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-05-02 12:49:51.000000 pkscreener-0.44.20240502.318/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 12:49:51.000000 pkscreener-0.44.20240502.318/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-02 12:49:51.000000 pkscreener-0.44.20240502.318/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-02 12:49:51.000000 pkscreener-0.44.20240502.318/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-02 12:49:51.000000 pkscreener-0.44.20240502.318/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-02 12:49:51.615947 pkscreener-0.44.20240502.318/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-05-02 12:44:28.000000 pkscreener-0.44.20240502.318/setup.py
```

### Comparing `pkscreener-0.44.20240502.317/LICENSE` & `pkscreener-0.44.20240502.318/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/LICENSE-Others` & `pkscreener-0.44.20240502.318/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/PKG-INFO` & `pkscreener-0.44.20240502.318/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240502.317
+Version: 0.44.20240502.318
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240502.317.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240502.318.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.316/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.317/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.316/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.317/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.316/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.317/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240502.317/README.md` & `pkscreener-0.44.20240502.318/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.316/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.317/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.316/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.317/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.316/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.317/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240502.317/pkscreener/__init__.py` & `pkscreener-0.44.20240502.318/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/Utility.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -129,21 +129,21 @@
             if platform.system() == "Windows":
                 try:
                     os.system('color 0f') # sets the background to black with white forerground
                 except:
                     pass
                 os.system("cls")
             elif "Darwin" in platform.system():
+                os.system("clear")
+            else:
                 try:
                     os.system('setterm -background black -foreground white -store')
                 except:
                     pass
                 os.system("clear")
-            else:
-                os.system("clear")
         try:
             if clearAlways or OutputControls().enableMultipleLineOutput:
                 art = colorText.GREEN + artText + colorText.END + f" | {marketStatus()}"
                 OutputControls().printOutput(art.encode('utf-8').decode(STD_ENCODING), enableMultipleLineOutput=True)
         except Exception as e:# pragma: no cover
             default_logger().debug(e, exc_info=True)
             pass
```

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/classes/keys.py` & `pkscreener-0.44.20240502.318/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/courbd.ttf` & `pkscreener-0.44.20240502.318/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/globals.py` & `pkscreener-0.44.20240502.318/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1199,14 +1199,18 @@
                 actualHistoricalDuration = samplingDuration - fillerPlaceHolder
                 if actualHistoricalDuration >= 0:
                     progressbar()
         sys.stdout.write(f"\x1b[1A") # Replace the download progress bar and start writing on the same line
         if not keyboardInterruptEventFired:
             global tasks_queue, results_queue, consumers, logging_queue
             screenResults, saveResults, backtest_df, tasks_queue, results_queue, consumers,logging_queue = PKScanRunner.runScanWithParams(userPassedArgs,keyboardInterruptEvent,screenCounter,screenResultsCounter,stockDictPrimary,stockDictSecondary,testing, backtestPeriod, menuOption, samplingDuration, items,screenResults, saveResults, backtest_df,scanningCb=runScanners,tasks_queue=tasks_queue, results_queue=results_queue, consumers=consumers,logging_queue=logging_queue)
+            if userPassedArgs is not None and (userPassedArgs.monitor is None and "|" not in userPassedArgs.options):
+                tasks_queue = None
+                results_queue = None
+                consumers = None
             if menuOption in ["C"]:
                 runOptionName = PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)
                 PKMarketOpenCloseAnalyser.runOpenCloseAnalysis(stockDictPrimary,endOfdayCandles,screenResults, saveResults,runOptionName=runOptionName)
             if downloadOnly and menuOption in ["X"]:
                 screener.getFreshMFIStatus(stock="LatestCheckedOnDate")
                 screener.getFairValue(stock="LatestCheckedOnDate", force=True)
             if not downloadOnly and menuOption in ["X", "G", "C"]:
```

### Comparing `pkscreener-0.44.20240502.317/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240502.318/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240502.318/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240502.318/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240502.318/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240502.317
+Version: 0.44.20240502.318
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240502.317.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240502.318.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.316/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.317/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.316/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.317/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.316/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240502.317/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240502.317/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240502.318/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240502.317/setup.py` & `pkscreener-0.44.20240502.318/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/hexital-1.1.1.tar.gz` & `tmp/hexital-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexital-1.1.1.tar", max compression
+gzip compressed data, was "hexital-1.1.2.tar", max compression
```

## Comparing `hexital-1.1.1.tar` & `hexital-1.1.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     5954 2024-05-01 16:43:32.128182 hexital-1.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     1067 2024-05-01 16:43:32.128182 hexital-1.1.1/LICENSE
--rw-r--r--   0        0        0    12974 2024-05-01 16:43:32.128182 hexital-1.1.1/README.md
--rw-r--r--   0        0        0      249 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/__init__.py
--rw-r--r--   0        0        0      835 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/analysis/__init__.py
--rw-r--r--   0        0        0    12357 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/analysis/movement.py
--rw-r--r--   0        0        0     3921 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/analysis/patterns.py
--rw-r--r--   0        0        0     6102 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/analysis/utils.py
--rw-r--r--   0        0        0       80 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/candlesticks/__init__.py
--rw-r--r--   0        0        0      719 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/candlesticks/heikinashi.py
--rw-r--r--   0        0        0        0 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/core/__init__.py
--rw-r--r--   0        0        0     5636 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/core/candle.py
--rw-r--r--   0        0        0     7806 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/core/candle_manager.py
--rw-r--r--   0        0        0      958 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/core/candlestick_type.py
--rw-r--r--   0        0        0     9721 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/core/hexital.py
--rw-r--r--   0        0        0    12456 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/core/indicator.py
--rw-r--r--   0        0        0      632 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/exceptions.py
--rw-r--r--   0        0        0     1272 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/__init__.py
--rw-r--r--   0        0        0     3476 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/adx.py
--rw-r--r--   0        0        0     2188 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/amorph.py
--rw-r--r--   0        0        0     1182 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/aroon.py
--rw-r--r--   0        0        0     1049 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/atr.py
--rw-r--r--   0        0        0     1391 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/bbands.py
--rw-r--r--   0        0        0     1102 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/counter.py
--rw-r--r--   0        0        0     1169 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/donchian.py
--rw-r--r--   0        0        0     1295 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/ema.py
--rw-r--r--   0        0        0      714 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/highest_lowest.py
--rw-r--r--   0        0        0      426 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/hla.py
--rw-r--r--   0        0        0     1708 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/hma.py
--rw-r--r--   0        0        0     1602 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/kc.py
--rw-r--r--   0        0        0     2818 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/macd.py
--rw-r--r--   0        0        0      818 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/obv.py
--rw-r--r--   0        0        0     1370 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/rma.py
--rw-r--r--   0        0        0      685 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/roc.py
--rw-r--r--   0        0        0     2550 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/rsi.py
--rw-r--r--   0        0        0     1168 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/sma.py
--rw-r--r--   0        0        0     1760 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/stdev.py
--rw-r--r--   0        0        0     1188 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/stdevthres.py
--rw-r--r--   0        0        0     2852 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/stoch.py
--rw-r--r--   0        0        0     2366 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/supertrend.py
--rw-r--r--   0        0        0      824 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/tr.py
--rw-r--r--   0        0        0     2782 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/tsi.py
--rw-r--r--   0        0        0     1363 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/vwap.py
--rw-r--r--   0        0        0      906 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/vwma.py
--rw-r--r--   0        0        0      962 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/wma.py
--rw-r--r--   0        0        0       89 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/utils/__init__.py
--rw-r--r--   0        0        0     2960 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/utils/candles.py
--rw-r--r--   0        0        0      585 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/utils/candlesticks.py
--rw-r--r--   0        0        0     1088 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/utils/indexing.py
--rw-r--r--   0        0        0     2792 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/utils/timeframe.py
--rw-r--r--   0        0        0     1534 2024-05-01 16:43:32.128182 hexital-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    13985 1970-01-01 00:00:00.000000 hexital-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6292 2024-05-03 20:50:34.299648 hexital-1.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1067 2024-05-03 20:50:34.299648 hexital-1.1.2/LICENSE
+-rw-r--r--   0        0        0    13009 2024-05-03 20:50:34.299648 hexital-1.1.2/README.md
+-rw-r--r--   0        0        0      249 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/__init__.py
+-rw-r--r--   0        0        0      835 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/analysis/__init__.py
+-rw-r--r--   0        0        0    10656 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/analysis/movement.py
+-rw-r--r--   0        0        0     3921 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/analysis/patterns.py
+-rw-r--r--   0        0        0     6102 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/analysis/utils.py
+-rw-r--r--   0        0        0       80 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/candlesticks/__init__.py
+-rw-r--r--   0        0        0      719 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/candlesticks/heikinashi.py
+-rw-r--r--   0        0        0        0 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/core/__init__.py
+-rw-r--r--   0        0        0     5636 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/core/candle.py
+-rw-r--r--   0        0        0     7908 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/core/candle_manager.py
+-rw-r--r--   0        0        0      958 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/core/candlestick_type.py
+-rw-r--r--   0        0        0     9735 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/core/hexital.py
+-rw-r--r--   0        0        0    12524 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/core/indicator.py
+-rw-r--r--   0        0        0      632 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/exceptions.py
+-rw-r--r--   0        0        0     1272 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/__init__.py
+-rw-r--r--   0        0        0     3476 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/adx.py
+-rw-r--r--   0        0        0     2188 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/amorph.py
+-rw-r--r--   0        0        0     1182 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/aroon.py
+-rw-r--r--   0        0        0     1049 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/atr.py
+-rw-r--r--   0        0        0     1391 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/bbands.py
+-rw-r--r--   0        0        0     1102 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/counter.py
+-rw-r--r--   0        0        0     1169 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/donchian.py
+-rw-r--r--   0        0        0     1295 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/ema.py
+-rw-r--r--   0        0        0      714 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/highest_lowest.py
+-rw-r--r--   0        0        0      426 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/hla.py
+-rw-r--r--   0        0        0     1708 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/hma.py
+-rw-r--r--   0        0        0     1602 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/kc.py
+-rw-r--r--   0        0        0     2818 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/macd.py
+-rw-r--r--   0        0        0      818 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/obv.py
+-rw-r--r--   0        0        0     1370 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/rma.py
+-rw-r--r--   0        0        0      685 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/roc.py
+-rw-r--r--   0        0        0     2550 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/rsi.py
+-rw-r--r--   0        0        0     1168 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/sma.py
+-rw-r--r--   0        0        0     1760 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/stdev.py
+-rw-r--r--   0        0        0     1188 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/stdevthres.py
+-rw-r--r--   0        0        0     2852 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/stoch.py
+-rw-r--r--   0        0        0     2366 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/supertrend.py
+-rw-r--r--   0        0        0      824 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/tr.py
+-rw-r--r--   0        0        0     2782 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/tsi.py
+-rw-r--r--   0        0        0     1363 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/vwap.py
+-rw-r--r--   0        0        0      906 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/vwma.py
+-rw-r--r--   0        0        0      962 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/indicators/wma.py
+-rw-r--r--   0        0        0       89 2024-05-03 20:50:34.299648 hexital-1.1.2/hexital/utils/__init__.py
+-rw-r--r--   0        0        0     3129 2024-05-03 20:50:34.303648 hexital-1.1.2/hexital/utils/candles.py
+-rw-r--r--   0        0        0      585 2024-05-03 20:50:34.303648 hexital-1.1.2/hexital/utils/candlesticks.py
+-rw-r--r--   0        0        0     1088 2024-05-03 20:50:34.303648 hexital-1.1.2/hexital/utils/indexing.py
+-rw-r--r--   0        0        0     2792 2024-05-03 20:50:34.303648 hexital-1.1.2/hexital/utils/timeframe.py
+-rw-r--r--   0        0        0     1582 2024-05-03 20:50:34.303648 hexital-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0    14020 1970-01-01 00:00:00.000000 hexital-1.1.2/PKG-INFO
```

### Comparing `hexital-1.1.1/CHANGELOG.md` & `hexital-1.1.2/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 1.1.2
+
+- Fixed Major incremental calculate flaw with sub indicators
+  - Causing sub indicators to almost always re-calc entire set rather than latest (incrementally)
+- Optimised Analysis and Movement functions for less calls and less loops
+- Removed Deepcopies on Candles unless being added to Extra timeframes to speed up appending
+
 ## 1.1.1 - 2024-05-01
+
 - Changed Movement rising/falling default length from 4 to 1
 - Added better exceptions to Hexital verifying dict indicators
 - Mass Indicator clean up to fix, unused/unended input_value's and unused sub indicators
 - Fixed minor donchian error
 - Fixed Highest and Lowest movement methods from returning bool False instead of None
 - Added Indicators
   - Added HighestLowest (HL)
```

### Comparing `hexital-1.1.1/LICENSE` & `hexital-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/README.md` & `hexital-1.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -199,30 +199,30 @@
 
 ## Testing
 
 Testing is a critical aspect of this library due to the complexity of ensuring the accuracy of generated indicator values. To achieve this, I rely on [Pandas-TA](https://github.com/twopirllc/pandas-ta) as the source of truth for indicator values. Each indicator added to this library undergoes testing, where the output is compared against the corresponding indicator output from Pandas-TA. Due to slight differences in calculations, particularly within NumPy, not all values are exactly identical. Therefore, if differences exceed a given threshold (usually beyond one decimal place), a Pearson correlation coefficient is calculated to ensure correct correlation with the expected output.
 
 ### Speed Tests
 
-The following charts illustrate the results and speed of Pandas-TA and Hexital in both bulk and incremental calculations. These results are obtained from running Pandas-TA and Hexital in bulk (_all candles calculated at once_) and incremental(_Caluclating after each new candle is added_) modes; charts _1 and 2_.
+The following charts illustrate the results and speed of Pandas-TA and Hexital in both bulk and incremental calculations. These results are obtained from running Pandas-TA and Hexital in bulk (_all candles calculated at once_) and incremental(_Caluclating after each new candle is added_) modes; chart _1_.
 
 The incremental charts demonstrate the process of calculating technical analysis, adding one candle at a time, and recalculating up to a specified number of candles. It's evident that using Pandas-TA, Pandas, and NumPy for incremental data processing incurs significant performance overhead. This is primarily due to the underlying behavior of NumPy, which involves reallocating memory when appending or concatenating data, rather than resizing it. As a result, it's recommended in NumPy and Pandas documentation to gather all data prior to running calculations. On the other hand, Hexital, being purely Pythonic, exhibits efficient performance both in bulk and incremental processing, with minimal to no additional overhead time. It significantly outperforms Pandas-TA in incremental processing and even surpasses Pandas-TA in speed, especially with smaller datasets.
 
-![EMA 10 test results.](tests/speed_tests/EMA_10.png)
+![EMA 10 test results.](tests/extra/speed_tests/EMA_10.png)
 
-From chart _(3)_, it's evident that in bulk calculations with an extremely large dataset, Pandas-TA outperforms Hexital. Pandas-TA maintains consistent performance, with processing times starting at 0.08 seconds for 1,000 candles and remaining stable at this level for 10,000 candles. In contrast, Hexital exhibits faster processing times, starting at 0.005 seconds for 1,000 candles but increasing to 0.05 seconds for 10,000 candles. While Hexital is initially faster, there is a noticeable growth in processing time as the dataset size increases. Therefore, for backtesting with a large dataset, Pandas-TA offers superior performance, while Hexital may experience slowdowns.
+From chart _(2)_, it's evident that in bulk calculations with an extremely large dataset, Pandas-TA outperforms Hexital. Pandas-TA maintains consistent performance, with processing times starting at 0.08 seconds for 1,000 candles and remaining stable at this level for 10,000 candles. In contrast, Hexital exhibits faster processing times, starting at 0.025 seconds for 2,000 candles but increasing to 0.16 seconds for 10,000 candles. While Hexital is initially faster, there is a noticeable growth in processing time as the dataset size increases. Therefore, for backtesting with a large dataset, Pandas-TA offers superior performance, while Hexital may experience slowdowns.
 
-![EMA 10 Bulk test results.](tests/speed_tests/EMA_10%20Bulk%20Calculations.png)
+![MACD 26 Bulk test results.](tests/extra/speed_tests/MACD_26_12_Bulk_Calculations.png)
 
-However referencing chart _(4)_ being an example of using both these libraries for a live application, whereby at n candles we incrementing a dataset with a candle and calculating the new TA; `Hexital` is far quicker. This is due to the speed that python can increment a list of data rather than Panda, as well as `Hexital` only needing to calculate the newest candle rather than having to re-calculate the entire dataset. Chart _3_ clearly shows the speed benefits it has over Pandas-TA and other Panda based Technical Analysis tools for incremental data sets.
+However referencing chart _(3)_ being an example of using both these libraries for a live incremental application, whereby at n candles we incrementing a dataset with a candle and calculating the new TA; `Hexital` is far quicker. This is due to the speed that python can increment a list of data rather than Panda, as well as `Hexital` only needing to calculate the newest candle rather than having to re-calculate the entire dataset. Chart _3_ clearly shows the speed benefits it has over Pandas-TA and other Panda based Technical Analysis tools for incremental data sets.
 
-![EMA 10 Real world usage.](tests/speed_tests/EMA_10_real_world.png)
+![MACD 26 Real world usage.](tests/extra/speed_tests/MACD_26_12_real_world.png)
 
 For reference, if using seconds Candle with 10,000 candles that is around 2 Hours 46 minutes.
 
 #### Note
 
-The code that produces these charts is: `tests/speed_tests/run_speed_test.py` and can be ran by calling `make speed-test`. Some noise is seen due to running on personal laptop while in use.
+The code that produces these charts is: `tests/extra/speed_tests/run_speed_test.py` and can be ran by calling `make speed-test`. Some noise is seen due to running on personal laptop while in use.
 
 ## Inspiration
 
 This library was inspired by [TALIpp](https://github.com/nardew/talipp), another Incremental Technical Analysis Library. However, I found the separate input lists rather cumbersome compared to working with an entire candle. Additionally, in TALIpp, outputs are separate entities, requiring extensive management. In contrast, Hexital stores all data within the candle, simplifying usage and management.
```

### Comparing `hexital-1.1.1/hexital/analysis/__init__.py` & `hexital-1.1.2/hexital/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/analysis/movement.py` & `hexital-1.1.2/hexital/analysis/movement.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from typing import List
 
 from hexital.core.candle import Candle
 from hexital.utils.candles import (
     reading_by_candle,
     reading_by_index,
-    reading_count,
-    reading_period,
 )
 from hexital.utils.indexing import absindex, valid_index
 
 
 def _get_clean_readings(
     candles: List[Candle], indicator: str, length: int, index: int, include_latest: bool = False
 ) -> List[float | int]:
-    """Goes through from index-length to index and returns a list of values, removes dict's and None values"""
+    """Goes through from index-length to index and returns a list of values, removes dict's and None values
+    Returns from newest at the front (reversed)"""
     to_index = index
     if include_latest:
         to_index += 1
 
-    readings = [
-        reading_by_candle(candle, indicator) for candle in candles[index - length : to_index]
-    ]
-    return [reading for reading in readings if isinstance(reading, (float, int))]
+    start = index - length
+    if start < 0:
+        start = 0
+
+    readings = [reading_by_candle(candle, indicator) for candle in candles[start:to_index]]
+    return [reading for reading in reversed(readings) if isinstance(reading, (float, int))]
 
 
 def positive(candles: Candle | List[Candle], index: int = -1) -> bool:
     if isinstance(candles, Candle):
         return candles.positive
 
     if not valid_index(index, len(candles)):
@@ -46,15 +47,15 @@
     """Check if indicator is a higher value than indicator_two"""
     if not candles:
         return False
 
     reading_one = reading_by_index(candles, indicator, index)
     reading_two = reading_by_index(candles, indicator_two, index)
 
-    if isinstance(reading_one, (float, int)) and isinstance(reading_two, (float, int)):
+    if reading_one is not None and reading_two is not None:
         return reading_one > reading_two
     return False
 
 
 def below(candles: List[Candle], indicator: str, indicator_two: str, index: int = -1) -> bool:
     """Check if indicator is a lower value than indicator_two"""
     if not candles:
@@ -71,194 +72,172 @@
 def value_range(
     candles: List[Candle], indicator: str, length: int = 4, index: int = -1
 ) -> float | None:
     """Returns the difference between the min and max values in a indicator series.
     Length `includes` latest, if lenth is too long for amount of candles,
     will check all of them"""
     index_ = absindex(index, len(candles))
-    if index_ is None:
+    if index_ is None or length < 2:
         return None
 
-    if not reading_period(candles, length, indicator):
-        length = reading_count(candles, indicator) - 1
+    readings = _get_clean_readings(candles, indicator, length, index_, True)
 
-    if length < 2:
+    if len(readings) < 2:
         return None
 
-    readings = _get_clean_readings(candles, indicator, length, index_, True)
-
     return abs(min(readings) - max(readings))
 
 
 def rising(candles: List[Candle], indicator: str, length: int = 1, index: int = -1) -> bool:
     """True if current `indicator` is greater than all previous `indicator`
     for `length` bars back, False otherwise.
     Length `excludes` latest"""
     index_ = absindex(index, len(candles))
-    if index_ is None:
-        return False
-
-    if not reading_period(candles, length, indicator):
-        length = reading_count(candles, indicator) - 1
 
-    if length < 1 or len(candles) < 2:
+    if index_ is None or length < 1 or len(candles) < 2:
         return False
 
-    latest_reading = reading_by_candle(candles[-1], indicator)
+    latest_reading = reading_by_candle(candles[index], indicator)
     if latest_reading is None or isinstance(latest_reading, dict):
         return False
 
     readings = _get_clean_readings(candles, indicator, length, index_)
+    if not readings:
+        return False
 
-    return all(reading < latest_reading for reading in readings)
+    for reading in readings:
+        if reading >= latest_reading:
+            return False
+    return True
 
 
 def falling(candles: List[Candle], indicator: str, length: int = 1, index: int = -1) -> bool:
     """True if current `indicator` reading is less than all previous `indicator`
     reading for `length` bars back, False otherwise.
     Length `excludes` latest"""
     index_ = absindex(index, len(candles))
-    if index_ is None:
-        return False
-
-    if not reading_period(candles, length, indicator):
-        length = reading_count(candles, indicator) - 1
-
-    if length < 1 or len(candles) < 2:
+    if index_ is None or length < 1 or len(candles) < 2:
         return False
 
-    latest_reading = reading_by_candle(candles[-1], indicator)
+    latest_reading = reading_by_candle(candles[index], indicator)
     if latest_reading is None or isinstance(latest_reading, dict):
         return False
 
     readings = _get_clean_readings(candles, indicator, length, index_)
+    if not readings:
+        return False
 
-    return all(reading > latest_reading for reading in readings)
+    for reading in readings:
+        if reading <= latest_reading:
+            return False
+    return True
 
 
 def mean_rising(candles: List[Candle], indicator: str, length: int = 4, index: int = -1) -> bool:
     """True if current `indicator` reading is greater than the avg of the previous
     `length` `indicator` reading bars back, False otherwise. Length `excludes` latest
 
     Calc:
         NewestCandle[indicator] > mean(Candles[newest] to Candles[length])"""
     index_ = absindex(index, len(candles))
-    if index_ is None:
+    if index_ is None or length < 1 or len(candles) < 2:
         return False
 
-    if not reading_period(candles, length, indicator):
-        length = reading_count(candles, indicator) - 1
-
-    if length < 1 or len(candles) < 2:
-        return False
-
-    latest_reading = reading_by_candle(candles[-1], indicator)
+    latest_reading = reading_by_candle(candles[index_], indicator)
     if latest_reading is None or isinstance(latest_reading, dict):
         return False
 
     readings = _get_clean_readings(candles, indicator, length, index_)
+    if not readings:
+        return False
 
-    mean = sum(reading for reading in readings) / length
-    return round(mean, 2) < latest_reading
+    return sum(readings) / len(readings) < latest_reading
 
 
 def mean_falling(candles: List[Candle], indicator: str, length: int = 4, index: int = -1) -> bool:
     """True if current `indicator` is less than the avg of the previous
     `length` `indicator` bars back, False otherwise. Length `excludes` latest
 
     Calc:
         NewestCandle[indicator] > mean(Candles[newest] to Candles[length])"""
     index_ = absindex(index, len(candles))
-    if index_ is None:
+    if index_ is None or length < 1 or len(candles) < 2:
         return False
 
-    if not reading_period(candles, length, indicator):
-        length = reading_count(candles, indicator) - 1
-
-    if length < 1 or len(candles) < 2:
-        return False
-
-    latest_reading = reading_by_candle(candles[-1], indicator)
+    latest_reading = reading_by_candle(candles[index_], indicator)
     if latest_reading is None or isinstance(latest_reading, dict):
         return False
 
     readings = _get_clean_readings(candles, indicator, length, index_)
+    if not readings:
+        return False
 
-    mean = sum(reading for reading in readings) / length
-    return round(mean, 2) > latest_reading
+    return sum(readings) / len(readings) > latest_reading
 
 
 def highest(
     candles: List[Candle], indicator: str, length: int = 4, index: int = -1
 ) -> float | None:
     """Highest reading for a given number of bars back.
     Returns:
         Highest reading in the series.
     """
     index_ = absindex(index, len(candles))
-    if index_ is None:
+    if index_ is None or length < 1 or not len(candles):
         return False
 
-    if not reading_period(candles, length, indicator, index_):
-        length = reading_count(candles, indicator) - 1
-
     readings = _get_clean_readings(candles, indicator, length, index_, True)
 
-    max_reading = max([reading for reading in readings], default=False)
-    return max_reading if max_reading else None
+    max_reading = max(readings, default=False)
+    return max_reading if max_reading is not False else None
 
 
 def lowest(
     candles: List[Candle], indicator: str, length: int = 4, index: int = -1
 ) -> float | None:
     """Lowest reading for a given number of bars back.
     Returns:
         Lowest reading in the series.
     """
     index_ = absindex(index, len(candles))
-    if index_ is None:
+    if index_ is None or length < 1 or not len(candles):
         return False
 
-    if not reading_period(candles, length, indicator):
-        length = reading_count(candles, indicator) - 1
-
     readings = _get_clean_readings(candles, indicator, length, index_, True)
 
-    min_reading = min([reading for reading in readings], default=False)
+    min_reading = min(readings, default=False)
 
-    return min_reading if min_reading else None
+    return min_reading if min_reading is not False else None
 
 
 def highestbar(
     candles: List[Candle], indicator: str, length: int = 4, index: int = -1
 ) -> int | None:
     """Highest reading offset for a given number of bars back.
     Returns:
         Offset to the lowest bar
     """
     index_ = absindex(index, len(candles))
     if index_ is None:
         return None
 
-    if not reading_period(candles, length, indicator):
-        length = reading_count(candles, indicator)
-
     high = None
     distance = 0
 
-    for dist, index in enumerate(range(index_, index_ - length, -1)):
+    for idx, index in enumerate(range(index_, index_ - length, -1)):
         current = reading_by_index(candles, indicator, index)
-        if current is None or isinstance(current, dict):
+        if current is None:
             continue
 
-        if high and high < current:
+        if high is None:
             high = current
-            distance = dist
-        elif high is None:
+
+        if high < current:
             high = current
+            distance = idx
 
     return distance
 
 
 def lowestbar(
     candles: List[Candle], indicator: str, length: int = 4, index: int = -1
 ) -> int | None:
@@ -266,55 +245,46 @@
     Returns:
         Offset to the lowest bar
     """
     index_ = absindex(index, len(candles))
     if index_ is None:
         return None
 
-    if not reading_period(candles, length, indicator):
-        length = reading_count(candles, indicator)
-
     low = None
     distance = 0
 
-    for dist, index in enumerate(range(index_, index_ - length, -1)):
+    for idx, index in enumerate(range(index_, index_ - length, -1)):
         current = reading_by_index(candles, indicator, index)
-        if current is None or isinstance(current, dict):
+        if current is None:
             continue
 
-        if low and low > current:
+        if low is None:
             low = current
-            distance = dist
-        elif low is None:
+
+        if low > current:
             low = current
+            distance = idx
 
     return distance
 
 
 def cross(
     candles: List[Candle], indicator_one: str, indicator_two: str, length: int = 1, index: int = -1
 ) -> bool:
     """The `indicator_one` reading is defined as having crossed `indicator_two` reading.
     Either direction"""
     index_ = absindex(index, len(candles))
     if index_ is None:
         return False
 
-    if not reading_period(candles, length, indicator_one) or not reading_period(
-        candles, length, indicator_two
-    ):
-        length = (
-            min([reading_count(candles, indicator_one), reading_count(candles, indicator_two)]) - 1
-        )
-
-    for index in range(index_, index_ - length, -1):
-        reading_one = reading_by_index(candles, indicator_two, index)
-        reading_two = reading_by_index(candles, indicator_one, index)
-        prev_one = reading_by_index(candles, indicator_one, index - 1)
-        prev_two = reading_by_index(candles, indicator_two, index - 1)
+    for idx in range(index_, index_ - length, -1):
+        reading_one = reading_by_index(candles, indicator_two, idx)
+        reading_two = reading_by_index(candles, indicator_one, idx)
+        prev_one = reading_by_index(candles, indicator_one, idx - 1)
+        prev_two = reading_by_index(candles, indicator_two, idx - 1)
 
         if (reading_one < reading_two and prev_one <= prev_two) or (
             reading_one > reading_two and prev_one >= prev_two
         ):
             return True
 
     return False
@@ -326,24 +296,17 @@
     """The `indicator_one` reading is defined as having crossed over `indicator_two` reading,
     If  `indicator_two` is higher then `indicator_one` and in the last `length` it was under.
     Length is how far back to check, if length is greater then amount of candles, check all"""
     index_ = absindex(index, len(candles))
     if index_ is None:
         return False
 
-    if not reading_period(candles, length, indicator_one) or not reading_period(
-        candles, length, indicator_two
-    ):
-        length = (
-            min([reading_count(candles, indicator_one), reading_count(candles, indicator_two)]) - 1
-        )
-
-    for index in range(index_, index_ - length, -1):
-        if above(candles, indicator_one, indicator_two, index) and below(
-            candles, indicator_one, indicator_two, index - 1
+    for idx in range(index_, index_ - length, -1):
+        if above(candles, indicator_one, indicator_two, idx) and below(
+            candles, indicator_one, indicator_two, idx - 1
         ):
             return True
 
     return False
 
 
 def crossunder(
@@ -352,21 +315,14 @@
     """The `indicator_one` reading is defined as having crossed under `indicator_two` reading,
     If `indicator_two` is lower then `indicator_one` and in the last `length` it was over.
     Length is how far back to check, if length is greater then amount of candles, check all"""
     index_ = absindex(index, len(candles))
     if index_ is None:
         return False
 
-    if not reading_period(candles, length, indicator_one) or not reading_period(
-        candles, length, indicator_two
-    ):
-        length = (
-            min([reading_count(candles, indicator_one), reading_count(candles, indicator_two)]) - 1
-        )
-
-    for index in range(index_, index_ - length, -1):
-        if below(candles, indicator_one, indicator_two, index) and above(
-            candles, indicator_one, indicator_two, index - 1
+    for idx in range(index_, index_ - length, -1):
+        if below(candles, indicator_one, indicator_two, idx) and above(
+            candles, indicator_one, indicator_two, idx - 1
         ):
             return True
 
     return False
```

### Comparing `hexital-1.1.1/hexital/analysis/patterns.py` & `hexital-1.1.2/hexital/analysis/patterns.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/analysis/utils.py` & `hexital-1.1.2/hexital/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/candlesticks/heikinashi.py` & `hexital-1.1.2/hexital/candlesticks/heikinashi.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/core/candle.py` & `hexital-1.1.2/hexital/core/candle.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/core/candle_manager.py` & `hexital-1.1.2/hexital/core/candle_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,19 @@
             elif isinstance(candles[0], list):
                 candles_.extend(Candle.from_lists(candles))
             else:
                 raise TypeError
         else:
             raise TypeError
 
-        self.candles.extend(deepcopy(candles_))
+        if self.name == DEFAULT_CANDLES:
+            self.candles.extend(candles_)
+        else:
+            self.candles.extend(deepcopy(candles_))
+
         self._tasks()
 
     def trim_candles(self):
         if self.candles_lifespan is None or not self.candles:
             return
 
         latest = self.candles[-1].timestamp
```

### Comparing `hexital-1.1.1/hexital/core/candlestick_type.py` & `hexital-1.1.2/hexital/core/candlestick_type.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/core/hexital.py` & `hexital-1.1.2/hexital/core/hexital.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from copy import deepcopy
+from copy import copy, deepcopy
 from datetime import timedelta
 from typing import Dict, List, Optional, Set
 
 from hexital.analysis import MOVEMENT_MAP, PATTERN_MAP
 from hexital.core.candle import Candle
 from hexital.core.candle_manager import DEFAULT_CANDLES, CandleManager
 from hexital.core.candlestick_type import CandlestickType
@@ -77,37 +77,35 @@
                     f"Indicator type invalid 'indicator' must be a dict or Indicator type: {indicator}"
                 )
 
             new_indicator = self._build_indicator(indicator)
             valid_indicators[new_indicator.name] = new_indicator
 
         for indicator in valid_indicators.values():
-            manager = CandleManager(
-                [],
-                candles_lifespan=self.candles_lifespan,
-                timeframe=indicator.timeframe if indicator.timeframe else self.timeframe,
-                timeframe_fill=self.timeframe_fill,
-                candlestick_type=self.candlestick_type,
-            )
-
-            if manager == self._candles[DEFAULT_CANDLES]:
+            if not indicator.timeframe:
                 indicator.candle_manager = self._candles[DEFAULT_CANDLES]
-            elif manager.name in self._candles:
-                indicator.candle_manager = self._candles[manager.name]
+            elif indicator.timeframe and indicator.timeframe in self._candles:
+                indicator.candle_manager = self._candles[indicator.timeframe]
             else:
+                manager = CandleManager(
+                    deepcopy(self._candles[DEFAULT_CANDLES]).candles,
+                    candles_lifespan=self.candles_lifespan,
+                    timeframe=indicator.timeframe if indicator.timeframe else self.timeframe,
+                    timeframe_fill=self.timeframe_fill,
+                    candlestick_type=self.candlestick_type,
+                )
                 self._candles[manager.name] = manager
-                manager.append(deepcopy(self._candles[DEFAULT_CANDLES]).candles)
                 indicator.candle_manager = self._candles[manager.name]
 
         return valid_indicators
 
     def _build_indicator(self, raw_indicator: dict) -> Indicator:
         analysis_map = PATTERN_MAP | MOVEMENT_MAP
         amorph_class = INDICATOR_MAP["Amorph"]
-        indicator = deepcopy(raw_indicator)
+        indicator = copy(raw_indicator)
 
         if indicator.get("indicator"):
             indicator_name = indicator.pop("indicator")
 
             if INDICATOR_MAP.get(indicator_name):
                 indicator_class = INDICATOR_MAP[indicator_name]
                 return indicator_class(**indicator)
```

### Comparing `hexital-1.1.1/hexital/core/indicator.py` & `hexital-1.1.2/hexital/core/indicator.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,25 +214,28 @@
 
         self._calculate_sub_indicators(False, start_index, end_index)
 
     def _find_calc_index(self) -> int:
         """Optimisation method, to find where to start calculating the indicator from
         Searches from newest to oldest to find the first candle without the indicator
         """
-        if len(self.candles) == 0 or self.name not in self.candles[0].indicators:
+        if len(self.candles) == 0 or (
+            self.name not in self.candles[0].indicators
+            and self.name not in self.candles[0].sub_indicators
+        ):
             return 0
 
         for index in range(len(self.candles) - 1, 0, -1):
             if (
                 self.name in self.candles[index].indicators
                 or self.name in self.candles[index].sub_indicators
             ):
                 return index + 1
 
-        return len(self.candles) - 1
+        return 0
 
     def _set_active_index(self, index: int):
         self._active_index = index
         for indicator in self.managed_indicators.values():
             if isinstance(indicator, Managed):
                 indicator.set_active_index(index)
```

### Comparing `hexital-1.1.1/hexital/exceptions.py` & `hexital-1.1.2/hexital/exceptions.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/__init__.py` & `hexital-1.1.2/hexital/indicators/__init__.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/adx.py` & `hexital-1.1.2/hexital/indicators/adx.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/amorph.py` & `hexital-1.1.2/hexital/indicators/amorph.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/aroon.py` & `hexital-1.1.2/hexital/indicators/aroon.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/atr.py` & `hexital-1.1.2/hexital/indicators/atr.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/bbands.py` & `hexital-1.1.2/hexital/indicators/bbands.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/counter.py` & `hexital-1.1.2/hexital/indicators/counter.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/donchian.py` & `hexital-1.1.2/hexital/indicators/donchian.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/ema.py` & `hexital-1.1.2/hexital/indicators/ema.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/highest_lowest.py` & `hexital-1.1.2/hexital/indicators/highest_lowest.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/hma.py` & `hexital-1.1.2/hexital/indicators/hma.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/kc.py` & `hexital-1.1.2/hexital/indicators/kc.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/macd.py` & `hexital-1.1.2/hexital/indicators/macd.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/obv.py` & `hexital-1.1.2/hexital/indicators/obv.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/rma.py` & `hexital-1.1.2/hexital/indicators/rma.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/roc.py` & `hexital-1.1.2/hexital/indicators/roc.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/rsi.py` & `hexital-1.1.2/hexital/indicators/rsi.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/sma.py` & `hexital-1.1.2/hexital/indicators/sma.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/stdev.py` & `hexital-1.1.2/hexital/indicators/stdev.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/stdevthres.py` & `hexital-1.1.2/hexital/indicators/stdevthres.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/stoch.py` & `hexital-1.1.2/hexital/indicators/stoch.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/supertrend.py` & `hexital-1.1.2/hexital/indicators/supertrend.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/tr.py` & `hexital-1.1.2/hexital/indicators/tr.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/tsi.py` & `hexital-1.1.2/hexital/indicators/tsi.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/vwap.py` & `hexital-1.1.2/hexital/indicators/vwap.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/vwma.py` & `hexital-1.1.2/hexital/indicators/vwma.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/indicators/wma.py` & `hexital-1.1.2/hexital/indicators/wma.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/utils/candles.py` & `hexital-1.1.2/hexital/utils/candles.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from itertools import chain
 from typing import List, Optional
 
 from hexital.core.candle import Candle
 from hexital.utils.indexing import absindex, valid_index
 
 
 def reading_by_index(candles: List[Candle], name: str, index: int = -1) -> float | dict | None:
@@ -16,39 +15,50 @@
 def reading_by_candle(candle: Candle, name: str) -> float | dict | None:
     """Simple method to get a reading from the given indicator from a candle
     Uses '.' to find nested reading, E.G 'MACD_12_26_9.MACD"""
 
     if "." in name:
         main_name, nested_name = name.split(".")
         reading = _nested_indicator(candle, main_name, nested_name)
-        if reading is not None:
-            return reading
+        return reading
 
-    if getattr(candle, name, None) is not None:
-        return getattr(candle, name)
+    attr = getattr(candle, name, None)
 
-    for key, reading in chain(candle.indicators.items(), candle.sub_indicators.items()):
+    if attr is not None:
+        return attr
+
+    for key in candle.indicators:
+        if key == name:
+            return candle.indicators[key]
+
+    for key in candle.sub_indicators:
         if key == name:
-            return reading
+            return candle.sub_indicators[key]
 
     return None
 
 
 def _nested_indicator(candle: Candle, name: str, nested_name: str) -> float | None:
-    for key, reading in chain(candle.indicators.items(), candle.sub_indicators.items()):
+    for key in candle.indicators:
+        if key == name:
+            reading = candle.indicators[key]
+            return reading.get(nested_name) if isinstance(reading, dict) else reading
+
+    for key in candle.sub_indicators:
         if key == name:
+            reading = candle.sub_indicators[key]
             return reading.get(nested_name) if isinstance(reading, dict) else reading
 
     return None
 
 
 def reading_count(candles: List[Candle], name: str) -> int:
     """Returns how many instance of the given indicator exist"""
     for count, candle in enumerate(reversed(candles)):
-        if not reading_by_candle(candle, name):
+        if reading_by_candle(candle, name) is None:
             return count
 
     return len(candles)
 
 
 def reading_period(
     candles: List[Candle], period: int, name: str, index: Optional[int] = None
@@ -61,29 +71,29 @@
         index = len(candles) - 1
     elif not valid_index(index, len(candles)):
         return False
 
     if index - period < 0:
         return False
 
-    return all(
-        bool(
+    for point in [
+        period,
+        period / 2,
+        0,
+    ]:
+        if (
             reading_by_index(
                 candles,
                 name,
                 index - int(point),
             )
-            is not None
-        )
-        for point in [
-            period,
-            period / 2,
-            0,
-        ]
-    )
+            is None
+        ):
+            return False
+    return True
 
 
 def candles_sum(
     candles: List[Candle], indicator: str, length: int, index: int = -1
 ) -> float | None:
     """Sum of `indicator` for `length` bars back. including index/latest"""
     index_ = absindex(index, len(candles))
@@ -91,8 +101,8 @@
         return
 
     index_ += 1
 
     length = len(candles) if length > len(candles) else length
     values = [reading_by_candle(candle, indicator) for candle in candles[index_ - length : index_]]
 
-    return sum(value for value in values if value and isinstance(value, (int, float)))
+    return sum(value for value in values if value is not None)
```

### Comparing `hexital-1.1.1/hexital/utils/candlesticks.py` & `hexital-1.1.2/hexital/utils/candlesticks.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/utils/indexing.py` & `hexital-1.1.2/hexital/utils/indexing.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/hexital/utils/timeframe.py` & `hexital-1.1.2/hexital/utils/timeframe.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.1/pyproject.toml` & `hexital-1.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hexital"
-version = "1.1.1"
+version = "1.1.2"
 description = "Hex Incremental Technical Analysis Library"
 readme = "README.md"
 license = "MIT"
 authors = ["Merlin Roe <merlin.roe@hotmail.co.uk>"]
 homepage = "https://github.com/MerlinR/Hexital"
 repository = "https://github.com/MerlinR/Hexital"
 documentation = "https://github.com/MerlinR/Hexital"
@@ -25,14 +25,16 @@
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.4.4"
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 deepdiff = "^7.0.1"
+pytest-profiling = "^1.7.0"
+snakeviz = "^2.2.0"
 
 [tool.poetry.group.truth]
 optional = true
 
 [tool.poetry.group.truth.dependencies]
 pandas = "^2.2.2"
 numpy = "^1.26.4"
```

### Comparing `hexital-1.1.1/PKG-INFO` & `hexital-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexital
-Version: 1.1.1
+Version: 1.1.2
 Summary: Hex Incremental Technical Analysis Library
 Home-page: https://github.com/MerlinR/Hexital
 License: MIT
 Keywords: trading,quant,indicators
 Author: Merlin Roe
 Author-email: merlin.roe@hotmail.co.uk
 Requires-Python: >=3.10,<4.0
@@ -224,31 +224,31 @@
 
 ## Testing
 
 Testing is a critical aspect of this library due to the complexity of ensuring the accuracy of generated indicator values. To achieve this, I rely on [Pandas-TA](https://github.com/twopirllc/pandas-ta) as the source of truth for indicator values. Each indicator added to this library undergoes testing, where the output is compared against the corresponding indicator output from Pandas-TA. Due to slight differences in calculations, particularly within NumPy, not all values are exactly identical. Therefore, if differences exceed a given threshold (usually beyond one decimal place), a Pearson correlation coefficient is calculated to ensure correct correlation with the expected output.
 
 ### Speed Tests
 
-The following charts illustrate the results and speed of Pandas-TA and Hexital in both bulk and incremental calculations. These results are obtained from running Pandas-TA and Hexital in bulk (_all candles calculated at once_) and incremental(_Caluclating after each new candle is added_) modes; charts _1 and 2_.
+The following charts illustrate the results and speed of Pandas-TA and Hexital in both bulk and incremental calculations. These results are obtained from running Pandas-TA and Hexital in bulk (_all candles calculated at once_) and incremental(_Caluclating after each new candle is added_) modes; chart _1_.
 
 The incremental charts demonstrate the process of calculating technical analysis, adding one candle at a time, and recalculating up to a specified number of candles. It's evident that using Pandas-TA, Pandas, and NumPy for incremental data processing incurs significant performance overhead. This is primarily due to the underlying behavior of NumPy, which involves reallocating memory when appending or concatenating data, rather than resizing it. As a result, it's recommended in NumPy and Pandas documentation to gather all data prior to running calculations. On the other hand, Hexital, being purely Pythonic, exhibits efficient performance both in bulk and incremental processing, with minimal to no additional overhead time. It significantly outperforms Pandas-TA in incremental processing and even surpasses Pandas-TA in speed, especially with smaller datasets.
 
-![EMA 10 test results.](tests/speed_tests/EMA_10.png)
+![EMA 10 test results.](tests/extra/speed_tests/EMA_10.png)
 
-From chart _(3)_, it's evident that in bulk calculations with an extremely large dataset, Pandas-TA outperforms Hexital. Pandas-TA maintains consistent performance, with processing times starting at 0.08 seconds for 1,000 candles and remaining stable at this level for 10,000 candles. In contrast, Hexital exhibits faster processing times, starting at 0.005 seconds for 1,000 candles but increasing to 0.05 seconds for 10,000 candles. While Hexital is initially faster, there is a noticeable growth in processing time as the dataset size increases. Therefore, for backtesting with a large dataset, Pandas-TA offers superior performance, while Hexital may experience slowdowns.
+From chart _(2)_, it's evident that in bulk calculations with an extremely large dataset, Pandas-TA outperforms Hexital. Pandas-TA maintains consistent performance, with processing times starting at 0.08 seconds for 1,000 candles and remaining stable at this level for 10,000 candles. In contrast, Hexital exhibits faster processing times, starting at 0.025 seconds for 2,000 candles but increasing to 0.16 seconds for 10,000 candles. While Hexital is initially faster, there is a noticeable growth in processing time as the dataset size increases. Therefore, for backtesting with a large dataset, Pandas-TA offers superior performance, while Hexital may experience slowdowns.
 
-![EMA 10 Bulk test results.](tests/speed_tests/EMA_10%20Bulk%20Calculations.png)
+![MACD 26 Bulk test results.](tests/extra/speed_tests/MACD_26_12_Bulk_Calculations.png)
 
-However referencing chart _(4)_ being an example of using both these libraries for a live application, whereby at n candles we incrementing a dataset with a candle and calculating the new TA; `Hexital` is far quicker. This is due to the speed that python can increment a list of data rather than Panda, as well as `Hexital` only needing to calculate the newest candle rather than having to re-calculate the entire dataset. Chart _3_ clearly shows the speed benefits it has over Pandas-TA and other Panda based Technical Analysis tools for incremental data sets.
+However referencing chart _(3)_ being an example of using both these libraries for a live incremental application, whereby at n candles we incrementing a dataset with a candle and calculating the new TA; `Hexital` is far quicker. This is due to the speed that python can increment a list of data rather than Panda, as well as `Hexital` only needing to calculate the newest candle rather than having to re-calculate the entire dataset. Chart _3_ clearly shows the speed benefits it has over Pandas-TA and other Panda based Technical Analysis tools for incremental data sets.
 
-![EMA 10 Real world usage.](tests/speed_tests/EMA_10_real_world.png)
+![MACD 26 Real world usage.](tests/extra/speed_tests/MACD_26_12_real_world.png)
 
 For reference, if using seconds Candle with 10,000 candles that is around 2 Hours 46 minutes.
 
 #### Note
 
-The code that produces these charts is: `tests/speed_tests/run_speed_test.py` and can be ran by calling `make speed-test`. Some noise is seen due to running on personal laptop while in use.
+The code that produces these charts is: `tests/extra/speed_tests/run_speed_test.py` and can be ran by calling `make speed-test`. Some noise is seen due to running on personal laptop while in use.
 
 ## Inspiration
 
 This library was inspired by [TALIpp](https://github.com/nardew/talipp), another Incremental Technical Analysis Library. However, I found the separate input lists rather cumbersome compared to working with an entire candle. Additionally, in TALIpp, outputs are separate entities, requiring extensive management. In contrast, Hexital stores all data within the candle, simplifying usage and management.
```


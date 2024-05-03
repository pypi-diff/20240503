# Comparing `tmp/moexalgo-1.0.1.tar.gz` & `tmp/moexalgo-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moexalgo-1.0.1.tar", last modified: Wed Oct 18 11:55:39 2023, max compression
+gzip compressed data, was "moexalgo-2.0.0.tar", last modified: Fri May  3 11:36:42 2024, max compression
```

## Comparing `moexalgo-1.0.1.tar` & `moexalgo-2.0.0.tar`

### file list

```diff
@@ -1,35 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 11:55:39.199729 moexalgo-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 11:55:39.183728 moexalgo-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 11:55:39.187728 moexalgo-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-10-18 11:55:21.000000 moexalgo-1.0.1/.github/workflows/python-publish_flow.yml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-10-18 11:55:21.000000 moexalgo-1.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2023-10-18 11:55:39.199729 moexalgo-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2023-10-18 11:55:21.000000 moexalgo-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 11:55:39.191728 moexalgo-1.0.1/moexalgo/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2023-10-18 11:55:21.000000 moexalgo-1.0.1/moexalgo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-18 11:55:39.000000 moexalgo-1.0.1/moexalgo/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2023-10-18 11:55:21.000000 moexalgo-1.0.1/moexalgo/candles.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-10-18 11:55:21.000000 moexalgo-1.0.1/moexalgo/indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     8643 2023-10-18 11:55:21.000000 moexalgo-1.0.1/moexalgo/market.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2023-10-18 11:55:21.000000 moexalgo-1.0.1/moexalgo/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 11:55:39.195728 moexalgo-1.0.1/moexalgo/models/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-10-18 11:55:21.000000 moexalgo-1.0.1/moexalgo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-10-18 11:55:21.000000 moexalgo-1.0.1/moexalgo/models/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2023-10-18 11:55:21.000000 moexalgo-1.0.1/moexalgo/models/indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2023-10-18 11:55:21.000000 moexalgo-1.0.1/moexalgo/models/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12982 2023-10-18 11:55:21.000000 moexalgo-1.0.1/moexalgo/models/shares.py
--rw-r--r--   0 runner    (1001) docker     (127)     7495 2023-10-18 11:55:21.000000 moexalgo-1.0.1/moexalgo/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2023-10-18 11:55:21.000000 moexalgo-1.0.1/moexalgo/shares.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2023-10-18 11:55:21.000000 moexalgo-1.0.1/moexalgo/tickers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2023-10-18 11:55:21.000000 moexalgo-1.0.1/moexalgo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 11:55:39.195728 moexalgo-1.0.1/moexalgo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2023-10-18 11:55:39.000000 moexalgo-1.0.1/moexalgo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      624 2023-10-18 11:55:39.000000 moexalgo-1.0.1/moexalgo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-18 11:55:39.000000 moexalgo-1.0.1/moexalgo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-18 11:55:39.000000 moexalgo-1.0.1/moexalgo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-18 11:55:39.000000 moexalgo-1.0.1/moexalgo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      776 2023-10-18 11:55:21.000000 moexalgo-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 11:55:39.199729 moexalgo-1.0.1/samples/
--rw-r--r--   0 runner    (1001) docker     (127)   304709 2023-10-18 11:55:21.000000 moexalgo-1.0.1/samples/quick_start.html
--rw-r--r--   0 runner    (1001) docker     (127)    53298 2023-10-18 11:55:21.000000 moexalgo-1.0.1/samples/quick_start.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-18 11:55:39.199729 moexalgo-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.988378 moexalgo-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.976378 moexalgo-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.976378 moexalgo-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-03 11:36:38.000000 moexalgo-2.0.0/.github/workflows/python-publish_flow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-03 11:36:38.000000 moexalgo-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-03 11:36:38.000000 moexalgo-2.0.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-03 11:36:38.000000 moexalgo-2.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-03 11:36:42.988378 moexalgo-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-03 11:36:38.000000 moexalgo-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.976378 moexalgo-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.980378 moexalgo-2.0.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.980378 moexalgo-2.0.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    48404 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/_static/newplot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34177 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/_static/output_4_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/candels.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.currency.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.futures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.indices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.market.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.models.common.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.models.indices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.models.shares.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.session.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.stocks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.tickers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-03 11:36:38.000000 moexalgo-2.0.0/docs/source/moexalgo.utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.984378 moexalgo-2.0.0/moexalgo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 11:36:42.000000 moexalgo-2.0.0/moexalgo/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/candles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13794 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24493 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/market.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.984378 moexalgo-2.0.0/moexalgo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/models/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/models/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/models/shares.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13962 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13607 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/stocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/tickers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-03 11:36:38.000000 moexalgo-2.0.0/moexalgo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.988378 moexalgo-2.0.0/moexalgo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-03 11:36:42.000000 moexalgo-2.0.0/moexalgo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-03 11:36:42.000000 moexalgo-2.0.0/moexalgo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:36:42.000000 moexalgo-2.0.0/moexalgo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 11:36:42.000000 moexalgo-2.0.0/moexalgo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 11:36:42.000000 moexalgo-2.0.0/moexalgo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-03 11:36:38.000000 moexalgo-2.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.984378 moexalgo-2.0.0/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 11:36:38.000000 moexalgo-2.0.0/samples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-03 11:36:38.000000 moexalgo-2.0.0/samples/auth.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-05-03 11:36:38.000000 moexalgo-2.0.0/samples/download_algopack_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   157564 2024-05-03 11:36:38.000000 moexalgo-2.0.0/samples/quick_start.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:36:42.988378 moexalgo-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:42.988378 moexalgo-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 11:36:38.000000 moexalgo-2.0.0/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-03 11:36:38.000000 moexalgo-2.0.0/tests/test_currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-03 11:36:38.000000 moexalgo-2.0.0/tests/test_futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-03 11:36:38.000000 moexalgo-2.0.0/tests/test_markets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-03 11:36:38.000000 moexalgo-2.0.0/tests/test_stocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:38.000000 moexalgo-2.0.0/tests/test_tickers.py
```

### Comparing `moexalgo-1.0.1/.github/workflows/python-publish_flow.yml` & `moexalgo-2.0.0/.github/workflows/python-publish_flow.yml`

 * *Files identical despite different names*

### Comparing `moexalgo-1.0.1/PKG-INFO` & `moexalgo-2.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,77 @@
-Metadata-Version: 2.1
-Name: moexalgo
-Version: 1.0.1
-Summary: Python lib for MOEX AlgoPack data
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Intended Audience :: Financial and Insurance Industry
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: httpx
-Provides-Extra: pandas
-Requires-Dist: pandas==1.4.1; extra == "pandas"
-
-# MoexAlgo: Получение уникальных данных от MOEX
-#### 100+ метрик
-
-<br>
-MoexAlgo предоставляет данные и аналитику по рынку акций Московской Биржи (MOEX).
-
-Можно получать:
-- Исторические данные - для тестирования торговых стратегий, проверки гипотез и бэктестов
-- Онлайн данные - для алгоритмической торговли
+# MoexAlgo: Получение уникальных данных MOEX ALGOPACK 📈
+
+### 🌐 [Сайт с полной документацией по продукту ALGOPACK](https://moexalgo.github.io/)
+
+<br>
+
+##### 🚀 MoexAlgo предоставляет данные и аналитику по рынку акций, фьючерсов и валют Московской Биржи (MOEX). 
+
+##### 📊 Более 100 уникальных метрик!
+
+##### С помощью ALGOPACK можно получать:
+- ###### Исторические данные - для тестирования торговых стратегий, проверки гипотез и бэктестов
+- ###### Онлайн данные - для алгоритмической торговли
 
 
 
 <br>
 [Changelog »](./CHANGELOG.md)
 <br><br>
 
-## MoexAlgo предоставляет три основных набора данных:
+## MoexAlgo предоставляет наборы данных:
 
-1.  `AlgoPack.TradeStats` - метрики, рассчитанные на потоке сделок: цены, объемы, соотношения покупок и продаж
-2.  `AlgoPack.OrderStats` - метрики, рассчитанные на потоке заявок: кол-во и объемы выставленных/снятых заявок
-3.  `AlgoPack.OBStats` - метрики, рассчитанные на стакане котировок: кол-во уровней цен, спреды, ликвидность и дисбаланс покупок/продаж
+* ⏰📊 Real-time market data 
+  1. 🕯️ `Candles` - свечи по тикеру за заданный период
+  2. 📚 `OrderBook` - стакан котировок по тикеру
 
-Также, можно получить справочную информацию по инструментам, свечи и прочую торговую статистику
+* 🚀🕯️ Super Candles
+  1.  💹 `TradeStats` - метрики, рассчитанные на потоке сделок: цены, объемы, соотношения покупок и продаж
+  2.  📊 `OrderStats` - метрики, рассчитанные на потоке заявок: кол-во и объемы выставленных/снятых заявок
+  3.   📈 `OBStats` - метрики, рассчитанные на стакане котировок: кол-во уровней цен, спреды, ликвидность и дисбаланс покупок/продаж
+* 🎯 `HI2` - Индекс рыночной концентрации 
+* 💼 `FUTOI` - Открытые позиции по фьючерсным контрактам в разрезе физ. и юр. лиц 
+
+Также, можно получить справочную информацию по инструментам, свечи и торговую статистику
 
 <br>
 
-## Пример использования
+## 🚀 Пример использования
+
+<hr>
+
+#### ⚡️ Быстрое знакомство с библиотекой MoexAlgo - [quick_start.ipynb](./samples/quick_start.ipynb)
+
+#### ⬇️ Получение данных через API - [download_algopack_data.ipynb](./samples/download_algopack_data.ipynb)
+
+#### 🔐 Пример авторизации - [auth.ipynb](./samples/auth.ipynb)
+<hr>
 
+Для работы с библиотекой необходимо авторизоваться на https://passport.moex.com
+
+```python
+from moexalgo import session
+
+username = "<email>"
+password = "<password>"
+
+session.authorize(username, password)
+
+```
+
+Чтобы получить доступ к полному набору данных, необходимо оформить бесплатную подписку на [странице](https://www.moex.com/ru/analyticalproducts?futoi) 
 
 ```python
 from moexalgo import Ticker
 
 # выбираем акции Сбера
 sber = Ticker('SBER')
 
 # получим дневные свечи с 2020 года
-sber.candles(date='2020-01-01', period='1d').head()
+sber.candles(start='2020-01-01', end='2023-11-01').head()
 ```
 
 <br>
 
 <div>
 <table border="1" class="dataframe">
   <thead>
@@ -130,30 +149,35 @@
 
 
 <br>
 Больше примеров смотрите в разделе samples
 
 <br>
 
-### Установка
+### 💻 Установка
 
 Установка с помощью `pip`:
 
 ``` bash
-$ pip install moexalgo
-
+pip install moexalgo
 ```
 
-### Requirements
+### 🔍 Requirements
 
 -   [Python](https://www.python.org) \>= 3.8+
 -   [pandas](https://github.com/pydata/pandas)
 -   [numpy](http://www.numpy.org) \>= 1.15.0
 
 
-### Вопросы?
+### 🤝 Комьюнити 
+
+- Самые важные новости ALGOPACK [подписывайтесь](https://t.me/moex_algopack_news)
+- Добавляйтесь в телеграмм-чат [ALGOPACK](https://t.me/moex_algopack)
+
+
+### ❓ Вопросы?
 
-Библиотека MoexAlgo будет дополняться. Если есть пожелания, идеи, замечания, пишите на <moexalgo@yandex.ru>
+Библиотека MoexAlgo будет дополняться. Если есть пожелания, идеи, замечания, пишите на <algopack@moex.com>
 
-### Licence
+### 📜 Licence
 
 Apache Software License
```

### Comparing `moexalgo-1.0.1/moexalgo/models/common.py` & `moexalgo-2.0.0/moexalgo/models/common.py`

 * *Files identical despite different names*

### Comparing `moexalgo-1.0.1/moexalgo/models/indices.py` & `moexalgo-2.0.0/moexalgo/models/indices.py`

 * *Files identical despite different names*

### Comparing `moexalgo-1.0.1/moexalgo/models/metrics.py` & `moexalgo-2.0.0/moexalgo/models/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# DEPRECATED!
 from dataclasses import dataclass
 from datetime import datetime
 from decimal import Decimal
 
 
 @dataclass
 class TradeStat:
```

### Comparing `moexalgo-1.0.1/moexalgo/models/shares.py` & `moexalgo-2.0.0/moexalgo/models/shares.py`

 * *Files identical despite different names*

### Comparing `moexalgo-1.0.1/pyproject.toml` & `moexalgo-2.0.0/pyproject.toml`

 * *Files identical despite different names*


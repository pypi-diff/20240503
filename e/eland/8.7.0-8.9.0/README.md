# Comparing `tmp/eland-8.7.0.tar.gz` & `tmp/eland-8.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/sethmlarson/eland/dist/.tmp-4ws7y1k1/eland-8.7.0.tar", last modified: Thu Mar 30 19:03:51 2023, max compression
+gzip compressed data, was "eland-8.9.0.tar", last modified: Thu Aug 24 13:59:35 2023, max compression
```

## Comparing `eland-8.7.0.tar` & `eland-8.9.0.tar`

### file list

```diff
@@ -1,70 +1,72 @@
-drwxrwxr-x   0 sethmlarson  (1000) sethmlarson  (1000)        0 2023-03-30 19:03:51.962687 eland-8.7.0/
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    11357 2021-09-21 15:47:58.000000 eland-8.7.0/LICENSE.txt
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)       61 2021-09-21 15:47:58.000000 eland-8.7.0/MANIFEST.in
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     2994 2021-09-21 15:47:58.000000 eland-8.7.0/NOTICE.txt
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    11734 2023-03-30 19:03:51.962687 eland-8.7.0/PKG-INFO
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    10377 2023-03-29 20:34:00.000000 eland-8.7.0/README.md
-drwxrwxr-x   0 sethmlarson  (1000) sethmlarson  (1000)        0 2023-03-30 19:03:51.942688 eland-8.7.0/bin/
--rwxrwxr-x   0 sethmlarson  (1000) sethmlarson  (1000)     7956 2022-07-08 12:51:07.000000 eland-8.7.0/bin/eland_import_hub_model
-drwxrwxr-x   0 sethmlarson  (1000) sethmlarson  (1000)        0 2023-03-30 19:03:51.950688 eland-8.7.0/eland/
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     1343 2021-09-21 15:47:58.000000 eland-8.7.0/eland/__init__.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     1149 2023-03-30 19:03:06.000000 eland-8.7.0/eland/_version.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     3619 2021-09-21 15:47:58.000000 eland-8.7.0/eland/actions.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     7421 2023-03-29 20:34:00.000000 eland-8.7.0/eland/arithmetics.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    15049 2023-03-29 20:34:00.000000 eland-8.7.0/eland/common.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     1276 2021-09-21 15:47:58.000000 eland-8.7.0/eland/conftest.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    81157 2021-12-09 21:14:18.000000 eland-8.7.0/eland/dataframe.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    21516 2022-02-10 20:33:35.000000 eland-8.7.0/eland/etl.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    32384 2022-02-10 20:33:35.000000 eland-8.7.0/eland/field_mappings.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     6290 2021-09-21 15:47:58.000000 eland-8.7.0/eland/filter.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    29060 2021-12-09 21:14:18.000000 eland-8.7.0/eland/groupby.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     3519 2021-09-21 15:47:58.000000 eland-8.7.0/eland/index.py
-drwxrwxr-x   0 sethmlarson  (1000) sethmlarson  (1000)        0 2023-03-30 19:03:51.954687 eland-8.7.0/eland/ml/
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)      880 2021-09-21 15:47:58.000000 eland-8.7.0/eland/ml/__init__.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     5841 2021-10-13 17:27:15.000000 eland-8.7.0/eland/ml/_model_serializer.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     4328 2021-09-21 15:47:58.000000 eland-8.7.0/eland/ml/_optional.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)      858 2021-09-21 15:47:58.000000 eland-8.7.0/eland/ml/common.py
-drwxrwxr-x   0 sethmlarson  (1000) sethmlarson  (1000)        0 2023-03-30 19:03:51.954687 eland-8.7.0/eland/ml/exporters/
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)      787 2023-03-29 20:34:00.000000 eland-8.7.0/eland/ml/exporters/__init__.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     8140 2023-03-29 20:34:00.000000 eland-8.7.0/eland/ml/exporters/_sklearn_deserializers.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     1712 2023-03-29 20:34:00.000000 eland-8.7.0/eland/ml/exporters/common.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    18086 2023-03-29 20:34:00.000000 eland-8.7.0/eland/ml/exporters/es_gb_models.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    19630 2023-03-29 20:34:00.000000 eland-8.7.0/eland/ml/ml_model.py
-drwxrwxr-x   0 sethmlarson  (1000) sethmlarson  (1000)        0 2023-03-30 19:03:51.958687 eland-8.7.0/eland/ml/pytorch/
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     1397 2022-07-08 12:51:07.000000 eland-8.7.0/eland/ml/pytorch/__init__.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     5673 2022-07-08 12:51:07.000000 eland-8.7.0/eland/ml/pytorch/_pytorch_model.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     9514 2023-03-29 20:34:00.000000 eland-8.7.0/eland/ml/pytorch/nlp_ml_model.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     1994 2022-07-08 12:51:07.000000 eland-8.7.0/eland/ml/pytorch/traceable_model.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    26677 2023-03-29 20:34:00.000000 eland-8.7.0/eland/ml/pytorch/transformers.py
-drwxrwxr-x   0 sethmlarson  (1000) sethmlarson  (1000)        0 2023-03-30 19:03:51.958687 eland-8.7.0/eland/ml/transformers/
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     3479 2023-03-29 20:34:00.000000 eland-8.7.0/eland/ml/transformers/__init__.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     1491 2021-09-21 15:47:58.000000 eland-8.7.0/eland/ml/transformers/base.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     9350 2021-10-13 17:27:15.000000 eland-8.7.0/eland/ml/transformers/lightgbm.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     9963 2022-07-08 12:51:07.000000 eland-8.7.0/eland/ml/transformers/sklearn.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     9811 2022-05-06 12:29:31.000000 eland-8.7.0/eland/ml/transformers/xgboost.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    23385 2023-03-29 20:34:00.000000 eland-8.7.0/eland/ndframe.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    58995 2023-03-29 20:34:00.000000 eland-8.7.0/eland/operations.py
-drwxrwxr-x   0 sethmlarson  (1000) sethmlarson  (1000)        0 2023-03-30 19:03:51.962687 eland-8.7.0/eland/plotting/
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     1088 2021-09-21 15:47:58.000000 eland-8.7.0/eland/plotting/__init__.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     3345 2021-12-09 21:14:18.000000 eland-8.7.0/eland/plotting/_core.py
-drwxrwxr-x   0 sethmlarson  (1000) sethmlarson  (1000)        0 2023-03-30 19:03:51.962687 eland-8.7.0/eland/plotting/_matplotlib/
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     1087 2021-09-21 15:47:58.000000 eland-8.7.0/eland/plotting/_matplotlib/__init__.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     4396 2021-12-09 20:28:41.000000 eland-8.7.0/eland/plotting/_matplotlib/hist.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)        0 2021-09-21 15:47:58.000000 eland-8.7.0/eland/py.typed
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    10798 2023-03-29 20:34:00.000000 eland-8.7.0/eland/query.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    27315 2023-03-29 20:34:00.000000 eland-8.7.0/eland/query_compiler.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    51331 2023-03-29 20:34:00.000000 eland-8.7.0/eland/series.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    12951 2021-09-21 15:47:58.000000 eland-8.7.0/eland/tasks.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     2321 2021-09-21 15:47:58.000000 eland-8.7.0/eland/utils.py
-drwxrwxr-x   0 sethmlarson  (1000) sethmlarson  (1000)        0 2023-03-30 19:03:51.950688 eland-8.7.0/eland.egg-info/
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    11734 2023-03-30 19:03:51.000000 eland-8.7.0/eland.egg-info/PKG-INFO
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     1374 2023-03-30 19:03:51.000000 eland-8.7.0/eland.egg-info/SOURCES.txt
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)        1 2023-03-30 19:03:51.000000 eland-8.7.0/eland.egg-info/dependency_links.txt
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)        1 2022-05-11 11:39:34.000000 eland-8.7.0/eland.egg-info/not-zip-safe
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)      419 2023-03-30 19:03:51.000000 eland-8.7.0/eland.egg-info/requires.txt
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)        6 2023-03-30 19:03:51.000000 eland-8.7.0/eland.egg-info/top_level.txt
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)      197 2023-03-30 19:03:51.962687 eland-8.7.0/setup.cfg
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     3297 2023-03-29 20:34:00.000000 eland-8.7.0/setup.py
-drwxrwxr-x   0 sethmlarson  (1000) sethmlarson  (1000)        0 2023-03-30 19:03:51.962687 eland-8.7.0/tests/
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     1631 2021-12-15 20:08:34.000000 eland-8.7.0/tests/test_common_pytest.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     1398 2021-09-21 15:47:58.000000 eland-8.7.0/tests/test_utils_pytest.py
+drwxrwxr-x   0 enrico    (1000) enrico    (1000)        0 2023-08-24 13:59:35.170328 eland-8.9.0/
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)    11357 2023-08-22 07:27:55.000000 eland-8.9.0/LICENSE.txt
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)       61 2023-08-22 07:27:55.000000 eland-8.9.0/MANIFEST.in
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     2994 2023-08-22 07:27:55.000000 eland-8.9.0/NOTICE.txt
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)    12538 2023-08-24 13:59:35.170328 eland-8.9.0/PKG-INFO
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)    11166 2023-08-22 07:27:55.000000 eland-8.9.0/README.md
+drwxrwxr-x   0 enrico    (1000) enrico    (1000)        0 2023-08-24 13:59:35.166328 eland-8.9.0/eland/
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     1343 2023-08-24 09:17:09.000000 eland-8.9.0/eland/__init__.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     1164 2023-08-24 09:17:12.000000 eland-8.9.0/eland/_version.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     3619 2023-08-22 07:27:55.000000 eland-8.9.0/eland/actions.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     7421 2023-08-22 07:27:55.000000 eland-8.9.0/eland/arithmetics.py
+drwxrwxr-x   0 enrico    (1000) enrico    (1000)        0 2023-08-24 13:59:35.166328 eland-8.9.0/eland/cli/
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)      787 2023-08-22 07:27:55.000000 eland-8.9.0/eland/cli/__init__.py
+-rwxrwxr-x   0 enrico    (1000) enrico    (1000)     9355 2023-08-22 07:27:55.000000 eland-8.9.0/eland/cli/eland_import_hub_model.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)    15206 2023-08-22 07:27:55.000000 eland-8.9.0/eland/common.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     1276 2023-08-22 07:27:55.000000 eland-8.9.0/eland/conftest.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)    81157 2023-08-22 07:27:55.000000 eland-8.9.0/eland/dataframe.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)    21516 2023-08-22 07:27:55.000000 eland-8.9.0/eland/etl.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)    33721 2023-08-22 07:27:55.000000 eland-8.9.0/eland/field_mappings.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     6290 2023-08-22 07:27:55.000000 eland-8.9.0/eland/filter.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)    29060 2023-08-22 07:27:55.000000 eland-8.9.0/eland/groupby.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     3519 2023-08-22 07:27:55.000000 eland-8.9.0/eland/index.py
+drwxrwxr-x   0 enrico    (1000) enrico    (1000)        0 2023-08-24 13:59:35.166328 eland-8.9.0/eland/ml/
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)      880 2023-08-22 07:27:55.000000 eland-8.9.0/eland/ml/__init__.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     5841 2023-08-22 07:27:55.000000 eland-8.9.0/eland/ml/_model_serializer.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     4328 2023-08-22 07:27:55.000000 eland-8.9.0/eland/ml/_optional.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)      858 2023-08-22 07:27:55.000000 eland-8.9.0/eland/ml/common.py
+drwxrwxr-x   0 enrico    (1000) enrico    (1000)        0 2023-08-24 13:59:35.166328 eland-8.9.0/eland/ml/exporters/
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)      787 2023-08-22 07:27:55.000000 eland-8.9.0/eland/ml/exporters/__init__.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     8303 2023-08-22 07:27:55.000000 eland-8.9.0/eland/ml/exporters/_sklearn_deserializers.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     1712 2023-08-22 07:27:55.000000 eland-8.9.0/eland/ml/exporters/common.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)    18086 2023-08-22 07:27:55.000000 eland-8.9.0/eland/ml/exporters/es_gb_models.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)    19630 2023-08-22 07:27:55.000000 eland-8.9.0/eland/ml/ml_model.py
+drwxrwxr-x   0 enrico    (1000) enrico    (1000)        0 2023-08-24 13:59:35.166328 eland-8.9.0/eland/ml/pytorch/
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     1436 2023-08-22 07:27:55.000000 eland-8.9.0/eland/ml/pytorch/__init__.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     5662 2023-08-22 07:27:55.000000 eland-8.9.0/eland/ml/pytorch/_pytorch_model.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)    10924 2023-08-22 07:27:55.000000 eland-8.9.0/eland/ml/pytorch/nlp_ml_model.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     2072 2023-08-22 07:27:55.000000 eland-8.9.0/eland/ml/pytorch/traceable_model.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)    31387 2023-08-22 07:27:55.000000 eland-8.9.0/eland/ml/pytorch/transformers.py
+drwxrwxr-x   0 enrico    (1000) enrico    (1000)        0 2023-08-24 13:59:35.166328 eland-8.9.0/eland/ml/transformers/
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     3479 2023-08-22 07:27:55.000000 eland-8.9.0/eland/ml/transformers/__init__.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     1491 2023-08-22 07:27:55.000000 eland-8.9.0/eland/ml/transformers/base.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     9350 2023-08-22 07:27:55.000000 eland-8.9.0/eland/ml/transformers/lightgbm.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     9963 2023-08-22 07:27:55.000000 eland-8.9.0/eland/ml/transformers/sklearn.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     9811 2023-08-22 07:27:55.000000 eland-8.9.0/eland/ml/transformers/xgboost.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)    23385 2023-08-22 07:27:55.000000 eland-8.9.0/eland/ndframe.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)    58995 2023-08-22 07:27:55.000000 eland-8.9.0/eland/operations.py
+drwxrwxr-x   0 enrico    (1000) enrico    (1000)        0 2023-08-24 13:59:35.166328 eland-8.9.0/eland/plotting/
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     1088 2023-08-22 07:27:55.000000 eland-8.9.0/eland/plotting/__init__.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     3345 2023-08-22 07:27:55.000000 eland-8.9.0/eland/plotting/_core.py
+drwxrwxr-x   0 enrico    (1000) enrico    (1000)        0 2023-08-24 13:59:35.166328 eland-8.9.0/eland/plotting/_matplotlib/
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     1087 2023-08-22 07:27:55.000000 eland-8.9.0/eland/plotting/_matplotlib/__init__.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     4396 2023-08-22 07:27:55.000000 eland-8.9.0/eland/plotting/_matplotlib/hist.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)        0 2023-08-22 07:27:55.000000 eland-8.9.0/eland/py.typed
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)    10798 2023-08-22 07:27:55.000000 eland-8.9.0/eland/query.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)    27315 2023-08-22 07:27:55.000000 eland-8.9.0/eland/query_compiler.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)    51458 2023-08-24 08:39:10.000000 eland-8.9.0/eland/series.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)    12951 2023-08-22 07:27:55.000000 eland-8.9.0/eland/tasks.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     2321 2023-08-22 07:27:55.000000 eland-8.9.0/eland/utils.py
+drwxrwxr-x   0 enrico    (1000) enrico    (1000)        0 2023-08-24 13:59:35.166328 eland-8.9.0/eland.egg-info/
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)    12538 2023-08-24 13:59:35.000000 eland-8.9.0/eland.egg-info/PKG-INFO
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     1437 2023-08-24 13:59:35.000000 eland-8.9.0/eland.egg-info/SOURCES.txt
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)        1 2023-08-24 13:59:35.000000 eland-8.9.0/eland.egg-info/dependency_links.txt
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)       81 2023-08-24 13:59:35.000000 eland-8.9.0/eland.egg-info/entry_points.txt
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)        1 2023-08-22 10:44:16.000000 eland-8.9.0/eland.egg-info/not-zip-safe
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)      421 2023-08-24 13:59:35.000000 eland-8.9.0/eland.egg-info/requires.txt
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)        6 2023-08-24 13:59:35.000000 eland-8.9.0/eland.egg-info/top_level.txt
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)      197 2023-08-24 13:59:35.170328 eland-8.9.0/setup.cfg
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     3377 2023-08-22 07:27:55.000000 eland-8.9.0/setup.py
+drwxrwxr-x   0 enrico    (1000) enrico    (1000)        0 2023-08-24 13:59:35.170328 eland-8.9.0/tests/
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     1631 2023-08-22 07:27:55.000000 eland-8.9.0/tests/test_common_pytest.py
+-rw-rw-r--   0 enrico    (1000) enrico    (1000)     1398 2023-08-22 07:27:55.000000 eland-8.9.0/tests/test_utils_pytest.py
```

### Comparing `eland-8.7.0/LICENSE.txt` & `eland-8.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/NOTICE.txt` & `eland-8.9.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/PKG-INFO` & `eland-8.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: eland
-Version: 8.7.0
+Version: 8.9.0
 Summary: Python Client and Toolkit for DataFrames, Big Data, Machine Learning and ETL in Elasticsearch
 Home-page: https://github.com/elastic/eland
 Author: Steve Dodson
 Author-email: steve.dodson@elastic.co
-Maintainer: Seth Michael Larson
-Maintainer-email: seth.larson@elastic.co
+Maintainer: Elastic Client Library Maintainers
+Maintainer-email: client-libs@elastic.co
 License: Apache-2.0
 Keywords: elastic eland pandas python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -81,21 +81,22 @@
 
 ```bash
 $ conda install -c conda-forge eland
 ```
 
 ### Compatibility
 
-- Supports Python 3.8+ and Pandas 1.5
+- Supports Python 3.8, 3.9, 3.10 and Pandas 1.5
 - Supports Elasticsearch clusters that are 7.11+, recommended 8.3 or later for all features to work.
   If you are using the NLP with PyTorch feature make sure your Eland minor version matches the minor 
   version of your Elasticsearch cluster. For all other features it is sufficient for the major versions
   to match.
-- You need to use PyTorch `1.11.0` or earlier to import an NLP model. 
-  Run `pip install torch==1.11` to install the aproppriate version of PyTorch.
+- You need to use PyTorch `1.13.1` or earlier to import an NLP model. 
+  Run `pip install torch==1.13.1` to install the aproppriate version of PyTorch.
+  
 
 ### Prerequisites
 
 Users installing Eland on Debian-based distributions may need to install prerequisite packages for the transitive
 dependencies of Eland:
 
 ```bash
@@ -126,16 +127,15 @@
 
 ```bash
 $ docker run -it --rm --network host \
     elastic/eland \
     eland_import_hub_model \
       --url http://host.docker.internal:9200/ \
       --hub-model-id elastic/distilbert-base-cased-finetuned-conll03-english \
-      --task-type ner \
-      --start
+      --task-type ner
 ```
 
 ### Connecting to Elasticsearch 
 
 Eland uses the [Elasticsearch low level client](https://elasticsearch-py.readthedocs.io) to connect to Elasticsearch. 
 This client supports a range of [connection options and authentication options](https://elasticsearch-py.readthedocs.io/en/stable/api.html#elasticsearch). 
 
@@ -269,32 +269,46 @@
 $ eland_import_hub_model \
   --url http://localhost:9200/ \
   --hub-model-id elastic/distilbert-base-cased-finetuned-conll03-english \
   --task-type ner \
   --start
 ```
 
+The example above will automatically start a model deployment. This is a
+good shortcut for initial experimentation, but for anything that needs
+good throughput you should omit the `--start` argument from the Eland
+command line and instead start the model using the ML UI in Kibana.
+The `--start` argument will deploy the model with one allocation and one
+thread per allocation, which will not offer good performance. When starting
+the model deployment using the ML UI in Kibana or the Elasticsearch
+[API](https://www.elastic.co/guide/en/elasticsearch/reference/current/start-trained-model-deployment.html)
+you will be able to set the threading options to make the best use of your
+hardware.
+
 ```python
 >>> import elasticsearch
 >>> from pathlib import Path
+>>> from eland.common import es_version
 >>> from eland.ml.pytorch import PyTorchModel
 >>> from eland.ml.pytorch.transformers import TransformerModel
 
+>>> es = elasticsearch.Elasticsearch("http://elastic:mlqa_admin@localhost:9200")
+>>> es_cluster_version = es_version(es)
+
 # Load a Hugging Face transformers model directly from the model hub
->>> tm = TransformerModel("elastic/distilbert-base-cased-finetuned-conll03-english", "ner")
+>>> tm = TransformerModel(model_id="elastic/distilbert-base-cased-finetuned-conll03-english", task_type="ner", es_version=es_cluster_version)
 Downloading: 100%|██████████| 257/257 [00:00<00:00, 108kB/s]
 Downloading: 100%|██████████| 954/954 [00:00<00:00, 372kB/s]
 Downloading: 100%|██████████| 208k/208k [00:00<00:00, 668kB/s] 
 Downloading: 100%|██████████| 112/112 [00:00<00:00, 43.9kB/s]
 Downloading: 100%|██████████| 249M/249M [00:23<00:00, 11.2MB/s]
 
 # Export the model in a TorchScrpt representation which Elasticsearch uses
 >>> tmp_path = "models"
 >>> Path(tmp_path).mkdir(parents=True, exist_ok=True)
 >>> model_path, config, vocab_path = tm.save(tmp_path)
 
 # Import model into Elasticsearch
->>> es = elasticsearch.Elasticsearch("http://elastic:mlqa_admin@localhost:9200", timeout=300)  # 5 minute timeout
 >>> ptm = PyTorchModel(es, tm.elasticsearch_model_id())
 >>> ptm.import_model(model_path=model_path, config_path=None, vocab_path=vocab_path, config=config)
 100%|██████████| 63/63 [00:12<00:00,  5.02it/s]
 ```
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: eland Version: 8.7.0 Summary: Python Client and
+Metadata-Version: 2.1 Name: eland Version: 8.9.0 Summary: Python Client and
 Toolkit for DataFrames, Big Data, Machine Learning and ETL in Elasticsearch
 Home-page: https://github.com/elastic/eland Author: Steve Dodson Author-email:
-steve.dodson@elastic.co Maintainer: Seth Michael Larson Maintainer-email:
-seth.larson@elastic.co License: Apache-2.0 Keywords: elastic eland pandas
-python Classifier: Development Status :: 5 - Production/Stable Classifier:
-License :: OSI Approved :: Apache Software License Classifier: Environment ::
-Console Classifier: Operating System :: OS Independent Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Topic :: Scientific/Engineering Requires-Python:
->=3.8 Description-Content-Type: text/markdown Provides-Extra: xgboost Provides-
-Extra: scikit-learn Provides-Extra: lightgbm Provides-Extra: pytorch Provides-
-Extra: all License-File: LICENSE.txt License-File: NOTICE.txt
+steve.dodson@elastic.co Maintainer: Elastic Client Library Maintainers
+Maintainer-email: client-libs@elastic.co License: Apache-2.0 Keywords: elastic
+eland pandas python Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Environment :: Console Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Science/Research Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
+xgboost Provides-Extra: scikit-learn Provides-Extra: lightgbm Provides-Extra:
+pytorch Provides-Extra: all License-File: LICENSE.txt License-File: NOTICE.txt
                                     _[_E_l_a_n_d_]
 
 _[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_C_o_n_d_a_ _V_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]_[_P_a_c_k_a_g_e_ _S_t_a_t_u_s_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]
                             _[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]
 ## About Eland is a Python Elasticsearch client for exploring and analyzing
 data in Elasticsearch with a familiar Pandas-compatible API. Where possible the
 package uses existing Python APIs and data structures to make it easy to switch
@@ -29,60 +29,60 @@
 provides tools to upload trained machine learning models from common libraries
 like [scikit-learn](https://scikit-learn.org), [XGBoost](https://
 xgboost.readthedocs.io), and [LightGBM](https://lightgbm.readthedocs.io) into
 Elasticsearch. ## Getting Started Eland can be installed from [PyPI](https://
 pypi.org/project/eland) with Pip: ```bash $ python -m pip install eland ```
 Eland can also be installed from [Conda Forge](https://anaconda.org/conda-
 forge/eland) with Conda: ```bash $ conda install -c conda-forge eland ``` ###
-Compatibility - Supports Python 3.8+ and Pandas 1.5 - Supports Elasticsearch
-clusters that are 7.11+, recommended 8.3 or later for all features to work. If
-you are using the NLP with PyTorch feature make sure your Eland minor version
-matches the minor version of your Elasticsearch cluster. For all other features
-it is sufficient for the major versions to match. - You need to use PyTorch
-`1.11.0` or earlier to import an NLP model. Run `pip install torch==1.11` to
-install the aproppriate version of PyTorch. ### Prerequisites Users installing
-Eland on Debian-based distributions may need to install prerequisite packages
-for the transitive dependencies of Eland: ```bash $ sudo apt-get install -y \
-build-essential pkg-config cmake \ python3-dev libzip-dev libjpeg-dev ``` Note
-that other distributions such as CentOS, RedHat, Arch, etc. may require using a
-different package manager and specifying different package names. ### Docker
-Users wishing to use Eland without installing it, in order to just run the
-available scripts, can build the Docker container: ```bash $ docker build -
-t elastic/eland . ``` The container can now be used interactively: ```bash $
-docker run -it --rm --network host elastic/eland ``` Running installed scripts
-is also possible without an interactive shell, e.g.: ```bash $ docker run -it -
--rm --network host \ elastic/eland \ eland_import_hub_model \ --url http://
-host.docker.internal:9200/ \ --hub-model-id elastic/distilbert-base-cased-
-finetuned-conll03-english \ --task-type ner \ --start ``` ### Connecting to
-Elasticsearch Eland uses the [Elasticsearch low level client](https://
-elasticsearch-py.readthedocs.io) to connect to Elasticsearch. This client
-supports a range of [connection options and authentication options](https://
-elasticsearch-py.readthedocs.io/en/stable/api.html#elasticsearch). You can pass
-either an instance of `elasticsearch.Elasticsearch` to Eland APIs or a string
-containing the host to connect to: ```python import eland as ed # Connecting to
-an Elasticsearch instance running on 'localhost:9200' df = ed.DataFrame
-("localhost:9200", es_index_pattern="flights") # Connecting to an Elastic Cloud
-instance from elasticsearch import Elasticsearch es = Elasticsearch
-( cloud_id="cluster-name:...", http_auth=("elastic", "") ) df = ed.DataFrame
-(es, es_index_pattern="flights") ``` ## DataFrames in Eland `eland.DataFrame`
-wraps an Elasticsearch index in a Pandas-like API and defers all processing and
-filtering of data to Elasticsearch instead of your local machine. This means
-you can process large amounts of data within Elasticsearch from a Jupyter
-Notebook without overloading your machine. â¤ [Eland DataFrame API
-documentation](https://eland.readthedocs.io/en/latest/reference/dataframe.html)
-â¤ [Advanced examples in a Jupyter Notebook](https://eland.readthedocs.io/en/
-latest/examples/demo_notebook.html) ```python >>> import eland as ed >>> #
-Connect to 'flights' index via localhost Elasticsearch node >>> df =
-ed.DataFrame('localhost:9200', 'flights') # eland.DataFrame instance has the
-same API as pandas.DataFrame # except all data is in Elasticsearch. See .info()
-memory usage. >>> df.head() AvgTicketPrice Cancelled ... dayOfWeek timestamp 0
-841.265642 False ... 0 2018-01-01 00:00:00 1 882.982662 False ... 0 2018-01-01
-18:27:00 2 190.636904 False ... 0 2018-01-01 17:11:14 3 181.694216 True ... 0
-2018-01-01 10:33:28 4 730.041778 False ... 0 2018-01-01 05:13:00 [5 rows x 27
-columns] >>> df.info()
+Compatibility - Supports Python 3.8, 3.9, 3.10 and Pandas 1.5 - Supports
+Elasticsearch clusters that are 7.11+, recommended 8.3 or later for all
+features to work. If you are using the NLP with PyTorch feature make sure your
+Eland minor version matches the minor version of your Elasticsearch cluster.
+For all other features it is sufficient for the major versions to match. - You
+need to use PyTorch `1.13.1` or earlier to import an NLP model. Run `pip
+install torch==1.13.1` to install the aproppriate version of PyTorch. ###
+Prerequisites Users installing Eland on Debian-based distributions may need to
+install prerequisite packages for the transitive dependencies of Eland: ```bash
+$ sudo apt-get install -y \ build-essential pkg-config cmake \ python3-dev
+libzip-dev libjpeg-dev ``` Note that other distributions such as CentOS,
+RedHat, Arch, etc. may require using a different package manager and specifying
+different package names. ### Docker Users wishing to use Eland without
+installing it, in order to just run the available scripts, can build the Docker
+container: ```bash $ docker build -t elastic/eland . ``` The container can now
+be used interactively: ```bash $ docker run -it --rm --network host elastic/
+eland ``` Running installed scripts is also possible without an interactive
+shell, e.g.: ```bash $ docker run -it --rm --network host \ elastic/eland \
+eland_import_hub_model \ --url http://host.docker.internal:9200/ \ --hub-model-
+id elastic/distilbert-base-cased-finetuned-conll03-english \ --task-type ner
+``` ### Connecting to Elasticsearch Eland uses the [Elasticsearch low level
+client](https://elasticsearch-py.readthedocs.io) to connect to Elasticsearch.
+This client supports a range of [connection options and authentication options]
+(https://elasticsearch-py.readthedocs.io/en/stable/api.html#elasticsearch). You
+can pass either an instance of `elasticsearch.Elasticsearch` to Eland APIs or a
+string containing the host to connect to: ```python import eland as ed #
+Connecting to an Elasticsearch instance running on 'localhost:9200' df =
+ed.DataFrame("localhost:9200", es_index_pattern="flights") # Connecting to an
+Elastic Cloud instance from elasticsearch import Elasticsearch es =
+Elasticsearch( cloud_id="cluster-name:...", http_auth=("elastic", "") ) df =
+ed.DataFrame(es, es_index_pattern="flights") ``` ## DataFrames in Eland
+`eland.DataFrame` wraps an Elasticsearch index in a Pandas-like API and defers
+all processing and filtering of data to Elasticsearch instead of your local
+machine. This means you can process large amounts of data within Elasticsearch
+from a Jupyter Notebook without overloading your machine. â¤ [Eland DataFrame
+API documentation](https://eland.readthedocs.io/en/latest/reference/
+dataframe.html) â¤ [Advanced examples in a Jupyter Notebook](https://
+eland.readthedocs.io/en/latest/examples/demo_notebook.html) ```python >>>
+import eland as ed >>> # Connect to 'flights' index via localhost Elasticsearch
+node >>> df = ed.DataFrame('localhost:9200', 'flights') # eland.DataFrame
+instance has the same API as pandas.DataFrame # except all data is in
+Elasticsearch. See .info() memory usage. >>> df.head() AvgTicketPrice Cancelled
+... dayOfWeek timestamp 0 841.265642 False ... 0 2018-01-01 00:00:00 1
+882.982662 False ... 0 2018-01-01 18:27:00 2 190.636904 False ... 0 2018-01-01
+17:11:14 3 181.694216 True ... 0 2018-01-01 10:33:28 4 730.041778 False ... 0
+2018-01-01 05:13:00 [5 rows x 27 columns] >>> df.info()
 eland.dataframe.DataFrame'> Index: 13059 entries, 0 to 13058 Data columns
 (total 27 columns): # Column Non-Null Count Dtype --- ------ -------------- ---
 -- 0 AvgTicketPrice 13059 non-null float64 1 Cancelled 13059 non-null bool 2
 Carrier 13059 non-null object ... 24 OriginWeather 13059 non-null object 25
 dayOfWeek 13059 non-null int64 26 timestamp 13059 non-null datetime64[ns]
 dtypes: bool(2), datetime64[ns](1), float64(5), int64(2), object(17) memory
 usage: 80.0 bytes Elasticsearch storage usage: 5.043 MB # Filtering of rows
@@ -111,26 +111,36 @@
 Elasticsearch with the training data >>> es_model.predict(training_data[0]) [0
 1 1 0 1 0 0 0 1 0] ``` ### NLP with PyTorch For NLP tasks, Eland allows
 importing PyTorch trained BERT models into Elasticsearch. Models can be either
 plain PyTorch models, or supported [transformers](https://huggingface.co/
 transformers) models from the [Hugging Face model hub](https://huggingface.co/
 models). ```bash $ eland_import_hub_model \ --url http://localhost:9200/ \ --
 hub-model-id elastic/distilbert-base-cased-finetuned-conll03-english \ --task-
-type ner \ --start ``` ```python >>> import elasticsearch >>> from pathlib
-import Path >>> from eland.ml.pytorch import PyTorchModel >>> from
-eland.ml.pytorch.transformers import TransformerModel # Load a Hugging Face
-transformers model directly from the model hub >>> tm = TransformerModel
-("elastic/distilbert-base-cased-finetuned-conll03-english", "ner") Downloading:
+type ner \ --start ``` The example above will automatically start a model
+deployment. This is a good shortcut for initial experimentation, but for
+anything that needs good throughput you should omit the `--start` argument from
+the Eland command line and instead start the model using the ML UI in Kibana.
+The `--start` argument will deploy the model with one allocation and one thread
+per allocation, which will not offer good performance. When starting the model
+deployment using the ML UI in Kibana or the Elasticsearch [API](https://
+www.elastic.co/guide/en/elasticsearch/reference/current/start-trained-model-
+deployment.html) you will be able to set the threading options to make the best
+use of your hardware. ```python >>> import elasticsearch >>> from pathlib
+import Path >>> from eland.common import es_version >>> from eland.ml.pytorch
+import PyTorchModel >>> from eland.ml.pytorch.transformers import
+TransformerModel >>> es = elasticsearch.Elasticsearch("http://elastic:
+mlqa_admin@localhost:9200") >>> es_cluster_version = es_version(es) # Load a
+Hugging Face transformers model directly from the model hub >>> tm =
+TransformerModel(model_id="elastic/distilbert-base-cased-finetuned-conll03-
+english", task_type="ner", es_version=es_cluster_version) Downloading:
 100%|ââââââââââ| 257/257 [00:00<00:00, 108kB/s]
 Downloading: 100%|ââââââââââ| 954/954 [00:00<00:00, 372kB/
 s] Downloading: 100%|ââââââââââ| 208k/208k [00:00<00:00,
 668kB/s] Downloading: 100%|ââââââââââ| 112/112 [00:00<00:
 00, 43.9kB/s] Downloading: 100%|ââââââââââ| 249M/249M [00:
 23<00:00, 11.2MB/s] # Export the model in a TorchScrpt representation which
 Elasticsearch uses >>> tmp_path = "models" >>> Path(tmp_path).mkdir
 (parents=True, exist_ok=True) >>> model_path, config, vocab_path = tm.save
-(tmp_path) # Import model into Elasticsearch >>> es =
-elasticsearch.Elasticsearch("http://elastic:mlqa_admin@localhost:9200",
-timeout=300) # 5 minute timeout >>> ptm = PyTorchModel(es,
+(tmp_path) # Import model into Elasticsearch >>> ptm = PyTorchModel(es,
 tm.elasticsearch_model_id()) >>> ptm.import_model(model_path=model_path,
 config_path=None, vocab_path=vocab_path, config=config)
 100%|ââââââââââ| 63/63 [00:12<00:00, 5.02it/s] ```
```

### Comparing `eland-8.7.0/README.md` & `eland-8.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -45,21 +45,22 @@
 
 ```bash
 $ conda install -c conda-forge eland
 ```
 
 ### Compatibility
 
-- Supports Python 3.8+ and Pandas 1.5
+- Supports Python 3.8, 3.9, 3.10 and Pandas 1.5
 - Supports Elasticsearch clusters that are 7.11+, recommended 8.3 or later for all features to work.
   If you are using the NLP with PyTorch feature make sure your Eland minor version matches the minor 
   version of your Elasticsearch cluster. For all other features it is sufficient for the major versions
   to match.
-- You need to use PyTorch `1.11.0` or earlier to import an NLP model. 
-  Run `pip install torch==1.11` to install the aproppriate version of PyTorch.
+- You need to use PyTorch `1.13.1` or earlier to import an NLP model. 
+  Run `pip install torch==1.13.1` to install the aproppriate version of PyTorch.
+  
 
 ### Prerequisites
 
 Users installing Eland on Debian-based distributions may need to install prerequisite packages for the transitive
 dependencies of Eland:
 
 ```bash
@@ -90,16 +91,15 @@
 
 ```bash
 $ docker run -it --rm --network host \
     elastic/eland \
     eland_import_hub_model \
       --url http://host.docker.internal:9200/ \
       --hub-model-id elastic/distilbert-base-cased-finetuned-conll03-english \
-      --task-type ner \
-      --start
+      --task-type ner
 ```
 
 ### Connecting to Elasticsearch 
 
 Eland uses the [Elasticsearch low level client](https://elasticsearch-py.readthedocs.io) to connect to Elasticsearch. 
 This client supports a range of [connection options and authentication options](https://elasticsearch-py.readthedocs.io/en/stable/api.html#elasticsearch). 
 
@@ -233,32 +233,46 @@
 $ eland_import_hub_model \
   --url http://localhost:9200/ \
   --hub-model-id elastic/distilbert-base-cased-finetuned-conll03-english \
   --task-type ner \
   --start
 ```
 
+The example above will automatically start a model deployment. This is a
+good shortcut for initial experimentation, but for anything that needs
+good throughput you should omit the `--start` argument from the Eland
+command line and instead start the model using the ML UI in Kibana.
+The `--start` argument will deploy the model with one allocation and one
+thread per allocation, which will not offer good performance. When starting
+the model deployment using the ML UI in Kibana or the Elasticsearch
+[API](https://www.elastic.co/guide/en/elasticsearch/reference/current/start-trained-model-deployment.html)
+you will be able to set the threading options to make the best use of your
+hardware.
+
 ```python
 >>> import elasticsearch
 >>> from pathlib import Path
+>>> from eland.common import es_version
 >>> from eland.ml.pytorch import PyTorchModel
 >>> from eland.ml.pytorch.transformers import TransformerModel
 
+>>> es = elasticsearch.Elasticsearch("http://elastic:mlqa_admin@localhost:9200")
+>>> es_cluster_version = es_version(es)
+
 # Load a Hugging Face transformers model directly from the model hub
->>> tm = TransformerModel("elastic/distilbert-base-cased-finetuned-conll03-english", "ner")
+>>> tm = TransformerModel(model_id="elastic/distilbert-base-cased-finetuned-conll03-english", task_type="ner", es_version=es_cluster_version)
 Downloading: 100%|██████████| 257/257 [00:00<00:00, 108kB/s]
 Downloading: 100%|██████████| 954/954 [00:00<00:00, 372kB/s]
 Downloading: 100%|██████████| 208k/208k [00:00<00:00, 668kB/s] 
 Downloading: 100%|██████████| 112/112 [00:00<00:00, 43.9kB/s]
 Downloading: 100%|██████████| 249M/249M [00:23<00:00, 11.2MB/s]
 
 # Export the model in a TorchScrpt representation which Elasticsearch uses
 >>> tmp_path = "models"
 >>> Path(tmp_path).mkdir(parents=True, exist_ok=True)
 >>> model_path, config, vocab_path = tm.save(tmp_path)
 
 # Import model into Elasticsearch
->>> es = elasticsearch.Elasticsearch("http://elastic:mlqa_admin@localhost:9200", timeout=300)  # 5 minute timeout
 >>> ptm = PyTorchModel(es, tm.elasticsearch_model_id())
 >>> ptm.import_model(model_path=model_path, config_path=None, vocab_path=vocab_path, config=config)
 100%|██████████| 63/63 [00:12<00:00,  5.02it/s]
 ```
```

#### html2text {}

```diff
@@ -11,60 +11,60 @@
 provides tools to upload trained machine learning models from common libraries
 like [scikit-learn](https://scikit-learn.org), [XGBoost](https://
 xgboost.readthedocs.io), and [LightGBM](https://lightgbm.readthedocs.io) into
 Elasticsearch. ## Getting Started Eland can be installed from [PyPI](https://
 pypi.org/project/eland) with Pip: ```bash $ python -m pip install eland ```
 Eland can also be installed from [Conda Forge](https://anaconda.org/conda-
 forge/eland) with Conda: ```bash $ conda install -c conda-forge eland ``` ###
-Compatibility - Supports Python 3.8+ and Pandas 1.5 - Supports Elasticsearch
-clusters that are 7.11+, recommended 8.3 or later for all features to work. If
-you are using the NLP with PyTorch feature make sure your Eland minor version
-matches the minor version of your Elasticsearch cluster. For all other features
-it is sufficient for the major versions to match. - You need to use PyTorch
-`1.11.0` or earlier to import an NLP model. Run `pip install torch==1.11` to
-install the aproppriate version of PyTorch. ### Prerequisites Users installing
-Eland on Debian-based distributions may need to install prerequisite packages
-for the transitive dependencies of Eland: ```bash $ sudo apt-get install -y \
-build-essential pkg-config cmake \ python3-dev libzip-dev libjpeg-dev ``` Note
-that other distributions such as CentOS, RedHat, Arch, etc. may require using a
-different package manager and specifying different package names. ### Docker
-Users wishing to use Eland without installing it, in order to just run the
-available scripts, can build the Docker container: ```bash $ docker build -
-t elastic/eland . ``` The container can now be used interactively: ```bash $
-docker run -it --rm --network host elastic/eland ``` Running installed scripts
-is also possible without an interactive shell, e.g.: ```bash $ docker run -it -
--rm --network host \ elastic/eland \ eland_import_hub_model \ --url http://
-host.docker.internal:9200/ \ --hub-model-id elastic/distilbert-base-cased-
-finetuned-conll03-english \ --task-type ner \ --start ``` ### Connecting to
-Elasticsearch Eland uses the [Elasticsearch low level client](https://
-elasticsearch-py.readthedocs.io) to connect to Elasticsearch. This client
-supports a range of [connection options and authentication options](https://
-elasticsearch-py.readthedocs.io/en/stable/api.html#elasticsearch). You can pass
-either an instance of `elasticsearch.Elasticsearch` to Eland APIs or a string
-containing the host to connect to: ```python import eland as ed # Connecting to
-an Elasticsearch instance running on 'localhost:9200' df = ed.DataFrame
-("localhost:9200", es_index_pattern="flights") # Connecting to an Elastic Cloud
-instance from elasticsearch import Elasticsearch es = Elasticsearch
-( cloud_id="cluster-name:...", http_auth=("elastic", "") ) df = ed.DataFrame
-(es, es_index_pattern="flights") ``` ## DataFrames in Eland `eland.DataFrame`
-wraps an Elasticsearch index in a Pandas-like API and defers all processing and
-filtering of data to Elasticsearch instead of your local machine. This means
-you can process large amounts of data within Elasticsearch from a Jupyter
-Notebook without overloading your machine. â¤ [Eland DataFrame API
-documentation](https://eland.readthedocs.io/en/latest/reference/dataframe.html)
-â¤ [Advanced examples in a Jupyter Notebook](https://eland.readthedocs.io/en/
-latest/examples/demo_notebook.html) ```python >>> import eland as ed >>> #
-Connect to 'flights' index via localhost Elasticsearch node >>> df =
-ed.DataFrame('localhost:9200', 'flights') # eland.DataFrame instance has the
-same API as pandas.DataFrame # except all data is in Elasticsearch. See .info()
-memory usage. >>> df.head() AvgTicketPrice Cancelled ... dayOfWeek timestamp 0
-841.265642 False ... 0 2018-01-01 00:00:00 1 882.982662 False ... 0 2018-01-01
-18:27:00 2 190.636904 False ... 0 2018-01-01 17:11:14 3 181.694216 True ... 0
-2018-01-01 10:33:28 4 730.041778 False ... 0 2018-01-01 05:13:00 [5 rows x 27
-columns] >>> df.info()
+Compatibility - Supports Python 3.8, 3.9, 3.10 and Pandas 1.5 - Supports
+Elasticsearch clusters that are 7.11+, recommended 8.3 or later for all
+features to work. If you are using the NLP with PyTorch feature make sure your
+Eland minor version matches the minor version of your Elasticsearch cluster.
+For all other features it is sufficient for the major versions to match. - You
+need to use PyTorch `1.13.1` or earlier to import an NLP model. Run `pip
+install torch==1.13.1` to install the aproppriate version of PyTorch. ###
+Prerequisites Users installing Eland on Debian-based distributions may need to
+install prerequisite packages for the transitive dependencies of Eland: ```bash
+$ sudo apt-get install -y \ build-essential pkg-config cmake \ python3-dev
+libzip-dev libjpeg-dev ``` Note that other distributions such as CentOS,
+RedHat, Arch, etc. may require using a different package manager and specifying
+different package names. ### Docker Users wishing to use Eland without
+installing it, in order to just run the available scripts, can build the Docker
+container: ```bash $ docker build -t elastic/eland . ``` The container can now
+be used interactively: ```bash $ docker run -it --rm --network host elastic/
+eland ``` Running installed scripts is also possible without an interactive
+shell, e.g.: ```bash $ docker run -it --rm --network host \ elastic/eland \
+eland_import_hub_model \ --url http://host.docker.internal:9200/ \ --hub-model-
+id elastic/distilbert-base-cased-finetuned-conll03-english \ --task-type ner
+``` ### Connecting to Elasticsearch Eland uses the [Elasticsearch low level
+client](https://elasticsearch-py.readthedocs.io) to connect to Elasticsearch.
+This client supports a range of [connection options and authentication options]
+(https://elasticsearch-py.readthedocs.io/en/stable/api.html#elasticsearch). You
+can pass either an instance of `elasticsearch.Elasticsearch` to Eland APIs or a
+string containing the host to connect to: ```python import eland as ed #
+Connecting to an Elasticsearch instance running on 'localhost:9200' df =
+ed.DataFrame("localhost:9200", es_index_pattern="flights") # Connecting to an
+Elastic Cloud instance from elasticsearch import Elasticsearch es =
+Elasticsearch( cloud_id="cluster-name:...", http_auth=("elastic", "") ) df =
+ed.DataFrame(es, es_index_pattern="flights") ``` ## DataFrames in Eland
+`eland.DataFrame` wraps an Elasticsearch index in a Pandas-like API and defers
+all processing and filtering of data to Elasticsearch instead of your local
+machine. This means you can process large amounts of data within Elasticsearch
+from a Jupyter Notebook without overloading your machine. â¤ [Eland DataFrame
+API documentation](https://eland.readthedocs.io/en/latest/reference/
+dataframe.html) â¤ [Advanced examples in a Jupyter Notebook](https://
+eland.readthedocs.io/en/latest/examples/demo_notebook.html) ```python >>>
+import eland as ed >>> # Connect to 'flights' index via localhost Elasticsearch
+node >>> df = ed.DataFrame('localhost:9200', 'flights') # eland.DataFrame
+instance has the same API as pandas.DataFrame # except all data is in
+Elasticsearch. See .info() memory usage. >>> df.head() AvgTicketPrice Cancelled
+... dayOfWeek timestamp 0 841.265642 False ... 0 2018-01-01 00:00:00 1
+882.982662 False ... 0 2018-01-01 18:27:00 2 190.636904 False ... 0 2018-01-01
+17:11:14 3 181.694216 True ... 0 2018-01-01 10:33:28 4 730.041778 False ... 0
+2018-01-01 05:13:00 [5 rows x 27 columns] >>> df.info()
 eland.dataframe.DataFrame'> Index: 13059 entries, 0 to 13058 Data columns
 (total 27 columns): # Column Non-Null Count Dtype --- ------ -------------- ---
 -- 0 AvgTicketPrice 13059 non-null float64 1 Cancelled 13059 non-null bool 2
 Carrier 13059 non-null object ... 24 OriginWeather 13059 non-null object 25
 dayOfWeek 13059 non-null int64 26 timestamp 13059 non-null datetime64[ns]
 dtypes: bool(2), datetime64[ns](1), float64(5), int64(2), object(17) memory
 usage: 80.0 bytes Elasticsearch storage usage: 5.043 MB # Filtering of rows
@@ -93,26 +93,36 @@
 Elasticsearch with the training data >>> es_model.predict(training_data[0]) [0
 1 1 0 1 0 0 0 1 0] ``` ### NLP with PyTorch For NLP tasks, Eland allows
 importing PyTorch trained BERT models into Elasticsearch. Models can be either
 plain PyTorch models, or supported [transformers](https://huggingface.co/
 transformers) models from the [Hugging Face model hub](https://huggingface.co/
 models). ```bash $ eland_import_hub_model \ --url http://localhost:9200/ \ --
 hub-model-id elastic/distilbert-base-cased-finetuned-conll03-english \ --task-
-type ner \ --start ``` ```python >>> import elasticsearch >>> from pathlib
-import Path >>> from eland.ml.pytorch import PyTorchModel >>> from
-eland.ml.pytorch.transformers import TransformerModel # Load a Hugging Face
-transformers model directly from the model hub >>> tm = TransformerModel
-("elastic/distilbert-base-cased-finetuned-conll03-english", "ner") Downloading:
+type ner \ --start ``` The example above will automatically start a model
+deployment. This is a good shortcut for initial experimentation, but for
+anything that needs good throughput you should omit the `--start` argument from
+the Eland command line and instead start the model using the ML UI in Kibana.
+The `--start` argument will deploy the model with one allocation and one thread
+per allocation, which will not offer good performance. When starting the model
+deployment using the ML UI in Kibana or the Elasticsearch [API](https://
+www.elastic.co/guide/en/elasticsearch/reference/current/start-trained-model-
+deployment.html) you will be able to set the threading options to make the best
+use of your hardware. ```python >>> import elasticsearch >>> from pathlib
+import Path >>> from eland.common import es_version >>> from eland.ml.pytorch
+import PyTorchModel >>> from eland.ml.pytorch.transformers import
+TransformerModel >>> es = elasticsearch.Elasticsearch("http://elastic:
+mlqa_admin@localhost:9200") >>> es_cluster_version = es_version(es) # Load a
+Hugging Face transformers model directly from the model hub >>> tm =
+TransformerModel(model_id="elastic/distilbert-base-cased-finetuned-conll03-
+english", task_type="ner", es_version=es_cluster_version) Downloading:
 100%|ââââââââââ| 257/257 [00:00<00:00, 108kB/s]
 Downloading: 100%|ââââââââââ| 954/954 [00:00<00:00, 372kB/
 s] Downloading: 100%|ââââââââââ| 208k/208k [00:00<00:00,
 668kB/s] Downloading: 100%|ââââââââââ| 112/112 [00:00<00:
 00, 43.9kB/s] Downloading: 100%|ââââââââââ| 249M/249M [00:
 23<00:00, 11.2MB/s] # Export the model in a TorchScrpt representation which
 Elasticsearch uses >>> tmp_path = "models" >>> Path(tmp_path).mkdir
 (parents=True, exist_ok=True) >>> model_path, config, vocab_path = tm.save
-(tmp_path) # Import model into Elasticsearch >>> es =
-elasticsearch.Elasticsearch("http://elastic:mlqa_admin@localhost:9200",
-timeout=300) # 5 minute timeout >>> ptm = PyTorchModel(es,
+(tmp_path) # Import model into Elasticsearch >>> ptm = PyTorchModel(es,
 tm.elasticsearch_model_id()) >>> ptm.import_model(model_path=model_path,
 config_path=None, vocab_path=vocab_path, config=config)
 100%|ââââââââââ| 63/63 [00:12<00:00, 5.02it/s] ```
```

### Comparing `eland-8.7.0/bin/eland_import_hub_model` & `eland-8.9.0/eland/cli/eland_import_hub_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 #  Licensed to Elasticsearch B.V. under one or more contributor
 #  license agreements. See the NOTICE file distributed with
 #  this work for additional information regarding copyright
 #  ownership. Elasticsearch B.V. licenses this file to you under
 #  the Apache License, Version 2.0 (the "License"); you may
 #  not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
@@ -30,18 +28,22 @@
 import sys
 import tempfile
 import textwrap
 
 from elastic_transport.client_utils import DEFAULT
 from elasticsearch import AuthenticationException, Elasticsearch
 
+from eland.common import parse_es_version
+
 MODEL_HUB_URL = "https://huggingface.co"
 
 
 def get_arg_parser():
+    from eland.ml.pytorch.transformers import SUPPORTED_TASK_TYPES
+
     parser = argparse.ArgumentParser()
     location_args = parser.add_mutually_exclusive_group(required=True)
     location_args.add_argument(
         "--url",
         default=os.environ.get("ES_URL"),
         help="An Elasticsearch connection URL, e.g. http://localhost:9200",
     )
@@ -50,49 +52,51 @@
         default=os.environ.get("CLOUD_ID"),
         help="Cloud ID as found in the 'Manage Deployment' page of an Elastic Cloud deployment",
     )
     parser.add_argument(
         "--hub-model-id",
         required=True,
         help="The model ID in the Hugging Face model hub, "
-             "e.g. dbmdz/bert-large-cased-finetuned-conll03-english",
+        "e.g. dbmdz/bert-large-cased-finetuned-conll03-english",
     )
     parser.add_argument(
         "--es-model-id",
         required=False,
         default=None,
         help="The model ID to use in Elasticsearch, "
-             "e.g. bert-large-cased-finetuned-conll03-english."
-             "When left unspecified, this will be auto-created from the `hub-id`",
+        "e.g. bert-large-cased-finetuned-conll03-english."
+        "When left unspecified, this will be auto-created from the `hub-id`",
     )
     parser.add_argument(
-        "-u", "--es-username",
+        "-u",
+        "--es-username",
         required=False,
         default=os.environ.get("ES_USERNAME"),
-        help="Username for Elasticsearch"
+        help="Username for Elasticsearch",
     )
     parser.add_argument(
-        "-p", "--es-password",
+        "-p",
+        "--es-password",
         required=False,
         default=os.environ.get("ES_PASSWORD"),
-        help="Password for the Elasticsearch user specified with -u/--username"
+        help="Password for the Elasticsearch user specified with -u/--username",
     )
     parser.add_argument(
         "--es-api-key",
         required=False,
         default=os.environ.get("ES_API_KEY"),
-        help="API key for Elasticsearch"
+        help="API key for Elasticsearch",
     )
     parser.add_argument(
         "--task-type",
         required=False,
         choices=SUPPORTED_TASK_TYPES,
         help="The task type for the model usage. Will attempt to auto-detect task type for the model if not provided. "
-             "Default: auto",
-        default="auto"
+        "Default: auto",
+        default="auto",
     )
     parser.add_argument(
         "--quantize",
         action="store_true",
         default=False,
         help="Quantize the model before uploading. Default: False",
     )
@@ -102,133 +106,185 @@
         default=False,
         help="Start the model deployment after uploading. Default: False",
     )
     parser.add_argument(
         "--clear-previous",
         action="store_true",
         default=False,
-        help="Should the model previously stored with `es-model-id` be deleted"
+        help="Should the model previously stored with `es-model-id` be deleted",
     )
     parser.add_argument(
         "--insecure",
         action="store_false",
         default=True,
-        help="Do not verify SSL certificates"
+        help="Do not verify SSL certificates",
     )
     parser.add_argument(
-        "--ca-certs",
-        required=False,
-        default=DEFAULT,
-        help="Path to CA bundle"
+        "--ca-certs", required=False, default=DEFAULT, help="Path to CA bundle"
     )
 
     return parser
 
 
-def get_es_client(cli_args):
+def get_es_client(cli_args, logger):
     try:
         es_args = {
-            'request_timeout': 300,
-            'verify_certs': cli_args.insecure,
-            'ca_certs': cli_args.ca_certs
+            "request_timeout": 300,
+            "verify_certs": cli_args.insecure,
+            "ca_certs": cli_args.ca_certs,
         }
 
         # Deployment location
         if cli_args.url:
-            es_args['hosts'] = cli_args.url
+            es_args["hosts"] = cli_args.url
 
         if cli_args.cloud_id:
-            es_args['cloud_id'] = cli_args.cloud_id
+            es_args["cloud_id"] = cli_args.cloud_id
 
         # Authentication
         if cli_args.es_api_key:
-            es_args['api_key'] = cli_args.es_api_key
+            es_args["api_key"] = cli_args.es_api_key
         elif cli_args.es_username:
             if not cli_args.es_password:
-                logging.error(f"Password for user {cli_args.es_username} was not specified.")
+                logging.error(
+                    f"Password for user {cli_args.es_username} was not specified."
+                )
                 exit(1)
 
-            es_args['basic_auth'] = (cli_args.es_username, cli_args.es_password)
+            es_args["basic_auth"] = (cli_args.es_username, cli_args.es_password)
 
         es_client = Elasticsearch(**es_args)
-        es_info = es_client.info()
-        logger.info(f"Connected to cluster named '{es_info['cluster_name']}' (version: {es_info['version']['number']})")
-
         return es_client
     except AuthenticationException as e:
         logger.error(e)
         exit(1)
 
 
-if __name__ == "__main__":
+def check_cluster_version(es_client, logger):
+    es_info = es_client.info()
+    logger.info(
+        f"Connected to cluster named '{es_info['cluster_name']}' (version: {es_info['version']['number']})"
+    )
+
+    sem_ver = parse_es_version(es_info["version"]["number"])
+    major_version = sem_ver[0]
+    minor_version = sem_ver[1]
+
+    # NLP models added in 8
+    if major_version < 8:
+        logger.error(
+            f"Elasticsearch version {major_version} does not support NLP models. Please upgrade Elasticsearch to the latest version"
+        )
+        exit(1)
+
+    # PyTorch was upgraded to version 1.13.1 in 8.7.
+    # and is incompatible with earlier versions
+    if major_version == 8 and minor_version < 7:
+        import torch
+
+        logger.error(
+            f"Eland uses PyTorch version {torch.__version__} which is incompatible with Elasticsearch versions prior to 8.7. Please upgrade Elasticsearch to at least version 8.7"
+        )
+        exit(1)
+
+    return sem_ver
+
+
+def main():
     # Configure logging
-    logging.basicConfig(format='%(asctime)s %(levelname)s : %(message)s')
+    logging.basicConfig(format="%(asctime)s %(levelname)s : %(message)s")
     logger = logging.getLogger(__name__)
     logger.setLevel(logging.INFO)
 
     try:
         from eland.ml.pytorch import PyTorchModel
         from eland.ml.pytorch.transformers import (
             SUPPORTED_TASK_TYPES,
             TaskTypeError,
             TransformerModel,
         )
     except ModuleNotFoundError as e:
-        logger.error(textwrap.dedent(f"""\
+        logger.error(
+            textwrap.dedent(
+                f"""\
             \033[31mFailed to run because module '{e.name}' is not available.\033[0m
-            
+
             This script requires PyTorch extras to run. You can install these by running:
-            
+
                 \033[1m{sys.executable} -m pip install 'eland[pytorch]'
-            \033[0m"""))
+            \033[0m"""
+            )
+        )
         exit(1)
+    assert SUPPORTED_TASK_TYPES
 
     # Parse arguments
     args = get_arg_parser().parse_args()
 
     # Connect to ES
     logger.info("Establishing connection to Elasticsearch")
-    es = get_es_client(args)
+    es = get_es_client(args, logger)
+    cluster_version = check_cluster_version(es, logger)
 
     # Trace and save model, then upload it from temp file
     with tempfile.TemporaryDirectory() as tmp_dir:
-        logger.info(f"Loading HuggingFace transformer tokenizer and model '{args.hub_model_id}'")
+        logger.info(
+            f"Loading HuggingFace transformer tokenizer and model '{args.hub_model_id}'"
+        )
 
         try:
-            tm = TransformerModel(args.hub_model_id, args.task_type, args.quantize)
+            tm = TransformerModel(
+                model_id=args.hub_model_id,
+                task_type=args.task_type,
+                es_version=cluster_version,
+                quantize=args.quantize,
+            )
             model_path, config, vocab_path = tm.save(tmp_dir)
         except TaskTypeError as err:
-            logger.error(f"Failed to get model for task type, please provide valid task type via '--task-type' parameter. Caused by {err}")
+            logger.error(
+                f"Failed to get model for task type, please provide valid task type via '--task-type' parameter. Caused by {err}"
+            )
             exit(1)
 
-        ptm = PyTorchModel(es, args.es_model_id if args.es_model_id else tm.elasticsearch_model_id())
-        model_exists = es.options(ignore_status=404).ml.get_trained_models(model_id=ptm.model_id).meta.status == 200
+        ptm = PyTorchModel(
+            es, args.es_model_id if args.es_model_id else tm.elasticsearch_model_id()
+        )
+        model_exists = (
+            es.options(ignore_status=404)
+            .ml.get_trained_models(model_id=ptm.model_id)
+            .meta.status
+            == 200
+        )
 
         if model_exists:
             if args.clear_previous:
                 logger.info(f"Stopping deployment for model with id '{ptm.model_id}'")
                 ptm.stop()
 
                 logger.info(f"Deleting model with id '{ptm.model_id}'")
                 ptm.delete()
             else:
                 logger.error(f"Trained model with id '{ptm.model_id}' already exists")
-                logger.info("Run the script with the '--clear-previous' flag if you want to overwrite the existing model.")
+                logger.info(
+                    "Run the script with the '--clear-previous' flag if you want to overwrite the existing model."
+                )
                 exit(1)
 
         logger.info(f"Creating model with id '{ptm.model_id}'")
         ptm.put_config(config=config)
 
-        logger.info(f"Uploading model definition")
+        logger.info("Uploading model definition")
         ptm.put_model(model_path)
 
-        logger.info(f"Uploading model vocabulary")
+        logger.info("Uploading model vocabulary")
         ptm.put_vocab(vocab_path)
 
     # Start the deployed model
     if args.start:
-        logger.info(f"Starting model deployment")
+        logger.info("Starting model deployment")
         ptm.start()
 
     logger.info(f"Model successfully imported with id '{ptm.model_id}'")
 
 
+if __name__ == "__main__":
+    main()
```

### Comparing `eland-8.7.0/eland/__init__.py` & `eland-8.9.0/eland/__init__.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/_version.py` & `eland-8.9.0/eland/_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
 __title__ = "eland"
 __description__ = "Python Client and Toolkit for DataFrames, Big Data, Machine Learning and ETL in Elasticsearch"
 __url__ = "https://github.com/elastic/eland"
-__version__ = "8.7.0"
+__version__ = "8.9.0"
 __author__ = "Steve Dodson"
 __author_email__ = "steve.dodson@elastic.co"
-__maintainer__ = "Seth Michael Larson"
-__maintainer_email__ = "seth.larson@elastic.co"
+__maintainer__ = "Elastic Client Library Maintainers"
+__maintainer_email__ = "client-libs@elastic.co"
```

### Comparing `eland-8.7.0/eland/actions.py` & `eland-8.9.0/eland/actions.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/arithmetics.py` & `eland-8.9.0/eland/arithmetics.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/common.py` & `eland-8.9.0/eland/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,23 +318,15 @@
 def es_version(es_client: Elasticsearch) -> Tuple[int, int, int]:
     """Tags the current ES client with a cached '_eland_es_version'
     property if one doesn't exist yet for the current Elasticsearch version.
     """
     eland_es_version: Tuple[int, int, int]
     if not hasattr(es_client, "_eland_es_version"):
         version_info = es_client.info()["version"]["number"]
-        match = re.match(r"^(\d+)\.(\d+)\.(\d+)", version_info)
-        if match is None:
-            raise ValueError(
-                f"Unable to determine Elasticsearch version. "
-                f"Received: {version_info}"
-            )
-        eland_es_version = cast(
-            Tuple[int, int, int], tuple(int(x) for x in match.groups())
-        )
+        eland_es_version = parse_es_version(version_info)
         es_client._eland_es_version = eland_es_version  # type: ignore
 
         # Raise a warning if the major version of the library doesn't match the
         # the Elasticsearch server major version.
         if eland_es_version[0] != _ELAND_MAJOR_VERSION:
             warnings.warn(
                 f"Eland major version ({_eland_version}) doesn't match the major "
@@ -343,7 +335,20 @@
                 "as your cluster major version.",
                 stacklevel=2,
             )
 
     else:
         eland_es_version = es_client._eland_es_version
     return eland_es_version
+
+
+def parse_es_version(version: str) -> Tuple[int, int, int]:
+    """
+    Parse the semantic version from a string e.g. '8.8.0'
+    Extensions such as '-SNAPSHOT' are ignored
+    """
+    match = re.match(r"^(\d+)\.(\d+)\.(\d+)", version)
+    if match is None:
+        raise ValueError(
+            f"Unable to determine Elasticsearch version. " f"Received: {version}"
+        )
+    return cast(Tuple[int, int, int], tuple(int(x) for x in match.groups()))
```

### Comparing `eland-8.7.0/eland/conftest.py` & `eland-8.9.0/eland/conftest.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/dataframe.py` & `eland-8.9.0/eland/dataframe.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/etl.py` & `eland-8.9.0/eland/etl.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/field_mappings.py` & `eland-8.9.0/eland/field_mappings.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     is_datetime_or_timedelta_dtype,
     is_float_dtype,
     is_integer_dtype,
     is_string_dtype,
 )
 from pandas.core.dtypes.inference import is_list_like
 
+from .common import es_version
+
 if TYPE_CHECKING:
     from elasticsearch import Elasticsearch
     from numpy.typing import DTypeLike
 
 
 ES_FLOAT_TYPES: Set[str] = {"double", "float", "half_float", "scaled_float"}
 ES_INTEGER_TYPES: Set[str] = {"long", "integer", "short", "byte"}
@@ -209,15 +211,15 @@
             raise ValueError(
                 f"Can not get mapping for {index_pattern} "
                 f"check indexes exist and client has permission to get mapping."
             )
 
         # Get all fields (including all nested) and then all field_caps
         all_fields = FieldMappings._extract_fields_from_mapping(get_mapping)
-        all_fields_caps = client.field_caps(index=index_pattern, fields="*")
+        all_fields_caps = _compat_field_caps(client, index=index_pattern, fields="*")
 
         # Get top level (not sub-field multifield) mappings
         source_fields = FieldMappings._extract_fields_from_mapping(
             get_mapping, source_only=True
         )
 
         # Populate capability matrix of fields
@@ -921,7 +923,38 @@
 
     if problems:
         problems_message = "\n".join(problems)
         raise ValueError(
             f"DataFrame dtypes and Elasticsearch index mapping "
             f"aren't compatible:\n{problems_message}"
         )
+
+
+def _compat_field_caps(client, fields, index=None):
+    """The field_caps API moved it's 'fields' parameter to the HTTP request body
+    in Elasticsearch 8.5.0 (previously was only accepted in the query string).
+    This can cause some unfortunate errors for users of Eland against old server
+    versions because at that point the version of the Elasticsearch client actually
+    matters for compatibility, which can be unexpected by consumers of *only* Eland.
+
+    Our work-around below is to force the parameter in the query string on older server versions.
+    """
+
+    # If the server version is 8.5.0 or later we don't need
+    # the query string work-around. Sending via any client
+    # version should be just fine.
+    if es_version(client) >= (8, 5, 0):
+        return client.field_caps(index=index, fields=fields)
+
+    # Otherwise we need to force sending via the query string.
+    from elasticsearch._sync.client import SKIP_IN_PATH, _quote
+
+    if index not in SKIP_IN_PATH:
+        __path = f"/{_quote(index)}/_field_caps"
+    else:
+        __path = "/_field_caps"
+    __query: Dict[str, Any] = {}
+    if fields is not None:
+        __query["fields"] = fields
+    return client.perform_request(
+        "POST", __path, params=__query, headers={"accept": "application/json"}
+    )
```

### Comparing `eland-8.7.0/eland/filter.py` & `eland-8.9.0/eland/filter.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/groupby.py` & `eland-8.9.0/eland/groupby.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/index.py` & `eland-8.9.0/eland/index.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/ml/__init__.py` & `eland-8.9.0/eland/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/ml/_model_serializer.py` & `eland-8.9.0/eland/ml/_model_serializer.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/ml/_optional.py` & `eland-8.9.0/eland/ml/_optional.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/ml/common.py` & `eland-8.9.0/eland/ml/common.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/ml/exporters/__init__.py` & `eland-8.9.0/eland/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/ml/exporters/_sklearn_deserializers.py` & `eland-8.9.0/eland/ml/exporters/_sklearn_deserializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,26 +93,31 @@
                     children_left[i],
                     children_right[i],
                     feature[i],
                     threshold[i],
                     impurity[i],
                     n_node_samples[i],
                     weighted_n_node_samples[i],
+                    True,
                 )
                 for i in range(node_count)
             ],
-            dtype=[
-                ("left_child", "<i8"),
-                ("right_child", "<i8"),
-                ("feature", "<i8"),
-                ("threshold", "<f8"),
-                ("impurity", "<f8"),
-                ("n_node_samples", "<i8"),
-                ("weighted_n_node_samples", "<f8"),
-            ],
+            dtype={
+                "names": [
+                    "left_child",
+                    "right_child",
+                    "feature",
+                    "threshold",
+                    "impurity",
+                    "n_node_samples",
+                    "weighted_n_node_samples",
+                    "missing_go_to_left",
+                ],
+                "formats": ["<i8", "<i8", "<i8", "<f8", "<f8", "<i8", "<f8", "u1"],
+            },
         )
         state = {
             "max_depth": self.max_depth,
             "node_count": node_count,
             "nodes": node_state,
             "values": value,
         }
```

### Comparing `eland-8.7.0/eland/ml/exporters/common.py` & `eland-8.9.0/eland/ml/exporters/common.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/ml/exporters/es_gb_models.py` & `eland-8.9.0/eland/ml/exporters/es_gb_models.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/ml/ml_model.py` & `eland-8.9.0/eland/ml/ml_model.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/ml/pytorch/__init__.py` & `eland-8.9.0/eland/ml/pytorch/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,10 +27,11 @@
 
 __all__ = [
     "PyTorchModel",
     "TraceableModel",
     "NlpTrainedModelConfig",
     "NlpBertTokenizationConfig",
     "NlpRobertaTokenizationConfig",
+    "NlpXLMRobertaTokenizationConfig",
     "NlpMPNetTokenizationConfig",
     "task_type_from_model_config",
 ]
```

### Comparing `eland-8.7.0/eland/ml/pytorch/_pytorch_model.py` & `eland-8.9.0/eland/ml/pytorch/_pytorch_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     ) -> Any:
         if docs is None:
             raise ValueError("Empty value passed for parameter 'docs'")
 
         __body: Dict[str, Any] = {}
         __body["docs"] = docs
 
-        __path = f"/_ml/trained_models/{_quote(self.model_id)}/deployment/_infer"
+        __path = f"/_ml/trained_models/{_quote(self.model_id)}/_infer"
         __query: Dict[str, Any] = {}
         __query["timeout"] = timeout
         __headers = {"accept": "application/json", "content-type": "application/json"}
 
         return self._client.options(request_timeout=60).perform_request(
             "POST", __path, params=__query, headers=__headers, body=__body
         )
```

### Comparing `eland-8.7.0/eland/ml/pytorch/nlp_ml_model.py` & `eland-8.9.0/eland/ml/pytorch/nlp_ml_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -62,14 +62,34 @@
             max_sequence_length=max_sequence_length,
             truncate=truncate,
             span=span,
         )
         self.add_prefix_space = add_prefix_space
 
 
+class NlpXLMRobertaTokenizationConfig(NlpTokenizationConfig):
+    def __init__(
+        self,
+        *,
+        with_special_tokens: t.Optional[bool] = None,
+        max_sequence_length: t.Optional[int] = None,
+        truncate: t.Optional[
+            t.Union["t.Literal['first', 'none', 'second']", str]
+        ] = None,
+        span: t.Optional[int] = None,
+    ):
+        super().__init__(
+            configuration_type="xlm_roberta",
+            with_special_tokens=with_special_tokens,
+            max_sequence_length=max_sequence_length,
+            truncate=truncate,
+            span=span,
+        )
+
+
 class NlpBertTokenizationConfig(NlpTokenizationConfig):
     def __init__(
         self,
         *,
         do_lower_case: t.Optional[bool] = None,
         with_special_tokens: t.Optional[bool] = None,
         max_sequence_length: t.Optional[int] = None,
@@ -84,14 +104,36 @@
             max_sequence_length=max_sequence_length,
             truncate=truncate,
             span=span,
         )
         self.do_lower_case = do_lower_case
 
 
+class NlpBertJapaneseTokenizationConfig(NlpTokenizationConfig):
+    def __init__(
+        self,
+        *,
+        do_lower_case: t.Optional[bool] = None,
+        with_special_tokens: t.Optional[bool] = None,
+        max_sequence_length: t.Optional[int] = None,
+        truncate: t.Optional[
+            t.Union["t.Literal['first', 'none', 'second']", str]
+        ] = None,
+        span: t.Optional[int] = None,
+    ):
+        super().__init__(
+            configuration_type="bert_ja",
+            with_special_tokens=with_special_tokens,
+            max_sequence_length=max_sequence_length,
+            truncate=truncate,
+            span=span,
+        )
+        self.do_lower_case = do_lower_case
+
+
 class NlpMPNetTokenizationConfig(NlpTokenizationConfig):
     def __init__(
         self,
         *,
         do_lower_case: t.Optional[bool] = None,
         with_special_tokens: t.Optional[bool] = None,
         max_sequence_length: t.Optional[int] = None,
@@ -234,18 +276,20 @@
 
 class TextEmbeddingInferenceOptions(InferenceConfig):
     def __init__(
         self,
         *,
         tokenization: NlpTokenizationConfig,
         results_field: t.Optional[str] = None,
+        embedding_size: t.Optional[int] = None,
     ):
         super().__init__(configuration_type="text_embedding")
         self.tokenization = tokenization
         self.results_field = results_field
+        self.embedding_size = embedding_size
 
 
 class TextExpansionInferenceOptions(InferenceConfig):
     def __init__(
         self,
         *,
         tokenization: NlpTokenizationConfig,
```

### Comparing `eland-8.7.0/eland/ml/pytorch/traceable_model.py` & `eland-8.9.0/eland/ml/pytorch/traceable_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,18 @@
 
     def trace(self) -> TracedModelTypes:
         # model needs to be in evaluate mode
         self._model.eval()
         return self._trace()
 
     @abstractmethod
+    def sample_output(self) -> torch.Tensor:
+        ...
+
+    @abstractmethod
     def _trace(self) -> TracedModelTypes:
         ...
 
     def classification_labels(self) -> Optional[List[str]]:
         return None
 
     def save(self, path: str) -> str:
```

### Comparing `eland-8.7.0/eland/ml/pytorch/transformers.py` & `eland-8.9.0/eland/ml/pytorch/transformers.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 """
 Support for and interoperability with HuggingFace transformers and related
 libraries such as sentence-transformers.
 """
 
 import json
 import os.path
+import re
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
 import torch  # type: ignore
 import transformers  # type: ignore
 from sentence_transformers import SentenceTransformer  # type: ignore
 from torch import Tensor, nn
@@ -38,19 +39,21 @@
     PreTrainedTokenizer,
     PreTrainedTokenizerFast,
 )
 
 from eland.ml.pytorch.nlp_ml_model import (
     FillMaskInferenceOptions,
     NerInferenceOptions,
+    NlpBertJapaneseTokenizationConfig,
     NlpBertTokenizationConfig,
     NlpMPNetTokenizationConfig,
     NlpRobertaTokenizationConfig,
     NlpTokenizationConfig,
     NlpTrainedModelConfig,
+    NlpXLMRobertaTokenizationConfig,
     PassThroughInferenceOptions,
     QuestionAnsweringInferenceOptions,
     TextClassificationInferenceOptions,
     TextEmbeddingInferenceOptions,
     TextExpansionInferenceOptions,
     TextSimilarityInferenceOptions,
     TrainedModelInput,
@@ -58,14 +61,15 @@
 )
 from eland.ml.pytorch.traceable_model import TraceableModel
 
 DEFAULT_OUTPUT_KEY = "sentence_embedding"
 SUPPORTED_TASK_TYPES = {
     "fill_mask",
     "ner",
+    "pass_through",
     "text_classification",
     "text_embedding",
     "text_expansion",
     "zero_shot_classification",
     "question_answering",
     "text_similarity",
 }
@@ -92,24 +96,26 @@
     "pass_through": PassThroughInferenceOptions,
     "question_answering": QuestionAnsweringInferenceOptions,
     "text_similarity": TextSimilarityInferenceOptions,
 }
 SUPPORTED_TASK_TYPES_NAMES = ", ".join(sorted(SUPPORTED_TASK_TYPES))
 SUPPORTED_TOKENIZERS = (
     transformers.BertTokenizer,
+    transformers.BertJapaneseTokenizer,
     transformers.MPNetTokenizer,
     transformers.DPRContextEncoderTokenizer,
     transformers.DPRQuestionEncoderTokenizer,
     transformers.DistilBertTokenizer,
     transformers.ElectraTokenizer,
     transformers.MobileBertTokenizer,
     transformers.RetriBertTokenizer,
     transformers.RobertaTokenizer,
     transformers.BartTokenizer,
     transformers.SqueezeBertTokenizer,
+    transformers.XLMRobertaTokenizer,
 )
 SUPPORTED_TOKENIZERS_NAMES = ", ".join(sorted([str(x) for x in SUPPORTED_TOKENIZERS]))
 
 TracedModelTypes = Union[
     torch.nn.Module,
     torch.ScriptModule,
     torch.jit.ScriptModule,
@@ -177,14 +183,15 @@
         model = AutoModelForQuestionAnswering.from_pretrained(
             model_id, torchscript=True
         )
         if isinstance(
             model.config,
             (
                 transformers.MPNetConfig,
+                transformers.XLMRobertaConfig,
                 transformers.RobertaConfig,
                 transformers.BartConfig,
             ),
         ):
             return _TwoParameterQuestionAnsweringWrapper(model)
         else:
             return _QuestionAnsweringWrapper(model)
@@ -283,29 +290,27 @@
         self._remove_pooling_layer()
         self._replace_transformer_layer()
 
     @staticmethod
     def from_pretrained(
         model_id: str, output_key: str = DEFAULT_OUTPUT_KEY
     ) -> Optional[Any]:
-        if model_id.startswith("sentence-transformers/"):
-            model = AutoModel.from_pretrained(model_id, torchscript=True)
-            if isinstance(
-                model.config,
-                (
-                    transformers.MPNetConfig,
-                    transformers.RobertaConfig,
-                    transformers.BartConfig,
-                ),
-            ):
-                return _TwoParameterSentenceTransformerWrapper(model, output_key)
-            else:
-                return _SentenceTransformerWrapper(model, output_key)
+        model = AutoModel.from_pretrained(model_id, torchscript=True)
+        if isinstance(
+            model.config,
+            (
+                transformers.MPNetConfig,
+                transformers.XLMRobertaConfig,
+                transformers.RobertaConfig,
+                transformers.BartConfig,
+            ),
+        ):
+            return _TwoParameterSentenceTransformerWrapper(model, output_key)
         else:
-            return None
+            return _SentenceTransformerWrapper(model, output_key)
 
     def _remove_pooling_layer(self) -> None:
         """
         Removes any last pooling layer which is not used to create embeddings.
         Leaving this layer in will cause it to return a NoneType which in turn
         will fail to load in libtorch. Alternatively, we can just use the output
         of the pooling layer as a dummy but this also affects (if only in a
@@ -389,19 +394,21 @@
 
     @staticmethod
     def from_pretrained(model_id: str) -> Optional[Any]:
         config = AutoConfig.from_pretrained(model_id)
 
         def is_compatible() -> bool:
             is_dpr_model = config.model_type == "dpr"
-            has_architectures = len(config.architectures) == 1
-            is_supported_architecture = (
+            has_architectures = (
+                config.architectures is not None and len(config.architectures) == 1
+            )
+            is_supported_architecture = has_architectures and (
                 config.architectures[0] in _DPREncoderWrapper._SUPPORTED_MODELS_NAMES
             )
-            return is_dpr_model and has_architectures and is_supported_architecture
+            return is_dpr_model and is_supported_architecture
 
         if is_compatible():
             model = getattr(transformers, config.architectures[0]).from_pretrained(
                 model_id, torchscript=True
             )
             return _DPREncoderWrapper(model)
         else:
@@ -436,55 +443,59 @@
             _DistilBertWrapper,
         ],
     ):
         super(_TransformerTraceableModel, self).__init__(model=model)
         self._tokenizer = tokenizer
 
     def _trace(self) -> TracedModelTypes:
+        inputs = self._compatible_inputs()
+        return torch.jit.trace(self._model, inputs)
+
+    def sample_output(self) -> Tensor:
+        inputs = self._compatible_inputs()
+        return self._model(*inputs)
+
+    def _compatible_inputs(self) -> Tuple[Tensor, ...]:
         inputs = self._prepare_inputs()
 
         # Add params when not provided by the tokenizer (e.g. DistilBERT), to conform to BERT interface
         if "token_type_ids" not in inputs:
             inputs["token_type_ids"] = torch.zeros(
                 inputs["input_ids"].size(1), dtype=torch.long
             )
         if isinstance(
             self._model.config,
             (
                 transformers.MPNetConfig,
+                transformers.XLMRobertaConfig,
                 transformers.RobertaConfig,
                 transformers.BartConfig,
             ),
         ):
-            return torch.jit.trace(
-                self._model,
-                (inputs["input_ids"], inputs["attention_mask"]),
-            )
+            del inputs["token_type_ids"]
+            return (inputs["input_ids"], inputs["attention_mask"])
 
         position_ids = torch.arange(inputs["input_ids"].size(1), dtype=torch.long)
-
-        return torch.jit.trace(
-            self._model,
-            (
-                inputs["input_ids"],
-                inputs["attention_mask"],
-                inputs["token_type_ids"],
-                position_ids,
-            ),
+        inputs["position_ids"] = position_ids
+        return (
+            inputs["input_ids"],
+            inputs["attention_mask"],
+            inputs["token_type_ids"],
+            inputs["position_ids"],
         )
 
     @abstractmethod
     def _prepare_inputs(self) -> transformers.BatchEncoding:
         ...
 
 
 class _TraceableClassificationModel(_TransformerTraceableModel, ABC):
     def classification_labels(self) -> Optional[List[str]]:
         id_label_items = self._model.config.id2label.items()
-        labels = [v for _, v in sorted(id_label_items, key=lambda kv: kv[0])]  # type: ignore
+        labels = [v for _, v in sorted(id_label_items, key=lambda kv: kv[0])]
 
         # Make classes like I-PER into I_PER which fits Java enumerations
         return [label.replace("-", "_") for label in labels]
 
 
 class _TraceableFillMaskModel(_TransformerTraceableModel):
     def _prepare_inputs(self) -> transformers.BatchEncoding:
@@ -504,14 +515,23 @@
                 "Its headquarters are in DUMBO, therefore very close to the Manhattan Bridge."
             ),
             padding="max_length",
             return_tensors="pt",
         )
 
 
+class _TraceablePassThroughModel(_TransformerTraceableModel):
+    def _prepare_inputs(self) -> transformers.BatchEncoding:
+        return self._tokenizer(
+            "This is an example sentence.",
+            padding="max_length",
+            return_tensors="pt",
+        )
+
+
 class _TraceableTextClassificationModel(_TraceableClassificationModel):
     def _prepare_inputs(self) -> transformers.BatchEncoding:
         return self._tokenizer(
             "This is an example sentence.",
             padding="max_length",
             return_tensors="pt",
         )
@@ -553,15 +573,45 @@
             "The meaning of life, according to the hitchikers guide, is 42.",
             padding="max_length",
             return_tensors="pt",
         )
 
 
 class TransformerModel:
-    def __init__(self, model_id: str, task_type: str, quantize: bool = False):
+    def __init__(
+        self,
+        model_id: str,
+        task_type: str,
+        *,
+        es_version: Optional[Tuple[int, int, int]] = None,
+        quantize: bool = False,
+    ):
+        """
+        Loads a model from the Hugging Face repository or local file and creates
+        the configuration for upload to Elasticsearch.
+
+        Parameters
+        ----------
+        model_id: str
+            A Hugging Face model Id or a file path to the directory containing
+            the model files.
+
+        task_type: str
+            One of the supported task types.
+
+        es_version: Optional[Tuple[int, int, int]]
+            The Elasticsearch cluster version.
+            Certain features are created only if the target cluster is
+            a high enough version to support them. If not set only
+            universally supported features are added.
+
+        quantize: bool, default False
+            Quantize the model.
+        """
+
         self._model_id = model_id
         self._task_type = task_type.replace("-", "_")
 
         # load Hugging Face model and tokenizer
         # use padding in the tokenizer to ensure max length sequences are used for tracing (at call time)
         #  - see: https://huggingface.co/transformers/serialization.html#dummy-inputs-and-standard-lengths
         self._tokenizer = transformers.AutoTokenizer.from_pretrained(
@@ -575,28 +625,42 @@
                 f"Tokenizer type {self._tokenizer} not supported, must be one of: {SUPPORTED_TOKENIZERS_NAMES}"
             )
 
         self._traceable_model = self._create_traceable_model()
         if quantize:
             self._traceable_model.quantize()
         self._vocab = self._load_vocab()
-        self._config = self._create_config()
+        self._config = self._create_config(es_version)
 
     def _load_vocab(self) -> Dict[str, List[str]]:
         vocab_items = self._tokenizer.get_vocab().items()
-        vocabulary = [k for k, _ in sorted(vocab_items, key=lambda kv: kv[1])]  # type: ignore
+        vocabulary = [k for k, _ in sorted(vocab_items, key=lambda kv: kv[1])]
         vocab_obj = {
             "vocabulary": vocabulary,
         }
         ranks = getattr(self._tokenizer, "bpe_ranks", {})
         if len(ranks) > 0:
             merges = [
                 " ".join(m) for m, _ in sorted(ranks.items(), key=lambda kv: kv[1])
             ]
             vocab_obj["merges"] = merges
+        sp_model = getattr(self._tokenizer, "sp_model", None)
+        if sp_model:
+            id_correction = getattr(self._tokenizer, "fairseq_offset", 0)
+            scores = []
+            for _ in range(0, id_correction):
+                scores.append(0.0)
+            for token_id in range(id_correction, len(vocabulary)):
+                try:
+                    scores.append(sp_model.get_score(token_id - id_correction))
+                except IndexError:
+                    scores.append(0.0)
+                    pass
+            if len(scores) > 0:
+                vocab_obj["scores"] = scores
         return vocab_obj
 
     def _create_tokenization_config(self) -> NlpTokenizationConfig:
         if isinstance(self._tokenizer, transformers.MPNetTokenizer):
             return NlpMPNetTokenizationConfig(
                 do_lower_case=getattr(self._tokenizer, "do_lower_case", None),
                 max_sequence_length=getattr(
@@ -608,40 +672,80 @@
         ):
             return NlpRobertaTokenizationConfig(
                 add_prefix_space=getattr(self._tokenizer, "add_prefix_space", None),
                 max_sequence_length=getattr(
                     self._tokenizer, "max_model_input_sizes", dict()
                 ).get(self._model_id),
             )
-        else:
-            return NlpBertTokenizationConfig(
-                do_lower_case=getattr(self._tokenizer, "do_lower_case", None),
+        elif isinstance(self._tokenizer, transformers.XLMRobertaTokenizer):
+            return NlpXLMRobertaTokenizationConfig(
                 max_sequence_length=getattr(
                     self._tokenizer, "max_model_input_sizes", dict()
                 ).get(self._model_id),
             )
+        else:
+            japanese_morphological_tokenizers = ["mecab"]
+            if (
+                hasattr(self._tokenizer, "word_tokenizer_type")
+                and self._tokenizer.word_tokenizer_type
+                in japanese_morphological_tokenizers
+            ):
+                return NlpBertJapaneseTokenizationConfig(
+                    do_lower_case=getattr(self._tokenizer, "do_lower_case", None),
+                    max_sequence_length=getattr(
+                        self._tokenizer, "max_model_input_sizes", dict()
+                    ).get(self._model_id),
+                )
+            else:
+                return NlpBertTokenizationConfig(
+                    do_lower_case=getattr(self._tokenizer, "do_lower_case", None),
+                    max_sequence_length=getattr(
+                        self._tokenizer, "max_model_input_sizes", dict()
+                    ).get(self._model_id),
+                )
 
-    def _create_config(self) -> NlpTrainedModelConfig:
+    def _create_config(
+        self, es_version: Optional[Tuple[int, int, int]]
+    ) -> NlpTrainedModelConfig:
         tokenization_config = self._create_tokenization_config()
 
         # Set squad well known defaults
         if self._task_type == "question_answering":
             tokenization_config.max_sequence_length = 386
             tokenization_config.span = 128
             tokenization_config.truncate = "none"
-        inference_config = (
-            TASK_TYPE_TO_INFERENCE_CONFIG[self._task_type](
+
+        if self._traceable_model.classification_labels():
+            inference_config = TASK_TYPE_TO_INFERENCE_CONFIG[self._task_type](
                 tokenization=tokenization_config,
                 classification_labels=self._traceable_model.classification_labels(),
             )
-            if self._traceable_model.classification_labels()
-            else TASK_TYPE_TO_INFERENCE_CONFIG[self._task_type](
+        elif self._task_type == "text_embedding":
+            # The embedding_size paramater was added in Elasticsearch 8.8
+            # If the version is not known use the basic config
+            if es_version is None or (es_version[0] <= 8 and es_version[1] < 8):
+                inference_config = TASK_TYPE_TO_INFERENCE_CONFIG[self._task_type](
+                    tokenization=tokenization_config
+                )
+            else:
+                sample_embedding = self._traceable_model.sample_output()
+                if type(sample_embedding) is tuple:
+                    text_embedding, _ = sample_embedding
+                else:
+                    text_embedding = sample_embedding
+
+                embedding_size = text_embedding.size(-1)
+                inference_config = TASK_TYPE_TO_INFERENCE_CONFIG[self._task_type](
+                    tokenization=tokenization_config,
+                    embedding_size=embedding_size,
+                )
+        else:
+            inference_config = TASK_TYPE_TO_INFERENCE_CONFIG[self._task_type](
                 tokenization=tokenization_config
             )
-        )
 
         return NlpTrainedModelConfig(
             description=f"Model {self._model_id} for task type '{self._task_type}'",
             model_type="pytorch",
             inference_config=inference_config,
             input=TrainedModelInput(
                 field_names=["text_field"],
@@ -679,50 +783,74 @@
             model = transformers.AutoModelForSequenceClassification.from_pretrained(
                 self._model_id, torchscript=True
             )
             model = _DistilBertWrapper.try_wrapping(model)
             return _TraceableTextClassificationModel(self._tokenizer, model)
 
         elif self._task_type == "text_embedding":
-            model = _SentenceTransformerWrapperModule.from_pretrained(self._model_id)
-            if not model:
-                model = _DPREncoderWrapper.from_pretrained(self._model_id)
+            model = _DPREncoderWrapper.from_pretrained(self._model_id)
             if not model:
-                model = transformers.AutoModel.from_pretrained(
-                    self._model_id, torchscript=True
+                model = _SentenceTransformerWrapperModule.from_pretrained(
+                    self._model_id
                 )
             return _TraceableTextEmbeddingModel(self._tokenizer, model)
 
         elif self._task_type == "zero_shot_classification":
             model = transformers.AutoModelForSequenceClassification.from_pretrained(
                 self._model_id, torchscript=True
             )
             model = _DistilBertWrapper.try_wrapping(model)
             return _TraceableZeroShotClassificationModel(self._tokenizer, model)
+
         elif self._task_type == "question_answering":
             model = _QuestionAnsweringWrapperModule.from_pretrained(self._model_id)
             return _TraceableQuestionAnsweringModel(self._tokenizer, model)
+
         elif self._task_type == "text_similarity":
             model = transformers.AutoModelForSequenceClassification.from_pretrained(
                 self._model_id, torchscript=True
             )
             model = _DistilBertWrapper.try_wrapping(model)
             return _TraceableTextSimilarityModel(self._tokenizer, model)
+
+        elif self._task_type == "pass_through":
+            model = transformers.AutoModel.from_pretrained(
+                self._model_id, torchscript=True
+            )
+            return _TraceablePassThroughModel(self._tokenizer, model)
+
         else:
             raise TypeError(
                 f"Unknown task type {self._task_type}, must be one of: {SUPPORTED_TASK_TYPES_NAMES}"
             )
 
     def elasticsearch_model_id(self) -> str:
-        # Elasticsearch model IDs need to be a specific format: no special chars, all lowercase, max 64 chars
-        return self._model_id.replace("/", "__").lower()[:64]
+        return elasticsearch_model_id(self._model_id)
 
     def save(self, path: str) -> Tuple[str, NlpTrainedModelConfig, str]:
         # save traced model
         model_path = self._traceable_model.save(path)
 
         # save vocabulary
         vocab_path = os.path.join(path, "vocabulary.json")
         with open(vocab_path, "w") as outfile:
             json.dump(self._vocab, outfile)
 
         return model_path, self._config, vocab_path
+
+
+def elasticsearch_model_id(model_id: str) -> str:
+    """
+    Elasticsearch model IDs need to be a specific format:
+    no special chars, all lowercase, max 64 chars. If the
+    Id is longer than 64 charaters take the last 64- in the
+    case where the id is long file path this captures the
+    model name.
+
+    Ids starting with __ are not valid elasticsearch Ids,
+    # this might be the case if model_id is a file path
+    """
+
+    id = re.sub(r"[\s\\/]", "__", model_id).lower()[-64:]
+    if id.startswith("__"):
+        id = id.removeprefix("__")
+    return id
```

### Comparing `eland-8.7.0/eland/ml/transformers/__init__.py` & `eland-8.9.0/eland/ml/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/ml/transformers/base.py` & `eland-8.9.0/eland/ml/transformers/base.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/ml/transformers/lightgbm.py` & `eland-8.9.0/eland/ml/transformers/lightgbm.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/ml/transformers/sklearn.py` & `eland-8.9.0/eland/ml/transformers/sklearn.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/ml/transformers/xgboost.py` & `eland-8.9.0/eland/ml/transformers/xgboost.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/ndframe.py` & `eland-8.9.0/eland/ndframe.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/operations.py` & `eland-8.9.0/eland/operations.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/plotting/__init__.py` & `eland-8.9.0/eland/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/plotting/_core.py` & `eland-8.9.0/eland/plotting/_core.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/plotting/_matplotlib/__init__.py` & `eland-8.9.0/eland/plotting/_matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/plotting/_matplotlib/hist.py` & `eland-8.9.0/eland/plotting/_matplotlib/hist.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/query.py` & `eland-8.9.0/eland/query.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/query_compiler.py` & `eland-8.9.0/eland/query_compiler.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/series.py` & `eland-8.9.0/eland/series.py`

 * *Files 1% similar despite different names*

```diff
@@ -1482,16 +1482,17 @@
         See Also
         --------
         :pandas_api_docs:`pandas.Series.median`
 
         Examples
         --------
         >>> s = ed.DataFrame('http://localhost:9200', 'flights')['AvgTicketPrice']
-        >>> int(s.median())
-        640
+        >>> m = int(s.median())
+        >>> print(m == 639 or m == 640) # required for ES >= 8.9, see https://github.com/elastic/elasticsearch/pull/96904
+        True
         """
         results = super().median(numeric_only=numeric_only)
         return results.squeeze()
 
     def min(self, numeric_only: Optional[bool] = None) -> pd.Series:
         """
         Return the minimum of the Series values
```

### Comparing `eland-8.7.0/eland/tasks.py` & `eland-8.9.0/eland/tasks.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland/utils.py` & `eland-8.9.0/eland/utils.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/eland.egg-info/PKG-INFO` & `eland-8.9.0/eland.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: eland
-Version: 8.7.0
+Version: 8.9.0
 Summary: Python Client and Toolkit for DataFrames, Big Data, Machine Learning and ETL in Elasticsearch
 Home-page: https://github.com/elastic/eland
 Author: Steve Dodson
 Author-email: steve.dodson@elastic.co
-Maintainer: Seth Michael Larson
-Maintainer-email: seth.larson@elastic.co
+Maintainer: Elastic Client Library Maintainers
+Maintainer-email: client-libs@elastic.co
 License: Apache-2.0
 Keywords: elastic eland pandas python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -81,21 +81,22 @@
 
 ```bash
 $ conda install -c conda-forge eland
 ```
 
 ### Compatibility
 
-- Supports Python 3.8+ and Pandas 1.5
+- Supports Python 3.8, 3.9, 3.10 and Pandas 1.5
 - Supports Elasticsearch clusters that are 7.11+, recommended 8.3 or later for all features to work.
   If you are using the NLP with PyTorch feature make sure your Eland minor version matches the minor 
   version of your Elasticsearch cluster. For all other features it is sufficient for the major versions
   to match.
-- You need to use PyTorch `1.11.0` or earlier to import an NLP model. 
-  Run `pip install torch==1.11` to install the aproppriate version of PyTorch.
+- You need to use PyTorch `1.13.1` or earlier to import an NLP model. 
+  Run `pip install torch==1.13.1` to install the aproppriate version of PyTorch.
+  
 
 ### Prerequisites
 
 Users installing Eland on Debian-based distributions may need to install prerequisite packages for the transitive
 dependencies of Eland:
 
 ```bash
@@ -126,16 +127,15 @@
 
 ```bash
 $ docker run -it --rm --network host \
     elastic/eland \
     eland_import_hub_model \
       --url http://host.docker.internal:9200/ \
       --hub-model-id elastic/distilbert-base-cased-finetuned-conll03-english \
-      --task-type ner \
-      --start
+      --task-type ner
 ```
 
 ### Connecting to Elasticsearch 
 
 Eland uses the [Elasticsearch low level client](https://elasticsearch-py.readthedocs.io) to connect to Elasticsearch. 
 This client supports a range of [connection options and authentication options](https://elasticsearch-py.readthedocs.io/en/stable/api.html#elasticsearch). 
 
@@ -269,32 +269,46 @@
 $ eland_import_hub_model \
   --url http://localhost:9200/ \
   --hub-model-id elastic/distilbert-base-cased-finetuned-conll03-english \
   --task-type ner \
   --start
 ```
 
+The example above will automatically start a model deployment. This is a
+good shortcut for initial experimentation, but for anything that needs
+good throughput you should omit the `--start` argument from the Eland
+command line and instead start the model using the ML UI in Kibana.
+The `--start` argument will deploy the model with one allocation and one
+thread per allocation, which will not offer good performance. When starting
+the model deployment using the ML UI in Kibana or the Elasticsearch
+[API](https://www.elastic.co/guide/en/elasticsearch/reference/current/start-trained-model-deployment.html)
+you will be able to set the threading options to make the best use of your
+hardware.
+
 ```python
 >>> import elasticsearch
 >>> from pathlib import Path
+>>> from eland.common import es_version
 >>> from eland.ml.pytorch import PyTorchModel
 >>> from eland.ml.pytorch.transformers import TransformerModel
 
+>>> es = elasticsearch.Elasticsearch("http://elastic:mlqa_admin@localhost:9200")
+>>> es_cluster_version = es_version(es)
+
 # Load a Hugging Face transformers model directly from the model hub
->>> tm = TransformerModel("elastic/distilbert-base-cased-finetuned-conll03-english", "ner")
+>>> tm = TransformerModel(model_id="elastic/distilbert-base-cased-finetuned-conll03-english", task_type="ner", es_version=es_cluster_version)
 Downloading: 100%|██████████| 257/257 [00:00<00:00, 108kB/s]
 Downloading: 100%|██████████| 954/954 [00:00<00:00, 372kB/s]
 Downloading: 100%|██████████| 208k/208k [00:00<00:00, 668kB/s] 
 Downloading: 100%|██████████| 112/112 [00:00<00:00, 43.9kB/s]
 Downloading: 100%|██████████| 249M/249M [00:23<00:00, 11.2MB/s]
 
 # Export the model in a TorchScrpt representation which Elasticsearch uses
 >>> tmp_path = "models"
 >>> Path(tmp_path).mkdir(parents=True, exist_ok=True)
 >>> model_path, config, vocab_path = tm.save(tmp_path)
 
 # Import model into Elasticsearch
->>> es = elasticsearch.Elasticsearch("http://elastic:mlqa_admin@localhost:9200", timeout=300)  # 5 minute timeout
 >>> ptm = PyTorchModel(es, tm.elasticsearch_model_id())
 >>> ptm.import_model(model_path=model_path, config_path=None, vocab_path=vocab_path, config=config)
 100%|██████████| 63/63 [00:12<00:00,  5.02it/s]
 ```
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: eland Version: 8.7.0 Summary: Python Client and
+Metadata-Version: 2.1 Name: eland Version: 8.9.0 Summary: Python Client and
 Toolkit for DataFrames, Big Data, Machine Learning and ETL in Elasticsearch
 Home-page: https://github.com/elastic/eland Author: Steve Dodson Author-email:
-steve.dodson@elastic.co Maintainer: Seth Michael Larson Maintainer-email:
-seth.larson@elastic.co License: Apache-2.0 Keywords: elastic eland pandas
-python Classifier: Development Status :: 5 - Production/Stable Classifier:
-License :: OSI Approved :: Apache Software License Classifier: Environment ::
-Console Classifier: Operating System :: OS Independent Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Topic :: Scientific/Engineering Requires-Python:
->=3.8 Description-Content-Type: text/markdown Provides-Extra: xgboost Provides-
-Extra: scikit-learn Provides-Extra: lightgbm Provides-Extra: pytorch Provides-
-Extra: all License-File: LICENSE.txt License-File: NOTICE.txt
+steve.dodson@elastic.co Maintainer: Elastic Client Library Maintainers
+Maintainer-email: client-libs@elastic.co License: Apache-2.0 Keywords: elastic
+eland pandas python Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Environment :: Console Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Science/Research Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
+xgboost Provides-Extra: scikit-learn Provides-Extra: lightgbm Provides-Extra:
+pytorch Provides-Extra: all License-File: LICENSE.txt License-File: NOTICE.txt
                                     _[_E_l_a_n_d_]
 
 _[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_C_o_n_d_a_ _V_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]_[_P_a_c_k_a_g_e_ _S_t_a_t_u_s_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]
                             _[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]
 ## About Eland is a Python Elasticsearch client for exploring and analyzing
 data in Elasticsearch with a familiar Pandas-compatible API. Where possible the
 package uses existing Python APIs and data structures to make it easy to switch
@@ -29,60 +29,60 @@
 provides tools to upload trained machine learning models from common libraries
 like [scikit-learn](https://scikit-learn.org), [XGBoost](https://
 xgboost.readthedocs.io), and [LightGBM](https://lightgbm.readthedocs.io) into
 Elasticsearch. ## Getting Started Eland can be installed from [PyPI](https://
 pypi.org/project/eland) with Pip: ```bash $ python -m pip install eland ```
 Eland can also be installed from [Conda Forge](https://anaconda.org/conda-
 forge/eland) with Conda: ```bash $ conda install -c conda-forge eland ``` ###
-Compatibility - Supports Python 3.8+ and Pandas 1.5 - Supports Elasticsearch
-clusters that are 7.11+, recommended 8.3 or later for all features to work. If
-you are using the NLP with PyTorch feature make sure your Eland minor version
-matches the minor version of your Elasticsearch cluster. For all other features
-it is sufficient for the major versions to match. - You need to use PyTorch
-`1.11.0` or earlier to import an NLP model. Run `pip install torch==1.11` to
-install the aproppriate version of PyTorch. ### Prerequisites Users installing
-Eland on Debian-based distributions may need to install prerequisite packages
-for the transitive dependencies of Eland: ```bash $ sudo apt-get install -y \
-build-essential pkg-config cmake \ python3-dev libzip-dev libjpeg-dev ``` Note
-that other distributions such as CentOS, RedHat, Arch, etc. may require using a
-different package manager and specifying different package names. ### Docker
-Users wishing to use Eland without installing it, in order to just run the
-available scripts, can build the Docker container: ```bash $ docker build -
-t elastic/eland . ``` The container can now be used interactively: ```bash $
-docker run -it --rm --network host elastic/eland ``` Running installed scripts
-is also possible without an interactive shell, e.g.: ```bash $ docker run -it -
--rm --network host \ elastic/eland \ eland_import_hub_model \ --url http://
-host.docker.internal:9200/ \ --hub-model-id elastic/distilbert-base-cased-
-finetuned-conll03-english \ --task-type ner \ --start ``` ### Connecting to
-Elasticsearch Eland uses the [Elasticsearch low level client](https://
-elasticsearch-py.readthedocs.io) to connect to Elasticsearch. This client
-supports a range of [connection options and authentication options](https://
-elasticsearch-py.readthedocs.io/en/stable/api.html#elasticsearch). You can pass
-either an instance of `elasticsearch.Elasticsearch` to Eland APIs or a string
-containing the host to connect to: ```python import eland as ed # Connecting to
-an Elasticsearch instance running on 'localhost:9200' df = ed.DataFrame
-("localhost:9200", es_index_pattern="flights") # Connecting to an Elastic Cloud
-instance from elasticsearch import Elasticsearch es = Elasticsearch
-( cloud_id="cluster-name:...", http_auth=("elastic", "") ) df = ed.DataFrame
-(es, es_index_pattern="flights") ``` ## DataFrames in Eland `eland.DataFrame`
-wraps an Elasticsearch index in a Pandas-like API and defers all processing and
-filtering of data to Elasticsearch instead of your local machine. This means
-you can process large amounts of data within Elasticsearch from a Jupyter
-Notebook without overloading your machine. â¤ [Eland DataFrame API
-documentation](https://eland.readthedocs.io/en/latest/reference/dataframe.html)
-â¤ [Advanced examples in a Jupyter Notebook](https://eland.readthedocs.io/en/
-latest/examples/demo_notebook.html) ```python >>> import eland as ed >>> #
-Connect to 'flights' index via localhost Elasticsearch node >>> df =
-ed.DataFrame('localhost:9200', 'flights') # eland.DataFrame instance has the
-same API as pandas.DataFrame # except all data is in Elasticsearch. See .info()
-memory usage. >>> df.head() AvgTicketPrice Cancelled ... dayOfWeek timestamp 0
-841.265642 False ... 0 2018-01-01 00:00:00 1 882.982662 False ... 0 2018-01-01
-18:27:00 2 190.636904 False ... 0 2018-01-01 17:11:14 3 181.694216 True ... 0
-2018-01-01 10:33:28 4 730.041778 False ... 0 2018-01-01 05:13:00 [5 rows x 27
-columns] >>> df.info()
+Compatibility - Supports Python 3.8, 3.9, 3.10 and Pandas 1.5 - Supports
+Elasticsearch clusters that are 7.11+, recommended 8.3 or later for all
+features to work. If you are using the NLP with PyTorch feature make sure your
+Eland minor version matches the minor version of your Elasticsearch cluster.
+For all other features it is sufficient for the major versions to match. - You
+need to use PyTorch `1.13.1` or earlier to import an NLP model. Run `pip
+install torch==1.13.1` to install the aproppriate version of PyTorch. ###
+Prerequisites Users installing Eland on Debian-based distributions may need to
+install prerequisite packages for the transitive dependencies of Eland: ```bash
+$ sudo apt-get install -y \ build-essential pkg-config cmake \ python3-dev
+libzip-dev libjpeg-dev ``` Note that other distributions such as CentOS,
+RedHat, Arch, etc. may require using a different package manager and specifying
+different package names. ### Docker Users wishing to use Eland without
+installing it, in order to just run the available scripts, can build the Docker
+container: ```bash $ docker build -t elastic/eland . ``` The container can now
+be used interactively: ```bash $ docker run -it --rm --network host elastic/
+eland ``` Running installed scripts is also possible without an interactive
+shell, e.g.: ```bash $ docker run -it --rm --network host \ elastic/eland \
+eland_import_hub_model \ --url http://host.docker.internal:9200/ \ --hub-model-
+id elastic/distilbert-base-cased-finetuned-conll03-english \ --task-type ner
+``` ### Connecting to Elasticsearch Eland uses the [Elasticsearch low level
+client](https://elasticsearch-py.readthedocs.io) to connect to Elasticsearch.
+This client supports a range of [connection options and authentication options]
+(https://elasticsearch-py.readthedocs.io/en/stable/api.html#elasticsearch). You
+can pass either an instance of `elasticsearch.Elasticsearch` to Eland APIs or a
+string containing the host to connect to: ```python import eland as ed #
+Connecting to an Elasticsearch instance running on 'localhost:9200' df =
+ed.DataFrame("localhost:9200", es_index_pattern="flights") # Connecting to an
+Elastic Cloud instance from elasticsearch import Elasticsearch es =
+Elasticsearch( cloud_id="cluster-name:...", http_auth=("elastic", "") ) df =
+ed.DataFrame(es, es_index_pattern="flights") ``` ## DataFrames in Eland
+`eland.DataFrame` wraps an Elasticsearch index in a Pandas-like API and defers
+all processing and filtering of data to Elasticsearch instead of your local
+machine. This means you can process large amounts of data within Elasticsearch
+from a Jupyter Notebook without overloading your machine. â¤ [Eland DataFrame
+API documentation](https://eland.readthedocs.io/en/latest/reference/
+dataframe.html) â¤ [Advanced examples in a Jupyter Notebook](https://
+eland.readthedocs.io/en/latest/examples/demo_notebook.html) ```python >>>
+import eland as ed >>> # Connect to 'flights' index via localhost Elasticsearch
+node >>> df = ed.DataFrame('localhost:9200', 'flights') # eland.DataFrame
+instance has the same API as pandas.DataFrame # except all data is in
+Elasticsearch. See .info() memory usage. >>> df.head() AvgTicketPrice Cancelled
+... dayOfWeek timestamp 0 841.265642 False ... 0 2018-01-01 00:00:00 1
+882.982662 False ... 0 2018-01-01 18:27:00 2 190.636904 False ... 0 2018-01-01
+17:11:14 3 181.694216 True ... 0 2018-01-01 10:33:28 4 730.041778 False ... 0
+2018-01-01 05:13:00 [5 rows x 27 columns] >>> df.info()
 eland.dataframe.DataFrame'> Index: 13059 entries, 0 to 13058 Data columns
 (total 27 columns): # Column Non-Null Count Dtype --- ------ -------------- ---
 -- 0 AvgTicketPrice 13059 non-null float64 1 Cancelled 13059 non-null bool 2
 Carrier 13059 non-null object ... 24 OriginWeather 13059 non-null object 25
 dayOfWeek 13059 non-null int64 26 timestamp 13059 non-null datetime64[ns]
 dtypes: bool(2), datetime64[ns](1), float64(5), int64(2), object(17) memory
 usage: 80.0 bytes Elasticsearch storage usage: 5.043 MB # Filtering of rows
@@ -111,26 +111,36 @@
 Elasticsearch with the training data >>> es_model.predict(training_data[0]) [0
 1 1 0 1 0 0 0 1 0] ``` ### NLP with PyTorch For NLP tasks, Eland allows
 importing PyTorch trained BERT models into Elasticsearch. Models can be either
 plain PyTorch models, or supported [transformers](https://huggingface.co/
 transformers) models from the [Hugging Face model hub](https://huggingface.co/
 models). ```bash $ eland_import_hub_model \ --url http://localhost:9200/ \ --
 hub-model-id elastic/distilbert-base-cased-finetuned-conll03-english \ --task-
-type ner \ --start ``` ```python >>> import elasticsearch >>> from pathlib
-import Path >>> from eland.ml.pytorch import PyTorchModel >>> from
-eland.ml.pytorch.transformers import TransformerModel # Load a Hugging Face
-transformers model directly from the model hub >>> tm = TransformerModel
-("elastic/distilbert-base-cased-finetuned-conll03-english", "ner") Downloading:
+type ner \ --start ``` The example above will automatically start a model
+deployment. This is a good shortcut for initial experimentation, but for
+anything that needs good throughput you should omit the `--start` argument from
+the Eland command line and instead start the model using the ML UI in Kibana.
+The `--start` argument will deploy the model with one allocation and one thread
+per allocation, which will not offer good performance. When starting the model
+deployment using the ML UI in Kibana or the Elasticsearch [API](https://
+www.elastic.co/guide/en/elasticsearch/reference/current/start-trained-model-
+deployment.html) you will be able to set the threading options to make the best
+use of your hardware. ```python >>> import elasticsearch >>> from pathlib
+import Path >>> from eland.common import es_version >>> from eland.ml.pytorch
+import PyTorchModel >>> from eland.ml.pytorch.transformers import
+TransformerModel >>> es = elasticsearch.Elasticsearch("http://elastic:
+mlqa_admin@localhost:9200") >>> es_cluster_version = es_version(es) # Load a
+Hugging Face transformers model directly from the model hub >>> tm =
+TransformerModel(model_id="elastic/distilbert-base-cased-finetuned-conll03-
+english", task_type="ner", es_version=es_cluster_version) Downloading:
 100%|ââââââââââ| 257/257 [00:00<00:00, 108kB/s]
 Downloading: 100%|ââââââââââ| 954/954 [00:00<00:00, 372kB/
 s] Downloading: 100%|ââââââââââ| 208k/208k [00:00<00:00,
 668kB/s] Downloading: 100%|ââââââââââ| 112/112 [00:00<00:
 00, 43.9kB/s] Downloading: 100%|ââââââââââ| 249M/249M [00:
 23<00:00, 11.2MB/s] # Export the model in a TorchScrpt representation which
 Elasticsearch uses >>> tmp_path = "models" >>> Path(tmp_path).mkdir
 (parents=True, exist_ok=True) >>> model_path, config, vocab_path = tm.save
-(tmp_path) # Import model into Elasticsearch >>> es =
-elasticsearch.Elasticsearch("http://elastic:mlqa_admin@localhost:9200",
-timeout=300) # 5 minute timeout >>> ptm = PyTorchModel(es,
+(tmp_path) # Import model into Elasticsearch >>> ptm = PyTorchModel(es,
 tm.elasticsearch_model_id()) >>> ptm.import_model(model_path=model_path,
 config_path=None, vocab_path=vocab_path, config=config)
 100%|ââââââââââ| 63/63 [00:12<00:00, 5.02it/s] ```
```

### Comparing `eland-8.7.0/eland.egg-info/SOURCES.txt` & `eland-8.9.0/eland.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE.txt
 MANIFEST.in
 NOTICE.txt
 README.md
 setup.cfg
 setup.py
-bin/eland_import_hub_model
 eland/__init__.py
 eland/_version.py
 eland/actions.py
 eland/arithmetics.py
 eland/common.py
 eland/conftest.py
 eland/dataframe.py
@@ -24,17 +23,20 @@
 eland/query_compiler.py
 eland/series.py
 eland/tasks.py
 eland/utils.py
 eland.egg-info/PKG-INFO
 eland.egg-info/SOURCES.txt
 eland.egg-info/dependency_links.txt
+eland.egg-info/entry_points.txt
 eland.egg-info/not-zip-safe
 eland.egg-info/requires.txt
 eland.egg-info/top_level.txt
+eland/cli/__init__.py
+eland/cli/eland_import_hub_model.py
 eland/ml/__init__.py
 eland/ml/_model_serializer.py
 eland/ml/_optional.py
 eland/ml/common.py
 eland/ml/ml_model.py
 eland/ml/exporters/__init__.py
 eland/ml/exporters/_sklearn_deserializers.py
```

### Comparing `eland-8.7.0/setup.py` & `eland-8.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,20 +52,20 @@
     for i, line in enumerate(lines):
         if line == "</p>":
             last_html_index = i + 1
     long_description = "\n".join(lines[last_html_index:])
 
 extras = {
     "xgboost": ["xgboost>=0.90,<2"],
-    "scikit-learn": ["scikit-learn>=0.22.1,<2"],
+    "scikit-learn": ["scikit-learn>=1.3,<2"],
     "lightgbm": ["lightgbm>=2,<4"],
     "pytorch": [
-        "torch>=1.11.0,<1.12.0",
+        "torch>=1.13.1,<2.0",
         "sentence-transformers>=2.1.0,<=2.2.2",
-        "transformers[torch]>=4.12.0,<=4.20.1",
+        "transformers[torch]>=4.12.0,<=4.27.4",
     ],
 }
 extras["all"] = list({dep for deps in extras.values() for dep in deps})
 
 setup(
     name=about["__title__"],
     version=about["__version__"],
@@ -79,18 +79,20 @@
     maintainer_email=about["__maintainer_email__"],
     license="Apache-2.0",
     classifiers=CLASSIFIERS,
     keywords="elastic eland pandas python",
     packages=find_packages(include=["eland", "eland.*"]),
     install_requires=[
         "elasticsearch>=8.3,<9",
-        "pandas>=1.5",
+        "pandas>=1.5,<2",
         "matplotlib>=3.6",
-        "numpy<2",
+        "numpy>=1.2.0,<1.24",
     ],
-    scripts=["bin/eland_import_hub_model"],
+    entry_points={
+        "console_scripts": "eland_import_hub_model=eland.cli.eland_import_hub_model:main"
+    },
     python_requires=">=3.8",
     package_data={"eland": ["py.typed"]},
     include_package_data=True,
     zip_safe=False,
     extras_require=extras,
 )
```

### Comparing `eland-8.7.0/tests/test_common_pytest.py` & `eland-8.9.0/tests/test_common_pytest.py`

 * *Files identical despite different names*

### Comparing `eland-8.7.0/tests/test_utils_pytest.py` & `eland-8.9.0/tests/test_utils_pytest.py`

 * *Files identical despite different names*


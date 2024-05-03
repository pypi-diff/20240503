# Comparing `tmp/exoml-0.1.5.tar.gz` & `tmp/exoml-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exoml-0.1.5.tar", last modified: Mon Jan 29 14:35:38 2024, max compression
+gzip compressed data, was "exoml-0.1.6.tar", last modified: Fri May  3 16:05:24 2024, max compression
```

## Comparing `exoml-0.1.5.tar` & `exoml-0.1.6.tar`

### file list

```diff
@@ -1,110 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.531529 exoml-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-01-29 14:35:38.531529 exoml-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-29 14:34:59.000000 exoml-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.511529 exoml-0.1.5/exoml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.511529 exoml-0.1.5/exoml/curve_prioritizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/curve_prioritizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/curve_prioritizer/curve_prioritizer_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/curve_prioritizer/curve_prioritizer_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.511529 exoml-0.1.5/exoml/detrend/
--rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/detrend/DETREND.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/detrend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/detrend/detrend_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.515529 exoml-0.1.5/exoml/ete6/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ete6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14866 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ete6/ete6_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.515529 exoml-0.1.5/exoml/iatson/
--rwxr-xr-x   0 runner    (1001) docker     (127)    23093 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/iatson/IATSON.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24283 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/iatson/IATSON_og.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    86699 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/iatson/IATSON_planet.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/iatson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/iatson/iatson_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/iatson/iatson_og_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    46616 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/iatson/iatson_planet_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    29748 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/iatson/watson_planet_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.515529 exoml-0.1.5/exoml/ml/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.515529 exoml-0.1.5/exoml/ml/calibration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/calibration/calibrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/calibration/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.519529 exoml-0.1.5/exoml/ml/callback/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/callback/auc.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/callback/basemodel_aware_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/callback/batch_aware_csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/callback/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/callback/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/callback/get_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/callback/learning_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/callback/training_data_aware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.519529 exoml-0.1.5/exoml/ml/encoding/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/encoding/time_position.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.519529 exoml-0.1.5/exoml/ml/functions/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/functions/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.519529 exoml-0.1.5/exoml/ml/layers/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/layers/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/layers/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/layers/transformer_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.523529 exoml-0.1.5/exoml/ml/learning_rate/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/learning_rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/learning_rate/schedulers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.523529 exoml-0.1.5/exoml/ml/log/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/log/get_weights_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/log/with_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.523529 exoml-0.1.5/exoml/ml/loss/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/loss/cross_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/loss/unsupervised.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.523529 exoml-0.1.5/exoml/ml/metrics/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18110 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/metrics/auc.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/metrics/fixed_mean.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3703 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/ml_data_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5180 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/ml_single_transits_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.523529 exoml-0.1.5/exoml/ml/model/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42228 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/model/binary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/model/categorical_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/model/imbalanced_binary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/model/imbalanced_categorical_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.527529 exoml-0.1.5/exoml/ml/physics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/physics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/physics/transit_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/ml/thread_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.527529 exoml-0.1.5/exoml/preparation/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/preparation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18135 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/preparation/empty_targets_preparer.py
--rw-r--r--   0 runner    (1001) docker     (127)    34080 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/preparation/ete6parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    30448 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/preparation/parser_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23784 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/preparation/q1q17dr25parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.527529 exoml-0.1.5/exoml/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 14:34:59.000000 exoml-0.1.5/exoml/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.527529 exoml-0.1.5/exoml/resources/q1_q17/
--rwxr-xr-x   0 runner    (1001) docker     (127)   114514 2024-01-29 14:35:11.000000 exoml-0.1.5/exoml/resources/q1_q17/apjac4399t13_mrt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.531529 exoml-0.1.5/exoml/santo/
--rw-r--r--   0 runner    (1001) docker     (127)    10492 2024-01-29 14:35:12.000000 exoml-0.1.5/exoml/santo/SANTO.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:12.000000 exoml-0.1.5/exoml/santo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-01-29 14:35:12.000000 exoml-0.1.5/exoml/santo/santo_test_data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.531529 exoml-0.1.5/exoml/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:12.000000 exoml-0.1.5/exoml/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      215 2024-01-29 14:35:12.000000 exoml-0.1.5/exoml/tests/test_exoml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.531529 exoml-0.1.5/exoml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-01-29 14:35:38.000000 exoml-0.1.5/exoml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-01-29 14:35:38.000000 exoml-0.1.5/exoml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 14:35:38.000000 exoml-0.1.5/exoml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-01-29 14:35:38.000000 exoml-0.1.5/exoml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-29 14:35:38.000000 exoml-0.1.5/exoml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-01-29 14:35:12.000000 exoml-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-01-29 14:35:12.000000 exoml-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 14:35:38.531529 exoml-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:38.531529 exoml-0.1.5/transpot/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11057 2024-01-29 14:35:12.000000 exoml-0.1.5/transpot/TRANSPOT.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:35:12.000000 exoml-0.1.5/transpot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-01-29 14:35:12.000000 exoml-0.1.5/transpot/transpot_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.780590 exoml-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-03 16:05:24.780590 exoml-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 16:05:04.000000 exoml-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.760590 exoml-0.1.6/exoml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.764590 exoml-0.1.6/exoml/curve_prioritizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/curve_prioritizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/curve_prioritizer/curve_prioritizer_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/curve_prioritizer/curve_prioritizer_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.764590 exoml-0.1.6/exoml/detrend/
+-rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/detrend/DETREND.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/detrend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/detrend/detrend_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.764590 exoml-0.1.6/exoml/ete6/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ete6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14866 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ete6/ete6_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.764590 exoml-0.1.6/exoml/iatson/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23093 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/iatson/IATSON.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24283 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/iatson/IATSON_og.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    86662 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/iatson/IATSON_planet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/iatson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/iatson/iatson_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/iatson/iatson_og_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46616 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/iatson/iatson_planet_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29748 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/iatson/watson_planet_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.768590 exoml-0.1.6/exoml/ml/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.768590 exoml-0.1.6/exoml/ml/calibration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/calibration/calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/calibration/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.768590 exoml-0.1.6/exoml/ml/callback/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/callback/auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/callback/basemodel_aware_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/callback/batch_aware_csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/callback/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/callback/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/callback/get_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21274 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/callback/learning_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/callback/training_data_aware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.768590 exoml-0.1.6/exoml/ml/encoding/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/encoding/time_position.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.768590 exoml-0.1.6/exoml/ml/functions/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/functions/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.772590 exoml-0.1.6/exoml/ml/layers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/layers/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/layers/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9851 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/layers/transformer_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.772590 exoml-0.1.6/exoml/ml/learning_rate/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/learning_rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/learning_rate/schedulers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.772590 exoml-0.1.6/exoml/ml/log/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/log/get_weights_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/log/with_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.772590 exoml-0.1.6/exoml/ml/loss/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/loss/cross_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/loss/unsupervised.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.772590 exoml-0.1.6/exoml/ml/metrics/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23950 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/metrics/auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/metrics/fixed_mean.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3703 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/ml_data_generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5180 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/ml_single_transits_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.772590 exoml-0.1.6/exoml/ml/model/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42083 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/model/binary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/model/categorical_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/model/imbalanced_binary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/model/imbalanced_categorical_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.776590 exoml-0.1.6/exoml/ml/physics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/physics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/physics/transit_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/thread_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.776590 exoml-0.1.6/exoml/preparation/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/preparation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18135 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/preparation/empty_targets_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34080 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/preparation/ete6parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31695 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/preparation/parser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27267 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/preparation/q1q17dr25parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.776590 exoml-0.1.6/exoml/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.776590 exoml-0.1.6/exoml/resources/q1_q17/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   114514 2024-05-03 16:05:13.000000 exoml-0.1.6/exoml/resources/q1_q17/apjac4399t13_mrt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.776590 exoml-0.1.6/exoml/santo/
+-rw-r--r--   0 runner    (1001) docker     (127)    35156 2024-05-03 16:05:13.000000 exoml-0.1.6/exoml/santo/SANTO.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:13.000000 exoml-0.1.6/exoml/santo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-03 16:05:13.000000 exoml-0.1.6/exoml/santo/santo_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-05-03 16:05:13.000000 exoml-0.1.6/exoml/santo/santo_test_data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.776590 exoml-0.1.6/exoml/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:13.000000 exoml-0.1.6/exoml/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      215 2024-05-03 16:05:13.000000 exoml-0.1.6/exoml/tests/test_exoml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.776590 exoml-0.1.6/exoml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-03 16:05:24.000000 exoml-0.1.6/exoml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-03 16:05:24.000000 exoml-0.1.6/exoml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:05:24.000000 exoml-0.1.6/exoml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-03 16:05:24.000000 exoml-0.1.6/exoml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 16:05:24.000000 exoml-0.1.6/exoml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-03 16:05:13.000000 exoml-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-03 16:05:13.000000 exoml-0.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:05:24.780590 exoml-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.776590 exoml-0.1.6/transpot/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11057 2024-05-03 16:05:13.000000 exoml-0.1.6/transpot/TRANSPOT.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:13.000000 exoml-0.1.6/transpot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-03 16:05:13.000000 exoml-0.1.6/transpot/transpot_generator.py
```

### Comparing `exoml-0.1.5/PKG-INFO` & `exoml-0.1.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: exoml
-Version: 0.1.5
+Version: 0.1.6
 Summary: ExoML tools for exoplanet detections
 Author-email: Martín Dévora-Pajares <mdevorapajares@protonmail.com>
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: keras==2.12.0
-Requires-Dist: tensorflow==2.12.0
-Requires-Dist: tensorflow-addons==0.21.0
+Requires-Dist: keras==2.15.0
+Requires-Dist: tensorflow==2.15.0
 Requires-Dist: ellc==1.8.8
-Requires-Dist: lcbuilder==0.16.4
+Requires-Dist: lcbuilder==0.17.0
 Requires-Dist: ruamel.yaml==0.17.32
 Requires-Dist: pydot==1.4.2
 Requires-Dist: graphviz==0.20.1
 Requires-Dist: pandas==1.5.3
 Requires-Dist: scikit-learn==1.2.2
 Requires-Dist: matplotlib==3.8.2
+Requires-Dist: typeguard==4.1.5
+Requires-Dist: tensorflow_addons
 
 # exoml
 ML POCs and projects for Exoplanets
```

### Comparing `exoml-0.1.5/exoml/curve_prioritizer/curve_prioritizer_generator.py` & `exoml-0.1.6/exoml/curve_prioritizer/curve_prioritizer_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/curve_prioritizer/curve_prioritizer_model.py` & `exoml-0.1.6/exoml/curve_prioritizer/curve_prioritizer_model.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/detrend/DETREND.py` & `exoml-0.1.6/exoml/detrend/DETREND.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/detrend/detrend_generator.py` & `exoml-0.1.6/exoml/detrend/detrend_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/ete6/ete6_generator.py` & `exoml-0.1.6/exoml/ete6/ete6_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/iatson/IATSON.py` & `exoml-0.1.6/exoml/iatson/IATSON.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/iatson/IATSON_og.py` & `exoml-0.1.6/exoml/iatson/IATSON_og.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/iatson/IATSON_planet.py` & `exoml-0.1.6/exoml/iatson/IATSON_planet.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import keras
 import tensorflow as tf
 from keras.layers import LeakyReLU
-from keras.utils import losses_utils
 from sklearn.isotonic import IsotonicRegression
 
 from sklearn.linear_model import LogisticRegression
 from sklearn.utils import shuffle
 from astropy import units as u
 from exoml.iatson.iatson_planet_generator import IatsonPlanetModelGenerator
 from exoml.iatson.watson_planet_generator import WatsonPlanetModelGenerator
```

### Comparing `exoml-0.1.5/exoml/iatson/iatson_generator.py` & `exoml-0.1.6/exoml/iatson/iatson_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/iatson/iatson_og_generator.py` & `exoml-0.1.6/exoml/iatson/iatson_og_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/iatson/iatson_planet_generator.py` & `exoml-0.1.6/exoml/iatson/iatson_planet_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/iatson/watson_planet_generator.py` & `exoml-0.1.6/exoml/iatson/watson_planet_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/ml/calibration/calibrator.py` & `exoml-0.1.6/exoml/ml/calibration/calibrator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/ml/calibration/utils.py` & `exoml-0.1.6/exoml/ml/calibration/utils.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/ml/callback/auc.py` & `exoml-0.1.6/exoml/ml/callback/auc.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/ml/callback/basemodel_aware_callback.py` & `exoml-0.1.6/exoml/ml/callback/basemodel_aware_callback.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/ml/callback/batch_aware_csv_logger.py` & `exoml-0.1.6/exoml/ml/callback/batch_aware_csv_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import collections
 import copy
 import csv
 import keras.backend as K
 from keras.callbacks import CSVLogger
 import numpy as np
-import tensorflow_addons as tfa
+from exoml.ml.callback.learning_rate import MultiOptimizer
 
 
 class BatchAwareCsvLogger(CSVLogger):
 
     def __init__(self, filename, steps_per_epoch, separator=',', append=False):
         super().__init__(filename, separator, append)
         self.steps_per_epoch = steps_per_epoch
@@ -40,25 +40,25 @@
             formatted_logs = dict((k, formatted_logs[k]) if k in formatted_logs else (k, 'NA') for k in keys)
         validation_fields = ['val_' + key for key in keys] if with_validation else []
         metric_fieldnames = list(keys) + validation_fields
         if not self.writer:
             class CustomDialect(csv.excel):
                 delimiter = self.sep
             lr_fieldnames = ['lr']
-            if isinstance(self.model.optimizer, tfa.optimizers.MultiOptimizer):
+            if isinstance(self.model.optimizer, MultiOptimizer):
                 lr_fieldnames = lr_fieldnames + ['lr_last']
             fieldnames = ['epoch', 'batch'] + lr_fieldnames +  metric_fieldnames
             self.writer = csv.DictWriter(
                 self.csv_file,
                 fieldnames=fieldnames,
                 dialect=CustomDialect)
             if self.append_header:
                 self.writer.writeheader()
         row_dict = {}
-        if isinstance(self.model.optimizer, tfa.optimizers.MultiOptimizer):
+        if isinstance(self.model.optimizer, MultiOptimizer):
             learning_rate = K.eval(K.eval(self.model.optimizer.optimizer_specs[0]['optimizer'].lr))
             last_learning_rate = K.eval(K.eval(self.model.optimizer.optimizer_specs[-1]['optimizer'].lr))
             row_dict['lr_last'] = last_learning_rate
         else:
             learning_rate = K.eval(self.model.optimizer.lr)
         row_dict['epoch'] = epoch
         row_dict['batch'] = batch
```

### Comparing `exoml-0.1.5/exoml/ml/callback/early_stopping.py` & `exoml-0.1.6/exoml/ml/callback/early_stopping.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/ml/callback/training_data_aware.py` & `exoml-0.1.6/exoml/ml/callback/training_data_aware.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/ml/layers/transformer.py` & `exoml-0.1.6/exoml/ml/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/ml/layers/transformer_classifier.py` & `exoml-0.1.6/exoml/ml/layers/transformer_classifier.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import tensorflow as tf
 from keras.layers import MultiHeadAttention, LeakyReLU
-import tensorflow_addons as tfa
-from keras.regularizers import L2
-from tensorflow_addons.layers import GELU
+from keras.src.layers import Dense
+from keras_nlp.src.layers import TransformerEncoder
 
 from exoml.ml.layers.dropout import AdaptiveStdDropout
 
 
 @tf.keras.utils.register_keras_serializable()
 class ClassToken(tf.keras.layers.Layer):
     """Append a class token to an input layer."""
@@ -62,83 +61,83 @@
         return config
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
 
 
-@tf.keras.utils.register_keras_serializable()
-class TransformerEncoder(tf.keras.layers.Layer):
-    """Implements a Transformer block."""
-
-    def __init__(self, *args, num_heads, mlp_dim, hyperparams, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.num_heads = num_heads
-        self.mlp_dim = mlp_dim
-        self.hyperparams = hyperparams
-        self.regularizer_value = 0.1
-
-    def build(self, input_shape):
-        self.att = MultiHeadAttention(num_heads=self.num_heads,
-            key_dim=input_shape[-1],
-            name="MultiHeadDotProductAttention_1"
-        )
-        self.mlpblock = tf.keras.Sequential(
-            [
-                tf.keras.layers.Dense(self.mlp_dim, activation=GELU(), name=f"{self.name}/Dense_0",
-                                      activity_regularizer=tf.keras.regularizers.L1L2(
-                                          l1=self.hyperparams.l1_regularization,
-                                          l2=self.hyperparams.l2_regularization)
-                                      ),
-                AdaptiveStdDropout(rate=self.hyperparams.dropout_rate,
-                                   max_rate=self.hyperparams.dropout_max_rate),
-                tf.keras.layers.Dense(input_shape[-1], name=f"{self.name}/Dense_1", activation=GELU(),
-                                      activity_regularizer=tf.keras.regularizers.L1L2(
-                                          l1=self.hyperparams.l1_regularization,
-                                          l2=self.hyperparams.l2_regularization)
-                                      )
-            ],
-            name="MlpBlock_3",
-        )
-        self.layernorm1 = tf.keras.layers.LayerNormalization(
-            epsilon=1e-6, name="LayerNorm_1"
-        )
-        self.layernorm2 = tf.keras.layers.LayerNormalization(
-            epsilon=1e-6, name="LayerNorm_2"
-        )
-        self.layernorm3 = tf.keras.layers.LayerNormalization(
-            epsilon=1e-6, name="LayerNorm_3"
-        )
-        self.dropout_layer = AdaptiveStdDropout(rate=self.hyperparams.dropout_rate,
-                                         max_rate=self.hyperparams.dropout_max_rate)
-
-    def call(self, inputs, training=True, return_attention_scores=True):
-        x = inputs
-        #x = self.layernorm1(x)
-        x, weights = self.att(x, x, training=training, return_attention_scores=return_attention_scores)
-        x = self.dropout_layer(x, training=training)
-        x = x + inputs
-        y = self.layernorm2(x)
-        y = self.mlpblock(y, training=training)
-        return self.layernorm3(x + y), weights
-
-    def get_config(self):
-        config = super().get_config()
-        config.update(
-            {
-                "num_heads": self.num_heads,
-                "mlp_dim": self.mlp_dim,
-                "dropout": self.hyperparams.dropout_rate,
-            }
-        )
-        return config
-
-    @classmethod
-    def from_config(cls, config):
-        return cls(**config)
+# @tf.keras.utils.register_keras_serializable()
+# class TransformerEncoder(tf.keras.layers.Layer):
+#     """Implements a Transformer block."""
+#
+#     def __init__(self, *args, num_heads, mlp_dim, hyperparams, **kwargs):
+#         super().__init__(*args, **kwargs)
+#         self.num_heads = num_heads
+#         self.mlp_dim = mlp_dim
+#         self.hyperparams = hyperparams
+#         self.regularizer_value = 0.1
+#
+#     def build(self, input_shape):
+#         self.att = MultiHeadAttention(num_heads=self.num_heads,
+#             key_dim=input_shape[-1],
+#             name="MultiHeadDotProductAttention_1"
+#         )
+#         self.mlpblock = tf.keras.Sequential(
+#             [
+#                 tf.keras.layers.Dense(self.mlp_dim, activation=LeakyReLU(), name=f"{self.name}/Dense_0",
+#                                       activity_regularizer=tf.keras.regularizers.L1L2(
+#                                           l1=self.hyperparams.l1_regularization,
+#                                           l2=self.hyperparams.l2_regularization)
+#                                       ),
+#                 AdaptiveStdDropout(rate=self.hyperparams.dropout_rate,
+#                                    max_rate=self.hyperparams.dropout_max_rate),
+#                 tf.keras.layers.Dense(input_shape[-1], name=f"{self.name}/Dense_1", activation=LeakyReLU(),
+#                                       activity_regularizer=tf.keras.regularizers.L1L2(
+#                                           l1=self.hyperparams.l1_regularization,
+#                                           l2=self.hyperparams.l2_regularization)
+#                                       )
+#             ],
+#             name="MlpBlock_3",
+#         )
+#         self.layernorm1 = tf.keras.layers.LayerNormalization(
+#             epsilon=1e-6, name="LayerNorm_1"
+#         )
+#         self.layernorm2 = tf.keras.layers.LayerNormalization(
+#             epsilon=1e-6, name="LayerNorm_2"
+#         )
+#         self.layernorm3 = tf.keras.layers.LayerNormalization(
+#             epsilon=1e-6, name="LayerNorm_3"
+#         )
+#         self.dropout_layer = AdaptiveStdDropout(rate=self.hyperparams.dropout_rate,
+#                                          max_rate=self.hyperparams.dropout_max_rate)
+#
+#     def call(self, inputs, training=True, return_attention_scores=True):
+#         x = inputs
+#         #x = self.layernorm1(x)
+#         x = self.att(x, x, training=training, return_attention_scores=return_attention_scores)
+#         x = self.dropout_layer(x, training=training)
+#         x = x + inputs
+#         y = self.layernorm2(x)
+#         y = self.mlpblock(y, training=training)
+#         return self.layernorm3(x + y)
+#
+#     def get_config(self):
+#         config = super().get_config()
+#         config.update(
+#             {
+#                 "num_heads": self.num_heads,
+#                 "mlp_dim": self.mlp_dim,
+#                 "dropout": self.hyperparams.dropout_rate,
+#             }
+#         )
+#         return config
+#
+#     @classmethod
+#     def from_config(cls, config):
+#         return cls(**config)
 
 
 @tf.keras.utils.register_keras_serializable()
 class Transformer(tf.keras.layers.Layer):
     def __init__(self, *args, num_heads, mlp_dim, hyperparams, num_blocks, **kwargs):
         super().__init__(*args, **kwargs)
         self.num_heads = num_heads
@@ -146,25 +145,36 @@
         self.hyperparams = hyperparams
         self.num_blocks = num_blocks
         self.transformer_encoders = []
         self.regularizer_value = 0.1
 
     def build(self, input_shape):
         for n in range(self.num_blocks):
-            self.transformer_encoders = self.transformer_encoders + [TransformerEncoder(
-                num_heads=self.num_heads,
-                mlp_dim=self.mlp_dim,
-                hyperparams=self.hyperparams,
-                name=f"Transformer/encoderblock_{n}"
+            self.transformer_encoders = self.transformer_encoders + \
+                                         [TransformerEncoder(
+                self.mlp_dim,
+                self.num_heads,
+                dropout=self.hyperparams.dropout_rate,
+                activation=LeakyReLU(),
+                layer_norm_epsilon=1e-05,
+                kernel_initializer="glorot_uniform",
+                bias_initializer="zeros",
+                normalize_first=False
             )]
+            # self.transformer_encoders = self.transformer_encoders + [TransformerEncoder(
+            #     num_heads=self.num_heads,
+            #     mlp_dim=self.mlp_dim,
+            #     hyperparams=self.hyperparams,
+            #     name=f"Transformer/encoderblock_{n}"
+            # )]
 
-    def call(self, inputs, training):
+    def call(self, inputs):
         result = inputs
         for n in range(self.num_blocks):
-            result, weights = self.transformer_encoders[n](result, training)
+            result = self.transformer_encoders[n](result)
         return result
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "num_heads": self.num_heads,
@@ -207,16 +217,16 @@
         #self.linear_proj = tf.keras.layers.Dense(self.transformer_input_size)
         # self.linear_proj = tf.keras.layers.Dense(self.transformer_input_size, activation="relu")
         #self.class_token = ClassToken(name="class_token")
         #self.add_pos_embedding = AddPositionEmbs(name="add_pos_embedding")
         self.transformer = Transformer(num_heads=self.num_heads, mlp_dim=self.mlp_dim,
                                        hyperparams=self.hyperparams, num_blocks=self.num_blocks)
         self.layer_norm = tf.keras.layers.LayerNormalization(epsilon=1e-6, name="Transformer/encoder_norm")
-        #activation = "softmax" if self.classes > 1 else "sigmoid"
-        self.head = tf.keras.layers.Dense(self.classes, name="head", activation=GELU(),
+        activation = "softmax" if self.classes > 1 else "sigmoid"
+        self.head = tf.keras.layers.Dense(self.classes, name="head", activation=activation,
                                           activity_regularizer=tf.keras.regularizers.L1L2(
                                               l1=self.hyperparams.l1_regularization,
                                               l2=self.hyperparams.l2_regularization)
                                           )
 
 
     def call(self, inputs, training=True):
```

### Comparing `exoml-0.1.5/exoml/ml/learning_rate/schedulers.py` & `exoml-0.1.6/exoml/ml/learning_rate/schedulers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import dataclasses
 
 import tensorflow as tf
-from keras.optimizers.schedules.learning_rate_schedule import LearningRateSchedule
+from keras.optimizers.schedules import LearningRateSchedule
 
 
 @dataclasses.dataclass(init=False)
 class ExponentialRescaleDecay(LearningRateSchedule):
     def __init__(
             self,
             initial_learning_rate,
```

### Comparing `exoml-0.1.5/exoml/ml/log/get_weights_logger.py` & `exoml-0.1.6/exoml/ml/log/get_weights_logger.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/ml/log/with_logging.py` & `exoml-0.1.6/exoml/ml/log/with_logging.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/ml/loss/cross_entropy.py` & `exoml-0.1.6/exoml/ml/loss/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/ml/loss/unsupervised.py` & `exoml-0.1.6/exoml/ml/loss/unsupervised.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/ml/ml_data_generator.py` & `exoml-0.1.6/exoml/ml/ml_data_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/ml/ml_single_transits_classifier.py` & `exoml-0.1.6/exoml/ml/ml_single_transits_classifier.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/ml/model/base_model.py` & `exoml-0.1.6/exoml/ml/model/base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 import copy
 import dataclasses
-import json
 import logging
 import os
-import shutil
-from copy import deepcopy
 from typing import List, Dict, Union, Any, Optional, Literal
 
 import numpy as np
 import tensorflow as tf
 import pandas as pd
-import ruamel.yaml
 from abc import abstractmethod
 
 from keras.optimizers import Adam
 from keras.utils import plot_model
 from sklearn.utils import shuffle
 
 from exoml.ml.callback.checkpoint import ModelCheckpointCallback
 from exoml.ml.callback.learning_rate import WarmUpAndLinDecreaseCallback
 from exoml.ml.callback.basemodel_aware_callback import MetricsPlotCallback
 from exoml.ml.callback.batch_aware_csv_logger import BatchAwareCsvLogger
 from exoml.ml.callback.early_stopping import ExoMlEarlyStopping
-from exoml.ml.callback.get_weights import GetWeights
 from exoml.ml.callback.training_data_aware import ValidationDataAwareCallback, ModelDirDataAwareCallback
 from exoml.ml.learning_rate.schedulers import ExponentialRescaleDecay
 from exoml.ml.log.get_weights_logger import ModelWeightsLogger
 from exoml.ml.log.with_logging import WithLogging
-from keras.optimizers.schedules.learning_rate_schedule import LearningRateSchedule
+from keras.optimizers.schedules import LearningRateSchedule
 
 from exoml.ml.metrics.auc import precision_at_k, mean_positive_value, mean_true_positive_value, mean_false_positive_value, \
     mean_true_negative_value, ThresholdAtPrecision
-import tensorflow_addons as tfa
+from exoml.ml.callback.learning_rate import MultiOptimizer, SWA
 
 
 @dataclasses.dataclass
 class HyperParams:
     '''Number of samples to be inclded in each mini-batch'''
     batch_size: int = 20
     '''Number of iterations over the entire dataset to be run before stopping'''
@@ -465,15 +460,15 @@
                     progressive_optimizer = self.build_swa_optimizer(hyperparams, progressive_lr_factor * initial_lr, steps_per_epoch)
                     progressive_optimizer.progressive_lr_factor = progressive_lr_factor
                     optimizers_and_layers = optimizers_and_layers + [
                         (progressive_optimizer, layer)]
                 else:
                     standard_layers = standard_layers + [layer]
             optimizers_and_layers = [(optimizer, standard_layers)] + optimizers_and_layers
-            optimizer = tfa.optimizers.MultiOptimizer(optimizers_and_layers)
+            optimizer = MultiOptimizer(optimizers_and_layers)
         return optimizer
 
     def compute_initial_lr(self, hyperparams: HyperParams):
         if hyperparams.lr_progression != 1:
             initial_lr = hyperparams.initial_learning_rate
         else:
             initial_lr = hyperparams.learning_rate_schedule \
@@ -482,15 +477,15 @@
 
     def build_swa_optimizer(self, hyperparams: HyperParams, lr, steps_per_epoch):
         if hyperparams.stochastic_weight_average_wait > 0:
             optimizer = tf.keras.optimizers.legacy.Adam(lr,
                                                         beta_1=0.9, beta_2=0.98, epsilon=1e-9,
                                                         clipnorm=hyperparams.gradient_clip_norm,
                                                         clipvalue=hyperparams.gradient_clip_value)
-            optimizer = tfa.optimizers.SWA(optimizer,
+            optimizer = SWA(optimizer,
                                            start_averaging=steps_per_epoch * hyperparams.stochastic_weight_average_wait,
                                            average_period=steps_per_epoch)
             if isinstance(lr, (int, float)):
                 optimizer.lr = lr
             else:
                 optimizer.lr = hyperparams.initial_learning_rate
         else:
```

### Comparing `exoml-0.1.5/exoml/ml/model/binary_model.py` & `exoml-0.1.6/exoml/ml/model/binary_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import logging
 
 from keras.losses import BinaryCrossentropy
 from keras.metrics import Precision, Recall, AUC, BinaryAccuracy, RecallAtPrecision
-from tensorflow_addons.metrics import F1Score
-
 from exoml.ml.loss.cross_entropy import binary_focal_loss
 from exoml.ml.metrics.auc import precision_at_k, mean_true_positive_value, mean_true_negative_value, \
     mean_false_negative_value, mean_false_positive_value, ThresholdAtPrecision
 from exoml.ml.model.base_model import BaseModel
 import pandas as pd
 import matplotlib.pyplot as plt
 
@@ -17,15 +15,15 @@
         super().__init__(name, input_size, class_ids, type_to_label, hyperparams)
 
     def instance_loss_accuracy(self):
         return BinaryCrossentropy(), BinaryAccuracy()
 
     def instance_metrics(self):
         return [Precision(name="precision"), Recall(name="recall"),
-                F1Score(num_classes=1, threshold=0.5, average='weighted', name='f1_score'),
+                #F1Score(num_classes=1, threshold=0.5, average='weighted', name='f1_score'),
                 RecallAtPrecision(precision=0.99, name="r@p99", num_thresholds=1000),
                 #ThresholdAtPrecision(precision=0.99, name="t@p99", num_thresholds=1000),
                 AUC(name="roc_auc"),
                 AUC(curve="PR", name="pr_auc")]
 
     def plot_metrics(self, model_dir, steps_per_epoch, with_validation=False):
         logging.info("Plotting metrics")
```

### Comparing `exoml-0.1.5/exoml/ml/model/categorical_model.py` & `exoml-0.1.6/exoml/ml/model/categorical_model.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/ml/physics/transit_functions.py` & `exoml-0.1.6/exoml/ml/physics/transit_functions.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/preparation/empty_targets_preparer.py` & `exoml-0.1.6/exoml/preparation/empty_targets_preparer.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/preparation/ete6parser.py` & `exoml-0.1.6/exoml/preparation/ete6parser.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/preparation/parser_utils.py` & `exoml-0.1.6/exoml/preparation/parser_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,29 +4,33 @@
 import os
 import sys
 import pathlib
 import re
 from itertools import chain
 from multiprocessing import Pool
 
+import gzip
+import shutil
 import lcbuilder.constants
 import triceratops.triceratops as tr
 import astropy.units as u
 import foldedleastsquares
 import lightkurve
 import numpy as np
 import wotan
 import pandas as pd
 from lcbuilder import constants
 from astropy.coordinates import SkyCoord
 from astropy.wcs import WCS
 from astroquery.mast import Catalogs, TesscutClass
 from lcbuilder.helper import LcbuilderHelper
 from lcbuilder.lcbuilder_class import LcBuilder
+from lcbuilder.objectinfo.MissionInputObjectInfo import MissionInputObjectInfo
 from lcbuilder.objectinfo.MissionObjectInfo import MissionObjectInfo
+from lcbuilder.objectinfo.preparer.MissionInputLightcurveBuilder import MissionInputLightcurveBuilder
 from lcbuilder.objectinfo.preparer.MissionLightcurveBuilder import MissionLightcurveBuilder
 from lcbuilder.photometry.aperture_extractor import ApertureExtractor
 from lcbuilder.star.HabitabilityCalculator import HabitabilityCalculator
 from lightkurve import TessLightCurve, KeplerLightCurve
 from watson.watson import Watson
 
 
@@ -375,63 +379,79 @@
         self.force = force
         self.tpf_files = tpf_files
         self.inject_random = inject_random
         self.mode = mode
 
 def create_target_csv(create_target_input):
     mission_lightcurve_builder = MissionLightcurveBuilder()
+    mission_input_lightcurve_builder = MissionInputLightcurveBuilder()
     mission_id = create_target_input.id
     file_id = mission_id.replace(' ', '_')
     file_prefix = create_target_input.target_dir + file_id
     file_planet_prefix = file_prefix + '_' + \
                          str(round(create_target_input.injected_files_df['period'], 2))
     pid = multiprocessing.current_process().pid
     tpfs_dir = create_target_input.target_dir + 'tpfs/'
     try:
         logging.info("PID %s: Trying to get short cadence info for %s", pid, file_planet_prefix)
         file_name = file_planet_prefix + '_metrics_short.csv'
         if create_target_input.force or not os.path.exists(file_name):
-            lcbuild_short = \
-                mission_lightcurve_builder.build(MissionObjectInfo('all', mission_id, cadence='short', high_rms_enabled=False),
-                                                 create_target_input.target_dir,
-                                                 create_target_input.cache_dir)
-            if os.path.exists(tpfs_dir):
-                for f in glob.glob(tpfs_dir + f"*{mission_id}*.fits"):
-                    os.remove(f)
+            if create_target_input.lc_file is None:
+                lcbuild_short = \
+                    mission_lightcurve_builder.build(MissionObjectInfo('all', mission_id, cadence='short', high_rms_enabled=False),
+                                                     create_target_input.target_dir,
+                                                     create_target_input.cache_dir)
+                if os.path.exists(tpfs_dir):
+                    for f in glob.glob(tpfs_dir + f"*{mission_id}*.fits"):
+                        os.remove(f)
+            else:
+                lc = KeplerLightCurve.read(create_target_input.lc_file)
+                lc_df = pd.DataFrame(columns=['#time', 'flux', 'flux_err'])
+                lc_df['#time'] = lc.time
+                lc_df['flux'] = lc.PDCSAP_FLUX
+                lc_df['flux_err'] = lc.flux_err
+                csv_filename = os.path.splitext(create_target_input.lc_file)[0] + '.csv'
+                lc_df.to_csv(csv_filename, index=False)
+                lcbuild_short = \
+                    mission_input_lightcurve_builder.build(
+                        MissionInputObjectInfo(mission_id, input_file=csv_filename, high_rms_enabled=False),
+                        create_target_input.target_dir,
+                        create_target_input.cache_dir)
             prepare_lc_data(file_planet_prefix, mission_id, lcbuild_short.lc_data,
                             create_target_input.injected_files_df['duration(h)'] / 24,
                             create_target_input.injected_files_df['period'],
                             create_target_input.injected_files_df['epoch'],
                             lcbuild_short.star_info.ra, lcbuild_short.star_info.dec, lcbuild_short.star_info, False,
                             modes=create_target_input.mode)
             for f in pathlib.Path(tpfs_dir).glob(f"*{file_id.split('_')[1]}*"):
                 os.remove(f)
         logging.info("PID %s: Finished to get short cadence info for %s", pid, file_planet_prefix)
     except Exception as e:
         logging.exception("PID %s: Failed short cadence for %s", pid, file_planet_prefix)
-    try:
-        logging.info("PID %s: Trying to get long cadence info for %s", pid, file_planet_prefix)
-        file_name = file_planet_prefix + '_metrics_long.csv'
-        if create_target_input.force or not os.path.exists(file_name):
-            lcbuild_long = \
-                mission_lightcurve_builder.build(MissionObjectInfo('all', mission_id, cadence='long', high_rms_enabled=False),
-                                                     create_target_input.target_dir,
-                                                     create_target_input.cache_dir)
-            prepare_lc_data(file_planet_prefix, mission_id, lcbuild_long.lc_data,
-                            create_target_input.injected_files_df['duration(h)'] / 24,
-                            create_target_input.injected_files_df['period'],
-                            create_target_input.injected_files_df['epoch'],
-                            lcbuild_long.star_info.ra, lcbuild_long.star_info.dec, lcbuild_long.star_info, True,
-                            modes=create_target_input.mode)
-            for f in pathlib.Path(tpfs_dir).glob(f"*{file_id.split('_')[1]}*"):
-                os.remove(f)
-        logging.info("PID %s: Finished to get long cadence info for index %s for file %s", pid,
-                     create_target_input.index, file_planet_prefix)
-    except Exception as e:
-        logging.exception("PID %s: Failed long cadence for %s", pid, file_planet_prefix)
+    if create_target_input.lc_file is not None:
+        try:
+            logging.info("PID %s: Trying to get long cadence info for %s", pid, file_planet_prefix)
+            file_name = file_planet_prefix + '_metrics_long.csv'
+            if create_target_input.force or not os.path.exists(file_name):
+                lcbuild_long = \
+                    mission_lightcurve_builder.build(MissionObjectInfo('all', mission_id, cadence='long', high_rms_enabled=False),
+                                                         create_target_input.target_dir,
+                                                         create_target_input.cache_dir)
+                prepare_lc_data(file_planet_prefix, mission_id, lcbuild_long.lc_data,
+                                create_target_input.injected_files_df['duration(h)'] / 24,
+                                create_target_input.injected_files_df['period'],
+                                create_target_input.injected_files_df['epoch'],
+                                lcbuild_long.star_info.ra, lcbuild_long.star_info.dec, lcbuild_long.star_info, True,
+                                modes=create_target_input.mode)
+                for f in pathlib.Path(tpfs_dir).glob(f"*{file_id.split('_')[1]}*"):
+                    os.remove(f)
+            logging.info("PID %s: Finished to get long cadence info for index %s for file %s", pid,
+                         create_target_input.index, file_planet_prefix)
+        except Exception as e:
+            logging.exception("PID %s: Failed long cadence for %s", pid, file_planet_prefix)
 
 def create_triceratops_prob(create_target_input):
     object_id = create_target_input.id
     file_id = object_id.replace(' ', '_')
     file_prefix = create_target_input.target_dir + file_id
     file_planet_prefix = file_prefix + '_' + \
                          str(round(create_target_input.injected_files_df['period'], 2))
```

### Comparing `exoml-0.1.5/exoml/preparation/q1q17dr25parser.py` & `exoml-0.1.6/exoml/preparation/q1q17dr25parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+import gzip
 import multiprocessing
+import os
+import re
+import shutil
 from multiprocessing import Pool
 import pandas as pd
 import numpy as np
 
-from preparation.parser_utils import CreateTargetInput, create_target_csv, create_triceratops_prob
+from exoml.preparation.parser_utils import CreateTargetInput, create_target_csv, create_triceratops_prob
 
 def create_targets_df(tces_dir):
     # Merge TCEs DF and cumulative DF ignoring everything not from Kepler or K2
     # Mark TCEs as planet only if they have photometric and rv measurements
     # test_df = pd.read_csv(tces_dir + '/classified_tces.csv', comment='#')
     # test_df = test_df.sort_values(by=["object_id", "period"], ascending=True)
     # test_df = test_df[test_df['type'].isin(['fp', 'planet', 'planet_transit', 'tce'])]
@@ -260,14 +264,61 @@
                                                   'tce_odd_even'])]
     result_df = result_df[~result_df['radius(earth)'].isna()]
     #TODO this next statement is to prevent confirmed planets not matching any tce nor koi
     #result_df = result_df[~result_df['object_id'].str.contains('<NA')]
     result_df.to_csv(tces_dir + '/injected_objects_tces_multi.csv')
 
 
+def create_synth_targets_df(tces_dir):
+    inj1_df = pd.read_csv(tces_dir + '/kplr_dr25_inj1_tces.csv', comment='#')
+    inj1_df['type'] = 'inj1'
+    inj2_df = pd.read_csv(tces_dir + '/kplr_dr25_inj2_tces.csv', comment='#')
+    inj2_df['type'] = 'inj2'
+    inj3_df = pd.read_csv(tces_dir + '/kplr_dr25_inj3_tces.csv', comment='#')
+    inj3_df['type'] = 'inj3'
+    inv_df = pd.read_csv(tces_dir + '/kplr_dr25_inv_tces.csv', comment='#')
+    inv_df['type'] = 'inv'
+    scr1_df = pd.read_csv(tces_dir + '/kplr_dr25_scr1_tces.csv', comment='#')
+    scr1_df['type'] = 'scr1'
+    scr2_df = pd.read_csv(tces_dir + '/kplr_dr25_scr2_tces.csv', comment='#')
+    scr2_df['type'] = 'scr2'
+    scr3_df = pd.read_csv(tces_dir + '/kplr_dr25_scr3_tces.csv', comment='#')
+    scr3_df['type'] = 'scr3'
+    synth_df = pd.concat([inj1_df, inj2_df, inj3_df, inv_df, scr1_df, scr2_df, scr3_df], ignore_index=True)
+    synth_df['duration(h)'] = synth_df['duration']
+    synth_df['depth_primary'] = synth_df['depth']
+    synth_df['radius(earth)'] = synth_df['Rp']
+    synth_df.to_csv(tces_dir + '/classified_tces_synthetic.csv')
+
+def download_synth_targets(download_dir, wget_files, df_file):
+    df = pd.read_csv(df_file, comment='#')
+    os.chdir(download_dir)
+    pattern = r'kplr(\d+).*'
+    pattern_date = r'(\d+)\_INJECTED.*'
+    for wget_file in wget_files:
+        with open(wget_file, 'r') as file:
+            for line in file:
+                match = re.search(pattern, line)
+                if match is not None:
+                    kepid = int(match.group(1))
+                    rows = df[df['KIC'] == kepid]
+                    for index, row in rows.iterrows():
+                        if 'inj' in row['type']:
+                            print(f"Downloading: {line}")
+                            os.system(line)
+                            match_date = re.search(pattern_date, line)
+                            lc_file = f'{download_dir}/kplr{kepid:09}-{match_date.group(1)}_INJECTED-' + row['type'] + '_llc.fits'
+                            compressed_file = f'{lc_file}.gz'
+                            if os.path.exists(compressed_file):
+                                with gzip.open(compressed_file, 'rb') as f_in:
+                                    with open(lc_file, 'wb') as f_out:
+                                        shutil.copyfileobj(f_in, f_out)
+                                        os.remove(compressed_file)
+
+
 def create_target_csvs(csv, target_dir, cache_dir, cores=multiprocessing.cpu_count() - 1, force=False, ids=None,
                        mode='all'):
     tces_df = pd.read_csv(csv, comment='#')
     tces_df = tces_df.sort_values(by=["kepid"], ascending=True)
     #tces_df = tces_df.drop_duplicates(subset=["kepid"], keep='last')
     tces_df = tces_df.sort_values(by=["period"], ascending=True)
     #tces_df = tces_df.sample(frac=1).reset_index(drop=True)
@@ -279,14 +330,33 @@
     print("Total number of targets is " + str(len(tces_df)))
     for index in ranges:
         tce_row = tces_df.iloc[index]
         inputs = inputs + [CreateTargetInput('KIC', tce_row['object_id'], None, target_dir, None, tce_row, cache_dir, index, force=force, mode=mode)]
     with Pool(processes=cores, maxtasksperchild=1) as pool:
         pool.map(create_target_csv, inputs, chunksize=1)
 
+
+def create_synth_curves(csv, lcs_dir, target_dir, cache_dir, cores=multiprocessing.cpu_count() - 1, force=False, ids=None, mode='all'):
+    synth_df = pd.read_csv(csv, comment='#')
+    synth_df = synth_df.sort_values(by=["TCE_ID"], ascending=True)
+    inputs = []
+    if ids is not None:
+        synth_df = synth_df[synth_df['TCE_ID'].isin(ids)]
+    synth_df = synth_df.reset_index(drop=True)
+    ranges = range(0, len(synth_df))
+    print("Total number of targets is " + str(len(synth_df)))
+    for index in ranges:
+        tce_row = synth_df.iloc[index]
+        kepid = int(tce_row['KIC'])
+        lc_file = None if 'inj' not in tce_row['type'] \
+            else f'{lcs_dir}/kplr{kepid:09}-2011271113734_INJECTED-' + tce_row['type'] + '_llc.fits'
+        inputs = inputs + [CreateTargetInput('KIC', kepid, lc_file, target_dir, None, tce_row, cache_dir, index, force=force, mode=mode)]
+    with Pool(processes=cores, maxtasksperchild=1) as pool:
+        pool.map(create_target_csv, inputs, chunksize=1)
+
 def create_triceratops_probs(csv, target_dir, cache_dir, cores=multiprocessing.cpu_count() - 1, force=False, ids=None):
     tces_df = pd.read_csv(csv, comment='#')
     tces_df = tces_df.sort_values(by=["kepid"], ascending=True)
     # tces_df = tces_df.drop_duplicates(subset=["kepid"], keep='last')
     #tces_df = tces_df.sample(frac=1).reset_index(drop=True)
     if not force and 'tric_tp_total' in tces_df.columns:
         tces_df = tces_df.loc[tces_df['tric_tp_total'].isna()]
```

### Comparing `exoml-0.1.5/exoml/resources/q1_q17/apjac4399t13_mrt.txt` & `exoml-0.1.6/exoml/resources/q1_q17/apjac4399t13_mrt.txt`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/exoml/santo/santo_test_data_generator.py` & `exoml-0.1.6/exoml/santo/santo_test_data_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-import os
 import sys
 
 import matplotlib.pyplot as plt
 import random
 from typing import Tuple
 import ellc
 import numpy as np
@@ -16,15 +15,14 @@
 
 class SantoTestDataGenerator:
     random_number_generator = default_rng()
 
     def __init__(self, output_dir: str, curves_len_boundaries: Tuple[int],
                  transit_depth_boundaries: Tuple[float],
                  transit_period_avg_std: Tuple[float],
-                 max_number_of_planets: int,
                  white_noise_power_boundaries: Tuple[float],
                  red_noise_frequency_boundaries: Tuple[float],
                  red_noise_power_boundaries: Tuple[float],
                  max_number_of_red_noise: int,
                  curves_count=10000, curves_cadence=120, only_plot=False):
         curves_with_planets = 0
         curves_with_red_noise = 0
@@ -58,23 +56,21 @@
                 timeseries_rn: ndarray = np.zeros(curve_len)
                 for time_index, value in enumerate(time):
                     rn_value = red_noise.sample_next(value, None, None)
                     rn_value = rn_value[0] if isinstance(rn_value, (list, np.ndarray)) else rn_value
                     timeseries_rn[time_index] = rn_value
                 flux[0] = flux[0] + timeseries_rn
             number_of_planets = random.uniform(0, 100)
-            if number_of_planets < 80:
-                number_of_planets = 0
-            elif number_of_planets < 95:
+            if number_of_planets < 50:
                 number_of_planets = 1
-            elif number_of_planets < 97:
+            elif number_of_planets < 80:
                 number_of_planets = 2
             else:
-                number_of_planets = int(random.uniform(3, max_number_of_planets))
-            curves_with_planets = curves_with_planets if number_of_planets == 0 else curves_with_planets + 1
+                number_of_planets = 3
+            curves_with_planets = curves_with_planets + 1
             star_radius = 1
             star_mass = 1
             for index in range(0, number_of_planets):
                 period = random.gauss(transit_period_avg_std[0], transit_period_avg_std[1])
                 if period < 0.5:
                     period = 0.5
                 t0 = time[0] + period / random.uniform(0, 1)
@@ -142,13 +138,12 @@
 
 SantoTestDataGenerator(output_dir="/data/scratch/ml/santo/training_data/",
                        curves_len_boundaries=(15000, 30000),
                        curves_count=10000,
                        curves_cadence=120,
                        transit_depth_boundaries=(0.0001, 0.05),
                        transit_period_avg_std=(7.5, 6),
-                       max_number_of_planets=6,
                        red_noise_frequency_boundaries=(0.01, 10),
                        red_noise_power_boundaries=(0.001, 0.05),
                        white_noise_power_boundaries=(0.001, 0.05),
                        max_number_of_red_noise=5,
                        only_plot=False)
```

### Comparing `exoml-0.1.5/exoml.egg-info/PKG-INFO` & `exoml-0.1.6/exoml.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: exoml
-Version: 0.1.5
+Version: 0.1.6
 Summary: ExoML tools for exoplanet detections
 Author-email: Martín Dévora-Pajares <mdevorapajares@protonmail.com>
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: keras==2.12.0
-Requires-Dist: tensorflow==2.12.0
-Requires-Dist: tensorflow-addons==0.21.0
+Requires-Dist: keras==2.15.0
+Requires-Dist: tensorflow==2.15.0
 Requires-Dist: ellc==1.8.8
-Requires-Dist: lcbuilder==0.16.4
+Requires-Dist: lcbuilder==0.17.0
 Requires-Dist: ruamel.yaml==0.17.32
 Requires-Dist: pydot==1.4.2
 Requires-Dist: graphviz==0.20.1
 Requires-Dist: pandas==1.5.3
 Requires-Dist: scikit-learn==1.2.2
 Requires-Dist: matplotlib==3.8.2
+Requires-Dist: typeguard==4.1.5
+Requires-Dist: tensorflow_addons
 
 # exoml
 ML POCs and projects for Exoplanets
```

### Comparing `exoml-0.1.5/exoml.egg-info/SOURCES.txt` & `exoml-0.1.6/exoml.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -71,13 +71,14 @@
 exoml/preparation/ete6parser.py
 exoml/preparation/parser_utils.py
 exoml/preparation/q1q17dr25parser.py
 exoml/resources/__init__.py
 exoml/resources/q1_q17/apjac4399t13_mrt.txt
 exoml/santo/SANTO.py
 exoml/santo/__init__.py
+exoml/santo/santo_generator.py
 exoml/santo/santo_test_data_generator.py
 exoml/tests/__init__.py
 exoml/tests/test_exoml.py
 transpot/TRANSPOT.py
 transpot/__init__.py
 transpot/transpot_generator.py
```

### Comparing `exoml-0.1.5/pyproject.toml` & `exoml-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 description = "ExoML tools for exoplanet detections"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = []
 license = {text = "MIT"}
 dynamic = ["dependencies"]
-version = "0.1.5"
+version = "0.1.6"
 
 [project.optional-dependencies]
 
 [project.scripts]
 #my-script = "my_package.module:function"
 
 [tool.setuptools]
```

### Comparing `exoml-0.1.5/transpot/TRANSPOT.py` & `exoml-0.1.6/transpot/TRANSPOT.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.5/transpot/transpot_generator.py` & `exoml-0.1.6/transpot/transpot_generator.py`

 * *Files identical despite different names*


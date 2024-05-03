# Comparing `tmp/exoml-0.1.6.tar.gz` & `tmp/exoml-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exoml-0.1.6.tar", last modified: Fri May  3 16:05:24 2024, max compression
+gzip compressed data, was "exoml-0.1.7.tar", last modified: Fri May  3 18:21:34 2024, max compression
```

## Comparing `exoml-0.1.6.tar` & `exoml-0.1.7.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.780590 exoml-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-03 16:05:24.780590 exoml-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 16:05:04.000000 exoml-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.760590 exoml-0.1.6/exoml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.764590 exoml-0.1.6/exoml/curve_prioritizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/curve_prioritizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/curve_prioritizer/curve_prioritizer_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/curve_prioritizer/curve_prioritizer_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.764590 exoml-0.1.6/exoml/detrend/
--rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/detrend/DETREND.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/detrend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/detrend/detrend_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.764590 exoml-0.1.6/exoml/ete6/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ete6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14866 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ete6/ete6_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.764590 exoml-0.1.6/exoml/iatson/
--rwxr-xr-x   0 runner    (1001) docker     (127)    23093 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/iatson/IATSON.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24283 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/iatson/IATSON_og.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    86662 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/iatson/IATSON_planet.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/iatson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/iatson/iatson_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/iatson/iatson_og_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    46616 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/iatson/iatson_planet_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    29748 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/iatson/watson_planet_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.768590 exoml-0.1.6/exoml/ml/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.768590 exoml-0.1.6/exoml/ml/calibration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/calibration/calibrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/calibration/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.768590 exoml-0.1.6/exoml/ml/callback/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/callback/auc.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/callback/basemodel_aware_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/callback/batch_aware_csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/callback/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/callback/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/callback/get_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)    21274 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/callback/learning_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/callback/training_data_aware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.768590 exoml-0.1.6/exoml/ml/encoding/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/encoding/time_position.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.768590 exoml-0.1.6/exoml/ml/functions/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/functions/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.772590 exoml-0.1.6/exoml/ml/layers/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/layers/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/layers/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9851 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/layers/transformer_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.772590 exoml-0.1.6/exoml/ml/learning_rate/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/learning_rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/learning_rate/schedulers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.772590 exoml-0.1.6/exoml/ml/log/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/log/get_weights_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/log/with_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.772590 exoml-0.1.6/exoml/ml/loss/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/loss/cross_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/loss/unsupervised.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.772590 exoml-0.1.6/exoml/ml/metrics/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23950 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/metrics/auc.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/metrics/fixed_mean.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3703 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/ml_data_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5180 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/ml_single_transits_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.772590 exoml-0.1.6/exoml/ml/model/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42083 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/model/binary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/model/categorical_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/model/imbalanced_binary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/model/imbalanced_categorical_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.776590 exoml-0.1.6/exoml/ml/physics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/physics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/physics/transit_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/ml/thread_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.776590 exoml-0.1.6/exoml/preparation/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/preparation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18135 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/preparation/empty_targets_preparer.py
--rw-r--r--   0 runner    (1001) docker     (127)    34080 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/preparation/ete6parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    31695 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/preparation/parser_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    27267 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/preparation/q1q17dr25parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.776590 exoml-0.1.6/exoml/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:04.000000 exoml-0.1.6/exoml/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.776590 exoml-0.1.6/exoml/resources/q1_q17/
--rwxr-xr-x   0 runner    (1001) docker     (127)   114514 2024-05-03 16:05:13.000000 exoml-0.1.6/exoml/resources/q1_q17/apjac4399t13_mrt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.776590 exoml-0.1.6/exoml/santo/
--rw-r--r--   0 runner    (1001) docker     (127)    35156 2024-05-03 16:05:13.000000 exoml-0.1.6/exoml/santo/SANTO.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:13.000000 exoml-0.1.6/exoml/santo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-03 16:05:13.000000 exoml-0.1.6/exoml/santo/santo_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-05-03 16:05:13.000000 exoml-0.1.6/exoml/santo/santo_test_data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.776590 exoml-0.1.6/exoml/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:13.000000 exoml-0.1.6/exoml/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      215 2024-05-03 16:05:13.000000 exoml-0.1.6/exoml/tests/test_exoml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.776590 exoml-0.1.6/exoml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-03 16:05:24.000000 exoml-0.1.6/exoml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-03 16:05:24.000000 exoml-0.1.6/exoml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:05:24.000000 exoml-0.1.6/exoml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-03 16:05:24.000000 exoml-0.1.6/exoml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 16:05:24.000000 exoml-0.1.6/exoml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-03 16:05:13.000000 exoml-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-03 16:05:13.000000 exoml-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:05:24.780590 exoml-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:24.776590 exoml-0.1.6/transpot/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11057 2024-05-03 16:05:13.000000 exoml-0.1.6/transpot/TRANSPOT.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:13.000000 exoml-0.1.6/transpot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-03 16:05:13.000000 exoml-0.1.6/transpot/transpot_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.087559 exoml-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-03 18:21:34.087559 exoml-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 18:21:10.000000 exoml-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.067559 exoml-0.1.7/exoml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.071559 exoml-0.1.7/exoml/curve_prioritizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/curve_prioritizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/curve_prioritizer/curve_prioritizer_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/curve_prioritizer/curve_prioritizer_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.071559 exoml-0.1.7/exoml/detrend/
+-rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/detrend/DETREND.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/detrend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/detrend/detrend_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.071559 exoml-0.1.7/exoml/ete6/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ete6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14866 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ete6/ete6_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.071559 exoml-0.1.7/exoml/iatson/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23093 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/iatson/IATSON.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24283 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/iatson/IATSON_og.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    86662 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/iatson/IATSON_planet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/iatson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/iatson/iatson_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/iatson/iatson_og_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46616 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/iatson/iatson_planet_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29748 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/iatson/watson_planet_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.075559 exoml-0.1.7/exoml/ml/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.075559 exoml-0.1.7/exoml/ml/calibration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/calibration/calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/calibration/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.075559 exoml-0.1.7/exoml/ml/callback/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/callback/auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/callback/basemodel_aware_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/callback/batch_aware_csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/callback/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/callback/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/callback/get_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21274 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/callback/learning_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/callback/training_data_aware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.079559 exoml-0.1.7/exoml/ml/encoding/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/encoding/time_position.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.079559 exoml-0.1.7/exoml/ml/functions/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/functions/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.079559 exoml-0.1.7/exoml/ml/layers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/layers/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/layers/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9851 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/layers/transformer_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.079559 exoml-0.1.7/exoml/ml/learning_rate/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/learning_rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/learning_rate/schedulers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.079559 exoml-0.1.7/exoml/ml/log/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/log/get_weights_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/log/with_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.079559 exoml-0.1.7/exoml/ml/loss/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/loss/cross_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/loss/unsupervised.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.083559 exoml-0.1.7/exoml/ml/metrics/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23950 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/metrics/auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/metrics/fixed_mean.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3703 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/ml_data_generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5180 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/ml_single_transits_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.083559 exoml-0.1.7/exoml/ml/model/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42083 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/model/binary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/model/categorical_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/model/imbalanced_binary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/model/imbalanced_categorical_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.083559 exoml-0.1.7/exoml/ml/physics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/physics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/physics/transit_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/ml/thread_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.083559 exoml-0.1.7/exoml/preparation/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/preparation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18135 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/preparation/empty_targets_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34080 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/preparation/ete6parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31695 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/preparation/parser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27267 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/preparation/q1q17dr25parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.087559 exoml-0.1.7/exoml/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:10.000000 exoml-0.1.7/exoml/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.087559 exoml-0.1.7/exoml/resources/q1_q17/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   114514 2024-05-03 18:21:18.000000 exoml-0.1.7/exoml/resources/q1_q17/apjac4399t13_mrt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.087559 exoml-0.1.7/exoml/santo/
+-rw-r--r--   0 runner    (1001) docker     (127)    35156 2024-05-03 18:21:19.000000 exoml-0.1.7/exoml/santo/SANTO.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:19.000000 exoml-0.1.7/exoml/santo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-03 18:21:19.000000 exoml-0.1.7/exoml/santo/santo_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-05-03 18:21:19.000000 exoml-0.1.7/exoml/santo/santo_test_data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.087559 exoml-0.1.7/exoml/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:19.000000 exoml-0.1.7/exoml/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      215 2024-05-03 18:21:19.000000 exoml-0.1.7/exoml/tests/test_exoml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.087559 exoml-0.1.7/exoml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-03 18:21:34.000000 exoml-0.1.7/exoml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-03 18:21:34.000000 exoml-0.1.7/exoml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 18:21:34.000000 exoml-0.1.7/exoml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-03 18:21:34.000000 exoml-0.1.7/exoml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 18:21:34.000000 exoml-0.1.7/exoml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-03 18:21:19.000000 exoml-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-03 18:21:19.000000 exoml-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 18:21:34.087559 exoml-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:34.087559 exoml-0.1.7/transpot/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11057 2024-05-03 18:21:19.000000 exoml-0.1.7/transpot/TRANSPOT.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:21:19.000000 exoml-0.1.7/transpot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-03 18:21:19.000000 exoml-0.1.7/transpot/transpot_generator.py
```

### Comparing `exoml-0.1.6/PKG-INFO` & `exoml-0.1.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: exoml
-Version: 0.1.6
+Version: 0.1.7
 Summary: ExoML tools for exoplanet detections
 Author-email: Martín Dévora-Pajares <mdevorapajares@protonmail.com>
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: keras==2.15.0
 Requires-Dist: tensorflow==2.15.0
 Requires-Dist: ellc==1.8.8
-Requires-Dist: lcbuilder==0.17.0
+Requires-Dist: lcbuilder==0.17.1
 Requires-Dist: ruamel.yaml==0.17.32
 Requires-Dist: pydot==1.4.2
 Requires-Dist: graphviz==0.20.1
 Requires-Dist: pandas==1.5.3
 Requires-Dist: scikit-learn==1.2.2
 Requires-Dist: matplotlib==3.8.2
 Requires-Dist: typeguard==4.1.5
```

### Comparing `exoml-0.1.6/exoml/curve_prioritizer/curve_prioritizer_generator.py` & `exoml-0.1.7/exoml/curve_prioritizer/curve_prioritizer_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/curve_prioritizer/curve_prioritizer_model.py` & `exoml-0.1.7/exoml/curve_prioritizer/curve_prioritizer_model.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/detrend/DETREND.py` & `exoml-0.1.7/exoml/detrend/DETREND.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/detrend/detrend_generator.py` & `exoml-0.1.7/exoml/detrend/detrend_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ete6/ete6_generator.py` & `exoml-0.1.7/exoml/ete6/ete6_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/iatson/IATSON.py` & `exoml-0.1.7/exoml/iatson/IATSON.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/iatson/IATSON_og.py` & `exoml-0.1.7/exoml/iatson/IATSON_og.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/iatson/IATSON_planet.py` & `exoml-0.1.7/exoml/iatson/IATSON_planet.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/iatson/iatson_generator.py` & `exoml-0.1.7/exoml/iatson/iatson_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/iatson/iatson_og_generator.py` & `exoml-0.1.7/exoml/iatson/iatson_og_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/iatson/iatson_planet_generator.py` & `exoml-0.1.7/exoml/iatson/iatson_planet_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/iatson/watson_planet_generator.py` & `exoml-0.1.7/exoml/iatson/watson_planet_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/calibration/calibrator.py` & `exoml-0.1.7/exoml/ml/calibration/calibrator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/calibration/utils.py` & `exoml-0.1.7/exoml/ml/calibration/utils.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/callback/auc.py` & `exoml-0.1.7/exoml/ml/callback/auc.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/callback/basemodel_aware_callback.py` & `exoml-0.1.7/exoml/ml/callback/basemodel_aware_callback.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/callback/batch_aware_csv_logger.py` & `exoml-0.1.7/exoml/ml/callback/batch_aware_csv_logger.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/callback/checkpoint.py` & `exoml-0.1.7/exoml/ml/callback/checkpoint.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/callback/early_stopping.py` & `exoml-0.1.7/exoml/ml/callback/early_stopping.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/callback/learning_rate.py` & `exoml-0.1.7/exoml/ml/callback/learning_rate.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/callback/training_data_aware.py` & `exoml-0.1.7/exoml/ml/callback/training_data_aware.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/layers/dropout.py` & `exoml-0.1.7/exoml/ml/layers/dropout.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/layers/transformer.py` & `exoml-0.1.7/exoml/ml/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/layers/transformer_classifier.py` & `exoml-0.1.7/exoml/ml/layers/transformer_classifier.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/learning_rate/schedulers.py` & `exoml-0.1.7/exoml/ml/learning_rate/schedulers.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/log/get_weights_logger.py` & `exoml-0.1.7/exoml/ml/log/get_weights_logger.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/log/with_logging.py` & `exoml-0.1.7/exoml/ml/log/with_logging.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/loss/cross_entropy.py` & `exoml-0.1.7/exoml/ml/loss/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/loss/unsupervised.py` & `exoml-0.1.7/exoml/ml/loss/unsupervised.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/metrics/auc.py` & `exoml-0.1.7/exoml/ml/metrics/auc.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/ml_data_generator.py` & `exoml-0.1.7/exoml/ml/ml_data_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/ml_single_transits_classifier.py` & `exoml-0.1.7/exoml/ml/ml_single_transits_classifier.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/model/base_model.py` & `exoml-0.1.7/exoml/ml/model/base_model.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/model/binary_model.py` & `exoml-0.1.7/exoml/ml/model/binary_model.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/model/categorical_model.py` & `exoml-0.1.7/exoml/ml/model/categorical_model.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/ml/physics/transit_functions.py` & `exoml-0.1.7/exoml/ml/physics/transit_functions.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/preparation/empty_targets_preparer.py` & `exoml-0.1.7/exoml/preparation/empty_targets_preparer.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/preparation/ete6parser.py` & `exoml-0.1.7/exoml/preparation/ete6parser.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/preparation/parser_utils.py` & `exoml-0.1.7/exoml/preparation/parser_utils.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/preparation/q1q17dr25parser.py` & `exoml-0.1.7/exoml/preparation/q1q17dr25parser.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/resources/q1_q17/apjac4399t13_mrt.txt` & `exoml-0.1.7/exoml/resources/q1_q17/apjac4399t13_mrt.txt`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/santo/SANTO.py` & `exoml-0.1.7/exoml/santo/SANTO.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/santo/santo_generator.py` & `exoml-0.1.7/exoml/santo/santo_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml/santo/santo_test_data_generator.py` & `exoml-0.1.7/exoml/santo/santo_test_data_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/exoml.egg-info/PKG-INFO` & `exoml-0.1.7/exoml.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: exoml
-Version: 0.1.6
+Version: 0.1.7
 Summary: ExoML tools for exoplanet detections
 Author-email: Martín Dévora-Pajares <mdevorapajares@protonmail.com>
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: keras==2.15.0
 Requires-Dist: tensorflow==2.15.0
 Requires-Dist: ellc==1.8.8
-Requires-Dist: lcbuilder==0.17.0
+Requires-Dist: lcbuilder==0.17.1
 Requires-Dist: ruamel.yaml==0.17.32
 Requires-Dist: pydot==1.4.2
 Requires-Dist: graphviz==0.20.1
 Requires-Dist: pandas==1.5.3
 Requires-Dist: scikit-learn==1.2.2
 Requires-Dist: matplotlib==3.8.2
 Requires-Dist: typeguard==4.1.5
```

### Comparing `exoml-0.1.6/exoml.egg-info/SOURCES.txt` & `exoml-0.1.7/exoml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/pyproject.toml` & `exoml-0.1.7/pyproject.toml`

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
-version = "0.1.6"
+version = "0.1.7"
 
 [project.optional-dependencies]
 
 [project.scripts]
 #my-script = "my_package.module:function"
 
 [tool.setuptools]
```

### Comparing `exoml-0.1.6/transpot/TRANSPOT.py` & `exoml-0.1.7/transpot/TRANSPOT.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.6/transpot/transpot_generator.py` & `exoml-0.1.7/transpot/transpot_generator.py`

 * *Files identical despite different names*


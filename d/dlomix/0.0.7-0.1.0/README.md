# Comparing `tmp/dlomix-0.0.7.tar.gz` & `tmp/dlomix-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlomix-0.0.7.tar", last modified: Mon Feb  5 22:20:58 2024, max compression
+gzip compressed data, was "dlomix-0.1.0.tar", last modified: Fri May  3 11:20:27 2024, max compression
```

## Comparing `dlomix-0.0.7.tar` & `dlomix-0.1.0.tar`

### file list

```diff
@@ -1,57 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:20:58.120502 dlomix-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-05 22:20:49.000000 dlomix-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-02-05 22:20:58.120502 dlomix-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-02-05 22:20:49.000000 dlomix-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:20:58.116502 dlomix-0.0.7/dlomix/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:20:58.116502 dlomix-0.0.7/dlomix/data/
--rw-r--r--   0 runner    (1001) docker     (127)    17357 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/data/IntensityDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    19242 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/data/RetentionTimeDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:20:58.116502 dlomix-0.0.7/dlomix/eval/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/eval/rt_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:20:58.116502 dlomix-0.0.7/dlomix/layers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/layers/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:20:58.116502 dlomix-0.0.7/dlomix/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/losses/intensity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:20:58.116502 dlomix-0.0.7/dlomix/models/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/models/deepLC.py
--rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/models/prosit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:20:58.116502 dlomix-0.0.7/dlomix/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/pipelines/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:20:58.120502 dlomix-0.0.7/dlomix/reports/
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/reports/IntensityReport.py
--rw-r--r--   0 runner    (1001) docker     (127)    12619 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/reports/Report.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/reports/RetentionTimeReport.py
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/reports/RetentionTimeReportModelComparisonWandb.py
--rw-r--r--   0 runner    (1001) docker     (127)    16908 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/reports/RetentionTimeReportRunComparisonWandb.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/reports/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-02-05 22:20:49.000000 dlomix-0.0.7/dlomix/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:20:58.120502 dlomix-0.0.7/dlomix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-02-05 22:20:58.000000 dlomix-0.0.7/dlomix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-02-05 22:20:58.000000 dlomix-0.0.7/dlomix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 22:20:58.000000 dlomix-0.0.7/dlomix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-05 22:20:58.000000 dlomix-0.0.7/dlomix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-05 22:20:58.000000 dlomix-0.0.7/dlomix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-05 22:20:49.000000 dlomix-0.0.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:20:58.120502 dlomix-0.0.7/run_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 22:20:49.000000 dlomix-0.0.7/run_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-02-05 22:20:49.000000 dlomix-0.0.7/run_scripts/run_deeplc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-02-05 22:20:49.000000 dlomix-0.0.7/run_scripts/run_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-02-05 22:20:49.000000 dlomix-0.0.7/run_scripts/run_prosit_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-02-05 22:20:49.000000 dlomix-0.0.7/run_scripts/run_prosit_retentiontime.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 22:20:58.120502 dlomix-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-02-05 22:20:49.000000 dlomix-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:20:58.120502 dlomix-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 22:20:49.000000 dlomix-0.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-02-05 22:20:49.000000 dlomix-0.0.7/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-02-05 22:20:49.000000 dlomix-0.0.7/tests/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-05 22:20:49.000000 dlomix-0.0.7/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.639659 dlomix-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-03 11:20:21.000000 dlomix-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-05-03 11:20:27.639659 dlomix-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-05-03 11:20:21.000000 dlomix-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 11:20:21.000000 dlomix-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:20:27.639659 dlomix-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-03 11:20:21.000000 dlomix-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.627658 dlomix-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.631659 dlomix-0.1.0/src/dlomix/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.631659 dlomix-0.1.0/src/dlomix/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25154 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/dataset_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/fragment_ion_intensity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.635659 dlomix-0.1.0/src/dlomix/data/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/processing/feature_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/processing/feature_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.635659 dlomix-0.1.0/src/dlomix/data/processing/pickled_feature_dicts/
+-rw-r--r--   0 runner    (1001) docker     (127)    18779 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/processing/pickled_feature_dicts/mz_diff.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/processing/pickled_feature_dicts/red_smiles.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    24289 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/processing/pickled_feature_dicts/saved_ac_count.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    23161 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/processing/pickled_feature_dicts/saved_gained_atoms.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    23161 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/processing/pickled_feature_dicts/saved_loss_atoms.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/processing/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/retention_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.635659 dlomix-0.1.0/src/dlomix/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/eval/rt_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.635659 dlomix-0.1.0/src/dlomix/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/layers/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.635659 dlomix-0.1.0/src/dlomix/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/losses/intensity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.635659 dlomix-0.1.0/src/dlomix/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/models/deepLC.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13817 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/models/prosit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.635659 dlomix-0.1.0/src/dlomix/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/pipelines/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.639659 dlomix-0.1.0/src/dlomix/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/reports/IntensityReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12619 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/reports/Report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/reports/RetentionTimeReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/reports/RetentionTimeReportModelComparisonWandb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16865 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/reports/RetentionTimeReportRunComparisonWandb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/reports/postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.639659 dlomix-0.1.0/src/dlomix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-05-03 11:20:27.000000 dlomix-0.1.0/src/dlomix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-03 11:20:27.000000 dlomix-0.1.0/src/dlomix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:20:27.000000 dlomix-0.1.0/src/dlomix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-03 11:20:27.000000 dlomix-0.1.0/src/dlomix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 11:20:27.000000 dlomix-0.1.0/src/dlomix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.639659 dlomix-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-03 11:20:21.000000 dlomix-0.1.0/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-03 11:20:21.000000 dlomix-0.1.0/tests/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-03 11:20:21.000000 dlomix-0.1.0/tests/test_models.py
```

### Comparing `dlomix-0.0.7/LICENSE` & `dlomix-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dlomix-0.0.7/PKG-INFO` & `dlomix-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: dlomix
-Version: 0.0.7
+Version: 0.1.0
 Summary: Deep Learning for Proteomics
 Home-page: https://github.com/wilhelm-lab/dlomix
 Author: Omar Shouman
 Author-email: o.shouman@tum.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: datasets
 Requires-Dist: fpdf
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scikit-learn
-Requires-Dist: tensorflow
+Requires-Dist: tensorflow<2.16,>=2.13
+Requires-Dist: tensorflow_probability>=0.21
 Requires-Dist: pyarrow
 Requires-Dist: seaborn
 Provides-Extra: dev
 Requires-Dist: pytest>=3.7; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: twine; extra == "dev"
@@ -60,50 +62,58 @@
 If you would like to use [Weights & Biases](wandb.ai) for experiment tracking and use the available reports for Retention Time under `/notebooks`, please install the optional `wandb` python dependency with `dlomix` by running:
 
 ```bash
 $ pip install dlomix[wandb]
 ```
 
 **General Overview**
--  `data`: structures for modeling the input data, currently based on `tf.Dataset`
+-  `data`: structures for modeling the input data, processing functions, and feature extractions based on Hugging Face datasets `Dataset` and `DatasetDict`
 -  `eval`: classes for evaluating models and reporting results
 -  `layers`: custom layers used for building models, based on `tf.keras.layers.Layer`
 -  `losses`: custom losses to be used for training with `model.fit()`
 - `models`: common model architectures for the relevant use-cases based on `tf.keras.Model` to allow for using the Keras training API
 -  `pipelines`: an exemplary high-level pipeline implementation
 -  `reports`: classes for generating reports related to the different tasks
 -  `constants.py`: constants and configuration values
 -  `utils.py`: utility functions
 
 
 
 **Use-cases**
 
-- Retention Time Prediction: 
-    - a regression problem where the retention time of a peptide sequence is to be predicted. 
+- Retention Time Prediction:
+    - a regression problem where the retention time of a peptide sequence is to be predicted.
+
+- Fragment Ion Intensity Prediction:
+    - a multi-output regression problem where the intensity values for fragment ions are predicted given a peptide sequence along with some additional features.
 
 
 
 **To-Do**
 
 Functionality:
 - [X] integrate prosit
-- [ ] extend pipeline for different types of models and backbones
-- [ ] extend pipeline to allow for fine-tuning with custom datasets
+- [X] integrate hugging face datasets
+- [X] extend data representation to include modifications
+- [X] add PTM features
 - [X] add residual plots to reporting, possibly other regression analysis tools
 - [X] output reporting results as PDF
-- [ ] extend data representation to include modifications
 - [X] refactor reporting module to use W&B Report API (Retention Time)
+- [ ] extend pipeline for different types of models and backbones
+- [ ] extend pipeline to allow for fine-tuning with custom datasets
+
+
 
 Package structure:
 
 - [X] integrate `deeplc.py` into `models.py`, preferably introduce a package structure (e.g. `models.retention_time`)
 - [X] add references for implemented models in the ReadMe
-- [ ] introduce a style guide and checking (e.g. PEP)
+- [X] introduce formatting and precommit hooks
 - [X] plan documentation (sphinx and readthedocs)
+- [X] refactor following best practices for cleaner install
 
 
 ## Developing DLOmix
 To install dlomix, along with the tools needed to develop and run tests, run the following command in your virtualenv:
 ```bash
 $ pip install -e .[dev]
 ```
@@ -118,8 +128,7 @@
 [**DeepLC**]
 
 [2] DeepLC can predict retention times for peptides that carry as-yet unseen modifications
 Robbin Bouwmeester, Ralf Gabriels, Niels Hulstaert, Lennart Martens, Sven Degroeve
 bioRxiv 2020.03.28.013003; doi: 10.1101/2020.03.28.013003
 
 [3] Bouwmeester, R., Gabriels, R., Hulstaert, N. et al. DeepLC can predict retention times for peptides that carry as-yet unseen modifications. Nat Methods 18, 1363–1369 (2021). https://doi.org/10.1038/s41592-021-01301-5
-
```

### Comparing `dlomix-0.0.7/README.md` & `dlomix-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,50 +25,58 @@
 If you would like to use [Weights & Biases](wandb.ai) for experiment tracking and use the available reports for Retention Time under `/notebooks`, please install the optional `wandb` python dependency with `dlomix` by running:
 
 ```bash
 $ pip install dlomix[wandb]
 ```
 
 **General Overview**
--  `data`: structures for modeling the input data, currently based on `tf.Dataset`
+-  `data`: structures for modeling the input data, processing functions, and feature extractions based on Hugging Face datasets `Dataset` and `DatasetDict`
 -  `eval`: classes for evaluating models and reporting results
 -  `layers`: custom layers used for building models, based on `tf.keras.layers.Layer`
 -  `losses`: custom losses to be used for training with `model.fit()`
 - `models`: common model architectures for the relevant use-cases based on `tf.keras.Model` to allow for using the Keras training API
 -  `pipelines`: an exemplary high-level pipeline implementation
 -  `reports`: classes for generating reports related to the different tasks
 -  `constants.py`: constants and configuration values
 -  `utils.py`: utility functions
 
 
 
 **Use-cases**
 
-- Retention Time Prediction: 
-    - a regression problem where the retention time of a peptide sequence is to be predicted. 
+- Retention Time Prediction:
+    - a regression problem where the retention time of a peptide sequence is to be predicted.
+
+- Fragment Ion Intensity Prediction:
+    - a multi-output regression problem where the intensity values for fragment ions are predicted given a peptide sequence along with some additional features.
 
 
 
 **To-Do**
 
 Functionality:
 - [X] integrate prosit
-- [ ] extend pipeline for different types of models and backbones
-- [ ] extend pipeline to allow for fine-tuning with custom datasets
+- [X] integrate hugging face datasets
+- [X] extend data representation to include modifications
+- [X] add PTM features
 - [X] add residual plots to reporting, possibly other regression analysis tools
 - [X] output reporting results as PDF
-- [ ] extend data representation to include modifications
 - [X] refactor reporting module to use W&B Report API (Retention Time)
+- [ ] extend pipeline for different types of models and backbones
+- [ ] extend pipeline to allow for fine-tuning with custom datasets
+
+
 
 Package structure:
 
 - [X] integrate `deeplc.py` into `models.py`, preferably introduce a package structure (e.g. `models.retention_time`)
 - [X] add references for implemented models in the ReadMe
-- [ ] introduce a style guide and checking (e.g. PEP)
+- [X] introduce formatting and precommit hooks
 - [X] plan documentation (sphinx and readthedocs)
+- [X] refactor following best practices for cleaner install
 
 
 ## Developing DLOmix
 To install dlomix, along with the tools needed to develop and run tests, run the following command in your virtualenv:
 ```bash
 $ pip install -e .[dev]
 ```
@@ -83,8 +91,7 @@
 [**DeepLC**]
 
 [2] DeepLC can predict retention times for peptides that carry as-yet unseen modifications
 Robbin Bouwmeester, Ralf Gabriels, Niels Hulstaert, Lennart Martens, Sven Degroeve
 bioRxiv 2020.03.28.013003; doi: 10.1101/2020.03.28.013003
 
 [3] Bouwmeester, R., Gabriels, R., Hulstaert, N. et al. DeepLC can predict retention times for peptides that carry as-yet unseen modifications. Nat Methods 18, 1363–1369 (2021). https://doi.org/10.1038/s41592-021-01301-5
-
```

### Comparing `dlomix-0.0.7/dlomix/eval/rt_eval.py` & `dlomix-0.1.0/src/dlomix/eval/rt_eval.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import tensorflow as tf
 import tensorflow.keras.backend as K
+import tensorflow_probability as tfp
 
 
 class TimeDeltaMetric(tf.keras.metrics.Metric):
-    r"""Implementation of the time delta metric as a Keras Metric.
+    """
+    Implementation of the time delta metric as a Keras Metric.
 
     Parameters
     ----------
     mean : int, optional
         Mean value of the targets in case normalization was performed. Defaults to 0.
     std : int, optional
         Standard deviation value of the targets in case normalization was performed. Defaults to 1.
@@ -41,14 +43,27 @@
         self.std = std
         self.percentage = percentage
         self.rescale_targets = rescale_targets
         self.rescale_predictions = rescale_predictions
         self.double_delta = double_delta
 
     def update_state(self, y_true, y_pred, sample_weight=None):
+        """
+        Update the metric state.
+
+        Parameters
+        ----------
+        y_true : tf.Tensor
+            True values of the target.
+        y_pred : tf.Tensor
+            Predicted values of the target.
+        sample_weight : tf.Tensor, optional
+            Sample weights. Defaults to None.
+        """
+
         # rescale
         if self.rescale_targets:
             y_true = y_true * self.std + self.mean
 
         if self.rescale_predictions:
             y_pred = y_pred * self.std + self.mean
 
@@ -83,7 +98,27 @@
     mark95 = tf.cast(
         tf.cast(tf.shape(y_true)[0], dtype=tf.float32) * 0.95, dtype=tf.int32
     )
     abs_error = K.abs(y_true - y_pred)
     delta = tf.sort(abs_error)[mark95 - 1]
     norm_range = K.max(y_true) - K.min(y_true)
     return (delta * 2) / (norm_range)
+
+
+def TimeDeltaMetric2():
+    """
+    The 95th percentile of absolute error between label and prediction
+
+    """
+
+    def calc_metric(y_true, y_pred, sample_weight=None):
+        # compute residuals and sort
+        abs_error = tf.abs(y_true - y_pred)
+        return tfp.stats.percentile(abs_error, 95)
+
+    calc_metric.__name__ = "delta95"
+    return calc_metric
+
+
+METRICS_DICT = {
+    "delta95": TimeDeltaMetric(),
+}
```

### Comparing `dlomix-0.0.7/dlomix/models/base.py` & `dlomix-0.1.0/src/dlomix/models/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 import tensorflow as tf
-from tensorflow.keras.layers.experimental import preprocessing
 
-from dlomix.constants import ALPHABET_UNMOD
+from ..constants import ALPHABET_UNMOD
 
 
 class RetentionTimePredictor(tf.keras.Model):
-    r"""A simple class for Retention Time prediction models.
+    """
+    A simple class for Retention Time prediction models.
 
     Parameters
     ----------
-        embedding_dim: int, optional
-            Dimensionality of the embeddings to be used for representing the Amino Acids. Defaults to ``16``.
-        seq_length: int, optional
-            Sequence length of the peptide sequences. Defaults to ``30``.
-        encoder: str, optional
-            String for specifying the decoder to use, either based on 1D conv-layers or LSTMs. Defaults to ``conv1d``.
-        vocab_dict: dict, optional
-            Dictionary mapping for the vocabulary (the amino acids in this case). Defaults to ``ALPHABET_UNMOD``.
+
+    embedding_dim: int, optional
+        Dimensionality of the embeddings to be used for representing the Amino Acids. Defaults to ``16``.
+    seq_length: int, optional
+        Sequence length of the peptide sequences. Defaults to ``30``.
+    encoder: str, optional
+        String for specifying the decoder to use, either based on 1D conv-layers or LSTMs. Defaults to ``conv1d``.
+    alphabet: dict, optional
+        Dictionary mapping for the alphabet (the amino acids in this case). Defaults to ``ALPHABET_UNMOD``.
     """
 
     def __init__(
         self,
         embedding_dim=16,
         seq_length=30,
         encoder="conv1d",
-        vocab_dict=ALPHABET_UNMOD,
+        alphabet=ALPHABET_UNMOD,
     ):
         super(RetentionTimePredictor, self).__init__()
 
         # tie the count of embeddings to the size of the vocabulary (count of amino acids)
-        self.embeddings_count = len(vocab_dict) + 2
-
-        self.string_lookup = preprocessing.StringLookup(
-            vocabulary=list(vocab_dict.keys())
-        )
+        self.embeddings_count = len(alphabet) + 2
 
         self.embedding = tf.keras.layers.Embedding(
             input_dim=self.embeddings_count,
             output_dim=embedding_dim,
             input_length=seq_length,
         )
 
@@ -71,15 +68,14 @@
                 [
                     tf.keras.layers.LSTM(256, return_sequences=True),
                     tf.keras.layers.LSTM(256),
                 ]
             )
 
     def call(self, inputs, **kwargs):
-        x = self.string_lookup(inputs)
-        x = self.embedding(x)
+        x = self.embedding(inputs)
         x = self.encoder(x)
         x = self.flatten(x)
         x = self.regressor(x)
         x = self.output_layer(x)
 
         return x
```

### Comparing `dlomix-0.0.7/dlomix/models/deepLC.py` & `dlomix-0.1.0/src/dlomix/models/deepLC.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 import tensorflow as tf
-from tensorflow.keras.layers.experimental import preprocessing
 
-from dlomix.constants import ALPHABET_UNMOD
+from ..constants import ALPHABET_UNMOD
 
 
 class DeepLCRetentionTimePredictor(tf.keras.Model):
     def __init__(
-        self, seq_length=60, vocab_dict=ALPHABET_UNMOD, use_global_features=False
+        self, seq_length=60, alphabet=ALPHABET_UNMOD, use_global_features=False
     ):
         super(DeepLCRetentionTimePredictor, self).__init__()
         self.seq_length = seq_length
         self._use_global_features = use_global_features
 
         self.leaky_relu = tf.keras.layers.ReLU(max_value=20, negative_slope=0.1)
-        self.string_lookup = preprocessing.StringLookup(
-            vocabulary=list(vocab_dict.keys())
-        )
 
         self._build_aminoacid_branch()
         self._build_diaminoacid_branch()
         self._build_onehot_encoding_branch()
         self._build_regressor()
         self.output_layer = tf.keras.layers.Dense(1)
 
@@ -108,16 +104,15 @@
             block.add(tf.keras.layers.MaxPooling1D(pool_size=2, strides=2))
 
         return block
 
     def call(self, inputs, **kwargs):
         outputs = {}
 
-        integer_encoded = self.string_lookup(inputs["seq"])
-        onehot_encoded = tf.one_hot(integer_encoded, depth=self.seq_length)
+        onehot_encoded = tf.one_hot(inputs["seq"], depth=self.seq_length)
 
         if self._use_global_features:
             outputs["global_features_output"] = self.global_features_branch(
                 inputs["global_features"]
             )
 
         outputs["onehot_branch_output"] = self.onehot_encoding_branch(onehot_encoded)
```

### Comparing `dlomix-0.0.7/dlomix/pipelines/pipeline.py` & `dlomix-0.1.0/src/dlomix/pipelines/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import zipfile
 from os import makedirs
 from os.path import dirname, join, splitext
 
 import numpy as np
 import requests
 
-from dlomix.constants import retention_time_pipeline_parameters
-from dlomix.data.RetentionTimeDataset import RetentionTimeDataset
-from dlomix.models.base import RetentionTimePredictor
-from dlomix.reports import RetentionTimeReport
+from ..constants import retention_time_pipeline_parameters
+from ..data import RetentionTimeDataset
+from ..models.base import RetentionTimePredictor
+from ..reports import RetentionTimeReport
 
 # pipelines can be used to train the model further or from scratch given a dataset
 # add string arguments (e.g. prosit to create the model, data source to create the dataset)
 
 # if neither  train nor test are provided --> use toy datasets to (train if necessary or load pre-trained weights), predict on test, and generate report
 # if test only --> load pre-trained weights, predict and generate report
 # if train and test --> do what you have to do
```

### Comparing `dlomix-0.0.7/dlomix/reports/IntensityReport.py` & `dlomix-0.1.0/src/dlomix/reports/IntensityReport.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.0.7/dlomix/reports/Report.py` & `dlomix-0.1.0/src/dlomix/reports/Report.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.0.7/dlomix/reports/RetentionTimeReport.py` & `dlomix-0.1.0/src/dlomix/reports/RetentionTimeReport.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from warnings import warn
 
 import numpy as np
 from matplotlib import pyplot as plt
 from matplotlib.colors import LogNorm
 from matplotlib.ticker import LogLocator
 
-from dlomix.reports.Report import PDFFile, Report
+from ..reports.Report import PDFFile, Report
 
 
 class RetentionTimeReport(Report):
     """Report generation for Retention Time Prediction tasks."""
 
     TARGETS_LABEL = "iRT (measured)"
     PREDICTIONS_LABEL = "iRT (predicted)"
```

### Comparing `dlomix-0.0.7/dlomix/reports/RetentionTimeReportModelComparisonWandb.py` & `dlomix-0.1.0/src/dlomix/reports/RetentionTimeReportModelComparisonWandb.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 
 import numpy as np
 import pandas as pd
 import wandb
 import wandb.apis.reports as wr
 
-from ..data.RetentionTimeDataset import RetentionTimeDataset
+from ..data.retention_time import RetentionTimeDataset
 
 
 class RetentionTimeReportModelComparisonWandb:
     """Creates a WandB report for comparing models.
 
     Parameters
     ----------
```

### Comparing `dlomix-0.0.7/dlomix/reports/RetentionTimeReportRunComparisonWandb.py` & `dlomix-0.1.0/src/dlomix/reports/RetentionTimeReportRunComparisonWandb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
 import re
 
 import numpy as np
 import pandas as pd
 import wandb
 import wandb.apis.reports as wr
-from wandb.keras import WandbCallback, WandbMetricsLogger
 
-from ..data import RetentionTimeDataset
+from ..data.retention_time import RetentionTimeDataset
 
 # ToDo: add R2 plot, TimeDelta plot, residuals
 
 
 class RetentionTimeReportRunComparisonWandb:
     """Create WandB report for comparing runs.
```

### Comparing `dlomix-0.0.7/dlomix/reports/postprocessing.py` & `dlomix-0.1.0/src/dlomix/reports/postprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 
 import numpy as np
 import tensorflow as tf
 
-import dlomix.losses as losses
+from ..losses import masked_spectral_distance
 
 
 def reshape_dims(array):
     n, dims = array.shape
     assert dims == 174
     nlosses = 1
     return array.reshape([array.shape[0], 30 - 1, 2, nlosses, 3])
@@ -55,15 +55,15 @@
             yield i, true[(i) * batch_size :], pred[(i) * batch_size :]
         else:
             yield 0, true, pred
 
     for i, t_b, p_b in iterate():
         tf.compat.v1.reset_default_graph()
         with tf.compat.v1.Session() as s:
-            sa_graph = losses.masked_spectral_distance(t_b, p_b)
+            sa_graph = masked_spectral_distance(t_b, p_b)
             sa_b = 1 - s.run(sa_graph)
             sa[i * batch_size : i * batch_size + sa_b.shape[0]] = sa_b
     sa = np.nan_to_num(sa)
     return sa
 
 
 def normalize_intensity_predictions(data, batch_size=600):
@@ -86,15 +86,15 @@
     intensities = reshape_dims(intensities)
     intensities = mask_outofrange(intensities, sequence_lengths)
     intensities = mask_outofcharge(intensities, charges)
     intensities = reshape_flat(intensities)
     m_idx = intensities == -1
     intensities = normalize_base_peak(intensities)
     intensities[m_idx] = -1
-    data["intensities_pred"] = intensities
+    data["intensities_pred"] = intensities.tolist()
 
     if "intensities_raw" in data:
         data["spectral_angle"] = get_spectral_angle(
             np.stack(data["intensities_raw"].to_numpy()).astype(np.float32),
             intensities,
             batch_size=batch_size,
         )
```

### Comparing `dlomix-0.0.7/dlomix.egg-info/PKG-INFO` & `dlomix-0.1.0/src/dlomix.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: dlomix
-Version: 0.0.7
+Version: 0.1.0
 Summary: Deep Learning for Proteomics
 Home-page: https://github.com/wilhelm-lab/dlomix
 Author: Omar Shouman
 Author-email: o.shouman@tum.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: datasets
 Requires-Dist: fpdf
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scikit-learn
-Requires-Dist: tensorflow
+Requires-Dist: tensorflow<2.16,>=2.13
+Requires-Dist: tensorflow_probability>=0.21
 Requires-Dist: pyarrow
 Requires-Dist: seaborn
 Provides-Extra: dev
 Requires-Dist: pytest>=3.7; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: twine; extra == "dev"
@@ -60,50 +62,58 @@
 If you would like to use [Weights & Biases](wandb.ai) for experiment tracking and use the available reports for Retention Time under `/notebooks`, please install the optional `wandb` python dependency with `dlomix` by running:
 
 ```bash
 $ pip install dlomix[wandb]
 ```
 
 **General Overview**
--  `data`: structures for modeling the input data, currently based on `tf.Dataset`
+-  `data`: structures for modeling the input data, processing functions, and feature extractions based on Hugging Face datasets `Dataset` and `DatasetDict`
 -  `eval`: classes for evaluating models and reporting results
 -  `layers`: custom layers used for building models, based on `tf.keras.layers.Layer`
 -  `losses`: custom losses to be used for training with `model.fit()`
 - `models`: common model architectures for the relevant use-cases based on `tf.keras.Model` to allow for using the Keras training API
 -  `pipelines`: an exemplary high-level pipeline implementation
 -  `reports`: classes for generating reports related to the different tasks
 -  `constants.py`: constants and configuration values
 -  `utils.py`: utility functions
 
 
 
 **Use-cases**
 
-- Retention Time Prediction: 
-    - a regression problem where the retention time of a peptide sequence is to be predicted. 
+- Retention Time Prediction:
+    - a regression problem where the retention time of a peptide sequence is to be predicted.
+
+- Fragment Ion Intensity Prediction:
+    - a multi-output regression problem where the intensity values for fragment ions are predicted given a peptide sequence along with some additional features.
 
 
 
 **To-Do**
 
 Functionality:
 - [X] integrate prosit
-- [ ] extend pipeline for different types of models and backbones
-- [ ] extend pipeline to allow for fine-tuning with custom datasets
+- [X] integrate hugging face datasets
+- [X] extend data representation to include modifications
+- [X] add PTM features
 - [X] add residual plots to reporting, possibly other regression analysis tools
 - [X] output reporting results as PDF
-- [ ] extend data representation to include modifications
 - [X] refactor reporting module to use W&B Report API (Retention Time)
+- [ ] extend pipeline for different types of models and backbones
+- [ ] extend pipeline to allow for fine-tuning with custom datasets
+
+
 
 Package structure:
 
 - [X] integrate `deeplc.py` into `models.py`, preferably introduce a package structure (e.g. `models.retention_time`)
 - [X] add references for implemented models in the ReadMe
-- [ ] introduce a style guide and checking (e.g. PEP)
+- [X] introduce formatting and precommit hooks
 - [X] plan documentation (sphinx and readthedocs)
+- [X] refactor following best practices for cleaner install
 
 
 ## Developing DLOmix
 To install dlomix, along with the tools needed to develop and run tests, run the following command in your virtualenv:
 ```bash
 $ pip install -e .[dev]
 ```
@@ -118,8 +128,7 @@
 [**DeepLC**]
 
 [2] DeepLC can predict retention times for peptides that carry as-yet unseen modifications
 Robbin Bouwmeester, Ralf Gabriels, Niels Hulstaert, Lennart Martens, Sven Degroeve
 bioRxiv 2020.03.28.013003; doi: 10.1101/2020.03.28.013003
 
 [3] Bouwmeester, R., Gabriels, R., Hulstaert, N. et al. DeepLC can predict retention times for peptides that carry as-yet unseen modifications. Nat Methods 18, 1363–1369 (2021). https://doi.org/10.1038/s41592-021-01301-5
-
```

### Comparing `dlomix-0.0.7/tests/test_losses.py` & `dlomix-0.1.0/tests/test_losses.py`

 * *Files identical despite different names*


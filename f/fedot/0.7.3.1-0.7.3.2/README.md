# Comparing `tmp/fedot-0.7.3.1.tar.gz` & `tmp/fedot-0.7.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedot-0.7.3.1.tar", last modified: Tue Mar  5 21:31:36 2024, max compression
+gzip compressed data, was "fedot-0.7.3.2.tar", last modified: Fri May  3 15:56:30 2024, max compression
```

## Comparing `fedot-0.7.3.1.tar` & `fedot-0.7.3.2.tar`

### file list

```diff
@@ -1,356 +1,358 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.380171 fedot-0.7.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-05 21:31:29.000000 fedot-0.7.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-05 21:31:29.000000 fedot-0.7.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19506 2024-03-05 21:31:36.380171 fedot-0.7.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21589 2024-03-05 21:31:29.000000 fedot-0.7.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.328171 fedot-0.7.3.1/cases/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:29.000000 fedot-0.7.3.1/cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-05 21:31:29.000000 fedot-0.7.3.1/cases/dataset_preparation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-03-05 21:31:29.000000 fedot-0.7.3.1/cases/kc2_sourcecode_defects_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-03-05 21:31:29.000000 fedot-0.7.3.1/cases/metocean_forecasting_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-03-05 21:31:29.000000 fedot-0.7.3.1/cases/multi_target_levels_forecasting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-03-05 21:31:29.000000 fedot-0.7.3.1/cases/multi_ts_level_forecasting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-03-05 21:31:29.000000 fedot-0.7.3.1/cases/multivariate_ts_forecasting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-03-05 21:31:29.000000 fedot-0.7.3.1/cases/spam_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-03-05 21:31:29.000000 fedot-0.7.3.1/cases/time_series_gapfilling_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.328171 fedot-0.7.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.328171 fedot-0.7.3.1/examples/advanced/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/additional_learning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.332171 fedot-0.7.3.1/examples/advanced/automl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/automl/h2o_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/automl/pipeline_from_automl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/automl/tpot_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/automl/tpot_vs_fedot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.332171 fedot-0.7.3.1/examples/advanced/decompose/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/decompose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/decompose/classification_refinement_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/decompose/refinement_forecast_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/decompose/regression_refinement_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.332171 fedot-0.7.3.1/examples/advanced/fedot_based_solutions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/fedot_based_solutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/fedot_based_solutions/external_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/gpu_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/multi_modal_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/multimodal_text_num_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/multiobj_optimisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/multitask_classification_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/parallelization_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/pipeline_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/profiler_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.332171 fedot-0.7.3.1/examples/advanced/remote_execution/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/remote_execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/remote_execution/remote_fit_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/remote_execution/ts_composer_with_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.332171 fedot-0.7.3.1/examples/advanced/structural_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/structural_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/structural_analysis/complex_analysis_with_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/structural_analysis/dataset_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/structural_analysis/pipelines_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/structural_analysis/structural_analysis_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/surrogate_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.336171 fedot-0.7.3.1/examples/advanced/time_series_forecasting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/time_series_forecasting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/time_series_forecasting/composing_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/time_series_forecasting/custom_model_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/time_series_forecasting/exogenous.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/time_series_forecasting/multi_ts_arctic_forecasting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/time_series_forecasting/multistep.py
--rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/time_series_forecasting/nemo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12366 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/time_series_forecasting/nemo_multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/time_series_forecasting/prediction_intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/advanced/time_series_forecasting/sparse_lagged_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/project_import_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.336171 fedot-0.7.3.1/examples/simple/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.336171 fedot-0.7.3.1/examples/simple/api_builder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/api_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/api_builder/classification_with_api_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/api_builder/multiple_ts_forecasting_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.336171 fedot-0.7.3.1/examples/simple/classification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/classification/api_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/classification/classification_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/classification/classification_with_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/classification/image_classification_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/classification/multiclass_prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/classification/resample_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.336171 fedot-0.7.3.1/examples/simple/cli_application/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/cli_application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/cli_application/cli_call_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.340171 fedot-0.7.3.1/examples/simple/interpretable/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/interpretable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/interpretable/api_explain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/interpretable/pipeline_explain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/pipeline_and_history_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/pipeline_import_export.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/pipeline_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/pipeline_tune.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/pipeline_tuning_with_iopt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/pipeline_visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.340171 fedot-0.7.3.1/examples/simple/regression/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/regression/api_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/regression/regression_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/regression/regression_with_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.340171 fedot-0.7.3.1/examples/simple/time_series_forecasting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/time_series_forecasting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/time_series_forecasting/api_forecasting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/time_series_forecasting/cgru.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/time_series_forecasting/fitted_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/time_series_forecasting/gapfilling.py
--rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/time_series_forecasting/ts_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-03-05 21:31:30.000000 fedot-0.7.3.1/examples/simple/time_series_forecasting/tuning_pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.340171 fedot-0.7.3.1/fedot/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.344171 fedot-0.7.3.1/fedot/api/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.344171 fedot-0.7.3.1/fedot/api/api_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/api_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/api_utils/api_composer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/api_utils/api_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/api_utils/api_params_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.344171 fedot-0.7.3.1/fedot/api/api_utils/assumptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/api_utils/assumptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8471 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/api_utils/assumptions/assumptions_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/api_utils/assumptions/assumptions_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/api_utils/assumptions/operations_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/api_utils/assumptions/preprocessing_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/api_utils/assumptions/task_assumptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/api_utils/data_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/api_utils/input_analyser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/api_utils/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/api_utils/predefined_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/api_utils/presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    19674 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/fedot_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/help.py
--rw-r--r--   0 runner    (1001) docker     (127)    27873 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/api/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.344171 fedot-0.7.3.1/fedot/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.348171 fedot-0.7.3.1/fedot/core/caching/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/caching/base_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/caching/base_cache_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/caching/pipelines_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/caching/pipelines_cache_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/caching/preprocessing_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/caching/preprocessing_cache_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.348171 fedot-0.7.3.1/fedot/core/composer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/composer/composer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/composer/composer_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.348171 fedot-0.7.3.1/fedot/core/composer/gp_composer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/composer/gp_composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/composer/gp_composer/gp_composer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/composer/gp_composer/specific_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/composer/meta_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/composer/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/composer/random_composer.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.352171 fedot-0.7.3.1/fedot/core/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/data/array_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/data/cv_folds.py
--rw-r--r--   0 runner    (1001) docker     (127)    35344 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/data/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/data/data_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/data/data_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/data/data_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/data/load_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.352171 fedot-0.7.3.1/fedot/core/data/merge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/data/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8425 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/data/merge/data_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/data/merge/supplementary_data_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10229 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/data/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/data/supplementary_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/data/visualisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.352171 fedot-0.7.3.1/fedot/core/operations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/atomized_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/atomized_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/automl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/data_operation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.356171 fedot-0.7.3.1/fedot/core/operations/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/automl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/boostings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/common_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/evaluation_interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.356171 fedot-0.7.3.1/fedot/core/operations/evaluation/gpu/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/gpu/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/gpu/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/gpu/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/gpu/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.356171 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.356171 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/categorical_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/decompose.py
--rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_imbalanced_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    16322 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/text_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/text_pretrained.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.360171 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/topological/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/topological/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/topological/fast_topological_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    35704 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/ts_transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/implementation_interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.360171 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/boostings_implementations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/custom_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/discriminant_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/knn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/svc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.360171 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/arima.py
--rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/cgru.py
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/naive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/poly.py
--rw-r--r--   0 runner    (1001) docker     (127)    13173 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/statsmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/evaluation/time_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/hyperparameters_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/operation_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/operations/operation_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.360171 fedot-0.7.3.1/fedot/core/optimisers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/optimisers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.360171 fedot-0.7.3.1/fedot/core/optimisers/objective/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/optimisers/objective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/optimisers/objective/data_objective_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     7778 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/optimisers/objective/data_source_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/optimisers/objective/metrics_objective.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/optimisers/objective/objective_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.364171 fedot-0.7.3.1/fedot/core/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/automl_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14726 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/node.py
--rw-r--r--   0 runner    (1001) docker     (127)    18841 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/pipeline_advisor.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/pipeline_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/pipeline_composer_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/pipeline_graph_generation_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/pipeline_node_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.364171 fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/graph_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/pipeline_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.368171 fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/solvers/best_pipelines_quantiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/solvers/last_generation_quantile_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/solvers/mutation_of_best_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/ts_mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/tuners.py
--rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/random_pipeline_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    18702 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    13862 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/ts_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.368171 fedot-0.7.3.1/fedot/core/pipelines/tuning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/tuning/hyperparams.py
--rw-r--r--   0 runner    (1001) docker     (127)    32286 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/tuning/search_space.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/tuning/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/tuning/tuner_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/verification.py
--rw-r--r--   0 runner    (1001) docker     (127)    16621 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/pipelines/verification_rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.368171 fedot-0.7.3.1/fedot/core/repository/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/repository/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.368171 fedot-0.7.3.1/fedot/core/repository/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/repository/data/automl_repository.json
--rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/repository/data/data_operation_repository.json
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/repository/data/default_operation_params.json
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/repository/data/gpu_models_repository.json
--rw-r--r--   0 runner    (1001) docker     (127)    11668 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/repository/data/model_repository.json
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/repository/dataset_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/repository/default_params_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/repository/graph_operation_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/repository/json_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/repository/metrics_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    20933 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/repository/operation_types_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/repository/pipeline_operation_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/repository/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.372171 fedot-0.7.3.1/fedot/core/visualisation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/core/visualisation/pipeline_specific_visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.372171 fedot-0.7.3.1/fedot/explainability/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/explainability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/explainability/explainer_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/explainability/explainers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/explainability/surrogate_explainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.372171 fedot-0.7.3.1/fedot/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/preprocessing/base_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/preprocessing/categorical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/preprocessing/data_type_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    24353 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/preprocessing/data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/preprocessing/dummy_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    22784 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/preprocessing/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/preprocessing/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.372171 fedot-0.7.3.1/fedot/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.372171 fedot-0.7.3.1/fedot/remote/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/remote/infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.372171 fedot-0.7.3.1/fedot/remote/infrastructure/clients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/remote/infrastructure/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/remote/infrastructure/clients/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/remote/infrastructure/clients/datamall_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/remote/infrastructure/clients/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/remote/pipeline_run_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/remote/remote_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/remote/run_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.372171 fedot-0.7.3.1/fedot/structural_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/structural_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.376171 fedot-0.7.3.1/fedot/structural_analysis/operations_hp_sensitivity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/structural_analysis/operations_hp_sensitivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/structural_analysis/operations_hp_sensitivity/multi_operations_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/structural_analysis/operations_hp_sensitivity/one_operation_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/structural_analysis/operations_hp_sensitivity/problem.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/structural_analysis/operations_hp_sensitivity/sa_and_sample_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/structural_analysis/sa_requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.376171 fedot-0.7.3.1/fedot/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/utilities/composer_timer.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/utilities/custom_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/utilities/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/utilities/define_metric_by_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/utilities/golem_imports_transition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/utilities/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/utilities/pattern_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/utilities/project_import_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/utilities/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/utilities/synth_dataset_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    19719 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/utilities/ts_gapfilling.py
--rw-r--r--   0 runner    (1001) docker     (127)    10688 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/utilities/window_size_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-05 21:31:30.000000 fedot-0.7.3.1/fedot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:31:36.376171 fedot-0.7.3.1/fedot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19506 2024-03-05 21:31:36.000000 fedot-0.7.3.1/fedot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-03-05 21:31:36.000000 fedot-0.7.3.1/fedot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 21:31:36.000000 fedot-0.7.3.1/fedot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-05 21:31:36.000000 fedot-0.7.3.1/fedot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-05 21:31:36.000000 fedot-0.7.3.1/fedot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 21:31:36.380171 fedot-0.7.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-03-05 21:31:30.000000 fedot-0.7.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.552146 fedot-0.7.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-03 15:56:26.000000 fedot-0.7.3.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 15:56:26.000000 fedot-0.7.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19799 2024-05-03 15:56:30.552146 fedot-0.7.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21856 2024-05-03 15:56:26.000000 fedot-0.7.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.500145 fedot-0.7.3.2/cases/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-03 15:56:26.000000 fedot-0.7.3.2/cases/dataset_preparation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-03 15:56:26.000000 fedot-0.7.3.2/cases/kc2_sourcecode_defects_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-03 15:56:26.000000 fedot-0.7.3.2/cases/metocean_forecasting_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-03 15:56:26.000000 fedot-0.7.3.2/cases/multi_target_levels_forecasting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-03 15:56:26.000000 fedot-0.7.3.2/cases/multi_ts_level_forecasting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-03 15:56:26.000000 fedot-0.7.3.2/cases/multivariate_ts_forecasting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-03 15:56:26.000000 fedot-0.7.3.2/cases/spam_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-03 15:56:26.000000 fedot-0.7.3.2/cases/time_series_gapfilling_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.500145 fedot-0.7.3.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.500145 fedot-0.7.3.2/examples/advanced/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/additional_learning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.500145 fedot-0.7.3.2/examples/advanced/automl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/automl/h2o_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/automl/pipeline_from_automl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/automl/tpot_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/automl/tpot_vs_fedot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.504145 fedot-0.7.3.2/examples/advanced/decompose/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/decompose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/decompose/classification_refinement_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/decompose/refinement_forecast_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/decompose/regression_refinement_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.504145 fedot-0.7.3.2/examples/advanced/fedot_based_solutions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/fedot_based_solutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/fedot_based_solutions/external_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/gpu_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/multi_modal_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/multimodal_text_num_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/multiobj_optimisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/multitask_classification_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/parallelization_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/pipeline_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/profiler_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.504145 fedot-0.7.3.2/examples/advanced/remote_execution/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/remote_execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/remote_execution/remote_fit_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/remote_execution/ts_composer_with_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.504145 fedot-0.7.3.2/examples/advanced/structural_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/structural_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/structural_analysis/complex_analysis_with_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/structural_analysis/dataset_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/structural_analysis/pipelines_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/structural_analysis/structural_analysis_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/surrogate_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.504145 fedot-0.7.3.2/examples/advanced/time_series_forecasting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/time_series_forecasting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/time_series_forecasting/composing_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/time_series_forecasting/custom_model_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/time_series_forecasting/exogenous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/time_series_forecasting/multi_ts_arctic_forecasting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/time_series_forecasting/multistep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/time_series_forecasting/nemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12366 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/time_series_forecasting/nemo_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/time_series_forecasting/prediction_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/advanced/time_series_forecasting/sparse_lagged_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/project_import_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.508145 fedot-0.7.3.2/examples/simple/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.508145 fedot-0.7.3.2/examples/simple/api_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/api_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/api_builder/classification_with_api_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/api_builder/multiple_ts_forecasting_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.508145 fedot-0.7.3.2/examples/simple/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/classification/api_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/classification/classification_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/classification/classification_with_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/classification/image_classification_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/classification/multiclass_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/classification/resample_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.508145 fedot-0.7.3.2/examples/simple/cli_application/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/cli_application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/cli_application/cli_call_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.508145 fedot-0.7.3.2/examples/simple/interpretable/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/interpretable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/interpretable/api_explain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/interpretable/pipeline_explain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/pipeline_and_history_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/pipeline_import_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/pipeline_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/pipeline_tune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/pipeline_tuning_with_iopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/pipeline_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.512145 fedot-0.7.3.2/examples/simple/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/regression/api_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/regression/regression_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/regression/regression_with_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.512145 fedot-0.7.3.2/examples/simple/time_series_forecasting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/time_series_forecasting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/time_series_forecasting/api_forecasting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/time_series_forecasting/cgru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/time_series_forecasting/fitted_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/time_series_forecasting/gapfilling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/time_series_forecasting/ts_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-03 15:56:26.000000 fedot-0.7.3.2/examples/simple/time_series_forecasting/tuning_pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.512145 fedot-0.7.3.2/fedot/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.512145 fedot-0.7.3.2/fedot/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.516145 fedot-0.7.3.2/fedot/api/api_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/api_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/api_utils/api_composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/api_utils/api_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/api_utils/api_params_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.516145 fedot-0.7.3.2/fedot/api/api_utils/assumptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/api_utils/assumptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8471 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/api_utils/assumptions/assumptions_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/api_utils/assumptions/assumptions_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/api_utils/assumptions/operations_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/api_utils/assumptions/preprocessing_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/api_utils/assumptions/task_assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/api_utils/data_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/api_utils/input_analyser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/api_utils/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/api_utils/predefined_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/api_utils/presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19674 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/fedot_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27873 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/api/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.516145 fedot-0.7.3.2/fedot/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.516145 fedot-0.7.3.2/fedot/core/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/caching/base_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/caching/base_cache_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/caching/pipelines_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/caching/pipelines_cache_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/caching/preprocessing_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/caching/preprocessing_cache_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.520145 fedot-0.7.3.2/fedot/core/composer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/composer/composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/composer/composer_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.520145 fedot-0.7.3.2/fedot/core/composer/gp_composer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/composer/gp_composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/composer/gp_composer/gp_composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/composer/gp_composer/specific_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/composer/meta_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/composer/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/composer/random_composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.520145 fedot-0.7.3.2/fedot/core/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/data/array_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/data/cv_folds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35348 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/data/data_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/data/data_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/data/data_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/data/load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.520145 fedot-0.7.3.2/fedot/core/data/merge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/data/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8425 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/data/merge/data_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/data/merge/supplementary_data_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10229 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/data/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/data/supplementary_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/data/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.524145 fedot-0.7.3.2/fedot/core/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/atomized_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/atomized_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/automl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/data_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.524145 fedot-0.7.3.2/fedot/core/operations/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/automl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/boostings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/common_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/evaluation_interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.528145 fedot-0.7.3.2/fedot/core/operations/evaluation/gpu/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/gpu/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/gpu/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/gpu/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/gpu/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.528145 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.528145 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/categorical_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/decompose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_imbalanced_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16740 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/text_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/text_pretrained.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.528145 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/topological/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/topological/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/topological/fast_topological_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35704 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/ts_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/implementation_interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.528145 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/boostings_implementations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/discriminant_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/knn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/svc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.532145 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/arima.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/cgru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/poly.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14181 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/statsmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/evaluation/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/hyperparameters_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/operation_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/operations/operation_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.532145 fedot-0.7.3.2/fedot/core/optimisers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/optimisers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.532145 fedot-0.7.3.2/fedot/core/optimisers/objective/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/optimisers/objective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/optimisers/objective/data_objective_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7778 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/optimisers/objective/data_source_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/optimisers/objective/metrics_objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/optimisers/objective/objective_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.536145 fedot-0.7.3.2/fedot/core/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/automl_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14726 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18841 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/pipeline_advisor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/pipeline_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/pipeline_composer_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/pipeline_graph_generation_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/pipeline_node_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.536145 fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/graph_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/pipeline_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.536145 fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/solvers/best_pipelines_quantiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/solvers/last_generation_quantile_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/solvers/mutation_of_best_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/ts_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/tuners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/random_pipeline_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18702 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13862 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/ts_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.540145 fedot-0.7.3.2/fedot/core/pipelines/tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/tuning/hyperparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32286 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/tuning/search_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/tuning/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/tuning/tuner_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16621 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/pipelines/verification_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.540145 fedot-0.7.3.2/fedot/core/repository/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/repository/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.540145 fedot-0.7.3.2/fedot/core/repository/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/repository/data/automl_repository.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/repository/data/data_operation_repository.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/repository/data/default_operation_params.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/repository/data/gpu_models_repository.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11668 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/repository/data/model_repository.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/repository/dataset_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/repository/default_params_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/repository/graph_operation_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/repository/json_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/repository/metrics_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20933 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/repository/operation_types_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/repository/pipeline_operation_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/repository/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.540145 fedot-0.7.3.2/fedot/core/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/core/visualisation/pipeline_specific_visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.540145 fedot-0.7.3.2/fedot/explainability/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/explainability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/explainability/explainer_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/explainability/explainers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/explainability/surrogate_explainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.544145 fedot-0.7.3.2/fedot/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/preprocessing/base_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/preprocessing/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/preprocessing/data_type_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24353 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/preprocessing/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/preprocessing/dummy_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22782 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/preprocessing/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/preprocessing/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.544145 fedot-0.7.3.2/fedot/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/remote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.544145 fedot-0.7.3.2/fedot/remote/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/remote/infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.544145 fedot-0.7.3.2/fedot/remote/infrastructure/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/remote/infrastructure/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/remote/infrastructure/clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/remote/infrastructure/clients/datamall_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/remote/infrastructure/clients/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/remote/pipeline_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/remote/remote_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/remote/run_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.544145 fedot-0.7.3.2/fedot/structural_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/structural_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.544145 fedot-0.7.3.2/fedot/structural_analysis/operations_hp_sensitivity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/structural_analysis/operations_hp_sensitivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/structural_analysis/operations_hp_sensitivity/multi_operations_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/structural_analysis/operations_hp_sensitivity/one_operation_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/structural_analysis/operations_hp_sensitivity/problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/structural_analysis/operations_hp_sensitivity/sa_and_sample_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/structural_analysis/sa_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.548145 fedot-0.7.3.2/fedot/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/utilities/composer_timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/utilities/custom_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/utilities/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/utilities/define_metric_by_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/utilities/golem_imports_transition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/utilities/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/utilities/pattern_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/utilities/project_import_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/utilities/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/utilities/synth_dataset_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19719 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/utilities/ts_gapfilling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10688 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/utilities/window_size_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 15:56:26.000000 fedot-0.7.3.2/fedot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.548145 fedot-0.7.3.2/fedot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19799 2024-05-03 15:56:30.000000 fedot-0.7.3.2/fedot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14434 2024-05-03 15:56:30.000000 fedot-0.7.3.2/fedot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:56:30.000000 fedot-0.7.3.2/fedot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-03 15:56:30.000000 fedot-0.7.3.2/fedot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 15:56:30.000000 fedot-0.7.3.2/fedot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:56:30.552146 fedot-0.7.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-03 15:56:26.000000 fedot-0.7.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:56:30.548145 fedot-0.7.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-03 15:56:26.000000 fedot-0.7.3.2/test/test_gpu_strategy.py
```

### Comparing `fedot-0.7.3.1/LICENSE.md` & `fedot-0.7.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/PKG-INFO` & `fedot-0.7.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: fedot
-Version: 0.7.3.1
+Version: 0.7.3.2
 Summary: Automated machine learning framework for composite pipelines
 Home-page: https://github.com/aimclub/FEDOT
 Author: NSS Lab
 Author-email: itmo.nss.team@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
+Requires-Dist: scipy<1.13.0
 Requires-Dist: thegolem==0.4.0
 Requires-Dist: numpy!=1.24.0,>=1.16.0
 Requires-Dist: pandas>=1.3.0; python_version >= "3.8"
 Requires-Dist: anytree>=2.8.0
 Requires-Dist: catboost>=0.25.0
 Requires-Dist: lightgbm>=3.0.0
 Requires-Dist: xgboost>=1.4.0
 Requires-Dist: statsmodels>=0.12.0
 Requires-Dist: ete3>=3.1.0
 Requires-Dist: networkx!=2.7.*,!=2.8.1,!=2.8.2,!=2.8.3,>=2.4
 Requires-Dist: scikit_learn>=1.0.0; python_version >= "3.8"
-Requires-Dist: sktime==0.16.1
+Requires-Dist: sktime==0.16.1; python_version <= "3.10"
+Requires-Dist: sktime>=0.16.1; python_version > "3.10"
 Requires-Dist: hyperopt==0.2.7
 Requires-Dist: SALib>=1.3.0
 Requires-Dist: scikit-optimize>=0.7.4
 Requires-Dist: matplotlib>=3.3.1; python_version >= "3.8"
 Requires-Dist: pyvis==0.2.1
 Requires-Dist: seaborn>=0.9.0
 Requires-Dist: func_timeout==4.3.5
@@ -49,15 +51,15 @@
 Requires-Dist: h2o==3.42.0.1; extra == "examples"
 Requires-Dist: openpyxl==3.0.7; extra == "examples"
 Provides-Extra: extra
 Requires-Dist: tensorflow>=2.8.0; python_version >= "3.8" and extra == "extra"
 Requires-Dist: torch>=1.9.0; extra == "extra"
 Requires-Dist: opencv-python>=4.5.5.64; extra == "extra"
 Requires-Dist: Pillow>=8.2.0; extra == "extra"
-Requires-Dist: gensim>=4.1.2; extra == "extra"
+Requires-Dist: gensim==4.3.2; extra == "extra"
 Requires-Dist: nltk>=3.5; extra == "extra"
 Requires-Dist: protobuf~=3.19.0; extra == "extra"
 Requires-Dist: giotto_tda==0.6.0; extra == "extra"
 Requires-Dist: ripser==0.6.4; extra == "extra"
 Provides-Extra: profilers
 Requires-Dist: snakeviz==2.1.0; extra == "profilers"
 Requires-Dist: gprof2dot==2021.2.21; extra == "profilers"
@@ -125,26 +127,32 @@
 - **Versatility.** FEDOT is `not limited to specific modeling tasks <https://fedot.readthedocs.io/en/master/advanced/architecture.html>`_, for example, it can be used in ODE or PDE;
 - **Reproducibility.** Resulting pipelines can be `exported separately as JSON <https://fedot.readthedocs.io/en/master/advanced/pipeline_import_export.html>`_ or `together with your input data as ZIP archive <https://fedot.readthedocs.io/en/master/advanced/project_import_export.html>`_ for experiments reproducibility;
 - **Customizability.** FEDOT allows `managing models complexity <https://fedot.readthedocs.io/en/master/introduction/fedot_features/automation_features.html#models-used>`_ and thereby achieving desired quality.
 
 Installation
 ============
 
+- Package installer for Python **pip**
+
 The simplest way to install FEDOT is using ``pip``:
 
 .. code-block::
 
   $ pip install fedot
 
 Installation with optional dependencies for image and text processing, and for DNNs:
 
 .. code-block::
 
   $ pip install fedot[extra]
 
+- **Docker** container
+
+Available docker images can be found here `here <https://github.com/aimclub/FEDOT/tree/master/docker/README_en.rst>`_.
+
 How to Use
 ==========
 
 FEDOT provides a high-level API that allows you to use its capabilities in a simple way. The API can be used for classification, regression, and time series forecasting problems.
 
 To use the API, follow these steps:
```

### Comparing `fedot-0.7.3.1/README.rst` & `fedot-0.7.3.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -59,26 +59,32 @@
 - **Универсальность.** FEDOT `не ограничивается конкретными задачами моделирования <https://fedot.readthedocs.io/en/master/advanced/architecture.html>`_, например, его можно использовать в ODE или PDE;
 - **Воспроизводимость.** Получаемые паплайны можно `экспортировать в формате JSON отдельно <https://fedot.readthedocs.io/en/master/advanced/pipeline_import_export.html>`_ или `вместе с входными данными в формате архива ZIP <https://fedot.readthedocs.io/en/master/advanced/project_import_export.html>`_, для воспроизведения экспериментов;
 - **Кастомизируемость.** FEDOT позволяет `настраивать сложность моделей <https://fedot.readthedocs.io/en/master/introduction/fedot_features/automation_features.html#models-used>`_, тем самым, получать необходимое качество.
 
 Установка
 =========
 
+- Cистема управления пакетами **pip**
+
 Самый простой способ установить FEDOT - это использовать ``pip``:
 
 .. code-block::
 
   $ pip install fedot
 
 Установка с дополнительными зависимостями для обработки изображений и текста, а также для DNN:
 
 .. code-block::
 
   $ pip install fedot[extra]
 
+- Контенер **Docker**
+
+Информацию по доступным образам можно посмотреть `здесь <https://github.com/aimclub/FEDOT/tree/master/docker/README.rst>`_.
+
 Как использовать
 ================
 
 FEDOT предоставляет высокоуровневый API, который удобно использовать. API может использоваться для задач классификации, регрессии и прогнозирования временных рядов.
 Чтобы использовать API, выполните следующие действия:
 
 1. Импортируйте класс ``Fedot``
```

### Comparing `fedot-0.7.3.1/cases/dataset_preparation.py` & `fedot-0.7.3.2/cases/dataset_preparation.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/cases/kc2_sourcecode_defects_classification.py` & `fedot-0.7.3.2/cases/kc2_sourcecode_defects_classification.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/cases/metocean_forecasting_problem.py` & `fedot-0.7.3.2/cases/metocean_forecasting_problem.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/cases/multi_target_levels_forecasting.py` & `fedot-0.7.3.2/cases/multi_target_levels_forecasting.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/cases/multi_ts_level_forecasting.py` & `fedot-0.7.3.2/cases/multi_ts_level_forecasting.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/cases/multivariate_ts_forecasting.py` & `fedot-0.7.3.2/cases/multivariate_ts_forecasting.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/cases/spam_detection.py` & `fedot-0.7.3.2/cases/spam_detection.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/cases/time_series_gapfilling_case.py` & `fedot-0.7.3.2/cases/time_series_gapfilling_case.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/additional_learning.py` & `fedot-0.7.3.2/examples/advanced/additional_learning.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/automl/h2o_example.py` & `fedot-0.7.3.2/examples/advanced/automl/h2o_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/automl/pipeline_from_automl.py` & `fedot-0.7.3.2/examples/advanced/automl/pipeline_from_automl.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/automl/tpot_example.py` & `fedot-0.7.3.2/examples/advanced/automl/tpot_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/automl/tpot_vs_fedot.py` & `fedot-0.7.3.2/examples/advanced/automl/tpot_vs_fedot.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/decompose/classification_refinement_example.py` & `fedot-0.7.3.2/examples/advanced/decompose/classification_refinement_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/decompose/refinement_forecast_example.py` & `fedot-0.7.3.2/examples/advanced/decompose/refinement_forecast_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/decompose/regression_refinement_example.py` & `fedot-0.7.3.2/examples/advanced/decompose/regression_refinement_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/fedot_based_solutions/external_optimizer.py` & `fedot-0.7.3.2/examples/advanced/fedot_based_solutions/external_optimizer.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/gpu_example.py` & `fedot-0.7.3.2/examples/advanced/gpu_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/multi_modal_pipeline.py` & `fedot-0.7.3.2/examples/advanced/multi_modal_pipeline.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/multimodal_text_num_example.py` & `fedot-0.7.3.2/examples/advanced/multimodal_text_num_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/multiobj_optimisation.py` & `fedot-0.7.3.2/examples/advanced/multiobj_optimisation.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/multitask_classification_regression.py` & `fedot-0.7.3.2/examples/advanced/multitask_classification_regression.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/parallelization_comparison.py` & `fedot-0.7.3.2/examples/advanced/parallelization_comparison.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/pipeline_sensitivity.py` & `fedot-0.7.3.2/examples/advanced/pipeline_sensitivity.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/profiler_example.py` & `fedot-0.7.3.2/examples/advanced/profiler_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/remote_execution/remote_fit_example.py` & `fedot-0.7.3.2/examples/advanced/remote_execution/remote_fit_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/remote_execution/ts_composer_with_integration.py` & `fedot-0.7.3.2/examples/advanced/remote_execution/ts_composer_with_integration.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/structural_analysis/complex_analysis_with_requirements.py` & `fedot-0.7.3.2/examples/advanced/structural_analysis/complex_analysis_with_requirements.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/structural_analysis/dataset_access.py` & `fedot-0.7.3.2/examples/advanced/structural_analysis/dataset_access.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/structural_analysis/pipelines_access.py` & `fedot-0.7.3.2/examples/advanced/structural_analysis/pipelines_access.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/structural_analysis/structural_analysis_example.py` & `fedot-0.7.3.2/examples/advanced/structural_analysis/structural_analysis_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/surrogate_optimization.py` & `fedot-0.7.3.2/examples/advanced/surrogate_optimization.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/time_series_forecasting/composing_pipelines.py` & `fedot-0.7.3.2/examples/advanced/time_series_forecasting/composing_pipelines.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/time_series_forecasting/custom_model_tuning.py` & `fedot-0.7.3.2/examples/advanced/time_series_forecasting/custom_model_tuning.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/time_series_forecasting/exogenous.py` & `fedot-0.7.3.2/examples/advanced/time_series_forecasting/exogenous.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/time_series_forecasting/multi_ts_arctic_forecasting.py` & `fedot-0.7.3.2/examples/advanced/time_series_forecasting/multi_ts_arctic_forecasting.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/time_series_forecasting/multistep.py` & `fedot-0.7.3.2/examples/advanced/time_series_forecasting/multistep.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/time_series_forecasting/nemo.py` & `fedot-0.7.3.2/examples/advanced/time_series_forecasting/nemo.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/time_series_forecasting/nemo_multiple.py` & `fedot-0.7.3.2/examples/advanced/time_series_forecasting/nemo_multiple.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/time_series_forecasting/prediction_intervals.py` & `fedot-0.7.3.2/examples/advanced/time_series_forecasting/prediction_intervals.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/advanced/time_series_forecasting/sparse_lagged_tuning.py` & `fedot-0.7.3.2/examples/advanced/time_series_forecasting/sparse_lagged_tuning.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/project_import_export.py` & `fedot-0.7.3.2/examples/project_import_export.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/api_builder/classification_with_api_builder.py` & `fedot-0.7.3.2/examples/simple/api_builder/classification_with_api_builder.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/api_builder/multiple_ts_forecasting_tasks.py` & `fedot-0.7.3.2/examples/simple/api_builder/multiple_ts_forecasting_tasks.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/classification/api_classification.py` & `fedot-0.7.3.2/examples/simple/classification/api_classification.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/classification/classification_pipelines.py` & `fedot-0.7.3.2/examples/simple/classification/classification_pipelines.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/classification/classification_with_tuning.py` & `fedot-0.7.3.2/examples/simple/classification/classification_with_tuning.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/classification/image_classification_problem.py` & `fedot-0.7.3.2/examples/simple/classification/image_classification_problem.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/classification/multiclass_prediction.py` & `fedot-0.7.3.2/examples/simple/classification/multiclass_prediction.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/classification/resample_example.py` & `fedot-0.7.3.2/examples/simple/classification/resample_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/cli_application/cli_call_example.py` & `fedot-0.7.3.2/examples/simple/cli_application/cli_call_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/interpretable/api_explain.py` & `fedot-0.7.3.2/examples/simple/interpretable/api_explain.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/interpretable/pipeline_explain.py` & `fedot-0.7.3.2/examples/simple/interpretable/pipeline_explain.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/pipeline_and_history_visualization.py` & `fedot-0.7.3.2/examples/simple/pipeline_and_history_visualization.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/pipeline_import_export.py` & `fedot-0.7.3.2/examples/simple/pipeline_import_export.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/pipeline_log.py` & `fedot-0.7.3.2/examples/simple/pipeline_log.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/pipeline_tune.py` & `fedot-0.7.3.2/examples/simple/pipeline_tune.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/pipeline_tuning_with_iopt.py` & `fedot-0.7.3.2/examples/simple/pipeline_tuning_with_iopt.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/pipeline_visualization.py` & `fedot-0.7.3.2/examples/simple/pipeline_visualization.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/regression/api_regression.py` & `fedot-0.7.3.2/examples/simple/regression/api_regression.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/regression/regression_pipelines.py` & `fedot-0.7.3.2/examples/simple/regression/regression_pipelines.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/regression/regression_with_tuning.py` & `fedot-0.7.3.2/examples/simple/regression/regression_with_tuning.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/time_series_forecasting/api_forecasting.py` & `fedot-0.7.3.2/examples/simple/time_series_forecasting/api_forecasting.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/time_series_forecasting/cgru.py` & `fedot-0.7.3.2/examples/simple/time_series_forecasting/cgru.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/time_series_forecasting/fitted_values.py` & `fedot-0.7.3.2/examples/simple/time_series_forecasting/fitted_values.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/time_series_forecasting/gapfilling.py` & `fedot-0.7.3.2/examples/simple/time_series_forecasting/gapfilling.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/time_series_forecasting/ts_pipelines.py` & `fedot-0.7.3.2/examples/simple/time_series_forecasting/ts_pipelines.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/examples/simple/time_series_forecasting/tuning_pipelines.py` & `fedot-0.7.3.2/examples/simple/time_series_forecasting/tuning_pipelines.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/api/api_utils/api_composer.py` & `fedot-0.7.3.2/fedot/api/api_utils/api_composer.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/api/api_utils/api_data.py` & `fedot-0.7.3.2/fedot/api/api_utils/api_data.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/api/api_utils/api_params_repository.py` & `fedot-0.7.3.2/fedot/api/api_utils/api_params_repository.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/api/api_utils/assumptions/assumptions_builder.py` & `fedot-0.7.3.2/fedot/api/api_utils/assumptions/assumptions_builder.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/api/api_utils/assumptions/assumptions_handler.py` & `fedot-0.7.3.2/fedot/api/api_utils/assumptions/assumptions_handler.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/api/api_utils/assumptions/operations_filter.py` & `fedot-0.7.3.2/fedot/api/api_utils/assumptions/operations_filter.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/api/api_utils/assumptions/preprocessing_builder.py` & `fedot-0.7.3.2/fedot/api/api_utils/assumptions/preprocessing_builder.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/api/api_utils/assumptions/task_assumptions.py` & `fedot-0.7.3.2/fedot/api/api_utils/assumptions/task_assumptions.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/api/api_utils/data_definition.py` & `fedot-0.7.3.2/fedot/api/api_utils/data_definition.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/api/api_utils/input_analyser.py` & `fedot-0.7.3.2/fedot/api/api_utils/input_analyser.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/api/api_utils/params.py` & `fedot-0.7.3.2/fedot/api/api_utils/params.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/api/api_utils/predefined_model.py` & `fedot-0.7.3.2/fedot/api/api_utils/predefined_model.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/api/api_utils/presets.py` & `fedot-0.7.3.2/fedot/api/api_utils/presets.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/api/builder.py` & `fedot-0.7.3.2/fedot/api/builder.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/api/fedot_cli.py` & `fedot-0.7.3.2/fedot/api/fedot_cli.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/api/help.py` & `fedot-0.7.3.2/fedot/api/help.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/api/main.py` & `fedot-0.7.3.2/fedot/api/main.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/api/time.py` & `fedot-0.7.3.2/fedot/api/time.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/caching/base_cache.py` & `fedot-0.7.3.2/fedot/core/caching/base_cache.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/caching/base_cache_db.py` & `fedot-0.7.3.2/fedot/core/caching/base_cache_db.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,23 +17,26 @@
     :param main_table: table to store into or load from
     :param cache_dir: path to the place where cache files should be stored.
     :param use_stats: bool indicating if it is needed to use cache performance dict
     :param stats_keys: sequence of keys for supporting cache effectiveness
     """
 
     def __init__(self, main_table: str = 'default', cache_dir: Optional[str] = None, use_stats: bool = False,
-                 stats_keys: Sequence = ('default_hit', 'default_total')):
+                 stats_keys: Sequence = ('default_hit', 'default_total'),
+                 custom_pid=None):
         self._main_table = main_table
         self._db_suffix = f'.{main_table}_db'
         if cache_dir is None or Path(cache_dir).samefile(default_fedot_data_dir()):
             self.db_path = Path(default_fedot_data_dir())
             self._del_prev_temps()
         else:
             self.db_path = Path(cache_dir)
-        self.db_path = self.db_path.joinpath(f'cache_{os.getpid()}').with_suffix(self._db_suffix)
+
+        pid = custom_pid if custom_pid is not None else os.getpid()
+        self.db_path = self.db_path.joinpath(f'cache_{pid}').with_suffix(self._db_suffix)
 
         self._eff_table = 'effectiveness'
         self.use_stats = use_stats
         self._effectiveness_keys = stats_keys
         self._init_eff()
 
     def get_effectiveness(self) -> Optional[Tuple[int, int, int, int]]:
```

### Comparing `fedot-0.7.3.1/fedot/core/caching/pipelines_cache.py` & `fedot-0.7.3.2/fedot/core/caching/pipelines_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 class OperationsCache(BaseCache):
     """
     Stores/loads nodes `fitted_operation` field to increase performance of calculations.
 
     :param cache_dir: path to the place where cache files should be stored.
     """
 
-    def __init__(self, cache_dir: Optional[str] = None):
-        super().__init__(OperationsCacheDB(cache_dir))
+    def __init__(self, cache_dir: Optional[str] = None, custom_pid=None):
+        super().__init__(OperationsCacheDB(cache_dir, custom_pid))
 
     def save_nodes(self, nodes: Union[PipelineNode, List[PipelineNode]], fold_id: Optional[int] = None):
         """
         :param nodes: node/nodes to be cached
         :param fold_id: optional part of cache item UID
                             (can be used to specify the number of CV fold)
         """
```

### Comparing `fedot-0.7.3.1/fedot/core/caching/pipelines_cache_db.py` & `fedot-0.7.3.2/fedot/core/caching/pipelines_cache_db.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     """
     Database for `OperationsCache` class.
     Includes low-level idea of caching pipeline nodes using relational database.
 
     :param cache_dir: path to the place where cache files should be stored.
     """
 
-    def __init__(self, cache_dir: Optional[str] = None):
+    def __init__(self, cache_dir: Optional[str] = None, custom_pid=None):
         super().__init__('operations', cache_dir, False, [
-            'pipelines_hit', 'pipelines_total', 'nodes_hit', 'nodes_total'])
+            'pipelines_hit', 'pipelines_total', 'nodes_hit', 'nodes_total'], custom_pid)
         self._init_db()
 
     @staticmethod
     def _create_temp_for_ordered_select(cur: sqlite3.Cursor, uids: List[str]) -> str:
         """
         Creates temp table to keep order of uids while doing select operation in operations getter.
```

### Comparing `fedot-0.7.3.1/fedot/core/caching/preprocessing_cache.py` & `fedot-0.7.3.2/fedot/core/caching/preprocessing_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     """
     Usage of that class makes sense only if you have table data.
     Stores/loads `DataPreprocessor`'s encoders and imputers for pipelines to decrease optional preprocessing time.
 
     :param cache_dir: path to the place where cache files should be stored.
     """
 
-    def __init__(self, cache_dir: Optional[str] = None):
-        super().__init__(PreprocessingCacheDB(cache_dir))
+    def __init__(self, cache_dir: Optional[str] = None, custom_pid=None):
+        super().__init__(PreprocessingCacheDB(cache_dir, custom_pid))
 
     def try_load_preprocessor(self, pipeline: 'Pipeline', fold_id: Union[int, None]):
         """
         Tries to find preprocessor in DB table and load it for pipeline
 
         :param pipeline: pipeline to load preprocessor for
         :param fold_id: number of fold
```

### Comparing `fedot-0.7.3.1/fedot/core/caching/preprocessing_cache_db.py` & `fedot-0.7.3.2/fedot/core/caching/preprocessing_cache_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     """
     Database for `PreprocessingCache` class.
     Includes low-level idea of caching pipeline preprocessor items using relational database.
 
     :param cache_dir: path to the place where cache files should be stored.
     """
 
-    def __init__(self, cache_dir: Optional[str] = None):
-        super().__init__('preprocessors', cache_dir, False, ['preprocessors_hit', 'preprocessors_total'])
+    def __init__(self, cache_dir: Optional[str] = None, custom_pid=None):
+        super().__init__('preprocessors', cache_dir, False, ['preprocessors_hit', 'preprocessors_total'], custom_pid)
         self._init_db()
 
     def get_preprocessor(self, uid: str) -> Optional[Tuple[
         Dict[str, OneHotEncodingImplementation], Dict[str, ImputationImplementation]
     ]]:
         """
         Tries to return both data processors, None if is not found
```

### Comparing `fedot-0.7.3.1/fedot/core/composer/composer.py` & `fedot-0.7.3.2/fedot/core/composer/composer.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/composer/composer_builder.py` & `fedot-0.7.3.2/fedot/core/composer/composer_builder.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/composer/gp_composer/gp_composer.py` & `fedot-0.7.3.2/fedot/core/composer/gp_composer/gp_composer.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/composer/gp_composer/specific_operators.py` & `fedot-0.7.3.2/fedot/core/composer/gp_composer/specific_operators.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/composer/meta_rules.py` & `fedot-0.7.3.2/fedot/core/composer/meta_rules.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/composer/metrics.py` & `fedot-0.7.3.2/fedot/core/composer/metrics.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/composer/random_composer.py` & `fedot-0.7.3.2/fedot/core/composer/random_composer.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/data/array_utilities.py` & `fedot-0.7.3.2/fedot/core/data/array_utilities.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/data/cv_folds.py` & `fedot-0.7.3.2/fedot/core/data/cv_folds.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/data/data.py` & `fedot-0.7.3.2/fedot/core/data/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                             data_type: the type of the data. Possible values are listed at :class:`DataTypesEnum`.
 
                         Returns:
                             data
                         """
         if isinstance(task, str):
             task = Task(TaskTypesEnum(task))
-        if not target_array:
+        if target_array is None:
             target_array = features_array
         return array_to_input_data(features_array, target_array, idx, task, data_type)
 
     @classmethod
     def from_dataframe(cls,
                        features_df: Union[pd.DataFrame, pd.Series],
                        target_df: Union[pd.DataFrame, pd.Series],
```

### Comparing `fedot-0.7.3.1/fedot/core/data/data_detection.py` & `fedot-0.7.3.2/fedot/core/data/data_detection.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/data/data_preprocessing.py` & `fedot-0.7.3.2/fedot/core/data/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/data/data_split.py` & `fedot-0.7.3.2/fedot/core/data/data_split.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/data/load_data.py` & `fedot-0.7.3.2/fedot/core/data/load_data.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/data/merge/data_merger.py` & `fedot-0.7.3.2/fedot/core/data/merge/data_merger.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/data/merge/supplementary_data_merger.py` & `fedot-0.7.3.2/fedot/core/data/merge/supplementary_data_merger.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/data/multi_modal.py` & `fedot-0.7.3.2/fedot/core/data/multi_modal.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/data/supplementary_data.py` & `fedot-0.7.3.2/fedot/core/data/supplementary_data.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/data/visualisation.py` & `fedot-0.7.3.2/fedot/core/data/visualisation.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/atomized_model.py` & `fedot-0.7.3.2/fedot/core/operations/atomized_model.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/atomized_template.py` & `fedot-0.7.3.2/fedot/core/operations/atomized_template.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/data_operation.py` & `fedot-0.7.3.2/fedot/core/operations/data_operation.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/automl.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/automl.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/boostings.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/boostings.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/classification.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/classification.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/clustering.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/clustering.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/common_preprocessing.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/common_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/custom.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/custom.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/data_source.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/data_source.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/evaluation_interfaces.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/evaluation_interfaces.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/gpu/classification.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/gpu/classification.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/gpu/clustering.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/gpu/clustering.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/gpu/common.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/gpu/common.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/gpu/regression.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/gpu/regression.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/categorical_encoders.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/categorical_encoders.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/decompose.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/decompose.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_filters.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_filters.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_imbalanced_class.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_imbalanced_class.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_selectors.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_selectors.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_transformations.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_transformations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,102 +3,111 @@
 
 import numpy as np
 import pandas as pd
 from sklearn.decomposition import FastICA, KernelPCA, PCA
 from sklearn.impute import SimpleImputer
 from sklearn.preprocessing import MinMaxScaler, PolynomialFeatures, StandardScaler
 
+from fedot.core.constants import PCA_MIN_THRESHOLD_TS
 from fedot.core.data.data import InputData, OutputData, data_type_is_table
 from fedot.core.data.data_preprocessing import convert_into_column, data_has_categorical_features, \
     divide_data_categorical_numerical, find_categorical_columns, replace_inf_with_nans
 from fedot.core.operations.evaluation.operation_implementations. \
     implementation_interfaces import DataOperationImplementation, EncodedInvariantImplementation
 from fedot.core.operations.operation_parameters import OperationParameters
+from fedot.core.repository.dataset_types import DataTypesEnum
 from fedot.preprocessing.data_types import TYPE_TO_ID
 
 
 class ComponentAnalysisImplementation(DataOperationImplementation):
-    """ Class for applying PCA and kernel PCA models from sklearn
+    """
+    Class for applying PCA and kernel PCA models from sklearn
 
     Args:
-        params: OpearationParameters with the arguments
+        params: OperationParameters with the arguments
     """
 
     def __init__(self, params: Optional[OperationParameters]):
         super().__init__(params)
         self.pca = None
         self.number_of_features = None
         self.number_of_samples = None
 
-    def fit(self, input_data: InputData):
-        """The method trains the PCA model
+    def fit(self, input_data: InputData) -> PCA:
+        """
+        The method trains the PCA model
 
         Args:
             input_data: data with features, target and ids for PCA training
 
         Returns:
             trained PCA model (optional output)
         """
 
         self.number_of_samples, self.number_of_features = np.array(input_data.features).shape
 
         if self.number_of_features > 1:
-            self.check_and_correct_params()
+            self.check_and_correct_params(is_ts_data=input_data.data_type is DataTypesEnum.ts)
             self.pca.fit(input_data.features)
 
         return self.pca
 
     def transform(self, input_data: InputData) -> OutputData:
-        """Method for transformation tabular data using PCA
+        """
+        Method for transformation tabular data using PCA
 
         Args:
             input_data: data with features, target and ids for PCA applying
 
         Returns:
             data with transformed features attribute
         """
 
         if self.number_of_features > 1:
             transformed_features = self.pca.transform(input_data.features)
         else:
             transformed_features = input_data.features
 
         # Update features
-        output_data = self._convert_to_output(input_data,
-                                              transformed_features)
+        output_data = self._convert_to_output(input_data, transformed_features)
         self.update_column_types(output_data)
         return output_data
 
-    def check_and_correct_params(self):
-        """Method check if number of features in data enough for ``n_components``
+    def check_and_correct_params(self, is_ts_data: bool = False):
+        """
+        Method check if number of features in data enough for ``n_components``
         parameter in PCA or not. And if not enough - fixes it
         """
         n_components = self.params.get('n_components')
         if isinstance(n_components, int):
             if n_components > self.number_of_features:
                 self.params.update(n_components=self.number_of_features)
         elif n_components == 'mle':
             # Check that n_samples correctly map with n_features
             if self.number_of_samples < self.number_of_features:
                 self.params.update(n_components=0.5)
+        if is_ts_data and (n_components * self.number_of_features) < PCA_MIN_THRESHOLD_TS:
+            self.params.update(n_components=PCA_MIN_THRESHOLD_TS / self.number_of_features)
 
         self.pca.set_params(**self.params.to_dict())
 
     @staticmethod
     def update_column_types(output_data: OutputData) -> OutputData:
-        """Update column types after applying PCA operations
+        """
+        Update column types after applying PCA operations
         """
 
         _, n_cols = output_data.predict.shape
         output_data.supplementary_data.col_type_ids['features'] = np.array([TYPE_TO_ID[float]] * n_cols)
         return output_data
 
 
 class PCAImplementation(ComponentAnalysisImplementation):
-    """Class for applying PCA from sklearn
+    """
+    Class for applying PCA from sklearn
 
     Args:
         params: OperationParameters with the hyperparameters
     """
 
     def __init__(self, params: Optional[OperationParameters] = None):
         super().__init__(params)
@@ -107,39 +116,42 @@
             default_params = {'svd_solver': 'full', 'n_components': 'mle'}
             self.params.update(**default_params)
         self.pca = PCA(**self.params.to_dict())
         self.number_of_features = None
 
 
 class KernelPCAImplementation(ComponentAnalysisImplementation):
-    """ Class for applying kernel PCA from sklearn
+    """
+    Class for applying kernel PCA from sklearn
 
     Args:
         params: OperationParameters with the hyperparameters
     """
 
     def __init__(self, params: Optional[OperationParameters]):
         super().__init__(params)
         self.pca = KernelPCA(**self.params.to_dict())
 
 
 class FastICAImplementation(ComponentAnalysisImplementation):
-    """ Class for applying FastICA from sklearn
+    """
+    Class for applying FastICA from sklearn
 
     Args:
         params: OperationParameters with the hyperparameters
     """
 
     def __init__(self, params: Optional[OperationParameters]):
         super().__init__(params)
         self.pca = FastICA(**self.params.to_dict())
 
 
 class PolyFeaturesImplementation(EncodedInvariantImplementation):
-    """ Class for application of :obj:`PolynomialFeatures` operation on data,
+    """
+    Class for application of :obj:`PolynomialFeatures` operation on data,
     where only not encoded features (were not converted from categorical using
     ``OneHot encoding``) are used
 
     Args:
         params: OperationParameters with the arguments
     """
 
@@ -154,27 +166,30 @@
             poly_params = {k: self.params.get(k) for k in
                            ['degree', 'interaction_only']}
             self.operation = PolynomialFeatures(include_bias=False,
                                                 **poly_params)
         self.columns_to_take = None
 
     def fit(self, input_data: InputData):
-        """ Method for fit Poly features operation """
+        """
+        Method for fit Poly features operation
+        """
         # Check the number of columns in source dataset
         n_rows, n_cols = input_data.features.shape
         if n_cols > self.th_columns:
             # Randomly choose subsample of features columns - 10 features
             column_indices = np.arange(n_cols)
             self.columns_to_take = random.sample(list(column_indices), self.th_columns)
             input_data = input_data.subset_features(self.columns_to_take)
 
         return super().fit(input_data)
 
     def transform(self, input_data: InputData) -> OutputData:
-        """Firstly perform filtration of columns
+        """
+        Firstly perform filtration of columns
         """
 
         clipped_input_data = input_data
         if self.columns_to_take is not None:
             clipped_input_data = input_data.subset_features(self.columns_to_take)
         output_data = super().transform(clipped_input_data)
```

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/text_preprocessing.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/text_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/text_pretrained.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/text_pretrained.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/topological/fast_topological_extractor.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/topological/fast_topological_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         self._shape = len(self.quantiles)
         self._window_size = None
 
     def fit(self, input_data: InputData):
         self._window_size = int(input_data.features.shape[1] * self.window_size_as_share)
         self._window_size = max(self._window_size, 2)
         self._window_size = min(self._window_size, input_data.features.shape[1] - 2)
+        self._window_size = max(self._window_size, 1)
         return self
 
     def transform(self, input_data: InputData) -> OutputData:
         features = input_data.features
         with Parallel(n_jobs=self.n_jobs, prefer='processes') as parallel:
             topological_features = parallel(delayed(self._extract_features)
                                             (np.mean(features[i:i + 2, ::self.stride], axis=0))
```

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/data_operations/ts_transformations.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/data_operations/ts_transformations.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/implementation_interfaces.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/implementation_interfaces.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/boostings_implementations.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/boostings_implementations.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/custom_model.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/discriminant_analysis.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/discriminant_analysis.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/keras.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/keras.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/knn.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/knn.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/svc.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/svc.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/arima.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/arima.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/cgru.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/cgru.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/naive.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/naive.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/poly.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/poly.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/statsmodels.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/statsmodels.py`

 * *Files 3% similar despite different names*

```diff
@@ -246,26 +246,32 @@
 
 class ExpSmoothingImplementation(ModelImplementation):
     """ Exponential smoothing implementation from statsmodels """
 
     def __init__(self, params: OperationParameters):
         super().__init__(params)
         self.model = None
-        if self.params.get("seasonal"):
-            self.seasonal_periods = int(self.params.get("seasonal_periods"))
+        if self.params.get('seasonal'):
+            self.seasonal_periods = int(self.params.get('seasonal_periods'))
         else:
             self.seasonal_periods = None
 
     def fit(self, input_data):
+        endog = input_data.features.astype('float64')
+
+        # check ets params according to statsmodels restrictions
+        if self._check_and_correct_params(endog):
+            self.log.info(f'Changed the following ETSModel parameters: {self.params.changed_parameters}')
+
         self.model = ETSModel(
-            input_data.features.astype("float64"),
-            error=self.params.get("error"),
-            trend=self.params.get("trend"),
-            seasonal=self.params.get("seasonal"),
-            damped_trend=self.params.get("damped_trend") if self.params.get("trend") else None,
+            endog=endog,
+            error=self.params.get('error'),
+            trend=self.params.get('trend'),
+            seasonal=self.params.get('seasonal'),
+            damped_trend=self.params.get('damped_trend') if self.params.get('trend') else None,
             seasonal_periods=self.seasonal_periods
         )
         self.model = self.model.fit(disp=False)
         return self.model
 
     def predict(self, input_data):
         input_data = copy(input_data)
@@ -308,7 +314,25 @@
         input_data.idx = new_idx
         input_data.target = target_columns
 
         output_data = self._convert_to_output(input_data,
                                               predict=predict,
                                               data_type=DataTypesEnum.table)
         return output_data
+
+    def _check_and_correct_params(self, endog: np.ndarray) -> bool:
+        ets_components = ['error', 'trend', 'seasonal']
+        params_changed = False
+        if any(self.params.get(component) == 'mul' for component in ets_components):
+            if np.any(endog <= 0):
+                for component in ets_components:
+                    if self.params.get(component) == 'mul':
+                        self.params.update(**{f'{component}': 'add'})
+                params_changed = True
+
+        if self.params.get('trend') == 'mul' \
+                and self.params.get('damped_trend') \
+                and not self.params.get('seasonal'):
+            self.params.update(trend='add')
+            params_changed = True
+
+        return params_changed
```

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/regression.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/regression.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/text.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/text.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/evaluation/time_series.py` & `fedot-0.7.3.2/fedot/core/operations/evaluation/time_series.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/factory.py` & `fedot-0.7.3.2/fedot/core/operations/factory.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/hyperparameters_preprocessing.py` & `fedot-0.7.3.2/fedot/core/operations/hyperparameters_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/model.py` & `fedot-0.7.3.2/fedot/core/operations/model.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/operation.py` & `fedot-0.7.3.2/fedot/core/operations/operation.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/operation_parameters.py` & `fedot-0.7.3.2/fedot/core/operations/operation_parameters.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/operations/operation_template.py` & `fedot-0.7.3.2/fedot/core/operations/operation_template.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/optimisers/objective/data_objective_eval.py` & `fedot-0.7.3.2/fedot/core/optimisers/objective/data_objective_eval.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/optimisers/objective/data_source_splitter.py` & `fedot-0.7.3.2/fedot/core/optimisers/objective/data_source_splitter.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/optimisers/objective/metrics_objective.py` & `fedot-0.7.3.2/fedot/core/optimisers/objective/metrics_objective.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/optimisers/objective/objective_serialization.py` & `fedot-0.7.3.2/fedot/core/optimisers/objective/objective_serialization.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/adapters.py` & `fedot-0.7.3.2/fedot/core/pipelines/adapters.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/automl_wrappers.py` & `fedot-0.7.3.2/fedot/core/pipelines/automl_wrappers.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/node.py` & `fedot-0.7.3.2/fedot/core/pipelines/node.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/pipeline.py` & `fedot-0.7.3.2/fedot/core/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/pipeline_advisor.py` & `fedot-0.7.3.2/fedot/core/pipelines/pipeline_advisor.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/pipeline_composer_requirements.py` & `fedot-0.7.3.2/fedot/core/pipelines/pipeline_composer_requirements.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/pipeline_graph_generation_params.py` & `fedot-0.7.3.2/fedot/core/pipelines/pipeline_graph_generation_params.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/pipeline_node_factory.py` & `fedot-0.7.3.2/fedot/core/pipelines/pipeline_node_factory.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/graph_distance.py` & `fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/graph_distance.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/main.py` & `fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/main.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/metrics.py` & `fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/metrics.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/params.py` & `fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/params.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/pipeline_constraints.py` & `fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/pipeline_constraints.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/solvers/best_pipelines_quantiles.py` & `fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/solvers/best_pipelines_quantiles.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/solvers/last_generation_quantile_loss.py` & `fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/solvers/last_generation_quantile_loss.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/solvers/mutation_of_best_pipeline.py` & `fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/solvers/mutation_of_best_pipeline.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/ts_mutation.py` & `fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/ts_mutation.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/tuners.py` & `fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/tuners.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/utils.py` & `fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/utils.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/prediction_intervals/visualization.py` & `fedot-0.7.3.2/fedot/core/pipelines/prediction_intervals/visualization.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/random_pipeline_factory.py` & `fedot-0.7.3.2/fedot/core/pipelines/random_pipeline_factory.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/template.py` & `fedot-0.7.3.2/fedot/core/pipelines/template.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/ts_wrappers.py` & `fedot-0.7.3.2/fedot/core/pipelines/ts_wrappers.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/tuning/hyperparams.py` & `fedot-0.7.3.2/fedot/core/pipelines/tuning/hyperparams.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/tuning/search_space.py` & `fedot-0.7.3.2/fedot/core/pipelines/tuning/search_space.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,15 @@
                     'type': 'categorical'},
                 'damped_trend': {
                     'hyperopt-dist': hp.choice,
                     'sampling-scope': [[True, False]],
                     'type': 'categorical'},
                 'seasonal_periods': {
                     'hyperopt-dist': hp.uniform,
-                    'sampling-scope': [1, 100],
+                    'sampling-scope': [2, 100],
                     'type': 'continuous'}
             },
             'glm': {
                 NESTED_PARAMS_LABEL: {
                     'hyperopt-dist': hp.choice,
                     'sampling-scope': [[
                         {
```

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/tuning/tuner_builder.py` & `fedot-0.7.3.2/fedot/core/pipelines/tuning/tuner_builder.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/verification.py` & `fedot-0.7.3.2/fedot/core/pipelines/verification.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/pipelines/verification_rules.py` & `fedot-0.7.3.2/fedot/core/pipelines/verification_rules.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/repository/data/automl_repository.json` & `fedot-0.7.3.2/fedot/core/repository/data/automl_repository.json`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/repository/data/data_operation_repository.json` & `fedot-0.7.3.2/fedot/core/repository/data/data_operation_repository.json`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/repository/data/default_operation_params.json` & `fedot-0.7.3.2/fedot/core/repository/data/default_operation_params.json`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/repository/data/gpu_models_repository.json` & `fedot-0.7.3.2/fedot/core/repository/data/gpu_models_repository.json`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/repository/data/model_repository.json` & `fedot-0.7.3.2/fedot/core/repository/data/model_repository.json`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/repository/dataset_types.py` & `fedot-0.7.3.2/fedot/core/repository/dataset_types.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/repository/default_params_repository.py` & `fedot-0.7.3.2/fedot/core/repository/default_params_repository.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/repository/graph_operation_repository.py` & `fedot-0.7.3.2/fedot/core/repository/graph_operation_repository.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/repository/json_evaluation.py` & `fedot-0.7.3.2/fedot/core/repository/json_evaluation.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/repository/metrics_repository.py` & `fedot-0.7.3.2/fedot/core/repository/metrics_repository.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/repository/operation_types_repository.py` & `fedot-0.7.3.2/fedot/core/repository/operation_types_repository.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/repository/pipeline_operation_repository.py` & `fedot-0.7.3.2/fedot/core/repository/pipeline_operation_repository.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/repository/tasks.py` & `fedot-0.7.3.2/fedot/core/repository/tasks.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/utils.py` & `fedot-0.7.3.2/fedot/core/utils.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/core/visualisation/pipeline_specific_visuals.py` & `fedot-0.7.3.2/fedot/core/visualisation/pipeline_specific_visuals.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/explainability/explainers.py` & `fedot-0.7.3.2/fedot/explainability/explainers.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/explainability/surrogate_explainer.py` & `fedot-0.7.3.2/fedot/explainability/surrogate_explainer.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/preprocessing/base_preprocessing.py` & `fedot-0.7.3.2/fedot/preprocessing/base_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/preprocessing/categorical.py` & `fedot-0.7.3.2/fedot/preprocessing/categorical.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/preprocessing/data_type_check.py` & `fedot-0.7.3.2/fedot/preprocessing/data_type_check.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/preprocessing/data_types.py` & `fedot-0.7.3.2/fedot/preprocessing/data_types.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/preprocessing/dummy_preprocessing.py` & `fedot-0.7.3.2/fedot/preprocessing/dummy_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/preprocessing/preprocessing.py` & `fedot-0.7.3.2/fedot/preprocessing/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         super().__init__()
 
         self.log = default_log(self)
 
     def __setstate__(self, state):
         # Implemented for backward compatibility for unpickling
         #  Pipelines with older preprocessor that had DiGraph with Nodes inside.
-        #  see https://github.com/nccr-itmo/FEDOT/pull/802
+        #  see https://github.com/aimclub/FEDOT/pull/802
         unrelevant_fields = ['structure_analysis']
         for field in unrelevant_fields:
             if field in state:
                 del state[field]
         self.__dict__.update(state)
 
     def _init_supplementary_preprocessors(self, data: Union[InputData, MultiModalData]):
```

### Comparing `fedot-0.7.3.1/fedot/preprocessing/structure.py` & `fedot-0.7.3.2/fedot/preprocessing/structure.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/remote/infrastructure/clients/client.py` & `fedot-0.7.3.2/fedot/remote/infrastructure/clients/client.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/remote/infrastructure/clients/datamall_client.py` & `fedot-0.7.3.2/fedot/remote/infrastructure/clients/datamall_client.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/remote/infrastructure/clients/test_client.py` & `fedot-0.7.3.2/fedot/remote/infrastructure/clients/test_client.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/remote/pipeline_run_config.py` & `fedot-0.7.3.2/fedot/remote/pipeline_run_config.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/remote/remote_evaluator.py` & `fedot-0.7.3.2/fedot/remote/remote_evaluator.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/remote/run_pipeline.py` & `fedot-0.7.3.2/fedot/remote/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/structural_analysis/operations_hp_sensitivity/multi_operations_sensitivity.py` & `fedot-0.7.3.2/fedot/structural_analysis/operations_hp_sensitivity/multi_operations_sensitivity.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/structural_analysis/operations_hp_sensitivity/one_operation_sensitivity.py` & `fedot-0.7.3.2/fedot/structural_analysis/operations_hp_sensitivity/one_operation_sensitivity.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/structural_analysis/operations_hp_sensitivity/problem.py` & `fedot-0.7.3.2/fedot/structural_analysis/operations_hp_sensitivity/problem.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/structural_analysis/operations_hp_sensitivity/sa_and_sample_methods.py` & `fedot-0.7.3.2/fedot/structural_analysis/operations_hp_sensitivity/sa_and_sample_methods.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/structural_analysis/sa_requirements.py` & `fedot-0.7.3.2/fedot/structural_analysis/sa_requirements.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/utilities/composer_timer.py` & `fedot-0.7.3.2/fedot/utilities/composer_timer.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/utilities/debug.py` & `fedot-0.7.3.2/fedot/utilities/debug.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/utilities/define_metric_by_task.py` & `fedot-0.7.3.2/fedot/utilities/define_metric_by_task.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/utilities/golem_imports_transition.py` & `fedot-0.7.3.2/fedot/utilities/golem_imports_transition.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/utilities/memory.py` & `fedot-0.7.3.2/fedot/utilities/memory.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/utilities/project_import_export.py` & `fedot-0.7.3.2/fedot/utilities/project_import_export.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/utilities/random.py` & `fedot-0.7.3.2/fedot/utilities/random.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/utilities/synth_dataset_generator.py` & `fedot-0.7.3.2/fedot/utilities/synth_dataset_generator.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/utilities/ts_gapfilling.py` & `fedot-0.7.3.2/fedot/utilities/ts_gapfilling.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot/utilities/window_size_selector.py` & `fedot-0.7.3.2/fedot/utilities/window_size_selector.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.3.1/fedot.egg-info/PKG-INFO` & `fedot-0.7.3.2/fedot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: fedot
-Version: 0.7.3.1
+Version: 0.7.3.2
 Summary: Automated machine learning framework for composite pipelines
 Home-page: https://github.com/aimclub/FEDOT
 Author: NSS Lab
 Author-email: itmo.nss.team@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
+Requires-Dist: scipy<1.13.0
 Requires-Dist: thegolem==0.4.0
 Requires-Dist: numpy!=1.24.0,>=1.16.0
 Requires-Dist: pandas>=1.3.0; python_version >= "3.8"
 Requires-Dist: anytree>=2.8.0
 Requires-Dist: catboost>=0.25.0
 Requires-Dist: lightgbm>=3.0.0
 Requires-Dist: xgboost>=1.4.0
 Requires-Dist: statsmodels>=0.12.0
 Requires-Dist: ete3>=3.1.0
 Requires-Dist: networkx!=2.7.*,!=2.8.1,!=2.8.2,!=2.8.3,>=2.4
 Requires-Dist: scikit_learn>=1.0.0; python_version >= "3.8"
-Requires-Dist: sktime==0.16.1
+Requires-Dist: sktime==0.16.1; python_version <= "3.10"
+Requires-Dist: sktime>=0.16.1; python_version > "3.10"
 Requires-Dist: hyperopt==0.2.7
 Requires-Dist: SALib>=1.3.0
 Requires-Dist: scikit-optimize>=0.7.4
 Requires-Dist: matplotlib>=3.3.1; python_version >= "3.8"
 Requires-Dist: pyvis==0.2.1
 Requires-Dist: seaborn>=0.9.0
 Requires-Dist: func_timeout==4.3.5
@@ -49,15 +51,15 @@
 Requires-Dist: h2o==3.42.0.1; extra == "examples"
 Requires-Dist: openpyxl==3.0.7; extra == "examples"
 Provides-Extra: extra
 Requires-Dist: tensorflow>=2.8.0; python_version >= "3.8" and extra == "extra"
 Requires-Dist: torch>=1.9.0; extra == "extra"
 Requires-Dist: opencv-python>=4.5.5.64; extra == "extra"
 Requires-Dist: Pillow>=8.2.0; extra == "extra"
-Requires-Dist: gensim>=4.1.2; extra == "extra"
+Requires-Dist: gensim==4.3.2; extra == "extra"
 Requires-Dist: nltk>=3.5; extra == "extra"
 Requires-Dist: protobuf~=3.19.0; extra == "extra"
 Requires-Dist: giotto_tda==0.6.0; extra == "extra"
 Requires-Dist: ripser==0.6.4; extra == "extra"
 Provides-Extra: profilers
 Requires-Dist: snakeviz==2.1.0; extra == "profilers"
 Requires-Dist: gprof2dot==2021.2.21; extra == "profilers"
@@ -125,26 +127,32 @@
 - **Versatility.** FEDOT is `not limited to specific modeling tasks <https://fedot.readthedocs.io/en/master/advanced/architecture.html>`_, for example, it can be used in ODE or PDE;
 - **Reproducibility.** Resulting pipelines can be `exported separately as JSON <https://fedot.readthedocs.io/en/master/advanced/pipeline_import_export.html>`_ or `together with your input data as ZIP archive <https://fedot.readthedocs.io/en/master/advanced/project_import_export.html>`_ for experiments reproducibility;
 - **Customizability.** FEDOT allows `managing models complexity <https://fedot.readthedocs.io/en/master/introduction/fedot_features/automation_features.html#models-used>`_ and thereby achieving desired quality.
 
 Installation
 ============
 
+- Package installer for Python **pip**
+
 The simplest way to install FEDOT is using ``pip``:
 
 .. code-block::
 
   $ pip install fedot
 
 Installation with optional dependencies for image and text processing, and for DNNs:
 
 .. code-block::
 
   $ pip install fedot[extra]
 
+- **Docker** container
+
+Available docker images can be found here `here <https://github.com/aimclub/FEDOT/tree/master/docker/README_en.rst>`_.
+
 How to Use
 ==========
 
 FEDOT provides a high-level API that allows you to use its capabilities in a simple way. The API can be used for classification, regression, and time series forecasting problems.
 
 To use the API, follow these steps:
```

### Comparing `fedot-0.7.3.1/fedot.egg-info/SOURCES.txt` & `fedot-0.7.3.2/fedot.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -294,8 +294,9 @@
 fedot/utilities/golem_imports_transition.py
 fedot/utilities/memory.py
 fedot/utilities/pattern_wrappers.py
 fedot/utilities/project_import_export.py
 fedot/utilities/random.py
 fedot/utilities/synth_dataset_generator.py
 fedot/utilities/ts_gapfilling.py
-fedot/utilities/window_size_selector.py
+fedot/utilities/window_size_selector.py
+test/test_gpu_strategy.py
```

### Comparing `fedot-0.7.3.1/fedot.egg-info/requires.txt` & `fedot-0.7.3.2/fedot.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,36 @@
+scipy<1.13.0
 thegolem==0.4.0
 numpy!=1.24.0,>=1.16.0
 anytree>=2.8.0
 catboost>=0.25.0
 lightgbm>=3.0.0
 xgboost>=1.4.0
 statsmodels>=0.12.0
 ete3>=3.1.0
 networkx!=2.7.*,!=2.8.1,!=2.8.2,!=2.8.3,>=2.4
-sktime==0.16.1
 hyperopt==0.2.7
 SALib>=1.3.0
 scikit-optimize>=0.7.4
 pyvis==0.2.1
 seaborn>=0.9.0
 func_timeout==4.3.5
 joblib>=0.17.0
 requests>=2.0
 typing>=3.7.0
 psutil>=5.9.2
 pytest>=6.2.0
 testfixtures>=6.18.0
 
+[:python_version <= "3.10"]
+sktime==0.16.1
+
+[:python_version > "3.10"]
+sktime>=0.16.1
+
 [:python_version >= "3.8"]
 pandas>=1.3.0
 scikit_learn>=1.0.0
 matplotlib>=3.3.1
 
 [docs]
 sphinx==4.2.0
@@ -38,15 +44,15 @@
 h2o==3.42.0.1
 openpyxl==3.0.7
 
 [extra]
 torch>=1.9.0
 opencv-python>=4.5.5.64
 Pillow>=8.2.0
-gensim>=4.1.2
+gensim==4.3.2
 nltk>=3.5
 protobuf~=3.19.0
 giotto_tda==0.6.0
 ripser==0.6.4
 
 [extra:python_version >= "3.8"]
 tensorflow>=2.8.0
```

### Comparing `fedot-0.7.3.1/setup.py` & `fedot-0.7.3.2/setup.py`

 * *Files identical despite different names*


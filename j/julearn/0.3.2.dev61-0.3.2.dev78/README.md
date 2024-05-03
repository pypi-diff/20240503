# Comparing `tmp/julearn-0.3.2.dev61.tar.gz` & `tmp/julearn-0.3.2.dev78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "julearn-0.3.2.dev61.tar", last modified: Mon Apr 29 15:28:19 2024, max compression
+gzip compressed data, was "julearn-0.3.2.dev78.tar", last modified: Fri May  3 14:51:10 2024, max compression
```

## Comparing `julearn-0.3.2.dev61.tar` & `julearn-0.3.2.dev78.tar`

### file list

```diff
@@ -1,288 +1,294 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.151298 julearn-0.3.2.dev61/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.103298 julearn-0.3.2.dev61/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.111298 julearn-0.3.2.dev61/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/.github/ISSUE_TEMPLATE/documentation_request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/.github/ISSUE_TEMPLATE/feature_request.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.111298 julearn-0.3.2.dev61/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/.github/workflows/check-stale.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/.github/workflows/ci-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/.github/workflows/docs-preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-29 15:28:19.151298 julearn-0.3.2.dev61/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.115298 julearn-0.3.2.dev61/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.103298 julearn-0.3.2.dev61/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.115298 julearn-0.3.2.dev61/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.115298 julearn-0.3.2.dev61/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/_static/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.115298 julearn-0.3.2.dev61/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/_templates/function.rst
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/_templates/function_warning.rst
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/_templates/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.119298 julearn-0.3.2.dev61/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/api/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/api/inspect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/api/main.rst
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/api/model_selection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/api/models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/api/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/api/prepare.rst
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/api/scoring.rst
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/api/stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/api/transformers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/api/viz.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/available_pipeline_steps.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.119298 julearn-0.3.2.dev61/docs/changes/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/changes/contributors.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.119298 julearn-0.3.2.dev61/docs/changes/newsfragments/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/changes/newsfragments/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/changes/newsfragments/224.misc
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/changes/newsfragments/244.misc
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/changes/newsfragments/249.bugfix
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/changes/newsfragments/251.misc
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/changes/newsfragments/255.bugfix
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/changes/newsfragments/260.enh
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/changes/newsfragments/260.misc
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.123298 julearn-0.3.2.dev61/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    69241 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/images/corrected_ttest.png
--rw-r--r--   0 runner    (1001) docker     (127)    39468 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/images/final_estimator.png
--rw-r--r--   0 runner    (1001) docker     (127)    16172 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/images/iris_X.png
--rw-r--r--   0 runner    (1001) docker     (127)    51228 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/images/iris_df.png
--rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/images/iris_y.png
--rw-r--r--   0 runner    (1001) docker     (127)    54482 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/images/julearn_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    74874 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/images/julearn_logo_calm.png
--rw-r--r--   0 runner    (1001) docker     (127)    78884 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/images/julearn_logo_confbias.png
--rw-r--r--   0 runner    (1001) docker     (127)    61311 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/images/julearn_logo_cv.png
--rw-r--r--   0 runner    (1001) docker     (127)    73031 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/images/julearn_logo_generalization.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    60581 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/images/julearn_logo_it.png
--rw-r--r--   0 runner    (1001) docker     (127)    66833 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/images/julearn_logo_ml.png
--rw-r--r--   0 runner    (1001) docker     (127)    60581 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/images/julearn_logo_mlit.png
--rw-r--r--   0 runner    (1001) docker     (127)    94858 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/images/multiple_scorers_run_cv.png
--rw-r--r--   0 runner    (1001) docker     (127)    84126 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/images/plot_scores.png
--rw-r--r--   0 runner    (1001) docker     (127)    43199 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/images/scores_run_cv.png
--rw-r--r--   0 runner    (1001) docker     (127)    83552 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/images/scores_run_cv_splitter.png
--rw-r--r--   0 runner    (1001) docker     (127)    47133 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/images/scores_run_cv_train.png
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/links.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/maintaining.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/redirect.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.123298 julearn-0.3.2.dev61/docs/selected_deeper_topics/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/selected_deeper_topics/CBPM.rst
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/selected_deeper_topics/confound_removal.rst
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/selected_deeper_topics/cross_validation_splitter.rst
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/selected_deeper_topics/hyperparameter_tuning.rst
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/selected_deeper_topics/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/selected_deeper_topics/model_inspect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/selected_deeper_topics/stacked_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/selected_deeper_topics/target_transformers.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.123298 julearn-0.3.2.dev61/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/sphinxext/gh_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.127298 julearn-0.3.2.dev61/docs/what_really_need_know/
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/what_really_need_know/cross_validation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/what_really_need_know/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/what_really_need_know/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/what_really_need_know/model_comparison.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/what_really_need_know/model_evaluation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/what_really_need_know/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/docs/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.127298 julearn-0.3.2.dev61/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.127298 julearn-0.3.2.dev61/examples/00_starting/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/00_starting/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/00_starting/plot_cm_acc_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/00_starting/plot_example_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/00_starting/plot_stratified_kfold_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/00_starting/run_combine_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/00_starting/run_grouped_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/00_starting/run_simple_binary_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.127298 julearn-0.3.2.dev61/examples/01_model_comparison/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/01_model_comparison/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/01_model_comparison/plot_simple_model_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.127298 julearn-0.3.2.dev61/examples/02_inspection/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/02_inspection/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/02_inspection/plot_groupcv_inspect_svm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/02_inspection/plot_inspect_random_forest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/02_inspection/plot_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/02_inspection/run_binary_inspect_folds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.131298 julearn-0.3.2.dev61/examples/03_complex_models/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/03_complex_models/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/03_complex_models/run_apply_to_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/03_complex_models/run_example_pca_featsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/03_complex_models/run_hyperparameter_multiple_grids.py
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/03_complex_models/run_hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/03_complex_models/run_hyperparameter_tuning_bayessearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/03_complex_models/run_stacked_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.131298 julearn-0.3.2.dev61/examples/04_confounds/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/04_confounds/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/04_confounds/plot_confound_removal_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/04_confounds/run_return_confounds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.131298 julearn-0.3.2.dev61/examples/05_customization/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/05_customization/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/05_customization/run_custom_scorers_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.131298 julearn-0.3.2.dev61/examples/99_docs/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/99_docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/99_docs/run_cbpm_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/99_docs/run_confound_removal_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/99_docs/run_cv_splitters_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/99_docs/run_data_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18320 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/99_docs/run_hyperparameters_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/99_docs/run_model_comparison_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/99_docs/run_model_evaluation_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/99_docs/run_model_inspection_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/99_docs/run_pipeline_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/99_docs/run_stacked_models_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/99_docs/run_target_transformer_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.131298 julearn-0.3.2.dev61/examples/XX_disabled/
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/XX_disabled/dis_run_n_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/examples/XX_disabled/dis_run_target_confound_removal.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/ignore_words.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.135298 julearn-0.3.2.dev61/julearn/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-29 15:28:18.000000 julearn-0.3.2.dev61/julearn/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.135298 julearn-0.3.2.dev61/julearn/base/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/base/column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    14916 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/base/estimators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.135298 julearn-0.3.2.dev61/julearn/base/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/base/tests/test_base_estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/base/tests/test_column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8766 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.135298 julearn-0.3.2.dev61/julearn/inspect/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/inspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/inspect/_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/inspect/_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/inspect/_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/inspect/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.135298 julearn-0.3.2.dev61/julearn/inspect/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/inspect/tests/test_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/inspect/tests/test_inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/inspect/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/inspect/tests/test_preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.139298 julearn-0.3.2.dev61/julearn/model_selection/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/model_selection/_skopt_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/model_selection/available_searchers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/model_selection/continuous_stratified_kfold.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/model_selection/stratified_bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.139298 julearn-0.3.2.dev61/julearn/model_selection/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/model_selection/tests/test_available_searchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/model_selection/tests/test_continous_stratified_kfold.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/model_selection/tests/test_stratified_bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.139298 julearn-0.3.2.dev61/julearn/models/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/models/available_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/models/dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.139298 julearn-0.3.2.dev61/julearn/models/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/models/tests/test_available_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/models/tests/test_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/models/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.139298 julearn-0.3.2.dev61/julearn/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/pipeline/merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    35354 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/pipeline/pipeline_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/pipeline/target_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/pipeline/target_pipeline_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.139298 julearn-0.3.2.dev61/julearn/pipeline/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/pipeline/tests/test_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    26467 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/pipeline/tests/test_pipeline_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/pipeline/tests/test_target_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/pipeline/tests/test_target_pipeline_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16207 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.139298 julearn-0.3.2.dev61/julearn/scoring/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/scoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/scoring/available_scorers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/scoring/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.143298 julearn-0.3.2.dev61/julearn/scoring/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/scoring/tests/test_available_scorers.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/scoring/tests/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.143298 julearn-0.3.2.dev61/julearn/stats/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/stats/corrected_ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.143298 julearn-0.3.2.dev61/julearn/stats/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/stats/tests/test_corrected_ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.143298 julearn-0.3.2.dev61/julearn/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    39240 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24533 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/tests/test_prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.143298 julearn-0.3.2.dev61/julearn/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/available_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/cbpm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.143298 julearn-0.3.2.dev61/julearn/transformers/dataframe/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/dataframe/change_column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/dataframe/drop_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/dataframe/filter_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/dataframe/set_column_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.143298 julearn-0.3.2.dev61/julearn/transformers/dataframe/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/dataframe/tests/test_change_column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/dataframe/tests/test_drop_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/dataframe/tests/test_filter_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/dataframe/tests/test_set_column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/ju_column_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.147298 julearn-0.3.2.dev61/julearn/transformers/target/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/target/available_target_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/target/ju_target_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/target/ju_transformed_target_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/target/target_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.147298 julearn-0.3.2.dev61/julearn/transformers/target/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/target/tests/test_available_target_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/target/tests/test_ju_target_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/target/tests/test_ju_transformed_target_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/target/tests/test_target_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.147298 julearn-0.3.2.dev61/julearn/transformers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/tests/test_available_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9852 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/tests/test_cbpm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/tests/test_confounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/transformers/tests/test_jucolumntransformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.147298 julearn-0.3.2.dev61/julearn/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/utils/_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    11247 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.147298 julearn-0.3.2.dev61/julearn/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/utils/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/utils/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/utils/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.147298 julearn-0.3.2.dev61/julearn/viz/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14647 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/viz/_scores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.147298 julearn-0.3.2.dev61/julearn/viz/res/
--rw-r--r--   0 runner    (1001) docker     (127)    73031 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/julearn/viz/res/julearn_logo_generalization.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:19.147298 julearn-0.3.2.dev61/julearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-29 15:28:19.000000 julearn-0.3.2.dev61/julearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-29 15:28:19.000000 julearn-0.3.2.dev61/julearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:28:19.000000 julearn-0.3.2.dev61/julearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-29 15:28:19.000000 julearn-0.3.2.dev61/julearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 15:28:19.000000 julearn-0.3.2.dev61/julearn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:28:19.151298 julearn-0.3.2.dev61/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-29 15:28:14.000000 julearn-0.3.2.dev61/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.611539 julearn-0.3.2.dev78/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.563539 julearn-0.3.2.dev78/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.567539 julearn-0.3.2.dev78/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/.github/ISSUE_TEMPLATE/documentation_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/.github/ISSUE_TEMPLATE/feature_request.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.571539 julearn-0.3.2.dev78/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/.github/workflows/check-stale.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/.github/workflows/ci-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/.github/workflows/docs-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-03 14:51:10.611539 julearn-0.3.2.dev78/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.571539 julearn-0.3.2.dev78/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.563539 julearn-0.3.2.dev78/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.571539 julearn-0.3.2.dev78/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.571539 julearn-0.3.2.dev78/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/_static/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.575539 julearn-0.3.2.dev78/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/_templates/function.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/_templates/function_warning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/_templates/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.575539 julearn-0.3.2.dev78/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/api/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/api/inspect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/api/main.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/api/model_selection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/api/models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/api/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/api/prepare.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/api/scoring.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/api/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/api/transformers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/api/viz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/available_pipeline_steps.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.575539 julearn-0.3.2.dev78/docs/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/changes/contributors.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.575539 julearn-0.3.2.dev78/docs/changes/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/changes/newsfragments/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/changes/newsfragments/224.misc
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/changes/newsfragments/244.misc
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/changes/newsfragments/249.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/changes/newsfragments/251.misc
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/changes/newsfragments/255.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/changes/newsfragments/260.enh
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/changes/newsfragments/260.misc
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/changes/newsfragments/262.doc
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/changes/newsfragments/262.enh
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/changes/newsfragments/262.feature
+-rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.579539 julearn-0.3.2.dev78/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    69241 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/images/corrected_ttest.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39468 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/images/final_estimator.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16172 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/images/iris_X.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51228 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/images/iris_df.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/images/iris_y.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54482 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/images/julearn_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    74874 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/images/julearn_logo_calm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78884 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/images/julearn_logo_confbias.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61311 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/images/julearn_logo_cv.png
+-rw-r--r--   0 runner    (1001) docker     (127)    73031 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/images/julearn_logo_generalization.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    60581 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/images/julearn_logo_it.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66833 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/images/julearn_logo_ml.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60581 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/images/julearn_logo_mlit.png
+-rw-r--r--   0 runner    (1001) docker     (127)    94858 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/images/multiple_scorers_run_cv.png
+-rw-r--r--   0 runner    (1001) docker     (127)    84126 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/images/plot_scores.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43199 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/images/scores_run_cv.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83552 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/images/scores_run_cv_splitter.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47133 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/images/scores_run_cv_train.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/links.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/maintaining.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/redirect.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.583539 julearn-0.3.2.dev78/docs/selected_deeper_topics/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/selected_deeper_topics/CBPM.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/selected_deeper_topics/confound_removal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/selected_deeper_topics/cross_validation_splitter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/selected_deeper_topics/hyperparameter_tuning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/selected_deeper_topics/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/selected_deeper_topics/model_inspect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/selected_deeper_topics/stacked_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/selected_deeper_topics/target_transformers.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.583539 julearn-0.3.2.dev78/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/sphinxext/gh_substitutions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.583539 julearn-0.3.2.dev78/docs/what_really_need_know/
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/what_really_need_know/cross_validation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/what_really_need_know/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/what_really_need_know/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/what_really_need_know/model_comparison.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/what_really_need_know/model_evaluation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/what_really_need_know/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/docs/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.583539 julearn-0.3.2.dev78/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.583539 julearn-0.3.2.dev78/examples/00_starting/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/00_starting/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/00_starting/plot_cm_acc_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/00_starting/plot_example_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/00_starting/plot_stratified_kfold_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/00_starting/run_combine_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/00_starting/run_grouped_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/00_starting/run_simple_binary_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.583539 julearn-0.3.2.dev78/examples/01_model_comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/01_model_comparison/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/01_model_comparison/plot_simple_model_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.587539 julearn-0.3.2.dev78/examples/02_inspection/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/02_inspection/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/02_inspection/plot_groupcv_inspect_svm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/02_inspection/plot_inspect_random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/02_inspection/plot_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/02_inspection/run_binary_inspect_folds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.587539 julearn-0.3.2.dev78/examples/03_complex_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/03_complex_models/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/03_complex_models/run_apply_to_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/03_complex_models/run_example_pca_featsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/03_complex_models/run_hyperparameter_multiple_grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/03_complex_models/run_hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/03_complex_models/run_hyperparameter_tuning_bayessearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/03_complex_models/run_stacked_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.587539 julearn-0.3.2.dev78/examples/04_confounds/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/04_confounds/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/04_confounds/plot_confound_removal_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/04_confounds/run_return_confounds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.587539 julearn-0.3.2.dev78/examples/05_customization/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/05_customization/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/05_customization/run_custom_scorers_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.591539 julearn-0.3.2.dev78/examples/99_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/99_docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/99_docs/run_cbpm_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/99_docs/run_confound_removal_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/99_docs/run_cv_splitters_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/99_docs/run_data_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23638 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/99_docs/run_hyperparameters_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/99_docs/run_model_comparison_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/99_docs/run_model_evaluation_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/99_docs/run_model_inspection_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/99_docs/run_pipeline_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/99_docs/run_stacked_models_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/99_docs/run_target_transformer_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.591539 julearn-0.3.2.dev78/examples/XX_disabled/
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/XX_disabled/dis_run_n_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/examples/XX_disabled/dis_run_target_confound_removal.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/ignore_words.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.591539 julearn-0.3.2.dev78/julearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-03 14:51:10.000000 julearn-0.3.2.dev78/julearn/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16093 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.591539 julearn-0.3.2.dev78/julearn/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/base/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14916 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/base/estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.591539 julearn-0.3.2.dev78/julearn/base/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/base/tests/test_base_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/base/tests/test_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.595539 julearn-0.3.2.dev78/julearn/inspect/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/inspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/inspect/_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/inspect/_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/inspect/_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/inspect/inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.595539 julearn-0.3.2.dev78/julearn/inspect/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/inspect/tests/test_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/inspect/tests/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/inspect/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/inspect/tests/test_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.595539 julearn-0.3.2.dev78/julearn/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/model_selection/_optuna_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/model_selection/_skopt_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/model_selection/available_searchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/model_selection/continuous_stratified_kfold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/model_selection/stratified_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.595539 julearn-0.3.2.dev78/julearn/model_selection/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/model_selection/tests/test_available_searchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/model_selection/tests/test_continous_stratified_kfold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/model_selection/tests/test_optuna_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/model_selection/tests/test_skopt_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/model_selection/tests/test_stratified_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.595539 julearn-0.3.2.dev78/julearn/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/models/available_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/models/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.595539 julearn-0.3.2.dev78/julearn/models/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/models/tests/test_available_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/models/tests/test_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/models/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.599539 julearn-0.3.2.dev78/julearn/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/pipeline/merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36758 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/pipeline/pipeline_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/pipeline/target_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/pipeline/target_pipeline_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.599539 julearn-0.3.2.dev78/julearn/pipeline/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/pipeline/tests/test_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27718 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/pipeline/tests/test_pipeline_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/pipeline/tests/test_target_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/pipeline/tests/test_target_pipeline_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16207 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.599539 julearn-0.3.2.dev78/julearn/scoring/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/scoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/scoring/available_scorers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/scoring/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.599539 julearn-0.3.2.dev78/julearn/scoring/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/scoring/tests/test_available_scorers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/scoring/tests/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.599539 julearn-0.3.2.dev78/julearn/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/stats/corrected_ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.599539 julearn-0.3.2.dev78/julearn/stats/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/stats/tests/test_corrected_ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.599539 julearn-0.3.2.dev78/julearn/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    39240 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24533 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/tests/test_prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.599539 julearn-0.3.2.dev78/julearn/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/available_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/cbpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.603539 julearn-0.3.2.dev78/julearn/transformers/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/dataframe/change_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/dataframe/drop_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/dataframe/filter_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/dataframe/set_column_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.603539 julearn-0.3.2.dev78/julearn/transformers/dataframe/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/dataframe/tests/test_change_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/dataframe/tests/test_drop_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/dataframe/tests/test_filter_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/dataframe/tests/test_set_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/ju_column_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.603539 julearn-0.3.2.dev78/julearn/transformers/target/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/target/available_target_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/target/ju_target_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/target/ju_transformed_target_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/target/target_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.603539 julearn-0.3.2.dev78/julearn/transformers/target/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/target/tests/test_available_target_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/target/tests/test_ju_target_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/target/tests/test_ju_transformed_target_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/target/tests/test_target_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.603539 julearn-0.3.2.dev78/julearn/transformers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/tests/test_available_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9852 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/tests/test_cbpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/tests/test_confounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/transformers/tests/test_jucolumntransformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.607539 julearn-0.3.2.dev78/julearn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/utils/_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11247 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.607539 julearn-0.3.2.dev78/julearn/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/utils/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/utils/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/utils/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.607539 julearn-0.3.2.dev78/julearn/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14647 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/viz/_scores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.607539 julearn-0.3.2.dev78/julearn/viz/res/
+-rw-r--r--   0 runner    (1001) docker     (127)    73031 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/julearn/viz/res/julearn_logo_generalization.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:51:10.607539 julearn-0.3.2.dev78/julearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-03 14:51:10.000000 julearn-0.3.2.dev78/julearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8742 2024-05-03 14:51:10.000000 julearn-0.3.2.dev78/julearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:51:10.000000 julearn-0.3.2.dev78/julearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-03 14:51:10.000000 julearn-0.3.2.dev78/julearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 14:51:10.000000 julearn-0.3.2.dev78/julearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 14:51:10.611539 julearn-0.3.2.dev78/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-03 14:51:06.000000 julearn-0.3.2.dev78/tox.ini
```

### Comparing `julearn-0.3.2.dev61/.github/ISSUE_TEMPLATE/bug_report.yaml` & `julearn-0.3.2.dev78/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/.github/ISSUE_TEMPLATE/documentation_request.yaml` & `julearn-0.3.2.dev78/.github/ISSUE_TEMPLATE/documentation_request.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/.github/ISSUE_TEMPLATE/feature_request.yaml` & `julearn-0.3.2.dev78/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/.github/workflows/ci-docs.yml` & `julearn-0.3.2.dev78/.github/workflows/ci-docs.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/.github/workflows/ci.yml` & `julearn-0.3.2.dev78/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/.github/workflows/docs-preview.yml` & `julearn-0.3.2.dev78/.github/workflows/docs-preview.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/.github/workflows/docs.yml` & `julearn-0.3.2.dev78/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/.github/workflows/lint.yml` & `julearn-0.3.2.dev78/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/.github/workflows/pypi.yml` & `julearn-0.3.2.dev78/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/.gitignore` & `julearn-0.3.2.dev78/.gitignore`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/.pre-commit-config.yaml` & `julearn-0.3.2.dev78/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/LICENSE.md` & `julearn-0.3.2.dev78/LICENSE.md`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/PKG-INFO` & `julearn-0.3.2.dev78/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: julearn
-Version: 0.3.2.dev61
+Version: 0.3.2.dev78
 Summary: Juelich Machine Learning Library
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Sami Hamdan <s.hamdan@fz-juelich.de>
 Maintainer-email: Sami Hamdan <s.hamdan@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/julearn
 Project-URL: documentation, https://juaml.github.io/julearn
 Project-URL: repository, https://github.com/juaml/julearn
@@ -37,24 +37,29 @@
 Requires-Dist: sphinx<7.3,>=5.3.0; extra == "docs"
 Requires-Dist: sphinx-gallery<0.15,>=0.13.0; extra == "docs"
 Requires-Dist: furo<2024.0.0,>=2022.9.29; extra == "docs"
 Requires-Dist: sphinx_copybutton<0.6,>=0.5.0; extra == "docs"
 Requires-Dist: numpydoc<1.6,>=1.5.0; extra == "docs"
 Requires-Dist: towncrier<24; extra == "docs"
 Requires-Dist: scikit-optimize<0.11,>=0.10.0; extra == "docs"
+Requires-Dist: optuna<3.7,>=3.6.0; extra == "docs"
+Requires-Dist: optuna_integration<3.7,>=3.6.0; extra == "docs"
 Provides-Extra: deslib
 Requires-Dist: deslib<0.4,>=0.3.5; extra == "deslib"
 Provides-Extra: viz
 Requires-Dist: panel>=1.3.0; extra == "viz"
 Requires-Dist: bokeh>=3.0.0; extra == "viz"
 Requires-Dist: param>=2.0.0; extra == "viz"
 Provides-Extra: skopt
 Requires-Dist: scikit-optimize<0.11,>=0.10.0; extra == "skopt"
+Provides-Extra: optuna
+Requires-Dist: optuna<3.7,>=3.6.0; extra == "optuna"
+Requires-Dist: optuna_integration<3.7,>=3.6.0; extra == "optuna"
 Provides-Extra: all
-Requires-Dist: julearn[skopt,viz]; extra == "all"
+Requires-Dist: julearn[optuna,skopt,viz]; extra == "all"
 
 # julearn
 
 ![PyPI](https://img.shields.io/pypi/v/julearn?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/julearn?style=flat-square)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/julearn?style=flat-square)
 ![GitHub](https://img.shields.io/github/license/juaml/julearn?style=flat-square)
```

### Comparing `julearn-0.3.2.dev61/README.md` & `julearn-0.3.2.dev78/README.md`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/codecov.yml` & `julearn-0.3.2.dev78/codecov.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/Makefile` & `julearn-0.3.2.dev78/docs/Makefile`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/_templates/class.rst` & `julearn-0.3.2.dev78/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/_templates/function_warning.rst` & `julearn-0.3.2.dev78/docs/_templates/function_warning.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/_templates/versions.html` & `julearn-0.3.2.dev78/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/api/base.rst` & `julearn-0.3.2.dev78/docs/api/base.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/api/model_selection.rst` & `julearn-0.3.2.dev78/docs/api/model_selection.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/api/models.rst` & `julearn-0.3.2.dev78/docs/api/models.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/api/scoring.rst` & `julearn-0.3.2.dev78/docs/api/scoring.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/api/transformers.rst` & `julearn-0.3.2.dev78/docs/api/transformers.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/api/utils.rst` & `julearn-0.3.2.dev78/docs/api/utils.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/api/viz.rst` & `julearn-0.3.2.dev78/docs/api/viz.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/available_pipeline_steps.rst` & `julearn-0.3.2.dev78/docs/available_pipeline_steps.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/conf.py` & `julearn-0.3.2.dev78/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -157,14 +157,19 @@
     "nibabel": ("https://nipy.org/nibabel/", None),
     "numpy": ("https://numpy.org/doc/stable/", None),
     "pandas": ("https://pandas.pydata.org/pandas-docs/dev", None),
     # "sqlalchemy": ("https://docs.sqlalchemy.org/en/20/", None),
     "joblib": ("https://joblib.readthedocs.io/en/latest/", None),
     "scipy": ("https://docs.scipy.org/doc/scipy/", None),
     "skopt": ("https://scikit-optimize.readthedocs.io/en/latest", None),
+    "optuna": ("https://optuna.readthedocs.io/en/stable", None),
+    "optuna_integration": (
+        "https://optuna-integration.readthedocs.io/en/stable",
+        None,
+    ),
 }
 
 
 # -- numpydoc configuration --------------------------------------------------
 
 numpydoc_show_class_members = False
 numpydoc_xref_param_type = False
```

### Comparing `julearn-0.3.2.dev61/docs/configuration.rst` & `julearn-0.3.2.dev78/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/contributing.rst` & `julearn-0.3.2.dev78/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/examples.rst` & `julearn-0.3.2.dev78/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/faq.rst` & `julearn-0.3.2.dev78/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/getting_started.rst` & `julearn-0.3.2.dev78/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/images/corrected_ttest.png` & `julearn-0.3.2.dev78/docs/images/corrected_ttest.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/images/final_estimator.png` & `julearn-0.3.2.dev78/docs/images/final_estimator.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/images/iris_X.png` & `julearn-0.3.2.dev78/docs/images/iris_X.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/images/iris_df.png` & `julearn-0.3.2.dev78/docs/images/iris_df.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/images/iris_y.png` & `julearn-0.3.2.dev78/docs/images/iris_y.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/images/julearn_logo.png` & `julearn-0.3.2.dev78/docs/images/julearn_logo.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/images/julearn_logo_calm.png` & `julearn-0.3.2.dev78/docs/images/julearn_logo_calm.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/images/julearn_logo_confbias.png` & `julearn-0.3.2.dev78/docs/images/julearn_logo_confbias.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/images/julearn_logo_cv.png` & `julearn-0.3.2.dev78/docs/images/julearn_logo_cv.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/images/julearn_logo_generalization.png` & `julearn-0.3.2.dev78/docs/images/julearn_logo_generalization.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/images/julearn_logo_it.png` & `julearn-0.3.2.dev78/docs/images/julearn_logo_it.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/images/julearn_logo_ml.png` & `julearn-0.3.2.dev78/docs/images/julearn_logo_ml.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/images/julearn_logo_mlit.png` & `julearn-0.3.2.dev78/docs/images/julearn_logo_mlit.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/images/multiple_scorers_run_cv.png` & `julearn-0.3.2.dev78/docs/images/multiple_scorers_run_cv.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/images/plot_scores.png` & `julearn-0.3.2.dev78/docs/images/plot_scores.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/images/scores_run_cv.png` & `julearn-0.3.2.dev78/docs/images/scores_run_cv.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/images/scores_run_cv_splitter.png` & `julearn-0.3.2.dev78/docs/images/scores_run_cv_splitter.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/images/scores_run_cv_train.png` & `julearn-0.3.2.dev78/docs/images/scores_run_cv_train.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/index.rst` & `julearn-0.3.2.dev78/docs/index.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/links.inc` & `julearn-0.3.2.dev78/docs/links.inc`

 * *Files 2% similar despite different names*

```diff
@@ -37,7 +37,8 @@
 
 .. _`sphinx gallery`: https://sphinx-gallery.github.io/stable/index.html
 .. _`sphinx RST reference`: https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#inline-markup
 
 
 .. _`DESlib`: https://github.com/scikit-learn-contrib/DESlib
 .. _`scikit-optimize`: https://scikit-optimize.readthedocs.io/en/stable/
+.. _`Optuna`: https://optuna.org
```

### Comparing `julearn-0.3.2.dev61/docs/maintaining.rst` & `julearn-0.3.2.dev78/docs/maintaining.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/sphinxext/gh_substitutions.py` & `julearn-0.3.2.dev78/docs/sphinxext/gh_substitutions.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/what_really_need_know/cross_validation.rst` & `julearn-0.3.2.dev78/docs/what_really_need_know/cross_validation.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/what_really_need_know/index.rst` & `julearn-0.3.2.dev78/docs/what_really_need_know/index.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/docs/whats_new.rst` & `julearn-0.3.2.dev78/docs/whats_new.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/00_starting/plot_cm_acc_multiclass.py` & `julearn-0.3.2.dev78/examples/00_starting/plot_cm_acc_multiclass.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/00_starting/plot_example_regression.py` & `julearn-0.3.2.dev78/examples/00_starting/plot_example_regression.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/00_starting/plot_stratified_kfold_reg.py` & `julearn-0.3.2.dev78/examples/00_starting/plot_stratified_kfold_reg.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/00_starting/run_combine_pandas.py` & `julearn-0.3.2.dev78/examples/00_starting/run_combine_pandas.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/00_starting/run_grouped_cv.py` & `julearn-0.3.2.dev78/examples/00_starting/run_grouped_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/00_starting/run_simple_binary_classification.py` & `julearn-0.3.2.dev78/examples/00_starting/run_simple_binary_classification.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/01_model_comparison/plot_simple_model_comparison.py` & `julearn-0.3.2.dev78/examples/01_model_comparison/plot_simple_model_comparison.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/02_inspection/plot_groupcv_inspect_svm.py` & `julearn-0.3.2.dev78/examples/02_inspection/plot_groupcv_inspect_svm.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/02_inspection/plot_inspect_random_forest.py` & `julearn-0.3.2.dev78/examples/02_inspection/plot_inspect_random_forest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/02_inspection/plot_preprocess.py` & `julearn-0.3.2.dev78/examples/02_inspection/plot_preprocess.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/02_inspection/run_binary_inspect_folds.py` & `julearn-0.3.2.dev78/examples/02_inspection/run_binary_inspect_folds.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/03_complex_models/run_apply_to_target.py` & `julearn-0.3.2.dev78/examples/03_complex_models/run_apply_to_target.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/03_complex_models/run_example_pca_featsets.py` & `julearn-0.3.2.dev78/examples/03_complex_models/run_example_pca_featsets.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/03_complex_models/run_hyperparameter_multiple_grids.py` & `julearn-0.3.2.dev78/examples/03_complex_models/run_hyperparameter_multiple_grids.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/03_complex_models/run_hyperparameter_tuning.py` & `julearn-0.3.2.dev78/examples/03_complex_models/run_hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/03_complex_models/run_hyperparameter_tuning_bayessearch.py` & `julearn-0.3.2.dev78/examples/03_complex_models/run_hyperparameter_tuning_bayessearch.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/03_complex_models/run_stacked_models.py` & `julearn-0.3.2.dev78/examples/03_complex_models/run_stacked_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/04_confounds/plot_confound_removal_classification.py` & `julearn-0.3.2.dev78/examples/04_confounds/plot_confound_removal_classification.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/04_confounds/run_return_confounds.py` & `julearn-0.3.2.dev78/examples/04_confounds/run_return_confounds.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/05_customization/run_custom_scorers_regression.py` & `julearn-0.3.2.dev78/examples/05_customization/run_custom_scorers_regression.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/99_docs/run_cbpm_docs.py` & `julearn-0.3.2.dev78/examples/99_docs/run_cbpm_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/99_docs/run_confound_removal_docs.py` & `julearn-0.3.2.dev78/examples/99_docs/run_confound_removal_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/99_docs/run_cv_splitters_docs.py` & `julearn-0.3.2.dev78/examples/99_docs/run_cv_splitters_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/99_docs/run_data_docs.py` & `julearn-0.3.2.dev78/examples/99_docs/run_data_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/99_docs/run_hyperparameters_docs.py` & `julearn-0.3.2.dev78/examples/99_docs/run_hyperparameters_docs.py`

 * *Files 18% similar despite different names*

```diff
@@ -249,16 +249,17 @@
 # the _grid_ of hyperparameters to try. As we see above, we have 3
 # hyperparameters to tune. So it constructs a 3-dimentional grid with all the
 # possible combinations of the hyperparameters values. The second step is to
 # perform cross-validation on each of the possible combinations of
 # hyperparameters values.
 #
 # Other searchers that ``julearn`` provides are the
-# :class:`~sklearn.model_selection.RandomizedSearchCV` and
-# :class:`~skopt.BayesSearchCV`.
+# :class:`~sklearn.model_selection.RandomizedSearchCV`, 
+# :class:`~skopt.BayesSearchCV` and
+# :class:`~optuna_integration.sklearn.OptunaSearchCV`.
 #
 # The randomized searcher
 # (:class:`~sklearn.model_selection.RandomizedSearchCV`) is similar to the
 # :class:`~sklearn.model_selection.GridSearchCV`, but instead
 # of trying all the possible combinations of hyperparameter values, it tries
 # a random subset of them. This is useful when we have a lot of hyperparameters
 # to tune, since it can be very time consuming to try all the possible
@@ -270,14 +271,20 @@
 # complex. It uses Bayesian optimization to find the best hyperparameter set.
 # As with the randomized search, it is useful when we have many
 # hyperparameters to tune, and we don't want to try all the possible
 # combinations due to computational constraints. For more information, see the
 # :class:`~skopt.BayesSearchCV` documentation, including how to specify
 # the prior distributions of the hyperparameters.
 #
+# The Optuna searcher (:class:`~optuna_integration.sklearn.OptunaSearchCV`)
+# uses the Optuna library to find the best hyperparameter set. Optuna is a
+# hyperparameter optimization framework that has several algorithms to find
+# the best hyperparameter set. For more information, see the
+# `Optuna`_ documentation.
+#
 # We can specify the kind of searcher and its parametrization, by setting the
 # ``search_params`` parameter in the :func:`.run_cross_validation` function.
 # For example, we can use the
 # :class:`~sklearn.model_selection.RandomizedSearchCV` searcher with
 # 10 iterations of random search.
 
 search_params = {
@@ -365,14 +372,148 @@
 
 print(
     "Scores with best hyperparameter using 10 iterations of "
     f"bayesian search and 3-fold CV: {scores_tuned['test_score'].mean()}"
 )
 pprint(model_tuned.best_params_)
 
+###############################################################################
+# An example using optuna searcher is shown below. The searcher is specified
+# as ``"optuna"`` and the hyperparameters are specified as a dictionary with
+# the hyperparameters to tune and their distributions as for the bayesian
+# searcher. However, the optuna searcher behaviour is controlled by a
+# :class:`~optuna.study.Study` object. This object can be passed to the
+# searcher using the ``study`` parameter in the ``search_params`` dictionary.
+# 
+# .. important::
+#    The optuna searcher requires that all the hyperparameters are specified
+#    as distributions, even the categorical ones. 
+#
+# We first modify the pipeline creator so the ``select_k`` parameter is
+# specified as a distribution. We exemplarily use a categorical distribution
+# for the ``class_weight`` hyperparameter, trying the ``"balanced"`` and 
+# ``None`` values.
+
+creator = PipelineCreator(problem_type="classification")
+creator.add("zscore")
+creator.add("select_k", k=(2, 4, "uniform"))
+creator.add(
+    "svm",
+    C=(0.01, 10, "log-uniform"),
+    gamma=(1e-3, 1e-1, "log-uniform"),
+    class_weight=("balanced", None, "categorical")
+)
+print(creator)
+
+###############################################################################
+# We can now use the optuna searcher with 10 trials and 3-fold cross-validation.
+
+import optuna
+
+study = optuna.create_study(
+    direction="maximize",
+    study_name="optuna-concept",
+    load_if_exists=True,
+)
+
+search_params = {
+    "kind": "optuna",
+    "study": study,
+    "cv": 3,
+}
+scores_tuned, model_tuned = run_cross_validation(
+    X=X,
+    y=y,
+    data=df,
+    X_types=X_types,
+    model=creator,
+    return_estimator="all",
+    search_params=search_params,
+)
+
+print(
+    "Scores with best hyperparameter using 10 iterations of "
+    f"optuna and 3-fold CV: {scores_tuned['test_score'].mean()}"
+)
+pprint(model_tuned.best_params_)
+
+###############################################################################
+#
+# Specifying distributions
+# ~~~~~~~~~~~~~~~~~~~~~~~~
+#
+# The hyperparameters can be specified as distributions for the randomized
+# searcher, bayesian searcher and optuna searcher. The distributions are
+# either specified toolbox-specific method or  a tuple convention with the
+# following format: ``(low, high, distribution)`` where the distribution can
+# be either ``"log-uniform"`` or ``"uniform"`` or 
+# ``(a, b, c, d, ..., "categorical")`` where ``a``, ``b``, ``c``, ``d``, etc.
+# are the possible categorical values for the hyperparameter.
+#
+# For example, we can specify the ``C`` and ``gamma`` hyperparameters of the 
+# :class:`~sklearn.svm.SVC` as  log-uniform distributions, while keeping 
+# the ``with_mean`` parameter of the
+# :class:`~sklearn.preprocessing.StandardScaler` as a categorical parameter
+# with two options.
+
+
+creator = PipelineCreator(problem_type="classification")
+creator.add("zscore", with_mean=(True, False, "categorical"))
+creator.add(
+    "svm",
+    C=(0.01, 10, "log-uniform"),
+    gamma=(1e-3, 1e-1, "log-uniform"),
+)
+print(creator)
+
+###############################################################################
+# While this will work for any of the ``random``, ``bayes`` or ``optuna``
+# searcher options, it is important to note that both ``bayes`` and ``optuna``
+# searchers accept further parameters to specify distributions. For example,
+# the ``bayes`` searcher distributions are defined using the 
+# :class:`~skopt.space.space.Categorical`, :class:`~skopt.space.space.Integer`
+# and :class:`~skopt.space.space.Real`.
+#
+# For example, we can define a log-uniform distribution with base 2 for the
+# ``C`` hyperparameter of the :class:`~sklearn.svm.SVC` model:
+from skopt.space import Real
+creator = PipelineCreator(problem_type="classification")
+creator.add("zscore", with_mean=(True, False, "categorical"))
+creator.add(
+    "svm",
+    C=Real(0.01, 10, prior="log-uniform", base=2),
+    gamma=(1e-3, 1e-1, "log-uniform"),
+)
+print(creator)
+
+###############################################################################
+# For the optuna searcher, the distributions are defined using the
+# :class:`~optuna.distributions.CategoricalDistribution`,
+# :class:`~optuna.distributions.FloatDistribution` and
+# :class:`~optuna.distributions.IntDistribution`.
+#
+#
+# For example, we can define a uniform distribution from 0.5 to 0.9 with a 0.05
+# step for the ``n_components`` of a :class:`~sklearn.decomposition.PCA` 
+# transformer, while keeping a log-uniform distribution for the ``C`` and
+# ``gamma`` hyperparameters of the :class:`~sklearn.svm.SVC` model.
+from optuna.distributions import FloatDistribution
+creator = PipelineCreator(problem_type="classification")
+creator.add("zscore")
+creator.add(
+    "pca",
+    n_components=FloatDistribution(0.5, 0.9, step=0.05),
+)
+creator.add(
+    "svm",
+    C=FloatDistribution(0.01, 10, log=True),
+    gamma=(1e-3, 1e-1, "log-uniform"),
+)
+print(creator)
+
 
 ###############################################################################
 #
 # Tuning more than one *grid*
 # ---------------------------
 #
 # Following our tuning of the :class:`~sklearn.svm.SVC` hyperparameters, we
```

### Comparing `julearn-0.3.2.dev61/examples/99_docs/run_model_comparison_docs.py` & `julearn-0.3.2.dev78/examples/99_docs/run_model_comparison_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/99_docs/run_model_evaluation_docs.py` & `julearn-0.3.2.dev78/examples/99_docs/run_model_evaluation_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/99_docs/run_model_inspection_docs.py` & `julearn-0.3.2.dev78/examples/99_docs/run_model_inspection_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/99_docs/run_pipeline_docs.py` & `julearn-0.3.2.dev78/examples/99_docs/run_pipeline_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/99_docs/run_stacked_models_docs.py` & `julearn-0.3.2.dev78/examples/99_docs/run_stacked_models_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/99_docs/run_target_transformer_docs.py` & `julearn-0.3.2.dev78/examples/99_docs/run_target_transformer_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/XX_disabled/dis_run_n_jobs.py` & `julearn-0.3.2.dev78/examples/XX_disabled/dis_run_n_jobs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/examples/XX_disabled/dis_run_target_confound_removal.py` & `julearn-0.3.2.dev78/examples/XX_disabled/dis_run_target_confound_removal.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/api.py` & `julearn-0.3.2.dev78/julearn/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,17 +131,26 @@
           is provided for at least one hyperparameter, a search will be
           performed.
 
     search_params : dict | None
         Additional parameters in case Hyperparameter Tuning is performed, with
         the following keys:
 
-        * 'kind': The kind of search algorithm to use, e.g.:
-            'grid', 'random' or 'bayes'. Can be any valid julearn searcher name
-            or scikit-learn compatible searcher.
+        * 'kind': The kind of search algorithm to use, Valid options are:
+
+          * ``"grid"`` : :class:`~sklearn.model_selection.GridSearchCV`
+          * ``"random"`` :
+            :class:`~sklearn.model_selection.RandomizedSearchCV`
+          * ``"bayes"`` : :class:`~skopt.BayesSearchCV`
+          * ``"optuna"`` :
+            :class:`~optuna_integration.sklearn.OptunaSearchCV`
+          * user-registered searcher name : see
+            :func:`~julearn.model_selection.register_searcher`
+          * ``scikit-learn``-compatible searcher
+
         * 'cv': If a searcher is going to be used, the cross-validation
             splitting strategy to use. Defaults to same CV as for the model
             evaluation.
         * 'scoring': If a searcher is going to be used, the scoring metric to
             evaluate the performance.
 
         See :ref:`hp_tuning` for details.
```

### Comparing `julearn-0.3.2.dev61/julearn/base/column_types.py` & `julearn-0.3.2.dev78/julearn/base/column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/base/estimators.py` & `julearn-0.3.2.dev78/julearn/base/estimators.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/base/tests/test_base_estimators.py` & `julearn-0.3.2.dev78/julearn/base/tests/test_base_estimators.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/base/tests/test_column_types.py` & `julearn-0.3.2.dev78/julearn/base/tests/test_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/config.py` & `julearn-0.3.2.dev78/julearn/config.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/conftest.py` & `julearn-0.3.2.dev78/julearn/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,15 +266,15 @@
     params=[
         {"kind": "bayes", "n_iter": 2, "cv": 3},
         {"kind": "bayes", "n_iter": 2},
     ],
     scope="function",
 )
 def bayes_search_params(request: FixtureRequest) -> Optional[Dict]:
-    """Return different  search_params argument for BayesSearchCV.
+    """Return different search_params argument for BayesSearchCV.
 
     Parameters
     ----------
     request : pytest.FixtureRequest
         The request object.
 
     Returns
@@ -282,14 +282,37 @@
     dict or None
         A dictionary with the search_params argument.
 
     """
 
     return request.param
 
+@fixture(
+    params=[
+        {"kind": "optuna", "n_trials": 10, "cv": 3},
+        {"kind": "optuna", "timeout": 20},
+    ],
+    scope="function",
+)
+def optuna_search_params(request: FixtureRequest) -> Optional[Dict]:
+    """Return different search_params argument for OptunaSearchCV.
+
+    Parameters
+    ----------
+    request : pytest.FixtureRequest
+        The request object.
+
+    Returns
+    -------
+    dict or None
+        A dictionary with the search_params argument.
+
+    """
+
+    return request.param
 
 _tuning_params = {
     "zscore": {"with_mean": [True, False]},
     "pca": {"n_components": [0.2, 0.7]},
     "select_univariate": {"mode": ["k_best", "percentile"]},
     "rf": {"n_estimators": [2, 5]},
     "svm": {"C": [1, 2]},
```

### Comparing `julearn-0.3.2.dev61/julearn/inspect/_cv.py` & `julearn-0.3.2.dev78/julearn/inspect/_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/inspect/_pipeline.py` & `julearn-0.3.2.dev78/julearn/inspect/_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/inspect/_preprocess.py` & `julearn-0.3.2.dev78/julearn/inspect/_preprocess.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/inspect/inspector.py` & `julearn-0.3.2.dev78/julearn/inspect/inspector.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/inspect/tests/test_cv.py` & `julearn-0.3.2.dev78/julearn/inspect/tests/test_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/inspect/tests/test_inspector.py` & `julearn-0.3.2.dev78/julearn/inspect/tests/test_inspector.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/inspect/tests/test_pipeline.py` & `julearn-0.3.2.dev78/julearn/inspect/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/inspect/tests/test_preprocess.py` & `julearn-0.3.2.dev78/julearn/inspect/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/model_selection/available_searchers.py` & `julearn-0.3.2.dev78/julearn/model_selection/available_searchers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/model_selection/continuous_stratified_kfold.py` & `julearn-0.3.2.dev78/julearn/model_selection/continuous_stratified_kfold.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/model_selection/stratified_bootstrap.py` & `julearn-0.3.2.dev78/julearn/model_selection/stratified_bootstrap.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/model_selection/tests/test_available_searchers.py` & `julearn-0.3.2.dev78/julearn/model_selection/tests/test_available_searchers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Provides tests for the available searchers."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Sami Hamdan <s.hamdan@fz-juelich.de>
 # License: AGPL
 
 import pytest
-from sklearn.model_selection import GridSearchCV, RandomizedSearchCV
+from sklearn.model_selection import GridSearchCV
 
 from julearn.model_selection import (
     get_searcher,
     register_searcher,
     reset_searcher_register,
 )
 from julearn.model_selection.available_searchers import (
@@ -47,37 +47,69 @@
     register_searcher("custom_grid", GridSearchCV, "param_grid")
     get_searcher("custom_grid")
     reset_searcher_register()
     with pytest.raises(ValueError, match="The specified searcher "):
         get_searcher("custom_grid")
 
 
-def test_get_searcher() -> None:
-    """Test getting a searcher."""
-    out = get_searcher("grid")
-    assert out == GridSearchCV
-
-    out = get_searcher("random")
-    assert out == RandomizedSearchCV
-
-    out = get_searcher("bayes")
-    assert out.__name__ == "BayesSearchCV"
-
-
-def test_get_searcher_params_attr() -> None:
-    """Test getting the params attribute of a searcher."""
-    out = get_searcher_params_attr("grid")
-    assert out == "param_grid"
+@pytest.mark.parametrize(
+    "searcher,expected",
+    [
+        ("grid", "GridSearchCV"),
+        ("random", "RandomizedSearchCV"),
+        ("bayes", "BayesSearchCV"),
+        ("optuna", "OptunaSearchCV"),
+    ],
+)
+def test_get_searcher(searcher: str, expected: str) -> None:
+    """Test getting a searcher.
 
-    out = get_searcher_params_attr("random")
-    assert out == "param_distributions"
+    Parameters
+    ----------
+    searcher : str
+        The searcher name.
+    expected : str
+        The expected searcher class name.
+
+    """
+    out = get_searcher(searcher)
+    assert out.__name__ == expected
+
+
+@pytest.mark.parametrize(
+    "searcher,expected",
+    [
+        ("grid", "param_grid"),
+        ("random", "param_distributions"),
+        ("bayes", "search_spaces"),
+        ("optuna", "param_distributions"),
+    ],
+)
+def test_get_searcher_params_attr(searcher: str, expected: str) -> None:
+    """Test getting the params attribute of a searcher.
 
-    out = get_searcher_params_attr("bayes")
-    assert out == "search_spaces"
+    Parameters
+    ----------
+    searcher : str
+        The searcher name.
+    expected : str
+        The expected attribute name.
+
+    """
+    out = get_searcher_params_attr(searcher)
+    assert out == expected
 
 
 @pytest.mark.nodeps
 def test_get_searchers_noskopt() -> None:
     """Test getting a searcher without skopt."""
     out = get_searcher("bayes")
     with pytest.raises(ImportError, match="BayesSearchCV requires"):
         out()  # type: ignore
+
+
+@pytest.mark.nodeps
+def test_get_searchers_nooptuna() -> None:
+    """Test getting a searcher without optuna."""
+    out = get_searcher("optuna")
+    with pytest.raises(ImportError, match="OptunaSearchCV requires"):
+        out()  # type: ignore
```

### Comparing `julearn-0.3.2.dev61/julearn/model_selection/tests/test_continous_stratified_kfold.py` & `julearn-0.3.2.dev78/julearn/model_selection/tests/test_continous_stratified_kfold.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/model_selection/tests/test_stratified_bootstrap.py` & `julearn-0.3.2.dev78/julearn/model_selection/tests/test_stratified_bootstrap.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/models/available_models.py` & `julearn-0.3.2.dev78/julearn/models/available_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/models/dynamic.py` & `julearn-0.3.2.dev78/julearn/models/dynamic.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/models/tests/test_available_models.py` & `julearn-0.3.2.dev78/julearn/models/tests/test_available_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/models/tests/test_dynamic.py` & `julearn-0.3.2.dev78/julearn/models/tests/test_dynamic.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/models/tests/test_models.py` & `julearn-0.3.2.dev78/julearn/models/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/pipeline/merger.py` & `julearn-0.3.2.dev78/julearn/pipeline/merger.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/pipeline/pipeline_creator.py` & `julearn-0.3.2.dev78/julearn/pipeline/pipeline_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 
 import numpy as np
 from scipy import stats
 from sklearn.model_selection import RandomizedSearchCV, check_cv
 from sklearn.pipeline import Pipeline
 
 from ..base import ColumnTypes, ColumnTypesLike, JuTransformer, WrapModel
+from ..model_selection._optuna_searcher import (
+    _prepare_optuna_hyperparameters_distributions,
+)
+from ..model_selection._skopt_searcher import (
+    _prepare_skopt_hyperparameters_distributions,
+)
 from ..model_selection.available_searchers import get_searcher, list_searchers
 from ..models import get_model, list_models
 from ..prepare import prepare_search_params
 from ..transformers import (
     JuColumnTransformer,
     SetColumnTypes,
     get_transformer,
@@ -894,15 +900,15 @@
 
     """
     mod_params_to_tune = {}
     for k, v in params_to_tune.items():
         if isinstance(v, tuple) and len(v) == 3:
             if v[2] == "uniform":
                 mod_params_to_tune[k] = stats.uniform(v[0], v[1])
-            elif v[2] in ("loguniform", "log-uniform"):
+            elif v[2] == "log-uniform":
                 mod_params_to_tune[k] = stats.loguniform(v[0], v[1])
             else:
                 mod_params_to_tune[k] = v
         else:
             mod_params_to_tune[k] = v
     return mod_params_to_tune
 
@@ -923,17 +929,26 @@
         'svm__probability': True will set the parameter 'probability' of
         the 'svm' step. The value of the parameter must be a list of
         values to test.
 
     search_params : dict
         The parameters for the search. The following keys are accepted:
 
-        * 'kind': The kind of search algorithm to use e.g.:
-            'grid', 'random' or 'bayes'. All valid julearn searchers can be
-            entered.
+        * 'kind': The kind of search algorithm to use. Valid options are:
+
+          * ``"grid"`` : :class:`~sklearn.model_selection.GridSearchCV`
+          * ``"random"`` :
+            :class:`~sklearn.model_selection.RandomizedSearchCV`
+          * ``"bayes"`` : :class:`~skopt.BayesSearchCV`
+          * ``"optuna"`` :
+            :class:`~optuna_integration.sklearn.OptunaSearchCV`
+          * user-registered searcher name : see
+            :func:`~julearn.model_selection.register_searcher`
+          * ``scikit-learn``-compatible searcher
+
         * 'cv': If search is going to be used, the cross-validation
             splitting strategy to use. Defaults to same CV as for the model
             evaluation.
         * 'scoring': If search is going to be used, the scoring metric to
             evaluate the performance.
 
     pipeline : sklearn.pipeline.Pipeline
@@ -991,15 +1006,34 @@
                     params_to_tune
                 )
             else:
                 params_to_tune = [
                     _prepare_hyperparameters_distributions(p)
                     for p in params_to_tune
                 ]
-
+        elif search.__name__ == "BayesSearchCV":
+            if isinstance(params_to_tune, dict):
+                params_to_tune = _prepare_skopt_hyperparameters_distributions(
+                    params_to_tune
+                )
+            else:
+                params_to_tune = [
+                    _prepare_skopt_hyperparameters_distributions(p)
+                    for p in params_to_tune
+                ]
+        elif search.__name__ == "OptunaSearchCV":
+            if isinstance(params_to_tune, dict):
+                params_to_tune = _prepare_optuna_hyperparameters_distributions(
+                    params_to_tune
+                )
+            else:
+                params_to_tune = [
+                    _prepare_optuna_hyperparameters_distributions(p)
+                    for p in params_to_tune
+                ]
         cv_inner = check_cv(cv_inner)  # type: ignore
         logger.info(f"Using inner CV scheme {cv_inner}")
         search_params["cv"] = cv_inner
         logger.info("Search Parameters:")
         for k, v in search_params.items():
             logger.info(f"\t{k}: {v}")
```

### Comparing `julearn-0.3.2.dev61/julearn/pipeline/target_pipeline.py` & `julearn-0.3.2.dev78/julearn/pipeline/target_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/pipeline/target_pipeline_creator.py` & `julearn-0.3.2.dev78/julearn/pipeline/target_pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/pipeline/tests/test_merger.py` & `julearn-0.3.2.dev78/julearn/pipeline/tests/test_merger.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/pipeline/tests/test_pipeline_creator.py` & `julearn-0.3.2.dev78/julearn/pipeline/tests/test_pipeline_creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
     X_types_iris: Dict[str, List[str]],  # noqa: N803
     model: str,
     preprocess: Union[str, List[str]],
     problem_type: str,
     get_tuning_params: Callable,
     bayes_search_params: Dict[str, List],
 ) -> None:
-    """Test that the pipeline hyperparameter tuning works as expected.
+    """Test that the pipeline hyperparameter tuning (bayes) works as expected.
 
     Parameters
     ----------
     X_types_iris : dict
         The iris dataset features types.
     model : str
         The model to test.
@@ -255,14 +255,55 @@
         get_tuning_params,
         bayes_search_params,
     )
     assert isinstance(pipeline, BayesSearchCV)
     assert pipeline.search_spaces == param_grid  # type: ignore
 
 
+def test_hyperparameter_tuning_optuna(
+    X_types_iris: Dict[str, List[str]],  # noqa: N803
+    model: str,
+    preprocess: Union[str, List[str]],
+    problem_type: str,
+    get_tuning_params: Callable,
+    optuna_search_params: Dict[str, List],
+) -> None:
+    """Test that the pipeline hyperparameter tuning (optuna) works as expected.
+
+    Parameters
+    ----------
+    X_types_iris : dict
+        The iris dataset features types.
+    model : str
+        The model to test.
+    preprocess : str or list of str
+        The preprocessing steps to test.
+    problem_type : str
+        The problem type to test.
+    get_tuning_params : Callable
+        A function that returns the tuning hyperparameters for a given step.
+    optuna_search_params : dict of str and list
+        The parameters for the search.
+
+    """
+    optuna_integration = pytest.importorskip("optuna_integration")
+    OptunaSearchCV = optuna_integration.OptunaSearchCV
+
+    pipeline, param_grid = _hyperparam_tuning_base_test(
+        X_types_iris,
+        model,
+        preprocess,
+        problem_type,
+        get_tuning_params,
+        optuna_search_params,
+    )
+    assert isinstance(pipeline, OptunaSearchCV)
+    assert pipeline.param_distributions == param_grid  # type: ignore
+
+
 def _compare_param_grids(a: Dict, b: Dict) -> None:
     """Compare two param grids.
 
     Parameters
     ----------
     a : dict
         The first param grid (processed).
@@ -276,15 +317,15 @@
 
     """
     for key, val in a.items():
         assert key in b
         if hasattr(val, "rvs"):
             assert val.args[0] == b[key][0]
             assert val.args[1] == b[key][1]
-            if b[key][2] in ["log-uniform", "loguniform"]:
+            if b[key][2] == "log-uniform":
                 assert val.dist.name == "loguniform"
             elif b[key][2] == "uniform":
                 assert val.dist.name == "uniform"
             else:
                 pytest.fail(
                     f"Unknown distributions {val.dist.name} or {b[key][2]}"
                 )
```

### Comparing `julearn-0.3.2.dev61/julearn/pipeline/tests/test_target_pipeline.py` & `julearn-0.3.2.dev78/julearn/pipeline/tests/test_target_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/pipeline/tests/test_target_pipeline_creator.py` & `julearn-0.3.2.dev78/julearn/pipeline/tests/test_target_pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/prepare.py` & `julearn-0.3.2.dev78/julearn/prepare.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/scoring/available_scorers.py` & `julearn-0.3.2.dev78/julearn/scoring/available_scorers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/scoring/metrics.py` & `julearn-0.3.2.dev78/julearn/scoring/metrics.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/scoring/tests/test_available_scorers.py` & `julearn-0.3.2.dev78/julearn/scoring/tests/test_available_scorers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/scoring/tests/test_metrics.py` & `julearn-0.3.2.dev78/julearn/scoring/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/stats/corrected_ttest.py` & `julearn-0.3.2.dev78/julearn/stats/corrected_ttest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/stats/tests/test_corrected_ttest.py` & `julearn-0.3.2.dev78/julearn/stats/tests/test_corrected_ttest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/tests/test_api.py` & `julearn-0.3.2.dev78/julearn/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/tests/test_config.py` & `julearn-0.3.2.dev78/julearn/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/tests/test_prepare.py` & `julearn-0.3.2.dev78/julearn/tests/test_prepare.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/__init__.py` & `julearn-0.3.2.dev78/julearn/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/available_transformers.py` & `julearn-0.3.2.dev78/julearn/transformers/available_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/cbpm.py` & `julearn-0.3.2.dev78/julearn/transformers/cbpm.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/confound_remover.py` & `julearn-0.3.2.dev78/julearn/transformers/confound_remover.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/dataframe/change_column_types.py` & `julearn-0.3.2.dev78/julearn/transformers/dataframe/change_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/dataframe/drop_columns.py` & `julearn-0.3.2.dev78/julearn/transformers/dataframe/drop_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/dataframe/filter_columns.py` & `julearn-0.3.2.dev78/julearn/transformers/dataframe/filter_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/dataframe/set_column_types.py` & `julearn-0.3.2.dev78/julearn/transformers/dataframe/set_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/dataframe/tests/test_change_column_types.py` & `julearn-0.3.2.dev78/julearn/transformers/dataframe/tests/test_change_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/dataframe/tests/test_drop_columns.py` & `julearn-0.3.2.dev78/julearn/transformers/dataframe/tests/test_drop_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/dataframe/tests/test_filter_columns.py` & `julearn-0.3.2.dev78/julearn/transformers/dataframe/tests/test_filter_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/dataframe/tests/test_set_column_types.py` & `julearn-0.3.2.dev78/julearn/transformers/dataframe/tests/test_set_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/ju_column_transformer.py` & `julearn-0.3.2.dev78/julearn/transformers/ju_column_transformer.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/target/__init__.py` & `julearn-0.3.2.dev78/julearn/transformers/target/__init__.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/target/available_target_transformers.py` & `julearn-0.3.2.dev78/julearn/transformers/target/available_target_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/target/ju_target_transformer.py` & `julearn-0.3.2.dev78/julearn/transformers/target/ju_target_transformer.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/target/ju_transformed_target_model.py` & `julearn-0.3.2.dev78/julearn/transformers/target/ju_transformed_target_model.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/target/target_confound_remover.py` & `julearn-0.3.2.dev78/julearn/transformers/target/target_confound_remover.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/target/tests/test_available_target_transformers.py` & `julearn-0.3.2.dev78/julearn/transformers/target/tests/test_available_target_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/target/tests/test_ju_transformed_target_model.py` & `julearn-0.3.2.dev78/julearn/transformers/target/tests/test_ju_transformed_target_model.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/target/tests/test_target_confound_remover.py` & `julearn-0.3.2.dev78/julearn/transformers/target/tests/test_target_confound_remover.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/tests/test_available_transformers.py` & `julearn-0.3.2.dev78/julearn/transformers/tests/test_available_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/tests/test_cbpm.py` & `julearn-0.3.2.dev78/julearn/transformers/tests/test_cbpm.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/tests/test_confounds.py` & `julearn-0.3.2.dev78/julearn/transformers/tests/test_confounds.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/transformers/tests/test_jucolumntransformers.py` & `julearn-0.3.2.dev78/julearn/transformers/tests/test_jucolumntransformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/utils/_cv.py` & `julearn-0.3.2.dev78/julearn/utils/_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/utils/checks.py` & `julearn-0.3.2.dev78/julearn/utils/checks.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/utils/logging.py` & `julearn-0.3.2.dev78/julearn/utils/logging.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/utils/testing.py` & `julearn-0.3.2.dev78/julearn/utils/testing.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/utils/tests/test_logging.py` & `julearn-0.3.2.dev78/julearn/utils/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/utils/tests/test_version.py` & `julearn-0.3.2.dev78/julearn/utils/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/utils/typing.py` & `julearn-0.3.2.dev78/julearn/utils/typing.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/utils/versions.py` & `julearn-0.3.2.dev78/julearn/utils/versions.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/viz/_scores.py` & `julearn-0.3.2.dev78/julearn/viz/_scores.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn/viz/res/julearn_logo_generalization.png` & `julearn-0.3.2.dev78/julearn/viz/res/julearn_logo_generalization.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev61/julearn.egg-info/PKG-INFO` & `julearn-0.3.2.dev78/julearn.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: julearn
-Version: 0.3.2.dev61
+Version: 0.3.2.dev78
 Summary: Juelich Machine Learning Library
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Sami Hamdan <s.hamdan@fz-juelich.de>
 Maintainer-email: Sami Hamdan <s.hamdan@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/julearn
 Project-URL: documentation, https://juaml.github.io/julearn
 Project-URL: repository, https://github.com/juaml/julearn
@@ -37,24 +37,29 @@
 Requires-Dist: sphinx<7.3,>=5.3.0; extra == "docs"
 Requires-Dist: sphinx-gallery<0.15,>=0.13.0; extra == "docs"
 Requires-Dist: furo<2024.0.0,>=2022.9.29; extra == "docs"
 Requires-Dist: sphinx_copybutton<0.6,>=0.5.0; extra == "docs"
 Requires-Dist: numpydoc<1.6,>=1.5.0; extra == "docs"
 Requires-Dist: towncrier<24; extra == "docs"
 Requires-Dist: scikit-optimize<0.11,>=0.10.0; extra == "docs"
+Requires-Dist: optuna<3.7,>=3.6.0; extra == "docs"
+Requires-Dist: optuna_integration<3.7,>=3.6.0; extra == "docs"
 Provides-Extra: deslib
 Requires-Dist: deslib<0.4,>=0.3.5; extra == "deslib"
 Provides-Extra: viz
 Requires-Dist: panel>=1.3.0; extra == "viz"
 Requires-Dist: bokeh>=3.0.0; extra == "viz"
 Requires-Dist: param>=2.0.0; extra == "viz"
 Provides-Extra: skopt
 Requires-Dist: scikit-optimize<0.11,>=0.10.0; extra == "skopt"
+Provides-Extra: optuna
+Requires-Dist: optuna<3.7,>=3.6.0; extra == "optuna"
+Requires-Dist: optuna_integration<3.7,>=3.6.0; extra == "optuna"
 Provides-Extra: all
-Requires-Dist: julearn[skopt,viz]; extra == "all"
+Requires-Dist: julearn[optuna,skopt,viz]; extra == "all"
 
 # julearn
 
 ![PyPI](https://img.shields.io/pypi/v/julearn?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/julearn?style=flat-square)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/julearn?style=flat-square)
 ![GitHub](https://img.shields.io/github/license/juaml/julearn?style=flat-square)
```

### Comparing `julearn-0.3.2.dev61/julearn.egg-info/SOURCES.txt` & `julearn-0.3.2.dev78/julearn.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,17 @@
 docs/changes/newsfragments/224.misc
 docs/changes/newsfragments/244.misc
 docs/changes/newsfragments/249.bugfix
 docs/changes/newsfragments/251.misc
 docs/changes/newsfragments/255.bugfix
 docs/changes/newsfragments/260.enh
 docs/changes/newsfragments/260.misc
+docs/changes/newsfragments/262.doc
+docs/changes/newsfragments/262.enh
+docs/changes/newsfragments/262.feature
 docs/images/corrected_ttest.png
 docs/images/final_estimator.png
 docs/images/iris_X.png
 docs/images/iris_df.png
 docs/images/iris_y.png
 docs/images/julearn_logo.png
 docs/images/julearn_logo_calm.png
@@ -156,20 +159,23 @@
 julearn/inspect/_preprocess.py
 julearn/inspect/inspector.py
 julearn/inspect/tests/test_cv.py
 julearn/inspect/tests/test_inspector.py
 julearn/inspect/tests/test_pipeline.py
 julearn/inspect/tests/test_preprocess.py
 julearn/model_selection/__init__.py
+julearn/model_selection/_optuna_searcher.py
 julearn/model_selection/_skopt_searcher.py
 julearn/model_selection/available_searchers.py
 julearn/model_selection/continuous_stratified_kfold.py
 julearn/model_selection/stratified_bootstrap.py
 julearn/model_selection/tests/test_available_searchers.py
 julearn/model_selection/tests/test_continous_stratified_kfold.py
+julearn/model_selection/tests/test_optuna_searcher.py
+julearn/model_selection/tests/test_skopt_searcher.py
 julearn/model_selection/tests/test_stratified_bootstrap.py
 julearn/models/__init__.py
 julearn/models/available_models.py
 julearn/models/dynamic.py
 julearn/models/tests/test_available_models.py
 julearn/models/tests/test_dynamic.py
 julearn/models/tests/test_models.py
```

### Comparing `julearn-0.3.2.dev61/pyproject.toml` & `julearn-0.3.2.dev78/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -56,27 +56,33 @@
     "sphinx>=5.3.0,<7.3",
     "sphinx-gallery>=0.13.0,<0.15",
     "furo>=2022.9.29,<2024.0.0",
     "sphinx_copybutton>=0.5.0,<0.6",
     "numpydoc>=1.5.0,<1.6",
     "towncrier<24",
     "scikit-optimize>=0.10.0,<0.11",
+    "optuna>=3.6.0,<3.7",
+    "optuna_integration>=3.6.0,<3.7",
 ]
 deslib = ["deslib>=0.3.5,<0.4"]
 viz = [
     "panel>=1.3.0",
     "bokeh>=3.0.0",
     "param>=2.0.0",
 ]
 
 skopt = ["scikit-optimize>=0.10.0,<0.11"]
+optuna = [
+    "optuna>=3.6.0,<3.7",
+    "optuna_integration>=3.6.0,<3.7",
+]
 
 # Add all optional functional dependencies (skip deslib until its fixed)
 # This does not include dev/docs building dependencies
-all = ["julearn[viz,skopt]"]
+all = ["julearn[viz,skopt,optuna]"]
 
 ################
 # Tool configs #
 ################
 
 [tool.setuptools]
 packages = ["julearn"]
```

### Comparing `julearn-0.3.2.dev61/tox.ini` & `julearn-0.3.2.dev78/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 [testenv]
 skip_install = false
 deps =
     pytest
     seaborn
     scikit-optimize>=0.10.0,<0.11
+    optuna>=3.6.0,<3.7
+    optuna_integration>=3.6.0,<3.7
 commands =
     pytest {toxinidir}/julearn
 
 [testenv:ruff]
 skip_install = true
 deps =
     ruff
@@ -38,14 +40,16 @@
     pytest
     seaborn
     deslib
     panel>=1.0.0b1
     bokeh>=3.0.0
     param
     scikit-optimize>=0.10.0,<0.11
+    optuna>=3.6.0,<3.7
+    optuna_integration>=3.6.0,<3.7
 commands =
     pytest -vv {toxinidir}/julearn
 
 [testenv:nodeps]
 skip_install = false
 deps =
     pytest
@@ -60,14 +64,16 @@
     pytest-cov
     seaborn
     deslib
     panel>=1.0.0b1
     bokeh>=3.0.0
     param
     scikit-optimize>=0.10.0,<0.11
+    optuna>=3.6.0,<3.7
+    optuna_integration>=3.6.0,<3.7
 commands =
     pytest --cov={envsitepackagesdir}/julearn --cov=./julearn --cov-report=xml --cov-report=term -vv
 
 [testenv:codespell]
 skip_install = true
 deps =
     codespell
```


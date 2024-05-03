# Comparing `tmp/jdaviz-3.9.0.tar.gz` & `tmp/jdaviz-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdaviz-3.9.0.tar", last modified: Fri Apr  5 17:58:48 2024, max compression
+gzip compressed data, was "jdaviz-3.9.1.tar", last modified: Fri Apr 19 19:34:01 2024, max compression
```

## Comparing `jdaviz-3.9.0.tar` & `jdaviz-3.9.1.tar`

### file list

```diff
@@ -1,580 +1,580 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.491143 jdaviz-3.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.bandit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.415144 jdaviz-3.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.415144 jdaviz-3.9.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.415144 jdaviz-3.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/workflows/changelog_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/workflows/check_milestone.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/workflows/ci_cron_weekly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/workflows/open_actions.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/workflows/predeps_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/workflows/standalone.yml
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.mailmap
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    62052 2024-04-05 17:58:39.000000 jdaviz-3.9.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-05 17:58:39.000000 jdaviz-3.9.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-05 17:58:39.000000 jdaviz-3.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-05 17:58:39.000000 jdaviz-3.9.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-05 17:58:39.000000 jdaviz-3.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-05 17:58:48.491143 jdaviz-3.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-04-05 17:58:39.000000 jdaviz-3.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 17:58:39.000000 jdaviz-3.9.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-05 17:58:39.000000 jdaviz-3.9.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.419144 jdaviz-3.9.0/jdaviz/
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/_astropy_init.py
--rw-r--r--   0 runner    (1001) docker     (127)   118731 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/app.vue
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.423144 jdaviz-3.9.0/jdaviz/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/docs_link.vue
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/external_link.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/glue_state_sync_wrapper.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/layer_viewer_icon.vue
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/multiselect_toggle.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/number_uncertainty.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/play_pause_widget.vue
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_action_button.vue
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_add_results.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_auto_label.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_dataset_select.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_editable_select.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_file_import_select.vue
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_inline_select.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_inline_select_item.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_layer_select.vue
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_layer_select_tabs.vue
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_plot.vue
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_popout.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_previews_temp_disabled.vue
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_section_header.vue
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_subset_select.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_table.vue
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_viewer_select.vue
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/toolbar_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/toolbar_nested.vue
--rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/tooltip.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/tray_plugin.vue
--rw-r--r--   0 runner    (1001) docker     (127)    13973 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/viewer_data_select.vue
--rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/viewer_data_select_item.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.427144 jdaviz-3.9.0/jdaviz/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.427144 jdaviz-3.9.0/jdaviz/configs/cubeviz/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/cubeviz.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/cubeviz.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9907 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.427144 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.427144 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/moment_maps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/moment_maps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14738 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.427144 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10298 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/test_moment_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)    21916 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.427144 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/slice/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/slice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/slice/slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/slice/slice.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.427144 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/slice/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/slice/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.427144 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/spectral_extraction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/spectral_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23868 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/spectral_extraction/spectral_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)    10597 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/spectral_extraction/spectral_extraction.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.427144 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/spectral_extraction/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/spectral_extraction/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16836 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/spectral_extraction/tests/test_spectral_extraction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.431144 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_aperphot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_export_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16929 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.431144 jdaviz-3.9.0/jdaviz/configs/default/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/default.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.431144 jdaviz-3.9.0/jdaviz/configs/default/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.431144 jdaviz-3.9.0/jdaviz/configs/default/plugins/collapse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/collapse/collapse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/collapse/collapse.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.431144 jdaviz-3.9.0/jdaviz/configs/default/plugins/collapse/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/collapse/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/collapse/tests/test_collapse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.431144 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_quality/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_quality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_quality/dq_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.431144 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_quality/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_quality/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_quality/tests/test_data_quality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.431144 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_tools/data_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_tools/data_tools.vue
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_tools/file_chooser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.435144 jdaviz-3.9.0/jdaviz/configs/default/plugins/export/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28350 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/export/export.py
--rw-r--r--   0 runner    (1001) docker     (127)    10572 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/export/export.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.435144 jdaviz-3.9.0/jdaviz/configs/default/plugins/export/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/export/tests/test_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.435144 jdaviz-3.9.0/jdaviz/configs/default/plugins/gaussian_smooth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/gaussian_smooth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.435144 jdaviz-3.9.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.435144 jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/line_list_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    36176 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/line_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)    15989 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/line_lists.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.435144 jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/tests/test_line_lists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.435144 jdaviz-3.9.0/jdaviz/configs/default/plugins/markers/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/markers/markers.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/markers/markers.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.435144 jdaviz-3.9.0/jdaviz/configs/default/plugins/markers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/markers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/markers/tests/test_markers_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.435144 jdaviz-3.9.0/jdaviz/configs/default/plugins/metadata_viewer/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/metadata_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.439144 jdaviz-3.9.0/jdaviz/configs/default/plugins/metadata_viewer/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/metadata_viewer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/metadata_viewer/tests/test_metadata_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.439144 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14046 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/fitting_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    44501 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.439144 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/tests/test_blackbody.py
--rw-r--r--   0 runner    (1001) docker     (127)    16343 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/tests/test_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)    19486 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/tests/test_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.439144 jdaviz-3.9.0/jdaviz/configs/default/plugins/plot_options/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/plot_options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59261 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/plot_options/plot_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    38152 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/plot_options/plot_options.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.439144 jdaviz-3.9.0/jdaviz/configs/default/plugins/plot_options/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/plot_options/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15827 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/plot_options/tests/test_plot_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.439144 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30851 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.439144 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/tests/test_subset_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.443144 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.443144 jdaviz-3.9.0/jdaviz/configs/default/plugins/viewer_creator/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/viewer_creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue
--rw-r--r--   0 runner    (1001) docker     (127)    15412 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.443144 jdaviz-3.9.0/jdaviz/configs/imviz/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16990 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/imviz.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/imviz.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.443144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.443144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/aper_phot_simple/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/aper_phot_simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46898 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.443144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/catalogs/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.443144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/compass/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/compass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/compass/compass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/compass/compass.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.447144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/coords_info/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/coords_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26887 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.447144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/footprints/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/footprints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25455 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/footprints/footprints.py
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/footprints/footprints.vue
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/footprints/preset_regions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.447144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/image_viewer_creator/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/image_viewer_creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.447144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/line_profile_xy/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/line_profile_xy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.447144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/orientation/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/orientation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32344 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/orientation/orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/orientation/orientation.vue
--rw-r--r--   0 runner    (1001) docker     (127)    16874 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.447144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/rotate_canvas/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/rotate_canvas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.447144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/test_rotate_canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16085 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.451144 jdaviz-3.9.0/jdaviz/configs/imviz/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.455144 jdaviz-3.9.0/jdaviz/configs/imviz/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/data/ds9_annulus_01.reg
--rw-r--r--   0 runner    (1001) docker     (127)   604800 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs.fits
--rw-r--r--   0 runner    (1001) docker     (127)   155520 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs_block_reduced.fits
--rw-r--r--   0 runner    (1001) docker     (127)   155520 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs_block_reduced_rotated.fits
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    15780 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_astrowidgets_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7993 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_catalogs.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_compass.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_delete_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_footprints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_line_profile_xy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_linking.py
--rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)    26072 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_parser_asdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_parser_roman.py
--rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23873 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_simple_aper_phot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_subset_centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_viewer_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_viewers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_wcs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20574 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/wcs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.455144 jdaviz-3.9.0/jdaviz/configs/mosviz/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38346 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/mosviz.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/mosviz.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.455144 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40180 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.455144 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/row_lock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/row_lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.455144 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/slit_overlay/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/slit_overlay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.455144 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    19272 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.455144 jdaviz-3.9.0/jdaviz/configs/mosviz/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/tests/test_data_loading.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/tests/test_source_identifier_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/tests/test_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.459143 jdaviz-3.9.0/jdaviz/configs/specviz/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13706 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.459143 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.459143 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22575 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     7697 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.459143 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17666 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_line_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_lineflux.py
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.459143 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/unit_conversion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/unit_conversion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.459143 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/test_unit_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.vue
--rw-r--r--   0 runner    (1001) docker     (127)    26312 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/viewers.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/specviz.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/specviz.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.459143 jdaviz-3.9.0/jdaviz/configs/specviz/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22581 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/tests/test_viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.459143 jdaviz-3.9.0/jdaviz/configs/specviz2d/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.459143 jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.463143 jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44142 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)    17012 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.463143 jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/test_spectral_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/specviz2d.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.463143 jdaviz-3.9.0/jdaviz/configs/specviz2d/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/container.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.467143 jdaviz-3.9.0/jdaviz/core/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23254 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/astrowidgets_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/custom_traitlets.py
--rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/data_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)    11992 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/freezable_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    42995 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/launcher.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/linelists.py
--rw-r--r--   0 runner    (1001) docker     (127)    25783 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/marks.py
--rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/region_translators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/registries.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/style_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)   198067 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/template_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.467143 jdaviz-3.9.0/jdaviz/core/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/tests/test_autoconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/tests/test_custom_traitlets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/tests/test_data_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/tests/test_region_translators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/tests/test_template_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    21790 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/user_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/validunits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.411144 jdaviz-3.9.0/jdaviz/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.467143 jdaviz-3.9.0/jdaviz/data/data_quality/
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/data_quality/jwst.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/data_quality/roman.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.475143 jdaviz-3.9.0/jdaviz/data/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/blink.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/checktoradial.svg
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/compass.svg
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/contrast.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/cubeviz_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/home.svg
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/home_match.svg
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/image.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/imviz_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/left-east.svg
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/line_select.svg
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/line_select_disabled.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/mosviz_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/pan.svg
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/pan2.svg
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/pan_x.svg
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/pan_x_match.svg
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/pan_y.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/pan_y_match.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/panzoom_match.svg
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/pixelspectra.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/radialtocheck.svg
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/right-east.svg
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/select_annulus.svg
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/select_circle.svg
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/select_ellipse.svg
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/select_lasso.svg
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/select_single_pixel.svg
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/select_x.svg
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/select_xy.svg
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/select_y.svg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/slice.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/spectral_range.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/specviz2d_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/specviz_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/stretch_bounds.svg
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/tune.svg
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/zoom_back.svg
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/zoom_box.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/zoom_box_match.svg
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/zoom_xrange.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/zoom_xrange_match.svg
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/zoom_yrange.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/zoom_yrange_match.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.479143 jdaviz-3.9.0/jdaviz/data/linelists/
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/Atomic-ISO.csv
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/Atomic-Ionic.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/CO-band-heads.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/CO.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/Common_Galactic_700A-2000A.csv
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/Common_nebular.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/Common_stellar.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/DEV_NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/H-He.csv
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/H-Paschen-Brackett.csv
--rw-r--r--   0 runner    (1001) docker     (127)    20639 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/H2-ISO.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/H2-alt.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/H2.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/HeI-HeII.csv
--rw-r--r--   0 runner    (1001) docker     (127)    21334 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/JWST_line_list_original.txt
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/PAH.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/SDSS-IV.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/SDSS.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/UV_linelist_vacuum.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/linelist_metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/jdaviz_cli.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/jdaviz_cli_launcher.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/main_styles.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.479143 jdaviz-3.9.0/jdaviz/models/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13731 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/models/physical_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/style_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.479143 jdaviz-3.9.0/jdaviz/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/tests/coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/tests/test_data_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/tests/test_plugin_is_active.py
--rw-r--r--   0 runner    (1001) docker     (127)    48140 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/tests/test_subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/tests/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/tests/test_viewer_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-05 17:58:48.000000 jdaviz-3.9.0/jdaviz/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.491143 jdaviz-3.9.0/jdaviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-05 17:58:48.000000 jdaviz-3.9.0/jdaviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20936 2024-04-05 17:58:48.000000 jdaviz-3.9.0/jdaviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:58:48.000000 jdaviz-3.9.0/jdaviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-05 17:58:48.000000 jdaviz-3.9.0/jdaviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:58:47.000000 jdaviz-3.9.0/jdaviz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-05 17:58:48.000000 jdaviz-3.9.0/jdaviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 17:58:48.000000 jdaviz-3.9.0/jdaviz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.479143 jdaviz-3.9.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-05 17:58:39.000000 jdaviz-3.9.0/licenses/GINGA_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-05 17:58:39.000000 jdaviz-3.9.0/licenses/IMEXAM_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-05 17:58:39.000000 jdaviz-3.9.0/licenses/IPYFILECHOOSER_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-05 17:58:39.000000 jdaviz-3.9.0/licenses/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-05 17:58:39.000000 jdaviz-3.9.0/licenses/TEMPLATE_LICENCE.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.483143 jdaviz-3.9.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/CubevizExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    16821 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/ImvizDitheredExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19158 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/ImvizExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/MosvizExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/MosvizNIRISSExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/Specviz2dExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/SpecvizExample.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.487143 jdaviz-3.9.0/notebooks/concepts/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    15331 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/cubeviz_aperture_photometry.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/cubeviz_contour_overlay.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/cubeviz_data_interactions.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8783 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/cubeviz_fitting.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/cubeviz_ndarray_gif.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/cubeviz_spectral_fitting.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13949 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/default_programmatic_viewers_from_blank.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_advanced_aper_phot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_color_display.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_colorbar_mpl.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15370 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_compass_mpl.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_custom_colormap.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_dithered_gwcs.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_edit_subset_programmatic.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_line_profiles.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_load_3d_slices.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_load_fits_hdu.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15426 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_roman_asdf.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_simple_aper_phot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    20908 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/mosviz_concept.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    33356 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/mosviz_generate_photometry.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/mosviz_niriss_parser.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/pypi_metrics.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/specviz_from_list.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    82825 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/specviz_from_splot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/specviz_glue_unit_conversion.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/specviz_line_lists.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/specviz_minimal.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/specviz_spectrum_list.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-05 17:58:39.000000 jdaviz-3.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:58:48.491143 jdaviz-3.9.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     5534 2024-04-05 17:58:39.000000 jdaviz-3.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.411144 jdaviz-3.9.0/share/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.411144 jdaviz-3.9.0/share/jupyter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.411144 jdaviz-3.9.0/share/jupyter/nbconvert/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.411144 jdaviz-3.9.0/share/jupyter/nbconvert/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.487143 jdaviz-3.9.0/share/jupyter/nbconvert/templates/jdaviz-default/
--rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-04-05 17:58:39.000000 jdaviz-3.9.0/share/jupyter/nbconvert/templates/jdaviz-default/ansi.js
--rwxr-xr-x   0 runner    (1001) docker     (127)     3653 2024-04-05 17:58:39.000000 jdaviz-3.9.0/share/jupyter/nbconvert/templates/jdaviz-default/app.html
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 17:58:39.000000 jdaviz-3.9.0/share/jupyter/nbconvert/templates/jdaviz-default/conf.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     3265 2024-04-05 17:58:39.000000 jdaviz-3.9.0/share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2
--rwxr-xr-x   0 runner    (1001) docker     (127)     5993 2024-04-05 17:58:39.000000 jdaviz-3.9.0/share/jupyter/nbconvert/templates/jdaviz-default/util.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.411144 jdaviz-3.9.0/share/jupyter/voila/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.411144 jdaviz-3.9.0/share/jupyter/voila/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.487143 jdaviz-3.9.0/share/jupyter/voila/templates/jdaviz-default/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-05 17:58:39.000000 jdaviz-3.9.0/share/jupyter/voila/templates/jdaviz-default/index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.487143 jdaviz-3.9.0/standalone/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/entitlements.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.491143 jdaviz-3.9.0/standalone/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-asdf.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-bqplot.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-debugpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-glue.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-glue_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-ipypopout.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-jdaviz.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-jupyter_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-jupyter_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-jupyter_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-mistune.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-photutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-pysiaf.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-regions.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-skimage.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-specreduce.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/jdaviz-cli-entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/jdaviz.spec
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/test_standalone.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-05 17:58:39.000000 jdaviz-3.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.182574 jdaviz-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.bandit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.106574 jdaviz-3.9.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.106574 jdaviz-3.9.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.106574 jdaviz-3.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.github/workflows/changelog_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.github/workflows/check_milestone.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.github/workflows/ci_cron_weekly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.github/workflows/open_actions.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.github/workflows/predeps_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.github/workflows/standalone.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-19 19:33:51.000000 jdaviz-3.9.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    63004 2024-04-19 19:33:51.000000 jdaviz-3.9.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-19 19:33:51.000000 jdaviz-3.9.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-19 19:33:51.000000 jdaviz-3.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-19 19:33:51.000000 jdaviz-3.9.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-19 19:33:51.000000 jdaviz-3.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-19 19:34:01.182574 jdaviz-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-04-19 19:33:51.000000 jdaviz-3.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-19 19:33:51.000000 jdaviz-3.9.1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-19 19:33:51.000000 jdaviz-3.9.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.110574 jdaviz-3.9.1/jdaviz/
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/_astropy_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118854 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/app.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.114574 jdaviz-3.9.1/jdaviz/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/docs_link.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/external_link.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/glue_state_sync_wrapper.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/layer_viewer_icon.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/multiselect_toggle.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/number_uncertainty.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/play_pause_widget.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/plugin_action_button.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/plugin_add_results.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/plugin_auto_label.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/plugin_dataset_select.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/plugin_editable_select.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/plugin_file_import_select.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/plugin_inline_select.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/plugin_inline_select_item.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/plugin_layer_select.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/plugin_layer_select_tabs.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/plugin_plot.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/plugin_popout.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/plugin_previews_temp_disabled.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/plugin_section_header.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/plugin_subset_select.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/plugin_table.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/plugin_viewer_select.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/toolbar_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/toolbar_nested.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/tooltip.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/tray_plugin.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    13973 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/viewer_data_select.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/components/viewer_data_select_item.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.114574 jdaviz-3.9.1/jdaviz/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.114574 jdaviz-3.9.1/jdaviz/configs/cubeviz/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/cubeviz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/cubeviz.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9773 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.118574 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.118574 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/moment_maps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/moment_maps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14738 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.118574 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/moment_maps/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/moment_maps/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10298 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/moment_maps/tests/test_moment_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21916 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.118574 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/slice/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/slice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/slice/slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/slice/slice.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.118574 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/slice/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/slice/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.118574 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/spectral_extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/spectral_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24058 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/spectral_extraction/spectral_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10597 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/spectral_extraction/spectral_extraction.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.118574 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/spectral_extraction/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/spectral_extraction/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16836 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/spectral_extraction/tests/test_spectral_extraction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.122574 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_aperphot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/tests/test_export_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/tests/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16473 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.122574 jdaviz-3.9.1/jdaviz/configs/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/default.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.122574 jdaviz-3.9.1/jdaviz/configs/default/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.122574 jdaviz-3.9.1/jdaviz/configs/default/plugins/collapse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/collapse/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/collapse/collapse.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.122574 jdaviz-3.9.1/jdaviz/configs/default/plugins/collapse/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/collapse/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/collapse/tests/test_collapse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.122574 jdaviz-3.9.1/jdaviz/configs/default/plugins/data_quality/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/data_quality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/data_quality/dq_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.122574 jdaviz-3.9.1/jdaviz/configs/default/plugins/data_quality/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/data_quality/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/data_quality/tests/test_data_quality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.122574 jdaviz-3.9.1/jdaviz/configs/default/plugins/data_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/data_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/data_tools/data_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/data_tools/data_tools.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/data_tools/file_chooser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.122574 jdaviz-3.9.1/jdaviz/configs/default/plugins/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28350 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/export/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10572 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/export/export.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.126574 jdaviz-3.9.1/jdaviz/configs/default/plugins/export/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/export/tests/test_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.126574 jdaviz-3.9.1/jdaviz/configs/default/plugins/gaussian_smooth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/gaussian_smooth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.126574 jdaviz-3.9.1/jdaviz/configs/default/plugins/gaussian_smooth/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/gaussian_smooth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.126574 jdaviz-3.9.1/jdaviz/configs/default/plugins/line_lists/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/line_lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/line_lists/line_list_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36176 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/line_lists/line_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15989 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/line_lists/line_lists.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.126574 jdaviz-3.9.1/jdaviz/configs/default/plugins/line_lists/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/line_lists/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/line_lists/tests/test_line_lists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.126574 jdaviz-3.9.1/jdaviz/configs/default/plugins/markers/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/markers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/markers/markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/markers/markers.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.126574 jdaviz-3.9.1/jdaviz/configs/default/plugins/markers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/markers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/markers/tests/test_markers_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.126574 jdaviz-3.9.1/jdaviz/configs/default/plugins/metadata_viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/metadata_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.126574 jdaviz-3.9.1/jdaviz/configs/default/plugins/metadata_viewer/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/metadata_viewer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/metadata_viewer/tests/test_metadata_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.130574 jdaviz-3.9.1/jdaviz/configs/default/plugins/model_fitting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/model_fitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14046 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/model_fitting/fitting_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/model_fitting/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44501 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/model_fitting/model_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/model_fitting/model_fitting.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.130574 jdaviz-3.9.1/jdaviz/configs/default/plugins/model_fitting/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/model_fitting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/model_fitting/tests/test_blackbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16343 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/model_fitting/tests/test_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19486 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/model_fitting/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.130574 jdaviz-3.9.1/jdaviz/configs/default/plugins/plot_options/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/plot_options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59261 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/plot_options/plot_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38152 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/plot_options/plot_options.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.130574 jdaviz-3.9.1/jdaviz/configs/default/plugins/plot_options/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/plot_options/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15827 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/plot_options/tests/test_plot_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.130574 jdaviz-3.9.1/jdaviz/configs/default/plugins/subset_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/subset_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30851 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.130574 jdaviz-3.9.1/jdaviz/configs/default/plugins/subset_plugin/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/subset_plugin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/subset_plugin/tests/test_subset_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/subset_plugin/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.130574 jdaviz-3.9.1/jdaviz/configs/default/plugins/subset_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/subset_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/subset_tools/subset_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/subset_tools/subset_tools.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.130574 jdaviz-3.9.1/jdaviz/configs/default/plugins/viewer_creator/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/viewer_creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    15523 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/default/plugins/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.134574 jdaviz-3.9.1/jdaviz/configs/imviz/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17092 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/imviz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/imviz.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.134574 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.134574 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/aper_phot_simple/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/aper_phot_simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46898 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.134574 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/catalogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/catalogs/catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/catalogs/catalogs.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.134574 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/compass/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/compass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/compass/compass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/compass/compass.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.134574 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/coords_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/coords_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26887 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/coords_info/coords_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/coords_info/coords_info.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.134574 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/footprints/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/footprints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26476 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/footprints/footprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/footprints/footprints.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/footprints/preset_regions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.138574 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/image_viewer_creator/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/image_viewer_creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.138574 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/line_profile_xy/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/line_profile_xy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.138574 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/orientation/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/orientation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33435 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/orientation/orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/orientation/orientation.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    16874 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.138574 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/rotate_canvas/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/rotate_canvas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.138574 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/rotate_canvas/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/rotate_canvas/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/rotate_canvas/tests/test_rotate_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16085 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/plugins/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.142574 jdaviz-3.9.1/jdaviz/configs/imviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.142574 jdaviz-3.9.1/jdaviz/configs/imviz/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/data/ds9_annulus_01.reg
+-rw-r--r--   0 runner    (1001) docker     (127)   604800 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   155520 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs_block_reduced.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   155520 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs_block_reduced_rotated.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    15780 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_astrowidgets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7993 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_compass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_delete_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_footprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_line_profile_xy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_linking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26072 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_parser_asdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_parser_roman.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23873 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_simple_aper_phot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_subset_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_viewer_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_wcs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20574 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/imviz/wcs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.146574 jdaviz-3.9.1/jdaviz/configs/mosviz/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38346 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/mosviz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/mosviz.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.146574 jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40180 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.146574 jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/row_lock/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/row_lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/row_lock/row_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/row_lock/row_lock.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.146574 jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/slit_overlay/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/slit_overlay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.146574 jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/slit_overlay/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/slit_overlay/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19272 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.146574 jdaviz-3.9.1/jdaviz/configs/mosviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/tests/test_data_loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/tests/test_source_identifier_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/mosviz/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.146574 jdaviz-3.9.1/jdaviz/configs/specviz/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13706 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.150574 jdaviz-3.9.1/jdaviz/configs/specviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.150574 jdaviz-3.9.1/jdaviz/configs/specviz/plugins/line_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/plugins/line_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22575 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7697 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.150574 jdaviz-3.9.1/jdaviz/configs/specviz/plugins/line_analysis/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/plugins/line_analysis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17666 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/plugins/line_analysis/tests/test_line_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/plugins/line_analysis/tests/test_lineflux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.150574 jdaviz-3.9.1/jdaviz/configs/specviz/plugins/unit_conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/plugins/unit_conversion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.150574 jdaviz-3.9.1/jdaviz/configs/specviz/plugins/unit_conversion/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/plugins/unit_conversion/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/plugins/unit_conversion/tests/test_unit_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    26312 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/plugins/viewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/specviz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/specviz.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.150574 jdaviz-3.9.1/jdaviz/configs/specviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22581 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz/tests/test_viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.150574 jdaviz-3.9.1/jdaviz/configs/specviz2d/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz2d/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.150574 jdaviz-3.9.1/jdaviz/configs/specviz2d/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz2d/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz2d/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.150574 jdaviz-3.9.1/jdaviz/configs/specviz2d/plugins/spectral_extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz2d/plugins/spectral_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44142 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17012 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.154574 jdaviz-3.9.1/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/test_spectral_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz2d/specviz2d.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.154574 jdaviz-3.9.1/jdaviz/configs/specviz2d/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz2d/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz2d/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/configs/specviz2d/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/container.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.158574 jdaviz-3.9.1/jdaviz/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23254 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/astrowidgets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/custom_traitlets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/data_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11992 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/freezable_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42995 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/launcher.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/linelists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25783 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/marks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/region_translators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/style_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)   198067 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/template_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.158574 jdaviz-3.9.1/jdaviz/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/tests/test_autoconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/tests/test_custom_traitlets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/tests/test_data_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/tests/test_region_translators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/tests/test_template_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21790 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/core/validunits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.098574 jdaviz-3.9.1/jdaviz/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.158574 jdaviz-3.9.1/jdaviz/data/data_quality/
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/data_quality/jwst.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/data_quality/roman.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.166574 jdaviz-3.9.1/jdaviz/data/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/blink.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/checktoradial.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/compass.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/contrast.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/cubeviz_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/home.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/home_match.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/image.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/imviz_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/left-east.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/line_select.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/line_select_disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/mosviz_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/pan.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/pan2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/pan_x.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/pan_x_match.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/pan_y.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/pan_y_match.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/panzoom_match.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/pixelspectra.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/radialtocheck.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/right-east.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/select_annulus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/select_circle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/select_ellipse.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/select_lasso.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/select_single_pixel.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/select_x.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/select_xy.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/select_y.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/slice.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/spectral_range.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/specviz2d_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/specviz_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/stretch_bounds.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/tune.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/zoom_back.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/zoom_box.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/zoom_box_match.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/zoom_xrange.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/zoom_xrange_match.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/zoom_yrange.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/icons/zoom_yrange_match.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.170574 jdaviz-3.9.1/jdaviz/data/linelists/
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/Atomic-ISO.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/Atomic-Ionic.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/CO-band-heads.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/CO.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/Common_Galactic_700A-2000A.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/Common_nebular.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/Common_stellar.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/DEV_NOTES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/H-He.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/H-Paschen-Brackett.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    20639 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/H2-ISO.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/H2-alt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/H2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/HeI-HeII.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    21334 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/JWST_line_list_original.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/PAH.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/SDSS-IV.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/SDSS.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/UV_linelist_vacuum.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/data/linelists/linelist_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/jdaviz_cli.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/jdaviz_cli_launcher.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/main_styles.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.170574 jdaviz-3.9.1/jdaviz/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13731 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/models/physical_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/style_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.170574 jdaviz-3.9.1/jdaviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/tests/coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/tests/test_data_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/tests/test_plugin_is_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48140 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/tests/test_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/tests/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/tests/test_viewer_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-04-19 19:33:51.000000 jdaviz-3.9.1/jdaviz/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-19 19:34:00.000000 jdaviz-3.9.1/jdaviz/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.182574 jdaviz-3.9.1/jdaviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-19 19:34:00.000000 jdaviz-3.9.1/jdaviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20936 2024-04-19 19:34:01.000000 jdaviz-3.9.1/jdaviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:34:00.000000 jdaviz-3.9.1/jdaviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-19 19:34:00.000000 jdaviz-3.9.1/jdaviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:34:00.000000 jdaviz-3.9.1/jdaviz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-19 19:34:00.000000 jdaviz-3.9.1/jdaviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 19:34:00.000000 jdaviz-3.9.1/jdaviz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.170574 jdaviz-3.9.1/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-19 19:33:51.000000 jdaviz-3.9.1/licenses/GINGA_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-19 19:33:51.000000 jdaviz-3.9.1/licenses/IMEXAM_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-19 19:33:51.000000 jdaviz-3.9.1/licenses/IPYFILECHOOSER_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-19 19:33:51.000000 jdaviz-3.9.1/licenses/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-19 19:33:51.000000 jdaviz-3.9.1/licenses/TEMPLATE_LICENCE.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.174574 jdaviz-3.9.1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/CubevizExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16821 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/ImvizDitheredExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19158 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/ImvizExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/MosvizExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/MosvizNIRISSExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/Specviz2dExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/SpecvizExample.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.178574 jdaviz-3.9.1/notebooks/concepts/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15331 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/cubeviz_aperture_photometry.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/cubeviz_contour_overlay.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/cubeviz_data_interactions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8783 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/cubeviz_fitting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/cubeviz_ndarray_gif.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/cubeviz_spectral_fitting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13949 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/default_programmatic_viewers_from_blank.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/imviz_advanced_aper_phot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/imviz_color_display.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/imviz_colorbar_mpl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15370 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/imviz_compass_mpl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/imviz_custom_colormap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/imviz_dithered_gwcs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/imviz_edit_subset_programmatic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/imviz_line_profiles.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/imviz_load_3d_slices.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/imviz_load_fits_hdu.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15426 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/imviz_roman_asdf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/imviz_simple_aper_phot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20908 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/mosviz_concept.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    33356 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/mosviz_generate_photometry.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/mosviz_niriss_parser.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/pypi_metrics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/specviz_from_list.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    82825 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/specviz_from_splot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/specviz_glue_unit_conversion.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/specviz_line_lists.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/specviz_minimal.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-19 19:33:51.000000 jdaviz-3.9.1/notebooks/concepts/specviz_spectrum_list.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-19 19:33:51.000000 jdaviz-3.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:34:01.182574 jdaviz-3.9.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5534 2024-04-19 19:33:51.000000 jdaviz-3.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.098574 jdaviz-3.9.1/share/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.098574 jdaviz-3.9.1/share/jupyter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.098574 jdaviz-3.9.1/share/jupyter/nbconvert/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.098574 jdaviz-3.9.1/share/jupyter/nbconvert/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.178574 jdaviz-3.9.1/share/jupyter/nbconvert/templates/jdaviz-default/
+-rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-04-19 19:33:51.000000 jdaviz-3.9.1/share/jupyter/nbconvert/templates/jdaviz-default/ansi.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3653 2024-04-19 19:33:51.000000 jdaviz-3.9.1/share/jupyter/nbconvert/templates/jdaviz-default/app.html
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 19:33:51.000000 jdaviz-3.9.1/share/jupyter/nbconvert/templates/jdaviz-default/conf.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3265 2024-04-19 19:33:51.000000 jdaviz-3.9.1/share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5993 2024-04-19 19:33:51.000000 jdaviz-3.9.1/share/jupyter/nbconvert/templates/jdaviz-default/util.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.098574 jdaviz-3.9.1/share/jupyter/voila/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.098574 jdaviz-3.9.1/share/jupyter/voila/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.178574 jdaviz-3.9.1/share/jupyter/voila/templates/jdaviz-default/
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-19 19:33:51.000000 jdaviz-3.9.1/share/jupyter/voila/templates/jdaviz-default/index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.178574 jdaviz-3.9.1/standalone/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-19 19:33:51.000000 jdaviz-3.9.1/standalone/entitlements.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:34:01.182574 jdaviz-3.9.1/standalone/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-19 19:33:51.000000 jdaviz-3.9.1/standalone/hooks/hook-asdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-19 19:33:51.000000 jdaviz-3.9.1/standalone/hooks/hook-bqplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-19 19:33:51.000000 jdaviz-3.9.1/standalone/hooks/hook-debugpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-19 19:33:51.000000 jdaviz-3.9.1/standalone/hooks/hook-glue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-19 19:33:51.000000 jdaviz-3.9.1/standalone/hooks/hook-glue_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-19 19:33:51.000000 jdaviz-3.9.1/standalone/hooks/hook-ipypopout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-19 19:33:51.000000 jdaviz-3.9.1/standalone/hooks/hook-jdaviz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-19 19:33:51.000000 jdaviz-3.9.1/standalone/hooks/hook-jupyter_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-19 19:33:51.000000 jdaviz-3.9.1/standalone/hooks/hook-jupyter_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-19 19:33:51.000000 jdaviz-3.9.1/standalone/hooks/hook-jupyter_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 19:33:51.000000 jdaviz-3.9.1/standalone/hooks/hook-mistune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 19:33:51.000000 jdaviz-3.9.1/standalone/hooks/hook-photutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-19 19:33:51.000000 jdaviz-3.9.1/standalone/hooks/hook-pysiaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-19 19:33:51.000000 jdaviz-3.9.1/standalone/hooks/hook-regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-19 19:33:51.000000 jdaviz-3.9.1/standalone/hooks/hook-skimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-19 19:33:51.000000 jdaviz-3.9.1/standalone/hooks/hook-specreduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-19 19:33:51.000000 jdaviz-3.9.1/standalone/jdaviz-cli-entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-19 19:33:51.000000 jdaviz-3.9.1/standalone/jdaviz.spec
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-19 19:33:51.000000 jdaviz-3.9.1/standalone/test_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-19 19:33:51.000000 jdaviz-3.9.1/tox.ini
```

### Comparing `jdaviz-3.9.0/.github/ISSUE_TEMPLATE/bug_report.yaml` & `jdaviz-3.9.1/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/.github/ISSUE_TEMPLATE/feature_request.yaml` & `jdaviz-3.9.1/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/.github/PULL_REQUEST_TEMPLATE.md` & `jdaviz-3.9.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/.github/dependabot.yml` & `jdaviz-3.9.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/.github/labeler.yml` & `jdaviz-3.9.1/.github/labeler.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/.github/workflows/check_milestone.yml` & `jdaviz-3.9.1/.github/workflows/check_milestone.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/.github/workflows/ci_cron_weekly.yml` & `jdaviz-3.9.1/.github/workflows/ci_cron_weekly.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/.github/workflows/ci_workflows.yml` & `jdaviz-3.9.1/.github/workflows/ci_workflows.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/.github/workflows/codeql-analysis.yml` & `jdaviz-3.9.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/.github/workflows/open_actions.yml` & `jdaviz-3.9.1/.github/workflows/open_actions.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/.github/workflows/predeps_workflows.yml` & `jdaviz-3.9.1/.github/workflows/predeps_workflows.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/.github/workflows/publish.yml` & `jdaviz-3.9.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/.github/workflows/standalone.yml` & `jdaviz-3.9.1/.github/workflows/standalone.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/.gitignore` & `jdaviz-3.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/.mailmap` & `jdaviz-3.9.1/.mailmap`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/.readthedocs.yaml` & `jdaviz-3.9.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/CHANGES.rst` & `jdaviz-3.9.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,42 @@
+3.9.1 (2024-04-19)
+==================
+
+- Fix mouseover display's top-layer logic to account for the visibility and contour toggles in
+  the plot options plugin. [#2818]
+
+Bug Fixes
+---------
+
+- Fix dropdown selection for table format in export plugin. [#2793]
+
+- Standalone mode: stop jdaviz/voila processes when closing app. [#2791]
+
+- Fixes compatibility with glue >= 1.19. [#2820]
+
+Cubeviz
+^^^^^^^
+
+- Spectral extraction errors will show in snackbar. [#2807]
+
+Imviz
+^^^^^
+
+- Fix bugs where API created footprints did not overlay and only last
+  footprint displayed if added before linking. [#2790, #2797]
+
+- Improved behavior when orientations are created or selected without having data loaded in the viewer. [#2789]
+
+- Fixed a bug in the Orientation plugin where a WCS orientation could sometimes be flipped. [#2802]
+
+Specviz
+^^^^^^^
+
+- H-Paschen-Brackett HI 5-4 line's rest wavelength is now correct. It was previously off by 0.5 micron. [#2819]
+
 3.9 (2024-04-05)
 ================
 
 New Features
 ------------
 - Stretch bounds tool now enables dynamic adjustment of spline knots. [#2545, #2623]
```

### Comparing `jdaviz-3.9.0/CITATION.cff` & `jdaviz-3.9.1/CITATION.cff`

 * *Files 6% similar despite different names*

```diff
@@ -69,13 +69,13 @@
   orcid: "https://orcid.org/0009-0008-4112-7418"
 - family-names: "Tollerud"
   given-names: "Erik"
   orcid: "https://orcid.org/0000-0002-9599-310X"
 - family-names: "Volfman"
   given-names: "Sabrina"
 title: "Jdaviz"
-version: 3.9.0
+version: 3.9.1
 doi: https://doi.org/10.5281/zenodo.5513927
-date-released: 2024-04-05
+date-released: 2024-04-19
 url: "https://github.com/spacetelescope/jdaviz"
 
 # see a full list of contributors here: https://github.com/spacetelescope/jdaviz/graphs/contributors
```

### Comparing `jdaviz-3.9.0/CODE_OF_CONDUCT.md` & `jdaviz-3.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/LICENSE.rst` & `jdaviz-3.9.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/PKG-INFO` & `jdaviz-3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdaviz
-Version: 3.9.0
+Version: 3.9.1
 Summary: Astronomical data analysis development leveraging the Jupyter platform
 Author-email: JDADF Developers <help@stsci.edu>
 Project-URL: Homepage, https://jdaviz.readthedocs.io/en/latest/
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: packaging
```

### Comparing `jdaviz-3.9.0/README.rst` & `jdaviz-3.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/conftest.py` & `jdaviz-3.9.1/conftest.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/__init__.py` & `jdaviz-3.9.1/jdaviz/__init__.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/_astropy_init.py` & `jdaviz-3.9.1/jdaviz/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/app.py` & `jdaviz-3.9.1/jdaviz/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,21 +91,25 @@
     def to_unit(self, data, cid, values, original_units, target_units):
         # Given a glue data object (data), a component ID (cid), the values
         # to convert, and the original and target units of the values, this method
         # should return the converted values. Note that original_units
         # gives the units of the values array, which might not be the same
         # as the original native units of the component in the data.
         if cid.label == "flux":
-            spec = data.get_object(cls=Spectrum1D)
-            if len(values) == 2:
-                # Need this for setting the y-limits
-                spec_limits = [spec.spectral_axis[0].value, spec.spectral_axis[-1].value]
-                eqv = u.spectral_density(spec_limits*spec.spectral_axis.unit)
+            try:
+                spec = data.get_object(cls=Spectrum1D)
+            except RuntimeError:
+                eqv = []
             else:
-                eqv = u.spectral_density(spec.spectral_axis)
+                if len(values) == 2:
+                    # Need this for setting the y-limits
+                    spec_limits = [spec.spectral_axis[0].value, spec.spectral_axis[-1].value]
+                    eqv = u.spectral_density(spec_limits * spec.spectral_axis.unit)
+                else:
+                    eqv = u.spectral_density(spec.spectral_axis)
         else:  # spectral axis
             eqv = u.spectral()
 
         return (values * u.Unit(original_units)).to_value(u.Unit(target_units), equivalencies=eqv)
 
 
 # Set default opacity for data layers to 1 instead of 0.8 in
```

### Comparing `jdaviz-3.9.0/jdaviz/app.vue` & `jdaviz-3.9.1/jdaviz/app.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/cli.py` & `jdaviz-3.9.1/jdaviz/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,15 +105,34 @@
         Voila.notebook_path = 'notebook.ipynb'
         VoilaConfiguration.template = 'jdaviz-default'
         VoilaConfiguration.enable_nbextensions = True
         VoilaConfiguration.file_whitelist = ['.*']
         VoilaConfiguration.theme = theme
         if browser != 'default':
             Voila.browser = browser
-        sys.exit(Voila().launch_instance(argv=[]))
+
+        voila = Voila.instance()
+        # monkey patch listen, so we can get a handle on the kernel_manager
+        # after it is created
+        previous_listen = voila.listen
+
+        def listen(*args, **kwargs):
+            # monkey patch remove_kernel, so we can stop the event loop
+            # when a kernel is removed (which means the browser page was closed)
+            previous_remove_kernel = voila.kernel_manager.remove_kernel
+
+            def remove_kernel(kernel_id):
+                previous_remove_kernel(kernel_id)
+                voila.ioloop.stop()
+
+            voila.kernel_manager.remove_kernel = remove_kernel
+            return previous_listen(*args, **kwargs)
+
+        voila.listen = listen
+        sys.exit(voila.launch_instance(argv=[]))
     finally:
         os.chdir(start_dir)
 
 
 def _main(config=None):
     import argparse
     import sys
```

### Comparing `jdaviz-3.9.0/jdaviz/components/docs_link.vue` & `jdaviz-3.9.1/jdaviz/components/docs_link.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/glue_state_sync_wrapper.vue` & `jdaviz-3.9.1/jdaviz/components/glue_state_sync_wrapper.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/layer_viewer_icon.vue` & `jdaviz-3.9.1/jdaviz/components/layer_viewer_icon.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/multiselect_toggle.vue` & `jdaviz-3.9.1/jdaviz/components/multiselect_toggle.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/number_uncertainty.vue` & `jdaviz-3.9.1/jdaviz/components/number_uncertainty.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/play_pause_widget.vue` & `jdaviz-3.9.1/jdaviz/components/play_pause_widget.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/plugin_action_button.vue` & `jdaviz-3.9.1/jdaviz/components/plugin_action_button.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/plugin_add_results.vue` & `jdaviz-3.9.1/jdaviz/components/plugin_add_results.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/plugin_auto_label.vue` & `jdaviz-3.9.1/jdaviz/components/plugin_auto_label.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/plugin_dataset_select.vue` & `jdaviz-3.9.1/jdaviz/components/plugin_dataset_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/plugin_editable_select.vue` & `jdaviz-3.9.1/jdaviz/components/plugin_editable_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/plugin_file_import_select.vue` & `jdaviz-3.9.1/jdaviz/components/plugin_file_import_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/plugin_inline_select.vue` & `jdaviz-3.9.1/jdaviz/components/plugin_inline_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/plugin_inline_select_item.vue` & `jdaviz-3.9.1/jdaviz/components/plugin_inline_select_item.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/plugin_layer_select.vue` & `jdaviz-3.9.1/jdaviz/components/plugin_layer_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/plugin_layer_select_tabs.vue` & `jdaviz-3.9.1/jdaviz/components/plugin_layer_select_tabs.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/plugin_plot.vue` & `jdaviz-3.9.1/jdaviz/components/plugin_plot.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/plugin_previews_temp_disabled.vue` & `jdaviz-3.9.1/jdaviz/components/plugin_previews_temp_disabled.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/plugin_section_header.vue` & `jdaviz-3.9.1/jdaviz/components/plugin_section_header.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/plugin_subset_select.vue` & `jdaviz-3.9.1/jdaviz/components/plugin_subset_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/plugin_table.vue` & `jdaviz-3.9.1/jdaviz/components/plugin_table.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/plugin_viewer_select.vue` & `jdaviz-3.9.1/jdaviz/components/plugin_viewer_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/toolbar_nested.py` & `jdaviz-3.9.1/jdaviz/components/toolbar_nested.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/toolbar_nested.vue` & `jdaviz-3.9.1/jdaviz/components/toolbar_nested.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/tooltip.vue` & `jdaviz-3.9.1/jdaviz/components/tooltip.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/tray_plugin.vue` & `jdaviz-3.9.1/jdaviz/components/tray_plugin.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/viewer_data_select.vue` & `jdaviz-3.9.1/jdaviz/components/viewer_data_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/components/viewer_data_select_item.vue` & `jdaviz-3.9.1/jdaviz/components/viewer_data_select_item.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/cubeviz.ipynb` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/cubeviz.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/cubeviz.yaml` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/cubeviz.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/helper.py` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 from astropy.io import fits
 from astropy.io import registry as io_registry
 from astropy.utils.decorators import deprecated
-from glue.core import BaseData
 from specutils import Spectrum1D
 from specutils.io.registers import _astropy_has_priorities
 
 from jdaviz.core.helpers import ImageConfigHelper
 from jdaviz.configs.default.plugins.line_lists.line_list_mixin import LineListMixin
 from jdaviz.configs.specviz import Specviz
 from jdaviz.core.events import (AddDataMessage,
@@ -177,18 +176,14 @@
         results : `~astropy.table.QTable` or `None`
             Photometry results if available or `None` otherwise.
 
         """
         return self.plugins['Aperture Photometry']._obj.export_table()
 
 
-def layer_is_cube_image_data(layer):
-    return isinstance(layer, BaseData) and layer.ndim in (2, 3)
-
-
 # TODO: We can remove this when specutils supports it, i.e.,
 #       https://github.com/astropy/specutils/issues/592 and
 #       https://github.com/astropy/specutils/pull/1009
 # NOTE: Cannot use custom_write decorator from specutils because
 #       that involves asking user to manually put something in
 #       their ~/.specutils directory.
```

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.py` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.vue` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/test_moment_maps.py` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/moment_maps/tests/test_moment_maps.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/parsers.py` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/slice/slice.py` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/slice/slice.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/slice/slice.vue` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/slice/slice.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/spectral_extraction/spectral_extraction.py` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/spectral_extraction/spectral_extraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,15 +408,20 @@
             # Cylindrical aperture
             slice_mask = aperture.to_mask(method=aper_method).to_image(im_shape)
             # Turn 2D slice_mask into 3D array that is the same shape as the flux cube
             mask_weights = np.stack([slice_mask] * len(flux_cube.spectral_axis), axis=2)
         return mask_weights
 
     def vue_spectral_extraction(self, *args, **kwargs):
-        self.collapse_to_spectrum(add_data=True)
+        try:
+            self.collapse_to_spectrum(add_data=True)
+        except Exception as e:
+            self.hub.broadcast(SnackbarMessage(
+                f"Extraction failed: {repr(e)}",
+                sender=self, color="error"))
 
     def vue_save_as_fits(self, *args):
         self._save_extracted_spec_to_fits()
 
     def vue_overwrite_fits(self, *args):
         """Attempt to force writing the spectral extraction if the user
         confirms the desire to overwrite."""
```

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/spectral_extraction/spectral_extraction.vue` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/spectral_extraction/spectral_extraction.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/spectral_extraction/tests/test_spectral_extraction.py` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/spectral_extraction/tests/test_spectral_extraction.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_aperphot.py` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_aperphot.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_helper.py` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_export_plots.py` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/tests/test_export_plots.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_parsers.py` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_regions.py` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/tests/test_regions.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_tools.py` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tools.py` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/viewers.py` & `jdaviz-3.9.1/jdaviz/configs/cubeviz/plugins/viewers.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from glue.core.subset_group import GroupedSubset
 from bqplot import Lines
 from glue_jupyter.bqplot.image import BqplotImageView
 
 from jdaviz.core.registries import viewer_registry
 from jdaviz.core.marks import SliceIndicatorMarks, ShadowSpatialSpectral
-from jdaviz.configs.cubeviz.helper import layer_is_cube_image_data
 from jdaviz.configs.default.plugins.viewers import JdavizViewerMixin
 from jdaviz.configs.specviz.plugins.viewers import SpecvizProfileView
 from jdaviz.core.events import AddDataMessage, RemoveDataMessage
 from jdaviz.core.freezable_state import FreezableBqplotImageViewerState
 from jdaviz.utils import get_subset_type
 
 __all__ = ['CubevizImageView', 'CubevizProfileView',
@@ -151,26 +150,14 @@
     def _default_flux_viewer_reference_name(self):
         return self.jdaviz_helper._default_flux_viewer_reference_name
 
     @property
     def _default_uncert_viewer_reference_name(self):
         return self.jdaviz_helper._default_uncert_viewer_reference_name
 
-    @property
-    def active_image_layer(self):
-        """Active image layer in the viewer, if available."""
-        # Find visible layers
-        visible_layers = [layer for layer in self.state.layers
-                          if (layer.visible and layer_is_cube_image_data(layer.layer))]
-
-        if len(visible_layers) == 0:
-            return None
-
-        return visible_layers[-1]
-
     def _initial_x_axis(self, *args):
         # Make sure that the x_att is correct on data load
         ref_data = self.state.reference_data
         if ref_data and ref_data.ndim == 3:
             for att_name in ["Right Ascension", "RA", "Galactic Longitude"]:
                 if att_name in ref_data.component_ids():
                     x_att = att_name
```

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/default.ipynb` & `jdaviz-3.9.1/jdaviz/configs/default/default.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/__init__.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/collapse/collapse.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/collapse/collapse.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/collapse/collapse.vue` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/collapse/collapse.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/collapse/tests/test_collapse.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/collapse/tests/test_collapse.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/data_quality/dq_utils.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/data_quality/dq_utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/data_quality/tests/test_data_quality.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/data_quality/tests/test_data_quality.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/data_tools/data_tools.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/data_tools/data_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/data_tools/data_tools.vue` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/data_tools/data_tools.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/data_tools/file_chooser.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/data_tools/file_chooser.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/export/export.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/export/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                                                    selected='viewer_format_selected',
                                                    manual_options=viewer_format_options)
 
         # NOTE: see self.plugin_table.selected_obj.write.list_formats() for full list of options,
         # although not all support passing overwrite
         plugin_table_format_options = ['ecsv', 'csv', 'fits']
         self.plugin_table_format = SelectPluginComponent(self,
-                                                         items='plugin-table_format_items',
+                                                         items='plugin_table_format_items',
                                                          selected='plugin_table_format_selected',
                                                          manual_options=plugin_table_format_options)
 
         subset_format_options = ['fits', 'reg']
         self.subset_format = SelectPluginComponent(self,
                                                    items='subset_format_items',
                                                    selected='subset_format_selected',
```

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/export/export.vue` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/export/export.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/export/tests/test_export.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/export/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/line_list_mixin.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/line_lists/line_list_mixin.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/line_lists.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/line_lists/line_lists.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/line_lists.vue` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/line_lists/line_lists.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/tests/test_line_lists.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/line_lists/tests/test_line_lists.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/markers/markers.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/markers/markers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/markers/markers.vue` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/markers/markers.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/markers/tests/test_markers_plugin.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/markers/tests/test_markers_plugin.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.vue` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/metadata_viewer/tests/test_metadata_viewer.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/metadata_viewer/tests/test_metadata_viewer.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/fitting_backend.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/model_fitting/fitting_backend.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/initializers.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/model_fitting/initializers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/model_fitting/model_fitting.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.vue` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/model_fitting/model_fitting.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/tests/test_blackbody.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/model_fitting/tests/test_blackbody.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/tests/test_fitting.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/model_fitting/tests/test_fitting.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/tests/test_plugin.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/model_fitting/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/plot_options/plot_options.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/plot_options/plot_options.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/plot_options/plot_options.vue` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/plot_options/plot_options.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/plot_options/tests/test_plot_options.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/plot_options/tests/test_plot_options.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.vue` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/tests/test_subset_plugin.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/subset_plugin/tests/test_subset_plugin.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/utils.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/subset_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/subset_tools/subset_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/default/plugins/viewers.py` & `jdaviz-3.9.1/jdaviz/configs/default/plugins/viewers.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,16 +310,17 @@
                     self.toolbar.active_tool = None
 
     @property
     def active_image_layer(self):
         """Active image layer in the viewer, if available."""
         # Find visible layers
         visible_layers = [layer for layer in self.state.layers
-                          if (layer.visible and layer_is_image_data(layer.layer))]
-
+                          if (layer.visible and
+                              layer_is_image_data(layer.layer) and
+                              (layer.bitmap_visible or layer.contour_visible))]
         if len(visible_layers) == 0:
             return None
 
         return visible_layers[-1]
 
     def initialize_toolbar(self, default_tool_priority=[]):
         # NOTE: this overrides glue_jupyter.IPyWidgetView
```

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/helper.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,16 +394,20 @@
 
 def layer_is_2d(layer):
     # returns True for subclasses of BaseData with ndim=2, both for
     # layers that are WCS-only as well as images containing data:
     return isinstance(layer, BaseData) and layer.ndim == 2
 
 
+def layer_is_2d_or_3d(layer):
+    return isinstance(layer, BaseData) and layer.ndim in (2, 3)
+
+
 def layer_is_image_data(layer):
-    return layer_is_2d(layer) and not layer.meta.get(_wcs_only_label, False)
+    return layer_is_2d_or_3d(layer) and not layer.meta.get(_wcs_only_label, False)
 
 
 def layer_is_wcs_only(layer):
     return layer_is_2d(layer) and layer.meta.get(_wcs_only_label, False)
 
 
 def get_wcs_only_layer_labels(app):
```

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/imviz.ipynb` & `jdaviz-3.9.1/jdaviz/configs/imviz/imviz.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/imviz.yaml` & `jdaviz-3.9.1/jdaviz/configs/imviz/imviz.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.vue` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/catalogs/catalogs.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.vue` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/catalogs/catalogs.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/compass/compass.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/compass/compass.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/compass/compass.vue` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/compass/compass.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/coords_info/coords_info.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.vue` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/coords_info/coords_info.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/footprints/footprints.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/footprints/footprints.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     """
     See the :ref:`Footprints Plugin Documentation <imviz-footprints>` for more details.
 
     Only the following attributes and methods are available through the
     :ref:`public plugin API <plugin-apis>`:
 
     * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.show`
-    * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.open_in_tray`
+    * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.open_in_tray`
     * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.close_in_tray`
     * ``overlay`` (:class:`~jdaviz.core.template_mixin.EditableSelectPluginComponent`): the
         currently active overlay (all other traitlets control this overlay instance)
     * :meth:`rename_overlay`
         rename any overlay
     * :meth:`add_overlay`
         add a new overlay instance (and select as active)
@@ -181,14 +181,21 @@
 
     def _on_link_type_updated(self, msg=None):
         self.is_pixel_linked = (getattr(self.app, '_link_type', None) == 'pixels' and
                                 len(self.app.data_collection) > 1)
         # toggle visibility as necessary
         self._on_is_active_changed()
 
+        # When footprint(s) are added via API before WCS link. Overlays visibility & is_active
+        # can be True, but only last footprint will display. This ensures all footprints display
+        if not self.is_pixel_linked:
+            for choice in self.overlay.choices:
+                # trigger the update without actually changing the user-selection
+                self._change_overlay(overlay_selected=choice, center_the_overlay=False)
+
     def vue_link_by_wcs(self, *args):
         # call other plugin so that other options (wcs_use_affine, wcs_use_fallback)
         # are retained.  Remove this method if support for plotting footprints
         # when pixel-linked is reintroduced.
         self.app._jdaviz_helper.plugins['Orientation'].link_type = 'WCS'
 
     def _ensure_first_overlay(self):
@@ -310,45 +317,51 @@
         self._ignore_traitlet_change = False
         self._preset_args_changed()  # process ra/dec simultaneously
 
     def vue_center_on_viewer(self, viewer_ref):
         self.center_on_viewer(viewer_ref)
 
     @observe('overlay_selected')
-    def _change_overlay(self, *args):
+    def _change_overlay(self, *args, overlay_selected=None, center_the_overlay=True):
         if not hasattr(self, 'overlay'):  # pragma: nocover
             # plugin/traitlet startup
             return
         if self.overlay_selected == '':
             # no overlay selected (this can happen when removing all overlays)
             return
 
-        if self.overlay_selected not in self._overlays:
+        overlay_selected = overlay_selected if overlay_selected is not None else self.overlay_selected  # noqa
+
+        if overlay_selected not in self._overlays:
+            # _on_link_type_updated() called in init but don't want to create
+            # the default overlay yet, since center_on_viewer() will cause a traceback
+            if not center_the_overlay:
+                return
             # create new entry with defaults (any defaults not provided here will be carried over
             # from the previous selection based on current traitlet values)
 
             # if this is the first overlay, there is a chance the traitlet for color was already set
             # to something other than the default, so we want to use that, otherwise for successive
             # new overlays, we want to ignore the traitlet and default back to "active" orange.
             default_color = '#c75109' if len(self._overlays) else self.color
-            self._overlays[self.overlay_selected] = {'color': default_color}
+            self._overlays[overlay_selected] = {'color': default_color}
 
             # similarly, if the user called any import APIs before opening the plugin, we want to
             # respect that, but when creating successive overlays, any selection from file/region
             # should be cleared for the next selection
             if self.preset_selected == 'From File...' and len(self._overlays) > 1:
-                self._overlays[self.overlay_selected]['from_file'] = ''
-                self._overlays[self.overlay_selected]['preset'] = self.preset.choices[0]
+                self._overlays[overlay_selected]['from_file'] = ''
+                self._overlays[overlay_selected]['preset'] = self.preset.choices[0]
 
             # for the first overlay only, default the position to be centered on the current
             # zoom limits of the first selected viewer
             if len(self._overlays) == 1 and len(self.viewer.selected):
                 self.center_on_viewer(self.viewer.selected[0])
 
-        fp = self._overlays[self.overlay_selected]
+        fp = self._overlays[overlay_selected]
 
         # we'll temporarily disable updating the overlays so that we can set all
         # traitlets simultaneously (and since we're only updating traitlets to a previously-set
         # overlay, we shouldn't have to update anything with the marks themselves)
         self._ignore_traitlet_change = True
         for attr in ('from_file', 'preset_selected',
                      'visible', 'color', 'fill_opacity', 'viewer_selected',
@@ -361,23 +374,25 @@
                 setattr(self, attr, fp[key])
             else:
                 # then adopt the value from the traitlet (copy from the previous selection).
                 # This should only ever occur for entries that are not defined in the default
                 # dict above.
                 fp[key] = getattr(self, attr)
         self._ignore_traitlet_change = False
-        self._preset_args_changed()
+        self._preset_args_changed(overlay_selected=overlay_selected)
 
     def _mark_visible(self, viewer_id, overlay=None):
         if not self.is_active:
             return False
         if self.is_pixel_linked:
             return False
         if overlay is None:
             overlay = self.overlay_selected
+        if overlay not in self._overlays:
+            return False
         fp = self._overlays[overlay]
         if viewer_id not in fp.get('viewer', []):
             return False
         else:
             return fp.get('visible', False)
 
     @observe('viewer_selected', 'visible', 'color', 'fill_opacity')
@@ -455,49 +470,50 @@
         elif self.has_pysiaf and self.preset_selected in preset_regions._instruments:
             regs = preset_regions.jwst_footprint(self.preset_selected, **callable_kwargs)
         else:  # pragma: no cover
             regs = []
         return regs
 
     @observe('preset_selected', 'from_file', 'ra', 'dec', 'pa', 'v2_offset', 'v3_offset')
-    def _preset_args_changed(self, msg={}):
+    def _preset_args_changed(self, msg={}, overlay_selected=None):
         if self._ignore_traitlet_change:
             return
-        if not self.overlay_selected:
+        overlay_selected = overlay_selected if overlay_selected is not None else self.overlay_selected  # noqa
+        if not overlay_selected:
             return
 
         name = msg.get('name', '').split('_selected')[0]
 
-        if self.overlay_selected not in self._overlays:
+        if overlay_selected not in self._overlays:
             # default dictionary has not been created yet
             return
 
         if len(name):
-            self._overlays[self.overlay_selected][name] = msg.get('new')
-        if name == 'from_file' and 'regions' in self._overlays[self.overlay_selected]:
+            self._overlays[overlay_selected][name] = msg.get('new')
+        if name == 'from_file' and 'regions' in self._overlays[overlay_selected]:
             # then the file may have been changed from the API, so we need to clear the cache
             # the cache will then be re-populated on the call to self.overlay_regions below
-            del self._overlays[self.overlay_selected]['regions']
+            del self._overlays[overlay_selected]['regions']
 
         regs = self.overlay_regions
 
         for viewer_id, viewer in self.app._viewer_store.items():
             visible = self._mark_visible(viewer_id)
             # TODO: need to re-call this logic when the reference_data is changed... which might
             # warrant some refactoring so we don't have to loop over all viewers if it has only
             # changed in one viewer
             wcs = getattr(viewer.state.reference_data, 'coords', None)
             if wcs is None:
                 continue
-            existing_overlays = self._get_marks(viewer, self.overlay_selected)
+            existing_overlays = self._get_marks(viewer, overlay_selected)
             update_existing = len(existing_overlays) == len(regs)
             if not update_existing and len(existing_overlays):
                 # clear any existing marks (length has changed, perhaps a new preset)
                 viewer.figure.marks = [m for m in viewer.figure.marks
-                                       if getattr(m, 'overlay', None) != self.overlay_selected]
+                                       if getattr(m, 'overlay', None) != overlay_selected]
 
             # the following logic is adapted from
             # https://github.com/spacetelescope/jwst_novt/blob/main/jwst_novt/interact/display.py
             new_marks = []
             for i, reg in enumerate(regs):
                 if (not isinstance(reg, regions.Region)
                         or not hasattr(reg, 'to_pixel')):   # pragma: no cover
@@ -530,15 +546,15 @@
                     mark = existing_overlays[i]
                     with mark.hold_sync():
                         mark.x = x_coords
                         mark.y = y_coords
                 else:
                     mark = FootprintOverlay(
                         viewer,
-                        self.overlay_selected,
+                        overlay_selected,
                         x=x_coords,
                         y=y_coords,
                         colors=[self.color],
                         fill_opacities=[self.fill_opacity],
                         visible=visible)
                     new_marks.append(mark)
```

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/footprints/footprints.vue` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/footprints/footprints.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/footprints/preset_regions.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/footprints/preset_regions.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/orientation/orientation.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/orientation/orientation.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,14 +271,17 @@
     def vue_reset_astrowidget_markers(self, *args):
         for viewer in self.app._viewer_store.values():
             viewer.reset_markers()
 
     def _get_wcs_angles(self, first_loaded_image=None):
         if first_loaded_image is None:
             first_loaded_image = self.viewer.selected_obj.first_loaded_data
+            if first_loaded_image is None:
+                # These won't end up getting used in this case, but we need an actual number
+                return 0, 0, 0
         degn, dege, flip = get_compass_info(
             first_loaded_image.coords, first_loaded_image.shape
         )[-3:]
         return degn, dege, flip
 
     def rotation_angle_deg(self, rotation_angle=None):
         if rotation_angle is None:
@@ -320,22 +323,34 @@
         wrt_data : str, optional
             Orientation calculations is done with respect to this data WCS.
             If `None`, it grabs the first loaded data in the selected viewer
             (may or may not be visible); If no data is loaded in the viewer,
             nothing will be done.
 
         """
+        self._add_orientation(rotation_angle=rotation_angle, east_left=east_left, label=label,
+                              set_on_create=set_on_create, wrt_data=wrt_data)
+
+    def _add_orientation(self, rotation_angle=None, east_left=None, label=None,
+                         set_on_create=True, wrt_data=None, from_ui=False):
+
         if self.link_type_selected != 'WCS':
             raise ValueError("must be aligned by WCS to add orientation options")
 
         if wrt_data is None:
             # if not specified, use first-loaded image layer as the
             # default rotation:
             wrt_data = self.viewer.selected_obj.first_loaded_data
             if wrt_data is None:  # Nothing in viewer
+                msg = "Viewer must have data loaded to add an orientation."
+                if from_ui:
+                    self.hub.broadcast(SnackbarMessage(msg, color="error",
+                                                       timeout=6000, sender=self))
+                else:
+                    raise ValueError(msg)
                 return
 
         rotation_angle = self.rotation_angle_deg(rotation_angle)
         if east_left is None:
             east_left = self.east_left
         if label is None:
             label = self.new_layer_label
@@ -410,15 +425,15 @@
             if hasattr(layer.layer, "meta")
         )
         if all_wcs_only_layers and msg.data.meta.get(_wcs_only_label, False):
             # on adding first data layer, reset the limits:
             self.viewer.selected_obj.state.reset_limits()
 
     def vue_add_orientation(self, *args, **kwargs):
-        self.add_orientation(set_on_create=True)
+        self._add_orientation(set_on_create=True, from_ui=True)
 
     @observe('orientation_layer_selected')
     def _change_reference_data(self, *args, **kwargs):
         if self._refdata_change_available:
             self.app._change_reference_data(
                 self.orientation.selected, viewer_id=self.viewer.selected
             )
@@ -482,43 +497,47 @@
     def _on_viewer_change(self, msg={}):
         # don't update choices until viewer is available:
         ref_data = self.ref_data
         if hasattr(self, 'viewer') and ref_data is not None:
             if ref_data.label in self.orientation.choices:
                 self.orientation.selected = ref_data.label
 
-    def create_north_up_east_left(self, label="North-up, East-left", set_on_create=False):
+    def create_north_up_east_left(self, label="North-up, East-left", set_on_create=False,
+                                  from_ui=False):
         """
         Set the rotation angle and flip to achieve North up and East left
         according to the reference image WCS.
         """
         if label not in self.orientation.choices:
             degn = self._get_wcs_angles()[-3]
-            self.add_orientation(rotation_angle=degn, east_left=True,
-                                 label=label, set_on_create=set_on_create)
+            self._add_orientation(rotation_angle=degn, east_left=True,
+                                  label=label, set_on_create=set_on_create,
+                                  from_ui=from_ui)
         elif set_on_create:
             self.orientation.selected = label
 
-    def create_north_up_east_right(self, label="North-up, East-right", set_on_create=False):
+    def create_north_up_east_right(self, label="North-up, East-right", set_on_create=False,
+                                   from_ui=False):
         """
         Set the rotation angle and flip to achieve North up and East right
         according to the reference image WCS.
         """
         if label not in self.orientation.choices:
             degn = self._get_wcs_angles()[-3]
-            self.add_orientation(rotation_angle=180 - degn, east_left=False,
-                                 label=label, set_on_create=set_on_create)
+            self._add_orientation(rotation_angle=180 - degn, east_left=False,
+                                  label=label, set_on_create=set_on_create,
+                                  from_ui=from_ui)
         elif set_on_create:
             self.orientation.selected = label
 
     def vue_select_north_up_east_left(self, *args, **kwargs):
-        self.create_north_up_east_left(set_on_create=True)
+        self.create_north_up_east_left(set_on_create=True, from_ui=True)
 
     def vue_select_north_up_east_right(self, *args, **kwargs):
-        self.create_north_up_east_right(set_on_create=True)
+        self.create_north_up_east_right(set_on_create=True, from_ui=True)
 
     def vue_select_default_orientation(self, *args, **kwargs):
         self.orientation.selected = base_wcs_layer_label
 
     @observe('east_left', 'rotation_angle')
     def _update_layer_label_default(self, event={}):
         self.new_layer_label_default = (
```

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/orientation/orientation.vue` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/orientation/orientation.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/parsers.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.vue` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/test_rotate_canvas.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/rotate_canvas/tests/test_rotate_canvas.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/tools.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/viewers.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/plugins/viewers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs.fits` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs.fits`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs_block_reduced.fits` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs_block_reduced.fits`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs_block_reduced_rotated.fits` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs_block_reduced_rotated.fits`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_astrowidgets_api.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_astrowidgets_api.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_catalogs.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_catalogs.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_delete_data.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_delete_data.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_helper.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_line_profile_xy.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_line_profile_xy.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_linking.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_linking.py`

 * *Files 3% similar despite different names*

```diff
@@ -192,24 +192,29 @@
         self.imviz.link_data(link_type='wcs')
 
         # The zoom box for GWCS is now a rotated rombus.
         fits_wcs_zoom_limits = self.viewer._get_zoom_limits(
             self.imviz.app.data_collection['fits_wcs[DATA]'])
         gwcs_zoom_limits = self.viewer._get_zoom_limits(
             self.imviz.app.data_collection['gwcs[DATA]'])
+
+        # x_min, y_min
+        # x_min, y_max
+        # x_max, y_max
+        # x_max, y_min
         assert_allclose(fits_wcs_zoom_limits,
-                        [[-1.590838, -0.423662],
-                         [-1.826862, 9.896219],
-                         [8.590838, 9.423662],
-                         [8.826862, -0.896219]], rtol=1e-5)
+                        [[-2.406711, -1.588057],
+                         [-2.697746, 11.137127],
+                         [10.148055, 10.554429],
+                         [10.439091, -2.170755]], rtol=1e-5)
         assert_allclose(gwcs_zoom_limits,
-                        [[3.186753, 11.337468],
-                         [11.895862, 5.072343],
-                         [6.158421, -3.145985],
-                         [-2.550688, 3.119141]], rtol=1e-5)
+                        [[2.636299, 12.732915],
+                         [13.375281, 5.007547],
+                         [6.300587, -5.126264],
+                         [-4.438394, 2.599103]], rtol=1e-5)
 
         # Also check the coordinates display: Last loaded is on top.
         # Cycle order: GWCS, FITS WCS
         label_mouseover = self.imviz.app.session.application._tools['g-coords-info']
         xy = self.viewer._get_real_xy(self.imviz.app.data_collection[0], 0, 0, reverse=True)
         label_mouseover._viewer_mouse_event(
             self.viewer, {'event': 'mousemove', 'domain': {'x': xy[0], 'y': xy[1]}})
```

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_orientation.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_orientation.py`

 * *Files 3% similar despite different names*

```diff
@@ -219,7 +219,31 @@
         assert_allclose(out_reg.center.ra.deg, reg.center.ra.deg)
         assert_allclose(out_reg.center.dec.deg, reg.center.dec.deg)
         assert_quantity_allclose(out_reg.width, reg.width)
         assert_quantity_allclose(out_reg.height, reg.height)
         # FIXME: However, sky angle has to stay the same as per regions convention.
         with pytest.raises(AssertionError, match="Not equal to tolerance"):
             assert_quantity_allclose(out_reg.angle, reg.angle)
+
+
+class TestOrientationNoData(BaseImviz_WCS_WCS):
+    def test_create_no_data(self):
+        lc_plugin = self.imviz.plugins['Orientation']
+        lc_plugin.link_type = 'WCS'
+
+        self.imviz.create_image_viewer()
+        lc_plugin.viewer = "imviz-1"
+
+        with pytest.raises(ValueError, match="Viewer must have data loaded"):
+            lc_plugin._obj.create_north_up_east_left(set_on_create=True)
+
+    def test_select_no_data(self):
+        lc_plugin = self.imviz.plugins['Orientation']
+        lc_plugin.link_type = 'WCS'
+
+        lc_plugin._obj.create_north_up_east_left(set_on_create=True)
+
+        self.imviz.create_image_viewer()
+        lc_plugin.viewer = "imviz-1"
+        # This would error prior to bugfix
+        lc_plugin.orientation = "North-up, East-left"
+        self.imviz.app.add_data_to_viewer("imviz-1", "has_wcs_1[SCI,1]")
```

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_parser.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_parser_asdf.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_parser_asdf.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_parser_roman.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_parser_roman.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_regions.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_regions.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_simple_aper_phot.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_simple_aper_phot.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_subset_centroid.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_subset_centroid.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_tools.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_viewer_tools.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_viewer_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_viewers.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_viewers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_wcs_utils.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/test_wcs_utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/tests/utils.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/imviz/wcs_utils.py` & `jdaviz-3.9.1/jdaviz/configs/imviz/wcs_utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/mosviz/helper.py` & `jdaviz-3.9.1/jdaviz/configs/mosviz/helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/mosviz/mosviz.ipynb` & `jdaviz-3.9.1/jdaviz/configs/mosviz/mosviz.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/mosviz/mosviz.yaml` & `jdaviz-3.9.1/jdaviz/configs/mosviz/mosviz.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/parsers.py` & `jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.py` & `jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/row_lock/row_lock.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py` & `jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.vue` & `jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py` & `jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/tools.py` & `jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/viewers.py` & `jdaviz-3.9.1/jdaviz/configs/mosviz/plugins/viewers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/mosviz/tests/test_data_loading.py` & `jdaviz-3.9.1/jdaviz/configs/mosviz/tests/test_data_loading.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/mosviz/tests/test_helper.py` & `jdaviz-3.9.1/jdaviz/configs/mosviz/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/mosviz/tests/test_parsers.py` & `jdaviz-3.9.1/jdaviz/configs/mosviz/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/mosviz/tests/test_source_identifier_extract.py` & `jdaviz-3.9.1/jdaviz/configs/mosviz/tests/test_source_identifier_extract.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/mosviz/tests/test_tools.py` & `jdaviz-3.9.1/jdaviz/configs/mosviz/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz/helper.py` & `jdaviz-3.9.1/jdaviz/configs/specviz/helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py` & `jdaviz-3.9.1/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue` & `jdaviz-3.9.1/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_line_analysis.py` & `jdaviz-3.9.1/jdaviz/configs/specviz/plugins/line_analysis/tests/test_line_analysis.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_lineflux.py` & `jdaviz-3.9.1/jdaviz/configs/specviz/plugins/line_analysis/tests/test_lineflux.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz/plugins/parsers.py` & `jdaviz-3.9.1/jdaviz/configs/specviz/plugins/parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/test_unit_conversion.py` & `jdaviz-3.9.1/jdaviz/configs/specviz/plugins/unit_conversion/tests/test_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.py` & `jdaviz-3.9.1/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.vue` & `jdaviz-3.9.1/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz/plugins/viewers.py` & `jdaviz-3.9.1/jdaviz/configs/specviz/plugins/viewers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz/specviz.ipynb` & `jdaviz-3.9.1/jdaviz/configs/specviz/specviz.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz/specviz.yaml` & `jdaviz-3.9.1/jdaviz/configs/specviz/specviz.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz/tests/test_helper.py` & `jdaviz-3.9.1/jdaviz/configs/specviz/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz/tests/test_viewers.py` & `jdaviz-3.9.1/jdaviz/configs/specviz/tests/test_viewers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz2d/helper.py` & `jdaviz-3.9.1/jdaviz/configs/specviz2d/helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/parsers.py` & `jdaviz-3.9.1/jdaviz/configs/specviz2d/plugins/parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py` & `jdaviz-3.9.1/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.vue` & `jdaviz-3.9.1/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/test_spectral_extraction.py` & `jdaviz-3.9.1/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/test_spectral_extraction.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz2d/specviz2d.yaml` & `jdaviz-3.9.1/jdaviz/configs/specviz2d/specviz2d.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz2d/tests/test_helper.py` & `jdaviz-3.9.1/jdaviz/configs/specviz2d/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/configs/specviz2d/tests/test_parsers.py` & `jdaviz-3.9.1/jdaviz/configs/specviz2d/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/conftest.py` & `jdaviz-3.9.1/jdaviz/conftest.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/container.vue` & `jdaviz-3.9.1/jdaviz/container.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/astrowidgets_api.py` & `jdaviz-3.9.1/jdaviz/core/astrowidgets_api.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/config.py` & `jdaviz-3.9.1/jdaviz/core/config.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/custom_traitlets.py` & `jdaviz-3.9.1/jdaviz/core/custom_traitlets.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/data_formats.py` & `jdaviz-3.9.1/jdaviz/core/data_formats.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/events.py` & `jdaviz-3.9.1/jdaviz/core/events.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/freezable_state.py` & `jdaviz-3.9.1/jdaviz/core/freezable_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,21 +163,26 @@
 
                 if return_as_world:
                     x_min = min(x_min, world_bottom_left.ra.value)
                     x_max = max(x_max, world_top_right.ra.value)
                     y_min = min(y_min, world_bottom_left.dec.value)
                     y_max = max(y_max, world_top_right.dec.value)
                 else:
-                    pixel_bottom_left = self.reference_data.coords.world_to_pixel(world_bottom_left)
-                    pixel_top_right = self.reference_data.coords.world_to_pixel(world_top_right)
+                    x_bl, y_bl = self.reference_data.coords.world_to_pixel(world_bottom_left)
+                    x_tr, y_tr = self.reference_data.coords.world_to_pixel(world_top_right)
 
-                    x_min = min(x_min, pixel_bottom_left[0] - 0.5)
-                    x_max = max(x_max, pixel_top_right[0] + 0.5)
-                    y_min = min(y_min, pixel_bottom_left[1] - 0.5)
-                    y_max = max(y_max, pixel_top_right[1] + 0.5)
+                    x_pix_min = min(x_bl, x_tr)
+                    x_pix_max = max(x_bl, x_tr)
+                    y_pix_min = min(y_bl, y_tr)
+                    y_pix_max = max(y_bl, y_tr)
+
+                    x_min = min(x_min, x_pix_min - 0.5)
+                    x_max = max(x_max, x_pix_max + 0.5)
+                    y_min = min(y_min, y_pix_min - 0.5)
+                    y_max = max(y_max, y_pix_max + 0.5)
                 wcs_success = True
 
         if not wcs_success:
             x_min, x_max = -0.5, -np.inf
             y_min, y_max = -0.5, -np.inf
             for layer in self.layers:
                 if not layer.visible or layer.layer.data.ndim == 1:
@@ -197,12 +202,16 @@
         if getattr(self, '_viewer', None) is not None and self._viewer.jdaviz_app.config != 'imviz':
             return super().reset_limits(*event)
         if self.reference_data is None:  # Nothing to do
             return
 
         x_min, x_max, y_min, y_max = self._get_reset_limits()
 
+        # If any bound wasn't set to a real value, don't update
+        if np.any(~np.isfinite([x_min, x_max, y_min, y_max])):
+            return
+
         with delay_callback(self, 'x_min', 'x_max', 'y_min', 'y_max'):
             self.x_min, self.x_max, self.y_min, self.y_max = x_min, x_max, y_min, y_max
             # We need to adjust the limits in here to avoid triggering all
             # the update events then changing the limits again.
             self._adjust_limits_aspect()
```

### Comparing `jdaviz-3.9.0/jdaviz/core/helpers.py` & `jdaviz-3.9.1/jdaviz/core/helpers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/launcher.py` & `jdaviz-3.9.1/jdaviz/core/launcher.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/launcher.vue` & `jdaviz-3.9.1/jdaviz/core/launcher.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/linelists.py` & `jdaviz-3.9.1/jdaviz/core/linelists.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/marks.py` & `jdaviz-3.9.1/jdaviz/core/marks.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/region_translators.py` & `jdaviz-3.9.1/jdaviz/core/region_translators.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/registries.py` & `jdaviz-3.9.1/jdaviz/core/registries.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/template_mixin.py` & `jdaviz-3.9.1/jdaviz/core/template_mixin.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/tests/test_autoconfig.py` & `jdaviz-3.9.1/jdaviz/core/tests/test_autoconfig.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/tests/test_custom_traitlets.py` & `jdaviz-3.9.1/jdaviz/core/tests/test_custom_traitlets.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/tests/test_data_menu.py` & `jdaviz-3.9.1/jdaviz/core/tests/test_data_menu.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/tests/test_helpers.py` & `jdaviz-3.9.1/jdaviz/core/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/tests/test_region_translators.py` & `jdaviz-3.9.1/jdaviz/core/tests/test_region_translators.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/tests/test_template_mixin.py` & `jdaviz-3.9.1/jdaviz/core/tests/test_template_mixin.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/tests/test_tools.py` & `jdaviz-3.9.1/jdaviz/core/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/tools.py` & `jdaviz-3.9.1/jdaviz/core/tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/user_api.py` & `jdaviz-3.9.1/jdaviz/core/user_api.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/core/validunits.py` & `jdaviz-3.9.1/jdaviz/core/validunits.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/data_quality/jwst.csv` & `jdaviz-3.9.1/jdaviz/data/data_quality/jwst.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/data_quality/roman.csv` & `jdaviz-3.9.1/jdaviz/data/data_quality/roman.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/checktoradial.svg` & `jdaviz-3.9.1/jdaviz/data/icons/checktoradial.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/compass.svg` & `jdaviz-3.9.1/jdaviz/data/icons/compass.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/cubeviz_icon.svg` & `jdaviz-3.9.1/jdaviz/data/icons/cubeviz_icon.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/home_match.svg` & `jdaviz-3.9.1/jdaviz/data/icons/home_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/imviz_icon.svg` & `jdaviz-3.9.1/jdaviz/data/icons/imviz_icon.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/line_select.svg` & `jdaviz-3.9.1/jdaviz/data/icons/line_select.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/line_select_disabled.svg` & `jdaviz-3.9.1/jdaviz/data/icons/line_select_disabled.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/mosviz_icon.svg` & `jdaviz-3.9.1/jdaviz/data/icons/mosviz_icon.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/pan.svg` & `jdaviz-3.9.1/jdaviz/data/icons/pan.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/pan2.svg` & `jdaviz-3.9.1/jdaviz/data/icons/pan2.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/pan_x_match.svg` & `jdaviz-3.9.1/jdaviz/data/icons/pan_x_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/pan_y_match.svg` & `jdaviz-3.9.1/jdaviz/data/icons/pan_y_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/panzoom_match.svg` & `jdaviz-3.9.1/jdaviz/data/icons/panzoom_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/pixelspectra.svg` & `jdaviz-3.9.1/jdaviz/data/icons/pixelspectra.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/radialtocheck.svg` & `jdaviz-3.9.1/jdaviz/data/icons/radialtocheck.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/select_annulus.svg` & `jdaviz-3.9.1/jdaviz/data/icons/select_annulus.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/select_circle.svg` & `jdaviz-3.9.1/jdaviz/data/icons/select_circle.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/select_ellipse.svg` & `jdaviz-3.9.1/jdaviz/data/icons/select_ellipse.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/select_lasso.svg` & `jdaviz-3.9.1/jdaviz/data/icons/select_lasso.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/select_single_pixel.svg` & `jdaviz-3.9.1/jdaviz/data/icons/select_single_pixel.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/select_xy.svg` & `jdaviz-3.9.1/jdaviz/data/icons/select_xy.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/slice.svg` & `jdaviz-3.9.1/jdaviz/data/icons/slice.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/spectral_range.svg` & `jdaviz-3.9.1/jdaviz/data/icons/spectral_range.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/specviz2d_icon.svg` & `jdaviz-3.9.1/jdaviz/data/icons/specviz2d_icon.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/specviz_icon.svg` & `jdaviz-3.9.1/jdaviz/data/icons/specviz_icon.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/stretch_bounds.svg` & `jdaviz-3.9.1/jdaviz/data/icons/stretch_bounds.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/zoom_box.svg` & `jdaviz-3.9.1/jdaviz/data/icons/zoom_box.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/zoom_box_match.svg` & `jdaviz-3.9.1/jdaviz/data/icons/zoom_box_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/zoom_xrange.svg` & `jdaviz-3.9.1/jdaviz/data/icons/zoom_xrange.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/zoom_xrange_match.svg` & `jdaviz-3.9.1/jdaviz/data/icons/zoom_xrange_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/zoom_yrange.svg` & `jdaviz-3.9.1/jdaviz/data/icons/zoom_yrange.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/icons/zoom_yrange_match.svg` & `jdaviz-3.9.1/jdaviz/data/icons/zoom_yrange_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/linelists/Atomic-ISO.csv` & `jdaviz-3.9.1/jdaviz/data/linelists/Atomic-ISO.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/linelists/Atomic-Ionic.csv` & `jdaviz-3.9.1/jdaviz/data/linelists/Atomic-Ionic.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv` & `jdaviz-3.9.1/jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/linelists/CO.csv` & `jdaviz-3.9.1/jdaviz/data/linelists/CO.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv` & `jdaviz-3.9.1/jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/linelists/Common_Galactic_700A-2000A.csv` & `jdaviz-3.9.1/jdaviz/data/linelists/Common_Galactic_700A-2000A.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/linelists/Common_nebular.csv` & `jdaviz-3.9.1/jdaviz/data/linelists/Common_nebular.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/linelists/Common_stellar.csv` & `jdaviz-3.9.1/jdaviz/data/linelists/Common_stellar.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/linelists/DEV_NOTES.txt` & `jdaviz-3.9.1/jdaviz/data/linelists/DEV_NOTES.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/linelists/H-He.csv` & `jdaviz-3.9.1/jdaviz/data/linelists/H-He.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/linelists/H2-ISO.csv` & `jdaviz-3.9.1/jdaviz/data/linelists/H2-ISO.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/linelists/H2-alt.csv` & `jdaviz-3.9.1/jdaviz/data/linelists/H2-alt.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/linelists/H2.csv` & `jdaviz-3.9.1/jdaviz/data/linelists/H2.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/linelists/HeI-HeII.csv` & `jdaviz-3.9.1/jdaviz/data/linelists/HeI-HeII.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/linelists/JWST_line_list_original.txt` & `jdaviz-3.9.1/jdaviz/data/linelists/JWST_line_list_original.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/linelists/PAH.csv` & `jdaviz-3.9.1/jdaviz/data/linelists/PAH.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/linelists/SDSS-IV.csv` & `jdaviz-3.9.1/jdaviz/data/linelists/SDSS-IV.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/linelists/SDSS.csv` & `jdaviz-3.9.1/jdaviz/data/linelists/SDSS.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/linelists/UV_linelist_vacuum.csv` & `jdaviz-3.9.1/jdaviz/data/linelists/UV_linelist_vacuum.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/data/linelists/linelist_metadata.json` & `jdaviz-3.9.1/jdaviz/data/linelists/linelist_metadata.json`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/jdaviz_cli.ipynb` & `jdaviz-3.9.1/jdaviz/jdaviz_cli.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/jdaviz_cli_launcher.ipynb` & `jdaviz-3.9.1/jdaviz/jdaviz_cli_launcher.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/main_styles.vue` & `jdaviz-3.9.1/jdaviz/main_styles.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/models/physical_models.py` & `jdaviz-3.9.1/jdaviz/models/physical_models.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/style_registry.py` & `jdaviz-3.9.1/jdaviz/style_registry.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/tests/coveragerc` & `jdaviz-3.9.1/jdaviz/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/tests/test_app.py` & `jdaviz-3.9.1/jdaviz/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/tests/test_data_formats.py` & `jdaviz-3.9.1/jdaviz/tests/test_data_formats.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/tests/test_metadata.py` & `jdaviz-3.9.1/jdaviz/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/tests/test_plugin_is_active.py` & `jdaviz-3.9.1/jdaviz/tests/test_plugin_is_active.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/tests/test_subsets.py` & `jdaviz-3.9.1/jdaviz/tests/test_subsets.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/tests/test_user_api.py` & `jdaviz-3.9.1/jdaviz/tests/test_user_api.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/tests/test_utils.py` & `jdaviz-3.9.1/jdaviz/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/tests/test_viewer_ids.py` & `jdaviz-3.9.1/jdaviz/tests/test_viewer_ids.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz/utils.py` & `jdaviz-3.9.1/jdaviz/utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz.egg-info/PKG-INFO` & `jdaviz-3.9.1/jdaviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdaviz
-Version: 3.9.0
+Version: 3.9.1
 Summary: Astronomical data analysis development leveraging the Jupyter platform
 Author-email: JDADF Developers <help@stsci.edu>
 Project-URL: Homepage, https://jdaviz.readthedocs.io/en/latest/
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: packaging
```

### Comparing `jdaviz-3.9.0/jdaviz.egg-info/SOURCES.txt` & `jdaviz-3.9.1/jdaviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/jdaviz.egg-info/requires.txt` & `jdaviz-3.9.1/jdaviz.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/licenses/GINGA_LICENSE.txt` & `jdaviz-3.9.1/licenses/GINGA_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/licenses/IMEXAM_LICENSE.txt` & `jdaviz-3.9.1/licenses/IMEXAM_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/licenses/IPYFILECHOOSER_LICENSE.rst` & `jdaviz-3.9.1/licenses/IPYFILECHOOSER_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/licenses/TEMPLATE_LICENCE.rst` & `jdaviz-3.9.1/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/CubevizExample.ipynb` & `jdaviz-3.9.1/notebooks/CubevizExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/ImvizDitheredExample.ipynb` & `jdaviz-3.9.1/notebooks/ImvizDitheredExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/ImvizExample.ipynb` & `jdaviz-3.9.1/notebooks/ImvizExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/MosvizExample.ipynb` & `jdaviz-3.9.1/notebooks/MosvizExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/MosvizNIRISSExample.ipynb` & `jdaviz-3.9.1/notebooks/MosvizNIRISSExample.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976593501984127%*

 * *Differences: {"'cells'": '{8: {\'source\': {insert: [(0, "example_data = '*

 * *            '\'https://stsci.box.com/shared/static/txtjqn2wn0oowolf7pt4x11cz4w2x1ga.zip\'\\n")], '*

 * *            'delete: [0]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.9.7'}}"}*

```diff
@@ -90,15 +90,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2ac93c58",
             "metadata": {},
             "outputs": [],
             "source": [
-                "example_data = 'https://stsci.box.com/shared/static/k94suj9yv9vdbusmcdrcodhxt9urwevr.zip'\n",
+                "example_data = 'https://stsci.box.com/shared/static/txtjqn2wn0oowolf7pt4x11cz4w2x1ga.zip'\n",
                 "fn = download_file(example_data, cache=True)\n",
                 "with ZipFile(fn, 'r') as sample_data_zip:\n",
                 "    sample_data_zip.extractall(data_dir)\n",
                 "\n",
                 "level3_path = pathlib.Path(data_dir)\n",
                 "data_dir = level3_path"
             ]
@@ -255,13 +255,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.6"
+            "version": "3.9.7"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `jdaviz-3.9.0/notebooks/Specviz2dExample.ipynb` & `jdaviz-3.9.1/notebooks/Specviz2dExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/SpecvizExample.ipynb` & `jdaviz-3.9.1/notebooks/SpecvizExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/cubeviz_aperture_photometry.ipynb` & `jdaviz-3.9.1/notebooks/concepts/cubeviz_aperture_photometry.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/cubeviz_contour_overlay.ipynb` & `jdaviz-3.9.1/notebooks/concepts/cubeviz_contour_overlay.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/cubeviz_data_interactions.ipynb` & `jdaviz-3.9.1/notebooks/concepts/cubeviz_data_interactions.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/cubeviz_fitting.ipynb` & `jdaviz-3.9.1/notebooks/concepts/cubeviz_fitting.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/cubeviz_ndarray_gif.ipynb` & `jdaviz-3.9.1/notebooks/concepts/cubeviz_ndarray_gif.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/cubeviz_spectral_fitting.ipynb` & `jdaviz-3.9.1/notebooks/concepts/cubeviz_spectral_fitting.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb` & `jdaviz-3.9.1/notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb` & `jdaviz-3.9.1/notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/default_programmatic_viewers_from_blank.ipynb` & `jdaviz-3.9.1/notebooks/concepts/default_programmatic_viewers_from_blank.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/imviz_advanced_aper_phot.ipynb` & `jdaviz-3.9.1/notebooks/concepts/imviz_advanced_aper_phot.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/imviz_color_display.ipynb` & `jdaviz-3.9.1/notebooks/concepts/imviz_color_display.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/imviz_colorbar_mpl.ipynb` & `jdaviz-3.9.1/notebooks/concepts/imviz_colorbar_mpl.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/imviz_compass_mpl.ipynb` & `jdaviz-3.9.1/notebooks/concepts/imviz_compass_mpl.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/imviz_custom_colormap.ipynb` & `jdaviz-3.9.1/notebooks/concepts/imviz_custom_colormap.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/imviz_dithered_gwcs.ipynb` & `jdaviz-3.9.1/notebooks/concepts/imviz_dithered_gwcs.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/imviz_edit_subset_programmatic.ipynb` & `jdaviz-3.9.1/notebooks/concepts/imviz_edit_subset_programmatic.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/imviz_line_profiles.ipynb` & `jdaviz-3.9.1/notebooks/concepts/imviz_line_profiles.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/imviz_load_3d_slices.ipynb` & `jdaviz-3.9.1/notebooks/concepts/imviz_load_3d_slices.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/imviz_load_fits_hdu.ipynb` & `jdaviz-3.9.1/notebooks/concepts/imviz_load_fits_hdu.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/imviz_roman_asdf.ipynb` & `jdaviz-3.9.1/notebooks/concepts/imviz_roman_asdf.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/imviz_simple_aper_phot.ipynb` & `jdaviz-3.9.1/notebooks/concepts/imviz_simple_aper_phot.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/mosviz_concept.ipynb` & `jdaviz-3.9.1/notebooks/concepts/mosviz_concept.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/mosviz_generate_photometry.ipynb` & `jdaviz-3.9.1/notebooks/concepts/mosviz_generate_photometry.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/mosviz_niriss_parser.ipynb` & `jdaviz-3.9.1/notebooks/concepts/mosviz_niriss_parser.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/pypi_metrics.ipynb` & `jdaviz-3.9.1/notebooks/concepts/pypi_metrics.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/specviz_from_list.ipynb` & `jdaviz-3.9.1/notebooks/concepts/specviz_from_list.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/specviz_from_splot.ipynb` & `jdaviz-3.9.1/notebooks/concepts/specviz_from_splot.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/specviz_glue_unit_conversion.ipynb` & `jdaviz-3.9.1/notebooks/concepts/specviz_glue_unit_conversion.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/specviz_line_lists.ipynb` & `jdaviz-3.9.1/notebooks/concepts/specviz_line_lists.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/specviz_minimal.ipynb` & `jdaviz-3.9.1/notebooks/concepts/specviz_minimal.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/notebooks/concepts/specviz_spectrum_list.ipynb` & `jdaviz-3.9.1/notebooks/concepts/specviz_spectrum_list.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/pyproject.toml` & `jdaviz-3.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/setup.py` & `jdaviz-3.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/share/jupyter/nbconvert/templates/jdaviz-default/ansi.js` & `jdaviz-3.9.1/share/jupyter/nbconvert/templates/jdaviz-default/ansi.js`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/share/jupyter/nbconvert/templates/jdaviz-default/app.html` & `jdaviz-3.9.1/share/jupyter/nbconvert/templates/jdaviz-default/app.html`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2` & `jdaviz-3.9.1/share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/share/jupyter/nbconvert/templates/jdaviz-default/util.js` & `jdaviz-3.9.1/share/jupyter/nbconvert/templates/jdaviz-default/util.js`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/share/jupyter/voila/templates/jdaviz-default/index.html.j2` & `jdaviz-3.9.1/share/jupyter/voila/templates/jdaviz-default/index.html.j2`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/standalone/jdaviz-cli-entrypoint.py` & `jdaviz-3.9.1/standalone/jdaviz-cli-entrypoint.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/standalone/jdaviz.spec` & `jdaviz-3.9.1/standalone/jdaviz.spec`

 * *Files identical despite different names*

### Comparing `jdaviz-3.9.0/tox.ini` & `jdaviz-3.9.1/tox.ini`

 * *Files identical despite different names*


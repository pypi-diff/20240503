# Comparing `tmp/datumaro-1.6.1rc2.tar.gz` & `tmp/datumaro-1.6.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datumaro-1.6.1rc2.tar", last modified: Mon Apr 15 13:12:22 2024, max compression
+gzip compressed data, was "datumaro-1.6.1rc3.tar", last modified: Fri Apr 19 02:44:12 2024, max compression
```

## Comparing `datumaro-1.6.1rc2.tar` & `datumaro-1.6.1rc3.tar`

### file list

```diff
@@ -1,396 +1,396 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.677652 datumaro-1.6.1rc2/
--rw-r--r--   0 runner    (1001) docker     (127)   393113 2024-04-15 13:12:17.000000 datumaro-1.6.1rc2/3rd-party.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-15 13:12:17.000000 datumaro-1.6.1rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-15 13:12:17.000000 datumaro-1.6.1rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-15 13:12:17.000000 datumaro-1.6.1rc2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-04-15 13:12:22.673651 datumaro-1.6.1rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-15 13:12:17.000000 datumaro-1.6.1rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/requirements-core.txt
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/requirements-default.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.613651 datumaro-1.6.1rc2/rust/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/rust/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.613651 datumaro-1.6.1rc2/rust/src/
--rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/rust/src/coco_page_mapper.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/rust/src/datum_page_mapper.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/rust/src/json_section_page_mapper.rs
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/rust/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/rust/src/page_mapper.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/rust/src/page_maps.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/rust/src/utils.rs
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:12:22.677652 datumaro-1.6.1rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.601651 datumaro-1.6.1rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.613651 datumaro-1.6.1rc2/src/datumaro/
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.617651 datumaro-1.6.1rc2/src/datumaro/capi/
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/capi/pybind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.617651 datumaro-1.6.1rc2/src/datumaro/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.617651 datumaro-1.6.1rc2/src/datumaro/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/detect_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/explain.py
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/explore.py
--rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/prune.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.617651 datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.621651 datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/modification/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/modification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/modification/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/modification/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/modification/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/modification/import_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/modification/remove.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.621651 datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/versioning/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/versioning/checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/versioning/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/versioning/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/versioning/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/versioning/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     8383 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/commands/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.621651 datumaro-1.6.1rc2/src/datumaro/cli/contexts/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/contexts/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.621651 datumaro-1.6.1rc2/src/datumaro/cli/contexts/project/
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/contexts/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/contexts/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/contexts/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.621651 datumaro-1.6.1rc2/src/datumaro/cli/util/
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/util/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/cli/util/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.629651 datumaro-1.6.1rc2/src/datumaro/components/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.629651 datumaro-1.6.1rc2/src/datumaro/components/abstracts/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/abstracts/merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/abstracts/model_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.629651 datumaro-1.6.1rc2/src/datumaro/components/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.629651 datumaro-1.6.1rc2/src/datumaro/components/algorithms/hash_key_inference/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/algorithms/hash_key_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/algorithms/hash_key_inference/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/algorithms/hash_key_inference/explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    13546 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/algorithms/hash_key_inference/prune.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.629651 datumaro-1.6.1rc2/src/datumaro/components/algorithms/noisy_label_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/algorithms/noisy_label_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8957 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/algorithms/rise.py
--rw-r--r--   0 runner    (1001) docker     (127)    36472 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.629651 datumaro-1.6.1rc2/src/datumaro/components/annotations/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/annotations/matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/annotations/merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    25400 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/comparator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/config_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.629651 datumaro-1.6.1rc2/src/datumaro/components/contexts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/contexts/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/crypter.py
--rw-r--r--   0 runner    (1001) docker     (127)    34148 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/dataset_item_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    26104 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/dataset_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    18441 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    14785 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19922 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/extractor_tfds.py
--rw-r--r--   0 runner    (1001) docker     (127)    14541 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19999 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/format_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.633651 datumaro-1.6.1rc2/src/datumaro/components/hl_ops/
--rw-r--r--   0 runner    (1001) docker     (127)    15576 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/hl_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8271 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/lazy_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    41468 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/media.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.633651 datumaro-1.6.1rc2/src/datumaro/components/merge/
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/merge/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/merge/exact_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/merge/extractor_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    24403 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/merge/intersect_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/merge/union_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/progress_reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)    89550 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/shift_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    23697 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/components/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.633651 datumaro-1.6.1rc2/src/datumaro/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.633651 datumaro-1.6.1rc2/src/datumaro/plugins/accuracy_checker_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/accuracy_checker_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.637651 datumaro-1.6.1rc2/src/datumaro/plugins/accuracy_checker_plugin/details/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15491 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/anchor_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    37755 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/configurable_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.641651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/ade20k2017.py
--rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/ade20k2020.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.641651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/arrow/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/arrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/arrow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/arrow/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/arrow/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/arrow/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.645651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/arrow/mapper/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/arrow/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/arrow/mapper/media.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.645651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/ava/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/ava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/ava/ava.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/brats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/brats_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17865 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/camvid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.645651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/celeba/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/celeba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/celeba/align_celeba.py
--rw-r--r--   0 runner    (1001) docker     (127)    10889 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/celeba/celeba.py
--rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/cityscapes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.645651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/coco/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24813 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/coco/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    33535 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/coco/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/coco/extractor_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/coco/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/coco/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/coco/page_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/common_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/common_super_resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.645651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/cvat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/cvat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16158 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/cvat/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21501 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/cvat/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/cvat/format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.649651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18239 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    19062 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro/page_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.649651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.649651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.649651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/icdar/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/icdar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/icdar/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/icdar/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/icdar/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/image_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/image_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/imagenet_txt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.649651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kaggle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kaggle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kaggle/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kinetics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.653651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kitti/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kitti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kitti/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kitti/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kitti/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kitti/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.653651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kitti_raw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kitti_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11539 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kitti_raw/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17906 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kitti_raw/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kitti_raw/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    20219 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/labelme.py
--rw-r--r--   0 runner    (1001) docker     (127)    15274 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/lfw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.653651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mapillary_vistas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mapillary_vistas/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mapillary_vistas/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/market1501.py
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mmdet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mnist_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.653651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mpii/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mpii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mpii/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mpii/mpii_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mpii/mpii_mat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.657651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mvtec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mvtec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mvtec/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mvtec/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mvtec/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mvtec/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/nyu_depth_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    38893 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/open_images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.657651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/roboflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/roboflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10251 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/roboflow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/roboflow/base_tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/roboflow/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.657651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/segment_anything/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/segment_anything/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/segment_anything/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.657651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/sly_pointcloud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/sly_pointcloud/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16317 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/sly_pointcloud/format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.657651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/synthia/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/synthia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/synthia/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/synthia/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/synthia/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.657651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/tf_detection_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/tf_detection_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/tf_detection_api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/tf_detection_api/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    15800 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/vgg_face2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.661651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/voc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16675 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/voc/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    31405 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/voc/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10734 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/voc/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/voc/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/vott_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/vott_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/widerface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.661651 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/yolo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/yolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14467 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/yolo/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/yolo/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/yolo/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/yolo/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/framework_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.661651 datumaro-1.6.1rc2/src/datumaro/plugins/inference_server_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/inference_server_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/inference_server_plugin/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/inference_server_plugin/ovms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.661651 datumaro-1.6.1rc2/src/datumaro/plugins/inference_server_plugin/samples/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/inference_server_plugin/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/inference_server_plugin/triton.py
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/missing_annotation_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    16787 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/ndr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.661651 datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.665651 datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/samples/coco.class
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/samples/imagenet.class
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/samples/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/shift_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.665651 datumaro-1.6.1rc2/src/datumaro/plugins/sam_transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/sam_transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/sam_transforms/automatic_mask_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/sam_transforms/bbox_to_inst_mask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.665651 datumaro-1.6.1rc2/src/datumaro/plugins/sam_transforms/interpreters/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/sam_transforms/interpreters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_amg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/sam_transforms/interpreters/sam_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.665651 datumaro-1.6.1rc2/src/datumaro/plugins/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/sampler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.665651 datumaro-1.6.1rc2/src/datumaro/plugins/sampler/algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/sampler/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/sampler/algorithm/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/sampler/algorithm/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/sampler/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/sampler/relevancy_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    51884 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/specs.json
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/specs.py
--rw-r--r--   0 runner    (1001) docker     (127)    32124 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.669651 datumaro-1.6.1rc2/src/datumaro/plugins/synthetic_data/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/synthetic_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/synthetic_data/background_colors.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/synthetic_data/image_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/synthetic_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.669651 datumaro-1.6.1rc2/src/datumaro/plugins/tiling/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/tiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/tiling/merge_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/tiling/tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/tiling/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    50015 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    45116 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/plugins/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.673651 datumaro-1.6.1rc2/src/datumaro/util/
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/util/annotation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/util/attrs_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/util/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/util/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13348 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/util/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/util/image_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/util/import_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/util/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14465 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/util/mask_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/util/meta_file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/util/multi_procs_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/util/os_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/util/pickle_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/util/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/util/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/util/telemetry_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/util/telemetry_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/util/tf_util.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 13:12:18.000000 datumaro-1.6.1rc2/src/datumaro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:12:22.673651 datumaro-1.6.1rc2/src/datumaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-04-15 13:12:22.000000 datumaro-1.6.1rc2/src/datumaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15527 2024-04-15 13:12:22.000000 datumaro-1.6.1rc2/src/datumaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:12:22.000000 datumaro-1.6.1rc2/src/datumaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 13:12:22.000000 datumaro-1.6.1rc2/src/datumaro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:12:22.000000 datumaro-1.6.1rc2/src/datumaro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-15 13:12:22.000000 datumaro-1.6.1rc2/src/datumaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 13:12:22.000000 datumaro-1.6.1rc2/src/datumaro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.525696 datumaro-1.6.1rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)   393113 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/3rd-party.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-04-19 02:44:12.525696 datumaro-1.6.1rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/requirements-core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/requirements-default.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.465696 datumaro-1.6.1rc3/rust/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/rust/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.465696 datumaro-1.6.1rc3/rust/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/rust/src/coco_page_mapper.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/rust/src/datum_page_mapper.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/rust/src/json_section_page_mapper.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/rust/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/rust/src/page_mapper.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/rust/src/page_maps.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/rust/src/utils.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 02:44:12.525696 datumaro-1.6.1rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.457696 datumaro-1.6.1rc3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.469696 datumaro-1.6.1rc3/src/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.469696 datumaro-1.6.1rc3/src/datumaro/capi/
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/capi/pybind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.469696 datumaro-1.6.1rc3/src/datumaro/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.473696 datumaro-1.6.1rc3/src/datumaro/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/detect_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/explain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/prune.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.473696 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.473696 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/import_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.473696 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8383 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.477696 datumaro-1.6.1rc3/src/datumaro/cli/contexts/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/contexts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.477696 datumaro-1.6.1rc3/src/datumaro/cli/contexts/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/contexts/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/contexts/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/contexts/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.477696 datumaro-1.6.1rc3/src/datumaro/cli/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/util/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/util/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.481696 datumaro-1.6.1rc3/src/datumaro/components/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.481696 datumaro-1.6.1rc3/src/datumaro/components/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/abstracts/merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/abstracts/model_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.481696 datumaro-1.6.1rc3/src/datumaro/components/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.485696 datumaro-1.6.1rc3/src/datumaro/components/algorithms/hash_key_inference/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/algorithms/hash_key_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/algorithms/hash_key_inference/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/algorithms/hash_key_inference/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13546 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/algorithms/hash_key_inference/prune.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.485696 datumaro-1.6.1rc3/src/datumaro/components/algorithms/noisy_label_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/algorithms/noisy_label_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8957 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/algorithms/rise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36472 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.485696 datumaro-1.6.1rc3/src/datumaro/components/annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/annotations/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/annotations/merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25400 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/config_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.485696 datumaro-1.6.1rc3/src/datumaro/components/contexts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/contexts/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/crypter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34148 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/dataset_item_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26104 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/dataset_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18441 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14785 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19973 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/extractor_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14541 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19999 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/format_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.485696 datumaro-1.6.1rc3/src/datumaro/components/hl_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)    15576 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/hl_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8271 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/lazy_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41468 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/media.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.485696 datumaro-1.6.1rc3/src/datumaro/components/merge/
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/merge/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/merge/exact_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/merge/extractor_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24403 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/merge/intersect_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/merge/union_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/progress_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89550 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23697 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.489696 datumaro-1.6.1rc3/src/datumaro/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.489696 datumaro-1.6.1rc3/src/datumaro/plugins/accuracy_checker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/accuracy_checker_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.489696 datumaro-1.6.1rc3/src/datumaro/plugins/accuracy_checker_plugin/details/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15491 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/anchor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37755 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/configurable_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.497696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/ade20k2017.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/ade20k2020.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.497696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.497696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/mapper/media.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.497696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/ava/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/ava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/ava/ava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/brats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/brats_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17865 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/camvid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.497696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/celeba/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/celeba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/celeba/align_celeba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10889 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/celeba/celeba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cityscapes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.497696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24813 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33535 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/extractor_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/page_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/common_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/common_super_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.501696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cvat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cvat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16158 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cvat/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21501 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cvat/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cvat/format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.501696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18239 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19062 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/page_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.501696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.501696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.505696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/icdar/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/icdar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/icdar/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/icdar/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/icdar/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/image_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/image_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/imagenet_txt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.505696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kaggle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kaggle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kaggle/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.505696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.505696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti_raw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11539 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti_raw/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17906 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti_raw/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti_raw/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20219 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/labelme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15274 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/lfw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.505696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mapillary_vistas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mapillary_vistas/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mapillary_vistas/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/market1501.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mnist_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.505696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mpii/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mpii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mpii/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mpii/mpii_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mpii/mpii_mat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.509696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mvtec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mvtec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mvtec/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mvtec/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mvtec/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mvtec/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/nyu_depth_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38893 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/open_images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.509696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/roboflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/roboflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10251 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/roboflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/roboflow/base_tfrecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/roboflow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.509696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/segment_anything/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/segment_anything/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/segment_anything/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.509696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/sly_pointcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/sly_pointcloud/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16317 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/sly_pointcloud/format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.509696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/synthia/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/synthia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/synthia/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/synthia/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/synthia/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.509696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/tf_detection_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/tf_detection_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/tf_detection_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/tf_detection_api/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15800 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/vgg_face2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.513696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/voc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16675 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/voc/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31405 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/voc/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10734 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/voc/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/voc/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/vott_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/vott_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/widerface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.513696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/yolo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/yolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14467 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/yolo/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/yolo/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/yolo/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/yolo/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/framework_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.513696 datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/ovms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.513696 datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/triton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/missing_annotation_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16787 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/ndr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.513696 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.517696 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/coco.class
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/imagenet.class
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/shift_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.517696 datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/automatic_mask_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/bbox_to_inst_mask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.517696 datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/interpreters/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/interpreters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_amg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/interpreters/sam_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.517696 datumaro-1.6.1rc3/src/datumaro/plugins/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sampler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.517696 datumaro-1.6.1rc3/src/datumaro/plugins/sampler/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sampler/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sampler/algorithm/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sampler/algorithm/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sampler/relevancy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51901 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/specs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32124 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.521696 datumaro-1.6.1rc3/src/datumaro/plugins/synthetic_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/synthetic_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/synthetic_data/background_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/synthetic_data/image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/synthetic_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.521696 datumaro-1.6.1rc3/src/datumaro/plugins/tiling/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/tiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/tiling/merge_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/tiling/tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/tiling/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50015 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45116 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.525696 datumaro-1.6.1rc3/src/datumaro/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/annotation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/attrs_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13348 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/image_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/import_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14465 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/mask_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/meta_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/multi_procs_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/pickle_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/telemetry_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/telemetry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/tf_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.525696 datumaro-1.6.1rc3/src/datumaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-04-19 02:44:12.000000 datumaro-1.6.1rc3/src/datumaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15527 2024-04-19 02:44:12.000000 datumaro-1.6.1rc3/src/datumaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 02:44:12.000000 datumaro-1.6.1rc3/src/datumaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 02:44:12.000000 datumaro-1.6.1rc3/src/datumaro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 02:44:12.000000 datumaro-1.6.1rc3/src/datumaro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-19 02:44:12.000000 datumaro-1.6.1rc3/src/datumaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 02:44:12.000000 datumaro-1.6.1rc3/src/datumaro.egg-info/top_level.txt
```

### Comparing `datumaro-1.6.1rc2/3rd-party.txt` & `datumaro-1.6.1rc3/3rd-party.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/LICENSE` & `datumaro-1.6.1rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/PKG-INFO` & `datumaro-1.6.1rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.6.1rc2
+Version: 1.6.1rc3
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: attrs>=21.3.0
 Requires-Dist: defusedxml>=0.7.0
 Requires-Dist: h5py>=2.10.0
 Requires-Dist: imagesize>=1.4.1
-Requires-Dist: lxml==5.2.0
+Requires-Dist: lxml<6,>=5.2.0
 Requires-Dist: matplotlib>=3.3.1
 Requires-Dist: networkx>=2.6
 Requires-Dist: nibabel>=3.2.1
 Requires-Dist: numpy<2,>=1.23.4
 Requires-Dist: orjson==3.10.0
 Requires-Dist: Pillow>=10.2.0
 Requires-Dist: ruamel.yaml>=0.17.0
@@ -30,15 +30,15 @@
 Requires-Dist: pycocotools>=2.0.4; platform_system != "Windows" or python_version >= "3.9"
 Requires-Dist: pycocotools-windows; platform_system == "Windows" and python_version < "3.9"
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: tensorboardX!=2.3,>=1.8
 Requires-Dist: scipy
 Requires-Dist: requests
 Requires-Dist: pandas~=1.4.0
-Requires-Dist: openvino<2024.0.0,>=2023.2.0
+Requires-Dist: openvino>=2023.2.0
 Requires-Dist: tokenizers
 Requires-Dist: cryptography>=38.03
 Requires-Dist: pyemd
 Requires-Dist: pyarrow
 Requires-Dist: protobuf
 Requires-Dist: tabulate
 Requires-Dist: ovmsclient
```

### Comparing `datumaro-1.6.1rc2/README.md` & `datumaro-1.6.1rc3/README.md`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/pyproject.toml` & `datumaro-1.6.1rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/requirements-core.txt` & `datumaro-1.6.1rc3/requirements-core.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 attrs>=21.3.0
 defusedxml>=0.7.0
 h5py>=2.10.0
 imagesize>=1.4.1
-lxml==5.2.0
+lxml<6,>=5.2.0
 matplotlib>=3.3.1
 networkx>=2.6
 nibabel>=3.2.1
 numpy<2,>=1.23.4
 orjson==3.10.0
 Pillow>=10.2.0
 ruamel.yaml>=0.17.0
@@ -30,15 +30,15 @@
 # Image generator
 requests
 
 # Sampler
 pandas~=1.4.0
 
 # OpenVINO
-openvino>=2023.2.0,<2024.0.0 # Accuracy checker is deprecated >=2024.0.0
+openvino>=2023.2.0
 tokenizers
 
 # Encryption
 cryptography>= 38.03
 
 # Shift analyzer
 pyemd
```

### Comparing `datumaro-1.6.1rc2/rust/src/coco_page_mapper.rs` & `datumaro-1.6.1rc3/rust/src/coco_page_mapper.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/rust/src/datum_page_mapper.rs` & `datumaro-1.6.1rc3/rust/src/datum_page_mapper.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/rust/src/json_section_page_mapper.rs` & `datumaro-1.6.1rc3/rust/src/json_section_page_mapper.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/rust/src/lib.rs` & `datumaro-1.6.1rc3/rust/src/lib.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/rust/src/page_mapper.rs` & `datumaro-1.6.1rc3/rust/src/page_mapper.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/rust/src/page_maps.rs` & `datumaro-1.6.1rc3/rust/src/page_maps.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/rust/src/utils.rs` & `datumaro-1.6.1rc3/rust/src/utils.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/setup.py` & `datumaro-1.6.1rc3/setup.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/__init__.py` & `datumaro-1.6.1rc3/src/datumaro/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/capi/pybind.cpp` & `datumaro-1.6.1rc3/src/datumaro/capi/pybind.cpp`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/__main__.py` & `datumaro-1.6.1rc3/src/datumaro/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/__init__.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/compare.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/compare.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/convert.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/convert.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/detect_format.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/detect_format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/download.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/explain.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/explain.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/explore.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/explore.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/filter.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/generate.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/info.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/merge.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/patch.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/patch.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/prune.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/prune.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/__init__.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/modification/add.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/add.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/modification/create.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/create.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/modification/export.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/export.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/modification/import_.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/import_.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/modification/remove.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/remove.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/versioning/checkout.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/checkout.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/versioning/commit.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/commit.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/versioning/info.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/versioning/log.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/log.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/require_project/versioning/status.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/status.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/stats.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/stats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/transform.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/transform.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/commands/validate.py` & `datumaro-1.6.1rc3/src/datumaro/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/contexts/model.py` & `datumaro-1.6.1rc3/src/datumaro/cli/contexts/model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/contexts/project/__init__.py` & `datumaro-1.6.1rc3/src/datumaro/cli/contexts/project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/contexts/source.py` & `datumaro-1.6.1rc3/src/datumaro/cli/contexts/source.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/contexts/util.py` & `datumaro-1.6.1rc3/src/datumaro/cli/contexts/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/util/__init__.py` & `datumaro-1.6.1rc3/src/datumaro/cli/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/util/compare.py` & `datumaro-1.6.1rc3/src/datumaro/cli/util/compare.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/cli/util/project.py` & `datumaro-1.6.1rc3/src/datumaro/cli/util/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/abstracts/merger.py` & `datumaro-1.6.1rc3/src/datumaro/components/abstracts/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/abstracts/model_interpreter.py` & `datumaro-1.6.1rc3/src/datumaro/components/abstracts/model_interpreter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/algorithms/hash_key_inference/base.py` & `datumaro-1.6.1rc3/src/datumaro/components/algorithms/hash_key_inference/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/algorithms/hash_key_inference/explorer.py` & `datumaro-1.6.1rc3/src/datumaro/components/algorithms/hash_key_inference/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py` & `datumaro-1.6.1rc3/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/algorithms/hash_key_inference/prune.py` & `datumaro-1.6.1rc3/src/datumaro/components/algorithms/hash_key_inference/prune.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py` & `datumaro-1.6.1rc3/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/algorithms/rise.py` & `datumaro-1.6.1rc3/src/datumaro/components/algorithms/rise.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/annotation.py` & `datumaro-1.6.1rc3/src/datumaro/components/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/annotations/matcher.py` & `datumaro-1.6.1rc3/src/datumaro/components/annotations/matcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/annotations/merger.py` & `datumaro-1.6.1rc3/src/datumaro/components/annotations/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/cli_plugin.py` & `datumaro-1.6.1rc3/src/datumaro/components/cli_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/comparator.py` & `datumaro-1.6.1rc3/src/datumaro/components/comparator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/config.py` & `datumaro-1.6.1rc3/src/datumaro/components/config.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/config_model.py` & `datumaro-1.6.1rc3/src/datumaro/components/config_model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/contexts/importer.py` & `datumaro-1.6.1rc3/src/datumaro/components/contexts/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/crypter.py` & `datumaro-1.6.1rc3/src/datumaro/components/crypter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/dataset.py` & `datumaro-1.6.1rc3/src/datumaro/components/dataset.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/dataset_base.py` & `datumaro-1.6.1rc3/src/datumaro/components/dataset_base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/dataset_item_storage.py` & `datumaro-1.6.1rc3/src/datumaro/components/dataset_item_storage.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/dataset_storage.py` & `datumaro-1.6.1rc3/src/datumaro/components/dataset_storage.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/environment.py` & `datumaro-1.6.1rc3/src/datumaro/components/environment.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/errors.py` & `datumaro-1.6.1rc3/src/datumaro/components/errors.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/exporter.py` & `datumaro-1.6.1rc3/src/datumaro/components/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/extractor_tfds.py` & `datumaro-1.6.1rc3/src/datumaro/components/extractor_tfds.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021-2023 Intel Corporation
+# Copyright (C) 2024 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import itertools
 import logging as log
@@ -26,31 +26,31 @@
 import attrs
 import numpy as np
 from attrs import field, frozen
 
 from datumaro.components.annotation import AnnotationType, Bbox, Label, LabelCategories
 from datumaro.components.dataset_base import CategoriesInfo, DatasetInfo, DatasetItem, IDataset
 from datumaro.components.media import Image, MediaElement
+from datumaro.util.import_util import lazy_import
 from datumaro.util.tf_util import import_tf
 
 TFDS_EXTRACTOR_AVAILABLE = True if find_spec("tensorflow_datasets") is not None else False
 
-if TYPE_CHECKING:
+if TFDS_EXTRACTOR_AVAILABLE:
     try:
-        tf = import_tf()
-        import tensorflow_datasets as tfds
+        if TYPE_CHECKING:
+            tf = import_tf()
+            import tensorflow_datasets as tfds
+        else:
+            tfds = lazy_import("tensorflow_datasets")
     except ImportError:
         log.debug(
             "Unable to import TensorFlow or TensorFlow Datasets. "
             "Dataset downloading via TFDS is disabled."
         )
-else:
-    from datumaro.util.import_util import lazy_import
-
-    tfds = lazy_import("tensorflow_datasets")
 
 
 @frozen(kw_only=True)
 class TfdsDatasetMetadata:
     # If you add attributes to this class, make sure to update the reporting logic
     # in the `describe-downloads` command to include them.
```

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/filter.py` & `datumaro-1.6.1rc3/src/datumaro/components/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/format_detection.py` & `datumaro-1.6.1rc3/src/datumaro/components/format_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/generator.py` & `datumaro-1.6.1rc3/src/datumaro/components/generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/hl_ops/__init__.py` & `datumaro-1.6.1rc3/src/datumaro/components/hl_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/importer.py` & `datumaro-1.6.1rc3/src/datumaro/components/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/launcher.py` & `datumaro-1.6.1rc3/src/datumaro/components/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/lazy_plugin.py` & `datumaro-1.6.1rc3/src/datumaro/components/lazy_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/media.py` & `datumaro-1.6.1rc3/src/datumaro/components/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/merge/__init__.py` & `datumaro-1.6.1rc3/src/datumaro/components/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/merge/base.py` & `datumaro-1.6.1rc3/src/datumaro/components/merge/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/merge/exact_merge.py` & `datumaro-1.6.1rc3/src/datumaro/components/merge/exact_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/merge/extractor_merger.py` & `datumaro-1.6.1rc3/src/datumaro/components/merge/extractor_merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/merge/intersect_merge.py` & `datumaro-1.6.1rc3/src/datumaro/components/merge/intersect_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/merge/union_merge.py` & `datumaro-1.6.1rc3/src/datumaro/components/merge/union_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/operations.py` & `datumaro-1.6.1rc3/src/datumaro/components/operations.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/progress_reporting.py` & `datumaro-1.6.1rc3/src/datumaro/components/progress_reporting.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/project.py` & `datumaro-1.6.1rc3/src/datumaro/components/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/registry.py` & `datumaro-1.6.1rc3/src/datumaro/components/registry.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/shift_analyzer.py` & `datumaro-1.6.1rc3/src/datumaro/components/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/transformer.py` & `datumaro-1.6.1rc3/src/datumaro/components/transformer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/validator.py` & `datumaro-1.6.1rc3/src/datumaro/components/validator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/components/visualizer.py` & `datumaro-1.6.1rc3/src/datumaro/components/visualizer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from datumaro.components.cli_plugin import CliPlugin
 from datumaro.components.launcher import Launcher
 from datumaro.components.lazy_plugin import extra_deps
 
 from .details.ac import GenericAcLauncher as _GenericAcLauncher
 
 
-@extra_deps("openvino.tools", "tensorflow")
+@extra_deps("tensorflow", "openvino.tools.accuracy_checker")
 class AcLauncher(Launcher, CliPlugin):
     """
     Generic model launcher with Accuracy Checker backend.
     """
 
     @classmethod
     def build_cmdline_parser(cls, **kwargs):
```

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,112 +1,121 @@
 # Copyright (C) 2020-2021 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 from itertools import groupby
 
-from openvino.tools.accuracy_checker.adapters import create_adapter
-from openvino.tools.accuracy_checker.data_readers import DataRepresentation
-from openvino.tools.accuracy_checker.launcher import InputFeeder, create_launcher
-from openvino.tools.accuracy_checker.postprocessor import PostprocessingExecutor
-from openvino.tools.accuracy_checker.preprocessor import PreprocessingExecutor
-from openvino.tools.accuracy_checker.utils import extract_image_representations
-
 from datumaro.components.annotation import AnnotationType, LabelCategories
 
 from .representation import import_predictions
 
-
-class _FakeDataset:
-    def __init__(self, metadata=None):
-        self.metadata = metadata or {}
-
-
-class GenericAcLauncher:
-    @staticmethod
-    def from_config(config):
-        launcher_config = config["launcher"]
-        launcher = create_launcher(launcher_config)
-
-        dataset = _FakeDataset()
-        adapter_config = config.get("adapter") or launcher_config.get("adapter")
-        label_config = adapter_config.get("labels") if isinstance(adapter_config, dict) else None
-        if label_config:
-            assert isinstance(label_config, (list, dict))
-            if isinstance(label_config, list):
-                label_config = dict(enumerate(label_config))
-
-            dataset.metadata = {
-                "label_map": {int(key): label for key, label in label_config.items()}
-            }
-        adapter = create_adapter(adapter_config, launcher, dataset)
-
-        preproc_config = config.get("preprocessing")
-        preproc = None
-        if preproc_config:
-            preproc = PreprocessingExecutor(
-                preproc_config,
-                dataset_meta=dataset.metadata,
-                input_shapes=launcher.inputs_info_for_meta(),
+try:
+    from openvino.tools.accuracy_checker.adapters import create_adapter
+    from openvino.tools.accuracy_checker.data_readers import DataRepresentation
+    from openvino.tools.accuracy_checker.launcher import InputFeeder, create_launcher
+    from openvino.tools.accuracy_checker.postprocessor import PostprocessingExecutor
+    from openvino.tools.accuracy_checker.preprocessor import PreprocessingExecutor
+    from openvino.tools.accuracy_checker.utils import extract_image_representations
+
+    class _FakeDataset:
+        def __init__(self, metadata=None):
+            self.metadata = metadata or {}
+
+    class GenericAcLauncher:
+        @staticmethod
+        def from_config(config):
+            launcher_config = config["launcher"]
+            launcher = create_launcher(launcher_config)
+
+            dataset = _FakeDataset()
+            adapter_config = config.get("adapter") or launcher_config.get("adapter")
+            label_config = (
+                adapter_config.get("labels") if isinstance(adapter_config, dict) else None
             )
-
-        postproc_config = config.get("postprocessing")
-        postproc = None
-        if postproc_config:
-            postproc = PostprocessingExecutor(
-                postproc_config,
-                dataset_meta=dataset.metadata,
+            if label_config:
+                assert isinstance(label_config, (list, dict))
+                if isinstance(label_config, list):
+                    label_config = dict(enumerate(label_config))
+
+                dataset.metadata = {
+                    "label_map": {int(key): label for key, label in label_config.items()}
+                }
+            adapter = create_adapter(adapter_config, launcher, dataset)
+
+            preproc_config = config.get("preprocessing")
+            preproc = None
+            if preproc_config:
+                preproc = PreprocessingExecutor(
+                    preproc_config,
+                    dataset_meta=dataset.metadata,
+                    input_shapes=launcher.inputs_info_for_meta(),
+                )
+
+            postproc_config = config.get("postprocessing")
+            postproc = None
+            if postproc_config:
+                postproc = PostprocessingExecutor(
+                    postproc_config,
+                    dataset_meta=dataset.metadata,
+                )
+
+            return __class__(launcher, adapter=adapter, preproc=preproc, postproc=postproc)
+
+        def __init__(self, launcher, adapter=None, preproc=None, postproc=None, input_feeder=None):
+            self._launcher = launcher
+            self._input_feeder = input_feeder or InputFeeder(
+                launcher.config.get("inputs", []),
+                launcher.inputs,
+                launcher.fit_to_input,
+                launcher.default_layout,
             )
+            self._adapter = adapter
+            self._preproc = preproc
+            self._postproc = postproc
 
-        return __class__(launcher, adapter=adapter, preproc=preproc, postproc=postproc)
+            self._categories = self._init_categories()
 
-    def __init__(self, launcher, adapter=None, preproc=None, postproc=None, input_feeder=None):
-        self._launcher = launcher
-        self._input_feeder = input_feeder or InputFeeder(
-            launcher.config.get("inputs", []),
-            launcher.inputs,
-            launcher.fit_to_input,
-            launcher.default_layout,
-        )
-        self._adapter = adapter
-        self._preproc = preproc
-        self._postproc = postproc
+        def launch_raw(self, inputs):
+            ids = range(len(inputs))
+            inputs = [DataRepresentation(inp, identifier=id) for id, inp in zip(ids, inputs)]
+            _, batch_meta = extract_image_representations(inputs)
 
-        self._categories = self._init_categories()
+            if self._preproc:
+                inputs = self._preproc.process(inputs)
 
-    def launch_raw(self, inputs):
-        ids = range(len(inputs))
-        inputs = [DataRepresentation(inp, identifier=id) for id, inp in zip(ids, inputs)]
-        _, batch_meta = extract_image_representations(inputs)
+            inputs = self._input_feeder.fill_inputs(inputs)
+            outputs = self._launcher.predict(inputs, batch_meta)
 
-        if self._preproc:
-            inputs = self._preproc.process(inputs)
+            if self._adapter:
+                outputs = self._adapter.process(outputs, ids, batch_meta)
 
-        inputs = self._input_feeder.fill_inputs(inputs)
-        outputs = self._launcher.predict(inputs, batch_meta)
+            if self._postproc:
+                outputs = self._postproc.process(outputs)
 
-        if self._adapter:
-            outputs = self._adapter.process(outputs, ids, batch_meta)
+            return outputs
 
-        if self._postproc:
-            outputs = self._postproc.process(outputs)
+        def launch(self, inputs):
+            outputs = self.launch_raw(inputs)
+            return [import_predictions(g) for _, g in groupby(outputs, key=lambda o: o.identifier)]
 
-        return outputs
+        def categories(self):
+            return self._categories
 
-    def launch(self, inputs):
-        outputs = self.launch_raw(inputs)
-        return [import_predictions(g) for _, g in groupby(outputs, key=lambda o: o.identifier)]
+        def _init_categories(self):
+            if self._adapter is None or self._adapter.label_map is None:
+                return None
 
-    def categories(self):
-        return self._categories
+            label_map = sorted(self._adapter.label_map.items(), key=lambda e: e[0])
 
-    def _init_categories(self):
-        if self._adapter is None or self._adapter.label_map is None:
-            return None
+            label_cat = LabelCategories()
+            for _, label in label_map:
+                label_cat.add(label)
 
-        label_map = sorted(self._adapter.label_map.items(), key=lambda e: e[0])
+            return {AnnotationType.label: label_cat}
 
-        label_cat = LabelCategories()
-        for _, label in label_map:
-            label_cat.add(label)
+except ImportError:
 
-        return {AnnotationType.label: label_cat}
+    class GenericAcLauncher:
+        def __init__(self):
+            raise ImportError(
+                "Accuracy Checker was deprecated from OpenVINO 2024.0. Please use lower OpenVINO version."
+            )
```

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/anchor_generator.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/configurable_validator.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/configurable_validator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/ade20k2017.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/ade20k2017.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/ade20k2020.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/ade20k2020.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/arrow/base.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/arrow/exporter.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/arrow/format.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/arrow/importer.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/arrow/mapper/media.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/ava/ava.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/ava/ava.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/brats.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/brats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/brats_numpy.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/brats_numpy.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/camvid.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/camvid.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/celeba/align_celeba.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/celeba/align_celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/celeba/celeba.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/celeba/celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/cifar.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cifar.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/cityscapes.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cityscapes.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/coco/base.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/coco/exporter.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/coco/extractor_merger.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/extractor_merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/coco/format.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/coco/importer.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/coco/page_mapper.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/page_mapper.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/common_semantic_segmentation.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/common_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/common_super_resolution.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/common_super_resolution.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/cvat/base.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cvat/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/cvat/exporter.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cvat/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/cvat/format.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cvat/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro/base.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro/exporter.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro/importer.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro/page_mapper.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/page_mapper.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/base.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/format.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/importer.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/icdar/base.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/icdar/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/icdar/exporter.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/icdar/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/image_dir.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/image_dir.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/image_zip.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/image_zip.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/imagenet.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/imagenet.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/imagenet_txt.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/imagenet_txt.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kaggle/base.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kaggle/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kinetics.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kinetics.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kitti/base.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kitti/exporter.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kitti/format.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kitti/importer.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kitti_raw/base.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti_raw/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kitti_raw/exporter.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti_raw/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/kitti_raw/format.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti_raw/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/labelme.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/labelme.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/lfw.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/lfw.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mapillary_vistas/base.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mapillary_vistas/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mapillary_vistas/format.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mapillary_vistas/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/market1501.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/market1501.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mars.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mars.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mmdet.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mmdet.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mnist.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mnist.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mnist_csv.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mnist_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mot.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mot.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mots.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mots.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mpii/format.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mpii/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mpii/mpii_json.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mpii/mpii_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mpii/mpii_mat.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mpii/mpii_mat.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mvtec/base.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mvtec/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mvtec/exporter.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mvtec/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mvtec/format.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mvtec/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/mvtec/importer.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mvtec/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/nyu_depth_v2.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/nyu_depth_v2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/open_images.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/open_images.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/roboflow/base.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/roboflow/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/roboflow/base_tfrecord.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/roboflow/base_tfrecord.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/roboflow/importer.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/roboflow/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/segment_anything/base.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/segment_anything/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/segment_anything/exporter.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/segment_anything/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/segment_anything/importer.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/segment_anything/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/sly_pointcloud/base.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/sly_pointcloud/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/synthia/base.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/synthia/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/synthia/format.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/synthia/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/synthia/importer.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/synthia/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/tabular.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/tabular.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/tf_detection_api/base.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/tf_detection_api/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/vgg_face2.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/vgg_face2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/video.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/video.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/voc/base.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/voc/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/voc/exporter.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/voc/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/voc/format.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/voc/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/voc/importer.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/voc/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/vott_csv.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/vott_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/vott_json.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/vott_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/widerface.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/widerface.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/yolo/base.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/yolo/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/yolo/exporter.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/yolo/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/yolo/format.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/yolo/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/data_formats/yolo/importer.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/yolo/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/explorer.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/framework_converter.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/framework_converter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/inference_server_plugin/base.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/inference_server_plugin/ovms.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/ovms.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/inference_server_plugin/triton.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/triton.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/missing_annotation_detection.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/missing_annotation_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/ndr.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/ndr.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/launcher.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/samples/coco.class` & `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/coco.class`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/samples/imagenet.class` & `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/imagenet.class`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/samples/utils.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/openvino_plugin/shift_launcher.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/shift_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/sam_transforms/automatic_mask_gen.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/automatic_mask_gen.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/sam_transforms/bbox_to_inst_mask.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/bbox_to_inst_mask.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_amg.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_amg.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_bbox.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_bbox.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/sam_transforms/interpreters/sam_encoder.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/interpreters/sam_encoder.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/sampler/algorithm/algorithm.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/sampler/algorithm/algorithm.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/sampler/algorithm/entropy.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/sampler/algorithm/entropy.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/sampler/random_sampler.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/sampler/random_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/sampler/relevancy_sampler.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/sampler/relevancy_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/specs.json` & `datumaro-1.6.1rc3/src/datumaro/plugins/specs.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996958637469585%*

 * *Differences: {'0': "{'extra_deps': {insert: [(1, 'openvino.tools.accuracy_checker')], delete: [0]}}"}*

```diff
@@ -1,12 +1,12 @@
 [
     {
         "extra_deps": [
-            "openvino.tools",
-            "tensorflow"
+            "tensorflow",
+            "openvino.tools.accuracy_checker"
         ],
         "import_path": "datumaro.plugins.accuracy_checker_plugin.ac_launcher.AcLauncher",
         "plugin_name": "ac",
         "plugin_type": "Launcher"
     },
     {
         "import_path": "datumaro.plugins.configurable_validator.ConfigurableValidator",
```

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/specs.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/specs.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/splitter.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/splitter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/synthetic_data/background_colors.txt` & `datumaro-1.6.1rc3/src/datumaro/plugins/synthetic_data/background_colors.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/synthetic_data/image_generator.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/synthetic_data/image_generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/synthetic_data/utils.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/synthetic_data/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/tiling/merge_tile.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/tiling/merge_tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/tiling/tile.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/tiling/tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/tiling/util.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/tiling/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/transforms.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/transforms.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/plugins/validators.py` & `datumaro-1.6.1rc3/src/datumaro/plugins/validators.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/util/__init__.py` & `datumaro-1.6.1rc3/src/datumaro/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/util/annotation_util.py` & `datumaro-1.6.1rc3/src/datumaro/util/annotation_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/util/attrs_util.py` & `datumaro-1.6.1rc3/src/datumaro/util/attrs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/util/definitions.py` & `datumaro-1.6.1rc3/src/datumaro/util/definitions.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/util/file_utils.py` & `datumaro-1.6.1rc3/src/datumaro/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/util/image.py` & `datumaro-1.6.1rc3/src/datumaro/util/image.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/util/image_cache.py` & `datumaro-1.6.1rc3/src/datumaro/util/image_cache.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/util/log_utils.py` & `datumaro-1.6.1rc3/src/datumaro/util/log_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/util/mask_tools.py` & `datumaro-1.6.1rc3/src/datumaro/util/mask_tools.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/util/meta_file_util.py` & `datumaro-1.6.1rc3/src/datumaro/util/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/util/multi_procs_util.py` & `datumaro-1.6.1rc3/src/datumaro/util/multi_procs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/util/os_util.py` & `datumaro-1.6.1rc3/src/datumaro/util/os_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/util/pickle_util.py` & `datumaro-1.6.1rc3/src/datumaro/util/pickle_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/util/scope.py` & `datumaro-1.6.1rc3/src/datumaro/util/scope.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/util/telemetry_stub.py` & `datumaro-1.6.1rc3/src/datumaro/util/telemetry_stub.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/util/telemetry_utils.py` & `datumaro-1.6.1rc3/src/datumaro/util/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro/util/tf_util.py` & `datumaro-1.6.1rc3/src/datumaro/util/tf_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro.egg-info/PKG-INFO` & `datumaro-1.6.1rc3/src/datumaro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.6.1rc2
+Version: 1.6.1rc3
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: attrs>=21.3.0
 Requires-Dist: defusedxml>=0.7.0
 Requires-Dist: h5py>=2.10.0
 Requires-Dist: imagesize>=1.4.1
-Requires-Dist: lxml==5.2.0
+Requires-Dist: lxml<6,>=5.2.0
 Requires-Dist: matplotlib>=3.3.1
 Requires-Dist: networkx>=2.6
 Requires-Dist: nibabel>=3.2.1
 Requires-Dist: numpy<2,>=1.23.4
 Requires-Dist: orjson==3.10.0
 Requires-Dist: Pillow>=10.2.0
 Requires-Dist: ruamel.yaml>=0.17.0
@@ -30,15 +30,15 @@
 Requires-Dist: pycocotools>=2.0.4; platform_system != "Windows" or python_version >= "3.9"
 Requires-Dist: pycocotools-windows; platform_system == "Windows" and python_version < "3.9"
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: tensorboardX!=2.3,>=1.8
 Requires-Dist: scipy
 Requires-Dist: requests
 Requires-Dist: pandas~=1.4.0
-Requires-Dist: openvino<2024.0.0,>=2023.2.0
+Requires-Dist: openvino>=2023.2.0
 Requires-Dist: tokenizers
 Requires-Dist: cryptography>=38.03
 Requires-Dist: pyemd
 Requires-Dist: pyarrow
 Requires-Dist: protobuf
 Requires-Dist: tabulate
 Requires-Dist: ovmsclient
```

### Comparing `datumaro-1.6.1rc2/src/datumaro.egg-info/SOURCES.txt` & `datumaro-1.6.1rc3/src/datumaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc2/src/datumaro.egg-info/requires.txt` & `datumaro-1.6.1rc3/src/datumaro.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 attrs>=21.3.0
 defusedxml>=0.7.0
 h5py>=2.10.0
 imagesize>=1.4.1
-lxml==5.2.0
+lxml<6,>=5.2.0
 matplotlib>=3.3.1
 networkx>=2.6
 nibabel>=3.2.1
 numpy<2,>=1.23.4
 orjson==3.10.0
 Pillow>=10.2.0
 ruamel.yaml>=0.17.0
@@ -14,15 +14,15 @@
 typing_extensions>=3.7.4.3
 tqdm
 PyYAML==6.0.1
 tensorboardX!=2.3,>=1.8
 scipy
 requests
 pandas~=1.4.0
-openvino<2024.0.0,>=2023.2.0
+openvino>=2023.2.0
 tokenizers
 cryptography>=38.03
 pyemd
 pyarrow
 protobuf
 tabulate
 ovmsclient
```


# Comparing `tmp/anemoi-datasets-0.1.4.tar.gz` & `tmp/anemoi_datasets-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemoi-datasets-0.1.4.tar", last modified: Mon Apr 29 09:36:45 2024, max compression
+gzip compressed data, was "anemoi_datasets-0.1.6.tar", last modified: Fri May  3 17:17:26 2024, max compression
```

## Comparing `anemoi-datasets-0.1.4.tar` & `anemoi_datasets-0.1.6.tar`

### file list

```diff
@@ -1,84 +1,280 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.453787 anemoi-datasets-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-29 09:36:45.453787 anemoi-datasets-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.441787 anemoi-datasets-0.1.4/anemoi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.445787 anemoi-datasets-0.1.4/anemoi/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.445787 anemoi-datasets-0.1.4/anemoi/datasets/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/commands/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/commands/copy.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/commands/create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.445787 anemoi-datasets-0.1.4/anemoi/datasets/commands/inspect/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/commands/inspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19684 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/commands/inspect/zarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/commands/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.449787 anemoi-datasets-0.1.4/anemoi/datasets/create/
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.449787 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.449787 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12520 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/accumulations.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/forcings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/grib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/mars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/netcdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/opendap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/perturbations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/tendencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.449787 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/noop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/rename.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/rotate_winds.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/unrotate_winds.py
--rw-r--r--   0 runner    (1001) docker     (127)    27846 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/input.py
--rw-r--r--   0 runner    (1001) docker     (127)    20490 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/loaders.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3682 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12690 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/zarr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.453787 anemoi-datasets-0.1.4/anemoi/datasets/data/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/forewards.py
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/grids.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/join.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/masked.py
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10121 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/stores.py
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/subset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/unchecked.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.453787 anemoi-datasets-0.1.4/anemoi/datasets/dates/
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/dates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/dates/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/grids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.453787 anemoi-datasets-0.1.4/anemoi/datasets/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.453787 anemoi-datasets-0.1.4/anemoi_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-29 09:36:45.000000 anemoi-datasets-0.1.4/anemoi_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-29 09:36:45.000000 anemoi-datasets-0.1.4/anemoi_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 09:36:45.000000 anemoi-datasets-0.1.4/anemoi_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-29 09:36:45.000000 anemoi-datasets-0.1.4/anemoi_datasets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-29 09:36:45.000000 anemoi-datasets-0.1.4/anemoi_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 09:36:45.000000 anemoi-datasets-0.1.4/anemoi_datasets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 09:36:45.000000 anemoi-datasets-0.1.4/anemoi_datasets.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 09:36:45.453787 anemoi-datasets-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.928238 anemoi_datasets-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.876238 anemoi_datasets-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.884238 anemoi_datasets-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.884238 anemoi_datasets-0.1.6/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/.vscode/spellright.dict
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15615 2024-05-03 17:17:26.928238 anemoi_datasets-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.884238 anemoi_datasets-0.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.884238 anemoi_datasets-0.1.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.884238 anemoi_datasets-0.1.6/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/_templates/.gitkeep
+-rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/apply-fmt.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.888238 anemoi_datasets-0.1.6/docs/building/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.888238 anemoi_datasets-0.1.6/docs/building/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/filters/empty.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/filters/noop.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/filters/rename.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/filters/rotate_winds.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/filters/select.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/filters/unrotate_winds.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/filters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/handling-missing-dates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/handling-missing-values.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/naming-variables.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/operations.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.888238 anemoi_datasets-0.1.6/docs/building/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/sources/accumulations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/sources/accumulations1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/sources/accumulations2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/sources/forcings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/sources/forcings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/sources/grib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/sources/mars.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/sources/mars1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/sources/mars2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/sources/netcdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/sources/netcdf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/sources/opendap.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/sources/opendap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/sources/perturbations.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.892238 anemoi_datasets-0.1.6/docs/building/sources/yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/sources/yaml/grib1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/sources/yaml/grib2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/sources/yaml/grib3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/sources/yaml/grib4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/sources/yaml/perturbations.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/sources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/statistics.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/syntax.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/syntax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.892238 anemoi_datasets-0.1.6/docs/building/yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/yaml/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/yaml/building1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/yaml/building1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/yaml/building2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/yaml/building2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/yaml/building3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/yaml/building3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/yaml/concat.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/yaml/input.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/yaml/missing_dates.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/building/yaml/pipe.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/check-index.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.892238 anemoi_datasets-0.1.6/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/cli/compare.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/cli/copy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/cli/create.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/cli/inspect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/cli/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58982 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/images.pptx
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/overview_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.896238 anemoi_datasets-0.1.6/docs/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)   106709 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/schemas/matrix.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (127)    53069 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/schemas/matrix.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/schemas/overview.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/schemas/overview.png
+-rw-r--r--   0 runner    (1001) docker     (127)    42125 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/schemas/recipe.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (127)    43845 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/schemas/recipe.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/test.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.896238 anemoi_datasets-0.1.6/docs/using/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.904238 anemoi_datasets-0.1.6/docs/using/code/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/area1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/area2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/chain_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/combine_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/concat1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/cutout_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/drop_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/end_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/ensembles1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/frequency_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/grids1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/join1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/matching0_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/matching1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/matching2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/matching3_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/matching4_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/misc1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/misc2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/missing_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/open_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/open_combine1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/open_combine2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/open_complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/open_dict_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/open_first_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/open_list_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/open_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/open_other.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/open_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/open_yaml_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/rename_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/reorder1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/reorder2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/select1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/select2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/shuffle_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/some_attributes_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/start_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/statistics_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/subset_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/thinning_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/zip1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/code/zip2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/combining.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/configuration.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/grids.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.908238 anemoi_datasets-0.1.6/docs/using/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   108038 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/images/area-1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    40564 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/images/concat.png
+-rw-r--r--   0 runner    (1001) docker     (127)   141221 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/images/cutout-1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   122139 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/images/cutout-2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   129758 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/images/cutout-3.png
+-rw-r--r--   0 runner    (1001) docker     (127)   151858 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/images/cutout-4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38066 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/images/join.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36070 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/images/overlay.png
+-rw-r--r--   0 runner    (1001) docker     (127)   109206 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/images/thinning-after.png
+-rw-r--r--   0 runner    (1001) docker     (127)   141221 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/images/thinning-before.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/matching.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/methods.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/miscellaneous.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/opening.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/other.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/selecting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/statistics.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/docs/using/subsetting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:17:26.928238 anemoi_datasets-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.880238 anemoi_datasets-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.880238 anemoi_datasets-0.1.6/src/anemoi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.908238 anemoi_datasets-0.1.6/src/anemoi/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 17:17:26.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.908238 anemoi_datasets-0.1.6/src/anemoi/datasets/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/commands/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/commands/copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/commands/create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.908238 anemoi_datasets-0.1.6/src/anemoi/datasets/commands/inspect/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/commands/inspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19684 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/commands/inspect/zarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/commands/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.908238 anemoi_datasets-0.1.6/src/anemoi/datasets/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/compute/perturbations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.912238 anemoi_datasets-0.1.6/src/anemoi/datasets/create/
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.912238 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.912238 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/filters/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/filters/noop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/filters/rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/filters/rotate_winds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/filters/unrotate_winds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.916238 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12520 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/accumulations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/forcings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/grib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/mars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/opendap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/tendencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27981 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28020 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/loaders.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3682 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/size.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.916238 anemoi_datasets-0.1.6/src/anemoi/datasets/create/statistics/
+-rw-r--r--   0 runner    (1001) docker     (127)    15388 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/statistics/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/create/zarr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.920238 anemoi_datasets-0.1.6/src/anemoi/datasets/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/data/concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/data/debug.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/data/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/data/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/data/forewards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/data/grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/data/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/data/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/data/masked.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/data/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/data/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/data/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/data/stores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/data/subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/data/unchecked.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.920238 anemoi_datasets-0.1.6/src/anemoi/datasets/dates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/dates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/dates/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/grids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.920238 anemoi_datasets-0.1.6/src/anemoi/datasets/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/src/anemoi/datasets/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.924238 anemoi_datasets-0.1.6/src/anemoi_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15615 2024-05-03 17:17:26.000000 anemoi_datasets-0.1.6/src/anemoi_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-05-03 17:17:26.000000 anemoi_datasets-0.1.6/src/anemoi_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:17:26.000000 anemoi_datasets-0.1.6/src/anemoi_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-03 17:17:26.000000 anemoi_datasets-0.1.6/src/anemoi_datasets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-03 17:17:26.000000 anemoi_datasets-0.1.6/src/anemoi_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 17:17:26.000000 anemoi_datasets-0.1.6/src/anemoi_datasets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.920238 anemoi_datasets-0.1.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.924238 anemoi_datasets-0.1.6/tests/create/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tests/create/concat.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tests/create/data_sources.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tests/create/join.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tests/create/missing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tests/create/nan.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tests/create/perturbations.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tests/create/pipe.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7619 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tests/create/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tests/create-perturbations-full.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tests/create-shift.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tests/test_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36578 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tests/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tests/test_indexing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.924238 anemoi_datasets-0.1.6/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tools/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.924238 anemoi_datasets-0.1.6/tools/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tools/examples/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tools/examples/an-oper-2023-2023-2p5-6h-v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:26.924238 anemoi_datasets-0.1.6/tools/grids/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tools/grids/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tools/grids/grids.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tools/grids/grids1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-03 17:17:16.000000 anemoi_datasets-0.1.6/tools/grids/grids2.yaml
```

### Comparing `anemoi-datasets-0.1.4/LICENSE` & `anemoi_datasets-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/README.md` & `anemoi_datasets-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/__init__.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # (C) Copyright 2023 European Centre for Medium-Range Weather Forecasts.
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 
+from ._version import __version__
 from .data import MissingDateError
 from .data import add_dataset_path
 from .data import add_named_dataset
 from .data import open_dataset
 
-__version__ = "0.1.4"
-
 __all__ = [
     "open_dataset",
     "MissingDateError",
     "add_dataset_path",
     "add_named_dataset",
 ]
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/__main__.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/commands/__init__.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/commands/compare.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/commands/compare.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/commands/copy.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/commands/copy.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/commands/create.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/commands/create.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/commands/inspect/__init__.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/commands/inspect/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 
 
 import os
 
 from .. import Command
+from .zarr import InspectZarr
 
 # from .checkpoint import InspectCheckpoint
-from .zarr import InspectZarr
 
 
 class Inspect(Command, InspectZarr):
     # class Inspect(Command, InspectCheckpoint, InspectZarr):
     """Inspect a checkpoint or zarr file."""
 
     def add_arguments(self, command_parser):
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/commands/inspect/zarr.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/commands/inspect/zarr.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/commands/scan.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/commands/scan.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/check.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/check.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,37 +4,22 @@
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
 import logging
-import os
 import re
 import warnings
 
 import numpy as np
-import tqdm
 
 LOG = logging.getLogger(__name__)
 
 
-def compute_directory_size(path):
-    if not os.path.isdir(path):
-        return None
-    size = 0
-    n = 0
-    for dirpath, _, filenames in tqdm.tqdm(os.walk(path), desc="Computing size", leave=False):
-        for filename in filenames:
-            file_path = os.path.join(dirpath, filename)
-            size += os.path.getsize(file_path)
-            n += 1
-    return size, n
-
-
 class DatasetName:
     def __init__(
         self,
         name,
         resolution=None,
         start_date=None,
         end_date=None,
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/config.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,15 @@
         self.setdefault("dataset_status", "experimental")
         self.setdefault("description", "No description provided.")
         self.setdefault("licence", "unknown")
         self.setdefault("attribution", "unknown")
 
         self.setdefault("build", Config())
         self.build.setdefault("group_by", "monthly")
+        self.build.setdefault("use_grib_paramid", False)
 
         self.setdefault("output", Config())
         self.output.setdefault("order_by", ["valid_datetime", "param_level", "number"])
         self.output.setdefault("remapping", Config(param_level="{param}_{levelist}"))
         self.output.setdefault("statistics", "param_level")
         self.output.setdefault("chunking", Config(dates=1, ensembles=1))
         self.output.setdefault("dtype", "float32")
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/__init__.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/accumulations.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/accumulations.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/constants.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/constants.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/forcings.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/forcings.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/grib.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/grib.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/mars.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/mars.py`

 * *Files 12% similar despite different names*

```diff
@@ -78,22 +78,40 @@
     for r in compressed.iterate():
         for k, v in r.items():
             if isinstance(v, (list, tuple)) and len(v) == 1:
                 r[k] = v[0]
         yield r
 
 
+def use_grib_paramid(r):
+    from anemoi.utils.grib import shortname_to_paramid
+
+    params = r["param"]
+    if isinstance(params, str):
+        params = params.split("/")
+    assert isinstance(params, (list, tuple)), params
+
+    params = [shortname_to_paramid(p) for p in params]
+    r["param"] = "/".join(str(p) for p in params)
+
+    return r
+
+
 def mars(context, dates, *requests, **kwargs):
     if not requests:
         requests = [kwargs]
 
     requests = factorise_requests(dates, *requests)
     ds = load_source("empty")
     for r in requests:
         r = {k: v for k, v in r.items() if v != ("-",)}
+
+        if context.use_grib_paramid and "param" in r:
+            r = use_grib_paramid(r)
+
         if DEBUG:
             context.trace("✅", f"load_source(mars, {r}")
 
         ds = ds + load_source("mars", **r)
     return ds
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/netcdf.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/netcdf.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/opendap.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/opendap.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/source.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/source.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/tendencies.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/sources/tendencies.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/empty.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/filters/empty.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/rename.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/filters/rename.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/rotate_winds.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/filters/rotate_winds.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 
 from collections import defaultdict
 
 from climetlab.indexing.fieldset import FieldArray
 
 
 def rotate_winds(lats, lons, x_wind, y_wind, source_projection, target_projection):
-    """
-    Code provided by MetNO
-    """
+    """Code provided by MetNO"""
     import numpy as np
     import pyproj
 
     if source_projection == target_projection:
         return x_wind, x_wind
 
     source_projection = pyproj.Proj(source_projection)
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/unrotate_winds.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/functions/filters/unrotate_winds.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,17 +74,15 @@
         return self.data
 
     def __getattr__(self, name):
         return getattr(self.field, name)
 
 
 def execute(context, input, u, v):
-    """
-    Unrotate the wind components of a GRIB file.
-    """
+    """Unrotate the wind components of a GRIB file."""
     result = FieldArray()
 
     wind_params = (u, v)
     wind_pairs = defaultdict(dict)
 
     for f in input:
         key = f.as_mars()
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/input.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -557,15 +557,15 @@
     @trace_select
     def select(self, dates):
         return FunctionResult(self.context, self.action_path, dates, action=self)
 
     @property
     def function(self):
         # name, delta = parse_function_name(self.name)
-        return import_function(self.name, "actions")
+        return import_function(self.name, "sources")
 
     def __repr__(self):
         content = ""
         content += ",".join([self._short_str(a) for a in self.args])
         content += " ".join([self._short_str(f"{k}={v}") for k, v in self.kwargs.items()])
         content = self._short_str(content)
         return super().__repr__(_inline_=content, _indent_=" ")
@@ -821,15 +821,15 @@
         "concat": ConcatAction,
         "join": JoinAction,
         "pipe": PipeAction,
         "function": FunctionAction,
     }.get(key)
 
     if cls is None:
-        if not is_function(key, "actions"):
+        if not is_function(key, "sources"):
             raise ValueError(f"Unknown action '{key}' in {config}")
         cls = FunctionAction
         args = [key] + args
 
     return cls(context, action_path + [key], *args, **kwargs)
 
 
@@ -865,29 +865,32 @@
         # print("========", args)
 
     return cls(context, action_path, previous_step, *args, **kwargs)
 
 
 class FunctionContext:
     """A FunctionContext is passed to all functions, it will be used to pass information
-    to the functions from the other actions and filters and results."""
+    to the functions from the other actions and filters and results.
+    """
 
     def __init__(self, owner):
         self.owner = owner
+        self.use_grib_paramid = owner.context.use_grib_paramid
 
     def trace(self, emoji, *args):
         trace(emoji, *args)
 
 
 class ActionContext(Context):
-    def __init__(self, /, order_by, flatten_grid, remapping):
+    def __init__(self, /, order_by, flatten_grid, remapping, use_grib_paramid):
         super().__init__()
         self.order_by = order_by
         self.flatten_grid = flatten_grid
         self.remapping = build_remapping(remapping)
+        self.use_grib_paramid = use_grib_paramid
 
 
 class InputBuilder:
     def __init__(self, config, data_sources, **kwargs):
         self.kwargs = kwargs
 
         config = deepcopy(config)
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/loaders.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/loaders.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,103 +5,61 @@
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 import datetime
 import logging
 import os
 import time
 import uuid
+import warnings
 from functools import cached_property
 
 import numpy as np
 import zarr
 
+from anemoi.datasets import MissingDateError
 from anemoi.datasets import open_dataset
+from anemoi.datasets.create.persistent import build_storage
 from anemoi.datasets.data.misc import as_first_date
 from anemoi.datasets.data.misc import as_last_date
 from anemoi.datasets.dates.groups import Groups
 
 from .check import DatasetName
 from .check import check_data_values
+from .chunks import ChunkFilter
 from .config import build_output
 from .config import loader_config
 from .input import build_input
-from .statistics import TempStatistics
+from .statistics import Summary
+from .statistics import TmpStatistics
+from .statistics import check_variance
 from .statistics import compute_statistics
-from .utils import bytes
-from .utils import compute_directory_sizes
+from .statistics import default_statistics_dates
 from .utils import normalize_and_check_dates
 from .utils import progress_bar
 from .utils import seconds
-from .writer import CubesFilter
 from .writer import ViewCacheArray
 from .zarr import ZarrBuiltRegistry
 from .zarr import add_zarr_dataset
 
 LOG = logging.getLogger(__name__)
 
 VERSION = "0.20"
 
 
-def default_statistics_dates(dates):
-    """
-    Calculate default statistics dates based on the given list of dates.
-
-    Args:
-        dates (list): List of datetime objects representing dates.
-
-    Returns:
-        tuple: A tuple containing the default start and end dates.
-    """
-
-    def to_datetime(d):
-        if isinstance(d, np.datetime64):
-            return d.tolist()
-        assert isinstance(d, datetime.datetime), d
-        return d
-
-    first = dates[0]
-    last = dates[-1]
-
-    first = to_datetime(first)
-    last = to_datetime(last)
-
-    n_years = round((last - first).total_seconds() / (365.25 * 24 * 60 * 60))
-
-    if n_years < 10:
-        # leave out 20% of the data
-        k = int(len(dates) * 0.8)
-        end = dates[k - 1]
-        LOG.info(f"Number of years {n_years} < 10, leaving out 20%. {end=}")
-        return dates[0], end
-
-    delta = 1
-    if n_years >= 20:
-        delta = 3
-    LOG.info(f"Number of years {n_years}, leaving out {delta} years.")
-    end_year = last.year - delta
-
-    end = max(d for d in dates if to_datetime(d).year == end_year)
-    return dates[0], end
-
-
-class Loader:
+class GenericDatasetHandler:
     def __init__(self, *, path, print=print, **kwargs):
         # Catch all floating point errors, including overflow, sqrt(<0), etc
         np.seterr(all="raise", under="warn")
 
         assert isinstance(path, str), path
 
         self.path = path
         self.kwargs = kwargs
         self.print = print
 
-        statistics_tmp = kwargs.get("statistics_tmp") or self.path + ".statistics"
-
-        self.statistics_registry = TempStatistics(statistics_tmp)
-
     @classmethod
     def from_config(cls, *, config, path, print=print, **kwargs):
         # config is the path to the config file or a dict with the config
         assert isinstance(config, dict) or isinstance(config, str), config
         return cls(config=config, path=path, print=print, **kwargs)
 
     @classmethod
@@ -113,67 +71,32 @@
         return cls.from_config(config=config, path=path, print=print, **kwargs)
 
     @classmethod
     def from_dataset(cls, *, path, **kwargs):
         assert os.path.exists(path), f"Path {path} does not exist."
         return cls(path=path, **kwargs)
 
-    def build_input(self):
-        from climetlab.core.order import build_remapping
-
-        builder = build_input(
-            self.main_config.input,
-            data_sources=self.main_config.get("data_sources", {}),
-            order_by=self.output.order_by,
-            flatten_grid=self.output.flatten_grid,
-            remapping=build_remapping(self.output.remapping),
-        )
-        LOG.info("✅ INPUT_BUILDER")
-        LOG.info(builder)
-        return builder
-
-    def build_statistics_dates(self, start, end):
-        ds = open_dataset(self.path)
-        dates = ds.dates
-
-        default_start, default_end = default_statistics_dates(dates)
-        if start is None:
-            start = default_start
-        if end is None:
-            end = default_end
-
-        start = as_first_date(start, dates)
-        end = as_last_date(end, dates)
-
-        start = start.astype(datetime.datetime)
-        end = end.astype(datetime.datetime)
-        return (start.isoformat(), end.isoformat())
-
     def read_dataset_metadata(self):
         ds = open_dataset(self.path)
         self.dataset_shape = ds.shape
         self.variables_names = ds.variables
         assert len(self.variables_names) == ds.shape[1], self.dataset_shape
         self.dates = ds.dates
 
-        z = zarr.open(self.path, "r")
-        self.missing_dates = z.attrs.get("missing_dates", [])
-        self.missing_dates = [np.datetime64(d) for d in self.missing_dates]
+        self.missing_dates = sorted(list([self.dates[i] for i in ds.missing]))
 
-    def allow_nan(self, name):
-        return name in self.main_config.statistics.get("allow_nans", [])
+        z = zarr.open(self.path, "r")
+        missing_dates = z.attrs.get("missing_dates", [])
+        missing_dates = sorted([np.datetime64(d) for d in missing_dates])
+        assert missing_dates == self.missing_dates, (missing_dates, self.missing_dates)
 
     @cached_property
     def registry(self):
         return ZarrBuiltRegistry(self.path)
 
-    def initialise_dataset_backend(self):
-        z = zarr.open(self.path, mode="w")
-        z.create_group("_build")
-
     def update_metadata(self, **kwargs):
         LOG.info(f"Updating metadata {kwargs}")
         z = zarr.open(self.path, mode="w+")
         for k, v in kwargs.items():
             if isinstance(v, np.datetime64):
                 v = v.astype(datetime.datetime)
             if isinstance(v, datetime.date):
@@ -192,20 +115,51 @@
         z = zarr.open(self.path, mode="r")
         try:
             LOG.info(z["data"].info)
         except Exception as e:
             LOG.info(e)
 
 
-class InitialiseLoader(Loader):
+class DatasetHandler(GenericDatasetHandler):
+    pass
+
+
+class DatasetHandlerWithStatistics(GenericDatasetHandler):
+    def __init__(self, statistics_tmp=None, **kwargs):
+        super().__init__(**kwargs)
+        statistics_tmp = kwargs.get("statistics_tmp") or os.path.join(self.path + ".tmp_data", "statistics")
+        self.tmp_statistics = TmpStatistics(statistics_tmp)
+
+
+class Loader(DatasetHandlerWithStatistics):
+    def build_input(self):
+        from climetlab.core.order import build_remapping
+
+        builder = build_input(
+            self.main_config.input,
+            data_sources=self.main_config.get("data_sources", {}),
+            order_by=self.output.order_by,
+            flatten_grid=self.output.flatten_grid,
+            remapping=build_remapping(self.output.remapping),
+            use_grib_paramid=self.main_config.build.use_grib_paramid,
+        )
+        LOG.info("✅ INPUT_BUILDER")
+        LOG.info(builder)
+        return builder
+
+    def allow_nan(self, name):
+        return name in self.main_config.statistics.get("allow_nans", [])
+
+
+class InitialiserLoader(Loader):
     def __init__(self, config, **kwargs):
         super().__init__(**kwargs)
         self.main_config = loader_config(config)
 
-        self.statistics_registry.delete()
+        self.tmp_statistics.delete()
 
         LOG.info(self.main_config.dates)
         self.groups = Groups(**self.main_config.dates)
 
         self.output = build_output(self.main_config.output, parent=self)
         self.input = self.build_input()
 
@@ -213,14 +167,35 @@
         all_dates = self.groups.dates
         self.minimal_input = self.input.select([all_dates[0]])
 
         LOG.info(self.groups)
         LOG.info("MINIMAL INPUT :")
         LOG.info(self.minimal_input)
 
+    def build_statistics_dates(self, start, end):
+        ds = open_dataset(self.path)
+        dates = ds.dates
+
+        default_start, default_end = default_statistics_dates(dates)
+        if start is None:
+            start = default_start
+        if end is None:
+            end = default_end
+
+        start = as_first_date(start, dates)
+        end = as_last_date(end, dates)
+
+        start = start.astype(datetime.datetime)
+        end = end.astype(datetime.datetime)
+        return (start.isoformat(), end.isoformat())
+
+    def initialise_dataset_backend(self):
+        z = zarr.open(self.path, mode="w")
+        z.create_group("_build")
+
     def initialise(self, check_name=True):
         """Create empty dataset."""
 
         self.print("Config loaded ok:")
         LOG.info(self.main_config)
 
         dates = self.groups.dates
@@ -326,16 +301,16 @@
 
         self._add_dataset(name="data", chunks=chunks, dtype=dtype, shape=total_shape)
         self._add_dataset(name="dates", array=dates)
         self._add_dataset(name="latitudes", array=grid_points[0])
         self._add_dataset(name="longitudes", array=grid_points[1])
 
         self.registry.create(lengths=lengths)
-        self.statistics_registry.create(exist_ok=False)
-        self.registry.add_to_history("statistics_registry_initialised", version=self.statistics_registry.version)
+        self.tmp_statistics.create(exist_ok=False)
+        self.registry.add_to_history("tmp_statistics_initialised", version=self.tmp_statistics.version)
 
         statistics_start, statistics_end = self.build_statistics_dates(
             self.main_config.statistics.get("start"),
             self.main_config.statistics.get("end"),
         )
         self.update_metadata(
             statistics_start_date=statistics_start,
@@ -356,29 +331,29 @@
         self.groups = Groups(**self.main_config.dates)
         self.output = build_output(self.main_config.output, parent=self)
         self.input = self.build_input()
         self.read_dataset_metadata()
 
         self.parts = parts
         total = len(self.registry.get_flags())
-        self.cube_filter = CubesFilter(parts=self.parts, total=total)
+        self.chunk_filter = ChunkFilter(parts=self.parts, total=total)
 
         self.data_array = zarr.open(self.path, mode="r+")["data"]
         self.n_groups = len(self.groups)
 
     def load(self):
         self.registry.add_to_history("loading_data_start", parts=self.parts)
 
         for igroup, group in enumerate(self.groups):
-            if not self.cube_filter(igroup):
+            if not self.chunk_filter(igroup):
                 continue
             if self.registry.get_flag(igroup):
                 LOG.info(f" -> Skipping {igroup} total={len(self.groups)} (already done)")
                 continue
-            self.print(f" -> Processing {igroup} total={len(self.groups)}")
+            # self.print(f" -> Processing {igroup} total={len(self.groups)}")
             # print("========", group)
             assert isinstance(group[0], datetime.datetime), group
 
             result = self.input.select(dates=group)
             assert result.dates == group, (len(result.dates), len(group))
 
             msg = f"Building data for group {igroup}/{self.n_groups}"
@@ -388,15 +363,15 @@
             # There are several groups.
             # There is one result to load for each group.
             self.load_result(result)
             self.registry.set_flag(igroup)
 
         self.registry.add_to_history("loading_data_end", parts=self.parts)
         self.registry.add_provenance(name="provenance_load")
-        self.statistics_registry.add_provenance(name="provenance_load", config=self.main_config)
+        self.tmp_statistics.add_provenance(name="provenance_load", config=self.main_config)
 
         self.print_info()
 
     def load_result(self, result):
         # There is one cube to load for each result.
         dates = result.dates
 
@@ -426,15 +401,15 @@
 
         indexes = dates_to_indexes(self.dates, dates_in_data)
 
         array = ViewCacheArray(self.data_array, shape=shape, indexes=indexes)
         self.load_cube(cube, array)
 
         stats = compute_statistics(array.cache, self.variables_names, allow_nan=self.allow_nan)
-        self.statistics_registry.write(indexes, stats, dates=dates_in_data)
+        self.tmp_statistics.write(indexes, stats, dates=dates_in_data)
 
         array.flush()
 
     def load_cube(self, cube, array):
         # There are several cubelets for each cube
         start = time.time()
         load = 0
@@ -472,55 +447,53 @@
         save += time.time() - now
         LOG.info("Written.")
         msg = f"Elapsed: {seconds(time.time() - start)}, load time: {seconds(load)}, write time: {seconds(save)}."
         self.print(msg)
         LOG.info(msg)
 
 
-class StatisticsLoader(Loader):
-    main_config = {}
-
+class StatisticsAdder(DatasetHandlerWithStatistics):
     def __init__(
         self,
-        config=None,
         statistics_output=None,
         statistics_start=None,
         statistics_end=None,
-        force=False,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.user_statistics_start = statistics_start
         self.user_statistics_end = statistics_end
 
         self.statistics_output = statistics_output
 
         self.output_writer = {
             None: self.write_stats_to_dataset,
             "-": self.write_stats_to_stdout,
         }.get(self.statistics_output, self.write_stats_to_file)
 
-        if config:
-            self.main_config = loader_config(config)
-
         self.read_dataset_metadata()
 
+    def allow_nan(self, name):
+        z = zarr.open(self.path, mode="r")
+        if "variables_with_nans" in z.attrs:
+            return name in z.attrs["variables_with_nans"]
+
+        warnings.warn(f"Cannot find 'variables_with_nans' in {self.path}. Assuming nans allowed for {name}.")
+        return True
+
     def _get_statistics_dates(self):
         dates = self.dates
         dtype = type(dates[0])
 
         def assert_dtype(d):
             assert type(d) is dtype, (type(d), dtype)
 
         # remove missing dates
         if self.missing_dates:
-            assert type(self.missing_dates[0]) is dtype, (
-                type(self.missing_dates[0]),
-                dtype,
-            )
+            assert_dtype(self.missing_dates[0])
         dates = [d for d in dates if d not in self.missing_dates]
 
         # filter dates according the the start and end dates in the metadata
         z = zarr.open(self.path, mode="r")
         start, end = z.attrs.get("statistics_start_date"), z.attrs.get("statistics_end_date")
         start, end = np.datetime64(start), np.datetime64(end)
         assert_dtype(start)
@@ -539,19 +512,19 @@
             assert_dtype(limit)
             dates = [d for d in dates if d <= limit]
 
         return dates
 
     def run(self):
         dates = self._get_statistics_dates()
-        stats = self.statistics_registry.get_aggregated(dates, self.variables_names, self.allow_nan)
+        stats = self.tmp_statistics.get_aggregated(dates, self.variables_names, self.allow_nan)
         self.output_writer(stats)
 
     def write_stats_to_file(self, stats):
-        stats.save(self.statistics_output, provenance=dict(config=self.main_config))
+        stats.save(self.statistics_output)
         LOG.info(f"✅ Statistics written in {self.statistics_output}")
 
     def write_stats_to_dataset(self, stats):
         if self.user_statistics_start or self.user_statistics_end:
             raise ValueError(
                 (
                     "Cannot write statistics in dataset with user specified dates. "
@@ -568,28 +541,236 @@
         self.registry.add_to_history("compute_statistics_end")
         LOG.info(f"Wrote statistics in {self.path}")
 
     def write_stats_to_stdout(self, stats):
         LOG.info(stats)
 
 
-class SizeLoader(Loader):
-    def __init__(self, path, print):
-        self.path = path
-        self.print = print
+class GenericAdditions(GenericDatasetHandler):
+    def __init__(self, name="", **kwargs):
+        super().__init__(**kwargs)
+        self.name = name
 
-    def add_total_size(self):
-        dic = compute_directory_sizes(self.path)
+        storage_path = f"{self.path}.tmp_storage_{name}"
+        self.tmp_storage = build_storage(directory=storage_path, create=True)
 
-        size = dic["total_size"]
-        n = dic["total_number_of_files"]
+    def initialise(self):
+        self.tmp_storage.delete()
+        self.tmp_storage.create()
+        LOG.info(f"Dataset {self.path} additions initialized.")
 
-        LOG.info(f"Total size: {bytes(size)}")
-        LOG.info(f"Total number of files: {n}")
+    @cached_property
+    def _variables_with_nans(self):
+        z = zarr.open(self.path, mode="r")
+        if "variables_with_nans" in z.attrs:
+            return z.attrs["variables_with_nans"]
+        return None
 
-        self.update_metadata(total_size=size, total_number_of_files=n)
+    def allow_nan(self, name):
+        if self._variables_with_nans is not None:
+            return name in self._variables_with_nans
+        warnings.warn(f"❗Cannot find 'variables_with_nans' in {self.path}, Assuming nans allowed for {name}.")
+        return True
 
+    @classmethod
+    def _check_type_equal(cls, a, b):
+        a = list(a)
+        b = list(b)
+        a = a[0] if a else None
+        b = b[0] if b else None
+        assert type(a) is type(b), (type(a), type(b))
+
+    def finalise(self):
+        shape = (len(self.dates), len(self.variables))
+        agg = dict(
+            minimum=np.full(shape, np.nan, dtype=np.float64),
+            maximum=np.full(shape, np.nan, dtype=np.float64),
+            sums=np.full(shape, np.nan, dtype=np.float64),
+            squares=np.full(shape, np.nan, dtype=np.float64),
+            count=np.full(shape, -1, dtype=np.int64),
+            has_nans=np.full(shape, False, dtype=np.bool_),
+        )
+        LOG.info(f"Aggregating {self.name} statistics on shape={shape}. Variables : {self.variables}")
 
-class CleanupLoader(Loader):
-    def run(self):
-        self.statistics_registry.delete()
-        self.registry.clean()
+        found = set()
+        ifound = set()
+        missing = set()
+        for _date, (date, i, stats) in self.tmp_storage.items():
+            assert _date == date
+            if stats == "missing":
+                missing.add(date)
+                continue
+
+            assert date not in found, f"Duplicates found {date}"
+            found.add(date)
+            ifound.add(i)
+
+            for k in ["minimum", "maximum", "sums", "squares", "count", "has_nans"]:
+                agg[k][i, ...] = stats[k]
+
+        assert len(found) + len(missing) == len(self.dates), (len(found), len(missing), len(self.dates))
+        assert found.union(missing) == set(self.dates), (found, missing, set(self.dates))
+
+        mask = sorted(list(ifound))
+        for k in ["minimum", "maximum", "sums", "squares", "count", "has_nans"]:
+            agg[k] = agg[k][mask, ...]
+
+        for k in ["minimum", "maximum", "sums", "squares", "count", "has_nans"]:
+            assert agg[k].shape == agg["count"].shape, (agg[k].shape, agg["count"].shape)
+
+        minimum = np.nanmin(agg["minimum"], axis=0)
+        maximum = np.nanmax(agg["maximum"], axis=0)
+        sums = np.nansum(agg["sums"], axis=0)
+        squares = np.nansum(agg["squares"], axis=0)
+        count = np.nansum(agg["count"], axis=0)
+        has_nans = np.any(agg["has_nans"], axis=0)
+
+        assert sums.shape == count.shape
+        assert sums.shape == squares.shape
+        assert sums.shape == minimum.shape
+        assert sums.shape == maximum.shape
+        assert sums.shape == has_nans.shape
+
+        mean = sums / count
+        assert sums.shape == mean.shape
+
+        x = squares / count - mean * mean
+        # remove negative variance due to numerical errors
+        # x[- 1e-15 < (x / (np.sqrt(squares / count) + np.abs(mean))) < 0] = 0
+        check_variance(x, self.variables, minimum, maximum, mean, count, sums, squares)
+
+        stdev = np.sqrt(x)
+        assert sums.shape == stdev.shape
+
+        self.summary = Summary(
+            minimum=minimum,
+            maximum=maximum,
+            mean=mean,
+            count=count,
+            sums=sums,
+            squares=squares,
+            stdev=stdev,
+            variables_names=self.variables,
+            has_nans=has_nans,
+        )
+        LOG.info(f"Dataset {self.path} additions finalized.")
+        self.check_statistics()
+        self._write(self.summary)
+        self.tmp_storage.delete()
+
+    def _write(self, summary):
+        for k in ["mean", "stdev", "minimum", "maximum", "sums", "squares", "count", "has_nans"]:
+            self._add_dataset(name=k, array=summary[k])
+        self.registry.add_to_history("compute_statistics_end")
+        LOG.info(f"Wrote {self.name} additions in {self.path}")
+
+    def check_statistics(self):
+        pass
+
+
+class StatisticsAddition(GenericAdditions):
+    def __init__(self, **kwargs):
+        super().__init__("statistics_", **kwargs)
+
+        z = zarr.open(self.path, mode="r")
+        start = z.attrs["statistics_start_date"]
+        end = z.attrs["statistics_end_date"]
+        self.ds = open_dataset(self.path, start=start, end=end)
+
+        self.variables = self.ds.variables
+        self.dates = self.ds.dates
+
+        assert len(self.variables) == self.ds.shape[1], self.ds.shape
+        self.total = len(self.dates)
+
+    def run(self, parts):
+        chunk_filter = ChunkFilter(parts=parts, total=self.total)
+        for i in range(0, self.total):
+            if not chunk_filter(i):
+                continue
+            date = self.dates[i]
+            try:
+                arr = self.ds[i : i + 1, ...]
+                stats = compute_statistics(arr, self.variables, allow_nan=self.allow_nan)
+                self.tmp_storage.add([date, i, stats], key=date)
+            except MissingDateError:
+                self.tmp_storage.add([date, i, "missing"], key=date)
+        self.tmp_storage.flush()
+        LOG.info(f"Dataset {self.path} additions run.")
+
+    def check_statistics(self):
+        ds = open_dataset(self.path)
+        ref = ds.statistics
+        for k in ds.statistics:
+            assert np.all(np.isclose(ref[k], self.summary[k], rtol=1e-4, atol=1e-4)), (
+                k,
+                ref[k],
+                self.summary[k],
+            )
+
+
+class DeltaDataset:
+    def __init__(self, ds, idelta):
+        self.ds = ds
+        self.idelta = idelta
+
+    def __getitem__(self, i):
+        j = i - self.idelta
+        if j < 0:
+            raise MissingDateError(f"Missing date {j}")
+        return self.ds[i : i + 1, ...] - self.ds[j : j + 1, ...]
+
+
+class TendenciesStatisticsDeltaNotMultipleOfFrequency(ValueError):
+    pass
+
+
+class TendenciesStatisticsAddition(GenericAdditions):
+    DATASET_NAME_PATTERN = "statistics_tendencies_{delta}"
+
+    def __init__(self, path, delta=None, **kwargs):
+        full_ds = open_dataset(path)
+        self.variables = full_ds.variables
+
+        frequency = full_ds.frequency
+        if delta is None:
+            delta = frequency
+        assert isinstance(delta, int), delta
+        if not delta % frequency == 0:
+            raise TendenciesStatisticsDeltaNotMultipleOfFrequency(
+                f"Delta {delta} is not a multiple of frequency {frequency}"
+            )
+        idelta = delta // frequency
+
+        super().__init__(path=path, name=self.DATASET_NAME_PATTERN.format(delta=f"{delta}h"), **kwargs)
+
+        z = zarr.open(self.path, mode="r")
+        start = z.attrs["statistics_start_date"]
+        end = z.attrs["statistics_end_date"]
+        start = datetime.datetime.fromisoformat(start)
+        ds = open_dataset(self.path, start=start + datetime.timedelta(hours=delta), end=end)
+        self.dates = ds.dates
+        self.total = len(self.dates)
+
+        ds = open_dataset(self.path, start=start, end=end)
+        self.ds = DeltaDataset(ds, idelta)
+
+    def run(self, parts):
+        chunk_filter = ChunkFilter(parts=parts, total=self.total)
+        for i in range(0, self.total):
+            if not chunk_filter(i):
+                continue
+            date = self.dates[i]
+            try:
+                arr = self.ds[i]
+                stats = compute_statistics(arr, self.variables, allow_nan=self.allow_nan)
+                self.tmp_storage.add([date, i, stats], key=date)
+            except MissingDateError:
+                self.tmp_storage.add([date, i, "missing"], key=date)
+        self.tmp_storage.flush()
+        LOG.info(f"Dataset {self.path} additions run.")
+
+    def _write(self, summary):
+        for k in ["mean", "stdev", "minimum", "maximum", "sums", "squares", "count", "has_nans"]:
+            self._add_dataset(name=f"{self.name}_{k}", array=summary[k])
+        self.registry.add_to_history(f"compute_{self.name}_end")
+        LOG.info(f"Wrote {self.name} additions in {self.path}")
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/patch.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/patch.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/statistics.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/statistics/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,26 +11,66 @@
 import hashlib
 import json
 import logging
 import os
 import pickle
 import shutil
 import socket
-from collections import defaultdict
 
 import numpy as np
 from anemoi.utils.provenance import gather_provenance_info
 
-from .check import StatisticsValueError
-from .check import check_data_values
-from .check import check_stats
+from ..check import check_data_values
+from .summary import Summary
 
 LOG = logging.getLogger(__name__)
 
 
+def default_statistics_dates(dates):
+    """
+    Calculate default statistics dates based on the given list of dates.
+
+    Args:
+        dates (list): List of datetime objects representing dates.
+
+    Returns:
+        tuple: A tuple containing the default start and end dates.
+    """
+
+    def to_datetime(d):
+        if isinstance(d, np.datetime64):
+            return d.tolist()
+        assert isinstance(d, datetime.datetime), d
+        return d
+
+    first = dates[0]
+    last = dates[-1]
+
+    first = to_datetime(first)
+    last = to_datetime(last)
+
+    n_years = round((last - first).total_seconds() / (365.25 * 24 * 60 * 60))
+
+    if n_years < 10:
+        # leave out 20% of the data
+        k = int(len(dates) * 0.8)
+        end = dates[k - 1]
+        LOG.info(f"Number of years {n_years} < 10, leaving out 20%. {end=}")
+        return dates[0], end
+
+    delta = 1
+    if n_years >= 20:
+        delta = 3
+    LOG.info(f"Number of years {n_years}, leaving out {delta} years.")
+    end_year = last.year - delta
+
+    end = max(d for d in dates if to_datetime(d).year == end_year)
+    return dates[0], end
+
+
 def to_datetime(date):
     if isinstance(date, str):
         return np.datetime64(date)
     if isinstance(date, datetime.datetime):
         return np.datetime64(date)
     return date
 
@@ -41,39 +81,40 @@
 
 def check_variance(x, variables_names, minimum, maximum, mean, count, sums, squares):
     if (x >= 0).all():
         return
     print(x)
     print(variables_names)
     print(count)
-    for i, (var, y) in enumerate(zip(variables_names, x)):
+    for i, (name, y) in enumerate(zip(variables_names, x)):
         if y >= 0:
             continue
+        print("---")
         print(
-            var,
+            name,
             y,
             maximum[i],
             minimum[i],
             mean[i],
             count[i],
             sums[i],
             squares[i],
         )
 
-        print(var, np.min(sums[i]), np.max(sums[i]), np.argmin(sums[i]))
-        print(var, np.min(squares[i]), np.max(squares[i]), np.argmin(squares[i]))
-        print(var, np.min(count[i]), np.max(count[i]), np.argmin(count[i]))
+        print(name, np.min(sums[i]), np.max(sums[i]), np.argmin(sums[i]))
+        print(name, np.min(squares[i]), np.max(squares[i]), np.argmin(squares[i]))
+        print(name, np.min(count[i]), np.max(count[i]), np.argmin(count[i]))
 
     raise ValueError("Negative variance")
 
 
 def compute_statistics(array, check_variables_names=None, allow_nan=False):
     nvars = array.shape[1]
 
-    LOG.info("Stats %s", (nvars, array.shape, check_variables_names))
+    LOG.info(f"Stats {nvars}, {array.shape}, {check_variables_names}")
     if check_variables_names:
         assert nvars == len(check_variables_names), (nvars, check_variables_names)
     stats_shape = (array.shape[0], nvars)
 
     count = np.zeros(stats_shape, dtype=np.int64)
     sums = np.zeros(stats_shape, dtype=np.float64)
     squares = np.zeros(stats_shape, dtype=np.float64)
@@ -104,15 +145,15 @@
         "sums": sums,
         "squares": squares,
         "count": count,
         "has_nans": has_nans,
     }
 
 
-class TempStatistics:
+class TmpStatistics:
     version = 3
     # Used in parrallel, during data loading,
     # to write statistics in pickled npz files.
     # can provide statistics for a subset of dates.
 
     def __init__(self, dirname, overwrite=False):
         self.dirname = dirname
@@ -158,15 +199,15 @@
                 yield pickle.load(f)
 
     def get_aggregated(self, *args, **kwargs):
         aggregator = StatAggregator(self, *args, **kwargs)
         return aggregator.aggregate()
 
     def __str__(self):
-        return f"TempStatistics({self.dirname})"
+        return f"TmpStatistics({self.dirname})"
 
 
 def normalise_date(d):
     if isinstance(d, str):
         d = np.datetime64(d)
     return d
 
@@ -285,99 +326,136 @@
                         mean[j],
                     ]
                 ),
                 name=name,
                 allow_nan=False,
             )
 
-        return Statistics(
+        return Summary(
             minimum=minimum,
             maximum=maximum,
             mean=mean,
             count=count,
             sums=sums,
             squares=squares,
             stdev=stdev,
             variables_names=self.variables_names,
             has_nans=has_nans,
         )
 
 
-class Statistics(dict):
-    STATS_NAMES = ["minimum", "maximum", "mean", "stdev", "has_nans"]  # order matter for __str__.
+class SummaryAggregator:
+    NAMES = ["minimum", "maximum", "sums", "squares", "count", "has_nans"]
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.check()
-
-    @property
-    def size(self):
-        return len(self["variables_names"])
-
-    def check(self):
-        for k, v in self.items():
-            if k == "variables_names":
-                assert len(v) == self.size
-                continue
-            assert v.shape == (self.size,)
-            if k == "count":
-                assert (v >= 0).all(), (k, v)
-                assert v.dtype == np.int64, (k, v)
-                continue
-            if k == "has_nans":
-                assert v.dtype == np.bool_, (k, v)
-                continue
-            if k == "stdev":
-                assert (v >= 0).all(), (k, v)
-            assert v.dtype == np.float64, (k, v)
-
-        for i, name in enumerate(self["variables_names"]):
-            try:
-                check_stats(**{k: v[i] for k, v in self.items()}, msg=f"{i} {name}")
-                check_data_values(self["minimum"][i], name=name)
-                check_data_values(self["maximum"][i], name=name)
-                check_data_values(self["mean"][i], name=name)
-            except StatisticsValueError as e:
-                e.args += (i, name)
-                raise
+    def __init__(self, owner, dates, variables_names, allow_nan):
+        dates = sorted(dates)
+        dates = to_datetimes(dates)
+        assert dates, "No dates selected"
+        self.owner = owner
+        self.dates = dates
+        self.variables_names = variables_names
+        self.allow_nan = allow_nan
 
-    def __str__(self):
-        header = ["Variables"] + self.STATS_NAMES
-        out = [" ".join(header)]
+        self.shape = (len(self.dates), len(self.variables_names))
+        LOG.info(f"Aggregating statistics on shape={self.shape}. Variables : {self.variables_names}")
 
-        out += [
-            " ".join([v] + [f"{self[n][i]:.2f}" for n in self.STATS_NAMES])
-            for i, v in enumerate(self["variables_names"])
-        ]
-        return "\n".join(out)
-
-    def save(self, filename, provenance=None):
-        assert filename.endswith(".json"), filename
-        dic = {}
-        for k in self.STATS_NAMES:
-            dic[k] = list(self[k])
-
-        out = dict(data=defaultdict(dict))
-        for i, name in enumerate(self["variables_names"]):
-            for k in self.STATS_NAMES:
-                out["data"][name][k] = dic[k][i]
-
-        out["provenance"] = provenance
-
-        with open(filename, "w") as f:
-            json.dump(out, f, indent=2)
-
-    def load(self, filename):
-        assert filename.endswith(".json"), filename
-        with open(filename) as f:
-            dic = json.load(f)
-
-        dic_ = {}
-        for k, v in dic.items():
-            if k == "count":
-                dic_[k] = np.array(v, dtype=np.int64)
-                continue
-            if k == "variables":
-                dic_[k] = v
+        self.minimum = np.full(self.shape, np.nan, dtype=np.float64)
+        self.maximum = np.full(self.shape, np.nan, dtype=np.float64)
+        self.sums = np.full(self.shape, np.nan, dtype=np.float64)
+        self.squares = np.full(self.shape, np.nan, dtype=np.float64)
+        self.count = np.full(self.shape, -1, dtype=np.int64)
+        self.has_nans = np.full(self.shape, False, dtype=np.bool_)
+
+        self._read()
+
+    def _read(self):
+        def check_type(a, b):
+            a = list(a)
+            b = list(b)
+            a = a[0] if a else None
+            b = b[0] if b else None
+            assert type(a) is type(b), (type(a), type(b))
+
+        found = set()
+        offset = 0
+        for _, _dates, stats in self.owner._gather_data():
+            for n in self.NAMES:
+                assert n in stats, (n, list(stats.keys()))
+            _dates = to_datetimes(_dates)
+            check_type(_dates, self.dates)
+            if found:
+                check_type(found, self.dates)
+                assert found.isdisjoint(_dates), "Duplicate dates found in precomputed statistics"
+
+            # filter dates
+            dates = set(_dates) & set(self.dates)
+
+            if not dates:
+                # dates have been completely filtered for this chunk
                 continue
-            dic_[k] = np.array(v, dtype=np.float64)
-        return Statistics(dic_)
+
+            # filter data
+            bitmap = np.isin(_dates, self.dates)
+            for k in self.NAMES:
+                stats[k] = stats[k][bitmap]
+
+            assert stats["minimum"].shape[0] == len(dates), (
+                stats["minimum"].shape,
+                len(dates),
+            )
+
+            # store data in self
+            found |= set(dates)
+            for name in self.NAMES:
+                array = getattr(self, name)
+                assert stats[name].shape[0] == len(dates), (
+                    stats[name].shape,
+                    len(dates),
+                )
+                array[offset : offset + len(dates)] = stats[name]
+            offset += len(dates)
+
+        for d in self.dates:
+            assert d in found, f"Statistics for date {d} not precomputed."
+        assert len(self.dates) == len(found), "Not all dates found in precomputed statistics"
+        assert len(self.dates) == offset, "Not all dates found in precomputed statistics."
+        LOG.info(f"Statistics for {len(found)} dates found.")
+
+    def aggregate(self):
+        minimum = np.nanmin(self.minimum, axis=0)
+        maximum = np.nanmax(self.maximum, axis=0)
+        sums = np.nansum(self.sums, axis=0)
+        squares = np.nansum(self.squares, axis=0)
+        count = np.nansum(self.count, axis=0)
+        has_nans = np.any(self.has_nans, axis=0)
+        mean = sums / count
+
+        assert sums.shape == count.shape == squares.shape == mean.shape == minimum.shape == maximum.shape
+
+        x = squares / count - mean * mean
+        # remove negative variance due to numerical errors
+        # x[- 1e-15 < (x / (np.sqrt(squares / count) + np.abs(mean))) < 0] = 0
+        check_variance(x, self.variables_names, minimum, maximum, mean, count, sums, squares)
+        stdev = np.sqrt(x)
+
+        for j, name in enumerate(self.variables_names):
+            check_data_values(
+                np.array(
+                    [
+                        mean[j],
+                    ]
+                ),
+                name=name,
+                allow_nan=False,
+            )
+
+        return Summary(
+            minimum=minimum,
+            maximum=maximum,
+            mean=mean,
+            count=count,
+            sums=sums,
+            squares=squares,
+            stdev=stdev,
+            variables_names=self.variables_names,
+            has_nans=has_nans,
+        )
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/template.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/template.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/utils.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,16 +27,15 @@
         return no_cache_context()
 
     os.makedirs(dirname, exist_ok=True)
     return settings.temporary("cache-directory", dirname)
 
 
 def bytes(n):
-    """
-    >>> bytes(4096)
+    """>>> bytes(4096)
     '4 KiB'
     >>> bytes(4000)
     '3.9 KiB'
     """
     if n < 0:
         sign = "-"
         n -= 0
@@ -68,29 +67,14 @@
         if path.endswith(".json"):
             return json.load(f)
         if path.endswith(".yaml") or path.endswith(".yml"):
             return yaml.safe_load(f)
         raise ValueError(f"Cannot read file {path}. Need json or yaml with appropriate extension.")
 
 
-def compute_directory_sizes(path):
-    if not os.path.isdir(path):
-        return None
-
-    size, n = 0, 0
-    bar = progress_bar(iterable=os.walk(path), desc=f"Computing size of {path}")
-    for dirpath, _, filenames in bar:
-        for filename in filenames:
-            file_path = os.path.join(dirpath, filename)
-            size += os.path.getsize(file_path)
-            n += 1
-
-    return dict(total_size=size, total_number_of_files=n)
-
-
 def make_list_int(value):
     if isinstance(value, str):
         if "/" not in value:
             return [value]
         bits = value.split("/")
         if len(bits) == 3 and bits[1].lower() == "to":
             value = list(range(int(bits[0]), int(bits[2]) + 1, 1))
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/create/zarr.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/create/zarr.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/data/__init__.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/data/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/data/concat.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/data/concat.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/data/dataset.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/data/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -218,7 +218,11 @@
 
         # for n in ('metadata_specific', 'tree', 'source'):
         #     if n not in overriden:
         #         warnings.warn(f"Method {n} is not overriden in {ds.__class__.__name__}")
 
     def _repr_html_(self):
         return self.tree().html()
+
+    @property
+    def label(self):
+        return self.__class__.__name__.lower()
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/data/debug.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/data/debug.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 
 DEPTH = 0
 
 # TODO: make numpy arrays read-only
 # a.flags.writeable = False
 
 
+def css(name):
+    path = os.path.join(os.path.dirname(__file__), f"{name}.css")
+    with open(path) as f:
+        return f"<style>{f.read()}</style>"
+
+
 class Node:
     def __init__(self, dataset, kids, **kwargs):
         self.dataset = dataset
         self.kids = kids
         self.kwargs = kwargs
 
     def _put(self, indent, result):
@@ -42,15 +48,15 @@
 
     def __repr__(self):
         result = []
         self._put(0, result)
         return "\n".join(result)
 
     def graph(self, digraph, nodes):
-        label = self.dataset.__class__.__name__.lower()
+        label = self.dataset.label  # dataset.__class__.__name__.lower()
         if self.kwargs:
             param = []
             for k, v in self.kwargs.items():
                 if k == "path" and isinstance(v, str):
                     v = os.path.basename(v)
                 if isinstance(v, (list, tuple)):
                     v = ", ".join(str(i) for i in v)
@@ -103,54 +109,63 @@
                 v = ", ".join(str(i) for i in v)
             else:
                 v = str(v)
             v = textwrap.shorten(v, width=80, placeholder="...")
             if k == "path":
                 v = v[::-1]
             kwargs[k] = v
-        label = self.dataset.__class__.__name__.lower()
+        label = self.dataset.label
         label = f'<span class="dataset">{label}</span>'
         if len(kwargs) == 1:
             k, v = list(kwargs.items())[0]
             rows.append([indent] + [label, v])
         else:
             rows.append([indent] + [label])
 
             for k, v in kwargs.items():
-                rows.append([indent] + [k, v])
+                rows.append([indent] + [f"<span class='param'>{k}</span>", f"<span class='param'>{v}</span>"])
 
         for kid in self.kids:
             kid._html(indent + "&nbsp;&nbsp;&nbsp;", rows)
 
     def html(self):
-        result = [
-            """
-<style>
-table.dataset td {
-    vertical-align: top;
-    text-align: left !important;
-}
-span.dataset {
-    font-weight: bold !important;
-}
-</style>
-                  """
-        ]
+        result = [css("debug")]
+
         result.append('<table class="dataset">')
         rows = []
 
         self._html("", rows)
 
         for r in rows:
             s = " ".join(str(x) for x in r)
             result.append(f"<tr><td>{s}</td></tr>")
 
         result.append("</table>")
         return "\n".join(result)
 
+    def _as_tree(self, tree):
+
+        for kid in self.kids:
+            n = tree.node(kid)
+            kid._as_tree(n)
+
+    def as_tree(self):
+        from anemoi.utils.text import Tree
+
+        tree = Tree(self)
+        self._as_tree(tree)
+        return tree
+
+    @property
+    def summary(self):
+        return self.dataset.label
+
+    def as_dict(self):
+        return {}
+
 
 class Source:
     """Class used to follow the provenance of a data point."""
 
     def __init__(self, dataset, index, source=None, info=None):
         self.dataset = dataset
         self.index = index
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/data/ensemble.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/data/ensemble.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/data/forewards.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/data/forewards.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,19 @@
     def variables(self):
         return self.forward.variables
 
     @property
     def statistics(self):
         return self.forward.statistics
 
+    def statistics_tendencies(self, delta=None):
+        if delta is None:
+            delta = self.frequency
+        return self.forward.statistics_tendencies(delta)
+
     @property
     def shape(self):
         return self.forward.shape
 
     @property
     def dtype(self):
         return self.forward.dtype
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/data/grids.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/data/grids.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
             result.extend(d.grids)
         return tuple(result)
 
     def tree(self):
         return Node(self, [d.tree() for d in self.datasets], mode="concat")
 
 
-class CutoutGrids(Grids):
+class Cutout(Grids):
     def __init__(self, datasets, axis):
         from anemoi.datasets.grids import cutout_mask
 
         super().__init__(datasets, axis)
         assert len(datasets) == 2, "CutoutGrids requires two datasets"
         assert axis == 3, "CutoutGrids requires axis=3"
 
@@ -232,8 +232,8 @@
 
     assert len(args) == 0
     assert isinstance(cutout, (list, tuple))
 
     datasets = [_open(e) for e in cutout]
     datasets, kwargs = _auto_adjust(datasets, kwargs)
 
-    return CutoutGrids(datasets, axis=axis)._subset(**kwargs)
+    return Cutout(datasets, axis=axis)._subset(**kwargs)
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/data/indexing.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/data/indexing.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 
 from functools import wraps
 
 import numpy as np
 
 
 def _tuple_with_slices(t, shape):
-    """
-    Replace all integers in a tuple with slices, so we preserve the dimensionality.
-    """
+    """Replace all integers in a tuple with slices, so we preserve the dimensionality."""
 
     result = tuple(slice(i, i + 1) if isinstance(i, int) else i for i in t)
     changes = tuple(j for (j, i) in enumerate(t) if isinstance(i, int))
     result = tuple(slice(*s.indices(shape[i])) for (i, s) in enumerate(result))
 
     return result, changes
 
@@ -48,43 +46,37 @@
         return _extend_shape(index, shape)
     if index is Ellipsis:
         return _extend_shape((Ellipsis,), shape)
     raise ValueError(f"Invalid index: {index}")
 
 
 def index_to_slices(index, shape):
-    """
-    Convert an index to a tuple of slices, with the same dimensionality as the shape.
-    """
+    """Convert an index to a tuple of slices, with the same dimensionality as the shape."""
     return _tuple_with_slices(_index_to_tuple(index, shape), shape)
 
 
 def apply_index_to_slices_changes(result, changes):
     if changes:
         shape = result.shape
         for i in changes:
             assert shape[i] == 1, (i, changes, shape)
         result = np.squeeze(result, axis=changes)
     return result
 
 
 def update_tuple(t, index, value):
-    """
-    Replace the elements of a tuple at the given index with a new value.
-    """
+    """Replace the elements of a tuple at the given index with a new value."""
     t = list(t)
     prev = t[index]
     t[index] = value
     return tuple(t), prev
 
 
 def length_to_slices(index, lengths):
-    """
-    Convert an index to a list of slices, given the lengths of the dimensions.
-    """
+    """Convert an index to a list of slices, given the lengths of the dimensions."""
     total = sum(lengths)
     start, stop, step = index.indices(total)
 
     result = []
 
     pos = 0
     for length in lengths:
@@ -123,16 +115,15 @@
 
         return i
 
     return tuple(_(i) for i in index)
 
 
 def expand_list_indexing(method):
-    """
-    Allows to use slices, lists, and tuples to select data from the dataset.
+    """Allows to use slices, lists, and tuples to select data from the dataset.
     Zarr does not support indexing with lists/arrays directly, so we need to implement it ourselves.
     """
 
     @wraps(method)
     def wrapper(self, index):
         if not isinstance(index, tuple):
             return method(self, index)
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/data/join.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/data/join.py`

 * *Files 18% similar despite different names*

```diff
@@ -117,14 +117,22 @@
 
     @property
     def statistics(self):
         return {
             k: np.concatenate([d.statistics[k] for d in self.datasets], axis=0) for k in self.datasets[0].statistics
         }
 
+    def statistics_tendencies(self, delta=None):
+        if delta is None:
+            delta = self.frequency
+        return {
+            k: np.concatenate([d.statistics_tendencies(delta)[k] for d in self.datasets], axis=0)
+            for k in self.datasets[0].statistics_tendencies(delta)
+        }
+
     def source(self, index):
         i = index
         for dataset in self.datasets:
             if i < dataset.shape[1]:
                 return Source(self, index, dataset.source(i))
             i -= dataset.shape[1]
         assert False
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/data/masked.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/data/masked.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/data/misc.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/data/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,15 +233,15 @@
 
     if isinstance(a, dict):
         return _open_dataset(**a)
 
     if isinstance(a, (list, tuple)):
         return _open_dataset(*a)
 
-    raise NotImplementedError("Unsupported argument: " + type(a))
+    raise NotImplementedError(f"Unsupported argument: {type(a)}")
 
 
 def _auto_adjust(datasets, kwargs):
 
     if "adjust" not in kwargs:
         return datasets, kwargs
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/data/select.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/data/select.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,19 @@
     def name_to_index(self):
         return {k: i for i, k in enumerate(self.variables)}
 
     @cached_property
     def statistics(self):
         return {k: v[self.indices] for k, v in self.dataset.statistics.items()}
 
+    def statistics_tendencies(self, delta=None):
+        if delta is None:
+            delta = self.frequency
+        return {k: v[self.indices] for k, v in self.dataset.statistics_tendencies(delta).items()}
+
     def metadata_specific(self, **kwargs):
         return super().metadata_specific(indices=self.indices, **kwargs)
 
     def source(self, index):
         return Source(self, index, self.dataset.source(self.indices[index]))
 
     def tree(self):
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/data/statistics.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/data/statistics.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,14 +25,19 @@
                 f"Incompatible variables: {dataset.variables} and {self._statistic.variables} ({dataset} {self._statistic})"
             )
 
     @cached_property
     def statistics(self):
         return self._statistic.statistics
 
+    def statistics_tendencies(self, delta=None):
+        if delta is None:
+            delta = self.frequency
+        return self._statistic.statistics_tendencies(delta)
+
     def metadata_specific(self, **kwargs):
         return super().metadata_specific(
             statistics=self._statistic.metadata_specific(),
             **kwargs,
         )
 
     def tree(self):
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/data/stores.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/data/stores.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 
     def __iter__(self):
         raise NotImplementedError()
 
 
 class HTTPStore(ReadOnlyStore):
     """We write our own HTTPStore because the one used by zarr (fsspec) does not play
-    well with fork() and multiprocessing."""
+    well with fork() and multiprocessing.
+    """
 
     def __init__(self, url):
         self.url = url
 
     def __getitem__(self, key):
         import requests
 
@@ -55,15 +56,16 @@
 
         r.raise_for_status()
         return r.content
 
 
 class S3Store(ReadOnlyStore):
     """We write our own S3Store because the one used by zarr (fsspec) does not play well
-    with fork() and multiprocessing."""
+    with fork() and multiprocessing.
+    """
 
     def __init__(self, url):
         import boto3
 
         self.bucket, self.key = url[5:].split("/", 1)
 
         # TODO: get the profile name from the url
@@ -96,29 +98,32 @@
         warnings.warn("DebugStore: iterating over the store")
         return iter(self.store)
 
     def __contains__(self, key):
         return key in self.store
 
 
-def open_zarr(path, dont_fail=False):
+def open_zarr(path, dont_fail=False, cache=None):
     try:
         store = path
 
         if store.startswith("http://") or store.startswith("https://"):
             store = HTTPStore(store)
 
         elif store.startswith("s3://"):
             store = S3Store(store)
 
         if DEBUG_ZARR_LOADING:
             if isinstance(store, str):
                 store = zarr.storage.DirectoryStore(store)
             store = DebugStore(store)
 
+        if cache is not None:
+            store = zarr.LRUStoreCache(store, max_size=cache)
+
         return zarr.convenience.open(store, "r")
     except zarr.errors.PathNotFoundError:
         if not dont_fail:
             raise zarr.errors.PathNotFoundError(path)
 
 
 class Zarr(Dataset):
@@ -209,14 +214,29 @@
         return dict(
             mean=self.z.mean[:],
             stdev=self.z.stdev[:],
             maximum=self.z.maximum[:],
             minimum=self.z.minimum[:],
         )
 
+    def statistics_tendencies(self, delta=None):
+        if delta is None:
+            delta = self.frequency
+        if isinstance(delta, int):
+            delta = f"{delta}h"
+        from anemoi.datasets.create.loaders import TendenciesStatisticsAddition
+
+        prefix = TendenciesStatisticsAddition.DATASET_NAME_PATTERN.format(delta=delta) + "_"
+        return dict(
+            mean=self.z[f"{prefix}mean"][:],
+            stdev=self.z[f"{prefix}stdev"][:],
+            maximum=self.z[f"{prefix}maximum"][:],
+            minimum=self.z[f"{prefix}minimum"][:],
+        )
+
     @property
     def resolution(self):
         return self.z.attrs["resolution"]
 
     @property
     def field_shape(self):
         return tuple(self.z.attrs["field_shape"])
@@ -322,14 +342,18 @@
 
     def _report_missing(self, n):
         raise MissingDateError(f"Date {self.missing_to_dates[n]} is missing (index={n})")
 
     def tree(self):
         return Node(self, [], path=self.path, missing=sorted(self.missing))
 
+    @property
+    def label(self):
+        return "zarr*"
+
 
 def zarr_lookup(name):
 
     if name.endswith(".zarr") or name.endswith(".zip"):
         return name
 
     config = load_config()["datasets"]
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/data/subset.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/data/subset.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,11 +96,16 @@
         return Source(self, index, self.forward.source(index))
 
     def __repr__(self):
         return f"Subset({self.dataset},{self.dates[0]}...{self.dates[-1]}/{self.frequency})"
 
     @cached_property
     def missing(self):
-        return {self.indices[i] for i in self.dataset.missing if i in self.indices}
+        missing = self.dataset.missing
+        result = set()
+        for j, i in enumerate(self.indices):
+            if i in missing:
+                result.add(j)
+        return result
 
     def tree(self):
         return Node(self, [self.dataset.tree()], **self.reason)
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/data/unchecked.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/data/unchecked.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,14 +97,18 @@
         raise NotImplementedError()
 
     @property
     @check("check_same_variables")
     def statistics(self):
         raise NotImplementedError()
 
+    @check("check_same_variables")
+    def statistics_tendencies(self, delta=None):
+        raise NotImplementedError()
+
     @property
     def shape(self):
         raise NotImplementedError()
 
     @property
     def dtype(self):
         raise NotImplementedError()
@@ -127,17 +131,15 @@
         result = set()
         for d in self.datasets:
             result = result | d.missing
         return result
 
 
 class Chain(ConcatMixin, Unchecked):
-    """
-    Same as Concat, but with no checks
-    """
+    """Same as Concat, but with no checks"""
 
     def __len__(self):
         return sum(len(d) for d in self.datasets)
 
     def __getitem__(self, n):
         return tuple(d[n] for d in self.datasets)
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/dates/__init__.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/dates/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/dates/groups.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/dates/groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 import itertools
 
 from anemoi.datasets.dates import Dates
 from anemoi.datasets.dates import no_time_zone
 
 
 class Groups:
-    """
-    >>> list(Groups(group_by="daily", start="2023-01-01 00:00", end="2023-01-05 00:00", frequency=12))[0]
+    """>>> list(Groups(group_by="daily", start="2023-01-01 00:00", end="2023-01-05 00:00", frequency=12))[0]
     [datetime.datetime(2023, 1, 1, 0, 0), datetime.datetime(2023, 1, 1, 12, 0)]
 
     >>> list(Groups(group_by="daily", start="2023-01-01 00:00", end="2023-01-05 00:00", frequency=12))[1]
     [datetime.datetime(2023, 1, 2, 0, 0), datetime.datetime(2023, 1, 2, 12, 0)]
 
     >>> g = Groups(group_by=3, start="2023-01-01 00:00", end="2023-01-05 00:00", frequency=24)
     >>> len(list(g))
```

### Comparing `anemoi-datasets-0.1.4/anemoi/datasets/grids.py` & `anemoi_datasets-0.1.6/src/anemoi/datasets/grids.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,17 +120,15 @@
     lons,
     global_lats,
     global_lons,
     cropping_distance=2.0,
     min_distance_km=None,
     plot=None,
 ):
-    """
-    Return a mask for the points in [global_lats, global_lons] that are inside of [lats, lons]
-    """
+    """Return a mask for the points in [global_lats, global_lons] that are inside of [lats, lons]"""
     from scipy.spatial import KDTree
 
     # TODO: transform min_distance from lat/lon to xyz
 
     assert global_lats.ndim == 1
     assert global_lons.ndim == 1
     assert lats.ndim == 1
@@ -231,17 +229,15 @@
 def thinning_mask(
     lats,
     lons,
     global_lats,
     global_lons,
     cropping_distance=2.0,
 ):
-    """
-    Return the list of points in [lats, lons] closest to [global_lats, global_lons]
-    """
+    """Return the list of points in [lats, lons] closest to [global_lats, global_lons]"""
     from scipy.spatial import KDTree
 
     assert global_lats.ndim == 1
     assert global_lons.ndim == 1
     assert lats.ndim == 1
     assert lons.ndim == 1
```


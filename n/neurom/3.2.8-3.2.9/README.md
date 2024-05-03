# Comparing `tmp/neurom-3.2.8.tar.gz` & `tmp/neurom-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurom-3.2.8.tar", last modified: Wed Feb  7 12:42:23 2024, max compression
+gzip compressed data, was "neurom-3.2.9.tar", last modified: Mon Apr 15 13:03:15 2024, max compression
```

## Comparing `neurom-3.2.8.tar` & `neurom-3.2.9.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:42:23.887294 neurom-3.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:42:23.871294 neurom-3.2.8/.binder/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-07 12:42:06.000000 neurom-3.2.8/.binder/postBuild
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-07 12:42:06.000000 neurom-3.2.8/.binder/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-07 12:42:06.000000 neurom-3.2.8/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-07 12:42:06.000000 neurom-3.2.8/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-07 12:42:06.000000 neurom-3.2.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:42:23.863294 neurom-3.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:42:23.871294 neurom-3.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-02-07 12:42:06.000000 neurom-3.2.8/.github/workflows/mirror-ebrains.yml
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-07 12:42:06.000000 neurom-3.2.8/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-07 12:42:06.000000 neurom-3.2.8/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-07 12:42:06.000000 neurom-3.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-02-07 12:42:06.000000 neurom-3.2.8/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-07 12:42:06.000000 neurom-3.2.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-02-07 12:42:06.000000 neurom-3.2.8/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-07 12:42:06.000000 neurom-3.2.8/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-02-07 12:42:06.000000 neurom-3.2.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-02-07 12:42:06.000000 neurom-3.2.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-07 12:42:06.000000 neurom-3.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-02-07 12:42:23.887294 neurom-3.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-02-07 12:42:06.000000 neurom-3.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-02-07 12:42:06.000000 neurom-3.2.8/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:42:23.871294 neurom-3.2.8/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/clean.sh
--rw-r--r--   0 runner    (1001) docker     (127)     7253 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:42:23.875294 neurom-3.2.8/doc/source/
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/definitions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/developer.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/features.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:42:23.875294 neurom-3.2.8/doc/source/images/
--rw-r--r--   0 runner    (1001) docker     (127)    27330 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/images/spherical_coordinates.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/images/spherical_coordinates.tex
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:42:23.875294 neurom-3.2.8/doc/source/logo/
--rw-r--r--   0 runner    (1001) docker     (127)   403060 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/logo/NeuroM.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/migration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/morph_check.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/morph_stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/spherical_coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-02-07 12:42:06.000000 neurom-3.2.8/doc/source/validation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:42:23.875294 neurom-3.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-02-07 12:42:06.000000 neurom-3.2.8/examples/boxplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-02-07 12:42:06.000000 neurom-3.2.8/examples/density_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4541 2024-02-07 12:42:06.000000 neurom-3.2.8/examples/end_to_end_distance.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2969 2024-02-07 12:42:06.000000 neurom-3.2.8/examples/extract_distribution.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3710 2024-02-07 12:42:06.000000 neurom-3.2.8/examples/features_graph_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6790 2024-02-07 12:42:06.000000 neurom-3.2.8/examples/get_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-02-07 12:42:06.000000 neurom-3.2.8/examples/histogram.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6050 2024-02-07 12:42:06.000000 neurom-3.2.8/examples/iteration_analysis.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3226 2024-02-07 12:42:06.000000 neurom-3.2.8/examples/nl_fst_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2957 2024-02-07 12:42:06.000000 neurom-3.2.8/examples/plot_somas.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4823 2024-02-07 12:42:06.000000 neurom-3.2.8/examples/radius_of_gyration.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2575 2024-02-07 12:42:06.000000 neurom-3.2.8/examples/section_ids.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2859 2024-02-07 12:42:06.000000 neurom-3.2.8/examples/soma_radius_fit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:42:23.879294 neurom-3.2.8/neurom/
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:42:23.879294 neurom-3.2.8/neurom/apps/
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/apps/annotate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/apps/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:42:23.879294 neurom-3.2.8/neurom/apps/config/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/apps/config/morph_check.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/apps/config/morph_stats.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/apps/morph_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    15020 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/apps/morph_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:42:23.879294 neurom-3.2.8/neurom/check/
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/check/morphology_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/check/morphtree.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/check/neuron_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/check/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:42:23.883294 neurom-3.2.8/neurom/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/core/dataformat.py
--rw-r--r--   0 runner    (1001) docker     (127)    18188 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/core/morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/core/neuron.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/core/population.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12976 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/core/soma.py
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/core/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:42:23.883294 neurom-3.2.8/neurom/features/
--rw-r--r--   0 runner    (1001) docker     (127)     9430 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/features/bifurcation.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/features/bifurcationfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)    27669 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/features/morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)    15769 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/features/neurite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/features/population.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/features/section.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/features/sectionfunc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:42:23.883294 neurom-3.2.8/neurom/geom/
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/geom/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:42:23.883294 neurom-3.2.8/neurom/io/
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8311 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/io/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17443 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/morphmath.py
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:42:23.883294 neurom-3.2.8/neurom/view/
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/view/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    17722 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/view/matplotlib_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    16900 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/view/matplotlib_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/view/plotly_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-02-07 12:42:06.000000 neurom-3.2.8/neurom/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:42:23.883294 neurom-3.2.8/neurom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-02-07 12:42:23.000000 neurom-3.2.8/neurom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-02-07 12:42:23.000000 neurom-3.2.8/neurom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 12:42:23.000000 neurom-3.2.8/neurom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-07 12:42:23.000000 neurom-3.2.8/neurom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-07 12:42:23.000000 neurom-3.2.8/neurom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-07 12:42:23.000000 neurom-3.2.8/neurom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-02-07 12:42:06.000000 neurom-3.2.8/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-02-07 12:42:06.000000 neurom-3.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 12:42:23.887294 neurom-3.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 12:42:06.000000 neurom-3.2.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-02-07 12:42:06.000000 neurom-3.2.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.498174 neurom-3.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.482174 neurom-3.2.9/.binder/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 13:03:10.000000 neurom-3.2.9/.binder/postBuild
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 13:03:10.000000 neurom-3.2.9/.binder/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-15 13:03:10.000000 neurom-3.2.9/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 13:03:10.000000 neurom-3.2.9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 13:03:10.000000 neurom-3.2.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.478174 neurom-3.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.482174 neurom-3.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-15 13:03:10.000000 neurom-3.2.9/.github/workflows/mirror-ebrains.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-15 13:03:10.000000 neurom-3.2.9/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-15 13:03:10.000000 neurom-3.2.9/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-15 13:03:10.000000 neurom-3.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-15 13:03:10.000000 neurom-3.2.9/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-15 13:03:10.000000 neurom-3.2.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-15 13:03:10.000000 neurom-3.2.9/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-15 13:03:10.000000 neurom-3.2.9/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-04-15 13:03:10.000000 neurom-3.2.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-15 13:03:10.000000 neurom-3.2.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 13:03:10.000000 neurom-3.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-15 13:03:15.498174 neurom-3.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-15 13:03:10.000000 neurom-3.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-15 13:03:10.000000 neurom-3.2.9/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.486173 neurom-3.2.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/clean.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     7253 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.486173 neurom-3.2.9/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/definitions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/developer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/features.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.486173 neurom-3.2.9/doc/source/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    27330 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/images/spherical_coordinates.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/images/spherical_coordinates.tex
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.486173 neurom-3.2.9/doc/source/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)   403060 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/logo/NeuroM.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/morph_check.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/morph_stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/spherical_coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-15 13:03:10.000000 neurom-3.2.9/doc/source/validation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.490174 neurom-3.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/density_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4541 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/end_to_end_distance.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2969 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/extract_distribution.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3710 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/features_graph_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6790 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/get_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/histogram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6050 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/iteration_analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3226 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/nl_fst_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2957 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/plot_somas.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4823 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/radius_of_gyration.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2575 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/section_ids.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2859 2024-04-15 13:03:10.000000 neurom-3.2.9/examples/soma_radius_fit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.490174 neurom-3.2.9/neurom/
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.494174 neurom-3.2.9/neurom/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/apps/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/apps/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.494174 neurom-3.2.9/neurom/apps/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/apps/config/morph_check.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/apps/config/morph_stats.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/apps/morph_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15020 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/apps/morph_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.494174 neurom-3.2.9/neurom/check/
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/check/morphology_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/check/morphtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/check/neuron_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/check/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.494174 neurom-3.2.9/neurom/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/core/dataformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18188 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/core/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/core/neuron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/core/population.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12976 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/core/soma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.494174 neurom-3.2.9/neurom/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     9430 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/features/bifurcation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/features/bifurcationfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27669 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/features/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15769 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/features/neurite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/features/population.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/features/section.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/features/sectionfunc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.494174 neurom-3.2.9/neurom/geom/
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/geom/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.498174 neurom-3.2.9/neurom/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8311 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17443 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/morphmath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.498174 neurom-3.2.9/neurom/view/
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/view/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17722 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/view/matplotlib_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16900 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/view/matplotlib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/view/plotly_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-15 13:03:10.000000 neurom-3.2.9/neurom/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:03:15.498174 neurom-3.2.9/neurom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-15 13:03:15.000000 neurom-3.2.9/neurom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-15 13:03:15.000000 neurom-3.2.9/neurom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:03:15.000000 neurom-3.2.9/neurom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 13:03:15.000000 neurom-3.2.9/neurom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-15 13:03:15.000000 neurom-3.2.9/neurom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 13:03:15.000000 neurom-3.2.9/neurom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-15 13:03:10.000000 neurom-3.2.9/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-15 13:03:10.000000 neurom-3.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:03:15.498174 neurom-3.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:03:10.000000 neurom-3.2.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-15 13:03:10.000000 neurom-3.2.9/tox.ini
```

### Comparing `neurom-3.2.8/.github/workflows/mirror-ebrains.yml` & `neurom-3.2.9/.github/workflows/mirror-ebrains.yml`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/.github/workflows/publish-sdist.yml` & `neurom-3.2.9/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/.github/workflows/run-tox.yml` & `neurom-3.2.9/.github/workflows/run-tox.yml`

 * *Files 19% similar despite different names*

```diff
@@ -24,14 +24,14 @@
       run: |
         python -m pip install --upgrade pip setuptools
         pip install tox-gh-actions
     - name: Run tox
       run: |
         tox
     - name: Upload to codecov
-      if: ${{matrix.python-version == '3.8'}}
-      uses: codecov/codecov-action@v1
+      uses: codecov/codecov-action@v4
       with:
         fail_ci_if_error: false
         files: ./coverage.xml
         flags: pytest
-        name: "neurom-py38"
+        name: "neurom-py${{ matrix.python-version }}"
+        token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `neurom-3.2.8/.gitlab-ci.yml` & `neurom-3.2.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/.zenodo.json` & `neurom-3.2.9/.zenodo.json`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/CHANGELOG.rst` & `neurom-3.2.9/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/LICENSE.txt` & `neurom-3.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/PKG-INFO` & `neurom-3.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurom
-Version: 3.2.8
+Version: 3.2.9
 Summary: NeuroM: a light-weight neuron morphology analysis package
 Author: Blue Brain Project, EPFL
 License: Copyright (c) 2015-2022 Blue Brain Project/EPFL 
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `neurom-3.2.8/README.md` & `neurom-3.2.9/README.md`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/asv.conf.json` & `neurom-3.2.9/asv.conf.json`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/Makefile` & `neurom-3.2.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/make.bat` & `neurom-3.2.9/doc/make.bat`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/api.rst` & `neurom-3.2.9/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/cli.rst` & `neurom-3.2.9/doc/source/cli.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/conf.py` & `neurom-3.2.9/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/definitions.rst` & `neurom-3.2.9/doc/source/definitions.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/developer.rst` & `neurom-3.2.9/doc/source/developer.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/documentation.rst` & `neurom-3.2.9/doc/source/documentation.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/examples.rst` & `neurom-3.2.9/doc/source/examples.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/features.rst` & `neurom-3.2.9/doc/source/features.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/images/spherical_coordinates.svg` & `neurom-3.2.9/doc/source/images/spherical_coordinates.svg`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/images/spherical_coordinates.tex` & `neurom-3.2.9/doc/source/images/spherical_coordinates.tex`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/index.rst` & `neurom-3.2.9/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/install.rst` & `neurom-3.2.9/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/license.rst` & `neurom-3.2.9/doc/source/license.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/logo/NeuroM.jpg` & `neurom-3.2.9/doc/source/logo/NeuroM.jpg`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/migration.rst` & `neurom-3.2.9/doc/source/migration.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/morph_check.rst` & `neurom-3.2.9/doc/source/morph_check.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/morph_stats.rst` & `neurom-3.2.9/doc/source/morph_stats.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/quickstart.rst` & `neurom-3.2.9/doc/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/spherical_coordinates.rst` & `neurom-3.2.9/doc/source/spherical_coordinates.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/tutorial.rst` & `neurom-3.2.9/doc/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/doc/source/validation.rst` & `neurom-3.2.9/doc/source/validation.rst`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/examples/boxplot.py` & `neurom-3.2.9/examples/boxplot.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/examples/density_plot.py` & `neurom-3.2.9/examples/density_plot.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/examples/end_to_end_distance.py` & `neurom-3.2.9/examples/end_to_end_distance.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/examples/extract_distribution.py` & `neurom-3.2.9/examples/extract_distribution.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/examples/features_graph_table.py` & `neurom-3.2.9/examples/features_graph_table.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/examples/get_features.py` & `neurom-3.2.9/examples/get_features.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/examples/histogram.py` & `neurom-3.2.9/examples/histogram.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/examples/iteration_analysis.py` & `neurom-3.2.9/examples/iteration_analysis.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/examples/nl_fst_compat.py` & `neurom-3.2.9/examples/nl_fst_compat.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/examples/plot_somas.py` & `neurom-3.2.9/examples/plot_somas.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/examples/radius_of_gyration.py` & `neurom-3.2.9/examples/radius_of_gyration.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/examples/section_ids.py` & `neurom-3.2.9/examples/section_ids.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/examples/soma_radius_fit.py` & `neurom-3.2.9/examples/soma_radius_fit.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/__init__.py` & `neurom-3.2.9/neurom/__init__.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/apps/__init__.py` & `neurom-3.2.9/neurom/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/apps/annotate.py` & `neurom-3.2.9/neurom/apps/annotate.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/apps/cli.py` & `neurom-3.2.9/neurom/apps/cli.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/apps/config/morph_check.yaml` & `neurom-3.2.9/neurom/apps/config/morph_check.yaml`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/apps/morph_check.py` & `neurom-3.2.9/neurom/apps/morph_check.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/apps/morph_stats.py` & `neurom-3.2.9/neurom/apps/morph_stats.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/check/__init__.py` & `neurom-3.2.9/neurom/check/__init__.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/check/morphology_checks.py` & `neurom-3.2.9/neurom/check/morphology_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Contains functions for checking validity of morphology neurites and somata.
 """
 from itertools import islice
 
 import numpy as np
 from neurom import NeuriteType
 from neurom.check import CheckResult
-from neurom.check.morphtree import get_flat_neurites
+from neurom.check.morphtree import get_flat_neurites, back_tracking_segments
 from neurom.core.morphology import Section, iter_neurites, iter_sections, iter_segments
 from neurom.core.dataformat import COLS
 from neurom.exceptions import NeuroMError
 from neurom.morphmath import section_length, segment_length
 from neurom.utils import flatten
 
 
@@ -351,7 +351,17 @@
     return CheckResult(len(bad_ids) == 0, bad_ids)
 
 
 def has_no_single_children(morph):
     """Check if the morphology has sections with only one child section."""
     bad_ids = [section.id for section in iter_sections(morph) if len(section.children) == 1]
     return CheckResult(len(bad_ids) == 0, bad_ids)
+
+
+def has_no_back_tracking(morph):
+    """Check if the morphology has sections with back-tracks."""
+    bad_ids = [
+        (i, morph.section(i[0]).points[np.newaxis, i[1]])
+        for neurite in iter_neurites(morph)
+        for i in back_tracking_segments(neurite)
+    ]
+    return CheckResult(len(bad_ids) == 0, bad_ids)
```

### Comparing `neurom-3.2.8/neurom/check/morphtree.py` & `neurom-3.2.9/neurom/check/morphtree.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,29 +80,30 @@
     assert method in ('tolerance', 'ratio'), "Method must be one of 'tolerance', 'ratio'"
     if method == 'ratio':
         sorted_ext = np.sort(ext)
         return sorted_ext[0] / sorted_ext[1] < float(tol)
     return any(ext < float(tol))
 
 
-def is_back_tracking(neurite):
+def back_tracking_segments(neurite):
     """Check if a neurite process backtracks to a previous node.
 
     Back-tracking takes place
     when a daughter of a branching process goes back and either overlaps with a previous point, or
     lies inside the cylindrical volume of the latter.
 
     Args:
         neurite(Neurite): neurite to operate on
 
     Returns:
-        True Under the following scenaria:
-            1. A segment endpoint falls back and overlaps with a previous segment's point
-            2. The geometry of a segment overlaps with a previous one in the section
+        A generator of tuples containing the section ID and the two segment indices in this section
+        for which a back tracking is detected (so the first point of these segments can be
+        retrieved with ``morph.section(section_id).points[segment_id]``.
     """
+    # pylint: disable=too-many-locals
     def pair(segs):
         """Pairs the input list into triplets."""
         return zip(segs, segs[1:])
 
     def coords(node):
         """Returns the first three values of the tree that correspond to the x, y, z coordinates."""
         return node[COLS.XYZ]
@@ -175,17 +176,35 @@
         # group each section's points intro triplets
         segment_pairs = list(filter(is_not_zero_seg, pair(sec.points)))
 
         # filter out zero length segments
         for i, seg1 in enumerate(segment_pairs[1:]):
             # check if the end point of the segment lies within the previous
             # ones in the current section
-            for seg2 in segment_pairs[0: i + 1]:
+            for j, seg2 in enumerate(segment_pairs[0: i + 1]):
                 if is_inside_cylinder(seg1, seg2):
-                    return True
+                    yield (sec.id, i, j)
+
+
+def is_back_tracking(neurite):
+    """Check if a neurite process backtracks to a previous node.
+
+    See back_tracking_segments() for more details.
+
+    Args:
+        neurite(Neurite): neurite to operate on
+
+    Returns:
+        True Under the following scenaria:
+            1. A segment endpoint falls back and overlaps with a previous segment's point
+            2. The geometry of a segment overlaps with a previous one in the section
+    """
+    for _i in back_tracking_segments(neurite):
+        # If one segment is found then the neurite is back tracking
+        return True
     return False
 
 
 def get_flat_neurites(morph, tol=0.1, method='ratio'):
     """Check if a morphology has neurites that are flat within a tolerance.
 
     Args:
```

### Comparing `neurom-3.2.8/neurom/check/runner.py` & `neurom-3.2.9/neurom/check/runner.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/core/__init__.py` & `neurom-3.2.9/neurom/core/__init__.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/core/dataformat.py` & `neurom-3.2.9/neurom/core/dataformat.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/core/morphology.py` & `neurom-3.2.9/neurom/core/morphology.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/core/population.py` & `neurom-3.2.9/neurom/core/population.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/core/soma.py` & `neurom-3.2.9/neurom/core/soma.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/core/types.py` & `neurom-3.2.9/neurom/core/types.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/exceptions.py` & `neurom-3.2.9/neurom/exceptions.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/features/__init__.py` & `neurom-3.2.9/neurom/features/__init__.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/features/bifurcation.py` & `neurom-3.2.9/neurom/features/bifurcation.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/features/morphology.py` & `neurom-3.2.9/neurom/features/morphology.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/features/neurite.py` & `neurom-3.2.9/neurom/features/neurite.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/features/population.py` & `neurom-3.2.9/neurom/features/population.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/features/section.py` & `neurom-3.2.9/neurom/features/section.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/geom/__init__.py` & `neurom-3.2.9/neurom/geom/__init__.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/geom/transform.py` & `neurom-3.2.9/neurom/geom/transform.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/io/__init__.py` & `neurom-3.2.9/neurom/io/__init__.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/io/utils.py` & `neurom-3.2.9/neurom/io/utils.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/morphmath.py` & `neurom-3.2.9/neurom/morphmath.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/stats.py` & `neurom-3.2.9/neurom/stats.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/utils.py` & `neurom-3.2.9/neurom/utils.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/view/__init__.py` & `neurom-3.2.9/neurom/view/__init__.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/view/dendrogram.py` & `neurom-3.2.9/neurom/view/dendrogram.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/view/matplotlib_impl.py` & `neurom-3.2.9/neurom/view/matplotlib_impl.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/view/matplotlib_utils.py` & `neurom-3.2.9/neurom/view/matplotlib_utils.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/view/plotly_impl.py` & `neurom-3.2.9/neurom/view/plotly_impl.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom/viewer.py` & `neurom-3.2.9/neurom/viewer.py`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/neurom.egg-info/PKG-INFO` & `neurom-3.2.9/neurom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurom
-Version: 3.2.8
+Version: 3.2.9
 Summary: NeuroM: a light-weight neuron morphology analysis package
 Author: Blue Brain Project, EPFL
 License: Copyright (c) 2015-2022 Blue Brain Project/EPFL 
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `neurom-3.2.8/neurom.egg-info/SOURCES.txt` & `neurom-3.2.9/neurom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/pylintrc` & `neurom-3.2.9/pylintrc`

 * *Files identical despite different names*

### Comparing `neurom-3.2.8/pyproject.toml` & `neurom-3.2.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -56,10 +56,14 @@
 Tracker = "https://github.com/BlueBrain/NeuroM/issues"
 
 [project.scripts]
 neurom = 'neurom.apps.cli:cli'
 
 [tool.setuptools.packages.find]
 include = ["neurom"]
+namespaces = false
+
+[tool.setuptools.package-data]
+"*" = ["morph_check.yaml", "morph_stats.yaml"]
 
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
```

### Comparing `neurom-3.2.8/tox.ini` & `neurom-3.2.9/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 [tox]
 envlist =
     lint
     docs
     coverage
     tutorial
+    check-packaging
     py{38,39,310,311,312}
 
 [testenv]
 deps =
     {[base]testdeps}
     pytest-cov
 extras = plotly
@@ -55,20 +56,29 @@
 deps =
     {[base]testdeps}
     nbmake
     ipywidgets
 commands =
     pytest --nbmake .
 
+[testenv:check-packaging]
+skip_install = true
+deps =
+    build
+    twine
+commands =
+    python -m build -o {envtmpdir}/dist
+    twine check {envtmpdir}/dist/*
+
 [pycodestyle]
 max-line-length=100
 
 [pydocstyle]
 convention = google
 
 [gh-actions]
 python =
   3.8: py38, lint
   3.9: py39, docs
   3.10: py310, tutorial
-  3.11: py311
+  3.11: py311, check-packaging
   3.12: py312
```


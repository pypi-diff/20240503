# Comparing `tmp/romanisim-0.5.0.tar.gz` & `tmp/romanisim-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "romanisim-0.5.0.tar", last modified: Tue Feb 20 14:06:03 2024, max compression
+gzip compressed data, was "romanisim-0.5.1.tar", last modified: Fri May  3 14:25:23 2024, max compression
```

## Comparing `romanisim-0.5.0.tar` & `romanisim-0.5.1.tar`

### file list

```diff
@@ -1,90 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:06:03.992075 romanisim-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-20 14:05:41.000000 romanisim-0.5.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:06:03.980075 romanisim-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-20 14:05:41.000000 romanisim-0.5.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:06:03.980075 romanisim-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-20 14:05:41.000000 romanisim-0.5.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-02-20 14:05:41.000000 romanisim-0.5.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-02-20 14:05:41.000000 romanisim-0.5.0/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-02-20 14:05:41.000000 romanisim-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-02-20 14:05:41.000000 romanisim-0.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-20 14:05:41.000000 romanisim-0.5.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-02-20 14:05:41.000000 romanisim-0.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-02-20 14:05:41.000000 romanisim-0.5.0/JenkinsfileRT_dev
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-02-20 14:05:41.000000 romanisim-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-02-20 14:06:03.992075 romanisim-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-02-20 14:05:41.000000 romanisim-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:06:03.980075 romanisim-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-02-20 14:05:41.000000 romanisim-0.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-02-20 14:05:41.000000 romanisim-0.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-20 14:05:41.000000 romanisim-0.5.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:06:03.984075 romanisim-0.5.0/docs/romanisim/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-02-20 14:05:41.000000 romanisim-0.5.0/docs/romanisim/apt.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-02-20 14:05:41.000000 romanisim-0.5.0/docs/romanisim/bandpass.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-02-20 14:05:41.000000 romanisim-0.5.0/docs/romanisim/catalog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-02-20 14:05:41.000000 romanisim-0.5.0/docs/romanisim/image.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-02-20 14:05:41.000000 romanisim-0.5.0/docs/romanisim/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-02-20 14:05:41.000000 romanisim-0.5.0/docs/romanisim/l1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-02-20 14:05:41.000000 romanisim-0.5.0/docs/romanisim/l2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-02-20 14:05:41.000000 romanisim-0.5.0/docs/romanisim/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-02-20 14:05:41.000000 romanisim-0.5.0/docs/romanisim/parameters.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-02-20 14:05:41.000000 romanisim-0.5.0/docs/romanisim/psf.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-02-20 14:05:41.000000 romanisim-0.5.0/docs/romanisim/refs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-02-20 14:05:41.000000 romanisim-0.5.0/docs/romanisim/running.rst
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-20 14:05:41.000000 romanisim-0.5.0/docs/romanisim/util.rst
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-20 14:05:41.000000 romanisim-0.5.0/docs/romanisim/wcs.rst
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-20 14:05:41.000000 romanisim-0.5.0/docs/rtd_environment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-02-20 14:05:41.000000 romanisim-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-02-20 14:05:41.000000 romanisim-0.5.0/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:06:03.988075 romanisim-0.5.0/romanisim/
--rwxr-xr-x   0 runner    (1001) docker     (127)      853 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/apt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/bandpass.py
--rw-r--r--   0 runner    (1001) docker     (127)    14833 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/cr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:06:03.988075 romanisim-0.5.0/romanisim/data/
--rw-r--r--   0 runner    (1001) docker     (127)    20073 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/data/Roman_effarea_20201130.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/gaia.py
--rw-r--r--   0 runner    (1001) docker     (127)    33955 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    21749 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/l1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/nonlinearity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/psf.py
--rw-r--r--   0 runner    (1001) docker     (127)    25518 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/ramp.py
--rw-r--r--   0 runner    (1001) docker     (127)  1212857 2024-02-20 14:06:03.000000 romanisim-0.5.0/romanisim/ramp_fit_casertano.c
--rw-r--r--   0 runner    (1001) docker     (127)     7727 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/ramp_fit_casertano.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:06:03.988075 romanisim-0.5.0/romanisim/regtest/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/regtest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/regtest/test_l1.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7903 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/ris_make_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:06:03.992075 romanisim-0.5.0/romanisim/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8894 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/tests/test_bandpass.py
--rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/tests/test_cr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/tests/test_gaia.py
--rw-r--r--   0 runner    (1001) docker     (127)    31442 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/tests/test_l1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/tests/test_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/tests/test_persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/tests/test_psf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/tests/test_ramp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/tests/test_ris_make_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/tests/test_wcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    13409 2024-02-20 14:05:41.000000 romanisim-0.5.0/romanisim/wcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:06:03.992075 romanisim-0.5.0/romanisim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-02-20 14:06:03.000000 romanisim-0.5.0/romanisim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-02-20 14:06:03.000000 romanisim-0.5.0/romanisim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 14:06:03.000000 romanisim-0.5.0/romanisim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 14:06:03.000000 romanisim-0.5.0/romanisim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-02-20 14:06:03.000000 romanisim-0.5.0/romanisim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-20 14:06:03.000000 romanisim-0.5.0/romanisim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:06:03.992075 romanisim-0.5.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4444 2024-02-20 14:05:41.000000 romanisim-0.5.0/scripts/romanisim-make-image
--rwxr-xr-x   0 runner    (1001) docker     (127)     9940 2024-02-20 14:05:41.000000 romanisim-0.5.0/scripts/romanisim-make-stack
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 14:06:03.992075 romanisim-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-02-20 14:05:41.000000 romanisim-0.5.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-02-20 14:05:41.000000 romanisim-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.542558 romanisim-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-03 14:25:08.000000 romanisim-0.5.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.518558 romanisim-0.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-03 14:25:08.000000 romanisim-0.5.1/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.522558 romanisim-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-03 14:25:08.000000 romanisim-0.5.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-03 14:25:08.000000 romanisim-0.5.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-03 14:25:08.000000 romanisim-0.5.1/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-03 14:25:08.000000 romanisim-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-03 14:25:08.000000 romanisim-0.5.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-03 14:25:08.000000 romanisim-0.5.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-03 14:25:08.000000 romanisim-0.5.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-03 14:25:08.000000 romanisim-0.5.1/JenkinsfileRT_dev
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-03 14:25:08.000000 romanisim-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-03 14:25:23.542558 romanisim-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-03 14:25:08.000000 romanisim-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.522558 romanisim-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.522558 romanisim-0.5.1/docs/romanisim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/apt.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/bandpass.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/catalog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/image.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/l1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/l2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/psf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/refs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/running.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/util.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/wcs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/rtd_environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-03 14:25:08.000000 romanisim-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-03 14:25:08.000000 romanisim-0.5.1/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.530557 romanisim-0.5.1/romanisim/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      853 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/apt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/bandpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14833 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/cr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.530557 romanisim-0.5.1/romanisim/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    20073 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/data/Roman_effarea_20201130.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  3936671 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/data/gaia-270-66-2027-06-01.ecsv
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34479 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21790 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/l1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/nonlinearity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7804 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/psf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25518 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1213393 2024-05-03 14:25:22.000000 romanisim-0.5.1/romanisim/ramp_fit_casertano.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7727 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/ramp_fit_casertano.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.538558 romanisim-0.5.1/romanisim/regtest/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/regtest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/regtest/test_l1.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11427 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/ris_make_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.538558 romanisim-0.5.1/romanisim/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8894 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_bandpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_cr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_gaia.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31953 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_l1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_psf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_ris_make_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13874 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/wcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.542558 romanisim-0.5.1/romanisim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-03 14:25:23.000000 romanisim-0.5.1/romanisim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-03 14:25:23.000000 romanisim-0.5.1/romanisim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:25:23.000000 romanisim-0.5.1/romanisim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:25:22.000000 romanisim-0.5.1/romanisim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-03 14:25:23.000000 romanisim-0.5.1/romanisim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 14:25:23.000000 romanisim-0.5.1/romanisim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.538558 romanisim-0.5.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-03 14:25:08.000000 romanisim-0.5.1/scripts/romancal_make_all_l1s.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-03 14:25:08.000000 romanisim-0.5.1/scripts/romancal_make_regtest_l1s.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2193 2024-05-03 14:25:08.000000 romanisim-0.5.1/scripts/romanisim-make-catalog
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5283 2024-05-03 14:25:08.000000 romanisim-0.5.1/scripts/romanisim-make-image
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10443 2024-05-03 14:25:08.000000 romanisim-0.5.1/scripts/romanisim-make-stack
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 14:25:23.542558 romanisim-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-03 14:25:08.000000 romanisim-0.5.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-03 14:25:08.000000 romanisim-0.5.1/tox.ini
```

### Comparing `romanisim-0.5.0/.github/workflows/build.yml` & `romanisim-0.5.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/.github/workflows/ci.yml` & `romanisim-0.5.1/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     runs-on: ubuntu-latest
     outputs:
       path: ${{ steps.data.outputs.path }}
       hash: ${{ steps.data_hash.outputs.hash }}
       webbpsf_path: ${{ steps.webbpsf_path.outputs.path }}
       galsim_cat_path: ${{ steps.galsim_cat_path.outputs.path }}
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - id: data
         run: |
           echo "webbpsf_url=https://stsci.box.com/shared/static/0ojjfg3cieqdpd18vl1bjnpe63r82dx8.gz" >> $GITHUB_OUTPUT
           echo "galsim_url=https://github.com/GalSim-developers/GalSim/raw/releases/2.4/examples/data/" >> $GITHUB_OUTPUT
           echo "path=/tmp/data" >> $GITHUB_OUTPUT
@@ -49,33 +49,38 @@
           tar -xzvf minimal-webbpsf-data.tar.gz
           mkdir galsim-data
           wget ${{ steps.data.outputs.galsim_url }}/real_galaxy_catalog_23.5_example.fits -O galsim-data/real_galaxy_catalog_23.5_example.fits
           wget ${{ steps.data.outputs.galsim_url }}/real_galaxy_catalog_23.5_example_selection.fits -O galsim-data/real_galaxy_catalog_23.5_example_selection.fits
           wget ${{ steps.data.outputs.galsim_url }}/real_galaxy_catalog_23.5_example_fits.fits -O galsim-data/real_galaxy_catalog_23.5_example_fits.fits
       - id: data_hash
         run: echo "hash=${{ hashFiles( 'romanisim/data' ) }}" >> $GITHUB_OUTPUT
-      - uses: actions/cache@v3
+      - uses: actions/cache@v4
         with:
           path: ${{ steps.data.outputs.path }}
           key: data-${{ steps.data_hash.outputs.hash }}
       - id: webbpsf_path
         run: echo "path=${{ steps.data.outputs.path }}/webbpsf-data" >> $GITHUB_OUTPUT
       - id: galsim_cat_path
         run: echo "path=${{ steps.data.outputs.path }}/galsim-data/real_galaxy_catalog_23.5_example.fits" >> $GITHUB_OUTPUT
   test:
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/tox.yml@main
     needs: [ data ]
     with:
+      libraries: |
+        brew:
+          - eigen
+          - fftw
       setenv: |
         WEBBPSF_PATH: ${{ needs.data.outputs.webbpsf_path }}
         GALSIM_CAT_PATH: ${{ needs.data.outputs.galsim_cat_path }}
+        FFTW_DIR: /opt/homebrew/opt/fftw/lib/
       cache-path: ${{ needs.data.outputs.path }}
       cache-key: data-${{ needs.data.outputs.hash }}
       envs: |
-        - linux: py39-oldestdeps-cov-xdist
-        - linux: py39-xdist
+        - linux: py310-oldestdeps-cov-xdist
         - linux: py310-xdist
+        - linux: py311-xdist
         - linux: py3-xdist
         - macos: py3-xdist
         - linux: py3-pyargs-xdist
         - linux: py3-cov-xdist
           coverage: codecov
```

### Comparing `romanisim-0.5.0/.github/workflows/ci_cron.yml` & `romanisim-0.5.1/.github/workflows/ci_cron.yml`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     runs-on: ubuntu-latest
     outputs:
       path: ${{ steps.data.outputs.path }}
       hash: ${{ steps.data_hash.outputs.hash }}
       webbpsf_path: ${{ steps.webbpsf_path.outputs.path }}
       galsim_cat_path: ${{ steps.galsim_cat_path.outputs.path }}
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - id: data
         run: |
           echo "webbpsf_url=https://stsci.box.com/shared/static/0ojjfg3cieqdpd18vl1bjnpe63r82dx8.gz" >> $GITHUB_OUTPUT
           echo "galsim_url=https://github.com/GalSim-developers/GalSim/raw/releases/2.4/examples/data/" >> $GITHUB_OUTPUT
           echo "path=/tmp/data" >> $GITHUB_OUTPUT
@@ -38,28 +38,33 @@
           tar -xzvf minimal-webbpsf-data.tar.gz
           mkdir galsim-data
           wget ${{ steps.data.outputs.galsim_url }}/real_galaxy_catalog_23.5_example.fits -O galsim-data/real_galaxy_catalog_23.5_example.fits
           wget ${{ steps.data.outputs.galsim_url }}/real_galaxy_catalog_23.5_example_selection.fits -O galsim-data/real_galaxy_catalog_23.5_example_selection.fits
           wget ${{ steps.data.outputs.galsim_url }}/real_galaxy_catalog_23.5_example_fits.fits -O galsim-data/real_galaxy_catalog_23.5_example_fits.fits
       - id: data_hash
         run: echo "hash=${{ hashFiles( 'romanisim/data' ) }}" >> $GITHUB_OUTPUT
-      - uses: actions/cache@v3
+      - uses: actions/cache@v4
         with:
           path: ${{ steps.data.outputs.path }}
           key: data-${{ steps.data_hash.outputs.hash }}
       - id: webbpsf_path
         run: echo "path=${{ steps.data.outputs.path }}/webbpsf-data" >> $GITHUB_OUTPUT
       - id: galsim_cat_path
         run: echo "path=${{ steps.data.outputs.path }}/galsim-data/real_galaxy_catalog_23.5_example.fits" >> $GITHUB_OUTPUT
   test:
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/tox.yml@main
     needs: [ data ]
     with:
+      libraries: |
+        brew:
+          - eigen
+          - fftw
       setenv: |
         WEBBPSF_PATH: ${{ needs.data.outputs.webbpsf_path }}
         GALSIM_CAT_PATH: ${{ needs.data.outputs.galsim_cat_path }}
+        FFTW_DIR: /opt/homebrew/opt/fftw/lib/
       cache-path: ${{ needs.data.outputs.path }}
       cache-key: data-${{ needs.data.outputs.hash }}
       envs: |
-        - macos: py39-xdist
         - macos: py310-xdist
+        - macos: py311-xdist
         - linux: py3-devdeps-xdist
```

### Comparing `romanisim-0.5.0/.gitignore` & `romanisim-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/.readthedocs.yaml` & `romanisim-0.5.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/CODE_OF_CONDUCT.md` & `romanisim-0.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/JenkinsfileRT_dev` & `romanisim-0.5.1/JenkinsfileRT_dev`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/LICENSE` & `romanisim-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/PKG-INFO` & `romanisim-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romanisim
-Version: 0.5.0
+Version: 0.5.1
 Summary: Nancy Grace Roman Space Telescope WFI Simulator
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2022 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -38,43 +38,43 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asdf>=2.15.1
 Requires-Dist: astropy>=5.3
-Requires-Dist: crds>=10.3.1
+Requires-Dist: crds>=11.16.16
 Requires-Dist: defusedxml>=0.5.0
-Requires-Dist: galsim>=2.5.0
-Requires-Dist: rad>=0.18.0
-Requires-Dist: roman_datamodels>=0.18.0
+Requires-Dist: galsim>=2.5.1
+Requires-Dist: rad>=0.19.2
+Requires-Dist: roman_datamodels>=0.19.1
 Requires-Dist: gwcs>=0.18.1
 Requires-Dist: jsonschema>=4.8
 Requires-Dist: numpy>=1.22
-Requires-Dist: webbpsf>=1.0.0
+Requires-Dist: webbpsf>=1.2.1
 Requires-Dist: Cython>=0.29.21
 Provides-Extra: docs
 Requires-Dist: sphinx<7; extra == "docs"
 Requires-Dist: sphinx-automodapi; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: stsci-rtd-theme; extra == "docs"
 Requires-Dist: sphinx-astropy; extra == "docs"
 Requires-Dist: sphinx-asdf>=0.1.1; extra == "docs"
 Requires-Dist: tomli; python_version < "3.11" and extra == "docs"
 Provides-Extra: test
 Requires-Dist: ci-watson>=0.3.0; extra == "test"
 Requires-Dist: colorama>=0.4.1; extra == "test"
 Requires-Dist: getch>=1.0.0; extra == "test"
-Requires-Dist: pytest>=4.6.0; extra == "test"
+Requires-Dist: pytest<=8.0,>=4.6.0; extra == "test"
 Requires-Dist: pytest-openfiles>=0.5.0; extra == "test"
 Requires-Dist: pytest-doctestplus>=0.10.0; extra == "test"
 Requires-Dist: pytest-cov>=2.9.0; extra == "test"
 Requires-Dist: flake8>=3.6.0; extra == "test"
 Requires-Dist: metrics_logger>=0.1.0; extra == "test"
 
 [![CI](https://github.com/spacetelescope/romanisim/actions/workflows/ci.yml/badge.svg)](https://github.com/spacetelescope/romanisim/actions/workflows/ci.yml) [![codecov](https://codecov.io/gh/spacetelescope/romanisim/branch/main/graph/badge.svg?token=pkoLtQOa2v)](https://codecov.io/gh/spacetelescope/romanisim)
```

### Comparing `romanisim-0.5.0/README.md` & `romanisim-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/docs/Makefile` & `romanisim-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/docs/conf.py` & `romanisim-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/docs/index.rst` & `romanisim-0.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/docs/romanisim/apt.rst` & `romanisim-0.5.1/docs/romanisim/apt.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/docs/romanisim/bandpass.rst` & `romanisim-0.5.1/docs/romanisim/bandpass.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/docs/romanisim/catalog.rst` & `romanisim-0.5.1/docs/romanisim/catalog.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/docs/romanisim/image.rst` & `romanisim-0.5.1/docs/romanisim/image.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/docs/romanisim/install.rst` & `romanisim-0.5.1/docs/romanisim/install.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/docs/romanisim/l1.rst` & `romanisim-0.5.1/docs/romanisim/l1.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/docs/romanisim/l2.rst` & `romanisim-0.5.1/docs/romanisim/l2.rst`

 * *Files 4% similar despite different names*

```diff
@@ -11,10 +11,9 @@
 
 The second approach follows `Casertano+2022 <https://webbpsf.readthedocs.io/en/latest/installation.html#installing-the-required-data-files>`_.  In this approach, a diagonal set of weights is used in place of the full covariance matrix.  The choice of weights depend on the particular pattern of reads assigned to each resultant and the amount of flux in the ramp, allowing them to interpolate from simply differencing the first and last resultants when the flux is very large to weighting the resultants by the number of reads when the flux is zero.  This approach more efficiently handles dealing with ramps that have been split by cosmic rays, and obtaining uncertainties within a few percent of the "optimal" weighting approach.  For these cases, we report final ramp slopes and variances derived from the inverse variance weighted subramp slopes and variances, using the read-noise derived variances.
 
 This is a fairly faithful representation of how level two image construction works, so there are not many additional effects to add here.  But mentioning some limitations:
 
 * We have a simplistic saturation treatment, just clipping resultants that exceed
   the saturation level to the saturation level and throwing a flag.
-* We do not include dark counts as part of the Poisson noise term in the ramp fitting.
 
 .. automodapi:: romanisim.ramp
```

### Comparing `romanisim-0.5.0/docs/romanisim/overview.rst` & `romanisim-0.5.1/docs/romanisim/overview.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/docs/romanisim/psf.rst` & `romanisim-0.5.1/docs/romanisim/psf.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Point Spread Function Modeling
 ==============================
 
 The simulator has two mechanisms for point source modeling.  The first uses the galsim implementation of the Roman point spread function; for more information, see the galsim Roman documentation.  The second uses the webbpsf package to make a model of the Roman PSF.
 
-In the current implementation, the simulator uses a spatially constant, achromatic bandpass for each filter when using webbpsf.  That is, the PSF is not modeled as varying across each SCA, nor does the PSF vary depending on the spectrum of the source being rendered.  However, it seems straightforward to implement either of these modes in the context of galsim, albeit at some computational expense.
+In the current implementation, the simulator uses a linearly varying, achromatic bandpass for each filter when using webbpsf.  That is, the PSF does not vary depending on the spectrum of the source being rendered.  However, it seems straightforward to implement either of these modes in the context of galsim, albeit at some computational expense.
 
 When using the galsim PSF, galsim's "photon shooting" mode is used for efficient rendering of chromatic sources.  When using webbpsf, FFTs are used to to do the convolution of the intrinsic source profile with the PSF and pixel grid of the instrument.
 
 .. automodapi:: romanisim.psf
```

### Comparing `romanisim-0.5.0/docs/romanisim/refs.rst` & `romanisim-0.5.1/docs/romanisim/refs.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/docs/romanisim/running.rst` & `romanisim-0.5.1/docs/romanisim/running.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/docs/romanisim/wcs.rst` & `romanisim-0.5.1/docs/romanisim/wcs.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/requirements-dev.txt` & `romanisim-0.5.1/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/__init__.py` & `romanisim-0.5.1/romanisim/__init__.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/apt.py` & `romanisim-0.5.1/romanisim/apt.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/bandpass.py` & `romanisim-0.5.1/romanisim/bandpass.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/catalog.py` & `romanisim-0.5.1/romanisim/catalog.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/cr.py` & `romanisim-0.5.1/romanisim/cr.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/data/Roman_effarea_20201130.csv` & `romanisim-0.5.1/romanisim/data/Roman_effarea_20201130.csv`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/gaia.py` & `romanisim-0.5.1/romanisim/gaia.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/image.py` & `romanisim-0.5.1/romanisim/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,19 +86,19 @@
     darkrate : np.ndarray[nx, ny] (float)
         dark rate image to subtract from ramps (electron / s)
     dq : np.ndarray[nresultants, nx, ny] (int)
         DQ image corresponding to resultants
 
     Returns
     -------
-    im : galsim.Image
+    im : np.ndarray
         best fitting slopes
-    var_rnoise : galsim.Image
+    var_rnoise : np.ndarray
         variance in slopes from read noise
-    var_poisson : galsim.Image
+    var_poisson : np.ndarray
         variance in slopes from source noise
     """
 
     if read_noise is None:
         read_noise = parameters.reference_data['readnoise']
 
     if gain is None:
@@ -126,24 +126,27 @@
         resultants * gain, dq & parameters.dq_do_not_use,
         read_noise * gain, read_pattern)
     # could iterate if we wanted to improve the flux estimates
 
     if darkrate is not None:
         ramppar[..., 1] -= darkrate
 
+    if isinstance(gain, u.Quantity):
+        gain = gain.value  # no values make sense except for electron / DN
+
     # The ramp fitter is not presently unit-aware; fix up the units by hand.
     # To do this right the ramp fitter should be made unit aware.
     # It takes a bit of work to get this right because we use the fact
     # that the variance of a Poisson distribution is equal to its mean,
     # which isn't true as soon as things start having units and requires
     # special handling.  And we use read_time without units a lot throughout
     # the code base.
-    slopes = ramppar[..., 1] * u.electron / u.s
-    readvar = rampvar[..., 0, 1, 1] * (u.electron / u.s)**2
-    poissonvar = rampvar[..., 1, 1, 1] * (u.electron / u.s)**2
+    slopes = ramppar[..., 1] / gain * u.DN / u.s
+    readvar = rampvar[..., 0, 1, 1] / gain**2 * (u.DN / u.s)**2
+    poissonvar = rampvar[..., 1, 1, 1] / gain**2 * (u.DN / u.s)**2
 
     if flat is not None:
         flat = np.clip(flat, 1e-9, np.inf)
         slopes /= flat
         readvar /= flat**2
         poissonvar /= flat**2
 
@@ -274,15 +277,19 @@
         image_pos = galsim.PositionD(xpos[i], ypos[i])
         profile = obj.profile
         if not chromatic:
             if obj.flux is None:
                 raise ValueError('Non-chromatic sources must have specified '
                                  'fluxes!')
             profile = profile.withFlux(obj.flux[filter_name])
-        final = galsim.Convolve(profile * flux_to_counts_factor, psf)
+        if hasattr(psf, 'at_position'):
+            psf0 = psf.at_position(xpos[i], ypos[i])
+        else:
+            psf0 = psf
+        final = galsim.Convolve(profile * flux_to_counts_factor, psf0)
         if chromatic:
             stamp = final.drawImage(
                 bandpass, center=image_pos, wcs=image.wcs.local(image_pos),
                 method='phot', rng=rng)
         else:
             try:
                 stamp = final.drawImage(center=image_pos,
@@ -447,15 +454,17 @@
         workim = image * 0
         workim += sky * maxflat * exptime
         workim.addNoise(poisson_noise)
         image += workim
 
     if not np.all(flat == 1):
         image.quantize()
-        image.array[:, :] = np.random.binomial(
+        rng_numpy_seed = rng.raw()
+        rng_numpy = np.random.default_rng(rng_numpy_seed)
+        image.array[:, :] = rng_numpy.binomial(
             image.array.astype('i4'), flat / maxflat)
 
     if dark is not None:
         workim = image * 0
         workim += dark * exptime
         workim.addNoise(poisson_noise)
         image += workim
@@ -464,15 +473,16 @@
     return objinfo
 
 
 def simulate_counts(metadata, objlist,
                     rng=None, seed=None,
                     ignore_distant_sources=10, usecrds=True,
                     webbpsf=True,
-                    darkrate=None, flat=None):
+                    darkrate=None, flat=None,
+                    psf_keywords=dict()):
     """Simulate total counts in a single SCA.
 
     This gives the total counts in an idealized instrument with no systematics;
     it includes only distortion & PSF convolution.
 
     Parameters
     ----------
@@ -488,14 +498,16 @@
         do not render sources more than this many pixels off edge of detector
     usecrds : bool
         use CRDS distortion map
     darkrate : float or np.ndarray[float]
         dark rate image to use (electrons / s)
     flat : float or np.ndarray[float]
         flat field to use
+    psf_keywords : dict
+        keywords passed to PSF generation routine
 
     Returns
     -------
     image : galsim.Image
         idealized image of scene as seen by Roman, giving total electron counts
         from rate sources (astronomical objects; backgrounds; dark current) in
         each pixel.
@@ -526,15 +538,16 @@
     imwcs = wcs.get_wcs(metadata, usecrds=usecrds)
     chromatic = False
     if (len(objlist) > 0
             and not isinstance(objlist, table.Table)  # this case is always gray
             and objlist[0].profile.spectral):
         chromatic = True
     psf = romanisim.psf.make_psf(sca, filter_name, wcs=imwcs,
-                                 chromatic=chromatic, webbpsf=webbpsf)
+                                 chromatic=chromatic, webbpsf=webbpsf,
+                                 variable=True, **psf_keywords)
     image = galsim.ImageF(roman.n_pix, roman.n_pix, wcs=imwcs, xmin=0, ymin=0)
     SCA_cent_pos = imwcs.toWorld(image.true_center)
     sky_level = roman.getSkyLevel(bandpass, world_pos=SCA_cent_pos,
                                   date=date.datetime, exptime=1)
     sky_level *= (1.0 + roman.stray_light_fraction)
     sky_image = image * 0
     imwcs.makeSkyImage(sky_image, sky_level)
@@ -655,15 +668,16 @@
 
     out['reffiles'] = reffiles
     return out
 
 
 def simulate(metadata, objlist,
              usecrds=True, webbpsf=True, level=2, crparam=dict(),
-             persistence=None, seed=None, rng=None, **kwargs
+             persistence=None, seed=None, rng=None,
+             psf_keywords=dict(), **kwargs
              ):
     """Simulate a sequence of observations on a field in different bandpasses.
 
     Parameters
     ----------
     metadata : dict
         metadata structure for Roman asdf file, including information about
@@ -689,14 +703,16 @@
     crparam : dict
         Parameters for cosmic ray simulations.  None for no cosmic rays.
         Empty dictionary for default parameters.
     rng : galsim.BaseDeviate
         Random number generator to use
     seed : int
         Seed for populating RNG.  Only used if rng is None.
+    psf_keywords : dict
+        Keywords passed to the PSF generation routine
 
     Returns
     -------
     image : roman_datamodels model
         simulated image
     extras : dict
         Dictionary of additionally valuable quantities.  Includes at least
@@ -750,15 +766,15 @@
 
     if persistence is None:
         persistence = romanisim.persistence.Persistence()
 
     log.info('Simulating filter {0}...'.format(filter_name))
     counts, simcatobj = simulate_counts(
         image_mod.meta, objlist, rng=rng, usecrds=usecrds, darkrate=darkrate,
-        webbpsf=webbpsf, flat=flat)
+        webbpsf=webbpsf, flat=flat, psf_keywords=psf_keywords)
     if level == 0:
         im = dict(data=counts.array, meta=dict(image_mod.meta.items()))
     else:
         l1, l1dq = romanisim.l1.make_l1(
             counts, ma_table_number, read_noise=read_noise, rng=rng, gain=gain,
             crparam=crparam,
             inv_linearity=inv_linearity,
@@ -782,14 +798,15 @@
 
     if reffiles:
         extras["simulate_reffiles"] = {}
         for key, value in reffiles.items():
             extras["simulate_reffiles"][key] = value
 
     extras['simcatobj'] = simcatobj
+    extras['wcs'] = wcs.convert_wcs_to_gwcs(counts.wcs)
     log.info('Simulation complete.')
     return im, extras
 
 
 def make_test_catalog_and_images(
         seed=12345, sca=7, filters=None, nobj=1000,
         usecrds=True, webbpsf=True, galaxy_sample_file_name=None, **kwargs):
@@ -860,20 +877,15 @@
     # amp33: leave blank for now.
     # data: image
     # var_flat: currently zero
     if metadata is not None:
         out['meta'].update(metadata)
 
     if imwcs is not None:  # add a WCS
-        if isinstance(imwcs, wcs.GWCS):
-            out['meta'].update(wcs=imwcs.wcs)
-        else:
-            # make a gwcs WCS from a galsim.roman WCS
-            out['meta'].update(
-                wcs=wcs.wcs_from_fits_header(imwcs.header.header))
+        out['meta'].update(wcs=wcs.convert_wcs_to_gwcs(imwcs))
 
     out['data'] = slope
     out['dq'] = np.zeros(slope.shape, dtype='u4')
     if dq is not None:
         out['dq'][:, :] = dq
     out['var_poisson'] = slopevar_poisson
     out['var_rnoise'] = slopevar_rn
```

### Comparing `romanisim-0.5.0/romanisim/l1.py` & `romanisim-0.5.1/romanisim/l1.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,14 +237,15 @@
         array of n_resultant images giving each resultant
     dq : np.ndarray[n_resultant, nx, ny]
         dq array marking CR hits in resultants
     """
     if not np.all(counts == np.round(counts)):
         raise ValueError('apportion_counts_to_resultants expects the counts '
                          'to be integers!')
+    counts = np.clip(counts, 0, 2 * 10**9).astype('i4')
 
     # Set rng for creating cosmic rays, persistence, and readnoise
     if rng is None and seed is None:
         seed = 46
         log.warning(
             'No RNG set, constructing a new default RNG from default seed.')
     if rng is None:
@@ -260,15 +261,15 @@
     # Convert readout times for each read entering a resultant to probabilities,
     # corresponding to the chance that a photon not yet assigned to a read so far
     # should be assigned to this read.
     pij = tij_to_pij(tij, remaining=True)
 
     # Create arrays to store various photon or electron counts and dq
     resultants = np.zeros((len(tij),) + counts.shape, dtype='f4')
-    counts_so_far = np.zeros(counts.shape, dtype='f4')
+    counts_so_far = np.zeros(counts.shape, dtype='i4')
     resultant_counts = np.zeros(counts.shape, dtype='f4')
     dq = np.zeros(resultants.shape, dtype=np.uint32)
 
     # Set initial instrument counts
     instrumental_so_far = 0
 
     if crparam is not None or persistence is not None:
@@ -284,15 +285,15 @@
     for i, pi in enumerate(pij):
         # Reset resultant counts
         resultant_counts[...] = 0
 
         # Loop over resultant probabilities
         for j, p in enumerate(pi):
             # Set read counts
-            read = rng_numpy.binomial((counts - counts_so_far).astype('i4'), p)
+            read = rng_numpy.binomial(counts - counts_so_far, p)
             counts_so_far += read
 
             # Apply cosmic rays
             if crparam is not None:
                 old_instrumental_so_far = instrumental_so_far.copy()
                 cr.simulate_crs(instrumental_so_far, parameters.read_time,
                                 **crparam, rng=rng_numpy_cr)
```

### Comparing `romanisim-0.5.0/romanisim/nonlinearity.py` & `romanisim-0.5.1/romanisim/nonlinearity.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/parameters.py` & `romanisim-0.5.1/romanisim/parameters.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,23 @@
                     [6 + x for x in range(8)],
                     [14],
                     [15 + x for x in range(9)],
                     [24 + x for x in range(25)]],
                 3: [[1 + x for x in range(25)],
                     [26 + x for x in range(8)],
                     [34],
-                    [35 + x for x in range(14)]]
+                    [35 + x for x in range(14)]],
+                109: [[1], [2, 3], [5, 6, 7], [10, 11, 12, 13],
+                      [15, 16, 17, 18, 19, 20], [21, 22, 23, 24, 25, 26],
+                      [27, 28, 29, 30, 31, 32], [33, 34, 35, 36, 37, 38],
+                      [39, 40, 41, 42, 43], [44]],
+                110: [[1], [2, 3, 4], [5, 6, 7], [8, 9, 10], [11, 12, 13],
+                      [14, 15, 16], [17, 18, 19], [20, 21, 22], [23, 24, 25],
+                      [26, 27, 28], [29, 30, 31], [32, 33, 34], [35, 36, 37],
+                      [38, 39, 40], [41, 42, 43], [44]],
                 }
 
 default_parameters_dictionary = {
     'instrument': {'name': 'WFI',
                    'detector': 'WFI07',
                    'optical_element': 'F184',
                    },
@@ -36,14 +44,18 @@
                  'dec_v1': 66.0,
                  },
     'wcsinfo': {'ra_ref': 270.0,
                 'dec_ref': 66.0,
                 'v2_ref': 0,
                 'v3_ref': 0,
                 'roll_ref': 0,
+                'vparity': -1,
+                'v3yangle': -60.0,
+                # I don't know what vparity and v3yangle should really be,
+                # but they are always -1 and -60 in existing files.
                 },
     'aperture': {'name': 'WFI_CEN',
                  'position_angle': 0
                 },
 }
 
 reference_data = {
```

### Comparing `romanisim-0.5.0/romanisim/persistence.py` & `romanisim-0.5.1/romanisim/persistence.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/ramp.py` & `romanisim-0.5.1/romanisim/ramp.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/ramp_fit_casertano.c` & `romanisim-0.5.1/romanisim/ramp_fit_casertano.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/core/include"
+            "/tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/core/include"
         ],
         "name": "romanisim.ramp_fit_casertano",
         "sources": [
             "romanisim/ramp_fit_casertano.pyx"
         ]
     },
     "module_name": "romanisim.ramp_fit_casertano"
@@ -42,18 +42,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -137,14 +137,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -198,14 +200,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -259,60 +263,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -395,14 +422,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -738,16 +768,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1091,15 +1126,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1178,15 +1213,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1294,32 +1329,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1651,177 +1669,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1854,42 +1872,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2712,30 +2730,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_8
-#define __PYX_HAVE_RT_ImportType_proto_3_0_8
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_8 {
-   __Pyx_ImportType_CheckSize_Error_3_0_8 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_8 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_8 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
@@ -18143,261 +18161,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18406,29 +18424,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18439,15 +18457,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18456,29 +18474,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18489,15 +18507,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18506,29 +18524,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18539,15 +18557,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18556,29 +18574,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18589,15 +18607,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18606,29 +18624,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18639,217 +18657,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18865,15 +18883,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18881,68 +18899,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18950,15 +18968,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18973,15 +18991,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18997,15 +19015,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19013,68 +19031,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19082,15 +19100,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19105,15 +19123,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19129,15 +19147,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19145,68 +19163,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19214,15 +19232,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19237,170 +19255,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -22691,26 +22709,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-mm26xe7y/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
@@ -23136,41 +23154,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_8(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 866, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -28040,18 +28058,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_3_0_8
-#define __PYX_HAVE_RT_ImportType_3_0_8
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -28097,23 +28115,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_8 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_8 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -29105,15 +29123,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `romanisim-0.5.0/romanisim/ramp_fit_casertano.pyx` & `romanisim-0.5.1/romanisim/ramp_fit_casertano.pyx`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/tests/test_bandpass.py` & `romanisim-0.5.1/romanisim/tests/test_bandpass.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/tests/test_catalog.py` & `romanisim-0.5.1/romanisim/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/tests/test_cr.py` & `romanisim-0.5.1/romanisim/tests/test_cr.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/tests/test_gaia.py` & `romanisim-0.5.1/romanisim/tests/test_gaia.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/tests/test_image.py` & `romanisim-0.5.1/romanisim/tests/test_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     assert np.allclose(slopes, 0)
     resultants[:, :, :] = np.arange(4)[:, None, None]
     resultants *= u.DN
     gain = 1 * u.electron / u.DN
     slopes, readvar, poissonvar = image.make_l2(
         resultants, read_pattern,
         gain=gain, flat=1, darkrate=0)
-    assert np.allclose(slopes, 1 / parameters.read_time / 4 * u.electron / u.s)
+    assert np.allclose(slopes, 1 / parameters.read_time / 4 * u.DN / u.s)
     assert np.all(np.array(slopes.shape) == np.array(readvar.shape))
     assert np.all(np.array(slopes.shape) == np.array(poissonvar.shape))
     assert np.all(readvar >= 0)
     assert np.all(poissonvar >= 0)
     slopes1, readvar1, poissonvar1 = image.make_l2(
         resultants, read_pattern, read_noise=1, darkrate=0)
     slopes2, readvar2, poissonvar2 = image.make_l2(
@@ -107,16 +107,18 @@
         darkrate=1 / parameters.read_time / 4)
     assert np.allclose(slopes, 0, atol=1e-6)
 
 
 def set_up_image_rendering_things():
     im = galsim.Image(100, 100, scale=0.1, xmin=0, ymin=0)
     filter_name = 'F158'
-    impsfgray = psf.make_psf(1, filter_name, webbpsf=True, chromatic=False)
-    impsfchromatic = psf.make_psf(1, filter_name, webbpsf=False, chromatic=True)
+    impsfgray = psf.make_psf(1, filter_name, webbpsf=True, chromatic=False,
+                             nlambda=1)  # nlambda = 1 speeds tests
+    impsfchromatic = psf.make_psf(1, filter_name, webbpsf=False,
+                                  chromatic=True)
     bandpass = roman.getBandpasses(AB_zeropoint=True)['H158']
     counts = 1000
     fluxdict = {filter_name: counts}
     from copy import deepcopy
     graycatalog = [
         catalog.CatalogObject(None, galsim.DeltaFunction(), deepcopy(fluxdict)),
         catalog.CatalogObject(None, galsim.Sersic(1, half_light_radius=0.2),
@@ -166,25 +168,25 @@
     - RSUBREQ-874 / DMS215: analytic model source generation
     """
     oversample = 4
     filter_name = 'F158'
     sca = 1
     pos = [50, 50]
     impsfgray = psf.make_psf(sca, filter_name, webbpsf=True, chromatic=False,
-                             pix=pos, oversample=oversample)
+                             pix=pos, oversample=oversample, nlambda=1)
     counts = 100000
     fluxdict = {filter_name: counts}
     psfcatalog = [catalog.CatalogObject(None, galsim.DeltaFunction(), fluxdict)]
     wfi = webbpsf.WFI()
     wfi.detector = f'SCA{sca:02d}'
     wfi.filter = filter_name
     wfi.detector_position = pos
     # oversample = kw.get('oversample', 4)
     # webbpsf doesn't do distortion
-    psfob = wfi.calc_psf(oversample=oversample)
+    psfob = wfi.calc_psf(oversample=oversample, nlambda=1)
     psfim = psfob[1].data * counts
     # PSF from WebbPSF
     im = galsim.Image(101, 101, scale=wfi.pixelscale, xmin=0, ymin=0)
     # also no distortion
     image.add_objects_to_image(im, psfcatalog, [pos[0]], [pos[1]],
                                impsfgray, flux_to_counts_factor=1,
                                filter_name=filter_name)
@@ -238,15 +240,15 @@
     mod = Sersic2D(amplitude=1, r_eff=oversample * sersic_hlr / wfi.pixelscale,
                    n=sersic_index,
                    x_0=pos[0] * oversample + off, y_0=pos[0] * oversample + off,
                    ellip=0, theta=0)
     modim = mod(xx, yy)
     from scipy.signal import fftconvolve
     # convolve with the PSF
-    psfob = wfi.calc_psf(oversample=oversample, fov_pixels=45)
+    psfob = wfi.calc_psf(oversample=oversample, fov_pixels=45, nlambda=1)
     psfim = psfob[0].data
     modim = fftconvolve(modim, psfim, mode='same')
     modim = np.sum(modim.reshape(-1, imsz, oversample), axis=-1)
     modim = np.sum(modim.reshape(imsz, oversample, -1), axis=1)
     bn = gammaincinv(2 * sersic_index, 0.5)
     g2n = gamma(2 * sersic_index)
     integral = (1 * (oversample * sersic_hlr / wfi.pixelscale)**2 * g2n * 2
@@ -435,15 +437,16 @@
         },
     }
     wcs.fill_in_parameters(meta, coord)
     im1 = image.simulate_counts(meta, chromcat, usecrds=False,
                                 webbpsf=False, ignore_distant_sources=100)
     im2 = image.simulate_counts(meta, graycat,
                                 usecrds=False, webbpsf=True,
-                                ignore_distant_sources=100)
+                                ignore_distant_sources=100,
+                                psf_keywords=dict(nlambda=1))
     im1 = im1[0].array
     im2 = im2[0].array
     maxim = np.where(im1 > im2, im1, im2)
     m = np.abs(im1 - im2) <= 20 * np.sqrt(maxim)
     assert np.all(m)
 
 
@@ -493,27 +496,29 @@
         o.sky_pos = center
         o.flux[filter_name] /= abfluxdict[filter_name]
     imdict['tabcatalog']['ra'] = center.ra.to(u.deg).value
     imdict['tabcatalog']['dec'] = center.dec.to(u.deg).value
     imdict['tabcatalog'][filter_name] = (
         imdict['tabcatalog'][filter_name] / abfluxdict[filter_name])
     l0 = image.simulate(meta, graycat, webbpsf=True, level=0,
-                        usecrds=False)
+                        usecrds=False, psf_keywords=dict(nlambda=1))
     l0tab = image.simulate(
-        meta, imdict['tabcatalog'], webbpsf=True, level=0, usecrds=False)
+        meta, imdict['tabcatalog'], webbpsf=True, level=0, usecrds=False,
+        psf_keywords=dict(nlambda=1))
     # seed = 0 is special and means "don't actually use a seed."  Any other
     # choice of seed gives deterministic behavior
     # note that we have scaled down the size of the image to 100x100 pix
     # in order to save time.  But the CR module fixes the area of the detector
     # rather than the area of a pixel, so this means that all of the normal
     # CRs are detected, except in a 100x100 region instead of a 4kx4k region;
     # i.e., there are 1600x too many CRs.  Fine for unit tests?
     rng = galsim.BaseDeviate(1)
     l1 = image.simulate(meta, graycat, webbpsf=True, level=1,
-                        crparam=dict(), usecrds=False, rng=rng)
+                        crparam=dict(), usecrds=False, rng=rng,
+                        psf_keywords=dict(nlambda=1))
     peakloc = np.nonzero(l0[0]['data'] == np.max(l0[0]['data']))
 
     # check that the location with the most flux is the location where the
     # source was simulated to be, using a real WCS with distortion.
     assert (peakloc[0][0] == sourcecen[0]) and (peakloc[1][0] == sourcecen[1])
     log.info('DMS218: successfully used WCS / focal plane geometry to render '
              'sources at correct locations with distortions.')
@@ -524,29 +529,32 @@
         af.tree = {'image': l0[0]['data'],
                    'imloc': peakloc,
                    'trueloc': sourcecen}
         af.write_to(os.path.join(artifactdir, 'dms218.asdf'))
 
     rng = galsim.BaseDeviate(1)
     l1_nocr = image.simulate(meta, graycat, webbpsf=True, level=1,
-                             usecrds=False, crparam=None, rng=rng)
+                             usecrds=False, crparam=None, rng=rng,
+                             psf_keywords=dict(nlambda=1))
     assert np.all(l1[0].data >= l1_nocr[0].data)
     log.info('DMS221: Successfully added cosmic rays to an L1 image.')
     l2 = image.simulate(meta, graycat, webbpsf=True, level=2,
-                        usecrds=False, crparam=dict())
+                        usecrds=False, crparam=dict(),
+                        psf_keywords=dict(nlambda=1))
     # throw in some CRs for fun
     l2c = image.simulate(meta, chromcat, webbpsf=False, level=2,
                          usecrds=False)
     persist = persistence.Persistence()
     fluence = 30000
     persist.update(l0[0]['data'] * 0 + fluence, time.mjd - 100 / 60 / 60 / 24)
     # zap the whole frame, 100 seconds ago.
     rng = galsim.BaseDeviate(1)
     l1p = image.simulate(meta, graycat, webbpsf=True, level=1, usecrds=False,
-                         persistence=persist, crparam=None, rng=rng)
+                         persistence=persist, crparam=None, rng=rng,
+                         psf_keywords=dict(nlambda=1))
     # the random number gets instatiated from the same seed, but the order in
     # which the numbers are generated is different so we can't guarantee, e.g.,
     # that all of the new values are strictly greater than the old ones.
     # But we've basically added a constant to the whole scene: we can at least
     # verify it's positive.
     diff = l1p[0]['data'][-1] * 1.0 - l1_nocr[0]['data'][-1] * 1.0
     # L1 files are unsigned, so the difference gets wonky unless you convert
@@ -625,15 +633,15 @@
     cat = catalog.make_dummy_table_catalog(
         rd_sca, bandpasses=[metadata['instrument']['optical_element']], nobj=1000)
 
     rng = galsim.UniformDeviate(None)
     im, simcatobj = image.simulate(
         metadata, cat, usecrds=True,
         webbpsf=True, level=level,
-        rng=rng)
+        rng=rng, psf_keywords=dict(nlambda=1))
 
     # Confirm that CRDS keyword was updated
     assert im.meta.ref_file.crds.sw_version != '12.3.1'
 
     if (level == 1):
         assert (type(im) is WfiScienceRaw)
     else:
```

### Comparing `romanisim-0.5.0/romanisim/tests/test_l1.py` & `romanisim-0.5.1/romanisim/tests/test_l1.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/tests/test_linear.py` & `romanisim-0.5.1/romanisim/tests/test_linear.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/tests/test_persistence.py` & `romanisim-0.5.1/romanisim/tests/test_persistence.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/tests/test_psf.py` & `romanisim-0.5.1/romanisim/tests/test_psf.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,25 +18,29 @@
 
     def local(self, *args, **kwargs):
         return galsim.JacobianWCS(0.1, 0, 0, 0.1)
 
 
 def test_make_psf():
     psfs = []
-    psfs.append(psf.make_psf(1, 'F087'))
-    psfs.append(psf.make_psf(2, 'F184', chromatic=False))
+    pkw = dict(nlambda=1)
+    psfs.append(psf.make_psf(1, 'F087', **pkw))
+    psfs.append(psf.make_psf(2, 'F184', chromatic=False, **pkw))
     psfs.append(psf.make_psf(3, 'F184', webbpsf=False))
     psfs.append(psf.make_psf(4, 'H158', webbpsf=False, chromatic=True))
     psfs.append(psf.make_psf(5, 'F184', pix=(1000, 1000), webbpsf=False))
-    psfs.append(psf.make_psf(6, 'F184', pix=(1000, 1000), webbpsf=True))
-    psfs.append(psf.make_psf(7, 'F129', wcs=FakeWCS()))
+    psfs.append(psf.make_psf(6, 'F184', pix=(1000, 1000), webbpsf=True,
+                             **pkw))
+    psfs.append(psf.make_psf(7, 'F129', wcs=FakeWCS(), **pkw))
     chromatic = [False] * 7
     chromatic[3] = True
     bandpass = galsim.roman.getBandpasses(AB_zeropoint=True)['H158']
     vega_sed = galsim.SED('vega.txt', 'nm', 'flambda')
+    varpsf = psf.make_psf(8, 'F087', webbpsf=True, variable=True, **pkw)
+    psfs.append(varpsf.at_position(100, 100))
     for p, c in zip(psfs, chromatic):
         if not c:
             im = p.drawImage().array
         else:
             im = (p * vega_sed.withFlux(1, bandpass)).drawImage(bandpass).array
         totsum = np.sum(im)
         assert totsum < 1
```

### Comparing `romanisim-0.5.0/romanisim/tests/test_ramp.py` & `romanisim-0.5.1/romanisim/tests/test_ramp.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/tests/test_ris_make_utils.py` & `romanisim-0.5.1/romanisim/tests/test_ris_make_utils.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/tests/test_util.py` & `romanisim-0.5.1/romanisim/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/tests/test_wcs.py` & `romanisim-0.5.1/romanisim/tests/test_wcs.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/romanisim/util.py` & `romanisim-0.5.1/romanisim/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -211,14 +211,48 @@
     metadata['exposure']['frame_time'] = parameters.read_time
     metadata['exposure']['exposure_time'] = openshuttertime
     metadata['exposure']['effective_exposure_time'] = openshuttertime
     metadata['exposure']['duration'] = openshuttertime
     metadata['exposure']['read_pattern'] = read_pattern
     # integration_start?  integration_end?  nints = 1?  ...
 
+    if 'target' not in metadata.keys():
+        metadata['target'] = {}
+    target = metadata['target']
+    target['type'] = 'FIXED'
+    if 'wcsinfo' in metadata.keys():
+        target['ra'] = metadata['wcsinfo']['ra_ref']
+        target['dec'] = metadata['wcsinfo']['dec_ref']
+        target['proposer_ra'] = target['ra']
+        target['proposer_dec'] = target['dec']
+    target['ra_uncertainty'] = 0
+    target['dec_uncertainty'] = 0
+    target['proper_motion_ra'] = 0
+    target['proper_motion_dec'] = 0
+    target['proper_motion_epoch'] = 'J2000'
+    target['source_type'] = 'EXTENDED'
+
+    # there are a few metadata keywords that have problematic, too-long
+    # defaults in RDM.
+    # program.category
+    # ephemeris.ephemeris_reference_frame
+    # guidestar.gs_epoch
+    # this truncates these to the maximum allowed characters.  Alternative
+    # solutions would include doing things like:
+    #   making the roman_datamodels defaults archivable
+    #   making the roman_datamodels validation check lengths of strings
+    if 'program' in metadata:
+        metadata['program']['category'] = metadata['program']['category'][:6]
+    if 'ephemeris' in metadata:
+        metadata['ephemeris']['ephemeris_reference_frame'] = (
+            metadata['ephemeris']['ephemeris_reference_frame'][:10])
+    if 'guidestar' in metadata:
+        metadata['guidestar']['gs_epoch'] = (
+            metadata['guidestar']['gs_epoch'][:10])
+
 
 def king_profile(r, rc, rt):
     """Compute the King (1962) profile.
 
     Parameters
     ----------
     r : np.ndarray[float]
```

### Comparing `romanisim-0.5.0/romanisim/wcs.py` & `romanisim-0.5.1/romanisim/wcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,15 +89,14 @@
         parameters['wcsinfo']['v2_ref'] = v2v3_wficen[0]
         parameters['wcsinfo']['v3_ref'] = v2v3_wficen[1]
         parameters['aperture']['name'] = 'WFI_CEN'
 
     parameters['aperture']['position_angle'] = pa_aper
 
 
-        
 def get_wcs(image, usecrds=True, distortion=None):
     """Get a WCS object for a given sca or set of CRDS parameters.
 
     Parameters
     ----------
     image : roman_datamodels.datamodels.ImageModel or dict
         Image model or dictionary containing CRDS parameters
@@ -278,15 +277,16 @@
     def _xy(self, ra, dec, color=None):
         # _xy accepts ra/dec in radians; we decorate r1, d1 appropriately.
         r1 = np.atleast_1d(ra) * u.rad
         d1 = np.atleast_1d(dec) * u.rad
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
-            x, y = self.wcs.world_to_pixel(r1, d1)
+            # x, y = self.wcs.world_to_pixel(r1, d1)
+            x, y = self.wcs.numerical_inverse(r1, d1)
 
         if np.ndim(ra) == np.ndim(dec) == 0:
             return x[0], y[0]
         else:
             if (np.ndim(ra) != np.ndim(dec)):
                 raise ValueError(
                     f"np.ndim(ra) != np.ndim(dec) => "
@@ -381,7 +381,26 @@
         unit=(u.deg, u.deg)
     )
     pipeline = [(detector_frame, det2sky), (sky_frame, None)]
     gw = gwcs.WCS(pipeline)
     gw.bounding_box = ((-0.5, nx - 0.5), (-0.5, ny - 0.5))
 
     return gw
+
+
+def convert_wcs_to_gwcs(wcs):
+    """Convert a GalSim WCS object into a GWCS object.
+
+    Parameters
+    ----------
+    wcs : gwcs.wcs.WCS or wcs.GWCS
+        input WCS to convert
+
+    Returns
+    -------
+    wcs.GWCS corresponding to wcs.
+    """
+    if isinstance(wcs, GWCS):
+        return wcs.wcs
+    else:
+        # make a gwcs WCS from a galsim.roman WCS
+        return wcs_from_fits_header(wcs.header.header)
```

### Comparing `romanisim-0.5.0/romanisim.egg-info/PKG-INFO` & `romanisim-0.5.1/romanisim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romanisim
-Version: 0.5.0
+Version: 0.5.1
 Summary: Nancy Grace Roman Space Telescope WFI Simulator
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2022 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -38,43 +38,43 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asdf>=2.15.1
 Requires-Dist: astropy>=5.3
-Requires-Dist: crds>=10.3.1
+Requires-Dist: crds>=11.16.16
 Requires-Dist: defusedxml>=0.5.0
-Requires-Dist: galsim>=2.5.0
-Requires-Dist: rad>=0.18.0
-Requires-Dist: roman_datamodels>=0.18.0
+Requires-Dist: galsim>=2.5.1
+Requires-Dist: rad>=0.19.2
+Requires-Dist: roman_datamodels>=0.19.1
 Requires-Dist: gwcs>=0.18.1
 Requires-Dist: jsonschema>=4.8
 Requires-Dist: numpy>=1.22
-Requires-Dist: webbpsf>=1.0.0
+Requires-Dist: webbpsf>=1.2.1
 Requires-Dist: Cython>=0.29.21
 Provides-Extra: docs
 Requires-Dist: sphinx<7; extra == "docs"
 Requires-Dist: sphinx-automodapi; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: stsci-rtd-theme; extra == "docs"
 Requires-Dist: sphinx-astropy; extra == "docs"
 Requires-Dist: sphinx-asdf>=0.1.1; extra == "docs"
 Requires-Dist: tomli; python_version < "3.11" and extra == "docs"
 Provides-Extra: test
 Requires-Dist: ci-watson>=0.3.0; extra == "test"
 Requires-Dist: colorama>=0.4.1; extra == "test"
 Requires-Dist: getch>=1.0.0; extra == "test"
-Requires-Dist: pytest>=4.6.0; extra == "test"
+Requires-Dist: pytest<=8.0,>=4.6.0; extra == "test"
 Requires-Dist: pytest-openfiles>=0.5.0; extra == "test"
 Requires-Dist: pytest-doctestplus>=0.10.0; extra == "test"
 Requires-Dist: pytest-cov>=2.9.0; extra == "test"
 Requires-Dist: flake8>=3.6.0; extra == "test"
 Requires-Dist: metrics_logger>=0.1.0; extra == "test"
 
 [![CI](https://github.com/spacetelescope/romanisim/actions/workflows/ci.yml/badge.svg)](https://github.com/spacetelescope/romanisim/actions/workflows/ci.yml) [![codecov](https://codecov.io/gh/spacetelescope/romanisim/branch/main/graph/badge.svg?token=pkoLtQOa2v)](https://codecov.io/gh/spacetelescope/romanisim)
```

### Comparing `romanisim-0.5.0/romanisim.egg-info/SOURCES.txt` & `romanisim-0.5.1/romanisim.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 romanisim.egg-info/PKG-INFO
 romanisim.egg-info/SOURCES.txt
 romanisim.egg-info/dependency_links.txt
 romanisim.egg-info/not-zip-safe
 romanisim.egg-info/requires.txt
 romanisim.egg-info/top_level.txt
 romanisim/data/Roman_effarea_20201130.csv
+romanisim/data/gaia-270-66-2027-06-01.ecsv
 romanisim/regtest/__init__.py
 romanisim/regtest/test_l1.py
 romanisim/tests/__init__.py
 romanisim/tests/test_bandpass.py
 romanisim/tests/test_catalog.py
 romanisim/tests/test_cr.py
 romanisim/tests/test_gaia.py
@@ -69,9 +70,12 @@
 romanisim/tests/test_linear.py
 romanisim/tests/test_persistence.py
 romanisim/tests/test_psf.py
 romanisim/tests/test_ramp.py
 romanisim/tests/test_ris_make_utils.py
 romanisim/tests/test_util.py
 romanisim/tests/test_wcs.py
+scripts/romancal_make_all_l1s.sh
+scripts/romancal_make_regtest_l1s.sh
+scripts/romanisim-make-catalog
 scripts/romanisim-make-image
 scripts/romanisim-make-stack
```

### Comparing `romanisim-0.5.0/scripts/romanisim-make-image` & `romanisim-0.5.1/scripts/romanisim-make-image`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,68 @@
 import yaml
 
 from astropy.coordinates import SkyCoord
 from astropy import units as u
 import galsim
 from romanisim import log, wcs, persistence, parameters
 from romanisim import ris_make_utils as ris
+from copy import copy
+
+
+def go(args):
+    if args.config is not None:
+        # Open and parse overrides file
+        with open(args.config, "r") as config_file:
+            config = yaml.safe_load(config_file)
+            combo_dict = parameters.__dict__
+            ris.merge_nested_dicts(combo_dict, config)
+            parameters.__dict__.update(combo_dict)
+    elif args.usecrds:
+        # don't use default values
+        for k in parameters.reference_data:
+            parameters.reference_data[k] = None
+
+    if args.sca == -1:
+        # simulate all 18 SCAs sequentially
+        origfilename = copy(args.filename)
+        origprevious = copy(args.previous)
+        for i in range(1, 19):
+            args.sca = i
+            args.filename = origfilename.format(f'WFI{args.sca:02d}')
+            if origprevious is not None:
+                args.previous = origprevious.format(f'WFI{args.sca:02d}')
+            go(args)
+        return
+
+    metadata = ris.set_metadata(
+        date=args.date, bandpass=args.bandpass,
+        sca=args.sca, ma_table_number=args.ma_table_number,
+        truncate=args.truncate)
+
+    if args.radec is not None:
+        coord = SkyCoord(ra=args.radec[0] * u.deg, dec=args.radec[1] * u.deg,
+                         frame='icrs')
+        wcs.fill_in_parameters(metadata, coord, boresight=args.boresight, pa_aper=args.roll)
+
+    rng = galsim.UniformDeviate(args.rng_seed)
+
+    # Create catalog
+    cat = ris.create_catalog(metadata=metadata, catalog_name=args.catalog,
+                             bandpasses=[args.bandpass], rng=rng,
+                             nobj=args.nobj, usecrds=args.usecrds)
+
+    # Create persistence object
+    if args.previous is not None:
+        persist = persistence.Persistence.read(args.previous)
+    else:
+        persist = persistence.Persistence()
+
+    # Simulate image and write to file
+    ris.simulate_image_file(args, metadata, cat, rng, persist)
+
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(
         description='Make a demo image.',
         epilog='EXAMPLE: %(prog)s output_image.asdf',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument('filename', type=str, help='output image (asdf)')
@@ -41,55 +95,24 @@
     parser.add_argument('--sca', type=int, default=7, help='SCA to simulate')
     parser.add_argument('--usecrds', action='store_true',
                         help='Use CRDS for distortion map')
     parser.add_argument('--webbpsf', action='store_true',
                         help='Use webbpsf for PSF')
     parser.add_argument('--truncate', type=int, default=None, help=(
         'If set, truncate the MA table at given number of resultants.'))
+    parser.add_argument('--pretend-spectral', type=str, default=None, help=(
+        'Pretend the image is spectral.  exposure.type and instrument.element '
+        'are updated to be grism / prism.'))
+    parser.add_argument('--drop-extra-dq', default=False, action='store_true',
+                        help=('Do not store the optional simulated dq array.'))
 
     args = parser.parse_args()
 
     log.info('Starting simulation...')
     log.warning("romanisim is under active development.  Its output has "
                 "not been formally validated; only limited testing has been "
                 "performed.  For this reason, use of romanisim for "
                 "preparation of ROSES proposals is not advised.  Other "
                 "packages like galsim's roman package or STIPS may better "
                 "serve such purposes.")
 
-    if args.config is not None:
-        # Open and parse overrides file
-        with open(args.config, "r") as config_file:
-            config = yaml.safe_load(config_file)
-            combo_dict = parameters.__dict__ 
-            ris.merge_nested_dicts(combo_dict, config)
-            parameters.__dict__.update(combo_dict)
-    elif args.usecrds:
-        # don't use default values
-        for k in parameters.reference_data:
-            parameters.reference_data[k] = None
-
-    metadata = ris.set_metadata(
-        date=args.date, bandpass=args.bandpass,
-        sca=args.sca, ma_table_number=args.ma_table_number,
-        truncate=args.truncate)
-    
-    if args.radec is not None:
-        coord = SkyCoord(ra=args.radec[0] * u.deg, dec=args.radec[1] * u.deg,
-                         frame='icrs')
-        wcs.fill_in_parameters(metadata, coord, boresight=args.boresight, pa_aper=args.roll)
-
-    rng = galsim.UniformDeviate(args.rng_seed)
-
-    # Create catalog
-    cat = ris.create_catalog(metadata=metadata, catalog_name=args.catalog,
-                             bandpasses=[args.bandpass], rng=rng,
-                             nobj=args.nobj, usecrds=args.usecrds)
-
-    # Create persistence object
-    if args.previous is not None:
-        persist = persistence.Persistence.read(args.previous)
-    else:
-        persist = persistence.Persistence()
-
-    # Simulate image and write to file
-    ris.simulate_image_file(args, metadata, cat, rng, persist)
+    go(args)
```

### Comparing `romanisim-0.5.0/scripts/romanisim-make-stack` & `romanisim-0.5.1/scripts/romanisim-make-stack`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from copy import deepcopy
 import yaml
 from astropy.coordinates import SkyCoord
 from astropy import units as u
 from astropy.table import Table
 from astropy.time import Time
 import galsim
-from romanisim import wcs, persistence, log, parameters
+from romanisim import wcs, persistence, log, parameters, apt
 from romanisim.parameters import default_parameters_dictionary
 from romanisim import ris_make_utils as ris
 
 
 def main():
     parser = argparse.ArgumentParser(
         description='Make a stack of demo images.',
@@ -21,21 +21,27 @@
 
     # Command line Argument - pointing file input
     parser.add_argument('pointing_file_name',
                         type=str,
                         metavar='mosaic_list.csv',
                         help='Input (csv) file containing lists of observation parameters: '
                              'ra, dec, roll_angle, optical_element, date, overhead_time, '
-                             'ms_table_number')
+                             'ma_table_number')
 
     # WCS Object Catalog
     parser.add_argument('cat_file_name',
                         type=str,
                         metavar='object_table.csv',
                         help='Object catalog file for wcs matching (csv)')
+    
+    # Create script making argument
+    parser.add_argument('-a', "--apt",
+                        type=str,
+                        metavar='small_dither_program.apt',
+                        help='APT file for metadata.')
 
     # Boresight
     parser.add_argument('-b', '--boresight',
                         action='store_true',
                         help=('RA & Dec specifies location of boresight, not center of WFI.'))
     
     # Use config file to override metadata or values in default parameters file
@@ -60,15 +66,14 @@
     parser.add_argument('-m', "--make_script",
                         type=str,
                         metavar='sims',
                         default=None,
                         help='Filename to output list of romanisim calls (sims.script) instead of '
                              'making simulation files (e.g. for cluster usage).')
     
-
     # Create script making argument
     parser.add_argument('-x', "--prefix",
                         type=str,
                         metavar='roman_simulated',
                         default='roman_simulated',
                         help='Filename prefix for simulated files.')
 
@@ -150,43 +155,50 @@
     # Set file name suffix
     suffix = "uncal" if (args.level == 1) else "cal"
 
     # If selected, reset persistence dictionary
     if args.persistence:
         previous_file_name = {}
 
-    # Obtain pointing information from input file
+    # Open csv table pointing file    
     pointings = Table.read(args.pointing_file_name, comment="#", delimiter=" ")
 
+    if args.apt:
+        apt_idx = 0
+        apt_prefix = ris.parse_apt_file(args.apt, len(pointings))
+
     # Loop over pointings
     for entry_idx, entry in enumerate(pointings):
 
         # Debug: print keys
         log.debug(f'entry.keys = {entry.keys()}')
 
         # Set initial (possibly only) SCA
         sca = args.sca if (args.sca > 0) else 1
 
         # If SCA value is within 1-18, only run once
         # otherwise loop over all detectors
         while (sca <= parameters.NUMBER_OF_DETECTORS):
             # Create output file name
-            output_file_name = f"{args.prefix}_{entry_idx}_{entry['BANDPASS']}_WFI{sca:02}_{suffix}.asdf"
+            if args.apt:
+                output_file_name = f"{apt_prefix[apt_idx]}_WFI{sca:02}_{suffix}.asdf"
+            else:
+                output_file_name = f"{args.prefix}_{entry_idx}_{entry['BANDPASS']}_WFI{sca:02}_{suffix}.asdf"
 
             log.debug(f"output_file_name = {output_file_name}")
 
             # If making a script, write the line and proceed
             # otherwise create simulation file
             if args.make_script:
                 line = f"romanisim-make-image {output_file_name}"
 
                 # Preserve relevant stack options for image lines
                 for option, value in options_dct.items():
                     if (type(value) != bool) and (option != 'sca') and (option != 'prefix') \
-                            and (option != 'cat_file_name'):
+                            and (option != 'cat_file_name') and (option != 'apt'):
                         line += f" --{option} {value}"
                     elif (option == 'sca'):
                         line += f" --{option} {sca}"
                     elif (value is True):
                         if (option != 'persistence'):
                             line += f" --{option}"
                         elif (sca in previous_file_name.keys()):
@@ -238,14 +250,16 @@
 
             # Break the loop if only one detector specified
             if args.sca > 0:
                 break
             else:
                 sca += 1
 
+        apt_idx += 1
+
         # Add time offset for the next exposure group
         time_offset += (float(entry['DURATION'])) * u.s
 
     # Close script file if appropriate
     if args.make_script:
         script_file.close()
```

### Comparing `romanisim-0.5.0/setup.py` & `romanisim-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.0/tox.ini` & `romanisim-0.5.1/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,16 @@
     CI
     TOXENV
     CRDS_*
     TEST_BIGDATA
     CODECOV_*
     WEBBPSF_PATH
     GALSIM_CAT_PATH
+    FFTW_DIR
+    LIBRARY_PATH
 extras =
     test
 deps =
     xdist: pytest-xdist
     oldestdeps: minimum_dependencies
 commands_pre =
     oldestdeps: minimum_dependencies romanisim --filename requirements-min.txt
```


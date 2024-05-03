# Comparing `tmp/ccdproc-2.4.1.tar.gz` & `tmp/ccdproc-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdproc-2.4.1.tar", last modified: Tue May 30 15:58:27 2023, max compression
+gzip compressed data, was "ccdproc-2.4.2.tar", last modified: Fri May  3 15:37:24 2024, max compression
```

## Comparing `ccdproc-2.4.1.tar` & `ccdproc-2.4.2.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.824422 ccdproc-2.4.1/
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.803008 ccdproc-2.4.1/.github/
--rw-r--r--   0 mattcraig   (501) staff       (20)      197 2021-03-19 20:06:38.000000 ccdproc-2.4.1/.github/CONTRIBUTING.md
--rw-r--r--   0 mattcraig   (501) staff       (20)      699 2018-08-14 01:14:56.000000 ccdproc-2.4.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 mattcraig   (501) staff       (20)     1217 2018-08-14 01:14:56.000000 ccdproc-2.4.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.803150 ccdproc-2.4.1/.github/workflows/
--rw-r--r--   0 mattcraig   (501) staff       (20)     3302 2021-12-14 21:17:21.000000 ccdproc-2.4.1/.github/workflows/ci_tests.yml
--rw-r--r--   0 mattcraig   (501) staff       (20)      771 2021-03-19 20:06:25.000000 ccdproc-2.4.1/.gitignore
--rw-r--r--   0 mattcraig   (501) staff       (20)        0 2019-12-24 20:04:16.000000 ccdproc-2.4.1/.gitmodules
--rw-r--r--   0 mattcraig   (501) staff       (20)     1134 2019-09-02 21:23:23.000000 ccdproc-2.4.1/.mailmap
--rw-r--r--   0 mattcraig   (501) staff       (20)      143 2021-11-24 18:20:46.000000 ccdproc-2.4.1/.readthedocs.yml
--rw-r--r--   0 mattcraig   (501) staff       (20)     2507 2023-05-30 15:52:39.000000 ccdproc-2.4.1/AUTHORS.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)    16811 2023-05-30 15:54:14.000000 ccdproc-2.4.1/CHANGES.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)     1822 2019-09-02 17:30:31.000000 ccdproc-2.4.1/CITATION.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)      180 2019-09-02 17:30:31.000000 ccdproc-2.4.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)     1503 2018-08-18 01:06:53.000000 ccdproc-2.4.1/LICENSE.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)      382 2020-11-28 20:18:08.000000 ccdproc-2.4.1/MANIFEST.in
--rw-r--r--   0 mattcraig   (501) staff       (20)      422 2023-05-30 15:58:27.824508 ccdproc-2.4.1/PKG-INFO
--rw-r--r--   0 mattcraig   (501) staff       (20)     3785 2021-03-19 20:06:38.000000 ccdproc-2.4.1/README.rst
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.806380 ccdproc-2.4.1/ccdproc/
--rw-r--r--   0 mattcraig   (501) staff       (20)     1124 2021-05-19 00:45:02.000000 ccdproc-2.4.1/ccdproc/__init__.py
--rw-r--r--   0 mattcraig   (501) staff       (20)      355 2021-05-19 00:45:02.000000 ccdproc-2.4.1/ccdproc/_astropy_init.py
--rw-r--r--   0 mattcraig   (501) staff       (20)      408 2018-08-18 01:06:53.000000 ccdproc-2.4.1/ccdproc/ccddata.py
--rw-r--r--   0 mattcraig   (501) staff       (20)    38231 2022-11-17 14:20:04.000000 ccdproc-2.4.1/ccdproc/combiner.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     1216 2022-01-19 16:10:46.000000 ccdproc-2.4.1/ccdproc/conftest.py
--rw-r--r--   0 mattcraig   (501) staff       (20)    76092 2022-06-01 13:16:23.000000 ccdproc-2.4.1/ccdproc/core.py
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.807448 ccdproc-2.4.1/ccdproc/extern/
--rw-r--r--   0 mattcraig   (501) staff       (20)       64 2018-08-18 01:06:53.000000 ccdproc-2.4.1/ccdproc/extern/__init__.py
--rw-r--r--   0 mattcraig   (501) staff       (20)    19025 2021-12-20 17:15:43.000000 ccdproc-2.4.1/ccdproc/extern/bitfield.py
--rw-r--r--   0 mattcraig   (501) staff       (20)    37438 2023-05-30 15:52:41.000000 ccdproc-2.4.1/ccdproc/image_collection.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     5533 2021-03-19 20:06:38.000000 ccdproc-2.4.1/ccdproc/log_meta.py
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.813213 ccdproc-2.4.1/ccdproc/tests/
--rw-r--r--   0 mattcraig   (501) staff       (20)      121 2018-08-14 01:14:56.000000 ccdproc-2.4.1/ccdproc/tests/__init__.py
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.815645 ccdproc-2.4.1/ccdproc/tests/data/
--rw-r--r--   0 mattcraig   (501) staff       (20)      257 2018-08-14 01:14:56.000000 ccdproc-2.4.1/ccdproc/tests/data/README.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)   561600 2021-12-21 15:57:22.000000 ccdproc-2.4.1/ccdproc/tests/data/a8280271.fits
--rw-r--r--   0 mattcraig   (501) staff       (20)      459 2019-09-02 17:30:31.000000 ccdproc-2.4.1/ccdproc/tests/data/expected_ifc_file_properties.csv
--rw-r--r--   0 mattcraig   (501) staff       (20)    20160 2019-09-02 17:30:31.000000 ccdproc-2.4.1/ccdproc/tests/data/flat-mef.fits
--rw-r--r--   0 mattcraig   (501) staff       (20)    20160 2019-09-02 17:30:31.000000 ccdproc-2.4.1/ccdproc/tests/data/science-mef.fits
--rw-r--r--   0 mattcraig   (501) staff       (20)    23040 2021-12-21 15:57:17.000000 ccdproc-2.4.1/ccdproc/tests/data/sip-wcs.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)     2156 2019-09-02 17:30:31.000000 ccdproc-2.4.1/ccdproc/tests/make_mef.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     2297 2022-01-19 16:10:46.000000 ccdproc-2.4.1/ccdproc/tests/pytest_fixtures.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     7044 2022-01-19 16:10:46.000000 ccdproc-2.4.1/ccdproc/tests/run_for_memory_profile.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     7763 2019-09-02 17:30:31.000000 ccdproc-2.4.1/ccdproc/tests/run_profile.ipynb
--rw-r--r--   0 mattcraig   (501) staff       (20)     9314 2021-03-15 15:22:51.000000 ccdproc-2.4.1/ccdproc/tests/run_with_file_number_limit.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     2253 2022-01-19 16:10:46.000000 ccdproc-2.4.1/ccdproc/tests/test_bitfield.py
--rw-r--r--   0 mattcraig   (501) staff       (20)    10893 2021-03-19 20:06:38.000000 ccdproc-2.4.1/ccdproc/tests/test_ccdmask.py
--rw-r--r--   0 mattcraig   (501) staff       (20)    42879 2022-01-19 16:10:46.000000 ccdproc-2.4.1/ccdproc/tests/test_ccdproc.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     4202 2021-03-19 20:06:38.000000 ccdproc-2.4.1/ccdproc/tests/test_ccdproc_logging.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     2109 2019-03-08 20:32:20.000000 ccdproc-2.4.1/ccdproc/tests/test_combine_open_files.py
--rw-r--r--   0 mattcraig   (501) staff       (20)    35523 2022-11-17 14:20:04.000000 ccdproc-2.4.1/ccdproc/tests/test_combiner.py
--rw-r--r--   0 mattcraig   (501) staff       (20)    15231 2021-12-21 15:57:22.000000 ccdproc-2.4.1/ccdproc/tests/test_cosmicray.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     2132 2021-03-15 15:22:51.000000 ccdproc-2.4.1/ccdproc/tests/test_gain.py
--rw-r--r--   0 mattcraig   (501) staff       (20)    47273 2023-05-30 15:52:41.000000 ccdproc-2.4.1/ccdproc/tests/test_image_collection.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     2170 2021-03-15 15:22:51.000000 ccdproc-2.4.1/ccdproc/tests/test_keyword.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     2731 2021-11-19 14:38:28.000000 ccdproc-2.4.1/ccdproc/tests/test_memory_use.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     2481 2022-01-19 16:10:46.000000 ccdproc-2.4.1/ccdproc/tests/test_rebin.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     2581 2021-03-15 15:22:51.000000 ccdproc-2.4.1/ccdproc/tests/test_wrapped_external_funcs.py
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.816153 ccdproc-2.4.1/ccdproc/utils/
--rw-r--r--   0 mattcraig   (501) staff       (20)      199 2018-08-14 01:14:56.000000 ccdproc-2.4.1/ccdproc/utils/__init__.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     2932 2019-09-06 01:45:09.000000 ccdproc-2.4.1/ccdproc/utils/sample_directory.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     4170 2018-08-18 01:06:53.000000 ccdproc-2.4.1/ccdproc/utils/slices.py
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.816503 ccdproc-2.4.1/ccdproc/utils/tests/
--rw-r--r--   0 mattcraig   (501) staff       (20)        0 2018-08-14 01:14:56.000000 ccdproc-2.4.1/ccdproc/utils/tests/__init__.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     4340 2018-08-18 01:06:53.000000 ccdproc-2.4.1/ccdproc/utils/tests/test_slices.py
--rw-r--r--   0 mattcraig   (501) staff       (20)      160 2023-05-30 15:58:27.000000 ccdproc-2.4.1/ccdproc/version.py
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.807157 ccdproc-2.4.1/ccdproc.egg-info/
--rw-r--r--   0 mattcraig   (501) staff       (20)      422 2023-05-30 15:58:27.000000 ccdproc-2.4.1/ccdproc.egg-info/PKG-INFO
--rw-r--r--   0 mattcraig   (501) staff       (20)     2513 2023-05-30 15:58:27.000000 ccdproc-2.4.1/ccdproc.egg-info/SOURCES.txt
--rw-r--r--   0 mattcraig   (501) staff       (20)        1 2023-05-30 15:58:27.000000 ccdproc-2.4.1/ccdproc.egg-info/dependency_links.txt
--rw-r--r--   0 mattcraig   (501) staff       (20)        1 2023-05-30 15:58:27.000000 ccdproc-2.4.1/ccdproc.egg-info/not-zip-safe
--rw-r--r--   0 mattcraig   (501) staff       (20)      162 2023-05-30 15:58:27.000000 ccdproc-2.4.1/ccdproc.egg-info/requires.txt
--rw-r--r--   0 mattcraig   (501) staff       (20)        8 2023-05-30 15:58:27.000000 ccdproc-2.4.1/ccdproc.egg-info/top_level.txt
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.820423 ccdproc-2.4.1/docs/
--rw-r--r--   0 mattcraig   (501) staff       (20)     4724 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/Makefile
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.822755 ccdproc-2.4.1/docs/_static/
--rw-r--r--   0 mattcraig   (501) staff       (20)   370070 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/_static/ccd_proc.ico
--rwxr-xr-x   0 mattcraig   (501) staff       (20)     6867 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/_static/ccd_proc.png
--rw-r--r--   0 mattcraig   (501) staff       (20)      208 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/_static/ccdproc.css
--rwxr-xr-x   0 mattcraig   (501) staff       (20)    51513 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/_static/ccdproc.svg
--rw-r--r--   0 mattcraig   (501) staff       (20)     9342 2019-09-02 17:30:31.000000 ccdproc-2.4.1/docs/_static/ccdproc_banner.pdf
--rw-r--r--   0 mattcraig   (501) staff       (20)    95067 2019-09-02 17:30:31.000000 ccdproc-2.4.1/docs/_static/ccdproc_banner.png
--rwxr-xr-x   0 mattcraig   (501) staff       (20)   222655 2019-12-24 20:04:16.000000 ccdproc-2.4.1/docs/_static/ccdproc_banner.svg
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.799877 ccdproc-2.4.1/docs/_templates/
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.823881 ccdproc-2.4.1/docs/_templates/autosummary/
--rw-r--r--   0 mattcraig   (501) staff       (20)      250 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)      251 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)      252 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/_templates/autosummary/module.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)      222 2019-09-02 17:30:31.000000 ccdproc-2.4.1/docs/api.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)       55 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/authors_for_sphinx.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)     7425 2019-09-02 17:30:31.000000 ccdproc-2.4.1/docs/ccddata.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)       90 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/changelog.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)       52 2019-09-02 17:30:31.000000 ccdproc-2.4.1/docs/citation.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)       54 2019-09-02 17:30:31.000000 ccdproc-2.4.1/docs/conduct.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)     6951 2021-12-21 15:57:22.000000 ccdproc-2.4.1/docs/conf.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     1599 2019-09-02 17:30:31.000000 ccdproc-2.4.1/docs/contributing.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)      280 2021-05-19 00:45:02.000000 ccdproc-2.4.1/docs/default_config.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)     3839 2019-09-02 17:30:31.000000 ccdproc-2.4.1/docs/getting_started.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)     9815 2021-12-21 15:57:22.000000 ccdproc-2.4.1/docs/image_combination.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)     8376 2021-12-21 15:57:22.000000 ccdproc-2.4.1/docs/image_management.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)     1637 2021-05-19 00:45:02.000000 ccdproc-2.4.1/docs/index.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)     1845 2021-03-19 20:06:38.000000 ccdproc-2.4.1/docs/install.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)      157 2019-03-08 17:03:24.000000 ccdproc-2.4.1/docs/license.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)     4513 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/make.bat
--rw-r--r--   0 mattcraig   (501) staff       (20)      892 2019-09-02 17:30:31.000000 ccdproc-2.4.1/docs/overview.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)      883 2019-09-02 17:30:31.000000 ccdproc-2.4.1/docs/reduction_examples.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)    21228 2019-12-24 20:04:16.000000 ccdproc-2.4.1/docs/reduction_toolbox.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)       67 2019-03-30 16:56:12.000000 ccdproc-2.4.1/docs/rtd-pip-requirements
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.824248 ccdproc-2.4.1/licenses/
--rw-r--r--   0 mattcraig   (501) staff       (20)     1463 2018-08-18 01:06:53.000000 ccdproc-2.4.1/licenses/LICENSE_STSCI_TOOLS.txt
--rw-r--r--   0 mattcraig   (501) staff       (20)      251 2018-08-18 01:06:53.000000 ccdproc-2.4.1/licenses/README.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)      132 2019-12-24 20:04:16.000000 ccdproc-2.4.1/pyproject.toml
--rw-r--r--   0 mattcraig   (501) staff       (20)     1890 2023-05-30 15:58:27.824947 ccdproc-2.4.1/setup.cfg
--rwxr-xr-x   0 mattcraig   (501) staff       (20)     1609 2019-12-24 20:04:16.000000 ccdproc-2.4.1/setup.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     2665 2023-05-30 15:52:39.000000 ccdproc-2.4.1/tox.ini
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2024-05-03 15:37:24.681443 ccdproc-2.4.2/
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2024-05-03 15:37:24.666717 ccdproc-2.4.2/.github/
+-rw-r--r--   0 mattcraig   (501) staff       (20)      197 2021-03-19 20:06:38.000000 ccdproc-2.4.2/.github/CONTRIBUTING.md
+-rw-r--r--   0 mattcraig   (501) staff       (20)      699 2018-08-14 01:14:56.000000 ccdproc-2.4.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1217 2018-08-14 01:14:56.000000 ccdproc-2.4.2/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2024-05-03 15:37:24.666875 ccdproc-2.4.2/.github/workflows/
+-rw-r--r--   0 mattcraig   (501) staff       (20)     3334 2024-05-03 15:23:45.000000 ccdproc-2.4.2/.github/workflows/ci_tests.yml
+-rw-r--r--   0 mattcraig   (501) staff       (20)      771 2021-03-19 20:06:25.000000 ccdproc-2.4.2/.gitignore
+-rw-r--r--   0 mattcraig   (501) staff       (20)        0 2019-12-24 20:04:16.000000 ccdproc-2.4.2/.gitmodules
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1134 2019-09-02 21:23:23.000000 ccdproc-2.4.2/.mailmap
+-rw-r--r--   0 mattcraig   (501) staff       (20)      169 2024-05-03 15:23:45.000000 ccdproc-2.4.2/.readthedocs.yml
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2577 2024-05-03 15:23:45.000000 ccdproc-2.4.2/AUTHORS.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)    17126 2024-05-03 15:37:17.000000 ccdproc-2.4.2/CHANGES.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1822 2019-09-02 17:30:31.000000 ccdproc-2.4.2/CITATION.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      180 2019-09-02 17:30:31.000000 ccdproc-2.4.2/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1503 2018-08-18 01:06:53.000000 ccdproc-2.4.2/LICENSE.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      382 2020-11-28 20:18:08.000000 ccdproc-2.4.2/MANIFEST.in
+-rw-r--r--   0 mattcraig   (501) staff       (20)      786 2024-05-03 15:37:24.681353 ccdproc-2.4.2/PKG-INFO
+-rw-r--r--   0 mattcraig   (501) staff       (20)     3785 2021-03-19 20:06:38.000000 ccdproc-2.4.2/README.rst
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2024-05-03 15:37:24.668589 ccdproc-2.4.2/ccdproc/
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1124 2021-05-19 00:45:02.000000 ccdproc-2.4.2/ccdproc/__init__.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)      355 2021-05-19 00:45:02.000000 ccdproc-2.4.2/ccdproc/_astropy_init.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)      408 2018-08-18 01:06:53.000000 ccdproc-2.4.2/ccdproc/ccddata.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    38231 2022-11-17 14:20:04.000000 ccdproc-2.4.2/ccdproc/combiner.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1216 2022-01-19 16:10:46.000000 ccdproc-2.4.2/ccdproc/conftest.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    76092 2022-06-01 13:16:23.000000 ccdproc-2.4.2/ccdproc/core.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2024-05-03 15:37:24.669806 ccdproc-2.4.2/ccdproc/extern/
+-rw-r--r--   0 mattcraig   (501) staff       (20)       64 2018-08-18 01:06:53.000000 ccdproc-2.4.2/ccdproc/extern/__init__.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    19008 2024-05-03 15:23:45.000000 ccdproc-2.4.2/ccdproc/extern/bitfield.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    37073 2024-05-03 15:23:45.000000 ccdproc-2.4.2/ccdproc/image_collection.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     5533 2021-03-19 20:06:38.000000 ccdproc-2.4.2/ccdproc/log_meta.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2024-05-03 15:37:24.672731 ccdproc-2.4.2/ccdproc/tests/
+-rw-r--r--   0 mattcraig   (501) staff       (20)      121 2018-08-14 01:14:56.000000 ccdproc-2.4.2/ccdproc/tests/__init__.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2024-05-03 15:37:24.673830 ccdproc-2.4.2/ccdproc/tests/data/
+-rw-r--r--   0 mattcraig   (501) staff       (20)      257 2018-08-14 01:14:56.000000 ccdproc-2.4.2/ccdproc/tests/data/README.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)   561600 2021-12-21 15:57:22.000000 ccdproc-2.4.2/ccdproc/tests/data/a8280271.fits
+-rw-r--r--   0 mattcraig   (501) staff       (20)      459 2019-09-02 17:30:31.000000 ccdproc-2.4.2/ccdproc/tests/data/expected_ifc_file_properties.csv
+-rw-r--r--   0 mattcraig   (501) staff       (20)    20160 2019-09-02 17:30:31.000000 ccdproc-2.4.2/ccdproc/tests/data/flat-mef.fits
+-rw-r--r--   0 mattcraig   (501) staff       (20)    20160 2019-09-02 17:30:31.000000 ccdproc-2.4.2/ccdproc/tests/data/science-mef.fits
+-rw-r--r--   0 mattcraig   (501) staff       (20)    23040 2021-12-21 15:57:17.000000 ccdproc-2.4.2/ccdproc/tests/data/sip-wcs.fit
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2156 2019-09-02 17:30:31.000000 ccdproc-2.4.2/ccdproc/tests/make_mef.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2297 2022-01-19 16:10:46.000000 ccdproc-2.4.2/ccdproc/tests/pytest_fixtures.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     7044 2022-01-19 16:10:46.000000 ccdproc-2.4.2/ccdproc/tests/run_for_memory_profile.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     7763 2019-09-02 17:30:31.000000 ccdproc-2.4.2/ccdproc/tests/run_profile.ipynb
+-rw-r--r--   0 mattcraig   (501) staff       (20)     9323 2024-05-03 15:23:45.000000 ccdproc-2.4.2/ccdproc/tests/run_with_file_number_limit.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2253 2022-01-19 16:10:46.000000 ccdproc-2.4.2/ccdproc/tests/test_bitfield.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    10893 2021-03-19 20:06:38.000000 ccdproc-2.4.2/ccdproc/tests/test_ccdmask.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    42970 2024-05-03 15:23:45.000000 ccdproc-2.4.2/ccdproc/tests/test_ccdproc.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     4202 2021-03-19 20:06:38.000000 ccdproc-2.4.2/ccdproc/tests/test_ccdproc_logging.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1765 2024-05-03 15:23:45.000000 ccdproc-2.4.2/ccdproc/tests/test_combine_open_files.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    35523 2022-11-17 14:20:04.000000 ccdproc-2.4.2/ccdproc/tests/test_combiner.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    15357 2024-05-03 15:23:45.000000 ccdproc-2.4.2/ccdproc/tests/test_cosmicray.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2132 2021-03-15 15:22:51.000000 ccdproc-2.4.2/ccdproc/tests/test_gain.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    47393 2024-05-03 15:23:45.000000 ccdproc-2.4.2/ccdproc/tests/test_image_collection.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2170 2021-03-15 15:22:51.000000 ccdproc-2.4.2/ccdproc/tests/test_keyword.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2731 2021-11-19 14:38:28.000000 ccdproc-2.4.2/ccdproc/tests/test_memory_use.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2481 2022-01-19 16:10:46.000000 ccdproc-2.4.2/ccdproc/tests/test_rebin.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2581 2021-03-15 15:22:51.000000 ccdproc-2.4.2/ccdproc/tests/test_wrapped_external_funcs.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2024-05-03 15:37:24.674230 ccdproc-2.4.2/ccdproc/utils/
+-rw-r--r--   0 mattcraig   (501) staff       (20)      199 2018-08-14 01:14:56.000000 ccdproc-2.4.2/ccdproc/utils/__init__.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2932 2019-09-06 01:45:09.000000 ccdproc-2.4.2/ccdproc/utils/sample_directory.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     4170 2018-08-18 01:06:53.000000 ccdproc-2.4.2/ccdproc/utils/slices.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2024-05-03 15:37:24.674481 ccdproc-2.4.2/ccdproc/utils/tests/
+-rw-r--r--   0 mattcraig   (501) staff       (20)        0 2018-08-14 01:14:56.000000 ccdproc-2.4.2/ccdproc/utils/tests/__init__.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     4340 2018-08-18 01:06:53.000000 ccdproc-2.4.2/ccdproc/utils/tests/test_slices.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)      411 2024-05-03 15:37:24.000000 ccdproc-2.4.2/ccdproc/version.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2024-05-03 15:37:24.680710 ccdproc-2.4.2/ccdproc.egg-info/
+-rw-r--r--   0 mattcraig   (501) staff       (20)      786 2024-05-03 15:37:24.000000 ccdproc-2.4.2/ccdproc.egg-info/PKG-INFO
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2513 2024-05-03 15:37:24.000000 ccdproc-2.4.2/ccdproc.egg-info/SOURCES.txt
+-rw-r--r--   0 mattcraig   (501) staff       (20)        1 2024-05-03 15:37:24.000000 ccdproc-2.4.2/ccdproc.egg-info/dependency_links.txt
+-rw-r--r--   0 mattcraig   (501) staff       (20)        1 2024-05-03 15:37:24.000000 ccdproc-2.4.2/ccdproc.egg-info/not-zip-safe
+-rw-r--r--   0 mattcraig   (501) staff       (20)      162 2024-05-03 15:37:24.000000 ccdproc-2.4.2/ccdproc.egg-info/requires.txt
+-rw-r--r--   0 mattcraig   (501) staff       (20)        8 2024-05-03 15:37:24.000000 ccdproc-2.4.2/ccdproc.egg-info/top_level.txt
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2024-05-03 15:37:24.678012 ccdproc-2.4.2/docs/
+-rw-r--r--   0 mattcraig   (501) staff       (20)     4724 2018-08-14 01:14:56.000000 ccdproc-2.4.2/docs/Makefile
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2024-05-03 15:37:24.679482 ccdproc-2.4.2/docs/_static/
+-rw-r--r--   0 mattcraig   (501) staff       (20)   370070 2018-08-14 01:14:56.000000 ccdproc-2.4.2/docs/_static/ccd_proc.ico
+-rwxr-xr-x   0 mattcraig   (501) staff       (20)     6867 2018-08-14 01:14:56.000000 ccdproc-2.4.2/docs/_static/ccd_proc.png
+-rw-r--r--   0 mattcraig   (501) staff       (20)      208 2018-08-14 01:14:56.000000 ccdproc-2.4.2/docs/_static/ccdproc.css
+-rwxr-xr-x   0 mattcraig   (501) staff       (20)    51513 2018-08-14 01:14:56.000000 ccdproc-2.4.2/docs/_static/ccdproc.svg
+-rw-r--r--   0 mattcraig   (501) staff       (20)     9342 2019-09-02 17:30:31.000000 ccdproc-2.4.2/docs/_static/ccdproc_banner.pdf
+-rw-r--r--   0 mattcraig   (501) staff       (20)    95067 2019-09-02 17:30:31.000000 ccdproc-2.4.2/docs/_static/ccdproc_banner.png
+-rwxr-xr-x   0 mattcraig   (501) staff       (20)   222655 2019-12-24 20:04:16.000000 ccdproc-2.4.2/docs/_static/ccdproc_banner.svg
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2024-05-03 15:37:24.663518 ccdproc-2.4.2/docs/_templates/
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2024-05-03 15:37:24.680172 ccdproc-2.4.2/docs/_templates/autosummary/
+-rw-r--r--   0 mattcraig   (501) staff       (20)      250 2018-08-14 01:14:56.000000 ccdproc-2.4.2/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      251 2018-08-14 01:14:56.000000 ccdproc-2.4.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      252 2018-08-14 01:14:56.000000 ccdproc-2.4.2/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      222 2019-09-02 17:30:31.000000 ccdproc-2.4.2/docs/api.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)       55 2018-08-14 01:14:56.000000 ccdproc-2.4.2/docs/authors_for_sphinx.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     7432 2024-05-03 15:23:45.000000 ccdproc-2.4.2/docs/ccddata.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)       90 2018-08-14 01:14:56.000000 ccdproc-2.4.2/docs/changelog.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)       52 2019-09-02 17:30:31.000000 ccdproc-2.4.2/docs/citation.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)       54 2019-09-02 17:30:31.000000 ccdproc-2.4.2/docs/conduct.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     6951 2021-12-21 15:57:22.000000 ccdproc-2.4.2/docs/conf.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1599 2019-09-02 17:30:31.000000 ccdproc-2.4.2/docs/contributing.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      280 2021-05-19 00:45:02.000000 ccdproc-2.4.2/docs/default_config.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     3839 2019-09-02 17:30:31.000000 ccdproc-2.4.2/docs/getting_started.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     9815 2021-12-21 15:57:22.000000 ccdproc-2.4.2/docs/image_combination.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     8376 2021-12-21 15:57:22.000000 ccdproc-2.4.2/docs/image_management.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1637 2021-05-19 00:45:02.000000 ccdproc-2.4.2/docs/index.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1845 2021-03-19 20:06:38.000000 ccdproc-2.4.2/docs/install.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      157 2019-03-08 17:03:24.000000 ccdproc-2.4.2/docs/license.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     4513 2018-08-14 01:14:56.000000 ccdproc-2.4.2/docs/make.bat
+-rw-r--r--   0 mattcraig   (501) staff       (20)      892 2019-09-02 17:30:31.000000 ccdproc-2.4.2/docs/overview.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      883 2019-09-02 17:30:31.000000 ccdproc-2.4.2/docs/reduction_examples.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)    21228 2019-12-24 20:04:16.000000 ccdproc-2.4.2/docs/reduction_toolbox.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)       78 2024-05-03 15:23:45.000000 ccdproc-2.4.2/docs/rtd-pip-requirements
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2024-05-03 15:37:24.680486 ccdproc-2.4.2/licenses/
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1463 2018-08-18 01:06:53.000000 ccdproc-2.4.2/licenses/LICENSE_STSCI_TOOLS.txt
+-rw-r--r--   0 mattcraig   (501) staff       (20)      251 2018-08-18 01:06:53.000000 ccdproc-2.4.2/licenses/README.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      132 2019-12-24 20:04:16.000000 ccdproc-2.4.2/pyproject.toml
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1902 2024-05-03 15:37:24.681860 ccdproc-2.4.2/setup.cfg
+-rwxr-xr-x   0 mattcraig   (501) staff       (20)     1609 2019-12-24 20:04:16.000000 ccdproc-2.4.2/setup.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2661 2024-05-03 15:23:45.000000 ccdproc-2.4.2/tox.ini
```

### Comparing `ccdproc-2.4.1/.github/ISSUE_TEMPLATE.md` & `ccdproc-2.4.2/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/.github/PULL_REQUEST_TEMPLATE.md` & `ccdproc-2.4.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/.github/workflows/ci_tests.yml` & `ccdproc-2.4.2/.github/workflows/ci_tests.yml`

 * *Files 12% similar despite different names*

```diff
@@ -43,62 +43,70 @@
             tox_env: 'py39-test-alldeps-numpy119-cov-bottleneck'
 
           - name: 'ubuntu-py310'
             os: ubuntu-latest
             python: '3.10'
             tox_env: 'py310-test-alldeps-numpy121'
 
-          - name: 'macos-py39'
+          - name: 'ubuntu-py311'
+            os: ubuntu-latest
+            python: '3.11'
+            tox_env: 'py311-test-alldeps-numpy123'
+
+          - name: 'ubuntu-py312'
+            os: ubuntu-latest
+            python: '3.12'
+            tox_env: 'py310-test-alldeps-numpy126'
+
+          - name: 'macos-py312'
             os: macos-latest
-            python: '3.9'
-            tox_env: 'py39-test-alldeps'
+            python: '3.12'
+            tox_env: 'py312-test-alldeps'
 
-          - name: 'windows-py310'
+          - name: 'windows-py312'
             os: windows-latest
-            python: '3.10'
-            tox_env: 'py310-test-alldeps'
+            python: '3.12'
+            tox_env: 'py312-test-alldeps'
 
           - name: 'ubuntu-codestyle'
             os: ubuntu-latest
             python: '3.10'
             tox_env: 'pycodestyle'
 
           - name: 'ubuntu-build_docs'
             os: ubuntu-latest
-            python: '3.10'
+            python: '3.12'
             tox_env: 'build_docs'
 
           - name: 'ubuntu-py310-test-alldeps-devdeps'
             os: ubuntu-latest
             python: '3.10'
             tox_env: 'py310-test-alldeps-devdeps'
 
     steps:
     - name: Check out repository
-      uses: actions/checkout@v2
+      uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python }}
     - name: Install base dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install tox wheel
     - name: Install graphviz dependency
       if: "endsWith(matrix.tox_env, 'build_docs')"
       run: sudo apt-get -y install graphviz
-    - name: Print Python, pip, setuptools, and tox versions
+    - name: Print Python env
       run: |
-        python -c "import sys; print(f'Python {sys.version}')"
-        python -c "import pip; print(f'pip {pip.__version__}')"
-        python -c "import setuptools; print(f'setuptools {setuptools.__version__}')"
-        python -c "import tox; print(f'tox {tox.__version__}')"
+        python --version
+        python -m pip list
     - name: Run tests
       if: "! matrix.use_remote_data"
       run: |
         tox -e ${{ matrix.tox_env }} -- ${{ matrix.toxposargs }}
     # - name: Run tests with remote data
     #   if: "matrix.use_remote_data"
     #   run: tox -e ${{ matrix.tox_env }} -- --remote-data=any
     - name: Upload coverage to codecov
       if: "endsWith(matrix.tox_env, '-cov')"
-      uses: codecov/codecov-action@v2
+      uses: codecov/codecov-action@v4
```

### Comparing `ccdproc-2.4.1/.gitignore` & `ccdproc-2.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/.mailmap` & `ccdproc-2.4.2/.mailmap`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/AUTHORS.rst` & `ccdproc-2.4.2/AUTHORS.rst`

 * *Files 6% similar despite different names*

```diff
@@ -25,28 +25,30 @@
 * Javier Blasco (@javierblasco)
 * Attila Bódi (@astrobatty)
 * Larry Bradley (@larrybradley)
 * Julio C. N. Campagnolo (@juliotux)
 * Mihai Cara (@mcara)
 * James Davenport (@jradavenport)
 * Christoph Deil (@cdeil)
+* Clément M.T. Robert (@neutrinoceros)
 * Timothy P. Ellsworth-Bowers (@tbowers7)
 * Forrest Gasdia (@fgasdia)
 * Carlos Gomez (@carlgogo)
 * Yash Gondhalekar (@Yash-10)
 * Hans Moritz Günther (@hamogu)
 * Nathan Heidt (@heidtha)
 * Michael Hlabathe (@hlabathems)
 * Elias Holte (@Sondanaa)
 * Anthony Horton (@AnthonyHorton)
 * Jennifer Karr (@JenniferKarr)
 * Yücel Kılıç (@yucelkilic)
 * Kelvin Lee (@laserkelvin)
 * Pey Lian Lim (@pllim)
 * James McCormac (@jmccormac01)
+* Abigale Moen (@AbigaleMoen)
 * Stefan Nelson (@stefannelson)
 * Joe Philip Ninan (@indiajoe)
 * Punyaslok Pattnaik (@Punyaslok)
 * Adrian Price-Whelan (@adrn)
 * JVSN Reddy (@janga1997)
 * Luca Rizzi (@lucarizzi)
 * Thomas Robitaille (@astrofrog)
```

### Comparing `ccdproc-2.4.1/CHANGES.rst` & `ccdproc-2.4.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+2.4.1 (unreleased)
+------------------
+
+New Features
+^^^^^^^^^^^^
+
+Other Changes and Additions
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+2.4.2 (2024-05-03)
+------------------
+
+New Features
+^^^^^^^^^^^^
+
+Other Changes and Additions
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+- Make ccdproc compatible with numpy 2. [#824]
+
+Bug Fixes
+^^^^^^^^^
+
 2.4.1 (2023-05-30)
 ------------------
 
 New Features
 ^^^^^^^^^^^^
 
 Other Changes and Additions
```

### Comparing `ccdproc-2.4.1/CITATION.rst` & `ccdproc-2.4.2/CITATION.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/LICENSE.rst` & `ccdproc-2.4.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/README.rst` & `ccdproc-2.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/__init__.py` & `ccdproc-2.4.2/ccdproc/__init__.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/combiner.py` & `ccdproc-2.4.2/ccdproc/combiner.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/conftest.py` & `ccdproc-2.4.2/ccdproc/conftest.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/core.py` & `ccdproc-2.4.2/ccdproc/core.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/extern/bitfield.py` & `ccdproc-2.4.2/ccdproc/extern/bitfield.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 #           (i.e., `numpy.uint64`), it was not converted to Python `int`.
 #       3. `bitfield_to_boolean_mask()` will no longer crash when
 #          `ignore_flags` argument contains bit flags beyond what the type of
 #          the argument `bitfield` can hold.
 # 1.1.1 (30-January-2018) - Improved filtering of high bits in flags.
 #
 INT_TYPE = (int, long,) if sys.version_info < (3,) else (int,)
-MAX_UINT_TYPE = np.maximum_sctype(np.uint)
+MAX_UINT_TYPE = np.uint64
 SUPPORTED_FLAGS = int(np.bitwise_not(
     0, dtype=MAX_UINT_TYPE, casting='unsafe'
 ))
 
 
 def is_bit_flag(n):
     """
```

### Comparing `ccdproc-2.4.1/ccdproc/image_collection.py` & `ccdproc-2.4.2/ccdproc/image_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,28 +8,25 @@
 import logging
 
 import numpy as np
 import numpy.ma as ma
 
 from astropy.table import Table, MaskedColumn
 import astropy.io.fits as fits
-from astropy.utils import minversion
 
 import warnings
 from astropy.utils.exceptions import AstropyUserWarning
 
 from .ccddata import fits_ccddata_reader, _recognized_fits_file_extensions
 
 logger = logging.getLogger(__name__)
 
 __all__ = ['ImageFileCollection']
 __doctest_skip__ = ['*']
 
-_ASTROPY_LT_1_3 = not minversion("astropy", "1.3")
-
 
 class ImageFileCollection:
     """
     Representation of a collection of image files.
 
     The class offers a table summarizing values of
     keywords in the FITS headers of the files in the collection and offers
@@ -799,15 +796,14 @@
                         files.append(infile)
 
         files.sort()
         return files
 
     def _generator(self, return_type,
                    save_with_name="", save_location='',
-                   clobber=False,
                    overwrite=False,
                    do_not_scale_image_data=True,
                    return_fname=False,
                    ccd_kwargs=None,
                    **kwd):
         """
         Generator that yields each {name} in the collection.
@@ -835,18 +831,14 @@
             ``save_location`` set.
             Default is ``''``.
 
         overwrite : bool, optional
             If ``True``, overwrite input FITS files.
             Default is ``False``.
 
-        clobber : bool, optional
-            Alias for ``overwrite``.
-            Default is ``False``.
-
         do_not_scale_image_data : bool, optional
             If ``True``, prevents fits from scaling images. Default is
             ``{default_scaling}``.
             Default is ``True``.
 
         return_fname : bool, optional
             If True, return the tuple (header, file_name) instead of just
@@ -934,39 +926,28 @@
             basename = path.basename(full_path)
             if save_with_name:
                 base, ext = path.splitext(basename)
                 basename = base + save_with_name + ext
 
             new_path = path.join(destination_dir, basename)
 
-            # I really should have called the option overwrite from
-            # the beginning. The hack below ensures old code works,
-            # at least...
-            if clobber or overwrite:
-                if _ASTROPY_LT_1_3:
-                    nuke_existing = {'clobber': True}
-                else:
-                    nuke_existing = {'overwrite': True}
-            else:
-                nuke_existing = {}
-
             if return_type == 'ccd':
                 pass
-            elif (new_path != full_path) or nuke_existing:
+            elif (new_path != full_path) or overwrite:
                 with fits.open(full_path, **add_kwargs) as hdulist:
                     ext_index = hdulist.index_of(self.ext)
                     if return_type == 'hdu':
                         hdulist[ext_index] = return_thing
                     elif return_type == 'data':
                         hdulist[ext_index].data = return_thing
                     elif return_type == 'header':
                         hdulist[ext_index].header = return_thing
 
                     try:
-                        hdulist.writeto(new_path, **nuke_existing)
+                        hdulist.writeto(new_path, overwrite=overwrite)
                     except IOError:
                         logger.error('error writing file %s', new_path)
                         raise
 
         # reset mask
         for col in self.summary.columns:
             self.summary[col].mask = current_mask[col]
@@ -987,24 +968,30 @@
         return_type='astropy.io.fits.Header')
 
     def hdus(self, do_not_scale_image_data=False, **kwd):
         return self._generator('hdu',
                                do_not_scale_image_data=do_not_scale_image_data,
                                **kwd)
     hdus.__doc__ = _generator.__doc__.format(
-        name='HDUList', default_scaling='False',
-        return_type='astropy.io.fits.HDUList')
+        name='HDU', default_scaling='False',
+        return_type="`, ` ".join(('astropy.io.fits.PrimaryHDU', 'astropy.io.fits.ImageHDU')))
 
     def data(self, do_not_scale_image_data=False, **kwd):
         return self._generator('data',
                                do_not_scale_image_data=do_not_scale_image_data,
                                **kwd)
     data.__doc__ = _generator.__doc__.format(
         name='image', default_scaling='False', return_type='numpy.ndarray')
 
     def ccds(self, ccd_kwargs=None, **kwd):
-        if kwd.get('clobber') or kwd.get('overwrite'):
-            raise NotImplementedError(
-                "overwrite=True (or clobber=True) is not supported for CCDs.")
+        if (clobber := kwd.get('clobber')) is not None:
+            warnings.warn(
+                "The 'clobber' keyword argument is a deprecated alias for 'overwrite'",
+                category=DeprecationWarning,
+                stacklevel=2
+            )
+            kwd["overwrite"] = clobber
+        if kwd.get('overwrite'):
+            raise NotImplementedError("overwrite=True is not supported for CCDs.")
         return self._generator('ccd', ccd_kwargs=ccd_kwargs, **kwd)
     ccds.__doc__ = _generator.__doc__.format(
         name='CCDData', default_scaling='True', return_type='astropy.nddata.CCDData')
```

### Comparing `ccdproc-2.4.1/ccdproc/log_meta.py` & `ccdproc-2.4.2/ccdproc/log_meta.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/tests/data/a8280271.fits` & `ccdproc-2.4.2/ccdproc/tests/data/a8280271.fits`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/tests/data/flat-mef.fits` & `ccdproc-2.4.2/ccdproc/tests/data/flat-mef.fits`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/tests/data/science-mef.fits` & `ccdproc-2.4.2/ccdproc/tests/data/science-mef.fits`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/tests/data/sip-wcs.fit` & `ccdproc-2.4.2/ccdproc/tests/data/sip-wcs.fit`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/tests/make_mef.py` & `ccdproc-2.4.2/ccdproc/tests/make_mef.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/tests/pytest_fixtures.py` & `ccdproc-2.4.2/ccdproc/tests/pytest_fixtures.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/tests/run_for_memory_profile.py` & `ccdproc-2.4.2/ccdproc/tests/run_for_memory_profile.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/tests/run_profile.ipynb` & `ccdproc-2.4.2/ccdproc/tests/run_profile.ipynb`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/tests/run_with_file_number_limit.py` & `ccdproc-2.4.2/ccdproc/tests/run_with_file_number_limit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-from argparse import ArgumentParser
 from tempfile import TemporaryDirectory
 from pathlib import Path
 import mmap
 import sys
 import gc
 
-import psutil
-
 import numpy as np
 from astropy.io import fits
 
 # This bit of hackery ensures that we can see ccdproc from within
 # the test suite
 sys.path.append(str(Path().cwd()))
 from ccdproc import combine
@@ -226,14 +223,18 @@
     else:
         print('Opens succeeded, files currently open:',
               len(proc.open_files()),
               flush=True)
 
 
 if __name__ == '__main__':
+    from argparse import ArgumentParser
+
+    import psutil
+
     parser = ArgumentParser()
     parser.add_argument('number', type=int,
                         help='Limit on number of open files.')
     parser.add_argument('--kind', action='store', default='plain',
                         choices=ALLOWED_EXTENSIONS.keys(),
                         help='Kind of file to generate for test; '
                              'default is plain')
```

### Comparing `ccdproc-2.4.1/ccdproc/tests/test_bitfield.py` & `ccdproc-2.4.2/ccdproc/tests/test_bitfield.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/tests/test_ccdmask.py` & `ccdproc-2.4.2/ccdproc/tests/test_ccdmask.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/tests/test_ccdproc.py` & `ccdproc-2.4.2/ccdproc/tests/test_ccdproc.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 try:
     from ..core import block_reduce, block_average, block_replicate
     HAS_BLOCK_X_FUNCS = True
 except ImportError:
     HAS_BLOCK_X_FUNCS = False
 
+_NUMPY_COPY_IF_NEEDED = False if np.__version__.startswith("1.") else None
 
 # Test creating deviation
 # Success expected if u_image * u_gain = u_readnoise
 @pytest.mark.parametrize('u_image,u_gain,u_readnoise,expect_success', [
                          (u.electron, None, u.electron, True),
                          (u.electron, u.electron, u.electron, False),
                          (u.adu, u.electron / u.adu, u.electron, True),
@@ -973,15 +974,15 @@
     # that the pixels have been scaled.
     np.testing.assert_allclose(ccd_data.data / 4,
                                data_cutout,
                                rtol=1e-5)
 
     # Mask should be true for four pixels (all nearest neighbors)
     # of the single pixel we masked initially.
-    new_center = np.array(new_ccd.wcs.wcs.crpix, dtype=int, copy=False)
+    new_center = np.array(new_ccd.wcs.wcs.crpix, dtype=int, copy=_NUMPY_COPY_IF_NEEDED)
     assert np.all(new_ccd.mask[new_center[0]:new_center[0]+2,
                                new_center[1]:new_center[1]+2])
 
     # Those four, and any that reproject made nan because they draw on
     # pixels outside the footprint of the original image, are the only
     # pixels that should be masked.
     assert new_ccd.mask.sum() == 4 + np.isnan(new_ccd.data).sum()
```

### Comparing `ccdproc-2.4.1/ccdproc/tests/test_ccdproc_logging.py` & `ccdproc-2.4.2/ccdproc/tests/test_ccdproc_logging.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/tests/test_combine_open_files.py` & `ccdproc-2.4.2/ccdproc/tests/test_combine_open_files.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,42 +16,36 @@
 common_args = [sys.executable, str(run_dir / 'run_with_file_number_limit.py'),
                '--kind', 'fits', '--overhead', OVERHEAD]
 
 
 # Regression test for #629
 @pytest.mark.skipif(os.environ.get('APPVEYOR') or os.sys.platform == 'win32',
                     reason='Test relies on linux/osx features of psutil')
-@pytest.mark.skipif(sys.version_info < (3, 5),
-                    reason='Test requires subprocess.run, introduced in 3.5')
 def test_open_files_combine_no_chunks():
     """
     Test that we are not opening (much) more than the number of files
     we are processing.
     """
     # Make a copy
     args = list(common_args)
     args.extend(['--open-by', 'combine-nochunk', NUM_FILE_LIMIT])
-    p = subprocess.run(args=args, stderr=subprocess.PIPE,
-                       cwd=str(subprocess_dir))
+    p = subprocess.run(args=args, cwd=str(subprocess_dir))
     # If we have succeeded the test passes. We are only checking that
     # we don't have too many files open.
     assert p.returncode == 0
 
 
 # Regression test for #629
 @pytest.mark.skipif(os.environ.get('APPVEYOR') or os.sys.platform == 'win32',
                     reason='Test relies on linux/osx features of psutil')
-@pytest.mark.skipif(sys.version_info < (3, 5),
-                    reason='Test requires subprocess.run, introduced in 3.5')
 def test_open_files_combine_chunks():
     """
     Test that we are not opening (much) more than the number of files
     we are processing when combination is broken into chunks.
     """
     # Make a copy
     args = list(common_args)
     args.extend(['--open-by', 'combine-chunk', NUM_FILE_LIMIT])
-    p = subprocess.run(args=args, stderr=subprocess.PIPE,
-                       cwd=str(subprocess_dir))
+    p = subprocess.run(args=args, cwd=str(subprocess_dir))
     # If we have succeeded the test passes. We are only checking that
     # we don't have too many files open.
     assert p.returncode == 0
```

### Comparing `ccdproc-2.4.1/ccdproc/tests/test_combiner.py` & `ccdproc-2.4.2/ccdproc/tests/test_combiner.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/tests/test_cosmicray.py` & `ccdproc-2.4.2/ccdproc/tests/test_cosmicray.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,35 +164,42 @@
         cosmicray_lacosmic(ccd_data,
                            gain=gain,
                            gain_apply=True,
                            readnoise=readnoise)
     assert 'Inconsistent units' in str(e.value)
 
 
-def test_cosmicray_lacosmic_warns_on_ccd_in_electrons(recwarn):
+if OLD_ASTROSCRAPPY:
+    decorator = pytest.mark.filterwarnings("ignore:`np.bool` is a deprecated alias:DeprecationWarning")
+else:
+    decorator = lambda f: f
+
+@decorator
+def test_cosmicray_lacosmic_warns_on_ccd_in_electrons():
     # Check that an input ccd in electrons raises a warning.
     ccd_data = ccd_data_func(data_scale=DATA_SCALE)
     # The unit below is important for the test; this unit on
     # input is supposed to raise an error.
     ccd_data.unit = u.electron
     threshold = 5
     add_cosmicrays(ccd_data, DATA_SCALE, threshold, ncrays=NCRAYS)
     noise = DATA_SCALE * np.ones_like(ccd_data.data)
     ccd_data.uncertainty = noise
     # No units here on purpose.
     gain = 2.0
     # Don't really need to set this (6.5 is the default value) but want to
     # make lack of units explicit.
     readnoise = 6.5
-    new_ccd = cosmicray_lacosmic(ccd_data,
-                                 gain=gain,
-                                 gain_apply=True,
-                                 readnoise=readnoise)
-
-    assert "Image unit is electron" in str(recwarn.pop())
+    with pytest.warns(UserWarning, match="Image unit is electron"):
+        cosmicray_lacosmic(
+            ccd_data,
+            gain=gain,
+            gain_apply=True,
+            readnoise=readnoise
+        )
 
 
 # The skip can be removed when the oldest supported astroscrappy
 # is 1.1.0 or higher
 @pytest.mark.skipif(OLD_ASTROSCRAPPY,
                     reason='astroscrappy < 1.1.0 does not support '
                            'this functionality')
```

### Comparing `ccdproc-2.4.1/ccdproc/tests/test_gain.py` & `ccdproc-2.4.2/ccdproc/tests/test_gain.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/tests/test_image_collection.py` & `ccdproc-2.4.2/ccdproc/tests/test_image_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -751,15 +751,15 @@
         Also CCDData doesn't explicitly support in-place operations so it's to
         easy to create a new CCDData object inadvertantly and all modifications
         might be lost.
         """
         ic = ImageFileCollection(triage_setup.test_dir)
         with pytest.raises(NotImplementedError):
             ic.ccds(overwrite=True)
-        with pytest.raises(NotImplementedError):
+        with pytest.deprecated_call(), pytest.raises(NotImplementedError):
             ic.ccds(clobber=True)
 
     def test_glob_matching(self, triage_setup):
         # We'll create two files with strange names to test glob
         # includes / excludes
         one = fits.PrimaryHDU()
         one.data = np.zeros((5, 5))
@@ -948,14 +948,15 @@
 
         for h in ic.headers(imagetyp='light'):
             assert h['imagetyp'].lower() == 'light'
             n_heads += 1
 
         assert n_heads == expected_heads
 
+    @pytest.mark.filterwarnings("ignore:The following header keyword is invalid:UserWarning")
     def test_less_strict_verify_option(self, triage_setup):
         # Tests for feature request
         #
         #    https://github.com/astropy/ccdproc/issues/607
         #
         # which would allow reading of otherwise invalid FITS headers.
```

### Comparing `ccdproc-2.4.1/ccdproc/tests/test_keyword.py` & `ccdproc-2.4.2/ccdproc/tests/test_keyword.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/tests/test_memory_use.py` & `ccdproc-2.4.2/ccdproc/tests/test_memory_use.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/tests/test_rebin.py` & `ccdproc-2.4.2/ccdproc/tests/test_rebin.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/tests/test_wrapped_external_funcs.py` & `ccdproc-2.4.2/ccdproc/tests/test_wrapped_external_funcs.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/utils/sample_directory.py` & `ccdproc-2.4.2/ccdproc/utils/sample_directory.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/utils/slices.py` & `ccdproc-2.4.2/ccdproc/utils/slices.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc/utils/tests/test_slices.py` & `ccdproc-2.4.2/ccdproc/utils/tests/test_slices.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/ccdproc.egg-info/SOURCES.txt` & `ccdproc-2.4.2/ccdproc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/docs/Makefile` & `ccdproc-2.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/docs/_static/ccd_proc.ico` & `ccdproc-2.4.2/docs/_static/ccd_proc.ico`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/docs/_static/ccd_proc.png` & `ccdproc-2.4.2/docs/_static/ccd_proc.png`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/docs/_static/ccdproc.svg` & `ccdproc-2.4.2/docs/_static/ccdproc.svg`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/docs/_static/ccdproc_banner.pdf` & `ccdproc-2.4.2/docs/_static/ccdproc_banner.pdf`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/docs/_static/ccdproc_banner.png` & `ccdproc-2.4.2/docs/_static/ccdproc_banner.png`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/docs/_static/ccdproc_banner.svg` & `ccdproc-2.4.2/docs/_static/ccdproc_banner.svg`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/docs/ccddata.rst` & `ccdproc-2.4.2/docs/ccddata.rst`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 Using these methods propagates errors correctly (if the errors are
 uncorrelated), take care of any necessary unit conversions, and apply masks
 appropriately. Note that the metadata of the result is *not* set if the operation
 is between two `~astropy.nddata.CCDData` objects.
 
     >>> result = ccd.multiply(0.2 * u.adu)
     >>> uncertainty_ratio = result.uncertainty.array[0, 0]/ccd.uncertainty.array[0, 0]
-    >>> round(uncertainty_ratio, 5)   # doctest: +FLOAT_CMP
+    >>> float(round(uncertainty_ratio, 5))   # doctest: +FLOAT_CMP
     0.2
     >>> result.unit
     Unit("adu electron")
 
 .. note::
     In most cases you should use the functions described in
     :ref:`reduction_toolbox` to perform common operations like scaling by gain or
```

### Comparing `ccdproc-2.4.1/docs/conf.py` & `ccdproc-2.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/docs/contributing.rst` & `ccdproc-2.4.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/docs/getting_started.rst` & `ccdproc-2.4.2/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/docs/image_combination.rst` & `ccdproc-2.4.2/docs/image_combination.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/docs/image_management.rst` & `ccdproc-2.4.2/docs/image_management.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/docs/index.rst` & `ccdproc-2.4.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/docs/install.rst` & `ccdproc-2.4.2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/docs/make.bat` & `ccdproc-2.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/docs/overview.rst` & `ccdproc-2.4.2/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/docs/reduction_examples.rst` & `ccdproc-2.4.2/docs/reduction_examples.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/docs/reduction_toolbox.rst` & `ccdproc-2.4.2/docs/reduction_toolbox.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/licenses/LICENSE_STSCI_TOOLS.txt` & `ccdproc-2.4.2/licenses/LICENSE_STSCI_TOOLS.txt`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/setup.cfg` & `ccdproc-2.4.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool:pytest]
 minversion = 2.2
 testpaths = "ccdproc" "docs"
 norecursedirs = build docs/_build
 doctest_plus = enabled
-addopts = --doctest-rst
+addopts = --doctest-rst --color=yes
 filterwarnings = 
 	error
 	ignore:numpy\.ufunc size changed:RuntimeWarning
 	ignore:numpy.ndarray size changed:RuntimeWarning
 	ignore:`np.bool` is a deprecated alias for the builtin `bool`:DeprecationWarning
 markers = 
 	data_size(N): set dimension of square data array for ccd_data fixture
```

### Comparing `ccdproc-2.4.1/setup.py` & `ccdproc-2.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.1/tox.ini` & `ccdproc-2.4.2/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -15,31 +15,31 @@
 
 description =
     run tests
     alldeps: with all optional dependencies
     devdeps: with the latest developer version of key dependencies
     oldestdeps: with the oldest supported version of key dependencies
     cov: and test coverage
-    numpy117: with numpy 1.17.*
     numpy118: with numpy 1.18.*
     numpy119: with numpy 1.19.*
     numpy120: with numpy 1.20.*
     numpy121: with numpy 1.21.*
     astropylts: with the latest astropy LTS
     bottleneck: with bottleneck
 
 # The following provides some specific pinnings for key packages
 deps =
     cov: coverage
 
-    numpy117: numpy==1.17.*
     numpy118: numpy==1.18.*
     numpy119: numpy==1.19.*
     numpy120: numpy==1.20.*
     numpy121: numpy==1.21.*
+    numpy123: numpy==1.23.*
+    numpy126: numpy==1.26.*
 
     astroscrappy11: astroscrappy==1.1.*
     astroscrappy10: astroscrappy==1.0.*
 
     astropylts: astropy==4.0.*
 
     bottleneck: bottleneck>=1.3.2
```


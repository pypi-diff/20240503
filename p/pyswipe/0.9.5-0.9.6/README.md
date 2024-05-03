# Comparing `tmp/pyswipe-0.9.5.tar.gz` & `tmp/pyswipe-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyswipe-0.9.5.tar", last modified: Thu Feb  8 08:11:10 2024, max compression
+gzip compressed data, was "pyswipe-0.9.6.tar", last modified: Fri May  3 06:12:18 2024, max compression
```

## Comparing `pyswipe-0.9.5.tar` & `pyswipe-0.9.6.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-02-08 08:11:10.671553 pyswipe-0.9.5/
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       68 2023-09-01 08:13:58.000000 pyswipe-0.9.5/.coveragerc
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      136 2023-12-04 08:56:34.000000 pyswipe-0.9.5/.gitignore
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     1241 2023-09-01 08:15:54.000000 pyswipe-0.9.5/.travis.yml
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       59 2023-09-01 08:14:31.000000 pyswipe-0.9.5/CHANGELOG.rst
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      518 2023-12-01 12:23:06.000000 pyswipe-0.9.5/CITATION.cff
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      281 2023-11-17 11:11:19.000000 pyswipe-0.9.5/CITATION_old.cff
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     1072 2023-09-01 08:14:52.000000 pyswipe-0.9.5/LICENSE
--rw-r--r--   0 spencerh  (1000) spencerh  (1000)     6592 2024-02-08 08:11:10.671553 pyswipe-0.9.5/PKG-INFO
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     4012 2023-12-05 06:10:31.000000 pyswipe-0.9.5/README.rst
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      189 2023-11-23 11:54:36.000000 pyswipe-0.9.5/TODO.md
-drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-02-08 08:11:10.611554 pyswipe-0.9.5/docs/
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      676 2023-09-01 08:36:02.000000 pyswipe-0.9.5/docs/Makefile
-drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-02-08 08:11:10.615554 pyswipe-0.9.5/docs/source/
-drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-02-08 08:11:10.615554 pyswipe-0.9.5/docs/source/.templates/
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      157 2021-08-20 11:22:35.000000 pyswipe-0.9.5/docs/source/.templates/layout.html
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       32 2021-08-20 11:22:35.000000 pyswipe-0.9.5/docs/source/changelog.rst
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     6212 2023-09-01 08:44:56.000000 pyswipe-0.9.5/docs/source/conf.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      476 2023-09-01 08:41:32.000000 pyswipe-0.9.5/docs/source/index.rst
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      632 2023-09-01 08:42:02.000000 pyswipe-0.9.5/docs/source/installation.rst
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     2874 2023-09-01 08:46:35.000000 pyswipe-0.9.5/docs/source/model_coefficients.rst
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       29 2021-08-20 11:22:35.000000 pyswipe-0.9.5/docs/source/readme.rst
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     1046 2023-09-01 08:46:59.000000 pyswipe-0.9.5/docs/source/reference.rst
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8103 2023-09-01 08:47:34.000000 pyswipe-0.9.5/docs/source/usage.rst
-drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-02-08 08:11:10.627554 pyswipe-0.9.5/docs/static/
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)  6334764 2021-08-20 11:22:35.000000 pyswipe-0.9.5/docs/static/animation.gif
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       47 2021-08-20 11:22:35.000000 pyswipe-0.9.5/docs/static/custom.css
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   220149 2023-09-14 07:11:29.000000 pyswipe-0.9.5/docs/static/example_plot.png
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     1466 2023-12-05 06:05:40.000000 pyswipe-0.9.5/pyproject.toml
-drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-02-08 08:11:10.655554 pyswipe-0.9.5/pyswipe/
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      305 2024-01-02 13:38:10.000000 pyswipe-0.9.5/pyswipe/__init__.py
-drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-02-08 08:11:10.655554 pyswipe-0.9.5/pyswipe/coefficients/
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   106494 2023-07-19 06:26:07.000000 pyswipe-0.9.5/pyswipe/coefficients/SW_OPER_MIO_SWI_2E_00000000T000000_99999999T999999_0101.txt
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      144 2023-10-19 09:49:00.000000 pyswipe-0.9.5/pyswipe/constants.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   310000 2023-04-17 09:31:48.000000 pyswipe-0.9.5/pyswipe/mlat_scalargrid.txt
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   300000 2023-04-17 09:31:58.000000 pyswipe-0.9.5/pyswipe/mlt_scalargrid.txt
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    13152 2021-08-20 11:22:35.000000 pyswipe-0.9.5/pyswipe/mlt_utils.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    10843 2023-12-30 09:48:19.000000 pyswipe-0.9.5/pyswipe/model_utils.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     5320 2021-08-20 11:22:35.000000 pyswipe-0.9.5/pyswipe/model_vector_to_txt.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    48412 2024-02-05 11:53:08.000000 pyswipe-0.9.5/pyswipe/plot_utils.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   312289 2023-04-17 09:32:08.000000 pyswipe-0.9.5/pyswipe/potential.txt
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    40562 2024-01-23 05:22:49.000000 pyswipe-0.9.5/pyswipe/sh_utils.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   158608 2024-02-05 11:55:28.000000 pyswipe-0.9.5/pyswipe/swipe.py
-drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-02-08 08:11:10.663554 pyswipe-0.9.5/pyswipe/tests/
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8557 2023-12-04 09:00:52.000000 pyswipe-0.9.5/pyswipe/tests/01__plot_cpcp_vs_hemi_bt_and_clockangle.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8061 2023-12-04 09:14:23.000000 pyswipe-0.9.5/pyswipe/tests/02__E_at_lowlatboundary.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    10936 2023-12-04 09:07:00.000000 pyswipe-0.9.5/pyswipe/tests/03__hi-c_cpcp_vs_other_studies.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     9022 2023-12-04 09:08:41.000000 pyswipe-0.9.5/pyswipe/tests/04__potential_dial_plots.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    11168 2023-12-04 09:07:46.000000 pyswipe-0.9.5/pyswipe/tests/04__potential_dial_plots__alternative_levels.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8162 2023-12-04 09:12:25.000000 pyswipe-0.9.5/pyswipe/tests/05__emwork_dial_plots.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8770 2023-12-04 09:09:48.000000 pyswipe-0.9.5/pyswipe/tests/05__emwork_dial_plots__alternative_levels.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     9489 2023-12-04 09:11:29.000000 pyswipe-0.9.5/pyswipe/tests/06__plot_emwork_vs_hemi_bt_and_clockangle.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8325 2023-12-04 09:13:42.000000 pyswipe-0.9.5/pyswipe/tests/08__conductance_dial_plots__filledcell.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     4853 2023-12-30 09:48:19.000000 pyswipe-0.9.5/pyswipe/tests/09__dask_functions_for_large_input.py
-drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-02-08 08:11:10.671553 pyswipe-0.9.5/pyswipe.egg-info/
--rw-r--r--   0 spencerh  (1000) spencerh  (1000)     6592 2024-02-08 08:11:10.000000 pyswipe-0.9.5/pyswipe.egg-info/PKG-INFO
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     1641 2024-02-08 08:11:10.000000 pyswipe-0.9.5/pyswipe.egg-info/SOURCES.txt
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)        1 2024-02-08 08:11:10.000000 pyswipe-0.9.5/pyswipe.egg-info/dependency_links.txt
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      156 2024-02-08 08:11:10.000000 pyswipe-0.9.5/pyswipe.egg-info/requires.txt
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)        8 2024-02-08 08:11:10.000000 pyswipe-0.9.5/pyswipe.egg-info/top_level.txt
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      106 2021-08-20 11:22:35.000000 pyswipe-0.9.5/requirements.txt
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       38 2024-02-08 08:11:10.671553 pyswipe-0.9.5/setup.cfg
-drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-02-08 08:11:10.667554 pyswipe-0.9.5/tests/
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      541 2021-08-20 11:22:35.000000 pyswipe-0.9.5/tests/test_basic.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     4231 2021-08-20 11:22:35.000000 pyswipe-0.9.5/tests/test_mlt_utils.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     1042 2021-08-20 11:22:35.000000 pyswipe-0.9.5/tests/test_model_utils.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      804 2021-08-20 11:22:35.000000 pyswipe-0.9.5/tests/test_model_vector_to_txt.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     3653 2021-08-20 11:22:35.000000 pyswipe-0.9.5/tests/test_plot_utils.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     6350 2021-08-20 11:22:35.000000 pyswipe-0.9.5/tests/test_sh_utils.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    17380 2023-09-14 05:36:06.000000 pyswipe-0.9.5/tests/test_swipe.py
+drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-03 06:12:18.213415 pyswipe-0.9.6/
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       68 2024-03-04 09:30:57.000000 pyswipe-0.9.6/.coveragerc
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      136 2024-03-04 09:30:57.000000 pyswipe-0.9.6/.gitignore
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     1241 2024-03-04 09:30:57.000000 pyswipe-0.9.6/.travis.yml
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       59 2024-03-04 09:30:57.000000 pyswipe-0.9.6/CHANGELOG.rst
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      518 2024-03-04 09:30:57.000000 pyswipe-0.9.6/CITATION.cff
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      281 2024-03-04 09:30:57.000000 pyswipe-0.9.6/CITATION_old.cff
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     1072 2024-03-04 09:30:57.000000 pyswipe-0.9.6/LICENSE
+-rw-r--r--   0 spencerh  (1000) spencerh  (1000)     6588 2024-05-03 06:12:18.213415 pyswipe-0.9.6/PKG-INFO
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     4008 2024-04-10 07:18:07.000000 pyswipe-0.9.6/README.rst
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      189 2024-03-04 09:30:57.000000 pyswipe-0.9.6/TODO.md
+drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-03 06:12:18.197415 pyswipe-0.9.6/docs/
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      676 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/Makefile
+drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-03 06:12:18.197415 pyswipe-0.9.6/docs/source/
+drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-03 06:12:18.197415 pyswipe-0.9.6/docs/source/.templates/
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      157 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/source/.templates/layout.html
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       32 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/source/changelog.rst
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     6212 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/source/conf.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      476 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/source/index.rst
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      632 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/source/installation.rst
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     2874 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/source/model_coefficients.rst
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       29 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/source/readme.rst
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     1046 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/source/reference.rst
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8103 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/source/usage.rst
+drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-03 06:12:18.205415 pyswipe-0.9.6/docs/static/
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)  6334764 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/static/animation.gif
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       47 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/static/custom.css
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   220149 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/static/example_plot.png
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     1466 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyproject.toml
+drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-03 06:12:18.209415 pyswipe-0.9.6/pyswipe/
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      305 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/__init__.py
+drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-03 06:12:18.213415 pyswipe-0.9.6/pyswipe/coefficients/
+-rw-r--r--   0 spencerh  (1000) spencerh  (1000)   106628 2024-03-04 09:27:34.000000 pyswipe-0.9.6/pyswipe/coefficients/SW_OPER_EIO_SWI_2E_00000000T000000_99999999T999999_0101.txt
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      144 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/constants.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   310000 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/mlat_scalargrid.txt
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   300000 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/mlt_scalargrid.txt
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    13152 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/mlt_utils.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    10843 2024-05-03 05:57:04.000000 pyswipe-0.9.6/pyswipe/model_utils.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     4406 2024-05-03 06:02:49.000000 pyswipe-0.9.6/pyswipe/model_vector_to_txt.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    48412 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/plot_utils.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   312289 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/potential.txt
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    40562 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/sh_utils.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   158608 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/swipe.py
+drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-03 06:12:18.213415 pyswipe-0.9.6/pyswipe/tests/
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8557 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/tests/01__plot_cpcp_vs_hemi_bt_and_clockangle.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8061 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/tests/02__E_at_lowlatboundary.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    10936 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/tests/03__hi-c_cpcp_vs_other_studies.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     9022 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/tests/04__potential_dial_plots.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    11467 2024-05-03 06:05:31.000000 pyswipe-0.9.6/pyswipe/tests/04__potential_dial_plots__alternative_levels.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8162 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/tests/05__emwork_dial_plots.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     9136 2024-05-03 06:05:45.000000 pyswipe-0.9.6/pyswipe/tests/05__emwork_dial_plots__alternative_levels.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     9489 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/tests/06__plot_emwork_vs_hemi_bt_and_clockangle.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8325 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/tests/08__conductance_dial_plots__filledcell.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     4853 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/tests/09__dask_functions_for_large_input.py
+drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-03 06:12:18.213415 pyswipe-0.9.6/pyswipe.egg-info/
+-rw-r--r--   0 spencerh  (1000) spencerh  (1000)     6588 2024-05-03 06:12:18.000000 pyswipe-0.9.6/pyswipe.egg-info/PKG-INFO
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)     1641 2024-05-03 06:12:18.000000 pyswipe-0.9.6/pyswipe.egg-info/SOURCES.txt
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)        1 2024-05-03 06:12:18.000000 pyswipe-0.9.6/pyswipe.egg-info/dependency_links.txt
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)      156 2024-05-03 06:12:18.000000 pyswipe-0.9.6/pyswipe.egg-info/requires.txt
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)        8 2024-05-03 06:12:18.000000 pyswipe-0.9.6/pyswipe.egg-info/top_level.txt
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      106 2024-03-04 09:31:09.000000 pyswipe-0.9.6/requirements.txt
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       38 2024-05-03 06:12:18.217415 pyswipe-0.9.6/setup.cfg
+drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-03 06:12:18.213415 pyswipe-0.9.6/tests/
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)      541 2021-08-20 11:22:35.000000 pyswipe-0.9.6/tests/test_basic.py
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)     4231 2021-08-20 11:22:35.000000 pyswipe-0.9.6/tests/test_mlt_utils.py
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)     1042 2021-08-20 11:22:35.000000 pyswipe-0.9.6/tests/test_model_utils.py
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)      804 2021-08-20 11:22:35.000000 pyswipe-0.9.6/tests/test_model_vector_to_txt.py
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)     3653 2021-08-20 11:22:35.000000 pyswipe-0.9.6/tests/test_plot_utils.py
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)     6350 2021-08-20 11:22:35.000000 pyswipe-0.9.6/tests/test_sh_utils.py
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)    17380 2023-09-14 05:36:06.000000 pyswipe-0.9.6/tests/test_swipe.py
```

### Comparing `pyswipe-0.9.5/.travis.yml` & `pyswipe-0.9.6/.travis.yml`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/CITATION.cff` & `pyswipe-0.9.6/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/LICENSE` & `pyswipe-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/PKG-INFO` & `pyswipe-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyswipe
-Version: 0.9.5
+Version: 0.9.6
 Summary: Python implementation of the Swarm Ionospheric Polar Electrodynamics (Swipe) model
 Author: Karl M. Laundal
 Author-email: "Spencer M. Hatch" <spencer.hatch@ift.uib.no>
 Maintainer-email: "Spencer M. Hatch" <spencer.hatch@ift.uib.no>
 License: MIT License
         
         Copyright (c) 2023 Spencer M Hatch
@@ -79,15 +79,15 @@
 - electric potential (scalar)
 - electric field E (vector)
 - convection v = - cross(E, B) (vector)
 - height-integrated electromagnetic work = dot(J, E) (scalar) in the earth's rotating frame of reference, with J given by the AMPS model and E by Swarm Hi-C
 - Hall and Pedersen conductances (scalars)
 - Poynting flux (scalar)
 
-For questions and comments, please contact spencer.hatch at ift.uib.no
+For questions and comments, please contact spencer.hatch at uib.no
 
 Installation
 ------------
 
 Using pip::
 
     pip install pyswipe
```

### Comparing `pyswipe-0.9.5/README.rst` & `pyswipe-0.9.6/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 - electric potential (scalar)
 - electric field E (vector)
 - convection v = - cross(E, B) (vector)
 - height-integrated electromagnetic work = dot(J, E) (scalar) in the earth's rotating frame of reference, with J given by the AMPS model and E by Swarm Hi-C
 - Hall and Pedersen conductances (scalars)
 - Poynting flux (scalar)
 
-For questions and comments, please contact spencer.hatch at ift.uib.no
+For questions and comments, please contact spencer.hatch at uib.no
 
 Installation
 ------------
 
 Using pip::
 
     pip install pyswipe
```

### Comparing `pyswipe-0.9.5/docs/Makefile` & `pyswipe-0.9.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/docs/source/conf.py` & `pyswipe-0.9.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/docs/source/installation.rst` & `pyswipe-0.9.6/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/docs/source/model_coefficients.rst` & `pyswipe-0.9.6/docs/source/model_coefficients.rst`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/docs/source/reference.rst` & `pyswipe-0.9.6/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/docs/source/usage.rst` & `pyswipe-0.9.6/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/docs/static/animation.gif` & `pyswipe-0.9.6/docs/static/animation.gif`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/docs/static/example_plot.png` & `pyswipe-0.9.6/docs/static/example_plot.png`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/pyproject.toml` & `pyswipe-0.9.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/pyswipe/coefficients/SW_OPER_MIO_SWI_2E_00000000T000000_99999999T999999_0101.txt` & `pyswipe-0.9.6/pyswipe/coefficients/SW_OPER_EIO_SWI_2E_00000000T000000_99999999T999999_0101.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Spherical harmonic coefficients for the Swarm HEmispherically resolved Ionospheric Convection (SHEIC) model
 # Produced 19 July 2023
 #
 # Based on Swarm convection measurements made between 2013-12 to 2020.
-# Reference: Laundal et al., "Solar wind and seasonal influence on ionospheric currents", Journal of Geophysical Research - Space Physics, doi:10.1029/2018JA025387, 2018
+# Reference: Hatch, S. M., Vanhamäki, H., Laundal, K. M., Reistad, J. P., Burchill, J., Lomidze, L., Knudsen, D., Madelaire, M., & Tesfaw, H. (2023). Does high-latitude ionospheric electrodynamics exhibit hemispheric mirror symmetry? EGUsphere, 2023, 1–41. https://doi.org/10.5194/egusphere-2023-2920
 #
 # Coefficient unit: mV/m
 # Apex reference height: 110 km
 # Earth radius: 6371.2 km
 #
 # Spherical harmonic degree, order: 65, 3 (for T)
 #
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyswipe-0.9.5/pyswipe/mlat_scalargrid.txt` & `pyswipe-0.9.6/pyswipe/mlat_scalargrid.txt`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/pyswipe/mlt_scalargrid.txt` & `pyswipe-0.9.6/pyswipe/mlt_scalargrid.txt`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/pyswipe/mlt_utils.py` & `pyswipe-0.9.6/pyswipe/mlt_utils.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/pyswipe/model_utils.py` & `pyswipe-0.9.6/pyswipe/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from functools import reduce
 from .sh_utils import get_A_matrix__Ephizero, get_A_matrix__potzero, SHkeys
 from .constants import REFRE,d2r
 
 basepath = os.path.dirname(__file__)
 # basepath = '/SPENCEdata/Research/database/SHEIC/matrices/10k_points/'
 
-default_coeff_fn = os.path.abspath(os.path.join(basepath,'coefficients','SW_OPER_MIO_SWI_2E_00000000T000000_99999999T999999_0101.txt'))
+default_coeff_fn = os.path.abspath(os.path.join(basepath,'coefficients','SW_OPER_EIO_SWI_2E_00000000T000000_99999999T999999_0101.txt'))
 
 # read coefficient file and store in pandas DataFrame - with column names from last row of header:
 colnames = ([x for x in open(default_coeff_fn).readlines() if x.startswith('#')][-1][1:]).strip().split(' ') 
 
 get_coeffs = lambda fn: pd.read_table(fn, skipinitialspace = True, comment = '#', sep = ' ', names = colnames, index_col = [0, 1])
```

### Comparing `pyswipe-0.9.5/pyswipe/plot_utils.py` & `pyswipe-0.9.6/pyswipe/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/pyswipe/potential.txt` & `pyswipe-0.9.6/pyswipe/potential.txt`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/pyswipe/sh_utils.py` & `pyswipe-0.9.6/pyswipe/sh_utils.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/pyswipe/swipe.py` & `pyswipe-0.9.6/pyswipe/swipe.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/pyswipe/tests/01__plot_cpcp_vs_hemi_bt_and_clockangle.py` & `pyswipe-0.9.6/pyswipe/tests/01__plot_cpcp_vs_hemi_bt_and_clockangle.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/pyswipe/tests/02__E_at_lowlatboundary.py` & `pyswipe-0.9.6/pyswipe/tests/02__E_at_lowlatboundary.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/pyswipe/tests/03__hi-c_cpcp_vs_other_studies.py` & `pyswipe-0.9.6/pyswipe/tests/03__hi-c_cpcp_vs_other_studies.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/pyswipe/tests/04__potential_dial_plots.py` & `pyswipe-0.9.6/pyswipe/tests/04__potential_dial_plots.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/pyswipe/tests/04__potential_dial_plots__alternative_levels.py` & `pyswipe-0.9.6/pyswipe/tests/04__potential_dial_plots__alternative_levels.py`

 * *Files 3% similar despite different names*

```diff
@@ -186,19 +186,22 @@
             dlevel = np.diff(tmplevels)[0]
             print(i,j,_ca,dlevel)
             tmplevels = tmplevels[:-1]+np.diff(tmplevels)[0]/2
             tmplevels = np.concatenate([[potmin], tmplevels ,[potmax]])
 
 
             axes[i][j].contourf(mlat_n, mlt_n, phin, levels = tmplevels, cmap = plt.cm.bwr, extend = 'both')
+
+            topleftstring = r"$\Delta$cont" + f" = {dlevel:.1f} kV"
+
             if not no_SH:
                 axes[i][j].contour (mlat_s, mlt_s, phis, levels = tmplevels, colors = 'k' , extend = 'both', linewidths = .4)
 
                 # showstring = f'$\Delta \Phi_N=$ {dPhiN:.1f}' + f' kV\n$\Delta \Phi_S=$ {dPhiS:.1f}' + f' kV\n$\Delta \Phi_N/\Delta \Phi_S=$ {dPhiN/dPhiS:.2f}'
-                showstring = f'$\Delta \Phi_N=$ {dPhiN:.0f}' + f' kV\n$\Delta \Phi_S=$ {dPhiS:.0f}' + f' kV\n$\Delta \Phi_N/\Delta \Phi_S=$ {dPhiN/dPhiS:.2f}'
+                showstring = f'$\Delta \Phi_N=$ {dPhiN:.0f}' + f' kV\n$\Delta \Phi_S=$ {dPhiS:.0f}' + f' kV\n$\Delta \Phi_N/\Delta \Phi_S=$ {dPhiN/dPhiS:.1f}'
 
             else:
 
                 showstring = f'$\Delta \Phi_N=$ {dPhiN:.0f} kV'
 
             if doCalcBhattacharyya:
                 # Separate into pos and neg current distributions
@@ -225,14 +228,19 @@
 
                 showstring += "\n"+r"$BC = $"+f"{facBhatcoeff:.2f}"
 
             axes[i][j].write(55, 10.2, showstring,
                              ha = 'left', va = 'top', size = 9, multialignment='left')
                 #axes[i][j].write(60, 10, '$\Delta+' + '{:.2f}'.format(psi.max()) + '\mu$A/m$^2$\n $\\nabla' + '{:.2f}'.format(psi.min()) + ' \mu$A/m$^2$', ha = 'left', va = 'bottom', size = 9, multialignment='left')
 
+            axes[i][j].write(55, 13.8, topleftstring,
+                             ha = 'center', va = 'top', size = 9,
+                             multialignment='center',
+                             ignore_plot_limits=True)
+
             # facdat = {'north_up':j_up_n, 'south_up':j_up_s,
             #           'north_down':j_down_n, 'south_down':j_down_s,
             #           'north_total':np.abs(j_up_n)+np.abs(j_down_n),
             #           'south_total':np.abs(j_up_s)+np.abs(j_down_s),
             #           'ca':_ca,'tilt':tilt,
             #           'By':By,
             #           'Bz':Bz}
```

### Comparing `pyswipe-0.9.5/pyswipe/tests/05__emwork_dial_plots.py` & `pyswipe-0.9.6/pyswipe/tests/05__emwork_dial_plots.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/pyswipe/tests/05__emwork_dial_plots__alternative_levels.py` & `pyswipe-0.9.6/pyswipe/tests/05__emwork_dial_plots__alternative_levels.py`

 * *Files 3% similar despite different names*

```diff
@@ -170,24 +170,26 @@
             # tmplocs.append([mins,maxs])
 
             tmpMAX = np.max(np.abs(np.array([phin.max(),phis.max()])))
             assert tmpMAX < potmax
 
             tmplevels = np.linspace(-tmpMAX,tmpMAX,Ncontour)
             dlevel = np.diff(tmplevels)[0]
-            print(i,j,_ca,dlevel)
+            print(i,j,_ca,dlevel,np.mean(phin),np.median(phin),np.mean(phis),np.median(phis))
             tmplevels = tmplevels[:-1]+np.diff(tmplevels)[0]/2
             tmplevels = np.concatenate([[potmin], tmplevels ,[potmax]])
 
             contn = axes[i][j].contourf(mlat_n, mlt_n, phin, levels = tmplevels, cmap = cmap, extend = extend)
 
+            topleftstring = r"$\Delta$cont" + f" = {dlevel:.1f} mW/m$^2$"
+
             if not no_SH:
                 conts = axes[i][j].contour (mlat_s, mlt_s, phis, levels = tmplevels, colors = 'k' , extend = extend, linewidths = .4)
 
-                showstring = f'$W_N=$ {dPhiN:.0f}' + f' GW\n$W_S=$ {dPhiS:.0f}' + f' GW\n$W_N/W_S=$ {dPhiN/dPhiS:.2f}'
+                showstring = f'$W_N=$ {dPhiN:.0f}' + f' GW\n$W_S=$ {dPhiS:.0f}' + f' GW\n$W_N/W_S=$ {dPhiN/dPhiS:.1f}'
 
             else:
                 
                 showstring = f'$W_N=$ {dPhiN:.0f} GW'
 
 
             if doCalcBhattacharyya:
@@ -217,14 +219,19 @@
 
             axes[i][j].write(60, 10.2, showstring,
                              ha = 'left', va = 'top', size = 9,
                              multialignment='left',
                              ignore_plot_limits=True)
 
 
+            axes[i][j].write(60, 13.8, topleftstring,
+                             ha = 'center', va = 'top', size = 9,
+                             multialignment='center',
+                             ignore_plot_limits=True)
+
     axdial.text(0, 0, r"$\mathbf{J}\cdot\mathbf{E}$ work"+u'\n(Earth-fixed frame)', ha = 'center', va = 'center', size = 14)
 
     plt.subplots_adjust(hspace = .01, wspace = .01, left = .01, right = .99, bottom = .05, top = .99)
 
     axdial.set_xlim(-1.2, 1.2)
     axdial.set_ylim(-1.2, 1.2)
 
@@ -253,11 +260,11 @@
         tiltstr = f"p{tilt}"
     else:
         tiltstr = f"n{np.abs(tilt)}"
     if no_SH:
         figname = plotdir+'swipe_emwork_ns_comparison_' + tiltstr + f'_deg_tilt_noSH__{Ncontour}contours.png'
     else:
         figname = plotdir+'swipe_emwork_ns_comparison_' + tiltstr + f'_deg_tilt__{Ncontour}contours.png'
-    plt.savefig(figname, dpi = 300)
+    # plt.savefig(figname, dpi = 300)
 
 print("Save data ...")
 plt.show()
```

### Comparing `pyswipe-0.9.5/pyswipe/tests/06__plot_emwork_vs_hemi_bt_and_clockangle.py` & `pyswipe-0.9.6/pyswipe/tests/06__plot_emwork_vs_hemi_bt_and_clockangle.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/pyswipe/tests/08__conductance_dial_plots__filledcell.py` & `pyswipe-0.9.6/pyswipe/tests/08__conductance_dial_plots__filledcell.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/pyswipe/tests/09__dask_functions_for_large_input.py` & `pyswipe-0.9.6/pyswipe/tests/09__dask_functions_for_large_input.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/pyswipe.egg-info/PKG-INFO` & `pyswipe-0.9.6/pyswipe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyswipe
-Version: 0.9.5
+Version: 0.9.6
 Summary: Python implementation of the Swarm Ionospheric Polar Electrodynamics (Swipe) model
 Author: Karl M. Laundal
 Author-email: "Spencer M. Hatch" <spencer.hatch@ift.uib.no>
 Maintainer-email: "Spencer M. Hatch" <spencer.hatch@ift.uib.no>
 License: MIT License
         
         Copyright (c) 2023 Spencer M Hatch
@@ -79,15 +79,15 @@
 - electric potential (scalar)
 - electric field E (vector)
 - convection v = - cross(E, B) (vector)
 - height-integrated electromagnetic work = dot(J, E) (scalar) in the earth's rotating frame of reference, with J given by the AMPS model and E by Swarm Hi-C
 - Hall and Pedersen conductances (scalars)
 - Poynting flux (scalar)
 
-For questions and comments, please contact spencer.hatch at ift.uib.no
+For questions and comments, please contact spencer.hatch at uib.no
 
 Installation
 ------------
 
 Using pip::
 
     pip install pyswipe
```

### Comparing `pyswipe-0.9.5/pyswipe.egg-info/SOURCES.txt` & `pyswipe-0.9.6/pyswipe.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 pyswipe/sh_utils.py
 pyswipe/swipe.py
 pyswipe.egg-info/PKG-INFO
 pyswipe.egg-info/SOURCES.txt
 pyswipe.egg-info/dependency_links.txt
 pyswipe.egg-info/requires.txt
 pyswipe.egg-info/top_level.txt
-pyswipe/coefficients/SW_OPER_MIO_SWI_2E_00000000T000000_99999999T999999_0101.txt
+pyswipe/coefficients/SW_OPER_EIO_SWI_2E_00000000T000000_99999999T999999_0101.txt
 pyswipe/tests/01__plot_cpcp_vs_hemi_bt_and_clockangle.py
 pyswipe/tests/02__E_at_lowlatboundary.py
 pyswipe/tests/03__hi-c_cpcp_vs_other_studies.py
 pyswipe/tests/04__potential_dial_plots.py
 pyswipe/tests/04__potential_dial_plots__alternative_levels.py
 pyswipe/tests/05__emwork_dial_plots.py
 pyswipe/tests/05__emwork_dial_plots__alternative_levels.py
```

### Comparing `pyswipe-0.9.5/tests/test_basic.py` & `pyswipe-0.9.6/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/tests/test_mlt_utils.py` & `pyswipe-0.9.6/tests/test_mlt_utils.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/tests/test_model_utils.py` & `pyswipe-0.9.6/tests/test_model_utils.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/tests/test_model_vector_to_txt.py` & `pyswipe-0.9.6/tests/test_model_vector_to_txt.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/tests/test_plot_utils.py` & `pyswipe-0.9.6/tests/test_plot_utils.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/tests/test_sh_utils.py` & `pyswipe-0.9.6/tests/test_sh_utils.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.5/tests/test_swipe.py` & `pyswipe-0.9.6/tests/test_swipe.py`

 * *Files identical despite different names*


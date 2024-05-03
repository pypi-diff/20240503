# Comparing `tmp/fstd2nc-0.20240401.0.tar.gz` & `tmp/fstd2nc-0.20240401.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fstd2nc-0.20240401.0.tar", last modified: Wed Apr  3 16:45:21 2024, max compression
+gzip compressed data, was "dist/fstd2nc-0.20240401.1.tar", last modified: Fri May  3 19:28:39 2024, max compression
```

## Comparing `fstd2nc-0.20240401.0.tar` & `fstd2nc-0.20240401.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.169491 fstd2nc-0.20240401.0/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1809 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/.gitignore
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    35147 2022-04-13 02:52:23.000000 fstd2nc-0.20240401.0/COPYING
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7651 2022-04-13 02:52:23.000000 fstd2nc-0.20240401.0/COPYING.LESSER
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    29844 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/Changelog
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      114 2024-03-25 14:07:01.000000 fstd2nc-0.20240401.0/Makefile
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14236 2024-04-03 16:45:21.169094 fstd2nc-0.20240401.0/PKG-INFO
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13489 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/README.md
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14775 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/README_fr.md
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.033633 fstd2nc-0.20240401.0/cccbuffer/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      777 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.0/cccbuffer/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      182 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.0/cccbuffer/__main__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1022 2024-03-27 16:22:27.000000 fstd2nc-0.20240401.0/cccbuffer/_xarray_hook.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      149 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.0/cccbuffer/cccdump.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.035944 fstd2nc-0.20240401.0/cccbuffer/mixins/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        0 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.0/cccbuffer/mixins/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3913 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.0/cccbuffer/mixins/ccc.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1193 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.0/cccbuffer/mixins/char.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2289 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.0/cccbuffer/mixins/grid.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4359 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.0/cccbuffer/mixins/levels.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3047 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.0/cccbuffer/mixins/superlabels.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6112 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.0/cccbuffer/mixins/times.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.037112 fstd2nc-0.20240401.0/conda.recipe/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      658 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/conda.recipe/README.md
--rwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)       67 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/conda.recipe/build.sh
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      512 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/conda.recipe/meta.yaml
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.079387 fstd2nc-0.20240401.0/debian/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      143 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/debian/changelog
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        2 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/debian/compat
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      624 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/debian/control
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1103 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/debian/copyright
--rwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)      607 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/debian/rules
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.079746 fstd2nc-0.20240401.0/debian/source/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       12 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/debian/source/format
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.081146 fstd2nc-0.20240401.0/fstd2nc/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3833 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     9889 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/__main__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7146 2024-03-27 16:22:57.000000 fstd2nc-0.20240401.0/fstd2nc/_xarray_hook.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20044 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/extra.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.083519 fstd2nc-0.20240401.0/fstd2nc/locale/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1526 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/fstd2nc/locale/Makefile
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      974 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/fstd2nc/locale/README.md
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.028507 fstd2nc-0.20240401.0/fstd2nc/locale/fr_CA/
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.083893 fstd2nc-0.20240401.0/fstd2nc/locale/fr_CA/LC_MESSAGES/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    25691 2024-04-03 16:44:59.000000 fstd2nc-0.20240401.0/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    27563 2024-04-03 16:44:59.000000 fstd2nc-0.20240401.0/fstd2nc/locale/fr_CA.po
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.168632 fstd2nc-0.20240401.0/fstd2nc/mixins/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    42803 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6457 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/accum.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1871 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/ascii.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20498 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/compat.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    11830 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/dates.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3138 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/diaghacks.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3220 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/ensembles.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    34534 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/extern.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3581 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/filter.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    12004 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/fstd.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    23130 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/gridhacks.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     8248 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/masks.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4249 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/mesh.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1786 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/misc.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20973 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/netcdf.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1735 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/pruneaxes.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4790 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/removestuff.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2610 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/select.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    23171 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/series.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     8075 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/sfc_codes.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     8783 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/vardict.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    41836 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/vcoords.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3058 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/xmeta.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    61231 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/xycoords.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2583 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/stdout.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.082876 fstd2nc-0.20240401.0/fstd2nc.egg-info/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14236 2024-04-03 16:45:20.000000 fstd2nc-0.20240401.0/fstd2nc.egg-info/PKG-INFO
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1578 2024-04-03 16:45:20.000000 fstd2nc-0.20240401.0/fstd2nc.egg-info/SOURCES.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        1 2024-04-03 16:45:20.000000 fstd2nc-0.20240401.0/fstd2nc.egg-info/dependency_links.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      289 2024-04-03 16:45:20.000000 fstd2nc-0.20240401.0/fstd2nc.egg-info/entry_points.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      218 2024-04-03 16:45:20.000000 fstd2nc-0.20240401.0/fstd2nc.egg-info/requires.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       18 2024-04-03 16:45:20.000000 fstd2nc-0.20240401.0/fstd2nc.egg-info/top_level.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       59 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/pyproject.toml
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1370 2022-04-13 02:52:23.000000 fstd2nc-0.20240401.0/sample_meta.ini
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       38 2024-04-03 16:45:21.169656 fstd2nc-0.20240401.0/setup.cfg
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2664 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/setup.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.373991 fstd2nc-0.20240401.1/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1809 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/.gitignore
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    35147 2022-04-13 02:52:23.000000 fstd2nc-0.20240401.1/COPYING
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7651 2022-04-13 02:52:23.000000 fstd2nc-0.20240401.1/COPYING.LESSER
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    30270 2024-05-03 18:40:05.000000 fstd2nc-0.20240401.1/Changelog
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      114 2024-03-25 14:07:01.000000 fstd2nc-0.20240401.1/Makefile
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14236 2024-05-03 19:28:39.373629 fstd2nc-0.20240401.1/PKG-INFO
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13489 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/README.md
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14775 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/README_fr.md
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.092862 fstd2nc-0.20240401.1/cccbuffer/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      777 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.1/cccbuffer/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      182 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.1/cccbuffer/__main__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1022 2024-03-27 16:22:27.000000 fstd2nc-0.20240401.1/cccbuffer/_xarray_hook.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      149 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.1/cccbuffer/cccdump.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.095437 fstd2nc-0.20240401.1/cccbuffer/mixins/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        0 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.1/cccbuffer/mixins/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4101 2024-05-03 18:40:05.000000 fstd2nc-0.20240401.1/cccbuffer/mixins/ccc.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1193 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.1/cccbuffer/mixins/char.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2289 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.1/cccbuffer/mixins/grid.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4359 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.1/cccbuffer/mixins/levels.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3047 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.1/cccbuffer/mixins/superlabels.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6112 2024-04-23 18:55:54.000000 fstd2nc-0.20240401.1/cccbuffer/mixins/times.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.096648 fstd2nc-0.20240401.1/conda.recipe/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      658 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/conda.recipe/README.md
+-rwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)       67 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/conda.recipe/build.sh
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      512 2024-05-03 18:40:05.000000 fstd2nc-0.20240401.1/conda.recipe/meta.yaml
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.185379 fstd2nc-0.20240401.1/debian/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      143 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/debian/changelog
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        2 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/debian/compat
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      624 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/debian/control
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1103 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/debian/copyright
+-rwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)      607 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/debian/rules
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.185905 fstd2nc-0.20240401.1/debian/source/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       12 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/debian/source/format
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.187446 fstd2nc-0.20240401.1/fstd2nc/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3833 2024-05-03 18:40:05.000000 fstd2nc-0.20240401.1/fstd2nc/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     9889 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/__main__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7537 2024-05-03 18:40:05.000000 fstd2nc-0.20240401.1/fstd2nc/_xarray_hook.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    21835 2024-05-03 18:40:05.000000 fstd2nc-0.20240401.1/fstd2nc/extra.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.189999 fstd2nc-0.20240401.1/fstd2nc/locale/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1526 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/fstd2nc/locale/Makefile
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      974 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/fstd2nc/locale/README.md
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.043405 fstd2nc-0.20240401.1/fstd2nc/locale/fr_CA/
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.190428 fstd2nc-0.20240401.1/fstd2nc/locale/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    25609 2024-05-03 19:26:40.000000 fstd2nc-0.20240401.1/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    27563 2024-05-03 19:27:20.000000 fstd2nc-0.20240401.1/fstd2nc/locale/fr_CA.po
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.373067 fstd2nc-0.20240401.1/fstd2nc/mixins/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    42803 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6457 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/accum.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1871 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/ascii.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20498 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/compat.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    11830 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/dates.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3138 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/diaghacks.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3220 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/ensembles.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    34534 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/extern.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3581 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/filter.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    12004 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/fstd.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    23129 2024-05-03 18:43:18.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/gridhacks.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     8248 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/masks.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4249 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/mesh.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1786 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/misc.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20973 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/netcdf.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1735 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/pruneaxes.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4790 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/removestuff.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2610 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/select.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    23171 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/series.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     8075 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/sfc_codes.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     8783 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/vardict.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    41836 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/vcoords.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3499 2024-05-03 18:40:05.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/xmeta.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    61231 2024-04-19 14:45:18.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/xycoords.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2583 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/fstd2nc/stdout.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.189068 fstd2nc-0.20240401.1/fstd2nc.egg-info/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14236 2024-05-03 19:28:38.000000 fstd2nc-0.20240401.1/fstd2nc.egg-info/PKG-INFO
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1578 2024-05-03 19:28:38.000000 fstd2nc-0.20240401.1/fstd2nc.egg-info/SOURCES.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        1 2024-05-03 19:28:38.000000 fstd2nc-0.20240401.1/fstd2nc.egg-info/dependency_links.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      289 2024-05-03 19:28:38.000000 fstd2nc-0.20240401.1/fstd2nc.egg-info/entry_points.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      218 2024-05-03 19:28:38.000000 fstd2nc-0.20240401.1/fstd2nc.egg-info/requires.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       18 2024-05-03 19:28:38.000000 fstd2nc-0.20240401.1/fstd2nc.egg-info/top_level.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       59 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/pyproject.toml
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1370 2022-04-13 02:52:23.000000 fstd2nc-0.20240401.1/sample_meta.ini
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       38 2024-05-03 19:28:39.374068 fstd2nc-0.20240401.1/setup.cfg
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2664 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/setup.py
```

### Comparing `fstd2nc-0.20240401.0/.gitignore` & `fstd2nc-0.20240401.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/COPYING` & `fstd2nc-0.20240401.1/COPYING`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/COPYING.LESSER` & `fstd2nc-0.20240401.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/Changelog` & `fstd2nc-0.20240401.1/Changelog`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,17 @@
-Version 0.20240401.0 (Apr 3, 2023)
+Version 0.20240401.1 (May 3, 2024)
+	* Fixed crash when importing fstd2nc.extra without having rpnpy or
+	  librmn in the environment.
+	* Some fixes for RSF support.  Detect more recent variants of header
+	  structures (e.g. for librmn 20.1.0-alpha3 snapshot).
+	* Fixed missing auto-detect for RSF in xarray interface.
+	* Fixed address overflow issue with CCC file interface, which was
+	  giving missing data for larger files.
+
+Version 0.20240401.0 (Apr 3, 2024)
 	* Some support for new RSF file container and fst24 data format.
 	* Fixed bug in fstpy bridge - nk no longer stored in Buffer.
 	* Fixed check for operational dictionary when opdict=True is used in
 	  Python interface.
 	* Added _CRS attribute to xarray interface.
 	* Fixed bug when using dask distributed - the keys were not integers,
 	  but rather numpy integers, which apparently was a problem.
```

### Comparing `fstd2nc-0.20240401.0/PKG-INFO` & `fstd2nc-0.20240401.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstd2nc
-Version: 0.20240401.0
+Version: 0.20240401.1
 Summary: Converts RPN standard files (from Environment Canada) to netCDF files.
 Home-page: https://github.com/neishm/fstd2nc
 Author: Mike Neish
 License: LGPL-3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `fstd2nc-0.20240401.0/README.md` & `fstd2nc-0.20240401.1/README.md`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/README_fr.md` & `fstd2nc-0.20240401.1/README_fr.md`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/cccbuffer/__init__.py` & `fstd2nc-0.20240401.1/cccbuffer/__init__.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/cccbuffer/_xarray_hook.py` & `fstd2nc-0.20240401.1/cccbuffer/_xarray_hook.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/cccbuffer/mixins/ccc.py` & `fstd2nc-0.20240401.1/cccbuffer/mixins/ccc.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,22 +35,25 @@
     # Read raw headers, and keep track of indices.
     # First record already read from above.
     raw = [magic]
     while len(raw[-1]) > 0:
       f.seek(raw[-1][-1]+4,1)
       raw.append(np.fromfile(f,'>i4',19))
     raw.pop()
-    raw = np.array(raw,'>i4')
-    # Hijack part of the raw buffer to include the addresses.
+    final = np.empty((len(raw),22),dtype='>u4')
+    final[:,:-3] = np.array(raw,'u4')
+    final[:,-3] = 0  # padding to align 64-bit address below.
+    # Encode the address information (not in file, have to compute here).
+    address = final.view('>i8')[:,-1]
     # First, fill with the lengths of each record (plus header)
-    raw[0,-2] = 0
-    raw[1:,-2] = raw[:-1,-1] + 80
+    address[0] = 0
+    address[1:] = final[:-1,-4] + 80
     # Then, addresses are the cumulative sum of these lengths.
-    raw[:,-2] = np.cumsum(raw[:,-2])
-    return raw.view('B')
+    address[:] = np.cumsum(address[:])
+    return final.view('B')
 
   # This method will take the collection of raw headers and decode them
   # into their final fields.  Result is stored internally in the _headers
   # attribute, which is a dictionary of 1D arrays (of size nrecs).
   @staticmethod
   def _decode_headers (raw):
     import numpy as np
@@ -64,17 +67,17 @@
     out['name'] = np.array(headers_str[:,2])
     out['level'] = np.array(headers_int[:,3],'uint64').view('int64')
     out['ilg'] = np.array(headers_int[:,4],'uint64')
     out['ilat'] = np.array(headers_int[:,5],'uint64')
     out['khem'] = np.array(headers_int[:,6],'uint64')
     out['pack'] = np.array(headers_int[:,7],'uint64')
     # Extra info (raw data length and position in file)
-    length = raw[:,-1] + 80
+    length = raw[:,-4] + 80
     out['length'] = np.array(length,'uint32')
-    out['address'] = np.array(raw[:,-2],'uint64')
+    out['address'] = np.array(raw.view('>u8')[:,-1],'uint64')
     out['dtype'] = np.array([np.float32]*len(raw))
     return out
 
   # This method takes a raw *data* record, and decodes it into the final
   # array of values.  Uses the 'address' and 'length' entries from _headers to
   # determine the location and length of each raw data record.
   # This method is called from the xarray interface, and to_netcdf().
```

### Comparing `fstd2nc-0.20240401.0/cccbuffer/mixins/char.py` & `fstd2nc-0.20240401.1/cccbuffer/mixins/char.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/cccbuffer/mixins/grid.py` & `fstd2nc-0.20240401.1/cccbuffer/mixins/grid.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/cccbuffer/mixins/levels.py` & `fstd2nc-0.20240401.1/cccbuffer/mixins/levels.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/cccbuffer/mixins/superlabels.py` & `fstd2nc-0.20240401.1/cccbuffer/mixins/superlabels.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/cccbuffer/mixins/times.py` & `fstd2nc-0.20240401.1/cccbuffer/mixins/times.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/conda.recipe/README.md` & `fstd2nc-0.20240401.1/conda.recipe/README.md`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/conda.recipe/meta.yaml` & `fstd2nc-0.20240401.1/conda.recipe/meta.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 package:
   name: fstd2nc
-  version: 0.20240401.0
+  version: 0.20240401.1
 
 
 requirements:
   build:
     - python
     - numpy  >1.15.3
     - netcdf4
```

### Comparing `fstd2nc-0.20240401.0/debian/control` & `fstd2nc-0.20240401.1/debian/control`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/debian/copyright` & `fstd2nc-0.20240401.1/debian/copyright`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/debian/rules` & `fstd2nc-0.20240401.1/debian/rules`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/__init__.py` & `fstd2nc-0.20240401.1/fstd2nc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ###############################################################################
 
 
 """
 Functionality for converting between FSTD and netCDF files.
 """
 
-__version__ = "0.20240401.0"
+__version__ = "0.20240401.1"
 
 
 # Check for bundled rpnpy package.
 # Fall back to this one if no standard rpnpy package available.
 try:
   # Importing the module will set up the appropriate search paths.
   import fstd2nc_deps
```

### Comparing `fstd2nc-0.20240401.0/fstd2nc/__main__.py` & `fstd2nc-0.20240401.1/fstd2nc/__main__.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/_xarray_hook.py` & `fstd2nc-0.20240401.1/fstd2nc/_xarray_hook.py`

 * *Files 9% similar despite different names*

```diff
@@ -155,16 +155,27 @@
     from fstd2nc.mixins import _expand_files
     try:
       infiles = _expand_files(filename_or_obj)
       infiles = list(zip(*infiles))[1]
       if len(infiles) == 0: return False
       # Check first matching file.
       with open(infiles[0],'rb') as f:
-        magic = f.read(16)
-      return len(magic) >= 16 and magic[12:] == b'STDR'
+        magic = f.read(24)
+      # fstd98 in XDF container
+      if len(magic) >= 16 and magic[12:] == b'STDR':
+        return True
+      # fst24 in RSF container (pre-release version?)
+      elif len(magic) >= 24 and magic[16:24] == b'RSF0STDR':
+        return True
+      # fst24 in RSF container
+      elif len(magic) >= 24 and magic[16:24] == b'RSF0STDF':
+        return True
+      # unrecognized file type, not supported in this engine.
+      else:
+        return False
     except Exception:
       # If something unexpected happened, then assume it's not a valid FST file.
       return False
 
 # Add a "to_fstd" shortcut to Dataset objects.
 import xarray as xr
 @xr.register_dataset_accessor("to_fstd")
```

### Comparing `fstd2nc-0.20240401.0/fstd2nc/extra.py` & `fstd2nc-0.20240401.1/fstd2nc/extra.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,34 +21,82 @@
 """
 Optional helper functions.
 These functions provide information about the FST files using alternative
 approaches (not the standard librmn/rpnpy functions).
 This is solely for performance considerations.
 """
 
-from rpnpy.librmn import librmn
-import ctypes as ct
-import numpy as np
-import numpy.ctypeslib as npc
-librmn.compact_float.argtypes = (npc.ndpointer(dtype='int32'), npc.ndpointer(dtype='int32'), npc.ndpointer(dtype='int32'), ct.c_int, ct.c_int, ct.c_int, ct.c_int, ct.c_int, ct.c_int, ct.POINTER(ct.c_double))
-librmn.compact_double.argtypes = (npc.ndpointer(dtype='int32'), npc.ndpointer(dtype='int32'), npc.ndpointer(dtype='int32'), ct.c_int, ct.c_int, ct.c_int, ct.c_int, ct.c_int, ct.c_int, ct.POINTER(ct.c_double))
-librmn.compact_integer.argtypes = (npc.ndpointer(dtype='int32'), ct.c_void_p, npc.ndpointer(dtype='int32'), ct.c_int, ct.c_int, ct.c_int, ct.c_int, ct.c_int)
-librmn.ieeepak_.argtypes = (npc.ndpointer(dtype='int32'), npc.ndpointer(dtype='int32'), ct.POINTER(ct.c_int), ct.POINTER(ct.c_int), ct.POINTER(ct.c_int), ct.POINTER(ct.c_int), ct.POINTER(ct.c_int))
-librmn.compact_char.argtypes = (npc.ndpointer(dtype='int32'), ct.c_void_p, npc.ndpointer(dtype='int32'), ct.c_int, ct.c_int, ct.c_int, ct.c_int, ct.c_int)
-librmn.c_armn_uncompress32.argtypes = (npc.ndpointer(dtype='int32'), npc.ndpointer(dtype='int32'), ct.c_int, ct.c_int, ct.c_int, ct.c_int)
-# API for armn_compress was updated after version 20 to include an extra
-# "swap_stream" integer flag.
 try:
-  librmn.c_armn_compress_setswap.argtypes = (ct.c_int,)
-  librmn.armn_compress.argtypes = (npc.ndpointer(dtype='int32'),ct.c_int,ct.c_int,ct.c_int,ct.c_int,ct.c_int)
-  _api_version = 20
-except AttributeError:
-  librmn.armn_compress.argtypes = (npc.ndpointer(dtype='int32'),ct.c_int,ct.c_int,ct.c_int,ct.c_int,ct.c_int,ct.c_int)
-  _api_version = 21
-librmn.c_float_unpacker.argtypes = (npc.ndpointer(dtype='int32'),npc.ndpointer(dtype='int32'),npc.ndpointer(dtype='int32'),ct.c_int,ct.POINTER(ct.c_int))
+  from rpnpy.librmn import librmn
+  import ctypes as ct
+  import numpy as np
+  import numpy.ctypeslib as npc
+  librmn.compact_float.argtypes = (npc.ndpointer(dtype='int32'), npc.ndpointer(dtype='int32'), npc.ndpointer(dtype='int32'), ct.c_int, ct.c_int, ct.c_int, ct.c_int, ct.c_int, ct.c_int, ct.POINTER(ct.c_double))
+  librmn.compact_double.argtypes = (npc.ndpointer(dtype='int32'), npc.ndpointer(dtype='int32'), npc.ndpointer(dtype='int32'), ct.c_int, ct.c_int, ct.c_int, ct.c_int, ct.c_int, ct.c_int, ct.POINTER(ct.c_double))
+  librmn.compact_integer.argtypes = (npc.ndpointer(dtype='int32'), ct.c_void_p, npc.ndpointer(dtype='int32'), ct.c_int, ct.c_int, ct.c_int, ct.c_int, ct.c_int)
+  librmn.ieeepak_.argtypes = (npc.ndpointer(dtype='int32'), npc.ndpointer(dtype='int32'), ct.POINTER(ct.c_int), ct.POINTER(ct.c_int), ct.POINTER(ct.c_int), ct.POINTER(ct.c_int), ct.POINTER(ct.c_int))
+  librmn.compact_char.argtypes = (npc.ndpointer(dtype='int32'), ct.c_void_p, npc.ndpointer(dtype='int32'), ct.c_int, ct.c_int, ct.c_int, ct.c_int, ct.c_int)
+  librmn.c_armn_uncompress32.argtypes = (npc.ndpointer(dtype='int32'), npc.ndpointer(dtype='int32'), ct.c_int, ct.c_int, ct.c_int, ct.c_int)
+  # API for armn_compress was updated after version 20 to include an extra
+  # "swap_stream" integer flag.
+  try:
+    librmn.c_armn_compress_setswap.argtypes = (ct.c_int,)
+    librmn.armn_compress.argtypes = (npc.ndpointer(dtype='int32'),ct.c_int,ct.c_int,ct.c_int,ct.c_int,ct.c_int)
+    _api_version = 20
+  except AttributeError:
+    librmn.armn_compress.argtypes = (npc.ndpointer(dtype='int32'),ct.c_int,ct.c_int,ct.c_int,ct.c_int,ct.c_int,ct.c_int)
+    _api_version = 21
+  librmn.c_float_unpacker.argtypes = (npc.ndpointer(dtype='int32'),npc.ndpointer(dtype='int32'),npc.ndpointer(dtype='int32'),ct.c_int,ct.POINTER(ct.c_int))
+except ModuleNotFoundError:
+  # If librmn not found, don't crash.  Some functions in this module still
+  # work without this library.
+  pass
+
+# Helper method for splitting metadata from a data segment.
+# Returns a tuple of (legacy metadata, extended metadata, data payload).
+# Also byte-swaps the data so it has the expected endianness.
+def _split_meta (data):
+  # Check if XDF or RSF container (fstd98 or fst24)
+  # This is a hack, which only works if RMETA is set to zero?
+  # For fstd98 this value is the address of the data (non-zero)
+  if data.view('i4')[1] == 0:  # RSF with RMETA=0
+    if data[0] == 0xfe:  # Data stored as big-endian on disk.
+      data = data.view('>i4').astype('i4')
+    elif data[3] == 0xfe:  # Data stored as little-endian on disk.
+      data = data.view('<i4').astype('i4')
+    else:
+      raise Exception  # Unknown endian / bad data?
+    # Determine header size (legacy plus extended metadata).
+    # This seemed to change between development versions of librmn 20.1.0,
+    # so need to check a few places where this info might be?
+    # First, check in (what I believe is) rmeta entry?
+    # In later alpha releases, this seems to contain length of metadata
+    # and extended metadata?
+    rmeta = data[5]
+    legacy_size = rmeta>>16
+    extended_size = rmeta&0xffff
+    if legacy_size > 0:
+      header = data[4+legacy_size-18:4+legacy_size]
+      xmeta = data[4+legacy_size:4+legacy_size+extended_size]
+      data = data[4+legacy_size+extended_size:]
+    else:
+      # Older alpha versions don't encode info here, but there seems to be
+      # a consistent value of header size in this other place?
+      header_size = 18 + (data[0]&0x00ffff00)>>8
+      header = data[4:4+18]
+      xmeta = data[4+18:4+header_size]
+      data = data[4+header_size:]
+  else:
+    data = data.view('>i4').astype('i4')
+    header_size = 20    # FSTD, two aux keys need to be skipped.
+    header = data[:header_size]
+    xmeta = None
+    data = data[header_size:]
+  return header, xmeta, data
+
 
 def decode (data):
   '''
   Decodes the raw FSTD data into the final 2D array of values.
   Similar to fstluk, but here the data is already loaded in memory.
   The data should also include the header information at the
   beginning of the array.
@@ -57,53 +105,28 @@
   ----------
   data : array
       The encoded data
   '''
   import rpnpy.librmn.all as rmn
   import numpy as np
   from fstd2nc.mixins.fstd import dtype_fst2numpy
-  # Check endianness, based on header.
-  # Currently, checks position of 'pad' byte next to nomvar.
-  # Could make this more robust, in case nomvars can start with a space?
-  if data.view('B').flatten()[0x37] == 0:
-    data = data.view('>i4').astype('i4')
-  else:
-    data = data.view('<i4').astype('i4')
-  ni, nj, nk = data[3]>>8, data[4]>>8, data[5]>>12
+  # Split header and data parts, and handle endian conversion.
+  header, xmeta, data = _split_meta (data)
+  # Extract some basic details about the data (data type, shape, bit packing).
+  ni, nj, nk = header[3]>>8, header[4]>>8, header[5]>>12
   nelm = ni*nj*nk
-  datyp = int(data[4]%256) & 191  # Ignore +64 mask.
+  datyp = int(header[4]%256) & 191  # Ignore +64 mask.
   if datyp == 8: nelm = nelm * 2  # For complex, have double the elements.
-  nbits = int(data[2]%256)
+  nbits = int(header[2]%256)
   dtype = dtype_fst2numpy (datyp, nbits)
   if nbits <= 32:
     work = np.empty(nelm,'int32')
   else:
     work = np.empty(nelm,'int64').view('int32')
-  # Strip header
-  # If data address is zero, assume that means this is from an RSF file
-  # (which has the address encoded somewhere else in the metadata).
-  # RSF files have a slightly smaller header (missing the two "aux" keys).
-  if data[1] == 0:
-    data = data[18:]   # Assume RSF, no aux keys
-    # Skip extended metadata.
-    # This has a variable size, so seek to null termination.
-    data = data.view('B')
-    # TODO: Need a more robust way of detecting extended metadata.
-    # Unfortunately, this information isn't encoded in this part of the file,
-    # only in the "directory".
-    # Limit to scanning the first 10000 bytes to avoid wasting too much
-    # time on this (assuming the extended header is smaller than that).
-    if data[:13].view('|S13') == b'{\n  "version"':
-      i = np.where(data[:10000]==0)[0][0]
-      # Skip end padding to 4-byte boundary.
-      while (i%4) != 3: i += 1
-      data = data[i+1:]
-    data = data.view('int32')
-  else:
-    data = data[20:]   # FSTD, two aux keys need to be skipped.
+
   # Extend data buffer for in-place decompression.
   if datyp in (129,130,134):
     d = np.empty(nelm + 100, dtype='int32')
     d[:len(data)] = data
     data = d
   shape = (nj,ni)
   ni = ct.c_int(ni)
@@ -181,18 +204,18 @@
   raw : numpy array (dtype='B')
       The raw array of headers to decode.
   '''
   import numpy as np
   # Check if this is from an RSF contain, which as extra info
   # appended at the end of the header.
   raw = raw.view('u4')
-  if raw.shape[-1] == 24:
-    raw = raw.reshape(-1,12,2)
-    rsf_info = raw[:,:3,:]
-    raw = raw[:,3:,:]
+  width = raw.shape[-1]
+  if width > 18:
+    rsf_info = raw[:,:-18]
+    raw = raw[:,-18:].reshape(-1,9,2)
     raw = np.array(raw)
   else:
     rsf_info = None
     raw = raw.view('>u4').reshape(-1,9,2)
   # Check endianness, based on first record.
   # Currently, checks position of 'pad' byte next to nomvar.
   # Could make this more robust, in case nomvars can start with a space?
@@ -305,17 +328,31 @@
   # NOTE: Date of origin is now calculated in the dates mixin, since it's more
   # involved than a simple arithmetic operation.
   # NOTE: xtra1, xtra2, xtra3 not returned (not used, and take up space in the
   # header table).
 
   # Add RSF record info
   if rsf_info is not None:
-    out['address'] = (rsf_info[:,0,0].astype(int)<<32) + rsf_info[:,0,1]
-    out['length'] = (rsf_info[:,1,0].astype(int)<<32) + rsf_info[:,1,1] - 16
-    out['meta_length'] = rsf_info[:,2,0].copy().view('H')[::2].copy()
+    out['address'] = (rsf_info[:,0].astype(int)<<32) + rsf_info[:,1]
+    out['length'] = (rsf_info[:,2].astype(int)<<32) + rsf_info[:,2] - 16
+    # old 20.1.0 alpha2 version:
+    if rsf_info.shape[1] == 6:
+      out['meta_length'] = rsf_info[:,4].copy().view('H')[::2].copy()
+    # some intermediate development version (?):
+    elif rsf_info.shape[1] == 8:
+      out['meta_length'] = rsf_info[:,6].copy().view('H')[::2].copy()
+    # 20.1.0 alpha3 version:
+    elif rsf_info.shape[1] == 9:
+      out['meta_length'] = rsf_info[:,6].copy().view('H')[::2].copy()
+    else:
+      # Unable to determine metadata length.
+      # There may have been an update to fst24 headers, which would require
+      # an update to this tool.
+      pass
+      #raise Exception(['0x%08x'%x for x in rsf_info[0,:]])
   return out
 
 
 # Extract raw headers from an FST file.
 def _raw_headers_fst (f):
   import numpy as np
   # Get the raw (packed) parameters.
@@ -370,34 +407,42 @@
     assert sos[0]%256 == 0x03  # Must be SOS record.
     # Seek to directory.
     dir_offset = (int(sos[11])<<32) + int(sos[12])
     if dir_offset > 0:
       f.seek(-len(sos)*4,1)
       f.seek(dir_offset,1)
       directory = _read_rsf_segment(f)
+      signature = directory[0]
+      assert signature == 0xfe000106
+      length = (directory[1] << 32) + directory[2]
+      lmeta = directory[3]
+      #assert lmeta == 0  # not used for directories?
       nrecs = int(directory[4])
-      # Metadata width is 96 bytes.
-      # 24 bytes for outer (RSF) metadata, 72 bytes for inner (FSTD) metadata.
-      directory = directory[5:-3].reshape(nrecs,24)
+      # Metadata width may be extended in the future, so don't hard-code it
+      # here.
+      size = len(directory[5:-3])
+      assert size % nrecs == 0, "Unable to determine record width."
+      width = size // nrecs
+      directory = directory[5:-3].reshape(nrecs,width)
       # Modify the address to be absolute file reference.
       address = (directory[:,0].astype(int)<<32) + directory[:,1]
-      address = address + (where_sos + 16)
+      address = address + where_sos
       directory[:,0] = address>>32
       directory[:,1] = address&0xFFFFFFFF
       # Directory must be the last record in a segment?
       eos = _read_rsf_segment(f)
       assert eos[0]%256 == 0x04
       raw.append(directory.astype('u4').view('B').flatten())
     else:
       # Directory must be the last record in a segment?
       eos = _read_rsf_segment(f)
       assert eos[0]%256 == 0x04
   raw = np.concatenate(raw)
   f.close()
-  return raw.reshape(-1,96)
+  return raw.reshape(-1,width*4)
 
 def raw_headers (filename):
   '''
   Extract record headers from the specified file.
   Returns a raw byte array with shape (nrec,72).
   NOTE: This includes deleted records as well.  You can filter them out using
         the 'dltf' flag.
```

### Comparing `fstd2nc-0.20240401.0/fstd2nc/locale/Makefile` & `fstd2nc-0.20240401.1/fstd2nc/locale/Makefile`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/locale/README.md` & `fstd2nc-0.20240401.1/fstd2nc/locale/README.md`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo` & `fstd2nc-0.20240401.1/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: fstd2nc\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-27 15:44+0000\n"
+"POT-Creation-Date: 2024-05-03 19:26+0000\n"
 "PO-Revision-Date: 2022-11-25 17:40+0000\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: fr_CA\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=ISO-8859-1\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -650,17 +650,14 @@
 
 msgid "an RPN standard file"
 msgstr "un fichier standard RPN"
 
 msgid "argument \"-\" with mode %r"
 msgstr "argument \"-\" avec le mode %r"
 
-msgid "can't open '%(filename)s': %(error)s"
-msgstr "impossible d'ouvrir '%s': %s"
-
 msgid "cannot have multiple subparser arguments"
 msgstr "impossible d'avoir plusiers arguments de sous-analyseur"
 
 msgid "cannot merge actions - two groups are named %r"
 msgstr "impossible de fusionner les actions - deux groupes sont nommés %r"
 
 msgid "conflicting option string: %s"
```

### Comparing `fstd2nc-0.20240401.0/fstd2nc/locale/fr_CA.po` & `fstd2nc-0.20240401.1/fstd2nc/locale/fr_CA.po`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/__init__.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/accum.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/accum.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/ascii.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/ascii.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/compat.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/compat.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/dates.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/dates.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/diaghacks.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/diaghacks.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/ensembles.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/ensembles.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/extern.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/extern.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/filter.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/filter.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/fstd.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/fstd.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/gridhacks.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/gridhacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -557,8 +557,7 @@
     d = super(Crop,cls)._postproc (data, **kwargs)
     if crop_j0 is not None and crop_jN is not None:
       d = d[crop_j0:crop_jN,:]
     if crop_i0 is not None and crop_iN is not None:
       d = d[:,crop_i0:crop_iN]
     return d
 
-
```

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/masks.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/masks.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/mesh.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/mesh.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/misc.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/misc.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/netcdf.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/netcdf.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/pruneaxes.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/pruneaxes.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/removestuff.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/removestuff.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/select.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/select.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/series.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/series.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/sfc_codes.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/sfc_codes.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/vardict.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/vardict.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/vcoords.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/vcoords.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/mixins/xycoords.py` & `fstd2nc-0.20240401.1/fstd2nc/mixins/xycoords.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc/stdout.py` & `fstd2nc-0.20240401.1/fstd2nc/stdout.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/fstd2nc.egg-info/PKG-INFO` & `fstd2nc-0.20240401.1/fstd2nc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstd2nc
-Version: 0.20240401.0
+Version: 0.20240401.1
 Summary: Converts RPN standard files (from Environment Canada) to netCDF files.
 Home-page: https://github.com/neishm/fstd2nc
 Author: Mike Neish
 License: LGPL-3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `fstd2nc-0.20240401.0/fstd2nc.egg-info/SOURCES.txt` & `fstd2nc-0.20240401.1/fstd2nc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/sample_meta.ini` & `fstd2nc-0.20240401.1/sample_meta.ini`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.0/setup.py` & `fstd2nc-0.20240401.1/setup.py`

 * *Files identical despite different names*


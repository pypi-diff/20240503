# Comparing `tmp/taurus_pyqtgraph-0.8.0.tar.gz` & `tmp/taurus_pyqtgraph-0.8.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taurus_pyqtgraph-0.8.0.tar", last modified: Mon Nov 27 15:27:00 2023, max compression
+gzip compressed data, was "taurus_pyqtgraph-0.8.1a0.tar", last modified: Fri May  3 08:21:02 2024, max compression
```

## Comparing `taurus_pyqtgraph-0.8.0.tar` & `taurus_pyqtgraph-0.8.1a0.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 15:27:00.221928 taurus_pyqtgraph-0.8.0/
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/CHANGELOG.md
--rwxrwxrwx   0 root         (0) root         (0)     3310 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     1483 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      250 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1738 2023-11-27 15:27:00.221928 taurus_pyqtgraph-0.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5014 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 15:27:00.213929 taurus_pyqtgraph-0.8.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      617 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/docs/Makefile
--rwxrwxrwx   0 root         (0) root         (0)     5043 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/docs/history.rst
--rw-rw-rw-   0 root         (0) root         (0)      275 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      778 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/docs/readme.rst
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/docs/usage.rst
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-11-27 15:27:00.222929 taurus_pyqtgraph-0.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3456 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 15:27:00.217929 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/
--rw-rw-rw-   0 root         (0) root         (0)     2186 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4758 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/autopantool.py
--rw-rw-rw-   0 root         (0) root         (0)     6596 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/buffersizetool.py
--rw-rw-rw-   0 root         (0) root         (0)     1452 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    32473 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/curveproperties.py
--rw-rw-rw-   0 root         (0) root         (0)    21153 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/curvesmodel.py
--rw-rw-rw-   0 root         (0) root         (0)     6762 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/curvespropertiestool.py
--rw-rw-rw-   0 root         (0) root         (0)    10307 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/datainspectortool.py
--rw-rw-rw-   0 root         (0) root         (0)    11913 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/dateaxisitem.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 15:27:00.219929 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/examples/
--rw-rw-rw-   0 root         (0) root         (0)     1011 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1496 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/examples/axislabels.py
--rw-rw-rw-   0 root         (0) root         (0)     2230 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/examples/legendExample.py
--rw-rw-rw-   0 root         (0) root         (0)     1797 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/examples/taurusplotdataitem.py
--rw-rw-rw-   0 root         (0) root         (0)     2072 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/examples/taurustrendset.py
--rw-rw-rw-   0 root         (0) root         (0)     1959 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/examples/y2axis.py
--rw-rw-rw-   0 root         (0) root         (0)     6495 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/forcedreadtool.py
--rw-rw-rw-   0 root         (0) root         (0)     2858 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/legendtool.py
--rw-rw-rw-   0 root         (0) root         (0)     9469 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/plot.py
--rw-rw-rw-   0 root         (0) root         (0)    10618 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/statisticstool.py
--rw-rw-rw-   0 root         (0) root         (0)     2428 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/taurusimageitem.py
--rw-rw-rw-   0 root         (0) root         (0)    22127 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/taurusmodelchoosertool.py
--rw-rw-rw-   0 root         (0) root         (0)     6979 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/taurusplotdataitem.py
--rw-rw-rw-   0 root         (0) root         (0)    19561 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/taurustrendset.py
--rw-rw-rw-   0 root         (0) root         (0)     1645 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/titlepatterneditor.py
--rw-rw-rw-   0 root         (0) root         (0)    20517 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/trend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 15:27:00.219929 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/ui/
--rw-rw-rw-   0 root         (0) root         (0)    11137 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/ui/CurvesAppearanceChooser.ui
--rw-rw-rw-   0 root         (0) root         (0)     3296 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/ui/TaurusItemConfDlg.ui
--rw-rw-rw-   0 root         (0) root         (0)      907 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/util.py
--rw-rw-rw-   0 root         (0) root         (0)    11038 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/y2axis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 15:27:00.218928 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1738 2023-11-27 15:27:00.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1681 2023-11-27 15:27:00.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-27 15:27:00.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      209 2023-11-27 15:27:00.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-11-27 15:27:00.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-11-27 15:27:00.000000 taurus_pyqtgraph-0.8.0/taurus_pyqtgraph.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 15:27:00.221928 taurus_pyqtgraph-0.8.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3143 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/tests/test_curveproperties.py
--rw-rw-rw-   0 root         (0) root         (0)     4561 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/tests/test_dateaxisitem.py
--rw-rw-rw-   0 root         (0) root         (0)    19187 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/tests/test_plot.py
--rw-rw-rw-   0 root         (0) root         (0)      643 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/tests/test_taurus_pyqtgraph.py
--rw-rw-rw-   0 root         (0) root         (0)    15834 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/tests/test_trend.py
--rw-rw-rw-   0 root         (0) root         (0)     1119 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/tests/test_util.py
--rw-rw-rw-   0 root         (0) root         (0)     1294 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/tests/test_y2axis.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-11-27 15:26:52.000000 taurus_pyqtgraph-0.8.0/tests/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:21:02.715392 taurus_pyqtgraph-0.8.1a0/
+-rw-rw-rw-   0 root         (0) root         (0)      603 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/CHANGELOG.md
+-rwxrwxrwx   0 root         (0) root         (0)     3310 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-05-03 08:21:02.715392 taurus_pyqtgraph-0.8.1a0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5197 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:21:02.706392 taurus_pyqtgraph-0.8.1a0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      617 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/docs/Makefile
+-rwxrwxrwx   0 root         (0) root         (0)     5043 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/docs/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)      275 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      567 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      778 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/docs/readme.rst
+-rw-rw-rw-   0 root         (0) root         (0)      161 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/docs/usage.rst
+-rw-rw-rw-   0 root         (0) root         (0)      861 2024-05-03 08:21:02.716392 taurus_pyqtgraph-0.8.1a0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3548 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:21:02.710392 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/
+-rw-rw-rw-   0 root         (0) root         (0)     2235 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5259 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/autopantool.py
+-rw-rw-rw-   0 root         (0) root         (0)     6596 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/buffersizetool.py
+-rw-rw-rw-   0 root         (0) root         (0)     1452 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    36050 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/curveproperties.py
+-rw-rw-rw-   0 root         (0) root         (0)    21153 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/curvesmodel.py
+-rw-rw-rw-   0 root         (0) root         (0)     6762 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/curvespropertiestool.py
+-rw-rw-rw-   0 root         (0) root         (0)    10307 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/datainspectortool.py
+-rw-rw-rw-   0 root         (0) root         (0)    11913 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/dateaxisitem.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:21:02.713392 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1496 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/examples/axislabels.py
+-rw-rw-rw-   0 root         (0) root         (0)     2230 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/examples/legendExample.py
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/examples/taurusplotdataitem.py
+-rw-rw-rw-   0 root         (0) root         (0)     2072 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/examples/taurustrendset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1959 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/examples/y2axis.py
+-rw-rw-rw-   0 root         (0) root         (0)     4983 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/exporters.py
+-rw-rw-rw-   0 root         (0) root         (0)     6495 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/forcedreadtool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2858 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/legendtool.py
+-rw-rw-rw-   0 root         (0) root         (0)     9469 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)    10618 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/statisticstool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2428 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/taurusimageitem.py
+-rw-rw-rw-   0 root         (0) root         (0)    22127 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/taurusmodelchoosertool.py
+-rw-rw-rw-   0 root         (0) root         (0)     6979 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/taurusplotdataitem.py
+-rw-rw-rw-   0 root         (0) root         (0)    19561 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/taurustrendset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1645 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/titlepatterneditor.py
+-rw-rw-rw-   0 root         (0) root         (0)    21366 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/trend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:21:02.713392 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/ui/
+-rw-rw-rw-   0 root         (0) root         (0)    15418 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/ui/CurvesAppearanceChooser.ui
+-rw-rw-rw-   0 root         (0) root         (0)     3296 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/ui/TaurusItemConfDlg.ui
+-rw-rw-rw-   0 root         (0) root         (0)      907 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/util.py
+-rw-rw-rw-   0 root         (0) root         (0)    11038 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/y2axis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:21:02.711392 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-05-03 08:21:02.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1711 2024-05-03 08:21:02.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 08:21:02.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      209 2024-05-03 08:21:02.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-03 08:21:02.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-03 08:21:02.000000 taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:21:02.715392 taurus_pyqtgraph-0.8.1a0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3143 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/tests/test_curveproperties.py
+-rw-rw-rw-   0 root         (0) root         (0)     4561 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/tests/test_dateaxisitem.py
+-rw-rw-rw-   0 root         (0) root         (0)    19187 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/tests/test_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      643 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/tests/test_taurus_pyqtgraph.py
+-rw-rw-rw-   0 root         (0) root         (0)    15834 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/tests/test_trend.py
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/tests/test_util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1294 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/tests/test_y2axis.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2024-05-03 08:20:53.000000 taurus_pyqtgraph-0.8.1a0/tests/util.py
```

### Comparing `taurus_pyqtgraph-0.8.0/CHANGELOG.md` & `taurus_pyqtgraph-0.8.1a0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/CONTRIBUTING.md` & `taurus_pyqtgraph-0.8.1a0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/LICENSE.txt` & `taurus_pyqtgraph-0.8.1a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/PKG-INFO` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: taurus_pyqtgraph
-Version: 0.8.0
+Name: taurus-pyqtgraph
+Version: 0.8.1a0
 Summary: Taurus extension providing pyqtgraph-based widgets
 Home-page: https://gitlab.com/taurus-org/taurus_pyqtgraph
 Author: Taurus Community
 Maintainer: Taurus Community
 Maintainer-email: tauruslib-devel@lists.sourceforge.net
 License: LGPLv3+
 Download-URL: https://gitlab.com/taurus-org/taurus_pyqtgraph
@@ -30,13 +30,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.5
+Provides-Extra: Archiving
 License-File: LICENSE.txt
 
 taurus_pyqtgraph is an extension for the Taurus package.
 It adds the taurus.qt.qtgui.tpg submodule which provides pyqtgraph-based
 widgets.
```

### Comparing `taurus_pyqtgraph-0.8.0/README.md` & `taurus_pyqtgraph-0.8.1a0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,17 +6,26 @@
 The rationale behind taurus_pyqtgraph is described in the [TEP17]
 
 ## Install
 
 Just install this module e.g.:
 
 For the latest release in PyPI:
-
 `pip install taurus_pyqtgraph`
 
+Or locally:
+`pip install .`
+
+If you need Archiving support (HDB++) on trends install it typing:
+`pip install taurus_pyqtgraph["Archiving"]`
+
+Or locally:
+`pip install .["Archiving"]`
+
+
 Alternatively, you can install with conda:
 
 `conda install -c conda-forge -c taurus-org taurus_pyqtgraph`
 
 For development, use a python3 virtual env (or conda, or similar) and:
 
 ```
```

### Comparing `taurus_pyqtgraph-0.8.0/docs/Makefile` & `taurus_pyqtgraph-0.8.1a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/docs/conf.py` & `taurus_pyqtgraph-0.8.1a0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/docs/installation.rst` & `taurus_pyqtgraph-0.8.1a0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/docs/make.bat` & `taurus_pyqtgraph-0.8.1a0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/setup.cfg` & `taurus_pyqtgraph-0.8.1a0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.8.0
+current_version = 0.8.1-alpha
 commit = True
 message = Bump version {current_version} to {new_version}
 tag = False
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}
```

### Comparing `taurus_pyqtgraph-0.8.0/setup.py` & `taurus_pyqtgraph-0.8.1a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,18 @@
 
 platforms = ["Linux", "Windows"]
 
 keywords = ["Taurus", "pyqtgraph", "plugin", "widgets"]
 
 install_requires = ["pyqtgraph>=0.11", "click", "taurus>=4.5.2", "lxml", "ply"]
 
+extras_require = {
+    "Archiving": ["pyhdbpp"]
+}
+
 entry_points = {
     "taurus.qt.qtgui": ["tpg = taurus_pyqtgraph"],
     "taurus.cli.subcommands": ["tpg = taurus_pyqtgraph.cli:tpg"],
     "taurus.plot.alts": ["tpg = taurus_pyqtgraph:TaurusPlot"],
     "taurus.trend.alts": ["tpg = taurus_pyqtgraph:TaurusTrend"],
 }
 
@@ -81,15 +85,15 @@
     "Topic :: Software Development :: User Interfaces",
     "Topic :: Software Development :: Widget Sets",
 ]
 
 
 setup(
     name="taurus_pyqtgraph",
-    version="0.8.0",
+    version="0.8.1-alpha",
     description=description,
     long_description=long_description,
     author=author,
     maintainer=maintainer,
     maintainer_email=maintainer_email,
     url=url,
     download_url=download_url,
@@ -99,8 +103,9 @@
     packages=find_packages(exclude=["tests"]),
     classifiers=classifiers,
     include_package_data=True,
     entry_points=entry_points,
     test_suite="tests",
     python_requires=">=3.5",
     install_requires=install_requires,
+    extras_require=extras_require,
 )
```

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/__init__.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,10 +49,11 @@
     CurveAppearanceProperties,
     CurvesAppearanceChooser,
     serialize_opts,
     deserialize_opts,
 )
 from .datainspectortool import DataInspectorLine, DataInspectorTool
 from .util import unique_data_item_name, ensure_unique_curve_name
+from .exporters import Taurus4TextExporter
 
 # Do not modify the __version__ manually. To be modified by bumpversion
-__version__ = "0.8.0"
+__version__ = "0.8.1-alpha"
```

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/autopantool.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/autopantool.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,25 +55,28 @@
         :param plot_item: (PlotItem)
         """
         self._plotItem = plot_item
         self._viewBox = plot_item.getViewBox()
         self._addToMenu(self._viewBox.menu)
         self._originalXAutoRange = self._viewBox.autoRangeEnabled()[0]
         self._viewBox.sigXRangeChanged.connect(self._onXRangeChanged)
+        self._plotItem.fixed_range_checkbox = self
 
     def _addToMenu(self, menu):
         # In newer PyQtGraph versions (>0.13.1) there is no "menu.axes"
         # property, yet in older versions the QMenu is not added in
         # as child of the menu.
         for submenu in menu.findChildren(QtWidgets.QMenu):
             if submenu.title() == "X axis":
                 x_menu = submenu
+                self._plotItem.x_axis_menu = x_menu.children()[1].children()[0]
                 break
         else:
             x_menu, _ = menu.axes
+            self._plotItem.x_axis_menu = menu.widgetGroups[0].layout()
 
         self._XactionMenu = x_menu.actions()[0]
         x_menu.insertAction(self._XactionMenu, self)
         self.setParent(x_menu)
 
     def _onToggled(self, checked):
         if checked:
@@ -87,15 +90,20 @@
             t = min(3000, t)
             t = max(50, t)
             self._timer.start(t)
         else:
             self._timer.stop()
             self._viewBox.enableAutoRange(x=self._originalXAutoRange)
 
-        self._XactionMenu.setEnabled(not checked)
+        # Get the custom context menu action widget. (X axis)
+        # Then disable editing children except for
+        # "range_label" and "range_combo_box"
+        for element in self.parent().children()[1].children():
+            if element.objectName() not in ["range_label", "range_combo_box"]:
+                element.setEnabled(not checked)
 
     def _onXRangeChanged(self):
         self.setChecked(False)
 
     def updateRange(self):
         """Pans the x axis (change the viewbox range maintaining width but
         ensuring that the right-most point is shown
```

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/buffersizetool.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/buffersizetool.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/cli.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/cli.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/curveproperties.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/curveproperties.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,22 +39,24 @@
 __all__ = [
     "CurveAppearanceProperties",
     "CurvesAppearanceChooser",
     "serialize_opts",
     "deserialize_opts",
     "get_properties_from_curves",
     "set_properties_on_curves",
+    "set_range_on_trend",
     "set_y_axis_for_curve",
     "CURVE_COLORS",
 ]
 
 import copy
+from datetime import datetime, timedelta
 
 from taurus import warning
-from taurus.external.qt import Qt
+from taurus.external.qt import Qt, QtGui
 from taurus.qt.qtgui.util.ui import UILoadable
 from .y2axis import Y2ViewBox, set_y_axis_for_curve
 import pyqtgraph
 
 
 class CONFLICT(object):
     """
@@ -87,14 +89,16 @@
     "right": "Right step",
 }
 
 ReverseNamedStepMode = {}
 for k, v in NamedStepMode.items():
     ReverseNamedStepMode[v] = k
 
+RangeOptions = ["", "5m", "30m", "1h", "12h", "1d", "1w", "1y"]
+
 NamedSymbolStyles = {
     CONFLICT: "",
     None: "No symbol",
     "o": "Circle",
     "s": "Square",
     "d": "Diamond",
     "t": "Down Triangle",
@@ -146,15 +150,27 @@
     0x93AA00,  # Vivid Yellowish Green
     0x593315,  # Deep Yellowish Brown
     # 0xF13A13, # Vivid Reddish Orange
     # 0x232C16, # Dark Olive Green
 ]
 
 CURVE_COLORS = [Qt.QColor(n) for n in NamedColors[:-2]]
-# CURVE_COLORS = [Qt.QColor(n) for n in kelly_colors_hex]
+
+AXIS_RANGE_UNIT_FORMAT_EXAMPLE = """
+The input string should be of the form '<num><unit>', where <num> is an
+  integer and <unit> is one of the next ones (note the space for entire word):
+  - 'm' or ' minutes' for minutes
+  - 'h' or ' hours' for hours
+  - 'd' or ' days' for days
+  - 'w' or ' weeks' for weeks
+  - 'y' or ' years' for years (day-converted based on 365.25 days per year)
+
+  Example: '1h' parses to 1 hours timedelta.
+  Example: '1 hours' parses to 1 hours
+"""
 
 
 @UILoadable
 class CurvesAppearanceChooser(Qt.QWidget):
     """
     A widget for choosing plot appearance for one or more curves.
     The current curves properties are passed using the setCurvesProps()
@@ -185,14 +201,16 @@
         super(CurvesAppearanceChooser, self).__init__(parent)
         self.loadUi()
         self.autoApply = autoApply
         self._curvesDict = curvesDict
         self.plotItem = plotItem
         self.Y2Axis = Y2Axis
 
+        self.ComboBox_Range.insertItems(0, RangeOptions)
+
         self.sStyleCB.insertItems(0, sorted(NamedSymbolStyles.values()))
         self.lStyleCB.insertItems(0, list(NamedLineStyles.values()))
         self.stepModeCB.insertItems(0, list(NamedStepMode.values()))
         self.sColorCB.addItem("")
         self.lColorCB.addItem("")
         self.cAreaDSB.setRange(float("-inf"), float("inf"))
         if not showButtons:
@@ -211,14 +229,16 @@
         self.curvesLW.itemSelectionChanged.connect(
             self._onSelectedCurveChanged
         )
         self.applyBT.clicked.connect(self.onApply)
         self.resetBT.clicked.connect(self.onReset)
         self.sStyleCB.currentIndexChanged.connect(self._onSymbolStyleChanged)
 
+        self.Button_TimeApply.clicked.connect(self.onTimeApply)
+
         self.curvesLW.itemChanged.connect(self._onControlChanged)
         self.sStyleCB.currentIndexChanged.connect(self._onControlChanged)
         self.lStyleCB.currentIndexChanged.connect(self._onControlChanged)
         self.sColorCB.currentIndexChanged.connect(self._onControlChanged)
         self.lColorCB.currentIndexChanged.connect(self._onControlChanged)
         self.stepModeCB.currentIndexChanged.connect(self._onControlChanged)
         self.sSizeSB.valueChanged.connect(self._onControlChanged)
@@ -289,14 +309,17 @@
                 | Qt.Qt.ItemIsSelectable
                 | Qt.Qt.ItemIsUserCheckable
                 | Qt.Qt.ItemIsDragEnabled
                 | Qt.Qt.ItemIsEditable
             )
         self.curvesLW.setCurrentRow(0)
 
+    def getTimeRange(self):
+        return self.ComboBox_Range.currentText()
+
     def getSelectedCurveNames(self):
         """Returns the curve names for the curves selected at the curves list.
 
         *Note*: The names may differ from the displayed text, which
         corresponds to the curve titles (this method is what you likely need if
         you want to get keys to use in curves or curveProp dicts).
 
@@ -504,14 +527,19 @@
             # both buttons should never be checked simultaneously
             raise RuntimeError("Inconsistent state of Y-axis buttons")
 
         # store the props
         self._shownProp = copy.deepcopy(prop)
         return copy.deepcopy(prop)
 
+    def onTimeApply(self):
+        """Sets the selected range on the Trend and stores the value
+        in a dictionary for future easy access."""
+        set_range_on_trend(self.getTimeRange(), plotItem=self.plotItem)
+
     def onApply(self):
         """Apply does 3 things:
 
             - It updates `self.curvePropDict` using the current values
               chosen in the dialog
             - It applies the properties to the curves (if the Chooser was
               initialized with the appropriate curvesDict)
@@ -611,14 +639,90 @@
             y2=y2,
             title=title,
         )
         curves_prop[key] = curve_appearance_properties
     return curves_prop
 
 
+def parse_timedelta(input_str):
+    """Parses a time range string into a timedelta object.
+
+    {}
+
+    Args:
+        input_str (str): The input time range string to parse.
+
+    Returns:
+        timedelta: The parsed timedelta object.
+    """.format(AXIS_RANGE_UNIT_FORMAT_EXAMPLE)
+
+    # Extract numeric value and unit from input
+    input_str = input_str.strip()
+
+    try:
+        if " " in input_str:
+            # Assuming whole word as units
+            value = float(input_str.split(' ')[0].replace(',', '.'))
+            unit = input_str.split(' ')[-1]
+
+            # Pluralize if necessary
+            if not unit.endswith('s'):
+                unit += 's'
+
+            if unit not in ["minutes", "hours", "days", "weeks", "years"]:
+                raise ValueError
+
+            # Convert years to days
+            # (considering an average year of 365.25 days)
+            if unit == "years":
+                value *= 365.25
+                unit = "days"
+
+            return timedelta(**{unit: value})
+        else:
+            # Assuming only a char as unit
+            value = float(input_str[:-1].strip().replace(',', '.'))
+            unit = input_str[-1]
+
+            # Convert years to days
+            # (considering an average year of 365.25 days)
+            if unit == 'y':
+                value *= 365.25
+                unit = 'd'
+
+            # Define a mapping between units and timedelta attributes
+            unit_mapping = {'m': 'minutes', 'h': 'hours', 'd': 'days',
+                            'w': 'weeks', 'y': 'days'}
+            # Create a timedelta object using the extracted values
+            delta = timedelta(**{unit_mapping[unit]: value})
+    except ValueError:
+        QtGui.QMessageBox().warning(None, "ValueError",
+                                    AXIS_RANGE_UNIT_FORMAT_EXAMPLE,
+                                    QtGui.QMessageBox.Ok)
+
+        delta = timedelta(**{"hours": 1})
+
+    return delta
+
+
+def set_range_on_trend(range, plotItem=None):
+    """Sets x-axis range on the plotItem viewbox based on a time range string.
+    Parses the range string into a timedelta, subtracts it from the current
+    time to get the past time, converts to timestamps, and sets the x-axis
+    range between past and current time.
+    """
+    vb = plotItem.getViewBox()
+    time_now = datetime.now()
+    time_past = time_now - parse_timedelta(range)
+    time_now_int = int(time_now.timestamp())
+    time_past_int = int(time_past.timestamp())
+    vb.setXRange(time_now_int, time_past_int, padding=0.0, update=False)
+    plotItem.fixed_range_checkbox.setChecked(True)
+
+
 def set_properties_on_curves(properties, curves, plotItem=None, y2Axis=None):
     """
     Sets properties provided in the `properties` dict to curves provided in
     the `curves` dict. The association of a given curve with a property is
     done by matching the keys in the respective dictionaries.
     If both `plotItem` and `y2Axis` are passed, the curve will be moved to the
     ViewBox defined in the .y2 property
```

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/curvesmodel.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/curvesmodel.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/curvespropertiestool.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/curvespropertiestool.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/datainspectortool.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/datainspectortool.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/dateaxisitem.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/dateaxisitem.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/examples/__init__.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/examples/axislabels.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/examples/axislabels.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/examples/legendExample.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/examples/legendExample.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/examples/taurusplotdataitem.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/examples/taurusplotdataitem.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/examples/taurustrendset.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/examples/taurustrendset.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/examples/y2axis.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/examples/y2axis.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/forcedreadtool.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/forcedreadtool.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/legendtool.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/legendtool.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/plot.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/plot.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/statisticstool.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/statisticstool.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/taurusimageitem.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/taurusimageitem.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/taurusmodelchoosertool.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/taurusmodelchoosertool.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/taurusplotdataitem.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/taurusplotdataitem.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/taurustrendset.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/taurustrendset.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/titlepatterneditor.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/titlepatterneditor.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/trend.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/trend.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from taurus.core.util.log import Logger
 from taurus.external.qt import QtGui, PYSIDE2
 from taurus.qt.qtcore.configuration import BaseConfigurableClass
 
 from taurus_pyqtgraph.statisticstool import StatisticsTool
 from .autopantool import XAutoPanTool
 from .buffersizetool import BufferSizeTool
-from .curveproperties import CURVE_COLORS
+from .curveproperties import CURVE_COLORS, RangeOptions, set_range_on_trend
 from .curvespropertiestool import CurvesPropertiesTool
 from .datainspectortool import DataInspectorTool
 from .dateaxisitem import DateAxisItem
 from .forcedreadtool import ForcedReadTool
 from .legendtool import PlotLegendTool
 from .taurusmodelchoosertool import TaurusXYModelChooserTool
 from .taurustrendset import TaurusTrendSet
@@ -178,14 +178,30 @@
         self.buffer_tool = BufferSizeTool(self, buffer_size=buffer_size)
         self.buffer_tool.attachToPlotItem(self.getPlotItem())
 
         # Add the auto-pan ("oscilloscope mode") tool
         self._autopan = XAutoPanTool()
         self._autopan.attachToPlotItem(self.getPlotItem())
 
+        # add Set View Range actions
+        x_axis_menu = self.plotItem.x_axis_menu
+
+        label = QtGui.QLabel("Set View Range: ")
+        label.setObjectName("range_label")
+        self.combo_box = QtGui.QComboBox(self)
+        self.combo_box.setObjectName("range_combo_box")
+        self.combo_box.setEditable(True)
+        for option in RangeOptions:
+            self.combo_box.addItem(str(option))
+
+        x_axis_menu.addWidget(label, 8, 0, 1, 2)
+        x_axis_menu.addWidget(self.combo_box, 8, 2, 1, 2)
+
+        self.combo_box.activated.connect(self._on_range_idx_changed)
+
         # Register config properties
         self.registerConfigDelegate(self._model_chooser_tool, "XYmodelchooser")
         # self.registerConfigDelegate(self._y2, "Y2Axis")
         self.registerConfigDelegate(self._cprop_tool, "CurvePropertiesTool")
         self.registerConfigDelegate(legend_tool, "legend")
         self.registerConfigDelegate(self._fr_tool, "forceread")
         self.registerConfigDelegate(self.buffer_tool, "buffer")
@@ -362,14 +378,20 @@
 
     def _disableAutoReloadAndDiscardData(self, message):
         self._askForConfirmation(message, buttons=QtGui.QMessageBox.Ok)
         self.info(message)
         self._auto_reload_checkbox.setChecked(False)
         self._onEnableDisableArchivingClicked()  # Force a trigger
 
+    def _on_range_idx_changed(self):
+        time_range = self.combo_box.currentText()
+        plot_item = self.getPlotItem()
+        set_range_on_trend(time_range, plotItem=plot_item)
+        plot_item.getViewBox().menu.close()
+
     def _getCurves(self):
         """returns a flat list with all items from all trend sets"""
         ret = []
         for ts in self.getTrendSets():
             ret += ts[:]
         return ret
```

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/ui/CurvesAppearanceChooser.ui` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/ui/CurvesAppearanceChooser.ui`

 * *Files 20% similar despite different names*

#### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/ui/CurvesAppearanceChooser.ui` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/ui/CurvesAppearanceChooser.ui`

```diff
@@ -2,341 +2,451 @@
 <ui version="4.0">
   <class>curvesAppearanceChooserDlg</class>
   <widget class="QWidget" name="curvesAppearanceChooserDlg">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>808</width>
-        <height>205</height>
+        <width>800</width>
+        <height>500</height>
       </rect>
     </property>
     <property name="sizePolicy">
-      <sizepolicy hsizetype="Preferred" vsizetype="Maximum">
+      <sizepolicy hsizetype="Preferred" vsizetype="MinimumExpanding">
         <horstretch>0</horstretch>
         <verstretch>0</verstretch>
       </sizepolicy>
     </property>
+    <property name="minimumSize">
+      <size>
+        <width>800</width>
+        <height>500</height>
+      </size>
+    </property>
     <property name="maximumSize">
       <size>
         <width>16777215</width>
-        <height>205</height>
+        <height>500</height>
       </size>
     </property>
     <property name="windowTitle">
       <string>Form</string>
     </property>
+    <property name="layoutDirection">
+      <enum>Qt::LeftToRight</enum>
+    </property>
     <layout class="QHBoxLayout">
       <item>
-        <layout class="QVBoxLayout">
+        <layout class="QVBoxLayout" name="VL_Top">
+          <property name="sizeConstraint">
+            <enum>QLayout::SetMaximumSize</enum>
+          </property>
           <item>
-            <widget class="QListWidget" name="curvesLW">
-              <property name="sizePolicy">
-                <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
-                  <horstretch>0</horstretch>
-                  <verstretch>0</verstretch>
-                </sizepolicy>
-              </property>
-              <property name="selectionMode">
-                <enum>QAbstractItemView::ExtendedSelection</enum>
-              </property>
-              <property name="sortingEnabled">
-                <bool>false</bool>
+            <widget class="QGroupBox" name="GB_Curve">
+              <property name="title">
+                <string>Curves Appearance</string>
               </property>
-            </widget>
-          </item>
-          <item>
-            <layout class="QHBoxLayout">
-              <item>
-                <widget class="QPushButton" name="resetBT">
-                  <property name="text">
-                    <string>&amp;Reset</string>
-                  </property>
-                </widget>
-              </item>
-              <item>
-                <widget class="QPushButton" name="applyBT">
-                  <property name="text">
-                    <string>&amp;Apply</string>
-                  </property>
-                </widget>
-              </item>
-            </layout>
-          </item>
-        </layout>
-      </item>
-      <item>
-        <widget class="QGroupBox" name="lineGB">
-          <property name="title">
-            <string>Line</string>
-          </property>
-          <layout class="QGridLayout">
-            <item row="4" column="0">
-              <widget class="QCheckBox" name="cFillCB">
-                <property name="sizePolicy">
-                  <sizepolicy hsizetype="Minimum" vsizetype="Preferred">
-                    <horstretch>0</horstretch>
-                    <verstretch>0</verstretch>
-                  </sizepolicy>
-                </property>
-                <property name="text">
-                  <string>&amp;Area Fill</string>
+              <widget class="QGroupBox" name="lineGB">
+                <property name="geometry">
+                  <rect>
+                    <x>261</x>
+                    <y>30</y>
+                    <width>172</width>
+                    <height>195</height>
+                  </rect>
                 </property>
-              </widget>
-            </item>
-            <item row="0" column="0">
-              <widget class="QLabel" name="label_4">
-                <property name="text">
-                  <string>S&amp;tyle</string>
-                </property>
-                <property name="buddy">
-                  <cstring>lStyleCB</cstring>
-                </property>
-              </widget>
-            </item>
-            <item row="1" column="1">
-              <widget class="QSpinBox" name="lWidthSB">
-                <property name="sizePolicy">
-                  <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
-                    <horstretch>0</horstretch>
-                    <verstretch>0</verstretch>
-                  </sizepolicy>
-                </property>
-                <property name="specialValueText">
-                  <string>--</string>
-                </property>
-                <property name="minimum">
-                  <number>-1</number>
-                </property>
-                <property name="maximum">
-                  <number>100</number>
-                </property>
-                <property name="value">
-                  <number>1</number>
-                </property>
-              </widget>
-            </item>
-            <item row="4" column="1">
-              <widget class="QDoubleSpinBox" name="cAreaDSB">
-                <property name="sizePolicy">
-                  <sizepolicy hsizetype="Minimum" vsizetype="Preferred">
-                    <horstretch>0</horstretch>
-                    <verstretch>0</verstretch>
-                  </sizepolicy>
-                </property>
-                <property name="accelerated">
-                  <bool>true</bool>
+                <property name="title">
+                  <string>Line</string>
                 </property>
-              </widget>
-            </item>
-            <item row="0" column="1">
-              <widget class="QComboBox" name="lStyleCB">
-                <property name="toolTip">
-                  <string>&lt;html&gt;&lt;head&gt;&lt;meta name=&quot;qrichtext&quot; content=&quot;1&quot; /&gt;&lt;style type=&quot;text/css&quot;&gt;
+                <layout class="QGridLayout">
+                  <item row="4" column="0">
+                    <widget class="QCheckBox" name="cFillCB">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Minimum" vsizetype="Preferred">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="text">
+                        <string>&amp;Area Fill</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="0" column="0">
+                    <widget class="QLabel" name="label_4">
+                      <property name="text">
+                        <string>S&amp;tyle</string>
+                      </property>
+                      <property name="buddy">
+                        <cstring>lStyleCB</cstring>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="1" column="1">
+                    <widget class="QSpinBox" name="lWidthSB">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="specialValueText">
+                        <string>--</string>
+                      </property>
+                      <property name="minimum">
+                        <number>-1</number>
+                      </property>
+                      <property name="maximum">
+                        <number>100</number>
+                      </property>
+                      <property name="value">
+                        <number>1</number>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="4" column="1">
+                    <widget class="QDoubleSpinBox" name="cAreaDSB">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Minimum" vsizetype="Preferred">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="accelerated">
+                        <bool>true</bool>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="0" column="1">
+                    <widget class="QComboBox" name="lStyleCB">
+                      <property name="toolTip">
+                        <string>&lt;html&gt;&lt;head&gt;&lt;meta name=&quot;qrichtext&quot; content=&quot;1&quot; /&gt;&lt;style type=&quot;text/css&quot;&gt;
 p, li { white-space: pre-wrap; }
 &lt;/style&gt;&lt;/head&gt;&lt;body style=&quot; font-family:'Sans Serif'; font-size:10pt; font-weight:400; font-style:normal;&quot;&gt;
 &lt;p style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Style of the pen used to connect the points.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                </property>
-              </widget>
-            </item>
-            <item row="3" column="0">
-              <widget class="QLabel" name="labelCurveStyle">
-                <property name="text">
-                  <string>Step mode</string>
-                </property>
-              </widget>
-            </item>
-            <item row="2" column="0">
-              <widget class="QLabel" name="label_6">
-                <property name="text">
-                  <string>Co&amp;lor</string>
-                </property>
-                <property name="buddy">
-                  <cstring>lColorCB</cstring>
-                </property>
-              </widget>
-            </item>
-            <item row="1" column="0">
-              <widget class="QLabel" name="label_5">
-                <property name="text">
-                  <string>&amp;Width</string>
-                </property>
-                <property name="buddy">
-                  <cstring>lWidthSB</cstring>
-                </property>
-              </widget>
-            </item>
-            <item row="3" column="1">
-              <widget class="QComboBox" name="stepModeCB">
-                <property name="toolTip">
-                  <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;&lt;span style=&quot; font-family:'Sans Serif';&quot;&gt;Step mode: whether the data points are connected with flat steps or straight lines&lt;/span&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                </property>
-              </widget>
-            </item>
-            <item row="2" column="1">
-              <widget class="QComboBox" name="lColorCB"/>
-            </item>
-          </layout>
-        </widget>
-      </item>
-      <item>
-        <widget class="QGroupBox" name="symbolGB">
-          <property name="title">
-            <string>Symbols</string>
-          </property>
-          <layout class="QGridLayout">
-            <item row="0" column="0">
-              <widget class="QLabel" name="label">
-                <property name="text">
-                  <string>&amp;Style</string>
-                </property>
-                <property name="buddy">
-                  <cstring>sStyleCB</cstring>
-                </property>
-              </widget>
-            </item>
-            <item row="1" column="0">
-              <widget class="QLabel" name="label_2">
-                <property name="text">
-                  <string>Si&amp;ze</string>
-                </property>
-                <property name="buddy">
-                  <cstring>sSizeSB</cstring>
-                </property>
-              </widget>
-            </item>
-            <item row="0" column="1">
-              <widget class="QComboBox" name="sStyleCB"/>
-            </item>
-            <item row="1" column="1">
-              <widget class="QSpinBox" name="sSizeSB">
-                <property name="specialValueText">
-                  <string>--</string>
-                </property>
-                <property name="minimum">
-                  <number>-1</number>
-                </property>
-                <property name="maximum">
-                  <number>100</number>
-                </property>
-                <property name="singleStep">
-                  <number>1</number>
-                </property>
-                <property name="value">
-                  <number>3</number>
-                </property>
-              </widget>
-            </item>
-            <item row="2" column="0">
-              <widget class="QLabel" name="label_3">
-                <property name="text">
-                  <string>&amp;Color</string>
-                </property>
-                <property name="buddy">
-                  <cstring>sColorCB</cstring>
-                </property>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="3" column="0">
+                    <widget class="QLabel" name="labelCurveStyle">
+                      <property name="text">
+                        <string>Step mode</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="2" column="0">
+                    <widget class="QLabel" name="label_6">
+                      <property name="text">
+                        <string>Co&amp;lor</string>
+                      </property>
+                      <property name="buddy">
+                        <cstring>lColorCB</cstring>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="1" column="0">
+                    <widget class="QLabel" name="label_5">
+                      <property name="text">
+                        <string>&amp;Width</string>
+                      </property>
+                      <property name="buddy">
+                        <cstring>lWidthSB</cstring>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="3" column="1">
+                    <widget class="QComboBox" name="stepModeCB">
+                      <property name="toolTip">
+                        <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;&lt;span style=&quot; font-family:'Sans Serif';&quot;&gt;Step mode: whether the data points are connected with flat steps or straight lines&lt;/span&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="2" column="1">
+                    <widget class="QComboBox" name="lColorCB"/>
+                  </item>
+                </layout>
               </widget>
-            </item>
-            <item row="4" column="0" colspan="2">
-              <spacer>
-                <property name="orientation">
-                  <enum>Qt::Vertical</enum>
-                </property>
-                <property name="sizeHint" stdset="0">
-                  <size>
-                    <width>111</width>
-                    <height>16</height>
-                  </size>
-                </property>
-              </spacer>
-            </item>
-            <item row="3" column="0" colspan="2">
-              <widget class="QCheckBox" name="sFillCB">
-                <property name="text">
-                  <string>&amp;Fill</string>
-                </property>
-                <property name="tristate">
-                  <bool>false</bool>
+              <widget class="QWidget" name="layoutWidget">
+                <property name="geometry">
+                  <rect>
+                    <x>14</x>
+                    <y>30</y>
+                    <width>241</width>
+                    <height>195</height>
+                  </rect>
                 </property>
+                <layout class="QVBoxLayout">
+                  <item>
+                    <widget class="QListWidget" name="curvesLW">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="selectionMode">
+                        <enum>QAbstractItemView::ExtendedSelection</enum>
+                      </property>
+                      <property name="sortingEnabled">
+                        <bool>false</bool>
+                      </property>
+                    </widget>
+                  </item>
+                  <item>
+                    <layout class="QHBoxLayout">
+                      <item>
+                        <widget class="QPushButton" name="resetBT">
+                          <property name="text">
+                            <string>&amp;Reset</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QPushButton" name="applyBT">
+                          <property name="text">
+                            <string>&amp;Apply</string>
+                          </property>
+                        </widget>
+                      </item>
+                    </layout>
+                  </item>
+                </layout>
               </widget>
-            </item>
-            <item row="2" column="1">
-              <widget class="QComboBox" name="sColorCB"/>
-            </item>
-          </layout>
-        </widget>
-      </item>
-      <item>
-        <widget class="QGroupBox" name="otherGB">
-          <property name="title">
-            <string>Other</string>
-          </property>
-          <layout class="QGridLayout">
-            <item row="1" column="0">
-              <widget class="QPushButton" name="changeTitlesBT">
-                <property name="text">
-                  <string>Curve Title(s)...</string>
+              <widget class="QGroupBox" name="symbolGB">
+                <property name="geometry">
+                  <rect>
+                    <x>439</x>
+                    <y>30</y>
+                    <width>135</width>
+                    <height>195</height>
+                  </rect>
                 </property>
-              </widget>
-            </item>
-            <item row="0" column="0">
-              <widget class="QGroupBox" name="groupBox">
                 <property name="title">
-                  <string>Assign to axis</string>
+                  <string>Symbols</string>
                 </property>
-                <layout class="QHBoxLayout">
-                  <item>
-                    <widget class="QRadioButton" name="assignToY1BT">
-                      <property name="toolTip">
-                        <string>&lt;html&gt;&lt;head&gt;&lt;meta name=&quot;qrichtext&quot; content=&quot;1&quot; /&gt;&lt;style type=&quot;text/css&quot;&gt;
-p, li { white-space: pre-wrap; }
-&lt;/style&gt;&lt;/head&gt;&lt;body style=&quot; font-family:'Sans Serif'; font-size:9pt; font-weight:400; font-style:normal;&quot;&gt;
-&lt;p style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Assign selected curves to Y1 (left axis)&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                <layout class="QGridLayout">
+                  <item row="0" column="0">
+                    <widget class="QLabel" name="label">
+                      <property name="text">
+                        <string>&amp;Style</string>
+                      </property>
+                      <property name="buddy">
+                        <cstring>sStyleCB</cstring>
                       </property>
+                    </widget>
+                  </item>
+                  <item row="1" column="0">
+                    <widget class="QLabel" name="label_2">
                       <property name="text">
-                        <string>&amp;Y1</string>
+                        <string>Si&amp;ze</string>
                       </property>
-                      <property name="autoExclusive">
-                        <bool>false</bool>
+                      <property name="buddy">
+                        <cstring>sSizeSB</cstring>
                       </property>
                     </widget>
                   </item>
-                  <item>
-                    <widget class="QRadioButton" name="assignToY2BT">
-                      <property name="toolTip">
-                        <string>&lt;html&gt;&lt;head&gt;&lt;meta name=&quot;qrichtext&quot; content=&quot;1&quot; /&gt;&lt;style type=&quot;text/css&quot;&gt;
-p, li { white-space: pre-wrap; }
-&lt;/style&gt;&lt;/head&gt;&lt;body style=&quot; font-family:'Sans Serif'; font-size:9pt; font-weight:400; font-style:normal;&quot;&gt;
-&lt;p style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Assign selected curves to Y2 (right axis)&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                  <item row="0" column="1">
+                    <widget class="QComboBox" name="sStyleCB"/>
+                  </item>
+                  <item row="1" column="1">
+                    <widget class="QSpinBox" name="sSizeSB">
+                      <property name="specialValueText">
+                        <string>--</string>
                       </property>
+                      <property name="minimum">
+                        <number>-1</number>
+                      </property>
+                      <property name="maximum">
+                        <number>100</number>
+                      </property>
+                      <property name="singleStep">
+                        <number>1</number>
+                      </property>
+                      <property name="value">
+                        <number>3</number>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="2" column="0">
+                    <widget class="QLabel" name="label_3">
                       <property name="text">
-                        <string>Y&amp;2</string>
+                        <string>&amp;Color</string>
+                      </property>
+                      <property name="buddy">
+                        <cstring>sColorCB</cstring>
                       </property>
-                      <property name="autoExclusive">
+                    </widget>
+                  </item>
+                  <item row="4" column="0" colspan="2">
+                    <spacer>
+                      <property name="orientation">
+                        <enum>Qt::Vertical</enum>
+                      </property>
+                      <property name="sizeHint" stdset="0">
+                        <size>
+                          <width>111</width>
+                          <height>16</height>
+                        </size>
+                      </property>
+                    </spacer>
+                  </item>
+                  <item row="3" column="0" colspan="2">
+                    <widget class="QCheckBox" name="sFillCB">
+                      <property name="text">
+                        <string>&amp;Fill</string>
+                      </property>
+                      <property name="tristate">
                         <bool>false</bool>
                       </property>
                     </widget>
                   </item>
+                  <item row="2" column="1">
+                    <widget class="QComboBox" name="sColorCB"/>
+                  </item>
                 </layout>
               </widget>
-            </item>
-            <item row="2" column="0">
-              <widget class="QPushButton" name="bckgndBT">
-                <property name="sizePolicy">
-                  <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
-                    <horstretch>0</horstretch>
-                    <verstretch>0</verstretch>
-                  </sizepolicy>
+              <widget class="QGroupBox" name="otherGB">
+                <property name="geometry">
+                  <rect>
+                    <x>580</x>
+                    <y>30</y>
+                    <width>132</width>
+                    <height>195</height>
+                  </rect>
                 </property>
-                <property name="text">
-                  <string>Background fill...</string>
+                <property name="title">
+                  <string>Other</string>
                 </property>
+                <layout class="QGridLayout">
+                  <item row="1" column="0">
+                    <widget class="QPushButton" name="changeTitlesBT">
+                      <property name="text">
+                        <string>Curve Title(s)...</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="0" column="0">
+                    <widget class="QGroupBox" name="groupBox">
+                      <property name="title">
+                        <string>Assign to axis</string>
+                      </property>
+                      <layout class="QHBoxLayout">
+                        <item>
+                          <widget class="QRadioButton" name="assignToY1BT">
+                            <property name="toolTip">
+                              <string>&lt;html&gt;&lt;head&gt;&lt;meta name=&quot;qrichtext&quot; content=&quot;1&quot; /&gt;&lt;style type=&quot;text/css&quot;&gt;
+p, li { white-space: pre-wrap; }
+&lt;/style&gt;&lt;/head&gt;&lt;body style=&quot; font-family:'Sans Serif'; font-size:9pt; font-weight:400; font-style:normal;&quot;&gt;
+&lt;p style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Assign selected curves to Y1 (left axis)&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                            </property>
+                            <property name="text">
+                              <string>&amp;Y1</string>
+                            </property>
+                            <property name="autoExclusive">
+                              <bool>false</bool>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QRadioButton" name="assignToY2BT">
+                            <property name="toolTip">
+                              <string>&lt;html&gt;&lt;head&gt;&lt;meta name=&quot;qrichtext&quot; content=&quot;1&quot; /&gt;&lt;style type=&quot;text/css&quot;&gt;
+p, li { white-space: pre-wrap; }
+&lt;/style&gt;&lt;/head&gt;&lt;body style=&quot; font-family:'Sans Serif'; font-size:9pt; font-weight:400; font-style:normal;&quot;&gt;
+&lt;p style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Assign selected curves to Y2 (right axis)&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                            </property>
+                            <property name="text">
+                              <string>Y&amp;2</string>
+                            </property>
+                            <property name="autoExclusive">
+                              <bool>false</bool>
+                            </property>
+                          </widget>
+                        </item>
+                      </layout>
+                    </widget>
+                  </item>
+                  <item row="2" column="0">
+                    <widget class="QPushButton" name="bckgndBT">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="text">
+                        <string>Background fill...</string>
+                      </property>
+                    </widget>
+                  </item>
+                </layout>
               </widget>
-            </item>
-          </layout>
-        </widget>
+            </widget>
+          </item>
+          <item>
+            <layout class="QHBoxLayout" name="horizontalLayout">
+              <property name="rightMargin">
+                <number>600</number>
+              </property>
+              <item>
+                <widget class="QGroupBox" name="GB_Time">
+                  <property name="sizePolicy">
+                    <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
+                      <horstretch>0</horstretch>
+                      <verstretch>0</verstretch>
+                    </sizepolicy>
+                  </property>
+                  <property name="maximumSize">
+                    <size>
+                      <width>300</width>
+                      <height>150</height>
+                    </size>
+                  </property>
+                  <property name="baseSize">
+                    <size>
+                      <width>0</width>
+                      <height>0</height>
+                    </size>
+                  </property>
+                  <property name="title">
+                    <string>X Axis Configuration</string>
+                  </property>
+                  <layout class="QGridLayout" name="_2">
+                    <item row="3" column="0" colspan="3">
+                      <widget class="QPushButton" name="Button_TimeApply">
+                        <property name="text">
+                          <string>Apply</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="1" colspan="2">
+                      <widget class="QComboBox" name="ComboBox_Range">
+                        <property name="toolTip">
+                          <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;&lt;span style=&quot; font-size:10pt;&quot;&gt;Range of time for the  X axis&lt;/span&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                        </property>
+                        <property name="editable">
+                          <bool>true</bool>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="0">
+                      <widget class="QLabel" name="Label_Range">
+                        <property name="text">
+                          <string>Range</string>
+                        </property>
+                        <property name="buddy">
+                          <cstring>lStyleCB</cstring>
+                        </property>
+                      </widget>
+                    </item>
+                  </layout>
+                </widget>
+              </item>
+            </layout>
+          </item>
+        </layout>
       </item>
     </layout>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/ui/TaurusItemConfDlg.ui` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/ui/TaurusItemConfDlg.ui`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/util.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/util.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph/y2axis.py` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph/y2axis.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph.egg-info/PKG-INFO` & `taurus_pyqtgraph-0.8.1a0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: taurus-pyqtgraph
-Version: 0.8.0
+Name: taurus_pyqtgraph
+Version: 0.8.1a0
 Summary: Taurus extension providing pyqtgraph-based widgets
 Home-page: https://gitlab.com/taurus-org/taurus_pyqtgraph
 Author: Taurus Community
 Maintainer: Taurus Community
 Maintainer-email: tauruslib-devel@lists.sourceforge.net
 License: LGPLv3+
 Download-URL: https://gitlab.com/taurus-org/taurus_pyqtgraph
@@ -30,13 +30,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.5
+Provides-Extra: Archiving
 License-File: LICENSE.txt
 
 taurus_pyqtgraph is an extension for the Taurus package.
 It adds the taurus.qt.qtgui.tpg submodule which provides pyqtgraph-based
 widgets.
```

### Comparing `taurus_pyqtgraph-0.8.0/taurus_pyqtgraph.egg-info/SOURCES.txt` & `taurus_pyqtgraph-0.8.1a0/taurus_pyqtgraph.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 taurus_pyqtgraph/buffersizetool.py
 taurus_pyqtgraph/cli.py
 taurus_pyqtgraph/curveproperties.py
 taurus_pyqtgraph/curvesmodel.py
 taurus_pyqtgraph/curvespropertiestool.py
 taurus_pyqtgraph/datainspectortool.py
 taurus_pyqtgraph/dateaxisitem.py
+taurus_pyqtgraph/exporters.py
 taurus_pyqtgraph/forcedreadtool.py
 taurus_pyqtgraph/legendtool.py
 taurus_pyqtgraph/plot.py
 taurus_pyqtgraph/statisticstool.py
 taurus_pyqtgraph/taurusimageitem.py
 taurus_pyqtgraph/taurusmodelchoosertool.py
 taurus_pyqtgraph/taurusplotdataitem.py
```

### Comparing `taurus_pyqtgraph-0.8.0/tests/test_curveproperties.py` & `taurus_pyqtgraph-0.8.1a0/tests/test_curveproperties.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/tests/test_dateaxisitem.py` & `taurus_pyqtgraph-0.8.1a0/tests/test_dateaxisitem.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/tests/test_plot.py` & `taurus_pyqtgraph-0.8.1a0/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/tests/test_taurus_pyqtgraph.py` & `taurus_pyqtgraph-0.8.1a0/tests/test_taurus_pyqtgraph.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/tests/test_trend.py` & `taurus_pyqtgraph-0.8.1a0/tests/test_trend.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/tests/test_util.py` & `taurus_pyqtgraph-0.8.1a0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/tests/test_y2axis.py` & `taurus_pyqtgraph-0.8.1a0/tests/test_y2axis.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.8.0/tests/util.py` & `taurus_pyqtgraph-0.8.1a0/tests/util.py`

 * *Files identical despite different names*


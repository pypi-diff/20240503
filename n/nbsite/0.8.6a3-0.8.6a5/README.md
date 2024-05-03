# Comparing `tmp/nbsite-0.8.6a3.tar.gz` & `tmp/nbsite-0.8.6a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbsite-0.8.6a3.tar", last modified: Mon Apr 22 12:56:01 2024, max compression
+gzip compressed data, was "nbsite-0.8.6a5.tar", last modified: Fri May  3 17:38:17 2024, max compression
```

## Comparing `nbsite-0.8.6a3.tar` & `nbsite-0.8.6a5.tar`

### file list

```diff
@@ -1,78 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:56:01.129107 nbsite-0.8.6a3/
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-22 12:56:01.129107 nbsite-0.8.6a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:56:01.117107 nbsite-0.8.6a3/nbsite/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-22 12:56:01.000000 nbsite-0.8.6a3/nbsite/.version
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:56:01.121107 nbsite-0.8.6a3/nbsite/_shared_static/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/_shared_static/alert.css
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/_shared_static/dataframe.css
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/_shared_static/gallery.css
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/_shared_static/holoviz-icon-white.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:56:01.121107 nbsite-0.8.6a3/nbsite/_shared_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/_shared_static/js/goatcounter.js
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/_shared_static/mystnb.css
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/_shared_static/nbsite.css
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/_shared_static/notebook.css
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/_shared_static/scroller.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:56:01.121107 nbsite-0.8.6a3/nbsite/_shared_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/_shared_templates/copyright-last-updated.html
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/_shared_templates/github-stars-button.html
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/_shared_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/_shared_templates/sidebar-nav-bs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:56:01.121107 nbsite-0.8.6a3/nbsite/analytics/
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:56:01.125107 nbsite-0.8.6a3/nbsite/gallery/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/gallery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31439 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/gallery/gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/gallery/thumbnailer.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/ipystartup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23511 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/nbbuild.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/paramdoc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:56:01.125107 nbsite-0.8.6a3/nbsite/pyodide/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/pyodide/ServiceHandler.js
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/pyodide/ServiceWorker.js
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/pyodide/WebWorker.js
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/pyodide/WorkerHandler.js
--rw-r--r--   0 runner    (1001) docker     (127)    17466 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/pyodide/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:56:01.125107 nbsite-0.8.6a3/nbsite/pyodide/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/pyodide/_static/run_cell.js
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/pyodide/_static/runbutton.css
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/pyodide/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/shared_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:56:01.117107 nbsite-0.8.6a3/nbsite/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:56:01.125107 nbsite-0.8.6a3/nbsite/templates/basic/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/templates/basic/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/templates/basic/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/templates/basic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:56:01.125107 nbsite-0.8.6a3/nbsite/templates/holoviz/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/templates/holoviz/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/templates/holoviz/about.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/templates/holoviz/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/templates/holoviz/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:56:01.129107 nbsite-0.8.6a3/nbsite/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18588 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/tests/test_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/tests/test_nbbuild.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/nbsite/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:56:01.129107 nbsite-0.8.6a3/nbsite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-22 12:56:01.000000 nbsite-0.8.6a3/nbsite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-22 12:56:01.000000 nbsite-0.8.6a3/nbsite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 12:56:01.000000 nbsite-0.8.6a3/nbsite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-22 12:56:01.000000 nbsite-0.8.6a3/nbsite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-22 12:56:01.000000 nbsite-0.8.6a3/nbsite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-22 12:56:01.000000 nbsite-0.8.6a3/nbsite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:56:01.129107 nbsite-0.8.6a3/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/scripts/nbsite_cleandisthtml.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5869 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/scripts/nbsite_fix_links.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/scripts/nbsite_from_tmplate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11144 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/scripts/nbsite_generate_modules.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/scripts/nbsite_nbpagebuild.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-22 12:56:01.129107 nbsite-0.8.6a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-22 12:55:03.000000 nbsite-0.8.6a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.586041 nbsite-0.8.6a5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-03 17:38:17.586041 nbsite-0.8.6a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.578041 nbsite-0.8.6a5/nbsite/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-03 17:38:17.000000 nbsite-0.8.6a5/nbsite/.version
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.578041 nbsite-0.8.6a5/nbsite/_shared_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_static/alert.css
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_static/dataframe.css
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_static/gallery.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_static/holoviz-icon-white.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.578041 nbsite-0.8.6a5/nbsite/_shared_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_static/js/goatcounter.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_static/mystnb.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_static/nbsite.css
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_static/notebook.css
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_static/scroller.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.578041 nbsite-0.8.6a5/nbsite/_shared_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_templates/copyright-last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_templates/github-stars-button.html
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_templates/sidebar-nav-bs-alt.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.578041 nbsite-0.8.6a5/nbsite/analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.582041 nbsite-0.8.6a5/nbsite/gallery/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/gallery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31847 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/gallery/gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/gallery/thumbnailer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/ipystartup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23506 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/nbbuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/paramdoc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.582041 nbsite-0.8.6a5/nbsite/pyodide/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/pyodide/ServiceHandler.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/pyodide/ServiceWorker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/pyodide/WebWorker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/pyodide/WorkerHandler.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17466 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/pyodide/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.582041 nbsite-0.8.6a5/nbsite/pyodide/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/pyodide/_static/run_cell.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/pyodide/_static/runbutton.css
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/pyodide/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/shared_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.574041 nbsite-0.8.6a5/nbsite/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.582041 nbsite-0.8.6a5/nbsite/templates/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/templates/basic/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/templates/basic/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/templates/basic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.582041 nbsite-0.8.6a5/nbsite/templates/holoviz/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/templates/holoviz/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/templates/holoviz/about.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/templates/holoviz/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/templates/holoviz/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.582041 nbsite-0.8.6a5/nbsite/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19655 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/tests/test_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/tests/test_nbbuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.586041 nbsite-0.8.6a5/nbsite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-03 17:38:17.000000 nbsite-0.8.6a5/nbsite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-03 17:38:17.000000 nbsite-0.8.6a5/nbsite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:38:17.000000 nbsite-0.8.6a5/nbsite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 17:38:17.000000 nbsite-0.8.6a5/nbsite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-03 17:38:17.000000 nbsite-0.8.6a5/nbsite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 17:38:17.000000 nbsite-0.8.6a5/nbsite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.586041 nbsite-0.8.6a5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/scripts/nbsite_cleandisthtml.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5869 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/scripts/nbsite_fix_links.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/scripts/nbsite_from_tmplate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11144 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/scripts/nbsite_generate_modules.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/scripts/nbsite_nbpagebuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-03 17:38:17.586041 nbsite-0.8.6a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/setup.py
```

### Comparing `nbsite-0.8.6a3/LICENSE.txt` & `nbsite-0.8.6a5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/PKG-INFO` & `nbsite-0.8.6a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbsite
-Version: 0.8.6a3
+Version: 0.8.6a5
 Summary: Build a tested, sphinx-based website from notebooks.
 Home-page: https://nbsite.holoviz.org
 Author: HoloViz developers
 Author-email: developers@holoviz.org
 Maintainer: HoloViz developers
 Maintainer-email: developers@holoviz.org
 License: BSD-3
@@ -13,45 +13,44 @@
 Project-URL: Bug Tracker, https://github.com/holoviz-dev/nbsite/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: param>=1.7.0
 Requires-Dist: pyviz_comms
 Requires-Dist: ipykernel
 Requires-Dist: nbformat
 Requires-Dist: nbconvert
 Requires-Dist: jupyter_client
-Requires-Dist: myst-nb<1,>=0.17
+Requires-Dist: myst-nb>=1.1
 Requires-Dist: sphinx-design
 Requires-Dist: notebook
-Requires-Dist: sphinx
+Requires-Dist: sphinx>=7
 Requires-Dist: beautifulsoup4
 Requires-Dist: jinja2
 Requires-Dist: pillow
-Requires-Dist: pydata-sphinx-theme<0.14,>=0.13.3
-Requires-Dist: myst-parser
+Requires-Dist: pydata-sphinx-theme<0.16,>=0.15
+Requires-Dist: myst-parser>=3
 Requires-Dist: sphinx-copybutton
 Requires-Dist: sphinx-design
 Requires-Dist: sphinxext-rediraffe
-Requires-Dist: urllib3<2.0.0
 Provides-Extra: refman
 Requires-Dist: graphviz; extra == "refman"
 Provides-Extra: gallery
 Requires-Dist: selenium; extra == "gallery"
 Requires-Dist: phantomjs; extra == "gallery"
 Provides-Extra: tests
 Requires-Dist: flake8; extra == "tests"
 Requires-Dist: pytest>=3.9.1; extra == "tests"
-Requires-Dist: importlib-metadata<5.0; extra == "tests"
+Requires-Dist: pre-commit; extra == "tests"
 Provides-Extra: build
 Requires-Dist: setuptools; extra == "build"
 Requires-Dist: param>=1.6.1; extra == "build"
 
 <img src="https://github.com/holoviz-dev/nbsite/raw/main/site/doc/_static/nbsite-logo.png" height=150><br>
 
 -----------------
```

### Comparing `nbsite-0.8.6a3/README.md` & `nbsite-0.8.6a5/README.md`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/__main__.py` & `nbsite-0.8.6a5/nbsite/__main__.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/_shared_static/alert.css` & `nbsite-0.8.6a5/nbsite/_shared_static/alert.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/_shared_static/dataframe.css` & `nbsite-0.8.6a5/nbsite/_shared_static/dataframe.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/_shared_static/holoviz-icon-white.svg` & `nbsite-0.8.6a5/nbsite/_shared_static/holoviz-icon-white.svg`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/_shared_static/js/goatcounter.js` & `nbsite-0.8.6a5/nbsite/_shared_static/js/goatcounter.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/_shared_static/mystnb.css` & `nbsite-0.8.6a5/nbsite/_shared_static/mystnb.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/_shared_static/nbsite.css` & `nbsite-0.8.6a5/nbsite/_shared_static/nbsite.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/_shared_static/notebook.css` & `nbsite-0.8.6a5/nbsite/_shared_static/notebook.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/_shared_static/scroller.css` & `nbsite-0.8.6a5/nbsite/_shared_static/scroller.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/_shared_templates/copyright-last-updated.html` & `nbsite-0.8.6a5/nbsite/_shared_templates/copyright-last-updated.html`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/analytics/__init__.py` & `nbsite-0.8.6a5/nbsite/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/cmd.py` & `nbsite-0.8.6a5/nbsite/cmd.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/gallery/gen.py` & `nbsite-0.8.6a5/nbsite/gallery/gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,21 +19,24 @@
 logging.getLogger(requests.packages.urllib3.__package__).setLevel(logging.ERROR)
 
 BUTTON_GROUP_TEMPLATE = """
 .. raw:: html
 
     <script>
     function gallery_toggle(input) {{
-        backends = {backends};
-        for (i in backends) {{
-            entries = $('.'+backends[i]+'-example').parent();
-            if (backends[i] == input) {{
-                entries.show();
-            }} else {{
-                entries.attr('style','display: none !important')
+        var backends = {backends};
+        for (var i = 0; i < backends.length; i++) {{
+            var entries = document.getElementsByClassName(backends[i] + '-example');
+            for (var j = 0; j < entries.length; j++) {{
+                var parent = entries[j].parentNode;
+                if (backends[i] == input) {{
+                    parent.style.display = '';
+                }} else {{
+                    parent.style.setProperty('display', 'none', 'important');
+                }}
             }}
         }}
     }}
     </script>
 
     <ul class="tab">
     {buttons}
@@ -48,20 +51,23 @@
         </li>
 """
 
 HIDE_JS = """
 .. raw:: html
 
     <script>
-        $(document).ready(function () {{
-            backends = {backends};
-            for (var i=0; i<backends.length; i++){{
-                $('.'+backends[i]+'-example').parent().attr('style','display: none !important');
+    document.addEventListener('DOMContentLoaded', function () {{
+        var backends = {backends};
+        for (var i = 0; i < backends.length; i++) {{
+            var elements = document.getElementsByClassName(backends[i] + '-example');
+            for (var j = 0; j < elements.length; j++) {{
+                elements[j].parentNode.style.setProperty('display', 'none', 'important');
             }}
-        }});
+        }}
+    }});
     </script>
 """
 
 THUMBNAIL_URL = 'https://assets.holoviews.org/thumbnails'
 
 PREFIX = """
 # -*- coding: utf-8 -*-
@@ -620,14 +626,15 @@
         buttons = []
         for n, backend in enumerate(backends):
             buttons.append(BUTTON_TEMPLATE.format(N=n+1, checked='' if n else 'checked="checked"',
                                                   label=backend.capitalize()))
         gallery_rst += BUTTON_GROUP_TEMPLATE.format(buttons=''.join(buttons), backends=backends)
 
     toc = '\n\n.. toctree::\n   :glob:\n   :hidden:\n\n'
+    section_backends = None
     for section in sections:
         if isinstance(section, dict):
             section_backends = section.get('backends', backends)
             skip = section.get('skip', content.get('skip', False))
             orphans = section.get('orphans', content.get('orphans', []))
             heading = section.get('title', section['path'])
             description = section.get('description', None)
```

### Comparing `nbsite-0.8.6a3/nbsite/gallery/thumbnailer.py` & `nbsite-0.8.6a5/nbsite/gallery/thumbnailer.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/nbbuild.py` & `nbsite-0.8.6a5/nbsite/nbbuild.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 import os
 import re
 import shutil
 import string
 import sys
 import typing
 
-from collections import OrderedDict
 from contextlib import contextmanager
 
 import nbformat
 
 from docutils.parsers.rst import Directive, directives
 from docutils.statemachine import string2lines
 from docutils.utils import new_document
@@ -462,29 +461,32 @@
         yield
     finally:
         # Restore execution mode
         if hasattr(env, 'mystnb_config'):
             env.mystnb_config.execution_mode = old_exec_mode
 
 @contextmanager
-def patch_project_source_suffix(env):
+def patch_project_doc2path(env, nb_path):
     # Ugly patch required as myst-nb obtains a reader that
-    # is inferred by sphinx from the document, sphinx literally
+    # is inferred by sphinx from the document. Sphinx literally
     # loops through a glob() result looking for files in a particular
     # order, starting from .rst. As the NotebookDirective is embedded
     # in a .rst, it finds that file instead of the Notebook to be parsed.
-    # Overriding this dict temporarily seems to do the trick.
-    old_source_suffix = env.project.source_suffix
-    env.project.source_suffix = OrderedDict([('.ipynb', 'myst-nb')])
+    # Overriding the doc2path Project method to directly return the
+    # absolute notebook path.
+    old_doc2path = env.project.doc2path
+
+    def new_doc2path(docname: str, absolute: bool):
+        return nb_path
+
+    env.project.doc2path = new_doc2path
     try:
         yield
     finally:
-        # Restore project source_suffix
-        env.project.source_suffix = old_source_suffix
-
+        env.project.doc2path = old_doc2path
 
 
 def render_notebook(nb_path, document, preprocessors=[]):
     env = document.settings.env
     doc = new_document(nb_path, document.settings)
 
     # Load notebook and run preprocessors
@@ -495,15 +497,15 @@
     for preprocessor in preprocessors:
         ntbk, _ = preprocessor(ntbk, {})
     sio = io.StringIO(json.dumps(ntbk))
 
     parser = Parser()
     parser.env = env
 
-    with disable_execution(env), patch_project_source_suffix(env):
+    with disable_execution(env), patch_project_doc2path(env, nb_path):
         parser.parse(sio.read(), doc)
 
     return doc.children
 
 
 class NotebookDirective(Directive):
     """Insert an evaluated notebook into a document
```

### Comparing `nbsite-0.8.6a3/nbsite/paramdoc.py` & `nbsite-0.8.6a5/nbsite/paramdoc.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/pyodide/ServiceWorker.js` & `nbsite-0.8.6a5/nbsite/pyodide/ServiceWorker.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/pyodide/WebWorker.js` & `nbsite-0.8.6a5/nbsite/pyodide/WebWorker.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/pyodide/WorkerHandler.js` & `nbsite-0.8.6a5/nbsite/pyodide/WorkerHandler.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/pyodide/__init__.py` & `nbsite-0.8.6a5/nbsite/pyodide/__init__.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/pyodide/_static/run_cell.js` & `nbsite-0.8.6a5/nbsite/pyodide/_static/run_cell.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/pyodide/_static/runbutton.css` & `nbsite-0.8.6a5/nbsite/pyodide/_static/runbutton.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/pyodide/site.webmanifest` & `nbsite-0.8.6a5/nbsite/pyodide/site.webmanifest`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/shared_conf.py` & `nbsite-0.8.6a5/nbsite/shared_conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,29 +106,42 @@
     'alert.css',
     'dataframe.css',
     'scroller.css'
 ]
 
 # A single line footer that includes the copyright and the last updated date.
 html_theme_options = {
-    "footer_items": [
+    "footer_start": [
         "copyright-last-updated",
     ],
+    # To avoid warning as this is the new default
+    # See https://github.com/pydata/pydata-sphinx-theme/issues/1492
+    "navigation_with_keys": False,
+}
+
+# Default is "**": ["sidebar-nav-bs", "sidebar-ethical-ads"]
+# Overriding the index sidebar to include the toctree on the landing page.
+# The layout.html template in pydata-sphinx-theme removes the default
+# sidebar-nav-bs.html template.
+html_sidebars = {
+    "index": ["sidebar-nav-bs-alt"],
+    "**": ["sidebar-nav-bs-alt"],
 }
 
 # To be reused in a conf.py file to define the `copyright` string reused
 # by sphinx to populate the footer content:
 # copyright_years['start_year'] = '2000'
 # copyright = copyright_fmt.format(**copyright_years)
 copyright_years = {'current_year': str(datetime.date.today().year)}
 copyright_fmt = "{start_year}-{current_year} Holoviz contributors"
 
 # Format of the last updated date in the footer.
 html_last_updated_fmt = '%Y-%m-%d'
 
+rediraffe_redirects = {}
 
 suppress_warnings = [
     # Ignore: (WARNING/2) Document headings start at H2, not H1
     "myst.header",
     # Ignores: skipping unknown output mime type: application/vnd.holoviews_exec.v0+json
     "mystnb.unknown_mime_type"
 ]
```

### Comparing `nbsite-0.8.6a3/nbsite/templates/basic/conf.py` & `nbsite-0.8.6a5/nbsite/templates/basic/conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/templates/holoviz/conf.py` & `nbsite-0.8.6a5/nbsite/templates/holoviz/conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/tests/test_cmd.py` & `nbsite-0.8.6a5/nbsite/tests/test_cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -419,27 +419,29 @@
     (project / "doc" / "Zeroth_Notebook.rst").write_text(EXAMPLE_0_RST)
     (project / "doc" / "First_Notebook.rst").write_text(EXAMPLE_1_RST)
     build('html', str(project / "builtdocs"), project_root=str(project), examples_assets='')
     assert not (project / "builtdocs" / ".doctrees").is_dir()
     assert (project / "builtdocs" / "First_Notebook.html").is_file()
     # Used to test for 10, bumped to 11 as the sphinx-design extension
     # adds a `_sphinx_design_static` folder in `builtdocs/`.
-    assert len(list((project / "builtdocs").iterdir())) == 11
+    # Further incremented when sphinx-rediraffe was added as it adds _rediraffe_redirected.json
+    assert len(list((project / "builtdocs").iterdir())) == 12
 
 @pytest.mark.slow
 def test_build_with_clean_dry_run_does_not_delete(tmp_project_with_docs_skeleton):
     project = tmp_project_with_docs_skeleton
     (project / "doc" / "Zeroth_Notebook.rst").write_text(EXAMPLE_0_RST)
     (project / "doc" / "First_Notebook.rst").write_text(EXAMPLE_1_RST)
     build('html', str(project / "builtdocs"), project_root=str(project), examples_assets='', clean_dry_run=True)
     assert (project / "builtdocs" / ".doctrees").is_dir()
     assert (project / "builtdocs" / "First_Notebook.html").is_file()
     # Used to test for 12, bumped to 13 as the sphinx-design extension
     # adds a `_sphinx_design_static` folder in `builtdocs/`.
-    assert len(list((project / "builtdocs").iterdir())) == 13
+    # Further incremented when sphinx-rediraffe was added as it adds _rediraffe_redirected.json
+    assert len(list((project / "builtdocs").iterdir())) == 14
 
 @pytest.mark.slow
 def test_build_copies_json(tmp_project_with_docs_skeleton):
     project = tmp_project_with_docs_skeleton
     (project / "doc" / "Zeroth_Notebook.rst").write_text(EXAMPLE_0_RST)
     (project / "doc" / "example_json_blob.json").write_text("some json")
     (project / "doc" / "topics").mkdir()
@@ -470,25 +472,39 @@
     (project / "doc" / "conf.py").write_text(CONF_CONTENT)
     (project / "examples" / "index.ipynb").write_text(EXAMPLE_0_CONTENT)
     generate_rst("test_project", project_root=str(project))
     build('html', str(project / "builtdocs"), project_root=str(project), examples_assets='')
     assert (project / "doc" / "1_First_Notebook.ipynb").is_file()
     assert (project / "builtdocs" / "First_Notebook.html").is_file()
     html = (project / "builtdocs" / "First_Notebook.html").read_text()
-    assert '<a class="reference internal" href="Zeroth_Notebook.html"><span class="doc std std-doc">right number' in html
-    assert '<a class="reference internal" href="Zeroth_Notebook.html"><span class="doc std std-doc">wrong number' in html
-    assert '<a class="reference internal" href="Zeroth_Notebook.html"><span class="doc std std-doc">no number' in html
+    assert '<a class="reference internal" href="Zeroth_Notebook.html"><span class="std std-doc">right number' in html
+    assert '<a class="reference internal" href="Zeroth_Notebook.html"><span class="std std-doc">wrong number' in html
+    assert '<a class="reference internal" href="Zeroth_Notebook.html"><span class="std std-doc">no number' in html
+
+@pytest.mark.slow
+def test_build_cell_content_displayed_as_html(tmp_project):
+    project = tmp_project
+    (project / "doc").mkdir()
+    (project / "doc" / "conf.py").write_text(CONF_CONTENT)
+    (project / "examples" / "index.ipynb").write_text(EXAMPLE_0_CONTENT)
+    generate_rst("test_project", project_root=str(project))
+    build('html', str(project / "builtdocs"), project_root=str(project), examples_assets='')
+    assert (project / "doc" / "1_First_Notebook.ipynb").is_file()
+    assert (project / "builtdocs" / "First_Notebook.html").is_file()
+    html = (project / "builtdocs" / "First_Notebook.html").read_text()
+    # Small check to ensure cells are parsed and injected in the HTML output
+    assert '<p>Here is a ref to another notebook with the <a class="reference internal" href="Zeroth_Notebook.html"><span class="std std-doc">right number</span></a>.</p>' in html  # noqa
 
 @pytest.mark.slow
 def test_build_with_keep_numbers_passes_even_when_link_target_does_not_exist(tmp_project):
     project = tmp_project
     (project / "doc").mkdir()
     (project / "doc" / "conf.py").write_text(CONF_CONTENT)
     (project / "examples" / "index.ipynb").write_text(EXAMPLE_0_CONTENT)
     generate_rst("test_project", project_root=str(project), keep_numbers=True)
     build('html', str(project / "builtdocs"), project_root=str(project), examples_assets='')
     assert (project / "doc" / "1_First_Notebook.ipynb").is_file()
     assert (project / "builtdocs" / "1_First_Notebook.html").is_file()
     html = (project / "builtdocs" / "1_First_Notebook.html").read_text()
-    assert '<a class="reference internal" href="0_Zeroth_Notebook.html"><span class="doc std std-doc">right number' in html
+    assert '<a class="reference internal" href="0_Zeroth_Notebook.html"><span class="std std-doc">right number' in html
     assert '<span class="xref myst">wrong number</span>' in html
     assert '<span class="xref myst">no number</span>' in html
```

### Comparing `nbsite-0.8.6a3/nbsite/tests/test_nbbuild.py` & `nbsite-0.8.6a5/nbsite/tests/test_nbbuild.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/tests/test_util.py` & `nbsite-0.8.6a5/nbsite/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite/util.py` & `nbsite-0.8.6a5/nbsite/util.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/nbsite.egg-info/PKG-INFO` & `nbsite-0.8.6a5/nbsite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbsite
-Version: 0.8.6a3
+Version: 0.8.6a5
 Summary: Build a tested, sphinx-based website from notebooks.
 Home-page: https://nbsite.holoviz.org
 Author: HoloViz developers
 Author-email: developers@holoviz.org
 Maintainer: HoloViz developers
 Maintainer-email: developers@holoviz.org
 License: BSD-3
@@ -13,45 +13,44 @@
 Project-URL: Bug Tracker, https://github.com/holoviz-dev/nbsite/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: param>=1.7.0
 Requires-Dist: pyviz_comms
 Requires-Dist: ipykernel
 Requires-Dist: nbformat
 Requires-Dist: nbconvert
 Requires-Dist: jupyter_client
-Requires-Dist: myst-nb<1,>=0.17
+Requires-Dist: myst-nb>=1.1
 Requires-Dist: sphinx-design
 Requires-Dist: notebook
-Requires-Dist: sphinx
+Requires-Dist: sphinx>=7
 Requires-Dist: beautifulsoup4
 Requires-Dist: jinja2
 Requires-Dist: pillow
-Requires-Dist: pydata-sphinx-theme<0.14,>=0.13.3
-Requires-Dist: myst-parser
+Requires-Dist: pydata-sphinx-theme<0.16,>=0.15
+Requires-Dist: myst-parser>=3
 Requires-Dist: sphinx-copybutton
 Requires-Dist: sphinx-design
 Requires-Dist: sphinxext-rediraffe
-Requires-Dist: urllib3<2.0.0
 Provides-Extra: refman
 Requires-Dist: graphviz; extra == "refman"
 Provides-Extra: gallery
 Requires-Dist: selenium; extra == "gallery"
 Requires-Dist: phantomjs; extra == "gallery"
 Provides-Extra: tests
 Requires-Dist: flake8; extra == "tests"
 Requires-Dist: pytest>=3.9.1; extra == "tests"
-Requires-Dist: importlib-metadata<5.0; extra == "tests"
+Requires-Dist: pre-commit; extra == "tests"
 Provides-Extra: build
 Requires-Dist: setuptools; extra == "build"
 Requires-Dist: param>=1.6.1; extra == "build"
 
 <img src="https://github.com/holoviz-dev/nbsite/raw/main/site/doc/_static/nbsite-logo.png" height=150><br>
 
 -----------------
```

### Comparing `nbsite-0.8.6a3/nbsite.egg-info/SOURCES.txt` & `nbsite-0.8.6a5/nbsite.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 nbsite/_shared_static/mystnb.css
 nbsite/_shared_static/nbsite.css
 nbsite/_shared_static/notebook.css
 nbsite/_shared_static/scroller.css
 nbsite/_shared_static/js/goatcounter.js
 nbsite/_shared_templates/copyright-last-updated.html
 nbsite/_shared_templates/github-stars-button.html
-nbsite/_shared_templates/layout.html
-nbsite/_shared_templates/sidebar-nav-bs.html
+nbsite/_shared_templates/sidebar-nav-bs-alt.html
 nbsite/analytics/__init__.py
 nbsite/gallery/__init__.py
 nbsite/gallery/gen.py
 nbsite/gallery/thumbnailer.py
 nbsite/pyodide/ServiceHandler.js
 nbsite/pyodide/ServiceWorker.js
 nbsite/pyodide/WebWorker.js
```

### Comparing `nbsite-0.8.6a3/pyproject.toml` & `nbsite-0.8.6a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/scripts/nbsite_cleandisthtml.py` & `nbsite-0.8.6a5/scripts/nbsite_cleandisthtml.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/scripts/nbsite_fix_links.py` & `nbsite-0.8.6a5/scripts/nbsite_fix_links.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/scripts/nbsite_generate_modules.py` & `nbsite-0.8.6a5/scripts/nbsite_generate_modules.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/scripts/nbsite_nbpagebuild.py` & `nbsite-0.8.6a5/scripts/nbsite_nbpagebuild.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a3/setup.cfg` & `nbsite-0.8.6a5/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-license_file = LICENSE.txt
+license_files = LICENSE.txt
 
 [tool:autover]
 reponame = nbsite
 
 [flake8]
 include = *.py
 exclude = .git,__pycache__,.tox,.eggs,*.egg,doc,dist,build,_build,examples,.ipynb_checkpoints,node_modules,apps
```

### Comparing `nbsite-0.8.6a3/setup.py` & `nbsite-0.8.6a5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,48 +48,47 @@
     url='https://nbsite.holoviz.org',
     project_urls={
         'Documentation': 'https://nbsite.holoviz.org/',
         'Source Code': 'https://github.com/holoviz-dev/nbsite',
         'Bug Tracker': 'https://github.com/holoviz-dev/nbsite/issues'
     },
     packages=find_packages(),
-    python_requires='>=3.8',
+    python_requires='>=3.9',
     install_requires=[
         'param >=1.7.0',
         'pyviz_comms',
         'ipykernel',
         'nbformat',
         'nbconvert',
         'jupyter_client',
-        'myst-nb >=0.17,<1',
+        'myst-nb >=1.1',
         'sphinx-design',
         'notebook',
-        'sphinx',
+        'sphinx >=7',
         'beautifulsoup4',
         'jinja2',
         'pillow',
-        'pydata-sphinx-theme >=0.13.3,<0.14',
-        'myst-parser',
+        'pydata-sphinx-theme >=0.15,<0.16',
+        'myst-parser >=3',
         'sphinx-copybutton',
         'sphinx-design',
         'sphinxext-rediraffe',
-        'urllib3 <2.0.0',
     ],
     extras_require= {
         'refman':[
             'graphviz',
         ],
         'gallery':[
             'selenium',
             'phantomjs'
         ],
         'tests':[
             'flake8',
             'pytest >=3.9.1',
-            'importlib-metadata <5.0', # Avoid errors to removal of EntryPoint shims https://importlib-metadata.readthedocs.io/en/latest/history.html#v5-0-0
+            'pre-commit',
         ],
         'build': [
             "setuptools",
             "param >=1.6.1",
         ]
     },
     include_package_data=True,
```


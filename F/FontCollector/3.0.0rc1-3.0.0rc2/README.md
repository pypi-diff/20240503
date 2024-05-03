# Comparing `tmp/fontcollector-3.0.0rc1.tar.gz` & `tmp/fontcollector-3.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fontcollector-3.0.0rc1.tar", last modified: Mon Apr 29 17:46:32 2024, max compression
+gzip compressed data, was "fontcollector-3.0.0rc2.tar", last modified: Fri May  3 16:40:55 2024, max compression
```

## Comparing `fontcollector-3.0.0rc1.tar` & `fontcollector-3.0.0rc2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:32.251258 fontcollector-3.0.0rc1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:32.251258 fontcollector-3.0.0rc1/FontCollector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-29 17:46:32.000000 fontcollector-3.0.0rc1/FontCollector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-29 17:46:32.000000 fontcollector-3.0.0rc1/FontCollector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:46:32.000000 fontcollector-3.0.0rc1/FontCollector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 17:46:32.000000 fontcollector-3.0.0rc1/FontCollector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-29 17:46:32.000000 fontcollector-3.0.0rc1/FontCollector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-29 17:46:32.000000 fontcollector-3.0.0rc1/FontCollector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-29 17:46:32.251258 fontcollector-3.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:32.247258 fontcollector-3.0.0rc1/font_collector/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:32.247258 fontcollector-3.0.0rc1/font_collector/ass/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/ass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/ass/abc_ass_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/ass/ass_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/ass/ass_style.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/ass/usage_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:32.247258 fontcollector-3.0.0rc1/font_collector/font/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12333 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/abc_font_face.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/chinese_variant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/cmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/factory_abc_font_face.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/font_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/font_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    10758 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/font_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    35666 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/font_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/font_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/font_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     9924 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/lcid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7705 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/name.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/normal_font_face.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:32.251258 fontcollector-3.0.0rc1/font_collector/font/selection_strategy/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/selection_strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/selection_strategy/font_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/selection_strategy/font_selection_strategy_libass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/selection_strategy/font_selection_strategy_vsfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/variable_font_face.py
--rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/mkvpropedit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/parse_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:32.251258 fontcollector-3.0.0rc1/font_collector/system_lang/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/system_lang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/system_lang/abc_system_lang.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/system_lang/linux_lang.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/system_lang/mac_lang.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/system_lang/system_lang.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/system_lang/windows_lang.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 17:46:32.251258 fontcollector-3.0.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:32.251258 fontcollector-3.0.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-29 17:46:28.000000 fontcollector-3.0.0rc1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-29 17:46:28.000000 fontcollector-3.0.0rc1/tests/test_mkvpropedit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:40:55.083694 fontcollector-3.0.0rc2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:40:55.079694 fontcollector-3.0.0rc2/FontCollector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-03 16:40:55.000000 fontcollector-3.0.0rc2/FontCollector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-03 16:40:55.000000 fontcollector-3.0.0rc2/FontCollector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:40:55.000000 fontcollector-3.0.0rc2/FontCollector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-03 16:40:55.000000 fontcollector-3.0.0rc2/FontCollector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-03 16:40:55.000000 fontcollector-3.0.0rc2/FontCollector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 16:40:55.000000 fontcollector-3.0.0rc2/FontCollector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-03 16:40:55.079694 fontcollector-3.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:40:55.075694 fontcollector-3.0.0rc2/font_collector/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:40:55.075694 fontcollector-3.0.0rc2/font_collector/ass/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/ass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/ass/abc_ass_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/ass/ass_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/ass/ass_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/ass/usage_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:40:55.079694 fontcollector-3.0.0rc2/font_collector/font/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/font/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12375 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/font/abc_font_face.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/font/chinese_variant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/font/cmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/font/factory_abc_font_face.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/font/font_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/font/font_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10758 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/font/font_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36471 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/font/font_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/font/font_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/font/font_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9924 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/font/lcid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7705 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/font/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/font/normal_font_face.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:40:55.079694 fontcollector-3.0.0rc2/font_collector/font/selection_strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/font/selection_strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/font/selection_strategy/font_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/font/selection_strategy/font_selection_strategy_libass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/font/selection_strategy/font_selection_strategy_vsfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/font/variable_font_face.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/mkvpropedit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/parse_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:40:55.079694 fontcollector-3.0.0rc2/font_collector/system_lang/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/system_lang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/system_lang/abc_system_lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/system_lang/linux_lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/system_lang/mac_lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/system_lang/system_lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/font_collector/system_lang/windows_lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:40:55.083694 fontcollector-3.0.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:40:55.079694 fontcollector-3.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-03 16:40:50.000000 fontcollector-3.0.0rc2/tests/test_mkvpropedit.py
```

### Comparing `fontcollector-3.0.0rc1/FontCollector.egg-info/PKG-INFO` & `fontcollector-3.0.0rc2/FontCollector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FontCollector
-Version: 3.0.0rc1
+Version: 3.0.0rc2
 Summary: FontCollector for Advanced SubStation Alpha file.
 Author-email: moi15moi <moi15moismokerlolilol@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/moi15moi/FontCollector/
 Project-URL: Tracker, https://github.com/moi15moi/FontCollector/issues/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fontcollector-3.0.0rc1/FontCollector.egg-info/SOURCES.txt` & `fontcollector-3.0.0rc2/FontCollector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/LICENSE` & `fontcollector-3.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/PKG-INFO` & `fontcollector-3.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FontCollector
-Version: 3.0.0rc1
+Version: 3.0.0rc2
 Summary: FontCollector for Advanced SubStation Alpha file.
 Author-email: moi15moi <moi15moismokerlolilol@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/moi15moi/FontCollector/
 Project-URL: Tracker, https://github.com/moi15moi/FontCollector/issues/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fontcollector-3.0.0rc1/README.md` & `fontcollector-3.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/__init__.py` & `fontcollector-3.0.0rc2/font_collector/__init__.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/__main__.py` & `fontcollector-3.0.0rc2/font_collector/__main__.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/ass/abc_ass_document.py` & `fontcollector-3.0.0rc2/font_collector/ass/abc_ass_document.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/ass/ass_document.py` & `fontcollector-3.0.0rc2/font_collector/ass/ass_document.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/ass/ass_style.py` & `fontcollector-3.0.0rc2/font_collector/ass/ass_style.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/ass/usage_data.py` & `fontcollector-3.0.0rc2/font_collector/ass/usage_data.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/exceptions.py` & `fontcollector-3.0.0rc2/font_collector/exceptions.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/font/abc_font_face.py` & `fontcollector-3.0.0rc2/font_collector/font/abc_font_face.py`

 * *Files 3% similar despite different names*

```diff
@@ -262,15 +262,15 @@
         # We cannot use FT_New_Face due to this issue: https://github.com/rougier/freetype-py/issues/157
         with open(self.font_file.filename, mode="rb") as f:
             filebody = f.read()
         error = FT_New_Memory_Face(library, filebody, len(filebody), self.font_index, byref(face))
         if error: raise FT_Exception(error)
 
         ttFont = TTFont(self.font_file.filename, fontNumber=self.font_index)
-        supported_cmaps = FontParser.get_supported_cmaps(ttFont)
+        supported_cmaps = FontParser.get_supported_cmaps(ttFont, self.font_file.filename, self.font_index)
         supported_charmaps = []
         for i in range(face.contents.num_charmaps):
             charmap = face.contents.charmaps[i]
             # Ignore the CMap created by freetype.
             # See: https://freetype.org/freetype2/docs/reference/ft2-truetype_tables.html#ft_get_cmap_format
             if FT_Get_CMap_Format(charmap) == -1:
                 continue
```

### Comparing `fontcollector-3.0.0rc1/font_collector/font/chinese_variant.py` & `fontcollector-3.0.0rc2/font_collector/font/chinese_variant.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/font/cmap.py` & `fontcollector-3.0.0rc2/font_collector/font/cmap.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/font/factory_abc_font_face.py` & `fontcollector-3.0.0rc2/font_collector/font/factory_abc_font_face.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         Args:
             ttFont: An fontTools object
             font_path: Font path.
             font_index: Font index.
         Returns:
             An FontFace instance that represent the ttFont.
         """
-        cmaps = FontParser.get_supported_cmaps(ttFont)
+        cmaps = FontParser.get_supported_cmaps(ttFont, font_path, font_index)
         if len(cmaps) == 0:
              raise InvalidNormalFontFaceException(f"The font doesn't contain any valid cmap.")
 
         cmap_platform_id = cmaps[0].platform_id
         family_names = FontParser.get_filtered_names(ttFont["name"].names, platformID=cmap_platform_id, nameID=NameID.FAMILY_NAME)
 
         font_type = FontType.from_font(ttFont)
```

### Comparing `fontcollector-3.0.0rc1/font_collector/font/font_collection.py` & `fontcollector-3.0.0rc2/font_collector/font/font_collection.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/font/font_file.py` & `fontcollector-3.0.0rc2/font_collector/font/font_file.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/font/font_loader.py` & `fontcollector-3.0.0rc2/font_collector/font/font_loader.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/font/font_parser.py` & `fontcollector-3.0.0rc2/font_collector/font/font_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,17 +370,18 @@
         """
         Args:
             font_path: Font path.
             font_index: Font index.
         Returns:
             is_italic, is_glyphs_emboldened, weight
         """
-        font = Face(font_path.open("rb"), font_index)
-        is_italic = bool(font.style_flags & FT_STYLE_FLAGS["FT_STYLE_FLAG_ITALIC"])
-        is_glyphs_emboldened = bool(font.style_flags & FT_STYLE_FLAGS["FT_STYLE_FLAG_BOLD"])
+        with font_path.open("rb") as f:
+            face = Face(f, font_index)
+        is_italic = bool(face.style_flags & FT_STYLE_FLAGS["FT_STYLE_FLAG_ITALIC"])
+        is_glyphs_emboldened = bool(face.style_flags & FT_STYLE_FLAGS["FT_STYLE_FLAG_BOLD"])
         weight = 700 if is_glyphs_emboldened else 400
 
         return is_italic, is_glyphs_emboldened, weight
 
 
     @staticmethod
     def get_font_italic_bold_property_microsoft_platform(
@@ -492,39 +493,56 @@
         # If there is a tie, prefer codepage different then cp1252
         codepage_encoding = max(count_codepage, key=lambda codepage: (count_codepage[codepage], codepage != 'cp1252'))
 
         return codepage_encoding
 
 
     @staticmethod
-    def get_supported_cmaps(font: TTFont) -> List[CMap]:
+    def get_supported_cmaps(
+        font: TTFont, font_path: Path, font_index: int
+    ) -> List[CMap]:
         """
         Retrieve supported CMaps from a TrueType font.
 
         Args:
             font: A fontTools object representing the font.
+            font_path: Font path.
+            font_index: Font index.
         Returns:
             A list of supported CMaps.
             - To determine which CMaps are supported, refer to FontParser.get_cmap_encoding().
             - If any Microsoft CMaps are present, only those will be returned.
             - If no Microsoft CMaps are found, the method will only return Macintosh CMaps if they are present.
         """
         microsoft_cmaps: List[CMap] = []
         macintosh_cmaps: List[CMap] = []
 
-        cmap_tables: List[CmapSubtable] = font["cmap"].tables
+        try:
+            cmap_tables: List[CmapSubtable] = font["cmap"].tables
 
-        for table in cmap_tables:
-            encoding = FontParser.get_cmap_encoding(table.platformID, table.platEncID)
-            if encoding is not None:
-                cmap = CMap(table.platformID, table.platEncID)
-                if table.platformID == PlatformID.MICROSOFT:
-                    microsoft_cmaps.append(cmap)
-                elif table.platformID == PlatformID.MACINTOSH:
-                    macintosh_cmaps.append(cmap)
+            for table in cmap_tables:
+                encoding = FontParser.get_cmap_encoding(table.platformID, table.platEncID)
+                if encoding is not None:
+                    cmap = CMap(table.platformID, table.platEncID)
+                    if table.platformID == PlatformID.MICROSOFT:
+                        microsoft_cmaps.append(cmap)
+                    elif table.platformID == PlatformID.MACINTOSH:
+                        macintosh_cmaps.append(cmap)
+        except Exception:
+            with font_path.open("rb") as f:
+                face = Face(f, font_index)
+
+            for charmap in face.charmaps:
+                encoding = FontParser.get_cmap_encoding(charmap.platform_id, charmap.encoding_id)
+                if encoding is not None:
+                    cmap = CMap(charmap.platform_id, charmap.encoding_id)
+                    if charmap.platform_id == PlatformID.MICROSOFT:
+                        microsoft_cmaps.append(cmap)
+                    elif charmap.platform_id == PlatformID.MACINTOSH:
+                        macintosh_cmaps.append(cmap)
         return macintosh_cmaps if len(microsoft_cmaps) == 0 else microsoft_cmaps
 
 
     @staticmethod
     def get_cmap_encoding(platform_id: int, encoding_id: int) -> Optional[str]:
         """
         Args:
```

### Comparing `fontcollector-3.0.0rc1/font_collector/font/font_result.py` & `fontcollector-3.0.0rc2/font_collector/font/font_result.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/font/font_type.py` & `fontcollector-3.0.0rc2/font_collector/font/font_type.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/font/lcid.py` & `fontcollector-3.0.0rc2/font_collector/font/lcid.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/font/name.py` & `fontcollector-3.0.0rc2/font_collector/font/name.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/font/normal_font_face.py` & `fontcollector-3.0.0rc2/font_collector/font/normal_font_face.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/font/selection_strategy/font_selection_strategy.py` & `fontcollector-3.0.0rc2/font_collector/font/selection_strategy/font_selection_strategy.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/font/selection_strategy/font_selection_strategy_libass.py` & `fontcollector-3.0.0rc2/font_collector/font/selection_strategy/font_selection_strategy_libass.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/font/selection_strategy/font_selection_strategy_vsfilter.py` & `fontcollector-3.0.0rc2/font_collector/font/selection_strategy/font_selection_strategy_vsfilter.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/font/variable_font_face.py` & `fontcollector-3.0.0rc2/font_collector/font/variable_font_face.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
             font for font in self.font_file.font_faces
             if font.font_index == self.font_index and isinstance(font, VariableFontFace)
         ]
 
         if len(fonts_face) == 0:
             raise ValueError(f"There is no valid font at the index {self.font_index}")
 
-        cmaps = FontParser.get_supported_cmaps(ttFont)
+        cmaps = FontParser.get_supported_cmaps(ttFont, self.font_file.filename, self.font_index)
 
         for font_face in fonts_face:
             generated_font_face = instancer.instantiateVariableFont(ttFont, font_face.named_instance_coordinates)
 
             for cmap in cmaps:
                 for family_name in font_face.family_names:
                     generated_font_face["name"].setName(family_name.value, NameID.FAMILY_NAME, cmap.platform_id, cmap.platform_enc_id, family_name.get_lang_id_from_platform_id(cmap.platform_id))
```

### Comparing `fontcollector-3.0.0rc1/font_collector/mkvpropedit.py` & `fontcollector-3.0.0rc2/font_collector/mkvpropedit.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/parse_arguments.py` & `fontcollector-3.0.0rc2/font_collector/parse_arguments.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/system_lang/mac_lang.py` & `fontcollector-3.0.0rc2/font_collector/system_lang/mac_lang.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/system_lang/system_lang.py` & `fontcollector-3.0.0rc2/font_collector/system_lang/system_lang.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/font_collector/system_lang/windows_lang.py` & `fontcollector-3.0.0rc2/font_collector/system_lang/windows_lang.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/pyproject.toml` & `fontcollector-3.0.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/tests/test_main.py` & `fontcollector-3.0.0rc2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `fontcollector-3.0.0rc1/tests/test_mkvpropedit.py` & `fontcollector-3.0.0rc2/tests/test_mkvpropedit.py`

 * *Files identical despite different names*


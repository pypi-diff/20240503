# Comparing `tmp/litecli-1.8.0.tar.gz` & `tmp/litecli-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litecli-1.8.0.tar", last modified: Wed Mar 30 00:49:22 2022, max compression
+gzip compressed data, was "litecli-1.9.0.tar", last modified: Tue Jun  7 03:11:13 2022, max compression
```

## Comparing `litecli-1.8.0.tar` & `litecli-1.9.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 amjith     (501) staff       (20)        0 2022-03-30 00:49:22.643688 litecli-1.8.0/
--rw-r--r--   0 amjith     (501) staff       (20)     2324 2022-03-30 00:41:47.000000 litecli-1.8.0/CHANGELOG.md
--rw-r--r--   0 amjith     (501) staff       (20)     1468 2022-03-30 00:30:08.000000 litecli-1.8.0/LICENSE
--rw-r--r--   0 amjith     (501) staff       (20)      221 2022-03-30 00:30:08.000000 litecli-1.8.0/MANIFEST.in
--rw-r--r--   0 amjith     (501) staff       (20)     2412 2022-03-30 00:49:22.643771 litecli-1.8.0/PKG-INFO
--rw-r--r--   0 amjith     (501) staff       (20)     1429 2022-03-30 00:30:08.000000 litecli-1.8.0/README.md
-drwxr-xr-x   0 amjith     (501) staff       (20)        0 2022-03-30 00:49:22.640325 litecli-1.8.0/litecli/
--rw-r--r--   0 amjith     (501) staff       (20)      265 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/AUTHORS
--rw-r--r--   0 amjith     (501) staff       (20)       22 2022-03-30 00:48:13.000000 litecli-1.8.0/litecli/__init__.py
--rw-r--r--   0 amjith     (501) staff       (20)     1272 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/clibuffer.py
--rw-r--r--   0 amjith     (501) staff       (20)     4776 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/clistyle.py
--rw-r--r--   0 amjith     (501) staff       (20)     1560 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/clitoolbar.py
--rw-r--r--   0 amjith     (501) staff       (20)      199 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/compat.py
--rw-r--r--   0 amjith     (501) staff       (20)     4501 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/completion_refresher.py
--rw-r--r--   0 amjith     (501) staff       (20)     1713 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/config.py
--rw-r--r--   0 amjith     (501) staff       (20)      746 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/encodingutils.py
--rw-r--r--   0 amjith     (501) staff       (20)     2470 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/key_bindings.py
--rw-r--r--   0 amjith     (501) staff       (20)      281 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/lexer.py
--rw-r--r--   0 amjith     (501) staff       (20)     4079 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/liteclirc
--rw-r--r--   0 amjith     (501) staff       (20)    34870 2022-03-30 00:40:41.000000 litecli-1.8.0/litecli/main.py
-drwxr-xr-x   0 amjith     (501) staff       (20)        0 2022-03-30 00:49:22.641317 litecli-1.8.0/litecli/packages/
--rw-r--r--   0 amjith     (501) staff       (20)        0 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/packages/__init__.py
--rw-r--r--   0 amjith     (501) staff       (20)    13316 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/packages/completion_engine.py
--rw-r--r--   0 amjith     (501) staff       (20)     2183 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/packages/filepaths.py
--rw-r--r--   0 amjith     (501) staff       (20)     7939 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/packages/parseutils.py
--rw-r--r--   0 amjith     (501) staff       (20)     1109 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/packages/prompt_utils.py
-drwxr-xr-x   0 amjith     (501) staff       (20)        0 2022-03-30 00:49:22.641875 litecli-1.8.0/litecli/packages/special/
--rw-r--r--   0 amjith     (501) staff       (20)      247 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/packages/special/__init__.py
--rw-r--r--   0 amjith     (501) staff       (20)     7206 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/packages/special/dbcommands.py
--rw-r--r--   0 amjith     (501) staff       (20)     2007 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/packages/special/favoritequeries.py
--rw-r--r--   0 amjith     (501) staff       (20)    13280 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/packages/special/iocommands.py
--rw-r--r--   0 amjith     (501) staff       (20)     3646 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/packages/special/main.py
--rw-r--r--   0 amjith     (501) staff       (20)     1442 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/packages/special/utils.py
--rw-r--r--   0 amjith     (501) staff       (20)    18321 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/sqlcompleter.py
--rw-r--r--   0 amjith     (501) staff       (20)     7349 2022-03-30 00:30:08.000000 litecli-1.8.0/litecli/sqlexecute.py
-drwxr-xr-x   0 amjith     (501) staff       (20)        0 2022-03-30 00:49:22.640869 litecli-1.8.0/litecli.egg-info/
--rw-r--r--   0 amjith     (501) staff       (20)     2412 2022-03-30 00:49:22.000000 litecli-1.8.0/litecli.egg-info/PKG-INFO
--rw-r--r--   0 amjith     (501) staff       (20)     1349 2022-03-30 00:49:22.000000 litecli-1.8.0/litecli.egg-info/SOURCES.txt
--rw-r--r--   0 amjith     (501) staff       (20)        1 2022-03-30 00:49:22.000000 litecli-1.8.0/litecli.egg-info/dependency_links.txt
--rw-r--r--   0 amjith     (501) staff       (20)      104 2022-03-30 00:49:22.000000 litecli-1.8.0/litecli.egg-info/entry_points.txt
--rw-r--r--   0 amjith     (501) staff       (20)      107 2022-03-30 00:49:22.000000 litecli-1.8.0/litecli.egg-info/requires.txt
--rw-r--r--   0 amjith     (501) staff       (20)        8 2022-03-30 00:49:22.000000 litecli-1.8.0/litecli.egg-info/top_level.txt
--rw-r--r--   0 amjith     (501) staff       (20)     2977 2022-03-30 00:48:37.000000 litecli-1.8.0/release.py
--rw-r--r--   0 amjith     (501) staff       (20)       75 2022-03-30 00:30:08.000000 litecli-1.8.0/requirements-dev.txt
--rw-r--r--   0 amjith     (501) staff       (20)      355 2022-03-30 00:49:22.644013 litecli-1.8.0/setup.cfg
--rwxr-xr-x   0 amjith     (501) staff       (20)     2039 2022-03-30 00:30:08.000000 litecli-1.8.0/setup.py
--rw-r--r--   0 amjith     (501) staff       (20)     3988 2022-03-30 00:30:08.000000 litecli-1.8.0/tasks.py
-drwxr-xr-x   0 amjith     (501) staff       (20)        0 2022-03-30 00:49:22.643463 litecli-1.8.0/tests/
--rw-r--r--   0 amjith     (501) staff       (20)      932 2022-03-30 00:30:08.000000 litecli-1.8.0/tests/conftest.py
-drwxr-xr-x   0 amjith     (501) staff       (20)        0 2022-03-30 00:49:22.643573 litecli-1.8.0/tests/data/
--rw-r--r--   0 amjith     (501) staff       (20)       12 2022-03-30 00:30:08.000000 litecli-1.8.0/tests/data/import_data.csv
--rw-r--r--   0 amjith     (501) staff       (20)     4754 2022-03-30 00:30:08.000000 litecli-1.8.0/tests/liteclirc
--rw-r--r--   0 amjith     (501) staff       (20)       20 2022-03-30 00:30:08.000000 litecli-1.8.0/tests/test.txt
--rw-r--r--   0 amjith     (501) staff       (20)      864 2022-03-30 00:30:08.000000 litecli-1.8.0/tests/test_clistyle.py
--rw-r--r--   0 amjith     (501) staff       (20)    20253 2022-03-30 00:30:08.000000 litecli-1.8.0/tests/test_completion_engine.py
--rw-r--r--   0 amjith     (501) staff       (20)     2450 2022-03-30 00:30:08.000000 litecli-1.8.0/tests/test_completion_refresher.py
--rw-r--r--   0 amjith     (501) staff       (20)     1884 2022-03-30 00:30:08.000000 litecli-1.8.0/tests/test_dbspecial.py
--rw-r--r--   0 amjith     (501) staff       (20)     7006 2022-03-30 00:40:41.000000 litecli-1.8.0/tests/test_main.py
--rw-r--r--   0 amjith     (501) staff       (20)     4100 2022-03-30 00:30:08.000000 litecli-1.8.0/tests/test_parseutils.py
--rw-r--r--   0 amjith     (501) staff       (20)      314 2022-03-30 00:30:08.000000 litecli-1.8.0/tests/test_prompt_utils.py
--rw-r--r--   0 amjith     (501) staff       (20)    13308 2022-03-30 00:30:08.000000 litecli-1.8.0/tests/test_smart_completion_public_schema_only.py
--rw-r--r--   0 amjith     (501) staff       (20)    12073 2022-03-30 00:30:08.000000 litecli-1.8.0/tests/test_sqlexecute.py
--rw-r--r--   0 amjith     (501) staff       (20)     2323 2022-03-30 00:30:08.000000 litecli-1.8.0/tests/utils.py
--rw-r--r--   0 amjith     (501) staff       (20)      168 2022-03-30 00:30:08.000000 litecli-1.8.0/tox.ini
+drwxr-xr-x   0 amjith     (501) staff       (20)        0 2022-06-07 03:11:13.880044 litecli-1.9.0/
+-rw-r--r--   0 amjith     (501) staff       (20)     2925 2022-06-07 03:10:32.000000 litecli-1.9.0/CHANGELOG.md
+-rw-r--r--   0 amjith     (501) staff       (20)     1468 2022-03-30 00:30:08.000000 litecli-1.9.0/LICENSE
+-rw-r--r--   0 amjith     (501) staff       (20)      221 2022-03-30 00:30:08.000000 litecli-1.9.0/MANIFEST.in
+-rw-r--r--   0 amjith     (501) staff       (20)     2412 2022-06-07 03:11:13.880101 litecli-1.9.0/PKG-INFO
+-rw-r--r--   0 amjith     (501) staff       (20)     1429 2022-03-30 00:30:08.000000 litecli-1.9.0/README.md
+drwxr-xr-x   0 amjith     (501) staff       (20)        0 2022-06-07 03:11:13.876512 litecli-1.9.0/litecli/
+-rw-r--r--   0 amjith     (501) staff       (20)      265 2022-03-30 00:30:08.000000 litecli-1.9.0/litecli/AUTHORS
+-rw-r--r--   0 amjith     (501) staff       (20)       22 2022-06-07 03:11:07.000000 litecli-1.9.0/litecli/__init__.py
+-rw-r--r--   0 amjith     (501) staff       (20)     1272 2022-03-30 00:30:08.000000 litecli-1.9.0/litecli/clibuffer.py
+-rw-r--r--   0 amjith     (501) staff       (20)     4776 2022-03-30 00:30:08.000000 litecli-1.9.0/litecli/clistyle.py
+-rw-r--r--   0 amjith     (501) staff       (20)     1599 2022-06-05 03:41:08.000000 litecli-1.9.0/litecli/clitoolbar.py
+-rw-r--r--   0 amjith     (501) staff       (20)      199 2022-03-30 00:30:08.000000 litecli-1.9.0/litecli/compat.py
+-rw-r--r--   0 amjith     (501) staff       (20)     4501 2022-03-30 00:30:08.000000 litecli-1.9.0/litecli/completion_refresher.py
+-rw-r--r--   0 amjith     (501) staff       (20)     1713 2022-03-30 00:30:08.000000 litecli-1.9.0/litecli/config.py
+-rw-r--r--   0 amjith     (501) staff       (20)      746 2022-03-30 00:30:08.000000 litecli-1.9.0/litecli/encodingutils.py
+-rw-r--r--   0 amjith     (501) staff       (20)     2470 2022-03-30 00:30:08.000000 litecli-1.9.0/litecli/key_bindings.py
+-rw-r--r--   0 amjith     (501) staff       (20)      281 2022-03-30 00:30:08.000000 litecli-1.9.0/litecli/lexer.py
+-rw-r--r--   0 amjith     (501) staff       (20)     4281 2022-06-07 03:09:57.000000 litecli-1.9.0/litecli/liteclirc
+-rw-r--r--   0 amjith     (501) staff       (20)    35157 2022-06-07 03:09:57.000000 litecli-1.9.0/litecli/main.py
+drwxr-xr-x   0 amjith     (501) staff       (20)        0 2022-06-07 03:11:13.877687 litecli-1.9.0/litecli/packages/
+-rw-r--r--   0 amjith     (501) staff       (20)        0 2022-03-30 00:30:08.000000 litecli-1.9.0/litecli/packages/__init__.py
+-rw-r--r--   0 amjith     (501) staff       (20)    13337 2022-06-07 03:09:57.000000 litecli-1.9.0/litecli/packages/completion_engine.py
+-rw-r--r--   0 amjith     (501) staff       (20)     2183 2022-03-30 00:30:08.000000 litecli-1.9.0/litecli/packages/filepaths.py
+-rw-r--r--   0 amjith     (501) staff       (20)     7939 2022-03-30 00:30:08.000000 litecli-1.9.0/litecli/packages/parseutils.py
+-rw-r--r--   0 amjith     (501) staff       (20)     1109 2022-03-30 00:30:08.000000 litecli-1.9.0/litecli/packages/prompt_utils.py
+drwxr-xr-x   0 amjith     (501) staff       (20)        0 2022-06-07 03:11:13.878291 litecli-1.9.0/litecli/packages/special/
+-rw-r--r--   0 amjith     (501) staff       (20)      247 2022-03-30 00:30:08.000000 litecli-1.9.0/litecli/packages/special/__init__.py
+-rw-r--r--   0 amjith     (501) staff       (20)     7707 2022-06-07 03:09:57.000000 litecli-1.9.0/litecli/packages/special/dbcommands.py
+-rw-r--r--   0 amjith     (501) staff       (20)     2007 2022-03-30 00:30:08.000000 litecli-1.9.0/litecli/packages/special/favoritequeries.py
+-rw-r--r--   0 amjith     (501) staff       (20)    13280 2022-03-30 00:30:08.000000 litecli-1.9.0/litecli/packages/special/iocommands.py
+-rw-r--r--   0 amjith     (501) staff       (20)     3646 2022-03-30 00:30:08.000000 litecli-1.9.0/litecli/packages/special/main.py
+-rw-r--r--   0 amjith     (501) staff       (20)     1442 2022-03-30 00:30:08.000000 litecli-1.9.0/litecli/packages/special/utils.py
+-rw-r--r--   0 amjith     (501) staff       (20)    18321 2022-03-30 00:30:08.000000 litecli-1.9.0/litecli/sqlcompleter.py
+-rw-r--r--   0 amjith     (501) staff       (20)     7506 2022-06-07 03:09:57.000000 litecli-1.9.0/litecli/sqlexecute.py
+drwxr-xr-x   0 amjith     (501) staff       (20)        0 2022-06-07 03:11:13.877210 litecli-1.9.0/litecli.egg-info/
+-rw-r--r--   0 amjith     (501) staff       (20)     2412 2022-06-07 03:11:13.000000 litecli-1.9.0/litecli.egg-info/PKG-INFO
+-rw-r--r--   0 amjith     (501) staff       (20)     1349 2022-06-07 03:11:13.000000 litecli-1.9.0/litecli.egg-info/SOURCES.txt
+-rw-r--r--   0 amjith     (501) staff       (20)        1 2022-06-07 03:11:13.000000 litecli-1.9.0/litecli.egg-info/dependency_links.txt
+-rw-r--r--   0 amjith     (501) staff       (20)      104 2022-06-07 03:11:13.000000 litecli-1.9.0/litecli.egg-info/entry_points.txt
+-rw-r--r--   0 amjith     (501) staff       (20)      107 2022-06-07 03:11:13.000000 litecli-1.9.0/litecli.egg-info/requires.txt
+-rw-r--r--   0 amjith     (501) staff       (20)        8 2022-06-07 03:11:13.000000 litecli-1.9.0/litecli.egg-info/top_level.txt
+-rw-r--r--   0 amjith     (501) staff       (20)     2977 2022-03-30 00:48:37.000000 litecli-1.9.0/release.py
+-rw-r--r--   0 amjith     (501) staff       (20)       75 2022-03-30 00:30:08.000000 litecli-1.9.0/requirements-dev.txt
+-rw-r--r--   0 amjith     (501) staff       (20)      355 2022-06-07 03:11:13.880323 litecli-1.9.0/setup.cfg
+-rwxr-xr-x   0 amjith     (501) staff       (20)     2039 2022-03-30 00:30:08.000000 litecli-1.9.0/setup.py
+-rw-r--r--   0 amjith     (501) staff       (20)     3988 2022-03-30 00:30:08.000000 litecli-1.9.0/tasks.py
+drwxr-xr-x   0 amjith     (501) staff       (20)        0 2022-06-07 03:11:13.879711 litecli-1.9.0/tests/
+-rw-r--r--   0 amjith     (501) staff       (20)      932 2022-03-30 00:30:08.000000 litecli-1.9.0/tests/conftest.py
+drwxr-xr-x   0 amjith     (501) staff       (20)        0 2022-06-07 03:11:13.879824 litecli-1.9.0/tests/data/
+-rw-r--r--   0 amjith     (501) staff       (20)       12 2022-03-30 00:30:08.000000 litecli-1.9.0/tests/data/import_data.csv
+-rw-r--r--   0 amjith     (501) staff       (20)     5058 2022-06-07 03:09:57.000000 litecli-1.9.0/tests/liteclirc
+-rw-r--r--   0 amjith     (501) staff       (20)       20 2022-03-30 00:30:08.000000 litecli-1.9.0/tests/test.txt
+-rw-r--r--   0 amjith     (501) staff       (20)      864 2022-03-30 00:30:08.000000 litecli-1.9.0/tests/test_clistyle.py
+-rw-r--r--   0 amjith     (501) staff       (20)    20253 2022-03-30 00:30:08.000000 litecli-1.9.0/tests/test_completion_engine.py
+-rw-r--r--   0 amjith     (501) staff       (20)     2450 2022-03-30 00:30:08.000000 litecli-1.9.0/tests/test_completion_refresher.py
+-rw-r--r--   0 amjith     (501) staff       (20)     2163 2022-06-07 03:09:57.000000 litecli-1.9.0/tests/test_dbspecial.py
+-rw-r--r--   0 amjith     (501) staff       (20)     7006 2022-03-30 00:40:41.000000 litecli-1.9.0/tests/test_main.py
+-rw-r--r--   0 amjith     (501) staff       (20)     4100 2022-03-30 00:30:08.000000 litecli-1.9.0/tests/test_parseutils.py
+-rw-r--r--   0 amjith     (501) staff       (20)      314 2022-03-30 00:30:08.000000 litecli-1.9.0/tests/test_prompt_utils.py
+-rw-r--r--   0 amjith     (501) staff       (20)    13308 2022-03-30 00:30:08.000000 litecli-1.9.0/tests/test_smart_completion_public_schema_only.py
+-rw-r--r--   0 amjith     (501) staff       (20)    12073 2022-03-30 00:30:08.000000 litecli-1.9.0/tests/test_sqlexecute.py
+-rw-r--r--   0 amjith     (501) staff       (20)     2323 2022-03-30 00:30:08.000000 litecli-1.9.0/tests/utils.py
+-rw-r--r--   0 amjith     (501) staff       (20)      168 2022-03-30 00:30:08.000000 litecli-1.9.0/tox.ini
```

### Comparing `litecli-1.8.0/CHANGELOG.md` & `litecli-1.9.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+## 1.9.0 - 2022-06-06
+
+### Features
+
+* Add support for ANSI escape sequences for coloring the prompt.
+* Add support for `.indexes` command.
+* Add an option to turn off the auto-completion menu. Completion menu can be
+  triggered by pressed the `<tab>` key when this option is set to False. Fixes
+  [#105](https://github.com/dbcli/litecli/issues/105).
+
+### Bug Fixes
+
+* Fix [#120](https://github.com/dbcli/litecli/issues/120). Make the `.read` command actually read and execute the commands from a file.
+* Fix  [#96](https://github.com/dbcli/litecli/issues/96) the crash in VI mode when pressing `r`.
+
 ## 1.8.0 - 2022-03-29
 
 ### Features
 
 * Update compatible Python versions. (Thanks: [blazewicz])
 * Add support for Python 3.10. (Thanks: [blazewicz])
 * Drop support for Python 3.6. (Thanks: [blazewicz])
```

### Comparing `litecli-1.8.0/LICENSE` & `litecli-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/PKG-INFO` & `litecli-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litecli
-Version: 1.8.0
+Version: 1.9.0
 Summary: CLI for SQLite Databases with auto-completion and syntax highlighting.
 Home-page: https://github.com/dbcli/litecli
 Author: dbcli
 Author-email: litecli-users@googlegroups.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `litecli-1.8.0/README.md` & `litecli-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/litecli/clibuffer.py` & `litecli-1.9.0/litecli/clibuffer.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/litecli/clistyle.py` & `litecli-1.9.0/litecli/clistyle.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/litecli/clitoolbar.py` & `litecli-1.9.0/litecli/clitoolbar.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,8 +44,9 @@
 def _get_vi_mode():
     """Get the current vi mode for display."""
     return {
         InputMode.INSERT: "I",
         InputMode.NAVIGATION: "N",
         InputMode.REPLACE: "R",
         InputMode.INSERT_MULTIPLE: "M",
+        InputMode.REPLACE_SINGLE: "R",
     }[get_app().vi_state.input_mode]
```

### Comparing `litecli-1.8.0/litecli/completion_refresher.py` & `litecli-1.9.0/litecli/completion_refresher.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/litecli/config.py` & `litecli-1.9.0/litecli/config.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/litecli/encodingutils.py` & `litecli-1.9.0/litecli/encodingutils.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/litecli/key_bindings.py` & `litecli-1.9.0/litecli/key_bindings.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/litecli/liteclirc` & `litecli-1.9.0/litecli/liteclirc`

 * *Files 4% similar despite different names*

```diff
@@ -48,24 +48,29 @@
 # Emacs mode: Ctrl-A is home, Ctrl-E is end. All emacs keybindings are available in the REPL.
 # When Vi mode is enabled you can use modal editing features offered by Vi in the REPL.
 key_bindings = emacs
 
 # Enabling this option will show the suggestions in a wider menu. Thus more items are suggested.
 wider_completion_menu = False
 
+# Autocompletion is on by default. This can be truned off by setting this
+# option to False. Pressing tab will still trigger completion.
+autocompletion = True
+
 # litecli prompt
 # \D - The full current date
 # \d - Database name
 # \f - File basename of the "main" database
 # \m - Minutes of the current time
 # \n - Newline
 # \P - AM/PM
 # \R - The current time, in 24-hour military time (0-23)
 # \r - The current time, standard 12-hour time (1-12)
 # \s - Seconds of the current time
+# \x1b[...m - insert ANSI escape sequence
 prompt = '\d> '
 prompt_continuation = '-> '
 
 # Show/hide the informational toolbar with function keymap at the footer.
 show_bottom_toolbar = True
 
 # Skip intro info on startup and outro info on exit
```

### Comparing `litecli-1.8.0/litecli/main.py` & `litecli-1.9.0/litecli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import sqlparse
 from prompt_toolkit.completion import DynamicCompleter
 from prompt_toolkit.enums import DEFAULT_BUFFER, EditingMode
 from prompt_toolkit.shortcuts import PromptSession, CompleteStyle
 from prompt_toolkit.styles.pygments import style_from_pygments_cls
 from prompt_toolkit.document import Document
 from prompt_toolkit.filters import HasFocus, IsDone
+from prompt_toolkit.formatted_text import ANSI
 from prompt_toolkit.layout.processors import (
     HighlightMatchingBracketProcessor,
     ConditionalProcessor,
 )
 from prompt_toolkit.lexers import PygmentsLexer
 from prompt_toolkit.history import FileHistory
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
@@ -84,14 +85,15 @@
         self.formatter.litecli = self
         self.syntax_style = c["main"]["syntax_style"]
         self.less_chatty = c["main"].as_bool("less_chatty")
         self.show_bottom_toolbar = c["main"].as_bool("show_bottom_toolbar")
         self.cli_style = c["colors"]
         self.output_style = style_factory_output(self.syntax_style, self.cli_style)
         self.wider_completion_menu = c["main"].as_bool("wider_completion_menu")
+        self.autocompletion = c["main"].as_bool("autocompletion")
         c_dest_warning = c["main"].as_bool("destructive_warning")
         self.destructive_warning = c_dest_warning if warn is None else warn
         self.login_path_as_host = c["main"].as_bool("login_path_as_host")
 
         # read from cli argument or user config file
         self.auto_vertical_output = auto_vertical_output or c["main"].as_bool(
             "auto_vertical_output"
@@ -157,18 +159,19 @@
             "\\T",
             "Change the table format used to output results.",
             aliases=("tableformat", "\\T"),
             case_sensitive=True,
         )
         special.register_special_command(
             self.execute_from_file,
-            "source",
+            ".read",
             "\\. filename",
             "Execute commands from file.",
-            aliases=("\\.",),
+            case_sensitive=True,
+            aliases=("\\.", "source"),
         )
         special.register_special_command(
             self.change_prompt_format,
             "prompt",
             "\\R",
             "Change prompt format.",
             aliases=("\\R",),
@@ -377,15 +380,16 @@
         def get_message():
             prompt = self.get_prompt(self.prompt_format)
             if (
                 self.prompt_format == self.default_prompt
                 and len(prompt) > self.max_len_prompt
             ):
                 prompt = self.get_prompt("\\d> ")
-            return [("class:prompt", prompt)]
+            prompt = prompt.replace("\\x1b", "\x1b")
+            return ANSI(prompt)
 
         def get_continuation(width, line_number, is_soft_wrap):
             continuation = " " * (width - 1) + " "
             return [("class:continuation", continuation)]
 
         def show_suggestion_tip():
             return iterations < 2
@@ -543,14 +547,17 @@
         get_toolbar_tokens = create_toolbar_tokens_func(self, show_suggestion_tip)
 
         if self.wider_completion_menu:
             complete_style = CompleteStyle.MULTI_COLUMN
         else:
             complete_style = CompleteStyle.COLUMN
 
+        if not self.autocompletion:
+            complete_style = CompleteStyle.READLINE_LIKE
+
         with self._completer_lock:
 
             if self.key_bindings == "vi":
                 editing_mode = EditingMode.VI
             else:
                 editing_mode = EditingMode.EMACS
```

### Comparing `litecli-1.8.0/litecli/packages/completion_engine.py` & `litecli-1.9.0/litecli/packages/completion_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,22 +101,22 @@
 
     if cmd in ("\\T"):
         return [{"type": "table_format"}]
 
     if cmd in ["\\f", "\\fs", "\\fd"]:
         return [{"type": "favoritequery"}]
 
-    if cmd in ["\\d", "\\dt", "\\dt+", ".schema"]:
+    if cmd in ["\\d", "\\dt", "\\dt+", ".schema", ".indexes"]:
         return [
             {"type": "table", "schema": []},
             {"type": "view", "schema": []},
             {"type": "schema"},
         ]
 
-    if cmd in ["\\.", "source", ".open"]:
+    if cmd in ["\\.", "source", ".open", ".read"]:
         return [{"type": "file_name"}]
 
     if cmd in [".import"]:
         # Usage: .import filename table
         if _expecting_arg_idx(arg, text) == 1:
             return [{"type": "file_name"}]
         else:
```

### Comparing `litecli-1.8.0/litecli/packages/filepaths.py` & `litecli-1.9.0/litecli/packages/filepaths.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/litecli/packages/parseutils.py` & `litecli-1.9.0/litecli/packages/parseutils.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/litecli/packages/prompt_utils.py` & `litecli-1.9.0/litecli/packages/prompt_utils.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/litecli/packages/special/dbcommands.py` & `litecli-1.9.0/litecli/packages/special/dbcommands.py`

 * *Files 8% similar despite different names*

```diff
@@ -107,14 +107,49 @@
         headers = [x[0] for x in cur.description]
         return [(None, cur, headers, "")]
     else:
         return [(None, None, None, "")]
 
 
 @special_command(
+    ".indexes",
+    ".indexes [tablename]",
+    "List indexes.",
+    arg_type=PARSED_QUERY,
+    case_sensitive=True,
+    aliases=("\\di",),
+)
+def list_indexes(cur, arg=None, arg_type=PARSED_QUERY, verbose=False):
+    if arg:
+        args = ("{0}%".format(arg),)
+        query = """
+            SELECT name FROM sqlite_master
+            WHERE type = 'index' AND tbl_name LIKE ? AND name NOT LIKE 'sqlite_%'
+            ORDER BY 1
+        """
+    else:
+        args = tuple()
+        query = """
+            SELECT name FROM sqlite_master
+            WHERE type = 'index' AND name NOT LIKE 'sqlite_%'
+            ORDER BY 1
+        """
+
+    log.debug(query)
+    cur.execute(query, args)
+    indexes = cur.fetchall()
+    status = ""
+    if cur.description:
+        headers = [x[0] for x in cur.description]
+    else:
+        return [(None, None, None, "")]
+    return [(None, indexes, headers, status)]
+
+
+@special_command(
     ".status",
     "\\s",
     "Show current settings.",
     arg_type=RAW_QUERY,
     aliases=("\\s",),
     case_sensitive=True,
 )
@@ -199,32 +234,14 @@
     else:
         return [(None, None, None, "")]
 
     return [(None, tables, headers, status)]
 
 
 @special_command(
-    ".read",
-    ".read path",
-    "Read input from path",
-    arg_type=PARSED_QUERY,
-    case_sensitive=True,
-)
-def read_script(cur, arg, **_):
-    args = shlex.split(arg)
-    if len(args) != 1:
-        raise TypeError(".read accepts exactly one path")
-    path = args[0]
-    with open(path, "r") as f:
-        script = f.read()
-        cur.executescript(script)
-    return [(None, None, None, "")]
-
-
-@special_command(
     ".import",
     ".import filename table",
     "Import data from filename into an existing table",
     arg_type=PARSED_QUERY,
     case_sensitive=True,
 )
 def import_file(cur, arg=None, **_):
```

### Comparing `litecli-1.8.0/litecli/packages/special/favoritequeries.py` & `litecli-1.9.0/litecli/packages/special/favoritequeries.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/litecli/packages/special/iocommands.py` & `litecli-1.9.0/litecli/packages/special/iocommands.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/litecli/packages/special/main.py` & `litecli-1.9.0/litecli/packages/special/main.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/litecli/packages/special/utils.py` & `litecli-1.9.0/litecli/packages/special/utils.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/litecli/sqlcompleter.py` & `litecli-1.9.0/litecli/sqlcompleter.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/litecli/sqlexecute.py` & `litecli-1.9.0/litecli/sqlexecute.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,21 @@
         SELECT m.name as tableName, p.name as columnName
         FROM sqlite_master m
         LEFT OUTER JOIN pragma_table_info((m.name)) p ON m.name <> p.name
         WHERE m.type IN ('table','view') AND m.name NOT LIKE 'sqlite_%'
         ORDER BY tableName, columnName
     """
 
+    indexes_query = """
+        SELECT name
+        FROM sqlite_master
+        WHERE type = 'index' AND name NOT LIKE 'sqlite_%'
+        ORDER BY 1
+    """
+
     functions_query = '''SELECT ROUTINE_NAME FROM INFORMATION_SCHEMA.ROUTINES
     WHERE ROUTINE_TYPE="FUNCTION" AND ROUTINE_SCHEMA = "%s"'''
 
     def __init__(self, database):
         self.dbname = database
         self._server_type = None
         self.connection_id = None
```

### Comparing `litecli-1.8.0/litecli.egg-info/PKG-INFO` & `litecli-1.9.0/litecli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litecli
-Version: 1.8.0
+Version: 1.9.0
 Summary: CLI for SQLite Databases with auto-completion and syntax highlighting.
 Home-page: https://github.com/dbcli/litecli
 Author: dbcli
 Author-email: litecli-users@googlegroups.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `litecli-1.8.0/litecli.egg-info/SOURCES.txt` & `litecli-1.9.0/litecli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/release.py` & `litecli-1.9.0/release.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/setup.py` & `litecli-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/tasks.py` & `litecli-1.9.0/tasks.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/tests/conftest.py` & `litecli-1.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/tests/liteclirc` & `litecli-1.9.0/tests/liteclirc`

 * *Files 4% similar despite different names*

```diff
@@ -47,27 +47,35 @@
 # Emacs mode: Ctrl-A is home, Ctrl-E is end. All emacs keybindings are available in the REPL.
 # When Vi mode is enabled you can use modal editing features offered by Vi in the REPL.
 key_bindings = emacs
 
 # Enabling this option will show the suggestions in a wider menu. Thus more items are suggested.
 wider_completion_menu = False
 
+# Autocompletion is on by default. This can be truned off by setting this
+# option to False. Pressing tab will still trigger completion.
+autocompletion = True
+
 # litecli prompt
 # \D - The full current date
 # \d - Database name
 # \f - File basename of the "main" database
 # \m - Minutes of the current time
 # \n - Newline
 # \P - AM/PM
 # \R - The current time, in 24-hour military time (0-23)
 # \r - The current time, standard 12-hour time (1-12)
 # \s - Seconds of the current time
+# \x1b[...m - insert ANSI escape sequence
 prompt = "\t :\d> "
 prompt_continuation = "-> "
 
+# Show/hide the informational toolbar with function keymap at the footer.
+show_bottom_toolbar = True
+
 # Skip intro info on startup and outro info on exit
 less_chatty = False
 
 # Use alias from --login-path instead of host name in prompt
 login_path_as_host = False
 
 # Cause result sets to be displayed vertically if they are too wide for the current window,
```

### Comparing `litecli-1.8.0/tests/test_clistyle.py` & `litecli-1.9.0/tests/test_clistyle.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/tests/test_completion_engine.py` & `litecli-1.9.0/tests/test_completion_engine.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/tests/test_completion_refresher.py` & `litecli-1.9.0/tests/test_completion_refresher.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/tests/test_dbspecial.py` & `litecli-1.9.0/tests/test_dbspecial.py`

 * *Files 18% similar despite different names*

```diff
@@ -59,7 +59,18 @@
     assert "15 hours 14 min 50 sec" == format_uptime(seconds)
 
     seconds = 598244
     assert "6 days 22 hours 10 min 44 sec" == format_uptime(seconds)
 
     seconds = 522600
     assert "6 days 1 hour 10 min 0 sec" == format_uptime(seconds)
+
+
+def test_indexes():
+    suggestions = suggest_type(".indexes", ".indexes ")
+    assert sorted_dicts(suggestions) == sorted_dicts(
+        [
+            {"type": "table", "schema": []},
+            {"type": "view", "schema": []},
+            {"type": "schema"},
+        ]
+    )
```

### Comparing `litecli-1.8.0/tests/test_main.py` & `litecli-1.9.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/tests/test_parseutils.py` & `litecli-1.9.0/tests/test_parseutils.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/tests/test_smart_completion_public_schema_only.py` & `litecli-1.9.0/tests/test_smart_completion_public_schema_only.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/tests/test_sqlexecute.py` & `litecli-1.9.0/tests/test_sqlexecute.py`

 * *Files identical despite different names*

### Comparing `litecli-1.8.0/tests/utils.py` & `litecli-1.9.0/tests/utils.py`

 * *Files identical despite different names*


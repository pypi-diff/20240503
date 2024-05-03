# Comparing `tmp/unasync-0.5.0.tar.gz` & `tmp/unasync-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unasync-0.5.0.tar", last modified: Sun May  3 04:33:49 2020, max compression
+gzip compressed data, was "unasync-0.6.0.tar", last modified: Fri May  3 11:13:10 2024, max compression
```

## Comparing `unasync-0.5.0.tar` & `unasync-0.6.0.tar`

### file list

```diff
@@ -1,80 +1,83 @@
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:49.000000 unasync-0.5.0/
--rw-r--r--   0 quentin    (501) staff       (20)      113 2020-05-03 04:31:45.000000 unasync-0.5.0/.coveragerc
--rw-r--r--   0 quentin    (501) staff       (20)      185 2020-05-03 04:31:45.000000 unasync-0.5.0/LICENSE
--rw-r--r--   0 quentin    (501) staff       (20)    11358 2020-05-03 04:31:45.000000 unasync-0.5.0/LICENSE.APACHE2
--rw-r--r--   0 quentin    (501) staff       (20)     1046 2020-05-03 04:31:45.000000 unasync-0.5.0/LICENSE.MIT
--rw-r--r--   0 quentin    (501) staff       (20)      192 2020-05-03 04:31:45.000000 unasync-0.5.0/MANIFEST.in
--rw-r--r--   0 quentin    (501) staff       (20)     4377 2020-05-03 04:33:49.000000 unasync-0.5.0/PKG-INFO
--rw-r--r--   0 quentin    (501) staff       (20)     2555 2020-05-03 04:31:45.000000 unasync-0.5.0/README.rst
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:49.000000 unasync-0.5.0/docs/
--rw-r--r--   0 quentin    (501) staff       (20)      609 2020-05-03 04:31:45.000000 unasync-0.5.0/docs/Makefile
--rw-r--r--   0 quentin    (501) staff       (20)      779 2020-05-03 04:31:45.000000 unasync-0.5.0/docs/make.bat
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:49.000000 unasync-0.5.0/docs/source/
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:49.000000 unasync-0.5.0/docs/source/_static/
--rw-r--r--   0 quentin    (501) staff       (20)        0 2020-05-03 04:31:45.000000 unasync-0.5.0/docs/source/_static/.gitkeep
--rw-r--r--   0 quentin    (501) staff       (20)     5924 2020-05-03 04:31:45.000000 unasync-0.5.0/docs/source/conf.py
--rw-r--r--   0 quentin    (501) staff       (20)       94 2020-05-03 04:31:45.000000 unasync-0.5.0/docs/source/history.rst
--rw-r--r--   0 quentin    (501) staff       (20)     3046 2020-05-03 04:31:45.000000 unasync-0.5.0/docs/source/index.rst
--rw-r--r--   0 quentin    (501) staff       (20)      217 2020-05-03 04:31:45.000000 unasync-0.5.0/pyproject.toml
--rw-r--r--   0 quentin    (501) staff       (20)       38 2020-05-03 04:33:49.000000 unasync-0.5.0/setup.cfg
--rw-r--r--   0 quentin    (501) staff       (20)     1551 2020-05-03 04:31:45.000000 unasync-0.5.0/setup.py
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:48.000000 unasync-0.5.0/src/
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:49.000000 unasync-0.5.0/src/unasync/
--rw-r--r--   0 quentin    (501) staff       (20)     6823 2020-05-03 04:31:45.000000 unasync-0.5.0/src/unasync/__init__.py
--rw-r--r--   0 quentin    (501) staff       (20)       89 2020-05-03 04:31:45.000000 unasync-0.5.0/src/unasync/_version.py
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:49.000000 unasync-0.5.0/src/unasync.egg-info/
--rw-r--r--   0 quentin    (501) staff       (20)     4377 2020-05-03 04:33:48.000000 unasync-0.5.0/src/unasync.egg-info/PKG-INFO
--rw-r--r--   0 quentin    (501) staff       (20)     1875 2020-05-03 04:33:48.000000 unasync-0.5.0/src/unasync.egg-info/SOURCES.txt
--rw-r--r--   0 quentin    (501) staff       (20)        1 2020-05-03 04:33:48.000000 unasync-0.5.0/src/unasync.egg-info/dependency_links.txt
--rw-r--r--   0 quentin    (501) staff       (20)        8 2020-05-03 04:33:48.000000 unasync-0.5.0/src/unasync.egg-info/top_level.txt
--rw-r--r--   0 quentin    (501) staff       (20)       24 2020-05-03 04:31:45.000000 unasync-0.5.0/test-requirements.txt
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:49.000000 unasync-0.5.0/tests/
--rw-r--r--   0 quentin    (501) staff       (20)       36 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/conftest.py
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:48.000000 unasync-0.5.0/tests/data/
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:49.000000 unasync-0.5.0/tests/data/async/
--rw-r--r--   0 quentin    (501) staff       (20)      265 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/async/acontext.py
--rw-r--r--   0 quentin    (501) staff       (20)      145 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/async/aiter.py
--rw-r--r--   0 quentin    (501) staff       (20)      231 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/async/classes.py
--rw-r--r--   0 quentin    (501) staff       (20)      128 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/async/encoding.py
--rw-r--r--   0 quentin    (501) staff       (20)      367 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/async/simple.py
--rw-r--r--   0 quentin    (501) staff       (20)      100 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/async/typing.py
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:49.000000 unasync-0.5.0/tests/data/example_custom_pkg/
--rw-r--r--   0 quentin    (501) staff       (20)        0 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/example_custom_pkg/__init__.py
--rw-r--r--   0 quentin    (501) staff       (20)      725 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/example_custom_pkg/setup.py
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:48.000000 unasync-0.5.0/tests/data/example_custom_pkg/src/
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:49.000000 unasync-0.5.0/tests/data/example_custom_pkg/src/ahip/
--rw-r--r--   0 quentin    (501) staff       (20)       34 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/example_custom_pkg/src/ahip/__init__.py
--rw-r--r--   0 quentin    (501) staff       (20)       34 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/example_custom_pkg/src/ahip/another_file.py
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:49.000000 unasync-0.5.0/tests/data/example_custom_pkg/src/ahip/some_dir/
--rw-r--r--   0 quentin    (501) staff       (20)       34 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/example_custom_pkg/src/ahip/some_dir/__init__.py
--rw-r--r--   0 quentin    (501) staff       (20)       34 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/example_custom_pkg/src/ahip/some_dir/another_file.py
--rw-r--r--   0 quentin    (501) staff       (20)       34 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/example_custom_pkg/src/ahip/some_dir/some_file.py
--rw-r--r--   0 quentin    (501) staff       (20)       34 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/example_custom_pkg/src/ahip/some_file.py
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:49.000000 unasync-0.5.0/tests/data/example_custom_pkg/src/ahip/tests/
--rw-r--r--   0 quentin    (501) staff       (20)        0 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/example_custom_pkg/src/ahip/tests/__init__.py
--rw-r--r--   0 quentin    (501) staff       (20)      101 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/example_custom_pkg/src/ahip/tests/test_conn.py
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:49.000000 unasync-0.5.0/tests/data/example_mod/
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:49.000000 unasync-0.5.0/tests/data/example_mod/_async/
--rw-r--r--   0 quentin    (501) staff       (20)       34 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/example_mod/_async/some_file.py
--rw-r--r--   0 quentin    (501) staff       (20)      360 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/example_mod/setup.py
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:49.000000 unasync-0.5.0/tests/data/example_pkg/
--rw-r--r--   0 quentin    (501) staff       (20)      435 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/example_pkg/setup.py
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:48.000000 unasync-0.5.0/tests/data/example_pkg/src/
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:49.000000 unasync-0.5.0/tests/data/example_pkg/src/example_pkg/
--rw-r--r--   0 quentin    (501) staff       (20)       21 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/example_pkg/src/example_pkg/__init__.py
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:49.000000 unasync-0.5.0/tests/data/example_pkg/src/example_pkg/_async/
--rw-r--r--   0 quentin    (501) staff       (20)       34 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/example_pkg/src/example_pkg/_async/__init__.py
--rw-r--r--   0 quentin    (501) staff       (20)       34 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/example_pkg/src/example_pkg/_async/another_file.py
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:49.000000 unasync-0.5.0/tests/data/example_pkg/src/example_pkg/_async/some_dir/
--rw-r--r--   0 quentin    (501) staff       (20)       34 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/example_pkg/src/example_pkg/_async/some_dir/__init__.py
--rw-r--r--   0 quentin    (501) staff       (20)       34 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/example_pkg/src/example_pkg/_async/some_dir/another_file.py
--rw-r--r--   0 quentin    (501) staff       (20)       34 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/example_pkg/src/example_pkg/_async/some_dir/some_file.py
--rw-r--r--   0 quentin    (501) staff       (20)       34 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/example_pkg/src/example_pkg/_async/some_file.py
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2020-05-03 04:33:49.000000 unasync-0.5.0/tests/data/sync/
--rw-r--r--   0 quentin    (501) staff       (20)      229 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/sync/acontext.py
--rw-r--r--   0 quentin    (501) staff       (20)      120 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/sync/aiter.py
--rw-r--r--   0 quentin    (501) staff       (20)      214 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/sync/classes.py
--rw-r--r--   0 quentin    (501) staff       (20)      128 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/sync/encoding.py
--rw-r--r--   0 quentin    (501) staff       (20)      337 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/sync/simple.py
--rw-r--r--   0 quentin    (501) staff       (20)       85 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/data/sync/typing.py
--rw-r--r--   0 quentin    (501) staff       (20)     4768 2020-05-03 04:31:45.000000 unasync-0.5.0/tests/test_unasync.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.233257 unasync-0.6.0/
+-rw-r--r--   0 q         (1000) q         (1000)      113 2024-05-03 07:18:38.000000 unasync-0.6.0/.coveragerc
+-rw-r--r--   0 q         (1000) q         (1000)      185 2024-05-03 07:18:38.000000 unasync-0.6.0/LICENSE
+-rw-r--r--   0 q         (1000) q         (1000)    11358 2024-05-03 07:18:38.000000 unasync-0.6.0/LICENSE.APACHE2
+-rw-r--r--   0 q         (1000) q         (1000)     1046 2024-05-03 07:18:38.000000 unasync-0.6.0/LICENSE.MIT
+-rw-r--r--   0 q         (1000) q         (1000)      192 2024-05-03 07:18:38.000000 unasync-0.6.0/MANIFEST.in
+-rw-r--r--   0 q         (1000) q         (1000)     3961 2024-05-03 11:13:10.233257 unasync-0.6.0/PKG-INFO
+-rw-r--r--   0 q         (1000) q         (1000)     2831 2024-05-03 07:18:38.000000 unasync-0.6.0/README.rst
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.227257 unasync-0.6.0/docs/
+-rw-r--r--   0 q         (1000) q         (1000)      609 2024-05-03 07:18:38.000000 unasync-0.6.0/docs/Makefile
+-rw-r--r--   0 q         (1000) q         (1000)      779 2024-05-03 07:18:38.000000 unasync-0.6.0/docs/make.bat
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.227257 unasync-0.6.0/docs/source/
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.227257 unasync-0.6.0/docs/source/_static/
+-rw-r--r--   0 q         (1000) q         (1000)        0 2024-05-03 07:18:38.000000 unasync-0.6.0/docs/source/_static/.gitkeep
+-rw-r--r--   0 q         (1000) q         (1000)     5900 2024-05-03 07:18:38.000000 unasync-0.6.0/docs/source/conf.py
+-rw-r--r--   0 q         (1000) q         (1000)      366 2024-05-03 11:01:53.000000 unasync-0.6.0/docs/source/history.rst
+-rw-r--r--   0 q         (1000) q         (1000)     3046 2024-05-03 07:18:38.000000 unasync-0.6.0/docs/source/index.rst
+-rw-r--r--   0 q         (1000) q         (1000)      217 2024-05-03 07:18:38.000000 unasync-0.6.0/pyproject.toml
+-rw-r--r--   0 q         (1000) q         (1000)       38 2024-05-03 11:13:10.233257 unasync-0.6.0/setup.cfg
+-rw-r--r--   0 q         (1000) q         (1000)     1411 2024-05-03 10:55:28.000000 unasync-0.6.0/setup.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.225257 unasync-0.6.0/src/
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.228257 unasync-0.6.0/src/unasync/
+-rw-r--r--   0 q         (1000) q         (1000)     5601 2024-05-03 07:34:48.000000 unasync-0.6.0/src/unasync/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)       89 2024-05-03 10:56:25.000000 unasync-0.6.0/src/unasync/_version.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.233257 unasync-0.6.0/src/unasync.egg-info/
+-rw-r--r--   0 q         (1000) q         (1000)     3961 2024-05-03 11:13:10.000000 unasync-0.6.0/src/unasync.egg-info/PKG-INFO
+-rw-r--r--   0 q         (1000) q         (1000)     1964 2024-05-03 11:13:10.000000 unasync-0.6.0/src/unasync.egg-info/SOURCES.txt
+-rw-r--r--   0 q         (1000) q         (1000)        1 2024-05-03 11:13:10.000000 unasync-0.6.0/src/unasync.egg-info/dependency_links.txt
+-rw-r--r--   0 q         (1000) q         (1000)       23 2024-05-03 11:13:10.000000 unasync-0.6.0/src/unasync.egg-info/requires.txt
+-rw-r--r--   0 q         (1000) q         (1000)        8 2024-05-03 11:13:10.000000 unasync-0.6.0/src/unasync.egg-info/top_level.txt
+-rw-r--r--   0 q         (1000) q         (1000)       24 2024-05-03 07:18:38.000000 unasync-0.6.0/test-requirements.txt
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.228257 unasync-0.6.0/tests/
+-rw-r--r--   0 q         (1000) q         (1000)       36 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/conftest.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.226257 unasync-0.6.0/tests/data/
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.229257 unasync-0.6.0/tests/data/async/
+-rw-r--r--   0 q         (1000) q         (1000)      265 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/async/acontext.py
+-rw-r--r--   0 q         (1000) q         (1000)      145 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/async/aiter.py
+-rw-r--r--   0 q         (1000) q         (1000)      215 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/async/classes.py
+-rw-r--r--   0 q         (1000) q         (1000)      128 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/async/encoding.py
+-rw-r--r--   0 q         (1000) q         (1000)       67 2024-05-03 07:19:40.000000 unasync-0.6.0/tests/data/async/fstring.py
+-rw-r--r--   0 q         (1000) q         (1000)      367 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/async/simple.py
+-rw-r--r--   0 q         (1000) q         (1000)      100 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/async/typing.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.230257 unasync-0.6.0/tests/data/example_custom_pkg/
+-rw-r--r--   0 q         (1000) q         (1000)        0 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/example_custom_pkg/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)      725 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/example_custom_pkg/setup.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.225257 unasync-0.6.0/tests/data/example_custom_pkg/src/
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.230257 unasync-0.6.0/tests/data/example_custom_pkg/src/ahip/
+-rw-r--r--   0 q         (1000) q         (1000)       34 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/example_custom_pkg/src/ahip/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)       34 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/example_custom_pkg/src/ahip/another_file.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.230257 unasync-0.6.0/tests/data/example_custom_pkg/src/ahip/some_dir/
+-rw-r--r--   0 q         (1000) q         (1000)       34 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/example_custom_pkg/src/ahip/some_dir/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)       34 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/example_custom_pkg/src/ahip/some_dir/another_file.py
+-rw-r--r--   0 q         (1000) q         (1000)       34 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/example_custom_pkg/src/ahip/some_dir/some_file.py
+-rw-r--r--   0 q         (1000) q         (1000)       34 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/example_custom_pkg/src/ahip/some_file.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.231258 unasync-0.6.0/tests/data/example_custom_pkg/src/ahip/tests/
+-rw-r--r--   0 q         (1000) q         (1000)        0 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/example_custom_pkg/src/ahip/tests/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)      101 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/example_custom_pkg/src/ahip/tests/test_conn.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.231258 unasync-0.6.0/tests/data/example_mod/
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.231258 unasync-0.6.0/tests/data/example_mod/_async/
+-rw-r--r--   0 q         (1000) q         (1000)       34 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/example_mod/_async/some_file.py
+-rw-r--r--   0 q         (1000) q         (1000)      360 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/example_mod/setup.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.231258 unasync-0.6.0/tests/data/example_pkg/
+-rw-r--r--   0 q         (1000) q         (1000)      435 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/example_pkg/setup.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.225257 unasync-0.6.0/tests/data/example_pkg/src/
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.231258 unasync-0.6.0/tests/data/example_pkg/src/example_pkg/
+-rw-r--r--   0 q         (1000) q         (1000)       21 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/example_pkg/src/example_pkg/__init__.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.231258 unasync-0.6.0/tests/data/example_pkg/src/example_pkg/_async/
+-rw-r--r--   0 q         (1000) q         (1000)       34 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/example_pkg/src/example_pkg/_async/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)       34 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/example_pkg/src/example_pkg/_async/another_file.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.232257 unasync-0.6.0/tests/data/example_pkg/src/example_pkg/_async/some_dir/
+-rw-r--r--   0 q         (1000) q         (1000)       34 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/example_pkg/src/example_pkg/_async/some_dir/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)       34 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/example_pkg/src/example_pkg/_async/some_dir/another_file.py
+-rw-r--r--   0 q         (1000) q         (1000)       34 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/example_pkg/src/example_pkg/_async/some_dir/some_file.py
+-rw-r--r--   0 q         (1000) q         (1000)       34 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/example_pkg/src/example_pkg/_async/some_file.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2024-05-03 11:13:10.233257 unasync-0.6.0/tests/data/sync/
+-rw-r--r--   0 q         (1000) q         (1000)      229 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/sync/acontext.py
+-rw-r--r--   0 q         (1000) q         (1000)      120 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/sync/aiter.py
+-rw-r--r--   0 q         (1000) q         (1000)      198 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/sync/classes.py
+-rw-r--r--   0 q         (1000) q         (1000)      128 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/sync/encoding.py
+-rw-r--r--   0 q         (1000) q         (1000)       67 2024-05-03 07:59:50.000000 unasync-0.6.0/tests/data/sync/fstring.py
+-rw-r--r--   0 q         (1000) q         (1000)      337 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/sync/simple.py
+-rw-r--r--   0 q         (1000) q         (1000)       85 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/data/sync/typing.py
+-rw-r--r--   0 q         (1000) q         (1000)     4876 2024-05-03 07:18:38.000000 unasync-0.6.0/tests/test_unasync.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `unasync-0.5.0/LICENSE.APACHE2` & `unasync-0.6.0/LICENSE.APACHE2`

 * *Files identical despite different names*

### Comparing `unasync-0.5.0/LICENSE.MIT` & `unasync-0.6.0/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `unasync-0.5.0/PKG-INFO` & `unasync-0.6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,108 +1,117 @@
 Metadata-Version: 2.1
 Name: unasync
-Version: 0.5.0
+Version: 0.6.0
 Summary: The async transformation code.
 Home-page: https://github.com/python-trio/unasync
 Author: Ratan Kulshreshtha
 Author-email: ratan.shreshtha@gmail.com
-License: MIT -or- Apache License 2.0
-Description: unasync
-        =======
-        
-        |documentation| |travis| |appveyor| |codecov|
-        
-        .. |travis| image:: https://travis-ci.com/python-trio/unasync.svg?branch=master
-            :alt: Travis Build Status
-            :target: https://travis-ci.com/python-trio/unasync
-        
-        .. |appveyor| image:: https://ci.appveyor.com/api/projects/status/ovhaitunqmdd6n44/branch/master?svg=true
-            :alt: AppVeyor Build Status
-            :target: https://ci.appveyor.com/project/njsmith/unasync
-        
-        .. |codecov| image:: https://codecov.io/gh/python-trio/unasync/branch/master/graph/badge.svg
-            :alt: Coverage Status
-            :target: https://codecov.io/gh/python-trio/unasync
-        
-        .. |documentation| image:: https://readthedocs.org/projects/unasync/badge/?version=latest
-            :alt: Documentation Status
-            :target: https://unasync.readthedocs.io/en/latest/?badge=latest
-        
-        
-        Welcome to `unasync <https://pypi.org/project/unasync/>`_, a project that can transform your asynchronous code into synchronous code.
-        
-        *Why are we doing it?* - `urllib3/urllib3#1335 <https://github.com/urllib3/urllib3/pull/1335/>`_
-        
-        Installation
-        ============
-        
-        ::
-        
-            pip install unasync
-        
-        Usage
-        =====
-        
-        To use the unasync project you need to install the package and then create a **_async** folder where you will place the asynchronous code that you want to transform into synchronous code.
-        
-        And then in your :code:`setup.py` place the following code.
-        
-        .. code-block:: python
-        
-            import unasync
-        
-            setuptools.setup(
-                ...
-                cmdclass={'build_py': unasync.cmdclass_build_py()},
-                ...
-            )
-        
-        And when you will build your package you will get your synchronous code in **_sync** folder.
-        
-        If you'd like to customize where certain rules are applied you can pass
-        customized :code:`unasync.Rule` instances to :code:`unasync.cmdclass_build_py()`
-        
-        .. code-block:: python
-        
-            import unasync
-        
-            setuptools.setup(
-                ...
-                cmdclass={'build_py': unasync.cmdclass_build_py(rules=[
-                    # This rule transforms files within 'ahip' -> 'hip'
-                    # instead of the default '_async' -> '_sync'.
-                    unasync.Rule("/ahip/", "/hip/"),
-        
-                    # This rule's 'fromdir' is more specific so will take precedent
-                    # over the above rule if the path is within /ahip/tests/...
-                    # This rule adds an additional token replacement over the default replacements.
-                    unasync.Rule("/ahip/tests/", "/hip/tests/", additional_replacements={"ahip": "hip"}),
-                ])},
-                ...
-            )
-        
-        Documentation
-        =============
-        
-        https://unasync.readthedocs.io/en/latest/
-        
-        License: Your choice of MIT or Apache License 2.0
-        
+License: MIT OR Apache-2.0
 Keywords: async
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Framework :: Trio
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, <4
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: LICENSE.APACHE2
+License-File: LICENSE.MIT
+Requires-Dist: tokenize_rt
+Requires-Dist: setuptools
+
+unasync
+=======
+
+|documentation| |travis| |appveyor| |codecov|
+
+.. |travis| image:: https://travis-ci.com/python-trio/unasync.svg?branch=master
+    :alt: Travis Build Status
+    :target: https://travis-ci.com/python-trio/unasync
+
+.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/ovhaitunqmdd6n44/branch/master?svg=true
+    :alt: AppVeyor Build Status
+    :target: https://ci.appveyor.com/project/njsmith/unasync
+
+.. |codecov| image:: https://codecov.io/gh/python-trio/unasync/branch/master/graph/badge.svg
+    :alt: Coverage Status
+    :target: https://codecov.io/gh/python-trio/unasync
+
+.. |documentation| image:: https://readthedocs.org/projects/unasync/badge/?version=latest
+    :alt: Documentation Status
+    :target: https://unasync.readthedocs.io/en/latest/?badge=latest
+
+
+Welcome to `unasync <https://pypi.org/project/unasync/>`_, a project that can transform your asynchronous code into synchronous code.
+
+See https://github.com/urllib3/urllib3/issues/1323 for more details about unasync.
+
+Users
+=====
+
+ * The official Elasticsearch Python client: https://github.com/elastic/elasticsearch-py
+ * Hip, a HTTP client: https://github.com/python-trio/hip
+ * httpcore, another low-level HTTP client uses a different implementation of the same idea: https://github.com/encode/httpcore
+ 
+Installation
+============
+
+::
+
+    pip install unasync
+
+Usage
+=====
+
+To use the unasync project you need to install the package and then create a **_async** folder where you will place the asynchronous code that you want to transform into synchronous code.
+
+And then in your :code:`setup.py` place the following code.
+
+.. code-block:: python
+
+    import unasync
+
+    setuptools.setup(
+        ...
+        cmdclass={'build_py': unasync.cmdclass_build_py()},
+        ...
+    )
+
+And when you will build your package you will get your synchronous code in **_sync** folder.
+
+If you'd like to customize where certain rules are applied you can pass
+customized :code:`unasync.Rule` instances to :code:`unasync.cmdclass_build_py()`
+
+.. code-block:: python
+
+    import unasync
+
+    setuptools.setup(
+        ...
+        cmdclass={'build_py': unasync.cmdclass_build_py(rules=[
+            # This rule transforms files within 'ahip' -> 'hip'
+            # instead of the default '_async' -> '_sync'.
+            unasync.Rule("/ahip/", "/hip/"),
+
+            # This rule's 'fromdir' is more specific so will take precedent
+            # over the above rule if the path is within /ahip/tests/...
+            # This rule adds an additional token replacement over the default replacements.
+            unasync.Rule("/ahip/tests/", "/hip/tests/", additional_replacements={"ahip": "hip"}),
+        ])},
+        ...
+    )
+
+Documentation
+=============
+
+https://unasync.readthedocs.io/en/latest/
+
+License: Your choice of MIT or Apache License 2.0
```

### Comparing `unasync-0.5.0/README.rst` & `unasync-0.6.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -18,16 +18,23 @@
 .. |documentation| image:: https://readthedocs.org/projects/unasync/badge/?version=latest
     :alt: Documentation Status
     :target: https://unasync.readthedocs.io/en/latest/?badge=latest
 
 
 Welcome to `unasync <https://pypi.org/project/unasync/>`_, a project that can transform your asynchronous code into synchronous code.
 
-*Why are we doing it?* - `urllib3/urllib3#1335 <https://github.com/urllib3/urllib3/pull/1335/>`_
+See https://github.com/urllib3/urllib3/issues/1323 for more details about unasync.
 
+Users
+=====
+
+ * The official Elasticsearch Python client: https://github.com/elastic/elasticsearch-py
+ * Hip, a HTTP client: https://github.com/python-trio/hip
+ * httpcore, another low-level HTTP client uses a different implementation of the same idea: https://github.com/encode/httpcore
+ 
 Installation
 ============
 
 ::
 
     pip install unasync
```

### Comparing `unasync-0.5.0/docs/Makefile` & `unasync-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `unasync-0.5.0/docs/make.bat` & `unasync-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `unasync-0.5.0/docs/source/conf.py` & `unasync-0.6.0/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 #
 # Documentation build configuration file, created by
 # sphinx-quickstart on Sat Jan 21 19:11:14 2017.
 #
 # This file is execfile()d with the current directory set to its
 # containing dir.
 #
```

### Comparing `unasync-0.5.0/docs/source/index.rst` & `unasync-0.6.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `unasync-0.5.0/setup.py` & `unasync-0.6.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,38 @@
-import io
+from setuptools import find_packages, setup
 
-from setuptools import setup, find_packages
+exec(open("src/unasync/_version.py", encoding="utf-8").read())
 
-exec(io.open("src/unasync/_version.py", encoding="utf-8").read())
-
-LONG_DESC = io.open("README.rst", encoding="utf-8").read()
+LONG_DESC = open("README.rst", encoding="utf-8").read()
 
 setup(
     name="unasync",
     version=__version__,
     description="The async transformation code.",
     url="https://github.com/python-trio/unasync",
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
     author="Ratan Kulshreshtha",
     author_email="ratan.shreshtha@gmail.com",
-    license="MIT -or- Apache License 2.0",
+    license="MIT OR Apache-2.0",
     include_package_data=True,
     packages=find_packages("src"),
     package_dir={"": "src"},
-    install_requires=[],
+    install_requires=["tokenize_rt", "setuptools"],
     keywords=["async"],
-    python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, <4",
+    python_requires=">=3.8",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "License :: OSI Approved :: Apache Software License",
         "Framework :: Trio",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
 )
```

### Comparing `unasync-0.5.0/src/unasync.egg-info/PKG-INFO` & `unasync-0.6.0/src/unasync.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,108 +1,117 @@
 Metadata-Version: 2.1
 Name: unasync
-Version: 0.5.0
+Version: 0.6.0
 Summary: The async transformation code.
 Home-page: https://github.com/python-trio/unasync
 Author: Ratan Kulshreshtha
 Author-email: ratan.shreshtha@gmail.com
-License: MIT -or- Apache License 2.0
-Description: unasync
-        =======
-        
-        |documentation| |travis| |appveyor| |codecov|
-        
-        .. |travis| image:: https://travis-ci.com/python-trio/unasync.svg?branch=master
-            :alt: Travis Build Status
-            :target: https://travis-ci.com/python-trio/unasync
-        
-        .. |appveyor| image:: https://ci.appveyor.com/api/projects/status/ovhaitunqmdd6n44/branch/master?svg=true
-            :alt: AppVeyor Build Status
-            :target: https://ci.appveyor.com/project/njsmith/unasync
-        
-        .. |codecov| image:: https://codecov.io/gh/python-trio/unasync/branch/master/graph/badge.svg
-            :alt: Coverage Status
-            :target: https://codecov.io/gh/python-trio/unasync
-        
-        .. |documentation| image:: https://readthedocs.org/projects/unasync/badge/?version=latest
-            :alt: Documentation Status
-            :target: https://unasync.readthedocs.io/en/latest/?badge=latest
-        
-        
-        Welcome to `unasync <https://pypi.org/project/unasync/>`_, a project that can transform your asynchronous code into synchronous code.
-        
-        *Why are we doing it?* - `urllib3/urllib3#1335 <https://github.com/urllib3/urllib3/pull/1335/>`_
-        
-        Installation
-        ============
-        
-        ::
-        
-            pip install unasync
-        
-        Usage
-        =====
-        
-        To use the unasync project you need to install the package and then create a **_async** folder where you will place the asynchronous code that you want to transform into synchronous code.
-        
-        And then in your :code:`setup.py` place the following code.
-        
-        .. code-block:: python
-        
-            import unasync
-        
-            setuptools.setup(
-                ...
-                cmdclass={'build_py': unasync.cmdclass_build_py()},
-                ...
-            )
-        
-        And when you will build your package you will get your synchronous code in **_sync** folder.
-        
-        If you'd like to customize where certain rules are applied you can pass
-        customized :code:`unasync.Rule` instances to :code:`unasync.cmdclass_build_py()`
-        
-        .. code-block:: python
-        
-            import unasync
-        
-            setuptools.setup(
-                ...
-                cmdclass={'build_py': unasync.cmdclass_build_py(rules=[
-                    # This rule transforms files within 'ahip' -> 'hip'
-                    # instead of the default '_async' -> '_sync'.
-                    unasync.Rule("/ahip/", "/hip/"),
-        
-                    # This rule's 'fromdir' is more specific so will take precedent
-                    # over the above rule if the path is within /ahip/tests/...
-                    # This rule adds an additional token replacement over the default replacements.
-                    unasync.Rule("/ahip/tests/", "/hip/tests/", additional_replacements={"ahip": "hip"}),
-                ])},
-                ...
-            )
-        
-        Documentation
-        =============
-        
-        https://unasync.readthedocs.io/en/latest/
-        
-        License: Your choice of MIT or Apache License 2.0
-        
+License: MIT OR Apache-2.0
 Keywords: async
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Framework :: Trio
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, <4
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: LICENSE.APACHE2
+License-File: LICENSE.MIT
+Requires-Dist: tokenize_rt
+Requires-Dist: setuptools
+
+unasync
+=======
+
+|documentation| |travis| |appveyor| |codecov|
+
+.. |travis| image:: https://travis-ci.com/python-trio/unasync.svg?branch=master
+    :alt: Travis Build Status
+    :target: https://travis-ci.com/python-trio/unasync
+
+.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/ovhaitunqmdd6n44/branch/master?svg=true
+    :alt: AppVeyor Build Status
+    :target: https://ci.appveyor.com/project/njsmith/unasync
+
+.. |codecov| image:: https://codecov.io/gh/python-trio/unasync/branch/master/graph/badge.svg
+    :alt: Coverage Status
+    :target: https://codecov.io/gh/python-trio/unasync
+
+.. |documentation| image:: https://readthedocs.org/projects/unasync/badge/?version=latest
+    :alt: Documentation Status
+    :target: https://unasync.readthedocs.io/en/latest/?badge=latest
+
+
+Welcome to `unasync <https://pypi.org/project/unasync/>`_, a project that can transform your asynchronous code into synchronous code.
+
+See https://github.com/urllib3/urllib3/issues/1323 for more details about unasync.
+
+Users
+=====
+
+ * The official Elasticsearch Python client: https://github.com/elastic/elasticsearch-py
+ * Hip, a HTTP client: https://github.com/python-trio/hip
+ * httpcore, another low-level HTTP client uses a different implementation of the same idea: https://github.com/encode/httpcore
+ 
+Installation
+============
+
+::
+
+    pip install unasync
+
+Usage
+=====
+
+To use the unasync project you need to install the package and then create a **_async** folder where you will place the asynchronous code that you want to transform into synchronous code.
+
+And then in your :code:`setup.py` place the following code.
+
+.. code-block:: python
+
+    import unasync
+
+    setuptools.setup(
+        ...
+        cmdclass={'build_py': unasync.cmdclass_build_py()},
+        ...
+    )
+
+And when you will build your package you will get your synchronous code in **_sync** folder.
+
+If you'd like to customize where certain rules are applied you can pass
+customized :code:`unasync.Rule` instances to :code:`unasync.cmdclass_build_py()`
+
+.. code-block:: python
+
+    import unasync
+
+    setuptools.setup(
+        ...
+        cmdclass={'build_py': unasync.cmdclass_build_py(rules=[
+            # This rule transforms files within 'ahip' -> 'hip'
+            # instead of the default '_async' -> '_sync'.
+            unasync.Rule("/ahip/", "/hip/"),
+
+            # This rule's 'fromdir' is more specific so will take precedent
+            # over the above rule if the path is within /ahip/tests/...
+            # This rule adds an additional token replacement over the default replacements.
+            unasync.Rule("/ahip/tests/", "/hip/tests/", additional_replacements={"ahip": "hip"}),
+        ])},
+        ...
+    )
+
+Documentation
+=============
+
+https://unasync.readthedocs.io/en/latest/
+
+License: Your choice of MIT or Apache License 2.0
```

### Comparing `unasync-0.5.0/src/unasync.egg-info/SOURCES.txt` & `unasync-0.6.0/src/unasync.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 docs/source/index.rst
 docs/source/_static/.gitkeep
 src/unasync/__init__.py
 src/unasync/_version.py
 src/unasync.egg-info/PKG-INFO
 src/unasync.egg-info/SOURCES.txt
 src/unasync.egg-info/dependency_links.txt
+src/unasync.egg-info/requires.txt
 src/unasync.egg-info/top_level.txt
 tests/conftest.py
 tests/test_unasync.py
 tests/data/async/acontext.py
 tests/data/async/aiter.py
 tests/data/async/classes.py
 tests/data/async/encoding.py
+tests/data/async/fstring.py
 tests/data/async/simple.py
 tests/data/async/typing.py
 tests/data/example_custom_pkg/__init__.py
 tests/data/example_custom_pkg/setup.py
 tests/data/example_custom_pkg/src/ahip/__init__.py
 tests/data/example_custom_pkg/src/ahip/another_file.py
 tests/data/example_custom_pkg/src/ahip/some_file.py
@@ -47,9 +49,10 @@
 tests/data/example_pkg/src/example_pkg/_async/some_dir/__init__.py
 tests/data/example_pkg/src/example_pkg/_async/some_dir/another_file.py
 tests/data/example_pkg/src/example_pkg/_async/some_dir/some_file.py
 tests/data/sync/acontext.py
 tests/data/sync/aiter.py
 tests/data/sync/classes.py
 tests/data/sync/encoding.py
+tests/data/sync/fstring.py
 tests/data/sync/simple.py
 tests/data/sync/typing.py
```

### Comparing `unasync-0.5.0/tests/data/example_custom_pkg/setup.py` & `unasync-0.6.0/tests/data/example_custom_pkg/setup.py`

 * *Files identical despite different names*

### Comparing `unasync-0.5.0/tests/test_unasync.py` & `unasync-0.6.0/tests/test_unasync.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import copy
-import io
+import errno
 import os
 import shutil
 import subprocess
 
 import pytest
 
 import unasync
 
 TEST_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "data")
 ASYNC_DIR = os.path.join(TEST_DIR, "async")
 SYNC_DIR = os.path.join(TEST_DIR, "sync")
-TEST_FILES = sorted([f for f in os.listdir(ASYNC_DIR) if f.endswith(".py")])
+TEST_FILES = sorted(f for f in os.listdir(ASYNC_DIR) if f.endswith(".py"))
 
 
 def list_files(startpath):
     output = ""
     for root, dirs, files in os.walk(startpath):
         level = root.replace(startpath, "").count(os.sep)
         indent = " " * 4 * (level)
-        output += "{}{}/".format(indent, os.path.basename(root))
+        output += f"{indent}{os.path.basename(root)}/"
         output += "\n"
         subindent = " " * 4 * (level + 1)
         for f in files:
-            output += "{}{}".format(subindent, f)
+            output += f"{subindent}{f}"
             output += "\n"
     return output
 
 
 def test_rule_on_short_path():
     rule = unasync.Rule("/ahip/tests/", "/hip/tests/")
     assert rule._match("/ahip/") is False
@@ -36,46 +36,48 @@
 @pytest.mark.parametrize("source_file", TEST_FILES)
 def test_unasync(tmpdir, source_file):
 
     rule = unasync.Rule(fromdir=ASYNC_DIR, todir=str(tmpdir))
     rule._unasync_file(os.path.join(ASYNC_DIR, source_file))
 
     encoding = "latin-1" if "encoding" in source_file else "utf-8"
-    with io.open(os.path.join(SYNC_DIR, source_file), encoding=encoding) as f:
+    with open(os.path.join(SYNC_DIR, source_file), encoding=encoding) as f:
         truth = f.read()
-    with io.open(os.path.join(str(tmpdir), source_file), encoding=encoding) as f:
+    with open(os.path.join(str(tmpdir), source_file), encoding=encoding) as f:
         unasynced_code = f.read()
         assert unasynced_code == truth
 
 
 def test_unasync_files(tmpdir):
     """Test the unasync_files API, not tied by a Rule or to setuptools."""
     unasync.unasync_files(
         [os.path.join(ASYNC_DIR, fpath) for fpath in TEST_FILES],
         rules=[unasync.Rule(fromdir=ASYNC_DIR, todir=str(tmpdir))],
     )
 
     for source_file in TEST_FILES:
         encoding = "latin-1" if "encoding" in source_file else "utf-8"
-        with io.open(os.path.join(SYNC_DIR, source_file), encoding=encoding) as f:
+        with open(os.path.join(SYNC_DIR, source_file), encoding=encoding) as f:
             truth = f.read()
-        with io.open(os.path.join(str(tmpdir), source_file), encoding=encoding) as f:
+        with open(os.path.join(str(tmpdir), source_file), encoding=encoding) as f:
             unasynced_code = f.read()
             assert unasynced_code == truth
 
 
 def test_build_py_modules(tmpdir):
 
     source_modules_dir = os.path.join(TEST_DIR, "example_mod")
     mod_dir = str(tmpdir) + "/" + "example_mod"
     shutil.copytree(source_modules_dir, mod_dir)
 
     env = copy.copy(os.environ)
     env["PYTHONPATH"] = os.path.realpath(os.path.join(TEST_DIR, ".."))
     subprocess.check_call(["python", "setup.py", "build"], cwd=mod_dir, env=env)
+    # Calling it twice to test the "if not copied" branch
+    subprocess.check_call(["python", "setup.py", "build"], cwd=mod_dir, env=env)
 
     unasynced = os.path.join(mod_dir, "build/lib/_sync/some_file.py")
     tree_build_dir = list_files(mod_dir)
 
     with open(unasynced) as f:
         unasynced_code = f.read()
         assert unasynced_code == "def f():\n    return 1\n"
```


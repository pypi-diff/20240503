# Comparing `tmp/plover_retro_untranslator-0.4.0.tar.gz` & `tmp/plover_retro_untranslator-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plover_retro_untranslator-0.4.0.tar", last modified: Wed Apr 17 11:24:36 2024, max compression
+gzip compressed data, was "dist/plover_retro_untranslator-0.4.1.tar", last modified: Fri May  3 12:10:31 2024, max compression
```

## Comparing `plover_retro_untranslator-0.4.0.tar` & `plover_retro_untranslator-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 josiah    (1000) josiah    (1000)        0 2024-04-17 11:24:36.806272 plover_retro_untranslator-0.4.0/
--rw-r--r--   0 josiah    (1000) josiah    (1000)    32406 2024-04-17 10:00:41.000000 plover_retro_untranslator-0.4.0/LICENSE
--rw-r--r--   0 josiah    (1000) josiah    (1000)     3601 2024-04-17 11:24:36.806272 plover_retro_untranslator-0.4.0/PKG-INFO
--rw-r--r--   0 josiah    (1000) josiah    (1000)     2598 2024-04-17 11:19:05.000000 plover_retro_untranslator-0.4.0/README.md
-drwxr-xr-x   0 josiah    (1000) josiah    (1000)        0 2024-04-17 11:24:36.806272 plover_retro_untranslator-0.4.0/plover_retro_untranslator/
--rw-r--r--   0 josiah    (1000) josiah    (1000)     3071 2024-04-17 11:08:50.000000 plover_retro_untranslator-0.4.0/plover_retro_untranslator/__init__.py
--rw-r--r--   0 josiah    (1000) josiah    (1000)     2146 2024-04-17 11:06:45.000000 plover_retro_untranslator-0.4.0/plover_retro_untranslator/spelling_converter.py
-drwxr-xr-x   0 josiah    (1000) josiah    (1000)        0 2024-04-17 11:24:36.806272 plover_retro_untranslator-0.4.0/plover_retro_untranslator.egg-info/
--rw-r--r--   0 josiah    (1000) josiah    (1000)     3601 2024-04-17 11:24:36.000000 plover_retro_untranslator-0.4.0/plover_retro_untranslator.egg-info/PKG-INFO
--rw-r--r--   0 josiah    (1000) josiah    (1000)      462 2024-04-17 11:24:36.000000 plover_retro_untranslator-0.4.0/plover_retro_untranslator.egg-info/SOURCES.txt
--rw-r--r--   0 josiah    (1000) josiah    (1000)        1 2024-04-17 11:24:36.000000 plover_retro_untranslator-0.4.0/plover_retro_untranslator.egg-info/dependency_links.txt
--rw-r--r--   0 josiah    (1000) josiah    (1000)       81 2024-04-17 11:24:36.000000 plover_retro_untranslator-0.4.0/plover_retro_untranslator.egg-info/entry_points.txt
--rw-r--r--   0 josiah    (1000) josiah    (1000)       30 2024-04-17 11:24:36.000000 plover_retro_untranslator-0.4.0/plover_retro_untranslator.egg-info/requires.txt
--rw-r--r--   0 josiah    (1000) josiah    (1000)       26 2024-04-17 11:24:36.000000 plover_retro_untranslator-0.4.0/plover_retro_untranslator.egg-info/top_level.txt
--rw-r--r--   0 josiah    (1000) josiah    (1000)        1 2024-04-17 10:02:30.000000 plover_retro_untranslator-0.4.0/plover_retro_untranslator.egg-info/zip-safe
--rw-r--r--   0 josiah    (1000) josiah    (1000)     1150 2024-04-17 11:24:36.810272 plover_retro_untranslator-0.4.0/setup.cfg
--rw-r--r--   0 josiah    (1000) josiah    (1000)       62 2024-04-17 10:00:41.000000 plover_retro_untranslator-0.4.0/setup.py
+drwxr-xr-x   0 josiah    (1000) josiah    (1000)        0 2024-05-03 12:10:31.787283 plover_retro_untranslator-0.4.1/
+-rw-r--r--   0 josiah    (1000) josiah    (1000)    32406 2024-04-17 10:00:41.000000 plover_retro_untranslator-0.4.1/LICENSE
+-rw-r--r--   0 josiah    (1000) josiah    (1000)     3641 2024-05-03 12:10:31.787283 plover_retro_untranslator-0.4.1/PKG-INFO
+-rw-r--r--   0 josiah    (1000) josiah    (1000)     2598 2024-04-17 11:19:05.000000 plover_retro_untranslator-0.4.1/README.md
+drwxr-xr-x   0 josiah    (1000) josiah    (1000)        0 2024-05-03 12:10:31.783283 plover_retro_untranslator-0.4.1/plover_retro_untranslator/
+-rw-r--r--   0 josiah    (1000) josiah    (1000)     3071 2024-04-17 11:08:50.000000 plover_retro_untranslator-0.4.1/plover_retro_untranslator/__init__.py
+-rw-r--r--   0 josiah    (1000) josiah    (1000)     2146 2024-04-17 11:06:45.000000 plover_retro_untranslator-0.4.1/plover_retro_untranslator/spelling_converter.py
+drwxr-xr-x   0 josiah    (1000) josiah    (1000)        0 2024-05-03 12:10:31.787283 plover_retro_untranslator-0.4.1/plover_retro_untranslator.egg-info/
+-rw-r--r--   0 josiah    (1000) josiah    (1000)     3641 2024-05-03 12:10:31.000000 plover_retro_untranslator-0.4.1/plover_retro_untranslator.egg-info/PKG-INFO
+-rw-r--r--   0 josiah    (1000) josiah    (1000)      462 2024-05-03 12:10:31.000000 plover_retro_untranslator-0.4.1/plover_retro_untranslator.egg-info/SOURCES.txt
+-rw-r--r--   0 josiah    (1000) josiah    (1000)        1 2024-05-03 12:10:31.000000 plover_retro_untranslator-0.4.1/plover_retro_untranslator.egg-info/dependency_links.txt
+-rw-r--r--   0 josiah    (1000) josiah    (1000)       81 2024-05-03 12:10:31.000000 plover_retro_untranslator-0.4.1/plover_retro_untranslator.egg-info/entry_points.txt
+-rw-r--r--   0 josiah    (1000) josiah    (1000)       30 2024-05-03 12:10:31.000000 plover_retro_untranslator-0.4.1/plover_retro_untranslator.egg-info/requires.txt
+-rw-r--r--   0 josiah    (1000) josiah    (1000)       26 2024-05-03 12:10:31.000000 plover_retro_untranslator-0.4.1/plover_retro_untranslator.egg-info/top_level.txt
+-rw-r--r--   0 josiah    (1000) josiah    (1000)        1 2024-04-17 10:02:30.000000 plover_retro_untranslator-0.4.1/plover_retro_untranslator.egg-info/zip-safe
+-rw-r--r--   0 josiah    (1000) josiah    (1000)     1190 2024-05-03 12:10:31.787283 plover_retro_untranslator-0.4.1/setup.cfg
+-rw-r--r--   0 josiah    (1000) josiah    (1000)       62 2024-04-17 10:00:41.000000 plover_retro_untranslator-0.4.1/setup.py
```

### Comparing `plover_retro_untranslator-0.4.0/LICENSE` & `plover_retro_untranslator-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plover_retro_untranslator-0.4.0/PKG-INFO` & `plover_retro_untranslator-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: plover_retro_untranslator
-Version: 0.4.0
+Version: 0.4.1
 Summary: Converts the last X translations to a specified format consisting of raw steno and/or a translation
 Home-page: https://github.com/Josiah-tan/plover-retro-untranslator
 Author: Josiah-tan
 License: GNU General Public License v3 (GPLv3)
-Keywords: plover
+Keywords: plover plover_plugin plover_retro_untranslator
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `plover_retro_untranslator-0.4.0/README.md` & `plover_retro_untranslator-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `plover_retro_untranslator-0.4.0/plover_retro_untranslator/__init__.py` & `plover_retro_untranslator-0.4.1/plover_retro_untranslator/__init__.py`

 * *Files identical despite different names*

### Comparing `plover_retro_untranslator-0.4.0/plover_retro_untranslator/spelling_converter.py` & `plover_retro_untranslator-0.4.1/plover_retro_untranslator/spelling_converter.py`

 * *Files identical despite different names*

### Comparing `plover_retro_untranslator-0.4.0/plover_retro_untranslator.egg-info/PKG-INFO` & `plover_retro_untranslator-0.4.1/plover_retro_untranslator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: plover_retro_untranslator
-Version: 0.4.0
+Version: 0.4.1
 Summary: Converts the last X translations to a specified format consisting of raw steno and/or a translation
 Home-page: https://github.com/Josiah-tan/plover-retro-untranslator
 Author: Josiah-tan
 License: GNU General Public License v3 (GPLv3)
-Keywords: plover
+Keywords: plover plover_plugin plover_retro_untranslator
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `plover_retro_untranslator-0.4.0/setup.cfg` & `plover_retro_untranslator-0.4.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 [metadata]
 name = plover_retro_untranslator
-version = 0.4.0
-keywords = plover
+version = 0.4.1
 description = Converts the last X translations to a specified format consisting of raw steno and/or a translation
 long_description = file:README.md
 long_description_content_type = text/markdown
 author = Josiah-tan
 license = GNU General Public License v3 (GPLv3)
 url = https://github.com/Josiah-tan/plover-retro-untranslator
 classifiers = 
@@ -16,14 +15,15 @@
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+keywords = plover plover_plugin plover_retro_untranslator
 
 [options]
 zip_safe = True
 setup_requires = 
 	setuptools>=30.3.0
 install_requires = 
 	plover>=4.0.0.dev8
```


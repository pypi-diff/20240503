# Comparing `tmp/nmk-vscode-0.7.0.tar.gz` & `tmp/nmk_vscode-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmk-vscode-0.7.0.tar", last modified: Mon Feb 19 12:52:05 2024, max compression
+gzip compressed data, was "nmk_vscode-0.7.1.tar", last modified: Fri May  3 11:27:48 2024, max compression
```

## Comparing `nmk-vscode-0.7.0.tar` & `nmk_vscode-0.7.1.tar`

### file list

```diff
@@ -1,31 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:52:05.314773 nmk-vscode-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-02-19 12:51:32.000000 nmk-vscode-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-02-19 12:52:05.314773 nmk-vscode-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-02-19 12:52:02.000000 nmk-vscode-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-02-19 12:52:05.314773 nmk-vscode-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-19 12:52:02.000000 nmk-vscode-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:52:05.310773 nmk-vscode-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:52:05.310773 nmk-vscode-0.7.0/src/nmk_vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-02-19 12:51:32.000000 nmk-vscode-0.7.0/src/nmk_vscode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-02-19 12:51:32.000000 nmk-vscode-0.7.0/src/nmk_vscode/base_settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-02-19 12:51:32.000000 nmk-vscode-0.7.0/src/nmk_vscode/buildenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-02-19 12:51:32.000000 nmk-vscode-0.7.0/src/nmk_vscode/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-02-19 12:51:32.000000 nmk-vscode-0.7.0/src/nmk_vscode/extensions.yml
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-19 12:51:32.000000 nmk-vscode-0.7.0/src/nmk_vscode/launch.yml
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-02-19 12:51:32.000000 nmk-vscode-0.7.0/src/nmk_vscode/plugin-defs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-19 12:51:32.000000 nmk-vscode-0.7.0/src/nmk_vscode/plugin-local.yml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-19 12:51:32.000000 nmk-vscode-0.7.0/src/nmk_vscode/plugin.yml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-19 12:51:32.000000 nmk-vscode-0.7.0/src/nmk_vscode/python.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-02-19 12:51:32.000000 nmk-vscode-0.7.0/src/nmk_vscode/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-02-19 12:51:32.000000 nmk-vscode-0.7.0/src/nmk_vscode/tasks.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:52:05.314773 nmk-vscode-0.7.0/src/nmk_vscode/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 12:51:32.000000 nmk-vscode-0.7.0/src/nmk_vscode/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-02-19 12:51:32.000000 nmk-vscode-0.7.0/src/nmk_vscode/templates/tasks.json.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-19 12:51:32.000000 nmk-vscode-0.7.0/src/nmk_vscode/templates/vscode.sh.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:52:05.314773 nmk-vscode-0.7.0/src/nmk_vscode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-02-19 12:52:05.000000 nmk-vscode-0.7.0/src/nmk_vscode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-02-19 12:52:05.000000 nmk-vscode-0.7.0/src/nmk_vscode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 12:52:05.000000 nmk-vscode-0.7.0/src/nmk_vscode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-19 12:52:05.000000 nmk-vscode-0.7.0/src/nmk_vscode.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-19 12:52:05.000000 nmk-vscode-0.7.0/src/nmk_vscode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-19 12:52:05.000000 nmk-vscode-0.7.0/src/nmk_vscode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:27:48.651919 nmk_vscode-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-03 11:27:16.000000 nmk_vscode-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-03 11:27:48.651919 nmk_vscode-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-03 11:27:45.000000 nmk_vscode-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-03 11:27:48.651919 nmk_vscode-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-03 11:27:45.000000 nmk_vscode-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:27:48.647919 nmk_vscode-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:27:48.647919 nmk_vscode-0.7.1/src/nmk_vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-03 11:27:16.000000 nmk_vscode-0.7.1/src/nmk_vscode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-03 11:27:16.000000 nmk_vscode-0.7.1/src/nmk_vscode/base_settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-03 11:27:16.000000 nmk_vscode-0.7.1/src/nmk_vscode/buildenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-03 11:27:16.000000 nmk_vscode-0.7.1/src/nmk_vscode/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-03 11:27:16.000000 nmk_vscode-0.7.1/src/nmk_vscode/extensions.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-03 11:27:16.000000 nmk_vscode-0.7.1/src/nmk_vscode/launch.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-03 11:27:16.000000 nmk_vscode-0.7.1/src/nmk_vscode/plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-03 11:27:16.000000 nmk_vscode-0.7.1/src/nmk_vscode/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-03 11:27:16.000000 nmk_vscode-0.7.1/src/nmk_vscode/tasks.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:27:48.651919 nmk_vscode-0.7.1/src/nmk_vscode/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:27:16.000000 nmk_vscode-0.7.1/src/nmk_vscode/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-03 11:27:16.000000 nmk_vscode-0.7.1/src/nmk_vscode/templates/tasks.json.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-03 11:27:16.000000 nmk_vscode-0.7.1/src/nmk_vscode/templates/vscode.sh.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:27:48.651919 nmk_vscode-0.7.1/src/nmk_vscode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-03 11:27:48.000000 nmk_vscode-0.7.1/src/nmk_vscode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-03 11:27:48.000000 nmk_vscode-0.7.1/src/nmk_vscode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:27:48.000000 nmk_vscode-0.7.1/src/nmk_vscode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 11:27:48.000000 nmk_vscode-0.7.1/src/nmk_vscode.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 11:27:48.000000 nmk_vscode-0.7.1/src/nmk_vscode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 11:27:48.000000 nmk_vscode-0.7.1/src/nmk_vscode.egg-info/top_level.txt
```

### Comparing `nmk-vscode-0.7.0/LICENSE` & `nmk_vscode-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nmk-vscode-0.7.0/PKG-INFO` & `nmk_vscode-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmk-vscode
-Version: 0.7.0
+Version: 0.7.1
 Summary: VSCode plugin for nmk build system
 Home-page: https://github.com/dynod/nmk-vscode
 Author: The dynod project
 Maintainer: The dynod project
 License: Mozilla Public License Version 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nmk-vscode-0.7.0/README.md` & `nmk_vscode-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `nmk-vscode-0.7.0/setup.cfg` & `nmk_vscode-0.7.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 exclude = 
 	__pycache__
 
 [metadata]
 name = nmk-vscode
 author = The dynod project
 maintainer = The dynod project
-version = 0.7.0
+version = 0.7.1
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Mozilla Public License Version 2.0
 classifiers = 
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
```

### Comparing `nmk-vscode-0.7.0/src/nmk_vscode/__init__.py` & `nmk_vscode-0.7.1/src/nmk_vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `nmk-vscode-0.7.0/src/nmk_vscode/base_settings.json` & `nmk_vscode-0.7.1/src/nmk_vscode/base_settings.json`

 * *Files identical despite different names*

### Comparing `nmk-vscode-0.7.0/src/nmk_vscode/buildenv.py` & `nmk_vscode-0.7.1/src/nmk_vscode/buildenv.py`

 * *Files identical despite different names*

### Comparing `nmk-vscode-0.7.0/src/nmk_vscode/builders.py` & `nmk_vscode-0.7.1/src/nmk_vscode/builders.py`

 * *Files identical despite different names*

### Comparing `nmk-vscode-0.7.0/src/nmk_vscode/extensions.yml` & `nmk_vscode-0.7.1/src/nmk_vscode/extensions.yml`

 * *Files identical despite different names*

### Comparing `nmk-vscode-0.7.0/src/nmk_vscode/launch.yml` & `nmk_vscode-0.7.1/src/nmk_vscode/launch.yml`

 * *Files identical despite different names*

### Comparing `nmk-vscode-0.7.0/src/nmk_vscode/plugin-defs.yml` & `nmk_vscode-0.7.1/src/nmk_vscode/plugin.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# Python plugin definition
+# Python plugin definition (for pip reference)
 refs:
+    - pip://nmk-base!plugin.yml
     - settings.yml      # VSCode settings generation
     - launch.yml        # VSCode launch configs generation
     - tasks.yml         # VSCode tasks generation
     - extensions.yml    # VSCode recommended extensions generation
 
 config:
     # Plugin version
```

### Comparing `nmk-vscode-0.7.0/src/nmk_vscode/settings.yml` & `nmk_vscode-0.7.1/src/nmk_vscode/settings.yml`

 * *Files identical despite different names*

### Comparing `nmk-vscode-0.7.0/src/nmk_vscode/tasks.yml` & `nmk_vscode-0.7.1/src/nmk_vscode/tasks.yml`

 * *Files identical despite different names*

### Comparing `nmk-vscode-0.7.0/src/nmk_vscode/templates/tasks.json.jinja` & `nmk_vscode-0.7.1/src/nmk_vscode/templates/tasks.json.jinja`

 * *Files identical despite different names*

### Comparing `nmk-vscode-0.7.0/src/nmk_vscode.egg-info/PKG-INFO` & `nmk_vscode-0.7.1/src/nmk_vscode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmk-vscode
-Version: 0.7.0
+Version: 0.7.1
 Summary: VSCode plugin for nmk build system
 Home-page: https://github.com/dynod/nmk-vscode
 Author: The dynod project
 Maintainer: The dynod project
 License: Mozilla Public License Version 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nmk-vscode-0.7.0/src/nmk_vscode.egg-info/SOURCES.txt` & `nmk_vscode-0.7.1/src/nmk_vscode.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,18 +4,15 @@
 setup.py
 src/nmk_vscode/__init__.py
 src/nmk_vscode/base_settings.json
 src/nmk_vscode/buildenv.py
 src/nmk_vscode/builders.py
 src/nmk_vscode/extensions.yml
 src/nmk_vscode/launch.yml
-src/nmk_vscode/plugin-defs.yml
-src/nmk_vscode/plugin-local.yml
 src/nmk_vscode/plugin.yml
-src/nmk_vscode/python.yml
 src/nmk_vscode/settings.yml
 src/nmk_vscode/tasks.yml
 src/nmk_vscode.egg-info/PKG-INFO
 src/nmk_vscode.egg-info/SOURCES.txt
 src/nmk_vscode.egg-info/dependency_links.txt
 src/nmk_vscode.egg-info/entry_points.txt
 src/nmk_vscode.egg-info/requires.txt
```


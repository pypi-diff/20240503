# Comparing `tmp/python_bridge-0.1.0.tar.gz` & `tmp/python_bridge-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_bridge-0.1.0.tar", last modified: Tue Apr 16 06:53:05 2024, max compression
+gzip compressed data, was "python_bridge-0.1.1.tar", last modified: Thu May  2 23:53:59 2024, max compression
```

## Comparing `python_bridge-0.1.0.tar` & `python_bridge-0.1.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:53:05.568328 python_bridge-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-16 06:53:00.000000 python_bridge-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-16 06:53:05.568328 python_bridge-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-16 06:53:00.000000 python_bridge-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:53:05.560328 python_bridge-0.1.0/bridge/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:53:05.564329 python_bridge-0.1.0/bridge/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/cli/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:53:05.564329 python_bridge-0.1.0/bridge/cli/db/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/cli/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/cli/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:53:05.564329 python_bridge-0.1.0/bridge/cli/init/
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/cli/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/cli/init/install_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/cli/init/render.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:53:05.564329 python_bridge-0.1.0/bridge/cli/init/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/cli/init/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/cli/init/templates/build__sh.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/cli/init/templates/build_worker__sh.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/cli/init/templates/deploy_to_render_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/cli/init/templates/render__yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/cli/init/templates/start__sh.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/cli/init/templates/start_worker__sh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:53:05.564329 python_bridge-0.1.0/bridge/cli/redis/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/cli/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/cli/stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:53:05.564329 python_bridge-0.1.0/bridge/framework/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/framework/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10069 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/framework/django.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:53:05.568328 python_bridge-0.1.0/bridge/platform/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/platform/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/platform/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/platform/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:53:05.568328 python_bridge-0.1.0/bridge/platform/render/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/platform/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/platform/render/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/platform/render/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:53:05.568328 python_bridge-0.1.0/bridge/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/service/django_celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/service/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/service/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/service/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:53:05.568328 python_bridge-0.1.0/bridge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/utils/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-16 06:53:00.000000 python_bridge-0.1.0/bridge/utils/sanitize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-16 06:53:00.000000 python_bridge-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:53:05.568328 python_bridge-0.1.0/python_bridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-16 06:53:05.000000 python_bridge-0.1.0/python_bridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-16 06:53:05.000000 python_bridge-0.1.0/python_bridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 06:53:05.000000 python_bridge-0.1.0/python_bridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 06:53:05.000000 python_bridge-0.1.0/python_bridge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-16 06:53:05.000000 python_bridge-0.1.0/python_bridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 06:53:05.000000 python_bridge-0.1.0/python_bridge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 06:53:05.568328 python_bridge-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:53:59.876668 python_bridge-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 23:53:55.000000 python_bridge-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-05-02 23:53:59.876668 python_bridge-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-02 23:53:55.000000 python_bridge-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:53:59.872667 python_bridge-0.1.1/bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:53:59.872667 python_bridge-0.1.1/bridge/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/cli/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:53:59.872667 python_bridge-0.1.1/bridge/cli/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/cli/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/cli/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:53:59.872667 python_bridge-0.1.1/bridge/cli/init/
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/cli/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/cli/init/install_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/cli/init/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:53:59.872667 python_bridge-0.1.1/bridge/cli/init/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/cli/init/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/cli/init/templates/build__sh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/cli/init/templates/build_worker__sh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/cli/init/templates/deploy_to_render_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/cli/init/templates/render__yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/cli/init/templates/start__sh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/cli/init/templates/start_worker__sh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:53:59.872667 python_bridge-0.1.1/bridge/cli/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/cli/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/cli/stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:53:59.876668 python_bridge-0.1.1/bridge/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/framework/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10069 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/framework/django.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:53:59.876668 python_bridge-0.1.1/bridge/platform/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/platform/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/platform/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/platform/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:53:59.876668 python_bridge-0.1.1/bridge/platform/render/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/platform/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/platform/render/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/platform/render/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:53:59.876668 python_bridge-0.1.1/bridge/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/service/django_celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/service/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/service/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/service/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:53:59.876668 python_bridge-0.1.1/bridge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/utils/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-02 23:53:55.000000 python_bridge-0.1.1/bridge/utils/sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-02 23:53:55.000000 python_bridge-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:53:59.876668 python_bridge-0.1.1/python_bridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-05-02 23:53:59.000000 python_bridge-0.1.1/python_bridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-02 23:53:59.000000 python_bridge-0.1.1/python_bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 23:53:59.000000 python_bridge-0.1.1/python_bridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 23:53:59.000000 python_bridge-0.1.1/python_bridge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 23:53:59.000000 python_bridge-0.1.1/python_bridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 23:53:59.000000 python_bridge-0.1.1/python_bridge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 23:53:59.876668 python_bridge-0.1.1/setup.cfg
```

### Comparing `python_bridge-0.1.0/LICENSE` & `python_bridge-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/PKG-INFO` & `python_bridge-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bridge
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python tool to abstract your Django infrastructure.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/bridge
 Project-URL: Issues, https://github.com/never-over/bridge/issues
 Keywords: python,deployment,local,infrastructure,postgres,django,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -28,18 +28,22 @@
 Requires-Dist: flower==2.0.1
 Requires-Dist: rich==13.7.1
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: dj-database-url==2.1.0
 Requires-Dist: psutil==5.9.8
 
+[![image](https://img.shields.io/pypi/v/python-bridge.svg)](https://pypi.python.org/pypi/python-bridge)
+[![image](https://img.shields.io/pypi/l/python-bridge.svg)](https://pypi.python.org/pypi/python-bridge)
+[![image](https://img.shields.io/pypi/pyversions/python-bridge.svg)](https://pypi.python.org/pypi/python-bridge)
+[![image](https://github.com/Never-Over/bridge/actions/workflows/ci.yml/badge.svg)](https://github.com/Never-Over/bridge/actions/workflows/ci.yml)
+[![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 # bridge
-
----
-Fully automate your local and deployed infrastructure.
+Fully automate your infrastructure for Django.
 
 ![](https://raw.githubusercontent.com/Never-Over/bridge/main/docs/runserver_demo.gif)
 
 [Full Documentation](https://never-over.github.io/bridge/)
 
 ### What is bridge?
 Bridge enables you to seamlessly run and deploy all the infrastructure you need for a complete Django project.
```

### Comparing `python_bridge-0.1.0/README.md` & `python_bridge-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+[![image](https://img.shields.io/pypi/v/python-bridge.svg)](https://pypi.python.org/pypi/python-bridge)
+[![image](https://img.shields.io/pypi/l/python-bridge.svg)](https://pypi.python.org/pypi/python-bridge)
+[![image](https://img.shields.io/pypi/pyversions/python-bridge.svg)](https://pypi.python.org/pypi/python-bridge)
+[![image](https://github.com/Never-Over/bridge/actions/workflows/ci.yml/badge.svg)](https://github.com/Never-Over/bridge/actions/workflows/ci.yml)
+[![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 # bridge
-
----
-Fully automate your local and deployed infrastructure.
+Fully automate your infrastructure for Django.
 
 ![](https://raw.githubusercontent.com/Never-Over/bridge/main/docs/runserver_demo.gif)
 
 [Full Documentation](https://never-over.github.io/bridge/)
 
 ### What is bridge?
 Bridge enables you to seamlessly run and deploy all the infrastructure you need for a complete Django project.
```

### Comparing `python_bridge-0.1.0/bridge/cli/bridge.py` & `python_bridge-0.1.1/bridge/cli/bridge.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/cli/init/__init__.py` & `python_bridge-0.1.1/bridge/cli/init/__init__.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/cli/init/install_deps.py` & `python_bridge-0.1.1/bridge/cli/init/install_deps.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/cli/init/render.py` & `python_bridge-0.1.1/bridge/cli/init/render.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/cli/init/templates/__init__.py` & `python_bridge-0.1.1/bridge/cli/init/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/cli/init/templates/build__sh.py` & `python_bridge-0.1.1/bridge/cli/init/templates/build__sh.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/cli/init/templates/build_worker__sh.py` & `python_bridge-0.1.1/bridge/cli/init/templates/build_worker__sh.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/cli/init/templates/deploy_to_render_button.py` & `python_bridge-0.1.1/bridge/cli/init/templates/deploy_to_render_button.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/cli/init/templates/render__yaml.py` & `python_bridge-0.1.1/bridge/cli/init/templates/render__yaml.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/cli/stop.py` & `python_bridge-0.1.1/bridge/cli/stop.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/config.py` & `python_bridge-0.1.1/bridge/config.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/console.py` & `python_bridge-0.1.1/bridge/console.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/framework/base.py` & `python_bridge-0.1.1/bridge/framework/base.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/framework/django.py` & `python_bridge-0.1.1/bridge/framework/django.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/platform/base.py` & `python_bridge-0.1.1/bridge/platform/base.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/platform/postgres.py` & `python_bridge-0.1.1/bridge/platform/postgres.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/platform/redis.py` & `python_bridge-0.1.1/bridge/platform/redis.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/platform/render/postgres.py` & `python_bridge-0.1.1/bridge/platform/render/postgres.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/platform/render/redis.py` & `python_bridge-0.1.1/bridge/platform/render/redis.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/service/django_celery.py` & `python_bridge-0.1.1/bridge/service/django_celery.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/service/docker.py` & `python_bridge-0.1.1/bridge/service/docker.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/service/postgres.py` & `python_bridge-0.1.1/bridge/service/postgres.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/service/redis.py` & `python_bridge-0.1.1/bridge/service/redis.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/utils/filesystem.py` & `python_bridge-0.1.1/bridge/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/bridge/utils/sanitize.py` & `python_bridge-0.1.1/bridge/utils/sanitize.py`

 * *Files identical despite different names*

### Comparing `python_bridge-0.1.0/pyproject.toml` & `python_bridge-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-bridge"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A Python tool to abstract your Django infrastructure."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `python_bridge-0.1.0/python_bridge.egg-info/PKG-INFO` & `python_bridge-0.1.1/python_bridge.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bridge
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python tool to abstract your Django infrastructure.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/bridge
 Project-URL: Issues, https://github.com/never-over/bridge/issues
 Keywords: python,deployment,local,infrastructure,postgres,django,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -28,18 +28,22 @@
 Requires-Dist: flower==2.0.1
 Requires-Dist: rich==13.7.1
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: dj-database-url==2.1.0
 Requires-Dist: psutil==5.9.8
 
+[![image](https://img.shields.io/pypi/v/python-bridge.svg)](https://pypi.python.org/pypi/python-bridge)
+[![image](https://img.shields.io/pypi/l/python-bridge.svg)](https://pypi.python.org/pypi/python-bridge)
+[![image](https://img.shields.io/pypi/pyversions/python-bridge.svg)](https://pypi.python.org/pypi/python-bridge)
+[![image](https://github.com/Never-Over/bridge/actions/workflows/ci.yml/badge.svg)](https://github.com/Never-Over/bridge/actions/workflows/ci.yml)
+[![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 # bridge
-
----
-Fully automate your local and deployed infrastructure.
+Fully automate your infrastructure for Django.
 
 ![](https://raw.githubusercontent.com/Never-Over/bridge/main/docs/runserver_demo.gif)
 
 [Full Documentation](https://never-over.github.io/bridge/)
 
 ### What is bridge?
 Bridge enables you to seamlessly run and deploy all the infrastructure you need for a complete Django project.
```

### Comparing `python_bridge-0.1.0/python_bridge.egg-info/SOURCES.txt` & `python_bridge-0.1.1/python_bridge.egg-info/SOURCES.txt`

 * *Files identical despite different names*


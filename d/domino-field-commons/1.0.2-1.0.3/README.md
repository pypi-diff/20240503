# Comparing `tmp/domino_field_commons-1.0.2.tar.gz` & `tmp/domino_field_commons-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domino_field_commons-1.0.2.tar", last modified: Mon Jan 22 15:16:52 2024, max compression
+gzip compressed data, was "domino_field_commons-1.0.3.tar", last modified: Fri May  3 08:24:02 2024, max compression
```

## Comparing `domino_field_commons-1.0.2.tar` & `domino_field_commons-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 vdhawan    (502) staff       (20)        0 2024-01-22 15:16:52.573853 domino_field_commons-1.0.2/
--rw-r--r--   0 vdhawan    (502) staff       (20)     1073 2024-01-22 11:05:31.000000 domino_field_commons-1.0.2/LICENSE
--rw-r--r--   0 vdhawan    (502) staff       (20)      197 2024-01-22 15:16:52.573383 domino_field_commons-1.0.2/PKG-INFO
--rw-r--r--   0 vdhawan    (502) staff       (20)     3354 2024-01-22 12:01:56.000000 domino_field_commons-1.0.2/README.md
--rw-r--r--   0 vdhawan    (502) staff       (20)     1051 2024-01-22 11:57:11.000000 domino_field_commons-1.0.2/pyproject.toml
--rw-r--r--   0 vdhawan    (502) staff       (20)       38 2024-01-22 15:16:52.573934 domino_field_commons-1.0.2/setup.cfg
-drwxr-xr-x   0 vdhawan    (502) staff       (20)        0 2024-01-22 15:16:52.565036 domino_field_commons-1.0.2/src/
-drwxr-xr-x   0 vdhawan    (502) staff       (20)        0 2024-01-22 15:16:52.572923 domino_field_commons-1.0.2/src/domino_field_commons.egg-info/
--rw-r--r--   0 vdhawan    (502) staff       (20)      197 2024-01-22 15:16:52.000000 domino_field_commons-1.0.2/src/domino_field_commons.egg-info/PKG-INFO
--rw-r--r--   0 vdhawan    (502) staff       (20)      429 2024-01-22 15:16:52.000000 domino_field_commons-1.0.2/src/domino_field_commons.egg-info/SOURCES.txt
--rw-r--r--   0 vdhawan    (502) staff       (20)        1 2024-01-22 15:16:52.000000 domino_field_commons-1.0.2/src/domino_field_commons.egg-info/dependency_links.txt
--rw-r--r--   0 vdhawan    (502) staff       (20)       14 2024-01-22 15:16:52.000000 domino_field_commons-1.0.2/src/domino_field_commons.egg-info/top_level.txt
-drwxr-xr-x   0 vdhawan    (502) staff       (20)        0 2024-01-22 15:16:52.569982 domino_field_commons-1.0.2/src/field_commons/
--rw-r--r--   0 vdhawan    (502) staff       (20)       57 2024-01-22 11:05:31.000000 domino_field_commons-1.0.2/src/field_commons/__init__.py
-drwxr-xr-x   0 vdhawan    (502) staff       (20)        0 2024-01-22 15:16:52.571243 domino_field_commons-1.0.2/src/field_commons/events_util/
--rw-r--r--   0 vdhawan    (502) staff       (20)     1452 2024-01-22 12:00:45.000000 domino_field_commons-1.0.2/src/field_commons/events_util/__init__.py
--rw-r--r--   0 vdhawan    (502) staff       (20)     2679 2024-01-22 11:59:48.000000 domino_field_commons-1.0.2/src/field_commons/events_util/threadedevents.py
-drwxr-xr-x   0 vdhawan    (502) staff       (20)        0 2024-01-22 15:16:52.571860 domino_field_commons-1.0.2/src/field_commons/keycloak_util/
--rw-r--r--   0 vdhawan    (502) staff       (20)      794 2024-01-22 11:05:31.000000 domino_field_commons-1.0.2/src/field_commons/keycloak_util/__init__.py
-drwxr-xr-x   0 vdhawan    (502) staff       (20)        0 2024-01-22 15:16:52.572293 domino_field_commons-1.0.2/src/field_commons/mongo_util/
--rw-r--r--   0 vdhawan    (502) staff       (20)     1212 2024-01-22 11:05:31.000000 domino_field_commons-1.0.2/src/field_commons/mongo_util/__init__.py
+drwxr-xr-x   0 vdhawan    (502) staff       (20)        0 2024-05-03 08:24:02.216816 domino_field_commons-1.0.3/
+-rw-r--r--   0 vdhawan    (502) staff       (20)     1073 2024-01-22 11:05:31.000000 domino_field_commons-1.0.3/LICENSE
+-rw-r--r--   0 vdhawan    (502) staff       (20)      197 2024-05-03 08:24:02.216349 domino_field_commons-1.0.3/PKG-INFO
+-rw-r--r--   0 vdhawan    (502) staff       (20)     3354 2024-01-22 12:01:56.000000 domino_field_commons-1.0.3/README.md
+-rw-r--r--   0 vdhawan    (502) staff       (20)     1051 2024-05-03 08:23:52.000000 domino_field_commons-1.0.3/pyproject.toml
+-rw-r--r--   0 vdhawan    (502) staff       (20)       38 2024-05-03 08:24:02.216887 domino_field_commons-1.0.3/setup.cfg
+drwxr-xr-x   0 vdhawan    (502) staff       (20)        0 2024-05-03 08:24:02.206968 domino_field_commons-1.0.3/src/
+drwxr-xr-x   0 vdhawan    (502) staff       (20)        0 2024-05-03 08:24:02.215535 domino_field_commons-1.0.3/src/domino_field_commons.egg-info/
+-rw-r--r--   0 vdhawan    (502) staff       (20)      197 2024-05-03 08:24:02.000000 domino_field_commons-1.0.3/src/domino_field_commons.egg-info/PKG-INFO
+-rw-r--r--   0 vdhawan    (502) staff       (20)      429 2024-05-03 08:24:02.000000 domino_field_commons-1.0.3/src/domino_field_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 vdhawan    (502) staff       (20)        1 2024-05-03 08:24:02.000000 domino_field_commons-1.0.3/src/domino_field_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 vdhawan    (502) staff       (20)       14 2024-05-03 08:24:02.000000 domino_field_commons-1.0.3/src/domino_field_commons.egg-info/top_level.txt
+drwxr-xr-x   0 vdhawan    (502) staff       (20)        0 2024-05-03 08:24:02.212324 domino_field_commons-1.0.3/src/field_commons/
+-rw-r--r--   0 vdhawan    (502) staff       (20)       57 2024-01-22 11:05:31.000000 domino_field_commons-1.0.3/src/field_commons/__init__.py
+drwxr-xr-x   0 vdhawan    (502) staff       (20)        0 2024-05-03 08:24:02.213520 domino_field_commons-1.0.3/src/field_commons/events_util/
+-rw-r--r--   0 vdhawan    (502) staff       (20)     1452 2024-05-02 15:27:05.000000 domino_field_commons-1.0.3/src/field_commons/events_util/__init__.py
+-rw-r--r--   0 vdhawan    (502) staff       (20)     2679 2024-05-02 15:27:05.000000 domino_field_commons-1.0.3/src/field_commons/events_util/threadedevents.py
+drwxr-xr-x   0 vdhawan    (502) staff       (20)        0 2024-05-03 08:24:02.214160 domino_field_commons-1.0.3/src/field_commons/keycloak_util/
+-rw-r--r--   0 vdhawan    (502) staff       (20)      794 2024-05-03 08:20:01.000000 domino_field_commons-1.0.3/src/field_commons/keycloak_util/__init__.py
+drwxr-xr-x   0 vdhawan    (502) staff       (20)        0 2024-05-03 08:24:02.214710 domino_field_commons-1.0.3/src/field_commons/mongo_util/
+-rw-r--r--   0 vdhawan    (502) staff       (20)     1212 2024-05-02 15:27:05.000000 domino_field_commons-1.0.3/src/field_commons/mongo_util/__init__.py
```

### Comparing `domino_field_commons-1.0.2/LICENSE` & `domino_field_commons-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `domino_field_commons-1.0.2/README.md` & `domino_field_commons-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `domino_field_commons-1.0.2/pyproject.toml` & `domino_field_commons-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name =  "domino_field_commons"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
     {name = "Field Engineering"},
 ]
 description = "Library of common APIs used by field deployed code"
 requires-python = ">=3.9.1"
 
 [build-system]
```

### Comparing `domino_field_commons-1.0.2/src/field_commons/events_util/__init__.py` & `domino_field_commons-1.0.3/src/field_commons/events_util/__init__.py`

 * *Files identical despite different names*

### Comparing `domino_field_commons-1.0.2/src/field_commons/events_util/threadedevents.py` & `domino_field_commons-1.0.3/src/field_commons/events_util/threadedevents.py`

 * *Files identical despite different names*

### Comparing `domino_field_commons-1.0.2/src/field_commons/keycloak_util/__init__.py` & `domino_field_commons-1.0.3/src/field_commons/keycloak_util/__init__.py`

 * *Files identical despite different names*

### Comparing `domino_field_commons-1.0.2/src/field_commons/mongo_util/__init__.py` & `domino_field_commons-1.0.3/src/field_commons/mongo_util/__init__.py`

 * *Files identical despite different names*


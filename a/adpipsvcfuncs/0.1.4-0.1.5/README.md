# Comparing `tmp/adpipsvcfuncs-0.1.4.tar.gz` & `tmp/adpipsvcfuncs-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adpipsvcfuncs-0.1.4.tar", last modified: Thu May  2 20:11:58 2024, max compression
+gzip compressed data, was "adpipsvcfuncs-0.1.5.tar", last modified: Fri May  3 01:16:53 2024, max compression
```

## Comparing `adpipsvcfuncs-0.1.4.tar` & `adpipsvcfuncs-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:11:58.954490 adpipsvcfuncs-0.1.4/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-05-02 20:11:27.000000 adpipsvcfuncs-0.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      329 2024-05-02 20:11:58.954490 adpipsvcfuncs-0.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       74 2024-05-02 20:11:27.000000 adpipsvcfuncs-0.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:11:58.954490 adpipsvcfuncs-0.1.4/adpipsvcfuncs/
--rw-r--r--   0 root         (0) root         (0)       28 2024-05-02 20:11:27.000000 adpipsvcfuncs-0.1.4/adpipsvcfuncs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1801 2024-05-02 20:11:27.000000 adpipsvcfuncs-0.1.4/adpipsvcfuncs/adpipsvcfuncs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:11:58.954490 adpipsvcfuncs-0.1.4/adpipsvcfuncs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      329 2024-05-02 20:11:58.000000 adpipsvcfuncs-0.1.4/adpipsvcfuncs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      231 2024-05-02 20:11:58.000000 adpipsvcfuncs-0.1.4/adpipsvcfuncs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:11:58.000000 adpipsvcfuncs-0.1.4/adpipsvcfuncs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-02 20:11:58.000000 adpipsvcfuncs-0.1.4/adpipsvcfuncs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 20:11:58.954490 adpipsvcfuncs-0.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      424 2024-05-02 20:11:27.000000 adpipsvcfuncs-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 01:16:53.190812 adpipsvcfuncs-0.1.5/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-05-03 01:16:16.000000 adpipsvcfuncs-0.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      329 2024-05-03 01:16:53.190812 adpipsvcfuncs-0.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       74 2024-05-03 01:16:16.000000 adpipsvcfuncs-0.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 01:16:53.190812 adpipsvcfuncs-0.1.5/adpipsvcfuncs/
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-03 01:16:16.000000 adpipsvcfuncs-0.1.5/adpipsvcfuncs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2024-05-03 01:16:16.000000 adpipsvcfuncs-0.1.5/adpipsvcfuncs/adpipsvcfuncs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 01:16:53.190812 adpipsvcfuncs-0.1.5/adpipsvcfuncs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      329 2024-05-03 01:16:53.000000 adpipsvcfuncs-0.1.5/adpipsvcfuncs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      267 2024-05-03 01:16:53.000000 adpipsvcfuncs-0.1.5/adpipsvcfuncs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 01:16:53.000000 adpipsvcfuncs-0.1.5/adpipsvcfuncs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-03 01:16:53.000000 adpipsvcfuncs-0.1.5/adpipsvcfuncs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-03 01:16:53.000000 adpipsvcfuncs-0.1.5/adpipsvcfuncs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 01:16:53.190812 adpipsvcfuncs-0.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      487 2024-05-03 01:16:16.000000 adpipsvcfuncs-0.1.5/setup.py
```

### Comparing `adpipsvcfuncs-0.1.4/LICENSE` & `adpipsvcfuncs-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adpipsvcfuncs-0.1.4/adpipsvcfuncs/adpipsvcfuncs.py` & `adpipsvcfuncs-0.1.5/adpipsvcfuncs/adpipsvcfuncs.py`

 * *Files identical despite different names*


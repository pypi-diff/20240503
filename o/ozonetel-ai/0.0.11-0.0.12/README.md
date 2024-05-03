# Comparing `tmp/ozonetel-ai-0.0.11.tar.gz` & `tmp/ozonetel-ai-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ozonetel-ai-0.0.11.tar", last modified: Thu May  2 12:02:02 2024, max compression
+gzip compressed data, was "ozonetel-ai-0.0.12.tar", last modified: Thu May  2 13:02:55 2024, max compression
```

## Comparing `ozonetel-ai-0.0.11.tar` & `ozonetel-ai-0.0.12.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:02:02.608670 ozonetel-ai-0.0.11/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-02 12:00:22.000000 ozonetel-ai-0.0.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-02 12:02:02.608670 ozonetel-ai-0.0.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-02 12:00:22.000000 ozonetel-ai-0.0.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:02:02.604670 ozonetel-ai-0.0.11/ozoneai/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-02 12:00:22.000000 ozonetel-ai-0.0.11/ozoneai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-02 12:00:22.000000 ozonetel-ai-0.0.11/ozoneai/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-05-02 12:00:22.000000 ozonetel-ai-0.0.11/ozoneai/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-02 12:00:22.000000 ozonetel-ai-0.0.11/ozoneai/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-02 12:00:22.000000 ozonetel-ai-0.0.11/ozoneai/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:02:02.608670 ozonetel-ai-0.0.11/ozonetel_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-02 12:02:02.000000 ozonetel-ai-0.0.11/ozonetel_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-02 12:02:02.000000 ozonetel-ai-0.0.11/ozonetel_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:02:02.000000 ozonetel-ai-0.0.11/ozonetel_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 12:02:02.000000 ozonetel-ai-0.0.11/ozonetel_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 12:02:02.000000 ozonetel-ai-0.0.11/ozonetel_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 12:02:02.608670 ozonetel-ai-0.0.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-02 12:00:22.000000 ozonetel-ai-0.0.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:02:55.442077 ozonetel-ai-0.0.12/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-02 13:01:10.000000 ozonetel-ai-0.0.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-05-02 13:02:55.442077 ozonetel-ai-0.0.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7690 2024-05-02 13:01:10.000000 ozonetel-ai-0.0.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:02:55.442077 ozonetel-ai-0.0.12/ozoneai/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-02 13:01:10.000000 ozonetel-ai-0.0.12/ozoneai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-02 13:01:10.000000 ozonetel-ai-0.0.12/ozoneai/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-05-02 13:01:10.000000 ozonetel-ai-0.0.12/ozoneai/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-02 13:01:10.000000 ozonetel-ai-0.0.12/ozoneai/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-02 13:01:10.000000 ozonetel-ai-0.0.12/ozoneai/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:02:55.442077 ozonetel-ai-0.0.12/ozonetel_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-05-02 13:02:55.000000 ozonetel-ai-0.0.12/ozonetel_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-02 13:02:55.000000 ozonetel-ai-0.0.12/ozonetel_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:02:55.000000 ozonetel-ai-0.0.12/ozonetel_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 13:02:55.000000 ozonetel-ai-0.0.12/ozonetel_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 13:02:55.000000 ozonetel-ai-0.0.12/ozonetel_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:02:55.442077 ozonetel-ai-0.0.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-02 13:01:10.000000 ozonetel-ai-0.0.12/setup.py
```

### Comparing `ozonetel-ai-0.0.11/LICENSE` & `ozonetel-ai-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.11/ozoneai/connector.py` & `ozonetel-ai-0.0.12/ozoneai/connector.py`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.11/ozoneai/embeddings.py` & `ozonetel-ai-0.0.12/ozoneai/embeddings.py`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.11/ozoneai/exception.py` & `ozonetel-ai-0.0.12/ozoneai/exception.py`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.11/ozoneai/models.py` & `ozonetel-ai-0.0.12/ozoneai/models.py`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.11/setup.py` & `ozonetel-ai-0.0.12/setup.py`

 * *Files identical despite different names*


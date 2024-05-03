# Comparing `tmp/bear_tools-0.1.0.tar.gz` & `tmp/bear_tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bear_tools-0.1.0.tar", max compression
+gzip compressed data, was "bear_tools-0.1.1.tar", max compression
```

## Comparing `bear_tools-0.1.0.tar` & `bear_tools-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,12 @@
--rw-r--r--   0        0        0     1061 2024-05-02 17:41:55.055549 bear_tools-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2024-05-02 17:43:14.943244 bear_tools-0.1.0/README.md
--rw-r--r--   0        0        0      396 2024-05-02 17:48:02.004093 bear_tools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-02 17:48:17.335873 bear_tools-0.1.0/src/bear-tools/__init__.py
--rw-r--r--   0        0        0     5302 2024-05-02 17:48:57.083194 bear_tools-0.1.0/src/bear-tools/transport_protocol.py
--rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 bear_tools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-02 17:41:55.055549 bear_tools-0.1.1/LICENSE
+-rw-r--r--   0        0        0      633 2024-05-02 23:46:08.179569 bear_tools-0.1.1/README.md
+-rw-r--r--   0        0        0      414 2024-05-02 23:54:16.649111 bear_tools-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       43 2024-05-02 23:18:26.108873 bear_tools-0.1.1/src/bear_tools/__init__.py
+-rw-r--r--   0        0        0     3246 2024-05-02 23:50:02.815697 bear_tools-0.1.1/src/bear_tools/lumberjack/README.md
+-rw-r--r--   0        0        0      245 2024-05-02 23:27:21.735538 bear_tools-0.1.1/src/bear_tools/lumberjack/__init__.py
+-rw-r--r--   0        0        0      274 2024-05-01 19:39:40.507714 bear_tools-0.1.1/src/bear_tools/lumberjack/callback_config.py
+-rw-r--r--   0        0        0     1586 2024-05-01 22:34:05.112359 bear_tools-0.1.1/src/bear_tools/lumberjack/color.py
+-rw-r--r--   0        0        0     1119 2024-05-02 19:03:37.011750 bear_tools-0.1.1/src/bear_tools/lumberjack/log_level.py
+-rw-r--r--   0        0        0    10481 2024-05-02 23:28:07.056885 bear_tools-0.1.1/src/bear_tools/lumberjack/logger.py
+-rw-r--r--   0        0        0     5302 2024-05-02 17:48:57.083194 bear_tools-0.1.1/src/bear_tools/transport_protocol.py
+-rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 bear_tools-0.1.1/PKG-INFO
```

### Comparing `bear_tools-0.1.0/LICENSE` & `bear_tools-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bear_tools-0.1.0/src/bear-tools/transport_protocol.py` & `bear_tools-0.1.1/src/bear_tools/transport_protocol.py`

 * *Files identical despite different names*


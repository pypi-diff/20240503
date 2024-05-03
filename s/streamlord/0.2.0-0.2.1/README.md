# Comparing `tmp/streamlord-0.2.0.tar.gz` & `tmp/streamlord-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlord-0.2.0.tar", max compression
+gzip compressed data, was "streamlord-0.2.1.tar", max compression
```

## Comparing `streamlord-0.2.0.tar` & `streamlord-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       59 2024-04-15 11:50:57.981205 streamlord-0.2.0/README.md
--rw-r--r--   0        0        0      357 2024-05-03 12:00:02.891581 streamlord-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       81 2024-04-02 15:23:42.893017 streamlord-0.2.0/streamlord/__init__.py
--rw-r--r--   0        0        0       30 2024-04-02 15:23:42.893115 streamlord-0.2.0/streamlord/collector/__init__.py
--rw-r--r--   0        0        0      144 2024-04-02 15:23:42.893228 streamlord-0.2.0/streamlord/collector/navigation.py
--rw-r--r--   0        0        0       24 2024-04-02 15:23:42.893330 streamlord-0.2.0/streamlord/definitions/__init__.py
--rw-r--r--   0        0        0      156 2024-05-03 11:59:54.089348 streamlord-0.2.0/streamlord/definitions/contracts.py
--rw-r--r--   0        0        0      922 2024-05-03 11:59:54.077897 streamlord-0.2.0/streamlord/pipeline.py
--rw-r--r--   0        0        0      143 2024-05-03 11:59:54.106639 streamlord-0.2.0/streamlord/transformer/__init__.py
--rw-r--r--   0        0        0      831 2024-05-03 11:59:54.085738 streamlord-0.2.0/streamlord/transformer/destroyer.py
--rw-r--r--   0        0        0      726 2024-05-03 11:59:54.104177 streamlord-0.2.0/streamlord/transformer/digger.py
--rw-r--r--   0        0        0     1287 2024-05-03 11:59:54.043206 streamlord-0.2.0/streamlord/transformer/injector.py
--rw-r--r--   0        0        0     1621 2024-05-03 11:59:54.097556 streamlord-0.2.0/streamlord/transformer/squeezer.py
--rw-r--r--   0        0        0     1316 2024-05-03 11:59:54.073387 streamlord-0.2.0/streamlord/transformer/stamper.py
--rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 streamlord-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       59 2024-04-15 11:50:57.981205 streamlord-0.2.1/README.md
+-rw-r--r--   0        0        0      357 2024-05-03 12:05:27.490002 streamlord-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       86 2024-05-03 12:05:27.530963 streamlord-0.2.1/streamlord/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-02 15:23:42.893115 streamlord-0.2.1/streamlord/collectors/__init__.py
+-rw-r--r--   0        0        0      144 2024-04-02 15:23:42.893228 streamlord-0.2.1/streamlord/collectors/navigation.py
+-rw-r--r--   0        0        0       24 2024-04-02 15:23:42.893330 streamlord-0.2.1/streamlord/definitions/__init__.py
+-rw-r--r--   0        0        0      156 2024-05-03 11:59:54.089348 streamlord-0.2.1/streamlord/definitions/contracts.py
+-rw-r--r--   0        0        0      922 2024-05-03 11:59:54.077897 streamlord-0.2.1/streamlord/pipeline.py
+-rw-r--r--   0        0        0      143 2024-05-03 11:59:54.106639 streamlord-0.2.1/streamlord/transformers/__init__.py
+-rw-r--r--   0        0        0      831 2024-05-03 11:59:54.085738 streamlord-0.2.1/streamlord/transformers/destroyer.py
+-rw-r--r--   0        0        0      726 2024-05-03 11:59:54.104177 streamlord-0.2.1/streamlord/transformers/digger.py
+-rw-r--r--   0        0        0     1287 2024-05-03 11:59:54.043206 streamlord-0.2.1/streamlord/transformers/injector.py
+-rw-r--r--   0        0        0     1621 2024-05-03 11:59:54.097556 streamlord-0.2.1/streamlord/transformers/squeezer.py
+-rw-r--r--   0        0        0     1316 2024-05-03 11:59:54.073387 streamlord-0.2.1/streamlord/transformers/stamper.py
+-rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 streamlord-0.2.1/PKG-INFO
```

### Comparing `streamlord-0.2.0/streamlord/pipeline.py` & `streamlord-0.2.1/streamlord/pipeline.py`

 * *Files identical despite different names*

### Comparing `streamlord-0.2.0/streamlord/transformer/destroyer.py` & `streamlord-0.2.1/streamlord/transformers/destroyer.py`

 * *Files identical despite different names*

### Comparing `streamlord-0.2.0/streamlord/transformer/digger.py` & `streamlord-0.2.1/streamlord/transformers/digger.py`

 * *Files identical despite different names*

### Comparing `streamlord-0.2.0/streamlord/transformer/injector.py` & `streamlord-0.2.1/streamlord/transformers/injector.py`

 * *Files identical despite different names*

### Comparing `streamlord-0.2.0/streamlord/transformer/squeezer.py` & `streamlord-0.2.1/streamlord/transformers/squeezer.py`

 * *Files identical despite different names*

### Comparing `streamlord-0.2.0/streamlord/transformer/stamper.py` & `streamlord-0.2.1/streamlord/transformers/stamper.py`

 * *Files identical despite different names*

### Comparing `streamlord-0.2.0/PKG-INFO` & `streamlord-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlord
-Version: 0.2.0
+Version: 0.2.1
 Summary: Collection of tools to manipulate data streams
 Home-page: https://github.com/smairon/streamlord
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```


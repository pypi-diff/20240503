# Comparing `tmp/hbox-0.1.20.tar.gz` & `tmp/hbox-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hbox-0.1.20.tar", max compression
+gzip compressed data, was "hbox-0.2.1.tar", max compression
```

## Comparing `hbox-0.1.20.tar` & `hbox-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1078 2024-05-03 02:06:15.856308 hbox-0.1.20/LICENSE
--rw-r--r--   0        0        0     6344 2024-05-03 02:06:15.856308 hbox-0.1.20/README.md
--rw-r--r--   0        0        0     6635 2024-05-03 02:06:15.856308 hbox-0.1.20/hbox/commands.py
--rw-r--r--   0        0        0     2212 2024-05-03 02:06:15.860308 hbox-0.1.20/hbox/config.py
--rw-r--r--   0        0        0      684 2024-05-03 02:06:15.860308 hbox-0.1.20/hbox/logger.py
--rw-r--r--   0        0        0     3094 2024-05-03 02:06:15.860308 hbox-0.1.20/hbox/main.py
--rw-r--r--   0        0        0     2292 2024-05-03 02:06:15.860308 hbox-0.1.20/hbox/utils.py
--rw-r--r--   0        0        0      428 2024-05-03 02:06:15.860308 hbox-0.1.20/pyproject.toml
--rw-r--r--   0        0        0     6815 1970-01-01 00:00:00.000000 hbox-0.1.20/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-03 05:14:25.705274 hbox-0.2.1/LICENSE
+-rw-r--r--   0        0        0     6344 2024-05-03 05:14:25.705274 hbox-0.2.1/README.md
+-rw-r--r--   0        0        0     6635 2024-05-03 05:14:25.705274 hbox-0.2.1/hbox/commands.py
+-rw-r--r--   0        0        0     2212 2024-05-03 05:14:25.705274 hbox-0.2.1/hbox/config.py
+-rw-r--r--   0        0        0      684 2024-05-03 05:14:25.705274 hbox-0.2.1/hbox/logger.py
+-rw-r--r--   0        0        0     3094 2024-05-03 05:14:25.705274 hbox-0.2.1/hbox/main.py
+-rw-r--r--   0        0        0     2292 2024-05-03 05:14:25.705274 hbox-0.2.1/hbox/utils.py
+-rw-r--r--   0        0        0     1861 2024-05-03 05:14:46.761070 hbox-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6814 1970-01-01 00:00:00.000000 hbox-0.2.1/PKG-INFO
```

### Comparing `hbox-0.1.20/LICENSE` & `hbox-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hbox-0.1.20/README.md` & `hbox-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hbox-0.1.20/hbox/commands.py` & `hbox-0.2.1/hbox/commands.py`

 * *Files identical despite different names*

### Comparing `hbox-0.1.20/hbox/config.py` & `hbox-0.2.1/hbox/config.py`

 * *Files identical despite different names*

### Comparing `hbox-0.1.20/hbox/logger.py` & `hbox-0.2.1/hbox/logger.py`

 * *Files identical despite different names*

### Comparing `hbox-0.1.20/hbox/main.py` & `hbox-0.2.1/hbox/main.py`

 * *Files identical despite different names*

### Comparing `hbox-0.1.20/hbox/utils.py` & `hbox-0.2.1/hbox/utils.py`

 * *Files identical despite different names*

### Comparing `hbox-0.1.20/PKG-INFO` & `hbox-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hbox
-Version: 0.1.20
+Version: 0.2.1
 Summary: CLI tool that leverages container technology to manage packages.
 License: MIT
 Author: Helton Carlos de Souza
 Author-email: heltoncarlossouza@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


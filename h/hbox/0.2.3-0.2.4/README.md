# Comparing `tmp/hbox-0.2.3.tar.gz` & `tmp/hbox-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hbox-0.2.3.tar", max compression
+gzip compressed data, was "hbox-0.2.4.tar", max compression
```

## Comparing `hbox-0.2.3.tar` & `hbox-0.2.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1078 2024-05-03 06:14:00.408609 hbox-0.2.3/LICENSE
--rw-r--r--   0        0        0     6344 2024-05-03 06:14:00.408609 hbox-0.2.3/README.md
--rw-r--r--   0        0        0     6635 2024-05-03 06:14:00.408609 hbox-0.2.3/hbox/commands.py
--rw-r--r--   0        0        0     2212 2024-05-03 06:14:00.408609 hbox-0.2.3/hbox/config.py
--rw-r--r--   0        0        0      684 2024-05-03 06:14:00.408609 hbox-0.2.3/hbox/logger.py
--rw-r--r--   0        0        0     3094 2024-05-03 06:14:00.408609 hbox-0.2.3/hbox/main.py
--rw-r--r--   0        0        0     2292 2024-05-03 06:14:00.408609 hbox-0.2.3/hbox/utils.py
--rw-r--r--   0        0        0     1961 2024-05-03 06:14:28.948699 hbox-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     6814 1970-01-01 00:00:00.000000 hbox-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-03 06:22:42.629986 hbox-0.2.4/LICENSE
+-rw-r--r--   0        0        0     6344 2024-05-03 06:22:42.629986 hbox-0.2.4/README.md
+-rw-r--r--   0        0        0     6635 2024-05-03 06:22:42.629986 hbox-0.2.4/hbox/commands.py
+-rw-r--r--   0        0        0     2212 2024-05-03 06:22:42.629986 hbox-0.2.4/hbox/config.py
+-rw-r--r--   0        0        0      684 2024-05-03 06:22:42.629986 hbox-0.2.4/hbox/logger.py
+-rw-r--r--   0        0        0     3094 2024-05-03 06:22:42.629986 hbox-0.2.4/hbox/main.py
+-rw-r--r--   0        0        0     2292 2024-05-03 06:22:42.633986 hbox-0.2.4/hbox/utils.py
+-rw-r--r--   0        0        0     1961 2024-05-03 06:23:01.894012 hbox-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     6814 1970-01-01 00:00:00.000000 hbox-0.2.4/PKG-INFO
```

### Comparing `hbox-0.2.3/LICENSE` & `hbox-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hbox-0.2.3/README.md` & `hbox-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `hbox-0.2.3/hbox/commands.py` & `hbox-0.2.4/hbox/commands.py`

 * *Files identical despite different names*

### Comparing `hbox-0.2.3/hbox/config.py` & `hbox-0.2.4/hbox/config.py`

 * *Files identical despite different names*

### Comparing `hbox-0.2.3/hbox/logger.py` & `hbox-0.2.4/hbox/logger.py`

 * *Files identical despite different names*

### Comparing `hbox-0.2.3/hbox/main.py` & `hbox-0.2.4/hbox/main.py`

 * *Files identical despite different names*

### Comparing `hbox-0.2.3/hbox/utils.py` & `hbox-0.2.4/hbox/utils.py`

 * *Files identical despite different names*

### Comparing `hbox-0.2.3/pyproject.toml` & `hbox-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hbox"
-version = "0.2.3"
+version = "0.2.4"
 description = "CLI tool that leverages container technology to manage packages."
 authors = ["Helton Carlos de Souza <heltoncarlossouza@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

### Comparing `hbox-0.2.3/PKG-INFO` & `hbox-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hbox
-Version: 0.2.3
+Version: 0.2.4
 Summary: CLI tool that leverages container technology to manage packages.
 License: MIT
 Author: Helton Carlos de Souza
 Author-email: heltoncarlossouza@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/ultima_scraper_renamer-1.1.71.tar.gz` & `tmp/ultima_scraper_renamer-1.1.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_renamer-1.1.71.tar", max compression
+gzip compressed data, was "ultima_scraper_renamer-1.1.72.tar", max compression
```

## Comparing `ultima_scraper_renamer-1.1.71.tar` & `ultima_scraper_renamer-1.1.72.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2022-12-05 14:42:02.218210 ultima_scraper_renamer-1.1.71/README.md
--rw-r--r--   0        0        0      669 2024-04-19 12:23:19.723407 ultima_scraper_renamer-1.1.71/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-05 14:42:02.218210 ultima_scraper_renamer-1.1.71/ultima_scraper_renamer/__init__.py
--rw-r--r--   0        0        0        0 2022-12-06 16:13:32.768074 ultima_scraper_renamer-1.1.71/ultima_scraper_renamer/py.typed
--rw-r--r--   0        0        0    11753 2024-04-19 12:21:59.361385 ultima_scraper_renamer-1.1.71/ultima_scraper_renamer/reformat.py
--rw-r--r--   0        0        0     7872 2023-05-14 17:44:23.086692 ultima_scraper_renamer-1.1.71/ultima_scraper_renamer/renamer.py
--rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 ultima_scraper_renamer-1.1.71/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-12-05 14:42:02.218210 ultima_scraper_renamer-1.1.72/README.md
+-rw-r--r--   0        0        0      666 2024-05-03 04:16:59.820401 ultima_scraper_renamer-1.1.72/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-05 14:42:02.218210 ultima_scraper_renamer-1.1.72/ultima_scraper_renamer/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-06 16:13:32.768074 ultima_scraper_renamer-1.1.72/ultima_scraper_renamer/py.typed
+-rw-r--r--   0        0        0    11753 2024-04-19 12:21:59.361385 ultima_scraper_renamer-1.1.72/ultima_scraper_renamer/reformat.py
+-rw-r--r--   0        0        0     7872 2023-05-14 17:44:23.086692 ultima_scraper_renamer-1.1.72/ultima_scraper_renamer/renamer.py
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 ultima_scraper_renamer-1.1.72/PKG-INFO
```

### Comparing `ultima_scraper_renamer-1.1.71/pyproject.toml` & `ultima_scraper_renamer-1.1.72/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "ultima-scraper-renamer"
-version = "1.1.71"
+version = "1.1.72"
 description = ""
 authors = ["UltimaHoarder <1285176+UltimaHoarder@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "ultima_scraper_renamer" }]
 include = ["ultima_scraper_renamer/py.typed"]
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.12"
+python = ">=3.10,<4"
 tqdm = "^4.64.1"
 orjson = "^3.8.3"
 ultima-scraper-api = "^2.0.0"
 ultima-scraper-collection = "^2.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `ultima_scraper_renamer-1.1.71/ultima_scraper_renamer/reformat.py` & `ultima_scraper_renamer-1.1.72/ultima_scraper_renamer/reformat.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_renamer-1.1.71/ultima_scraper_renamer/renamer.py` & `ultima_scraper_renamer-1.1.72/ultima_scraper_renamer/renamer.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_renamer-1.1.71/PKG-INFO` & `ultima_scraper_renamer-1.1.72/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-renamer
-Version: 1.1.71
+Version: 1.1.72
 Summary: 
 Author: UltimaHoarder
 Author-email: 1285176+UltimaHoarder@users.noreply.github.com
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: orjson (>=3.8.3,<4.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: ultima-scraper-api (>=2.0.0,<3.0.0)
 Requires-Dist: ultima-scraper-collection (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
```


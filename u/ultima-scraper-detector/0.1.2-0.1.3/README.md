# Comparing `tmp/ultima_scraper_detector-0.1.2.tar.gz` & `tmp/ultima_scraper_detector-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_detector-0.1.2.tar", max compression
+gzip compressed data, was "ultima_scraper_detector-0.1.3.tar", max compression
```

## Comparing `ultima_scraper_detector-0.1.2.tar` & `ultima_scraper_detector-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      275 2023-11-15 04:30:18.028494 ultima_scraper_detector-0.1.2/README.md
--rw-r--r--   0        0        0      524 2023-11-15 04:35:28.156207 ultima_scraper_detector-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-12 11:39:01.674212 ultima_scraper_detector-0.1.2/ultima_scraper_detector/__init__.py
--rw-r--r--   0        0        0     3235 2023-11-15 02:52:47.529333 ultima_scraper_detector-0.1.2/ultima_scraper_detector/gui.py
--rw-r--r--   0        0        0      977 2023-11-15 04:31:03.162413 ultima_scraper_detector-0.1.2/ultima_scraper_detector/server.py
--rw-r--r--   0        0        0     4902 2023-11-15 04:16:56.140393 ultima_scraper_detector-0.1.2/ultima_scraper_detector/ultima_scraper_detector.py
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 ultima_scraper_detector-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      275 2023-11-15 04:30:18.028494 ultima_scraper_detector-0.1.3/README.md
+-rw-r--r--   0        0        0      528 2024-05-03 05:13:15.271563 ultima_scraper_detector-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-12 11:39:01.674212 ultima_scraper_detector-0.1.3/ultima_scraper_detector/__init__.py
+-rw-r--r--   0        0        0     3235 2023-11-15 02:52:47.529333 ultima_scraper_detector-0.1.3/ultima_scraper_detector/gui.py
+-rw-r--r--   0        0        0        0 2023-11-15 11:17:27.301097 ultima_scraper_detector-0.1.3/ultima_scraper_detector/py.typed
+-rw-r--r--   0        0        0      977 2023-11-15 04:31:03.162413 ultima_scraper_detector-0.1.3/ultima_scraper_detector/server.py
+-rw-r--r--   0        0        0     4902 2023-11-15 04:16:56.140393 ultima_scraper_detector-0.1.3/ultima_scraper_detector/ultima_scraper_detector.py
+-rw-r--r--   0        0        0      918 1970-01-01 00:00:00.000000 ultima_scraper_detector-0.1.3/PKG-INFO
```

### Comparing `ultima_scraper_detector-0.1.2/pyproject.toml` & `ultima_scraper_detector-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [tool.poetry]
 name = "ultima-scraper-detector"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
-authors = ["DIGITALCRIMINAL <21285176+digitalcriminal@users.noreply.github.com>"]
-packages = [{include = "ultima_scraper_detector"}]
+authors = [
+    "DIGITALCRIMINAL <21285176+digitalcriminal@users.noreply.github.com>",
+]
+packages = [{ include = "ultima_scraper_detector" }]
 include = ["ultima_scraper_detector/py.typed"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.12"
+python = ">=3.10,<4"
 nudenet = "^3.0.8"
 pillow = "^10.1.0"
 psutil = "^5.9.6"
-fastapi = "^0.104.1"
+fastapi = "^0.100"
 uvicorn = "^0.24.0.post1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ultima_scraper_detector-0.1.2/ultima_scraper_detector/gui.py` & `ultima_scraper_detector-0.1.3/ultima_scraper_detector/gui.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_detector-0.1.2/ultima_scraper_detector/server.py` & `ultima_scraper_detector-0.1.3/ultima_scraper_detector/server.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_detector-0.1.2/ultima_scraper_detector/ultima_scraper_detector.py` & `ultima_scraper_detector-0.1.3/ultima_scraper_detector/ultima_scraper_detector.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_detector-0.1.2/PKG-INFO` & `ultima_scraper_detector-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-detector
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: DIGITALCRIMINAL
 Author-email: 21285176+digitalcriminal@users.noreply.github.com
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fastapi (>=0.104.1,<0.105.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: fastapi (>=0.100,<0.101)
 Requires-Dist: nudenet (>=3.0.8,<4.0.0)
 Requires-Dist: pillow (>=10.1.0,<11.0.0)
 Requires-Dist: psutil (>=5.9.6,<6.0.0)
 Requires-Dist: uvicorn (>=0.24.0.post1,<0.25.0)
 Description-Content-Type: text/markdown
 
 Benchmarks:
```


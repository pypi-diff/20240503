# Comparing `tmp/edgegap_service-1.5.3.tar.gz` & `tmp/edgegap_service-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_service-1.5.3.tar", max compression
+gzip compressed data, was "edgegap_service-1.5.4.tar", max compression
```

## Comparing `edgegap_service-1.5.3.tar` & `edgegap_service-1.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1993 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/LICENSE
--rw-r--r--   0        0        0     2188 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/README.md
--rw-r--r--   0        0        0       17 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/BUILD
--rw-r--r--   0        0        0      225 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/__init__.py
--rw-r--r--   0        0        0     2931 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/_configuration.py
--rw-r--r--   0        0        0      735 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/_documentation.py
--rw-r--r--   0        0        0      717 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/_environment.py
--rw-r--r--   0        0        0     2890 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/_scheduling.py
--rw-r--r--   0        0        0     8268 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/_service.py
--rw-r--r--   0        0        0      739 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/_templating.py
--rw-r--r--   0        0        0       17 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/health/BUILD
--rw-r--r--   0        0        0      102 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/health/__init__.py
--rw-r--r--   0        0        0     1453 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/health/_health.py
--rw-r--r--   0        0        0      394 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/health/_model.py
--rw-r--r--   0        0        0       17 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/health/checks/BUILD
--rw-r--r--   0        0        0      300 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/health/checks/__init__.py
--rw-r--r--   0        0        0      594 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/health/checks/_consul.py
--rw-r--r--   0        0        0      740 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/health/checks/_database.py
--rw-r--r--   0        0        0      577 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/health/checks/_interface.py
--rw-r--r--   0        0        0      329 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/health/checks/_model.py
--rw-r--r--   0        0        0      152 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/logging/__init__.py
--rw-r--r--   0        0        0     2135 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/logging/_configuration.py
--rw-r--r--   0        0        0     1657 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/logging/_logger.py
--rw-r--r--   0        0        0     1880 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/static/html/index.html
--rw-r--r--   0        0        0     4286 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/static/images/favicon.ico
--rw-r--r--   0        0        0      972 2024-05-03 19:52:15.283229 edgegap_service-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 edgegap_service-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/LICENSE
+-rw-r--r--   0        0        0     2188 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/README.md
+-rw-r--r--   0        0        0       17 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/BUILD
+-rw-r--r--   0        0        0      225 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/__init__.py
+-rw-r--r--   0        0        0     2931 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/_configuration.py
+-rw-r--r--   0        0        0      735 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/_documentation.py
+-rw-r--r--   0        0        0      717 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/_environment.py
+-rw-r--r--   0        0        0     2890 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/_scheduling.py
+-rw-r--r--   0        0        0     8268 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/_service.py
+-rw-r--r--   0        0        0      739 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/_templating.py
+-rw-r--r--   0        0        0       17 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/health/BUILD
+-rw-r--r--   0        0        0      102 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/health/__init__.py
+-rw-r--r--   0        0        0     1453 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/health/_health.py
+-rw-r--r--   0        0        0      394 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/health/_model.py
+-rw-r--r--   0        0        0       17 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/health/checks/BUILD
+-rw-r--r--   0        0        0      300 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/health/checks/__init__.py
+-rw-r--r--   0        0        0      594 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/health/checks/_consul.py
+-rw-r--r--   0        0        0      740 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/health/checks/_database.py
+-rw-r--r--   0        0        0      577 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/health/checks/_interface.py
+-rw-r--r--   0        0        0      329 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/health/checks/_model.py
+-rw-r--r--   0        0        0      152 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/logging/__init__.py
+-rw-r--r--   0        0        0     2135 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/logging/_configuration.py
+-rw-r--r--   0        0        0     1657 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/logging/_logger.py
+-rw-r--r--   0        0        0     1880 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/static/html/index.html
+-rw-r--r--   0        0        0     4286 2024-05-03 19:55:51.591548 edgegap_service-1.5.4/edgegap_service/static/images/favicon.ico
+-rw-r--r--   0        0        0      972 2024-05-03 19:56:41.587308 edgegap_service-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 edgegap_service-1.5.4/PKG-INFO
```

### Comparing `edgegap_service-1.5.3/LICENSE` & `edgegap_service-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.3/README.md` & `edgegap_service-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.3/edgegap_service/_configuration.py` & `edgegap_service-1.5.4/edgegap_service/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.3/edgegap_service/_documentation.py` & `edgegap_service-1.5.4/edgegap_service/_documentation.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.3/edgegap_service/_environment.py` & `edgegap_service-1.5.4/edgegap_service/_environment.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.3/edgegap_service/_scheduling.py` & `edgegap_service-1.5.4/edgegap_service/_scheduling.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.3/edgegap_service/_service.py` & `edgegap_service-1.5.4/edgegap_service/_service.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.3/edgegap_service/_templating.py` & `edgegap_service-1.5.4/edgegap_service/_templating.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.3/edgegap_service/health/_health.py` & `edgegap_service-1.5.4/edgegap_service/health/_health.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.3/edgegap_service/health/checks/_consul.py` & `edgegap_service-1.5.4/edgegap_service/health/checks/_consul.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.3/edgegap_service/health/checks/_database.py` & `edgegap_service-1.5.4/edgegap_service/health/checks/_database.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.3/edgegap_service/health/checks/_interface.py` & `edgegap_service-1.5.4/edgegap_service/health/checks/_interface.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.3/edgegap_service/logging/_configuration.py` & `edgegap_service-1.5.4/edgegap_service/logging/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.3/edgegap_service/logging/_logger.py` & `edgegap_service-1.5.4/edgegap_service/logging/_logger.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.3/edgegap_service/static/html/index.html` & `edgegap_service-1.5.4/edgegap_service/static/html/index.html`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.3/edgegap_service/static/images/favicon.ico` & `edgegap_service-1.5.4/edgegap_service/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.3/pyproject.toml` & `edgegap_service-1.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-service"
-version = "1.5.3"
+version = "1.5.4"
 description = "The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 include = ["static/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `edgegap_service-1.5.3/PKG-INFO` & `edgegap_service-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-service
-Version: 1.5.3
+Version: 1.5.4
 Summary: The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


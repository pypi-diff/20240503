# Comparing `tmp/edgegap_settings-1.5.2.tar.gz` & `tmp/edgegap_settings-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_settings-1.5.2.tar", max compression
+gzip compressed data, was "edgegap_settings-1.5.3.tar", max compression
```

## Comparing `edgegap_settings-1.5.2.tar` & `edgegap_settings-1.5.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1993 2024-05-03 14:09:58.510569 edgegap_settings-1.5.2/LICENSE
--rw-r--r--   0        0        0     2182 2024-05-03 14:09:58.510752 edgegap_settings-1.5.2/README.md
--rw-r--r--   0        0        0       17 2024-05-03 14:09:58.510863 edgegap_settings-1.5.2/edgegap_settings/BUILD
--rw-r--r--   0        0        0      359 2024-05-03 14:09:58.511175 edgegap_settings-1.5.2/edgegap_settings/__init__.py
--rw-r--r--   0        0        0      531 2024-05-03 14:09:58.511374 edgegap_settings-1.5.2/edgegap_settings/_apm.py
--rw-r--r--   0        0        0     1169 2024-05-03 14:09:58.511566 edgegap_settings-1.5.2/edgegap_settings/_base.py
--rw-r--r--   0        0        0      119 2024-05-03 14:09:58.511876 edgegap_settings-1.5.2/edgegap_settings/_configuration.py
--rw-r--r--   0        0        0     2998 2024-05-03 14:09:58.512055 edgegap_settings-1.5.2/edgegap_settings/_factory.py
--rw-r--r--   0        0        0      917 2024-05-03 14:09:58.512327 edgegap_settings-1.5.2/edgegap_settings/_fields.py
--rw-r--r--   0        0        0      427 2024-05-03 14:09:58.512526 edgegap_settings-1.5.2/edgegap_settings/_logstash.py
--rw-r--r--   0        0        0      741 2024-05-03 14:41:21.792307 edgegap_settings-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     2976 1970-01-01 00:00:00.000000 edgegap_settings-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-03 14:42:17.470940 edgegap_settings-1.5.3/LICENSE
+-rw-r--r--   0        0        0     2182 2024-05-03 14:42:17.470940 edgegap_settings-1.5.3/README.md
+-rw-r--r--   0        0        0       17 2024-05-03 14:42:17.470940 edgegap_settings-1.5.3/edgegap_settings/BUILD
+-rw-r--r--   0        0        0      359 2024-05-03 14:42:17.470940 edgegap_settings-1.5.3/edgegap_settings/__init__.py
+-rw-r--r--   0        0        0      531 2024-05-03 14:42:17.470940 edgegap_settings-1.5.3/edgegap_settings/_apm.py
+-rw-r--r--   0        0        0     1169 2024-05-03 14:42:17.470940 edgegap_settings-1.5.3/edgegap_settings/_base.py
+-rw-r--r--   0        0        0      119 2024-05-03 14:42:17.470940 edgegap_settings-1.5.3/edgegap_settings/_configuration.py
+-rw-r--r--   0        0        0     2998 2024-05-03 14:42:17.470940 edgegap_settings-1.5.3/edgegap_settings/_factory.py
+-rw-r--r--   0        0        0      917 2024-05-03 14:42:17.470940 edgegap_settings-1.5.3/edgegap_settings/_fields.py
+-rw-r--r--   0        0        0      427 2024-05-03 14:42:17.470940 edgegap_settings-1.5.3/edgegap_settings/_logstash.py
+-rw-r--r--   0        0        0      741 2024-05-03 14:42:47.907115 edgegap_settings-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2925 1970-01-01 00:00:00.000000 edgegap_settings-1.5.3/PKG-INFO
```

### Comparing `edgegap_settings-1.5.2/LICENSE` & `edgegap_settings-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.5.2/README.md` & `edgegap_settings-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.5.2/edgegap_settings/_apm.py` & `edgegap_settings-1.5.3/edgegap_settings/_apm.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.5.2/edgegap_settings/_base.py` & `edgegap_settings-1.5.3/edgegap_settings/_base.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.5.2/edgegap_settings/_factory.py` & `edgegap_settings-1.5.3/edgegap_settings/_factory.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.5.2/edgegap_settings/_fields.py` & `edgegap_settings-1.5.3/edgegap_settings/_fields.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.5.2/pyproject.toml` & `edgegap_settings-1.5.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-settings"
-version = "1.5.2"
+version = "1.5.3"
 description = "The Edgegap Settings library includes various tools and helpers for interacting with Explicit Settings Models. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic-settings = "^2.2.1"
```

### Comparing `edgegap_settings-1.5.2/PKG-INFO` & `edgegap_settings-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: edgegap-settings
-Version: 1.5.2
+Version: 1.5.3
 Summary: The Edgegap Settings library includes various tools and helpers for interacting with Explicit Settings Models. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: edgegap-consul (>=1.0.0,<2.0.0)
 Requires-Dist: edgegap-logging (>=1.0.0,<2.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
```


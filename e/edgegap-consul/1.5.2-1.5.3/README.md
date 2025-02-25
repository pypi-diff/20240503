# Comparing `tmp/edgegap_consul-1.5.2.tar.gz` & `tmp/edgegap_consul-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_consul-1.5.2.tar", max compression
+gzip compressed data, was "edgegap_consul-1.5.3.tar", max compression
```

## Comparing `edgegap_consul-1.5.2.tar` & `edgegap_consul-1.5.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1993 2024-05-03 14:42:17.462940 edgegap_consul-1.5.2/LICENSE
--rw-r--r--   0        0        0     2152 2024-05-03 14:42:17.462940 edgegap_consul-1.5.2/README.md
--rw-r--r--   0        0        0       17 2024-05-03 14:42:17.462940 edgegap_consul-1.5.2/edgegap_consul/BUILD
--rw-r--r--   0        0        0      341 2024-05-03 14:42:17.462940 edgegap_consul-1.5.2/edgegap_consul/__init__.py
--rw-r--r--   0        0        0     2257 2024-05-03 14:42:17.466940 edgegap_consul-1.5.2/edgegap_consul/_client.py
--rw-r--r--   0        0        0      399 2024-05-03 14:42:17.466940 edgegap_consul-1.5.2/edgegap_consul/_configuration.py
--rw-r--r--   0        0        0     1325 2024-05-03 14:42:17.466940 edgegap_consul-1.5.2/edgegap_consul/_factory.py
--rw-r--r--   0        0        0     1623 2024-05-03 14:42:17.466940 edgegap_consul-1.5.2/edgegap_consul/_reader.py
--rw-r--r--   0        0        0      720 2024-05-03 14:42:38.127058 edgegap_consul-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     2778 1970-01-01 00:00:00.000000 edgegap_consul-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-03 19:51:34.390796 edgegap_consul-1.5.3/LICENSE
+-rw-r--r--   0        0        0     2152 2024-05-03 19:51:34.390796 edgegap_consul-1.5.3/README.md
+-rw-r--r--   0        0        0       17 2024-05-03 19:51:34.390796 edgegap_consul-1.5.3/edgegap_consul/BUILD
+-rw-r--r--   0        0        0      341 2024-05-03 19:51:34.390796 edgegap_consul-1.5.3/edgegap_consul/__init__.py
+-rw-r--r--   0        0        0     2257 2024-05-03 19:51:34.390796 edgegap_consul-1.5.3/edgegap_consul/_client.py
+-rw-r--r--   0        0        0      399 2024-05-03 19:51:34.390796 edgegap_consul-1.5.3/edgegap_consul/_configuration.py
+-rw-r--r--   0        0        0     1325 2024-05-03 19:51:34.390796 edgegap_consul-1.5.3/edgegap_consul/_factory.py
+-rw-r--r--   0        0        0     1623 2024-05-03 19:51:34.390796 edgegap_consul-1.5.3/edgegap_consul/_reader.py
+-rw-r--r--   0        0        0      720 2024-05-03 19:52:10.807180 edgegap_consul-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2778 1970-01-01 00:00:00.000000 edgegap_consul-1.5.3/PKG-INFO
```

### Comparing `edgegap_consul-1.5.2/LICENSE` & `edgegap_consul-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.5.2/README.md` & `edgegap_consul-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.5.2/edgegap_consul/_client.py` & `edgegap_consul-1.5.3/edgegap_consul/_client.py`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.5.2/edgegap_consul/_factory.py` & `edgegap_consul-1.5.3/edgegap_consul/_factory.py`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.5.2/edgegap_consul/_reader.py` & `edgegap_consul-1.5.3/edgegap_consul/_reader.py`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.5.2/pyproject.toml` & `edgegap_consul-1.5.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-consul"
-version = "1.5.2"
+version = "1.5.3"
 description = "The Edgegap Consul library includes various tools and helpers for interacting with Consul. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = { version = "^3.9.5", extras = ["speedups"] }
```

### Comparing `edgegap_consul-1.5.2/PKG-INFO` & `edgegap_consul-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-consul
-Version: 1.5.2
+Version: 1.5.3
 Summary: The Edgegap Consul library includes various tools and helpers for interacting with Consul. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


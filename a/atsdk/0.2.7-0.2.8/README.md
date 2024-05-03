# Comparing `tmp/atsdk-0.2.7.tar.gz` & `tmp/atsdk-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atsdk-0.2.7.tar", max compression
+gzip compressed data, was "atsdk-0.2.8.tar", max compression
```

## Comparing `atsdk-0.2.7.tar` & `atsdk-0.2.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1529 2024-03-04 16:00:22.445410 atsdk-0.2.7/LICENSE
--rw-r--r--   0        0        0     5788 2024-03-04 16:00:22.445410 atsdk-0.2.7/README.PyPI.md
--rw-r--r--   0        0        0       30 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/__init__.py
--rw-r--r--   0        0        0    20497 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/atclient.py
--rw-r--r--   0        0        0       57 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/common/__init__.py
--rw-r--r--   0        0        0     1413 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/common/atsign.py
--rw-r--r--   0        0        0     5175 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/common/keys.py
--rw-r--r--   0        0        0     8442 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/common/metadata.py
--rw-r--r--   0        0        0      359 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/connections/__init__.py
--rw-r--r--   0        0        0      793 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/connections/address.py
--rw-r--r--   0        0        0     5356 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/connections/atconnection.py
--rw-r--r--   0        0        0    10512 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/connections/atmonitorconnection.py
--rw-r--r--   0        0        0     4121 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/connections/atrootconnection.py
--rw-r--r--   0        0        0     2341 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/connections/atsecondaryconnection.py
--rw-r--r--   0        0        0     1281 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/connections/notification/atevents.py
--rw-r--r--   0        0        0     1874 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/connections/notification/atnotification.py
--rw-r--r--   0        0        0     3491 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/connections/response.py
--rw-r--r--   0        0        0       26 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/exception/__init__.py
--rw-r--r--   0        0        0     3985 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/exception/atexception.py
--rw-r--r--   0        0        0      300 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/util/__init__.py
--rw-r--r--   0        0        0      320 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/util/atconstants.py
--rw-r--r--   0        0        0     2450 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/util/authutil.py
--rw-r--r--   0        0        0     4100 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/util/encryptionutil.py
--rw-r--r--   0        0        0     2769 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/util/keystringutil.py
--rw-r--r--   0        0        0     3481 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/util/keysutil.py
--rw-r--r--   0        0        0     1677 2024-03-04 16:00:22.445410 atsdk-0.2.7/at_client/util/onboardingutil.py
--rw-r--r--   0        0        0     3897 2024-03-04 16:00:22.449410 atsdk-0.2.7/at_client/util/registerutil.py
--rw-r--r--   0        0        0      695 2024-03-04 16:00:22.449410 atsdk-0.2.7/at_client/util/socketutil.py
--rw-r--r--   0        0        0      743 2024-03-04 16:00:22.449410 atsdk-0.2.7/at_client/util/syncdecorator.py
--rw-r--r--   0        0        0      116 2024-03-04 16:00:22.449410 atsdk-0.2.7/at_client/util/timeutil.py
--rw-r--r--   0        0        0    15945 2024-03-04 16:00:22.449410 atsdk-0.2.7/at_client/util/verbbuilder.py
--rw-r--r--   0        0        0      682 2024-03-04 16:00:22.461410 atsdk-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     6584 1970-01-01 00:00:00.000000 atsdk-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1529 2024-03-11 07:08:11.174644 atsdk-0.2.8/LICENSE
+-rw-r--r--   0        0        0     5788 2024-03-11 07:08:11.174644 atsdk-0.2.8/README.PyPI.md
+-rw-r--r--   0        0        0       30 2024-03-11 07:08:11.174644 atsdk-0.2.8/at_client/__init__.py
+-rw-r--r--   0        0        0    20497 2024-03-11 07:08:11.174644 atsdk-0.2.8/at_client/atclient.py
+-rw-r--r--   0        0        0       57 2024-03-11 07:08:11.174644 atsdk-0.2.8/at_client/common/__init__.py
+-rw-r--r--   0        0        0     1413 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/common/atsign.py
+-rw-r--r--   0        0        0     5175 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/common/keys.py
+-rw-r--r--   0        0        0     8442 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/common/metadata.py
+-rw-r--r--   0        0        0      359 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/connections/__init__.py
+-rw-r--r--   0        0        0      793 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/connections/address.py
+-rw-r--r--   0        0        0     5356 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/connections/atconnection.py
+-rw-r--r--   0        0        0    10512 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/connections/atmonitorconnection.py
+-rw-r--r--   0        0        0     4121 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/connections/atrootconnection.py
+-rw-r--r--   0        0        0     2341 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/connections/atsecondaryconnection.py
+-rw-r--r--   0        0        0     1281 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/connections/notification/atevents.py
+-rw-r--r--   0        0        0     1874 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/connections/notification/atnotification.py
+-rw-r--r--   0        0        0     3491 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/connections/response.py
+-rw-r--r--   0        0        0       26 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/exception/__init__.py
+-rw-r--r--   0        0        0     3985 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/exception/atexception.py
+-rw-r--r--   0        0        0      300 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/util/__init__.py
+-rw-r--r--   0        0        0      320 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/util/atconstants.py
+-rw-r--r--   0        0        0     2450 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/util/authutil.py
+-rw-r--r--   0        0        0     4100 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/util/encryptionutil.py
+-rw-r--r--   0        0        0     2769 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/util/keystringutil.py
+-rw-r--r--   0        0        0     3481 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/util/keysutil.py
+-rw-r--r--   0        0        0     1677 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/util/onboardingutil.py
+-rw-r--r--   0        0        0     3897 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/util/registerutil.py
+-rw-r--r--   0        0        0      695 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/util/socketutil.py
+-rw-r--r--   0        0        0      743 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/util/syncdecorator.py
+-rw-r--r--   0        0        0      116 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/util/timeutil.py
+-rw-r--r--   0        0        0    15945 2024-03-11 07:08:11.178644 atsdk-0.2.8/at_client/util/verbbuilder.py
+-rw-r--r--   0        0        0      682 2024-03-11 07:08:11.194644 atsdk-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     6584 1970-01-01 00:00:00.000000 atsdk-0.2.8/PKG-INFO
```

### Comparing `atsdk-0.2.7/LICENSE` & `atsdk-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/README.PyPI.md` & `atsdk-0.2.8/README.PyPI.md`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/atclient.py` & `atsdk-0.2.8/at_client/atclient.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/common/atsign.py` & `atsdk-0.2.8/at_client/common/atsign.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/common/keys.py` & `atsdk-0.2.8/at_client/common/keys.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/common/metadata.py` & `atsdk-0.2.8/at_client/common/metadata.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/connections/address.py` & `atsdk-0.2.8/at_client/connections/address.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/connections/atconnection.py` & `atsdk-0.2.8/at_client/connections/atconnection.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/connections/atmonitorconnection.py` & `atsdk-0.2.8/at_client/connections/atmonitorconnection.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/connections/atrootconnection.py` & `atsdk-0.2.8/at_client/connections/atrootconnection.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/connections/atsecondaryconnection.py` & `atsdk-0.2.8/at_client/connections/atsecondaryconnection.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/connections/notification/atevents.py` & `atsdk-0.2.8/at_client/connections/notification/atevents.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/connections/notification/atnotification.py` & `atsdk-0.2.8/at_client/connections/notification/atnotification.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/connections/response.py` & `atsdk-0.2.8/at_client/connections/response.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/exception/atexception.py` & `atsdk-0.2.8/at_client/exception/atexception.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/util/authutil.py` & `atsdk-0.2.8/at_client/util/authutil.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/util/encryptionutil.py` & `atsdk-0.2.8/at_client/util/encryptionutil.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/util/keystringutil.py` & `atsdk-0.2.8/at_client/util/keystringutil.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/util/keysutil.py` & `atsdk-0.2.8/at_client/util/keysutil.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/util/onboardingutil.py` & `atsdk-0.2.8/at_client/util/onboardingutil.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/util/registerutil.py` & `atsdk-0.2.8/at_client/util/registerutil.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/util/socketutil.py` & `atsdk-0.2.8/at_client/util/socketutil.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/util/syncdecorator.py` & `atsdk-0.2.8/at_client/util/syncdecorator.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/at_client/util/verbbuilder.py` & `atsdk-0.2.8/at_client/util/verbbuilder.py`

 * *Files identical despite different names*

### Comparing `atsdk-0.2.7/pyproject.toml` & `atsdk-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atsdk"
-version = "0.2.7"
+version = "0.2.8"
 description = "Python SDK for atPlatform"
 authors = ["Umang Shah <shahumang19@gmail.com>","Chris Swan <chris@atsign.com>"]
 maintainers = ["Chris Swan <chris@atsign.com>"]
 readme = "README.PyPI.md"
 packages = [{include = "at_client"}]
 homepage = "https://github.com/atsign-foundation/at_python"
 
@@ -16,12 +16,12 @@
 python-dateutil = "2.9.0.post0"
 requests = "2.31.0"
 six = "1.16.0"
 
 [tool.poetry.group.dev.dependencies]
 pip ="24.0"
 flake8 = "7.0.0"
-pytest = "8.1.0"
+pytest = "8.1.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `atsdk-0.2.7/PKG-INFO` & `atsdk-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atsdk
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python SDK for atPlatform
 Home-page: https://github.com/atsign-foundation/at_python
 Author: Umang Shah
 Author-email: shahumang19@gmail.com
 Maintainer: Chris Swan
 Maintainer-email: chris@atsign.com
 Requires-Python: >=3.8.1,<4.0.0
```


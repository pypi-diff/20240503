# Comparing `tmp/accentnotifications-0.0.7.tar.gz` & `tmp/accentnotifications-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accentnotifications-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "accentnotifications-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `accentnotifications-0.0.7.tar` & `accentnotifications-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       99 2022-10-05 10:37:49.000000 accentnotifications-0.0.7/.flake8
--rw-r--r--   0        0        0      929 2023-07-17 11:26:35.290624 accentnotifications-0.0.7/.github/workflows/test.yml
--rw-r--r--   0        0        0      109 2023-07-17 09:30:14.313081 accentnotifications-0.0.7/.gitignore
--rw-r--r--   0        0        0     1089 2022-10-07 18:12:15.000000 accentnotifications-0.0.7/LICENSE
--rw-r--r--   0        0        0      490 2023-07-17 09:30:14.314070 accentnotifications-0.0.7/README.md
--rw-r--r--   0        0        0       81 2023-12-04 14:59:52.606706 accentnotifications-0.0.7/accentnotifications/__init__.py
--rw-r--r--   0        0        0      246 2022-10-12 08:48:23.000000 accentnotifications-0.0.7/accentnotifications/manager.py
--rw-r--r--   0        0        0      112 2023-07-17 09:30:14.314592 accentnotifications-0.0.7/accentnotifications/notifications/__init__.py
--rw-r--r--   0        0        0      897 2023-07-17 11:16:34.607700 accentnotifications-0.0.7/accentnotifications/notifications/base.py
--rw-r--r--   0        0        0     2845 2023-07-17 11:16:33.855651 accentnotifications-0.0.7/accentnotifications/notifications/smtp.py
--rw-r--r--   0        0        0     3038 2023-07-17 11:16:34.605170 accentnotifications-0.0.7/accentnotifications/notifications/twilio_sms.py
--rw-r--r--   0        0        0     1670 2023-07-17 11:16:15.640920 accentnotifications-0.0.7/accentnotifications/types.py
--rw-r--r--   0        0        0     1363 2023-11-16 17:03:05.257025 accentnotifications-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1640 1970-01-01 00:00:00.000000 accentnotifications-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       99 2022-10-05 10:37:49.000000 accentnotifications-0.0.9/.flake8
+-rw-r--r--   0        0        0      937 2024-03-13 12:55:36.092209 accentnotifications-0.0.9/.github/workflows/test.yml
+-rw-r--r--   0        0        0      109 2023-07-17 09:30:14.313081 accentnotifications-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1089 2022-10-07 18:12:15.000000 accentnotifications-0.0.9/LICENSE
+-rw-r--r--   0        0        0      490 2023-07-17 09:30:14.314070 accentnotifications-0.0.9/README.md
+-rw-r--r--   0        0        0       81 2024-03-13 12:56:22.353520 accentnotifications-0.0.9/accentnotifications/__init__.py
+-rw-r--r--   0        0        0      246 2022-10-12 08:48:23.000000 accentnotifications-0.0.9/accentnotifications/manager.py
+-rw-r--r--   0        0        0      112 2023-07-17 09:30:14.314592 accentnotifications-0.0.9/accentnotifications/notifications/__init__.py
+-rw-r--r--   0        0        0      897 2023-07-17 11:16:34.607700 accentnotifications-0.0.9/accentnotifications/notifications/base.py
+-rw-r--r--   0        0        0     2845 2023-07-17 11:16:33.855651 accentnotifications-0.0.9/accentnotifications/notifications/smtp.py
+-rw-r--r--   0        0        0     3038 2023-07-17 11:16:34.605170 accentnotifications-0.0.9/accentnotifications/notifications/twilio_sms.py
+-rw-r--r--   0        0        0     1670 2023-07-17 11:16:15.640920 accentnotifications-0.0.9/accentnotifications/types.py
+-rw-r--r--   0        0        0     1363 2024-03-13 12:53:12.646699 accentnotifications-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1640 1970-01-01 00:00:00.000000 accentnotifications-0.0.9/PKG-INFO
```

### Comparing `accentnotifications-0.0.7/.github/workflows/test.yml` & `accentnotifications-0.0.9/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     types: [opened, synchronize]
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.9", "3.10", "3.11"]
+        python-version: ["3.9", "3.10", "3.11", "3.12"]
       fail-fast: false
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
```

### Comparing `accentnotifications-0.0.7/LICENSE` & `accentnotifications-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `accentnotifications-0.0.7/accentnotifications/notifications/base.py` & `accentnotifications-0.0.9/accentnotifications/notifications/base.py`

 * *Files identical despite different names*

### Comparing `accentnotifications-0.0.7/accentnotifications/notifications/smtp.py` & `accentnotifications-0.0.9/accentnotifications/notifications/smtp.py`

 * *Files identical despite different names*

### Comparing `accentnotifications-0.0.7/accentnotifications/notifications/twilio_sms.py` & `accentnotifications-0.0.9/accentnotifications/notifications/twilio_sms.py`

 * *Files identical despite different names*

### Comparing `accentnotifications-0.0.7/accentnotifications/types.py` & `accentnotifications-0.0.9/accentnotifications/types.py`

 * *Files identical despite different names*

### Comparing `accentnotifications-0.0.7/pyproject.toml` & `accentnotifications-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python",
 ]
 dependencies = [
-    "pydantic>=2.0.1,<2.6.0",
-    "pydantic-settings>=2.0.1,<2.2.0",
+    "pydantic>=2.0.1,<2.7.0",
+    "pydantic-settings>=2.0.1,<2.3.0",
 ]
 dynamic = ["version", "description"]
 
 [project.urls]
 Homepage = "https://github.com/accentdesign/accentnotifications"
 
 [project.optional-dependencies]
```

### Comparing `accentnotifications-0.0.7/PKG-INFO` & `accentnotifications-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: accentnotifications
-Version: 0.0.7
+Version: 0.0.9
 Summary: Sending various forms of notifications such as smtp
 Author-email: Accent Design Group Ltd <support@accentdesign.co.uk>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
-Requires-Dist: pydantic>=2.0.1,<2.6.0
-Requires-Dist: pydantic-settings>=2.0.1,<2.2.0
+Requires-Dist: pydantic>=2.0.1,<2.7.0
+Requires-Dist: pydantic-settings>=2.0.1,<2.3.0
 Requires-Dist: autoflake ; extra == "dev"
 Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: aiosmtplib ; extra == "smtp"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-asyncio ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-mock ; extra == "test"
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: accentnotifications Version: 0.0.7 Summary: Sending
+Metadata-Version: 2.1 Name: accentnotifications Version: 0.0.9 Summary: Sending
 various forms of notifications such as smtp Author-email: Accent Design Group
 Ltd
 accentdesign.co.uk> Requires-Python: >=3.9 Description-Content-Type: text/
 markdown Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-Requires-Dist: pydantic>=2.0.1,<2.6.0 Requires-Dist: pydantic-
-settings>=2.0.1,<2.2.0 Requires-Dist: autoflake ; extra == "dev" Requires-Dist:
+Requires-Dist: pydantic>=2.0.1,<2.7.0 Requires-Dist: pydantic-
+settings>=2.0.1,<2.3.0 Requires-Dist: autoflake ; extra == "dev" Requires-Dist:
 flake8 ; extra == "dev" Requires-Dist: aiosmtplib ; extra == "smtp" Requires-
 Dist: pytest ; extra == "test" Requires-Dist: pytest-asyncio ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test" Requires-Dist: pytest-mock ; extra
 == "test" Requires-Dist: mypy ; extra == "test" Requires-Dist: flake8 ; extra
 == "test" Requires-Dist: black ; extra == "test" Requires-Dist: isort ; extra
 == "test" Requires-Dist: aiohttp ; extra == "twiliosms" Project-URL: Homepage,
 https://github.com/accentdesign/accentnotifications Provides-Extra: dev
```


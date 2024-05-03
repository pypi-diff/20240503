# Comparing `tmp/trustcaptcha-python-1.0.1.tar.gz` & `tmp/trustcaptcha_python-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustcaptcha-python-1.0.1.tar", last modified: Mon Mar 18 18:48:12 2024, max compression
+gzip compressed data, was "trustcaptcha_python-1.1.0.tar", last modified: Fri May  3 19:14:21 2024, max compression
```

## Comparing `trustcaptcha-python-1.0.1.tar` & `trustcaptcha_python-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 18:48:12.751185 trustcaptcha-python-1.0.1/
--rw-r--r--   0 root         (0) root         (0)     1930 2024-03-18 18:48:12.751185 trustcaptcha-python-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1421 2024-03-18 18:44:15.000000 trustcaptcha-python-1.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      644 2024-03-18 18:48:07.000000 trustcaptcha-python-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-18 18:48:12.751185 trustcaptcha-python-1.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 18:48:12.743184 trustcaptcha-python-1.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 18:48:12.747184 trustcaptcha-python-1.0.1/src/trustcaptcha/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-18 18:47:39.000000 trustcaptcha-python-1.0.1/src/trustcaptcha/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      735 2024-03-18 18:44:15.000000 trustcaptcha-python-1.0.1/src/trustcaptcha/aes_encryption.py
--rw-rw-rw-   0 root         (0) root         (0)     2625 2024-03-18 18:44:15.000000 trustcaptcha-python-1.0.1/src/trustcaptcha/captcha_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 18:48:12.747184 trustcaptcha-python-1.0.1/src/trustcaptcha/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-18 18:47:39.000000 trustcaptcha-python-1.0.1/src/trustcaptcha/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      514 2024-03-18 18:44:15.000000 trustcaptcha-python-1.0.1/src/trustcaptcha/model/result_reason.py
--rw-rw-rw-   0 root         (0) root         (0)     1367 2024-03-18 18:44:15.000000 trustcaptcha-python-1.0.1/src/trustcaptcha/model/verification_result.py
--rw-rw-rw-   0 root         (0) root         (0)      520 2024-03-18 18:44:15.000000 trustcaptcha-python-1.0.1/src/trustcaptcha/model/verification_token.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 18:48:12.747184 trustcaptcha-python-1.0.1/src/trustcaptcha_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1930 2024-03-18 18:48:12.000000 trustcaptcha-python-1.0.1/src/trustcaptcha_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      574 2024-03-18 18:48:12.000000 trustcaptcha-python-1.0.1/src/trustcaptcha_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-18 18:48:12.000000 trustcaptcha-python-1.0.1/src/trustcaptcha_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-03-18 18:48:12.000000 trustcaptcha-python-1.0.1/src/trustcaptcha_python.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       79 2024-03-18 18:48:12.000000 trustcaptcha-python-1.0.1/src/trustcaptcha_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-03-18 18:48:12.000000 trustcaptcha-python-1.0.1/src/trustcaptcha_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 19:14:21.844791 trustcaptcha_python-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1930 2024-05-03 19:14:21.844791 trustcaptcha_python-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1421 2024-05-03 19:05:14.000000 trustcaptcha_python-1.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      644 2024-05-03 19:14:18.000000 trustcaptcha_python-1.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 19:14:21.844791 trustcaptcha_python-1.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 19:14:21.836790 trustcaptcha_python-1.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 19:14:21.840790 trustcaptcha_python-1.1.0/src/trustcaptcha/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 19:13:51.000000 trustcaptcha_python-1.1.0/src/trustcaptcha/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      735 2024-05-03 19:05:14.000000 trustcaptcha_python-1.1.0/src/trustcaptcha/aes_encryption.py
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2024-05-03 19:05:14.000000 trustcaptcha_python-1.1.0/src/trustcaptcha/captcha_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 19:14:21.840790 trustcaptcha_python-1.1.0/src/trustcaptcha/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 19:13:51.000000 trustcaptcha_python-1.1.0/src/trustcaptcha/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2024-05-03 19:05:14.000000 trustcaptcha_python-1.1.0/src/trustcaptcha/model/verification_result.py
+-rw-rw-rw-   0 root         (0) root         (0)      520 2024-05-03 19:05:14.000000 trustcaptcha_python-1.1.0/src/trustcaptcha/model/verification_token.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 19:14:21.840790 trustcaptcha_python-1.1.0/src/trustcaptcha_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1930 2024-05-03 19:14:21.000000 trustcaptcha_python-1.1.0/src/trustcaptcha_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      534 2024-05-03 19:14:21.000000 trustcaptcha_python-1.1.0/src/trustcaptcha_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 19:14:21.000000 trustcaptcha_python-1.1.0/src/trustcaptcha_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-03 19:14:21.000000 trustcaptcha_python-1.1.0/src/trustcaptcha_python.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2024-05-03 19:14:21.000000 trustcaptcha_python-1.1.0/src/trustcaptcha_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-03 19:14:21.000000 trustcaptcha_python-1.1.0/src/trustcaptcha_python.egg-info/top_level.txt
```

### Comparing `trustcaptcha-python-1.0.1/PKG-INFO` & `trustcaptcha_python-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustcaptcha-python
-Version: 1.0.1
+Version: 1.1.0
 Summary: Trustcaptcha library for python
 Author-email: Trustcaptcha GmbH <mail@trustcaptcha.com>
 License: Apache-2.0
 Keywords: captcha,gdpr,privacy,security,made-in-germany,eu,european-union
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: numpy
```

### Comparing `trustcaptcha-python-1.0.1/README.md` & `trustcaptcha_python-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `trustcaptcha-python-1.0.1/pyproject.toml` & `trustcaptcha_python-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=42", "wheel",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "trustcaptcha-python"
-version = "1.0.1"
+version = "1.1.0"
 description = "Trustcaptcha library for python"
 readme = "README.md"
 dependencies = [ "requests", "numpy", "pycryptodome==3.19.0", "pycryptodomex==3.19.0",]
 keywords = [ "captcha", "gdpr", "privacy", "security", "made-in-germany", "eu", "european-union",]
 [[project.authors]]
 name = "Trustcaptcha GmbH"
 email = "mail@trustcaptcha.com"
```

### Comparing `trustcaptcha-python-1.0.1/src/trustcaptcha/aes_encryption.py` & `trustcaptcha_python-1.1.0/src/trustcaptcha/aes_encryption.py`

 * *Files identical despite different names*

### Comparing `trustcaptcha-python-1.0.1/src/trustcaptcha/captcha_manager.py` & `trustcaptcha_python-1.1.0/src/trustcaptcha/captcha_manager.py`

 * *Files identical despite different names*

### Comparing `trustcaptcha-python-1.0.1/src/trustcaptcha/model/verification_result.py` & `trustcaptcha_python-1.1.0/src/trustcaptcha/model/verification_result.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import json
 from dataclasses import dataclass, asdict
 from uuid import UUID
 
-from .result_reason import ResultReason
-
-
 @dataclass
 class VerificationResult:
     captchaId: UUID
     verificationId: UUID
     score: float
-    reason: ResultReason
+    reason: str
+    mode: str
     origin: str
     ipAddress: str
     deviceFamily: str
     operatingSystem: str
     browser: str
     creationTimestamp: str
     releaseTimestamp: str
@@ -27,15 +25,16 @@
     @classmethod
     def from_json(cls, json_data):
         data = json.loads(json_data) if isinstance(json_data, str) else json_data
         return cls(
             captchaId=UUID(data['captchaId']),
             verificationId=UUID(data['verificationId']),
             score=data['score'],
-            reason=ResultReason(data['reason']),
+            reason=data['reason'],
+            mode=data['mode'],
             origin=data['origin'],
             ipAddress=data['ipAddress'],
             deviceFamily=data['deviceFamily'],
             operatingSystem=data['operatingSystem'],
             browser=data['browser'],
             creationTimestamp=data['creationTimestamp'],
             releaseTimestamp=data['releaseTimestamp'],
```

### Comparing `trustcaptcha-python-1.0.1/src/trustcaptcha/model/verification_token.py` & `trustcaptcha_python-1.1.0/src/trustcaptcha/model/verification_token.py`

 * *Files identical despite different names*

### Comparing `trustcaptcha-python-1.0.1/src/trustcaptcha_python.egg-info/PKG-INFO` & `trustcaptcha_python-1.1.0/src/trustcaptcha_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustcaptcha-python
-Version: 1.0.1
+Version: 1.1.0
 Summary: Trustcaptcha library for python
 Author-email: Trustcaptcha GmbH <mail@trustcaptcha.com>
 License: Apache-2.0
 Keywords: captcha,gdpr,privacy,security,made-in-germany,eu,european-union
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: numpy
```

### Comparing `trustcaptcha-python-1.0.1/src/trustcaptcha_python.egg-info/SOURCES.txt` & `trustcaptcha_python-1.1.0/src/trustcaptcha_python.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 README.md
 pyproject.toml
 src/trustcaptcha/__init__.py
 src/trustcaptcha/aes_encryption.py
 src/trustcaptcha/captcha_manager.py
 src/trustcaptcha/model/__init__.py
-src/trustcaptcha/model/result_reason.py
 src/trustcaptcha/model/verification_result.py
 src/trustcaptcha/model/verification_token.py
 src/trustcaptcha_python.egg-info/PKG-INFO
 src/trustcaptcha_python.egg-info/SOURCES.txt
 src/trustcaptcha_python.egg-info/dependency_links.txt
 src/trustcaptcha_python.egg-info/entry_points.txt
 src/trustcaptcha_python.egg-info/requires.txt
```


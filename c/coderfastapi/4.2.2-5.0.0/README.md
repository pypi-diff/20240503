# Comparing `tmp/coderfastapi-4.2.2.tar.gz` & `tmp/coderfastapi-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coderfastapi-4.2.2.tar", last modified: Wed Apr  3 14:47:15 2024, max compression
+gzip compressed data, was "coderfastapi-5.0.0.tar", last modified: Fri May  3 09:38:33 2024, max compression
```

## Comparing `coderfastapi-4.2.2.tar` & `coderfastapi-5.0.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.422729 coderfastapi-4.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-03 14:47:15.422729 coderfastapi-4.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.402729 coderfastapi-4.2.2/coderfastapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.402729 coderfastapi-4.2.2/coderfastapi/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/handlers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.406729 coderfastapi-4.2.2/coderfastapi/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.406729 coderfastapi-4.2.2/coderfastapi/lib/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/decorators/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.406729 coderfastapi-4.2.2/coderfastapi/lib/security/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/acl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.406729 coderfastapi-4.2.2/coderfastapi/lib/security/policies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.406729 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.406729 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/jwt/
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/jwt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.410729 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/jwt/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/jwt/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/jwt/providers/expiration.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/jwt/providers/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.410729 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authorization/
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authorization/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.410729 coderfastapi-4.2.2/coderfastapi/lib/security/session/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/session/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/session/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.410729 coderfastapi-4.2.2/coderfastapi/lib/validation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.414729 coderfastapi-4.2.2/coderfastapi/lib/validation/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/validation/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/validation/schemas/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/validation/schemas/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/validation/schemas/request.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/validation/schemas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.414729 coderfastapi-4.2.2/coderfastapi/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/logging/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/logging/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/logging/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.414729 coderfastapi-4.2.2/coderfastapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-03 14:47:15.000000 coderfastapi-4.2.2/coderfastapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-03 14:47:15.000000 coderfastapi-4.2.2/coderfastapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:47:15.000000 coderfastapi-4.2.2/coderfastapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-03 14:47:15.000000 coderfastapi-4.2.2/coderfastapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 14:47:15.000000 coderfastapi-4.2.2/coderfastapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:47:15.422729 coderfastapi-4.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:33.279255 coderfastapi-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-03 09:38:33.275255 coderfastapi-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:33.259255 coderfastapi-5.0.0/coderfastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:33.263255 coderfastapi-5.0.0/coderfastapi/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/handlers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:33.263255 coderfastapi-5.0.0/coderfastapi/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:33.263255 coderfastapi-5.0.0/coderfastapi/lib/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/decorators/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:33.263255 coderfastapi-5.0.0/coderfastapi/lib/security/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/security/acl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:33.263255 coderfastapi-5.0.0/coderfastapi/lib/security/policies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/security/policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:33.263255 coderfastapi-5.0.0/coderfastapi/lib/security/policies/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/security/policies/authentication/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:33.267255 coderfastapi-5.0.0/coderfastapi/lib/security/policies/authentication/jwt/
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/security/policies/authentication/jwt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:33.267255 coderfastapi-5.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/expiration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/security/policies/authentication/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:33.267255 coderfastapi-5.0.0/coderfastapi/lib/security/policies/authorization/
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/security/policies/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/security/policies/authorization/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:33.267255 coderfastapi-5.0.0/coderfastapi/lib/security/session/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/security/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/security/session/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/security/session/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:33.267255 coderfastapi-5.0.0/coderfastapi/lib/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:33.271255 coderfastapi-5.0.0/coderfastapi/lib/validation/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/validation/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/validation/schemas/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/validation/schemas/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/validation/schemas/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/lib/validation/schemas/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:33.271255 coderfastapi-5.0.0/coderfastapi/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/logging/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/logging/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/logging/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/coderfastapi/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:33.271255 coderfastapi-5.0.0/coderfastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-03 09:38:33.000000 coderfastapi-5.0.0/coderfastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-03 09:38:33.000000 coderfastapi-5.0.0/coderfastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:38:33.000000 coderfastapi-5.0.0/coderfastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-03 09:38:33.000000 coderfastapi-5.0.0/coderfastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 09:38:33.000000 coderfastapi-5.0.0/coderfastapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-03 09:37:31.000000 coderfastapi-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 09:38:33.279255 coderfastapi-5.0.0/setup.cfg
```

### Comparing `coderfastapi-4.2.2/PKG-INFO` & `coderfastapi-5.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: coderfastapi
-Version: 4.2.2
+Version: 5.0.0
 Summary: coderfastapi
 Author-email: Code R <hello@coderstudio.dev>
 Description-Content-Type: text/markdown
-Requires-Dist: codercore~=5.0
+Requires-Dist: codercore~=6.0
 Requires-Dist: fastapi[all]~=0.89
 Requires-Dist: google-cloud-logging~=3.7
 Requires-Dist: orjson~=3.8
 Requires-Dist: pydantic~=2.4
 Requires-Dist: python-jose~=3.3
 Provides-Extra: test
 Requires-Dist: pytest~=7.2; extra == "test"
```

### Comparing `coderfastapi-4.2.2/coderfastapi/lib/decorators/__init__.py` & `coderfastapi-5.0.0/coderfastapi/lib/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.2/coderfastapi/lib/decorators/pagination.py` & `coderfastapi-5.0.0/coderfastapi/lib/decorators/pagination.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.2/coderfastapi/lib/router.py` & `coderfastapi-5.0.0/coderfastapi/lib/router.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/jwt/__init__.py` & `coderfastapi-5.0.0/coderfastapi/lib/security/policies/authentication/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py` & `coderfastapi-5.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/jwt/providers/user.py` & `coderfastapi-5.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/user.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/session.py` & `coderfastapi-5.0.0/coderfastapi/lib/security/policies/authentication/session.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.2/coderfastapi/lib/security/policies/authorization/__init__.py` & `coderfastapi-5.0.0/coderfastapi/lib/security/policies/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.2/coderfastapi/lib/security/policies/authorization/user.py` & `coderfastapi-5.0.0/coderfastapi/lib/security/policies/authorization/user.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.2/coderfastapi/lib/security/session/base.py` & `coderfastapi-5.0.0/coderfastapi/lib/security/session/base.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.2/coderfastapi/lib/security/session/user.py` & `coderfastapi-5.0.0/coderfastapi/lib/security/session/user.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.2/coderfastapi/lib/signature.py` & `coderfastapi-5.0.0/coderfastapi/lib/signature.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.2/coderfastapi/lib/validation/schemas/query.py` & `coderfastapi-5.0.0/coderfastapi/lib/validation/schemas/query.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.2/coderfastapi/lib/validation/schemas/request.py` & `coderfastapi-5.0.0/coderfastapi/lib/validation/schemas/request.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.2/coderfastapi/logging/__init__.py` & `coderfastapi-5.0.0/coderfastapi/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.2/coderfastapi/logging/context.py` & `coderfastapi-5.0.0/coderfastapi/logging/context.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.2/coderfastapi/logging/filter.py` & `coderfastapi-5.0.0/coderfastapi/logging/filter.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.2/coderfastapi/logging/middleware.py` & `coderfastapi-5.0.0/coderfastapi/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.2/coderfastapi.egg-info/PKG-INFO` & `coderfastapi-5.0.0/coderfastapi.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: coderfastapi
-Version: 4.2.2
+Version: 5.0.0
 Summary: coderfastapi
 Author-email: Code R <hello@coderstudio.dev>
 Description-Content-Type: text/markdown
-Requires-Dist: codercore~=5.0
+Requires-Dist: codercore~=6.0
 Requires-Dist: fastapi[all]~=0.89
 Requires-Dist: google-cloud-logging~=3.7
 Requires-Dist: orjson~=3.8
 Requires-Dist: pydantic~=2.4
 Requires-Dist: python-jose~=3.3
 Provides-Extra: test
 Requires-Dist: pytest~=7.2; extra == "test"
```

### Comparing `coderfastapi-4.2.2/coderfastapi.egg-info/SOURCES.txt` & `coderfastapi-5.0.0/coderfastapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.2/pyproject.toml` & `coderfastapi-5.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coderfastapi"
-version = "4.2.2"
+version = "5.0.0"
 description = "coderfastapi"
 readme = "README.md"
 authors = [{ name = "Code R", email = "hello@coderstudio.dev" }]
 dependencies = [
-    'codercore ~= 5.0',
+    'codercore ~= 6.0',
     'fastapi[all] ~= 0.89',
     'google-cloud-logging ~= 3.7',
     'orjson ~= 3.8',
     'pydantic ~= 2.4',
     'python-jose ~= 3.3',
 ]
 
@@ -29,15 +29,15 @@
     'black ~= 22.12',
     'bumpver ~= 2023.1127',
     'flake8 ~= 6.0',
     'isort ~= 5.12',
 ]
 
 [tool.bumpver]
-current_version = "4.2.2"
+current_version = "5.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```


# Comparing `tmp/wagtail-cjk404-23.7.1.tar.gz` & `tmp/wagtail_cjk404-24.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-cjk404-23.7.1.tar", last modified: Tue Jul 11 06:48:08 2023, max compression
+gzip compressed data, was "wagtail_cjk404-24.5.1.tar", last modified: Fri May  3 08:27:23 2024, max compression
```

## Comparing `wagtail-cjk404-23.7.1.tar` & `wagtail_cjk404-24.5.1.tar`

### file list

```diff
@@ -1,33 +1,40 @@
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-11 06:48:08.394096 wagtail-cjk404-23.7.1/
--rw-r--r--   0 grze      (1000) grze      (1000)     1542 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/LICENSE
--rw-r--r--   0 grze      (1000) grze      (1000)       59 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/MANIFEST.in
--rw-r--r--   0 grze      (1000) grze      (1000)     5477 2023-07-11 06:48:08.394096 wagtail-cjk404-23.7.1/PKG-INFO
--rw-r--r--   0 grze      (1000) grze      (1000)     4433 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/README.md
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-11 06:48:08.394096 wagtail-cjk404-23.7.1/cjk404/
--rw-r--r--   0 grze      (1000) grze      (1000)      315 2023-07-11 06:47:53.000000 wagtail-cjk404-23.7.1/cjk404/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)      219 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/apps.py
--rw-r--r--   0 grze      (1000) grze      (1000)     6696 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/middleware.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-11 06:48:08.394096 wagtail-cjk404-23.7.1/cjk404/migrations/
--rw-r--r--   0 grze      (1000) grze      (1000)     1391 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/migrations/0001_initial.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1968 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/migrations/0001_squashed_0006_auto_20211011_2219.py
--rw-r--r--   0 grze      (1000) grze      (1000)      442 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/migrations/0002_alter_pagenotfoundentry_id.py
--rw-r--r--   0 grze      (1000) grze      (1000)      680 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/migrations/0002_pagenotfoundentry_fallback_redirect.py
--rw-r--r--   0 grze      (1000) grze      (1000)      704 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/migrations/0003_alter_pagenotfoundentry_redirect_to_url_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)      417 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/migrations/0003_pagenotfoundentry_regular_expression.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2007 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/migrations/0004_auto_20210830_1007.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1891 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/migrations/0005_auto_20211011_2131.py
--rw-r--r--   0 grze      (1000) grze      (1000)      820 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/migrations/0006_auto_20211011_2219.py
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/migrations/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2607 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/models.py
--rw-r--r--   0 grze      (1000) grze      (1000)     7278 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/tests.py
--rw-r--r--   0 grze      (1000) grze      (1000)      434 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/testsettings.py
--rw-r--r--   0 grze      (1000) grze      (1000)      802 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/wagtail_hooks.py
--rw-r--r--   0 grze      (1000) grze      (1000)       93 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/pyproject.toml
--rw-r--r--   0 grze      (1000) grze      (1000)     1079 2023-07-11 06:48:08.394096 wagtail-cjk404-23.7.1/setup.cfg
--rw-r--r--   0 grze      (1000) grze      (1000)       38 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/setup.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-11 06:48:08.394096 wagtail-cjk404-23.7.1/wagtail_cjk404.egg-info/
--rw-r--r--   0 grze      (1000) grze      (1000)     5477 2023-07-11 06:48:08.000000 wagtail-cjk404-23.7.1/wagtail_cjk404.egg-info/PKG-INFO
--rw-r--r--   0 grze      (1000) grze      (1000)      898 2023-07-11 06:48:08.000000 wagtail-cjk404-23.7.1/wagtail_cjk404.egg-info/SOURCES.txt
--rw-r--r--   0 grze      (1000) grze      (1000)        1 2023-07-11 06:48:08.000000 wagtail-cjk404-23.7.1/wagtail_cjk404.egg-info/dependency_links.txt
--rw-r--r--   0 grze      (1000) grze      (1000)       15 2023-07-11 06:48:08.000000 wagtail-cjk404-23.7.1/wagtail_cjk404.egg-info/requires.txt
--rw-r--r--   0 grze      (1000) grze      (1000)        7 2023-07-11 06:48:08.000000 wagtail-cjk404-23.7.1/wagtail_cjk404.egg-info/top_level.txt
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-03 08:27:23.939193 wagtail_cjk404-24.5.1/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1542 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/LICENSE
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      137 2024-05-03 08:15:31.000000 wagtail_cjk404-24.5.1/MANIFEST.in
+-rw-r--r--   0 grzegorz  (1000) grzegorz  (1000)     5781 2024-05-03 08:27:23.939193 wagtail_cjk404-24.5.1/PKG-INFO
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     4425 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/README.md
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-03 08:27:23.927192 wagtail_cjk404-24.5.1/cjk404/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      120 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/cjk404/.gitignore
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      315 2024-05-03 08:01:10.000000 wagtail_cjk404-24.5.1/cjk404/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      219 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/cjk404/apps.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     6592 2024-05-03 07:50:02.000000 wagtail_cjk404-24.5.1/cjk404/middleware.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-03 08:27:23.931192 wagtail_cjk404-24.5.1/cjk404/migrations/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1391 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/cjk404/migrations/0001_initial.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1968 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/cjk404/migrations/0001_squashed_0006_auto_20211011_2219.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      442 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/cjk404/migrations/0002_alter_pagenotfoundentry_id.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      680 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/cjk404/migrations/0002_pagenotfoundentry_fallback_redirect.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      704 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/cjk404/migrations/0003_alter_pagenotfoundentry_redirect_to_url_and_more.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      417 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/cjk404/migrations/0003_pagenotfoundentry_regular_expression.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      458 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/cjk404/migrations/0004_alter_pagenotfoundentry_url.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2007 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/cjk404/migrations/0004_auto_20210830_1007.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1891 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/cjk404/migrations/0005_auto_20211011_2131.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      820 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/cjk404/migrations/0006_auto_20211011_2219.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/cjk404/migrations/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2608 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/cjk404/models.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     7697 2024-05-03 07:55:36.000000 wagtail_cjk404-24.5.1/cjk404/tests.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      434 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/cjk404/testsettings.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      786 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/cjk404/wagtail_hooks.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-03 08:27:23.931192 wagtail_cjk404-24.5.1/docs/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    76563 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/docs/404.png
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)   469564 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/docs/All Redirects.jpg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)   320607 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/docs/Edit Redirect.jpg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1551 2024-05-03 08:27:08.000000 wagtail_cjk404-24.5.1/pyproject.toml
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       21 2024-05-03 08:04:53.000000 wagtail_cjk404-24.5.1/requirements-dev.txt
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1079 2024-05-03 08:27:23.939193 wagtail_cjk404-24.5.1/setup.cfg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       38 2024-05-03 07:37:44.000000 wagtail_cjk404-24.5.1/setup.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-03 08:27:23.935193 wagtail_cjk404-24.5.1/wagtail_cjk404.egg-info/
+-rw-r--r--   0 grzegorz  (1000) grzegorz  (1000)     5781 2024-05-03 08:27:23.000000 wagtail_cjk404-24.5.1/wagtail_cjk404.egg-info/PKG-INFO
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1050 2024-05-03 08:27:23.000000 wagtail_cjk404-24.5.1/wagtail_cjk404.egg-info/SOURCES.txt
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        1 2024-05-03 08:27:23.000000 wagtail_cjk404-24.5.1/wagtail_cjk404.egg-info/dependency_links.txt
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       43 2024-05-03 08:27:23.000000 wagtail_cjk404-24.5.1/wagtail_cjk404.egg-info/requires.txt
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        7 2024-05-03 08:27:23.000000 wagtail_cjk404-24.5.1/wagtail_cjk404.egg-info/top_level.txt
```

### Comparing `wagtail-cjk404-23.7.1/LICENSE` & `wagtail_cjk404-24.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-cjk404-23.7.1/PKG-INFO` & `wagtail_cjk404-24.5.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 Metadata-Version: 2.1
 Name: wagtail-cjk404
-Version: 23.7.1
-Summary: A Wagtail app to automatically log and/or manually create of redirects for 404 pages from within Wagtail admin panel.
+Version: 24.5.1
+Summary: 404 handler for Wagtail, with regexp support
 Home-page: https://github.com/cjkpl/wagtail-cjk404
 Author: Grzegorz Krol, Filip Wozniak
-Author-email: gk@cjk.pl, fw@cjk.pl
-License: BSD-3-Clause  # Example license
+Author-email: Grzegorz Krol <gk@cjk.pl>
+License: BSD-3-Clause
+Project-URL: Homepage, https://github.com/cjkpl/wagtail-cjk404
+Project-URL: Repository, https://github.com/cjkpl/wagtail-cjk404
+Keywords: wagtail,django,cms
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Wagtail :: 5
+Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Wagtail>=4.0.1
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: codespell; extra == "dev"
+Requires-Dist: build; extra == "dev"
 
 ![PyPI - Python Vesion](https://img.shields.io/pypi/pyversions/wagtail-cjk404)
 [![GitHub license](https://img.shields.io/github/license/cjkpl/wagtail-cjk404)](https://github.com/cjkpl/wagtail-cjk404/blob/main/LICENSE)
 [![GitHub issues](https://img.shields.io/github/issues/cjkpl/wagtail-cjk404)](https://github.com/cjkpl/wagtail-cjk404/issues) 
 
 
 # Managed 404 Pages with Redirects
@@ -91,15 +101,15 @@
 
 
 2. Add 'cjk404' to the INSTALLED_APPS:
 
 ```python
 INSTALLED_APPS = [
     ...
-    'wagtail.contrib.modeladmin', # required dependency
+    'wagtail_modeladmin', # required dependency
     'cjk404'
     ...
 ]
 ```
 
 3. Add the supplied middleware. You may also want to disable Wagtail's default ```RedirectMiddleware```:
```

### Comparing `wagtail-cjk404-23.7.1/README.md` & `wagtail_cjk404-24.5.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 
 2. Add 'cjk404' to the INSTALLED_APPS:
 
 ```python
 INSTALLED_APPS = [
     ...
-    'wagtail.contrib.modeladmin', # required dependency
+    'wagtail_modeladmin', # required dependency
     'cjk404'
     ...
 ]
 ```
 
 3. Add the supplied middleware. You may also want to disable Wagtail's default ```RedirectMiddleware```:
```

### Comparing `wagtail-cjk404-23.7.1/cjk404/middleware.py` & `wagtail_cjk404-24.5.1/cjk404/middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 import re
-from sys import stdout
-
-from django import http
 from django.conf import settings
 from django.core.cache import cache
-from django.core.exceptions import ImproperlyConfigured
 from django.http import HttpResponsePermanentRedirect, HttpResponseRedirect
 from django.utils.timezone import now
 
 from .models import PageNotFoundEntry
 from wagtail.models import Site
 
 IGNORED_404S = getattr(settings, "IGNORED_404S", [r"^/static/", r"^/favicon.ico"])
```

### Comparing `wagtail-cjk404-23.7.1/cjk404/migrations/0001_initial.py` & `wagtail_cjk404-24.5.1/cjk404/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjk404-23.7.1/cjk404/migrations/0001_squashed_0006_auto_20211011_2219.py` & `wagtail_cjk404-24.5.1/cjk404/migrations/0001_squashed_0006_auto_20211011_2219.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjk404-23.7.1/cjk404/migrations/0002_pagenotfoundentry_fallback_redirect.py` & `wagtail_cjk404-24.5.1/cjk404/migrations/0002_pagenotfoundentry_fallback_redirect.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjk404-23.7.1/cjk404/migrations/0003_alter_pagenotfoundentry_redirect_to_url_and_more.py` & `wagtail_cjk404-24.5.1/cjk404/migrations/0003_alter_pagenotfoundentry_redirect_to_url_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjk404-23.7.1/cjk404/migrations/0004_auto_20210830_1007.py` & `wagtail_cjk404-24.5.1/cjk404/migrations/0004_auto_20210830_1007.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjk404-23.7.1/cjk404/migrations/0005_auto_20211011_2131.py` & `wagtail_cjk404-24.5.1/cjk404/migrations/0005_auto_20211011_2131.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjk404-23.7.1/cjk404/migrations/0006_auto_20211011_2219.py` & `wagtail_cjk404-24.5.1/cjk404/migrations/0006_auto_20211011_2219.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjk404-23.7.1/cjk404/models.py` & `wagtail_cjk404-24.5.1/cjk404/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     site = models.ForeignKey(
         Site,
         related_name="pagenotfound_entries",
         on_delete=models.CASCADE,
         verbose_name="Site",
     )
 
-    url = models.CharField(max_length=400, verbose_name="Redirect from URL")
+    url = models.CharField(max_length=1000, verbose_name="Redirect from URL")
     redirect_to_url = models.CharField(
         max_length=400,
         null=True,
         blank=True,
         verbose_name="Redirect to URL",
     )
     redirect_to_page = models.ForeignKey(
```

### Comparing `wagtail-cjk404-23.7.1/cjk404/tests.py` & `wagtail_cjk404-24.5.1/cjk404/tests.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-from unittest.case import skipUnless
-
-from django.conf import settings
 from django.test import TestCase
-from django.test.utils import override_settings
 from django.core.cache import cache
 from wagtail.models import Site, Page
 from typing import Union, Optional
 
 from cjk404.middleware import (
     DJANGO_REGEX_REDIRECTS_CACHE_KEY,
     DJANGO_REGEX_REDIRECTS_CACHE_REGEX_KEY,
@@ -60,15 +56,15 @@
                 status_code=status_code,
                 target_status_code=target_status_code,
             )
         else:
             self.assertRedirects(response, expected_redirect_url)
 
     def test_model(self):
-        site = Site.objects.filter(is_default_site=True)[0]
+        # site = Site.objects.filter(is_default_site=True)[0]
         r1 = self.create_redirect("/initial/", "/new_target/")
         self.assertEqual(r1.__str__(), "/initial/ ---> /new_target/")
 
     def test_redirect(self):
         pnfe = self.create_redirect("/initial/", "/new_target/", None)
         self.assertEqual(pnfe.hits, 0)
         self.redirect_url("/initial/", "/new_target/", 302)
@@ -82,42 +78,57 @@
         pnfe.refresh_from_db()
         self.assertEqual(pnfe.hits, 1)
 
     def test_redirect_premanent(self):
         pnfe = self.create_redirect("/initial2/", "/new_target/", None, True)
         self.assertEqual(pnfe.hits, 0)
         self.redirect_url("/initial2/", "/new_target/", 301)
+        pnfe.refresh_from_db()
+        self.assertEqual(pnfe.hits, 1)
 
     def test_simple_redirect(self):
         pnfe = self.create_redirect("/news/index/b/", "/new_target/")
         self.redirect_url("/news/index/b/", "/new_target/", 302)
+        pnfe.refresh_from_db()
+        self.assertEqual(pnfe.hits, 1)
 
     def test_premanent_regular_expression_without_wildcard(self):
         pnfe = self.create_redirect("/news/index/b/", "/new_target/", None, True)
         self.redirect_url("/news/index/b/", "/new_target/", 301)
+        pnfe.refresh_from_db()
+        self.assertEqual(pnfe.hits, 1)
 
     def test_regular_expression_witout_replacement(self):
         pnfe = self.create_redirect("/news/index/.*/", "/news/boo/b/")
+        self.assertEqual(pnfe.hits, 0)
         self.redirect_url(
             "/news/index/.*/",
             "/news/boo/b/",
             302,
         )
+        pnfe.refresh_from_db()
+        self.assertEqual(pnfe.hits, 1)
 
     def test_regular_expression_with_replacement_302(self):
         pnfe = self.create_redirect(
             "/news01/index/(.*)/", "/news02/boo/$1/", None, False, True
         )
+        self.assertEqual(pnfe.hits, 0)
         self.redirect_url("/news01/index/b/", "/news02/boo/b/", 302, 404)
+        pnfe.refresh_from_db()
+        self.assertEqual(pnfe.hits, 1)
 
     def test_regular_expression_with_replacement_301(self):
-        pnfe1 = self.create_redirect(
+        pnfe = self.create_redirect(
             "/news03/index/(.*)/", "/news04/boo/$1/", None, True, True
         )
+        self.assertEqual(pnfe.hits, 0)
         self.redirect_url("/news03/index/b/", "/news04/boo/b/", 301, 404)
+        pnfe.refresh_from_db()
+        self.assertEqual(pnfe.hits, 1)
 
     def test_fallback_redirects(self):
         """
         Ensure redirects with fallback_redirect set are the last evaluated
         """
         site = Site.objects.filter(is_default_site=True)[0]
```

### Comparing `wagtail-cjk404-23.7.1/setup.cfg` & `wagtail_cjk404-24.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `wagtail-cjk404-23.7.1/wagtail_cjk404.egg-info/PKG-INFO` & `wagtail_cjk404-24.5.1/wagtail_cjk404.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 Metadata-Version: 2.1
 Name: wagtail-cjk404
-Version: 23.7.1
-Summary: A Wagtail app to automatically log and/or manually create of redirects for 404 pages from within Wagtail admin panel.
+Version: 24.5.1
+Summary: 404 handler for Wagtail, with regexp support
 Home-page: https://github.com/cjkpl/wagtail-cjk404
 Author: Grzegorz Krol, Filip Wozniak
-Author-email: gk@cjk.pl, fw@cjk.pl
-License: BSD-3-Clause  # Example license
+Author-email: Grzegorz Krol <gk@cjk.pl>
+License: BSD-3-Clause
+Project-URL: Homepage, https://github.com/cjkpl/wagtail-cjk404
+Project-URL: Repository, https://github.com/cjkpl/wagtail-cjk404
+Keywords: wagtail,django,cms
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Wagtail :: 5
+Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Wagtail>=4.0.1
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: codespell; extra == "dev"
+Requires-Dist: build; extra == "dev"
 
 ![PyPI - Python Vesion](https://img.shields.io/pypi/pyversions/wagtail-cjk404)
 [![GitHub license](https://img.shields.io/github/license/cjkpl/wagtail-cjk404)](https://github.com/cjkpl/wagtail-cjk404/blob/main/LICENSE)
 [![GitHub issues](https://img.shields.io/github/issues/cjkpl/wagtail-cjk404)](https://github.com/cjkpl/wagtail-cjk404/issues) 
 
 
 # Managed 404 Pages with Redirects
@@ -91,15 +101,15 @@
 
 
 2. Add 'cjk404' to the INSTALLED_APPS:
 
 ```python
 INSTALLED_APPS = [
     ...
-    'wagtail.contrib.modeladmin', # required dependency
+    'wagtail_modeladmin', # required dependency
     'cjk404'
     ...
 ]
 ```
 
 3. Add the supplied middleware. You may also want to disable Wagtail's default ```RedirectMiddleware```:
```

### Comparing `wagtail-cjk404-23.7.1/wagtail_cjk404.egg-info/SOURCES.txt` & `wagtail_cjk404-24.5.1/wagtail_cjk404.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+requirements-dev.txt
 setup.cfg
 setup.py
+cjk404/.gitignore
 cjk404/__init__.py
 cjk404/apps.py
 cjk404/middleware.py
 cjk404/models.py
 cjk404/tests.py
 cjk404/testsettings.py
 cjk404/wagtail_hooks.py
 cjk404/migrations/0001_initial.py
 cjk404/migrations/0001_squashed_0006_auto_20211011_2219.py
 cjk404/migrations/0002_alter_pagenotfoundentry_id.py
 cjk404/migrations/0002_pagenotfoundentry_fallback_redirect.py
 cjk404/migrations/0003_alter_pagenotfoundentry_redirect_to_url_and_more.py
 cjk404/migrations/0003_pagenotfoundentry_regular_expression.py
+cjk404/migrations/0004_alter_pagenotfoundentry_url.py
 cjk404/migrations/0004_auto_20210830_1007.py
 cjk404/migrations/0005_auto_20211011_2131.py
 cjk404/migrations/0006_auto_20211011_2219.py
 cjk404/migrations/__init__.py
+docs/404.png
+docs/All Redirects.jpg
+docs/Edit Redirect.jpg
 wagtail_cjk404.egg-info/PKG-INFO
 wagtail_cjk404.egg-info/SOURCES.txt
 wagtail_cjk404.egg-info/dependency_links.txt
 wagtail_cjk404.egg-info/requires.txt
 wagtail_cjk404.egg-info/top_level.txt
```


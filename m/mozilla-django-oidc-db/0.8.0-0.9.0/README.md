# Comparing `tmp/mozilla-django-oidc-db-0.8.0.tar.gz` & `tmp/mozilla-django-oidc-db-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla-django-oidc-db-0.8.0.tar", last modified: Tue Feb 15 12:09:52 2022, max compression
+gzip compressed data, was "mozilla-django-oidc-db-0.9.0.tar", last modified: Thu Apr 21 15:15:29 2022, max compression
```

## Comparing `mozilla-django-oidc-db-0.8.0.tar` & `mozilla-django-oidc-db-0.9.0.tar`

### file list

```diff
@@ -1,46 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 12:09:52.756974 mozilla-django-oidc-db-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2960 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8817 2022-02-15 12:09:52.756974 mozilla-django-oidc-db-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7849 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 12:09:52.752974 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1617 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     6075 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/backends.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2218 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 12:09:52.756974 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     4706 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      723 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/migrations/0002_openidconnectconfig_oidc_op_discovery_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/migrations/0003_auto_20210719_0803.py
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/migrations/0004_auto_20210812_1044.py
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/migrations/0005_openidconnectconfig_sync_groups_glob_pattern.py
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/migrations/0006_openidconnectconfig_unique_id_claim.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      872 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)     8249 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 12:09:52.752974 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8817 2022-02-15 12:09:52.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-02-15 12:09:52.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-15 12:09:52.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-15 12:09:52.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-02-15 12:09:52.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-02-15 12:09:52.000000 mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1819 2022-02-15 12:09:52.756974 mozilla-django-oidc-db-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 12:09:52.756974 mozilla-django-oidc-db-0.8.0/testapp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/testapp/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/testapp/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 12:09:52.756974 mozilla-django-oidc-db-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     6379 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/tests/test_admin_form.py
--rw-r--r--   0 runner    (1001) docker     (121)    13313 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     3122 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)     3059 2022-02-15 12:09:45.000000 mozilla-django-oidc-db-0.8.0/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 15:15:29.393849 mozilla-django-oidc-db-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     3894 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     9732 2022-04-21 15:15:29.393849 mozilla-django-oidc-db-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8764 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 15:15:29.385849 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7177 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/backends.py
+-rw-r--r--   0 runner    (1001) docker     (121)      305 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2218 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/forms.py
+-rw-r--r--   0 runner    (1001) docker     (121)      779 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 15:15:29.389849 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     4706 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/migrations/0002_openidconnectconfig_oidc_op_discovery_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)      867 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/migrations/0003_auto_20210719_0803.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2029 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/migrations/0004_auto_20210812_1044.py
+-rw-r--r--   0 runner    (1001) docker     (121)      655 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/migrations/0005_openidconnectconfig_sync_groups_glob_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (121)      641 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/migrations/0006_openidconnectconfig_unique_id_claim.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2077 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/migrations/0007_auto_20220307_1128.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9986 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 15:15:29.385849 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 15:15:29.389849 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (121)      628 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/templates/admin/oidc_failure.html
+-rw-r--r--   0 runner    (1001) docker     (121)      976 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 15:15:29.389849 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     9732 2022-04-21 15:15:28.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1630 2022-04-21 15:15:29.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-21 15:15:28.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-21 15:15:28.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-04-21 15:15:29.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-04-21 15:15:29.000000 mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-04-21 15:15:29.393849 mozilla-django-oidc-db-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 15:15:29.389849 mozilla-django-oidc-db-0.9.0/testapp/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/testapp/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/testapp/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 15:15:29.389849 mozilla-django-oidc-db-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6689 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/tests/test_admin_form.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15969 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3556 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1344 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3059 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6511 2022-04-21 15:15:23.000000 mozilla-django-oidc-db-0.9.0/tests/test_views.py
```

### Comparing `mozilla-django-oidc-db-0.8.0/LICENSE` & `mozilla-django-oidc-db-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla-django-oidc-db-0.8.0/PKG-INFO` & `mozilla-django-oidc-db-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-django-oidc-db
-Version: 0.8.0
+Version: 0.9.0
 Summary: A database-backed configuration for mozilla-django-oidc
 Home-page: https://github.com/maykinmedia/mozilla-django-oidc-db
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Keywords: OIDC,django,database,authentication
 Platform: UNKNOWN
@@ -31,15 +31,15 @@
 .. mozilla_django_oidc_db documentation master file, created by startproject.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 Welcome to mozilla_django_oidc_db's documentation!
 ==================================================
 
-:Version: 0.8.0
+:Version: 0.9.0
 :Source: https://github.com/maykinmedia/mozilla-django-oidc-db
 :Keywords: OIDC, django, database, authentication
 :PythonVersion: 3.7
 
 |build-status| |coverage| |black|
 
 |python-versions| |django-versions| |pypi-version|
@@ -139,17 +139,30 @@
     ]
 
 Furthermore, ensure the following settings are configured:
 
 .. code-block:: python
 
     OIDC_AUTHENTICATE_CLASS = "mozilla_django_oidc_db.views.OIDCAuthenticationRequestView"
+    OIDC_CALLBACK_CLASS = "mozilla_django_oidc_db.views.OIDCCallbackView"
     MOZILLA_DJANGO_OIDC_DB_CACHE = "oidc"
     MOZILLA_DJANGO_OIDC_DB_CACHE_TIMEOUT = 1
 
+In order to properly catch admin login errors, add the following to urlpatterns:
+
+.. code-block:: python
+
+    from mozilla_django_oidc_db.views import AdminLoginFailure
+
+    urlpatterns = [
+        ...
+        path("admin/login/failure/", AdminLoginFailure.as_view(), name="admin-oidc-error"),
+        ...
+    ]
+
 ``MOZILLA_DJANGO_OIDC_DB_CACHE`` is used to cache the configuration that is stored in the database,
 to prevent a lot of database lookups. Ensure this cache is configured in ``CACHES`` (using the backend of choice):
 
 .. code-block:: python
 
     CACHES = {
         "default": {"BACKEND": "django.core.cache.backends.locmem.LocMemCache"},
@@ -229,14 +242,36 @@
 Custom username claim
 ---------------------
 
 The name of the claim that is used for the ``User.username`` property
 can be configured via the admin. By default, the username is derived from the ``sub`` claim that
 is returned by the OIDC provider.
 
+If the desired claim is nested in one or more objects, its path can be specified with dots, e.g.:
+
+.. code-block:: json
+
+    {
+        "some": {
+            "nested": {
+                "claim": "foo"
+            }
+        }
+    }
+
+Can be retrieved by setting the username claim to ``some.nested.claim``
+
+**NOTE**: the username claim does not support claims that have dots in their name, it cannot be configured to retrieve the following claim for instance:
+
+.. code-block:: json
+
+    {
+        "some.dotted.claim": "foo"
+    }
+
 .. |build-status| image:: https://github.com/maykinmedia/mozilla-django-oidc-db/workflows/Run%20CI/badge.svg?branch=master
     :target: https://github.com/maykinmedia/mozilla-django-oidc-db/actions?query=workflow%3A%22Run+CI%22+branch%3Amaster
 
 .. |coverage| image:: https://codecov.io/gh/maykinmedia/mozilla-django-oidc-db/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/maykinmedia/mozilla-django-oidc-db
     :alt: Coverage status
```

### Comparing `mozilla-django-oidc-db-0.8.0/README.rst` & `mozilla-django-oidc-db-0.9.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 .. mozilla_django_oidc_db documentation master file, created by startproject.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 Welcome to mozilla_django_oidc_db's documentation!
 ==================================================
 
-:Version: 0.8.0
+:Version: 0.9.0
 :Source: https://github.com/maykinmedia/mozilla-django-oidc-db
 :Keywords: OIDC, django, database, authentication
 :PythonVersion: 3.7
 
 |build-status| |coverage| |black|
 
 |python-versions| |django-versions| |pypi-version|
@@ -111,17 +111,30 @@
     ]
 
 Furthermore, ensure the following settings are configured:
 
 .. code-block:: python
 
     OIDC_AUTHENTICATE_CLASS = "mozilla_django_oidc_db.views.OIDCAuthenticationRequestView"
+    OIDC_CALLBACK_CLASS = "mozilla_django_oidc_db.views.OIDCCallbackView"
     MOZILLA_DJANGO_OIDC_DB_CACHE = "oidc"
     MOZILLA_DJANGO_OIDC_DB_CACHE_TIMEOUT = 1
 
+In order to properly catch admin login errors, add the following to urlpatterns:
+
+.. code-block:: python
+
+    from mozilla_django_oidc_db.views import AdminLoginFailure
+
+    urlpatterns = [
+        ...
+        path("admin/login/failure/", AdminLoginFailure.as_view(), name="admin-oidc-error"),
+        ...
+    ]
+
 ``MOZILLA_DJANGO_OIDC_DB_CACHE`` is used to cache the configuration that is stored in the database,
 to prevent a lot of database lookups. Ensure this cache is configured in ``CACHES`` (using the backend of choice):
 
 .. code-block:: python
 
     CACHES = {
         "default": {"BACKEND": "django.core.cache.backends.locmem.LocMemCache"},
@@ -201,14 +214,36 @@
 Custom username claim
 ---------------------
 
 The name of the claim that is used for the ``User.username`` property
 can be configured via the admin. By default, the username is derived from the ``sub`` claim that
 is returned by the OIDC provider.
 
+If the desired claim is nested in one or more objects, its path can be specified with dots, e.g.:
+
+.. code-block:: json
+
+    {
+        "some": {
+            "nested": {
+                "claim": "foo"
+            }
+        }
+    }
+
+Can be retrieved by setting the username claim to ``some.nested.claim``
+
+**NOTE**: the username claim does not support claims that have dots in their name, it cannot be configured to retrieve the following claim for instance:
+
+.. code-block:: json
+
+    {
+        "some.dotted.claim": "foo"
+    }
+
 .. |build-status| image:: https://github.com/maykinmedia/mozilla-django-oidc-db/workflows/Run%20CI/badge.svg?branch=master
     :target: https://github.com/maykinmedia/mozilla-django-oidc-db/actions?query=workflow%3A%22Run+CI%22+branch%3Amaster
 
 .. |coverage| image:: https://codecov.io/gh/maykinmedia/mozilla-django-oidc-db/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/maykinmedia/mozilla-django-oidc-db
     :alt: Coverage status
```

### Comparing `mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/admin.py` & `mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/admin.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,8 +49,22 @@
                     "claim_mapping",
                     "sync_groups",
                     "sync_groups_glob_pattern",
                     "make_users_staff",
                 )
             },
         ),
+        (
+            _("Advanced settings"),
+            {
+                "fields": (
+                    "oidc_use_nonce",
+                    "oidc_nonce_size",
+                    "oidc_state_size",
+                    "oidc_exempt_urls",
+                ),
+                "classes": [
+                    "collapse in",
+                ],
+            },
+        ),
     )
```

### Comparing `mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/backends.py` & `mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/backends.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,97 +1,120 @@
 import fnmatch
 import logging
+from typing import Any, Dict
 
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import Group
 from django.core.exceptions import ObjectDoesNotExist
 
+from glom import glom
 from mozilla_django_oidc.auth import (
     OIDCAuthenticationBackend as _OIDCAuthenticationBackend,
 )
 
-from .mixins import SoloConfigMixin
+from .mixins import GetAttributeMixin, SoloConfigMixin
+from .utils import obfuscate_claims
 
 logger = logging.getLogger(__name__)
 
 
-class OIDCAuthenticationBackend(SoloConfigMixin, _OIDCAuthenticationBackend):
+class OIDCAuthenticationBackend(
+    GetAttributeMixin, SoloConfigMixin, _OIDCAuthenticationBackend
+):
     """
     Modifies the default OIDCAuthenticationBackend to use a configurable claim
     as unique identifier (default `sub`).
     """
 
-    def __getattribute__(self, attr):
-        if attr.startswith("OIDC"):
-            return self.get_settings(attr, None)
-        return super().__getattribute__(attr)
+    config_identifier_field = "username_claim"
+    sensitive_claim_names = []
 
     def __init__(self, *args, **kwargs):
         self.UserModel = get_user_model()
 
         # See: https://github.com/maykinmedia/mozilla-django-oidc-db/issues/30
         # `super().__init__` is not called here, because this attempts to initialize
         # the settings (which should be retrieved from `OpenIDConnectConfig`).
 
         # The retrieval of these settings has been moved to runtime (`__getattribute__`)
         # to avoid a large number of `OpenIDConnectConfig.get_solo` calls when
         # `OIDCAuthenticationBackend.__init__` is called for permission checks
 
+    def retrieve_identifier_claim(self, claims: dict) -> str:
+        # NOTE: this does not support the extraction of claims that contain dots "." in
+        # their name (e.g. {"foo.bar": "baz"})
+        identifier_claim_name = getattr(self.config, self.config_identifier_field)
+        unique_id = glom(claims, identifier_claim_name, default="")
+        return unique_id
+
+    def get_sensitive_claims_names(self) -> list:
+        """
+        Defines the claims that should be obfuscated before logging claims.
+        Nested claims can be specified by using a dotted path (e.g. "foo.bar.baz")
+
+        NOTE: this does not support claim names that have dots in them, so the following
+        claim cannot be marked as a sensitive claim
+
+            {
+                "foo.bar": "baz"
+            }
+        """
+        identifier_claim_name = getattr(self.config, self.config_identifier_field)
+        return [identifier_claim_name] + self.sensitive_claim_names
+
     def authenticate(self, *args, **kwargs):
         if not self.config.enabled:
             return None
 
         return super().authenticate(*args, **kwargs)
 
-    def get_user_instance_values(self, claims):
+    def get_user_instance_values(self, claims) -> Dict[str, Any]:
         """
         Map the names and values of the claims to the fields of the User model
         """
         return {
-            model_field: claims.get(claims_field, "")
+            model_field: glom(claims, claims_field, default="")
             for model_field, claims_field in self.config.claim_mapping.items()
         }
 
     def create_user(self, claims):
         """Return object for a newly created user account."""
-        username_claim = self.config.username_claim
-        unique_id = claims.get(username_claim)
+        unique_id = self.retrieve_identifier_claim(claims)
 
         logger.debug("Creating OIDC user: %s", unique_id)
 
         user = self.UserModel.objects.create_user(
             **{self.UserModel.USERNAME_FIELD: unique_id}
         )
         self.update_user(user, claims)
 
         return user
 
     def filter_users_by_claims(self, claims):
         """Return all users matching the specified subject."""
-        username_claim = self.config.username_claim
-        unique_id = claims.get(username_claim)
+        unique_id = self.retrieve_identifier_claim(claims)
 
         if not unique_id:
             return self.UserModel.objects.none()
         return self.UserModel.objects.filter(
             **{f"{self.UserModel.USERNAME_FIELD}__iexact": unique_id}
         )
 
-    def verify_claims(self, claims):
+    def verify_claims(self, claims) -> bool:
         """Verify the provided claims to decide if authentication should be allowed."""
-        scopes = self.get_settings("OIDC_RP_SCOPES", "openid email")
+        claims_to_obfuscate = self.get_sensitive_claims_names()
+        obfuscated_claims = obfuscate_claims(claims, claims_to_obfuscate)
 
-        logger.debug("OIDC claims received: %s", claims)
+        logger.debug("OIDC claims received: %s", obfuscated_claims)
 
-        username_claim = self.config.username_claim
-
-        if username_claim not in claims:
+        identifier_claim_name = getattr(self.config, self.config_identifier_field)
+        if not glom(claims, identifier_claim_name, default=""):
             logger.error(
                 "%s not in OIDC claims, cannot proceed with authentication",
-                username_claim,
+                identifier_claim_name,
             )
             return False
         return True
 
     def update_user(self, user, claims):
         """Update existing user with new claims, if necessary save, and return user"""
         values = self.get_user_instance_values(claims)
@@ -117,17 +140,16 @@
         Copied and modified from: https://github.com/snok/django-auth-adfs/blob/master/django_auth_adfs/backend.py
         """
         groups_claim = self.config.groups_claim
 
         if groups_claim:
             # Update the user's group memberships
             django_groups = [group.name for group in user.groups.all()]
-
-            if groups_claim in claims:
-                claim_groups = claims[groups_claim]
+            claim_groups = glom(claims, groups_claim, default=[])
+            if claim_groups:
                 if not isinstance(claim_groups, list):
                     claim_groups = [
                         claim_groups,
                     ]
             else:
                 logger.debug(
                     "The configured groups claim '%s' was not found in the access token",
```

### Comparing `mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/forms.py` & `mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/forms.py`

 * *Files identical despite different names*

### Comparing `mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/migrations/0001_initial.py` & `mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/migrations/0002_openidconnectconfig_oidc_op_discovery_endpoint.py` & `mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/migrations/0002_openidconnectconfig_oidc_op_discovery_endpoint.py`

 * *Files identical despite different names*

### Comparing `mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/migrations/0003_auto_20210719_0803.py` & `mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/migrations/0003_auto_20210719_0803.py`

 * *Files identical despite different names*

### Comparing `mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/migrations/0004_auto_20210812_1044.py` & `mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/migrations/0004_auto_20210812_1044.py`

 * *Files identical despite different names*

### Comparing `mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/migrations/0005_openidconnectconfig_sync_groups_glob_pattern.py` & `mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/migrations/0005_openidconnectconfig_sync_groups_glob_pattern.py`

 * *Files identical despite different names*

### Comparing `mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/migrations/0006_openidconnectconfig_unique_id_claim.py` & `mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/migrations/0006_openidconnectconfig_unique_id_claim.py`

 * *Files identical despite different names*

### Comparing `mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db/models.py` & `mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from typing import Dict
+from typing import Dict, List
 
+import django
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.contrib.postgres.fields import JSONField
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.utils.encoding import force_text
 from django.utils.translation import gettext_lazy as _
 
 from django_better_admin_arrayfield.models.fields import ArrayField
 from solo.models import SingletonModel, get_cache
 
 import mozilla_django_oidc_db.settings as oidc_settings
 
+from .compat import classproperty
 
-def get_default_scopes():
+
+def get_default_scopes() -> List[str]:
     """
     Returns the default scopes to request for OpenID Connect logins
     """
     return ["openid", "email", "profile"]
 
 
 def get_claim_mapping() -> Dict[str, str]:
@@ -27,17 +30,73 @@
     return {
         "email": "email",
         "first_name": "given_name",
         "last_name": "family_name",
     }
 
 
-class OpenIDConnectConfig(SingletonModel):
+class CachingMixin:
+    @classmethod
+    def clear_cache(cls):
+        cache_name = getattr(
+            settings, "OIDC_CACHE", oidc_settings.MOZILLA_DJANGO_OIDC_DB_CACHE
+        )
+        if cache_name:
+            cache = get_cache(cache_name)
+            cache_key = cls.get_cache_key()
+            cache.delete(cache_key)
+
+    def set_to_cache(self):
+        cache_name = getattr(
+            settings,
+            "MOZILLA_DJANGO_OIDC_DB_CACHE",
+            oidc_settings.MOZILLA_DJANGO_OIDC_DB_CACHE,
+        )
+        if not cache_name:
+            return None
+        cache = get_cache(cache_name)
+        cache_key = self.get_cache_key()
+        timeout = getattr(
+            settings,
+            "MOZILLA_DJANGO_OIDC_DB_CACHE_TIMEOUT",
+            oidc_settings.MOZILLA_DJANGO_OIDC_DB_CACHE_TIMEOUT,
+        )
+        cache.set(cache_key, self, timeout)
+
+    @classmethod
+    def get_cache_key(cls) -> str:
+        prefix = cls.custom_oidc_db_prefix or getattr(
+            settings,
+            "MOZILLA_DJANGO_OIDC_DB_PREFIX",
+            oidc_settings.MOZILLA_DJANGO_OIDC_DB_PREFIX,
+        )
+        return "%s:%s" % (prefix, cls.__name__.lower())
+
+    @classmethod
+    def get_solo(cls) -> SingletonModel:
+        cache_name = getattr(
+            settings,
+            "MOZILLA_DJANGO_OIDC_DB_CACHE",
+            oidc_settings.MOZILLA_DJANGO_OIDC_DB_CACHE,
+        )
+        if not cache_name:
+            obj, created = cls.objects.get_or_create(pk=cls.singleton_instance_id)
+            return obj
+        cache = get_cache(cache_name)
+        cache_key = cls.get_cache_key()
+        obj = cache.get(cache_key)
+        if not obj:
+            obj, created = cls.objects.get_or_create(pk=cls.singleton_instance_id)
+            obj.set_to_cache()
+        return obj
+
+
+class OpenIDConnectConfigBase(SingletonModel):
     """
-    Configuration for authentication/authorization via OpenID connect
+    Defines the required fields for a config to establish an OIDC connection
     """
 
     enabled = models.BooleanField(
         _("enable"),
         default=False,
         help_text=_(
             "Indicates whether OpenID Connect for authentication/authorization is enabled"
@@ -107,14 +166,67 @@
         max_length=1000,
         help_text=_(
             "Key the Identity Provider uses to sign ID tokens in the case of an RSA sign algorithm. Should be the signing key in PEM or DER format"
         ),
         blank=True,
     )
 
+    # Advanced settings
+    oidc_use_nonce = models.BooleanField(
+        _("Use nonce"),
+        help_text=_(
+            "Controls whether the OpenID Connect client uses nonce verification"
+        ),
+        default=True,
+    )
+    oidc_nonce_size = models.PositiveIntegerField(
+        _("Nonce size"),
+        help_text=_(
+            "Sets the length of the random string used for OpenID Connect nonce verification"
+        ),
+        default=32,
+    )
+    oidc_state_size = models.PositiveIntegerField(
+        _("State size"),
+        help_text=_(
+            "Sets the length of the random string used for OpenID Connect state verification"
+        ),
+        default=32,
+    )
+    oidc_exempt_urls = ArrayField(
+        verbose_name=_("URLs exempt from session renewal"),
+        base_field=models.CharField(_("Exempt URL"), max_length=1000),
+        default=list,
+        blank=True,
+        help_text=_(
+            "This is a list of absolute url paths, regular expressions for url paths, "
+            "or Django view names. This plus the mozilla-django-oidc urls are exempted "
+            "from the session renewal by the SessionRefresh middleware."
+        ),
+    )
+
+    @property
+    def oidc_rp_scopes(self) -> str:
+        """
+        Scopes should be formatted as a string with spaces
+        """
+        return " ".join(self.oidc_rp_scopes_list)
+
+    class Meta:
+        abstract = True
+
+    def __str__(self) -> str:
+        return force_text(self._meta.verbose_name)
+
+
+class OpenIDConnectConfig(CachingMixin, OpenIDConnectConfigBase):
+    """
+    Configuration for authentication/authorization via OpenID connect
+    """
+
     username_claim = models.CharField(
         _("username claim"),
         max_length=50,
         default="sub",
         help_text=_("The name of the OIDC claim that is used as the username"),
     )
     claim_mapping = JSONField(
@@ -155,17 +267,14 @@
             "Users will be flagged as being a staff user automatically. This allows users to login to the admin interface. By default they have no permissions, even if they are staff."
         ),
     )
 
     class Meta:
         verbose_name = _("OpenID Connect configuration")
 
-    def __str__(self):
-        return force_text(self._meta.verbose_name)
-
     def clean(self):
         super().clean()
 
         # validate claim mapping
         User = get_user_model()
         for field in self.claim_mapping.keys():
             try:
@@ -184,67 +293,13 @@
                 {
                     "claim_mapping": _(
                         "The username field may not be in the claim mapping"
                     ),
                 }
             )
 
-    @property
-    def oidc_rp_scopes(self):
+    @classproperty
+    def custom_oidc_db_prefix(cls) -> str:
         """
-        Scopes should be formatted as a string with spaces
+        Cache prefix that can be overridden
         """
-        return " ".join(self.oidc_rp_scopes_list)
-
-    @classmethod
-    def clear_cache(cls):
-        cache_name = getattr(
-            settings, "OIDC_CACHE", oidc_settings.MOZILLA_DJANGO_OIDC_DB_CACHE
-        )
-        if cache_name:
-            cache = get_cache(cache_name)
-            cache_key = cls.get_cache_key()
-            cache.delete(cache_key)
-
-    def set_to_cache(self):
-        cache_name = getattr(
-            settings,
-            "MOZILLA_DJANGO_OIDC_DB_CACHE",
-            oidc_settings.MOZILLA_DJANGO_OIDC_DB_CACHE,
-        )
-        if not cache_name:
-            return None
-        cache = get_cache(cache_name)
-        cache_key = self.get_cache_key()
-        timeout = getattr(
-            settings,
-            "MOZILLA_DJANGO_OIDC_DB_CACHE_TIMEOUT",
-            oidc_settings.MOZILLA_DJANGO_OIDC_DB_CACHE_TIMEOUT,
-        )
-        cache.set(cache_key, self, timeout)
-
-    @classmethod
-    def get_cache_key(cls):
-        prefix = getattr(
-            settings,
-            "MOZILLA_DJANGO_OIDC_DB_PREFIX",
-            oidc_settings.MOZILLA_DJANGO_OIDC_DB_PREFIX,
-        )
-        return "%s:%s" % (prefix, cls.__name__.lower())
-
-    @classmethod
-    def get_solo(cls):
-        cache_name = getattr(
-            settings,
-            "MOZILLA_DJANGO_OIDC_DB_CACHE",
-            oidc_settings.MOZILLA_DJANGO_OIDC_DB_CACHE,
-        )
-        if not cache_name:
-            obj, created = cls.objects.get_or_create(pk=cls.singleton_instance_id)
-            return obj
-        cache = get_cache(cache_name)
-        cache_key = cls.get_cache_key()
-        obj = cache.get(cache_key)
-        if not obj:
-            obj, created = cls.objects.get_or_create(pk=cls.singleton_instance_id)
-            obj.set_to_cache()
-        return obj
+        return oidc_settings.MOZILLA_DJANGO_OIDC_DB_PREFIX
```

### Comparing `mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db.egg-info/PKG-INFO` & `mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-django-oidc-db
-Version: 0.8.0
+Version: 0.9.0
 Summary: A database-backed configuration for mozilla-django-oidc
 Home-page: https://github.com/maykinmedia/mozilla-django-oidc-db
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Keywords: OIDC,django,database,authentication
 Platform: UNKNOWN
@@ -31,15 +31,15 @@
 .. mozilla_django_oidc_db documentation master file, created by startproject.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 Welcome to mozilla_django_oidc_db's documentation!
 ==================================================
 
-:Version: 0.8.0
+:Version: 0.9.0
 :Source: https://github.com/maykinmedia/mozilla-django-oidc-db
 :Keywords: OIDC, django, database, authentication
 :PythonVersion: 3.7
 
 |build-status| |coverage| |black|
 
 |python-versions| |django-versions| |pypi-version|
@@ -139,17 +139,30 @@
     ]
 
 Furthermore, ensure the following settings are configured:
 
 .. code-block:: python
 
     OIDC_AUTHENTICATE_CLASS = "mozilla_django_oidc_db.views.OIDCAuthenticationRequestView"
+    OIDC_CALLBACK_CLASS = "mozilla_django_oidc_db.views.OIDCCallbackView"
     MOZILLA_DJANGO_OIDC_DB_CACHE = "oidc"
     MOZILLA_DJANGO_OIDC_DB_CACHE_TIMEOUT = 1
 
+In order to properly catch admin login errors, add the following to urlpatterns:
+
+.. code-block:: python
+
+    from mozilla_django_oidc_db.views import AdminLoginFailure
+
+    urlpatterns = [
+        ...
+        path("admin/login/failure/", AdminLoginFailure.as_view(), name="admin-oidc-error"),
+        ...
+    ]
+
 ``MOZILLA_DJANGO_OIDC_DB_CACHE`` is used to cache the configuration that is stored in the database,
 to prevent a lot of database lookups. Ensure this cache is configured in ``CACHES`` (using the backend of choice):
 
 .. code-block:: python
 
     CACHES = {
         "default": {"BACKEND": "django.core.cache.backends.locmem.LocMemCache"},
@@ -229,14 +242,36 @@
 Custom username claim
 ---------------------
 
 The name of the claim that is used for the ``User.username`` property
 can be configured via the admin. By default, the username is derived from the ``sub`` claim that
 is returned by the OIDC provider.
 
+If the desired claim is nested in one or more objects, its path can be specified with dots, e.g.:
+
+.. code-block:: json
+
+    {
+        "some": {
+            "nested": {
+                "claim": "foo"
+            }
+        }
+    }
+
+Can be retrieved by setting the username claim to ``some.nested.claim``
+
+**NOTE**: the username claim does not support claims that have dots in their name, it cannot be configured to retrieve the following claim for instance:
+
+.. code-block:: json
+
+    {
+        "some.dotted.claim": "foo"
+    }
+
 .. |build-status| image:: https://github.com/maykinmedia/mozilla-django-oidc-db/workflows/Run%20CI/badge.svg?branch=master
     :target: https://github.com/maykinmedia/mozilla-django-oidc-db/actions?query=workflow%3A%22Run+CI%22+branch%3Amaster
 
 .. |coverage| image:: https://codecov.io/gh/maykinmedia/mozilla-django-oidc-db/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/maykinmedia/mozilla-django-oidc-db
     :alt: Coverage status
```

### Comparing `mozilla-django-oidc-db-0.8.0/mozilla_django_oidc_db.egg-info/SOURCES.txt` & `mozilla-django-oidc-db-0.9.0/mozilla_django_oidc_db.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,36 +4,44 @@
 README.rst
 setup.cfg
 setup.py
 mozilla_django_oidc_db/__init__.py
 mozilla_django_oidc_db/admin.py
 mozilla_django_oidc_db/apps.py
 mozilla_django_oidc_db/backends.py
+mozilla_django_oidc_db/compat.py
 mozilla_django_oidc_db/constants.py
 mozilla_django_oidc_db/forms.py
 mozilla_django_oidc_db/middleware.py
 mozilla_django_oidc_db/mixins.py
 mozilla_django_oidc_db/models.py
 mozilla_django_oidc_db/settings.py
+mozilla_django_oidc_db/utils.py
 mozilla_django_oidc_db/views.py
 mozilla_django_oidc_db.egg-info/PKG-INFO
 mozilla_django_oidc_db.egg-info/SOURCES.txt
 mozilla_django_oidc_db.egg-info/dependency_links.txt
 mozilla_django_oidc_db.egg-info/not-zip-safe
 mozilla_django_oidc_db.egg-info/requires.txt
 mozilla_django_oidc_db.egg-info/top_level.txt
 mozilla_django_oidc_db/migrations/0001_initial.py
 mozilla_django_oidc_db/migrations/0002_openidconnectconfig_oidc_op_discovery_endpoint.py
 mozilla_django_oidc_db/migrations/0003_auto_20210719_0803.py
 mozilla_django_oidc_db/migrations/0004_auto_20210812_1044.py
 mozilla_django_oidc_db/migrations/0005_openidconnectconfig_sync_groups_glob_pattern.py
 mozilla_django_oidc_db/migrations/0006_openidconnectconfig_unique_id_claim.py
+mozilla_django_oidc_db/migrations/0007_auto_20220307_1128.py
 mozilla_django_oidc_db/migrations/__init__.py
+mozilla_django_oidc_db/templates/admin/oidc_failure.html
 testapp/__init__.py
 testapp/settings.py
 testapp/urls.py
 tests/__init__.py
 tests/conftest.py
+tests/factories.py
 tests/test_admin_form.py
 tests/test_backend.py
 tests/test_middleware.py
-tests/test_settings.py
+tests/test_models.py
+tests/test_settings.py
+tests/test_utils.py
+tests/test_views.py
```

### Comparing `mozilla-django-oidc-db-0.8.0/setup.cfg` & `mozilla-django-oidc-db-0.9.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mozilla-django-oidc-db
-version = 0.8.0
+version = 0.9.0
 description = A database-backed configuration for mozilla-django-oidc
 long_description = file: README.rst
 url = https://github.com/maykinmedia/mozilla-django-oidc-db
 license = MIT
 author = Maykin Media
 author_email = support@maykinmedia.nl
 keywords = OIDC, django, database, authentication
@@ -26,15 +26,16 @@
 include_package_data = True
 packages = find:
 install_requires = 
 	django
 	psycopg2
 	django-better-admin-arrayfield
 	django-solo
-	mozilla-django-oidc >=1.0.0, <2.0.0
+	glom
+	mozilla-django-oidc >=1.0.0, <3.0
 tests_require = 
 	psycopg2
 	pytest
 	pytest-django
 	requests_mock
 	tox
 	isort
@@ -42,14 +43,15 @@
 
 [options.extras_require]
 tests = 
 	psycopg2
 	pytest
 	pytest-django
 	requests_mock
+	factory-boy
 	tox
 	isort
 	black
 pep8 = flake8
 coverage = pytest-cov
 docs = 
 	sphinx
```

### Comparing `mozilla-django-oidc-db-0.8.0/testapp/settings.py` & `mozilla-django-oidc-db-0.9.0/testapp/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
 
+from django.urls import reverse_lazy
+
 BASE_DIR = os.path.abspath(os.path.dirname(__file__))
 
 SECRET_KEY = "so-secret-i-cant-believe-you-are-looking-at-this"
 
 DATABASES = {
     "default": {
         "ENGINE": "django.db.backends.postgresql",
@@ -59,7 +61,11 @@
 
 ROOT_URLCONF = "testapp.urls"
 
 AUTHENTICATION_BACKENDS = [
     "django.contrib.auth.backends.ModelBackend",
     "mozilla_django_oidc_db.backends.OIDCAuthenticationBackend",
 ]
+
+MOZILLA_DJANGO_OIDC_DB_PREFIX = "default"
+OIDC_CALLBACK_CLASS = "mozilla_django_oidc_db.views.OIDCCallbackView"
+LOGIN_REDIRECT_URL = reverse_lazy("admin:index")
```

### Comparing `mozilla-django-oidc-db-0.8.0/tests/test_admin_form.py` & `mozilla-django-oidc-db-0.9.0/tests/test_admin_form.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,16 @@
         "oidc_rp_client_secret": "secret",
         "oidc_rp_sign_algo": "RS256",
         "oidc_op_discovery_endpoint": "http://discovery-endpoint.nl/",
         "claim_mapping": get_claim_mapping(),
         "groups_claim": "roles",
         "sync_groups_glob_pattern": "*",
         "username_claim": "sub",
+        "oidc_nonce_size": 32,
+        "oidc_state_size": 32,
     }
     form = OpenIDConnectConfigForm(data=form_data)
 
     configuration = {
         "authorization_endpoint": "http://provider.com/auth/realms/master/protocol/openid-connect/auth",
         "token_endpoint": "http://provider.com/auth/realms/master/protocol/openid-connect/token",
         "userinfo_endpoint": "http://provider.com/auth/realms/master/protocol/openid-connect/userinfo",
@@ -65,14 +67,16 @@
         "oidc_rp_client_secret": "secret",
         "oidc_rp_sign_algo": "RS256",
         "oidc_op_discovery_endpoint": "http://discovery-endpoint.nl/",
         "claim_mapping": get_claim_mapping(),
         "groups_claim": "roles",
         "sync_groups_glob_pattern": "*",
         "username_claim": "sub",
+        "oidc_nonce_size": 32,
+        "oidc_state_size": 32,
     }
 
     class ExtendedOpenIDConnectConfigForm(OpenIDConnectConfigForm):
         required_endpoints = OpenIDConnectConfigForm.required_endpoints
         # Define an extra field to derive from the configuration
         oidc_mapping = dict(
             **OpenIDConnectConfigForm.oidc_mapping,
@@ -110,14 +114,16 @@
         "oidc_rp_client_secret": "secret",
         "oidc_rp_sign_algo": "RS256",
         "oidc_op_discovery_endpoint": "http://discovery-endpoint.nl",
         "claim_mapping": get_claim_mapping(),
         "groups_claim": "roles",
         "sync_groups_glob_pattern": "*",
         "username_claim": "sub",
+        "oidc_nonce_size": 32,
+        "oidc_state_size": 32,
     }
     form = OpenIDConnectConfigForm(data=form_data)
 
     form.is_valid()
 
     assert form.errors == {
         "oidc_op_discovery_endpoint": [
@@ -133,14 +139,16 @@
         "oidc_rp_client_secret": "secret",
         "oidc_rp_sign_algo": "RS256",
         "oidc_op_discovery_endpoint": "http://discovery-endpoint.nl",
         "claim_mapping": get_claim_mapping(),
         "groups_claim": "roles",
         "sync_groups_glob_pattern": "*",
         "username_claim": "sub",
+        "oidc_nonce_size": 32,
+        "oidc_state_size": 32,
     }
     form = OpenIDConnectConfigForm(data=form_data)
 
     form.is_valid()
 
     assert form.errors == {
         "oidc_op_discovery_endpoint": [
@@ -154,14 +162,16 @@
         "oidc_rp_client_id": "clientid",
         "oidc_rp_client_secret": "secret",
         "oidc_rp_sign_algo": "RS256",
         "claim_mapping": get_claim_mapping(),
         "groups_claim": "roles",
         "sync_groups_glob_pattern": "*",
         "username_claim": "sub",
+        "oidc_nonce_size": 32,
+        "oidc_state_size": 32,
     }
     form = OpenIDConnectConfigForm(data=form_data)
 
     form.is_valid()
 
     assert form.errors == {
         "oidc_op_authorization_endpoint": [_("This field is required.")],
```

### Comparing `mozilla-django-oidc-db-0.8.0/tests/test_backend.py` & `mozilla-django-oidc-db-0.9.0/tests/test_backend.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,31 @@
 
     # Authentication with the backend should not return a result,
     # because OIDC is not enabled
     assert backend.authenticate(request) is None
 
 
 @patch("mozilla_django_oidc_db.models.OpenIDConnectConfig.get_solo")
+def test_backend_get_sensitive_claims(mock_get_solo):
+    mock_get_solo.return_value = OpenIDConnectConfig(enabled=True, username_claim="sub")
+
+    class CustomOIDCBackend(OIDCAuthenticationBackend):
+        sensitive_claim_names = ["sensitive_claim1", "sensitive_claim2"]
+
+    backend = CustomOIDCBackend()
+
+    # Only the sensitive claims + the identifier claim should be obfuscated
+    assert backend.get_sensitive_claims_names() == [
+        "sub",
+        "sensitive_claim1",
+        "sensitive_claim2",
+    ]
+
+
+@patch("mozilla_django_oidc_db.models.OpenIDConnectConfig.get_solo")
 def test_backend_get_user_instance_values(mock_get_solo):
     mock_get_solo.return_value = OpenIDConnectConfig(
         claim_mapping=OpenIDConnectConfig._meta.get_field("claim_mapping").get_default()
     )
 
     claims = {
         "sub": "123456",
@@ -43,14 +60,44 @@
     assert user_values == {
         "email": "admin@localhost",
         "first_name": "John",
         "last_name": "Doe",
     }
 
 
+@patch("mozilla_django_oidc_db.models.OpenIDConnectConfig.get_solo")
+def test_backend_get_user_instance_values_nested_claims(mock_get_solo):
+    mock_get_solo.return_value = OpenIDConnectConfig(
+        claim_mapping={
+            "email": "user_info.email",
+            "first_name": "user_info.given_name",
+            "last_name": "user_info.family_name",
+        }
+    )
+
+    claims = {
+        "sub": "123456",
+        "user_info": {
+            "email": "admin@localhost",
+            "given_name": "John",
+            "family_name": "Doe",
+        },
+    }
+
+    backend = OIDCAuthenticationBackend()
+
+    user_values = backend.get_user_instance_values(claims)
+
+    assert user_values == {
+        "email": "admin@localhost",
+        "first_name": "John",
+        "last_name": "Doe",
+    }
+
+
 @pytest.mark.django_db
 @patch("mozilla_django_oidc_db.models.OpenIDConnectConfig.get_solo")
 def test_backend_create_user(mock_get_solo):
     mock_get_solo.return_value = OpenIDConnectConfig(
         enabled=True,
         oidc_rp_client_id="testid",
         oidc_rp_client_secret="secret",
@@ -329,14 +376,52 @@
     # Verify that a user is created with the correct values
     assert user.username == "123456"
     assert list(user.groups.values_list("name", flat=True)) == ["groupadmin"]
 
 
 @pytest.mark.django_db
 @patch("mozilla_django_oidc_db.models.OpenIDConnectConfig.get_solo")
+def test_backend_create_user_sync_all_groups_nested_groups_claim(mock_get_solo):
+    mock_get_solo.return_value = OpenIDConnectConfig(
+        enabled=True,
+        oidc_rp_client_id="testid",
+        oidc_rp_client_secret="secret",
+        oidc_rp_sign_algo="HS256",
+        oidc_rp_scopes_list=["openid", "email"],
+        oidc_op_jwks_endpoint="http://some.endpoint/v1/jwks",
+        oidc_op_authorization_endpoint="http://some.endpoint/v1/auth",
+        oidc_op_token_endpoint="http://some.endpoint/v1/token",
+        oidc_op_user_endpoint="http://some.endpoint/v1/user",
+        groups_claim="nested_object.roles",
+        sync_groups=True,
+        sync_groups_glob_pattern="*",
+    )
+
+    claims = {
+        "sub": "123456",
+        "nested_object": {"roles": ["useradmin", "groupadmin"]},
+    }
+
+    backend = OIDCAuthenticationBackend()
+
+    user = backend.create_user(claims)
+
+    # Verify that the groups were created
+    assert Group.objects.count() == 2
+
+    # Verify that a user is created with the correct values
+    assert user.username == "123456"
+    assert list(user.groups.values_list("name", flat=True)) == [
+        "useradmin",
+        "groupadmin",
+    ]
+
+
+@pytest.mark.django_db
+@patch("mozilla_django_oidc_db.models.OpenIDConnectConfig.get_solo")
 def test_backend_create_user_with_profile_settings(mock_get_solo):
     Group.objects.all().delete()
 
     mock_get_solo.return_value = OpenIDConnectConfig(
         enabled=True,
         oidc_rp_client_id="testid",
         oidc_rp_client_secret="secret",
```

### Comparing `mozilla-django-oidc-db-0.8.0/tests/test_middleware.py` & `mozilla-django-oidc-db-0.9.0/tests/test_settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,77 +1,71 @@
 from unittest.mock import patch
-from urllib.parse import parse_qs, urlparse
-
-from django.contrib.sessions.middleware import SessionMiddleware
-from django.http.response import HttpResponseRedirect
-from django.test import RequestFactory
 
 import pytest
 
+from mozilla_django_oidc_db.backends import OIDCAuthenticationBackend
 from mozilla_django_oidc_db.middleware import SessionRefresh
 from mozilla_django_oidc_db.models import OpenIDConnectConfig
+from mozilla_django_oidc_db.views import OIDCAuthenticationRequestView
 
 
 @patch("mozilla_django_oidc_db.models.OpenIDConnectConfig.get_solo")
-def test_sessionrefresh_oidc_not_enabled(mock_get_solo):
+def test_backend_settings_derived_from_model_oidc_not_enabled(mock_get_solo):
     mock_get_solo.return_value = OpenIDConnectConfig(enabled=False)
 
-    request = RequestFactory().get("/")
+    backend = OIDCAuthenticationBackend()
 
-    # Running the middleware should return None, since OIDC is disabled
-    result = SessionRefresh(get_response=lambda: None).process_request(request)
+    # verify that the settings are not set in __init__
+    assert backend.OIDC_RP_CLIENT_ID is None
+    assert backend.OIDC_RP_CLIENT_SECRET is None
+    assert backend.OIDC_RP_SIGN_ALGO == "HS256"  # default from mozilla-django-oidc
+    assert backend.OIDC_OP_JWKS_ENDPOINT is None
+    assert backend.OIDC_OP_TOKEN_ENDPOINT is None
+    assert backend.OIDC_OP_USER_ENDPOINT is None
+    assert backend.OIDC_RP_IDP_SIGN_KEY is None
 
-    assert result is None
+
+@patch("mozilla_django_oidc_db.models.OpenIDConnectConfig.get_solo")
+def test_backend_settings_derived_from_model_oidc_enabled(mock_get_solo):
+    mock_get_solo.return_value = OpenIDConnectConfig(
+        enabled=True,
+        oidc_rp_client_id="testid",
+        oidc_rp_client_secret="secret",
+        oidc_rp_sign_algo="HS256",
+        oidc_rp_scopes_list=["openid", "email"],
+        oidc_op_jwks_endpoint="http://some.endpoint/v1/jwks",
+        oidc_op_authorization_endpoint="http://some.endpoint/v1/auth",
+        oidc_op_token_endpoint="http://some.endpoint/v1/token",
+        oidc_op_user_endpoint="http://some.endpoint/v1/user",
+    )
+
+    backend = OIDCAuthenticationBackend()
+
+    # verify that the settings are derived from OpenIDConnectConfig
+    assert backend.OIDC_RP_CLIENT_ID == "testid"
+    assert backend.OIDC_RP_CLIENT_SECRET == "secret"
+    assert backend.OIDC_RP_SIGN_ALGO == "HS256"
+    assert backend.OIDC_OP_JWKS_ENDPOINT == "http://some.endpoint/v1/jwks"
+    assert backend.OIDC_OP_TOKEN_ENDPOINT == "http://some.endpoint/v1/token"
+    assert backend.OIDC_OP_USER_ENDPOINT == "http://some.endpoint/v1/user"
+    assert backend.OIDC_RP_IDP_SIGN_KEY is None
 
 
 @patch("mozilla_django_oidc_db.models.OpenIDConnectConfig.get_solo")
-def test_sessionrefresh_config_always_refreshed(mock_get_solo):
-    """
-    Middleware should refresh the config on every call of `process_request`
-    """
+def test_view_settings_derived_from_model_oidc_enabled(mock_get_solo):
     mock_get_solo.return_value = OpenIDConnectConfig(
         enabled=True,
         oidc_rp_client_id="testid",
         oidc_rp_client_secret="secret",
         oidc_rp_sign_algo="HS256",
         oidc_rp_scopes_list=["openid", "email"],
         oidc_op_jwks_endpoint="http://some.endpoint/v1/jwks",
         oidc_op_authorization_endpoint="http://some.endpoint/v1/auth",
         oidc_op_token_endpoint="http://some.endpoint/v1/token",
         oidc_op_user_endpoint="http://some.endpoint/v1/user",
     )
 
-    middleware = SessionRefresh(get_response=lambda: None)
-    request = RequestFactory().get("/")
-    SessionMiddleware().process_request(request)
-
-    with patch(
-        "mozilla_django_oidc_db.middleware.SessionRefresh.is_refreshable_url",
-        return_value=True,
-    ):
-        with patch("mozilla_django_oidc.middleware.reverse", return_value="/callback"):
-            result1 = middleware.process_request(request)
-
-            # Update the config and call the middleware again (without reinstantiating)
-            mock_get_solo.return_value = OpenIDConnectConfig(
-                enabled=True,
-                oidc_rp_client_id="some-other-id",
-                oidc_rp_client_secret="secret",
-                oidc_rp_sign_algo="HS256",
-                oidc_rp_scopes_list=["openid", "email", "other_scope"],
-                oidc_op_jwks_endpoint="http://some.endpoint/v1/jwks",
-                oidc_op_authorization_endpoint="http://some.endpoint/v1/auth",
-                oidc_op_token_endpoint="http://some.endpoint/v1/token",
-                oidc_op_user_endpoint="http://some.endpoint/v1/user",
-            )
-            result2 = middleware.process_request(request)
-
-    assert isinstance(result1, HttpResponseRedirect)
-    assert isinstance(result2, HttpResponseRedirect)
-
-    parsed1 = parse_qs(urlparse(result1.url).query)
-    assert parsed1["client_id"] == ["testid"]
-    assert parsed1["scope"] == ["openid email"]
-
-    parsed2 = parse_qs(urlparse(result2.url).query)
-    assert parsed2["client_id"] == ["some-other-id"]
-    assert parsed2["scope"] == ["openid email other_scope"]
+    view = OIDCAuthenticationRequestView()
+
+    # verify that the settings are derived from OpenIDConnectConfig
+    assert view.OIDC_RP_CLIENT_ID == "testid"
+    assert view.OIDC_OP_AUTH_ENDPOINT == "http://some.endpoint/v1/auth"
```


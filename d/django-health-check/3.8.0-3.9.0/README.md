# Comparing `tmp/django-health-check-3.8.0.tar.gz` & `tmp/django-health-check-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-health-check-3.8.0.tar", last modified: Fri Oct 19 15:02:29 2018, max compression
+gzip compressed data, was "dist/django-health-check-3.9.0.tar", last modified: Mon Feb  4 08:08:17 2019, max compression
```

## Comparing `django-health-check-3.8.0.tar` & `django-health-check-3.9.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-10-19 15:02:29.000000 django-health-check-3.8.0/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-10-19 15:02:29.000000 django-health-check-3.8.0/django_health_check.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)    11472 2018-10-19 15:02:29.000000 django-health-check-3.8.0/django_health_check.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)     2059 2018-10-19 15:02:29.000000 django-health-check-3.8.0/django_health_check.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-10-19 15:02:29.000000 django-health-check-3.8.0/django_health_check.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-10-19 15:02:29.000000 django-health-check-3.8.0/django_health_check.egg-info/not-zip-safe
--rw-r--r--   0 travis    (2000) travis    (2000)       47 2018-10-19 15:02:29.000000 django-health-check-3.8.0/django_health_check.egg-info/pbr.json
--rw-r--r--   0 travis    (2000) travis    (2000)       13 2018-10-19 15:02:29.000000 django-health-check-3.8.0/django_health_check.egg-info/top_level.txt
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-10-19 15:02:29.000000 django-health-check-3.8.0/docs/
--rw-r--r--   0 travis    (2000) travis    (2000)      204 2018-10-19 15:01:27.000000 django-health-check-3.8.0/docs/changelog.rst
--rw-r--r--   0 travis    (2000) travis    (2000)      224 2018-10-19 15:01:27.000000 django-health-check-3.8.0/docs/conf.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1038 2018-10-19 15:01:27.000000 django-health-check-3.8.0/docs/contrib.rst
--rw-r--r--   0 travis    (2000) travis    (2000)      349 2018-10-19 15:01:27.000000 django-health-check-3.8.0/docs/index.rst
--rw-r--r--   0 travis    (2000) travis    (2000)       27 2018-10-19 15:01:27.000000 django-health-check-3.8.0/docs/readme.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     2147 2018-10-19 15:01:27.000000 django-health-check-3.8.0/docs/settings.rst
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-10-19 15:02:29.000000 django-health-check-3.8.0/health_check/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-10-19 15:02:29.000000 django-health-check-3.8.0/health_check/cache/
--rw-r--r--   0 travis    (2000) travis    (2000)       65 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/cache/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)      256 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/cache/apps.py
--rw-r--r--   0 travis    (2000) travis    (2000)      842 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/cache/backends.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-10-19 15:02:29.000000 django-health-check-3.8.0/health_check/contrib/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-10-19 15:02:29.000000 django-health-check-3.8.0/health_check/contrib/celery/
--rw-r--r--   0 travis    (2000) travis    (2000)       74 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/contrib/celery/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)      512 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/contrib/celery/apps.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1037 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/contrib/celery/backends.py
--rw-r--r--   0 travis    (2000) travis    (2000)       99 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/contrib/celery/tasks.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-10-19 15:02:29.000000 django-health-check-3.8.0/health_check/contrib/psutil/
--rw-r--r--   0 travis    (2000) travis    (2000)       74 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/contrib/psutil/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)      852 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/contrib/psutil/apps.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1576 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/contrib/psutil/backends.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-10-19 15:02:29.000000 django-health-check-3.8.0/health_check/contrib/rabbitmq/
--rw-r--r--   0 travis    (2000) travis    (2000)       76 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/contrib/rabbitmq/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)      282 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/contrib/rabbitmq/apps.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1539 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/contrib/rabbitmq/backends.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-10-19 15:02:29.000000 django-health-check-3.8.0/health_check/contrib/s3boto3_storage/
--rw-r--r--   0 travis    (2000) travis    (2000)       83 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/contrib/s3boto3_storage/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)      300 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/contrib/s3boto3_storage/apps.py
--rw-r--r--   0 travis    (2000) travis    (2000)      799 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/contrib/s3boto3_storage/backends.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-10-19 15:02:29.000000 django-health-check-3.8.0/health_check/contrib/s3boto_storage/
--rw-r--r--   0 travis    (2000) travis    (2000)       82 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/contrib/s3boto_storage/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)      297 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/contrib/s3boto_storage/apps.py
--rw-r--r--   0 travis    (2000) travis    (2000)      722 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/contrib/s3boto_storage/backends.py
--rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/contrib/__init__.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-10-19 15:02:29.000000 django-health-check-3.8.0/health_check/db/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-10-19 15:02:29.000000 django-health-check-3.8.0/health_check/db/migrations/
--rw-r--r--   0 travis    (2000) travis    (2000)      695 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/db/migrations/0001_initial.py
--rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/db/migrations/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)       62 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/db/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)      259 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/db/apps.py
--rw-r--r--   0 travis    (2000) travis    (2000)      652 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/db/backends.py
--rw-r--r--   0 travis    (2000) travis    (2000)      171 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/db/models.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-10-19 15:02:29.000000 django-health-check-3.8.0/health_check/storage/
--rw-r--r--   0 travis    (2000) travis    (2000)       67 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/storage/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)      292 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/storage/apps.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2601 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/storage/backends.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-10-19 15:02:29.000000 django-health-check-3.8.0/health_check/templates/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-10-19 15:02:29.000000 django-health-check-3.8.0/health_check/templates/health_check/
--rw-r--r--   0 travis    (2000) travis    (2000)     1100 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/templates/health_check/index.html
--rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1700 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/backends.py
--rw-r--r--   0 travis    (2000) travis    (2000)      228 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/conf.py
--rw-r--r--   0 travis    (2000) travis    (2000)      736 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/exceptions.py
--rw-r--r--   0 travis    (2000) travis    (2000)      623 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/plugins.py
--rw-r--r--   0 travis    (2000) travis    (2000)      155 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/urls.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1925 2018-10-19 15:01:27.000000 django-health-check-3.8.0/health_check/views.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-10-19 15:02:29.000000 django-health-check-3.8.0/tests/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-10-19 15:02:29.000000 django-health-check-3.8.0/tests/testapp/
--rw-r--r--   0 travis    (2000) travis    (2000)       43 2018-10-19 15:01:27.000000 django-health-check-3.8.0/tests/testapp/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)      118 2018-10-19 15:01:27.000000 django-health-check-3.8.0/tests/testapp/celery.py
--rwxr-xr-x   0 travis    (2000) travis    (2000)      242 2018-10-19 15:01:27.000000 django-health-check-3.8.0/tests/testapp/manage.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1173 2018-10-19 15:01:27.000000 django-health-check-3.8.0/tests/testapp/settings.py
--rw-r--r--   0 travis    (2000) travis    (2000)      109 2018-10-19 15:01:27.000000 django-health-check-3.8.0/tests/testapp/urls.py
--rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-10-19 15:01:27.000000 django-health-check-3.8.0/tests/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)      875 2018-10-19 15:01:27.000000 django-health-check-3.8.0/tests/test_autodiscover.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3006 2018-10-19 15:01:27.000000 django-health-check-3.8.0/tests/test_backends.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2774 2018-10-19 15:01:27.000000 django-health-check-3.8.0/tests/test_cache.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2300 2018-10-19 15:01:27.000000 django-health-check-3.8.0/tests/test_db.py
--rw-r--r--   0 travis    (2000) travis    (2000)      554 2018-10-19 15:01:27.000000 django-health-check-3.8.0/tests/test_plugins.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3038 2018-10-19 15:01:27.000000 django-health-check-3.8.0/tests/test_rabbitmq.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3506 2018-10-19 15:01:27.000000 django-health-check-3.8.0/tests/test_storage.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3061 2018-10-19 15:01:27.000000 django-health-check-3.8.0/tests/test_views.py
--rw-r--r--   0 travis    (2000) travis    (2000)      714 2018-10-19 15:01:27.000000 django-health-check-3.8.0/.editorconfig
--rw-r--r--   0 travis    (2000) travis    (2000)      825 2018-10-19 15:01:27.000000 django-health-check-3.8.0/.travis.yml
--rw-r--r--   0 travis    (2000) travis    (2000)     1085 2018-10-19 15:01:27.000000 django-health-check-3.8.0/LICENSE
--rw-r--r--   0 travis    (2000) travis    (2000)       49 2018-10-19 15:01:27.000000 django-health-check-3.8.0/MANIFEST.in
--rw-r--r--   0 travis    (2000) travis    (2000)     8518 2018-10-19 15:01:27.000000 django-health-check-3.8.0/README.rst
--rw-r--r--   0 travis    (2000) travis    (2000)       90 2018-10-19 15:01:27.000000 django-health-check-3.8.0/requirements-dev.txt
--rw-r--r--   0 travis    (2000) travis    (2000)     1435 2018-10-19 15:02:29.000000 django-health-check-3.8.0/setup.cfg
--rw-r--r--   0 travis    (2000) travis    (2000)      103 2018-10-19 15:01:27.000000 django-health-check-3.8.0/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)      822 2018-10-19 15:01:27.000000 django-health-check-3.8.0/tox.ini
--rw-r--r--   0 travis    (2000) travis    (2000)    11472 2018-10-19 15:02:29.000000 django-health-check-3.8.0/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-04 08:08:17.000000 django-health-check-3.9.0/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-04 08:08:17.000000 django-health-check-3.9.0/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2147 2019-02-04 08:07:50.000000 django-health-check-3.9.0/docs/settings.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      349 2019-02-04 08:07:50.000000 django-health-check-3.9.0/docs/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1038 2019-02-04 08:07:50.000000 django-health-check-3.9.0/docs/contrib.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       27 2019-02-04 08:07:50.000000 django-health-check-3.9.0/docs/readme.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      204 2019-02-04 08:07:50.000000 django-health-check-3.9.0/docs/changelog.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      224 2019-02-04 08:07:50.000000 django-health-check-3.9.0/docs/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8518 2019-02-04 08:07:50.000000 django-health-check-3.9.0/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      103 2019-02-04 08:07:50.000000 django-health-check-3.9.0/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1085 2019-02-04 08:07:50.000000 django-health-check-3.9.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      714 2019-02-04 08:07:50.000000 django-health-check-3.9.0/.editorconfig
+-rw-rw-r--   0 travis    (2000) travis    (2000)      822 2019-02-04 08:07:50.000000 django-health-check-3.9.0/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-04 08:08:17.000000 django-health-check-3.9.0/django_health_check.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       13 2019-02-04 08:08:17.000000 django-health-check-3.9.0/django_health_check.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-02-04 08:08:17.000000 django-health-check-3.9.0/django_health_check.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11472 2019-02-04 08:08:17.000000 django-health-check-3.9.0/django_health_check.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)       47 2019-02-04 08:08:17.000000 django-health-check-3.9.0/django_health_check.egg-info/pbr.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-02-04 08:08:17.000000 django-health-check-3.9.0/django_health_check.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2059 2019-02-04 08:08:17.000000 django-health-check-3.9.0/django_health_check.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1207 2019-02-04 08:07:50.000000 django-health-check-3.9.0/.travis.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1435 2019-02-04 08:08:17.000000 django-health-check-3.9.0/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-04 08:08:17.000000 django-health-check-3.9.0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3506 2019-02-04 08:07:50.000000 django-health-check-3.9.0/tests/test_storage.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3074 2019-02-04 08:07:50.000000 django-health-check-3.9.0/tests/test_views.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-04 08:07:50.000000 django-health-check-3.9.0/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3038 2019-02-04 08:07:50.000000 django-health-check-3.9.0/tests/test_rabbitmq.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3006 2019-02-04 08:07:50.000000 django-health-check-3.9.0/tests/test_backends.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-04 08:08:17.000000 django-health-check-3.9.0/tests/testapp/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1173 2019-02-04 08:07:50.000000 django-health-check-3.9.0/tests/testapp/settings.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      242 2019-02-04 08:07:50.000000 django-health-check-3.9.0/tests/testapp/manage.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       43 2019-02-04 08:07:50.000000 django-health-check-3.9.0/tests/testapp/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      109 2019-02-04 08:07:50.000000 django-health-check-3.9.0/tests/testapp/urls.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      118 2019-02-04 08:07:50.000000 django-health-check-3.9.0/tests/testapp/celery.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      554 2019-02-04 08:07:50.000000 django-health-check-3.9.0/tests/test_plugins.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      875 2019-02-04 08:07:50.000000 django-health-check-3.9.0/tests/test_autodiscover.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2300 2019-02-04 08:07:50.000000 django-health-check-3.9.0/tests/test_db.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2774 2019-02-04 08:07:50.000000 django-health-check-3.9.0/tests/test_cache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       49 2019-02-04 08:07:50.000000 django-health-check-3.9.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)       92 2019-02-04 08:07:50.000000 django-health-check-3.9.0/requirements-dev.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11472 2019-02-04 08:08:17.000000 django-health-check-3.9.0/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-04 08:08:17.000000 django-health-check-3.9.0/health_check/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      750 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1707 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/backends.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-04 08:08:17.000000 django-health-check-3.9.0/health_check/contrib/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-04 08:08:17.000000 django-health-check-3.9.0/health_check/contrib/s3boto3_storage/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      799 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/contrib/s3boto3_storage/backends.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       83 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/contrib/s3boto3_storage/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      300 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/contrib/s3boto3_storage/apps.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-04 08:08:17.000000 django-health-check-3.9.0/health_check/contrib/celery/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       99 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/contrib/celery/tasks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1037 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/contrib/celery/backends.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       74 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/contrib/celery/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      512 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/contrib/celery/apps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/contrib/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-04 08:08:17.000000 django-health-check-3.9.0/health_check/contrib/psutil/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1576 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/contrib/psutil/backends.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       74 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/contrib/psutil/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      852 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/contrib/psutil/apps.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-04 08:08:17.000000 django-health-check-3.9.0/health_check/contrib/rabbitmq/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1539 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/contrib/rabbitmq/backends.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       76 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/contrib/rabbitmq/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      282 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/contrib/rabbitmq/apps.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-04 08:08:17.000000 django-health-check-3.9.0/health_check/contrib/s3boto_storage/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      722 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/contrib/s3boto_storage/backends.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       82 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/contrib/s3boto_storage/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      297 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/contrib/s3boto_storage/apps.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-04 08:08:17.000000 django-health-check-3.9.0/health_check/db/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      652 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/db/backends.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       62 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/db/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      171 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/db/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      259 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/db/apps.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-04 08:08:17.000000 django-health-check-3.9.0/health_check/db/migrations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/db/migrations/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      695 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/db/migrations/0001_initial.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      182 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/urls.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-04 08:08:17.000000 django-health-check-3.9.0/health_check/storage/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2601 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/storage/backends.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/storage/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      292 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/storage/apps.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-04 08:08:17.000000 django-health-check-3.9.0/health_check/templates/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-04 08:08:17.000000 django-health-check-3.9.0/health_check/templates/health_check/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1100 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/templates/health_check/index.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      623 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/plugins.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1925 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/views.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-04 08:08:17.000000 django-health-check-3.9.0/health_check/cache/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      842 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/cache/backends.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       65 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/cache/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      256 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/cache/apps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      228 2019-02-04 08:07:50.000000 django-health-check-3.9.0/health_check/conf.py
```

### Comparing `django-health-check-3.8.0/django_health_check.egg-info/PKG-INFO` & `django-health-check-3.9.0/django_health_check.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-health-check
-Version: 3.8.0
+Version: 3.9.0
 Summary: Run checks on services like databases, queue servers, celery processes, etc.
 Home-page: https://github.com/KristianOellegaard/django-health-check
 Author: Kristian Ollegaard
 Author-email: kristian@oellegaard.com
 License: BSD License
 Description: ===================
         django-health-check
```

### Comparing `django-health-check-3.8.0/django_health_check.egg-info/SOURCES.txt` & `django-health-check-3.9.0/django_health_check.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/docs/contrib.rst` & `django-health-check-3.9.0/docs/contrib.rst`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/docs/settings.rst` & `django-health-check-3.9.0/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/health_check/cache/backends.py` & `django-health-check-3.9.0/health_check/cache/backends.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/health_check/contrib/celery/apps.py` & `django-health-check-3.9.0/health_check/contrib/celery/apps.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/health_check/contrib/celery/backends.py` & `django-health-check-3.9.0/health_check/contrib/celery/backends.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/health_check/contrib/psutil/apps.py` & `django-health-check-3.9.0/health_check/contrib/psutil/apps.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/health_check/contrib/psutil/backends.py` & `django-health-check-3.9.0/health_check/contrib/psutil/backends.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/health_check/contrib/rabbitmq/backends.py` & `django-health-check-3.9.0/health_check/contrib/rabbitmq/backends.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/health_check/contrib/s3boto3_storage/backends.py` & `django-health-check-3.9.0/health_check/contrib/s3boto3_storage/backends.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/health_check/contrib/s3boto_storage/backends.py` & `django-health-check-3.9.0/health_check/contrib/s3boto_storage/backends.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/health_check/db/migrations/0001_initial.py` & `django-health-check-3.9.0/health_check/db/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/health_check/db/backends.py` & `django-health-check-3.9.0/health_check/db/backends.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/health_check/storage/backends.py` & `django-health-check-3.9.0/health_check/storage/backends.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/health_check/templates/health_check/index.html` & `django-health-check-3.9.0/health_check/templates/health_check/index.html`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/health_check/backends.py` & `django-health-check-3.9.0/health_check/backends.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging
 from timeit import default_timer as timer
 
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import ugettext_lazy as _  # noqa: N812
 
 from health_check.exceptions import HealthCheckException
 
 logger = logging.getLogger('health-check')
 
 
 class BaseHealthCheckBackend:
     critical_service = True
     """
     Define if service is critical to the operation of the site.
 
-    If set to ``False`` service failures will cause a 500 response code on the
+    If set to ``True`` service failures return 500 response code on the
     health check endpoint.
     """
 
     def __init__(self):
         self.errors = []
 
     def check_status(self):
```

### Comparing `django-health-check-3.8.0/health_check/exceptions.py` & `django-health-check-3.9.0/health_check/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import ugettext_lazy as _  # noqa: N812
 
 
 class HealthCheckException(Exception):
     message_type = _("unknown error")
 
     def __init__(self, message):
         self.message = message
```

### Comparing `django-health-check-3.8.0/health_check/plugins.py` & `django-health-check-3.9.0/health_check/plugins.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/health_check/views.py` & `django-health-check-3.9.0/health_check/views.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/tests/testapp/settings.py` & `django-health-check-3.9.0/tests/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/tests/test_autodiscover.py` & `django-health-check-3.9.0/tests/test_autodiscover.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/tests/test_backends.py` & `django-health-check-3.9.0/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/tests/test_cache.py` & `django-health-check-3.9.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/tests/test_db.py` & `django-health-check-3.9.0/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/tests/test_plugins.py` & `django-health-check-3.9.0/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/tests/test_rabbitmq.py` & `django-health-check-3.9.0/tests/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/tests/test_storage.py` & `django-health-check-3.9.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/tests/test_views.py` & `django-health-check-3.9.0/tests/test_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 try:
     from django.urls import reverse
 except ImportError:
     from django.core.urlresolvers import reverse
 
 
 class TestMainView:
-    url = reverse('health_check_home')
+    url = reverse('health_check:health_check_home')
 
     def test_success(self, client):
         response = client.get(self.url)
         assert response.status_code == 200, response.content.decode('utf-8')
 
     def test_error(self, client):
         class MyBackend(BaseHealthCheckBackend):
```

### Comparing `django-health-check-3.8.0/.editorconfig` & `django-health-check-3.9.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/.travis.yml` & `django-health-check-3.9.0/.travis.yml`

 * *Files 24% similar despite different names*

```diff
@@ -22,17 +22,24 @@
     export TOXENV=py$(echo $TRAVIS_PYTHON_VERSION | sed -e 's/\.//g')-dj$DJANGO
   fi
 - echo $TOXENV
 script:
 - tox -e $TOXENV
 after_success:
 - codecov
-deploy:
-  provider: pypi
-  user: codingjoe
-  password:
-    secure: jJyadofJm7F1Qco+EDCyN/aMZaYSbfQ0GAE02Bx7I499MkjPYvv38X2btg+PjdW3rzGD0d/kq24lfWLkgKncyQ/YMgLQ7H/GuCCHHYbKUklxllaoFXActBjstmKOvXyWWC5oEb+YEJ4HTwgkvS6wkp69B7C1d4BAOqGs5IKnCSo=
-  on:
-    tags: true
-    distributions: sdist bdist_wheel
-    repo: KristianOellegaard/django-health-check
-    branch: master
+jobs:
+  include:
+    - stage: PyPI release  # will run after the default "test" stage succeeds
+      script: echo "Deploying to PyPI ..."  # override regular test script; "skip" should also work
+      env:
+        - TOXENV=qa  # if not set explicitly, build matrix vars will use their first value
+      if: tag IS present
+      deploy:
+        provider: pypi
+        user: codingjoe
+        password:
+          secure: jJyadofJm7F1Qco+EDCyN/aMZaYSbfQ0GAE02Bx7I499MkjPYvv38X2btg+PjdW3rzGD0d/kq24lfWLkgKncyQ/YMgLQ7H/GuCCHHYbKUklxllaoFXActBjstmKOvXyWWC5oEb+YEJ4HTwgkvS6wkp69B7C1d4BAOqGs5IKnCSo=
+        on:
+          tags: true
+          distributions: sdist bdist_wheel
+          repo: KristianOellegaard/django-health-check
+          branch: master
```

### Comparing `django-health-check-3.8.0/LICENSE` & `django-health-check-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/README.rst` & `django-health-check-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/setup.cfg` & `django-health-check-3.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/tox.ini` & `django-health-check-3.9.0/tox.ini`

 * *Files identical despite different names*

### Comparing `django-health-check-3.8.0/PKG-INFO` & `django-health-check-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-health-check
-Version: 3.8.0
+Version: 3.9.0
 Summary: Run checks on services like databases, queue servers, celery processes, etc.
 Home-page: https://github.com/KristianOellegaard/django-health-check
 Author: Kristian Ollegaard
 Author-email: kristian@oellegaard.com
 License: BSD License
 Description: ===================
         django-health-check
```


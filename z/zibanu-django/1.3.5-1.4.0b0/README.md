# Comparing `tmp/zibanu-django-1.3.5.tar.gz` & `tmp/zibanu_django-1.4.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zibanu-django-1.3.5.tar", last modified: Wed Apr  3 22:29:28 2024, max compression
+gzip compressed data, was "zibanu_django-1.4.0b0.tar", last modified: Fri May  3 11:31:01 2024, max compression
```

## Comparing `zibanu-django-1.3.5.tar` & `zibanu_django-1.4.0b0.tar`

### file list

```diff
@@ -1,102 +1,109 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.342325 zibanu-django-1.3.5/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-1.3.5/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      105 2023-08-07 23:22:31.000000 zibanu-django-1.3.5/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)    68384 2024-04-03 22:29:28.341325 zibanu-django-1.3.5/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    27020 2023-09-12 12:23:03.000000 zibanu-django-1.3.5/README.md
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      932 2024-04-03 22:28:23.000000 zibanu-django-1.3.5/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2024-04-03 22:29:28.342325 zibanu-django-1.3.5/setup.cfg
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.328325 zibanu-django-1.3.5/zibanu/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      618 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.329325 zibanu-django-1.3.5/zibanu/django/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      503 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.329325 zibanu-django-1.3.5/zibanu/django/api/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      312 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/api/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.329325 zibanu-django-1.3.5/zibanu/django/api/services/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      447 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/api/services/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1301 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/api/services/language.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1280 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/api/services/timezone.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1147 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.330325 zibanu-django-1.3.5/zibanu/django/db/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      503 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/db/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.330325 zibanu-django-1.3.5/zibanu/django/db/backends/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      500 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/db/backends/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.330325 zibanu-django-1.3.5/zibanu/django/db/backends/oracle/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      500 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/db/backends/oracle/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1572 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/db/backends/oracle/base.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.331325 zibanu-django-1.3.5/zibanu/django/db/models/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      761 2024-04-03 22:22:00.000000 zibanu-django-1.3.5/zibanu/django/db/models/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1120 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/db/models/dated_model.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1593 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/db/models/manager.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2082 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/db/models/model.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.331325 zibanu-django-1.3.5/zibanu/django/lib/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      536 2024-04-03 22:22:00.000000 zibanu-django-1.3.5/zibanu/django/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.332325 zibanu-django-1.3.5/zibanu/django/lib/classes/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      644 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/lib/classes/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     5879 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/lib/classes/code_generator.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1182 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/lib/classes/extended_json_encoder.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      731 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/lib/classes/model_name.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.326325 zibanu-django-1.3.5/zibanu/django/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.326325 zibanu-django-1.3.5/zibanu/django/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.332325 zibanu-django-1.3.5/zibanu/django/locale/es/LC_MESSAGES/
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2493 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 macercha  (1000) macercha  (1000)     4500 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.333325 zibanu-django-1.3.5/zibanu/django/rest_framework/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      503 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/rest_framework/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2197 2024-03-13 14:44:10.000000 zibanu-django-1.3.5/zibanu/django/rest_framework/decorators.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.334325 zibanu-django-1.3.5/zibanu/django/rest_framework/exceptions/
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1171 2024-03-15 01:58:14.000000 zibanu-django-1.3.5/zibanu/django/rest_framework/exceptions/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     3076 2024-03-15 01:58:14.000000 zibanu-django-1.3.5/zibanu/django/rest_framework/exceptions/api_exception.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      850 2024-03-11 22:02:32.000000 zibanu-django-1.3.5/zibanu/django/rest_framework/exceptions/multiple_login_error.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      957 2024-03-15 01:58:14.000000 zibanu-django-1.3.5/zibanu/django/rest_framework/exceptions/not_implemented_exception.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1058 2024-03-18 23:17:34.000000 zibanu-django-1.3.5/zibanu/django/rest_framework/exceptions/permission_denied.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.334325 zibanu-django-1.3.5/zibanu/django/rest_framework/fields/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      718 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/rest_framework/fields/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1343 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/rest_framework/fields/current_user_default.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     3394 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/rest_framework/fields/hybrid_image.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.335325 zibanu-django-1.3.5/zibanu/django/rest_framework/permissions/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      652 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/rest_framework/permissions/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1174 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/rest_framework/permissions/is_owner_or_read_only.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.335325 zibanu-django-1.3.5/zibanu/django/rest_framework/serializers/
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1649 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/rest_framework/serializers/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      646 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/rest_framework/serializers/fields.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      863 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/rest_framework/serializers/model_serializer.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1031 2024-03-19 00:59:35.000000 zibanu-django-1.3.5/zibanu/django/rest_framework/utils.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.336325 zibanu-django-1.3.5/zibanu/django/rest_framework/viewsets/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      779 2024-03-19 00:59:46.000000 zibanu-django-1.3.5/zibanu/django/rest_framework/viewsets/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)    15113 2024-03-22 18:43:56.000000 zibanu-django-1.3.5/zibanu/django/rest_framework/viewsets/model_viewset.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1737 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/rest_framework/viewsets/viewset.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.336325 zibanu-django-1.3.5/zibanu/django/template/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      501 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/template/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      825 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/template/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.337325 zibanu-django-1.3.5/zibanu/django/template/context_processors/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      619 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/template/context_processors/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1055 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/template/context_processors/full_static_uri.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      819 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/template/context_processors/site.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.327325 zibanu-django-1.3.5/zibanu/django/template/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.327325 zibanu-django-1.3.5/zibanu/django/template/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.337325 zibanu-django-1.3.5/zibanu/django/template/locale/es/LC_MESSAGES/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      709 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/template/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1083 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/template/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.338325 zibanu-django-1.3.5/zibanu/django/template/templatetags/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      501 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/template/templatetags/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2317 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/template/templatetags/static_uri.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      889 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/template/templatetags/string_concat.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2673 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/template/templatetags/subtotal_dict.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1549 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/template/templatetags/sum_dict.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      655 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/urls.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.340324 zibanu-django-1.3.5/zibanu/django/utils/
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1075 2024-03-12 21:02:22.000000 zibanu-django-1.3.5/zibanu/django/utils/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1986 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/utils/date_time.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1168 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/utils/error_messages.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1493 2024-03-12 21:02:08.000000 zibanu-django-1.3.5/zibanu/django/utils/generic_utils.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     7608 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/utils/mail.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2423 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/utils/model_utils.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1263 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/utils/receivers_utils.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1511 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/utils/request_utils.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1559 2024-03-11 02:33:38.000000 zibanu-django-1.3.5/zibanu/django/utils/user_utils.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-03 22:29:28.341325 zibanu-django-1.3.5/zibanu_django.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    68384 2024-04-03 22:29:28.000000 zibanu-django-1.3.5/zibanu_django.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2984 2024-04-03 22:29:28.000000 zibanu-django-1.3.5/zibanu_django.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2024-04-03 22:29:28.000000 zibanu-django-1.3.5/zibanu_django.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       91 2024-04-03 22:29:28.000000 zibanu-django-1.3.5/zibanu_django.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2024-04-03 22:29:28.000000 zibanu-django-1.3.5/zibanu_django.egg-info/top_level.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.395956 zibanu_django-1.4.0b0/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu_django-1.4.0b0/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      105 2023-08-07 23:22:31.000000 zibanu_django-1.4.0b0/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    68386 2024-05-03 11:31:01.394956 zibanu_django-1.4.0b0/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    27020 2023-09-12 12:23:03.000000 zibanu_django-1.4.0b0/README.md
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1009 2024-05-03 10:34:00.000000 zibanu_django-1.4.0b0/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2024-05-03 11:31:01.395956 zibanu_django-1.4.0b0/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.379957 zibanu_django-1.4.0b0/zibanu/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      618 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.380957 zibanu_django-1.4.0b0/zibanu/django/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      583 2024-05-03 11:17:35.000000 zibanu_django-1.4.0b0/zibanu/django/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.380957 zibanu_django-1.4.0b0/zibanu/django/api/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      312 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/api/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.381956 zibanu_django-1.4.0b0/zibanu/django/api/services/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      512 2024-04-04 21:09:36.000000 zibanu_django-1.4.0b0/zibanu/django/api/services/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1040 2024-04-04 21:51:55.000000 zibanu_django-1.4.0b0/zibanu/django/api/services/dial_codes.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1301 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/api/services/language.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1280 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/api/services/timezone.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1147 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.381956 zibanu_django-1.4.0b0/zibanu/django/db/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      503 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/db/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.381956 zibanu_django-1.4.0b0/zibanu/django/db/backends/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      500 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/db/backends/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.382956 zibanu_django-1.4.0b0/zibanu/django/db/backends/oracle/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      500 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/db/backends/oracle/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1572 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/db/backends/oracle/base.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.383957 zibanu_django-1.4.0b0/zibanu/django/db/models/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      799 2024-04-03 22:31:00.000000 zibanu_django-1.4.0b0/zibanu/django/db/models/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1120 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/db/models/dated_model.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.383957 zibanu_django-1.4.0b0/zibanu/django/db/models/fields/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      372 2024-04-03 22:31:00.000000 zibanu_django-1.4.0b0/zibanu/django/db/models/fields/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2261 2024-04-04 21:09:36.000000 zibanu_django-1.4.0b0/zibanu/django/db/models/fields/phone_field.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1580 2024-05-03 11:24:21.000000 zibanu_django-1.4.0b0/zibanu/django/db/models/manager.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2082 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/db/models/model.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.383957 zibanu_django-1.4.0b0/zibanu/django/lib/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      556 2024-04-03 22:31:00.000000 zibanu_django-1.4.0b0/zibanu/django/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.384956 zibanu_django-1.4.0b0/zibanu/django/lib/classes/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      644 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/lib/classes/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     5879 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/lib/classes/code_generator.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1182 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/lib/classes/extended_json_encoder.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      731 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/lib/classes/model_name.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.385956 zibanu_django-1.4.0b0/zibanu/django/lib/enums/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      521 2024-04-04 21:09:36.000000 zibanu_django-1.4.0b0/zibanu/django/lib/enums/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1943 2024-04-04 22:29:20.000000 zibanu_django-1.4.0b0/zibanu/django/lib/enums/dial_codes.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.377956 zibanu_django-1.4.0b0/zibanu/django/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.377956 zibanu_django-1.4.0b0/zibanu/django/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.385956 zibanu_django-1.4.0b0/zibanu/django/locale/es/LC_MESSAGES/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     3239 2024-05-03 11:26:43.000000 zibanu_django-1.4.0b0/zibanu/django/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     7517 2024-05-03 11:26:33.000000 zibanu_django-1.4.0b0/zibanu/django/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.386956 zibanu_django-1.4.0b0/zibanu/django/rest_framework/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      503 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2197 2024-03-13 14:44:10.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/decorators.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.386956 zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1171 2024-03-15 01:58:14.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     3076 2024-03-15 01:58:14.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/api_exception.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      850 2024-03-11 22:02:32.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/multiple_login_error.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      957 2024-03-15 01:58:14.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/not_implemented_exception.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1058 2024-03-18 23:17:34.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/permission_denied.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.387956 zibanu_django-1.4.0b0/zibanu/django/rest_framework/fields/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      718 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/fields/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1343 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/fields/current_user_default.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     5815 2024-04-05 11:24:32.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/fields/hybrid_image.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.387956 zibanu_django-1.4.0b0/zibanu/django/rest_framework/permissions/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      652 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/permissions/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1174 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/permissions/is_owner_or_read_only.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.388956 zibanu_django-1.4.0b0/zibanu/django/rest_framework/serializers/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1649 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/serializers/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      646 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/serializers/fields.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      863 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/serializers/model_serializer.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1031 2024-03-19 00:59:35.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/utils.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.389956 zibanu_django-1.4.0b0/zibanu/django/rest_framework/viewsets/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      779 2024-03-19 00:59:46.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/viewsets/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    15232 2024-05-03 10:58:52.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/viewsets/model_viewset.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1737 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/viewsets/viewset.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.389956 zibanu_django-1.4.0b0/zibanu/django/template/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      501 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      825 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.390956 zibanu_django-1.4.0b0/zibanu/django/template/context_processors/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      619 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/context_processors/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1055 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/context_processors/full_static_uri.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      819 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/context_processors/site.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.378957 zibanu_django-1.4.0b0/zibanu/django/template/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.378957 zibanu_django-1.4.0b0/zibanu/django/template/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.390956 zibanu_django-1.4.0b0/zibanu/django/template/locale/es/LC_MESSAGES/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      709 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1083 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.391956 zibanu_django-1.4.0b0/zibanu/django/template/templatetags/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      501 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/templatetags/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2317 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/templatetags/static_uri.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      889 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/templatetags/string_concat.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2673 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/templatetags/subtotal_dict.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1549 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/templatetags/sum_dict.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      809 2024-04-04 21:09:36.000000 zibanu_django-1.4.0b0/zibanu/django/urls.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.393956 zibanu_django-1.4.0b0/zibanu/django/utils/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1075 2024-03-12 21:02:22.000000 zibanu_django-1.4.0b0/zibanu/django/utils/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1986 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/utils/date_time.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1168 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/utils/error_messages.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1770 2024-05-03 10:58:52.000000 zibanu_django-1.4.0b0/zibanu/django/utils/generic_utils.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     7608 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/utils/mail.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2423 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/utils/model_utils.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1263 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/utils/receivers_utils.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1511 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/utils/request_utils.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1559 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/utils/user_utils.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.394956 zibanu_django-1.4.0b0/zibanu_django.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    68386 2024-05-03 11:31:01.000000 zibanu_django-1.4.0b0/zibanu_django.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     3188 2024-05-03 11:31:01.000000 zibanu_django-1.4.0b0/zibanu_django.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2024-05-03 11:31:01.000000 zibanu_django-1.4.0b0/zibanu_django.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       91 2024-05-03 11:31:01.000000 zibanu_django-1.4.0b0/zibanu_django.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2024-05-03 11:31:01.000000 zibanu_django-1.4.0b0/zibanu_django.egg-info/top_level.txt
```

### Comparing `zibanu-django-1.3.5/LICENSE` & `zibanu_django-1.4.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/PKG-INFO` & `zibanu_django-1.4.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibanu-django
-Version: 1.3.5
+Version: 1.4.0b0
 Summary: Zibanu library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `zibanu-django-1.3.5/README.md` & `zibanu_django-1.4.0b0/README.md`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/pyproject.toml` & `zibanu_django-1.4.0b0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zibanu-django"
-version = "1.3.5"
+dynamic = ["version"]
 authors = [
     { name = "Mario Cerón", email = "mario.ceron@cqinversiones.co" }
 ]
 description = "Zibanu library for django projects"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
@@ -33,8 +33,11 @@
     "drf-extra-fields>=3.7"
 ]
 keywords = [
     "django",
     "zibanu",
     "library",
     "auth"
-]
+]
+
+[tool.setuptools.dynamic]
+version = {attr= "zibanu.django.__version__"}
```

### Comparing `zibanu-django-1.3.5/zibanu/__init__.py` & `zibanu_django-1.4.0b0/zibanu/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/api/services/language.py` & `zibanu_django-1.4.0b0/zibanu/django/api/services/language.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/api/services/timezone.py` & `zibanu_django-1.4.0b0/zibanu/django/api/services/timezone.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/apps.py` & `zibanu_django-1.4.0b0/zibanu/django/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/db/backends/oracle/base.py` & `zibanu_django-1.4.0b0/zibanu/django/db/backends/oracle/base.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/db/models/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/db/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 # Developed by: macercha
 # Date:         13/12/22 10:14 AM
 # Project:      Zibanu Django Project
 # Module Name:  __init__.py
 # Description:
 # ****************************************************************
 from django.db.models import *
+from .dated_model import DatedModel
+from .fields import *
 from .manager import Manager
 from .model import Model
-from .dated_model import DatedModel
 from django.db.models import __all__ as models_all
 
 __all__ = models_all
 
 __all__ += [
     "DatedModel",
     "Manager",
-    "Model"
+    "Model",
+    "PhoneField"
 ]
-
-
```

### Comparing `zibanu-django-1.3.5/zibanu/django/db/models/dated_model.py` & `zibanu_django-1.4.0b0/zibanu/django/db/models/dated_model.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/db/models/manager.py` & `zibanu_django-1.4.0b0/zibanu/django/db/models/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,9 +45,9 @@
         Returns
         -------
         qs: Queryset object
         """
         # Validate if pk key exists
         qs = self.get_queryset().filter(pk=pk)
         if len(qs) == 0:
-            raise self.model.DoesNotExist(_("OASIS Error. The object does not exists."))
+            raise self.model.DoesNotExist(_("The object does not exists."))
         return qs
```

### Comparing `zibanu-django-1.3.5/zibanu/django/db/models/model.py` & `zibanu_django-1.4.0b0/zibanu/django/db/models/model.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/lib/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/lib/classes/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,8 +8,10 @@
 # Developed by: macercha
 # Date:         30/01/24 08:57
 # Project:      Zibanu - Django
 # Module Name:  __init__.py
 # Description:
 # ****************************************************************
 # Default imports
-from .classes import *
+from .code_generator import CodeGenerator
+from .extended_json_encoder import ExtendedJSONEncoder
+from .model_name import ModelName
```

### Comparing `zibanu-django-1.3.5/zibanu/django/lib/classes/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/multiple_login_error.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # -*- coding: utf-8 -*-
 
-#  Developed by CQ Inversiones SAS. Copyright ©. 2019 - 2024. All rights reserved.
-#  Desarrollado por CQ Inversiones SAS. Copyright ©. 2019 - 2024. Todos los derechos reservado
+#  Developed by CQ Inversiones SAS. Copyright ©. 2019 - 2023. All rights reserved.
+#  Desarrollado por CQ Inversiones SAS. Copyright ©. 2019 - 2023. Todos los derechos reservado
 
 # ****************************************************************
 # IDE:          PyCharm
 # Developed by: macercha
-# Date:         30/01/24 08:57
+# Date:         8/11/23 06:13
 # Project:      Zibanu - Django
-# Module Name:  __init__.py
+# Module Name:  validation_error
 # Description:
 # ****************************************************************
 # Default imports
-from .code_generator import CodeGenerator
-from .extended_json_encoder import ExtendedJSONEncoder
-from .model_name import ModelName
+from .api_exception import APIException
+from rest_framework import status
+
+
+class MultipleLoginError(APIException):
+    """
+    Override class for ValidationError
+    """
+    def __init__(self, detail: str = None):
+        super().__init__(detail=detail, status_code=status.HTTP_412_PRECONDITION_FAILED, code="multiple_login_error")
```

### Comparing `zibanu-django-1.3.5/zibanu/django/lib/classes/code_generator.py` & `zibanu_django-1.4.0b0/zibanu/django/lib/classes/code_generator.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/lib/classes/extended_json_encoder.py` & `zibanu_django-1.4.0b0/zibanu/django/lib/classes/extended_json_encoder.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/lib/classes/model_name.py` & `zibanu_django-1.4.0b0/zibanu/django/lib/classes/model_name.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/locale/es/LC_MESSAGES/django.mo` & `zibanu_django-1.4.0b0/zibanu/django/locale/es/LC_MESSAGES/django.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,14 +7,29 @@
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
+msgid "'dial_code' and 'phone_number' keys are required."
+msgstr "'codig pais' y 'número telefónico' son claves requeridas."
+
+msgid "A Phone Field object"
+msgstr "Campo tipo teléfono"
+
+msgid "API Exception"
+msgstr "Excepción tipo API"
+
+msgid "Could not load import serializer class: "
+msgstr "No se puede importar la clase serializadora: "
+
+msgid "Country code is not valid. Please try again."
+msgstr "El código de país no es válido. Por favor inténtelo nuevamente."
+
 msgid "Created at"
 msgstr "Creado el"
 
 msgid "Data required at request not found."
 msgstr "El dato requerido no existe."
 
 msgid "Data required not found."
@@ -49,19 +64,24 @@
 
 msgid "Error! There is not record matching."
 msgstr "Error! No existen registros que coincidan."
 
 msgid "Generic error."
 msgstr "Error genérico."
 
+msgid "Invalid Token"
+msgstr "Token inválido"
+
 msgid "Modified at"
 msgstr "Modificado el"
 
-msgid "OASIS Error. The object does not exists."
-msgstr "El objeto no existe."
+msgid "Number of keys major than required. Please try again."
+msgstr ""
+"El número de claves es mayor que las requeridas. Por favor inténtelo de "
+"nuevo."
 
 msgid "Object does not exists."
 msgstr "El objeto no existe."
 
 msgid "Object has not been created."
 msgstr "El objeto no ha sido creado."
 
@@ -73,12 +93,16 @@
 
 msgid "The generated values are invalid."
 msgstr "El valor generado es inválido."
 
 msgid "The width or height of the file is invalid."
 msgstr "El ancho o alto del archivo es inválido."
 
+msgid "Type of field keys are wrong. Please try again."
+msgstr ""
+"El tipo de claves de campo son erradas. Por favor inténtelo nuevamente."
+
 msgid "You are not authorized for this resource."
 msgstr "No está autorizado para utilizar este recurso."
 
 msgid "You do not have permission to perform this action."
 msgstr "No posee permisos para ejecutar esta acción."
```

### Comparing `zibanu-django-1.3.5/zibanu/django/rest_framework/decorators.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/decorators.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/rest_framework/exceptions/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/rest_framework/exceptions/api_exception.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/rest_framework/exceptions/multiple_login_error.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/not_implemented_exception.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 
 #  Developed by CQ Inversiones SAS. Copyright ©. 2019 - 2023. All rights reserved.
 #  Desarrollado por CQ Inversiones SAS. Copyright ©. 2019 - 2023. Todos los derechos reservado
 
 # ****************************************************************
 # IDE:          PyCharm
 # Developed by: macercha
-# Date:         8/11/23 06:13
+# Date:         8/11/23 22:19
 # Project:      Zibanu - Django
-# Module Name:  validation_error
+# Module Name:  service_not_implemented
 # Description:
 # ****************************************************************
 # Default imports
+import logging
+import traceback
+from django.utils.translation import gettext_lazy as _
 from .api_exception import APIException
 from rest_framework import status
 
 
-class MultipleLoginError(APIException):
+class NotImplementedException(APIException):
     """
-    Override class for ValidationError
+    Class to raise error for not implemented method
     """
-    def __init__(self, detail: str = None):
-        super().__init__(detail=detail, status_code=status.HTTP_412_PRECONDITION_FAILED, code="multiple_login_error")
+    def __init__(self):
+        super().__init__(detail=_("Service not implemented"), code="not_implemented", status_code=status.HTTP_405_METHOD_NOT_ALLOWED)
```

### Comparing `zibanu-django-1.3.5/zibanu/django/rest_framework/exceptions/permission_denied.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/permission_denied.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/rest_framework/fields/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/rest_framework/fields/current_user_default.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/fields/current_user_default.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/rest_framework/permissions/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/rest_framework/permissions/is_owner_or_read_only.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/permissions/is_owner_or_read_only.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/rest_framework/serializers/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/rest_framework/serializers/fields.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/rest_framework/serializers/model_serializer.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/serializers/model_serializer.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/rest_framework/utils.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/utils.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/rest_framework/viewsets/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/viewsets/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/rest_framework/viewsets/model_viewset.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/viewsets/model_viewset.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,36 +243,39 @@
         -------
         response: Response object with status 201 if successfully and record created from model object.
         """
         try:
             data_return = []
             status_return = status.HTTP_400_BAD_REQUEST
             request_data = request.data
+            context = kwargs.get("context", {})
+            context["request"] = request
+
             if len(request_data) > 0:
-                serializer = self.get_serializer(data=request_data)
+                serializer = self.get_serializer(data=request_data, context=context)
                 if serializer.is_valid(raise_exception=True):
                     created_record = serializer.create(validated_data=serializer.validated_data)
                     if created_record is not None:
                         data_return = self.get_serializer(created_record).data
                         status_return = status.HTTP_201_CREATED
                     else:
                         raise ValidationError(ErrorMessages.CREATE_ERROR, "create_object")
             else:
-                raise APIException(ErrorMessages.DATA_REQUIRED, "data_required")
+                raise ValidationError(ErrorMessages.DATA_REQUIRED, "data_required")
         except DatabaseError as exc:
             raise APIException(detail=str(exc), code="database_error",
                                status_code=status.HTTP_500_INTERNAL_SERVER_ERROR) from exc
         except ValidationError as exc:
             raise APIException(detail=exc.detail, status_code=status.HTTP_406_NOT_ACCEPTABLE) from exc
         except CoreValidationError as exc:
             raise APIException(detail=exc.messages, status_code=status.HTTP_406_NOT_ACCEPTABLE) from exc
         except APIException:
             raise
         except Exception as exc:
-            raise APIException(detail=str(exc), status_code=status.HTTP_500_INTERNAL_SERVER_ERROR)
+            raise APIException(detail=str(exc), status_code=status.HTTP_500_INTERNAL_SERVER_ERROR) from exc
         else:
             return Response(status=status_return, data=data_return)
 
     def create(self, request, *args, **kwargs):
         """
         Overridden class method to disallow access
```

### Comparing `zibanu-django-1.3.5/zibanu/django/rest_framework/viewsets/viewset.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/viewsets/viewset.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/template/apps.py` & `zibanu_django-1.4.0b0/zibanu/django/template/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/template/context_processors/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/template/context_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/template/context_processors/full_static_uri.py` & `zibanu_django-1.4.0b0/zibanu/django/template/context_processors/full_static_uri.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/template/context_processors/site.py` & `zibanu_django-1.4.0b0/zibanu/django/template/context_processors/site.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/template/locale/es/LC_MESSAGES/django.mo` & `zibanu_django-1.4.0b0/zibanu/django/template/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/template/locale/es/LC_MESSAGES/django.po` & `zibanu_django-1.4.0b0/zibanu/django/template/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/template/templatetags/static_uri.py` & `zibanu_django-1.4.0b0/zibanu/django/template/templatetags/static_uri.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/template/templatetags/string_concat.py` & `zibanu_django-1.4.0b0/zibanu/django/template/templatetags/string_concat.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/template/templatetags/subtotal_dict.py` & `zibanu_django-1.4.0b0/zibanu/django/template/templatetags/subtotal_dict.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/template/templatetags/sum_dict.py` & `zibanu_django-1.4.0b0/zibanu/django/template/templatetags/sum_dict.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/urls.py` & `zibanu_django-1.4.0b0/zibanu/django/urls.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 # Developed by: macercha
 # Date:         7/07/23 7:44
 # Project:      Zibanu - Django
 # Module Name:  urls
 # Description:
 # ****************************************************************
 from django.urls import path
+from zibanu.django.api.services import DialCodesViewSet
 from zibanu.django.api.services import LanguageViewSet
 from zibanu.django.api.services import TimeZoneViewSet
 
 urlpatterns = [
+    path("dial_codes/list/", DialCodesViewSet.as_view({"post": "list"}), name="Dial codes list"),
     path("timezone/list/", TimeZoneViewSet.as_view({"post": "list"}), name="TimeZone list"),
     path("language/list/", LanguageViewSet.as_view({"post": "list"}), name="Django languages list")
 ]
```

### Comparing `zibanu-django-1.3.5/zibanu/django/utils/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/utils/date_time.py` & `zibanu_django-1.4.0b0/zibanu/django/utils/date_time.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/utils/error_messages.py` & `zibanu_django-1.4.0b0/zibanu/django/utils/error_messages.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/utils/generic_utils.py` & `zibanu_django-1.4.0b0/zibanu/django/utils/generic_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,28 +9,33 @@
 # Date:         28/02/24 15:27
 # Project:      Zibanu - Django
 # Module Name:  object_to_list
 # Description:
 # ****************************************************************
 # Default imports
 from typing import Any
+from django.utils.translation import gettext_lazy as _
 from django.utils.module_loading import import_string
 
 
 def object_to_list(obj: Any) -> list:
     l_return = []
     if isinstance(obj, str):
         l_return.append(obj)
     elif isinstance(obj, dict):
         for key, value in obj.items():
             if isinstance(value, dict):
                 l_return = l_return + object_to_list(value)
             elif isinstance(value, list):
                 for value_detail in value:
-                    l_return.append(key + ": " + str(value_detail))
+                    if len(value_detail) > 0:
+                        if isinstance(value_detail, dict):
+                            l_return = l_return + object_to_list(value_detail)
+                        else:
+                            l_return.append(key + ": " + str(value_detail))
             elif isinstance(value, str):
                 l_return.append(key + ": " + value)
     elif isinstance(obj, list):
         l_return = obj.copy()
     else:
         l_return.append(str(obj))
```

### Comparing `zibanu-django-1.3.5/zibanu/django/utils/mail.py` & `zibanu_django-1.4.0b0/zibanu/django/utils/mail.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/utils/model_utils.py` & `zibanu_django-1.4.0b0/zibanu/django/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/utils/receivers_utils.py` & `zibanu_django-1.4.0b0/zibanu/django/utils/receivers_utils.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/utils/request_utils.py` & `zibanu_django-1.4.0b0/zibanu/django/utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu/django/utils/user_utils.py` & `zibanu_django-1.4.0b0/zibanu/django/utils/user_utils.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.5/zibanu_django.egg-info/PKG-INFO` & `zibanu_django-1.4.0b0/zibanu_django.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibanu-django
-Version: 1.3.5
+Version: 1.4.0b0
 Summary: Zibanu library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `zibanu-django-1.3.5/zibanu_django.egg-info/SOURCES.txt` & `zibanu_django-1.4.0b0/zibanu_django.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,34 @@
 pyproject.toml
 zibanu/__init__.py
 zibanu/django/__init__.py
 zibanu/django/apps.py
 zibanu/django/urls.py
 zibanu/django/api/__init__.py
 zibanu/django/api/services/__init__.py
+zibanu/django/api/services/dial_codes.py
 zibanu/django/api/services/language.py
 zibanu/django/api/services/timezone.py
 zibanu/django/db/__init__.py
 zibanu/django/db/backends/__init__.py
 zibanu/django/db/backends/oracle/__init__.py
 zibanu/django/db/backends/oracle/base.py
 zibanu/django/db/models/__init__.py
 zibanu/django/db/models/dated_model.py
 zibanu/django/db/models/manager.py
 zibanu/django/db/models/model.py
+zibanu/django/db/models/fields/__init__.py
+zibanu/django/db/models/fields/phone_field.py
 zibanu/django/lib/__init__.py
 zibanu/django/lib/classes/__init__.py
 zibanu/django/lib/classes/code_generator.py
 zibanu/django/lib/classes/extended_json_encoder.py
 zibanu/django/lib/classes/model_name.py
+zibanu/django/lib/enums/__init__.py
+zibanu/django/lib/enums/dial_codes.py
 zibanu/django/locale/es/LC_MESSAGES/django.mo
 zibanu/django/locale/es/LC_MESSAGES/django.po
 zibanu/django/rest_framework/__init__.py
 zibanu/django/rest_framework/decorators.py
 zibanu/django/rest_framework/utils.py
 zibanu/django/rest_framework/exceptions/__init__.py
 zibanu/django/rest_framework/exceptions/api_exception.py
```


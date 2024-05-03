# Comparing `tmp/lino-cms-23.10.0.tar.gz` & `tmp/lino-cms-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino-cms-23.10.0.tar", last modified: Sat Oct  7 15:16:38 2023, max compression
+gzip compressed data, was "lino-cms-24.5.0.tar", last modified: Fri May  3 13:31:06 2024, max compression
```

## Comparing `lino-cms-23.10.0.tar` & `lino-cms-24.5.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-10-07 15:16:38.582676 lino-cms-23.10.0/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2022-09-11 01:24:12.000000 lino-cms-23.10.0/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)       69 2022-09-11 01:24:12.000000 lino-cms-23.10.0/MANIFEST.in
--rw-rw-r--   0 luc       (1000) www-data    (33)     1443 2023-10-07 15:16:38.582676 lino-cms-23.10.0/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)      657 2022-09-20 14:16:08.000000 lino-cms-23.10.0/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-10-07 15:16:38.578676 lino-cms-23.10.0/lino_cms/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      462 2022-09-21 06:55:46.000000 lino-cms-23.10.0/lino_cms/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-10-07 15:16:38.582676 lino-cms-23.10.0/lino_cms/lib/
--rw-rw-r--   0 luc       (1000) www-data    (33)      221 2022-09-21 12:20:15.000000 lino-cms-23.10.0/lino_cms/lib/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-10-07 15:16:38.582676 lino-cms-23.10.0/lino_cms/lib/cal/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      290 2021-09-06 10:42:59.000000 lino-cms-23.10.0/lino_cms/lib/cal/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-10-07 15:16:38.582676 lino-cms-23.10.0/lino_cms/lib/cal/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:36:34.000000 lino-cms-23.10.0/lino_cms/lib/cal/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       45 2016-02-22 08:52:24.000000 lino-cms-23.10.0/lino_cms/lib/cal/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1248 2021-04-07 10:22:55.000000 lino-cms-23.10.0/lino_cms/lib/cal/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1177 2022-09-27 08:37:31.000000 lino-cms-23.10.0/lino_cms/lib/cal/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-10-07 15:16:38.582676 lino-cms-23.10.0/lino_cms/lib/cms/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      140 2022-09-30 06:57:05.000000 lino-cms-23.10.0/lino_cms/lib/cms/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      433 2022-09-20 14:11:43.000000 lino-cms-23.10.0/lino_cms/lib/cms/help_texts.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      380 2023-03-26 18:58:23.000000 lino-cms-23.10.0/lino_cms/lib/cms/layouts.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-10-07 15:16:38.578676 lino-cms-23.10.0/lino_cms/lib/cms/locale/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-10-07 15:16:38.578676 lino-cms-23.10.0/lino_cms/lib/cms/locale/de/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-10-07 15:16:38.582676 lino-cms-23.10.0/lino_cms/lib/cms/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3670 2022-09-11 01:24:12.000000 lino-cms-23.10.0/lino_cms/lib/cms/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 luc       (1000) www-data    (33)    13588 2022-09-21 12:23:06.000000 lino-cms-23.10.0/lino_cms/lib/cms/locale/de/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-10-07 15:16:38.578676 lino-cms-23.10.0/lino_cms/lib/cms/locale/et/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-10-07 15:16:38.582676 lino-cms-23.10.0/lino_cms/lib/cms/locale/et/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    27800 2022-09-11 01:24:12.000000 lino-cms-23.10.0/lino_cms/lib/cms/locale/et/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-10-07 15:16:38.578676 lino-cms-23.10.0/lino_cms/lib/cms/locale/fr/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-10-07 15:16:38.582676 lino-cms-23.10.0/lino_cms/lib/cms/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 luc       (1000) www-data    (33)    13271 2022-09-21 12:23:07.000000 lino-cms-23.10.0/lino_cms/lib/cms/locale/fr/LC_MESSAGES/django.po
--rw-rw-rw-   0 luc       (1000) www-data    (33)      670 2022-09-11 01:24:12.000000 lino-cms-23.10.0/lino_cms/lib/cms/migrate.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      140 2022-09-11 01:24:12.000000 lino-cms-23.10.0/lino_cms/lib/cms/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     2069 2023-09-28 02:47:39.000000 lino-cms-23.10.0/lino_cms/lib/cms/settings.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1578 2023-09-28 03:52:00.000000 lino-cms-23.10.0/lino_cms/lib/cms/user_types.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-10-07 15:16:38.582676 lino-cms-23.10.0/lino_cms/lib/users/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      233 2022-09-21 06:57:17.000000 lino-cms-23.10.0/lino_cms/lib/users/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-10-07 15:16:38.582676 lino-cms-23.10.0/lino_cms/lib/users/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2022-09-11 01:24:12.000000 lino-cms-23.10.0/lino_cms/lib/users/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2022-09-11 01:24:12.000000 lino-cms-23.10.0/lino_cms/lib/users/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2022-09-11 01:24:12.000000 lino-cms-23.10.0/lino_cms/lib/users/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       52 2022-09-11 01:24:12.000000 lino-cms-23.10.0/lino_cms/lib/users/fixtures/demo_users.py
--rw-rw-r--   0 luc       (1000) www-data    (33)      333 2023-01-07 06:56:16.000000 lino-cms-23.10.0/lino_cms/lib/users/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)      636 2023-01-07 06:56:16.000000 lino-cms-23.10.0/lino_cms/lib/users/ui.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2607 2023-10-07 15:16:31.000000 lino-cms-23.10.0/lino_cms/setup_info.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-10-07 15:16:38.582676 lino-cms-23.10.0/lino_cms.egg-info/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1443 2023-10-07 15:16:38.000000 lino-cms-23.10.0/lino_cms.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1179 2023-10-07 15:16:38.000000 lino-cms-23.10.0/lino_cms.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-10-07 15:16:38.000000 lino-cms-23.10.0/lino_cms.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        8 2023-10-07 15:16:38.000000 lino-cms-23.10.0/lino_cms.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        9 2023-10-07 15:16:38.000000 lino-cms-23.10.0/lino_cms.egg-info/top_level.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       60 2022-09-11 01:24:12.000000 lino-cms-23.10.0/requirements-install.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       36 2022-09-11 01:24:12.000000 lino-cms-23.10.0/requirements.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-10-07 15:16:38.582676 lino-cms-23.10.0/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      179 2022-09-11 01:24:12.000000 lino-cms-23.10.0/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      287 2022-09-21 12:22:41.000000 lino-cms-23.10.0/tasks.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-10-07 15:16:38.582676 lino-cms-23.10.0/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1238 2022-09-11 01:24:12.000000 lino-cms-23.10.0/tests/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      189 2022-09-11 01:24:12.000000 lino-cms-23.10.0/tests/test_docs.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      242 2022-09-11 01:24:12.000000 lino-cms-23.10.0/tests/test_packages.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-03 13:31:06.984931 lino-cms-24.5.0/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2022-09-11 01:24:12.000000 lino-cms-24.5.0/COPYING
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       69 2022-09-11 01:24:12.000000 lino-cms-24.5.0/MANIFEST.in
+-rw-r--r--   0 luc       (1000) www-data    (33)     1469 2024-05-03 13:31:06.984931 lino-cms-24.5.0/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      698 2023-10-22 20:23:51.000000 lino-cms-24.5.0/README.rst
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-03 13:31:06.980931 lino-cms-24.5.0/lino_cms/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      461 2024-02-14 17:37:55.000000 lino-cms-24.5.0/lino_cms/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-03 13:31:06.980931 lino-cms-24.5.0/lino_cms/lib/
+-rw-rw-r--   0 luc       (1000) www-data    (33)      220 2024-02-14 17:37:55.000000 lino-cms-24.5.0/lino_cms/lib/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-03 13:31:06.980931 lino-cms-24.5.0/lino_cms/lib/cal/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      288 2024-02-14 17:37:55.000000 lino-cms-24.5.0/lino_cms/lib/cal/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-03 13:31:06.980931 lino-cms-24.5.0/lino_cms/lib/cal/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:36:34.000000 lino-cms-24.5.0/lino_cms/lib/cal/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       45 2016-02-22 08:52:24.000000 lino-cms-24.5.0/lino_cms/lib/cal/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1617 2024-02-14 17:37:55.000000 lino-cms-24.5.0/lino_cms/lib/cal/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1180 2024-02-14 17:37:55.000000 lino-cms-24.5.0/lino_cms/lib/cal/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-03 13:31:06.980931 lino-cms-24.5.0/lino_cms/lib/cms/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      140 2022-09-30 06:57:05.000000 lino-cms-24.5.0/lino_cms/lib/cms/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      442 2024-02-14 17:37:55.000000 lino-cms-24.5.0/lino_cms/lib/cms/help_texts.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      374 2023-10-29 08:51:05.000000 lino-cms-24.5.0/lino_cms/lib/cms/layouts.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-03 13:31:06.976931 lino-cms-24.5.0/lino_cms/lib/cms/locale/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-03 13:31:06.976931 lino-cms-24.5.0/lino_cms/lib/cms/locale/de/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-03 13:31:06.980931 lino-cms-24.5.0/lino_cms/lib/cms/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3670 2022-09-11 01:24:12.000000 lino-cms-24.5.0/lino_cms/lib/cms/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 luc       (1000) www-data    (33)    13588 2022-09-21 12:23:06.000000 lino-cms-24.5.0/lino_cms/lib/cms/locale/de/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-03 13:31:06.976931 lino-cms-24.5.0/lino_cms/lib/cms/locale/et/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-03 13:31:06.980931 lino-cms-24.5.0/lino_cms/lib/cms/locale/et/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    27800 2022-09-11 01:24:12.000000 lino-cms-24.5.0/lino_cms/lib/cms/locale/et/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-03 13:31:06.976931 lino-cms-24.5.0/lino_cms/lib/cms/locale/fr/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-03 13:31:06.980931 lino-cms-24.5.0/lino_cms/lib/cms/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 luc       (1000) www-data    (33)    13271 2022-09-21 12:23:07.000000 lino-cms-24.5.0/lino_cms/lib/cms/locale/fr/LC_MESSAGES/django.po
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      670 2024-02-14 17:37:55.000000 lino-cms-24.5.0/lino_cms/lib/cms/migrate.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      140 2022-09-11 01:24:12.000000 lino-cms-24.5.0/lino_cms/lib/cms/models.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     2726 2024-03-27 08:42:23.000000 lino-cms-24.5.0/lino_cms/lib/cms/settings.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1631 2024-02-14 17:37:55.000000 lino-cms-24.5.0/lino_cms/lib/cms/user_types.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-03 13:31:06.980931 lino-cms-24.5.0/lino_cms/lib/users/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      233 2022-09-21 06:57:17.000000 lino-cms-24.5.0/lino_cms/lib/users/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-03 13:31:06.984931 lino-cms-24.5.0/lino_cms/lib/users/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2022-09-11 01:24:12.000000 lino-cms-24.5.0/lino_cms/lib/users/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2022-09-11 01:24:12.000000 lino-cms-24.5.0/lino_cms/lib/users/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       47 2024-02-14 17:37:55.000000 lino-cms-24.5.0/lino_cms/lib/users/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       52 2022-09-11 01:24:12.000000 lino-cms-24.5.0/lino_cms/lib/users/fixtures/demo_users.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)      333 2023-01-07 06:56:16.000000 lino-cms-24.5.0/lino_cms/lib/users/models.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)      684 2024-02-14 17:37:55.000000 lino-cms-24.5.0/lino_cms/lib/users/ui.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2801 2024-05-03 13:30:41.000000 lino-cms-24.5.0/lino_cms/setup_info.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-03 13:31:06.984931 lino-cms-24.5.0/lino_cms.egg-info/
+-rw-r--r--   0 luc       (1000) www-data    (33)     1469 2024-05-03 13:31:06.000000 lino-cms-24.5.0/lino_cms.egg-info/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1179 2024-05-03 13:31:06.000000 lino-cms-24.5.0/lino_cms.egg-info/SOURCES.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2024-05-03 13:31:06.000000 lino-cms-24.5.0/lino_cms.egg-info/dependency_links.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        8 2024-05-03 13:31:06.000000 lino-cms-24.5.0/lino_cms.egg-info/requires.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        9 2024-05-03 13:31:06.000000 lino-cms-24.5.0/lino_cms.egg-info/top_level.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       60 2022-09-11 01:24:12.000000 lino-cms-24.5.0/requirements-install.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       36 2022-09-11 01:24:12.000000 lino-cms-24.5.0/requirements.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)       38 2024-05-03 13:31:06.984931 lino-cms-24.5.0/setup.cfg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      180 2024-02-14 17:37:55.000000 lino-cms-24.5.0/setup.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      319 2024-02-14 17:37:55.000000 lino-cms-24.5.0/tasks.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-03 13:31:06.984931 lino-cms-24.5.0/tests/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1236 2024-02-14 17:37:55.000000 lino-cms-24.5.0/tests/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      180 2024-02-14 17:37:55.000000 lino-cms-24.5.0/tests/test_docs.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      243 2024-02-14 17:37:55.000000 lino-cms-24.5.0/tests/test_packages.py
```

### Comparing `lino-cms-23.10.0/COPYING` & `lino-cms-24.5.0/COPYING`

 * *Files identical despite different names*

### Comparing `lino-cms-23.10.0/PKG-INFO` & `lino-cms-24.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 Metadata-Version: 2.1
 Name: lino-cms
-Version: 23.10.0
+Version: 24.5.0
 Summary: Manage the content of your website
 Home-page: https://gitlab.com/lino-framework/cms
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 License-File: COPYING
+Requires-Dist: lino-xl
 
 
 **Lino CMS** is a Content Management System à la Lino.
 
-- Source code: https://gitlab.com/lino-framework/cms
+- Public demo : https://cms1.mylino.net
 
 - Documentation: https://lino-framework.gitlab.io/cms/
 
+- Source code: https://gitlab.com/lino-framework/cms
+
 - This project is part of the Lino framework, which is documented
   at https://www.lino-framework.org
 
 - Changelog: https://lino-framework.gitlab.io/cms/changes.html
 
 - For introductions, commercial information and hosting solutions
   see https://www.saffre-rumma.net
 
 - This is a sustainably free open-source project. Your contributions are
   welcome.  See https://community.lino-framework.org for details.
 
 
-
-
```

### Comparing `lino-cms-23.10.0/README.rst` & `lino-cms-24.5.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 
 
 **Lino CMS** is a Content Management System à la Lino.
 
 - Source code: https://gitlab.com/lino-framework/cms
 
+- Public demo : https://cms1.mylino.net
+
 - Documentation: https://lino-framework.gitlab.io/cms/
 
 - This project is part of the Lino framework, which is documented
   at https://www.lino-framework.org
 
 - Changelog: https://lino-framework.gitlab.io/cms/changes.html
```

### Comparing `lino-cms-23.10.0/lino_cms/lib/cal/fixtures/std.py` & `lino-cms-24.5.0/lino_cms/lib/cal/fixtures/std.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,25 +17,28 @@
 
     yield GuestRole(**dd.str2kw('name', _("Participant")))
     yield GuestRole(**dd.str2kw('name', _("Guide")))
     yield GuestRole(**dd.str2kw('name', _("Teacher")))
 
     EventType = rt.models.cal.EventType
     RecurrentEvent = rt.models.cal.RecurrentEvent
-    Recurrencies = rt.models.cal.Recurrencies
+    Recurrences = rt.models.cal.Recurrences
     DEMO_START_YEAR = rt.models.cal.DEMO_START_YEAR
 
-    holidays = EventType.objects.get(
-        **dd.str2kw('name', _("Holidays")))
-    yield RecurrentEvent(
-        event_type=holidays,
-        every_unit=Recurrencies.yearly,
-        monday=True, tuesday=True, wednesday=True, thursday=True,
-        friday=True, saturday=True, sunday=True,
-        every=1,
-        start_date=datetime.date(
-            year=DEMO_START_YEAR,
-            month=7, day=1),
-        end_date=datetime.date(
-            year=DEMO_START_YEAR,
-            month=8, day=31),
-        **dd.str2kw('name', _("Summer holidays")))
+    holidays = EventType.objects.get(**dd.str2kw('name', _("Holidays")))
+    yield RecurrentEvent(event_type=holidays,
+                         every_unit=Recurrences.yearly,
+                         monday=True,
+                         tuesday=True,
+                         wednesday=True,
+                         thursday=True,
+                         friday=True,
+                         saturday=True,
+                         sunday=True,
+                         every=1,
+                         start_date=datetime.date(year=DEMO_START_YEAR,
+                                                  month=7,
+                                                  day=1),
+                         end_date=datetime.date(year=DEMO_START_YEAR,
+                                                month=8,
+                                                day=31),
+                         **dd.str2kw('name', _("Summer holidays")))
```

### Comparing `lino-cms-23.10.0/lino_cms/lib/cal/models.py` & `lino-cms-24.5.0/lino_cms/lib/cal/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # -*- coding: UTF-8 -*-
 # Copyright 2013-2022 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
-
 from django.utils.translation import gettext_lazy as _
 
 from lino.modlib.users.choicelists import UserTypes
 from lino.modlib.office.roles import OfficeUser
 from lino.modlib.publisher.mixins import Publishable
-from lino.modlib.publisher.choicelists import PublisherViews
+# from lino.modlib.publisher.choicelists import PublisherViews
 from lino.modlib.memo.mixins import BabelPreviewable
 from lino_xl.lib.cal.models import *
 from lino_xl.lib.courses.choicelists import EnrolmentStates
 
 
-
 class Room(Room, Publishable, BabelPreviewable):
 
     class Meta(Room.Meta):
         abstract = dd.is_abstract_model(__name__, 'Room')
 
 
 class Rooms(Rooms):
     column_names = "name company company__city *"
     detail_layout = """
     id name
     company contact_person contact_role
     cal.EntriesByRoom
     """
 
-PublisherViews.add_item_lazy("rooms", Rooms)
+
+# PublisherViews.add_item_lazy("rooms", Rooms)
 
 
 class Event(Event, Publishable, BabelPreviewable):
 
     class Meta(Event.Meta):
         abstract = dd.is_abstract_model(__name__, 'Event')
```

### Comparing `lino-cms-23.10.0/lino_cms/lib/cms/locale/de/LC_MESSAGES/django.mo` & `lino-cms-24.5.0/lino_cms/lib/cms/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-cms-23.10.0/lino_cms/lib/cms/locale/de/LC_MESSAGES/django.po` & `lino-cms-24.5.0/lino_cms/lib/cms/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-cms-23.10.0/lino_cms/lib/cms/locale/et/LC_MESSAGES/django.po` & `lino-cms-24.5.0/lino_cms/lib/cms/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-cms-23.10.0/lino_cms/lib/cms/locale/fr/LC_MESSAGES/django.po` & `lino-cms-24.5.0/lino_cms/lib/cms/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-cms-23.10.0/lino_cms/lib/cms/migrate.py` & `lino-cms-24.5.0/lino_cms/lib/cms/migrate.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: UTF-8 -*-
 # Copyright 2016-2022 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
-
 """Default data migrator for Lino Cms.
 
 
 """
 
 from django.conf import settings
 from lino.api import dd, rt
 from lino.utils.dpy import Migrator, override
 
+
 class Migrator(Migrator):
     """The standard migrator for Lino Cms.
 
     This is used because
     :class:`lino_cms.projects.cms.settings.Site` has
     :attr:`migration_class <lino.core.site.Site.migration_class>` set
     to ``"lino_cms.lib.cms.migrate.Migrator"``.
 
     """
+
     def migrate_from_0_0_1(self, globals_dict):
         # do something here
         return '0.0.2'
-
```

### Comparing `lino-cms-23.10.0/lino_cms/lib/cms/settings.py` & `lino-cms-24.5.0/lino_cms/lib/cms/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,77 @@
 # -*- coding: UTF-8 -*-
-# Copyright 2016-2023 Rumma & Ko Ltd
+# Copyright 2016-2024 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 from lino.projects.std.settings import *
 from lino_cms import SETUP_INFO
 
+
 class Site(Site):
 
     verbose_name = "Lino CMS"
     description = SETUP_INFO['description']
     version = SETUP_INFO['version']
     url = SETUP_INFO['url']
+    # use_linod = True
 
+    # demo_fixtures = ['std', 'demo', 'demo2', 'checkdata', 'checksummaries']
     demo_fixtures = ['std', 'demo', 'demo2', 'checkdata']
     user_types_module = 'lino_cms.lib.cms.user_types'
     custom_layouts_module = 'lino_cms.lib.cms.layouts'
     migration_class = 'lino_cms.lib.cms.migrate.Migrator'
-    default_ui = "lino_react.react"
+    # default_ui = "lino_react.react"
+
+    default_ui = None
+    web_front_ends = [(None, "lino.modlib.publisher"),
+                      ('admin', "lino_react.react")]
 
-    def setup_features(self):
-        super().setup_features()
-        self.enable_feature('third_party_authentication')
+    # ('ext', "lino.modlib.extjs")]
 
-    def get_installed_apps(self):
-        """Implements :meth:`lino.core.site.Site.get_installed_apps`.
+    def get_installed_plugins(self):
+        """Implements :meth:`lino.core.site.Site.get_installed_plugins`.
 
         """
-        yield super(Site, self).get_installed_apps()
+        yield super().get_installed_plugins()
         yield 'lino_cms.lib.cms'
         yield 'lino_cms.lib.users'
         yield 'lino_xl.lib.contacts'
         # yield 'lino_cms.lib.cal'
         # yield 'lino_xl.lib.calview'
         yield 'lino_xl.lib.pages'
         yield 'lino_xl.lib.blogs'
         yield 'lino_xl.lib.albums'
+        yield 'lino_xl.lib.topics'
+        yield 'lino_xl.lib.sources'
         yield 'lino.modlib.comments'
         # yield 'lino.modlib.uploads'
         yield 'lino.modlib.help'
         yield 'lino.modlib.publisher'
+        # yield 'lino.modlib.summaries'
         yield 'lino.modlib.checkdata'  # fill body_preview during prep
 
     # def setup_quicklinks(self, ut, tb):
     #     super(Site, self).setup_quicklinks(ut, tb)
 
     def get_plugin_configs(self):
         yield super().get_plugin_configs()
         # yield ('system', 'use_dashboard_layouts', True)
+        # yield ('linod', 'use_channels', True)
         yield ('users', 'allow_online_registration', True)
+        yield 'users', 'third_party_authentication', True
         # yield ('cal', 'with_demo_appointments', False)
         yield ('help', 'make_help_pages', True)
         yield ('help', 'use_contacts', True)
         yield ('help', 'include_useless', True)
-        yield ('memo', 'short_preview_length', 600)
+        yield ('memo', 'short_preview_length', 1200)
+        yield ('publisher', 'locations',
+               (('b', 'blogs.LatestEntries'),
+                ('p', 'pages.Pages'),
+                ('r', 'uploads.Uploads'),
+                ('s', 'sources.Sources'),
+                ('t', 'topics.Topics'),
+                ('u', 'users.Users')))
+
 
 from lino.core.auth.utils import activate_social_auth_testing
+
 activate_social_auth_testing(globals())
```

### Comparing `lino-cms-23.10.0/lino_cms/lib/cms/user_types.py` & `lino-cms-24.5.0/lino_cms/lib/cms/user_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # -*- coding: UTF-8 -*-
 # Copyright 2017-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
-
 """Defines the user types for a Lino CMS.
 
 """
 
 from lino.core.roles import UserRole, SiteAdmin, SiteStaff, SiteUser
 from lino_xl.lib.blogs.roles import BlogsReader
+from lino_xl.lib.topics.roles import TopicsUser
 from lino_xl.lib.cal.roles import CalendarReader
 from lino.modlib.checkdata.roles import CheckdataUser
 from lino.modlib.search.roles import SiteSearcher
 from lino.modlib.office.roles import OfficeUser, OfficeStaff, OfficeOperator
 from lino.modlib.uploads.roles import UploadsReader
 from lino.modlib.comments.roles import CommentsUser, CommentsStaff, CommentsReader
 
 from lino.modlib.users.choicelists import UserTypes
 from django.utils.translation import gettext_lazy as _
 
 
-class EndUser(BlogsReader, SiteUser, CheckdataUser, CommentsUser,
-    OfficeUser, CommentsReader, CalendarReader):
+class EndUser(BlogsReader, SiteUser, CheckdataUser, CommentsUser, OfficeUser,
+              CommentsReader, CalendarReader, TopicsUser):
     """An **end user** is somebody who uses our database, but won't work
     on it.
 
     """
     pass
 
 
@@ -36,14 +36,19 @@
     """Can do everything."""
 
 
 # class Anonymous(CommentsReader, CalendarReader):
 class Anonymous(SiteSearcher, BlogsReader, CalendarReader, UploadsReader):
     pass
 
+
 UserTypes.clear()
 add = UserTypes.add_item
-add('000', _("Anonymous"),        Anonymous, 'anonymous',
-    readonly=True, authenticated=False)
-add('100', _("User"),             EndUser, 'user')
-add('800', _("Staff"),            Staff, 'staff')
-add('900', _("Administrator"),    Admin, 'admin')
+add('000',
+    _("Anonymous"),
+    Anonymous,
+    'anonymous',
+    readonly=True,
+    authenticated=False)
+add('100', _("User"), EndUser, 'user')
+add('800', _("Staff"), Staff, 'staff')
+add('900', _("Administrator"), Admin, 'admin')
```

### Comparing `lino-cms-23.10.0/lino_cms/lib/users/ui.py` & `lino-cms-24.5.0/lino_cms/lib/users/ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # -*- coding: UTF-8 -*-
 # Copyright 2016-2022 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 from lino.api import dd, _
 from lino.modlib.users.ui import *
 
+
 class UserDetail(UserDetail):
 
     main = "general contact"
 
     general = dd.Panel("""
     box1
     remarks:40 users.AuthoritiesGiven:20
-    """, label=_("General"))
+    """,
+                       label=_("General"))
 
     box1 = """
     username user_type:20
     language time_zone
     id created modified
     """
 
     contact = dd.Panel("""
     first_name last_name initials
-    """, label=_("Contact"))
+    """,
+                       label=_("Contact"))
+
 
 Users.detail_layout = UserDetail()
 
 Users.column_names = "first_name email"
```

### Comparing `lino-cms-23.10.0/lino_cms/setup_info.py` & `lino-cms-24.5.0/lino_cms/setup_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 # -*- coding: UTF-8 -*-
-# Copyright 2022-2023 Rumma & Ko Ltd
+# Copyright 2022-2024 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 # Some content of this file is explicitly modified by `getlino startproject`.
 # Please check for consistency with getlino.startproject.py file before you
 # modify anything.
 
-SETUP_INFO = dict(
-    name='lino-cms',
-    version='23.10.0',
-    install_requires=['lino-xl'],
-    description=('Manage the content of your website'),
-    long_description="""\
+SETUP_INFO = dict(name='lino-cms',
+                  version='24.5.0',
+                  install_requires=['lino-xl'],
+                  description=('Manage the content of your website'),
+                  long_description="""\
 
 **Lino CMS** is a Content Management System à la Lino.
 
-- Source code: https://gitlab.com/lino-framework/cms
+- Public demo : https://cms1.mylino.net
 
 - Documentation: https://lino-framework.gitlab.io/cms/
 
+- Source code: https://gitlab.com/lino-framework/cms
+
 - This project is part of the Lino framework, which is documented
   at https://www.lino-framework.org
 
 - Changelog: https://lino-framework.gitlab.io/cms/changes.html
 
 - For introductions, commercial information and hosting solutions
   see https://www.saffre-rumma.net
 
 - This is a sustainably free open-source project. Your contributions are
   welcome.  See https://community.lino-framework.org for details.
 
 
 """,
-    author='Rumma & Ko Ltd',
-    author_email='info@lino-framework.org',
-    url="https://gitlab.com/lino-framework/cms",
-    license_files=['COPYING'],
-    test_suite='tests')
+                  author='Rumma & Ko Ltd',
+                  author_email='info@lino-framework.org',
+                  url="https://gitlab.com/lino-framework/cms",
+                  license_files=['COPYING'],
+                  test_suite='tests')
 
 SETUP_INFO.update(classifiers="""
 Programming Language :: Python
 Programming Language :: Python :: 3
 Development Status :: 1 - Planning
 Environment :: Web Environment
 Framework :: Django
@@ -58,22 +59,23 @@
     'lino_cms.lib.cal',
     'lino_cms.lib.cal.fixtures',
     'lino_cms.lib.cms',
     'lino_cms.lib.users',
     'lino_cms.lib.users.fixtures',
 ])
 
-SETUP_INFO.update(message_extractors={
-    'lino_cms': [
-        ('**/cache/**', 'ignore', None),
-        ('**.py', 'python', None),
-        ('**.js', 'javascript', None),
-        ('**/config/**.html', 'jinja2', None),
-    ],
-})
+SETUP_INFO.update(
+    message_extractors={
+        'lino_cms': [
+            ('**/cache/**', 'ignore', None),
+            ('**.py', 'python', None),
+            ('**.js', 'javascript', None),
+            ('**/config/**.html', 'jinja2', None),
+        ],
+    })
 
 SETUP_INFO.update(include_package_data=True)
 
 # SETUP_INFO.update(package_data=dict())
 #
 # def add_package_data(package, *patterns):
 #     l = SETUP_INFO['package_data'].setdefault(package, [])
```

### Comparing `lino-cms-23.10.0/lino_cms.egg-info/PKG-INFO` & `lino-cms-24.5.0/lino_cms.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 Metadata-Version: 2.1
 Name: lino-cms
-Version: 23.10.0
+Version: 24.5.0
 Summary: Manage the content of your website
 Home-page: https://gitlab.com/lino-framework/cms
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 License-File: COPYING
+Requires-Dist: lino-xl
 
 
 **Lino CMS** is a Content Management System à la Lino.
 
-- Source code: https://gitlab.com/lino-framework/cms
+- Public demo : https://cms1.mylino.net
 
 - Documentation: https://lino-framework.gitlab.io/cms/
 
+- Source code: https://gitlab.com/lino-framework/cms
+
 - This project is part of the Lino framework, which is documented
   at https://www.lino-framework.org
 
 - Changelog: https://lino-framework.gitlab.io/cms/changes.html
 
 - For introductions, commercial information and hosting solutions
   see https://www.saffre-rumma.net
 
 - This is a sustainably free open-source project. Your contributions are
   welcome.  See https://community.lino-framework.org for details.
 
 
-
-
```

### Comparing `lino-cms-23.10.0/lino_cms.egg-info/SOURCES.txt` & `lino-cms-24.5.0/lino_cms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lino-cms-23.10.0/tests/__init__.py` & `lino-cms-24.5.0/tests/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 exec(compile(open(filename, "rb").read(), filename, 'exec'))
 
 from lino.utils.pythontest import TestCase
 
 import os
 #os.environ['DJANGO_SETTINGS_MODULE'] = "lino_cms.settings.test"
 
-
 # class BaseTestCase(TestCase):
 #     project_root = ROOTDIR
 #     django_settings_module = 'lino_noi.settings.test'
 
 
 class PackagesTests(TestCase):
 
@@ -47,8 +46,7 @@
 
 class DemoTests(TestCase):
     """Run tests on the demo projects.
     """
 
     def test_cms(self):
         self.run_django_manage_test('lino_cms/projects/cms')
-
```


# Comparing `tmp/pigeonpost-0.4.5.tar.gz` & `tmp/pigeonpost-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigeonpost-0.4.5.tar", last modified: Thu May  2 23:58:02 2024, max compression
+gzip compressed data, was "pigeonpost-0.4.6.tar", last modified: Fri May  3 08:15:48 2024, max compression
```

## Comparing `pigeonpost-0.4.5.tar` & `pigeonpost-0.4.6.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.064853 pigeonpost-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 23:58:02.064853 pigeonpost-0.4.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.052853 pigeonpost-0.4.5/pigeon/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.052853 pigeonpost-0.4.5/pigeon/conf/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/conf/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/conf/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/conf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.056853 pigeonpost-0.4.5/pigeon/core/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/core/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/core/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/core/secure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/core/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.056853 pigeonpost-0.4.5/pigeon/default/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/default/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.056853 pigeonpost-0.4.5/pigeon/files/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/files/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/files/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.056853 pigeonpost-0.4.5/pigeon/http/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/http/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/http/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/http/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/http/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.056853 pigeonpost-0.4.5/pigeon/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.060853 pigeonpost-0.4.5/pigeon/middleware/components/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/cache_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/component.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/content_negotiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/cors.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/date.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/host.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/mediafiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/method.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/staticfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.060853 pigeonpost-0.4.5/pigeon/middleware/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/conversion/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.060853 pigeonpost-0.4.5/pigeon/middleware/conversion/mime/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/conversion/mime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/conversion/mime/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/conversion/mime/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.060853 pigeonpost-0.4.5/pigeon/templating/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/templating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/templating/templater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.060853 pigeonpost-0.4.5/pigeon/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/utils/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3260 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.064853 pigeonpost-0.4.5/pigeonpost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 23:58:02.000000 pigeonpost-0.4.5/pigeonpost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-02 23:58:02.000000 pigeonpost-0.4.5/pigeonpost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 23:58:02.000000 pigeonpost-0.4.5/pigeonpost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 23:58:02.000000 pigeonpost-0.4.5/pigeonpost.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 23:58:02.000000 pigeonpost-0.4.5/pigeonpost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 23:58:02.000000 pigeonpost-0.4.5/pigeonpost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-02 23:58:02.064853 pigeonpost-0.4.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.587046 pigeonpost-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-03 08:15:48.587046 pigeonpost-0.4.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.579046 pigeonpost-0.4.6/pigeon/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.579046 pigeonpost-0.4.6/pigeon/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/conf/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/conf/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/conf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.583046 pigeonpost-0.4.6/pigeon/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/core/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/core/secure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/core/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.583046 pigeonpost-0.4.6/pigeon/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/default/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.583046 pigeonpost-0.4.6/pigeon/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/files/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/files/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.583046 pigeonpost-0.4.6/pigeon/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/http/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/http/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/http/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/http/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.583046 pigeonpost-0.4.6/pigeon/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.587046 pigeonpost-0.4.6/pigeon/middleware/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/cache_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/content_negotiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/mediafiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/staticfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.587046 pigeonpost-0.4.6/pigeon/middleware/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/conversion/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.587046 pigeonpost-0.4.6/pigeon/middleware/conversion/mime/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/conversion/mime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/conversion/mime/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/conversion/mime/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.587046 pigeonpost-0.4.6/pigeon/templating/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/templating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/templating/templater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.587046 pigeonpost-0.4.6/pigeon/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/utils/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3260 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.587046 pigeonpost-0.4.6/pigeonpost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-03 08:15:48.000000 pigeonpost-0.4.6/pigeonpost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-03 08:15:48.000000 pigeonpost-0.4.6/pigeonpost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 08:15:48.000000 pigeonpost-0.4.6/pigeonpost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-03 08:15:48.000000 pigeonpost-0.4.6/pigeonpost.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 08:15:48.000000 pigeonpost-0.4.6/pigeonpost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 08:15:48.000000 pigeonpost-0.4.6/pigeonpost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-03 08:15:48.591046 pigeonpost-0.4.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/setup.py
```

### Comparing `pigeonpost-0.4.5/pigeon/__init__.py` & `pigeonpost-0.4.6/pigeon/__init__.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/conf/manager.py` & `pigeonpost-0.4.6/pigeon/conf/manager.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/conf/settings.py` & `pigeonpost-0.4.6/pigeon/conf/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # VERBOSITY
 VERBOSITY = 2
 
 # ADDRESS
 ADDRESS = ''
 PORT = 8080
 
-# REUSE SOCKET AUTOMATICALLY
-REUSE_SOCKET = True
-
 # ALLOWED HOSTS
 ALLOWED_HOSTS = ['*']
 # ALLOWED METHODS
 ALLOWED_METHODS = ['POST', 'GET', 'HEAD', 'POST', 'PUT', 'OPTIONS']
 
 # ACCESS-CONTROL
 CORS_ALLOWED_ORIGINS = []
```

### Comparing `pigeonpost-0.4.5/pigeon/core/app.py` & `pigeonpost-0.4.6/pigeon/core/app.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/core/handler.py` & `pigeonpost-0.4.6/pigeon/core/handler.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/core/secure.py` & `pigeonpost-0.4.6/pigeon/core/secure.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/core/server.py` & `pigeonpost-0.4.6/pigeon/core/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 def serve():
     log.info(f'ADDRESS: {Manager.address if Manager.address else "ANY"}')
     log.info(f'PORT: {Manager.port}')
 
     # open socket
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    if Manager.reuse_socket:
+    if Manager.debug_mode:
         sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
     sock.setblocking(False)
     sock.bind((Manager.address, Manager.port))
 
     # configure https if specified in settings
     if Manager.use_https:
         log.verbose('USING HTTPS')
```

### Comparing `pigeonpost-0.4.5/pigeon/default/errors.py` & `pigeonpost-0.4.6/pigeon/default/errors.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/files/media.py` & `pigeonpost-0.4.6/pigeon/files/media.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/files/static.py` & `pigeonpost-0.4.6/pigeon/files/static.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/http/message.py` & `pigeonpost-0.4.6/pigeon/http/message.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,23 +67,28 @@
 
 
 
 class HTTPMessage:
     """
     An HTTP message (obv either response or request)
     """
-    def __init__(self, headers: dict[str, str], data: str, protocol: str, content_type=None):
+    def __init__(self, headers: dict[str, str], data: str, protocol: str, content_type=None, cookies=None, **kwargs):
         # headers of HTTP message
         self.headers: HTTPHeaders = HTTPHeaders(headers or None)
         if content_type:
             self.headers.content_type = content_type
         # http message body (data)
         self.data: Any = data
         # protocol used (e.g. 1.1, 1.0, 2.0, ...)
         self.protocol: str = protocol
+        # cookies of request
+        self.cookies: LowerParameterDict = LowerParameterDict(cookies or dict())
+
+        # kwargs for additional processing e.g. for middleware components
+        self.additional = kwargs
 
     @property
     def is_error(self):
         raise NotImplementedError
 
     def set_headers(self, headers):
         """
```

### Comparing `pigeonpost-0.4.5/pigeon/http/request.py` & `pigeonpost-0.4.6/pigeon/http/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from pigeon.http.message import HTTPMessage
 from pigeon.utils.common import ParameterDict
 
 
 class HTTPRequest(HTTPMessage):
-    def __init__(self, method: str, path: str, headers: dict = None, get: dict = None, data=None, files=None, protocol: str='1.1', content_type=None):
+    def __init__(self, method: str, path: str, headers: dict = None, get: dict = None, data=None, files=None, protocol: str='1.1', content_type=None, **kwargs):
         """
         Class representing an HTTP request
         """
-        super().__init__(headers, data, protocol, content_type)
+        super().__init__(headers, data, protocol, content_type, kwargs)
         self.method = method
         self.path = path
 
         self.get = ParameterDict(get or None)
         self.files = ParameterDict(get or None)
 
         # credentials (or other auth related) send in request
```

### Comparing `pigeonpost-0.4.5/pigeon/http/response.py` & `pigeonpost-0.4.6/pigeon/http/response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from typing import Any
 from pigeon.http.message import HTTPMessage
 import pigeon.http.common as common
 import json
 
-
 class HTTPResponse(HTTPMessage):
-    def __init__(self, headers: dict = None, data: str = None, status: int = 200, cookies=None, protocol: str = '1.1', content_type=None):
+    def __init__(self, headers: dict = None, data: str = None, status: int = 200, cookies=None, protocol: str = '1.1', content_type=None, **kwargs):
         """
         Class representing an HTTP response
         """
-        super().__init__(headers, data, protocol, content_type)
+        super().__init__(headers, data, protocol, content_type, cookies, **kwargs)
 
         # HTTP Response status
         self.status = status
 
 
     @property
     def is_error(self):
```

### Comparing `pigeonpost-0.4.5/pigeon/middleware/auth.py` & `pigeonpost-0.4.6/pigeon/middleware/auth.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/middleware/components/__init__.py` & `pigeonpost-0.4.6/pigeon/middleware/components/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,11 +5,10 @@
 import pigeon.middleware.components.connection as connection
 import pigeon.middleware.components.server as server
 import pigeon.middleware.components.date as date
 import pigeon.middleware.components.cache_control as cache_control
 import pigeon.middleware.components.content_negotiation as content_negotiation
 import pigeon.middleware.components.mediafiles as mediafiles
 import pigeon.middleware.components.staticfiles as staticfiles
+import pigeon.middleware.components.cookies as cookies
 
-#
-# Components used by middleware preprocessors and postprocessors to process requests.
-#
+# Components are used by middleware preprocessors and postprocessors to process requests.
```

### Comparing `pigeonpost-0.4.5/pigeon/middleware/components/cache_control.py` & `pigeonpost-0.4.6/pigeon/middleware/components/cache_control.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/middleware/components/component.py` & `pigeonpost-0.4.6/pigeon/middleware/components/component.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/middleware/components/connection.py` & `pigeonpost-0.4.6/pigeon/middleware/components/connection.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/middleware/components/content_negotiation.py` & `pigeonpost-0.4.6/pigeon/middleware/components/content_negotiation.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/middleware/components/cors.py` & `pigeonpost-0.4.6/pigeon/middleware/components/cors.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/middleware/components/host.py` & `pigeonpost-0.4.6/pigeon/middleware/components/host.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/middleware/components/mediafiles.py` & `pigeonpost-0.4.6/pigeon/middleware/components/mediafiles.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/middleware/components/method.py` & `pigeonpost-0.4.6/pigeon/middleware/components/method.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/middleware/components/staticfiles.py` & `pigeonpost-0.4.6/pigeon/middleware/components/staticfiles.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/middleware/conversion/converter.py` & `pigeonpost-0.4.6/pigeon/middleware/conversion/converter.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/middleware/conversion/mime/parsers.py` & `pigeonpost-0.4.6/pigeon/middleware/conversion/mime/parsers.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/middleware/pipe.py` & `pigeonpost-0.4.6/pigeon/middleware/pipe.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/middleware/processing.py` & `pigeonpost-0.4.6/pigeon/middleware/processing.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,26 +72,28 @@
     """
     preprocessing_components = [
         comp.host.HostComponent,
         comp.cors.CORSComponent,
         comp.method.MethodComponent,
         comp.connection.ConnectionComponent,
         comp.cache_control.CacheControlComponent,
+        comp.cookies.CookieComponent,
         comp.content_negotiation.ContentNegotiationComponent,
     ]
     processing_components = [
         comp.content_negotiation.ContentNegotiationComponent,
         comp.staticfiles.StaticFilesComponent,
         comp.mediafiles.MediaFilesComponent,
     ]
     postprocessing_components = [
         comp.server.ServerComponent,
         comp.cors.CORSComponent,
         comp.connection.ConnectionComponent,
         comp.cache_control.CacheControlComponent,
+        comp.cookies.CookieComponent,
         comp.content_negotiation.ContentNegotiationComponent,
     ]
 
 
 class Raven(ComponentProcessor):
     """
     Processes requests using the HTTP/2.0 protocol
```

### Comparing `pigeonpost-0.4.5/pigeon/middleware/tags.py` & `pigeonpost-0.4.6/pigeon/middleware/tags.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/middleware/views.py` & `pigeonpost-0.4.6/pigeon/middleware/views.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/templating/templater.py` & `pigeonpost-0.4.6/pigeon/templating/templater.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeon/utils/common.py` & `pigeonpost-0.4.6/pigeon/utils/common.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -34,8 +34,8 @@
         super().__init__(data)
 
     @classmethod
     def _lower_key(cls, key):
         return key.replace('-', '_').lower()
 
     def __getattr__(self, key):
-        return self.data.get(LowerParameterDict._lower_key(key))
+        return self.data.get(LowerParameterDict._lower_key(key))
```

### Comparing `pigeonpost-0.4.5/pigeon/utils/logger.py` & `pigeonpost-0.4.6/pigeon/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.5/pigeonpost.egg-info/SOURCES.txt` & `pigeonpost-0.4.6/pigeonpost.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 pigeon/middleware/tags.py
 pigeon/middleware/views.py
 pigeon/middleware/components/__init__.py
 pigeon/middleware/components/cache_control.py
 pigeon/middleware/components/component.py
 pigeon/middleware/components/connection.py
 pigeon/middleware/components/content_negotiation.py
+pigeon/middleware/components/cookies.py
 pigeon/middleware/components/cors.py
 pigeon/middleware/components/date.py
 pigeon/middleware/components/host.py
 pigeon/middleware/components/mediafiles.py
 pigeon/middleware/components/method.py
 pigeon/middleware/components/server.py
 pigeon/middleware/components/staticfiles.py
```


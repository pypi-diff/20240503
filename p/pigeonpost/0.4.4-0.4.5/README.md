# Comparing `tmp/pigeonpost-0.4.4.tar.gz` & `tmp/pigeonpost-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigeonpost-0.4.4.tar", last modified: Thu May  2 21:57:37 2024, max compression
+gzip compressed data, was "pigeonpost-0.4.5.tar", last modified: Thu May  2 23:58:02 2024, max compression
```

## Comparing `pigeonpost-0.4.4.tar` & `pigeonpost-0.4.5.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.136956 pigeonpost-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-02 21:57:37.136956 pigeonpost-0.4.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.128956 pigeonpost-0.4.4/pigeon/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.128956 pigeonpost-0.4.4/pigeon/conf/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/conf/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/conf/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/conf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.128956 pigeonpost-0.4.4/pigeon/core/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/core/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/core/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/core/secure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/core/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.128956 pigeonpost-0.4.4/pigeon/default/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/default/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.128956 pigeonpost-0.4.4/pigeon/files/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/files/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/files/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.128956 pigeonpost-0.4.4/pigeon/http/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/http/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/http/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/http/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/http/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.132956 pigeonpost-0.4.4/pigeon/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.132956 pigeonpost-0.4.4/pigeon/middleware/components/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/cache_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/component.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/content_negotiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/cors.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/date.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/host.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/mediafiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/method.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/staticfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.132956 pigeonpost-0.4.4/pigeon/middleware/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/conversion/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.132956 pigeonpost-0.4.4/pigeon/middleware/conversion/mime/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/conversion/mime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/conversion/mime/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/conversion/mime/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.132956 pigeonpost-0.4.4/pigeon/templating/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/templating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/templating/templater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.136956 pigeonpost-0.4.4/pigeon/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/utils/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3260 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.136956 pigeonpost-0.4.4/pigeonpost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-02 21:57:37.000000 pigeonpost-0.4.4/pigeonpost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-02 21:57:37.000000 pigeonpost-0.4.4/pigeonpost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 21:57:37.000000 pigeonpost-0.4.4/pigeonpost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 21:57:37.000000 pigeonpost-0.4.4/pigeonpost.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 21:57:37.000000 pigeonpost-0.4.4/pigeonpost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 21:57:37.000000 pigeonpost-0.4.4/pigeonpost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-02 21:57:37.136956 pigeonpost-0.4.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.064853 pigeonpost-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 23:58:02.064853 pigeonpost-0.4.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.052853 pigeonpost-0.4.5/pigeon/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.052853 pigeonpost-0.4.5/pigeon/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/conf/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/conf/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/conf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.056853 pigeonpost-0.4.5/pigeon/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/core/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/core/secure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/core/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.056853 pigeonpost-0.4.5/pigeon/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/default/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.056853 pigeonpost-0.4.5/pigeon/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/files/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/files/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.056853 pigeonpost-0.4.5/pigeon/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/http/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/http/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/http/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/http/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.056853 pigeonpost-0.4.5/pigeon/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.060853 pigeonpost-0.4.5/pigeon/middleware/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/cache_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/content_negotiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/mediafiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/components/staticfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.060853 pigeonpost-0.4.5/pigeon/middleware/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/conversion/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.060853 pigeonpost-0.4.5/pigeon/middleware/conversion/mime/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/conversion/mime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/conversion/mime/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/conversion/mime/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/middleware/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.060853 pigeonpost-0.4.5/pigeon/templating/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/templating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/templating/templater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.060853 pigeonpost-0.4.5/pigeon/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/utils/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3260 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/pigeon/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:58:02.064853 pigeonpost-0.4.5/pigeonpost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 23:58:02.000000 pigeonpost-0.4.5/pigeonpost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-02 23:58:02.000000 pigeonpost-0.4.5/pigeonpost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 23:58:02.000000 pigeonpost-0.4.5/pigeonpost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 23:58:02.000000 pigeonpost-0.4.5/pigeonpost.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 23:58:02.000000 pigeonpost-0.4.5/pigeonpost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 23:58:02.000000 pigeonpost-0.4.5/pigeonpost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-02 23:58:02.064853 pigeonpost-0.4.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-05-02 23:57:56.000000 pigeonpost-0.4.5/setup.py
```

### Comparing `pigeonpost-0.4.4/pigeon/conf/manager.py` & `pigeonpost-0.4.5/pigeon/conf/manager.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/conf/settings.py` & `pigeonpost-0.4.5/pigeon/conf/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # VERBOSITY
 VERBOSITY = 2
 
 # ADDRESS
 ADDRESS = ''
 PORT = 8080
 
+# REUSE SOCKET AUTOMATICALLY
+REUSE_SOCKET = True
+
 # ALLOWED HOSTS
 ALLOWED_HOSTS = ['*']
 # ALLOWED METHODS
 ALLOWED_METHODS = ['POST', 'GET', 'HEAD', 'POST', 'PUT', 'OPTIONS']
 
 # ACCESS-CONTROL
 CORS_ALLOWED_ORIGINS = []
```

### Comparing `pigeonpost-0.4.4/pigeon/core/app.py` & `pigeonpost-0.4.5/pigeon/core/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,24 +4,29 @@
 import traceback
 from typing import Callable
 from pigeon.conf import Manager
 import pigeon.core.server as server
 import pigeon.middleware.views as views
 import pigeon.middleware.auth as auth
 import pigeon.utils.logger as logger
+from watchdog.observers import Observer
+from watchdog.events import FileSystemEventHandler
 
 log = logger.Log('PIGEON', '#30b3ff')
 
-
 class Pigeon:
     settings = None
     autorun = True
+
+    # watchdog
+    observers = []
     @classmethod
     def __init__(cls, settings=None):
         log.info('STARTING..')
+
         # overwrite standard settings if new settings provided
         if settings:
             Manager.override(settings)
 
         # view handlers
         Manager.view_handler = views.ViewHandler()
         Manager.error_handler = views.ErrorHandler()
@@ -33,40 +38,66 @@
 
         # configure runtime settings
         Manager._setup()
 
         # exception handling
         sys.excepthook = cls.handle_exception
         sys.exit = cls.handle_exit
-
         # run pigeon after everything has been configured (all decorators executed)
         atexit.register(Pigeon.run)
 
     @classmethod
     def run(cls, auto=False) -> None:
         """
         auto specifies whether the application has been started automatically due to the atexit call,
         if so we will check back whether this
         """
+        if Manager.debug_mode:
+            log.debug('WATCHING MODULES FOR CHANGES: (DEBUG MODE)')
+            for module in Manager.module_dirs:
+                log.sublog(module)
+            log.info('INITIALIZING WATCHDOG CONFIGURATION')
+            event_handler = FileSystemEventHandler()
+
+            def restart_event(event):
+                log.debug(f"FILE EVENT: {event}")
+                cls.restart()
+
+            event_handler.on_modified = restart_event
+            for module in Manager.module_dirs:
+                watchdog_observer = Observer()
+                watchdog_observer.schedule(event_handler, path=module, recursive=False)
+                watchdog_observer.start()
+                cls.observers.append(watchdog_observer)
+
         if not cls.autorun:
             log.verbose("AUTORUN DISABLED - SKIPPING")
             return
+
         cls.autorun = False
 
         log.info('STARTING')
         try:
             # start server
             server.start()
             server.serve()
         except PermissionError as e:
             if e.errno == 13: log.critical("PERMISSION DENIED (PORTS 0-1024 REQUIRE ADMINISTRATIVE PRIVILEGES)")
         except OSError as e:
             if e.errno == 98: log.critical("ADDRESS ALREADY IN USE")
 
     @classmethod
+    def restart(cls):
+        """
+        Restarts the entire application
+        """
+        log.info("RESTARTING THE APPLICATION")
+        os.execl(sys.executable, sys.executable, *sys.argv)
+
+    @classmethod
     def handle_exception(cls, exception_type, exception, *args, custom_log: logger.Log = log, description: str='AN EXCEPTION OCCURED') -> None:
         """
         This is a custom exception handler. It facilitates the following:
         - if an exception occurs before the server has started, the server will not start
         - exceptions during runtime will be logged and if the CRASH_ON_FAILURE setting is set to True the app will terminate
         """
         sys.last_exc = exception
```

### Comparing `pigeonpost-0.4.4/pigeon/core/handler.py` & `pigeonpost-0.4.5/pigeon/core/handler.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/core/secure.py` & `pigeonpost-0.4.5/pigeon/core/secure.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/core/server.py` & `pigeonpost-0.4.5/pigeon/core/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 
 
 def serve():
     log.info(f'ADDRESS: {Manager.address if Manager.address else "ANY"}')
     log.info(f'PORT: {Manager.port}')
 
     # open socket
-    sock = socket.socket(socket.AF_INET)
+    sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+    if Manager.reuse_socket:
+        sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
     sock.setblocking(False)
     sock.bind((Manager.address, Manager.port))
 
     # configure https if specified in settings
     if Manager.use_https:
         log.verbose('USING HTTPS')
         secure_sock = secure.make_secure(sock, Manager.certificate_path, Manager.private_key_path, Manager.private_key_passwd)
```

### Comparing `pigeonpost-0.4.4/pigeon/default/errors.py` & `pigeonpost-0.4.5/pigeon/default/errors.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/files/media.py` & `pigeonpost-0.4.5/pigeon/files/media.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/files/static.py` & `pigeonpost-0.4.5/pigeon/files/static.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/http/message.py` & `pigeonpost-0.4.5/pigeon/http/message.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/http/request.py` & `pigeonpost-0.4.5/pigeon/http/request.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/http/response.py` & `pigeonpost-0.4.5/pigeon/http/response.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/middleware/auth.py` & `pigeonpost-0.4.5/pigeon/middleware/auth.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/middleware/components/__init__.py` & `pigeonpost-0.4.5/pigeon/middleware/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/middleware/components/cache_control.py` & `pigeonpost-0.4.5/pigeon/middleware/components/cache_control.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/middleware/components/component.py` & `pigeonpost-0.4.5/pigeon/middleware/components/component.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/middleware/components/connection.py` & `pigeonpost-0.4.5/pigeon/middleware/components/connection.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/middleware/components/content_negotiation.py` & `pigeonpost-0.4.5/pigeon/middleware/components/content_negotiation.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/middleware/components/cors.py` & `pigeonpost-0.4.5/pigeon/middleware/components/cors.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/middleware/components/host.py` & `pigeonpost-0.4.5/pigeon/middleware/components/host.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/middleware/components/mediafiles.py` & `pigeonpost-0.4.5/pigeon/middleware/components/mediafiles.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/middleware/components/method.py` & `pigeonpost-0.4.5/pigeon/middleware/components/method.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/middleware/components/staticfiles.py` & `pigeonpost-0.4.5/pigeon/middleware/components/staticfiles.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/middleware/conversion/converter.py` & `pigeonpost-0.4.5/pigeon/middleware/conversion/converter.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/middleware/conversion/mime/parsers.py` & `pigeonpost-0.4.5/pigeon/middleware/conversion/mime/parsers.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/middleware/pipe.py` & `pigeonpost-0.4.5/pigeon/middleware/pipe.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/middleware/processing.py` & `pigeonpost-0.4.5/pigeon/middleware/processing.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/middleware/tags.py` & `pigeonpost-0.4.5/pigeon/middleware/tags.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/middleware/views.py` & `pigeonpost-0.4.5/pigeon/middleware/views.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/templating/templater.py` & `pigeonpost-0.4.5/pigeon/templating/templater.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/utils/common.py` & `pigeonpost-0.4.5/pigeon/utils/common.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeon/utils/logger.py` & `pigeonpost-0.4.5/pigeon/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.4/pigeonpost.egg-info/SOURCES.txt` & `pigeonpost-0.4.5/pigeonpost.egg-info/SOURCES.txt`

 * *Files identical despite different names*


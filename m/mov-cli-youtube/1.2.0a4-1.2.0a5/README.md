# Comparing `tmp/mov_cli_youtube-1.2.0a4.tar.gz` & `tmp/mov_cli_youtube-1.2.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli_youtube-1.2.0a4.tar", last modified: Fri Apr 26 01:05:44 2024, max compression
+gzip compressed data, was "mov_cli_youtube-1.2.0a5.tar", last modified: Fri Apr 26 11:28:55 2024, max compression
```

## Comparing `mov_cli_youtube-1.2.0a4.tar` & `mov_cli_youtube-1.2.0a5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 01:05:44.834520 mov_cli_youtube-1.2.0a4/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:22:29.000000 mov_cli_youtube-1.2.0a4/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2990 2024-04-26 01:05:44.834520 mov_cli_youtube-1.2.0a4/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      674 2024-03-21 15:27:20.000000 mov_cli_youtube-1.2.0a4/README.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 01:05:44.834520 mov_cli_youtube-1.2.0a4/mov_cli_youtube/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      656 2024-04-26 00:59:40.000000 mov_cli_youtube-1.2.0a4/mov_cli_youtube/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2526 2024-04-26 00:35:08.000000 mov_cli_youtube-1.2.0a4/mov_cli_youtube/pytube.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3765 2024-04-26 01:01:35.000000 mov_cli_youtube-1.2.0a4/mov_cli_youtube/yt_dlp.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 01:05:44.834520 mov_cli_youtube-1.2.0a4/mov_cli_youtube.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2990 2024-04-26 01:05:44.000000 mov_cli_youtube-1.2.0a4/mov_cli_youtube.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      306 2024-04-26 01:05:44.000000 mov_cli_youtube-1.2.0a4/mov_cli_youtube.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-26 01:05:44.000000 mov_cli_youtube-1.2.0a4/mov_cli_youtube.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       97 2024-04-26 01:05:44.000000 mov_cli_youtube-1.2.0a4/mov_cli_youtube.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       16 2024-04-26 01:05:44.000000 mov_cli_youtube-1.2.0a4/mov_cli_youtube.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1295 2024-04-26 00:34:40.000000 mov_cli_youtube-1.2.0a4/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-26 01:05:44.834520 mov_cli_youtube-1.2.0a4/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 11:28:55.274617 mov_cli_youtube-1.2.0a5/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:22:29.000000 mov_cli_youtube-1.2.0a5/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2990 2024-04-26 11:28:55.274617 mov_cli_youtube-1.2.0a5/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      674 2024-03-21 15:27:20.000000 mov_cli_youtube-1.2.0a5/README.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 11:28:55.271284 mov_cli_youtube-1.2.0a5/mov_cli_youtube/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      656 2024-04-26 11:28:36.000000 mov_cli_youtube-1.2.0a5/mov_cli_youtube/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2460 2024-04-26 11:27:05.000000 mov_cli_youtube-1.2.0a5/mov_cli_youtube/pytube.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3765 2024-04-26 11:27:25.000000 mov_cli_youtube-1.2.0a5/mov_cli_youtube/yt_dlp.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 11:28:55.274617 mov_cli_youtube-1.2.0a5/mov_cli_youtube.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2990 2024-04-26 11:28:55.000000 mov_cli_youtube-1.2.0a5/mov_cli_youtube.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      306 2024-04-26 11:28:55.000000 mov_cli_youtube-1.2.0a5/mov_cli_youtube.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-26 11:28:55.000000 mov_cli_youtube-1.2.0a5/mov_cli_youtube.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       97 2024-04-26 11:28:55.000000 mov_cli_youtube-1.2.0a5/mov_cli_youtube.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       16 2024-04-26 11:28:55.000000 mov_cli_youtube-1.2.0a5/mov_cli_youtube.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1295 2024-04-26 00:34:40.000000 mov_cli_youtube-1.2.0a5/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-26 11:28:55.274617 mov_cli_youtube-1.2.0a5/setup.cfg
```

### Comparing `mov_cli_youtube-1.2.0a4/LICENSE` & `mov_cli_youtube-1.2.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli_youtube-1.2.0a4/PKG-INFO` & `mov_cli_youtube-1.2.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-youtube
-Version: 1.2.0a4
+Version: 1.2.0a5
 Summary: A mov-cli v4 plugin for watching youtube.
 Author-email: Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mov_cli_youtube-1.2.0a4/README.md` & `mov_cli_youtube-1.2.0a5/README.md`

 * *Files identical despite different names*

### Comparing `mov_cli_youtube-1.2.0a4/mov_cli_youtube/__init__.py` & `mov_cli_youtube-1.2.0a5/mov_cli_youtube/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
         "IOS.DEFAULT": PyTubeScraper, 
 
         "yt-dlp": YTDlpScraper, 
         "pytube": PyTubeScraper, 
     }
 }
 
-__version__ = "1.2.0alpha4"
+__version__ = "1.2.0alpha5"
```

### Comparing `mov_cli_youtube-1.2.0a4/mov_cli_youtube/pytube.py` & `mov_cli_youtube-1.2.0a5/mov_cli_youtube/pytube.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,18 +54,18 @@
         if audio_only:
             url = video.streams.get_audio_only().url
 
         elif self.config.resolution is not None:
             url = video.streams.get_by_resolution(f"{self.config.resolution}p").url
 
             if url is None:
-                url = video.streams.filter(progressive = False).order_by("resolution").last().url
+                url = video.streams.get_highest_resolution().url
 
         else:
-            url = video.streams.filter(progressive = False).order_by("resolution").last().url
+            url = video.streams.get_highest_resolution().url
 
         return Single(
             url = url, 
             title = metadata.title, 
             year = metadata.year
         )
```

### Comparing `mov_cli_youtube-1.2.0a4/mov_cli_youtube/yt_dlp.py` & `mov_cli_youtube-1.2.0a5/mov_cli_youtube/yt_dlp.py`

 * *Files identical despite different names*

### Comparing `mov_cli_youtube-1.2.0a4/mov_cli_youtube.egg-info/PKG-INFO` & `mov_cli_youtube-1.2.0a5/mov_cli_youtube.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-youtube
-Version: 1.2.0a4
+Version: 1.2.0a5
 Summary: A mov-cli v4 plugin for watching youtube.
 Author-email: Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mov_cli_youtube-1.2.0a4/pyproject.toml` & `mov_cli_youtube-1.2.0a5/pyproject.toml`

 * *Files identical despite different names*


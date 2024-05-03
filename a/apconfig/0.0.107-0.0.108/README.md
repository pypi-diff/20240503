# Comparing `tmp/apconfig-0.0.107.tar.gz` & `tmp/apconfig-0.0.108.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apconfig-0.0.107.tar", max compression
+gzip compressed data, was "apconfig-0.0.108.tar", max compression
```

## Comparing `apconfig-0.0.107.tar` & `apconfig-0.0.108.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-03-27 10:34:40.761324 apconfig-0.0.107/README.md
--rw-r--r--   0        0        0     3214 2024-04-24 10:30:10.717114 apconfig-0.0.107/apconfig/__init__.py
--rw-r--r--   0        0        0      114 2024-04-05 10:57:51.982200 apconfig-0.0.107/apconfig/utilities.py
--rw-r--r--   0        0        0      305 2024-04-24 10:33:04.202613 apconfig-0.0.107/pyproject.toml
--rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 apconfig-0.0.107/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-27 10:34:40.761324 apconfig-0.0.108/README.md
+-rw-r--r--   0        0        0     3251 2024-05-03 12:52:16.604678 apconfig-0.0.108/apconfig/__init__.py
+-rw-r--r--   0        0        0      114 2024-04-05 10:57:51.982200 apconfig-0.0.108/apconfig/utilities.py
+-rw-r--r--   0        0        0      305 2024-05-03 13:15:12.822453 apconfig-0.0.108/pyproject.toml
+-rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 apconfig-0.0.108/PKG-INFO
```

### Comparing `apconfig-0.0.107/apconfig/__init__.py` & `apconfig-0.0.108/apconfig/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         raise
 
 
 setup_data = get_api_setup_data()
 
 # TSO Configuration
 chains = ['coston', 'coston2', 'songbird', 'flare']
+active_chains = setup_data["chains"]
 
 # Data Service Streamers and APIs
 WS = 'ws://'
 WSS = 'wss://'
 HTTP = 'http://'
 HTTPS = 'https://'
```


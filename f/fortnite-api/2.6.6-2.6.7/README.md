# Comparing `tmp/fortnite_api-2.6.6.tar.gz` & `tmp/fortnite_api-2.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortnite_api-2.6.6.tar", last modified: Thu Apr 18 07:52:51 2024, max compression
+gzip compressed data, was "fortnite_api-2.6.7.tar", last modified: Fri May  3 19:48:07 2024, max compression
```

## Comparing `fortnite_api-2.6.6.tar` & `fortnite_api-2.6.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:52:51.144000 fortnite_api-2.6.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-18 07:52:48.000000 fortnite_api-2.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-04-18 07:52:51.144000 fortnite_api-2.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-04-18 07:52:48.000000 fortnite_api-2.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:52:51.144000 fortnite_api-2.6.6/fortnite_api/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-18 07:52:48.000000 fortnite_api-2.6.6/fortnite_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-18 07:52:48.000000 fortnite_api-2.6.6/fortnite_api/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-18 07:52:48.000000 fortnite_api-2.6.6/fortnite_api/aes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-18 07:52:48.000000 fortnite_api-2.6.6/fortnite_api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-18 07:52:48.000000 fortnite_api-2.6.6/fortnite_api/banner.py
--rw-r--r--   0 runner    (1001) docker     (127)    17888 2024-04-18 07:52:48.000000 fortnite_api-2.6.6/fortnite_api/cosmetics.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-18 07:52:48.000000 fortnite_api-2.6.6/fortnite_api/creator_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    23263 2024-04-18 07:52:48.000000 fortnite_api-2.6.6/fortnite_api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-18 07:52:48.000000 fortnite_api-2.6.6/fortnite_api/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-18 07:52:48.000000 fortnite_api-2.6.6/fortnite_api/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-18 07:52:48.000000 fortnite_api-2.6.6/fortnite_api/http.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-18 07:52:48.000000 fortnite_api-2.6.6/fortnite_api/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-18 07:52:48.000000 fortnite_api-2.6.6/fortnite_api/news.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-18 07:52:48.000000 fortnite_api-2.6.6/fortnite_api/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-04-18 07:52:48.000000 fortnite_api-2.6.6/fortnite_api/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-18 07:52:48.000000 fortnite_api-2.6.6/fortnite_api/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:52:51.144000 fortnite_api-2.6.6/fortnite_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-04-18 07:52:51.000000 fortnite_api-2.6.6/fortnite_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-18 07:52:51.000000 fortnite_api-2.6.6/fortnite_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 07:52:51.000000 fortnite_api-2.6.6/fortnite_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-18 07:52:51.000000 fortnite_api-2.6.6/fortnite_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 07:52:51.000000 fortnite_api-2.6.6/fortnite_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-18 07:52:51.144000 fortnite_api-2.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-18 07:52:48.000000 fortnite_api-2.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:48:07.943653 fortnite_api-2.6.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-03 19:48:05.000000 fortnite_api-2.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-05-03 19:48:07.943653 fortnite_api-2.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-05-03 19:48:05.000000 fortnite_api-2.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:48:07.943653 fortnite_api-2.6.7/fortnite_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-03 19:48:05.000000 fortnite_api-2.6.7/fortnite_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-03 19:48:05.000000 fortnite_api-2.6.7/fortnite_api/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-03 19:48:05.000000 fortnite_api-2.6.7/fortnite_api/aes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-03 19:48:05.000000 fortnite_api-2.6.7/fortnite_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-03 19:48:05.000000 fortnite_api-2.6.7/fortnite_api/banner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17888 2024-05-03 19:48:05.000000 fortnite_api-2.6.7/fortnite_api/cosmetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-03 19:48:05.000000 fortnite_api-2.6.7/fortnite_api/creator_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23263 2024-05-03 19:48:05.000000 fortnite_api-2.6.7/fortnite_api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-03 19:48:05.000000 fortnite_api-2.6.7/fortnite_api/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-03 19:48:05.000000 fortnite_api-2.6.7/fortnite_api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-03 19:48:05.000000 fortnite_api-2.6.7/fortnite_api/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-03 19:48:05.000000 fortnite_api-2.6.7/fortnite_api/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-03 19:48:05.000000 fortnite_api-2.6.7/fortnite_api/news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-03 19:48:05.000000 fortnite_api-2.6.7/fortnite_api/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-05-03 19:48:05.000000 fortnite_api-2.6.7/fortnite_api/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-03 19:48:05.000000 fortnite_api-2.6.7/fortnite_api/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:48:07.943653 fortnite_api-2.6.7/fortnite_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-05-03 19:48:07.000000 fortnite_api-2.6.7/fortnite_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-03 19:48:07.000000 fortnite_api-2.6.7/fortnite_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:48:07.000000 fortnite_api-2.6.7/fortnite_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 19:48:07.000000 fortnite_api-2.6.7/fortnite_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 19:48:07.000000 fortnite_api-2.6.7/fortnite_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-03 19:48:07.943653 fortnite_api-2.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-03 19:48:05.000000 fortnite_api-2.6.7/setup.py
```

### Comparing `fortnite_api-2.6.6/LICENSE` & `fortnite_api-2.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fortnite_api-2.6.6/PKG-INFO` & `fortnite_api-2.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fortnite-api
-Version: 2.6.6
+Version: 2.6.7
 Summary: A python wrapper for Fortnite-API.com
 Home-page: https://github.com/Fortnite-API/py-wrapper
-Download-URL: https://github.com/Fortnite-API/py-wrapper/archive/refs/tags/v2.6.6.tar.gz
+Download-URL: https://github.com/Fortnite-API/py-wrapper/archive/refs/tags/v2.6.7.tar.gz
 Author: Luc1412
 Author-email: Luc1412.lh@gmail.com
 License: MIT
 Project-URL: Issue tracker, https://github.com/Fortnite-API/py-wrapper/issues
 Project-URL: Code, https://github.com/Fortnite-API/py-wrapper
 Keywords: fortnite,fortnite-api.com,shop,cosmetics,fortnite api,fortnite shop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fortnite_api-2.6.6/README.md` & `fortnite_api-2.6.7/README.md`

 * *Files identical despite different names*

### Comparing `fortnite_api-2.6.6/fortnite_api/account.py` & `fortnite_api-2.6.7/fortnite_api/account.py`

 * *Files identical despite different names*

### Comparing `fortnite_api-2.6.6/fortnite_api/aes.py` & `fortnite_api-2.6.7/fortnite_api/aes.py`

 * *Files identical despite different names*

### Comparing `fortnite_api-2.6.6/fortnite_api/api.py` & `fortnite_api-2.6.7/fortnite_api/api.py`

 * *Files identical despite different names*

### Comparing `fortnite_api-2.6.6/fortnite_api/banner.py` & `fortnite_api-2.6.7/fortnite_api/banner.py`

 * *Files identical despite different names*

### Comparing `fortnite_api-2.6.6/fortnite_api/cosmetics.py` & `fortnite_api-2.6.7/fortnite_api/cosmetics.py`

 * *Files identical despite different names*

### Comparing `fortnite_api-2.6.6/fortnite_api/creator_code.py` & `fortnite_api-2.6.7/fortnite_api/creator_code.py`

 * *Files identical despite different names*

### Comparing `fortnite_api-2.6.6/fortnite_api/endpoints.py` & `fortnite_api-2.6.7/fortnite_api/endpoints.py`

 * *Files identical despite different names*

### Comparing `fortnite_api-2.6.6/fortnite_api/enums.py` & `fortnite_api-2.6.7/fortnite_api/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -119,14 +119,16 @@
 
 
 class ShopTileSize(Enum):
     SMALL = 'Size_1_x_1'
     NORMAL = 'Size_1_x_2'
     DOUBLE_WIDE = 'Size_2_x_2'
     TRIPLE_WIDE = 'Size_3_x_2'
+    QUAD_WIDE = 'Size_4_x_2'
+    PENTA_WIDE = 'Size_5_x_2'
 
 
 class CosmeticCompatibleMode(Enum):
     BATTLE_ROYALE = 'ECosmeticCompatibleMode::BattleRoyale'
     LEGO = 'ECosmeticCompatibleMode::Juno'
     ROCKET_RACING = 'ECosmeticCompatibleMode::DelMar'
     FESTIVAL = 'ECosmeticCompatibleMode::Sparks'
```

### Comparing `fortnite_api-2.6.6/fortnite_api/http.py` & `fortnite_api-2.6.7/fortnite_api/http.py`

 * *Files identical despite different names*

### Comparing `fortnite_api-2.6.6/fortnite_api/map.py` & `fortnite_api-2.6.7/fortnite_api/map.py`

 * *Files identical despite different names*

### Comparing `fortnite_api-2.6.6/fortnite_api/news.py` & `fortnite_api-2.6.7/fortnite_api/news.py`

 * *Files identical despite different names*

### Comparing `fortnite_api-2.6.6/fortnite_api/playlist.py` & `fortnite_api-2.6.7/fortnite_api/playlist.py`

 * *Files identical despite different names*

### Comparing `fortnite_api-2.6.6/fortnite_api/shop.py` & `fortnite_api-2.6.7/fortnite_api/shop.py`

 * *Files identical despite different names*

### Comparing `fortnite_api-2.6.6/fortnite_api/stats.py` & `fortnite_api-2.6.7/fortnite_api/stats.py`

 * *Files identical despite different names*

### Comparing `fortnite_api-2.6.6/fortnite_api.egg-info/PKG-INFO` & `fortnite_api-2.6.7/fortnite_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fortnite-api
-Version: 2.6.6
+Version: 2.6.7
 Summary: A python wrapper for Fortnite-API.com
 Home-page: https://github.com/Fortnite-API/py-wrapper
-Download-URL: https://github.com/Fortnite-API/py-wrapper/archive/refs/tags/v2.6.6.tar.gz
+Download-URL: https://github.com/Fortnite-API/py-wrapper/archive/refs/tags/v2.6.7.tar.gz
 Author: Luc1412
 Author-email: Luc1412.lh@gmail.com
 License: MIT
 Project-URL: Issue tracker, https://github.com/Fortnite-API/py-wrapper/issues
 Project-URL: Code, https://github.com/Fortnite-API/py-wrapper
 Keywords: fortnite,fortnite-api.com,shop,cosmetics,fortnite api,fortnite shop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fortnite_api-2.6.6/fortnite_api.egg-info/SOURCES.txt` & `fortnite_api-2.6.7/fortnite_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fortnite_api-2.6.6/setup.py` & `fortnite_api-2.6.7/setup.py`

 * *Files identical despite different names*


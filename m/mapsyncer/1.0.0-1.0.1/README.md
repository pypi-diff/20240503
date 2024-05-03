# Comparing `tmp/mapsyncer-1.0.0.tar.gz` & `tmp/mapsyncer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapsyncer-1.0.0.tar", last modified: Fri Apr 19 14:15:52 2024, max compression
+gzip compressed data, was "mapsyncer-1.0.1.tar", last modified: Fri May  3 06:53:22 2024, max compression
```

## Comparing `mapsyncer-1.0.0.tar` & `mapsyncer-1.0.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:52.801068 mapsyncer-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:52.793069 mapsyncer-1.0.0/MapSyncer/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13151 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:52.797068 mapsyncer-1.0.0/MapSyncer/components/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/common_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    10417 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/download.py
--rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/get_exif.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/osc_api_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    19217 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/osc_api_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/osc_api_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:52.797068 mapsyncer-1.0.0/MapSyncer/components/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/parsers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:52.797068 mapsyncer-1.0.0/MapSyncer/components/parsers/exif/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/parsers/exif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15285 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/parsers/exif/exif.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/parsers/exif/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:52.797068 mapsyncer-1.0.0/MapSyncer/components/parsers/osc_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/parsers/osc_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/parsers/osc_metadata/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/version_.py
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:52.801068 mapsyncer-1.0.0/MapSyncer/static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17051 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/static/app.js
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/static/edit-sequence.js
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/static/global.js
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/static/mapilio_fav.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:52.801068 mapsyncer-1.0.0/MapSyncer/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/templates/details.html
--rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/templates/display-sequence.html
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/templates/kartaview-login.html
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/templates/mapilio-login.html
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/templates/sequence-edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-19 14:15:52.801068 mapsyncer-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:52.801068 mapsyncer-1.0.0/mapsyncer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-19 14:15:52.000000 mapsyncer-1.0.0/mapsyncer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-19 14:15:52.000000 mapsyncer-1.0.0/mapsyncer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:15:52.000000 mapsyncer-1.0.0/mapsyncer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-19 14:15:52.000000 mapsyncer-1.0.0/mapsyncer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-19 14:15:52.000000 mapsyncer-1.0.0/mapsyncer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 14:15:52.000000 mapsyncer-1.0.0/mapsyncer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:15:52.801068 mapsyncer-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:53:22.584101 mapsyncer-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:53:22.576100 mapsyncer-1.0.1/MapSyncer/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13215 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:53:22.580100 mapsyncer-1.0.1/MapSyncer/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/components/common_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/components/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10417 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/components/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/components/get_exif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/components/osc_api_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19440 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/components/osc_api_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/components/osc_api_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:53:22.580100 mapsyncer-1.0.1/MapSyncer/components/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/components/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/components/parsers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:53:22.580100 mapsyncer-1.0.1/MapSyncer/components/parsers/exif/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/components/parsers/exif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15285 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/components/parsers/exif/exif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/components/parsers/exif/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:53:22.580100 mapsyncer-1.0.1/MapSyncer/components/parsers/osc_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/components/parsers/osc_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/components/parsers/osc_metadata/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/components/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/components/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/components/version_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:53:22.580100 mapsyncer-1.0.1/MapSyncer/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17051 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/static/app.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/static/edit-sequence.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/static/global.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/static/mapilio_fav.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:53:22.580100 mapsyncer-1.0.1/MapSyncer/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/templates/details.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/templates/display-sequence.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/templates/kartaview-login.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/templates/mapilio-login.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/MapSyncer/templates/sequence-edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-03 06:53:22.584101 mapsyncer-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:53:22.584101 mapsyncer-1.0.1/mapsyncer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-03 06:53:22.000000 mapsyncer-1.0.1/mapsyncer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-03 06:53:22.000000 mapsyncer-1.0.1/mapsyncer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 06:53:22.000000 mapsyncer-1.0.1/mapsyncer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-03 06:53:22.000000 mapsyncer-1.0.1/mapsyncer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-03 06:53:22.000000 mapsyncer-1.0.1/mapsyncer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 06:53:22.000000 mapsyncer-1.0.1/mapsyncer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 06:53:22.584101 mapsyncer-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-03 06:52:59.000000 mapsyncer-1.0.1/setup.py
```

### Comparing `mapsyncer-1.0.0/LICENSE` & `mapsyncer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/MapSyncer/app.py` & `mapsyncer-1.0.1/MapSyncer/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import math
 import os
 import shutil
 import ssl
+import webbrowser
 
 from flask import Flask, render_template, request, jsonify, redirect, url_for, session
 from mapilio_kit.base import authenticator
 from mapilio_kit.components.edit_config import edit_config
 from mapilio_kit.components.login import list_all_users
 from osm_login_python.core import Auth
 
@@ -363,12 +364,12 @@
 
     return jsonify(success=True), 200
 
 
 def main():
     ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
     ssl_context.load_cert_chain(CERT_PEM, KEY_PEM)
-    app.run(host='0.0.0.0', port=5050, threaded=True, debug=True, ssl_context=ssl_context)
-
+    webbrowser.open('https://127.0.0.1:5050')
+    app.run(host='0.0.0.0', port=5050, threaded=True, debug=False, ssl_context=ssl_context)
 
 if __name__ == '__main__':
     main()
```

### Comparing `mapsyncer-1.0.0/MapSyncer/components/common_models.py` & `mapsyncer-1.0.1/MapSyncer/components/common_models.py`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/MapSyncer/components/download.py` & `mapsyncer-1.0.1/MapSyncer/components/download.py`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/MapSyncer/components/get_exif.py` & `mapsyncer-1.0.1/MapSyncer/components/get_exif.py`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/MapSyncer/components/osc_api_gateway.py` & `mapsyncer-1.0.1/MapSyncer/components/osc_api_gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,15 +341,18 @@
                                           data=parameters).json()
             merged_json_response.update({'0': json_response})
 
         except requests.RequestException as ex:
             return None, ex
 
         if 'totalFilteredItems' not in json_response:
-            return [], Exception("OSC API bug missing totalFilteredItems from response")
+            api_message = json_response.get('status', {}).get('apiMessage', 'Unknown Error')
+            if api_message == "Invalid username!":
+                return [], Exception("No Kartaview account associated with OpenStreetMap was found.")
+            return [], Exception(f"OSC API error: {api_message}")
 
         total_items = int(json_response['totalFilteredItems'][0])
         pages_count = int(total_items / parameters['ipp']) + 1
         print(
             f"{Fore.BLUE}Total count of images: {Fore.LIGHTBLUE_EX}{total_items}{Fore.RESET}{Fore.BLUE} Total count of pages: {Fore.LIGHTBLUE_EX}{pages_count}")
 
         sequences = []
```

### Comparing `mapsyncer-1.0.0/MapSyncer/components/osc_api_models.py` & `mapsyncer-1.0.1/MapSyncer/components/osc_api_models.py`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/MapSyncer/components/parsers/base.py` & `mapsyncer-1.0.1/MapSyncer/components/parsers/base.py`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/MapSyncer/components/parsers/exif/exif.py` & `mapsyncer-1.0.1/MapSyncer/components/parsers/exif/exif.py`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/MapSyncer/components/parsers/exif/utils.py` & `mapsyncer-1.0.1/MapSyncer/components/parsers/exif/utils.py`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/MapSyncer/components/parsers/osc_metadata/parser.py` & `mapsyncer-1.0.1/MapSyncer/components/parsers/osc_metadata/parser.py`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/MapSyncer/components/ssl.py` & `mapsyncer-1.0.1/MapSyncer/components/ssl.py`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/MapSyncer/components/storage.py` & `mapsyncer-1.0.1/MapSyncer/components/storage.py`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/MapSyncer/run.py` & `mapsyncer-1.0.1/MapSyncer/run.py`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/MapSyncer/static/app.js` & `mapsyncer-1.0.1/MapSyncer/static/app.js`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/MapSyncer/static/edit-sequence.js` & `mapsyncer-1.0.1/MapSyncer/static/edit-sequence.js`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/MapSyncer/static/global.js` & `mapsyncer-1.0.1/MapSyncer/static/global.js`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/MapSyncer/static/mapilio_fav.png` & `mapsyncer-1.0.1/MapSyncer/static/mapilio_fav.png`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/MapSyncer/templates/details.html` & `mapsyncer-1.0.1/MapSyncer/templates/details.html`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/MapSyncer/templates/display-sequence.html` & `mapsyncer-1.0.1/MapSyncer/templates/display-sequence.html`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
         }
 
         .card-text {
             overflow: hidden;
             text-overflow: ellipsis;
             white-space: nowrap;
         }
-
     </style>
 </head>
 <body>
     <div class="container">
         <nav class="navbar navbar-expand-lg navbar-dark bg-primary mt-4 rounded-4">
             <a class="navbar-brand mx-4" href="#">MapSyncer</a>
             <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarToggleExternalContent" aria-controls="navbarToggleExternalContent" aria-expanded="false" aria-label="Toggle navigation">
@@ -175,28 +174,32 @@
                                 {% endif %}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
             {% endfor %}
-            <div class="alert alert-warning alert-dismissible fade show mt-4" role="alert" id="info-message-missing">
-                <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button><p>If you think your sequences are missing, please <a href="#" id="clickHere" class="text-decoration-none">click here</a>.</p></button>
-            </div>
+            {% if not sequence_data %}
+                <div class="col-12 text-center mt-4">
+                    <div class="alert alert-warning" role="alert">
+                        No sequence to fetch was found in your KartaView account.
+                    </div>
+                </div>
+            {% endif %}
         </div>
         {% endif %}
     </div>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
     <script src="{{ url_for('static', filename='global.js') }}"></script>
     <script src="{{ url_for('static', filename='app.js') }}"></script>
     <script>
         var user_name = "{{ user_name }}";
         if (user_name === "None" || user_name === null || user_name === "") {
             window.location.href = "/";
         } else {
             localStorage.setItem('user_name', user_name);
         }
-      </script>
+    </script>
     <link href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.3/css/bootstrap.min.css" rel="stylesheet">
     <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.3/js/bootstrap.bundle.min.js"></script>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -35,10 +35,11 @@
 {% for item in sequence_data %}
 NNuummbbeerr:: {{{{ ((ccuurrrreenntt__ppaaggee -- 11)) ** iitteemmss__ppeerr__ppaaggee ++ lloooopp..iinnddeexx }}}}
 SSeeqquueennccee IIDD:: {{ item.id }}
 
 LLooccaattiioonn:: {{ item.location }}
 {% if item.download_disabled %} Downloaded {% if item.upload_disabled %}
 Uploaded {% else %} Upload {% endif %} {% else %} Download Upload {% endif %}
-{% endfor %}
-If you think your sequences are missing, please _c_l_i_c_k_ _h_e_r_e.
+{% endfor %} {% if not sequence_data %}
+No sequence to fetch was found in your KartaView account.
+{% endif %}
 {% endif %}
```

### Comparing `mapsyncer-1.0.0/MapSyncer/templates/kartaview-login.html` & `mapsyncer-1.0.1/MapSyncer/templates/kartaview-login.html`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/MapSyncer/templates/mapilio-login.html` & `mapsyncer-1.0.1/MapSyncer/templates/mapilio-login.html`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/MapSyncer/templates/sequence-edit.html` & `mapsyncer-1.0.1/MapSyncer/templates/sequence-edit.html`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/PKG-INFO` & `mapsyncer-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapsyncer
-Version: 1.0.0
+Version: 1.0.1
 Summary: A toolkit to download and upload the data from KartaView to Mapilio
 Home-page: https://github.com/mapilio/MapSyncer
 Author: Mapilio
 License: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -69,15 +69,15 @@
 
 * [Mapilio Kit](https://github.com/mapilio/mapilio-kit) `In case you would like to follow the manual way you should install mapilio-kit manually.`
 * [Exiftool](https://exiftool.org/install.html)
 
 
 ## Pip Installation and Usage
 
-You may simply install and use the MapSyncer by using these commands below;
+<b>Note:</b> To install MapSyncer, you'll need to have Python and Pip installed on your system. Ensure you have Python version above <b>3.6</b> but below <b>3.12</b>. If you meet these criteria, please run the following commands:
 
 ```bash
 # Installation
 pip install mapsyncer
 
 # CLI Usage
 RunMapSyncer
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mapsyncer Version: 1.0.0 Summary: A toolkit to
+Metadata-Version: 2.1 Name: mapsyncer Version: 1.0.1 Summary: A toolkit to
 download and upload the data from KartaView to Mapilio Home-page: https://
 github.com/mapilio/MapSyncer Author: Mapilio License: MIT License Requires-
 Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: mapilio-kit Requires-Dist: ExifRead Requires-Dist: calculation-
 mapilio==0.1.39 Requires-Dist: requests_oauthlib Requires-Dist: imagesize
 Requires-Dist: setuptools Requires-Dist: psutil Requires-Dist: flask Requires-
 Dist: python-dotenv Requires-Dist: osm-login-python
@@ -18,17 +18,19 @@
 You can select specific sequences or all downloaded sequences that you want to
 upload to Mapilio. 6. And the process ends successfully. Don't worry, the
 RunMapSyncer command will check and do all these operations. ð« ## Install
 dependencies MapSyncer depends on the following libraries that need to be
 installed before building it.
 * [Mapilio Kit](https://github.com/mapilio/mapilio-kit) `In case you would like
 to follow the manual way you should install mapilio-kit manually.` * [Exiftool]
-(https://exiftool.org/install.html) ## Pip Installation and Usage You may
-simply install and use the MapSyncer by using these commands below; ```bash #
-Installation pip install mapsyncer # CLI Usage RunMapSyncer ```
+(https://exiftool.org/install.html) ## Pip Installation and Usage NNoottee:: To
+install MapSyncer, you'll need to have Python and Pip installed on your system.
+Ensure you have Python version above 33..66 but below 33..1122. If you meet these
+criteria, please run the following commands: ```bash # Installation pip install
+mapsyncer # CLI Usage RunMapSyncer ```
 When accessing the provided address, you may encounter a security warning
 stating ""YYoouurr ccoonnnneeccttiioonn iiss nnoott pprriivvaattee"" in your web browser. To proceed,
 please click the ""AAddvvaanncceedd"" button and select the option to continue to the
 site. This warning is due to the SSL certificate currently being in the process
 of approval and will be validated shortly.
 ## Manual Installation 1. Clone the **MapSyncer** repository: ```bash git clone
 https://github.com/mapilio/MapSyncer.git cd MapSyncer ``` 2. Create Virtualenv
```

### Comparing `mapsyncer-1.0.0/README.md` & `mapsyncer-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 * [Mapilio Kit](https://github.com/mapilio/mapilio-kit) `In case you would like to follow the manual way you should install mapilio-kit manually.`
 * [Exiftool](https://exiftool.org/install.html)
 
 
 ## Pip Installation and Usage
 
-You may simply install and use the MapSyncer by using these commands below;
+<b>Note:</b> To install MapSyncer, you'll need to have Python and Pip installed on your system. Ensure you have Python version above <b>3.6</b> but below <b>3.12</b>. If you meet these criteria, please run the following commands:
 
 ```bash
 # Installation
 pip install mapsyncer
 
 # CLI Usage
 RunMapSyncer
```

#### html2text {}

```diff
@@ -10,17 +10,19 @@
 You can select specific sequences or all downloaded sequences that you want to
 upload to Mapilio. 6. And the process ends successfully. Don't worry, the
 RunMapSyncer command will check and do all these operations. ð« ## Install
 dependencies MapSyncer depends on the following libraries that need to be
 installed before building it.
 * [Mapilio Kit](https://github.com/mapilio/mapilio-kit) `In case you would like
 to follow the manual way you should install mapilio-kit manually.` * [Exiftool]
-(https://exiftool.org/install.html) ## Pip Installation and Usage You may
-simply install and use the MapSyncer by using these commands below; ```bash #
-Installation pip install mapsyncer # CLI Usage RunMapSyncer ```
+(https://exiftool.org/install.html) ## Pip Installation and Usage NNoottee:: To
+install MapSyncer, you'll need to have Python and Pip installed on your system.
+Ensure you have Python version above 33..66 but below 33..1122. If you meet these
+criteria, please run the following commands: ```bash # Installation pip install
+mapsyncer # CLI Usage RunMapSyncer ```
 When accessing the provided address, you may encounter a security warning
 stating ""YYoouurr ccoonnnneeccttiioonn iiss nnoott pprriivvaattee"" in your web browser. To proceed,
 please click the ""AAddvvaanncceedd"" button and select the option to continue to the
 site. This warning is due to the SSL certificate currently being in the process
 of approval and will be validated shortly.
 ## Manual Installation 1. Clone the **MapSyncer** repository: ```bash git clone
 https://github.com/mapilio/MapSyncer.git cd MapSyncer ``` 2. Create Virtualenv
```

### Comparing `mapsyncer-1.0.0/mapsyncer.egg-info/PKG-INFO` & `mapsyncer-1.0.1/mapsyncer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapsyncer
-Version: 1.0.0
+Version: 1.0.1
 Summary: A toolkit to download and upload the data from KartaView to Mapilio
 Home-page: https://github.com/mapilio/MapSyncer
 Author: Mapilio
 License: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -69,15 +69,15 @@
 
 * [Mapilio Kit](https://github.com/mapilio/mapilio-kit) `In case you would like to follow the manual way you should install mapilio-kit manually.`
 * [Exiftool](https://exiftool.org/install.html)
 
 
 ## Pip Installation and Usage
 
-You may simply install and use the MapSyncer by using these commands below;
+<b>Note:</b> To install MapSyncer, you'll need to have Python and Pip installed on your system. Ensure you have Python version above <b>3.6</b> but below <b>3.12</b>. If you meet these criteria, please run the following commands:
 
 ```bash
 # Installation
 pip install mapsyncer
 
 # CLI Usage
 RunMapSyncer
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mapsyncer Version: 1.0.0 Summary: A toolkit to
+Metadata-Version: 2.1 Name: mapsyncer Version: 1.0.1 Summary: A toolkit to
 download and upload the data from KartaView to Mapilio Home-page: https://
 github.com/mapilio/MapSyncer Author: Mapilio License: MIT License Requires-
 Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: mapilio-kit Requires-Dist: ExifRead Requires-Dist: calculation-
 mapilio==0.1.39 Requires-Dist: requests_oauthlib Requires-Dist: imagesize
 Requires-Dist: setuptools Requires-Dist: psutil Requires-Dist: flask Requires-
 Dist: python-dotenv Requires-Dist: osm-login-python
@@ -18,17 +18,19 @@
 You can select specific sequences or all downloaded sequences that you want to
 upload to Mapilio. 6. And the process ends successfully. Don't worry, the
 RunMapSyncer command will check and do all these operations. ð« ## Install
 dependencies MapSyncer depends on the following libraries that need to be
 installed before building it.
 * [Mapilio Kit](https://github.com/mapilio/mapilio-kit) `In case you would like
 to follow the manual way you should install mapilio-kit manually.` * [Exiftool]
-(https://exiftool.org/install.html) ## Pip Installation and Usage You may
-simply install and use the MapSyncer by using these commands below; ```bash #
-Installation pip install mapsyncer # CLI Usage RunMapSyncer ```
+(https://exiftool.org/install.html) ## Pip Installation and Usage NNoottee:: To
+install MapSyncer, you'll need to have Python and Pip installed on your system.
+Ensure you have Python version above 33..66 but below 33..1122. If you meet these
+criteria, please run the following commands: ```bash # Installation pip install
+mapsyncer # CLI Usage RunMapSyncer ```
 When accessing the provided address, you may encounter a security warning
 stating ""YYoouurr ccoonnnneeccttiioonn iiss nnoott pprriivvaattee"" in your web browser. To proceed,
 please click the ""AAddvvaanncceedd"" button and select the option to continue to the
 site. This warning is due to the SSL certificate currently being in the process
 of approval and will be validated shortly.
 ## Manual Installation 1. Clone the **MapSyncer** repository: ```bash git clone
 https://github.com/mapilio/MapSyncer.git cd MapSyncer ``` 2. Create Virtualenv
```

### Comparing `mapsyncer-1.0.0/mapsyncer.egg-info/SOURCES.txt` & `mapsyncer-1.0.1/mapsyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapsyncer-1.0.0/setup.py` & `mapsyncer-1.0.1/setup.py`

 * *Files identical despite different names*


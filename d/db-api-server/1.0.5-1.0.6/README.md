# Comparing `tmp/db-api-server-1.0.5.tar.gz` & `tmp/db_api_server-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/krink/db-api/dist/tmp238ofo5b/db-api-server-1.0.5.tar", last modified: Sun Jan 16 06:43:02 2022, max compression
+gzip compressed data, was "/Users/krink/git/db-api/dist/.tmp-ohkg9bpc/db_api_server-1.0.6.tar", last modified: Fri May  3 12:36:11 2024, max compression
```

## Comparing `db-api-server-1.0.5.tar` & `db_api_server-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 krink      (501) staff       (20)        0 2022-01-16 06:43:02.877570 db-api-server-1.0.5/
--rw-r--r--   0 krink      (501) staff       (20)     1070 2022-01-16 01:03:16.000000 db-api-server-1.0.5/LICENSE
--rw-r--r--   0 krink      (501) staff       (20)      847 2022-01-16 06:43:02.877709 db-api-server-1.0.5/PKG-INFO
--rw-r--r--   0 krink      (501) staff       (20)     6936 2022-01-16 03:08:48.000000 db-api-server-1.0.5/README.md
--rw-r--r--   0 krink      (501) staff       (20)      104 2022-01-16 01:03:16.000000 db-api-server-1.0.5/pyproject.toml
--rw-r--r--   0 krink      (501) staff       (20)      828 2022-01-16 06:43:02.878359 db-api-server-1.0.5/setup.cfg
--rw-r--r--   0 krink      (501) staff       (20)      592 2022-01-16 06:37:37.000000 db-api-server-1.0.5/setup.py
-drwxr-xr-x   0 krink      (501) staff       (20)        0 2022-01-16 06:43:02.871993 db-api-server-1.0.5/src/
-drwxr-xr-x   0 krink      (501) staff       (20)        0 2022-01-16 06:43:02.875341 db-api-server-1.0.5/src/db_api_server/
--rw-r--r--   0 krink      (501) staff       (20)       84 2022-01-16 01:03:16.000000 db-api-server-1.0.5/src/db_api_server/__init__.py
--rw-r--r--   0 krink      (501) staff       (20)      180 2022-01-16 01:03:16.000000 db-api-server-1.0.5/src/db_api_server/__main__.py
--rw-r--r--   0 krink      (501) staff       (20)    15168 2022-01-16 06:36:44.000000 db-api-server-1.0.5/src/db_api_server/server.py
-drwxr-xr-x   0 krink      (501) staff       (20)        0 2022-01-16 06:43:02.877252 db-api-server-1.0.5/src/db_api_server.egg-info/
--rw-r--r--   0 krink      (501) staff       (20)      847 2022-01-16 06:43:02.000000 db-api-server-1.0.5/src/db_api_server.egg-info/PKG-INFO
--rw-r--r--   0 krink      (501) staff       (20)      387 2022-01-16 06:43:02.000000 db-api-server-1.0.5/src/db_api_server.egg-info/SOURCES.txt
--rw-r--r--   0 krink      (501) staff       (20)        1 2022-01-16 06:43:02.000000 db-api-server-1.0.5/src/db_api_server.egg-info/dependency_links.txt
--rw-r--r--   0 krink      (501) staff       (20)       61 2022-01-16 06:43:02.000000 db-api-server-1.0.5/src/db_api_server.egg-info/entry_points.txt
--rw-r--r--   0 krink      (501) staff       (20)       33 2022-01-16 06:43:02.000000 db-api-server-1.0.5/src/db_api_server.egg-info/requires.txt
--rw-r--r--   0 krink      (501) staff       (20)       14 2022-01-16 06:43:02.000000 db-api-server-1.0.5/src/db_api_server.egg-info/top_level.txt
+drwxr-xr-x   0 krink      (501) staff       (20)        0 2024-05-03 12:36:11.906284 db_api_server-1.0.6/
+-rw-r--r--   0 krink      (501) staff       (20)     1070 2024-05-03 12:26:16.000000 db_api_server-1.0.6/LICENSE
+-rw-r--r--   0 krink      (501) staff       (20)      878 2024-05-03 12:36:11.906139 db_api_server-1.0.6/PKG-INFO
+-rw-r--r--   0 krink      (501) staff       (20)     6936 2024-05-03 12:26:16.000000 db_api_server-1.0.6/README.md
+-rw-r--r--   0 krink      (501) staff       (20)      104 2024-05-03 12:26:16.000000 db_api_server-1.0.6/pyproject.toml
+-rw-r--r--   0 krink      (501) staff       (20)      817 2024-05-03 12:36:11.906967 db_api_server-1.0.6/setup.cfg
+-rw-r--r--   0 krink      (501) staff       (20)      581 2024-05-03 12:31:07.000000 db_api_server-1.0.6/setup.py
+drwxr-xr-x   0 krink      (501) staff       (20)        0 2024-05-03 12:36:11.900853 db_api_server-1.0.6/src/
+drwxr-xr-x   0 krink      (501) staff       (20)        0 2024-05-03 12:36:11.902997 db_api_server-1.0.6/src/db_api_server/
+-rw-r--r--   0 krink      (501) staff       (20)       84 2024-05-03 12:26:16.000000 db_api_server-1.0.6/src/db_api_server/__init__.py
+-rw-r--r--   0 krink      (501) staff       (20)      180 2024-05-03 12:26:16.000000 db_api_server-1.0.6/src/db_api_server/__main__.py
+-rw-r--r--   0 krink      (501) staff       (20)    15162 2024-05-03 12:31:07.000000 db_api_server-1.0.6/src/db_api_server/server.py
+drwxr-xr-x   0 krink      (501) staff       (20)        0 2024-05-03 12:36:11.905437 db_api_server-1.0.6/src/db_api_server.egg-info/
+-rw-r--r--   0 krink      (501) staff       (20)      878 2024-05-03 12:36:11.000000 db_api_server-1.0.6/src/db_api_server.egg-info/PKG-INFO
+-rw-r--r--   0 krink      (501) staff       (20)      387 2024-05-03 12:36:11.000000 db_api_server-1.0.6/src/db_api_server.egg-info/SOURCES.txt
+-rw-r--r--   0 krink      (501) staff       (20)        1 2024-05-03 12:36:11.000000 db_api_server-1.0.6/src/db_api_server.egg-info/dependency_links.txt
+-rw-r--r--   0 krink      (501) staff       (20)       60 2024-05-03 12:36:11.000000 db_api_server-1.0.6/src/db_api_server.egg-info/entry_points.txt
+-rw-r--r--   0 krink      (501) staff       (20)       33 2024-05-03 12:36:11.000000 db_api_server-1.0.6/src/db_api_server.egg-info/requires.txt
+-rw-r--r--   0 krink      (501) staff       (20)       14 2024-05-03 12:36:11.000000 db_api_server-1.0.6/src/db_api_server.egg-info/top_level.txt
```

### Comparing `db-api-server-1.0.5/LICENSE` & `db_api_server-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `db-api-server-1.0.5/PKG-INFO` & `db_api_server-1.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: db-api-server
-Version: 1.0.5
+Version: 1.0.6
 Summary: db-api-server flask mysql.connector
 Home-page: https://gitlab.com/krink/db-api-server
-Author: Karl Rink
-Author-email: karl@rink.us
-License: UNKNOWN
+Author: K
+Author-email: k@rink.us
 Project-URL: Bug Tracker, https://gitlab.com/krink/db-api-server/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Database :: Database Engines/Servers
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: flask
+Requires-Dist: flask-cors
+Requires-Dist: mysql.connector
 
 RESTful API for mysql/mariadb
-
```

### Comparing `db-api-server-1.0.5/README.md` & `db_api_server-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `db-api-server-1.0.5/setup.cfg` & `db_api_server-1.0.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = db-api-server-pkg-krink
-version = 1.0.5
-author = Karl Rink
-author_email = karl@rink.us
+version = 1.0.6
+author = K
+author_email = k@rink.us
 description = db-api-server
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/krink/db-api-server
 project_urls = 
 	Bug Tracker = https://gitlab.com/krink/db-api-server/issues
 classifiers =
```

### Comparing `db-api-server-1.0.5/setup.py` & `db_api_server-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 setup(
     name = "db-api-server",
     packages = ["db_api_server"],
     entry_points = {
         "console_scripts": ['db-api-server = db_api_server.server:main']
         },
-    version = '1.0.5',
+    version = '1.0.6',
     description = "db-api-server flask mysql.connector",
     long_description = "RESTful API for mysql/mariadb",
-    author = "Karl Rink",
-    author_email = "karl@rink.us",
+    author = "K",
+    author_email = "k@rink.us",
     url = "https://gitlab.com/krink/db-api-server",
     install_requires = [ 'flask', 'flask-cors', 'mysql.connector' ]
     )
```

### Comparing `db-api-server-1.0.5/src/db_api_server/server.py` & `db_api_server-1.0.6/src/db_api_server/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 # -*- coding: utf-8 -*-
 
 """server: db-api."""
 
 from __future__ import absolute_import
 
-__version__ = '1.0.5'
+__version__ = '1.0.6'
 
 import base64
 import decimal
 import json
 
 import flask.json
 from flask import Flask
@@ -17,15 +17,15 @@
 from flask import jsonify
 from werkzeug.exceptions import HTTPException
 from flask_cors import CORS
 
 import mysql.connector
 
 
-class AppJSONEncoder(flask.json.JSONEncoder):
+class AppJSONEncoder(json.JSONEncoder):
     """app: json encoder."""
 
     def default(self, o):
         """default: self."""
         if isinstance(o, decimal.Decimal):
             # Convert decimal instance to string
             return str(o)
```

### Comparing `db-api-server-1.0.5/src/db_api_server.egg-info/PKG-INFO` & `db_api_server-1.0.6/src/db_api_server.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: db-api-server
-Version: 1.0.5
+Version: 1.0.6
 Summary: db-api-server flask mysql.connector
 Home-page: https://gitlab.com/krink/db-api-server
-Author: Karl Rink
-Author-email: karl@rink.us
-License: UNKNOWN
+Author: K
+Author-email: k@rink.us
 Project-URL: Bug Tracker, https://gitlab.com/krink/db-api-server/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Database :: Database Engines/Servers
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: flask
+Requires-Dist: flask-cors
+Requires-Dist: mysql.connector
 
 RESTful API for mysql/mariadb
-
```


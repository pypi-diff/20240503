# Comparing `tmp/intervalsicu_to_influxdb-0.2.4.tar.gz` & `tmp/intervalsicu_to_influxdb-0.2.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intervalsicu_to_influxdb-0.2.4.tar", last modified: Wed Sep  6 10:39:35 2023, max compression
+gzip compressed data, was "intervalsicu_to_influxdb-0.2.41.tar", last modified: Fri May  3 17:12:06 2024, max compression
```

## Comparing `intervalsicu_to_influxdb-0.2.4.tar` & `intervalsicu_to_influxdb-0.2.41.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-09-06 10:39:35.959290 intervalsicu_to_influxdb-0.2.4/
--rw-r--r--   0 pi        (1000) pi        (1000)    35063 2023-09-01 10:51:36.000000 intervalsicu_to_influxdb-0.2.4/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     6516 2023-09-06 10:39:35.959290 intervalsicu_to_influxdb-0.2.4/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     5728 2023-09-06 10:34:12.000000 intervalsicu_to_influxdb-0.2.4/README.md
--rw-r--r--   0 pi        (1000) pi        (1000)      716 2023-09-06 10:38:52.000000 intervalsicu_to_influxdb-0.2.4/pyproject.toml
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-09-06 10:39:35.959290 intervalsicu_to_influxdb-0.2.4/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)     1006 2023-09-06 10:38:52.000000 intervalsicu_to_influxdb-0.2.4/setup.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-09-06 10:39:35.939290 intervalsicu_to_influxdb-0.2.4/src/
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-09-06 10:39:35.949290 intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb/
--rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-09-05 10:19:09.000000 intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb/__init__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-09-06 10:39:35.959290 intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb/clients/
--rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-09-05 10:19:09.000000 intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb/clients/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1751 2023-09-05 10:19:09.000000 intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb/clients/influx_client.py
--rw-r--r--   0 pi        (1000) pi        (1000)     7548 2023-09-05 10:19:09.000000 intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb/clients/intervals_client.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-09-06 10:39:35.959290 intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb/entities/
--rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-09-05 10:19:09.000000 intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb/entities/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6675 2023-09-06 10:22:27.000000 intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb/entities/activity.py
--rw-r--r--   0 pi        (1000) pi        (1000)      230 2023-09-06 10:22:27.000000 intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb/entities/streams.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1560 2023-09-05 10:37:20.000000 intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb/entities/wellness.py
--rw-r--r--   0 pi        (1000) pi        (1000)     7785 2023-09-05 10:19:09.000000 intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb/extractor.py
--rw-r--r--   0 pi        (1000) pi        (1000)      916 2023-09-05 10:19:09.000000 intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb/my_utils.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-09-06 10:39:35.949290 intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     6516 2023-09-06 10:39:35.000000 intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      783 2023-09-06 10:39:35.000000 intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-09-06 10:39:35.000000 intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       39 2023-09-06 10:39:35.000000 intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       25 2023-09-06 10:39:35.000000 intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 17:12:06.850730 intervalsicu_to_influxdb-0.2.41/
+-rw-rw-rw-   0 root         (0) root         (0)    35063 2024-05-03 17:12:02.000000 intervalsicu_to_influxdb-0.2.41/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6499 2024-05-03 17:12:06.850730 intervalsicu_to_influxdb-0.2.41/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5733 2024-05-03 17:12:02.000000 intervalsicu_to_influxdb-0.2.41/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-03 17:12:02.000000 intervalsicu_to_influxdb-0.2.41/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 17:12:06.850730 intervalsicu_to_influxdb-0.2.41/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      491 2024-05-03 17:12:02.000000 intervalsicu_to_influxdb-0.2.41/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 17:12:06.845730 intervalsicu_to_influxdb-0.2.41/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 17:12:06.847730 intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 17:12:02.000000 intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 17:12:06.849729 intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb/clients/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 17:12:02.000000 intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1751 2024-05-03 17:12:02.000000 intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb/clients/influx_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2024-05-03 17:12:02.000000 intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb/clients/intervals_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 17:12:06.850730 intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb/entities/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 17:12:02.000000 intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb/entities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6675 2024-05-03 17:12:02.000000 intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb/entities/activity.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2024-05-03 17:12:02.000000 intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb/entities/streams.py
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2024-05-03 17:12:02.000000 intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb/entities/wellness.py
+-rw-rw-rw-   0 root         (0) root         (0)     7785 2024-05-03 17:12:02.000000 intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb/extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)      916 2024-05-03 17:12:02.000000 intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb/my_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 17:12:06.850730 intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6499 2024-05-03 17:12:06.000000 intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      783 2024-05-03 17:12:06.000000 intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 17:12:06.000000 intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-05-03 17:12:06.000000 intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-03 17:12:06.000000 intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb.egg-info/top_level.txt
```

### Comparing `intervalsicu_to_influxdb-0.2.4/LICENSE` & `intervalsicu_to_influxdb-0.2.41/LICENSE`

 * *Files identical despite different names*

### Comparing `intervalsicu_to_influxdb-0.2.4/PKG-INFO` & `intervalsicu_to_influxdb-0.2.41/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
-Name: intervalsicu_to_influxdb
-Version: 0.2.4
+Name: intervalsicu-to-influxdb
+Version: 0.2.41
 Summary: A package to extract data from intervals.icu to influxDB
-Home-page: https://codeberg.org/tmllull/intervalsicu-to-influxdb
-Author: Toni Miquel Llull
 Author-email: Toni Miquel Llull <tonimiquel.llull@gmail.com>
-License: GPL3
-Project-URL: Homepage, https://codeberg.org/tmllull/intervalsicu-to-influxdb
-Project-URL: Bug Tracker, https://codeberg.org/tmllull/intervalsicu-to-influxdb/issues
+Project-URL: Homepage, https://gitlab.com/tmllull/intervalsicu-to-influxdb
+Project-URL: Bug Tracker, https://gitlab.com/tmllull/intervalsicu-to-influxdb/issues
 Project-URL: Documentation, https://intervalsicu-to-influxdb.readthedocs.io
 Keywords: intervalsicu,influxdb,sport
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: influxdb-client
+Requires-Dist: python-dotenv
+Requires-Dist: requests
 
 # Intervals.icu to InfluxDB
 Intervalsicu-to-influxdb is a personal project to extract data from Intervals.icu to InfluxDB (oh, really?). But if Intervals.icu already shows a lot of graphics, statistics and more, why I need to extract it?
 
 Full documentation can be found in [here](https://intervalsicu-to-influxdb.readthedocs.io)
 
 ## Why
@@ -169,15 +169,15 @@
 ```
 And then, just run it like the Docker section above (but with the image name)
 
 ```bash
 docker run --env-file PATH/TO/FILE -it --rm intervals-to-influxdb app.py [-h] [--start-date START_DATE] [--end-date END_DATE] [--streams] [--reset]
 ```
 
-Run with Python
+#### Run with Python
 First, install dependencies from source
 ```
 pip install .
 ```
 
 And then, run the script
 ```
```

### Comparing `intervalsicu_to_influxdb-0.2.4/README.md` & `intervalsicu_to_influxdb-0.2.41/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 ```
 And then, just run it like the Docker section above (but with the image name)
 
 ```bash
 docker run --env-file PATH/TO/FILE -it --rm intervals-to-influxdb app.py [-h] [--start-date START_DATE] [--end-date END_DATE] [--streams] [--reset]
 ```
 
-Run with Python
+#### Run with Python
 First, install dependencies from source
 ```
 pip install .
 ```
 
 And then, run the script
 ```
```

### Comparing `intervalsicu_to_influxdb-0.2.4/pyproject.toml` & `intervalsicu_to_influxdb-0.2.41/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "intervalsicu_to_influxdb"
-version = "0.2.4"
+dynamic = ["version", "dependencies"]
+name = "intervalsicu-to-influxdb"
 authors = [{ name = "Toni Miquel Llull", email = "tonimiquel.llull@gmail.com" }]
 description = "A package to extract data from intervals.icu to influxDB"
 readme = "README.md"
 requires-python = ">=3.6"
+keywords = ["intervalsicu", "influxdb", "sport"]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
 ]
 
 [project.urls]
-"Homepage" = "https://codeberg.org/tmllull/intervalsicu-to-influxdb"
-"Bug Tracker" = "https://codeberg.org/tmllull/intervalsicu-to-influxdb/issues"
+"Homepage" = "https://gitlab.com/tmllull/intervalsicu-to-influxdb"
+"Bug Tracker" = "https://gitlab.com/tmllull/intervalsicu-to-influxdb/issues"
 "Documentation" = "https://intervalsicu-to-influxdb.readthedocs.io"
```

### Comparing `intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb/clients/influx_client.py` & `intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb/clients/influx_client.py`

 * *Files identical despite different names*

### Comparing `intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb/clients/intervals_client.py` & `intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb/clients/intervals_client.py`

 * *Files identical despite different names*

### Comparing `intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb/entities/activity.py` & `intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb/entities/activity.py`

 * *Files identical despite different names*

### Comparing `intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb/entities/wellness.py` & `intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb/entities/wellness.py`

 * *Files identical despite different names*

### Comparing `intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb/extractor.py` & `intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb/extractor.py`

 * *Files identical despite different names*

### Comparing `intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb/my_utils.py` & `intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb/my_utils.py`

 * *Files identical despite different names*

### Comparing `intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb.egg-info/PKG-INFO` & `intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: intervalsicu-to-influxdb
-Version: 0.2.4
+Version: 0.2.41
 Summary: A package to extract data from intervals.icu to influxDB
-Home-page: https://codeberg.org/tmllull/intervalsicu-to-influxdb
-Author: Toni Miquel Llull
 Author-email: Toni Miquel Llull <tonimiquel.llull@gmail.com>
-License: GPL3
-Project-URL: Homepage, https://codeberg.org/tmllull/intervalsicu-to-influxdb
-Project-URL: Bug Tracker, https://codeberg.org/tmllull/intervalsicu-to-influxdb/issues
+Project-URL: Homepage, https://gitlab.com/tmllull/intervalsicu-to-influxdb
+Project-URL: Bug Tracker, https://gitlab.com/tmllull/intervalsicu-to-influxdb/issues
 Project-URL: Documentation, https://intervalsicu-to-influxdb.readthedocs.io
 Keywords: intervalsicu,influxdb,sport
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: influxdb-client
+Requires-Dist: python-dotenv
+Requires-Dist: requests
 
 # Intervals.icu to InfluxDB
 Intervalsicu-to-influxdb is a personal project to extract data from Intervals.icu to InfluxDB (oh, really?). But if Intervals.icu already shows a lot of graphics, statistics and more, why I need to extract it?
 
 Full documentation can be found in [here](https://intervalsicu-to-influxdb.readthedocs.io)
 
 ## Why
@@ -169,15 +169,15 @@
 ```
 And then, just run it like the Docker section above (but with the image name)
 
 ```bash
 docker run --env-file PATH/TO/FILE -it --rm intervals-to-influxdb app.py [-h] [--start-date START_DATE] [--end-date END_DATE] [--streams] [--reset]
 ```
 
-Run with Python
+#### Run with Python
 First, install dependencies from source
 ```
 pip install .
 ```
 
 And then, run the script
 ```
```

### Comparing `intervalsicu_to_influxdb-0.2.4/src/intervalsicu_to_influxdb.egg-info/SOURCES.txt` & `intervalsicu_to_influxdb-0.2.41/src/intervalsicu_to_influxdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*


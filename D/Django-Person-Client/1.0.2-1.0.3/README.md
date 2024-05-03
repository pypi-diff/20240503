# Comparing `tmp/Django-Person-Client-1.0.2.tar.gz` & `tmp/Django-Person-Client-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Django-Person-Client-1.0.2.tar", last modified: Fri Apr 12 16:51:18 2024, max compression
+gzip compressed data, was "Django-Person-Client-1.0.3.tar", last modified: Fri May  3 16:50:54 2024, max compression
```

## Comparing `Django-Person-Client-1.0.2.tar` & `Django-Person-Client-1.0.3.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:18.157783 Django-Person-Client-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:18.153783 Django-Person-Client-1.0.2/Django_Person_Client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-12 16:51:18.000000 Django-Person-Client-1.0.2/Django_Person_Client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-12 16:51:18.000000 Django-Person-Client-1.0.2/Django_Person_Client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:51:18.000000 Django-Person-Client-1.0.2/Django_Person_Client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 16:51:18.000000 Django-Person-Client-1.0.2/Django_Person_Client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 16:51:18.000000 Django-Person-Client-1.0.2/Django_Person_Client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-12 16:51:18.153783 Django-Person-Client-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 16:51:18.157783 Django-Person-Client-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:18.153783 Django-Person-Client-1.0.2/uw_person_client/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 16:51:17.000000 Django-Person-Client-1.0.2/uw_person_client/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:18.153783 Django-Person-Client-1.0.2/uw_person_client/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/fixtures/adviser.json
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/fixtures/degree.json
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/fixtures/employee.json
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/fixtures/hold.json
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/fixtures/major.json
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/fixtures/person.json
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/fixtures/sport.json
--rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/fixtures/student.json
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/fixtures/term.json
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/fixtures/transcript.json
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/fixtures/transfer.json
--rw-r--r--   0 runner    (1001) docker     (127)    32447 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:18.153783 Django-Person-Client-1.0.2/uw_person_client/test_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    32894 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/test_migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/test_migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:18.153783 Django-Person-Client-1.0.2/uw_person_client/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/tests/test_adviser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/tests/test_major.py
--rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/tests/test_person.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-12 16:51:06.000000 Django-Person-Client-1.0.2/uw_person_client/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:50:54.871142 Django-Person-Client-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:50:54.867142 Django-Person-Client-1.0.3/Django_Person_Client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-03 16:50:54.000000 Django-Person-Client-1.0.3/Django_Person_Client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-03 16:50:54.000000 Django-Person-Client-1.0.3/Django_Person_Client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:50:54.000000 Django-Person-Client-1.0.3/Django_Person_Client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 16:50:54.000000 Django-Person-Client-1.0.3/Django_Person_Client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 16:50:54.000000 Django-Person-Client-1.0.3/Django_Person_Client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-03 16:50:54.871142 Django-Person-Client-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:50:54.871142 Django-Person-Client-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:50:54.867142 Django-Person-Client-1.0.3/uw_person_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 16:50:53.000000 Django-Person-Client-1.0.3/uw_person_client/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:50:54.867142 Django-Person-Client-1.0.3/uw_person_client/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/fixtures/adviser.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/fixtures/degree.json
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/fixtures/employee.json
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/fixtures/hold.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/fixtures/major.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/fixtures/person.json
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/fixtures/sport.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/fixtures/student.json
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/fixtures/term.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/fixtures/transcript.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/fixtures/transfer.json
+-rw-r--r--   0 runner    (1001) docker     (127)    32447 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:50:54.867142 Django-Person-Client-1.0.3/uw_person_client/test_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    32894 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/test_migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/test_migrations/0002_alter_ordering_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/test_migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:50:54.871142 Django-Person-Client-1.0.3/uw_person_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/tests/test_adviser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/tests/test_major.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/tests/test_person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-03 16:50:44.000000 Django-Person-Client-1.0.3/uw_person_client/urls.py
```

### Comparing `Django-Person-Client-1.0.2/Django_Person_Client.egg-info/PKG-INFO` & `Django-Person-Client-1.0.3/Django_Person_Client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Django-Person-Client
-Version: 1.0.2
+Version: 1.0.3
 Summary: A UW Person Client Django app
 Home-page: https://github.com/uw-it-aca/django-person-client
 Author: UW-IT T&LS
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `Django-Person-Client-1.0.2/Django_Person_Client.egg-info/SOURCES.txt` & `Django-Person-Client-1.0.3/Django_Person_Client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,12 +20,13 @@
 uw_person_client/fixtures/person.json
 uw_person_client/fixtures/sport.json
 uw_person_client/fixtures/student.json
 uw_person_client/fixtures/term.json
 uw_person_client/fixtures/transcript.json
 uw_person_client/fixtures/transfer.json
 uw_person_client/test_migrations/0001_initial.py
+uw_person_client/test_migrations/0002_alter_ordering_options.py
 uw_person_client/test_migrations/__init__.py
 uw_person_client/tests/__init__.py
 uw_person_client/tests/test_adviser.py
 uw_person_client/tests/test_major.py
 uw_person_client/tests/test_person.py
```

### Comparing `Django-Person-Client-1.0.2/LICENSE` & `Django-Person-Client-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.2/PKG-INFO` & `Django-Person-Client-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Django-Person-Client
-Version: 1.0.2
+Version: 1.0.3
 Summary: A UW Person Client Django app
 Home-page: https://github.com/uw-it-aca/django-person-client
 Author: UW-IT T&LS
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `Django-Person-Client-1.0.2/README.md` & `Django-Person-Client-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.2/setup.py` & `Django-Person-Client-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.2/uw_person_client/fixtures/adviser.json` & `Django-Person-Client-1.0.3/uw_person_client/fixtures/adviser.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.2/uw_person_client/fixtures/degree.json` & `Django-Person-Client-1.0.3/uw_person_client/fixtures/degree.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.2/uw_person_client/fixtures/employee.json` & `Django-Person-Client-1.0.3/uw_person_client/fixtures/employee.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.2/uw_person_client/fixtures/hold.json` & `Django-Person-Client-1.0.3/uw_person_client/fixtures/hold.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.2/uw_person_client/fixtures/major.json` & `Django-Person-Client-1.0.3/uw_person_client/fixtures/major.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.2/uw_person_client/fixtures/person.json` & `Django-Person-Client-1.0.3/uw_person_client/fixtures/person.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.2/uw_person_client/fixtures/sport.json` & `Django-Person-Client-1.0.3/uw_person_client/fixtures/sport.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.2/uw_person_client/fixtures/student.json` & `Django-Person-Client-1.0.3/uw_person_client/fixtures/student.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.2/uw_person_client/fixtures/transcript.json` & `Django-Person-Client-1.0.3/uw_person_client/fixtures/transcript.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.2/uw_person_client/fixtures/transfer.json` & `Django-Person-Client-1.0.3/uw_person_client/fixtures/transfer.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.2/uw_person_client/models.py` & `Django-Person-Client-1.0.3/uw_person_client/models.py`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.2/uw_person_client/test_migrations/0001_initial.py` & `Django-Person-Client-1.0.3/uw_person_client/test_migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.2/uw_person_client/tests/test_adviser.py` & `Django-Person-Client-1.0.3/uw_person_client/tests/test_adviser.py`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.2/uw_person_client/tests/test_major.py` & `Django-Person-Client-1.0.3/uw_person_client/tests/test_major.py`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.2/uw_person_client/tests/test_person.py` & `Django-Person-Client-1.0.3/uw_person_client/tests/test_person.py`

 * *Files identical despite different names*


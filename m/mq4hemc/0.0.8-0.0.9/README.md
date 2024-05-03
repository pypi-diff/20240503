# Comparing `tmp/mq4hemc-0.0.8.tar.gz` & `tmp/mq4hemc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mq4hemc-0.0.8.tar", max compression
+gzip compressed data, was "mq4hemc-0.0.9.tar", last modified: Thu May  2 15:54:45 2024, max compression
```

## Comparing `mq4hemc-0.0.8.tar` & `mq4hemc-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,30 @@
--rw-r--r--   0        0        0     1077 2024-04-30 09:39:00.954452 mq4hemc-0.0.8/LICENSE
--rw-r--r--   0        0        0     2954 2024-05-02 11:59:52.479573 mq4hemc-0.0.8/README.md
--rw-r--r--   0        0        0      877 2024-05-02 12:50:50.401723 mq4hemc-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      155 2024-05-02 08:01:43.802063 mq4hemc-0.0.8/src/mq4hemc/__init__.py
--rw-r--r--   0        0        0     1215 2024-05-02 08:02:58.866952 mq4hemc-0.0.8/src/mq4hemc/hemc_observer.py
--rw-r--r--   0        0        0     3973 2024-05-02 08:22:35.280538 mq4hemc-0.0.8/src/mq4hemc/hemc_queue.py
--rw-r--r--   0        0        0     1752 2024-05-02 08:04:40.060122 mq4hemc-0.0.8/src/mq4hemc/hemc_service.py
--rw-r--r--   0        0        0     3758 1970-01-01 00:00:00.000000 mq4hemc-0.0.8/PKG-INFO
+drwxrwxr-x   0 oshevchenko  (1000) oshevchenko  (1000)        0 2024-05-02 15:54:45.056076 mq4hemc-0.0.9/
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     3101 2024-05-02 12:01:36.000000 mq4hemc-0.0.9/.gitignore
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     1077 2024-04-30 09:39:00.000000 mq4hemc-0.0.9/LICENSE
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      952 2024-05-02 15:49:59.000000 mq4hemc-0.0.9/Makefile
+-rw-r--r--   0 oshevchenko  (1000) oshevchenko  (1000)     3444 2024-05-02 15:54:45.056076 mq4hemc-0.0.9/PKG-INFO
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     2954 2024-05-02 11:59:52.000000 mq4hemc-0.0.9/README.md
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      244 2024-05-02 09:34:00.000000 mq4hemc-0.0.9/poetry.lock
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      161 2024-05-02 15:48:47.000000 mq4hemc-0.0.9/pyproject.toml
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      672 2024-05-02 14:23:44.000000 mq4hemc-0.0.9/pyproject.toml.in
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      659 2024-05-02 09:41:02.000000 mq4hemc-0.0.9/requirements.txt
+drwxrwxr-x   0 oshevchenko  (1000) oshevchenko  (1000)        0 2024-05-02 15:54:45.052076 mq4hemc-0.0.9/scripts/
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     1120 2024-05-02 15:29:08.000000 mq4hemc-0.0.9/scripts/generate-pyproject.py
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      632 2024-05-02 15:54:45.056076 mq4hemc-0.0.9/setup.cfg
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)       38 2024-05-02 15:33:15.000000 mq4hemc-0.0.9/setup.py
+drwxrwxr-x   0 oshevchenko  (1000) oshevchenko  (1000)        0 2024-05-02 15:54:45.052076 mq4hemc-0.0.9/src/
+drwxrwxr-x   0 oshevchenko  (1000) oshevchenko  (1000)        0 2024-05-02 15:54:45.052076 mq4hemc-0.0.9/src/mq4hemc/
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      155 2024-05-02 08:01:43.000000 mq4hemc-0.0.9/src/mq4hemc/__init__.py
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     1215 2024-05-02 08:02:58.000000 mq4hemc-0.0.9/src/mq4hemc/hemc_observer.py
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     3973 2024-05-02 08:22:35.000000 mq4hemc-0.0.9/src/mq4hemc/hemc_queue.py
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     1752 2024-05-02 08:04:40.000000 mq4hemc-0.0.9/src/mq4hemc/hemc_service.py
+drwxrwxr-x   0 oshevchenko  (1000) oshevchenko  (1000)        0 2024-05-02 15:54:45.056076 mq4hemc-0.0.9/src/mq4hemc.egg-info/
+-rw-r--r--   0 oshevchenko  (1000) oshevchenko  (1000)     3444 2024-05-02 15:54:45.000000 mq4hemc-0.0.9/src/mq4hemc.egg-info/PKG-INFO
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      484 2024-05-02 15:54:45.000000 mq4hemc-0.0.9/src/mq4hemc.egg-info/SOURCES.txt
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)        1 2024-05-02 15:54:45.000000 mq4hemc-0.0.9/src/mq4hemc.egg-info/dependency_links.txt
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)        8 2024-05-02 15:54:45.000000 mq4hemc-0.0.9/src/mq4hemc.egg-info/top_level.txt
+drwxrwxr-x   0 oshevchenko  (1000) oshevchenko  (1000)        0 2024-05-02 15:54:45.056076 mq4hemc-0.0.9/tests/
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     3728 2024-05-02 11:23:22.000000 mq4hemc-0.0.9/tests/test_mq4hemc.py
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     2807 2024-05-02 11:22:48.000000 mq4hemc-0.0.9/tests/test_observer.py
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     1747 2024-05-02 11:39:26.000000 mq4hemc-0.0.9/tests/test_readme.py
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     3588 2024-05-02 11:23:02.000000 mq4hemc-0.0.9/tests/test_real_use.py
```

### Comparing `mq4hemc-0.0.8/LICENSE` & `mq4hemc-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mq4hemc-0.0.8/README.md` & `mq4hemc-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mq4hemc-0.0.8/src/mq4hemc/hemc_observer.py` & `mq4hemc-0.0.9/src/mq4hemc/hemc_observer.py`

 * *Files identical despite different names*

### Comparing `mq4hemc-0.0.8/src/mq4hemc/hemc_queue.py` & `mq4hemc-0.0.9/src/mq4hemc/hemc_queue.py`

 * *Files identical despite different names*

### Comparing `mq4hemc-0.0.8/src/mq4hemc/hemc_service.py` & `mq4hemc-0.0.9/src/mq4hemc/hemc_service.py`

 * *Files identical despite different names*

### Comparing `mq4hemc-0.0.8/PKG-INFO` & `mq4hemc-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 Metadata-Version: 2.1
 Name: mq4hemc
-Version: 0.0.8
+Version: 0.0.9
 Summary: Message Queue related Python library
+Home-page: https://github.com/oshevchenko/mq4hemc
 Author: Oleksandr Shevchenko
 Author-email: shevchenko.adb@gmail.com
-Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Project-URL: Homepage, https://github.com/oshevchenko/mq4hemc
-Project-URL: Issues, https://github.com/oshevchenko/mq4hemc/issues
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Message Queue Based Service
 ```py
 from mq4hemc import HemcMessage, HemcService
 ```
 `HemcService` - a class to create a separate thread which is extracting messages
 from the message queue and passes them to user callback for processing.
@@ -94,8 +89,7 @@
 2024-05-02 14:39:29 - test_mq4hemc - INFO - Processed message 'test0'
 2024-05-02 14:39:30 - test_mq4hemc - INFO - Processed message 'test1'
 2024-05-02 14:39:31 - test_mq4hemc - INFO - Processed message 'test2'
 2024-05-02 14:39:32 - test_mq4hemc - INFO - Processed message 'test_sync'
 2024-05-02 14:39:32 - test_mq4hemc - INFO - Message test_sync processed, reply: test_sync
 2024-05-02 14:39:32 - test_mq4hemc - INFO - Service stopped.
 ```
-
```


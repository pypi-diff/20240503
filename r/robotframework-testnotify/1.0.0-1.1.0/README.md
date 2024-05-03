# Comparing `tmp/robotframework_testnotify-1.tar.gz` & `tmp/robotframework-testnotify-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_testnotify-1.tar", last modified: Mon Apr 29 15:40:10 2024, max compression
+gzip compressed data, was "robotframework-testnotify-1.1.0.tar", last modified: Fri May  3 14:39:45 2024, max compression
```

## Comparing `robotframework_testnotify-1.tar` & `robotframework-testnotify-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 15:40:10.087937 robotframework_testnotify-1/
--rw-rw-rw-   0        0        0      688 2024-04-29 15:40:10.086937 robotframework_testnotify-1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 15:40:10.069933 robotframework_testnotify-1/TestNotification/
--rw-rw-rw-   0        0        0     4580 2024-04-29 15:29:08.000000 robotframework_testnotify-1/TestNotification/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 15:40:10.085935 robotframework_testnotify-1/robotframework_testnotify.egg-info/
--rw-rw-rw-   0        0        0      688 2024-04-29 15:40:09.000000 robotframework_testnotify-1/robotframework_testnotify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-04-29 15:40:10.000000 robotframework_testnotify-1/robotframework_testnotify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 15:40:09.000000 robotframework_testnotify-1/robotframework_testnotify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-29 15:40:10.000000 robotframework_testnotify-1/robotframework_testnotify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-29 15:40:10.000000 robotframework_testnotify-1/robotframework_testnotify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 15:40:10.088938 robotframework_testnotify-1/setup.cfg
--rw-rw-rw-   0        0        0      986 2024-04-29 15:35:34.000000 robotframework_testnotify-1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 14:39:45.057199 robotframework-testnotify-1.1.0/
+-rw-rw-rw-   0        0        0     1073 2024-05-03 14:38:24.000000 robotframework-testnotify-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2600 2024-05-03 14:39:45.056192 robotframework-testnotify-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 14:39:45.022109 robotframework-testnotify-1.1.0/TestNotification/
+-rw-rw-rw-   0        0        0     9053 2024-05-03 12:37:39.000000 robotframework-testnotify-1.1.0/TestNotification/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 14:39:45.055198 robotframework-testnotify-1.1.0/robotframework_testnotify.egg-info/
+-rw-rw-rw-   0        0        0     2600 2024-05-03 14:39:44.000000 robotframework-testnotify-1.1.0/robotframework_testnotify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-05-03 14:39:45.000000 robotframework-testnotify-1.1.0/robotframework_testnotify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 14:39:44.000000 robotframework-testnotify-1.1.0/robotframework_testnotify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-03 14:39:44.000000 robotframework-testnotify-1.1.0/robotframework_testnotify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-03 14:39:44.000000 robotframework-testnotify-1.1.0/robotframework_testnotify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 14:39:45.058201 robotframework-testnotify-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      986 2024-05-03 14:35:30.000000 robotframework-testnotify-1.1.0/setup.py
```

### Comparing `robotframework_testnotify-1/setup.py` & `robotframework-testnotify-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="robotframework-testnotify",
-    version="1.0.0",
+    version="1.1.0",
     description="Send notifications to chat using Robot Framework.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/barbosamp/robotframework-testnotification.git",
     author="Marcos Barbosa",
     author_email="",
     license="MIT",
```


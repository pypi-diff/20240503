# Comparing `tmp/slack_approval-0.1.7.0.tar.gz` & `tmp/slack_approval-0.1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack_approval-0.1.7.0.tar", last modified: Wed Oct  4 14:21:42 2023, max compression
+gzip compressed data, was "slack_approval-0.1.7.1.tar", last modified: Fri May  3 17:18:24 2024, max compression
```

## Comparing `slack_approval-0.1.7.0.tar` & `slack_approval-0.1.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-10-04 14:21:42.789853 slack_approval-0.1.7.0/
--rw-r--r--   0 austen.novis   (502) staff       (20)     4912 2023-10-04 14:21:42.789653 slack_approval-0.1.7.0/PKG-INFO
--rw-r--r--   0 austen.novis   (502) staff       (20)     4079 2023-05-16 17:36:53.000000 slack_approval-0.1.7.0/README.md
--rw-r--r--   0 austen.novis   (502) staff       (20)       38 2023-10-04 14:21:42.789923 slack_approval-0.1.7.0/setup.cfg
--rw-r--r--   0 austen.novis   (502) staff       (20)     2828 2023-10-04 14:21:34.000000 slack_approval-0.1.7.0/setup.py
-drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-10-04 14:21:42.788386 slack_approval-0.1.7.0/slack_approval/
--rw-r--r--   0 austen.novis   (502) staff       (20)        0 2023-05-16 17:36:53.000000 slack_approval-0.1.7.0/slack_approval/__init__.py
--rw-r--r--   0 austen.novis   (502) staff       (20)      293 2023-05-16 17:36:53.000000 slack_approval-0.1.7.0/slack_approval/cli.py
--rw-r--r--   0 austen.novis   (502) staff       (20)    23192 2023-10-04 14:21:34.000000 slack_approval-0.1.7.0/slack_approval/slack_provision.py
--rw-r--r--   0 austen.novis   (502) staff       (20)     3470 2023-08-24 21:17:18.000000 slack_approval-0.1.7.0/slack_approval/slack_request.py
--rw-r--r--   0 austen.novis   (502) staff       (20)     3603 2023-08-24 21:17:18.000000 slack_approval-0.1.7.0/slack_approval/utils.py
-drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-10-04 14:21:42.789368 slack_approval-0.1.7.0/slack_approval.egg-info/
--rw-r--r--   0 austen.novis   (502) staff       (20)     4912 2023-10-04 14:21:42.000000 slack_approval-0.1.7.0/slack_approval.egg-info/PKG-INFO
--rw-r--r--   0 austen.novis   (502) staff       (20)      387 2023-10-04 14:21:42.000000 slack_approval-0.1.7.0/slack_approval.egg-info/SOURCES.txt
--rw-r--r--   0 austen.novis   (502) staff       (20)        1 2023-10-04 14:21:42.000000 slack_approval-0.1.7.0/slack_approval.egg-info/dependency_links.txt
--rw-r--r--   0 austen.novis   (502) staff       (20)       59 2023-10-04 14:21:42.000000 slack_approval-0.1.7.0/slack_approval.egg-info/entry_points.txt
--rw-r--r--   0 austen.novis   (502) staff       (20)       36 2023-10-04 14:21:42.000000 slack_approval-0.1.7.0/slack_approval.egg-info/requires.txt
--rw-r--r--   0 austen.novis   (502) staff       (20)       15 2023-10-04 14:21:42.000000 slack_approval-0.1.7.0/slack_approval.egg-info/top_level.txt
+drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2024-05-03 17:18:24.834142 slack_approval-0.1.7.1/
+-rw-r--r--   0 austennovis   (501) staff       (20)     4978 2024-05-03 17:18:24.833971 slack_approval-0.1.7.1/PKG-INFO
+-rw-r--r--   0 austennovis   (501) staff       (20)     4079 2024-05-03 17:17:57.000000 slack_approval-0.1.7.1/README.md
+-rw-r--r--   0 austennovis   (501) staff       (20)       38 2024-05-03 17:18:24.834173 slack_approval-0.1.7.1/setup.cfg
+-rw-r--r--   0 austennovis   (501) staff       (20)     2828 2024-05-03 17:18:14.000000 slack_approval-0.1.7.1/setup.py
+drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2024-05-03 17:18:24.832988 slack_approval-0.1.7.1/slack_approval/
+-rw-r--r--   0 austennovis   (501) staff       (20)        0 2024-05-03 17:17:57.000000 slack_approval-0.1.7.1/slack_approval/__init__.py
+-rw-r--r--   0 austennovis   (501) staff       (20)      293 2024-05-03 17:17:57.000000 slack_approval-0.1.7.1/slack_approval/cli.py
+-rw-r--r--   0 austennovis   (501) staff       (20)    23192 2024-05-03 17:17:57.000000 slack_approval-0.1.7.1/slack_approval/slack_provision.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     3628 2024-05-03 17:17:57.000000 slack_approval-0.1.7.1/slack_approval/slack_request.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     3603 2024-05-03 17:17:57.000000 slack_approval-0.1.7.1/slack_approval/utils.py
+drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2024-05-03 17:18:24.833658 slack_approval-0.1.7.1/slack_approval.egg-info/
+-rw-r--r--   0 austennovis   (501) staff       (20)     4978 2024-05-03 17:18:24.000000 slack_approval-0.1.7.1/slack_approval.egg-info/PKG-INFO
+-rw-r--r--   0 austennovis   (501) staff       (20)      387 2024-05-03 17:18:24.000000 slack_approval-0.1.7.1/slack_approval.egg-info/SOURCES.txt
+-rw-r--r--   0 austennovis   (501) staff       (20)        1 2024-05-03 17:18:24.000000 slack_approval-0.1.7.1/slack_approval.egg-info/dependency_links.txt
+-rw-r--r--   0 austennovis   (501) staff       (20)       59 2024-05-03 17:18:24.000000 slack_approval-0.1.7.1/slack_approval.egg-info/entry_points.txt
+-rw-r--r--   0 austennovis   (501) staff       (20)       36 2024-05-03 17:18:24.000000 slack_approval-0.1.7.1/slack_approval.egg-info/requires.txt
+-rw-r--r--   0 austennovis   (501) staff       (20)       15 2024-05-03 17:18:24.000000 slack_approval-0.1.7.1/slack_approval.egg-info/top_level.txt
```

### Comparing `slack_approval-0.1.7.0/PKG-INFO` & `slack_approval-0.1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack_approval
-Version: 0.1.7.0
+Version: 0.1.7.1
 Summary: Library for managing and deploying a lightweight approval workflow based on Slack and GCP
 Home-page: https://github.com/premisedata/slack-approval
 Author: Austen
 Author-email: austen.novis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -13,14 +13,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
+Requires-Dist: goblet-gcp>=0.9.2
+Requires-Dist: slack_sdk==3.18.1
 
 
 # slack_approval
 
 ![PyPI](https://img.shields.io/pypi/v/slack_approval?color=blue&style=plastic)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/slack_approval?style=plastic)
```

### Comparing `slack_approval-0.1.7.0/README.md` & `slack_approval-0.1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `slack_approval-0.1.7.0/setup.py` & `slack_approval-0.1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    version="0.1.7.0",
+    version="0.1.7.1",
     license='MIT',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

### Comparing `slack_approval-0.1.7.0/slack_approval/slack_provision.py` & `slack_approval-0.1.7.1/slack_approval/slack_provision.py`

 * *Files identical despite different names*

### Comparing `slack_approval-0.1.7.0/slack_approval/slack_request.py` & `slack_approval-0.1.7.1/slack_approval/slack_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 logger.setLevel(logging.DEBUG)
 
 
 class SlackRequest:
     def __init__(self, request):
         """requesters_channel only necessary for `pending` messages"""
         self.inputs = request.json
-        self.name = self.inputs["provision_class"]
+        if "provision_class_human_readable_name" in self.inputs:
+            self.name = self.inputs["provision_class_human_readable_name"]
+        else:
+            self.name = self.inputs["provision_class"]
         self.value = self.inputs.copy()  # save inputs before hiding anything
         hide = self.inputs.get("hide")
         if hide:
             for field in hide:
                 self.inputs.pop(field, None)
             self.inputs.pop("hide")
         self.token = os.environ.get("SLACK_BOT_TOKEN")
```

### Comparing `slack_approval-0.1.7.0/slack_approval/utils.py` & `slack_approval-0.1.7.1/slack_approval/utils.py`

 * *Files identical despite different names*

### Comparing `slack_approval-0.1.7.0/slack_approval.egg-info/PKG-INFO` & `slack_approval-0.1.7.1/slack_approval.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-approval
-Version: 0.1.7.0
+Version: 0.1.7.1
 Summary: Library for managing and deploying a lightweight approval workflow based on Slack and GCP
 Home-page: https://github.com/premisedata/slack-approval
 Author: Austen
 Author-email: austen.novis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -13,14 +13,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
+Requires-Dist: goblet-gcp>=0.9.2
+Requires-Dist: slack_sdk==3.18.1
 
 
 # slack_approval
 
 ![PyPI](https://img.shields.io/pypi/v/slack_approval?color=blue&style=plastic)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/slack_approval?style=plastic)
```


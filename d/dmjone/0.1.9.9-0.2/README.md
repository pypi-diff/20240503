# Comparing `tmp/dmjone-0.1.9.9.tar.gz` & `tmp/dmjone-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmjone-0.1.9.9.tar", last modified: Mon Apr  8 05:37:43 2024, max compression
+gzip compressed data, was "dmjone-0.2.tar", last modified: Fri May  3 17:21:43 2024, max compression
```

## Comparing `dmjone-0.1.9.9.tar` & `dmjone-0.2.tar`

### file list

```diff
@@ -1,33 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:37:43.979690 dmjone-0.1.9.9/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-08 05:37:39.000000 dmjone-0.1.9.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 05:37:39.000000 dmjone-0.1.9.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    49649 2024-04-08 05:37:43.975690 dmjone-0.1.9.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-04-08 05:37:39.000000 dmjone-0.1.9.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-08 05:37:39.000000 dmjone-0.1.9.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 05:37:43.979690 dmjone-0.1.9.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:37:43.971690 dmjone-0.1.9.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:37:43.971690 dmjone-0.1.9.9/src/dmjone/
--rw-r--r--   0 runner    (1001) docker     (127)    12688 2024-04-08 05:37:39.000000 dmjone-0.1.9.9/src/dmjone/StudentManagementSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-08 05:37:39.000000 dmjone-0.1.9.9/src/dmjone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:37:43.975690 dmjone-0.1.9.9/src/dmjone/aarushi/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-08 05:37:39.000000 dmjone-0.1.9.9/src/dmjone/aarushi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-08 05:37:39.000000 dmjone-0.1.9.9/src/dmjone/aarushi/aarushi_todolist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:37:43.975690 dmjone-0.1.9.9/src/dmjone/anurag/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 05:37:39.000000 dmjone-0.1.9.9/src/dmjone/anurag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-08 05:37:39.000000 dmjone-0.1.9.9/src/dmjone/hello.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:37:43.975690 dmjone-0.1.9.9/src/dmjone/kaustuv/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-08 05:37:39.000000 dmjone-0.1.9.9/src/dmjone/kaustuv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-08 05:37:39.000000 dmjone-0.1.9.9/src/dmjone/kaustuv/kaustuv_common.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-08 05:37:39.000000 dmjone-0.1.9.9/src/dmjone/kaustuv/kaustuv_project.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-08 05:37:39.000000 dmjone-0.1.9.9/src/dmjone/lab4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:37:43.975690 dmjone-0.1.9.9/src/dmjone/lakshika/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-08 05:37:39.000000 dmjone-0.1.9.9/src/dmjone/lakshika/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-08 05:37:39.000000 dmjone-0.1.9.9/src/dmjone/lakshika/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-08 05:37:39.000000 dmjone-0.1.9.9/src/dmjone/lakshika/lakshika_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-08 05:37:39.000000 dmjone-0.1.9.9/src/dmjone/lakshika/typecasting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:37:43.975690 dmjone-0.1.9.9/src/dmjone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    49649 2024-04-08 05:37:43.000000 dmjone-0.1.9.9/src/dmjone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-08 05:37:43.000000 dmjone-0.1.9.9/src/dmjone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 05:37:43.000000 dmjone-0.1.9.9/src/dmjone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-08 05:37:43.000000 dmjone-0.1.9.9/src/dmjone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 05:37:43.000000 dmjone-0.1.9.9/src/dmjone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:21:43.157179 dmjone-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-03 17:21:35.000000 dmjone-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 17:21:35.000000 dmjone-0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    49737 2024-05-03 17:21:43.157179 dmjone-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-05-03 17:21:35.000000 dmjone-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-03 17:21:35.000000 dmjone-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:21:43.157179 dmjone-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:21:43.149179 dmjone-0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:21:43.149179 dmjone-0.2/src/dmjone/
+-rw-r--r--   0 runner    (1001) docker     (127)    12781 2024-05-03 17:21:35.000000 dmjone-0.2/src/dmjone/StudentManagementSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-03 17:21:35.000000 dmjone-0.2/src/dmjone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:21:43.153179 dmjone-0.2/src/dmjone/aarushi/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-03 17:21:35.000000 dmjone-0.2/src/dmjone/aarushi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-03 17:21:35.000000 dmjone-0.2/src/dmjone/aarushi/aarushi_todolist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:21:43.153179 dmjone-0.2/src/dmjone/anurag/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:21:35.000000 dmjone-0.2/src/dmjone/anurag/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:21:43.153179 dmjone-0.2/src/dmjone/gaurav/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:21:35.000000 dmjone-0.2/src/dmjone/gaurav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-03 17:21:35.000000 dmjone-0.2/src/dmjone/hello.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:21:43.153179 dmjone-0.2/src/dmjone/kaustuv/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-03 17:21:35.000000 dmjone-0.2/src/dmjone/kaustuv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-03 17:21:35.000000 dmjone-0.2/src/dmjone/kaustuv/kaustuv_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 17:21:35.000000 dmjone-0.2/src/dmjone/kaustuv/kaustuv_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 17:21:35.000000 dmjone-0.2/src/dmjone/lab4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:21:43.153179 dmjone-0.2/src/dmjone/lakshika/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-03 17:21:35.000000 dmjone-0.2/src/dmjone/lakshika/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-03 17:21:35.000000 dmjone-0.2/src/dmjone/lakshika/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-03 17:21:35.000000 dmjone-0.2/src/dmjone/lakshika/lakshika_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-03 17:21:35.000000 dmjone-0.2/src/dmjone/lakshika/typecasting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:21:43.153179 dmjone-0.2/src/dmjone/team5/
+-rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-05-03 17:21:35.000000 dmjone-0.2/src/dmjone/team5/ashutosh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-05-03 17:21:35.000000 dmjone-0.2/src/dmjone/team5/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:21:43.153179 dmjone-0.2/src/dmjone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    49737 2024-05-03 17:21:43.000000 dmjone-0.2/src/dmjone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-03 17:21:43.000000 dmjone-0.2/src/dmjone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:21:43.000000 dmjone-0.2/src/dmjone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-03 17:21:43.000000 dmjone-0.2/src/dmjone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 17:21:43.000000 dmjone-0.2/src/dmjone.egg-info/top_level.txt
```

### Comparing `dmjone-0.1.9.9/LICENSE` & `dmjone-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.9.9/PKG-INFO` & `dmjone-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmjone
-Version: 0.1.9.9
+Version: 0.2
 Summary: Public Welfare initiatives by dmj.one - Educational Initiative
 Author-email: Divya Mohan <contact@dmj.one>
 Maintainer-email: Aarushi Sharma <aarushi@dmj.one>, Kaustuv Sharma <kaustuv@dmj.one>, Lakshika Tanwar <lakshika@dmj.one>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -773,16 +773,16 @@
 
 ## Highlighted Features and Collaborations
 - **Student Management System**: A simple yet powerful system for managing student records, designed for educational institutions.
 - **Lab Projects**: Access to various educational projects and lab work to facilitate learning and teaching.
 - **Educational Tools**: A collection of tools aimed at enhancing the learning experience.
 
 ## Authors
-- Subject Experts: **Dr. Anurag Rana** [GitHub](https://github.com/AI-ARana) | **Dr. Pankaj Vaidya**
-- **Divya Mohan** - _init_ - [GitHub](https://github.com/divyamohan1993) |  **Lakshika Tanwar** - *Top Contributor* - [GitHub](https://github.com/LakshikaTanwar) | **Aarushi Sharma** - *Contributor* - [GitHub](https://github.com/letscodeitup) | **Kaustuv Sharma** - *Contributor* - [GitHub](https://github.com/kaustuvsharma)
+- Subject Matter Experts: **Dr. Anurag Rana** [GitHub](https://github.com/AI-ARana) | **Dr. Pankaj Vaidya** | **Dr. Gaurav Gupta** [GitHub](https://github.com/solangaurav) 
+- **Divya Mohan** - _init_ - [GitHub](https://github.com/divyamohan1993) |  **Lakshika Tanwar** - *Top Contributor* - [GitHub](https://github.com/LakshikaTanwar) | **Aarushi Sharma** - *Contributor* - [GitHub](https://github.com/letscodeitup) | **Kaustuv Sharma** - *Contributor* - [GitHub](https://github.com/kaustuvsharma) | **Aarchit Joshi**
 - **Anshuman Mohanty** - [GitHub](https://github.com/anshumanmohanty00) | **Ashutosh Rana** | **Jatin Sharma** | **Rijul Chaudhary** - [GitHub](https://github.com/Rijul777) | **Subhojeet Ghosh** [GitHub](https://github.com/subhojeetghosh123) | **Vedansh Sharma** - [GitHub](https://github.com/Elysian-Reverie) | **Yuvraj Kumar** [GitHub](https://github.com/YuvRaj-Kumar-95)
 
 See also the list of [contributors](https://github.com/dmjone/dmjone_pypi/contributors) who participated in this project.
 
 ## How To Contribute
 
 We thank you for your interest in contributing to `dmjone`! 🎉 Your efforts make a big difference. Whether you're fixing a bug, adding a feature, or improving documentation, we appreciate your help. Here’s how to contribute in a friendly and easy way:
```

### Comparing `dmjone-0.1.9.9/README.md` & `dmjone-0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,16 @@
 
 ## Highlighted Features and Collaborations
 - **Student Management System**: A simple yet powerful system for managing student records, designed for educational institutions.
 - **Lab Projects**: Access to various educational projects and lab work to facilitate learning and teaching.
 - **Educational Tools**: A collection of tools aimed at enhancing the learning experience.
 
 ## Authors
-- Subject Experts: **Dr. Anurag Rana** [GitHub](https://github.com/AI-ARana) | **Dr. Pankaj Vaidya**
-- **Divya Mohan** - _init_ - [GitHub](https://github.com/divyamohan1993) |  **Lakshika Tanwar** - *Top Contributor* - [GitHub](https://github.com/LakshikaTanwar) | **Aarushi Sharma** - *Contributor* - [GitHub](https://github.com/letscodeitup) | **Kaustuv Sharma** - *Contributor* - [GitHub](https://github.com/kaustuvsharma)
+- Subject Matter Experts: **Dr. Anurag Rana** [GitHub](https://github.com/AI-ARana) | **Dr. Pankaj Vaidya** | **Dr. Gaurav Gupta** [GitHub](https://github.com/solangaurav) 
+- **Divya Mohan** - _init_ - [GitHub](https://github.com/divyamohan1993) |  **Lakshika Tanwar** - *Top Contributor* - [GitHub](https://github.com/LakshikaTanwar) | **Aarushi Sharma** - *Contributor* - [GitHub](https://github.com/letscodeitup) | **Kaustuv Sharma** - *Contributor* - [GitHub](https://github.com/kaustuvsharma) | **Aarchit Joshi**
 - **Anshuman Mohanty** - [GitHub](https://github.com/anshumanmohanty00) | **Ashutosh Rana** | **Jatin Sharma** | **Rijul Chaudhary** - [GitHub](https://github.com/Rijul777) | **Subhojeet Ghosh** [GitHub](https://github.com/subhojeetghosh123) | **Vedansh Sharma** - [GitHub](https://github.com/Elysian-Reverie) | **Yuvraj Kumar** [GitHub](https://github.com/YuvRaj-Kumar-95)
 
 See also the list of [contributors](https://github.com/dmjone/dmjone_pypi/contributors) who participated in this project.
 
 ## How To Contribute
 
 We thank you for your interest in contributing to `dmjone`! 🎉 Your efforts make a big difference. Whether you're fixing a bug, adding a feature, or improving documentation, we appreciate your help. Here’s how to contribute in a friendly and easy way:
```

### Comparing `dmjone-0.1.9.9/pyproject.toml` & `dmjone-0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmjone"
-version = "0.1.9.9"
+version = "0.2"
 description = "Public Welfare initiatives by dmj.one - Educational Initiative"
 # summary = "A suite of public welfare and educational tools developed by dmj.one, focusing on accessibility and innovation in learning resources."
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     {name = "Divya Mohan", email = "contact@dmj.one"}
 ]
```

### Comparing `dmjone-0.1.9.9/src/dmjone/StudentManagementSystem.py` & `dmjone-0.2/src/dmjone/StudentManagementSystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+###### Saving all iterations for backup. 
+
+#iteration ACTUAL - April 9th, 2024 02:31 PM
+
 # Run when dmjone.projectsms() is called
 
 def projectsms():
     import mysql.connector
     import getpass
     import random
     import os
```

### Comparing `dmjone-0.1.9.9/src/dmjone/__init__.py` & `dmjone-0.2/src/dmjone/__init__.py`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.9.9/src/dmjone/aarushi/aarushi_todolist.py` & `dmjone-0.2/src/dmjone/aarushi/aarushi_todolist.py`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.9.9/src/dmjone/lakshika/lakshika_functions.py` & `dmjone-0.2/src/dmjone/lakshika/lakshika_functions.py`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.9.9/src/dmjone.egg-info/PKG-INFO` & `dmjone-0.2/src/dmjone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmjone
-Version: 0.1.9.9
+Version: 0.2
 Summary: Public Welfare initiatives by dmj.one - Educational Initiative
 Author-email: Divya Mohan <contact@dmj.one>
 Maintainer-email: Aarushi Sharma <aarushi@dmj.one>, Kaustuv Sharma <kaustuv@dmj.one>, Lakshika Tanwar <lakshika@dmj.one>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -773,16 +773,16 @@
 
 ## Highlighted Features and Collaborations
 - **Student Management System**: A simple yet powerful system for managing student records, designed for educational institutions.
 - **Lab Projects**: Access to various educational projects and lab work to facilitate learning and teaching.
 - **Educational Tools**: A collection of tools aimed at enhancing the learning experience.
 
 ## Authors
-- Subject Experts: **Dr. Anurag Rana** [GitHub](https://github.com/AI-ARana) | **Dr. Pankaj Vaidya**
-- **Divya Mohan** - _init_ - [GitHub](https://github.com/divyamohan1993) |  **Lakshika Tanwar** - *Top Contributor* - [GitHub](https://github.com/LakshikaTanwar) | **Aarushi Sharma** - *Contributor* - [GitHub](https://github.com/letscodeitup) | **Kaustuv Sharma** - *Contributor* - [GitHub](https://github.com/kaustuvsharma)
+- Subject Matter Experts: **Dr. Anurag Rana** [GitHub](https://github.com/AI-ARana) | **Dr. Pankaj Vaidya** | **Dr. Gaurav Gupta** [GitHub](https://github.com/solangaurav) 
+- **Divya Mohan** - _init_ - [GitHub](https://github.com/divyamohan1993) |  **Lakshika Tanwar** - *Top Contributor* - [GitHub](https://github.com/LakshikaTanwar) | **Aarushi Sharma** - *Contributor* - [GitHub](https://github.com/letscodeitup) | **Kaustuv Sharma** - *Contributor* - [GitHub](https://github.com/kaustuvsharma) | **Aarchit Joshi**
 - **Anshuman Mohanty** - [GitHub](https://github.com/anshumanmohanty00) | **Ashutosh Rana** | **Jatin Sharma** | **Rijul Chaudhary** - [GitHub](https://github.com/Rijul777) | **Subhojeet Ghosh** [GitHub](https://github.com/subhojeetghosh123) | **Vedansh Sharma** - [GitHub](https://github.com/Elysian-Reverie) | **Yuvraj Kumar** [GitHub](https://github.com/YuvRaj-Kumar-95)
 
 See also the list of [contributors](https://github.com/dmjone/dmjone_pypi/contributors) who participated in this project.
 
 ## How To Contribute
 
 We thank you for your interest in contributing to `dmjone`! 🎉 Your efforts make a big difference. Whether you're fixing a bug, adding a feature, or improving documentation, we appreciate your help. Here’s how to contribute in a friendly and easy way:
```

### Comparing `dmjone-0.1.9.9/src/dmjone.egg-info/SOURCES.txt` & `dmjone-0.2/src/dmjone.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 src/dmjone.egg-info/SOURCES.txt
 src/dmjone.egg-info/dependency_links.txt
 src/dmjone.egg-info/requires.txt
 src/dmjone.egg-info/top_level.txt
 src/dmjone/aarushi/__init__.py
 src/dmjone/aarushi/aarushi_todolist.py
 src/dmjone/anurag/__init__.py
+src/dmjone/gaurav/__init__.py
 src/dmjone/kaustuv/__init__.py
 src/dmjone/kaustuv/kaustuv_common.py
 src/dmjone/kaustuv/kaustuv_project.py
 src/dmjone/lakshika/__init__.py
 src/dmjone/lakshika/calculator.py
 src/dmjone/lakshika/lakshika_functions.py
-src/dmjone/lakshika/typecasting.py
+src/dmjone/lakshika/typecasting.py
+src/dmjone/team5/ashutosh.py
+src/dmjone/team5/test.py
```


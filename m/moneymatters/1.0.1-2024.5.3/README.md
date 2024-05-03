# Comparing `tmp/moneymatters-1.0.1.tar.gz` & `tmp/moneymatters-2024.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneymatters-1.0.1.tar", last modified: Tue Apr 30 12:25:30 2024, max compression
+gzip compressed data, was "moneymatters-2024.5.3.tar", last modified: Fri May  3 07:57:21 2024, max compression
```

## Comparing `moneymatters-1.0.1.tar` & `moneymatters-2024.5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-04-30 12:25:30.733324 moneymatters-1.0.1/
--rw-r--r--   0 gkoduri    (502) staff       (20)    34523 2024-04-30 09:29:22.000000 moneymatters-1.0.1/LICENSE
--rw-r--r--   0 gkoduri    (502) staff       (20)       33 2024-04-30 11:08:59.000000 moneymatters-1.0.1/MANIFEST.in
--rw-r--r--   0 gkoduri    (502) staff       (20)     3648 2024-04-30 12:25:30.733112 moneymatters-1.0.1/PKG-INFO
--rw-r--r--   0 gkoduri    (502) staff       (20)     2430 2024-04-30 11:07:29.000000 moneymatters-1.0.1/README.md
-drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-04-30 12:25:30.732083 moneymatters-1.0.1/moneymatters/
--rw-r--r--   0 gkoduri    (502) staff       (20)        0 2024-04-30 12:24:53.000000 moneymatters-1.0.1/moneymatters/__init__.py
--rw-r--r--   0 gkoduri    (502) staff       (20)     5929 2024-04-30 10:57:41.000000 moneymatters-1.0.1/moneymatters/api.py
-drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-04-30 12:25:30.732889 moneymatters-1.0.1/moneymatters.egg-info/
--rw-r--r--   0 gkoduri    (502) staff       (20)     3648 2024-04-30 12:25:30.000000 moneymatters-1.0.1/moneymatters.egg-info/PKG-INFO
--rw-r--r--   0 gkoduri    (502) staff       (20)      262 2024-04-30 12:25:30.000000 moneymatters-1.0.1/moneymatters.egg-info/SOURCES.txt
--rw-r--r--   0 gkoduri    (502) staff       (20)        1 2024-04-30 12:25:30.000000 moneymatters-1.0.1/moneymatters.egg-info/dependency_links.txt
--rw-r--r--   0 gkoduri    (502) staff       (20)       42 2024-04-30 12:25:30.000000 moneymatters-1.0.1/moneymatters.egg-info/requires.txt
--rw-r--r--   0 gkoduri    (502) staff       (20)       13 2024-04-30 12:25:30.000000 moneymatters-1.0.1/moneymatters.egg-info/top_level.txt
--rw-r--r--   0 gkoduri    (502) staff       (20)       38 2024-04-30 12:25:30.733362 moneymatters-1.0.1/setup.cfg
--rw-r--r--   0 gkoduri    (502) staff       (20)     1492 2024-04-30 12:25:26.000000 moneymatters-1.0.1/setup.py
+drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-03 07:57:21.217370 moneymatters-2024.5.3/
+-rw-r--r--   0 gkoduri    (502) staff       (20)    34523 2024-04-30 09:29:22.000000 moneymatters-2024.5.3/LICENSE
+-rw-r--r--   0 gkoduri    (502) staff       (20)       33 2024-04-30 11:08:59.000000 moneymatters-2024.5.3/MANIFEST.in
+-rw-r--r--   0 gkoduri    (502) staff       (20)     3641 2024-05-03 07:57:21.217142 moneymatters-2024.5.3/PKG-INFO
+-rw-r--r--   0 gkoduri    (502) staff       (20)     2426 2024-05-03 07:56:04.000000 moneymatters-2024.5.3/README.md
+drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-03 07:57:21.215688 moneymatters-2024.5.3/moneymatters/
+-rw-r--r--   0 gkoduri    (502) staff       (20)        0 2024-04-30 12:24:53.000000 moneymatters-2024.5.3/moneymatters/__init__.py
+-rw-r--r--   0 gkoduri    (502) staff       (20)     5929 2024-04-30 10:57:41.000000 moneymatters-2024.5.3/moneymatters/api.py
+drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-03 07:57:21.216891 moneymatters-2024.5.3/moneymatters.egg-info/
+-rw-r--r--   0 gkoduri    (502) staff       (20)     3641 2024-05-03 07:57:21.000000 moneymatters-2024.5.3/moneymatters.egg-info/PKG-INFO
+-rw-r--r--   0 gkoduri    (502) staff       (20)      262 2024-05-03 07:57:21.000000 moneymatters-2024.5.3/moneymatters.egg-info/SOURCES.txt
+-rw-r--r--   0 gkoduri    (502) staff       (20)        1 2024-05-03 07:57:21.000000 moneymatters-2024.5.3/moneymatters.egg-info/dependency_links.txt
+-rw-r--r--   0 gkoduri    (502) staff       (20)       42 2024-05-03 07:57:21.000000 moneymatters-2024.5.3/moneymatters.egg-info/requires.txt
+-rw-r--r--   0 gkoduri    (502) staff       (20)       13 2024-05-03 07:57:21.000000 moneymatters-2024.5.3/moneymatters.egg-info/top_level.txt
+-rw-r--r--   0 gkoduri    (502) staff       (20)       38 2024-05-03 07:57:21.217410 moneymatters-2024.5.3/setup.cfg
+-rw-r--r--   0 gkoduri    (502) staff       (20)     1491 2024-05-03 07:54:57.000000 moneymatters-2024.5.3/setup.py
```

### Comparing `moneymatters-1.0.1/LICENSE` & `moneymatters-2024.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `moneymatters-1.0.1/PKG-INFO` & `moneymatters-2024.5.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: moneymatters
-Version: 1.0.1
+Version: 2024.5.3
 Summary: A Python package that encompasses money related stuff into one package - money formatting, currency conversion etc
-Home-page: https://github.com/gopalkoduri/moneymatters
+Home-page: https://github.com/musicmuni/moneymatters
 Author: Gopala Krishna Koduri
 Author-email: gopal@riyazapp.com
-Project-URL: Source Code, https://github.com/gopalkoduri/moneymatters
-Project-URL: Issue Tracker, https://github.com/gopalkoduri/moneymatters/issues
+Project-URL: Source Code, https://github.com/musicmuni/moneymatters
+Project-URL: Issue Tracker, https://github.com/musicmuni/moneymatters/issues
 Project-URL: Connect w/ Author, https://linkedin.com/in/gopalkoduri
 Project-URL: Riyaz - Learn to sing, https://riyazapp.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -88,15 +88,15 @@
 
 This project is licensed under the Affero GNU Public License v3 - see the [LICENSE](LICENSE) file for details.
 
 ## Contact
 
 - **Author**: Gopala Krishna Koduri
 - **Email**: [gopal@riyazapp.com](mailto:gopal@riyazapp.com)
-- [GitHub Repository](https://github.com/gopalkoduri/moneymatters)
-- [Issue Tracker](https://github.com/gopalkoduri/moneymatters/issues)
+- [GitHub Repository](https://github.com/musicmuni/moneymatters)
+- [Issue Tracker](https://github.com/musicmuni/moneymatters/issues)
 - [LinkedIn](https://linkedin.com/in/gopalkoduri)
 - [Learn to Sing with Riyaz App](https://riyazapp.com)
 
 ## Acknowledgments
 
 Thanks to all contributors who have helped shape MoneyMatters, making it easier to deal with currency related stuff for developers around the globe.
```

### Comparing `moneymatters-1.0.1/README.md` & `moneymatters-2024.5.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 This project is licensed under the Affero GNU Public License v3 - see the [LICENSE](LICENSE) file for details.
 
 ## Contact
 
 - **Author**: Gopala Krishna Koduri
 - **Email**: [gopal@riyazapp.com](mailto:gopal@riyazapp.com)
-- [GitHub Repository](https://github.com/gopalkoduri/moneymatters)
-- [Issue Tracker](https://github.com/gopalkoduri/moneymatters/issues)
+- [GitHub Repository](https://github.com/musicmuni/moneymatters)
+- [Issue Tracker](https://github.com/musicmuni/moneymatters/issues)
 - [LinkedIn](https://linkedin.com/in/gopalkoduri)
 - [Learn to Sing with Riyaz App](https://riyazapp.com)
 
 ## Acknowledgments
 
 Thanks to all contributors who have helped shape MoneyMatters, making it easier to deal with currency related stuff for developers around the globe.
```

### Comparing `moneymatters-1.0.1/moneymatters/api.py` & `moneymatters-2024.5.3/moneymatters/api.py`

 * *Files identical despite different names*

### Comparing `moneymatters-1.0.1/moneymatters.egg-info/PKG-INFO` & `moneymatters-2024.5.3/moneymatters.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: moneymatters
-Version: 1.0.1
+Version: 2024.5.3
 Summary: A Python package that encompasses money related stuff into one package - money formatting, currency conversion etc
-Home-page: https://github.com/gopalkoduri/moneymatters
+Home-page: https://github.com/musicmuni/moneymatters
 Author: Gopala Krishna Koduri
 Author-email: gopal@riyazapp.com
-Project-URL: Source Code, https://github.com/gopalkoduri/moneymatters
-Project-URL: Issue Tracker, https://github.com/gopalkoduri/moneymatters/issues
+Project-URL: Source Code, https://github.com/musicmuni/moneymatters
+Project-URL: Issue Tracker, https://github.com/musicmuni/moneymatters/issues
 Project-URL: Connect w/ Author, https://linkedin.com/in/gopalkoduri
 Project-URL: Riyaz - Learn to sing, https://riyazapp.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -88,15 +88,15 @@
 
 This project is licensed under the Affero GNU Public License v3 - see the [LICENSE](LICENSE) file for details.
 
 ## Contact
 
 - **Author**: Gopala Krishna Koduri
 - **Email**: [gopal@riyazapp.com](mailto:gopal@riyazapp.com)
-- [GitHub Repository](https://github.com/gopalkoduri/moneymatters)
-- [Issue Tracker](https://github.com/gopalkoduri/moneymatters/issues)
+- [GitHub Repository](https://github.com/musicmuni/moneymatters)
+- [Issue Tracker](https://github.com/musicmuni/moneymatters/issues)
 - [LinkedIn](https://linkedin.com/in/gopalkoduri)
 - [Learn to Sing with Riyaz App](https://riyazapp.com)
 
 ## Acknowledgments
 
 Thanks to all contributors who have helped shape MoneyMatters, making it easier to deal with currency related stuff for developers around the globe.
```

### Comparing `moneymatters-1.0.1/setup.py` & `moneymatters-2024.5.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name="moneymatters",
-    version="1.0.1",
+    version="2024.05.03",
     description="A Python package that encompasses money related stuff into one package - money formatting, currency conversion etc",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",  # Ensure you include a README.md in your package
     author="Gopala Krishna Koduri",
     author_email="gopal@riyazapp.com",
-    url="https://github.com/gopalkoduri/moneymatters",  # Company URL
+    url="https://github.com/musicmuni/moneymatters",  # Company URL
     project_urls={  # Additional URLs
-        "Source Code": "https://github.com/gopalkoduri/moneymatters",
-        "Issue Tracker": "https://github.com/gopalkoduri/moneymatters/issues",
+        "Source Code": "https://github.com/musicmuni/moneymatters",
+        "Issue Tracker": "https://github.com/musicmuni/moneymatters/issues",
         "Connect w/ Author": "https://linkedin.com/in/gopalkoduri",
         "Riyaz - Learn to sing": "https://riyazapp.com",
     },
     packages=find_packages(),
     include_package_data=True,
     install_requires=["CurrencyConverter", "requests", "beautifulsoup4"],
     classifiers=[
```


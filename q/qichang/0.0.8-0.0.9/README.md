# Comparing `tmp/qichang-0.0.8.tar.gz` & `tmp/qichang-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qichang-0.0.8.tar", last modified: Mon Nov 13 00:40:21 2023, max compression
+gzip compressed data, was "qichang-0.0.9.tar", last modified: Mon Nov 13 00:41:50 2023, max compression
```

## Comparing `qichang-0.0.8.tar` & `qichang-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-11-13 00:40:21.870916 qichang-0.0.8/
--rw-rw-rw-   0        0        0    11558 2023-11-12 10:38:04.000000 qichang-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1046 2023-11-13 00:40:21.870916 qichang-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-11-12 09:47:02.000000 qichang-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-11-13 00:40:21.862917 qichang-0.0.8/qichang/
--rw-rw-rw-   0        0        0       22 2023-11-13 00:26:47.000000 qichang-0.0.8/qichang/__init__.py
--rw-rw-rw-   0        0        0     3738 2023-11-13 00:40:17.000000 qichang-0.0.8/qichang/qichang.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:40:21.869916 qichang-0.0.8/qichang.egg-info/
--rw-rw-rw-   0        0        0     1046 2023-11-13 00:40:21.000000 qichang-0.0.8/qichang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-11-13 00:40:21.000000 qichang-0.0.8/qichang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-13 00:40:21.000000 qichang-0.0.8/qichang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-11-13 00:40:21.000000 qichang-0.0.8/qichang.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-11-13 00:40:21.000000 qichang-0.0.8/qichang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-13 00:40:21.870916 qichang-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1170 2023-11-13 00:27:54.000000 qichang-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-13 00:41:50.735857 qichang-0.0.9/
+-rw-rw-rw-   0        0        0    11558 2023-11-12 10:38:04.000000 qichang-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1046 2023-11-13 00:41:50.734856 qichang-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-11-12 09:47:02.000000 qichang-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-11-13 00:41:50.727855 qichang-0.0.9/qichang/
+-rw-rw-rw-   0        0        0       22 2023-11-13 00:26:47.000000 qichang-0.0.9/qichang/__init__.py
+-rw-rw-rw-   0        0        0     3738 2023-11-13 00:41:43.000000 qichang-0.0.9/qichang/qichang.py
+drwxrwxrwx   0        0        0        0 2023-11-13 00:41:50.734856 qichang-0.0.9/qichang.egg-info/
+-rw-rw-rw-   0        0        0     1046 2023-11-13 00:41:50.000000 qichang-0.0.9/qichang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-11-13 00:41:50.000000 qichang-0.0.9/qichang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-13 00:41:50.000000 qichang-0.0.9/qichang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-11-13 00:41:50.000000 qichang-0.0.9/qichang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-11-13 00:41:50.000000 qichang-0.0.9/qichang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-11-13 00:41:50.735857 qichang-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1170 2023-11-13 00:27:54.000000 qichang-0.0.9/setup.py
```

### Comparing `qichang-0.0.8/LICENSE` & `qichang-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qichang-0.0.8/PKG-INFO` & `qichang-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qichang
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python library for interacting with various language model APIs
 Home-page: https://github.com/QichangZheng/qichang.git
 Author: Qichang Zheng
 Author-email: qichangzheng@uchicago.edu
 License: Apache License 2.0
 Keywords: language models API client
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `qichang-0.0.8/qichang/qichang.py` & `qichang-0.0.9/qichang/qichang.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 This is a personal API developed by Qichang Zheng. If you have any questions, please feel free to contact me via email.
 """
 
 import requests
 from time import sleep
 from ping3 import ping
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 
 app_api_dict = {
     "GPT3.5": 'fastgpt-ZadxgXx4pZV4OqSyi7dcYHambSq',
     'GPT4': 'fastgpt-BmDbL0SAmNUcyrRxDK5SF3lApP',
     'stock_api': 'fastgpt-lmiAMrgderiIfidhxQ5HVOD6PJIr3ntpxO4',
     'shannon_test1': 'fastgpt-I8yveuOpvtf5NNjCc4feXkscEQGiKxwH3J'
 }
```

### Comparing `qichang-0.0.8/qichang.egg-info/PKG-INFO` & `qichang-0.0.9/qichang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qichang
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python library for interacting with various language model APIs
 Home-page: https://github.com/QichangZheng/qichang.git
 Author: Qichang Zheng
 Author-email: qichangzheng@uchicago.edu
 License: Apache License 2.0
 Keywords: language models API client
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `qichang-0.0.8/setup.py` & `qichang-0.0.9/setup.py`

 * *Files identical despite different names*


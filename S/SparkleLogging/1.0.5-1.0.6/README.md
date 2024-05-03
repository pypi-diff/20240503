# Comparing `tmp/SparkleLogging-1.0.5.tar.gz` & `tmp/SparkleLogging-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SparkleLogging-1.0.5.tar", last modified: Thu May  2 17:17:55 2024, max compression
+gzip compressed data, was "SparkleLogging-1.0.6.tar", last modified: Fri May  3 03:56:55 2024, max compression
```

## Comparing `SparkleLogging-1.0.5.tar` & `SparkleLogging-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 17:17:55.482156 SparkleLogging-1.0.5/
--rw-rw-rw-   0        0        0     2938 2024-05-02 17:17:55.481156 SparkleLogging-1.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 17:17:55.455514 SparkleLogging-1.0.5/SparkleLogging/
--rw-rw-rw-   0        0        0        0 2024-05-01 12:32:10.000000 SparkleLogging-1.0.5/SparkleLogging/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 17:17:55.474172 SparkleLogging-1.0.5/SparkleLogging/plugins/
--rw-rw-rw-   0        0        0      450 2024-02-21 07:45:12.000000 SparkleLogging-1.0.5/SparkleLogging/plugins/DecoratorsTools.py
--rw-rw-rw-   0        0        0     1160 2024-02-20 08:39:34.000000 SparkleLogging-1.0.5/SparkleLogging/plugins/HttpHander.py
--rw-rw-rw-   0        0        0        0 2024-02-20 09:06:56.000000 SparkleLogging-1.0.5/SparkleLogging/plugins/__init__.py
--rw-rw-rw-   0        0        0      954 2024-02-18 04:21:24.000000 SparkleLogging-1.0.5/SparkleLogging/plugins/websocketHander.py
-drwxrwxrwx   0        0        0        0 2024-05-02 17:17:55.478164 SparkleLogging-1.0.5/SparkleLogging/utils/
--rw-rw-rw-   0        0        0        0 2024-04-30 09:33:18.000000 SparkleLogging-1.0.5/SparkleLogging/utils/__init__.py
--rw-rw-rw-   0        0        0      445 2024-05-02 17:04:22.000000 SparkleLogging-1.0.5/SparkleLogging/utils/core.py
--rw-rw-rw-   0        0        0     5056 2024-05-02 17:16:55.000000 SparkleLogging-1.0.5/SparkleLogging/utils/getLog.py
--rw-rw-rw-   0        0        0      372 2024-05-01 05:44:51.000000 SparkleLogging-1.0.5/SparkleLogging/utils/plugins_for_core.py
-drwxrwxrwx   0        0        0        0 2024-05-02 17:17:55.480161 SparkleLogging-1.0.5/SparkleLogging.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-05-02 17:17:55.000000 SparkleLogging-1.0.5/SparkleLogging.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2024-05-02 17:17:55.000000 SparkleLogging-1.0.5/SparkleLogging.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 17:17:55.000000 SparkleLogging-1.0.5/SparkleLogging.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-02 17:17:55.000000 SparkleLogging-1.0.5/SparkleLogging.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-02 17:17:55.000000 SparkleLogging-1.0.5/SparkleLogging.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 17:17:55.483152 SparkleLogging-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      724 2024-05-02 17:17:53.000000 SparkleLogging-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:56:55.313408 SparkleLogging-1.0.6/
+-rw-rw-rw-   0        0        0     3015 2024-05-03 03:56:55.312411 SparkleLogging-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 03:56:55.207569 SparkleLogging-1.0.6/SparkleLogging/
+-rw-rw-rw-   0        0        0        0 2024-05-01 12:32:10.000000 SparkleLogging-1.0.6/SparkleLogging/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:56:55.307422 SparkleLogging-1.0.6/SparkleLogging/plugins/
+-rw-rw-rw-   0        0        0      450 2024-02-21 07:45:12.000000 SparkleLogging-1.0.6/SparkleLogging/plugins/DecoratorsTools.py
+-rw-rw-rw-   0        0        0     1160 2024-02-20 08:39:34.000000 SparkleLogging-1.0.6/SparkleLogging/plugins/HttpHander.py
+-rw-rw-rw-   0        0        0        0 2024-02-20 09:06:56.000000 SparkleLogging-1.0.6/SparkleLogging/plugins/__init__.py
+-rw-rw-rw-   0        0        0      954 2024-02-18 04:21:24.000000 SparkleLogging-1.0.6/SparkleLogging/plugins/websocketHander.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:56:55.310415 SparkleLogging-1.0.6/SparkleLogging/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-30 09:33:18.000000 SparkleLogging-1.0.6/SparkleLogging/utils/__init__.py
+-rw-rw-rw-   0        0        0      500 2024-05-03 03:54:03.000000 SparkleLogging-1.0.6/SparkleLogging/utils/core.py
+-rw-rw-rw-   0        0        0     4725 2024-05-03 03:53:37.000000 SparkleLogging-1.0.6/SparkleLogging/utils/getLog.py
+-rw-rw-rw-   0        0        0      372 2024-05-01 05:44:51.000000 SparkleLogging-1.0.6/SparkleLogging/utils/plugins_for_core.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:56:55.311414 SparkleLogging-1.0.6/SparkleLogging.egg-info/
+-rw-rw-rw-   0        0        0     3015 2024-05-03 03:56:54.000000 SparkleLogging-1.0.6/SparkleLogging.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2024-05-03 03:56:55.000000 SparkleLogging-1.0.6/SparkleLogging.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 03:56:54.000000 SparkleLogging-1.0.6/SparkleLogging.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-03 03:56:54.000000 SparkleLogging-1.0.6/SparkleLogging.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-03 03:56:54.000000 SparkleLogging-1.0.6/SparkleLogging.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 03:56:55.313408 SparkleLogging-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      724 2024-05-03 03:56:41.000000 SparkleLogging-1.0.6/setup.py
```

### Comparing `SparkleLogging-1.0.5/PKG-INFO` & `SparkleLogging-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SparkleLogging
-Version: 1.0.5
+Version: 1.0.6
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/SparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -82,7 +82,11 @@
 # 2024/5/3 1:05
 
 更新了一个默认日志记录器
 
 # 2024/5/3 1:17
 
 修复了一个bug
+
+# 2024/5/3 11:54
+
+更改了core.py文件,让其导入可以直接使用
```

### Comparing `SparkleLogging-1.0.5/SparkleLogging/plugins/HttpHander.py` & `SparkleLogging-1.0.6/SparkleLogging/plugins/HttpHander.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.5/SparkleLogging/plugins/websocketHander.py` & `SparkleLogging-1.0.6/SparkleLogging/plugins/websocketHander.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.5/SparkleLogging/utils/getLog.py` & `SparkleLogging-1.0.6/SparkleLogging/utils/getLog.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 from SparkleLogging.utils.plugins_for_core import *
 
-FOMATTER = logging.Formatter(
+# 建议不要改这个地方
+DEFAUIT_FOMATTER = logging.Formatter(
     fmt='[%(asctime)s.%(msecs)d| %(levelname)-8s |%(threadName)s|%(name)s.%(funcName)s|%(filename)s:%(lineno)d]: %(message)s',
     datefmt='%Y-%m-%d %H:%M:%S'
 )
 
 class LogManager:
     def __init__(self) -> None:
-        self.public_formatter = logging.Formatter(
-            fmt='[%(asctime)s.%(msecs)d| %(levelname)-8s |%(threadName)s|%(name)s.%(funcName)s|%(filename)s:%(lineno)d]: %(message)s',
-            datefmt='%Y-%m-%d %H:%M:%S'
-        )
+        self.public_formatter = DEFAUIT_FOMATTER
 
     def GetLogger(self, log_name: str = "default",
                   setConsoleLevel: int = logging.DEBUG,
                   setFileLevel: int = logging.INFO,
                   setWebsocketLevel: int = logging.INFO,
                   setHTTPLevel: int = logging.INFO,
                   out_to_console: bool = True,
                   web_log_mode: bool = False,
                   WSpost_url: str = "",
                   HTTPpost_url: str = "",
                   http_mode: bool = False,
-                  custom_formatter: logging.Formatter = logging.Formatter(
-            fmt='[%(asctime)s.%(msecs)d| %(levelname)-8s |%(threadName)s|%(name)s.%(funcName)s|%(filename)s:%(lineno)d]: %(message)s',
-            datefmt='%Y-%m-%d %H:%M:%S'
-        )):
+                  custom_formatter: logging.Formatter = DEFAUIT_FOMATTER
+        ):
         # 确保日志名称有效
         log_name = log_name if log_name else "default"
         if out_to_console:
             log_folder = f'./logs/{log_name}'
             if not os.path.exists(log_folder):
                 os.makedirs(log_folder, exist_ok=True)
```

### Comparing `SparkleLogging-1.0.5/SparkleLogging.egg-info/PKG-INFO` & `SparkleLogging-1.0.6/SparkleLogging.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SparkleLogging
-Version: 1.0.5
+Version: 1.0.6
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/SparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -82,7 +82,11 @@
 # 2024/5/3 1:05
 
 更新了一个默认日志记录器
 
 # 2024/5/3 1:17
 
 修复了一个bug
+
+# 2024/5/3 11:54
+
+更改了core.py文件,让其导入可以直接使用
```

### Comparing `SparkleLogging-1.0.5/SparkleLogging.egg-info/SOURCES.txt` & `SparkleLogging-1.0.6/SparkleLogging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.5/setup.py` & `SparkleLogging-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SparkleLogging',
-    version='1.0.5',
+    version='1.0.6',
     packages=find_packages(),
     author='花火official',
     author_email='3072252442@qq.com',
     description='A logging library for Python',
     long_description=open('Readme.md','r',encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KOKOMI12345/SparkleLogging',
```


# Comparing `tmp/PJYSDK-1.0.5.tar.gz` & `tmp/pjysdk-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PJYSDK-1.0.5.tar", last modified: Sat Mar 16 16:50:07 2024, max compression
+gzip compressed data, was "pjysdk-1.0.6.tar", last modified: Fri May  3 17:04:02 2024, max compression
```

## Comparing `PJYSDK-1.0.5.tar` & `pjysdk-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-16 16:50:07.601337 PJYSDK-1.0.5/
--rw-rw-rw-   0        0        0     1084 2022-03-20 14:14:39.000000 PJYSDK-1.0.5/LICENSE
-drwxrwxrwx   0        0        0        0 2024-03-16 16:50:07.583364 PJYSDK-1.0.5/PJYSDK/
--rw-rw-rw-   0        0        0    19695 2024-03-16 16:07:35.000000 PJYSDK-1.0.5/PJYSDK/PJYSDK.py
--rw-rw-rw-   0        0        0       23 2022-03-20 15:13:08.000000 PJYSDK-1.0.5/PJYSDK/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-16 16:50:07.597794 PJYSDK-1.0.5/PJYSDK.egg-info/
--rw-rw-rw-   0        0        0      633 2024-03-16 16:50:07.000000 PJYSDK-1.0.5/PJYSDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2024-03-16 16:50:07.000000 PJYSDK-1.0.5/PJYSDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-16 16:50:07.000000 PJYSDK-1.0.5/PJYSDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-03-16 16:50:07.000000 PJYSDK-1.0.5/PJYSDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-16 16:50:07.000000 PJYSDK-1.0.5/PJYSDK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      633 2024-03-16 16:50:07.599388 PJYSDK-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      114 2022-03-20 15:21:10.000000 PJYSDK-1.0.5/README.md
--rw-rw-rw-   0        0        0      106 2024-03-16 16:43:02.000000 PJYSDK-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-16 16:50:07.601348 PJYSDK-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      977 2024-03-16 16:13:22.000000 PJYSDK-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 17:04:02.163608 pjysdk-1.0.6/
+-rw-rw-rw-   0        0        0     1084 2022-03-20 14:14:39.000000 pjysdk-1.0.6/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-03 17:04:02.149640 pjysdk-1.0.6/PJYSDK/
+-rw-rw-rw-   0        0        0    19866 2024-05-03 14:15:06.000000 pjysdk-1.0.6/PJYSDK/PJYSDK.py
+-rw-rw-rw-   0        0        0       23 2022-03-20 15:13:08.000000 pjysdk-1.0.6/PJYSDK/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 17:04:02.161252 pjysdk-1.0.6/PJYSDK.egg-info/
+-rw-rw-rw-   0        0        0      633 2024-05-03 17:04:02.000000 pjysdk-1.0.6/PJYSDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2024-05-03 17:04:02.000000 pjysdk-1.0.6/PJYSDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 17:04:02.000000 pjysdk-1.0.6/PJYSDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-03 17:04:02.000000 pjysdk-1.0.6/PJYSDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-03 17:04:02.000000 pjysdk-1.0.6/PJYSDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      633 2024-05-03 17:04:02.162577 pjysdk-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      114 2022-03-20 15:21:10.000000 pjysdk-1.0.6/README.md
+-rw-rw-rw-   0        0        0      106 2024-03-16 16:43:02.000000 pjysdk-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 17:04:02.164112 pjysdk-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      977 2024-05-03 17:03:11.000000 pjysdk-1.0.6/setup.py
```

### Comparing `PJYSDK-1.0.5/LICENSE` & `pjysdk-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PJYSDK-1.0.5/PJYSDK/PJYSDK.py` & `pjysdk-1.0.6/PJYSDK/PJYSDK.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,17 +53,17 @@
             if is_stop:
                 break
 
 
 class PJYSDK(object):
     def __init__(self, app_key, app_secret):
         self.debug = True
-        self._lib_version = 'v1.0.5'
+        self._lib_version = 'v1.0.6'
         self._protocol = 'http'
-        self._hosts = ['api3.paojiaoyun.com', 'api2.paojiaoyun.com', 'api.paojiaoyun.com']
+        self._hosts = ['api3.paojiaoyun.com', 'api6.paojiaoyun.com', 'api.paojiaoyun.com', 'api2.paojiaoyun.com']
         self._host = self._hosts[0]
         self._device_id = ''
         self._retry_count = 9
         self._switch_count = 0
         self._timeout = 5
         
         self._app_key = app_key
@@ -79,15 +79,15 @@
             card_type='',
             expires='',
             expires_ts=0,
             config='',
         )
 
         self._auto_heartbeat = True  # 是否自动开启心跳任务
-        self._heartbeat_gap = 120  # 默认120秒
+        self._heartbeat_gap = 10*60  # 默认10分钟
         self._heartbeat_task = None
         self._heartbeat_ret = DotDict({'code': -9, 'message': u'还未开始验证'})
         self.on_heartbeat_failed = lambda ret: print(ret.message)  # 心跳失败回调函数 自定义
 
         self._prev_nonce = None
         self._is_ping = False
     
@@ -145,17 +145,17 @@
             logger.info("api连接成功")
             self._is_ping = True
         except Exception as e:
             self.switch_host()
 
     @staticmethod
     def retry_fib(num):
-        if num > 9:
-            return 34
-        a, b = 0, 1
+        if num > 5:
+            return 55
+        a, b = 3, 5
         for i in range(0, num):
             tmp = a + b
             a = b
             b = tmp
         return a
 
     @staticmethod
@@ -284,14 +284,15 @@
         method = 'POST'
         path = '/v1/card/login'
         data = {'card': self._card, 'device_id': self._device_id}
         ret = self.request(method, path, data)
         if ret.code == 0:
             self._token = ret.result.token
             self.login_result = ret.result
+            self._heartbeat_gap = ret.result.hg
             if self._auto_heartbeat:
                 self._start_heartbeat(self.card_heartbeat)
         return ret
 
     def card_heartbeat(self):  # 卡密心跳
         if self._token in (None, ''):
             return DotDict({'code': -2, 'message': u'请在卡密登录成功后调用'})
@@ -369,14 +370,15 @@
         method = 'POST'
         path = '/v1/user/login'
         data = {'username': self._username, 'password': self._password, 'device_id': self._device_id}
         ret = self.request(method, path, data)
         if ret.code == 0:
             self._token = ret.result.token
             self.login_result = ret.result
+            self._heartbeat_gap = ret.result.hg
             if self._auto_heartbeat:
                 self._start_heartbeat(self.user_heartbeat)
         return ret
 
     def user_heartbeat(self):  # 用户心跳，默认会自动开启
         if self._token in (None, ''):
             return DotDict({'code': -2, 'message': u'请在卡密登录成功后调用'})
@@ -480,14 +482,15 @@
         path = '/v1/trial/login'
         data = {'device_id': self._device_id}
         ret = self.request(method, path, data)
         if ret.code == 0:
             self.is_trial = True
             self._token = ret.result.token
             self.login_result = ret.result
+            self._heartbeat_gap = ret.result.hg
             if self._auto_heartbeat:
                 self._start_heartbeat(self.trial_heartbeat)
         return ret
 
     def trial_heartbeat(self):
         method = 'POST'
         path = '/v1/trial/heartbeat'
```

### Comparing `PJYSDK-1.0.5/PJYSDK.egg-info/PKG-INFO` & `pjysdk-1.0.6/PJYSDK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PJYSDK
-Version: 1.0.5
+Version: 1.0.6
 Summary: 泡椒云网络验证 Python SDK
 Home-page: https://www.paojiaoyun.com
 Author: huaishan
 Author-email: admin@paojiaoyun.com
 Project-URL: Docs, https://docs.paojiaoyun.com/py_sdk.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PJYSDK-1.0.5/PKG-INFO` & `pjysdk-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PJYSDK
-Version: 1.0.5
+Version: 1.0.6
 Summary: 泡椒云网络验证 Python SDK
 Home-page: https://www.paojiaoyun.com
 Author: huaishan
 Author-email: admin@paojiaoyun.com
 Project-URL: Docs, https://docs.paojiaoyun.com/py_sdk.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PJYSDK-1.0.5/setup.py` & `pjysdk-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8", errors="ignore") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PJYSDK",
-    version="1.0.5",
+    version="1.0.6",
     author="huaishan",
     author_email="admin@paojiaoyun.com",
     description=u"泡椒云网络验证 Python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.paojiaoyun.com",
     project_urls={
```


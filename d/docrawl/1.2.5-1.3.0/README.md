# Comparing `tmp/docrawl-1.2.5.tar.gz` & `tmp/docrawl-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docrawl-1.2.5.tar", last modified: Tue Apr  9 10:47:51 2024, max compression
+gzip compressed data, was "docrawl-1.3.0.tar", last modified: Fri May  3 13:11:26 2024, max compression
```

## Comparing `docrawl-1.2.5.tar` & `docrawl-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 10:47:51.711438 docrawl-1.2.5/
--rw-rw-rw-   0        0        0     1090 2024-03-01 01:29:38.000000 docrawl-1.2.5/LICENSE
--rw-rw-rw-   0        0        0      527 2024-04-09 10:47:51.711438 docrawl-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-03-01 01:29:38.000000 docrawl-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 10:47:51.685599 docrawl-1.2.5/docrawl/
--rw-rw-rw-   0        0        0        0 2024-03-01 01:29:38.000000 docrawl-1.2.5/docrawl/__init__.py
--rw-rw-rw-   0        0        0    12654 2024-03-18 17:46:30.000000 docrawl-1.2.5/docrawl/docrawl_client.py
--rw-rw-rw-   0        0        0    42925 2024-03-14 09:32:09.000000 docrawl-1.2.5/docrawl/docrawl_core.py
--rw-rw-rw-   0        0        0     6847 2024-03-01 01:29:38.000000 docrawl-1.2.5/docrawl/docrawl_launcher.py
--rw-rw-rw-   0        0        0     1108 2024-03-01 01:29:38.000000 docrawl-1.2.5/docrawl/docrawl_logger.py
--rw-rw-rw-   0        0        0     2674 2024-03-01 01:29:38.000000 docrawl-1.2.5/docrawl/elements.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:47:51.709837 docrawl-1.2.5/docrawl.egg-info/
--rw-rw-rw-   0        0        0      527 2024-04-09 10:47:51.000000 docrawl-1.2.5/docrawl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2024-04-09 10:47:51.000000 docrawl-1.2.5/docrawl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 10:47:51.000000 docrawl-1.2.5/docrawl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2024-04-09 10:47:51.000000 docrawl-1.2.5/docrawl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-09 10:47:51.000000 docrawl-1.2.5/docrawl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 10:47:51.711438 docrawl-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      834 2024-04-09 10:47:33.000000 docrawl-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:11:26.472505 docrawl-1.3.0/
+-rw-rw-rw-   0        0        0     1090 2024-03-01 01:29:38.000000 docrawl-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0      527 2024-05-03 13:11:26.471185 docrawl-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-03-01 01:29:38.000000 docrawl-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 13:11:26.424036 docrawl-1.3.0/docrawl/
+-rw-rw-rw-   0        0        0        0 2024-03-01 01:29:38.000000 docrawl-1.3.0/docrawl/__init__.py
+-rw-rw-rw-   0        0        0    12660 2024-05-03 13:10:38.000000 docrawl-1.3.0/docrawl/docrawl_client.py
+-rw-rw-rw-   0        0        0    42929 2024-05-03 13:10:38.000000 docrawl-1.3.0/docrawl/docrawl_core.py
+-rw-rw-rw-   0        0        0     6847 2024-03-01 01:29:38.000000 docrawl-1.3.0/docrawl/docrawl_launcher.py
+-rw-rw-rw-   0        0        0     1108 2024-03-01 01:29:38.000000 docrawl-1.3.0/docrawl/docrawl_logger.py
+-rw-rw-rw-   0        0        0     2674 2024-03-01 01:29:38.000000 docrawl-1.3.0/docrawl/elements.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:11:26.470185 docrawl-1.3.0/docrawl.egg-info/
+-rw-rw-rw-   0        0        0      527 2024-05-03 13:11:26.000000 docrawl-1.3.0/docrawl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2024-05-03 13:11:26.000000 docrawl-1.3.0/docrawl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 13:11:26.000000 docrawl-1.3.0/docrawl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2024-05-03 13:11:26.000000 docrawl-1.3.0/docrawl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-03 13:11:26.000000 docrawl-1.3.0/docrawl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 13:11:26.472505 docrawl-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      834 2024-05-03 13:11:11.000000 docrawl-1.3.0/setup.py
```

### Comparing `docrawl-1.2.5/LICENSE` & `docrawl-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docrawl-1.2.5/PKG-INFO` & `docrawl-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 1.2.5
+Version: 1.3.0
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `docrawl-1.2.5/docrawl/docrawl_client.py` & `docrawl-1.3.0/docrawl/docrawl_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,25 +20,25 @@
     headless: bool
     last_function: str
 
 
 class DocrawlClient:
     id_iter = itertools.count()
 
-    def __init__(self, kv_redis=KeepVariableDummyRedisServer(), kv_redis_keys=None, number_of_spawn_browsers=0, redis_key_prefix=""):
+    def __init__(self, kv_redis=None, kv_redis_keys=None, number_of_spawn_browsers=0, redis_key_prefix=""):
         """number of spawn browsers = how many browser processes are ready in standby mode to not initialize + close the browser, currently support 0 and 1"""
-        self._client_id = next(self.id_iter)
+        self._client_id = redis_key_prefix.split(':')[1] or next(self.id_iter)
 
-        self.kv_redis = kv_redis
-        self.kv_redis_keys = kv_redis_keys or dict()
+        self.kv_redis = kv_redis or KeepVariableDummyRedisServer()
+        self.kv_redis_keys = kv_redis_keys or {}
         self.redis_key_prefix = redis_key_prefix
 
-        self._kv_redis_key_browser_metadata = self.kv_redis_keys.get(self.redis_key_prefix+'browser_meta_data', self.redis_key_prefix+'browser_meta_data')
-        self._kv_redis_key_scanned_elements = self.kv_redis_keys.get(self.redis_key_prefix+'elements', self.redis_key_prefix+'elements')
-        self._kv_redis_key_screenshot = self.kv_redis_keys.get(self.redis_key_prefix+'screenshot', self.redis_key_prefix+'screenshot')
+        self._kv_redis_key_browser_metadata = self.kv_redis_keys.get('browser_meta_data', f'{self.redis_key_prefix}:browser_meta_data')
+        self._kv_redis_key_scanned_elements = self.kv_redis_keys.get('elements', f'{self.redis_key_prefix}:elements')
+        self._kv_redis_key_screenshot = self.kv_redis_keys.get('screenshot', f'{self.redis_key_prefix}:screenshot')
         
         
         docrawl_logger.info(f'Initialised DocrawlClient with ID {self._client_id}')
         
         if number_of_spawn_browsers > 0: #TODO: increase number of spawned browsers, support just 1 standby browser at this moment
             self.run_spider()
 
@@ -48,21 +48,21 @@
     def get_browser_meta_data(self):
         return self.kv_redis.get(key=self._kv_redis_key_browser_metadata)
 
     def set_browser_scanned_elements(self, elements: list):
         self.kv_redis.set(key=self._kv_redis_key_scanned_elements, value=elements)
 
     def get_browser_scanned_elements(self):
-        self.kv_redis.get(key=self._kv_redis_key_scanned_elements)
+        return self.kv_redis.get(key=self._kv_redis_key_scanned_elements)
 
     def set_browser_screenshot(self, screenshot: str):
         self.kv_redis.set(key=self._kv_redis_key_screenshot, value=screenshot)
 
-    def get_browser_screenshot(self):
-        self.kv_redis.get(key=self._kv_redis_key_screenshot)
+    def get_browser_screenshot(self) -> str:
+        return self.kv_redis.get(key=self._kv_redis_key_screenshot)
 
     def is_browser_active(self):
         # TODO: finish later
         pid = self.get_browser_meta_data()['browser'].get('pid', 0)
 
         return psutil.pid_exists(pid)
 
@@ -86,15 +86,15 @@
         timeout_start = time.time()
         while not is_page_loaded and time.time() < timeout_start + timeout:
             try:
                 is_page_loaded = self.get_browser_meta_data()['request']['loaded']
             except:
                 is_page_loaded = False
             time.sleep(0.5)
-            docrawl_logger.info('Page is still loading, waiting 0.5 sec ...')
+            # docrawl_logger.info('Page is still loading, waiting 0.5 sec ...')
 
         if is_page_loaded:
             docrawl_logger.success('Page loaded')
         else:
             docrawl_logger.error('Page was not loaded')
 
     def _wait_until_function_is_done(self, timeout):
@@ -109,15 +109,15 @@
         timeout_start = time.time()
         while not is_function_done and time.time() < timeout_start + timeout:
             try:
                 is_function_done = self.get_browser_meta_data()['function']['done']
             except:
                 is_function_done = False
             time.sleep(0.5)
-            docrawl_logger.info('Function is still running, waiting 0.5 sec ...')
+            # docrawl_logger.info('Function is still running, waiting 0.5 sec ...')
 
         if is_function_done:
             docrawl_logger.success('Function finished')
         else:
             docrawl_logger.error('Function was not finished')
 
     def _execute_function(self, function, function_input=None, timeout=30):
```

### Comparing `docrawl-1.2.5/docrawl/docrawl_core.py` & `docrawl-1.3.0/docrawl/docrawl_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -987,15 +987,15 @@
     def parse(self, response):
         
         browser_meta_data=self.docrawl_client.get_browser_meta_data()
         browser_request = browser_meta_data.get("request")
         while browser_request is None:
             
             
-            docrawl_logger.info('Waiting for getting a request in browser metadata')
+            # docrawl_logger.info('Waiting for getting a request in browser metadata')
             time.sleep(1)
             
             browser_meta_data=self.docrawl_client.get_browser_meta_data()
             browser_request = browser_meta_data.get("request")
         
         
         
@@ -1011,15 +1011,15 @@
             spider_request = browser_meta_data['request']
             spider_function = browser_meta_data['function']
             proxy = browser_meta_data['browser']['proxy']
 
             try:
                 
                 time.sleep(1)
-                docrawl_logger.info('Docrawl core loop, page loaded: '+str(spider_request['loaded'])+', function name :'+str(spider_function["name"])+" function done: "+str(spider_function["done"]))
+                # docrawl_logger.info('Docrawl core loop, page loaded: '+str(spider_request['loaded'])+', function name :'+str(spider_function["name"])+" function done: "+str(spider_function["done"]))
 
                 if not spider_request['loaded']:
                     
                     #self.initialize_screenshot_thread_if_not_existing()
 
                     if proxy != self.browser.proxy:
                         docrawl_logger.warning('Proxy was updated in meanwhile')
```

### Comparing `docrawl-1.2.5/docrawl/docrawl_launcher.py` & `docrawl-1.3.0/docrawl/docrawl_launcher.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.2.5/docrawl/docrawl_logger.py` & `docrawl-1.3.0/docrawl/docrawl_logger.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.2.5/docrawl/elements.py` & `docrawl-1.3.0/docrawl/elements.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.2.5/docrawl.egg-info/PKG-INFO` & `docrawl-1.3.0/docrawl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 1.2.5
+Version: 1.3.0
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `docrawl-1.2.5/setup.py` & `docrawl-1.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='docrawl',
-    version='1.2.5',
+    version='1.3.0',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Do automated crawling of pages using scrapy',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/docrawl',
     packages=setuptools.find_packages(),
```


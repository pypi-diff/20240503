# Comparing `tmp/django_cache_helper-1.0.6.tar.gz` & `tmp/django_cache_helper-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cache_helper-1.0.6.tar", last modified: Wed May  1 19:45:20 2024, max compression
+gzip compressed data, was "django_cache_helper-1.0.7.tar", last modified: Fri May  3 19:42:03 2024, max compression
```

## Comparing `django_cache_helper-1.0.6.tar` & `django_cache_helper-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 anthonypanat   (502) staff       (20)        0 2024-05-01 19:45:20.574371 django_cache_helper-1.0.6/
--rw-r--r--   0 anthonypanat   (502) staff       (20)     3466 2024-05-01 19:45:20.574034 django_cache_helper-1.0.6/PKG-INFO
--rw-r--r--   0 anthonypanat   (502) staff       (20)     2884 2024-05-01 18:07:28.000000 django_cache_helper-1.0.6/README.md
-drwxr-xr-x   0 anthonypanat   (502) staff       (20)        0 2024-05-01 19:45:20.571409 django_cache_helper-1.0.6/cache_helper/
--rw-r--r--   0 anthonypanat   (502) staff       (20)       20 2024-05-01 19:43:12.000000 django_cache_helper-1.0.6/cache_helper/__init__.py
--rw-r--r--   0 anthonypanat   (502) staff       (20)     8136 2024-05-01 19:43:12.000000 django_cache_helper-1.0.6/cache_helper/decorators.py
--rw-r--r--   0 anthonypanat   (502) staff       (20)      110 2024-05-01 18:07:28.000000 django_cache_helper-1.0.6/cache_helper/exceptions.py
--rw-r--r--   0 anthonypanat   (502) staff       (20)      470 2024-05-01 18:07:28.000000 django_cache_helper-1.0.6/cache_helper/interfaces.py
--rw-r--r--   0 anthonypanat   (502) staff       (20)       94 2024-05-01 18:07:28.000000 django_cache_helper-1.0.6/cache_helper/settings.py
--rw-r--r--   0 anthonypanat   (502) staff       (20)     4323 2024-05-01 18:07:28.000000 django_cache_helper-1.0.6/cache_helper/utils.py
-drwxr-xr-x   0 anthonypanat   (502) staff       (20)        0 2024-05-01 19:45:20.573467 django_cache_helper-1.0.6/django_cache_helper.egg-info/
--rw-r--r--   0 anthonypanat   (502) staff       (20)     3466 2024-05-01 19:45:20.000000 django_cache_helper-1.0.6/django_cache_helper.egg-info/PKG-INFO
--rw-r--r--   0 anthonypanat   (502) staff       (20)      349 2024-05-01 19:45:20.000000 django_cache_helper-1.0.6/django_cache_helper.egg-info/SOURCES.txt
--rw-r--r--   0 anthonypanat   (502) staff       (20)        1 2024-05-01 19:45:20.000000 django_cache_helper-1.0.6/django_cache_helper.egg-info/dependency_links.txt
--rw-r--r--   0 anthonypanat   (502) staff       (20)       13 2024-05-01 19:45:20.000000 django_cache_helper-1.0.6/django_cache_helper.egg-info/top_level.txt
--rw-r--r--   0 anthonypanat   (502) staff       (20)      841 2024-05-01 18:07:28.000000 django_cache_helper-1.0.6/pyproject.toml
--rw-r--r--   0 anthonypanat   (502) staff       (20)       38 2024-05-01 19:45:20.574450 django_cache_helper-1.0.6/setup.cfg
+drwxr-xr-x   0 anthonypanat   (502) staff       (20)        0 2024-05-03 19:42:03.780829 django_cache_helper-1.0.7/
+-rw-r--r--   0 anthonypanat   (502) staff       (20)     3466 2024-05-03 19:42:03.780526 django_cache_helper-1.0.7/PKG-INFO
+-rw-r--r--   0 anthonypanat   (502) staff       (20)     2884 2024-05-01 18:07:28.000000 django_cache_helper-1.0.7/README.md
+drwxr-xr-x   0 anthonypanat   (502) staff       (20)        0 2024-05-03 19:42:03.777865 django_cache_helper-1.0.7/cache_helper/
+-rw-r--r--   0 anthonypanat   (502) staff       (20)       20 2024-05-03 19:41:25.000000 django_cache_helper-1.0.7/cache_helper/__init__.py
+-rw-r--r--   0 anthonypanat   (502) staff       (20)     9546 2024-05-03 19:41:25.000000 django_cache_helper-1.0.7/cache_helper/decorators.py
+-rw-r--r--   0 anthonypanat   (502) staff       (20)      110 2024-05-01 18:07:28.000000 django_cache_helper-1.0.7/cache_helper/exceptions.py
+-rw-r--r--   0 anthonypanat   (502) staff       (20)      470 2024-05-01 18:07:28.000000 django_cache_helper-1.0.7/cache_helper/interfaces.py
+-rw-r--r--   0 anthonypanat   (502) staff       (20)       94 2024-05-01 18:07:28.000000 django_cache_helper-1.0.7/cache_helper/settings.py
+-rw-r--r--   0 anthonypanat   (502) staff       (20)     4323 2024-05-01 18:07:28.000000 django_cache_helper-1.0.7/cache_helper/utils.py
+drwxr-xr-x   0 anthonypanat   (502) staff       (20)        0 2024-05-03 19:42:03.780085 django_cache_helper-1.0.7/django_cache_helper.egg-info/
+-rw-r--r--   0 anthonypanat   (502) staff       (20)     3466 2024-05-03 19:42:03.000000 django_cache_helper-1.0.7/django_cache_helper.egg-info/PKG-INFO
+-rw-r--r--   0 anthonypanat   (502) staff       (20)      349 2024-05-03 19:42:03.000000 django_cache_helper-1.0.7/django_cache_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonypanat   (502) staff       (20)        1 2024-05-03 19:42:03.000000 django_cache_helper-1.0.7/django_cache_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonypanat   (502) staff       (20)       13 2024-05-03 19:42:03.000000 django_cache_helper-1.0.7/django_cache_helper.egg-info/top_level.txt
+-rw-r--r--   0 anthonypanat   (502) staff       (20)      841 2024-05-01 18:07:28.000000 django_cache_helper-1.0.7/pyproject.toml
+-rw-r--r--   0 anthonypanat   (502) staff       (20)       38 2024-05-03 19:42:03.780894 django_cache_helper-1.0.7/setup.cfg
```

### Comparing `django_cache_helper-1.0.6/PKG-INFO` & `django_cache_helper-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cache-helper
-Version: 1.0.6
+Version: 1.0.7
 Summary: a simple tool for making caching functions, methods, and class methods a little bit easier.
 Author-email: YCharts <developers@ycharts.com>
 Project-URL: Homepage, https://github.com/ycharts/django_cache_helper
 Keywords: cache,django
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `django_cache_helper-1.0.6/README.md` & `django_cache_helper-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `django_cache_helper-1.0.6/cache_helper/decorators.py` & `django_cache_helper-1.0.7/cache_helper/decorators.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,15 +32,24 @@
             except Exception:
                 logger.warning(
                     f'Error retrieving value from Cache for Key: {function_cache_key}',
                     exc_info=True,
                 )
                 value = sentinel
 
-            if value is sentinel:
+            # If there is an issue with our cache client deserializing the value (due to memory or some other issue),
+            # we get a None response so log anytime this happens
+            if value is None:
+                logger.warning(
+                    'None cache value found for cache key: {}, function cache key: {}, value: {}'.format(
+                        cache_key, function_cache_key, value
+                    )
+                )
+
+            if value is sentinel or value is None:
                 value = func(*args, **kwargs)
                 # Try and set the key, value pair in the cache.
                 # But if it fails on an error from the underlying
                 # cache system, handle it.
                 try:
                     cache.set(cache_key, value, timeout)
                 except CacheSetError:
@@ -87,15 +96,24 @@
             except Exception:
                 logger.warning(
                     f'Error retrieving value from Cache for Key: {function_cache_key}',
                     exc_info=True,
                 )
                 value = sentinel
 
-            if value is sentinel:
+            # If there is an issue with our cache client deserializing the value (due to memory or some other issue),
+            # we get a None response so log anytime this happens
+            if value is None:
+                logger.warning(
+                    'None cache value found for cache key: {}, function cache key: {}, value: {}'.format(
+                        cache_key, function_cache_key, value
+                    )
+                )
+
+            if value is sentinel or value is None:
                 value = func(*args, **kwargs)
                 # Try and set the key, value pair in the cache.
                 # But if it fails on an error from the underlying
                 # cache system, handle it.
                 try:
                     cache.set(cache_key, value, timeout)
                 except CacheSetError:
@@ -163,15 +181,24 @@
             except Exception:
                 logger.warning(
                     f'Error retrieving value from Cache for Key: {function_cache_key}',
                     exc_info=True,
                 )
                 value = sentinel
 
-            if value is sentinel:
+            # If there is an issue with our cache client deserializing the value (due to memory or some other issue),
+            # we get a None response so log anytime this happens
+            if value is None:
+                logger.warning(
+                    'None cache value found for cache key: {}, function cache key: {}, value: {}'.format(
+                        cache_key, function_cache_key, value
+                    )
+                )
+
+            if value is sentinel or value is None:
                 value = self.func(*args, **kwargs)
                 # Try and set the key, value pair in the cache.
                 # But if it fails on an error from the underlying
                 # cache system, handle it.
                 try:
                     cache.set(cache_key, value, timeout)
                 except CacheSetError:
```

### Comparing `django_cache_helper-1.0.6/cache_helper/utils.py` & `django_cache_helper-1.0.7/cache_helper/utils.py`

 * *Files identical despite different names*

### Comparing `django_cache_helper-1.0.6/django_cache_helper.egg-info/PKG-INFO` & `django_cache_helper-1.0.7/django_cache_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cache-helper
-Version: 1.0.6
+Version: 1.0.7
 Summary: a simple tool for making caching functions, methods, and class methods a little bit easier.
 Author-email: YCharts <developers@ycharts.com>
 Project-URL: Homepage, https://github.com/ycharts/django_cache_helper
 Keywords: cache,django
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `django_cache_helper-1.0.6/pyproject.toml` & `django_cache_helper-1.0.7/pyproject.toml`

 * *Files identical despite different names*


# Comparing `tmp/ding_api_client-3.4.4.tar.gz` & `tmp/ding_api_client-3.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ding_api_client-3.4.4.tar", last modified: Tue Apr 23 07:16:27 2024, max compression
+gzip compressed data, was "ding_api_client-3.4.5.tar", last modified: Fri May  3 00:12:26 2024, max compression
```

## Comparing `ding_api_client-3.4.4.tar` & `ding_api_client-3.4.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:16:27.253769 ding_api_client-3.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-04-23 07:16:27.253769 ding_api_client-3.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 07:16:27.253769 ding_api_client-3.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:16:27.245769 ding_api_client-3.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:16:27.245769 ding_api_client-3.4.4/src/ding/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:16:27.245769 ding_api_client-3.4.4/src/ding/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:16:27.245769 ding_api_client-3.4.4/src/ding/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:16:27.249769 ding_api_client-3.4.4/src/ding/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/components/createauthenticationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/components/createauthenticationresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/components/createcheckrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/components/createcheckresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/components/feedbackrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/components/feedbackresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/components/lookupresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/components/retryauthenticationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/components/retryauthenticationresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/components/security.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:16:27.249769 ding_api_client-3.4.4/src/ding/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/errors/errorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:16:27.249769 ding_api_client-3.4.4/src/ding/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/operations/check.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/operations/create_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/operations/feedback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/operations/lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/models/operations/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    15284 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:16:27.249769 ding_api_client-3.4.4/src/ding/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32093 2024-04-23 07:16:18.000000 ding_api_client-3.4.4/src/ding/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:16:27.249769 ding_api_client-3.4.4/src/ding_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-04-23 07:16:27.000000 ding_api_client-3.4.4/src/ding_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-23 07:16:27.000000 ding_api_client-3.4.4/src/ding_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 07:16:27.000000 ding_api_client-3.4.4/src/ding_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-23 07:16:27.000000 ding_api_client-3.4.4/src/ding_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 07:16:27.000000 ding_api_client-3.4.4/src/ding_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:12:26.678560 ding_api_client-3.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-05-03 00:12:26.678560 ding_api_client-3.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 00:12:26.678560 ding_api_client-3.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:12:26.674560 ding_api_client-3.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:12:26.674560 ding_api_client-3.4.5/src/ding/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:12:26.674560 ding_api_client-3.4.5/src/ding/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:12:26.674560 ding_api_client-3.4.5/src/ding/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:12:26.674560 ding_api_client-3.4.5/src/ding/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/createauthenticationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/createauthenticationresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/createcheckrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/createcheckresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/feedbackrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/feedbackresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/lookupresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/retryauthenticationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/retryauthenticationresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:12:26.678560 ding_api_client-3.4.5/src/ding/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/errors/errorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:12:26.678560 ding_api_client-3.4.5/src/ding/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/operations/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/operations/create_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/operations/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/operations/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/operations/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15284 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:12:26.678560 ding_api_client-3.4.5/src/ding/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32093 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:12:26.678560 ding_api_client-3.4.5/src/ding_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-05-03 00:12:26.000000 ding_api_client-3.4.5/src/ding_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-03 00:12:26.000000 ding_api_client-3.4.5/src/ding_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 00:12:26.000000 ding_api_client-3.4.5/src/ding_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-03 00:12:26.000000 ding_api_client-3.4.5/src/ding_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 00:12:26.000000 ding_api_client-3.4.5/src/ding_api_client.egg-info/top_level.txt
```

### Comparing `ding_api_client-3.4.4/PKG-INFO` & `ding_api_client-3.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ding_api_client
-Version: 3.4.4
+Version: 3.4.5
 Summary: Python Client SDK
 Home-page: https://github.com/ding-live/ding-python.git
 Author: Ding
 License: UNKNOWN
 Description: # Ding Python SDK
         
         The Ding Python library provides convenient access to the Ding API from applications written in the Python language.
```

### Comparing `ding_api_client-3.4.4/README.md` & `ding_api_client-3.4.5/README.md`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/setup.py` & `ding_api_client-3.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='ding_api_client',
-    version='3.4.4',
+    version='3.4.5',
     author='Ding',
     description='Python Client SDK',
     url='https://github.com/ding-live/ding-python.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `ding_api_client-3.4.4/src/ding/_hooks/sdkhooks.py` & `ding_api_client-3.4.5/src/ding/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/_hooks/types.py` & `ding_api_client-3.4.5/src/ding/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/lookup.py` & `ding_api_client-3.4.5/src/ding/lookup.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/models/components/__init__.py` & `ding_api_client-3.4.5/src/ding/models/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/models/components/createauthenticationrequest.py` & `ding_api_client-3.4.5/src/ding/models/components/createauthenticationrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/models/components/createauthenticationresponse.py` & `ding_api_client-3.4.5/src/ding/models/components/createauthenticationresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/models/components/createcheckrequest.py` & `ding_api_client-3.4.5/src/ding/models/components/createcheckrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/models/components/createcheckresponse.py` & `ding_api_client-3.4.5/src/ding/models/components/createcheckresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/models/components/feedbackrequest.py` & `ding_api_client-3.4.5/src/ding/models/components/feedbackrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/models/components/feedbackresponse.py` & `ding_api_client-3.4.5/src/ding/models/components/feedbackresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/models/components/lookupresponse.py` & `ding_api_client-3.4.5/src/ding/models/components/lookupresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/models/components/retryauthenticationrequest.py` & `ding_api_client-3.4.5/src/ding/models/components/retryauthenticationrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/models/components/retryauthenticationresponse.py` & `ding_api_client-3.4.5/src/ding/models/components/retryauthenticationresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/models/errors/errorresponse.py` & `ding_api_client-3.4.5/src/ding/models/errors/errorresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/models/errors/sdkerror.py` & `ding_api_client-3.4.5/src/ding/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/models/operations/check.py` & `ding_api_client-3.4.5/src/ding/models/operations/check.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/models/operations/create_authentication.py` & `ding_api_client-3.4.5/src/ding/models/operations/create_authentication.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/models/operations/feedback.py` & `ding_api_client-3.4.5/src/ding/models/operations/feedback.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/models/operations/lookup.py` & `ding_api_client-3.4.5/src/ding/models/operations/lookup.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/models/operations/retry.py` & `ding_api_client-3.4.5/src/ding/models/operations/retry.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/otp.py` & `ding_api_client-3.4.5/src/ding/otp.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/sdk.py` & `ding_api_client-3.4.5/src/ding/sdk.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/sdkconfiguration.py` & `ding_api_client-3.4.5/src/ding/sdkconfiguration.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '1.0.0'
-    sdk_version: str = '3.4.4'
-    gen_version: str = '2.312.1'
-    user_agent: str = 'speakeasy-sdk/python 3.4.4 2.312.1 1.0.0 ding_api_client'
+    sdk_version: str = '3.4.5'
+    gen_version: str = '2.319.10'
+    user_agent: str = 'speakeasy-sdk/python 3.4.5 2.319.10 1.0.0 ding_api_client'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `ding_api_client-3.4.4/src/ding/utils/retries.py` & `ding_api_client-3.4.5/src/ding/utils/retries.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding/utils/utils.py` & `ding_api_client-3.4.5/src/ding/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.4/src/ding_api_client.egg-info/PKG-INFO` & `ding_api_client-3.4.5/src/ding_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ding-api-client
-Version: 3.4.4
+Version: 3.4.5
 Summary: Python Client SDK
 Home-page: https://github.com/ding-live/ding-python.git
 Author: Ding
 License: UNKNOWN
 Description: # Ding Python SDK
         
         The Ding Python library provides convenient access to the Ding API from applications written in the Python language.
```

### Comparing `ding_api_client-3.4.4/src/ding_api_client.egg-info/SOURCES.txt` & `ding_api_client-3.4.5/src/ding_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*


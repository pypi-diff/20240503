# Comparing `tmp/tf_serving-0.1.0.tar.gz` & `tmp/tf_serving-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf_serving-0.1.0.tar", last modified: Fri May  3 11:03:54 2024, max compression
+gzip compressed data, was "tf_serving-0.1.1.tar", last modified: Fri May  3 11:25:36 2024, max compression
```

## Comparing `tf_serving-0.1.0.tar` & `tf_serving-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-03 11:03:54.928680 tf_serving-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      474 2024-05-03 11:03:54.928680 tf_serving-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       69 2024-05-03 10:45:48.000000 tf_serving-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      605 2024-05-03 11:01:55.000000 tf_serving-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-03 11:03:54.928680 tf_serving-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-03 11:03:54.918680 tf_serving-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-03 11:03:54.918680 tf_serving-0.1.0/src/tf/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-03 11:03:54.928680 tf_serving-0.1.0/src/tf/serving/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      174 2024-05-03 11:01:51.000000 tf_serving-0.1.0/src/tf/serving/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      192 2024-05-03 11:03:29.000000 tf_serving-0.1.0/src/tf/serving/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      917 2024-05-03 11:03:12.000000 tf_serving-0.1.0/src/tf/serving/multibatch.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      992 2024-05-03 11:01:35.000000 tf_serving-0.1.0/src/tf/serving/request.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      357 2024-05-03 10:49:32.000000 tf_serving-0.1.0/src/tf/serving/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-03 11:03:54.928680 tf_serving-0.1.0/src/tf_serving.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      474 2024-05-03 11:03:54.000000 tf_serving-0.1.0/src/tf_serving.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      347 2024-05-03 11:03:54.000000 tf_serving-0.1.0/src/tf_serving.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-03 11:03:54.000000 tf_serving-0.1.0/src/tf_serving.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       40 2024-05-03 11:03:54.000000 tf_serving-0.1.0/src/tf_serving.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-05-03 11:03:54.000000 tf_serving-0.1.0/src/tf_serving.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-03 11:25:36.495552 tf_serving-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1040 2024-05-03 11:25:36.495552 tf_serving-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      635 2024-05-03 11:25:35.000000 tf_serving-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      605 2024-05-03 11:25:34.000000 tf_serving-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-03 11:25:36.495552 tf_serving-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-03 11:25:36.495552 tf_serving-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-03 11:25:36.495552 tf_serving-0.1.1/src/tf/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-03 11:25:36.495552 tf_serving-0.1.1/src/tf/serving/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      174 2024-05-03 11:01:51.000000 tf_serving-0.1.1/src/tf/serving/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      230 2024-05-03 11:18:51.000000 tf_serving-0.1.1/src/tf/serving/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      210 2024-05-03 11:18:43.000000 tf_serving-0.1.1/src/tf/serving/b64.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      917 2024-05-03 11:03:12.000000 tf_serving-0.1.1/src/tf/serving/multibatch.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      987 2024-05-03 11:17:37.000000 tf_serving-0.1.1/src/tf/serving/request.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      315 2024-05-03 11:21:17.000000 tf_serving-0.1.1/src/tf/serving/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-03 11:25:36.495552 tf_serving-0.1.1/src/tf_serving.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1040 2024-05-03 11:25:36.000000 tf_serving-0.1.1/src/tf_serving.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      369 2024-05-03 11:25:36.000000 tf_serving-0.1.1/src/tf_serving.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-03 11:25:36.000000 tf_serving-0.1.1/src/tf_serving.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       40 2024-05-03 11:25:36.000000 tf_serving-0.1.1/src/tf_serving.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-05-03 11:25:36.000000 tf_serving-0.1.1/src/tf_serving.egg-info/top_level.txt
```

### Comparing `tf_serving-0.1.0/pyproject.toml` & `tf_serving-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tf-serving"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Client for OCR predictions against TensorFlow Serving"
 dependencies = [
   "aiohttp", "pydantic", "haskellian", "lazy-loader"
 ]
```

### Comparing `tf_serving-0.1.0/src/tf/serving/multibatch.py` & `tf_serving-0.1.1/src/tf/serving/multibatch.py`

 * *Files identical despite different names*

### Comparing `tf_serving-0.1.0/src/tf/serving/request.py` & `tf_serving-0.1.1/src/tf/serving/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing_extensions import TypedDict, NotRequired, Sequence, overload
 import aiohttp
 from haskellian import Either, Left, Right
 from .types import TFSResponse, ImagePreds
-  
+
 class Params(TypedDict):
   host: NotRequired[str]
   port: NotRequired[int]
   endpoint: NotRequired[str]
 
 PredictErr = aiohttp.ClientError
 
@@ -14,15 +14,14 @@
   b64imgs: Sequence[str], *,
   host: str = 'http://localhost',
   port: int = 8501,
   endpoint: str = '/v1/models/ocr:predict'
 ) -> Either[PredictErr, Sequence[ImagePreds]]:
   """Each `b64imgs[i]` is a base64-encoded JPG/PNG/WEBP image"""
   base = f'{host.strip("/")}:{port}'
-  
   try:
     async with aiohttp.ClientSession(base) as session:
       req = session.post(endpoint, json={
         "signature_name": "serving_default",
         "instances": b64imgs
       })
       async with req as res:
```


# Comparing `tmp/oshepherd-0.0.5.tar.gz` & `tmp/oshepherd-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oshepherd-0.0.5.tar", last modified: Mon Apr 29 13:18:14 2024, max compression
+gzip compressed data, was "oshepherd-0.0.6.tar", last modified: Fri May  3 21:16:03 2024, max compression
```

## Comparing `oshepherd-0.0.5.tar` & `oshepherd-0.0.6.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-04-29 13:18:14.352509 oshepherd-0.0.5/
--rw-r--r--   0 raulpino   (501) staff       (20)     1064 2024-04-09 19:32:21.000000 oshepherd-0.0.5/LICENSE
--rw-r--r--   0 raulpino   (501) staff       (20)       47 2024-04-09 19:47:56.000000 oshepherd-0.0.5/MANIFEST.in
--rw-r--r--   0 raulpino   (501) staff       (20)     3459 2024-04-29 13:18:14.352329 oshepherd-0.0.5/PKG-INFO
--rw-r--r--   0 raulpino   (501) staff       (20)     2425 2024-04-28 14:19:44.000000 oshepherd-0.0.5/README.md
-drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-04-29 13:18:14.347523 oshepherd-0.0.5/oshepherd/
--rw-r--r--   0 raulpino   (501) staff       (20)        0 2024-04-07 01:40:19.000000 oshepherd-0.0.5/oshepherd/__init__.py
-drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-04-29 13:18:14.350284 oshepherd-0.0.5/oshepherd/api/
--rw-r--r--   0 raulpino   (501) staff       (20)        0 2024-04-07 02:37:24.000000 oshepherd-0.0.5/oshepherd/api/__init__.py
--rw-r--r--   0 raulpino   (501) staff       (20)      932 2024-04-08 01:56:54.000000 oshepherd-0.0.5/oshepherd/api/app.py
--rw-r--r--   0 raulpino   (501) staff       (20)      353 2024-04-08 03:25:51.000000 oshepherd-0.0.5/oshepherd/api/config.py
-drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-04-29 13:18:14.350905 oshepherd-0.0.5/oshepherd/api/generate/
--rw-r--r--   0 raulpino   (501) staff       (20)        0 2024-04-07 02:37:24.000000 oshepherd-0.0.5/oshepherd/api/generate/__init__.py
--rw-r--r--   0 raulpino   (501) staff       (20)      847 2024-04-09 03:21:09.000000 oshepherd-0.0.5/oshepherd/api/generate/models.py
--rw-r--r--   0 raulpino   (501) staff       (20)     1262 2024-04-08 03:36:28.000000 oshepherd-0.0.5/oshepherd/api/generate/routes.py
--rw-r--r--   0 raulpino   (501) staff       (20)      304 2024-04-07 02:37:24.000000 oshepherd-0.0.5/oshepherd/api/utils.py
--rw-r--r--   0 raulpino   (501) staff       (20)     1208 2024-04-08 03:34:21.000000 oshepherd-0.0.5/oshepherd/cli.py
--rw-r--r--   0 raulpino   (501) staff       (20)      665 2024-04-08 03:21:10.000000 oshepherd-0.0.5/oshepherd/lib.py
-drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-04-29 13:18:14.351656 oshepherd-0.0.5/oshepherd/worker/
--rw-r--r--   0 raulpino   (501) staff       (20)        0 2024-04-07 02:47:11.000000 oshepherd-0.0.5/oshepherd/worker/__init__.py
--rw-r--r--   0 raulpino   (501) staff       (20)     1236 2024-04-29 13:18:02.000000 oshepherd-0.0.5/oshepherd/worker/app.py
--rw-r--r--   0 raulpino   (501) staff       (20)      459 2024-04-29 13:18:02.000000 oshepherd-0.0.5/oshepherd/worker/config.py
--rw-r--r--   0 raulpino   (501) staff       (20)     2302 2024-04-29 13:18:02.000000 oshepherd-0.0.5/oshepherd/worker/ollama_task.py
--rw-r--r--   0 raulpino   (501) staff       (20)      877 2024-04-29 13:18:02.000000 oshepherd-0.0.5/oshepherd/worker/tasks.py
-drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-04-29 13:18:14.351881 oshepherd-0.0.5/oshepherd.egg-info/
--rw-r--r--   0 raulpino   (501) staff       (20)     3459 2024-04-29 13:18:14.000000 oshepherd-0.0.5/oshepherd.egg-info/PKG-INFO
--rw-r--r--   0 raulpino   (501) staff       (20)      642 2024-04-29 13:18:14.000000 oshepherd-0.0.5/oshepherd.egg-info/SOURCES.txt
--rw-r--r--   0 raulpino   (501) staff       (20)        1 2024-04-29 13:18:14.000000 oshepherd-0.0.5/oshepherd.egg-info/dependency_links.txt
--rw-r--r--   0 raulpino   (501) staff       (20)       49 2024-04-29 13:18:14.000000 oshepherd-0.0.5/oshepherd.egg-info/entry_points.txt
--rw-r--r--   0 raulpino   (501) staff       (20)      142 2024-04-29 13:18:14.000000 oshepherd-0.0.5/oshepherd.egg-info/requires.txt
--rw-r--r--   0 raulpino   (501) staff       (20)       16 2024-04-29 13:18:14.000000 oshepherd-0.0.5/oshepherd.egg-info/top_level.txt
--rw-r--r--   0 raulpino   (501) staff       (20)      870 2024-04-29 13:18:02.000000 oshepherd-0.0.5/pyproject.toml
--rw-r--r--   0 raulpino   (501) staff       (20)       38 2024-04-29 13:18:14.352552 oshepherd-0.0.5/setup.cfg
--rw-r--r--   0 raulpino   (501) staff       (20)     1271 2024-04-29 13:18:02.000000 oshepherd-0.0.5/setup.py
+drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-05-03 21:16:03.664336 oshepherd-0.0.6/
+-rw-r--r--   0 raulpino   (501) staff       (20)     1064 2024-04-09 19:32:21.000000 oshepherd-0.0.6/LICENSE
+-rw-r--r--   0 raulpino   (501) staff       (20)       47 2024-04-09 19:47:56.000000 oshepherd-0.0.6/MANIFEST.in
+-rw-r--r--   0 raulpino   (501) staff       (20)     4867 2024-05-03 21:16:03.664156 oshepherd-0.0.6/PKG-INFO
+-rw-r--r--   0 raulpino   (501) staff       (20)     3833 2024-05-03 21:12:19.000000 oshepherd-0.0.6/README.md
+drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-05-03 21:16:03.659815 oshepherd-0.0.6/oshepherd/
+-rw-r--r--   0 raulpino   (501) staff       (20)        0 2024-04-07 01:40:19.000000 oshepherd-0.0.6/oshepherd/__init__.py
+drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-05-03 21:16:03.661493 oshepherd-0.0.6/oshepherd/api/
+-rw-r--r--   0 raulpino   (501) staff       (20)        0 2024-04-07 02:37:24.000000 oshepherd-0.0.6/oshepherd/api/__init__.py
+-rw-r--r--   0 raulpino   (501) staff       (20)     1028 2024-05-03 21:12:19.000000 oshepherd-0.0.6/oshepherd/api/app.py
+drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-05-03 21:16:03.662133 oshepherd-0.0.6/oshepherd/api/chat/
+-rw-r--r--   0 raulpino   (501) staff       (20)        0 2024-05-03 21:12:19.000000 oshepherd-0.0.6/oshepherd/api/chat/__init__.py
+-rw-r--r--   0 raulpino   (501) staff       (20)      881 2024-05-03 21:12:19.000000 oshepherd-0.0.6/oshepherd/api/chat/models.py
+-rw-r--r--   0 raulpino   (501) staff       (20)     1461 2024-05-03 21:12:19.000000 oshepherd-0.0.6/oshepherd/api/chat/routes.py
+-rw-r--r--   0 raulpino   (501) staff       (20)      353 2024-04-08 03:25:51.000000 oshepherd-0.0.6/oshepherd/api/config.py
+drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-05-03 21:16:03.662634 oshepherd-0.0.6/oshepherd/api/generate/
+-rw-r--r--   0 raulpino   (501) staff       (20)        0 2024-04-07 02:37:24.000000 oshepherd-0.0.6/oshepherd/api/generate/__init__.py
+-rw-r--r--   0 raulpino   (501) staff       (20)      953 2024-05-03 21:12:19.000000 oshepherd-0.0.6/oshepherd/api/generate/models.py
+-rw-r--r--   0 raulpino   (501) staff       (20)     1511 2024-05-03 21:12:19.000000 oshepherd-0.0.6/oshepherd/api/generate/routes.py
+-rw-r--r--   0 raulpino   (501) staff       (20)      304 2024-04-07 02:37:24.000000 oshepherd-0.0.6/oshepherd/api/utils.py
+-rw-r--r--   0 raulpino   (501) staff       (20)     1332 2024-05-03 21:12:19.000000 oshepherd-0.0.6/oshepherd/cli.py
+-rw-r--r--   0 raulpino   (501) staff       (20)      665 2024-04-08 03:21:10.000000 oshepherd-0.0.6/oshepherd/lib.py
+drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-05-03 21:16:03.663521 oshepherd-0.0.6/oshepherd/worker/
+-rw-r--r--   0 raulpino   (501) staff       (20)        0 2024-04-07 02:47:11.000000 oshepherd-0.0.6/oshepherd/worker/__init__.py
+-rw-r--r--   0 raulpino   (501) staff       (20)     1236 2024-04-29 15:15:15.000000 oshepherd-0.0.6/oshepherd/worker/app.py
+-rw-r--r--   0 raulpino   (501) staff       (20)      539 2024-05-03 21:12:19.000000 oshepherd-0.0.6/oshepherd/worker/config.py
+-rw-r--r--   0 raulpino   (501) staff       (20)     2302 2024-04-29 15:15:15.000000 oshepherd-0.0.6/oshepherd/worker/ollama_task.py
+-rw-r--r--   0 raulpino   (501) staff       (20)      991 2024-05-03 21:12:19.000000 oshepherd-0.0.6/oshepherd/worker/tasks.py
+drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-05-03 21:16:03.663700 oshepherd-0.0.6/oshepherd.egg-info/
+-rw-r--r--   0 raulpino   (501) staff       (20)     4867 2024-05-03 21:16:03.000000 oshepherd-0.0.6/oshepherd.egg-info/PKG-INFO
+-rw-r--r--   0 raulpino   (501) staff       (20)      731 2024-05-03 21:16:03.000000 oshepherd-0.0.6/oshepherd.egg-info/SOURCES.txt
+-rw-r--r--   0 raulpino   (501) staff       (20)        1 2024-05-03 21:16:03.000000 oshepherd-0.0.6/oshepherd.egg-info/dependency_links.txt
+-rw-r--r--   0 raulpino   (501) staff       (20)       49 2024-05-03 21:16:03.000000 oshepherd-0.0.6/oshepherd.egg-info/entry_points.txt
+-rw-r--r--   0 raulpino   (501) staff       (20)      142 2024-05-03 21:16:03.000000 oshepherd-0.0.6/oshepherd.egg-info/requires.txt
+-rw-r--r--   0 raulpino   (501) staff       (20)       16 2024-05-03 21:16:03.000000 oshepherd-0.0.6/oshepherd.egg-info/top_level.txt
+-rw-r--r--   0 raulpino   (501) staff       (20)      870 2024-05-03 21:12:45.000000 oshepherd-0.0.6/pyproject.toml
+-rw-r--r--   0 raulpino   (501) staff       (20)       38 2024-05-03 21:16:03.664379 oshepherd-0.0.6/setup.cfg
+-rw-r--r--   0 raulpino   (501) staff       (20)     1271 2024-05-03 21:12:40.000000 oshepherd-0.0.6/setup.py
```

### Comparing `oshepherd-0.0.5/LICENSE` & `oshepherd-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `oshepherd-0.0.5/oshepherd/api/app.py` & `oshepherd-0.0.6/oshepherd/api/app.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from flask import Flask, Blueprint
 from oshepherd.api.config import ApiConfig
 from oshepherd.api.generate.routes import generate_blueprint
+from oshepherd.api.chat.routes import chat_blueprint
 from oshepherd.worker.app import create_celery_app_for_flask
 
 
 def start_flask_app(config: ApiConfig):
     app = Flask(config.FLASK_PROJECT_NAME)
     app.config["FLASK_RUN_PORT"] = config.FLASK_RUN_PORT
     app.config["FLASK_DEBUG"] = config.FLASK_DEBUG
@@ -15,14 +16,15 @@
     # celery setup
     celery_app = create_celery_app_for_flask(app)
     app.celery = celery_app
 
     # endpoints
     api = Blueprint("api", __name__)
     api.register_blueprint(generate_blueprint)
+    api.register_blueprint(chat_blueprint)
     app.register_blueprint(api)
 
     app.run(
         debug=app.config["FLASK_DEBUG"],
         host=app.config["FLASK_HOST"],
         port=app.config["FLASK_RUN_PORT"],
     )
```

### Comparing `oshepherd-0.0.5/oshepherd/api/generate/models.py` & `oshepherd-0.0.6/oshepherd/api/generate/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from pydantic import BaseModel
 from typing import Optional, List
 
 
-class GenerateRequest(BaseModel):
+class GenerateRequestPayload(BaseModel):
     model: str
     prompt: str
     images: Optional[List[str]] = None
     format: Optional[str] = "json"
     options: Optional[dict] = None
     system: Optional[str] = None
     template: Optional[str] = None
     context: Optional[List[int]] = None
     stream: Optional[bool] = False
     raw: Optional[bool] = False
     keep_alive: Optional[str] = "5m"
 
 
+class GenerateRequest(BaseModel):
+    type: str = "generate"
+    payload: GenerateRequestPayload
+
+
 class GenerateResponse(BaseModel):
     model: str
     created_at: str
     response: str
     done: bool
     context: Optional[List[int]] = None
     total_duration: Optional[int] = None
```

### Comparing `oshepherd-0.0.5/oshepherd/api/generate/routes.py` & `oshepherd-0.0.6/oshepherd/api/generate/routes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,43 @@
+"""
+Generate a completion
+API implementation of `POST /api/generate` endpoint, handling completion orchestration, as replica of the same Ollama server endpoint.
+Ollama endpoint reference: https://github.com/ollama/ollama/blob/main/docs/api.md#generate-a-completion
+"""
+
 import time
 from flask import Blueprint, request
 from oshepherd.api.utils import streamify_json
 from oshepherd.api.generate.models import GenerateRequest
 
 generate_blueprint = Blueprint("generate", __name__, url_prefix="/api/generate")
 
 
 @generate_blueprint.route("/", methods=["POST"])
 def generate():
-    # TODO use .send_task() instead?
-    from oshepherd.worker.tasks import make_generate_request
+    from oshepherd.worker.tasks import exec_completion
 
     print(f" # request.json {request.json}")
-    generate_request = GenerateRequest(**request.json)
+    generate_request = GenerateRequest(**{"payload": request.json})
 
-    # req as json string ready to be sent though broker
+    # req as json string ready to be sent through broker
     generate_request_json_str = generate_request.model_dump_json()
-    print(generate_request_json_str)
+    print(f" # generate request {generate_request_json_str}")
 
-    # queue request to remote ollama api server though
-    task = make_generate_request.delay(generate_request_json_str)
+    # queue request to remote ollama api server
+    task = exec_completion.delay(generate_request_json_str)
     while not task.ready():
         print(" > waiting for response...")
         time.sleep(1)
     ollama_res = task.get(timeout=1)
 
     status = 200
     if ollama_res.get("error"):
         ollama_res = {
             "error": "Internal Server Error",
-            "message": f"error triggering llm inference: {ollama_res['error']['message']}",
+            "message": f"error executing completion: {ollama_res['error']['message']}",
         }
         status = 500
 
     print(f" $ ollama response {status}: {ollama_res}")
 
     return streamify_json(ollama_res, status)
```

### Comparing `oshepherd-0.0.5/oshepherd/cli.py` & `oshepherd-0.0.6/oshepherd/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -35,13 +35,15 @@
     config: WorkerConfig = load_and_validate_env(env_file, WorkerConfig)
 
     celery_app = create_celery_app(config)
     worker = celery_app.Worker(
         loglevel=config.LOGLEVEL,
         concurrency=config.CONCURRENCY,
         prefetch_multiplier=config.PREFETCH_MULTIPLIER,
+        redis_retry_on_timeout=config.REDIS_RETRY_ON_TIMEOUT,
+        redis_socket_keepalive=config.REDIS_SOCKET_KEEPALIVE,
     )
     worker.start()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `oshepherd-0.0.5/oshepherd/lib.py` & `oshepherd-0.0.6/oshepherd/lib.py`

 * *Files identical despite different names*

### Comparing `oshepherd-0.0.5/oshepherd/worker/app.py` & `oshepherd-0.0.6/oshepherd/worker/app.py`

 * *Files identical despite different names*

### Comparing `oshepherd-0.0.5/oshepherd/worker/ollama_task.py` & `oshepherd-0.0.6/oshepherd/worker/ollama_task.py`

 * *Files identical despite different names*

### Comparing `oshepherd-0.0.5/oshepherd.egg-info/SOURCES.txt` & `oshepherd-0.0.6/oshepherd.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 oshepherd.egg-info/entry_points.txt
 oshepherd.egg-info/requires.txt
 oshepherd.egg-info/top_level.txt
 oshepherd/api/__init__.py
 oshepherd/api/app.py
 oshepherd/api/config.py
 oshepherd/api/utils.py
+oshepherd/api/chat/__init__.py
+oshepherd/api/chat/models.py
+oshepherd/api/chat/routes.py
 oshepherd/api/generate/__init__.py
 oshepherd/api/generate/models.py
 oshepherd/api/generate/routes.py
 oshepherd/worker/__init__.py
 oshepherd/worker/app.py
 oshepherd/worker/config.py
 oshepherd/worker/ollama_task.py
```

### Comparing `oshepherd-0.0.5/pyproject.toml` & `oshepherd-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "oshepherd"
-version = "0.0.5"
+version = "0.0.6"
 description = "The Oshepherd guiding the Ollama(s) inference orchestration."
 readme = "README.md"
 authors = [
     {name = "mnemonica.ai", email = "info@mnemonica.ai"},
 ]
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `oshepherd-0.0.5/setup.py` & `oshepherd-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="oshepherd",
-    version="0.0.5",
+    version="0.0.6",
     description="The Oshepherd guiding the Ollama(s) inference orchestration.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author="mnemonica.ai",
     author_email="info@mnemonica.ai",
     packages=find_packages(),
     python_requires=">=3.8",
```


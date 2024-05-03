# Comparing `tmp/loopquest-0.2.1.tar.gz` & `tmp/loopquest-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopquest-0.2.1.tar", last modified: Wed May  1 06:20:38 2024, max compression
+gzip compressed data, was "loopquest-0.2.2.tar", last modified: Fri May  3 16:54:35 2024, max compression
```

## Comparing `loopquest-0.2.1.tar` & `loopquest-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 06:20:38.614737 loopquest-0.2.1/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)    11357 2024-04-19 04:42:45.000000 loopquest-0.2.1/LICENSE
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6605 2024-05-01 06:20:38.614737 loopquest-0.2.1/PKG-INFO
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5418 2024-04-29 17:12:15.000000 loopquest-0.2.1/README.md
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 06:20:38.610737 loopquest-0.2.1/loopquest/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       86 2024-04-24 04:38:12.000000 loopquest-0.2.1/loopquest/__init__.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1439 2024-04-24 05:33:47.000000 loopquest-0.2.1/loopquest/api.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9075 2024-04-28 15:10:40.000000 loopquest-0.2.1/loopquest/crud.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1933 2024-04-19 04:43:26.000000 loopquest-0.2.1/loopquest/datasets.py
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 06:20:38.610737 loopquest-0.2.1/loopquest/env/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 05:17:29.000000 loopquest-0.2.1/loopquest/env/__init__.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4217 2024-04-29 05:10:05.000000 loopquest-0.2.1/loopquest/env/api.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5767 2024-04-19 04:43:26.000000 loopquest-0.2.1/loopquest/env/gym_wrappers.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9238 2024-04-19 04:43:26.000000 loopquest-0.2.1/loopquest/env/space_utils.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5145 2024-04-29 04:54:43.000000 loopquest-0.2.1/loopquest/eval.py
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 06:20:38.610737 loopquest-0.2.1/loopquest/policy/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-04-19 04:43:26.000000 loopquest-0.2.1/loopquest/policy/__init__.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      173 2024-04-19 04:43:26.000000 loopquest-0.2.1/loopquest/policy/base.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1383 2024-04-19 04:43:26.000000 loopquest-0.2.1/loopquest/policy/sb3_policy.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1994 2024-04-24 04:19:39.000000 loopquest-0.2.1/loopquest/private_api.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5685 2024-04-28 05:00:52.000000 loopquest-0.2.1/loopquest/schema.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      168 2024-04-19 04:43:26.000000 loopquest-0.2.1/loopquest/typing.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      376 2024-04-19 04:42:45.000000 loopquest-0.2.1/loopquest/ui.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4216 2024-04-19 04:43:26.000000 loopquest-0.2.1/loopquest/utils.py
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 06:20:38.610737 loopquest-0.2.1/loopquest.egg-info/
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6605 2024-05-01 06:20:38.000000 loopquest-0.2.1/loopquest.egg-info/PKG-INFO
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      578 2024-05-01 06:20:38.000000 loopquest-0.2.1/loopquest.egg-info/SOURCES.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        1 2024-05-01 06:20:38.000000 loopquest-0.2.1/loopquest.egg-info/dependency_links.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      302 2024-05-01 06:20:38.000000 loopquest-0.2.1/loopquest.egg-info/requires.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       10 2024-05-01 06:20:38.000000 loopquest-0.2.1/loopquest.egg-info/top_level.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       38 2024-05-01 06:20:38.614737 loopquest-0.2.1/setup.cfg
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1144 2024-05-01 06:20:16.000000 loopquest-0.2.1/setup.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-03 16:54:35.259745 loopquest-0.2.2/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)    11357 2024-04-19 04:42:45.000000 loopquest-0.2.2/LICENSE
+-rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6605 2024-05-03 16:54:35.259745 loopquest-0.2.2/PKG-INFO
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5418 2024-04-29 17:12:15.000000 loopquest-0.2.2/README.md
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-03 16:54:35.255745 loopquest-0.2.2/loopquest/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       86 2024-04-24 04:38:12.000000 loopquest-0.2.2/loopquest/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1439 2024-04-24 05:33:47.000000 loopquest-0.2.2/loopquest/api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9416 2024-05-03 05:47:41.000000 loopquest-0.2.2/loopquest/crud.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1933 2024-04-19 04:43:26.000000 loopquest-0.2.2/loopquest/datasets.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-03 16:54:35.255745 loopquest-0.2.2/loopquest/env/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 05:17:29.000000 loopquest-0.2.2/loopquest/env/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4217 2024-04-29 05:10:05.000000 loopquest-0.2.2/loopquest/env/api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     6340 2024-05-03 16:52:23.000000 loopquest-0.2.2/loopquest/env/gym_wrappers.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9238 2024-04-19 04:43:26.000000 loopquest-0.2.2/loopquest/env/space_utils.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5145 2024-04-29 04:54:43.000000 loopquest-0.2.2/loopquest/eval.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-03 16:54:35.255745 loopquest-0.2.2/loopquest/policy/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-04-19 04:43:26.000000 loopquest-0.2.2/loopquest/policy/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      173 2024-04-19 04:43:26.000000 loopquest-0.2.2/loopquest/policy/base.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1383 2024-04-19 04:43:26.000000 loopquest-0.2.2/loopquest/policy/sb3_policy.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     2001 2024-05-03 04:41:02.000000 loopquest-0.2.2/loopquest/private_api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5685 2024-04-28 05:00:52.000000 loopquest-0.2.2/loopquest/schema.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      168 2024-04-19 04:43:26.000000 loopquest-0.2.2/loopquest/typing.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      376 2024-04-19 04:42:45.000000 loopquest-0.2.2/loopquest/ui.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4740 2024-05-03 05:20:31.000000 loopquest-0.2.2/loopquest/utils.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-03 16:54:35.255745 loopquest-0.2.2/loopquest.egg-info/
+-rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6605 2024-05-03 16:54:35.000000 loopquest-0.2.2/loopquest.egg-info/PKG-INFO
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      578 2024-05-03 16:54:35.000000 loopquest-0.2.2/loopquest.egg-info/SOURCES.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        1 2024-05-03 16:54:35.000000 loopquest-0.2.2/loopquest.egg-info/dependency_links.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      302 2024-05-03 16:54:35.000000 loopquest-0.2.2/loopquest.egg-info/requires.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       10 2024-05-03 16:54:35.000000 loopquest-0.2.2/loopquest.egg-info/top_level.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       38 2024-05-03 16:54:35.259745 loopquest-0.2.2/setup.cfg
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1144 2024-05-03 16:53:36.000000 loopquest-0.2.2/setup.py
```

### Comparing `loopquest-0.2.1/LICENSE` & `loopquest-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.1/PKG-INFO` & `loopquest-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopquest
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Production Tool for Embodied AI.
 Home-page: https://github.com/LoopMind-AI/loopquest
 Author: LoopMind
 Author-email: contactus@loopmind.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `loopquest-0.2.1/README.md` & `loopquest-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.1/loopquest/api.py` & `loopquest-0.2.2/loopquest/api.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.1/loopquest/crud.py` & `loopquest-0.2.2/loopquest/crud.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,24 @@
     Project,
     ProjectCreate,
     Experiment,
     ExperimentCreate,
     Step,
     ExperimentUpdate,
     EnvironmentCreate,
+    EnvironmentUpdate,
+    Environment,
 )
 from .env.space_utils import create_var_tree
 
 # NOTE: the current requests are not async, which could be a performance bottle neck.
 import requests
 from .utils import (
     rgb_array_to_image_bytes,
     replace_special_chars_with_dash,
-    safe_jsonize,
 )
 import numpy as np
 import gymnasium
 from PIL import Image
 from io import BytesIO
 from .private_api import TOKEN_ENV_VAR_NAME
 from dotenv import load_dotenv
@@ -72,23 +73,35 @@
     created_environment = response.json()
     return created_environment["id"]
 
 
 def get_environment(backend_url: str, id: str):
     id = replace_special_chars_with_dash(id)
     response = make_request("GET", f"{backend_url}/env/{id}")
+    data = response.json()
+    env = Environment(**data)
+    return env
+
+
+def update_environment(backend_url: str, id: str, environment: EnvironmentUpdate):
+    response = make_request(
+        "PUT",
+        f"{backend_url}/env/{id}",
+        json=environment.model_dump(exclude_none=True),
+    )
     environment = response.json()
     return environment["id"]
 
 
 def get_or_create_environment(
     backend_url: str, env: gymnasium.Env, user_id: str
 ) -> str:
     try:
-        env_id = get_environment(backend_url, env.spec.id)
+        env = get_environment(backend_url, env.spec.id)
+        env_id = env.id
     except HTTPError as e:
         if e.response.status_code == 404:
             env_id = create_environment(backend_url, env, user_id)
         else:
             raise e
     return env_id
```

### Comparing `loopquest-0.2.1/loopquest/datasets.py` & `loopquest-0.2.2/loopquest/datasets.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.1/loopquest/env/api.py` & `loopquest-0.2.2/loopquest/env/api.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.1/loopquest/env/gym_wrappers.py` & `loopquest-0.2.2/loopquest/env/gym_wrappers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from typing import Any
 import gymnasium
 from ..crud import (
     create_step,
+    get_environment,
+    update_environment,
     update_experiment,
     upload_rgb_as_image,
+    get_image_by_url,
 )
-from ..schema import (
-    StepCreate,
-    ExperimentUpdate,
-    ExperimentStatus,
-)
+from ..schema import StepCreate, ExperimentUpdate, ExperimentStatus, EnvironmentUpdate
 from ..utils import safe_jsonize
 from .space_utils import construct_space_val
 from ..api import get_backend_url, get_user_id
 from concurrent.futures import ThreadPoolExecutor
 
 
 class LoopquestGymWrapper(gymnasium.Wrapper):
@@ -103,17 +102,14 @@
         observation, info = self.env.reset(seed=seed, options=options)
         # TODO: update status for each of the environment and episode.
         update_experiment(
             self.backend_url,
             self.exp_id,
             ExperimentUpdate(status=ExperimentStatus.RUNNING),
         )
-        # TODO: #4 support multiple episodes, the frontend is not ready yet.
-        # else:
-        #     self.current_episode += 1
 
         info_jsonable = safe_jsonize(info)
         self.executor.submit(
             create_step,
             self.backend_url,
             StepCreate(
                 id=self.step_id,
@@ -129,18 +125,32 @@
 
     def close(self):
         update_experiment(
             self.backend_url,
             self.exp_id,
             ExperimentUpdate(status=ExperimentStatus.FINISHED),
         )
+        self._try_update_env_profile_image()
         self.env.close()
         self.executor.shutdown()
         # TODO: add a callback to compute custom metrics.
 
+    def _try_update_env_profile_image(self):
+        env_info = get_environment(self.backend_url, self.cloud_env_id)
+        env_update = EnvironmentUpdate()
+        if env_info.profile_image is None:
+            step_id = f"{self.exp_id}-{self.cloud_env_id}-0-1"
+            image_url = get_backend_url() + f"/step/{step_id}/image/0"
+            try:
+                img = get_image_by_url(image_url)
+                env_update.profile_image = image_url
+            except Exception as e:
+                print(e)
+        update_environment(self.backend_url, self.cloud_env_id, env_update)
+
     def render(self):
         if self.render_mode == "human":
             raise ValueError(
                 "'human' mode is not supported for cloud rendering. Please use other render mode."
             )
         elif self.render_mode in ["ansi", "ansi_list"]:
             raise ValueError(
```

### Comparing `loopquest-0.2.1/loopquest/env/space_utils.py` & `loopquest-0.2.2/loopquest/env/space_utils.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.1/loopquest/eval.py` & `loopquest-0.2.2/loopquest/eval.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.1/loopquest/policy/sb3_policy.py` & `loopquest-0.2.2/loopquest/policy/sb3_policy.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.1/loopquest/private_api.py` & `loopquest-0.2.2/loopquest/private_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import time
 import requests
 import os
 from .utils import update_or_append_env_var, is_docker_installed
 
+
+# For Dev
 # CLOUD_FRONTEND_URL = "http://localhost:5667"
 # CLOUD_BACKEND_URL = "http://localhost:5667/api"
 
-# For Dev
-CLOUD_FRONTEND_URL = "http://localhost:5667"
-CLOUD_BACKEND_URL = "http://localhost:5667/api"
+CLOUD_FRONTEND_URL = "https://www.loopquest.ai"
+CLOUD_BACKEND_URL = "https://www.loopquest.ai/api"
 TOKEN_ENV_VAR_NAME = "LOOPQUEST_USER_TOKEN"
 
 
 def is_cloud_instance_initialized():
     from .crud import get_cloud_user_id
 
     try:
```

### Comparing `loopquest-0.2.1/loopquest/schema.py` & `loopquest-0.2.2/loopquest/schema.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.1/loopquest/utils.py` & `loopquest-0.2.2/loopquest/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,32 +69,60 @@
         "Revolutionary",
         "Dynamic",
         "Epic",
         "Creative",
         "Ultimate",
         "Smart",
         "NewAge",
+        "Advanced",
+        "Interactive",
+        "Seamless",
+        "Integrated",
+        "CuttingEdge",
     ]
     nouns = [
         "Explorer",
         "Creator",
         "Vision",
         "Quest",
         "Journey",
         "Horizon",
         "Pioneer",
         "Odyssey",
         "Voyage",
         "Destination",
+        "Framework",
+        "Engine",
+        "Module",
+        "Navigator",
+        "Builder",
+    ]
+    colors = [
+        "Red",
+        "Blue",
+        "Green",
+        "Yellow",
+        "Orange",
+        "Purple",
+        "Black",
+        "White",
+        "Grey",
+        "Crimson",
+        "Cyan",
+        "Magenta",
+        "Teal",
+        "Silver",
+        "Gold",
     ]
 
     adjective = random.choice(adjectives)
+    color = random.choice(colors)
     noun = random.choice(nouns)
 
-    return f"{adjective}-{noun}"
+    return f"{color}-{adjective}-{noun}"
 
 
 def generate_experiment_name():
     adjectives = [
         "fuzzy",
         "giant",
         "tiny",
```

### Comparing `loopquest-0.2.1/loopquest.egg-info/PKG-INFO` & `loopquest-0.2.2/loopquest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopquest
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Production Tool for Embodied AI.
 Home-page: https://github.com/LoopMind-AI/loopquest
 Author: LoopMind
 Author-email: contactus@loopmind.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `loopquest-0.2.1/loopquest.egg-info/SOURCES.txt` & `loopquest-0.2.2/loopquest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.1/setup.py` & `loopquest-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="loopquest",
-    version="0.2.1",
+    version="0.2.2",
     description="A Production Tool for Embodied AI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="LoopMind",
     author_email="contactus@loopmind.ai",
     url="https://github.com/LoopMind-AI/loopquest",
     packages=find_packages(),
```


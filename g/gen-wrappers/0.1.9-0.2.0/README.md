# Comparing `tmp/gen_wrappers-0.1.9.tar.gz` & `tmp/gen_wrappers-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.1.9.tar", last modified: Fri May  3 18:04:35 2024, max compression
+gzip compressed data, was "gen_wrappers-0.2.0.tar", last modified: Fri May  3 18:22:15 2024, max compression
```

## Comparing `gen_wrappers-0.1.9.tar` & `gen_wrappers-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 18:04:35.886183 gen_wrappers-0.1.9/
--rw-rw-rw-   0        0        0      823 2024-05-03 18:04:35.883921 gen_wrappers-0.1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 18:04:35.569432 gen_wrappers-0.1.9/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.1.9/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:04:35.632963 gen_wrappers-0.1.9/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.1.9/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     5883 2024-05-02 20:42:34.000000 gen_wrappers-0.1.9/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     4184 2024-05-02 20:52:05.000000 gen_wrappers-0.1.9/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.1.9/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:04:35.707772 gen_wrappers-0.1.9/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.1.9/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1253 2024-05-02 15:57:38.000000 gen_wrappers-0.1.9/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.1.9/creator/base/base_request.py
--rw-rw-rw-   0        0        0     1569 2024-05-02 16:04:46.000000 gen_wrappers-0.1.9/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.1.9/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:04:35.771157 gen_wrappers-0.1.9/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.1.9/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9441 2024-05-02 21:06:52.000000 gen_wrappers-0.1.9/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0     2793 2024-05-02 20:53:05.000000 gen_wrappers-0.1.9/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.1.9/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:04:35.822454 gen_wrappers-0.1.9/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.1.9/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6340 2024-05-02 16:04:46.000000 gen_wrappers-0.1.9/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3846 2024-05-03 17:59:38.000000 gen_wrappers-0.1.9/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.1.9/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:04:35.880893 gen_wrappers-0.1.9/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      823 2024-05-03 18:04:35.000000 gen_wrappers-0.1.9/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      710 2024-05-03 18:04:35.000000 gen_wrappers-0.1.9/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 18:04:35.000000 gen_wrappers-0.1.9/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-03 18:04:35.000000 gen_wrappers-0.1.9/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-03 18:04:35.000000 gen_wrappers-0.1.9/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 18:04:35.886183 gen_wrappers-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1015 2024-05-03 18:00:10.000000 gen_wrappers-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:22:15.375227 gen_wrappers-0.2.0/
+-rw-rw-rw-   0        0        0      823 2024-05-03 18:22:15.373127 gen_wrappers-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 18:22:15.301812 gen_wrappers-0.2.0/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.2.0/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:22:15.319567 gen_wrappers-0.2.0/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.2.0/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     5883 2024-05-02 20:42:34.000000 gen_wrappers-0.2.0/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     4184 2024-05-02 20:52:05.000000 gen_wrappers-0.2.0/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.2.0/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:22:15.330583 gen_wrappers-0.2.0/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.2.0/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1253 2024-05-02 15:57:38.000000 gen_wrappers-0.2.0/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.2.0/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     1569 2024-05-02 16:04:46.000000 gen_wrappers-0.2.0/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.2.0/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:22:15.338575 gen_wrappers-0.2.0/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.2.0/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9441 2024-05-02 21:06:52.000000 gen_wrappers-0.2.0/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0     2793 2024-05-02 20:53:05.000000 gen_wrappers-0.2.0/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.2.0/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:22:15.347480 gen_wrappers-0.2.0/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.2.0/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6344 2024-05-03 18:21:55.000000 gen_wrappers-0.2.0/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3973 2024-05-03 18:13:30.000000 gen_wrappers-0.2.0/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.2.0/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:22:15.371056 gen_wrappers-0.2.0/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      823 2024-05-03 18:22:15.000000 gen_wrappers-0.2.0/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      710 2024-05-03 18:22:15.000000 gen_wrappers-0.2.0/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 18:22:15.000000 gen_wrappers-0.2.0/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-03 18:22:15.000000 gen_wrappers-0.2.0/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-03 18:22:15.000000 gen_wrappers-0.2.0/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 18:22:15.376227 gen_wrappers-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2024-05-03 18:22:12.000000 gen_wrappers-0.2.0/setup.py
```

### Comparing `gen_wrappers-0.1.9/PKG-INFO` & `gen_wrappers-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.1.9
+Version: 0.2.0
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.1.9/creator/auto/creator_auto.py` & `gen_wrappers-0.2.0/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.9/creator/auto/request_auto.py` & `gen_wrappers-0.2.0/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.9/creator/auto/response_auto.py` & `gen_wrappers-0.2.0/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.9/creator/base/base_app.py` & `gen_wrappers-0.2.0/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.9/creator/base/base_request.py` & `gen_wrappers-0.2.0/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.9/creator/base/base_response.py` & `gen_wrappers-0.2.0/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.9/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.2.0/creator/cmfy/creator_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.9/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.2.0/creator/cmfy/request_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.9/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.2.0/creator/fcus_api/creator_fcus_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             raise ValueError("Invalid parameters for creation")
         if model is not None and model not in self.loaded_models:
             self.loaded_models.append(model)
         max_cached_models = os.environ.get("MAX_CACHED_MODELS", 3)
         if len(self.loaded_models) > max_cached_models:
             self.loaded_models = self.loaded_models[-max_cached_models:]
 
-        data = json.dumps(params.__dict__)
+        data = json.dumps(params.model_dump())
         headers = {'Content-Type': 'application/json'}
         response = requests.post(url, data=data, headers=headers)
         # If we have a 422 here, print what the unprocessable entity is
         if response.status_code == 422:
             logger.warning(f"Unprocessable entity: {response.text}")
         response.raise_for_status()
```

### Comparing `gen_wrappers-0.1.9/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.2.0/creator/fcus_api/request_fcus_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,23 +31,26 @@
     inpaint_engine: str = "v1"
     freeu_enabled: bool = False
     freeu_b1: float = 1.01
     freeu_b2: float = 1.02
     freeu_s1: float = 0.99
     freeu_s2: float = 0.95
 
+
 @dataclass
 class Lora:
     model_name: str = ""
     weight: float = 1.0
 
+
 class FcusTxt2Img(BaseRequest):
     prompt: str = ""
     negative_prompt: str = ""
-    style_selections: List[str] = Field(default_factory=list, examples=[["Fooocus V2", "Fooocus Enhance", "Fooocus Sharp"]])
+    style_selections: List[str] = Field(default_factory=list,
+                                        examples=[["Fooocus V2", "Fooocus Enhance", "Fooocus Sharp"]])
     performance_selection: str = "Speed"
     aspect_ratios_selection: str = "1152*896"
     image_number: int = 2
     image_seed: int = -1
     sharpness: float = 0.0
     guidance_scale: float = 7.5
     base_model_name: str = "RunDiffusion-XL-Photo.safetensors"
@@ -60,15 +63,16 @@
 
 
 class FcusUpscaleOrVary(BaseRequest):
     input_image: str = ""
     uov_method: str = ""
     prompt: str = ""
     negative_prompt: str = ""
-    style_selections: List[str] = Field(default_factory=list, examples=[["Fooocus V2", "Fooocus Enhance", "Fooocus Sharp"]])
+    style_selections: List[str] = Field(default_factory=list,
+                                        examples=[["Fooocus V2", "Fooocus Enhance", "Fooocus Sharp"]])
     performance_selection: str = ""
     aspect_ratios_selection: str = ""
     image_number: int = 1
     image_seed: int = -1
     sharpness: float = 0.0
     guidance_scale: float = 7.5
     base_model_name: str = "RunDiffusion-XL-Photo.safetensors"
@@ -83,15 +87,16 @@
 class FcusInpaintOrOutpaint(BaseRequest):
     request_params: str = ""
     input_image: str = ""
     input_mask: str = ""
     outpaint_selections: List[str] = Field(default_factory=list, examples=[])
     prompt: str = ""
     negative_prompt: str = ""
-    style_selections: List[str] = Field(default_factory=list, examples=[["Fooocus V2", "Fooocus Enhance", "Fooocus Sharp"]])
+    style_selections: List[str] = Field(default_factory=list,
+                                        examples=[["Fooocus V2", "Fooocus Enhance", "Fooocus Sharp"]])
     performance_selection: str = ""
     aspect_ratios_selection: str = ""
     image_number: int = 1
     image_seed: int = -1
     sharpness: float = 0.0
     guidance_scale: float = 7.5
     base_model_name: str = "RunDiffusion-XL-Photo.safetensors"
```

### Comparing `gen_wrappers-0.1.9/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.2.0/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.9/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.2.0/gen_wrappers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.1.9
+Version: 0.2.0
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.1.9/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.2.0/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.9/setup.py` & `gen_wrappers-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.1.9',
+    version='0.2.0',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```


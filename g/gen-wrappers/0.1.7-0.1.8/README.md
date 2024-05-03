# Comparing `tmp/gen_wrappers-0.1.7.tar.gz` & `tmp/gen_wrappers-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.1.7.tar", last modified: Thu May  2 21:00:09 2024, max compression
+gzip compressed data, was "gen_wrappers-0.1.8.tar", last modified: Thu May  2 21:07:05 2024, max compression
```

## Comparing `gen_wrappers-0.1.7.tar` & `gen_wrappers-0.1.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 21:00:09.168674 gen_wrappers-0.1.7/
--rw-rw-rw-   0        0        0      823 2024-05-02 21:00:09.164861 gen_wrappers-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 21:00:09.095070 gen_wrappers-0.1.7/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.1.7/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 21:00:09.107038 gen_wrappers-0.1.7/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.1.7/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     5883 2024-05-02 20:42:34.000000 gen_wrappers-0.1.7/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     4184 2024-05-02 20:52:05.000000 gen_wrappers-0.1.7/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.1.7/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-02 21:00:09.126863 gen_wrappers-0.1.7/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.1.7/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1253 2024-05-02 15:57:38.000000 gen_wrappers-0.1.7/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.1.7/creator/base/base_request.py
--rw-rw-rw-   0        0        0     1569 2024-05-02 16:04:46.000000 gen_wrappers-0.1.7/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.1.7/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-02 21:00:09.132512 gen_wrappers-0.1.7/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.1.7/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9974 2024-05-02 20:53:05.000000 gen_wrappers-0.1.7/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0     2793 2024-05-02 20:53:05.000000 gen_wrappers-0.1.7/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.1.7/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-02 21:00:09.139517 gen_wrappers-0.1.7/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.1.7/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6340 2024-05-02 16:04:46.000000 gen_wrappers-0.1.7/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3911 2024-05-02 20:32:31.000000 gen_wrappers-0.1.7/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.1.7/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-02 21:00:09.162859 gen_wrappers-0.1.7/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      823 2024-05-02 21:00:08.000000 gen_wrappers-0.1.7/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      710 2024-05-02 21:00:08.000000 gen_wrappers-0.1.7/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 21:00:08.000000 gen_wrappers-0.1.7/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-02 21:00:08.000000 gen_wrappers-0.1.7/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-02 21:00:08.000000 gen_wrappers-0.1.7/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 21:00:09.168674 gen_wrappers-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1015 2024-05-02 20:59:58.000000 gen_wrappers-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:07:05.932774 gen_wrappers-0.1.8/
+-rw-rw-rw-   0        0        0      823 2024-05-02 21:07:05.931774 gen_wrappers-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 21:07:05.897988 gen_wrappers-0.1.8/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.1.8/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:07:05.902524 gen_wrappers-0.1.8/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.1.8/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     5883 2024-05-02 20:42:34.000000 gen_wrappers-0.1.8/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     4184 2024-05-02 20:52:05.000000 gen_wrappers-0.1.8/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.1.8/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:07:05.906946 gen_wrappers-0.1.8/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.1.8/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1253 2024-05-02 15:57:38.000000 gen_wrappers-0.1.8/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.1.8/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     1569 2024-05-02 16:04:46.000000 gen_wrappers-0.1.8/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.1.8/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:07:05.912072 gen_wrappers-0.1.8/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.1.8/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9441 2024-05-02 21:06:52.000000 gen_wrappers-0.1.8/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0     2793 2024-05-02 20:53:05.000000 gen_wrappers-0.1.8/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.1.8/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:07:05.916075 gen_wrappers-0.1.8/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.1.8/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6340 2024-05-02 16:04:46.000000 gen_wrappers-0.1.8/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3911 2024-05-02 20:32:31.000000 gen_wrappers-0.1.8/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.1.8/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:07:05.930775 gen_wrappers-0.1.8/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      823 2024-05-02 21:07:05.000000 gen_wrappers-0.1.8/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      710 2024-05-02 21:07:05.000000 gen_wrappers-0.1.8/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 21:07:05.000000 gen_wrappers-0.1.8/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-02 21:07:05.000000 gen_wrappers-0.1.8/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-02 21:07:05.000000 gen_wrappers-0.1.8/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 21:07:05.932774 gen_wrappers-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2024-05-02 21:07:01.000000 gen_wrappers-0.1.8/setup.py
```

### Comparing `gen_wrappers-0.1.7/PKG-INFO` & `gen_wrappers-0.1.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.1.7
+Version: 0.1.8
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.1.7/creator/auto/creator_auto.py` & `gen_wrappers-0.1.8/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.7/creator/auto/request_auto.py` & `gen_wrappers-0.1.8/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.7/creator/auto/response_auto.py` & `gen_wrappers-0.1.8/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.7/creator/base/base_app.py` & `gen_wrappers-0.1.8/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.7/creator/base/base_request.py` & `gen_wrappers-0.1.8/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.7/creator/base/base_response.py` & `gen_wrappers-0.1.8/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.7/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.1.8/creator/cmfy/creator_cmfy.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,38 +18,14 @@
 from creator.base.job_status import JobStatus
 from creator.cmfy.request_cmfy import CmfyWorkflow
 from creator.cmfy.response_cmfy import ResponseCmfy
 
 logger = logging.getLogger(__name__)
 
 
-@dataclasses.dataclass
-class NodeInput:
-    inputs: Dict[str, Any]
-    class_type: str
-
-
-@dataclasses.dataclass
-class CmfyWorkflow:
-    prompt: str
-    nodes: Dict[str, NodeInput]
-
-    @staticmethod
-    def from_json(params: CmfyWorkflow) -> str:
-        json_str = params.workflow_json
-        return json_str
-
-    def to_json(self) -> str:
-        dump = {}
-        for node_id, node in self.nodes.items():
-            dump[node_id] = dataclasses.asdict(node)
-
-        return json.dumps({"prompt": dump})
-
-
 class AppCmfy(BaseApp):
     param_classes = [CmfyWorkflow]
     output = {}
 
     def __init__(self):
         super().__init__()
         focus_port = os.environ.get("PORT_CMFY", 8888)
```

### Comparing `gen_wrappers-0.1.7/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.1.8/creator/cmfy/request_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.7/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.1.8/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.7/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.1.8/creator/fcus_api/request_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.7/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.1.8/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.7/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.1.8/gen_wrappers.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.1.7
+Version: 0.1.8
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.1.7/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.1.8/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.7/setup.py` & `gen_wrappers-0.1.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.1.7',
+    version='0.1.8',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```


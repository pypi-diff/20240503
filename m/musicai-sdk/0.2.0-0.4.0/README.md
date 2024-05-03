# Comparing `tmp/musicai_sdk-0.2.0.tar.gz` & `tmp/musicai_sdk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicai_sdk-0.2.0.tar", max compression
+gzip compressed data, was "musicai_sdk-0.4.0.tar", max compression
```

## Comparing `musicai_sdk-0.2.0.tar` & `musicai_sdk-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1125 2024-01-24 01:04:57.245806 musicai_sdk-0.2.0/README.md
--rw-r--r--   0        0        0       33 2024-01-24 01:04:57.245806 musicai_sdk-0.2.0/musicai_sdk/__init__.py
--rw-r--r--   0        0        0     2556 2024-01-24 01:04:57.245806 musicai_sdk-0.2.0/musicai_sdk/client.py
--rw-r--r--   0        0        0      437 2024-01-24 01:04:57.245806 musicai_sdk-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 musicai_sdk-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2049 2024-05-03 02:57:24.684399 musicai_sdk-0.4.0/README.md
+-rw-r--r--   0        0        0       76 2024-05-03 02:57:24.684399 musicai_sdk-0.4.0/musicai_sdk/__init__.py
+-rw-r--r--   0        0        0     3210 2024-05-03 02:57:24.684399 musicai_sdk-0.4.0/musicai_sdk/client.py
+-rw-r--r--   0        0        0     3476 2024-05-03 02:57:24.684399 musicai_sdk-0.4.0/musicai_sdk/process_folder.py
+-rw-r--r--   0        0        0      437 2024-05-03 02:57:24.684399 musicai_sdk-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2670 1970-01-01 00:00:00.000000 musicai_sdk-0.4.0/PKG-INFO
```

### Comparing `musicai_sdk-0.2.0/musicai_sdk/client.py` & `musicai_sdk-0.4.0/musicai_sdk/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import time
 import requests
 from requests.exceptions import HTTPError
 
+
 class MusicAiClient:
-    def __init__(self, api_key):
+    def __init__(self, api_key, job_monitor_interval=2):
         self.api_key = api_key
         self.base_url = 'https://api.music.ai/api'
+        self.job_monitor_interval = job_monitor_interval
 
     def get_headers(self):
         return {
             'Authorization': self.api_key
         }
 
     def upload_file(self, file_path):
@@ -24,14 +27,20 @@
 
     def get_job(self, job_id):
         response = requests.get(f'{self.base_url}/job/{job_id}', headers=self.get_headers())
         if response.status_code // 100 != 2:
             raise HTTPError(f'Error getting job: {response.status_code} {response.text}')
         return response.json()
 
+    def get_job_status(self, job_id):
+        response = requests.get(f'{self.base_url}/job/{job_id}/status', headers=self.get_headers())
+        if response.status_code // 100 != 2:
+            raise HTTPError(f'Error getting job: {response.status_code} {response.text}')
+        return response.json()
+
     def get_jobs(self):
         response = requests.get(f'{self.base_url}/job', headers=self.get_headers())
         if response.status_code // 100 != 2:
             raise HTTPError(f'Error getting jobs: {response.status_code} {response.text}')
         return response.json()
 
     def create_job(self, job_name, workflow_id, params):
@@ -47,12 +56,19 @@
 
     def delete_job(self, job_id):
         response = requests.delete(f'{self.base_url}/job/{job_id}', headers=self.get_headers())
         if response.status_code // 100 != 2:
             raise HTTPError(f'Error deleting job: {response.status_code} {response.text}')
         return response.json()
 
+    def wait_for_job_completion(self, id):
+        while True:
+            job = self.get_job_status(id)
+            if job['status'] in ['SUCCEEDED', 'FAILED']:
+                return self.get_job(id)
+            time.sleep(self.job_monitor_interval),
+
     def get_application_info(self):
         response = requests.get(f'{self.base_url}/application', headers=self.get_headers())
         if response.status_code // 100 != 2:
             raise HTTPError(f'Error getting application info: {response.status_code} {response.text}')
-        return response.json()
+        return response.json()
```

### Comparing `musicai_sdk-0.2.0/PKG-INFO` & `musicai_sdk-0.4.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,66 @@
-Metadata-Version: 2.1
-Name: musicai-sdk
-Version: 0.2.0
-Summary: Python sdk for music.ai
-License: MIT
-Author: Music.ai Support
-Author-email: support@music.ai
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Description-Content-Type: text/markdown
-
 # Music.ai Python Client Library
 
 This is a Python client library for the Music.AI API. For more information on the API and its capabilities, see the [API documentation](https://music.ai/docs/getting-started/introduction/).
 
 ## Installation
 
 You can install the library via pip:
 
 ```bash
 pip install musicai_sdk
 ```
 
 ## Usage
 
+Here's an example of how you can use the client to upload a local file, create a job and more:
+
+
 ```python
 from musicai_sdk import MusicAiClient
 
 client = MusicAiClient(api_key='your-api-key')
 
 # Get application info
 app_info = client.get_application_info()
 print('Application Info:', app_info)
 
-# Upload local ile
+# Upload local file
 file_url = client.upload_file(file_path='your-file-path')
 print('File Url:', file_url)
 
 # Create Job
 workflow_params = {
     'inputUrl': file_url,
 }
 create_job_info = client.create_job(job_name='your-job-name', workflow_id='your-workflow-id',params=workflow_params)
 job_id = create_job_info['id']
 print('Job Created:', job_id)
 
+# Wait for job to complete
+job_info = client.wait_for_job_completion(job_id)
+print('Job Status:', job_info['status'])
+print('Job Result:', job_info['result'])
+
 # Get job info
 job_info = client.get_job(job_id=job_id)
 print('Job Status:', job_info['status'])
 print('Job Result:', job_info['result'])
 
 # Delete job
 client.delete_job(job_id=job_id)
 
 # Get all jobs
 jobs = client.get_jobs()
 print('Jobs:', jobs)
 
 ```
 
+The library also provides a `process_folder` function that you can use to process all files in a folder. Please keep in mind this requires a workflow with a single input file. Here's an example of how you can use this function:
+
+```python
+from musicai_sdk import MusicAiClient, process_folder
+
+client = MusicAiClient(api_key='your-api-key')
+
+# Use the "parallelism" parameter to set the number of parallel processes and the "delete" parameter to delete the job at MusicAI platform after download completion.
+process_folder(input_folder="local input folder", output_folder="local output folder", workflow_id="workflow ID", client=client, parallelism=10, delete=True)
```


# Comparing `tmp/custom_erp_connector-0.24.tar.gz` & `tmp/custom_erp_connector-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_erp_connector-0.24.tar", last modified: Fri May  3 13:26:35 2024, max compression
+gzip compressed data, was "custom_erp_connector-0.3.tar", last modified: Tue Apr 16 09:00:37 2024, max compression
```

## Comparing `custom_erp_connector-0.24.tar` & `custom_erp_connector-0.3.tar`

### file list

```diff
@@ -1,44 +1,42 @@
-drwxr-xr-x   0 dinesh.sharma (285385805) 1798103863        0 2024-05-03 13:26:35.952849 custom_erp_connector-0.24/
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     1543 2024-05-03 13:26:35.952732 custom_erp_connector-0.24/PKG-INFO
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     1290 2024-04-17 07:13:21.000000 custom_erp_connector-0.24/README.md
-drwxr-xr-x   0 dinesh.sharma (285385805) 1798103863        0 2024-05-03 13:26:35.945808 custom_erp_connector-0.24/custom_erp_connector.egg-info/
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     1543 2024-05-03 13:26:35.000000 custom_erp_connector-0.24/custom_erp_connector.egg-info/PKG-INFO
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     1178 2024-05-03 13:26:35.000000 custom_erp_connector-0.24/custom_erp_connector.egg-info/SOURCES.txt
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863        1 2024-05-03 13:26:35.000000 custom_erp_connector-0.24/custom_erp_connector.egg-info/dependency_links.txt
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863       58 2024-05-03 13:26:35.000000 custom_erp_connector-0.24/custom_erp_connector.egg-info/entry_points.txt
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863      216 2024-05-03 13:26:35.000000 custom_erp_connector-0.24/custom_erp_connector.egg-info/requires.txt
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863       14 2024-05-03 13:26:35.000000 custom_erp_connector-0.24/custom_erp_connector.egg-info/top_level.txt
-drwxr-xr-x   0 dinesh.sharma (285385805) 1798103863        0 2024-05-03 13:26:35.946161 custom_erp_connector-0.24/erp_connector/
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863        2 2024-04-15 08:26:18.000000 custom_erp_connector-0.24/erp_connector/__init__.py
-drwxr-xr-x   0 dinesh.sharma (285385805) 1798103863        0 2024-05-03 13:26:35.946984 custom_erp_connector-0.24/erp_connector/clients/
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863        0 2024-04-15 08:08:29.000000 custom_erp_connector-0.24/erp_connector/clients/__init__.py
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     1627 2024-04-19 06:21:22.000000 custom_erp_connector-0.24/erp_connector/clients/euclid_client.py
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     6765 2024-04-18 09:22:06.000000 custom_erp_connector-0.24/erp_connector/clients/one_integration_client.py
-drwxr-xr-x   0 dinesh.sharma (285385805) 1798103863        0 2024-05-03 13:26:35.947289 custom_erp_connector-0.24/erp_connector/config/
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863        0 2024-04-15 08:08:29.000000 custom_erp_connector-0.24/erp_connector/config/__init__.py
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     1435 2024-04-18 09:13:42.000000 custom_erp_connector-0.24/erp_connector/config/config_loader.py
-drwxr-xr-x   0 dinesh.sharma (285385805) 1798103863        0 2024-05-03 13:26:35.949213 custom_erp_connector-0.24/erp_connector/db/
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863        0 2024-04-15 08:08:29.000000 custom_erp_connector-0.24/erp_connector/db/__init__.py
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863      529 2024-04-18 09:32:57.000000 custom_erp_connector-0.24/erp_connector/db/db_connector.py
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     2382 2024-04-18 09:29:44.000000 custom_erp_connector-0.24/erp_connector/db/db_loader.py
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     3323 2024-04-18 10:29:08.000000 custom_erp_connector-0.24/erp_connector/db/mssql_connector.py
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     3467 2024-04-18 09:32:57.000000 custom_erp_connector-0.24/erp_connector/db/mysql_connector.py
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     3587 2024-05-03 13:26:14.000000 custom_erp_connector-0.24/erp_connector/db/oracle_connector.py
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     2540 2024-04-18 10:30:39.000000 custom_erp_connector-0.24/erp_connector/db/postgresql_connector.py
-drwxr-xr-x   0 dinesh.sharma (285385805) 1798103863        0 2024-05-03 13:26:35.949425 custom_erp_connector-0.24/erp_connector/exceptions/
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     1491 2024-04-15 08:08:29.000000 custom_erp_connector-0.24/erp_connector/exceptions/__init__.py
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     1274 2024-04-18 09:32:57.000000 custom_erp_connector-0.24/erp_connector/scheduler.py
-drwxr-xr-x   0 dinesh.sharma (285385805) 1798103863        0 2024-05-03 13:26:35.950149 custom_erp_connector-0.24/erp_connector/service/
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863        0 2024-04-15 08:08:29.000000 custom_erp_connector-0.24/erp_connector/service/__init__.py
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     6650 2024-04-22 18:21:31.000000 custom_erp_connector-0.24/erp_connector/service/connector_service.py
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     3476 2024-04-18 09:49:31.000000 custom_erp_connector-0.24/erp_connector/service/event_service.py
-drwxr-xr-x   0 dinesh.sharma (285385805) 1798103863        0 2024-05-03 13:26:35.952366 custom_erp_connector-0.24/erp_connector/utils/
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     1065 2024-04-16 11:45:13.000000 custom_erp_connector-0.24/erp_connector/utils/InProcessBatch.py
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863      116 2024-04-15 08:08:29.000000 custom_erp_connector-0.24/erp_connector/utils/__init__.py
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     2865 2024-04-18 05:49:23.000000 custom_erp_connector-0.24/erp_connector/utils/custlogging.py
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863      426 2024-04-15 12:19:39.000000 custom_erp_connector-0.24/erp_connector/utils/file_utils.py
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     2679 2024-04-22 18:21:31.000000 custom_erp_connector-0.24/erp_connector/utils/mysql_query_utils.py
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     1748 2024-04-16 11:13:57.000000 custom_erp_connector-0.24/erp_connector/utils/retryable_session.py
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863      317 2024-04-15 08:08:29.000000 custom_erp_connector-0.24/erp_connector/utils/singleton.py
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863       38 2024-05-03 13:26:35.952886 custom_erp_connector-0.24/setup.cfg
--rw-r--r--   0 dinesh.sharma (285385805) 1798103863     1171 2024-05-03 13:26:23.000000 custom_erp_connector-0.24/setup.py
+drwxr-xr-x   0 dinesh.sharma (285385805) 1798103863        0 2024-04-16 09:00:37.159658 custom_erp_connector-0.3/
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863      275 2024-04-16 09:00:37.159528 custom_erp_connector-0.3/PKG-INFO
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863       22 2024-04-15 08:21:31.000000 custom_erp_connector-0.3/README.md
+drwxr-xr-x   0 dinesh.sharma (285385805) 1798103863        0 2024-04-16 09:00:37.152984 custom_erp_connector-0.3/custom_erp_connector.egg-info/
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863      275 2024-04-16 09:00:37.000000 custom_erp_connector-0.3/custom_erp_connector.egg-info/PKG-INFO
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863     1103 2024-04-16 09:00:37.000000 custom_erp_connector-0.3/custom_erp_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863        1 2024-04-16 09:00:37.000000 custom_erp_connector-0.3/custom_erp_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863       58 2024-04-16 09:00:37.000000 custom_erp_connector-0.3/custom_erp_connector.egg-info/entry_points.txt
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863      214 2024-04-16 09:00:37.000000 custom_erp_connector-0.3/custom_erp_connector.egg-info/requires.txt
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863       14 2024-04-16 09:00:37.000000 custom_erp_connector-0.3/custom_erp_connector.egg-info/top_level.txt
+drwxr-xr-x   0 dinesh.sharma (285385805) 1798103863        0 2024-04-16 09:00:37.153317 custom_erp_connector-0.3/erp_connector/
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863        2 2024-04-15 08:26:18.000000 custom_erp_connector-0.3/erp_connector/__init__.py
+drwxr-xr-x   0 dinesh.sharma (285385805) 1798103863        0 2024-04-16 09:00:37.153728 custom_erp_connector-0.3/erp_connector/clients/
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863        0 2024-04-15 08:08:29.000000 custom_erp_connector-0.3/erp_connector/clients/__init__.py
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863     4916 2024-04-16 06:18:00.000000 custom_erp_connector-0.3/erp_connector/clients/one_integration_client.py
+drwxr-xr-x   0 dinesh.sharma (285385805) 1798103863        0 2024-04-16 09:00:37.154129 custom_erp_connector-0.3/erp_connector/config/
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863        0 2024-04-15 08:08:29.000000 custom_erp_connector-0.3/erp_connector/config/__init__.py
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863      921 2024-04-16 06:21:41.000000 custom_erp_connector-0.3/erp_connector/config/config_loader.py
+drwxr-xr-x   0 dinesh.sharma (285385805) 1798103863        0 2024-04-16 09:00:37.155715 custom_erp_connector-0.3/erp_connector/db/
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863        0 2024-04-15 08:08:29.000000 custom_erp_connector-0.3/erp_connector/db/__init__.py
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863      533 2024-04-16 06:33:31.000000 custom_erp_connector-0.3/erp_connector/db/db_connector.py
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863     1342 2024-04-16 06:29:07.000000 custom_erp_connector-0.3/erp_connector/db/db_loader.py
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863     2505 2024-04-16 06:34:10.000000 custom_erp_connector-0.3/erp_connector/db/mssql_connector.py
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863     2405 2024-04-16 06:32:17.000000 custom_erp_connector-0.3/erp_connector/db/mysql_connector.py
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863     1673 2024-04-16 06:34:34.000000 custom_erp_connector-0.3/erp_connector/db/postgresql_connector.py
+drwxr-xr-x   0 dinesh.sharma (285385805) 1798103863        0 2024-04-16 09:00:37.155999 custom_erp_connector-0.3/erp_connector/exceptions/
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863     1491 2024-04-15 08:08:29.000000 custom_erp_connector-0.3/erp_connector/exceptions/__init__.py
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863      836 2024-04-15 10:57:41.000000 custom_erp_connector-0.3/erp_connector/scheduler.py
+drwxr-xr-x   0 dinesh.sharma (285385805) 1798103863        0 2024-04-16 09:00:37.156783 custom_erp_connector-0.3/erp_connector/service/
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863        0 2024-04-15 08:08:29.000000 custom_erp_connector-0.3/erp_connector/service/__init__.py
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863     2883 2024-04-16 06:33:31.000000 custom_erp_connector-0.3/erp_connector/service/connector_service.py
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863     1474 2024-04-15 12:18:40.000000 custom_erp_connector-0.3/erp_connector/service/sqlite_service.py
+drwxr-xr-x   0 dinesh.sharma (285385805) 1798103863        0 2024-04-16 09:00:37.159270 custom_erp_connector-0.3/erp_connector/utils/
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863     1065 2024-04-15 08:08:29.000000 custom_erp_connector-0.3/erp_connector/utils/InProcessBatch.py
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863      116 2024-04-15 08:08:29.000000 custom_erp_connector-0.3/erp_connector/utils/__init__.py
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863     2561 2024-04-15 08:08:29.000000 custom_erp_connector-0.3/erp_connector/utils/custlogging.py
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863      426 2024-04-15 12:19:39.000000 custom_erp_connector-0.3/erp_connector/utils/file_utils.py
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863     2388 2024-04-16 05:45:50.000000 custom_erp_connector-0.3/erp_connector/utils/mysql_query_utils.py
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863     1748 2024-04-15 08:08:29.000000 custom_erp_connector-0.3/erp_connector/utils/retryable_session.py
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863      317 2024-04-15 08:08:29.000000 custom_erp_connector-0.3/erp_connector/utils/singleton.py
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863       38 2024-04-16 09:00:37.159693 custom_erp_connector-0.3/setup.cfg
+-rw-r--r--   0 dinesh.sharma (285385805) 1798103863     1168 2024-04-16 09:00:31.000000 custom_erp_connector-0.3/setup.py
```

### Comparing `custom_erp_connector-0.24/custom_erp_connector.egg-info/SOURCES.txt` & `custom_erp_connector-0.3/custom_erp_connector.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,27 @@
 custom_erp_connector.egg-info/dependency_links.txt
 custom_erp_connector.egg-info/entry_points.txt
 custom_erp_connector.egg-info/requires.txt
 custom_erp_connector.egg-info/top_level.txt
 erp_connector/__init__.py
 erp_connector/scheduler.py
 erp_connector/clients/__init__.py
-erp_connector/clients/euclid_client.py
 erp_connector/clients/one_integration_client.py
 erp_connector/config/__init__.py
 erp_connector/config/config_loader.py
 erp_connector/db/__init__.py
 erp_connector/db/db_connector.py
 erp_connector/db/db_loader.py
 erp_connector/db/mssql_connector.py
 erp_connector/db/mysql_connector.py
-erp_connector/db/oracle_connector.py
 erp_connector/db/postgresql_connector.py
 erp_connector/exceptions/__init__.py
 erp_connector/service/__init__.py
 erp_connector/service/connector_service.py
-erp_connector/service/event_service.py
+erp_connector/service/sqlite_service.py
 erp_connector/utils/InProcessBatch.py
 erp_connector/utils/__init__.py
 erp_connector/utils/custlogging.py
 erp_connector/utils/file_utils.py
 erp_connector/utils/mysql_query_utils.py
 erp_connector/utils/retryable_session.py
 erp_connector/utils/singleton.py
```

### Comparing `custom_erp_connector-0.24/erp_connector/clients/one_integration_client.py` & `custom_erp_connector-0.3/erp_connector/clients/one_integration_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,23 @@
 import json
-import os
 
 import requests
 from erp_connector.utils.retryable_session import RetryableSession
-from erp_connector.utils.custlogging import LoggerProvider
-from erp_connector.service.event_service import publish_event, get_request_data
-from erp_connector.utils.custlogging import CustomLogHandler
-
-logger = LoggerProvider().get_logger(os.path.basename(__file__))
-
-logs = []
-log_handler = CustomLogHandler(logs)
-logger.addHandler(log_handler)
 
 
 class OneIntegrationClient:
 
-    def __init__(self, erp_config):
-        self.base_url = f'https://api-{erp_config.env}.clear.in/one-integration'
+    def __init__(self,erp_config):
+        self.base_url = f'https://one-integration-{erp_config.env}-http-server.internal.cleartax.co'
         self.auth_token = erp_config.authToken
         self.x_erp_instance_id = erp_config.erpInstanceId
 
-    def ping(self):
-        session = RetryableSession()
-        url = f"{self.base_url}/erp_connection/ping"
-        headers = {
-            "accept": "*/*",
-            "x-clear-auth-token": self.auth_token,
-            "x-erp-instance-id": self.x_erp_instance_id
-        }
-
-        try:
-            response = session.get(url, headers=headers, timeout=45, max_retry=2, backoff_factor=1)
-            response.raise_for_status()
-            response_data = response.json()
-            return response_data
-        except requests.exceptions.HTTPError as http_err:
-            raise Exception(f"HTTP error occurred: {http_err}")
-        except requests.exceptions.ConnectionError as conn_err:
-            raise Exception(f"Connection error occurred: {conn_err}")
-        except requests.exceptions.Timeout as timeout_err:
-            raise Exception(f"Timeout error occurred: {timeout_err}")
-        except requests.exceptions.RequestException as req_err:
-            raise Exception(f"An error occurred: {req_err}")
-
     def get_command(self):
         session = RetryableSession()
-        url = f"{self.base_url}/command/get"
+        url = f"{self.base_url}/api/one-integration/integration/command/get"
         headers = {
             "accept": "*/*",
             "x-clear-auth-token": self.auth_token,
             "x-erp-instance-id": self.x_erp_instance_id
         }
 
         try:
@@ -63,66 +30,63 @@
         except requests.exceptions.ConnectionError as conn_err:
             raise Exception(f"Connection error occurred: {conn_err}")
         except requests.exceptions.Timeout as timeout_err:
             raise Exception(f"Timeout error occurred: {timeout_err}")
         except requests.exceptions.RequestException as req_err:
             raise Exception(f"An error occurred: {req_err}")
 
-    def get_presign(self, file_name, command_id,trace_id):
+    def get_presign(self, file_name, command_id):
         session = RetryableSession()
-        url = f"{self.base_url}/action/pre_sign?file_name={file_name}&command_id={command_id}"
+        url = f"{self.base_url}/api/one-integration/integration/action/pre_sign?file_name={file_name}&command_id={command_id}"
         headers = {
             "accept": "*/*",
             "x-clear-auth-token": self.auth_token,
             "x-erp-instance-id": self.x_erp_instance_id,
             "fileContentType": "application/zip"
         }
 
         try:
             response = session.get(url, headers=headers, timeout=45)
             response.raise_for_status()
             response_data = response.json()
-            logger.info(f"presign response: {response_data}")
-            publish_event(get_request_data(trace_id,command_id,"",self.x_erp_instance_id),logs)
             return response_data
         except requests.exceptions.HTTPError as http_err:
             raise Exception(f"HTTP error occurred: {http_err}")
         except requests.exceptions.ConnectionError as conn_err:
             raise Exception(f"Connection error occurred: {conn_err}")
         except requests.exceptions.Timeout as timeout_err:
             raise Exception(f"Timeout error occurred: {timeout_err}")
         except requests.exceptions.RequestException as req_err:
             raise Exception(f"An error occurred: {req_err}")
 
-    def upload_to_s3(self, upload_url, file_path,trace_id):
+    def upload_to_s3(self, upload_url, file_path):
         session = RetryableSession()
         headers = {
             'Content-Type': 'application/zip'
         }
         payload = open(file_path, 'rb')
 
         try:
             response = session.put(upload_url, headers=headers, data=payload, timeout=45)
             response.raise_for_status()
             if response.status_code != 200 and response.status_code != 201:
-                logger.info("s3 upload failure: ", response.text)
-                publish_event(get_request_data(trace_id,"","",""),logs)
+                print("s3 upload failure: ", response.text)
             return None
         except requests.exceptions.HTTPError as http_err:
             raise Exception(f"HTTP error occurred: {http_err}")
         except requests.exceptions.ConnectionError as conn_err:
             raise Exception(f"Connection error occurred: {conn_err}")
         except requests.exceptions.Timeout as timeout_err:
             raise Exception(f"Timeout error occurred: {timeout_err}")
         except requests.exceptions.RequestException as req_err:
             raise Exception(f"An error occurred: {req_err}")
 
-    def post_command(self, presign_url, command_id,trace_id):
+    def post_command(self, presign_url, command_id):
         session = RetryableSession()
-        url = f"{self.base_url}/command/send/result"
+        url = f"{self.base_url}/api/one-integration/integration/command/send/result"
         headers = {
             "accept": "*/*",
             'Content-Type': 'application/json',
             "x-clear-auth-token": self.auth_token,
             "x-erp-instance-id": self.x_erp_instance_id
         }
         payload = json.dumps({
@@ -131,22 +95,19 @@
                 "s3Details": [
                     {
                         "url": presign_url
                     }
                 ]
             }
         })
-        logger.info(f"post command header: {headers} payload: {payload}")
-        publish_event(get_request_data(trace_id,command_id,"",self.x_erp_instance_id),logs)
+
         try:
             response = session.post(url, headers=headers, data=payload, timeout=45)
             response.raise_for_status()
             response_data = response.json()
-            logger.info(f"post command response: {response_data}")
-            publish_event(get_request_data(trace_id,command_id,"",self.x_erp_instance_id),logs)
             return response_data
         except requests.exceptions.HTTPError as http_err:
             raise Exception(f"HTTP error occurred: {http_err}")
         except requests.exceptions.ConnectionError as conn_err:
             raise Exception(f"Connection error occurred: {conn_err}")
         except requests.exceptions.Timeout as timeout_err:
             raise Exception(f"Timeout error occurred: {timeout_err}")
```

### Comparing `custom_erp_connector-0.24/erp_connector/config/config_loader.py` & `custom_erp_connector-0.3/erp_connector/config/config_loader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,10 @@
 import json
-import os
 
 from erp_connector.utils.singleton import SingletonMeta
-from erp_connector.utils.custlogging import LoggerProvider
-from erp_connector.service.event_service import publish_event, get_request_data
-from erp_connector.utils.custlogging import CustomLogHandler
-
-logger = LoggerProvider().get_logger(os.path.basename(__file__))
-
-logs = []
-log_handler = CustomLogHandler(logs)
-logger.addHandler(log_handler)
 
 
 class CustomErpConnectorConfig(metaclass=SingletonMeta):
     def __init__(self, config_dict):
         self._config = config_dict
 
     @property
@@ -36,17 +26,14 @@
     @property
     def erpInstanceId(self):
         return self._config.get("erpInstanceId")
 
 
 class ConfigLoader(metaclass=SingletonMeta):
 
-    def __init__(self, config_path,trace_id):
+    def __init__(self, config_path):
         self.config_path = config_path
-        self.trace_id = trace_id
 
     def load(self):
         with open(self.config_path, 'r') as file:
             config_dict = json.load(file)
-            logger.info("config loaded")
-            publish_event(get_request_data(self.trace_id, "", "", ""),logs)
         return CustomErpConnectorConfig(config_dict)
```

### Comparing `custom_erp_connector-0.24/erp_connector/db/db_connector.py` & `custom_erp_connector-0.3/erp_connector/db/db_connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,17 @@
         pass
 
     @abstractmethod
     def fetch_data(self, query):
         pass
 
     @abstractmethod
-    def generate_query(self, json_data):
+    def insert_data(self, insert_query):
         pass
 
     @abstractmethod
-    def get_total_table_count(self):
+    def generate_query(self, json_data):
         pass
 
     @abstractmethod
     def close_connection(self):
         pass
```

### Comparing `custom_erp_connector-0.24/erp_connector/exceptions/__init__.py` & `custom_erp_connector-0.3/erp_connector/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `custom_erp_connector-0.24/erp_connector/scheduler.py` & `custom_erp_connector-0.3/erp_connector/scheduler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,24 @@
 import argparse
-import uuid
-
 from apscheduler.schedulers.background import BackgroundScheduler
-from erp_connector.service.connector_service import process_connector, verifying_config
+from erp_connector.service.connector_service import process_connector
 import time
-from erp_connector.service.event_service import create_table
+from erp_connector.service.sqlite_service import create_table
 
 
 def run_scheduler(config_path):
-    trace_id = str(uuid.uuid4())
     create_table()
-    config_response = verifying_config(config_path)
-    erp_instance_id = config_response["erpInstanceId"]
-    db_connector = config_response["dbConnector"]
-    one_integration_client = config_response["client"]
     scheduler = BackgroundScheduler(daemon=True)
-    process_connector(db_connector,one_integration_client,erp_instance_id)
-    scheduler.add_job(process_connector, 'interval', minutes=1, max_instances=1, args=(db_connector,one_integration_client,erp_instance_id))
+    scheduler.add_job(process_connector, 'interval', minutes=1, max_instances=1,args=(config_path,))
     scheduler.start()
 
     try:
         while True:
             time.sleep(1)
     except (KeyboardInterrupt, SystemExit):
-        db_connector.close_connection(trace_id)
         scheduler.shutdown()
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description='ERP Connector Scheduler')
     parser.add_argument('config_path', type=str, help='Path to configuration file')
     args = parser.parse_args()
```

### Comparing `custom_erp_connector-0.24/erp_connector/utils/InProcessBatch.py` & `custom_erp_connector-0.3/erp_connector/utils/InProcessBatch.py`

 * *Files identical despite different names*

### Comparing `custom_erp_connector-0.24/erp_connector/utils/custlogging.py` & `custom_erp_connector-0.3/erp_connector/utils/custlogging.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,27 +58,14 @@
             'WARNING': logging.WARNING,
             'WARN': logging.WARNING,
             'DEBUG': logging.DEBUG
         }
         return log_levels.get(level, logging.INFO)
 
 
-class CustomLogHandler(logging.Handler):
-    def __init__(self, logs):
-        super().__init__()
-        self.logs = logs
-
-    def emit(self, record):
-        log_entry = {
-            "level": record.levelname,
-            "message": self.format(record)
-        }
-        self.logs.append(log_entry)
-
-
 class LogFilterDummy(logging.Filter):
 
     def __init__(self):
         super().__init__()
 
     def filter(self, record) -> bool:
         record.elt_client = None
```

### Comparing `custom_erp_connector-0.24/erp_connector/utils/mysql_query_utils.py` & `custom_erp_connector-0.3/erp_connector/utils/mysql_query_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,60 @@
-from sqlglot import parse, condition
+from sqlglot import parse
 
 
 def _generate_join_clause(joins):
     clauses = []
-    if len(joins) > 0:
-        for join in joins:
-            join_table = join["name"]
-            join_alias = join["alias"]
-            join_conditions = " AND ".join([
-                f"{cond['left']['alias']}.{cond['left']['name']} = {cond['right']['alias']}.{cond['right']['name']}"
-                for cond in join["on"]
-            ])
-            clause = f"JOIN {join_table} AS {join_alias} ON {join_conditions}"
-            clauses.append(clause)
-    else:
-        return ""
+    for join in joins:
+        join_table = join["name"]
+        join_alias = join["alias"]
+        join_conditions = " AND ".join([
+            f"{cond['left']['alias']}.{cond['left']['name']} = {cond['right']['alias']}.{cond['right']['name']}"
+            for cond in join["on"]
+        ])
+        clause = f"JOIN {join_table} AS {join_alias} ON {join_conditions}"
+        clauses.append(clause)
     return " ".join(clauses)
 
 
 def _generate_expr(expr):
-    if "expr" in expr:
-        data_expr = expr["expr"]
-        if "column" in data_expr:
-            column = f"{data_expr['column']['alias']}.{data_expr['column']['name']}"
-            operator = data_expr["operator"]
-            value = data_expr["value"][0]
-            return f"{column} {operator} '{value}'"
-        elif "booleanOperator" in data_expr:
-            return data_expr["booleanOperator"]
+    if "column" in expr:
+        column = f"{expr['column']['alias']}.{expr['column']['name']}"
+        operator = expr["operator"]
+        value = expr["value"][0]  # Assuming only one value in the list
+        return f"{column} {operator} '{value}'"
     elif "booleanOperator" in expr:
         return expr["booleanOperator"]
 
 
 def _generate_order_by_clause(order_by):
     clauses = [f"{item['column']['alias']}.{item['column']['name']} {item.get('order', 'ASC')}" for item in order_by]
     return "ORDER BY " + ", ".join(clauses) if clauses else ""
 
 
 def _generate_where_clause(conditions):
-    where_conditions = []
+    clauses = []
     for cond_metadata in conditions:
         if "listOfExpr" in cond_metadata:
             sublist = [_generate_expr(expr) for expr in cond_metadata["listOfExpr"]]
-            where_conditions.append(" ".join(sublist))
+            clauses.append("(" + " ".join(sublist) + ")")
         elif "expr" in cond_metadata and "column" in cond_metadata["expr"]:
-            # expr = cond_metadata["expr"]
-            where_conditions.append(_generate_expr(cond_metadata))
-    where_condition = " AND ".join(where_conditions)
-    return f"WHERE {where_condition}" if where_condition else ""
+            expr = cond_metadata["expr"]
+            clauses.append(_generate_expr(expr))
+    return "WHERE " + " AND ".join(clauses) if clauses else ""
 
 
 def generate_data_query(json_data):
     queries = []
     for entity in json_data:
         select_clause = ", ".join([f"{item['name']}" for item in entity["select"]])
         from_table = entity["fromTable"]["name"]
-        table_alias = entity["fromTable"]["alias"]
         join_clause = _generate_join_clause(entity.get("join", []))
         where_clause = _generate_where_clause(entity.get("where", []))
         order_by_clause = _generate_order_by_clause(entity.get("order_by", []))
 
-        sql_query = f"SELECT {select_clause} FROM {from_table} {table_alias} {join_clause} {where_clause} {order_by_clause}"
+        # Construct the SQL query string
+        sql_query = f"SELECT {select_clause} FROM {from_table} {join_clause} {where_clause} {order_by_clause}"
 
-        # parsed_query = parse(sql_query)
-        queries.append({"tableName": from_table, "query": str(sql_query)})
+        # Parse the SQL query string to validate and normalize it
+        parsed_query = parse(sql_query)
+        queries.append({"tableName": from_table, "query": str(parsed_query)})
     return queries
```

### Comparing `custom_erp_connector-0.24/erp_connector/utils/retryable_session.py` & `custom_erp_connector-0.3/erp_connector/utils/retryable_session.py`

 * *Files identical despite different names*

### Comparing `custom_erp_connector-0.24/setup.py` & `custom_erp_connector-0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
 package_name = "custom_erp_connector"
 
-package_version = "0.24"
+package_version = "0.3"
 description = """custom-erp-connector"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=long_description,
@@ -29,15 +29,15 @@
     install_requires=[
         "mysql-connector-python==8.3.0",
         "psycopg2==2.9.9",
         "requests==2.31.0",
         "APScheduler==3.10.4",
         "pyodbc==5.1.0",
         "sqlparse==0.4.3",
+        "pandas==1.5.1",
         "SQLAlchemy==1.4.46",
         "python-dateutil==2.8.2",
         "h2==4.1.0",
         "simplejson==3.18.3",
-        "sqlglot==18.7.0",
-        "oracledb==2.1.2"
+        "sqlglot==18.7.0"
     ]
 )
```


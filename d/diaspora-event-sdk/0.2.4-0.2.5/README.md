# Comparing `tmp/diaspora-event-sdk-0.2.4.tar.gz` & `tmp/diaspora-event-sdk-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diaspora-event-sdk-0.2.4.tar", last modified: Sat Apr 13 12:51:36 2024, max compression
+gzip compressed data, was "diaspora-event-sdk-0.2.5.tar", last modified: Fri May  3 15:59:45 2024, max compression
```

## Comparing `diaspora-event-sdk-0.2.4.tar` & `diaspora-event-sdk-0.2.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-13 12:51:36.240509 diaspora-event-sdk-0.2.4/
--rw-r--r--   0 haochen    (501) staff       (20)    11357 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.4/LICENSE
--rw-r--r--   0 haochen    (501) staff       (20)       58 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.4/MANIFEST.in
--rw-r--r--   0 haochen    (501) staff       (20)     2092 2024-04-13 12:51:36.240364 diaspora-event-sdk-0.2.4/PKG-INFO
--rw-r--r--   0 haochen    (501) staff       (20)     1722 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.4/README.md
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-13 12:51:36.236358 diaspora-event-sdk-0.2.4/diaspora_event_sdk/
--rw-r--r--   0 haochen    (501) staff       (20)      457 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk/__init__.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-13 12:51:36.237994 diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)      204 2024-04-07 17:27:11.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/_environments.py
--rw-r--r--   0 haochen    (501) staff       (20)     8016 2024-04-13 12:31:39.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/client.py
--rw-r--r--   0 haochen    (501) staff       (20)      884 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/decorators.py
--rw-r--r--   0 haochen    (501) staff       (20)     4361 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/kafka_client.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-13 12:51:36.239488 diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/login_manager/
--rw-r--r--   0 haochen    (501) staff       (20)      239 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/login_manager/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)     1835 2024-04-08 03:36:21.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/login_manager/client_login.py
--rw-r--r--   0 haochen    (501) staff       (20)     1047 2024-04-08 03:39:08.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/login_manager/decorators.py
--rw-r--r--   0 haochen    (501) staff       (20)      430 2024-04-08 03:40:29.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/login_manager/globus_auth.py
--rw-r--r--   0 haochen    (501) staff       (20)      977 2024-04-08 03:45:19.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/login_manager/login_flow.py
--rw-r--r--   0 haochen    (501) staff       (20)     7040 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/login_manager/manager.py
--rw-r--r--   0 haochen    (501) staff       (20)      710 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/login_manager/protocol.py
--rw-r--r--   0 haochen    (501) staff       (20)     2094 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/login_manager/tokenstore.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-13 12:51:36.239795 diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/utils/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/utils/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)      470 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/utils/uuid_like.py
--rw-r--r--   0 haochen    (501) staff       (20)     4222 2024-04-13 12:42:58.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/web_client.py
--rw-r--r--   0 haochen    (501) staff       (20)       22 2024-04-13 12:50:30.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk/version.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-13 12:51:36.236906 diaspora-event-sdk-0.2.4/diaspora_event_sdk.egg-info/
--rw-r--r--   0 haochen    (501) staff       (20)     2092 2024-04-13 12:51:36.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk.egg-info/PKG-INFO
--rw-r--r--   0 haochen    (501) staff       (20)     1068 2024-04-13 12:51:36.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 haochen    (501) staff       (20)        1 2024-04-13 12:51:36.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 haochen    (501) staff       (20)      141 2024-04-13 12:51:36.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk.egg-info/requires.txt
--rw-r--r--   0 haochen    (501) staff       (20)       25 2024-04-13 12:51:36.000000 diaspora-event-sdk-0.2.4/diaspora_event_sdk.egg-info/top_level.txt
--rw-r--r--   0 haochen    (501) staff       (20)       38 2024-04-13 12:51:36.240557 diaspora-event-sdk-0.2.4/setup.cfg
--rw-r--r--   0 haochen    (501) staff       (20)     1389 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.4/setup.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-13 12:51:36.239925 diaspora-event-sdk-0.2.4/tests/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.4/tests/__init__.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-13 12:51:36.240019 diaspora-event-sdk-0.2.4/tests/unit/
--rw-r--r--   0 haochen    (501) staff       (20)     3019 2024-04-08 02:07:35.000000 diaspora-event-sdk-0.2.4/tests/unit/test_client.py
--rw-r--r--   0 haochen    (501) staff       (20)      241 2024-04-08 03:50:13.000000 diaspora-event-sdk-0.2.4/tox.ini
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-03 15:59:45.162057 diaspora-event-sdk-0.2.5/
+-rw-r--r--   0 haochen    (501) staff       (20)    11357 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/LICENSE
+-rw-r--r--   0 haochen    (501) staff       (20)       58 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/MANIFEST.in
+-rw-r--r--   0 haochen    (501) staff       (20)     2105 2024-05-03 15:59:45.161919 diaspora-event-sdk-0.2.5/PKG-INFO
+-rw-r--r--   0 haochen    (501) staff       (20)     1735 2024-05-03 15:59:19.000000 diaspora-event-sdk-0.2.5/README.md
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-03 15:59:45.159171 diaspora-event-sdk-0.2.5/diaspora_event_sdk/
+-rw-r--r--   0 haochen    (501) staff       (20)      457 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/__init__.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-03 15:59:45.160408 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)      204 2024-04-07 17:27:11.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/_environments.py
+-rw-r--r--   0 haochen    (501) staff       (20)     8541 2024-05-03 15:08:27.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/client.py
+-rw-r--r--   0 haochen    (501) staff       (20)      884 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/decorators.py
+-rw-r--r--   0 haochen    (501) staff       (20)     4361 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/kafka_client.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-03 15:59:45.161369 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/
+-rw-r--r--   0 haochen    (501) staff       (20)      239 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)     1835 2024-04-08 03:36:21.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/client_login.py
+-rw-r--r--   0 haochen    (501) staff       (20)     1047 2024-04-08 03:39:08.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/decorators.py
+-rw-r--r--   0 haochen    (501) staff       (20)      430 2024-04-08 03:40:29.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/globus_auth.py
+-rw-r--r--   0 haochen    (501) staff       (20)      977 2024-04-08 03:45:19.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/login_flow.py
+-rw-r--r--   0 haochen    (501) staff       (20)     7040 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/manager.py
+-rw-r--r--   0 haochen    (501) staff       (20)      710 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/protocol.py
+-rw-r--r--   0 haochen    (501) staff       (20)     2094 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/tokenstore.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-03 15:59:45.161565 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/utils/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/utils/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)      470 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/utils/uuid_like.py
+-rw-r--r--   0 haochen    (501) staff       (20)     4770 2024-05-03 14:59:36.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/web_client.py
+-rw-r--r--   0 haochen    (501) staff       (20)       22 2024-05-03 14:44:05.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/version.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-03 15:59:45.159692 diaspora-event-sdk-0.2.5/diaspora_event_sdk.egg-info/
+-rw-r--r--   0 haochen    (501) staff       (20)     2105 2024-05-03 15:59:45.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 haochen    (501) staff       (20)     1068 2024-05-03 15:59:45.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 haochen    (501) staff       (20)        1 2024-05-03 15:59:45.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 haochen    (501) staff       (20)      141 2024-05-03 15:59:45.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk.egg-info/requires.txt
+-rw-r--r--   0 haochen    (501) staff       (20)       25 2024-05-03 15:59:45.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk.egg-info/top_level.txt
+-rw-r--r--   0 haochen    (501) staff       (20)       38 2024-05-03 15:59:45.162103 diaspora-event-sdk-0.2.5/setup.cfg
+-rw-r--r--   0 haochen    (501) staff       (20)     1389 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/setup.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-03 15:59:45.161672 diaspora-event-sdk-0.2.5/tests/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/tests/__init__.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-03 15:59:45.161757 diaspora-event-sdk-0.2.5/tests/unit/
+-rw-r--r--   0 haochen    (501) staff       (20)     3019 2024-04-08 02:07:35.000000 diaspora-event-sdk-0.2.5/tests/unit/test_client.py
+-rw-r--r--   0 haochen    (501) staff       (20)      241 2024-04-08 03:50:13.000000 diaspora-event-sdk-0.2.5/tox.ini
```

### Comparing `diaspora-event-sdk-0.2.4/LICENSE` & `diaspora-event-sdk-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.4/PKG-INFO` & `diaspora-event-sdk-0.2.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,8 @@
-Metadata-Version: 2.1
-Name: diaspora-event-sdk
-Version: 0.2.4
-Summary: SDK of Diaspora Event Fabric: Resilience-enabling services for science from HPC to edge
-Home-page: https://github.com/globus-labs/diaspora-event-sdk
-License: LICENSE
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Provides-Extra: kafka-python
-Provides-Extra: test
-License-File: LICENSE
-
-# Diaspora: Resilience-enabling services for science from HPC to edge
+# Diaspora: Hybrid Event-Driven Architecture for Distributed Scientific Computing
 
 ## Event Fabric SDK Installation Guide
 ### Recommended Method: Use with `kafka-python`
 For easy integration with Diaspora Event Fabric, use the `KafkaProducer` and `KafkaConsumer` classes from our SDK. This requires the `kafka-python` library.
 
 To install the Event Fabric SDK and `kafka-python,` with the following command:
 ```bash
@@ -35,8 +23,7 @@
 **Getting Started**: Visit our [QuickStart Guide](docs/quickstart.md) for details on using the SDK with the kafka-python library and instructions for other Kafka clients.
 
 **Troubleshooting and Credential Management**: Consult our [TrobleShooting Guide](docs/troubleshooting.md) for solving common issues and tips on managing keys effectively.
 
 **Advanced Consumers with Faust**: Explore the [Faust Streaming Guide](docs/faust_weather_app.md) for advanced event streaming with Faust.
 
 **Advanced Consumer Functions**: See our [Colab example](https://colab.research.google.com/drive/1tPKfxU2qPsLvNTreF6nKINU62k7pQWxa?usp=sharing) for demonstration.
-
```

### Comparing `diaspora-event-sdk-0.2.4/README.md` & `diaspora-event-sdk-0.2.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,20 @@
-# Diaspora: Resilience-enabling services for science from HPC to edge
+Metadata-Version: 2.1
+Name: diaspora-event-sdk
+Version: 0.2.5
+Summary: SDK of Diaspora Event Fabric: Resilience-enabling services for science from HPC to edge
+Home-page: https://github.com/globus-labs/diaspora-event-sdk
+License: LICENSE
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+Provides-Extra: kafka-python
+Provides-Extra: test
+License-File: LICENSE
+
+# Diaspora: Hybrid Event-Driven Architecture for Distributed Scientific Computing
 
 ## Event Fabric SDK Installation Guide
 ### Recommended Method: Use with `kafka-python`
 For easy integration with Diaspora Event Fabric, use the `KafkaProducer` and `KafkaConsumer` classes from our SDK. This requires the `kafka-python` library.
 
 To install the Event Fabric SDK and `kafka-python,` with the following command:
 ```bash
@@ -22,8 +34,10 @@
 
 **Getting Started**: Visit our [QuickStart Guide](docs/quickstart.md) for details on using the SDK with the kafka-python library and instructions for other Kafka clients.
 
 **Troubleshooting and Credential Management**: Consult our [TrobleShooting Guide](docs/troubleshooting.md) for solving common issues and tips on managing keys effectively.
 
 **Advanced Consumers with Faust**: Explore the [Faust Streaming Guide](docs/faust_weather_app.md) for advanced event streaming with Faust.
 
-**Advanced Consumer Functions**: See our [Colab example](https://colab.research.google.com/drive/1tPKfxU2qPsLvNTreF6nKINU62k7pQWxa?usp=sharing) for demonstration.
+**Advanced Consumer Functions**: See our [Colab example](https://colab.research.google.com/drive/1tPKfxU2qPsLvNTreF6nKINU62k7pQWxa?usp=sharing) for demonstration.
+
+
```

### Comparing `diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/client.py` & `diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,28 +150,42 @@
     def update_topic_partitions(self, topic, new_partitions):
         """
         Increases the number of partitions for a given topic to the specified new partition count.
         """
         return self.web_client.update_topic_partitions(self.subject_openid, topic, new_partitions)
 
     @requires_login
+    def reset_topic(self, topic):
+        """
+        Deletes and recreates the topic, removing all messages and restoring the topic to the default configurations while user access is not affected.
+        """
+        return self.web_client.reset_topic(self.subject_openid, topic)
+
+    @requires_login
     def grant_user_access(self, topic, user):
         """
         Authorizes another user to access a registered topic under the invoker's account.
         """
         return self.web_client.grant_user_access(self.subject_openid, topic, user, "grant")
 
     @requires_login
     def revoke_user_access(self, topic, user):
         """
         Removes access permissions for another user from a registered topic under the invoker's account.
         """
         return self.web_client.grant_user_access(self.subject_openid, topic, user, "revoke")
 
     @requires_login
+    def list_topic_users(self, topic):
+        """
+        Returns a list of users that have access to the topic.
+        """
+        return self.web_client.list_topic_users(self.subject_openid, topic)
+
+    @requires_login
     def list_triggers(self):
         """
         Retrieves a list of triggers associated created under the user's account, showing each trigger's configurations and UUID.
         """
         return self.web_client.list_triggers(self.subject_openid)
 
     @requires_login
```

### Comparing `diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/decorators.py` & `diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/decorators.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/kafka_client.py` & `diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/kafka_client.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/login_manager/client_login.py` & `diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/client_login.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/login_manager/decorators.py` & `diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/login_manager/login_flow.py` & `diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/login_flow.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/login_manager/manager.py` & `diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/manager.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/login_manager/protocol.py` & `diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/protocol.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/login_manager/tokenstore.py` & `diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/tokenstore.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.4/diaspora_event_sdk/sdk/web_client.py` & `diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/web_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,23 +62,41 @@
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.post(
             f"/api/v2/topic/{topic}/partitions",
             headers={"Subject": str(subject), "Topic": topic,
                      "NewPartitions": str(new_partitions)}
         )
 
+    def reset_topic(
+        self, subject: UUID_LIKE_T, topic: str
+    ) -> globus_sdk.GlobusHTTPResponse:
+        return self.post(
+            f"/api/v2/topic/{topic}/reset",
+            headers={"Subject": str(subject),
+                     "Topic": topic}
+        )
+
     def grant_user_access(
         self, subject: UUID_LIKE_T, topic: str, user: UUID_LIKE_T, action: str
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.post(
             f"/api/v2/topic/{topic}/user",
             headers={"Subject": str(subject), "Action": action,
                      "Topic": topic, "User": str(user)}
         )
 
+    def list_topic_users(
+        self, subject: UUID_LIKE_T, topic: str
+    ) -> globus_sdk.GlobusHTTPResponse:
+        return self.get(
+            f"/api/v2/topic/{topic}/users",
+            headers={"Subject": str(subject),
+                     "Topic": topic}
+        )
+
     def list_triggers(self, subject: UUID_LIKE_T) -> globus_sdk.GlobusHTTPResponse:
         return self.get("/api/v2/triggers", headers={"Subject": str(subject)})
 
     def create_trigger(
         self, subject: UUID_LIKE_T, topic: str, function: str, action: str,
         function_configs: dict, trigger_configs: dict
     ) -> globus_sdk.GlobusHTTPResponse:
```

### Comparing `diaspora-event-sdk-0.2.4/diaspora_event_sdk.egg-info/PKG-INFO` & `diaspora-event-sdk-0.2.5/diaspora_event_sdk.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: diaspora-event-sdk
-Version: 0.2.4
+Version: 0.2.5
 Summary: SDK of Diaspora Event Fabric: Resilience-enabling services for science from HPC to edge
 Home-page: https://github.com/globus-labs/diaspora-event-sdk
 License: LICENSE
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: kafka-python
 Provides-Extra: test
 License-File: LICENSE
 
-# Diaspora: Resilience-enabling services for science from HPC to edge
+# Diaspora: Hybrid Event-Driven Architecture for Distributed Scientific Computing
 
 ## Event Fabric SDK Installation Guide
 ### Recommended Method: Use with `kafka-python`
 For easy integration with Diaspora Event Fabric, use the `KafkaProducer` and `KafkaConsumer` classes from our SDK. This requires the `kafka-python` library.
 
 To install the Event Fabric SDK and `kafka-python,` with the following command:
 ```bash
@@ -36,7 +36,8 @@
 
 **Troubleshooting and Credential Management**: Consult our [TrobleShooting Guide](docs/troubleshooting.md) for solving common issues and tips on managing keys effectively.
 
 **Advanced Consumers with Faust**: Explore the [Faust Streaming Guide](docs/faust_weather_app.md) for advanced event streaming with Faust.
 
 **Advanced Consumer Functions**: See our [Colab example](https://colab.research.google.com/drive/1tPKfxU2qPsLvNTreF6nKINU62k7pQWxa?usp=sharing) for demonstration.
 
+
```

### Comparing `diaspora-event-sdk-0.2.4/diaspora_event_sdk.egg-info/SOURCES.txt` & `diaspora-event-sdk-0.2.5/diaspora_event_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.4/setup.py` & `diaspora-event-sdk-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.4/tests/unit/test_client.py` & `diaspora-event-sdk-0.2.5/tests/unit/test_client.py`

 * *Files identical despite different names*


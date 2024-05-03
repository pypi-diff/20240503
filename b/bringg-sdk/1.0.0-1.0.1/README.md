# Comparing `tmp/bringg_sdk-1.0.0.tar.gz` & `tmp/bringg_sdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bringg_sdk-1.0.0.tar", last modified: Sat Apr 27 11:30:09 2024, max compression
+gzip compressed data, was "bringg_sdk-1.0.1.tar", last modified: Fri May  3 04:24:16 2024, max compression
```

## Comparing `bringg_sdk-1.0.0.tar` & `bringg_sdk-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 elkhayyat   (501) staff       (20)        0 2024-04-27 11:30:09.545369 bringg_sdk-1.0.0/
--rw-r--r--   0 elkhayyat   (501) staff       (20)       54 2024-04-27 11:30:09.544967 bringg_sdk-1.0.0/PKG-INFO
--rw-r--r--   0 elkhayyat   (501) staff       (20)     2942 2024-04-26 12:28:08.000000 bringg_sdk-1.0.0/README.md
-drwxr-xr-x   0 elkhayyat   (501) staff       (20)        0 2024-04-27 11:30:09.541995 bringg_sdk-1.0.0/bringg_sdk/
--rw-r--r--   0 elkhayyat   (501) staff       (20)        0 2024-04-27 11:03:16.000000 bringg_sdk-1.0.0/bringg_sdk/__init__.py
--rw-r--r--   0 elkhayyat   (501) staff       (20)    10490 2024-04-27 10:01:24.000000 bringg_sdk-1.0.0/bringg_sdk/client.py
--rw-r--r--   0 elkhayyat   (501) staff       (20)      391 2024-04-26 12:16:39.000000 bringg_sdk-1.0.0/bringg_sdk/exceptions.py
--rw-r--r--   0 elkhayyat   (501) staff       (20)    13149 2024-04-26 07:16:39.000000 bringg_sdk-1.0.0/bringg_sdk/models.py
--rw-r--r--   0 elkhayyat   (501) staff       (20)     3286 2024-04-26 11:59:17.000000 bringg_sdk-1.0.0/bringg_sdk/request_factory.py
--rw-r--r--   0 elkhayyat   (501) staff       (20)     5358 2024-04-26 12:18:02.000000 bringg_sdk-1.0.0/bringg_sdk/responses.py
-drwxr-xr-x   0 elkhayyat   (501) staff       (20)        0 2024-04-27 11:30:09.544403 bringg_sdk-1.0.0/bringg_sdk.egg-info/
--rw-r--r--   0 elkhayyat   (501) staff       (20)       54 2024-04-27 11:30:09.000000 bringg_sdk-1.0.0/bringg_sdk.egg-info/PKG-INFO
--rw-r--r--   0 elkhayyat   (501) staff       (20)      331 2024-04-27 11:30:09.000000 bringg_sdk-1.0.0/bringg_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 elkhayyat   (501) staff       (20)        1 2024-04-27 11:30:09.000000 bringg_sdk-1.0.0/bringg_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 elkhayyat   (501) staff       (20)        9 2024-04-27 11:30:09.000000 bringg_sdk-1.0.0/bringg_sdk.egg-info/requires.txt
--rw-r--r--   0 elkhayyat   (501) staff       (20)       11 2024-04-27 11:30:09.000000 bringg_sdk-1.0.0/bringg_sdk.egg-info/top_level.txt
--rw-r--r--   0 elkhayyat   (501) staff       (20)       38 2024-04-27 11:30:09.545462 bringg_sdk-1.0.0/setup.cfg
--rw-r--r--   0 elkhayyat   (501) staff       (20)      176 2024-04-27 11:05:00.000000 bringg_sdk-1.0.0/setup.py
+drwxr-xr-x   0 elkhayyat   (501) staff       (20)        0 2024-05-03 04:24:16.882361 bringg_sdk-1.0.1/
+-rw-r--r--   0 elkhayyat   (501) staff       (20)     3042 2024-05-03 04:24:16.882207 bringg_sdk-1.0.1/PKG-INFO
+-rw-r--r--   0 elkhayyat   (501) staff       (20)     2947 2024-04-27 11:56:36.000000 bringg_sdk-1.0.1/README.md
+drwxr-xr-x   0 elkhayyat   (501) staff       (20)        0 2024-05-03 04:24:16.881254 bringg_sdk-1.0.1/bringg_sdk/
+-rw-r--r--   0 elkhayyat   (501) staff       (20)        0 2024-04-27 11:03:16.000000 bringg_sdk-1.0.1/bringg_sdk/__init__.py
+-rw-r--r--   0 elkhayyat   (501) staff       (20)    11290 2024-05-03 03:54:39.000000 bringg_sdk-1.0.1/bringg_sdk/client.py
+-rw-r--r--   0 elkhayyat   (501) staff       (20)      391 2024-04-26 12:16:39.000000 bringg_sdk-1.0.1/bringg_sdk/exceptions.py
+-rw-r--r--   0 elkhayyat   (501) staff       (20)    13149 2024-04-26 07:16:39.000000 bringg_sdk-1.0.1/bringg_sdk/models.py
+-rw-r--r--   0 elkhayyat   (501) staff       (20)     3286 2024-04-26 11:59:17.000000 bringg_sdk-1.0.1/bringg_sdk/request_factory.py
+-rw-r--r--   0 elkhayyat   (501) staff       (20)     5358 2024-04-26 12:18:02.000000 bringg_sdk-1.0.1/bringg_sdk/responses.py
+drwxr-xr-x   0 elkhayyat   (501) staff       (20)        0 2024-05-03 04:24:16.882018 bringg_sdk-1.0.1/bringg_sdk.egg-info/
+-rw-r--r--   0 elkhayyat   (501) staff       (20)     3042 2024-05-03 04:24:16.000000 bringg_sdk-1.0.1/bringg_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 elkhayyat   (501) staff       (20)      331 2024-05-03 04:24:16.000000 bringg_sdk-1.0.1/bringg_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 elkhayyat   (501) staff       (20)        1 2024-05-03 04:24:16.000000 bringg_sdk-1.0.1/bringg_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 elkhayyat   (501) staff       (20)        9 2024-05-03 04:24:16.000000 bringg_sdk-1.0.1/bringg_sdk.egg-info/requires.txt
+-rw-r--r--   0 elkhayyat   (501) staff       (20)       11 2024-05-03 04:24:16.000000 bringg_sdk-1.0.1/bringg_sdk.egg-info/top_level.txt
+-rw-r--r--   0 elkhayyat   (501) staff       (20)       38 2024-05-03 04:24:16.882409 bringg_sdk-1.0.1/setup.cfg
+-rw-r--r--   0 elkhayyat   (501) staff       (20)      453 2024-05-03 04:20:59.000000 bringg_sdk-1.0.1/setup.py
```

### Comparing `bringg_sdk-1.0.0/README.md` & `bringg_sdk-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 The Bringg Python SDK provides a simple way to integrate the Bringg platform with your Python application.
 
 ## Installation
 
 To install the Bringg Python SDK, simply run the following command:
 
 ```bash
-pip install bringg-sdk
+pip install bringg_sdk
 ```
 
 ## Getting Started
 
-To get started, you will need to create an account on the [Bringg platform](https://app.bringg.com/).
+To get started, you will need to have an account on the [Bringg fleet platform](https://fleet.bringg.com).
 Once you have created an account, you will need to generate an API key.
 
 ## API Reference
 
 The Bringg Python SDK provides a simple interface to interact with the Bringg API.
 The SDK provides the following classes:
```

### Comparing `bringg_sdk-1.0.0/bringg_sdk/client.py` & `bringg_sdk-1.0.1/bringg_sdk/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,15 +82,24 @@
             data['green_delivery'] = green_delivery
         request = AssignDriverRequest(url, data, self.get_token())
         response = request.post()
         return response
 
     def start_order(self, task_id: int, lat: float | None = None, lng: float | None = None,
                     reported_time_in_timestamp: int = None, delivery_cost_in_cents: int = None, green_delivery=True):
-
+        """
+        This endpoint is used to start an order. This is the first step in the delivery process.
+        :param task_id:
+        :param lat:
+        :param lng:
+        :param reported_time_in_timestamp:
+        :param delivery_cost_in_cents:
+        :param green_delivery:
+        :return:
+        """
         url = self.get_url('start_order')
 
         data = {
             "task_id": task_id,
             "green_delivery": green_delivery
         }
         if lat and lng:
@@ -103,14 +112,23 @@
 
         request = AssignDriverRequest(url, data, self.get_token())
         response = request.post()
         return response
 
     def update_driver_location(self, user_external_id: str, lat: float, lng: float,
                                reported_time_in_timestamp: int = None, started_tasks: list = None):
+        """
+        This endpoint is used to update the driver's location.
+        :param user_external_id:
+        :param lat:
+        :param lng:
+        :param reported_time_in_timestamp:
+        :param started_tasks:
+        :return:
+        """
         url = self.get_url('update_driver_location')
         data = {
             "external_id": user_external_id,
             "lat": lat,
             "lng": lng
         }
         if reported_time_in_timestamp:
@@ -120,14 +138,15 @@
         request = bringg_requests.UpdateDriverLocationRequest(url, data, self.get_token())
         response = request.post()
         return response
 
     def check_in(self, task_id: int, lat: float, lng: float, reported_time_in_timestamp: int = None,
                  pickup_dropoff_option: str = None):
         """
+        This endpoint is used to check in the driver to the pickup or drop-off location.
         :param task_id: bringg order id
         :param lat: driver latitude
         :param lng: driver longitude
         :param reported_time_in_timestamp:
         :param pickup_dropoff_option: choices: ['pickup', 'dropoff']
         :return:
         """
@@ -182,15 +201,15 @@
         """
 
         raise NotImplementedError()
 
     def complete_order(self, task_id: int, lat: float = None, lng: float = None, reported_time_in_timestamp: int = None,
                        delivery_cost_in_cents: int = None):
         """
-
+        This endpoint is used to complete an order. This is the last step in the delivery process.
         :param task_id:
         :param lat:
         :param lng:
         :param reported_time_in_timestamp:
         :param delivery_cost_in_cents:
         :return:
         """
@@ -208,15 +227,15 @@
         request = bringg_requests.CompleteOrderRequest(url, data, self.get_token())
         response = request.post()
         return response
 
     def cancel_order(self, task_id: int, reason_id: int = 0, reason: str = None, lng: float = None,
                      lat: float = None, reported_time_in_timestamp: int = None):
         """
-
+        This endpoint is used to cancel an order.
         :param task_id: Bringg's unique ID for this order. Use either this field or task_external_id to identify the
                         relevant order.
         :param reason_id: MANDATORY: Bringg's reason ID for this order
                                      You will usually get this value from discussions with the relevant merchant
                                      As a default, use 0
         :param reason: The reason you are cancelling the order/delivery
         :param lng: The latitude of where the driver was when the order was started
```

### Comparing `bringg_sdk-1.0.0/bringg_sdk/models.py` & `bringg_sdk-1.0.1/bringg_sdk/models.py`

 * *Files identical despite different names*

### Comparing `bringg_sdk-1.0.0/bringg_sdk/request_factory.py` & `bringg_sdk-1.0.1/bringg_sdk/request_factory.py`

 * *Files identical despite different names*

### Comparing `bringg_sdk-1.0.0/bringg_sdk/responses.py` & `bringg_sdk-1.0.1/bringg_sdk/responses.py`

 * *Files identical despite different names*


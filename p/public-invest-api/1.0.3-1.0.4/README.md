# Comparing `tmp/public_invest_api-1.0.3.tar.gz` & `tmp/public_invest_api-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "public_invest_api-1.0.3.tar", last modified: Wed May  1 23:45:35 2024, max compression
+gzip compressed data, was "public_invest_api-1.0.4.tar", last modified: Fri May  3 21:23:22 2024, max compression
```

## Comparing `public_invest_api-1.0.3.tar` & `public_invest_api-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:45:35.374617 public_invest_api-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-01 23:45:35.374617 public_invest_api-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-01 23:45:31.000000 public_invest_api-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:45:35.374617 public_invest_api-1.0.3/public_invest_api/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-01 23:45:31.000000 public_invest_api-1.0.3/public_invest_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-01 23:45:31.000000 public_invest_api-1.0.3/public_invest_api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-01 23:45:31.000000 public_invest_api-1.0.3/public_invest_api/public.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:45:35.374617 public_invest_api-1.0.3/public_invest_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-01 23:45:35.000000 public_invest_api-1.0.3/public_invest_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-01 23:45:35.000000 public_invest_api-1.0.3/public_invest_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 23:45:35.000000 public_invest_api-1.0.3/public_invest_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 23:45:35.000000 public_invest_api-1.0.3/public_invest_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 23:45:35.000000 public_invest_api-1.0.3/public_invest_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 23:45:35.374617 public_invest_api-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-01 23:45:31.000000 public_invest_api-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:23:22.620449 public_invest_api-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-03 21:23:22.620449 public_invest_api-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-03 21:23:18.000000 public_invest_api-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:23:22.620449 public_invest_api-1.0.4/public_invest_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-03 21:23:18.000000 public_invest_api-1.0.4/public_invest_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-03 21:23:18.000000 public_invest_api-1.0.4/public_invest_api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 21:23:18.000000 public_invest_api-1.0.4/public_invest_api/public.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:23:22.620449 public_invest_api-1.0.4/public_invest_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-03 21:23:22.000000 public_invest_api-1.0.4/public_invest_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-03 21:23:22.000000 public_invest_api-1.0.4/public_invest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 21:23:22.000000 public_invest_api-1.0.4/public_invest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 21:23:22.000000 public_invest_api-1.0.4/public_invest_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 21:23:22.000000 public_invest_api-1.0.4/public_invest_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 21:23:22.620449 public_invest_api-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-03 21:23:18.000000 public_invest_api-1.0.4/setup.py
```

### Comparing `public_invest_api-1.0.3/PKG-INFO` & `public_invest_api-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: public_invest_api
-Version: 1.0.3
+Version: 1.0.4
 Summary: Unofficial Public.com Invest API written in Python Requests
 Home-page: https://github.com/NelsonDane/public-invest-api
 Author: Nelson Dane
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: python-dotenv
```

### Comparing `public_invest_api-1.0.3/README.md` & `public_invest_api-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `public_invest_api-1.0.3/public_invest_api/endpoints.py` & `public_invest_api-1.0.4/public_invest_api/endpoints.py`

 * *Files 20% similar despite different names*

```diff
@@ -38,14 +38,20 @@
 
     def submit_put_order_url(self, account_uuid, order_id):
         return f"{self.ordergateway}/accounts/{account_uuid}/orders/{order_id}"
 
     def submit_get_order_url(self, account_uuid, order_id):
         return f"{self.prodapi}/hstier1service/account/{account_uuid}/order/{order_id}"
 
+    def get_pending_orders_url(self, account_uuid):
+        return f"{self.prodapi}/hstier2service/history?&&status=PENDING&type=ALL&accountUuids={account_uuid}"
+
+    def cancel_pending_order_url(self, account_uuid, order_id):
+        return f"{self.ordergateway}/accounts/{account_uuid}/orders/{order_id}"
+
     @staticmethod
     def build_headers(auth=None, prodApi=False):
         headers = {
             "authority": "public.com",
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.5",
             "content-type": "application/json",
```

### Comparing `public_invest_api-1.0.3/public_invest_api/public.py` & `public_invest_api-1.0.4/public_invest_api/public.py`

 * *Files 6% similar despite different names*

```diff
@@ -274,7 +274,39 @@
         check_response["success"] = False
         # Order doesn't always fill immediately, but one of these should work
         if check_response["rejectionDetails"] is None:
             check_response["success"] = True
         if check_response["status"] == "FILLED":
             check_response["success"] = True
         return check_response
+
+    @login_required
+    def get_pending_orders(self):
+        headers = self.endpoints.build_headers(self.access_token)
+        response = self.session.get(
+            self.endpoints.get_pending_orders_url(self.account_uuid),
+            headers=headers,
+            timeout=self.timeout,
+        )
+        if response.status_code != 200:
+            return None
+        return response.json()
+
+    @login_required
+    def cancel_order(self, order_id):
+        headers = self.endpoints.build_headers(self.access_token)
+        preflight = self.session.options(
+            self.endpoints.cancel_pending_order_url(self.account_uuid, order_id),
+            headers=headers,
+            timeout=self.timeout,
+        )
+        if preflight.status_code != 200:
+            raise Exception(f"Preflight failed: {preflight.text}")
+
+        response = self.session.delete(
+            self.endpoints.cancel_pending_order_url(self.account_uuid, order_id),
+            headers=headers,
+            timeout=self.timeout,
+        )
+        if response.status_code != 200:
+            return None
+        return response.json()
```

### Comparing `public_invest_api-1.0.3/public_invest_api.egg-info/PKG-INFO` & `public_invest_api-1.0.4/public_invest_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: public_invest_api
-Version: 1.0.3
+Version: 1.0.4
 Summary: Unofficial Public.com Invest API written in Python Requests
 Home-page: https://github.com/NelsonDane/public-invest-api
 Author: Nelson Dane
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: python-dotenv
```


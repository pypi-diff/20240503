# Comparing `tmp/mom_test_py-1.0.1.tar.gz` & `tmp/mom_test_py-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mom_test_py-1.0.1.tar", last modified: Tue Apr 23 09:05:31 2024, max compression
+gzip compressed data, was "mom_test_py-1.0.2.tar", last modified: Fri May  3 01:21:01 2024, max compression
```

## Comparing `mom_test_py-1.0.1.tar` & `mom_test_py-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxr-x   0 sreymom   (1000) sreymom   (1000)        0 2024-04-23 09:05:31.651826 mom_test_py-1.0.1/
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)     1707 2024-04-23 09:05:31.651826 mom_test_py-1.0.1/PKG-INFO
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)     1508 2024-04-23 08:52:00.000000 mom_test_py-1.0.1/README.md
-drwxrwxr-x   0 sreymom   (1000) sreymom   (1000)        0 2024-04-23 09:05:31.651826 mom_test_py-1.0.1/mom_test_py/
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)       24 2024-04-23 07:21:34.000000 mom_test_py-1.0.1/mom_test_py/__init__.py
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)       62 2024-04-23 07:57:43.000000 mom_test_py-1.0.1/mom_test_py/main.py
-drwxrwxr-x   0 sreymom   (1000) sreymom   (1000)        0 2024-04-23 09:05:31.651826 mom_test_py-1.0.1/mom_test_py.egg-info/
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)     1707 2024-04-23 09:05:31.000000 mom_test_py-1.0.1/mom_test_py.egg-info/PKG-INFO
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)      202 2024-04-23 09:05:31.000000 mom_test_py-1.0.1/mom_test_py.egg-info/SOURCES.txt
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)        1 2024-04-23 09:05:31.000000 mom_test_py-1.0.1/mom_test_py.egg-info/dependency_links.txt
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)       12 2024-04-23 09:05:31.000000 mom_test_py-1.0.1/mom_test_py.egg-info/top_level.txt
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)       38 2024-04-23 09:05:31.651826 mom_test_py-1.0.1/setup.cfg
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)      427 2024-04-23 09:03:23.000000 mom_test_py-1.0.1/setup.py
+drwxrwxr-x   0 sreymom   (1000) sreymom   (1000)        0 2024-05-03 01:21:01.583993 mom_test_py-1.0.2/
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)     1468 2024-05-03 01:21:01.583993 mom_test_py-1.0.2/PKG-INFO
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)     1269 2024-04-24 06:32:01.000000 mom_test_py-1.0.2/README.md
+drwxrwxr-x   0 sreymom   (1000) sreymom   (1000)        0 2024-05-03 01:21:01.579993 mom_test_py-1.0.2/mom_test_py/
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)       24 2024-04-24 10:03:17.000000 mom_test_py-1.0.2/mom_test_py/__init__.py
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)     3758 2024-05-02 09:26:11.000000 mom_test_py-1.0.2/mom_test_py/main.py
+drwxrwxr-x   0 sreymom   (1000) sreymom   (1000)        0 2024-05-03 01:21:01.583993 mom_test_py-1.0.2/mom_test_py/rest/
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)       36 2024-04-24 10:03:26.000000 mom_test_py-1.0.2/mom_test_py/rest/__init__.py
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)     6457 2024-05-02 09:43:00.000000 mom_test_py-1.0.2/mom_test_py/test_validation.py
+drwxrwxr-x   0 sreymom   (1000) sreymom   (1000)        0 2024-05-03 01:21:01.583993 mom_test_py-1.0.2/mom_test_py.egg-info/
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)     1468 2024-05-03 01:21:01.000000 mom_test_py-1.0.2/mom_test_py.egg-info/PKG-INFO
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)      262 2024-05-03 01:21:01.000000 mom_test_py-1.0.2/mom_test_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)        1 2024-05-03 01:21:01.000000 mom_test_py-1.0.2/mom_test_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)       12 2024-05-03 01:21:01.000000 mom_test_py-1.0.2/mom_test_py.egg-info/top_level.txt
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)       38 2024-05-03 01:21:01.583993 mom_test_py-1.0.2/setup.cfg
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)      427 2024-05-03 01:15:23.000000 mom_test_py-1.0.2/setup.py
```

### Comparing `mom_test_py-1.0.1/PKG-INFO` & `mom_test_py-1.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mom_test_py
-Version: 1.0.1
+Version: 1.0.2
 Summary: Helper library for working with tests
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 ### Supported Python Versions
@@ -21,38 +21,32 @@
 
 ```shell
 pip3 install plasgate
 ```
 
 ### Test your installation
 
-Try sending yourself an SMS message. Save the following code sample to your computer with a text editor. Be sure to update the `account_sid`, `auth_token`, and `from_` phone number with values from your [Twilio account](https://console.twilio.com). The `to` phone number will be your own mobile phone.
+Try sending yourself an SMS message. Save the following code sample to your computer with a text editor. Be sure to update the `account_sid`, and `auth_token` from your [Plasgate account](https://cloud.plasgate.com/).
 
 ```python
 from twilio.rest import Client
 
-# Your Account SID and Auth Token from console.twilio.com
-account_sid = "ACXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
-auth_token  = "your_auth_token"
+# Your Account private_key and x-secret_key from plasgate
+account_sid = "your_private_key"
+auth_token  = "your_X_secret_key"
 
 client = Client(account_sid, auth_token)
 
 message = client.messages.create(
-    to="+15558675309",
-    from_="+15017250604",
-    body="Hello from Python!")
+    to="+85558675309",
+    sender="text_your_sender_name",
+    content="text_your_message")
 
 print(message.sid)
 ```
 
-Save the file as `send_sms.py`. In the terminal, `cd` to the directory containing the file you just saved then run:
-
-```shell
-python3 send_sms.py
-```
-
 After a brief delay, you will receive the text message on your phone.
 
 > **Warning**
 > It's okay to hardcode your credentials when testing locally, but you should use environment variables to keep them secret before committing any code or deploying to production. Check out [How to Set Environment Variables](https://www.twilio.com/blog/2017/01/how-to-set-environment-variables.html) for more information.
```

### Comparing `mom_test_py-1.0.1/README.md` & `mom_test_py-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -12,36 +12,30 @@
 
 ```shell
 pip3 install plasgate
 ```
 
 ### Test your installation
 
-Try sending yourself an SMS message. Save the following code sample to your computer with a text editor. Be sure to update the `account_sid`, `auth_token`, and `from_` phone number with values from your [Twilio account](https://console.twilio.com). The `to` phone number will be your own mobile phone.
+Try sending yourself an SMS message. Save the following code sample to your computer with a text editor. Be sure to update the `account_sid`, and `auth_token` from your [Plasgate account](https://cloud.plasgate.com/).
 
 ```python
 from twilio.rest import Client
 
-# Your Account SID and Auth Token from console.twilio.com
-account_sid = "ACXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
-auth_token  = "your_auth_token"
+# Your Account private_key and x-secret_key from plasgate
+account_sid = "your_private_key"
+auth_token  = "your_X_secret_key"
 
 client = Client(account_sid, auth_token)
 
 message = client.messages.create(
-    to="+15558675309",
-    from_="+15017250604",
-    body="Hello from Python!")
+    to="+85558675309",
+    sender="text_your_sender_name",
+    content="text_your_message")
 
 print(message.sid)
 ```
 
-Save the file as `send_sms.py`. In the terminal, `cd` to the directory containing the file you just saved then run:
-
-```shell
-python3 send_sms.py
-```
-
 After a brief delay, you will receive the text message on your phone.
 
 > **Warning**
 > It's okay to hardcode your credentials when testing locally, but you should use environment variables to keep them secret before committing any code or deploying to production. Check out [How to Set Environment Variables](https://www.twilio.com/blog/2017/01/how-to-set-environment-variables.html) for more information.
```

### Comparing `mom_test_py-1.0.1/mom_test_py.egg-info/PKG-INFO` & `mom_test_py-1.0.2/mom_test_py.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mom-test-py
-Version: 1.0.1
+Version: 1.0.2
 Summary: Helper library for working with tests
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 ### Supported Python Versions
@@ -21,38 +21,32 @@
 
 ```shell
 pip3 install plasgate
 ```
 
 ### Test your installation
 
-Try sending yourself an SMS message. Save the following code sample to your computer with a text editor. Be sure to update the `account_sid`, `auth_token`, and `from_` phone number with values from your [Twilio account](https://console.twilio.com). The `to` phone number will be your own mobile phone.
+Try sending yourself an SMS message. Save the following code sample to your computer with a text editor. Be sure to update the `account_sid`, and `auth_token` from your [Plasgate account](https://cloud.plasgate.com/).
 
 ```python
 from twilio.rest import Client
 
-# Your Account SID and Auth Token from console.twilio.com
-account_sid = "ACXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
-auth_token  = "your_auth_token"
+# Your Account private_key and x-secret_key from plasgate
+account_sid = "your_private_key"
+auth_token  = "your_X_secret_key"
 
 client = Client(account_sid, auth_token)
 
 message = client.messages.create(
-    to="+15558675309",
-    from_="+15017250604",
-    body="Hello from Python!")
+    to="+85558675309",
+    sender="text_your_sender_name",
+    content="text_your_message")
 
 print(message.sid)
 ```
 
-Save the file as `send_sms.py`. In the terminal, `cd` to the directory containing the file you just saved then run:
-
-```shell
-python3 send_sms.py
-```
-
 After a brief delay, you will receive the text message on your phone.
 
 > **Warning**
 > It's okay to hardcode your credentials when testing locally, but you should use environment variables to keep them secret before committing any code or deploying to production. Check out [How to Set Environment Variables](https://www.twilio.com/blog/2017/01/how-to-set-environment-variables.html) for more information.
```


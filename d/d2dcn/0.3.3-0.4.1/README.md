# Comparing `tmp/d2dcn-0.3.3.tar.gz` & `tmp/d2dcn-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d2dcn-0.3.3.tar", last modified: Sun Mar 17 18:34:07 2024, max compression
+gzip compressed data, was "d2dcn-0.4.1.tar", last modified: Fri May  3 07:40:01 2024, max compression
```

## Comparing `d2dcn-0.3.3.tar` & `d2dcn-0.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2024-03-17 18:34:07.101415 d2dcn-0.3.3/
--rw-r--r--   0 docker    (1000) docker    (1000)      271 2024-03-17 18:34:07.101415 d2dcn-0.3.3/PKG-INFO
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2024-03-17 18:34:07.097415 d2dcn-0.3.3/d2dcn/
--rw-r--r--   0 docker    (1000) docker    (1000)      692 2024-01-03 16:45:16.000000 d2dcn-0.3.3/d2dcn/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)    38524 2024-03-17 18:33:42.000000 d2dcn-0.3.3/d2dcn/d2dcn.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2024-03-17 18:34:07.101415 d2dcn-0.3.3/d2dcn.egg-info/
--rw-r--r--   0 docker    (1000) docker    (1000)      271 2024-03-17 18:34:06.000000 d2dcn-0.3.3/d2dcn.egg-info/PKG-INFO
--rw-r--r--   0 docker    (1000) docker    (1000)      185 2024-03-17 18:34:06.000000 d2dcn-0.3.3/d2dcn.egg-info/SOURCES.txt
--rw-r--r--   0 docker    (1000) docker    (1000)        1 2024-03-17 18:34:06.000000 d2dcn-0.3.3/d2dcn.egg-info/dependency_links.txt
--rw-r--r--   0 docker    (1000) docker    (1000)       34 2024-03-17 18:34:06.000000 d2dcn-0.3.3/d2dcn.egg-info/requires.txt
--rw-r--r--   0 docker    (1000) docker    (1000)        6 2024-03-17 18:34:06.000000 d2dcn-0.3.3/d2dcn.egg-info/top_level.txt
--rw-r--r--   0 docker    (1000) docker    (1000)       38 2024-03-17 18:34:07.105415 d2dcn-0.3.3/setup.cfg
--rwxr-xr-x   0 docker    (1000) docker    (1000)      570 2024-01-18 22:44:40.000000 d2dcn-0.3.3/setup.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2024-05-03 07:40:01.631321 d2dcn-0.4.1/
+-rw-r--r--   0 docker    (1000) docker    (1000)      271 2024-05-03 07:40:01.631321 d2dcn-0.4.1/PKG-INFO
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2024-05-03 07:40:01.631321 d2dcn-0.4.1/d2dcn/
+-rw-r--r--   0 docker    (1000) docker    (1000)      692 2024-01-03 16:45:16.000000 d2dcn-0.4.1/d2dcn/__init__.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)    38454 2024-05-02 20:29:45.000000 d2dcn-0.4.1/d2dcn/d2dcn.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2024-05-03 07:40:01.631321 d2dcn-0.4.1/d2dcn.egg-info/
+-rw-r--r--   0 docker    (1000) docker    (1000)      271 2024-05-03 07:40:01.000000 d2dcn-0.4.1/d2dcn.egg-info/PKG-INFO
+-rw-r--r--   0 docker    (1000) docker    (1000)      185 2024-05-03 07:40:01.000000 d2dcn-0.4.1/d2dcn.egg-info/SOURCES.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)        1 2024-05-03 07:40:01.000000 d2dcn-0.4.1/d2dcn.egg-info/dependency_links.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)       34 2024-05-03 07:40:01.000000 d2dcn-0.4.1/d2dcn.egg-info/requires.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)        6 2024-05-03 07:40:01.000000 d2dcn-0.4.1/d2dcn.egg-info/top_level.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)       38 2024-05-03 07:40:01.631321 d2dcn-0.4.1/setup.cfg
+-rwxr-xr-x   0 docker    (1000) docker    (1000)      570 2024-01-18 22:44:40.000000 d2dcn-0.4.1/setup.py
```

### Comparing `d2dcn-0.3.3/d2dcn/__init__.py` & `d2dcn-0.4.1/d2dcn/__init__.py`

 * *Files identical despite different names*

### Comparing `d2dcn-0.3.3/d2dcn/d2dcn.py` & `d2dcn-0.4.1/d2dcn/d2dcn.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,18 @@
 import uuid
 import psutil
 import json
 import re
 import paho.mqtt.client
 import ServiceDiscovery
 import weakref
+import pyroute2
 
 
-version = "0.3.3"
+version = "0.4.1"
 
 
 class d2dConstants():
     MQTT_SERVICE_NAME = "MQTT_BROKER"
     MQTT_BROKER_PORT = 1883
     MTU = 4096
     MAX_LISTEN_TCP_SOKETS = 0
@@ -127,20 +128,14 @@
         chn_msg = [msg[idx : idx + d2dConstants.MTU] for idx in range(0, len(msg), d2dConstants.MTU)]
 
         for chn in chn_msg:
             self.__sock.sendto(chn, (ip, port))
 
 
     @property
-    def ip(self):
-        hostname = socket.gethostname()
-        return socket.gethostbyname(hostname)
-
-
-    @property
     def port(self):
         return self.__sock.getsockname()[1]
 
 
     def close(self):
         self.__open = False
         self.__sock.close()
@@ -255,20 +250,14 @@
 
 
         def isConnected(self):
             return self.__open
 
 
         @property
-        def ip(self):
-            hostname = socket.gethostname()
-            return socket.gethostbyname(hostname)
-
-
-        @property
         def port(self):
             return self.__sock.getsockname()[1]
 
 
         def close(self):
             self.__open = False
             self.__sock.close()
@@ -284,20 +273,14 @@
 
 
     def __del__(self):
         self.close()
 
 
     @property
-    def ip(self):
-        hostname = socket.gethostname()
-        return socket.gethostbyname(hostname)
-
-
-    @property
     def port(self):
         return self.__sock.getsockname()[1]
 
 
     def waitConnection(self, timeout=-1):
 
         current_epoch_time = int(time.time())
@@ -618,14 +601,15 @@
         self.__services = {}
         self.__info_used_paths = {}
         self.__unused_received_paths = []
 
         self.__subscriptions = []
         self.__publications = {}
         self.__client = None
+        self.__broker_ip = None
 
         self.__checkBrokerConnection()
 
 
     def __del__(self):
         if self.__client:
             self.__client.disconnect()
@@ -842,28 +826,28 @@
                     if self.__client.is_connected():
                         return True
 
                 return self.__client.is_connected()
 
 
         discover_client = ServiceDiscovery.client()
-        broker_ip = discover_client.getServiceIP(d2dConstants.MQTT_SERVICE_NAME,
+        self.__broker_ip = discover_client.getServiceIP(d2dConstants.MQTT_SERVICE_NAME,
             timeout=self.__broker_discover_timeout, retry=self.__broker_discover_retry)
-        if not broker_ip:
+        if not self.__broker_ip:
             return False
 
         version_array = paho.mqtt.__version__.split(".")
         if version_array[0] == "1":
             client = paho.mqtt.client.Client()
         else:
             client = paho.mqtt.client.Client(paho.mqtt.client.CallbackAPIVersion.VERSION1)
 
         try:
             client.will_set(self.__local_path + d2dConstants.STATE, payload=d2dConstants.state.OFFLINE, qos=1, retain=True)
-            client.connect(broker_ip, d2dConstants.MQTT_BROKER_PORT)
+            client.connect(self.__broker_ip, d2dConstants.MQTT_BROKER_PORT)
         except:
             return False
 
         client.on_message = lambda client, weak_self, message : d2d.__brokerMessageReceived(message, weak_self)
         client.on_connect = lambda client, weak_self, flags, rc : d2d.__onConnect(weak_self)
         client.user_data_set(weakref.ref(self))
         client.loop_start()
@@ -1164,14 +1148,22 @@
                     self.__subscriptions.append(mqtt_path)
             except:
                 return False
 
         return True
 
 
+    def __getOwnIP(self, dst='127.0.0.1'):
+        ipr = pyroute2.IPRoute().route('get', dst=dst)
+        if len(ipr) > 0:
+            return ipr[0].get_attr('RTA_PREFSRC')
+        else:
+            return "127.0.0.1"
+
+
     def addServiceCommand(self, cmdCallback, name:str, input_params:dict, output_params:dict, category:str="", enable=True, timeout=5, protocol=d2dConstants.commandProtocol.JSON_UDP)-> bool:
 
         if not cmdCallback:
             return False
 
         for field in input_params:
             if not d2d.__checkInOutDefinedField(input_params[field]):
@@ -1212,15 +1204,15 @@
         mqtt_path = self.__createMQTTPath(self.__mac, self.__service, category, d2dConstants.COMMAND_LEVEL, name)
         if not mqtt_path:
             return False
         self.__service_used_paths[name] = mqtt_path
 
         self.__service_container[name].map = {}
         self.__service_container[name].map[d2dConstants.commandField.PROTOCOL] = protocol
-        self.__service_container[name].map[d2dConstants.commandField.IP] = listen_socket.ip
+        self.__service_container[name].map[d2dConstants.commandField.IP] = self.__getOwnIP(self.__broker_ip)
         self.__service_container[name].map[d2dConstants.commandField.PORT] = listen_socket.port
         self.__service_container[name].map[d2dConstants.commandField.INPUT] = input_params
         self.__service_container[name].map[d2dConstants.commandField.OUTPUT] = output_params
         self.__service_container[name].map[d2dConstants.commandField.ENABLE] = enable
         self.__service_container[name].map[d2dConstants.commandField.TIMEOUT] = timeout
 
         return self.__publish(self.__service_used_paths[name], payload=json.dumps(self.__service_container[name].map, indent=1))
```

### Comparing `d2dcn-0.3.3/setup.py` & `d2dcn-0.4.1/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/modpoll-0.7.1.tar.gz` & `tmp/modpoll-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modpoll-0.7.1.tar", max compression
+gzip compressed data, was "modpoll-0.7.2.tar", max compression
```

## Comparing `modpoll-0.7.1.tar` & `modpoll-0.7.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1075 2024-02-23 11:55:14.816672 modpoll-0.7.1/LICENSE
--rw-r--r--   0        0        0    10963 2024-02-23 11:55:14.816672 modpoll-0.7.1/README.md
--rw-r--r--   0        0        0      166 2024-02-23 11:55:14.849672 modpoll-0.7.1/modpoll/__init__.py
--rw-r--r--   0        0        0       29 2024-02-23 11:55:14.849672 modpoll-0.7.1/modpoll/__main__.py
--rw-r--r--   0        0        0     5150 2024-02-23 11:55:14.849672 modpoll-0.7.1/modpoll/arg_parser.py
--rw-r--r--   0        0        0     3713 2024-02-23 11:55:14.849672 modpoll-0.7.1/modpoll/main.py
--rw-r--r--   0        0        0    22422 2024-02-23 11:55:14.849672 modpoll-0.7.1/modpoll/modbus_task.py
--rw-r--r--   0        0        0     4781 2024-02-23 11:55:14.849672 modpoll-0.7.1/modpoll/mqtt_task.py
--rw-r--r--   0        0        0      950 2024-02-23 11:55:14.850672 modpoll-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    11806 1970-01-01 00:00:00.000000 modpoll-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-03 12:58:58.586459 modpoll-0.7.2/LICENSE
+-rw-r--r--   0        0        0    11058 2024-05-03 12:58:58.587459 modpoll-0.7.2/README.md
+-rw-r--r--   0        0        0      166 2024-05-03 12:58:58.631459 modpoll-0.7.2/modpoll/__init__.py
+-rw-r--r--   0        0        0       29 2024-05-03 12:58:58.631459 modpoll-0.7.2/modpoll/__main__.py
+-rw-r--r--   0        0        0     5159 2024-05-03 12:58:58.631459 modpoll-0.7.2/modpoll/arg_parser.py
+-rw-r--r--   0        0        0     3722 2024-05-03 12:58:58.631459 modpoll-0.7.2/modpoll/main.py
+-rw-r--r--   0        0        0    22643 2024-05-03 12:58:58.631459 modpoll-0.7.2/modpoll/modbus_task.py
+-rw-r--r--   0        0        0     4939 2024-05-03 12:58:58.631459 modpoll-0.7.2/modpoll/mqtt_task.py
+-rw-r--r--   0        0        0      959 2024-05-03 12:58:58.632459 modpoll-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0    11910 1970-01-01 00:00:00.000000 modpoll-0.7.2/PKG-INFO
```

### Comparing `modpoll-0.7.1/LICENSE` & `modpoll-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modpoll-0.7.1/README.md` & `modpoll-0.7.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# modpoll - A New Command-line Tool for Modbus
+# modpoll - A New Command-line Tool for Modbus and MQTT
 
 [![pipeline status](https://gitlab.com/helloysd/modpoll/badges/master/pipeline.svg)](https://gitlab.com/helloysd/modpoll/-/commits/master)
 [![License](https://img.shields.io/pypi/l/modpoll)](https://gitlab.com/helloysd/modpoll/-/blob/master/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/modpoll/week)](https://pepy.tech/project/modpoll)
 
 > Learn more about *modpoll* usage at [documentation](https://helloysd.gitlab.io/modpoll) site.
 
@@ -155,30 +155,35 @@
 > *Refer to the [documentation](https://helloysd.gitlab.io/modpoll/configure.html) site for more details.*
 
 ### Poll local device (modsim)
 
 If you are blocked by company firewall for online device or prefer a local test, you can launch your own device simulator by running *modsim* locally,
 
 ```bash
-docker run -p 5020:5020 helloysd/modsim
+docker run --rm -p 5020:5020 helloysd/modsim
 ```
 
-It will create a virtual Modbus TCP device running at `localhost:5020`, and then you can poll it using *modpoll* tool,
+It will create a virtual Modbus TCP device running at `localhost:5020`, and you can open a new terminal, poll the virtual device using *modpoll* tool,
 
 ```bash
 modpoll \
   --tcp localhost \
   --tcp-port 5020 \
   --config https://raw.githubusercontent.com/gavinying/modpoll/master/examples/modsim.csv
 ```
 
 > Use `sudo` before the docker command if you want to use the standard port `502`.
 
 ```bash
-sudo docker run -p 502:5020 helloysd/modsim
+sudo docker run --rm -p 502:5020 helloysd/modsim
+```
+
+In a new terminal,
+
+```
 modpoll \
   --tcp localhost \
   --config https://raw.githubusercontent.com/gavinying/modpoll/master/examples/modsim.csv
 ```
 
 ### Publish data to MQTT broker
 
@@ -229,33 +234,33 @@
 
 
 ## Run with docker
 
 A docker image has been provided for user to directly run the program without local installation,
 
   ```bash
-  docker run helloysd/modpoll
+  docker run --rm helloysd/modpoll
   ```
 
 It shows the version of the program by default.
 
 Similar to the above *modsim* test, we can poll data with `docker run`, in order to avoid printing out received data, the argument `--daemon` or `-d` is recommended to use with docker.
 
   ```bash
-  docker run helloysd/modpoll \
+  docker run --rm helloysd/modpoll \
     modpoll -d \
       --tcp modsim.topmaker.net \
       --config https://raw.githubusercontent.com/gavinying/modpoll/master/examples/modsim.csv
   ```
 
 If you want to load a local configure file, you need to mount a local folder onto container volume,
 for example, if the child folder `examples` contains the config file `modsim.csv`, we can use it via the following command,
 
   ```bash
-  docker run -v $(pwd)/examples:/app/examples helloysd/modpoll \
+  docker run --rm -v $(pwd)/examples:/app/examples helloysd/modpoll \
     modpoll -d \
       --tcp modsim.topmaker.net \
       --config /app/examples/modsim.csv
   ```
 
 
 ## Basic Usage
```

### Comparing `modpoll-0.7.1/modpoll/arg_parser.py` & `modpoll-0.7.2/modpoll/arg_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 
 from . import __version__
 
 
 def get_parser():
     parser = argparse.ArgumentParser(
-        description=f"modpoll v{__version__} - A New Command Line Tool for Modbus"
+        description=f"modpoll v{__version__} - A New Command-line Tool for Modbus and MQTT"
     )
     parser.add_argument(
         "-v",
         "--version",
         action="version",
         version=f"modpoll v{__version__}",
     )
```

### Comparing `modpoll-0.7.1/modpoll/main.py` & `modpoll-0.7.2/modpoll/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 def get_utc_time():
     dt = datetime.datetime.now(timezone.utc)
     utc_time = dt.replace(tzinfo=timezone.utc)
     return utc_time.timestamp()
 
 
 def app(name="modpoll"):
-    print("\nmodpoll - A New Command Line Tool for Modbus\n", flush=True)
+    print("\nmodpoll - A New Command-line Tool for Modbus and MQTT\n", flush=True)
 
     signal.signal(signal.SIGINT, _signal_handler)
 
     # parse args
     args = get_parser().parse_args()
 
     # get logger
```

### Comparing `modpoll-0.7.1/modpoll/modbus_task.py` & `modpoll-0.7.2/modpoll/modbus_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,17 @@
                     cur_ref += ref.ref_width
                 elif "uint64" == ref.dtype:
                     ref.update_value(decoder.decode_64bit_uint())
                     cur_ref += ref.ref_width
                 elif "int64" == ref.dtype:
                     ref.update_value(decoder.decode_64bit_int())
                     cur_ref += ref.ref_width
+                elif "float16" == ref.dtype:
+                    ref.update_value(decoder.decode_16bit_float())
+                    cur_ref += ref.ref_width
                 elif "float32" == ref.dtype:
                     ref.update_value(decoder.decode_32bit_float())
                     cur_ref += ref.ref_width
                 elif "float64" == ref.dtype:
                     ref.update_value(decoder.decode_64bit_float())
                     cur_ref += ref.ref_width
                 elif "bool8" == ref.dtype or "bool" == ref.dtype:
@@ -227,14 +230,16 @@
             self.ref_width = 2
         elif "uint32" == dtype:
             self.ref_width = 2
         elif "int64" == dtype:
             self.ref_width = 4
         elif "uint64" == dtype:
             self.ref_width = 4
+        elif "float16" == dtype:
+            self.ref_width = 1
         elif "float32" == dtype:
             self.ref_width = 2
         elif "float64" == dtype:
             self.ref_width = 4
         elif "bool8" == dtype or "bool" == dtype:
             self.ref_width = 1
         elif "bool16" == dtype:
```

### Comparing `modpoll-0.7.1/modpoll/mqtt_task.py` & `modpoll-0.7.2/modpoll/mqtt_task.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 
 # Callbacks
 def _on_connect(client, userdata, flags, rc, properties=None):
     if rc == 0:
         log.info("Connection successful")
         # Subscribing in on_connect() means that if we lose the connection and
         # reconnect then subscriptions will be renewed.
-        client.subscribe(f"{args.mqtt_topic_prefix}+/set")
+        qos = userdata.get("qos", 0)  # Default to QoS 0 if not provided
+        client.subscribe(f"{args.mqtt_topic_prefix}+/set", qos)
     elif rc == 1:
         log.warning("Connection refused - incorrect protocol version")
     elif rc == 2:
         log.warning("Connection refused - invalid client identifier")
     elif rc == 3:
         log.warning("Connection refused - server unavailable")
     elif rc == 4:
@@ -79,15 +80,19 @@
             if args.mqtt_qos == 0:
                 clientid = ""
             else:
                 clientid = socket.gethostname()
         else:
             clientid = args.mqtt_clientid
         global mqttc
-        mqttc = mqtt.Client(clientid, clean_session=(args.mqtt_qos == 0))
+        mqttc = mqtt.Client(
+            clientid,
+            clean_session=(args.mqtt_qos == 0),
+            userdata={"qos": args.mqtt_qos},
+        )
         if args.mqtt_use_tls:
             if args.mqtt_tls_version == "tlsv1.2":
                 tlsVersion = ssl.PROTOCOL_TLSv1_2
             elif args.mqtt_tls_version == "tlsv1.1":
                 tlsVersion = ssl.PROTOCOL_TLSv1_1
             elif args.mqtt_tls_version == "tlsv1":
                 tlsVersion = ssl.PROTOCOL_TLSv1
```

### Comparing `modpoll-0.7.1/pyproject.toml` & `modpoll-0.7.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "modpoll"
-version = "0.7.1"
-description = "A New Command Line Tool for Modbus"
+version = "0.7.2"
+description = "A New Command-line Tool for Modbus and MQTT"
 authors = ["Ying Shaodong <helloysd@gmail.com>"]
 readme = "README.md"
 homepage = "https://helloysd.gitlab.io/modpoll"
 repository = "https://github.com/gavinying/modpoll"
 license = "MIT"
 include = [
   "LICENSE",
```

### Comparing `modpoll-0.7.1/PKG-INFO` & `modpoll-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: modpoll
-Version: 0.7.1
-Summary: A New Command Line Tool for Modbus
+Version: 0.7.2
+Summary: A New Command-line Tool for Modbus and MQTT
 Home-page: https://helloysd.gitlab.io/modpoll
 License: MIT
 Author: Ying Shaodong
 Author-email: helloysd@gmail.com
 Requires-Python: >=3.8.2,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 Requires-Dist: prettytable (>=3.6.0,<4.0.0)
 Requires-Dist: pymodbus (>=3.5.4,<4.0.0)
 Requires-Dist: pyserial (>=3.5,<4.0) ; extra == "serial"
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Repository, https://github.com/gavinying/modpoll
 Description-Content-Type: text/markdown
 
-# modpoll - A New Command-line Tool for Modbus
+# modpoll - A New Command-line Tool for Modbus and MQTT
 
 [![pipeline status](https://gitlab.com/helloysd/modpoll/badges/master/pipeline.svg)](https://gitlab.com/helloysd/modpoll/-/commits/master)
 [![License](https://img.shields.io/pypi/l/modpoll)](https://gitlab.com/helloysd/modpoll/-/blob/master/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/modpoll/week)](https://pepy.tech/project/modpoll)
 
 > Learn more about *modpoll* usage at [documentation](https://helloysd.gitlab.io/modpoll) site.
 
@@ -178,30 +178,35 @@
 > *Refer to the [documentation](https://helloysd.gitlab.io/modpoll/configure.html) site for more details.*
 
 ### Poll local device (modsim)
 
 If you are blocked by company firewall for online device or prefer a local test, you can launch your own device simulator by running *modsim* locally,
 
 ```bash
-docker run -p 5020:5020 helloysd/modsim
+docker run --rm -p 5020:5020 helloysd/modsim
 ```
 
-It will create a virtual Modbus TCP device running at `localhost:5020`, and then you can poll it using *modpoll* tool,
+It will create a virtual Modbus TCP device running at `localhost:5020`, and you can open a new terminal, poll the virtual device using *modpoll* tool,
 
 ```bash
 modpoll \
   --tcp localhost \
   --tcp-port 5020 \
   --config https://raw.githubusercontent.com/gavinying/modpoll/master/examples/modsim.csv
 ```
 
 > Use `sudo` before the docker command if you want to use the standard port `502`.
 
 ```bash
-sudo docker run -p 502:5020 helloysd/modsim
+sudo docker run --rm -p 502:5020 helloysd/modsim
+```
+
+In a new terminal,
+
+```
 modpoll \
   --tcp localhost \
   --config https://raw.githubusercontent.com/gavinying/modpoll/master/examples/modsim.csv
 ```
 
 ### Publish data to MQTT broker
 
@@ -252,33 +257,33 @@
 
 
 ## Run with docker
 
 A docker image has been provided for user to directly run the program without local installation,
 
   ```bash
-  docker run helloysd/modpoll
+  docker run --rm helloysd/modpoll
   ```
 
 It shows the version of the program by default.
 
 Similar to the above *modsim* test, we can poll data with `docker run`, in order to avoid printing out received data, the argument `--daemon` or `-d` is recommended to use with docker.
 
   ```bash
-  docker run helloysd/modpoll \
+  docker run --rm helloysd/modpoll \
     modpoll -d \
       --tcp modsim.topmaker.net \
       --config https://raw.githubusercontent.com/gavinying/modpoll/master/examples/modsim.csv
   ```
 
 If you want to load a local configure file, you need to mount a local folder onto container volume,
 for example, if the child folder `examples` contains the config file `modsim.csv`, we can use it via the following command,
 
   ```bash
-  docker run -v $(pwd)/examples:/app/examples helloysd/modpoll \
+  docker run --rm -v $(pwd)/examples:/app/examples helloysd/modpoll \
     modpoll -d \
       --tcp modsim.topmaker.net \
       --config /app/examples/modsim.csv
   ```
 
 
 ## Basic Usage
```


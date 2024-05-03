# Comparing `tmp/ocks-0.1.tar.gz` & `tmp/ocks-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocks-0.1.tar", last modified: Fri May  3 21:20:56 2024, max compression
+gzip compressed data, was "ocks-0.2.tar", last modified: Fri May  3 21:38:36 2024, max compression
```

## Comparing `ocks-0.1.tar` & `ocks-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 21:20:56.623496 ocks-0.1/
--rw-rw-rw-   0        0        0     1083 2024-05-03 18:19:34.000000 ocks-0.1/LICENSE
--rw-rw-rw-   0        0        0       69 2024-05-03 21:16:02.000000 ocks-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1410 2024-05-03 21:20:56.622045 ocks-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1138 2024-05-03 21:16:56.000000 ocks-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 21:20:56.612646 ocks-0.1/ocks/
--rw-rw-rw-   0        0        0       36 2024-05-03 21:15:07.000000 ocks-0.1/ocks/__init__.py
--rw-rw-rw-   0        0        0     3599 2024-05-03 18:44:54.000000 ocks-0.1/ocks/ssd1306.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:20:56.620993 ocks-0.1/ocks.egg-info/
--rw-rw-rw-   0        0        0     1410 2024-05-03 21:20:56.000000 ocks-0.1/ocks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2024-05-03 21:20:56.000000 ocks-0.1/ocks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 21:20:56.000000 ocks-0.1/ocks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-03 21:20:56.000000 ocks-0.1/ocks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 21:20:56.624011 ocks-0.1/setup.cfg
--rw-rw-rw-   0        0        0      932 2024-05-03 21:18:16.000000 ocks-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:38:36.066890 ocks-0.2/
+-rw-rw-rw-   0        0        0     1083 2024-05-03 18:19:34.000000 ocks-0.2/LICENSE
+-rw-rw-rw-   0        0        0       69 2024-05-03 21:16:02.000000 ocks-0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1459 2024-05-03 21:38:36.066890 ocks-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1186 2024-05-03 21:38:30.000000 ocks-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 21:38:36.040891 ocks-0.2/ocks/
+-rw-rw-rw-   0        0        0       36 2024-05-03 21:15:07.000000 ocks-0.2/ocks/__init__.py
+-rw-rw-rw-   0        0        0     3599 2024-05-03 18:44:54.000000 ocks-0.2/ocks/ssd1306.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:38:36.064893 ocks-0.2/ocks.egg-info/
+-rw-rw-rw-   0        0        0     1459 2024-05-03 21:38:35.000000 ocks-0.2/ocks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2024-05-03 21:38:35.000000 ocks-0.2/ocks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 21:38:35.000000 ocks-0.2/ocks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-03 21:38:35.000000 ocks-0.2/ocks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 21:38:36.067890 ocks-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      933 2024-05-03 21:34:55.000000 ocks-0.2/setup.py
```

### Comparing `ocks-0.1/LICENSE` & `ocks-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ocks-0.1/PKG-INFO` & `ocks-0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ocks
-Version: 0.1
-Summary: river for micropython compatible with ssd1306 OLED displays.
+Version: 0.2
+Summary: driver for micropython compatible with ssd1306 OLED displays.
 Author: Cesar
 Author-email: cesar.bautista@uelectronics.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SSD1306 Library
@@ -19,29 +19,29 @@
 ```python
 import machine
 
 i2c = machine.I2C(0, sda=machine.Pin(21), scl=machine.Pin(22))
 
 print(i2c.scan())
 ```
-
+![thonny install](./Images/ins.png)
 
 Code example
 
 ```py
 
 
 '''
-Unit Electronics 2023
-          (o_
-   (o_    //\
-   (/)_   V_/_ 
-tested code mark
-   version: 0.0.1
-   revision: 0.0.1
+    Unit Electronics 2023
+           (o_
+    (o_    //\
+    (/)_   V_/_ 
+    tested code mark
+    version: 0.0.1
+    revision: 0.0.1
 
 '''
 
 import machine
 from ocks import SSD1306_I2C
 
 i2c = machine.I2C(0,sda=machine.Pin(21), scl=machine.Pin(22))
```

### Comparing `ocks-0.1/README.md` & `ocks-0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -9,29 +9,29 @@
 ```python
 import machine
 
 i2c = machine.I2C(0, sda=machine.Pin(21), scl=machine.Pin(22))
 
 print(i2c.scan())
 ```
-
+![thonny install](./Images/ins.png)
 
 Code example
 
 ```py
 
 
 '''
-Unit Electronics 2023
-          (o_
-   (o_    //\
-   (/)_   V_/_ 
-tested code mark
-   version: 0.0.1
-   revision: 0.0.1
+    Unit Electronics 2023
+           (o_
+    (o_    //\
+    (/)_   V_/_ 
+    tested code mark
+    version: 0.0.1
+    revision: 0.0.1
 
 '''
 
 import machine
 from ocks import SSD1306_I2C
 
 i2c = machine.I2C(0,sda=machine.Pin(21), scl=machine.Pin(22))
```

### Comparing `ocks-0.1/ocks/ssd1306.py` & `ocks-0.2/ocks/ssd1306.py`

 * *Files identical despite different names*

### Comparing `ocks-0.1/ocks.egg-info/PKG-INFO` & `ocks-0.2/ocks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ocks
-Version: 0.1
-Summary: river for micropython compatible with ssd1306 OLED displays.
+Version: 0.2
+Summary: driver for micropython compatible with ssd1306 OLED displays.
 Author: Cesar
 Author-email: cesar.bautista@uelectronics.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SSD1306 Library
@@ -19,29 +19,29 @@
 ```python
 import machine
 
 i2c = machine.I2C(0, sda=machine.Pin(21), scl=machine.Pin(22))
 
 print(i2c.scan())
 ```
-
+![thonny install](./Images/ins.png)
 
 Code example
 
 ```py
 
 
 '''
-Unit Electronics 2023
-          (o_
-   (o_    //\
-   (/)_   V_/_ 
-tested code mark
-   version: 0.0.1
-   revision: 0.0.1
+    Unit Electronics 2023
+           (o_
+    (o_    //\
+    (/)_   V_/_ 
+    tested code mark
+    version: 0.0.1
+    revision: 0.0.1
 
 '''
 
 import machine
 from ocks import SSD1306_I2C
 
 i2c = machine.I2C(0,sda=machine.Pin(21), scl=machine.Pin(22))
```

### Comparing `ocks-0.1/setup.py` & `ocks-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.1'
+VERSION = '0.2'
 PACKAGE_NAME = 'ocks'
 AUTHOR = 'Cesar'
 AUTHOR_EMAIL = 'cesar.bautista@uelectronics.com'
 LICENSE = 'MIT License'
-DESCRIPTION = 'river for micropython compatible with ssd1306 OLED displays.'
+DESCRIPTION = 'driver for micropython compatible with ssd1306 OLED displays.'
 # Read the contents of your README file for the long description
 with open('README.md', 'r', encoding='utf-8') as f:
     LONG_DESCRIPTION = f.read()
 
 # Add your required packages to INSTALL_REQUIRES list
 INSTALL_REQUIRES = []
```


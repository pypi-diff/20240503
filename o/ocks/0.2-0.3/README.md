# Comparing `tmp/ocks-0.2.tar.gz` & `tmp/ocks-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocks-0.2.tar", last modified: Fri May  3 21:38:36 2024, max compression
+gzip compressed data, was "ocks-0.3.tar", last modified: Fri May  3 21:43:02 2024, max compression
```

## Comparing `ocks-0.2.tar` & `ocks-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 21:38:36.066890 ocks-0.2/
--rw-rw-rw-   0        0        0     1083 2024-05-03 18:19:34.000000 ocks-0.2/LICENSE
--rw-rw-rw-   0        0        0       69 2024-05-03 21:16:02.000000 ocks-0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1459 2024-05-03 21:38:36.066890 ocks-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1186 2024-05-03 21:38:30.000000 ocks-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 21:38:36.040891 ocks-0.2/ocks/
--rw-rw-rw-   0        0        0       36 2024-05-03 21:15:07.000000 ocks-0.2/ocks/__init__.py
--rw-rw-rw-   0        0        0     3599 2024-05-03 18:44:54.000000 ocks-0.2/ocks/ssd1306.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:38:36.064893 ocks-0.2/ocks.egg-info/
--rw-rw-rw-   0        0        0     1459 2024-05-03 21:38:35.000000 ocks-0.2/ocks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2024-05-03 21:38:35.000000 ocks-0.2/ocks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 21:38:35.000000 ocks-0.2/ocks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-03 21:38:35.000000 ocks-0.2/ocks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 21:38:36.067890 ocks-0.2/setup.cfg
--rw-rw-rw-   0        0        0      933 2024-05-03 21:34:55.000000 ocks-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:43:02.277333 ocks-0.3/
+-rw-rw-rw-   0        0        0     1083 2024-05-03 18:19:34.000000 ocks-0.3/LICENSE
+-rw-rw-rw-   0        0        0       69 2024-05-03 21:16:02.000000 ocks-0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1524 2024-05-03 21:43:02.276376 ocks-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1251 2024-05-03 21:42:24.000000 ocks-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 21:43:02.248336 ocks-0.3/ocks/
+-rw-rw-rw-   0        0        0       36 2024-05-03 21:15:07.000000 ocks-0.3/ocks/__init__.py
+-rw-rw-rw-   0        0        0     3599 2024-05-03 18:44:54.000000 ocks-0.3/ocks/ssd1306.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:43:02.275332 ocks-0.3/ocks.egg-info/
+-rw-rw-rw-   0        0        0     1524 2024-05-03 21:43:02.000000 ocks-0.3/ocks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2024-05-03 21:43:02.000000 ocks-0.3/ocks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 21:43:02.000000 ocks-0.3/ocks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-03 21:43:02.000000 ocks-0.3/ocks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 21:43:02.277333 ocks-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      933 2024-05-03 21:42:46.000000 ocks-0.3/setup.py
```

### Comparing `ocks-0.2/LICENSE` & `ocks-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ocks-0.2/PKG-INFO` & `ocks-0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocks
-Version: 0.2
+Version: 0.3
 Summary: driver for micropython compatible with ssd1306 OLED displays.
 Author: Cesar
 Author-email: cesar.bautista@uelectronics.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -19,15 +19,15 @@
 ```python
 import machine
 
 i2c = machine.I2C(0, sda=machine.Pin(21), scl=machine.Pin(22))
 
 print(i2c.scan())
 ```
-![thonny install](./Images/ins.png)
+![thonny install](https://raw.githubusercontent.com/Cesarbautista10/ISE_SSD1306/main/Images/ins.png)
 
 Code example
 
 ```py
 
 
 '''
```

### Comparing `ocks-0.2/README.md` & `ocks-0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ```python
 import machine
 
 i2c = machine.I2C(0, sda=machine.Pin(21), scl=machine.Pin(22))
 
 print(i2c.scan())
 ```
-![thonny install](./Images/ins.png)
+![thonny install](https://raw.githubusercontent.com/Cesarbautista10/ISE_SSD1306/main/Images/ins.png)
 
 Code example
 
 ```py
 
 
 '''
```

### Comparing `ocks-0.2/ocks/ssd1306.py` & `ocks-0.3/ocks/ssd1306.py`

 * *Files identical despite different names*

### Comparing `ocks-0.2/ocks.egg-info/PKG-INFO` & `ocks-0.3/ocks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocks
-Version: 0.2
+Version: 0.3
 Summary: driver for micropython compatible with ssd1306 OLED displays.
 Author: Cesar
 Author-email: cesar.bautista@uelectronics.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -19,15 +19,15 @@
 ```python
 import machine
 
 i2c = machine.I2C(0, sda=machine.Pin(21), scl=machine.Pin(22))
 
 print(i2c.scan())
 ```
-![thonny install](./Images/ins.png)
+![thonny install](https://raw.githubusercontent.com/Cesarbautista10/ISE_SSD1306/main/Images/ins.png)
 
 Code example
 
 ```py
 
 
 '''
```

### Comparing `ocks-0.2/setup.py` & `ocks-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.2'
+VERSION = '0.3'
 PACKAGE_NAME = 'ocks'
 AUTHOR = 'Cesar'
 AUTHOR_EMAIL = 'cesar.bautista@uelectronics.com'
 LICENSE = 'MIT License'
 DESCRIPTION = 'driver for micropython compatible with ssd1306 OLED displays.'
 # Read the contents of your README file for the long description
 with open('README.md', 'r', encoding='utf-8') as f:
```


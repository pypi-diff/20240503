# Comparing `tmp/picchick-0.4.0.tar.gz` & `tmp/picchick-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picchick-0.4.0.tar", last modified: Sat Oct 29 23:00:01 2022, max compression
+gzip compressed data, was "picchick-0.4.1.tar", last modified: Fri May  3 00:09:20 2024, max compression
```

## Comparing `picchick-0.4.0.tar` & `picchick-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 rex       (1000) rex       (1000)        0 2022-10-29 23:00:01.987957 picchick-0.4.0/
--rw-r--r--   0 rex       (1000) rex       (1000)     1637 2022-03-06 03:50:04.000000 picchick-0.4.0/LICENSE
--rw-r--r--   0 rex       (1000) rex       (1000)     2969 2022-10-29 23:00:01.987957 picchick-0.4.0/PKG-INFO
--rw-r--r--   0 rex       (1000) rex       (1000)     2471 2022-10-29 22:57:31.000000 picchick-0.4.0/README.md
-drwxr-xr-x   0 rex       (1000) rex       (1000)        0 2022-10-29 23:00:01.987957 picchick-0.4.0/picchick/
--rw-r--r--   0 rex       (1000) rex       (1000)       45 2022-10-28 18:50:29.000000 picchick-0.4.0/picchick/__init__.py
--rw-r--r--   0 rex       (1000) rex       (1000)       59 2022-10-24 16:25:20.000000 picchick-0.4.0/picchick/__main__.py
--rwxr-xr-x   0 rex       (1000) rex       (1000)     9277 2022-10-28 19:09:05.000000 picchick-0.4.0/picchick/cli.py
--rw-r--r--   0 rex       (1000) rex       (1000)    11389 2022-10-27 20:58:34.000000 picchick-0.4.0/picchick/devices.py
--rw-r--r--   0 rex       (1000) rex       (1000)    10420 2022-10-26 22:36:29.000000 picchick-0.4.0/picchick/hexfile.py
-drwxr-xr-x   0 rex       (1000) rex       (1000)        0 2022-10-29 23:00:01.987957 picchick-0.4.0/picchick/programmer/
--rw-r--r--   0 rex       (1000) rex       (1000)       72 2022-10-24 16:37:11.000000 picchick-0.4.0/picchick/programmer/__init__.py
--rw-r--r--   0 rex       (1000) rex       (1000)     6612 2022-10-28 19:51:13.000000 picchick-0.4.0/picchick/programmer/flipflop.py
--rw-r--r--   0 rex       (1000) rex       (1000)     4048 2022-10-27 16:44:59.000000 picchick-0.4.0/picchick/programmer/picstick.py
--rw-r--r--   0 rex       (1000) rex       (1000)     2562 2022-10-26 23:53:05.000000 picchick-0.4.0/picchick/programmer/programmer.py
-drwxr-xr-x   0 rex       (1000) rex       (1000)        0 2022-10-29 23:00:01.987957 picchick-0.4.0/picchick.egg-info/
--rw-r--r--   0 rex       (1000) rex       (1000)     2969 2022-10-29 23:00:01.000000 picchick-0.4.0/picchick.egg-info/PKG-INFO
--rw-r--r--   0 rex       (1000) rex       (1000)      464 2022-10-29 23:00:01.000000 picchick-0.4.0/picchick.egg-info/SOURCES.txt
--rw-r--r--   0 rex       (1000) rex       (1000)        1 2022-10-29 23:00:01.000000 picchick-0.4.0/picchick.egg-info/dependency_links.txt
--rw-r--r--   0 rex       (1000) rex       (1000)       44 2022-10-29 23:00:01.000000 picchick-0.4.0/picchick.egg-info/entry_points.txt
--rw-r--r--   0 rex       (1000) rex       (1000)        9 2022-10-29 23:00:01.000000 picchick-0.4.0/picchick.egg-info/requires.txt
--rw-r--r--   0 rex       (1000) rex       (1000)        9 2022-10-29 23:00:01.000000 picchick-0.4.0/picchick.egg-info/top_level.txt
--rw-r--r--   0 rex       (1000) rex       (1000)       89 2022-03-06 00:45:02.000000 picchick-0.4.0/pyproject.toml
--rw-r--r--   0 rex       (1000) rex       (1000)      697 2022-10-29 23:00:01.987957 picchick-0.4.0/setup.cfg
+drwxr-xr-x   0 rex       (1000) rex       (1000)        0 2024-05-03 00:09:20.659282 picchick-0.4.1/
+-rw-r--r--   0 rex       (1000) rex       (1000)     1642 2024-05-03 00:01:50.000000 picchick-0.4.1/LICENSE
+-rw-r--r--   0 rex       (1000) rex       (1000)     3062 2024-05-03 00:09:20.659282 picchick-0.4.1/PKG-INFO
+-rw-r--r--   0 rex       (1000) rex       (1000)     2540 2024-05-03 00:01:50.000000 picchick-0.4.1/README.md
+drwxr-xr-x   0 rex       (1000) rex       (1000)        0 2024-05-03 00:09:20.655948 picchick-0.4.1/picchick/
+-rw-r--r--   0 rex       (1000) rex       (1000)       45 2024-04-11 20:30:32.000000 picchick-0.4.1/picchick/__init__.py
+-rw-r--r--   0 rex       (1000) rex       (1000)       59 2024-04-11 20:30:32.000000 picchick-0.4.1/picchick/__main__.py
+-rwxr-xr-x   0 rex       (1000) rex       (1000)     9398 2024-05-03 00:01:50.000000 picchick-0.4.1/picchick/cli.py
+-rw-r--r--   0 rex       (1000) rex       (1000)    11389 2024-04-11 20:30:32.000000 picchick-0.4.1/picchick/devices.py
+-rw-r--r--   0 rex       (1000) rex       (1000)    10420 2024-04-11 20:30:32.000000 picchick-0.4.1/picchick/hexfile.py
+drwxr-xr-x   0 rex       (1000) rex       (1000)        0 2024-05-03 00:09:20.659282 picchick-0.4.1/picchick/programmer/
+-rw-r--r--   0 rex       (1000) rex       (1000)       99 2024-05-03 00:01:50.000000 picchick-0.4.1/picchick/programmer/__init__.py
+-rw-r--r--   0 rex       (1000) rex       (1000)     2875 2024-05-03 00:01:50.000000 picchick-0.4.1/picchick/programmer/arduino_icsp.py
+-rw-r--r--   0 rex       (1000) rex       (1000)     6612 2024-04-11 20:30:32.000000 picchick-0.4.1/picchick/programmer/flipflop.py
+-rw-r--r--   0 rex       (1000) rex       (1000)     4048 2024-04-11 20:30:32.000000 picchick-0.4.1/picchick/programmer/picstick.py
+-rw-r--r--   0 rex       (1000) rex       (1000)     2562 2024-04-11 20:30:32.000000 picchick-0.4.1/picchick/programmer/programmer.py
+drwxr-xr-x   0 rex       (1000) rex       (1000)        0 2024-05-03 00:09:20.659282 picchick-0.4.1/picchick.egg-info/
+-rw-r--r--   0 rex       (1000) rex       (1000)     3062 2024-05-03 00:09:20.000000 picchick-0.4.1/picchick.egg-info/PKG-INFO
+-rw-r--r--   0 rex       (1000) rex       (1000)      500 2024-05-03 00:09:20.000000 picchick-0.4.1/picchick.egg-info/SOURCES.txt
+-rw-r--r--   0 rex       (1000) rex       (1000)        1 2024-05-03 00:09:20.000000 picchick-0.4.1/picchick.egg-info/dependency_links.txt
+-rw-r--r--   0 rex       (1000) rex       (1000)       44 2024-05-03 00:09:20.000000 picchick-0.4.1/picchick.egg-info/entry_points.txt
+-rw-r--r--   0 rex       (1000) rex       (1000)        9 2024-05-03 00:09:20.000000 picchick-0.4.1/picchick.egg-info/requires.txt
+-rw-r--r--   0 rex       (1000) rex       (1000)        9 2024-05-03 00:09:20.000000 picchick-0.4.1/picchick.egg-info/top_level.txt
+-rw-r--r--   0 rex       (1000) rex       (1000)       89 2024-04-11 20:30:32.000000 picchick-0.4.1/pyproject.toml
+-rw-r--r--   0 rex       (1000) rex       (1000)      697 2024-05-03 00:09:20.659282 picchick-0.4.1/setup.cfg
```

### Comparing `picchick-0.4.0/LICENSE` & `picchick-0.4.1/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 University of Illinois/NCSA Open Source License
 
-Copyright (c) 2022, Rex McKinnon. All rights reserved.
+Copyright (c) 2022-2024, Rex McKinnon. All rights reserved.
 
 Developed by:
 
             Rex McKinnon
 
             https://github.com/rex--/picchick
```

### Comparing `picchick-0.4.0/PKG-INFO` & `picchick-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: picchick
-Version: 0.4.0
+Version: 0.4.1
 Summary: A utility for programming and debugging microcontrollers.
 Home-page: https://github.com/rex--/picchick
 Author: Rex McKinnon
 Author-email: 0xff@rexploits.com
 License: University of Illinois/NCSA Open Source License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: University of Illinois/NCSA Open Source License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyserial
 
 # picchick
 `picchick` is a command-line utility used for programming and debugging
 microcontrollers.
 
 The function is the same as `avrdude`, i.e. to provide a way to flash a compiled
 .hex file onto a microcontroller.
@@ -66,20 +67,21 @@
 $ picchick -h
 usage: picchick [-d <mcu>] [-c <programmer>] [-r <addr> [len] | -w <addr> <word> | -f] [-e [addr]] [-v] [hexfile]
        picchick [-d <mcu>] [--map | --list-ports] [hexfile]
 
 A utility for programming and debugging microcontrollers.
 
 positional arguments:
-  hexfile               path to a hexfile
+  hexfile                 path to a hexfile
 
 options:
-  -c programmer         type of programmer
-  -d mcu, --device mcu  device to be programmed
-  -h, --help            print this message and exit
+  -c programmer           type of programmer
+  -d mcu, --device mcu    device to be programmed
+  --version               print version number and exit
+  -h, --help              print this message and exit
 
 actions:
   -r, --read addr [len]   read bytes from specified address
   -w, --write addr word   write word to specified address
   -f, --flash             flash hexfile onto the device
   -e, --erase [addr]      erase device or specified address
   -v, --verify            verify device memory
@@ -95,10 +97,10 @@
 **Github:** https://github.com/rex--/picchick
 
 **PyPi:** https://pypi.org/project/picchick/
 
 
 ## Copying
 
-Copyright (C) 2022 Rex McKinnon \
+Copyright (C) 2022-2024 Rex McKinnon \
 This software is released under the University of Illinois/NCSA
 Open Source License. Check the LICENSE file for more details.
```

### Comparing `picchick-0.4.0/README.md` & `picchick-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -52,20 +52,21 @@
 $ picchick -h
 usage: picchick [-d <mcu>] [-c <programmer>] [-r <addr> [len] | -w <addr> <word> | -f] [-e [addr]] [-v] [hexfile]
        picchick [-d <mcu>] [--map | --list-ports] [hexfile]
 
 A utility for programming and debugging microcontrollers.
 
 positional arguments:
-  hexfile               path to a hexfile
+  hexfile                 path to a hexfile
 
 options:
-  -c programmer         type of programmer
-  -d mcu, --device mcu  device to be programmed
-  -h, --help            print this message and exit
+  -c programmer           type of programmer
+  -d mcu, --device mcu    device to be programmed
+  --version               print version number and exit
+  -h, --help              print this message and exit
 
 actions:
   -r, --read addr [len]   read bytes from specified address
   -w, --write addr word   write word to specified address
   -f, --flash             flash hexfile onto the device
   -e, --erase [addr]      erase device or specified address
   -v, --verify            verify device memory
@@ -81,10 +82,10 @@
 **Github:** https://github.com/rex--/picchick
 
 **PyPi:** https://pypi.org/project/picchick/
 
 
 ## Copying
 
-Copyright (C) 2022 Rex McKinnon \
+Copyright (C) 2022-2024 Rex McKinnon \
 This software is released under the University of Illinois/NCSA
 Open Source License. Check the LICENSE file for more details.
```

### Comparing `picchick-0.4.0/picchick/cli.py` & `picchick-0.4.1/picchick/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,27 +211,30 @@
             # And further group the rows into pages
             hexobj.page_rows(page_size=dev.page_size)
             success_blocks = 0
             print(f"Starting write of flash...")
             for address, block in hexobj.pages.items():
                 if dev.write(address, block):
                     success_blocks += 1
-            print(f"Successfully wrote  bytes in {success_blocks} chunks.")
+            print(f"Successfully wrote {success_blocks*dev.page_size} bytes in {success_blocks} chunks.")
 
             for address, word in hexobj.config.items():
                 dev.write(address, programmer.INTBYTES(word))
         elif args.write:
-            dev.write(int(args.write[0], base=16), bytes.fromhex(args.write[1]))
+            dev.write(int(args.write[0], 0), int(args.write[1]).to_bytes(2, 'big'))
             # dev.word(int(args.write[0], base=16), int(args.write[1], base=16))
         
         if args.read:
             if (len(args.read) < 2):
                 args.read.extend('1')
             read_resp = dev.read(int(args.read[0], base=16), int(args.read[1]))
-            print(read_resp.hex(' ', -2))
+            if read_resp is not None:
+                print(read_resp.hex(' ', -2))
+            else:
+                fail = True
         
         if args.verify:
             print('Verifying memory...')
             fail = False
 
             # If we have loaded the hexfile verify against that
             if hexfile_reqd:
```

### Comparing `picchick-0.4.0/picchick/devices.py` & `picchick-0.4.1/picchick/devices.py`

 * *Files identical despite different names*

### Comparing `picchick-0.4.0/picchick/hexfile.py` & `picchick-0.4.1/picchick/hexfile.py`

 * *Files identical despite different names*

### Comparing `picchick-0.4.0/picchick/programmer/flipflop.py` & `picchick-0.4.1/picchick/programmer/flipflop.py`

 * *Files identical despite different names*

### Comparing `picchick-0.4.0/picchick/programmer/picstick.py` & `picchick-0.4.1/picchick/programmer/picstick.py`

 * *Files identical despite different names*

### Comparing `picchick-0.4.0/picchick/programmer/programmer.py` & `picchick-0.4.1/picchick/programmer/programmer.py`

 * *Files identical despite different names*

### Comparing `picchick-0.4.0/picchick.egg-info/PKG-INFO` & `picchick-0.4.1/picchick.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: picchick
-Version: 0.4.0
+Version: 0.4.1
 Summary: A utility for programming and debugging microcontrollers.
 Home-page: https://github.com/rex--/picchick
 Author: Rex McKinnon
 Author-email: 0xff@rexploits.com
 License: University of Illinois/NCSA Open Source License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: University of Illinois/NCSA Open Source License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyserial
 
 # picchick
 `picchick` is a command-line utility used for programming and debugging
 microcontrollers.
 
 The function is the same as `avrdude`, i.e. to provide a way to flash a compiled
 .hex file onto a microcontroller.
@@ -66,20 +67,21 @@
 $ picchick -h
 usage: picchick [-d <mcu>] [-c <programmer>] [-r <addr> [len] | -w <addr> <word> | -f] [-e [addr]] [-v] [hexfile]
        picchick [-d <mcu>] [--map | --list-ports] [hexfile]
 
 A utility for programming and debugging microcontrollers.
 
 positional arguments:
-  hexfile               path to a hexfile
+  hexfile                 path to a hexfile
 
 options:
-  -c programmer         type of programmer
-  -d mcu, --device mcu  device to be programmed
-  -h, --help            print this message and exit
+  -c programmer           type of programmer
+  -d mcu, --device mcu    device to be programmed
+  --version               print version number and exit
+  -h, --help              print this message and exit
 
 actions:
   -r, --read addr [len]   read bytes from specified address
   -w, --write addr word   write word to specified address
   -f, --flash             flash hexfile onto the device
   -e, --erase [addr]      erase device or specified address
   -v, --verify            verify device memory
@@ -95,10 +97,10 @@
 **Github:** https://github.com/rex--/picchick
 
 **PyPi:** https://pypi.org/project/picchick/
 
 
 ## Copying
 
-Copyright (C) 2022 Rex McKinnon \
+Copyright (C) 2022-2024 Rex McKinnon \
 This software is released under the University of Illinois/NCSA
 Open Source License. Check the LICENSE file for more details.
```

### Comparing `picchick-0.4.0/setup.cfg` & `picchick-0.4.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = picchick
-version = 0.4.0
+version = 0.4.1
 author = Rex McKinnon
 author_email = 0xff@rexploits.com
 description = A utility for programming and debugging microcontrollers.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/rex--/picchick
 license = University of Illinois/NCSA Open Source License
```


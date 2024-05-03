# Comparing `tmp/pyspacemouse-1.1.2.tar.gz` & `tmp/pyspacemouse-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspacemouse-1.1.2.tar", last modified: Sat Apr 20 20:22:33 2024, max compression
+gzip compressed data, was "pyspacemouse-1.1.3.tar", last modified: Fri May  3 08:47:38 2024, max compression
```

## Comparing `pyspacemouse-1.1.2.tar` & `pyspacemouse-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-20 20:22:33.871932 pyspacemouse-1.1.2/
--rw-r--r--   0 kuba       (501) staff       (20)     1108 2022-09-26 12:42:07.000000 pyspacemouse-1.1.2/LICENSE
--rw-r--r--   0 kuba       (501) staff       (20)     8148 2024-04-20 20:22:33.871699 pyspacemouse-1.1.2/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     6950 2024-04-20 20:09:14.000000 pyspacemouse-1.1.2/README.md
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-20 20:22:33.867685 pyspacemouse-1.1.2/pyspacemouse/
--rw-r--r--   0 kuba       (501) staff       (20)       27 2024-02-09 17:06:41.000000 pyspacemouse-1.1.2/pyspacemouse/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)    41586 2024-02-09 17:11:27.000000 pyspacemouse-1.1.2/pyspacemouse/pyspacemouse.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-20 20:22:33.870833 pyspacemouse-1.1.2/pyspacemouse.egg-info/
--rw-r--r--   0 kuba       (501) staff       (20)     8148 2024-04-20 20:22:33.000000 pyspacemouse-1.1.2/pyspacemouse.egg-info/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)      411 2024-04-20 20:22:33.000000 pyspacemouse-1.1.2/pyspacemouse.egg-info/SOURCES.txt
--rw-r--r--   0 kuba       (501) staff       (20)        1 2024-04-20 20:22:33.000000 pyspacemouse-1.1.2/pyspacemouse.egg-info/dependency_links.txt
--rw-r--r--   0 kuba       (501) staff       (20)        1 2022-10-15 23:04:25.000000 pyspacemouse-1.1.2/pyspacemouse.egg-info/not-zip-safe
--rw-r--r--   0 kuba       (501) staff       (20)      148 2024-04-20 20:22:33.000000 pyspacemouse-1.1.2/pyspacemouse.egg-info/requires.txt
--rw-r--r--   0 kuba       (501) staff       (20)       13 2024-04-20 20:22:33.000000 pyspacemouse-1.1.2/pyspacemouse.egg-info/top_level.txt
--rw-r--r--   0 kuba       (501) staff       (20)       38 2024-04-20 20:22:33.871978 pyspacemouse-1.1.2/setup.cfg
--rw-r--r--   0 kuba       (501) staff       (20)     1479 2024-04-20 20:21:15.000000 pyspacemouse-1.1.2/setup.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-20 20:22:33.870559 pyspacemouse-1.1.2/tests/
--rw-r--r--   0 kuba       (501) staff       (20)     2111 2022-09-26 12:42:07.000000 pyspacemouse-1.1.2/tests/test_callbacks_arr.py
--rw-r--r--   0 kuba       (501) staff       (20)      904 2022-09-26 12:42:07.000000 pyspacemouse-1.1.2/tests/test_clb_axis_arr.py
--rw-r--r--   0 kuba       (501) staff       (20)      273 2022-09-26 12:42:07.000000 pyspacemouse-1.1.2/tests/test_config.py
--rw-r--r--   0 kuba       (501) staff       (20)     5537 2023-01-24 23:02:11.000000 pyspacemouse-1.1.2/tests/test_mouse.py
--rw-r--r--   0 kuba       (501) staff       (20)     1969 2023-01-24 23:02:11.000000 pyspacemouse-1.1.2/tests/test_readme.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-03 08:47:38.250323 pyspacemouse-1.1.3/
+-rw-r--r--   0 kuba       (501) staff       (20)     1108 2022-09-26 12:42:07.000000 pyspacemouse-1.1.3/LICENSE
+-rw-r--r--   0 kuba       (501) staff       (20)     8931 2024-05-03 08:47:38.249852 pyspacemouse-1.1.3/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     7733 2024-05-03 08:44:34.000000 pyspacemouse-1.1.3/README.md
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-03 08:47:38.246095 pyspacemouse-1.1.3/pyspacemouse/
+-rw-r--r--   0 kuba       (501) staff       (20)       27 2024-05-02 22:19:46.000000 pyspacemouse-1.1.3/pyspacemouse/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)    42519 2024-05-03 08:41:33.000000 pyspacemouse-1.1.3/pyspacemouse/pyspacemouse.py
+-rw-r--r--   0 kuba       (501) staff       (20)     3332 2024-05-03 08:41:24.000000 pyspacemouse-1.1.3/pyspacemouse/pyspacemouse_cli.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-03 08:47:38.249222 pyspacemouse-1.1.3/pyspacemouse.egg-info/
+-rw-r--r--   0 kuba       (501) staff       (20)     8931 2024-05-03 08:47:38.000000 pyspacemouse-1.1.3/pyspacemouse.egg-info/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)      483 2024-05-03 08:47:38.000000 pyspacemouse-1.1.3/pyspacemouse.egg-info/SOURCES.txt
+-rw-r--r--   0 kuba       (501) staff       (20)        1 2024-05-03 08:47:38.000000 pyspacemouse-1.1.3/pyspacemouse.egg-info/dependency_links.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       68 2024-05-03 08:47:38.000000 pyspacemouse-1.1.3/pyspacemouse.egg-info/entry_points.txt
+-rw-r--r--   0 kuba       (501) staff       (20)        1 2022-10-15 23:04:25.000000 pyspacemouse-1.1.3/pyspacemouse.egg-info/not-zip-safe
+-rw-r--r--   0 kuba       (501) staff       (20)      148 2024-05-03 08:47:38.000000 pyspacemouse-1.1.3/pyspacemouse.egg-info/requires.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       13 2024-05-03 08:47:38.000000 pyspacemouse-1.1.3/pyspacemouse.egg-info/top_level.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       38 2024-05-03 08:47:38.250387 pyspacemouse-1.1.3/setup.cfg
+-rw-r--r--   0 kuba       (501) staff       (20)     1617 2024-05-03 08:46:52.000000 pyspacemouse-1.1.3/setup.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-03 08:47:38.248895 pyspacemouse-1.1.3/tests/
+-rw-r--r--   0 kuba       (501) staff       (20)     2111 2022-09-26 12:42:07.000000 pyspacemouse-1.1.3/tests/test_callbacks_arr.py
+-rw-r--r--   0 kuba       (501) staff       (20)      904 2022-09-26 12:42:07.000000 pyspacemouse-1.1.3/tests/test_clb_axis_arr.py
+-rw-r--r--   0 kuba       (501) staff       (20)      273 2022-09-26 12:42:07.000000 pyspacemouse-1.1.3/tests/test_config.py
+-rw-r--r--   0 kuba       (501) staff       (20)     5537 2023-01-24 23:02:11.000000 pyspacemouse-1.1.3/tests/test_mouse.py
+-rw-r--r--   0 kuba       (501) staff       (20)     1969 2023-01-24 23:02:11.000000 pyspacemouse-1.1.3/tests/test_readme.py
```

### Comparing `pyspacemouse-1.1.2/LICENSE` & `pyspacemouse-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspacemouse-1.1.2/PKG-INFO` & `pyspacemouse-1.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspacemouse
-Version: 1.1.2
+Version: 1.1.3
 Summary: Multiplatform Python interface to the 3DConnexion Space Mouse - forked from pyspacenavigator
 Home-page: https://github.com/JakubAndrysek/pyspacemouse
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Keywords: pyspacemouse,3d,6 DoF,HID,python,open-source,spacemouse,spacenavigator,3dconnection,3d-mouse
 Classifier: License :: OSI Approved :: MIT License
@@ -102,14 +102,15 @@
             </pre>
             </details>
 
     - ### Windows
         - Install the latest release of hidapi.dll and hidapi.lib from
           the [hidapi releases](https://github.com/libusb/hidapi/releases) page.
         - Set system environment: add absolute path for `x64` or `x86` folder in Path.
+        - More info on [Troubleshooting - WIndows](./troubleshooting.md#windows) page.
 
     - ### Mac OS X (M1)
         - Install from [Homebrew](https://formulae.brew.sh/formula/hidapi)
         - `brew install hidapi`
         - Add hidapi to your `DYLD_LIBRARY_PATH` directory.
             ```bash
             export DYLD_LIBRARY_PATH=/opt/homebrew/Cellar/hidapi/0.14.0/lib:$DYLD_LIBRARY_PATH
@@ -117,15 +118,15 @@
         - On MacOS M1 you will need patched version of easyhid. If easyhid is already installed, please uninstall it first.
             ```bash
             pip install git+https://github.com/bglopez/python-easyhid.git
             ```
         - In case of problem with M1 chip, try to run you code with Rosseta 2
             - How to use Rosseta 2 - [Setup Rosetta](https://apple.stackexchange.com/questions/428768/on-apple-m1-with-rosetta-how-to-open-entire-terminal-iterm-in-x86-64-architec)
         - Tested and developed by [consi](https://github.com/JakubAndrysek/PySpaceMouse/issues/10#issuecomment-1768362007) - thanks!
-        - More info in [Troubleshooting - Mac OS (M1)](./troubleshooting.md#mac-os-m1) page.
+        - More info on [Troubleshooting - Mac OS (M1)](./troubleshooting.md#mac-os-m1) page.
 
 - ### [easyhid](https://github.com/bglopez/python-easyhid) is `hidapi` interface for Python - required on all platforms
     - `pip install git+https://github.com/bglopez/python-easyhid.git`
     - this fork fix problems with `hidapi` on MacOS.
     - on other platforms it possible works with original package `pip install easyhid`
 
 ## Basic Usage:
@@ -144,14 +145,35 @@
 if success:
     while 1:
         state = pyspacemouse.read()
         time.sleep(0.01)
 ````
 More examples can be found in the [/examples](https://github.com/JakubAndrysek/PySpaceMouse/tree/master/examples) directory or in page with [Examples](https://spacemouse.kubaandrysek.cz/mouseApi/examples/).
 
+## Available CLI test commands
+```bash
+usage: pyspacemouse [-h] [--version] [--list-spacemouse]
+                    [--list-supported-devices] [--list-all-hid-devices]
+                    [--test-connect]
+
+PySpaceMouse CLI
+
+options:
+  -h, --help            show this help message and exit
+  --version             Version of pyspacemouse
+  --list-spacemouse     List connected SpaceMouse devices
+  --list-supported-devices
+                        List supported SpaceMouse devices
+  --list-all-hid-devices
+                        List all connected HID devices
+  --test-connect        Test connect to the first available device
+
+For more information, visit https://spacemouse.kubaandrysek.cz
+```
+
 
 ## Troubleshooting
 
 Look at the [Troubleshooting](./troubleshooting.md) page for help with common issues.
 
 ## References
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyspacemouse Version: 1.1.2 Summary: Multiplatform
+Metadata-Version: 2.1 Name: pyspacemouse Version: 1.1.3 Summary: Multiplatform
 Python interface to the 3DConnexion Space Mouse - forked from pyspacenavigator
 Home-page: https://github.com/JakubAndrysek/pyspacemouse Author: Jakub
 AndrÃ½sek Author-email: email@kubaandrysek.cz License: MIT Keywords:
 pyspacemouse,3d,6 DoF,HID,python,open-
 source,spacemouse,spacenavigator,3dconnection,3d-mouse Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
@@ -54,40 +54,48 @@
 Aleternative option - with tee (RPi)
             echo 'KERNEL=="hidraw*", SUBSYSTEM=="hidraw", MODE="0664",
 GROUP="plugdev"' | sudo tee /etc/udev/rules.d/99-hidraw-permissions.rules
             sudo usermod -aG plugdev $USER
             newgrp plugdev
 - ### Windows - Install the latest release of hidapi.dll and hidapi.lib from
 the [hidapi releases](https://github.com/libusb/hidapi/releases) page. - Set
-system environment: add absolute path for `x64` or `x86` folder in Path. - ###
+system environment: add absolute path for `x64` or `x86` folder in Path. - More
+info on [Troubleshooting - WIndows](./troubleshooting.md#windows) page. - ###
 Mac OS X (M1) - Install from [Homebrew](https://formulae.brew.sh/formula/
 hidapi) - `brew install hidapi` - Add hidapi to your `DYLD_LIBRARY_PATH`
 directory. ```bash export DYLD_LIBRARY_PATH=/opt/homebrew/Cellar/hidapi/0.14.0/
 lib:$DYLD_LIBRARY_PATH ``` - On MacOS M1 you will need patched version of
 easyhid. If easyhid is already installed, please uninstall it first. ```bash
 pip install git+https://github.com/bglopez/python-easyhid.git ``` - In case of
 problem with M1 chip, try to run you code with Rosseta 2 - How to use Rosseta 2
 - [Setup Rosetta](https://apple.stackexchange.com/questions/428768/on-apple-m1-
 with-rosetta-how-to-open-entire-terminal-iterm-in-x86-64-architec) - Tested and
 developed by [consi](https://github.com/JakubAndrysek/PySpaceMouse/issues/
-10#issuecomment-1768362007) - thanks! - More info in [Troubleshooting - Mac OS
+10#issuecomment-1768362007) - thanks! - More info on [Troubleshooting - Mac OS
 (M1)](./troubleshooting.md#mac-os-m1) page. - ### [easyhid](https://github.com/
 bglopez/python-easyhid) is `hidapi` interface for Python - required on all
 platforms - `pip install git+https://github.com/bglopez/python-easyhid.git` -
 this fork fix problems with `hidapi` on MacOS. - on other platforms it possible
 works with original package `pip install easyhid` ## Basic Usage: If the
 3Dconnexion driver is installed, please ensure to stop `3DconnexionHelper`
 before running your python scripts. ## Basic example ````py import pyspacemouse
 import time success = pyspacemouse.open(dof_callback=pyspacemouse.print_state,
 button_callback=pyspacemouse.print_buttons) if success: while 1: state =
 pyspacemouse.read() time.sleep(0.01) ```` More examples can be found in the [/
 examples](https://github.com/JakubAndrysek/PySpaceMouse/tree/master/examples)
 directory or in page with [Examples](https://spacemouse.kubaandrysek.cz/
-mouseApi/examples/). ## Troubleshooting Look at the [Troubleshooting](./
-troubleshooting.md) page for help with common issues. ## References
+mouseApi/examples/). ## Available CLI test commands ```bash usage: pyspacemouse
+[-h] [--version] [--list-spacemouse] [--list-supported-devices] [--list-all-
+hid-devices] [--test-connect] PySpaceMouse CLI options: -h, --help show this
+help message and exit --version Version of pyspacemouse --list-spacemouse List
+connected SpaceMouse devices --list-supported-devices List supported SpaceMouse
+devices --list-all-hid-devices List all connected HID devices --test-connect
+Test connect to the first available device For more information, visit https://
+spacemouse.kubaandrysek.cz ``` ## Troubleshooting Look at the [Troubleshooting]
+(./troubleshooting.md) page for help with common issues. ## References
 PySpaceMouse is used in the following projects: - [PySpaceApp](https://
 github.com/JakubAndrysek/pyspaceapp) - Control your PC with SpaceMouse (basic
 hotkeys, mouse control, and more) - [TeleMoMa](https://github.com/UT-Austin-
 RobIn/telemoma) - A Modular and Versatile Teleoperation System for Mobile
 Manipulation - [SERL](https://github.com/rail-berkeley/serl) - SERL: A Software
 Suite for Sample-Efficient Robotic Reinforcement Learning - ![](https://
 github.com/rail-berkeley/serl/raw/e59dc0d2721399af2e629d7bcad678fa2ffce9ae/
```

### Comparing `pyspacemouse-1.1.2/README.md` & `pyspacemouse-1.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -74,14 +74,15 @@
             </pre>
             </details>
 
     - ### Windows
         - Install the latest release of hidapi.dll and hidapi.lib from
           the [hidapi releases](https://github.com/libusb/hidapi/releases) page.
         - Set system environment: add absolute path for `x64` or `x86` folder in Path.
+        - More info on [Troubleshooting - WIndows](./troubleshooting.md#windows) page.
 
     - ### Mac OS X (M1)
         - Install from [Homebrew](https://formulae.brew.sh/formula/hidapi)
         - `brew install hidapi`
         - Add hidapi to your `DYLD_LIBRARY_PATH` directory.
             ```bash
             export DYLD_LIBRARY_PATH=/opt/homebrew/Cellar/hidapi/0.14.0/lib:$DYLD_LIBRARY_PATH
@@ -89,15 +90,15 @@
         - On MacOS M1 you will need patched version of easyhid. If easyhid is already installed, please uninstall it first.
             ```bash
             pip install git+https://github.com/bglopez/python-easyhid.git
             ```
         - In case of problem with M1 chip, try to run you code with Rosseta 2
             - How to use Rosseta 2 - [Setup Rosetta](https://apple.stackexchange.com/questions/428768/on-apple-m1-with-rosetta-how-to-open-entire-terminal-iterm-in-x86-64-architec)
         - Tested and developed by [consi](https://github.com/JakubAndrysek/PySpaceMouse/issues/10#issuecomment-1768362007) - thanks!
-        - More info in [Troubleshooting - Mac OS (M1)](./troubleshooting.md#mac-os-m1) page.
+        - More info on [Troubleshooting - Mac OS (M1)](./troubleshooting.md#mac-os-m1) page.
 
 - ### [easyhid](https://github.com/bglopez/python-easyhid) is `hidapi` interface for Python - required on all platforms
     - `pip install git+https://github.com/bglopez/python-easyhid.git`
     - this fork fix problems with `hidapi` on MacOS.
     - on other platforms it possible works with original package `pip install easyhid`
 
 ## Basic Usage:
@@ -116,14 +117,35 @@
 if success:
     while 1:
         state = pyspacemouse.read()
         time.sleep(0.01)
 ````
 More examples can be found in the [/examples](https://github.com/JakubAndrysek/PySpaceMouse/tree/master/examples) directory or in page with [Examples](https://spacemouse.kubaandrysek.cz/mouseApi/examples/).
 
+## Available CLI test commands
+```bash
+usage: pyspacemouse [-h] [--version] [--list-spacemouse]
+                    [--list-supported-devices] [--list-all-hid-devices]
+                    [--test-connect]
+
+PySpaceMouse CLI
+
+options:
+  -h, --help            show this help message and exit
+  --version             Version of pyspacemouse
+  --list-spacemouse     List connected SpaceMouse devices
+  --list-supported-devices
+                        List supported SpaceMouse devices
+  --list-all-hid-devices
+                        List all connected HID devices
+  --test-connect        Test connect to the first available device
+
+For more information, visit https://spacemouse.kubaandrysek.cz
+```
+
 
 ## Troubleshooting
 
 Look at the [Troubleshooting](./troubleshooting.md) page for help with common issues.
 
 ## References
```

#### html2text {}

```diff
@@ -38,40 +38,48 @@
 Aleternative option - with tee (RPi)
             echo 'KERNEL=="hidraw*", SUBSYSTEM=="hidraw", MODE="0664",
 GROUP="plugdev"' | sudo tee /etc/udev/rules.d/99-hidraw-permissions.rules
             sudo usermod -aG plugdev $USER
             newgrp plugdev
 - ### Windows - Install the latest release of hidapi.dll and hidapi.lib from
 the [hidapi releases](https://github.com/libusb/hidapi/releases) page. - Set
-system environment: add absolute path for `x64` or `x86` folder in Path. - ###
+system environment: add absolute path for `x64` or `x86` folder in Path. - More
+info on [Troubleshooting - WIndows](./troubleshooting.md#windows) page. - ###
 Mac OS X (M1) - Install from [Homebrew](https://formulae.brew.sh/formula/
 hidapi) - `brew install hidapi` - Add hidapi to your `DYLD_LIBRARY_PATH`
 directory. ```bash export DYLD_LIBRARY_PATH=/opt/homebrew/Cellar/hidapi/0.14.0/
 lib:$DYLD_LIBRARY_PATH ``` - On MacOS M1 you will need patched version of
 easyhid. If easyhid is already installed, please uninstall it first. ```bash
 pip install git+https://github.com/bglopez/python-easyhid.git ``` - In case of
 problem with M1 chip, try to run you code with Rosseta 2 - How to use Rosseta 2
 - [Setup Rosetta](https://apple.stackexchange.com/questions/428768/on-apple-m1-
 with-rosetta-how-to-open-entire-terminal-iterm-in-x86-64-architec) - Tested and
 developed by [consi](https://github.com/JakubAndrysek/PySpaceMouse/issues/
-10#issuecomment-1768362007) - thanks! - More info in [Troubleshooting - Mac OS
+10#issuecomment-1768362007) - thanks! - More info on [Troubleshooting - Mac OS
 (M1)](./troubleshooting.md#mac-os-m1) page. - ### [easyhid](https://github.com/
 bglopez/python-easyhid) is `hidapi` interface for Python - required on all
 platforms - `pip install git+https://github.com/bglopez/python-easyhid.git` -
 this fork fix problems with `hidapi` on MacOS. - on other platforms it possible
 works with original package `pip install easyhid` ## Basic Usage: If the
 3Dconnexion driver is installed, please ensure to stop `3DconnexionHelper`
 before running your python scripts. ## Basic example ````py import pyspacemouse
 import time success = pyspacemouse.open(dof_callback=pyspacemouse.print_state,
 button_callback=pyspacemouse.print_buttons) if success: while 1: state =
 pyspacemouse.read() time.sleep(0.01) ```` More examples can be found in the [/
 examples](https://github.com/JakubAndrysek/PySpaceMouse/tree/master/examples)
 directory or in page with [Examples](https://spacemouse.kubaandrysek.cz/
-mouseApi/examples/). ## Troubleshooting Look at the [Troubleshooting](./
-troubleshooting.md) page for help with common issues. ## References
+mouseApi/examples/). ## Available CLI test commands ```bash usage: pyspacemouse
+[-h] [--version] [--list-spacemouse] [--list-supported-devices] [--list-all-
+hid-devices] [--test-connect] PySpaceMouse CLI options: -h, --help show this
+help message and exit --version Version of pyspacemouse --list-spacemouse List
+connected SpaceMouse devices --list-supported-devices List supported SpaceMouse
+devices --list-all-hid-devices List all connected HID devices --test-connect
+Test connect to the first available device For more information, visit https://
+spacemouse.kubaandrysek.cz ``` ## Troubleshooting Look at the [Troubleshooting]
+(./troubleshooting.md) page for help with common issues. ## References
 PySpaceMouse is used in the following projects: - [PySpaceApp](https://
 github.com/JakubAndrysek/pyspaceapp) - Control your PC with SpaceMouse (basic
 hotkeys, mouse control, and more) - [TeleMoMa](https://github.com/UT-Austin-
 RobIn/telemoma) - A Modular and Versatile Teleoperation System for Mobile
 Manipulation - [SERL](https://github.com/rail-berkeley/serl) - SERL: A Software
 Suite for Sample-Efficient Robotic Reinforcement Learning - ![](https://
 github.com/rail-berkeley/serl/raw/e59dc0d2721399af2e629d7bcad678fa2ffce9ae/
```

### Comparing `pyspacemouse-1.1.2/pyspacemouse/pyspacemouse.py` & `pyspacemouse-1.1.3/pyspacemouse/pyspacemouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,15 +376,15 @@
             # ButtonSpec(channel=3, byte=5, bit=1),
             # ButtonSpec(channel=3, byte=5, bit=2),
             # ButtonSpec(channel=3, byte=5, bit=3),
             # ButtonSpec(channel=3, byte=5, bit=4),
             # ButtonSpec(channel=3, byte=5, bit=5),
             # ButtonSpec(channel=3, byte=5, bit=6),
             # ButtonSpec(channel=3, byte=5, bit=7),
-        
+
             ButtonSpec(channel=3, byte=2, bit=4), # 1
             ButtonSpec(channel=3, byte=2, bit=5), # 2
             ButtonSpec(channel=3, byte=2, bit=6), # 3
             ButtonSpec(channel=3, byte=2, bit=7), # 4
 
             ButtonSpec(channel=3, byte=3, bit=0), # 5
             ButtonSpec(channel=3, byte=3, bit=1), # 6
@@ -404,15 +404,15 @@
             ButtonSpec(channel=3, byte=3, bit=6), # ESC
             ButtonSpec(channel=3, byte=3, bit=7), # ALT
 
             ButtonSpec(channel=3, byte=4, bit=0), # SHIFT
             ButtonSpec(channel=3, byte=4, bit=1), # CTRL
             ButtonSpec(channel=3, byte=4, bit=2), # LOCK
 
-            
+
 
         ],
         axis_scale=350.0,
     ),
     "SpaceExplorer": DeviceSpec(
         name="SpaceExplorer",
         # vendor ID and product ID
@@ -752,15 +752,16 @@
         A list of string names of the devices supported which were found. Empty if no supported devices found
     """
     devices = []
     try:
         hid = Enumeration()
     except AttributeError as e:
         raise Exception(
-            "HID API is probably not installed. See README.md for details."
+            "HID API is probably not installed. "
+            "Look at https://spacemouse.kubaandrysek.cz for details."
         ) from e
 
     all_hids = hid.find()
 
     if all_hids:
         for device in all_hids:
             devices.extend(
@@ -769,14 +770,43 @@
                 if (
                     device.vendor_id == spec.hid_id[0]
                     and device.product_id == spec.hid_id[1]
                 )
             )
     return devices
 
+def list_available_devices():
+    """Return a list of all supported devices from config
+
+    Returns:
+        A list of string names of the devices supported (device_name, vid_id, pid_id)
+    """
+    return [
+        (device_name, spec.hid_id[0], spec.hid_id[1])
+        for device_name, spec in device_specs.items()
+    ]
+
+def list_all_hid_devices():
+    """Return a list of all HID devices connected
+
+    Returns:
+        A list of HID devices (product_string, manufacturer_string, vendor_id, product_id)
+    """
+    try:
+        hid = Enumeration()
+    except AttributeError as e:
+        raise Exception(
+            "HID API is probably not installed."
+            "Look at https://spacemouse.kubaandrysek.cz for details."
+        ) from e
+
+    return [
+        (device.product_string, device.manufacturer_string, device.vendor_id, device.product_id)
+        for device in hid.find()
+    ]
 
 def openCfg(config: Config, set_nonblocking_loop: bool = True, device=None, DeviceNumber=0):
     """
     Open a 3D space navigator device. Same as open() but input one config file -> class Config
 
     Returns:
         Device object if the device was opened successfully
@@ -820,15 +850,15 @@
 
     # if no device name specified, look for any matching device and choose the first
     if device is None:
         all_devices = list_devices()
         if len(all_devices) > 0:
             device = all_devices[0]
         else:
-            raise Exception("No device connected/supported!")
+            raise Exception("No found any connected or supported devices.")
 
     found_devices = []
     hid = Enumeration()
     all_hids = hid.find()
     if all_hids:
         for dev in all_hids:
             if path:
```

### Comparing `pyspacemouse-1.1.2/pyspacemouse.egg-info/PKG-INFO` & `pyspacemouse-1.1.3/pyspacemouse.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspacemouse
-Version: 1.1.2
+Version: 1.1.3
 Summary: Multiplatform Python interface to the 3DConnexion Space Mouse - forked from pyspacenavigator
 Home-page: https://github.com/JakubAndrysek/pyspacemouse
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Keywords: pyspacemouse,3d,6 DoF,HID,python,open-source,spacemouse,spacenavigator,3dconnection,3d-mouse
 Classifier: License :: OSI Approved :: MIT License
@@ -102,14 +102,15 @@
             </pre>
             </details>
 
     - ### Windows
         - Install the latest release of hidapi.dll and hidapi.lib from
           the [hidapi releases](https://github.com/libusb/hidapi/releases) page.
         - Set system environment: add absolute path for `x64` or `x86` folder in Path.
+        - More info on [Troubleshooting - WIndows](./troubleshooting.md#windows) page.
 
     - ### Mac OS X (M1)
         - Install from [Homebrew](https://formulae.brew.sh/formula/hidapi)
         - `brew install hidapi`
         - Add hidapi to your `DYLD_LIBRARY_PATH` directory.
             ```bash
             export DYLD_LIBRARY_PATH=/opt/homebrew/Cellar/hidapi/0.14.0/lib:$DYLD_LIBRARY_PATH
@@ -117,15 +118,15 @@
         - On MacOS M1 you will need patched version of easyhid. If easyhid is already installed, please uninstall it first.
             ```bash
             pip install git+https://github.com/bglopez/python-easyhid.git
             ```
         - In case of problem with M1 chip, try to run you code with Rosseta 2
             - How to use Rosseta 2 - [Setup Rosetta](https://apple.stackexchange.com/questions/428768/on-apple-m1-with-rosetta-how-to-open-entire-terminal-iterm-in-x86-64-architec)
         - Tested and developed by [consi](https://github.com/JakubAndrysek/PySpaceMouse/issues/10#issuecomment-1768362007) - thanks!
-        - More info in [Troubleshooting - Mac OS (M1)](./troubleshooting.md#mac-os-m1) page.
+        - More info on [Troubleshooting - Mac OS (M1)](./troubleshooting.md#mac-os-m1) page.
 
 - ### [easyhid](https://github.com/bglopez/python-easyhid) is `hidapi` interface for Python - required on all platforms
     - `pip install git+https://github.com/bglopez/python-easyhid.git`
     - this fork fix problems with `hidapi` on MacOS.
     - on other platforms it possible works with original package `pip install easyhid`
 
 ## Basic Usage:
@@ -144,14 +145,35 @@
 if success:
     while 1:
         state = pyspacemouse.read()
         time.sleep(0.01)
 ````
 More examples can be found in the [/examples](https://github.com/JakubAndrysek/PySpaceMouse/tree/master/examples) directory or in page with [Examples](https://spacemouse.kubaandrysek.cz/mouseApi/examples/).
 
+## Available CLI test commands
+```bash
+usage: pyspacemouse [-h] [--version] [--list-spacemouse]
+                    [--list-supported-devices] [--list-all-hid-devices]
+                    [--test-connect]
+
+PySpaceMouse CLI
+
+options:
+  -h, --help            show this help message and exit
+  --version             Version of pyspacemouse
+  --list-spacemouse     List connected SpaceMouse devices
+  --list-supported-devices
+                        List supported SpaceMouse devices
+  --list-all-hid-devices
+                        List all connected HID devices
+  --test-connect        Test connect to the first available device
+
+For more information, visit https://spacemouse.kubaandrysek.cz
+```
+
 
 ## Troubleshooting
 
 Look at the [Troubleshooting](./troubleshooting.md) page for help with common issues.
 
 ## References
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyspacemouse Version: 1.1.2 Summary: Multiplatform
+Metadata-Version: 2.1 Name: pyspacemouse Version: 1.1.3 Summary: Multiplatform
 Python interface to the 3DConnexion Space Mouse - forked from pyspacenavigator
 Home-page: https://github.com/JakubAndrysek/pyspacemouse Author: Jakub
 AndrÃ½sek Author-email: email@kubaandrysek.cz License: MIT Keywords:
 pyspacemouse,3d,6 DoF,HID,python,open-
 source,spacemouse,spacenavigator,3dconnection,3d-mouse Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
@@ -54,40 +54,48 @@
 Aleternative option - with tee (RPi)
             echo 'KERNEL=="hidraw*", SUBSYSTEM=="hidraw", MODE="0664",
 GROUP="plugdev"' | sudo tee /etc/udev/rules.d/99-hidraw-permissions.rules
             sudo usermod -aG plugdev $USER
             newgrp plugdev
 - ### Windows - Install the latest release of hidapi.dll and hidapi.lib from
 the [hidapi releases](https://github.com/libusb/hidapi/releases) page. - Set
-system environment: add absolute path for `x64` or `x86` folder in Path. - ###
+system environment: add absolute path for `x64` or `x86` folder in Path. - More
+info on [Troubleshooting - WIndows](./troubleshooting.md#windows) page. - ###
 Mac OS X (M1) - Install from [Homebrew](https://formulae.brew.sh/formula/
 hidapi) - `brew install hidapi` - Add hidapi to your `DYLD_LIBRARY_PATH`
 directory. ```bash export DYLD_LIBRARY_PATH=/opt/homebrew/Cellar/hidapi/0.14.0/
 lib:$DYLD_LIBRARY_PATH ``` - On MacOS M1 you will need patched version of
 easyhid. If easyhid is already installed, please uninstall it first. ```bash
 pip install git+https://github.com/bglopez/python-easyhid.git ``` - In case of
 problem with M1 chip, try to run you code with Rosseta 2 - How to use Rosseta 2
 - [Setup Rosetta](https://apple.stackexchange.com/questions/428768/on-apple-m1-
 with-rosetta-how-to-open-entire-terminal-iterm-in-x86-64-architec) - Tested and
 developed by [consi](https://github.com/JakubAndrysek/PySpaceMouse/issues/
-10#issuecomment-1768362007) - thanks! - More info in [Troubleshooting - Mac OS
+10#issuecomment-1768362007) - thanks! - More info on [Troubleshooting - Mac OS
 (M1)](./troubleshooting.md#mac-os-m1) page. - ### [easyhid](https://github.com/
 bglopez/python-easyhid) is `hidapi` interface for Python - required on all
 platforms - `pip install git+https://github.com/bglopez/python-easyhid.git` -
 this fork fix problems with `hidapi` on MacOS. - on other platforms it possible
 works with original package `pip install easyhid` ## Basic Usage: If the
 3Dconnexion driver is installed, please ensure to stop `3DconnexionHelper`
 before running your python scripts. ## Basic example ````py import pyspacemouse
 import time success = pyspacemouse.open(dof_callback=pyspacemouse.print_state,
 button_callback=pyspacemouse.print_buttons) if success: while 1: state =
 pyspacemouse.read() time.sleep(0.01) ```` More examples can be found in the [/
 examples](https://github.com/JakubAndrysek/PySpaceMouse/tree/master/examples)
 directory or in page with [Examples](https://spacemouse.kubaandrysek.cz/
-mouseApi/examples/). ## Troubleshooting Look at the [Troubleshooting](./
-troubleshooting.md) page for help with common issues. ## References
+mouseApi/examples/). ## Available CLI test commands ```bash usage: pyspacemouse
+[-h] [--version] [--list-spacemouse] [--list-supported-devices] [--list-all-
+hid-devices] [--test-connect] PySpaceMouse CLI options: -h, --help show this
+help message and exit --version Version of pyspacemouse --list-spacemouse List
+connected SpaceMouse devices --list-supported-devices List supported SpaceMouse
+devices --list-all-hid-devices List all connected HID devices --test-connect
+Test connect to the first available device For more information, visit https://
+spacemouse.kubaandrysek.cz ``` ## Troubleshooting Look at the [Troubleshooting]
+(./troubleshooting.md) page for help with common issues. ## References
 PySpaceMouse is used in the following projects: - [PySpaceApp](https://
 github.com/JakubAndrysek/pyspaceapp) - Control your PC with SpaceMouse (basic
 hotkeys, mouse control, and more) - [TeleMoMa](https://github.com/UT-Austin-
 RobIn/telemoma) - A Modular and Versatile Teleoperation System for Mobile
 Manipulation - [SERL](https://github.com/rail-berkeley/serl) - SERL: A Software
 Suite for Sample-Efficient Robotic Reinforcement Learning - ![](https://
 github.com/rail-berkeley/serl/raw/e59dc0d2721399af2e629d7bcad678fa2ffce9ae/
```

### Comparing `pyspacemouse-1.1.2/setup.py` & `pyspacemouse-1.1.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,44 +6,49 @@
 
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 long_description = (HERE / "README.md").read_text()
 
 setuptools.setup(
-    name='pyspacemouse',
-    version='1.1.2',
-    author='Jakub Andrýsek',
-    author_email='email@kubaandrysek.cz',
-    description='Multiplatform Python interface to the 3DConnexion Space Mouse - forked from pyspacenavigator',
-    url='https://github.com/JakubAndrysek/pyspacemouse',
+    name="pyspacemouse",
+    version="1.1.3",
+    author="Jakub Andrýsek",
+    author_email="email@kubaandrysek.cz",
+    description="Multiplatform Python interface to the 3DConnexion Space Mouse - forked from pyspacenavigator",
+    url="https://github.com/JakubAndrysek/pyspacemouse",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    keywords='pyspacemouse, 3d, 6 DoF, HID, python, open-source, spacemouse, spacenavigator, 3dconnection, 3d-mouse',
-    license='MIT',
-    packages=['pyspacemouse'],
+    long_description_content_type="text/markdown",
+    keywords="pyspacemouse, 3d, 6 DoF, HID, python, open-source, spacemouse, spacenavigator, 3dconnection, 3d-mouse",
+    license="MIT",
+    packages=["pyspacemouse"],
     install_requires=[
         "easyhid",
     ],
     extras_require={
-        'develop': [
-            'mkdocs',
-            'mkdocs-material',
-            'mkdocs-glightbox',
-            'mkdocs-redirects',
-            'mkdoxy',
-            'mkdocs-open-in-new-tab',
-            'mkdocs-git-revision-date-localized-plugin'],
+        "develop": [
+            "mkdocs",
+            "mkdocs-material",
+            "mkdocs-glightbox",
+            "mkdocs-redirects",
+            "mkdoxy",
+            "mkdocs-open-in-new-tab",
+            "mkdocs-git-revision-date-localized-plugin",
+        ],
     },
-
     zip_safe=False,
     include_package_data=True,
     classifiers=[
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Operating System :: OS Independent',
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Operating System :: OS Independent",
     ],
     python_requires=">=3.8",
+    entry_points={
+        "console_scripts": [
+            "pyspacemouse=pyspacemouse.pyspacemouse_cli:main",
+        ],
+    },
 )
```

### Comparing `pyspacemouse-1.1.2/tests/test_callbacks_arr.py` & `pyspacemouse-1.1.3/tests/test_callbacks_arr.py`

 * *Files identical despite different names*

### Comparing `pyspacemouse-1.1.2/tests/test_clb_axis_arr.py` & `pyspacemouse-1.1.3/tests/test_clb_axis_arr.py`

 * *Files identical despite different names*

### Comparing `pyspacemouse-1.1.2/tests/test_mouse.py` & `pyspacemouse-1.1.3/tests/test_mouse.py`

 * *Files identical despite different names*

### Comparing `pyspacemouse-1.1.2/tests/test_readme.py` & `pyspacemouse-1.1.3/tests/test_readme.py`

 * *Files identical despite different names*


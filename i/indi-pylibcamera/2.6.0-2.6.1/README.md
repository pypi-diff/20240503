# Comparing `tmp/indi_pylibcamera-2.6.0.tar.gz` & `tmp/indi_pylibcamera-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indi_pylibcamera-2.6.0.tar", last modified: Thu Feb 29 07:31:00 2024, max compression
+gzip compressed data, was "indi_pylibcamera-2.6.1.tar", last modified: Fri May  3 11:09:10 2024, max compression
```

## Comparing `indi_pylibcamera-2.6.0.tar` & `indi_pylibcamera-2.6.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-02-29 07:31:00.872298 indi_pylibcamera-2.6.0/
--rw-r--r--   0 sbr       (1000) sbr       (1000)     1967 2024-02-29 06:41:25.000000 indi_pylibcamera-2.6.0/CHANGELOG
--rw-r--r--   0 sbr       (1000) sbr       (1000)     1074 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.0/LICENSE
--rw-r--r--   0 sbr       (1000) sbr       (1000)      187 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.0/MANIFEST.in
--rw-r--r--   0 sbr       (1000) sbr       (1000)    21487 2024-02-29 07:31:00.872298 indi_pylibcamera-2.6.0/PKG-INFO
--rw-r--r--   0 sbr       (1000) sbr       (1000)    18034 2024-02-27 18:59:44.000000 indi_pylibcamera-2.6.0/README.md
--rw-r--r--   0 sbr       (1000) sbr       (1000)       81 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.0/pyproject.toml
--rw-r--r--   0 sbr       (1000) sbr       (1000)      903 2024-02-29 07:31:00.872298 indi_pylibcamera-2.6.0/setup.cfg
--rw-r--r--   0 sbr       (1000) sbr       (1000)       40 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.0/setup.py
-drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-02-29 07:31:00.862298 indi_pylibcamera-2.6.0/src/
-drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-02-29 07:31:00.865631 indi_pylibcamera-2.6.0/src/indi_pylibcamera/
--rw-r--r--   0 sbr       (1000) sbr       (1000)    48831 2024-02-28 15:35:19.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera/CameraControl.py
-drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-02-29 07:31:00.868965 indi_pylibcamera-2.6.0/src/indi_pylibcamera/CameraInfos/
--rw-r--r--   0 sbr       (1000) sbr       (1000)     1397 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera/CameraInfos/Arducam_Pivariety_IMX462.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)     1903 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera/CameraInfos/IMX290.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)     2074 2024-02-23 15:06:38.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera/CameraInfos/Raspi_GlobalShutter_IMX296.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)     2654 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera/CameraInfos/Raspi_HQ_IMX477.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)     1960 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera/CameraInfos/Raspi_M3_IMX708.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)     2621 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera/CameraInfos/Raspi_V1_OV5647.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)     3244 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera/SnoopingManager.py
--rw-r--r--   0 sbr       (1000) sbr       (1000)       75 2024-02-29 06:41:25.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera/__init__.py
--rw-r--r--   0 sbr       (1000) sbr       (1000)     2472 2024-02-27 18:59:44.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera/indi_pylibcamera.ini
--rwxr-xr-x   0 sbr       (1000) sbr       (1000)    60404 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera/indi_pylibcamera.py
--rw-r--r--   0 sbr       (1000) sbr       (1000)      216 2024-02-29 06:41:25.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera/indi_pylibcamera.xml
--rw-r--r--   0 sbr       (1000) sbr       (1000)     2825 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera/indi_pylibcamera_postinstall.py
--rwxr-xr-x   0 sbr       (1000) sbr       (1000)    28758 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera/indidevice.py
--rw-r--r--   0 sbr       (1000) sbr       (1000)      902 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera/make_driver_xml.py
--rwxr-xr-x   0 sbr       (1000) sbr       (1000)     1944 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera/print_camera_information.py
-drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-02-29 07:31:00.872298 indi_pylibcamera-2.6.0/src/indi_pylibcamera/testpattern/
--rwxr-xr-x   0 sbr       (1000) sbr       (1000)    19253 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera/testpattern/RBG_testpattern.png
-drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-02-29 07:31:00.872298 indi_pylibcamera-2.6.0/src/indi_pylibcamera.egg-info/
--rw-r--r--   0 sbr       (1000) sbr       (1000)    21487 2024-02-29 07:31:00.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera.egg-info/PKG-INFO
--rw-r--r--   0 sbr       (1000) sbr       (1000)     1134 2024-02-29 07:31:00.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera.egg-info/SOURCES.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)        1 2024-02-29 07:31:00.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera.egg-info/dependency_links.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)      249 2024-02-29 07:31:00.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera.egg-info/entry_points.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)       23 2024-02-29 07:31:00.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera.egg-info/requires.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)       17 2024-02-29 07:31:00.000000 indi_pylibcamera-2.6.0/src/indi_pylibcamera.egg-info/top_level.txt
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-03 11:09:10.623809 indi_pylibcamera-2.6.1/
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     2291 2024-05-03 10:48:35.000000 indi_pylibcamera-2.6.1/CHANGELOG
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     1074 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.1/LICENSE
+-rw-r--r--   0 sbr       (1000) sbr       (1000)      187 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.1/MANIFEST.in
+-rw-r--r--   0 sbr       (1000) sbr       (1000)    22413 2024-05-03 11:09:10.623809 indi_pylibcamera-2.6.1/PKG-INFO
+-rw-r--r--   0 sbr       (1000) sbr       (1000)    18619 2024-05-03 11:01:07.000000 indi_pylibcamera-2.6.1/README.md
+-rw-r--r--   0 sbr       (1000) sbr       (1000)       81 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.1/pyproject.toml
+-rw-r--r--   0 sbr       (1000) sbr       (1000)      920 2024-05-03 11:09:10.627143 indi_pylibcamera-2.6.1/setup.cfg
+-rw-r--r--   0 sbr       (1000) sbr       (1000)       40 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.1/setup.py
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-03 11:09:10.610476 indi_pylibcamera-2.6.1/src/
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-03 11:09:10.613809 indi_pylibcamera-2.6.1/src/indi_pylibcamera/
+-rw-r--r--   0 sbr       (1000) sbr       (1000)    48830 2024-04-21 18:26:02.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera/CameraControl.py
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-03 11:09:10.620476 indi_pylibcamera-2.6.1/src/indi_pylibcamera/CameraInfos/
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     1397 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera/CameraInfos/Arducam_Pivariety_IMX462.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     1903 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera/CameraInfos/IMX290.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     2074 2024-02-23 15:06:38.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera/CameraInfos/Raspi_GlobalShutter_IMX296.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     2654 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera/CameraInfos/Raspi_HQ_IMX477.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     1960 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera/CameraInfos/Raspi_M3_IMX708.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     2621 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera/CameraInfos/Raspi_V1_OV5647.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     3244 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera/SnoopingManager.py
+-rw-r--r--   0 sbr       (1000) sbr       (1000)       75 2024-05-03 11:07:36.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera/__init__.py
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     2472 2024-02-27 18:59:44.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera/indi_pylibcamera.ini
+-rwxr-xr-x   0 sbr       (1000) sbr       (1000)    60404 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera/indi_pylibcamera.py
+-rw-r--r--   0 sbr       (1000) sbr       (1000)      216 2024-05-03 11:07:36.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera/indi_pylibcamera.xml
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     2825 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera/indi_pylibcamera_postinstall.py
+-rwxr-xr-x   0 sbr       (1000) sbr       (1000)    28758 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera/indidevice.py
+-rw-r--r--   0 sbr       (1000) sbr       (1000)      902 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera/make_driver_xml.py
+-rwxr-xr-x   0 sbr       (1000) sbr       (1000)     1944 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera/print_camera_information.py
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-03 11:09:10.623809 indi_pylibcamera-2.6.1/src/indi_pylibcamera/testpattern/
+-rwxr-xr-x   0 sbr       (1000) sbr       (1000)    19253 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera/testpattern/RBG_testpattern.png
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-03 11:09:10.623809 indi_pylibcamera-2.6.1/src/indi_pylibcamera.egg-info/
+-rw-r--r--   0 sbr       (1000) sbr       (1000)    22413 2024-05-03 11:09:10.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera.egg-info/PKG-INFO
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     1134 2024-05-03 11:09:10.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera.egg-info/SOURCES.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)        1 2024-05-03 11:09:10.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera.egg-info/dependency_links.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)      249 2024-05-03 11:09:10.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera.egg-info/entry_points.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)       40 2024-05-03 11:09:10.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera.egg-info/requires.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)       17 2024-05-03 11:09:10.000000 indi_pylibcamera-2.6.1/src/indi_pylibcamera.egg-info/top_level.txt
```

### Comparing `indi_pylibcamera-2.6.0/CHANGELOG` & `indi_pylibcamera-2.6.1/CHANGELOG`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+2.6.1
+- fixed ROWORDER attribute in FITS files (KStars/EKOS ignores this but some postprocessing tools need this fix to
+  have the Bayer pattern in the correct order)
+- more details in install_requires of the wheel
+- adapted install instructions in README.md to meet newer OS versions (installation in virtual environment)
+
 2.6.0
 - support for monochrome cameras
 - support for new raw and RGB frame formats (including monochrome)
 - disable astropy to download the latest IERS-A table from internet to avoid errors during observation session
 - better stability of exposure loop
 
 2.5.0
```

### Comparing `indi_pylibcamera-2.6.0/LICENSE` & `indi_pylibcamera-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.0/PKG-INFO` & `indi_pylibcamera-2.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: indi_pylibcamera
-Version: 2.6.0
+Version: 2.6.1
 Summary: An INDI driver for Raspberry Pi cameras supported by libcamera
 Home-page: https://github.com/scriptorron/indi_pylibcamera
 Author: Ronald Schreiber
 Author-email: ronald.schreiber01@gmx.de
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: picamera2
-Requires-Dist: lxml
-Requires-Dist: astropy
+Requires-Dist: numpy>=1.24
+Requires-Dist: astropy>=5.2
+Requires-Dist: picamera2>=0.3
 
 # indi_pylibcamera
 This project implements a Raspberry Pi camera driver for INDI (https://indilib.org/). 
 
 Raspberry Pi cameras allow the amateur astronomer to make astonishing pictures with small budget. Especially the
 Raspberry Pi HQ camera can compete with expensive astro cameras.
 
@@ -37,15 +37,15 @@
 ```
 It can not work when the versions of `libcamera` and `picamera2` are too old (both are in a dynamic development).
 And it can not work when the libcamera-tools (like `libcamera-hello` and `libcamera-still`) have issues with your
 camera.
 
 ## Requirements and installation
 Some packages need to be installed with apt-get:
-- `libcamera` (if not already installed). You can test libcamera and the support
+- `libcamera` and `libcamera-apps` (if not already installed). You can test libcamera and the support
 for your camera with: 
   ```commandline
   libcamera-hello --list-cameras
   ```
   You must be able to make RAW pictures in all modes. For instance `libcamera-hello` shows for the HQ camera:
   ```
   0 : imx477 [4056x3040] (/base/soc/i2c0mux/i2c@1/imx477@1a)
@@ -62,45 +62,57 @@
   libcamera-still -r --mode 4056:3040 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   ```
   Something with your libcamera or kernel driver installation will be wrong if this does not work.
 - Install INDI core library. If there is no pre-compiled package for your hardware you will need to compile it
 by yourself. Instructions can be found here: https://github.com/indilib/indi. A Raspberry Pi Zero does not
 have enough RAM to compile with 4 threads in parallel: you need to do `make -j1` instead of `make -j4`. 
 Finally, after installation, you need to have a working INDI server: `indiserver -v indi_simulator_telescope`
-- The Python packages `picamera2`, `numpy`, `lxml` and `astropy`. Theoretically these packages can be installed with `pip`. 
-But at least the version of `picamera2` must fit to the `libcamera` you installed with `apt-get`. Therefore it is
-safer to install these Python packages with `apt-get` too. 
-
-The command line to install all is:
+- The Python packages `PyQt5`, `picamera2` and `numpy` must be installed with `apt-get`. Typically they are already
+installed. If not you can install them with:
 ```commandline
-sudo apt-get install libcamera-apps indi-bin python3-picamera2 python3-lxml python3-astropy python3-numpy
+sudo apt-get install python3-picamera2 python3-pyqt5 python3-numpy
 ```
 
-The `indi_pylibcamera` driver package is available on PyPi. Please install with:
+The Raspberry PI OS requires a virtual environment to install non-system Python packages. Trying to install
+`indi_pylibcamera` without a virtual environment will fail with `error: externally-managed-environment`. 
+
+Run the following on a command line to install `indi_pylibcamera`in a virtual environment called `venv_indi_pylibcamera`:
 ```commandline
-sudo pip3 install indi_pylibcamera
+python3 -m venv --system-site-packages ~/venv_indi_pylibcamera
+source ~/venv_indi_pylibcamera/bin/activate
+pip install --upgrade pip
+pip install indi_pylibcamera
 sudo indi_pylibcamera_postinstall
 ```
 
 The `indi_pylibcamera_postinstall` script creates in `/usr/share/indi` a symbolic link to the driver XML. That makes
 the driver available in the KStars/EKOS profile editor in "CCD"->"OTHERS". Not all versions ov KStars/ECOS support this
 (for instance it works with KStars 3.6.5 but not with KStars 3.4.3).
 
 ## Uninstall
 For uninstalling the driver do:
 ```commandline
 sudo rm -f /usr/share/indi/indi_pylibcamera.xml
-sudo pip3 uninstall indi_pylibcamera
+rm -rf ~/venv_indi_pylibcamera
 ```
 
 ## Running
+You can start the deriver only in shell with activated virtual environment:
+```commandline
+source ~/venv_indi_pylibcamera/bin/activate
+```
+
 You can start the INDI server with `indiserver -v indi_pylibcamera`. When the server is running you can connect to
 the server from another computer with an INDI client (for instance KStars/EKOS). The camera name is the one
 you configure in `indi_pylibcamera.ini`.
 
+I have not tested it but when you want to start the driver from KStars/ECOS you likely need to start `kstars` from
+a shell with activated virtual environment. I recommend you to make a wrapper script to activate the environment and
+start the driver or KStars.
+
 ## Global Configuration
 The driver uses a hierarchy of configuration files to set global parameter. These configuration files are loaded in the
 following order:
 - `indi_pylibcamera.ini` in the program installation directory (typically in `/usr/lib/python*/site_packages`)
 - `$INDI_PYLIBCAMERA_CONFIG_PATH/indi_pylibcamera.ini`
 - `$HOME/.indi_pylibcamera/indi_pylibcamera.ini`
 - `./.indi_pylibcamera/indi_pylibcamera.ini`
@@ -327,14 +339,20 @@
 - Simon Šander
 - Aaron W Morris
 - Caden Gobat
 - anjok
 
 I hope I did not forget someone. If so please do not be angry and tell me.
 
+2.6.1
+- fixed ROWORDER attribute in FITS files (KStars/EKOS ignores this but some postprocessing tools need this fix to
+  have the Bayer pattern in the correct order)
+- more details in install_requires of the wheel
+- adapted install instructions in README.md to meet newer OS versions (installation in virtual environment)
+
 2.6.0
 - support for monochrome cameras
 - support for new raw and RGB frame formats (including monochrome)
 - disable astropy to download the latest IERS-A table from internet to avoid errors during observation session
 - better stability of exposure loop
 
 2.5.0
```

### Comparing `indi_pylibcamera-2.6.0/README.md` & `indi_pylibcamera-2.6.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ```
 It can not work when the versions of `libcamera` and `picamera2` are too old (both are in a dynamic development).
 And it can not work when the libcamera-tools (like `libcamera-hello` and `libcamera-still`) have issues with your
 camera.
 
 ## Requirements and installation
 Some packages need to be installed with apt-get:
-- `libcamera` (if not already installed). You can test libcamera and the support
+- `libcamera` and `libcamera-apps` (if not already installed). You can test libcamera and the support
 for your camera with: 
   ```commandline
   libcamera-hello --list-cameras
   ```
   You must be able to make RAW pictures in all modes. For instance `libcamera-hello` shows for the HQ camera:
   ```
   0 : imx477 [4056x3040] (/base/soc/i2c0mux/i2c@1/imx477@1a)
@@ -48,45 +48,57 @@
   libcamera-still -r --mode 4056:3040 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   ```
   Something with your libcamera or kernel driver installation will be wrong if this does not work.
 - Install INDI core library. If there is no pre-compiled package for your hardware you will need to compile it
 by yourself. Instructions can be found here: https://github.com/indilib/indi. A Raspberry Pi Zero does not
 have enough RAM to compile with 4 threads in parallel: you need to do `make -j1` instead of `make -j4`. 
 Finally, after installation, you need to have a working INDI server: `indiserver -v indi_simulator_telescope`
-- The Python packages `picamera2`, `numpy`, `lxml` and `astropy`. Theoretically these packages can be installed with `pip`. 
-But at least the version of `picamera2` must fit to the `libcamera` you installed with `apt-get`. Therefore it is
-safer to install these Python packages with `apt-get` too. 
-
-The command line to install all is:
+- The Python packages `PyQt5`, `picamera2` and `numpy` must be installed with `apt-get`. Typically they are already
+installed. If not you can install them with:
 ```commandline
-sudo apt-get install libcamera-apps indi-bin python3-picamera2 python3-lxml python3-astropy python3-numpy
+sudo apt-get install python3-picamera2 python3-pyqt5 python3-numpy
 ```
 
-The `indi_pylibcamera` driver package is available on PyPi. Please install with:
+The Raspberry PI OS requires a virtual environment to install non-system Python packages. Trying to install
+`indi_pylibcamera` without a virtual environment will fail with `error: externally-managed-environment`. 
+
+Run the following on a command line to install `indi_pylibcamera`in a virtual environment called `venv_indi_pylibcamera`:
 ```commandline
-sudo pip3 install indi_pylibcamera
+python3 -m venv --system-site-packages ~/venv_indi_pylibcamera
+source ~/venv_indi_pylibcamera/bin/activate
+pip install --upgrade pip
+pip install indi_pylibcamera
 sudo indi_pylibcamera_postinstall
 ```
 
 The `indi_pylibcamera_postinstall` script creates in `/usr/share/indi` a symbolic link to the driver XML. That makes
 the driver available in the KStars/EKOS profile editor in "CCD"->"OTHERS". Not all versions ov KStars/ECOS support this
 (for instance it works with KStars 3.6.5 but not with KStars 3.4.3).
 
 ## Uninstall
 For uninstalling the driver do:
 ```commandline
 sudo rm -f /usr/share/indi/indi_pylibcamera.xml
-sudo pip3 uninstall indi_pylibcamera
+rm -rf ~/venv_indi_pylibcamera
 ```
 
 ## Running
+You can start the deriver only in shell with activated virtual environment:
+```commandline
+source ~/venv_indi_pylibcamera/bin/activate
+```
+
 You can start the INDI server with `indiserver -v indi_pylibcamera`. When the server is running you can connect to
 the server from another computer with an INDI client (for instance KStars/EKOS). The camera name is the one
 you configure in `indi_pylibcamera.ini`.
 
+I have not tested it but when you want to start the driver from KStars/ECOS you likely need to start `kstars` from
+a shell with activated virtual environment. I recommend you to make a wrapper script to activate the environment and
+start the driver or KStars.
+
 ## Global Configuration
 The driver uses a hierarchy of configuration files to set global parameter. These configuration files are loaded in the
 following order:
 - `indi_pylibcamera.ini` in the program installation directory (typically in `/usr/lib/python*/site_packages`)
 - `$INDI_PYLIBCAMERA_CONFIG_PATH/indi_pylibcamera.ini`
 - `$HOME/.indi_pylibcamera/indi_pylibcamera.ini`
 - `./.indi_pylibcamera/indi_pylibcamera.ini`
```

### Comparing `indi_pylibcamera-2.6.0/setup.cfg` & `indi_pylibcamera-2.6.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 [options]
 package_dir = 
 	=src
 packages = find:
 include_package_data = True
 python_requires = >=3.7
 install_requires = 
-	picamera2
-	lxml
-	astropy
+	numpy>=1.24
+	astropy>=5.2
+	picamera2>=0.3
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	indi_pylibcamera = indi_pylibcamera.indi_pylibcamera:main
```

### Comparing `indi_pylibcamera-2.6.0/src/indi_pylibcamera/CameraControl.py` & `indi_pylibcamera-2.6.1/src/indi_pylibcamera/CameraControl.py`

 * *Files 0% similar despite different names*

```diff
@@ -551,15 +551,15 @@
         with self.parent.knownVectorsLock:
             # determine frame type
             FrameType = self.parent.knownVectors["CCD_FRAME_TYPE"].get_OnSwitchesLabels()[0]
             # FITS header and metadata
             FitsHeader = {
                 "BZERO": (2 ** (bit_pix - 1), "offset data range"),
                 "BSCALE": (1, "default scaling factor"),
-                "ROWORDER": ("BOTTOM-UP", "Row order"),
+                "ROWORDER": ("TOP-DOWN", "Row order"),
                 "INSTRUME": (self.parent.device, "CCD Name"),
                 "TELESCOP": (self.parent.knownVectors["ACTIVE_DEVICES"]["ACTIVE_TELESCOPE"].value, "Telescope name"),
                 **self.parent.knownVectors["FITS_HEADER"].FitsHeader,
                 "EXPTIME": (metadata["ExposureTime"]/1e6, "[s] Total Exposure Time"),
                 "CCD-TEMP": (metadata.get('SensorTemperature', 0), "[degC] CCD Temperature"),
                 "PIXSIZE1": (self.getProp("UnitCellSize")[0] / 1e3, "[um] Pixel Size 1"),
                 "PIXSIZE2": (self.getProp("UnitCellSize")[1] / 1e3, "[um] Pixel Size 2"),
```

### Comparing `indi_pylibcamera-2.6.0/src/indi_pylibcamera/CameraInfos/Arducam_Pivariety_IMX462.txt` & `indi_pylibcamera-2.6.1/src/indi_pylibcamera/CameraInfos/Arducam_Pivariety_IMX462.txt`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.0/src/indi_pylibcamera/CameraInfos/IMX290.txt` & `indi_pylibcamera-2.6.1/src/indi_pylibcamera/CameraInfos/IMX290.txt`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.0/src/indi_pylibcamera/CameraInfos/Raspi_GlobalShutter_IMX296.txt` & `indi_pylibcamera-2.6.1/src/indi_pylibcamera/CameraInfos/Raspi_GlobalShutter_IMX296.txt`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.0/src/indi_pylibcamera/CameraInfos/Raspi_HQ_IMX477.txt` & `indi_pylibcamera-2.6.1/src/indi_pylibcamera/CameraInfos/Raspi_HQ_IMX477.txt`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.0/src/indi_pylibcamera/CameraInfos/Raspi_M3_IMX708.txt` & `indi_pylibcamera-2.6.1/src/indi_pylibcamera/CameraInfos/Raspi_M3_IMX708.txt`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.0/src/indi_pylibcamera/CameraInfos/Raspi_V1_OV5647.txt` & `indi_pylibcamera-2.6.1/src/indi_pylibcamera/CameraInfos/Raspi_V1_OV5647.txt`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.0/src/indi_pylibcamera/SnoopingManager.py` & `indi_pylibcamera-2.6.1/src/indi_pylibcamera/SnoopingManager.py`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.0/src/indi_pylibcamera/indi_pylibcamera.ini` & `indi_pylibcamera-2.6.1/src/indi_pylibcamera/indi_pylibcamera.ini`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.0/src/indi_pylibcamera/indi_pylibcamera.py` & `indi_pylibcamera-2.6.1/src/indi_pylibcamera/indi_pylibcamera.py`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.0/src/indi_pylibcamera/indi_pylibcamera_postinstall.py` & `indi_pylibcamera-2.6.1/src/indi_pylibcamera/indi_pylibcamera_postinstall.py`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.0/src/indi_pylibcamera/indidevice.py` & `indi_pylibcamera-2.6.1/src/indi_pylibcamera/indidevice.py`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.0/src/indi_pylibcamera/make_driver_xml.py` & `indi_pylibcamera-2.6.1/src/indi_pylibcamera/make_driver_xml.py`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.0/src/indi_pylibcamera/print_camera_information.py` & `indi_pylibcamera-2.6.1/src/indi_pylibcamera/print_camera_information.py`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.0/src/indi_pylibcamera/testpattern/RBG_testpattern.png` & `indi_pylibcamera-2.6.1/src/indi_pylibcamera/testpattern/RBG_testpattern.png`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.0/src/indi_pylibcamera.egg-info/PKG-INFO` & `indi_pylibcamera-2.6.1/src/indi_pylibcamera.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: indi_pylibcamera
-Version: 2.6.0
+Version: 2.6.1
 Summary: An INDI driver for Raspberry Pi cameras supported by libcamera
 Home-page: https://github.com/scriptorron/indi_pylibcamera
 Author: Ronald Schreiber
 Author-email: ronald.schreiber01@gmx.de
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: picamera2
-Requires-Dist: lxml
-Requires-Dist: astropy
+Requires-Dist: numpy>=1.24
+Requires-Dist: astropy>=5.2
+Requires-Dist: picamera2>=0.3
 
 # indi_pylibcamera
 This project implements a Raspberry Pi camera driver for INDI (https://indilib.org/). 
 
 Raspberry Pi cameras allow the amateur astronomer to make astonishing pictures with small budget. Especially the
 Raspberry Pi HQ camera can compete with expensive astro cameras.
 
@@ -37,15 +37,15 @@
 ```
 It can not work when the versions of `libcamera` and `picamera2` are too old (both are in a dynamic development).
 And it can not work when the libcamera-tools (like `libcamera-hello` and `libcamera-still`) have issues with your
 camera.
 
 ## Requirements and installation
 Some packages need to be installed with apt-get:
-- `libcamera` (if not already installed). You can test libcamera and the support
+- `libcamera` and `libcamera-apps` (if not already installed). You can test libcamera and the support
 for your camera with: 
   ```commandline
   libcamera-hello --list-cameras
   ```
   You must be able to make RAW pictures in all modes. For instance `libcamera-hello` shows for the HQ camera:
   ```
   0 : imx477 [4056x3040] (/base/soc/i2c0mux/i2c@1/imx477@1a)
@@ -62,45 +62,57 @@
   libcamera-still -r --mode 4056:3040 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   ```
   Something with your libcamera or kernel driver installation will be wrong if this does not work.
 - Install INDI core library. If there is no pre-compiled package for your hardware you will need to compile it
 by yourself. Instructions can be found here: https://github.com/indilib/indi. A Raspberry Pi Zero does not
 have enough RAM to compile with 4 threads in parallel: you need to do `make -j1` instead of `make -j4`. 
 Finally, after installation, you need to have a working INDI server: `indiserver -v indi_simulator_telescope`
-- The Python packages `picamera2`, `numpy`, `lxml` and `astropy`. Theoretically these packages can be installed with `pip`. 
-But at least the version of `picamera2` must fit to the `libcamera` you installed with `apt-get`. Therefore it is
-safer to install these Python packages with `apt-get` too. 
-
-The command line to install all is:
+- The Python packages `PyQt5`, `picamera2` and `numpy` must be installed with `apt-get`. Typically they are already
+installed. If not you can install them with:
 ```commandline
-sudo apt-get install libcamera-apps indi-bin python3-picamera2 python3-lxml python3-astropy python3-numpy
+sudo apt-get install python3-picamera2 python3-pyqt5 python3-numpy
 ```
 
-The `indi_pylibcamera` driver package is available on PyPi. Please install with:
+The Raspberry PI OS requires a virtual environment to install non-system Python packages. Trying to install
+`indi_pylibcamera` without a virtual environment will fail with `error: externally-managed-environment`. 
+
+Run the following on a command line to install `indi_pylibcamera`in a virtual environment called `venv_indi_pylibcamera`:
 ```commandline
-sudo pip3 install indi_pylibcamera
+python3 -m venv --system-site-packages ~/venv_indi_pylibcamera
+source ~/venv_indi_pylibcamera/bin/activate
+pip install --upgrade pip
+pip install indi_pylibcamera
 sudo indi_pylibcamera_postinstall
 ```
 
 The `indi_pylibcamera_postinstall` script creates in `/usr/share/indi` a symbolic link to the driver XML. That makes
 the driver available in the KStars/EKOS profile editor in "CCD"->"OTHERS". Not all versions ov KStars/ECOS support this
 (for instance it works with KStars 3.6.5 but not with KStars 3.4.3).
 
 ## Uninstall
 For uninstalling the driver do:
 ```commandline
 sudo rm -f /usr/share/indi/indi_pylibcamera.xml
-sudo pip3 uninstall indi_pylibcamera
+rm -rf ~/venv_indi_pylibcamera
 ```
 
 ## Running
+You can start the deriver only in shell with activated virtual environment:
+```commandline
+source ~/venv_indi_pylibcamera/bin/activate
+```
+
 You can start the INDI server with `indiserver -v indi_pylibcamera`. When the server is running you can connect to
 the server from another computer with an INDI client (for instance KStars/EKOS). The camera name is the one
 you configure in `indi_pylibcamera.ini`.
 
+I have not tested it but when you want to start the driver from KStars/ECOS you likely need to start `kstars` from
+a shell with activated virtual environment. I recommend you to make a wrapper script to activate the environment and
+start the driver or KStars.
+
 ## Global Configuration
 The driver uses a hierarchy of configuration files to set global parameter. These configuration files are loaded in the
 following order:
 - `indi_pylibcamera.ini` in the program installation directory (typically in `/usr/lib/python*/site_packages`)
 - `$INDI_PYLIBCAMERA_CONFIG_PATH/indi_pylibcamera.ini`
 - `$HOME/.indi_pylibcamera/indi_pylibcamera.ini`
 - `./.indi_pylibcamera/indi_pylibcamera.ini`
@@ -327,14 +339,20 @@
 - Simon Šander
 - Aaron W Morris
 - Caden Gobat
 - anjok
 
 I hope I did not forget someone. If so please do not be angry and tell me.
 
+2.6.1
+- fixed ROWORDER attribute in FITS files (KStars/EKOS ignores this but some postprocessing tools need this fix to
+  have the Bayer pattern in the correct order)
+- more details in install_requires of the wheel
+- adapted install instructions in README.md to meet newer OS versions (installation in virtual environment)
+
 2.6.0
 - support for monochrome cameras
 - support for new raw and RGB frame formats (including monochrome)
 - disable astropy to download the latest IERS-A table from internet to avoid errors during observation session
 - better stability of exposure loop
 
 2.5.0
```

### Comparing `indi_pylibcamera-2.6.0/src/indi_pylibcamera.egg-info/SOURCES.txt` & `indi_pylibcamera-2.6.1/src/indi_pylibcamera.egg-info/SOURCES.txt`

 * *Files identical despite different names*


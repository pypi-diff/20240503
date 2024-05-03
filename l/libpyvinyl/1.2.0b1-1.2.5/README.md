# Comparing `tmp/libpyvinyl-1.2.0b1.tar.gz` & `tmp/libpyvinyl-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libpyvinyl-1.2.0b1.tar", last modified: Wed Jan 10 16:13:55 2024, max compression
+gzip compressed data, was "libpyvinyl-1.2.5.tar", last modified: Fri May  3 14:59:43 2024, max compression
```

## Comparing `libpyvinyl-1.2.0b1.tar` & `libpyvinyl-1.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 juncheng (30952) exfel     (3555)        0 2024-01-10 16:13:55.996690 libpyvinyl-1.2.0b1/
--rw-r--r--   0 juncheng (30952) exfel     (3555)     7440 2021-07-22 07:57:20.000000 libpyvinyl-1.2.0b1/LICENSE
--rw-r--r--   0 juncheng (30952) exfel     (3555)     1169 2024-01-10 16:13:55.996906 libpyvinyl-1.2.0b1/PKG-INFO
--rw-r--r--   0 juncheng (30952) exfel     (3555)     3836 2023-11-22 14:44:21.000000 libpyvinyl-1.2.0b1/README.md
-drwxr-xr-x   0 juncheng (30952) exfel     (3555)        0 2024-01-10 16:13:55.988401 libpyvinyl-1.2.0b1/libpyvinyl/
--rw-r--r--   0 juncheng (30952) exfel     (3555)     2032 2022-09-27 13:01:23.000000 libpyvinyl-1.2.0b1/libpyvinyl/AbstractBaseClass.py
--rw-r--r--   0 juncheng (30952) exfel     (3555)    16674 2024-01-10 13:54:46.000000 libpyvinyl-1.2.0b1/libpyvinyl/BaseCalculator.py
--rw-r--r--   0 juncheng (30952) exfel     (3555)    19205 2024-01-10 13:58:10.000000 libpyvinyl-1.2.0b1/libpyvinyl/BaseData.py
--rw-r--r--   0 juncheng (30952) exfel     (3555)     3989 2024-01-10 14:05:51.000000 libpyvinyl-1.2.0b1/libpyvinyl/BaseFormat.py
--rw-r--r--   0 juncheng (30952) exfel     (3555)     6013 2024-01-10 13:55:59.000000 libpyvinyl-1.2.0b1/libpyvinyl/Instrument.py
-drwxr-xr-x   0 juncheng (30952) exfel     (3555)        0 2024-01-10 16:13:55.995660 libpyvinyl-1.2.0b1/libpyvinyl/Parameters/
--rw-r--r--   0 juncheng (30952) exfel     (3555)    12670 2023-11-22 14:44:21.000000 libpyvinyl-1.2.0b1/libpyvinyl/Parameters/Collections.py
--rw-r--r--   0 juncheng (30952) exfel     (3555)    17676 2022-09-27 13:01:23.000000 libpyvinyl-1.2.0b1/libpyvinyl/Parameters/Parameter.py
--rw-r--r--   0 juncheng (30952) exfel     (3555)      118 2022-09-27 13:01:23.000000 libpyvinyl-1.2.0b1/libpyvinyl/Parameters/__init__.py
--rw-r--r--   0 juncheng (30952) exfel     (3555)      586 2024-01-10 16:11:31.000000 libpyvinyl-1.2.0b1/libpyvinyl/__init__.py
-drwxr-xr-x   0 juncheng (30952) exfel     (3555)        0 2024-01-10 16:13:55.991959 libpyvinyl-1.2.0b1/libpyvinyl.egg-info/
--rw-r--r--   0 juncheng (30952) exfel     (3555)     1169 2024-01-10 16:13:55.989363 libpyvinyl-1.2.0b1/libpyvinyl.egg-info/PKG-INFO
--rw-r--r--   0 juncheng (30952) exfel     (3555)      468 2024-01-10 16:13:55.990015 libpyvinyl-1.2.0b1/libpyvinyl.egg-info/SOURCES.txt
--rw-r--r--   0 juncheng (30952) exfel     (3555)        1 2024-01-10 16:13:55.990702 libpyvinyl-1.2.0b1/libpyvinyl.egg-info/dependency_links.txt
--rw-r--r--   0 juncheng (30952) exfel     (3555)       62 2024-01-10 16:13:55.991392 libpyvinyl-1.2.0b1/libpyvinyl.egg-info/requires.txt
--rw-r--r--   0 juncheng (30952) exfel     (3555)       11 2024-01-10 16:13:55.992123 libpyvinyl-1.2.0b1/libpyvinyl.egg-info/top_level.txt
--rw-r--r--   0 juncheng (30952) exfel     (3555)      186 2024-01-10 16:13:55.997715 libpyvinyl-1.2.0b1/setup.cfg
--rw-r--r--   0 juncheng (30952) exfel     (3555)     1979 2022-11-04 13:31:03.000000 libpyvinyl-1.2.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:59:43.175114 libpyvinyl-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-05-03 14:59:27.000000 libpyvinyl-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-03 14:59:43.175114 libpyvinyl-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-03 14:59:27.000000 libpyvinyl-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:59:43.171114 libpyvinyl-1.2.5/libpyvinyl/
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-03 14:59:27.000000 libpyvinyl-1.2.5/libpyvinyl/AbstractBaseClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16671 2024-05-03 14:59:27.000000 libpyvinyl-1.2.5/libpyvinyl/BaseCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-05-03 14:59:27.000000 libpyvinyl-1.2.5/libpyvinyl/BaseData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-03 14:59:27.000000 libpyvinyl-1.2.5/libpyvinyl/BaseFormat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-03 14:59:27.000000 libpyvinyl-1.2.5/libpyvinyl/Instrument.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:59:43.171114 libpyvinyl-1.2.5/libpyvinyl/Parameters/
+-rw-r--r--   0 runner    (1001) docker     (127)    12670 2024-05-03 14:59:27.000000 libpyvinyl-1.2.5/libpyvinyl/Parameters/Collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17676 2024-05-03 14:59:27.000000 libpyvinyl-1.2.5/libpyvinyl/Parameters/Parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-03 14:59:27.000000 libpyvinyl-1.2.5/libpyvinyl/Parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-03 14:59:27.000000 libpyvinyl-1.2.5/libpyvinyl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:59:43.171114 libpyvinyl-1.2.5/libpyvinyl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-03 14:59:43.000000 libpyvinyl-1.2.5/libpyvinyl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-03 14:59:43.000000 libpyvinyl-1.2.5/libpyvinyl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:59:43.000000 libpyvinyl-1.2.5/libpyvinyl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 14:59:43.000000 libpyvinyl-1.2.5/libpyvinyl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 14:59:43.000000 libpyvinyl-1.2.5/libpyvinyl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-03 14:59:43.175114 libpyvinyl-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-03 14:59:27.000000 libpyvinyl-1.2.5/setup.py
```

### Comparing `libpyvinyl-1.2.0b1/LICENSE` & `libpyvinyl-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `libpyvinyl-1.2.0b1/README.md` & `libpyvinyl-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `libpyvinyl-1.2.0b1/libpyvinyl/AbstractBaseClass.py` & `libpyvinyl-1.2.5/libpyvinyl/AbstractBaseClass.py`

 * *Files identical despite different names*

### Comparing `libpyvinyl-1.2.0b1/libpyvinyl/BaseCalculator.py` & `libpyvinyl-1.2.5/libpyvinyl/BaseCalculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 )
 
 
 class BaseCalculator(AbstractBaseClass):
     """
     Base class of all calculators.
 
-    This class is provides the libpyvinyl API. It defines all methods
+    This class provides the libpyvinyl API. It defines all methods
     through which a user interacts with the simulation backengines.
 
     This class is to be used as a base class for all calculators that implement
     a special simulation module, such as a photon diffraction calculator. Such a
     specialized Calculator has the same interface to the simulation
     backengine as all other ViNYL Calculators.
```

### Comparing `libpyvinyl-1.2.0b1/libpyvinyl/BaseData.py` & `libpyvinyl-1.2.5/libpyvinyl/BaseData.py`

 * *Files identical despite different names*

### Comparing `libpyvinyl-1.2.0b1/libpyvinyl/BaseFormat.py` & `libpyvinyl-1.2.5/libpyvinyl/BaseFormat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from abc import abstractmethod
 from libpyvinyl.AbstractBaseClass import AbstractBaseClass
 from libpyvinyl.BaseData import BaseData
 
 
 class BaseFormat(AbstractBaseClass):
     """
-    The abstract format class.
-    It's the interface of a certain data format.
+    The abstract format class which serves as the common interface for derived format classes.
     """
 
     def __init__(self):
         # Nothing needs to be done here.
         pass
 
     @classmethod
```

### Comparing `libpyvinyl-1.2.0b1/libpyvinyl/Instrument.py` & `libpyvinyl-1.2.5/libpyvinyl/Instrument.py`

 * *Files identical despite different names*

### Comparing `libpyvinyl-1.2.0b1/libpyvinyl/Parameters/Collections.py` & `libpyvinyl-1.2.5/libpyvinyl/Parameters/Collections.py`

 * *Files identical despite different names*

### Comparing `libpyvinyl-1.2.0b1/libpyvinyl/Parameters/Parameter.py` & `libpyvinyl-1.2.5/libpyvinyl/Parameters/Parameter.py`

 * *Files identical despite different names*

### Comparing `libpyvinyl-1.2.0b1/libpyvinyl/__init__.py` & `libpyvinyl-1.2.5/libpyvinyl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ :module: Exposes all user facing classes in the common libpyvinyl namespace"""
 __author__ = "Carsten Fortmann-Grote, Mads Bertelsen, Juncheng E, Shervin Nourbakhsh"
 __email__ = "carsten.grote@xfel.eu, juncheng.e@xfel.eu, Mads.Bertelsen@ess.eu, nourbakhsh@ill.fr"
-__version__ = "1.2.0b1"
+__version__ = "1.2.5"
 __release__ = __version__
 
 from .BaseCalculator import BaseCalculator, CalculatorParameters
 from .BaseData import BaseData
 from .Parameters.Parameter import Parameter
 from .Instrument import Instrument
```

### Comparing `libpyvinyl-1.2.0b1/setup.py` & `libpyvinyl-1.2.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 version = get_from_init(initfile, "__version__")
 setup(
     name="libpyvinyl",
     packages=find_packages(include=["libpyvinyl", "libpyvinyl.*"]),
     version=version,
     license="LGPLv3",
     description="The python API for photon and neutron simulation codes in the Photon and Neutron Open Science Cloud (PaNOSC).",
+    long_description_content_type="text/markdown",
+    long_description=read("README.md"),
     author=get_from_init(initfile, "__author__"),
     author_email=get_from_init(initfile, "__email__"),
     url="https://github.com/PaNOSC-ViNYL/libpyvinyl",
     download_url=f"https://github.com/PaNOSC-ViNYL/libpyvinyl/archive/v{version}.tar.gz",
     keywords=["photons", "neutrons", "simulations"],
     install_requires=requirements,
     classifiers=[
```


# Comparing `tmp/d2dcnWidget-0.1.2.tar.gz` & `tmp/d2dcnWidget-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d2dcnWidget-0.1.2.tar", last modified: Sun Mar 17 18:54:06 2024, max compression
+gzip compressed data, was "d2dcnWidget-0.1.3.tar", last modified: Fri May  3 08:43:54 2024, max compression
```

## Comparing `d2dcnWidget-0.1.2.tar` & `d2dcnWidget-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mou       (1000) mou       (1000)        0 2024-03-17 18:54:06.784927 d2dcnWidget-0.1.2/
--rw-r--r--   0 mou       (1000) mou       (1000)    35146 2024-01-03 16:45:16.000000 d2dcnWidget-0.1.2/LICENSE
--rw-rw-r--   0 mou       (1000) mou       (1000)      232 2024-03-17 18:54:06.784927 d2dcnWidget-0.1.2/PKG-INFO
-drwxrwxr-x   0 mou       (1000) mou       (1000)        0 2024-03-17 18:54:06.780927 d2dcnWidget-0.1.2/d2dcnWidget/
--rw-r--r--   0 mou       (1000) mou       (1000)      705 2024-01-03 22:33:57.000000 d2dcnWidget-0.1.2/d2dcnWidget/__init__.py
--rwxr-xr-x   0 mou       (1000) mou       (1000)     4072 2024-03-09 11:12:57.000000 d2dcnWidget-0.1.2/d2dcnWidget/d2dcnGUI.py
--rw-r--r--   0 mou       (1000) mou       (1000)    25951 2024-03-17 18:50:15.000000 d2dcnWidget-0.1.2/d2dcnWidget/d2dcnWidget.py
-drwxrwxr-x   0 mou       (1000) mou       (1000)        0 2024-03-17 18:54:06.784927 d2dcnWidget-0.1.2/d2dcnWidget.egg-info/
--rw-r--r--   0 mou       (1000) mou       (1000)      232 2024-03-17 18:54:06.000000 d2dcnWidget-0.1.2/d2dcnWidget.egg-info/PKG-INFO
--rw-r--r--   0 mou       (1000) mou       (1000)      303 2024-03-17 18:54:06.000000 d2dcnWidget-0.1.2/d2dcnWidget.egg-info/SOURCES.txt
--rw-r--r--   0 mou       (1000) mou       (1000)        1 2024-03-17 18:54:06.000000 d2dcnWidget-0.1.2/d2dcnWidget.egg-info/dependency_links.txt
--rw-r--r--   0 mou       (1000) mou       (1000)       55 2024-03-17 18:54:06.000000 d2dcnWidget-0.1.2/d2dcnWidget.egg-info/entry_points.txt
--rw-r--r--   0 mou       (1000) mou       (1000)       12 2024-03-17 18:54:06.000000 d2dcnWidget-0.1.2/d2dcnWidget.egg-info/requires.txt
--rw-r--r--   0 mou       (1000) mou       (1000)       12 2024-03-17 18:54:06.000000 d2dcnWidget-0.1.2/d2dcnWidget.egg-info/top_level.txt
--rw-rw-r--   0 mou       (1000) mou       (1000)       38 2024-03-17 18:54:06.784927 d2dcnWidget-0.1.2/setup.cfg
--rwxr-xr-x   0 mou       (1000) mou       (1000)      698 2024-03-09 11:12:57.000000 d2dcnWidget-0.1.2/setup.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2024-05-03 08:43:54.208278 d2dcnWidget-0.1.3/
+-rw-r--r--   0 docker    (1000) docker    (1000)    35146 2024-01-03 16:45:16.000000 d2dcnWidget-0.1.3/LICENSE
+-rw-r--r--   0 docker    (1000) docker    (1000)      283 2024-05-03 08:43:54.204278 d2dcnWidget-0.1.3/PKG-INFO
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2024-05-03 08:43:54.204278 d2dcnWidget-0.1.3/d2dcnWidget/
+-rw-r--r--   0 docker    (1000) docker    (1000)      705 2024-01-03 22:33:57.000000 d2dcnWidget-0.1.3/d2dcnWidget/__init__.py
+-rwxr-xr-x   0 docker    (1000) docker    (1000)     4072 2024-03-09 11:12:57.000000 d2dcnWidget-0.1.3/d2dcnWidget/d2dcnGUI.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    25947 2024-05-03 08:43:07.000000 d2dcnWidget-0.1.3/d2dcnWidget/d2dcnWidget.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2024-05-03 08:43:54.204278 d2dcnWidget-0.1.3/d2dcnWidget.egg-info/
+-rw-r--r--   0 docker    (1000) docker    (1000)      283 2024-05-03 08:43:54.000000 d2dcnWidget-0.1.3/d2dcnWidget.egg-info/PKG-INFO
+-rw-r--r--   0 docker    (1000) docker    (1000)      303 2024-05-03 08:43:54.000000 d2dcnWidget-0.1.3/d2dcnWidget.egg-info/SOURCES.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)        1 2024-05-03 08:43:54.000000 d2dcnWidget-0.1.3/d2dcnWidget.egg-info/dependency_links.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)       56 2024-05-03 08:43:54.000000 d2dcnWidget-0.1.3/d2dcnWidget.egg-info/entry_points.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)       12 2024-05-03 08:43:54.000000 d2dcnWidget-0.1.3/d2dcnWidget.egg-info/requires.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)       12 2024-05-03 08:43:54.000000 d2dcnWidget-0.1.3/d2dcnWidget.egg-info/top_level.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)       38 2024-05-03 08:43:54.208278 d2dcnWidget-0.1.3/setup.cfg
+-rwxr-xr-x   0 docker    (1000) docker    (1000)      698 2024-03-09 11:12:57.000000 d2dcnWidget-0.1.3/setup.py
```

### Comparing `d2dcnWidget-0.1.2/LICENSE` & `d2dcnWidget-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `d2dcnWidget-0.1.2/d2dcnWidget/__init__.py` & `d2dcnWidget-0.1.3/d2dcnWidget/__init__.py`

 * *Files identical despite different names*

### Comparing `d2dcnWidget-0.1.2/d2dcnWidget/d2dcnGUI.py` & `d2dcnWidget-0.1.3/d2dcnWidget/d2dcnGUI.py`

 * *Files identical despite different names*

### Comparing `d2dcnWidget-0.1.2/d2dcnWidget/d2dcnWidget.py` & `d2dcnWidget-0.1.3/d2dcnWidget/d2dcnWidget.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from PyQt5.QtGui import QFontMetrics
 
 import weakref
 
 import d2dcn
 
 
-version = "0.1.2"
+version = "0.1.3"
 
 class QHLine(QFrame):
     def __init__(self):
         super(QHLine, self).__init__()
         self.setFrameShape(QFrame.HLine)
         self.setFrameShadow(QFrame.Sunken)
         self.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Fixed)
@@ -266,15 +266,15 @@
         self.__main_layout.addWidget(self.__info_widget)
 
         self.__dif_line = QVLine()
         self.__main_layout.addWidget(self.__dif_line)
         self.__dif_line.hide()
 
         self.__command_widget = QWidget()
-        self.__command_widget.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
+        self.__command_widget.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Expanding)
         self.__command_widget.hide()
 
         if object_hlayout:
             self.__command_layout = QHBoxLayout()
         else:
             self.__command_layout = QVBoxLayout()
```

### Comparing `d2dcnWidget-0.1.2/setup.py` & `d2dcnWidget-0.1.3/setup.py`

 * *Files identical despite different names*


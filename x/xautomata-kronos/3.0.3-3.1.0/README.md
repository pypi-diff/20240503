# Comparing `tmp/xautomata-kronos-3.0.3.tar.gz` & `tmp/xautomata_kronos-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xautomata-kronos-3.0.3.tar", last modified: Mon Jan 29 07:49:30 2024, max compression
+gzip compressed data, was "xautomata_kronos-3.1.0.tar", last modified: Fri May  3 11:35:07 2024, max compression
```

## Comparing `xautomata-kronos-3.0.3.tar` & `xautomata_kronos-3.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 07:49:30.557258 xautomata-kronos-3.0.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 07:49:30.553258 xautomata-kronos-3.0.3/Kronos/
--rw-r--r--   0 root         (0) root         (0)     3672 2024-01-29 07:49:30.000000 xautomata-kronos-3.0.3/Kronos/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2002 2024-01-29 07:49:30.000000 xautomata-kronos-3.0.3/Kronos/converters.py
--rw-r--r--   0 root         (0) root         (0)     7346 2024-01-29 07:49:30.000000 xautomata-kronos-3.0.3/Kronos/costructors.py
--rw-r--r--   0 root         (0) root         (0)     3839 2024-01-29 07:49:30.000000 xautomata-kronos-3.0.3/Kronos/hourglass.py
--rw-r--r--   0 root         (0) root         (0)     1802 2024-01-29 07:49:30.000000 xautomata-kronos-3.0.3/Kronos/periods.py
--rw-r--r--   0 root         (0) root         (0)     8716 2024-01-29 07:49:30.000000 xautomata-kronos-3.0.3/Kronos/sliders.py
--rw-r--r--   0 root         (0) root         (0)       17 2024-01-29 07:49:30.000000 xautomata-kronos-3.0.3/Kronos/version.py
--rw-r--r--   0 root         (0) root         (0)     1066 2024-01-29 07:49:30.000000 xautomata-kronos-3.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6257 2024-01-29 07:49:30.553258 xautomata-kronos-3.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5997 2024-01-29 07:49:30.000000 xautomata-kronos-3.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-29 07:49:30.557258 xautomata-kronos-3.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      771 2024-01-29 07:49:30.000000 xautomata-kronos-3.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 07:49:30.553258 xautomata-kronos-3.0.3/xautomata_kronos.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6257 2024-01-29 07:49:30.000000 xautomata-kronos-3.0.3/xautomata_kronos.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      322 2024-01-29 07:49:30.000000 xautomata-kronos-3.0.3/xautomata_kronos.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-29 07:49:30.000000 xautomata-kronos-3.0.3/xautomata_kronos.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-01-29 07:49:30.000000 xautomata-kronos-3.0.3/xautomata_kronos.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 11:35:07.849754 xautomata_kronos-3.1.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 11:35:07.845754 xautomata_kronos-3.1.0/Kronos/
+-rw-r--r--   0 root         (0) root         (0)     4033 2024-05-03 11:35:07.000000 xautomata_kronos-3.1.0/Kronos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2466 2024-05-03 11:35:07.000000 xautomata_kronos-3.1.0/Kronos/converters.py
+-rw-r--r--   0 root         (0) root         (0)     7353 2024-05-03 11:35:07.000000 xautomata_kronos-3.1.0/Kronos/costructors.py
+-rw-r--r--   0 root         (0) root         (0)     3839 2024-05-03 11:35:07.000000 xautomata_kronos-3.1.0/Kronos/hourglass.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2024-05-03 11:35:07.000000 xautomata_kronos-3.1.0/Kronos/periods.py
+-rw-r--r--   0 root         (0) root         (0)     8716 2024-05-03 11:35:07.000000 xautomata_kronos-3.1.0/Kronos/sliders.py
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-03 11:35:07.000000 xautomata_kronos-3.1.0/Kronos/version.py
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-05-03 11:35:07.000000 xautomata_kronos-3.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6257 2024-05-03 11:35:07.849754 xautomata_kronos-3.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5997 2024-05-03 11:35:07.000000 xautomata_kronos-3.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 11:35:07.849754 xautomata_kronos-3.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      771 2024-05-03 11:35:07.000000 xautomata_kronos-3.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 11:35:07.849754 xautomata_kronos-3.1.0/xautomata_kronos.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6257 2024-05-03 11:35:07.000000 xautomata_kronos-3.1.0/xautomata_kronos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      322 2024-05-03 11:35:07.000000 xautomata_kronos-3.1.0/xautomata_kronos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 11:35:07.000000 xautomata_kronos-3.1.0/xautomata_kronos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-03 11:35:07.000000 xautomata_kronos-3.1.0/xautomata_kronos.egg-info/top_level.txt
```

### Comparing `xautomata-kronos-3.0.3/Kronos/__init__.py` & `xautomata_kronos-3.1.0/Kronos/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from Kronos.hourglass import Core, TimeZones, Format
+from Kronos.hourglass import Core, TimeZones, Format, Converters
 
 
 def now(tz=None):
     """
     Produce the current datetime
 
     Args:
@@ -173,7 +173,19 @@
     Args:
         list_iso (list[str]): list of isoformat string
         tz: Timezone. Default to Rome
 
     Returns: list[Kronos]
     """
     return Core.from_list_iso(list_iso=list_iso, tz=tz)
+
+#
+# def move_tz_from_list(list_old_tz, tz=None):
+#     """
+#     modify the time accordingly to a new timezone for a list of Kronos
+#     Args:
+#         list_old_tz (list[str]): list of Kronos
+#         tz: Timezone. Default to Rome
+#
+#     Returns: list[Kronos]
+#     """
+#     return Converters.move_tz_from_list(list_old_tz=list_old_tz, tz=tz)
```

### Comparing `xautomata-kronos-3.0.3/Kronos/costructors.py` & `xautomata_kronos-3.1.0/Kronos/costructors.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     if isinstance(tz, str): tz = TimeZones.dict_zones[tz]
 
     if type(dt) == date and dt is not None:  # permette di identificare le date, senza prendere i datetime
         # le date vengono trasformate in datetime senza tz, che viene aggiunta dopo
         dt = datetime(year=dt.year, month=dt.month, day=dt.day, hour=0, minute=0, second=0, microsecond=0)
 
     if isinstance(dt, datetime):  # serve per leggere i datetime
-        if tz is None:
-            tz = TimeZones(dt).rome
-
         if dt.tzinfo is None:
+            if tz is None:
+                tz = TimeZones(dt).rome
             dt = dt.replace(tzinfo=tz)
     return dt
 
 
 class TimeZones:
     utc = timezone.utc
     rome = timezone(timedelta(hours=1))  # time zone invernale o solare
```

### Comparing `xautomata-kronos-3.0.3/Kronos/hourglass.py` & `xautomata_kronos-3.1.0/Kronos/hourglass.py`

 * *Files identical despite different names*

### Comparing `xautomata-kronos-3.0.3/Kronos/periods.py` & `xautomata_kronos-3.1.0/Kronos/periods.py`

 * *Files identical despite different names*

### Comparing `xautomata-kronos-3.0.3/Kronos/sliders.py` & `xautomata_kronos-3.1.0/Kronos/sliders.py`

 * *Files identical despite different names*

### Comparing `xautomata-kronos-3.0.3/LICENSE` & `xautomata_kronos-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xautomata-kronos-3.0.3/PKG-INFO` & `xautomata_kronos-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xautomata-kronos
-Version: 3.0.3
+Version: 3.1.0
 Home-page: https://github.com/sherlogic/xautomata-kronos.git
 Author: Andrea Jacassi
 Author-email: 
 License: MIT
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `xautomata-kronos-3.0.3/README.md` & `xautomata_kronos-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `xautomata-kronos-3.0.3/setup.py` & `xautomata_kronos-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `xautomata-kronos-3.0.3/xautomata_kronos.egg-info/PKG-INFO` & `xautomata_kronos-3.1.0/xautomata_kronos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xautomata-kronos
-Version: 3.0.3
+Version: 3.1.0
 Home-page: https://github.com/sherlogic/xautomata-kronos.git
 Author: Andrea Jacassi
 Author-email: 
 License: MIT
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```


# Comparing `tmp/icalcli-1.0.5.tar.gz` & `tmp/icalcli-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icalcli-1.0.5.tar", last modified: Wed Apr 17 13:41:05 2024, max compression
+gzip compressed data, was "icalcli-1.0.6.tar", last modified: Fri May  3 11:51:17 2024, max compression
```

## Comparing `icalcli-1.0.5.tar` & `icalcli-1.0.6.tar`

### file list

```diff
@@ -1,29 +1,26 @@
-drwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)        0 2024-04-17 13:41:05.252852 icalcli-1.0.5/
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     2634 2024-04-17 13:16:33.000000 icalcli-1.0.5/CHANGELOG.md
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     1137 2019-12-19 12:54:20.000000 icalcli-1.0.5/LICENSE
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     6814 2024-04-17 13:41:05.252852 icalcli-1.0.5/PKG-INFO
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     6256 2024-04-17 13:10:57.000000 icalcli-1.0.5/README.md
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)      104 2020-01-08 05:10:41.000000 icalcli-1.0.5/exclude
-drwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)        0 2024-04-17 13:41:05.252852 icalcli-1.0.5/icalcli/
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)      450 2022-10-11 15:38:57.000000 icalcli-1.0.5/icalcli/__init__.py
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)    11604 2024-04-17 09:15:43.000000 icalcli-1.0.5/icalcli/argparsers.py
-drwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)        0 2024-04-17 13:41:05.252852 icalcli-1.0.5/icalcli/etesync_backend/
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)       29 2022-07-12 07:50:56.000000 icalcli-1.0.5/icalcli/etesync_backend/__init__.py
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     3908 2022-07-25 08:52:55.000000 icalcli-1.0.5/icalcli/etesync_backend/etesync_crud.py
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     3325 2020-01-08 14:23:24.000000 icalcli-1.0.5/icalcli/etesync_backend/etesync_interface.py
-drwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)        0 2024-04-17 13:41:05.252852 icalcli-1.0.5/icalcli/file_backend/
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)       29 2022-07-12 07:48:59.000000 icalcli-1.0.5/icalcli/file_backend/__init__.py
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     2627 2024-04-17 12:29:26.000000 icalcli-1.0.5/icalcli/file_backend/ics_interface.py
--rwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)    68901 2024-04-17 12:28:55.000000 icalcli-1.0.5/icalcli/icalcli.py
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     4037 2019-02-28 12:11:14.000000 icalcli-1.0.5/icalcli/printer.py
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     4193 2022-08-10 09:40:48.000000 icalcli-1.0.5/icalcli/utils.py
-drwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)        0 2024-04-17 13:41:05.252852 icalcli-1.0.5/icalcli.egg-info/
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     6814 2024-04-17 13:41:05.000000 icalcli-1.0.5/icalcli.egg-info/PKG-INFO
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)      541 2024-04-17 13:41:05.000000 icalcli-1.0.5/icalcli.egg-info/SOURCES.txt
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)        1 2024-04-17 13:41:05.000000 icalcli-1.0.5/icalcli.egg-info/dependency_links.txt
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)       49 2024-04-17 13:41:05.000000 icalcli-1.0.5/icalcli.egg-info/entry_points.txt
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)       93 2024-04-17 13:41:05.000000 icalcli-1.0.5/icalcli.egg-info/requires.txt
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)        8 2024-04-17 13:41:05.000000 icalcli-1.0.5/icalcli.egg-info/top_level.txt
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)       38 2024-04-17 13:41:05.252852 icalcli-1.0.5/setup.cfg
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     1173 2024-04-17 13:16:47.000000 icalcli-1.0.5/setup.py
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)      890 2020-09-10 14:15:34.000000 icalcli-1.0.5/update-github.md
+drwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)        0 2024-05-03 11:51:17.730177 icalcli-1.0.6/
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     1137 2019-12-19 12:54:20.000000 icalcli-1.0.6/LICENSE
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     6991 2024-05-03 11:51:17.730177 icalcli-1.0.6/PKG-INFO
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     6256 2024-04-17 13:10:57.000000 icalcli-1.0.6/README.md
+drwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)        0 2024-05-03 11:51:17.730177 icalcli-1.0.6/icalcli/
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)      450 2022-10-11 15:38:57.000000 icalcli-1.0.6/icalcli/__init__.py
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)    11604 2024-04-17 09:15:43.000000 icalcli-1.0.6/icalcli/argparsers.py
+drwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)        0 2024-05-03 11:51:17.730177 icalcli-1.0.6/icalcli/etesync_backend/
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)       29 2022-07-12 07:50:56.000000 icalcli-1.0.6/icalcli/etesync_backend/__init__.py
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     3908 2022-07-25 08:52:55.000000 icalcli-1.0.6/icalcli/etesync_backend/etesync_crud.py
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     3325 2020-01-08 14:23:24.000000 icalcli-1.0.6/icalcli/etesync_backend/etesync_interface.py
+drwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)        0 2024-05-03 11:51:17.730177 icalcli-1.0.6/icalcli/file_backend/
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)       29 2022-07-12 07:48:59.000000 icalcli-1.0.6/icalcli/file_backend/__init__.py
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     2627 2024-04-17 12:29:26.000000 icalcli-1.0.6/icalcli/file_backend/ics_interface.py
+-rwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)    68952 2024-05-03 11:44:28.000000 icalcli-1.0.6/icalcli/icalcli.py
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     4037 2019-02-28 12:11:14.000000 icalcli-1.0.6/icalcli/printer.py
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     4193 2022-08-10 09:40:48.000000 icalcli-1.0.6/icalcli/utils.py
+drwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)        0 2024-05-03 11:51:17.730177 icalcli-1.0.6/icalcli.egg-info/
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     6991 2024-05-03 11:51:17.000000 icalcli-1.0.6/icalcli.egg-info/PKG-INFO
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)      503 2024-05-03 11:51:17.000000 icalcli-1.0.6/icalcli.egg-info/SOURCES.txt
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)        1 2024-05-03 11:51:17.000000 icalcli-1.0.6/icalcli.egg-info/dependency_links.txt
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)       49 2024-05-03 11:51:17.000000 icalcli-1.0.6/icalcli.egg-info/entry_points.txt
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)       93 2024-05-03 11:51:17.000000 icalcli-1.0.6/icalcli.egg-info/requires.txt
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)        8 2024-05-03 11:51:17.000000 icalcli-1.0.6/icalcli.egg-info/top_level.txt
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)       38 2024-05-03 11:51:17.730177 icalcli-1.0.6/setup.cfg
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     1173 2024-05-03 11:45:04.000000 icalcli-1.0.6/setup.py
```

### Comparing `icalcli-1.0.5/LICENSE` & `icalcli-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `icalcli-1.0.5/PKG-INFO` & `icalcli-1.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: icalcli
-Version: 1.0.5
+Version: 1.0.6
 Summary: Icalendar Calendar Command Line Interface
 Home-page: https://github.com/jrvarma/icalcli
 Maintainer: Jayanth R. Varma
 Maintainer-email: jrvarma@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: parsedatetime
 License-File: LICENSE
+Requires-Dist: python-dateutil
+Requires-Dist: parsedatetime
+Requires-Dist: icalendar
+Requires-Dist: recurring_ical_events
+Provides-Extra: parsedatetime
+Requires-Dist: parsedatetime; extra == "parsedatetime"
 
 # icalcli
 
 ### An iCalendar Command Line Interface
 
 `icalcli` - a modification of [gcalcli](https://github.com/insanum/gcalcli) - is a Python command line front-end to your Calendar. It allows you to get your agenda, view weekly and monthly calendars (ascii text graphical calendar), search for events, add new events, delete events, and edit events.
```

### Comparing `icalcli-1.0.5/README.md` & `icalcli-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `icalcli-1.0.5/icalcli/argparsers.py` & `icalcli-1.0.6/icalcli/argparsers.py`

 * *Files identical despite different names*

### Comparing `icalcli-1.0.5/icalcli/etesync_backend/etesync_crud.py` & `icalcli-1.0.6/icalcli/etesync_backend/etesync_crud.py`

 * *Files identical despite different names*

### Comparing `icalcli-1.0.5/icalcli/etesync_backend/etesync_interface.py` & `icalcli-1.0.6/icalcli/etesync_backend/etesync_interface.py`

 * *Files identical despite different names*

### Comparing `icalcli-1.0.5/icalcli/file_backend/ics_interface.py` & `icalcli-1.0.6/icalcli/file_backend/ics_interface.py`

 * *Files identical despite different names*

### Comparing `icalcli-1.0.5/icalcli/icalcli.py` & `icalcli-1.0.6/icalcli/icalcli.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,21 +381,21 @@
                 and 'location' in event
                 and event.Decoded('location').decode().strip()
         ):
             summary += " [%s]" % (event.Decoded('location').
                                   decode().strip())
         if self.graphical_outputs.get('uid'):
             summary += " <%s>" % (event.Decoded('uid').decode().strip())
-        # if (
-        #         self.graphical_outputs.get('description')
-        #         and 'description' in event
-        #         and event.Decoded('description').decode().strip()
-        #         and self.outputs.get('description')
-        # ):
-        #     summary += event.Decoded('description'). decode().strip()
+        if (
+                self.graphical_outputs.get('description')
+                and 'description' in event
+                and event.Decoded('description').decode().strip()
+                and self.outputs.get('description')
+        ):
+            summary += event.Decoded('description'). decode().strip()
         return summary
 
     def get_week_events(self, start_dt, end_dt, event_list):
         r"""Returns all events during a week (start_dt to end_dt)
 
         Parameters
         ----------
@@ -547,30 +547,31 @@
         string : string (will be split into list of words)
         cur_print_len : int
 
         Returns
         -------
         int: where to cut the word
         """
-        print_len = 0
+        # print_len = 0
 
         words = _u(string).split()
         for i, word in enumerate(words):
+            print_len = self.printed_len(' '.join(words[:i]))
             word_len = self.printed_len(word)
             if (
                     (cur_print_len + word_len + print_len
                      ) >= self.options['cal_width']
             ):
                 cut_idx = len(' '.join(words[:i]))
                 # if the  word is too long,
                 # we cannot cut between words
                 if cut_idx == 0:
                     return self.word_cut(word)
                 return (print_len, cut_idx)
-            print_len += word_len + i  # +i for the space between words
+            # print_len += word_len + i  # +i for the space between words
         return (print_len, len(' '.join(words[:i])))
 
     def get_cut_index(self, event_string):
         r"""Cut string at line break, between words or within word
         to cal_width
 
         Parameters
@@ -737,15 +738,14 @@
                         continue
 
                     curr_event = week_events[j][0]
                     print_len, cut_idx = self.get_cut_index(
                         curr_event.title)
                     padding = ' ' * (self.options['cal_width']
                                      - print_len)
-
                     self.printer.msg(
                             curr_event.title[:cut_idx] + padding,
                             curr_event.color)
 
                     # trim what we've already printed
                     trimmed_title = curr_event.title[cut_idx:].strip()
```

### Comparing `icalcli-1.0.5/icalcli/printer.py` & `icalcli-1.0.6/icalcli/printer.py`

 * *Files identical despite different names*

### Comparing `icalcli-1.0.5/icalcli/utils.py` & `icalcli-1.0.6/icalcli/utils.py`

 * *Files identical despite different names*

### Comparing `icalcli-1.0.5/icalcli.egg-info/PKG-INFO` & `icalcli-1.0.6/icalcli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: icalcli
-Version: 1.0.5
+Version: 1.0.6
 Summary: Icalendar Calendar Command Line Interface
 Home-page: https://github.com/jrvarma/icalcli
 Maintainer: Jayanth R. Varma
 Maintainer-email: jrvarma@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: parsedatetime
 License-File: LICENSE
+Requires-Dist: python-dateutil
+Requires-Dist: parsedatetime
+Requires-Dist: icalendar
+Requires-Dist: recurring_ical_events
+Provides-Extra: parsedatetime
+Requires-Dist: parsedatetime; extra == "parsedatetime"
 
 # icalcli
 
 ### An iCalendar Command Line Interface
 
 `icalcli` - a modification of [gcalcli](https://github.com/insanum/gcalcli) - is a Python command line front-end to your Calendar. It allows you to get your agenda, view weekly and monthly calendars (ascii text graphical calendar), search for events, add new events, delete events, and edit events.
```

### Comparing `icalcli-1.0.5/setup.py` & `icalcli-1.0.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='icalcli',
-      version='1.0.5',
+      version='1.0.6',
       maintainer='Jayanth R. Varma',
       maintainer_email='jrvarma@gmail.com',
       description='Icalendar Calendar Command Line Interface',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/jrvarma/icalcli",
       packages=['icalcli', 'icalcli.etesync_backend', 'icalcli.file_backend'],
```


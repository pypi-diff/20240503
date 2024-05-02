# Comparing `tmp/inspyre_toolbox-1.4.1.tar.gz` & `tmp/inspyre_toolbox-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspyre_toolbox-1.4.1.tar", max compression
+gzip compressed data, was "inspyre_toolbox-1.4.2.tar", max compression
```

## Comparing `inspyre_toolbox-1.4.1.tar` & `inspyre_toolbox-1.4.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      209 2024-04-30 20:45:10.403940 inspyre_toolbox-1.4.1/inspyre_toolbox/__about__.py
--rw-r--r--   0        0        0     2639 2024-04-30 20:44:59.194115 inspyre_toolbox-1.4.1/inspyre_toolbox/__init__.py
--rw-r--r--   0        0        0       16 2024-04-30 20:45:10.403940 inspyre_toolbox-1.4.1/inspyre_toolbox/api_changes.ini
--rw-r--r--   0        0        0        0 2024-04-30 20:45:10.405306 inspyre_toolbox-1.4.1/inspyre_toolbox/cli/__init__.py
--rw-r--r--   0        0        0     3005 2024-04-30 20:45:10.405306 inspyre_toolbox-1.4.1/inspyre_toolbox/cli/ist_bytes_converter/__init__.py
--rw-r--r--   0        0        0     3388 2024-04-30 20:45:10.405306 inspyre_toolbox-1.4.1/inspyre_toolbox/cli/ist_bytes_converter/arguments.py
--rw-r--r--   0        0        0     1425 2024-04-30 20:45:10.406705 inspyre_toolbox-1.4.1/inspyre_toolbox/cli/ist_bytes_converter/helpers.py
--rw-r--r--   0        0        0        0 2024-04-30 20:45:10.406705 inspyre_toolbox-1.4.1/inspyre_toolbox/common/__init__.py
--rw-r--r--   0        0        0      934 2024-04-30 21:17:34.719515 inspyre_toolbox-1.4.1/inspyre_toolbox/common/meta.py
--rw-r--r--   0        0        0     2808 2024-04-30 20:44:59.194115 inspyre_toolbox-1.4.1/inspyre_toolbox/console_kit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 20:44:59.195113 inspyre_toolbox-1.4.1/inspyre_toolbox/conversions/__init__.py
--rw-r--r--   0        0        0     4240 2024-04-30 20:45:10.407939 inspyre_toolbox-1.4.1/inspyre_toolbox/conversions/bytes/__init__.py
--rw-r--r--   0        0        0     5299 2024-04-30 20:45:10.407939 inspyre_toolbox-1.4.1/inspyre_toolbox/conversions/roman_numerals/__init__.py
--rw-r--r--   0        0        0     1143 2024-04-30 20:44:59.196112 inspyre_toolbox-1.4.1/inspyre_toolbox/conversions/roman_numerals/errors.py
--rw-r--r--   0        0        0        0 2024-04-30 20:44:59.196112 inspyre_toolbox-1.4.1/inspyre_toolbox/core/errors/__init__.py
--rw-r--r--   0        0        0     2636 2024-04-30 20:44:59.196112 inspyre_toolbox-1.4.1/inspyre_toolbox/core/errors/version.py
--rw-r--r--   0        0        0       97 2024-04-30 20:44:59.197472 inspyre_toolbox-1.4.1/inspyre_toolbox/core_helpers/__init__.py
--rw-r--r--   0        0        0      424 2024-04-30 20:44:59.197472 inspyre_toolbox-1.4.1/inspyre_toolbox/core_helpers/debugging.py
--rw-r--r--   0        0        0     4065 2024-04-30 20:45:10.409300 inspyre_toolbox-1.4.1/inspyre_toolbox/core_helpers/logging.py
--rw-r--r--   0        0        0     1951 2024-04-30 20:45:10.409300 inspyre_toolbox-1.4.1/inspyre_toolbox/docs/conversions/bytes.md
--rw-r--r--   0        0        0     3413 2024-04-30 20:45:10.410790 inspyre_toolbox-1.4.1/inspyre_toolbox/generations/__init__.py
--rw-r--r--   0        0        0    22944 2024-04-30 20:45:10.410790 inspyre_toolbox-1.4.1/inspyre_toolbox/humanize/__init__.py
--rw-r--r--   0        0        0      262 2024-04-30 20:44:59.198686 inspyre_toolbox-1.4.1/inspyre_toolbox/humanize/errors/__init__.py
--rw-r--r--   0        0        0     1927 2024-04-30 20:44:59.199745 inspyre_toolbox-1.4.1/inspyre_toolbox/humanize/errors/numerical.py
--rw-r--r--   0        0        0     9240 2024-04-30 20:44:59.200756 inspyre_toolbox-1.4.1/inspyre_toolbox/live_timer/__init__.py
--rw-r--r--   0        0        0     1100 2024-04-30 20:44:59.200756 inspyre_toolbox-1.4.1/inspyre_toolbox/live_timer/errors.py
--rw-r--r--   0        0        0     2297 2024-04-30 20:44:59.201755 inspyre_toolbox-1.4.1/inspyre_toolbox/live_timer/history.py
--rw-r--r--   0        0        0    11458 2024-04-30 20:45:10.412229 inspyre_toolbox-1.4.1/inspyre_toolbox/proc_man/__init__.py
--rw-r--r--   0        0        0      689 2024-04-30 20:44:59.202755 inspyre_toolbox-1.4.1/inspyre_toolbox/proc_man/errors.py
--rw-r--r--   0        0        0        0 2024-04-30 20:44:59.202755 inspyre_toolbox-1.4.1/inspyre_toolbox/pypi/__init__.py
--rw-r--r--   0        0        0      900 2024-04-30 20:44:59.203757 inspyre_toolbox-1.4.1/inspyre_toolbox/pypi/packages.py
--rw-r--r--   0        0        0      596 2024-04-30 20:44:59.203757 inspyre_toolbox-1.4.1/inspyre_toolbox/settings.py
--rw-r--r--   0        0        0     1868 2024-04-30 20:45:10.412229 inspyre_toolbox-1.4.1/inspyre_toolbox/solve_kit/__init__.py
--rw-r--r--   0        0        0      175 2024-04-30 20:44:59.204758 inspyre_toolbox-1.4.1/inspyre_toolbox/spanners/__init__.py
--rw-r--r--   0        0        0     2210 2024-04-30 20:44:59.204758 inspyre_toolbox-1.4.1/inspyre_toolbox/spanners/span_arg_parse.py
--rw-r--r--   0        0        0     1014 2024-04-30 20:44:59.204758 inspyre_toolbox-1.4.1/inspyre_toolbox/syntactic_sweets/__init__.py
--rw-r--r--   0        0        0     2265 2024-04-30 20:44:59.205757 inspyre_toolbox-1.4.1/inspyre_toolbox/sys_man/__init__.py
--rw-r--r--   0        0        0     6999 2024-04-30 20:45:10.413573 inspyre_toolbox-1.4.1/inspyre_toolbox/version.py
--rw-r--r--   0        0        0     1122 2024-04-30 20:45:10.401205 inspyre_toolbox-1.4.1/LICENSE
--rw-r--r--   0        0        0     1636 2024-04-30 20:57:32.686977 inspyre_toolbox-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 inspyre_toolbox-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0      209 2024-04-30 20:45:10.403940 inspyre_toolbox-1.4.2/inspyre_toolbox/__about__.py
+-rw-r--r--   0        0        0     2639 2024-04-30 20:44:59.194115 inspyre_toolbox-1.4.2/inspyre_toolbox/__init__.py
+-rw-r--r--   0        0        0       16 2024-04-30 20:45:10.403940 inspyre_toolbox-1.4.2/inspyre_toolbox/api_changes.ini
+-rw-r--r--   0        0        0        0 2024-04-30 20:45:10.405306 inspyre_toolbox-1.4.2/inspyre_toolbox/cli/__init__.py
+-rw-r--r--   0        0        0     3005 2024-04-30 20:45:10.405306 inspyre_toolbox-1.4.2/inspyre_toolbox/cli/ist_bytes_converter/__init__.py
+-rw-r--r--   0        0        0     3388 2024-04-30 20:45:10.405306 inspyre_toolbox-1.4.2/inspyre_toolbox/cli/ist_bytes_converter/arguments.py
+-rw-r--r--   0        0        0     1425 2024-04-30 20:45:10.406705 inspyre_toolbox-1.4.2/inspyre_toolbox/cli/ist_bytes_converter/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:45:10.406705 inspyre_toolbox-1.4.2/inspyre_toolbox/common/__init__.py
+-rw-r--r--   0        0        0      931 2024-05-02 21:18:35.679690 inspyre_toolbox-1.4.2/inspyre_toolbox/common/meta.py
+-rw-r--r--   0        0        0     2808 2024-04-30 20:44:59.194115 inspyre_toolbox-1.4.2/inspyre_toolbox/console_kit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:44:59.195113 inspyre_toolbox-1.4.2/inspyre_toolbox/conversions/__init__.py
+-rw-r--r--   0        0        0     4240 2024-04-30 20:45:10.407939 inspyre_toolbox-1.4.2/inspyre_toolbox/conversions/bytes/__init__.py
+-rw-r--r--   0        0        0     5299 2024-04-30 20:45:10.407939 inspyre_toolbox-1.4.2/inspyre_toolbox/conversions/roman_numerals/__init__.py
+-rw-r--r--   0        0        0     1143 2024-04-30 20:44:59.196112 inspyre_toolbox-1.4.2/inspyre_toolbox/conversions/roman_numerals/errors.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:44:59.196112 inspyre_toolbox-1.4.2/inspyre_toolbox/core/errors/__init__.py
+-rw-r--r--   0        0        0     2636 2024-04-30 20:44:59.196112 inspyre_toolbox-1.4.2/inspyre_toolbox/core/errors/version.py
+-rw-r--r--   0        0        0       97 2024-04-30 20:44:59.197472 inspyre_toolbox-1.4.2/inspyre_toolbox/core_helpers/__init__.py
+-rw-r--r--   0        0        0      424 2024-04-30 20:44:59.197472 inspyre_toolbox-1.4.2/inspyre_toolbox/core_helpers/debugging.py
+-rw-r--r--   0        0        0     4065 2024-04-30 20:45:10.409300 inspyre_toolbox-1.4.2/inspyre_toolbox/core_helpers/logging.py
+-rw-r--r--   0        0        0     1951 2024-04-30 20:45:10.409300 inspyre_toolbox-1.4.2/inspyre_toolbox/docs/conversions/bytes.md
+-rw-r--r--   0        0        0     3413 2024-04-30 20:45:10.410790 inspyre_toolbox-1.4.2/inspyre_toolbox/generations/__init__.py
+-rw-r--r--   0        0        0    22944 2024-04-30 20:45:10.410790 inspyre_toolbox-1.4.2/inspyre_toolbox/humanize/__init__.py
+-rw-r--r--   0        0        0      262 2024-04-30 20:44:59.198686 inspyre_toolbox-1.4.2/inspyre_toolbox/humanize/errors/__init__.py
+-rw-r--r--   0        0        0     1927 2024-04-30 20:44:59.199745 inspyre_toolbox-1.4.2/inspyre_toolbox/humanize/errors/numerical.py
+-rw-r--r--   0        0        0    10359 2024-05-02 22:55:50.816773 inspyre_toolbox-1.4.2/inspyre_toolbox/live_timer/__init__.py
+-rw-r--r--   0        0        0     1100 2024-04-30 20:44:59.200756 inspyre_toolbox-1.4.2/inspyre_toolbox/live_timer/errors.py
+-rw-r--r--   0        0        0     2596 2024-05-02 22:30:57.895734 inspyre_toolbox-1.4.2/inspyre_toolbox/live_timer/history.py
+-rw-r--r--   0        0        0    11458 2024-04-30 20:45:10.412229 inspyre_toolbox-1.4.2/inspyre_toolbox/proc_man/__init__.py
+-rw-r--r--   0        0        0      689 2024-04-30 20:44:59.202755 inspyre_toolbox-1.4.2/inspyre_toolbox/proc_man/errors.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:44:59.202755 inspyre_toolbox-1.4.2/inspyre_toolbox/pypi/__init__.py
+-rw-r--r--   0        0        0      900 2024-04-30 20:44:59.203757 inspyre_toolbox-1.4.2/inspyre_toolbox/pypi/packages.py
+-rw-r--r--   0        0        0      596 2024-04-30 20:44:59.203757 inspyre_toolbox-1.4.2/inspyre_toolbox/settings.py
+-rw-r--r--   0        0        0     1868 2024-04-30 20:45:10.412229 inspyre_toolbox-1.4.2/inspyre_toolbox/solve_kit/__init__.py
+-rw-r--r--   0        0        0      175 2024-04-30 20:44:59.204758 inspyre_toolbox-1.4.2/inspyre_toolbox/spanners/__init__.py
+-rw-r--r--   0        0        0     2210 2024-04-30 20:44:59.204758 inspyre_toolbox-1.4.2/inspyre_toolbox/spanners/span_arg_parse.py
+-rw-r--r--   0        0        0     1014 2024-04-30 20:44:59.204758 inspyre_toolbox-1.4.2/inspyre_toolbox/syntactic_sweets/__init__.py
+-rw-r--r--   0        0        0     2265 2024-04-30 20:44:59.205757 inspyre_toolbox-1.4.2/inspyre_toolbox/sys_man/__init__.py
+-rw-r--r--   0        0        0     6999 2024-04-30 20:45:10.413573 inspyre_toolbox-1.4.2/inspyre_toolbox/version.py
+-rw-r--r--   0        0        0     1122 2024-04-30 20:45:10.401205 inspyre_toolbox-1.4.2/LICENSE
+-rw-r--r--   0        0        0     1636 2024-05-02 22:37:50.192362 inspyre_toolbox-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 inspyre_toolbox-1.4.2/PKG-INFO
```

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/__init__.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/cli/ist_bytes_converter/__init__.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/cli/ist_bytes_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/cli/ist_bytes_converter/arguments.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/cli/ist_bytes_converter/arguments.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/cli/ist_bytes_converter/helpers.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/cli/ist_bytes_converter/helpers.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/common/meta.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/common/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 
 
 URLS = dict(
     developer_url='https://inspyre.tech',
     docs_url='https://inspyre-toolbox.readthedocs.io/en/latest',
     github_url='https://github.com/tayjaybabee/Inspyre-Toolbox',
-    pypi_url='https://pypi.org/project/inspyre-toolbox',
+    pypi_url='https://pypi.org/pypi/inspyre-toolbox',
 )
 """The URLs used in the project."""
 
 
 AUTHORS = [
     ('Inspyre-Softworks', URLS['developer_url']),
     ('Taylor-Jayde Blackstone', '<t.blackstone@inspyre.tech>')
@@ -31,12 +31,12 @@
 }
 """The release map for the project."""
 
 
 VERSION = {
     'major': 1,
     'minor': 4,
-    'patch': 1,
+    'patch': 2,
     'release': 'final',
     'release_num': 0
 }
 """The version information for the project."""
```

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/console_kit/__init__.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/console_kit/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/conversions/bytes/__init__.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/conversions/bytes/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/conversions/roman_numerals/__init__.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/conversions/roman_numerals/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/conversions/roman_numerals/errors.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/conversions/roman_numerals/errors.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/core/errors/version.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/core/errors/version.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/core_helpers/logging.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/core_helpers/logging.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/docs/conversions/bytes.md` & `inspyre_toolbox-1.4.2/inspyre_toolbox/docs/conversions/bytes.md`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/generations/__init__.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/humanize/__init__.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/humanize/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/humanize/errors/numerical.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/humanize/errors/numerical.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/live_timer/__init__.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/live_timer/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,21 @@
     
     GIT_REPO_ROOT/examples/live_timer
 
 """
 
 from time import time
 
-from inspyre_toolbox.core_helpers.logging import ROOT_ISL_DEVICE, add_isl_child
+from inspy_logger import Loggable
+
+from inspyre_toolbox.core_helpers.logging import add_isl_child
 from inspyre_toolbox.live_timer.errors import TimerNotRunningError, TimerNotStartedError
 from inspyre_toolbox.live_timer.history import TimerHistory
 
-LOG_NAME = 'InspyreToolbox.live_timer'
+LOG_NAME = 'live_timer'
 
 LOG = add_isl_child(LOG_NAME)
 
 #ROOT_ISL_DEVICE.adjust_level('debug')
 
 LOG.debug('Log started!')
 
@@ -43,50 +45,83 @@
     hours = seconds // (60 * 60)
     seconds %= (60 * 60)
     minutes = seconds // 60
     seconds %= 60
     return "%02i:%02i:%02i" % (hours, minutes, seconds)
 
 
-class Timer(object):
+class Timer(Loggable):
     def __repr__(self):
-        statement = "Timer(" \
-                    f"Started: {self.started} |"
+        """
+        Return a string representation of the Timer object.
+
+        Returns:
+            str: A formatted string representing the Timer object.
+        """
+        status = "Running" if self.running else "Stopped"
+        state = "Paused" if self.paused else "Not Paused"
+        start_info = f"Started at: {self.start_time}" if self.started else "Not Started"
+        runtime_info = ""
         if self.started:
             runtime = time() - self.start_time
-            runtime = format_seconds_to_hhmmss(runtime)
-            statement += f" Started: {self.start_time} - Current Runtime: {runtime}"
+            runtime_info = f" | Runtime: {format_seconds_to_hhmmss(runtime)}"
+        return f"Timer(Status: {status} | State: {state} | {start_info}{runtime_info})"
 
     def __init__(self, auto_start=False, history=None):
+        super().__init__(parent_log_device=LOG)
+
+        self.log = self.class_logger
 
-        self.log_name = f'{LOG_NAME}.Timer'
+        self.__auto_start = False
+        self._status = 'Stopped'
 
-        # Set up logger
-        self.log = add_isl_child(self.log_name)
+        self.class_logger.debug('Setting up Timer class attributes...')
 
         # Define some default attribute values
 
         self.running = False
         self.mark_2 = None
         self.pause_end = None
         self.pause_start = time()
         self.paused = False
         self.start_time = None
         self.started = False
+
         self.stopped = False
         self.total_pause_time = 0
         self.was_paused = False
 
         self.log.debug('Set up class attributes.')
 
         # Start a Timer history object to track times for resets
         self.history = TimerHistory(self.__get_elapsed) if history is None else history
 
         self.log.debug('Timer class instantiated!')
 
+        self.auto_start = auto_start
+
+    @property
+    def auto_start(self):
+        return self.__auto_start
+
+    @auto_start.setter
+    def auto_start(self, new: bool):
+        if new and not self.started:
+            self.start()
+
+        self.__auto_start = new
+
+    @property
+    def elapsed(self):
+        return self.get_elapsed(seconds=True)
+
+    @property
+    def num_resets(self):
+        return self.history.num_resets
+
     def __get_elapsed(self, ts=None, sans_pause: bool = False, seconds=False):
         """
         The __get_elapsed function is a private function that is called by the public functions
         start(), pause(), and stop(). It returns the elapsed time in seconds, or as a string if
         seconds=False. The __get_elapsed function does not take any parameters. If you call this
         private function directly, it will return an error
 
@@ -104,15 +139,15 @@
             seconds (bool):
                 Return the elapsed time as number of seconds. (Optional; defaults
                 to False)
 
         Returns:
             The time elapsed since the start of the timer
         """
-        log = add_isl_child(f'{self.log_name}__get_elapsed')
+        log = self.create_child_logger()
 
         diff_time = self.start_time if ts is None else ts
 
         # ver1.2.7
         # If we were running but are now stopped, we will skip marking
         if not self.stopped:
             self.mark_2 = time()
@@ -171,23 +206,26 @@
         # self.total_pause_time = 0
         # self.pause_start = None
         # self.pause_end = None
         # self.started = False
 
     def restart(self):
         """
-        The restart function resets the timer to its original state and starts it
-        running.
+        The restart function resets the timer to its original state and starts it running.
+
+        This method modifies the current instance instead of creating a new one.
 
         Returns:
             None
         """
         self.reset()
         if not self.started:
             self.start()
+        # Update the current instance instead of creating a new one
+        self.__dict__.update(Timer(history=self.history).__dict__)
 
     def start(self):
         """
 
         Store the time the thread was started and assign the attribute 'self.started' to 'True' to indicate this.
 
         """
```

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/live_timer/errors.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/live_timer/errors.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/live_timer/history.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/live_timer/history.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,25 @@
                 "UNPAUSE",
                 "RESET",
                 "CREATE",
                 "QUERY"
         ]
         self.add("CREATE")
 
+    @property
+    def num_resets(self) -> int:
+        """
+        Get the number of times the timer has been reset
+
+        Returns:
+            The number of times the timer has been reset
+
+        """
+        return len([entry for entry in self.ledger if entry['action'] == "RESET"])
+
     def add(self, action: str = "START") -> dict:
         """
         The add function adds a new entry to the ledger.
 
         Args:
             self:
                 Refer to the object instance
```

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/proc_man/__init__.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/proc_man/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/proc_man/errors.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/proc_man/errors.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/pypi/packages.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/pypi/packages.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/settings.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/settings.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/solve_kit/__init__.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/solve_kit/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/spanners/span_arg_parse.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/spanners/span_arg_parse.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/syntactic_sweets/__init__.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/syntactic_sweets/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/sys_man/__init__.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/sys_man/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/inspyre_toolbox/version.py` & `inspyre_toolbox-1.4.2/inspyre_toolbox/version.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/LICENSE` & `inspyre_toolbox-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.1/pyproject.toml` & `inspyre_toolbox-1.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "inspyre-toolbox"
-version = "v1.4.1"
+version = "v1.4.2"
 description = "A toolbox containing some useful tools for Inspyre Softworks packages. Generally useful to some programmers too."
 authors = [ "T Blackstone <t.blackstone@inspyre.tech>",]
 license = "MIT"
 classifiers = [ "Intended Audience :: Developers", "License :: OSI Approved :: MIT License", "Natural Language :: English", "Operating System :: OS Independent", "Programming Language :: Python :: 3", "Programming Language :: Python :: 3.6", "Programming Language :: Python :: 3.7", "Programming Language :: Python :: 3.8", "Programming Language :: Python :: 3.9", "Programming Language :: Python :: 3 :: Only", "Topic :: Scientific/Engineering :: Mathematics", "Topic :: Software Development", "Topic :: Software Development :: Build Tools", "Topic :: Software Development :: Libraries :: Python Modules", "Topic :: Terminals", "Topic :: Utilities",]
 keywords = [ "toolbox", "timer", "commify", "strings", "elapsed",]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 inflect = "^5.3.0"
 psutil = "^5.8.0"
 DateTime = "^4.3"
 pypattyrn = "^1.2"
 tqdm = "^4.64.0"
 inspyred-print = "^1.2.1"
-inspy-logger = "3.0.2.dev1"
+inspy-logger = "3.1.0.dev3"
 
 [tool.poetry.scripts]
 ist-bytes-converter = "inspyre_toolbox.cli.ist_bytes_converter:main"
 
 [tool.poetry.group.dev.dependencies]
 ptipython = "^1.0.1"
 prompt-toolkit = "^3.0.43"
```

### Comparing `inspyre_toolbox-1.4.1/PKG-INFO` & `inspyre_toolbox-1.4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspyre-toolbox
-Version: 1.4.1
+Version: 1.4.2
 Summary: A toolbox containing some useful tools for Inspyre Softworks packages. Generally useful to some programmers too.
 License: MIT
 Keywords: toolbox,timer,commify,strings,elapsed
 Author: T Blackstone
 Author-email: t.blackstone@inspyre.tech
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
@@ -24,12 +24,12 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
 Requires-Dist: DateTime (>=4.3,<5.0)
 Requires-Dist: inflect (>=5.3.0,<6.0.0)
-Requires-Dist: inspy-logger (==3.0.2.dev1)
+Requires-Dist: inspy-logger (==3.1.0.dev3)
 Requires-Dist: inspyred-print (>=1.2.1,<2.0.0)
 Requires-Dist: psutil (>=5.8.0,<6.0.0)
 Requires-Dist: pypattyrn (>=1.2,<2.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
```


# Comparing `tmp/zdaemon-5.0.tar.gz` & `tmp/zdaemon-5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zdaemon-5.0.tar", last modified: Wed May 24 06:09:28 2023, max compression
+gzip compressed data, was "zdaemon-5.1.tar", last modified: Fri May  3 05:29:00 2024, max compression
```

## Comparing `zdaemon-5.0.tar` & `zdaemon-5.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-24 06:09:28.797851 zdaemon-5.0/
--rw-r--r--   0 mac        (513) staff       (20)      564 2023-05-24 06:09:28.000000 zdaemon-5.0/.coveragerc
--rw-r--r--   0 mac        (513) staff       (20)     8818 2023-05-24 06:09:28.000000 zdaemon-5.0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      808 2023-05-24 06:09:28.000000 zdaemon-5.0/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2023-05-24 06:09:28.000000 zdaemon-5.0/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2023-05-24 06:09:28.000000 zdaemon-5.0/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      305 2023-05-24 06:09:28.000000 zdaemon-5.0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)    25325 2023-05-24 06:09:28.798005 zdaemon-5.0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      298 2023-05-24 06:09:28.000000 zdaemon-5.0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      454 2023-05-24 06:09:28.798541 zdaemon-5.0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     2484 2023-05-24 06:09:28.000000 zdaemon-5.0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-24 06:09:28.785110 zdaemon-5.0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-24 06:09:28.792288 zdaemon-5.0/src/zdaemon/
--rw-r--r--   0 mac        (513) staff       (20)    15160 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      701 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       40 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/__main__.py
--rw-r--r--   0 mac        (513) staff       (20)    12245 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/component.xml
--rw-r--r--   0 mac        (513) staff       (20)      437 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/sample.conf
--rw-r--r--   0 mac        (513) staff       (20)     1010 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/schema.xml
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-24 06:09:28.797584 zdaemon-5.0/src/zdaemon/tests/
--rw-r--r--   0 mac        (513) staff       (20)       46 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/tests/__init__.py
--rwxr-xr-x   0 mac        (513) staff       (20)      118 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/tests/nokill.py
--rw-r--r--   0 mac        (513) staff       (20)     1563 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/tests/parent.py
--rw-r--r--   0 mac        (513) staff       (20)    12093 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/tests/tests.py
--rw-r--r--   0 mac        (513) staff       (20)     4050 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/tests/testuser.py
--rw-r--r--   0 mac        (513) staff       (20)     2459 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/tests/testzdctl.py
--rw-r--r--   0 mac        (513) staff       (20)    18007 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/tests/testzdoptions.py
--rw-r--r--   0 mac        (513) staff       (20)    15741 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/tests/testzdrun.py
--rwxr-xr-x   0 mac        (513) staff       (20)    21550 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/zdctl.py
--rw-r--r--   0 mac        (513) staff       (20)    18841 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/zdoptions.py
--rwxr-xr-x   0 mac        (513) staff       (20)    25450 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/zdrun.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-24 06:09:28.794869 zdaemon-5.0/src/zdaemon.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)    25325 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      812 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)       47 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon.egg-info/entry_points.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)       86 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        8 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1173 2023-05-24 06:09:28.000000 zdaemon-5.0/tox.ini
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:29:00.851274 zdaemon-5.1/
+-rw-r--r--   0 jens       (501) staff       (20)      564 2024-05-02 20:43:59.000000 zdaemon-5.1/.coveragerc
+-rw-r--r--   0 jens       (501) staff       (20)     9061 2024-05-03 05:22:32.000000 zdaemon-5.1/CHANGES.rst
+-rw-r--r--   0 jens       (501) staff       (20)      808 2024-05-02 20:43:59.000000 zdaemon-5.1/CONTRIBUTING.md
+-rw-r--r--   0 jens       (501) staff       (20)       32 2021-11-02 08:53:15.000000 zdaemon-5.1/COPYRIGHT.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2070 2021-11-02 08:53:15.000000 zdaemon-5.1/LICENSE.txt
+-rw-r--r--   0 jens       (501) staff       (20)      305 2024-05-02 20:43:59.000000 zdaemon-5.1/MANIFEST.in
+-rw-r--r--   0 jens       (501) staff       (20)    25887 2024-05-03 05:29:00.851188 zdaemon-5.1/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)      298 2021-11-02 08:53:15.000000 zdaemon-5.1/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)      425 2024-05-03 05:29:00.851485 zdaemon-5.1/setup.cfg
+-rw-r--r--   0 jens       (501) staff       (20)     2534 2024-05-03 05:22:41.000000 zdaemon-5.1/setup.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:29:00.846664 zdaemon-5.1/src/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:29:00.848905 zdaemon-5.1/src/zdaemon/
+-rw-r--r--   0 jens       (501) staff       (20)    15160 2021-11-02 08:53:15.000000 zdaemon-5.1/src/zdaemon/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)      701 2021-11-02 08:53:15.000000 zdaemon-5.1/src/zdaemon/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)       40 2023-04-20 08:27:23.000000 zdaemon-5.1/src/zdaemon/__main__.py
+-rw-r--r--   0 jens       (501) staff       (20)    12245 2021-11-02 08:53:15.000000 zdaemon-5.1/src/zdaemon/component.xml
+-rw-r--r--   0 jens       (501) staff       (20)      437 2021-11-02 08:53:15.000000 zdaemon-5.1/src/zdaemon/sample.conf
+-rw-r--r--   0 jens       (501) staff       (20)     1010 2021-11-02 08:53:15.000000 zdaemon-5.1/src/zdaemon/schema.xml
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:29:00.850537 zdaemon-5.1/src/zdaemon/tests/
+-rw-r--r--   0 jens       (501) staff       (20)       46 2021-11-02 08:53:15.000000 zdaemon-5.1/src/zdaemon/tests/__init__.py
+-rwxr-xr-x   0 jens       (501) staff       (20)      118 2023-04-20 08:27:23.000000 zdaemon-5.1/src/zdaemon/tests/nokill.py
+-rw-r--r--   0 jens       (501) staff       (20)     1563 2023-04-20 08:27:23.000000 zdaemon-5.1/src/zdaemon/tests/parent.py
+-rw-r--r--   0 jens       (501) staff       (20)    13139 2024-05-03 05:13:42.000000 zdaemon-5.1/src/zdaemon/tests/tests.py
+-rw-r--r--   0 jens       (501) staff       (20)     4050 2023-08-01 09:36:32.000000 zdaemon-5.1/src/zdaemon/tests/testuser.py
+-rw-r--r--   0 jens       (501) staff       (20)     2459 2021-11-02 08:53:15.000000 zdaemon-5.1/src/zdaemon/tests/testzdctl.py
+-rw-r--r--   0 jens       (501) staff       (20)    18007 2023-08-01 09:36:32.000000 zdaemon-5.1/src/zdaemon/tests/testzdoptions.py
+-rw-r--r--   0 jens       (501) staff       (20)    15741 2023-08-01 09:36:32.000000 zdaemon-5.1/src/zdaemon/tests/testzdrun.py
+-rwxr-xr-x   0 jens       (501) staff       (20)    21550 2023-08-01 09:36:32.000000 zdaemon-5.1/src/zdaemon/zdctl.py
+-rw-r--r--   0 jens       (501) staff       (20)    18841 2023-08-01 09:36:32.000000 zdaemon-5.1/src/zdaemon/zdoptions.py
+-rwxr-xr-x   0 jens       (501) staff       (20)    27648 2024-05-03 05:13:42.000000 zdaemon-5.1/src/zdaemon/zdrun.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:29:00.850679 zdaemon-5.1/src/zdaemon.egg-info/
+-rw-r--r--   0 jens       (501) staff       (20)    25887 2024-05-03 05:29:00.000000 zdaemon-5.1/src/zdaemon.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)      812 2024-05-03 05:29:00.000000 zdaemon-5.1/src/zdaemon.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2024-05-03 05:29:00.000000 zdaemon-5.1/src/zdaemon.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (501) staff       (20)       47 2024-05-03 05:29:00.000000 zdaemon-5.1/src/zdaemon.egg-info/entry_points.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2024-05-02 20:44:02.000000 zdaemon-5.1/src/zdaemon.egg-info/not-zip-safe
+-rw-r--r--   0 jens       (501) staff       (20)       86 2024-05-03 05:29:00.000000 zdaemon-5.1/src/zdaemon.egg-info/requires.txt
+-rw-r--r--   0 jens       (501) staff       (20)        8 2024-05-03 05:29:00.000000 zdaemon-5.1/src/zdaemon.egg-info/top_level.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1578 2024-05-03 05:13:42.000000 zdaemon-5.1/tox.ini
```

### Comparing `zdaemon-5.0/.coveragerc` & `zdaemon-5.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `zdaemon-5.0/CHANGES.rst` & `zdaemon-5.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 ==========
 Change log
 ==========
 
+5.1 (2024-05-03)
+================
+
+- Add support for Python 3.12.
+
+- Fix ``SIGCHLD``/``wait`` raise condition associated with the
+  ``start-test-program`` option.
+  For details see `#33 <https://github.com/zopefoundation/zdaemon/pull/33>`_.
+
+
 5.0 (2023-05-24)
 ================
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 
 4.4 (2022-12-02)
```

### Comparing `zdaemon-5.0/CONTRIBUTING.md` & `zdaemon-5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zdaemon-5.0/LICENSE.txt` & `zdaemon-5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zdaemon-5.0/PKG-INFO` & `zdaemon-5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zdaemon
-Version: 5.0
+Version: 5.1
 Summary: Daemon process control library and tools for Unix-based systems
 Home-page: https://github.com/zopefoundation/zdaemon
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -12,21 +12,29 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
-Provides-Extra: test
 License-File: LICENSE.txt
+Requires-Dist: ZConfig
+Requires-Dist: setuptools
+Provides-Extra: test
+Requires-Dist: manuel; extra == "test"
+Requires-Dist: mock; extra == "test"
+Requires-Dist: zc.customdoctests; extra == "test"
+Requires-Dist: zope.testing; extra == "test"
+Requires-Dist: zope.testrunner; extra == "test"
 
 *****************************************************
 ``zdaemon`` process controller for Unix-based systems
 *****************************************************
 
 ``zdaemon`` is a Unix (Unix, Linux, Mac OS X) Python program that wraps
 commands to make them behave as proper daemons.
@@ -560,14 +568,24 @@
 Log output from zdaemon usually isn't very interesting but can be
 handy for debugging.
 
 ==========
 Change log
 ==========
 
+5.1 (2024-05-03)
+================
+
+- Add support for Python 3.12.
+
+- Fix ``SIGCHLD``/``wait`` raise condition associated with the
+  ``start-test-program`` option.
+  For details see `#33 <https://github.com/zopefoundation/zdaemon/pull/33>`_.
+
+
 5.0 (2023-05-24)
 ================
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 
 4.4 (2022-12-02)
```

### Comparing `zdaemon-5.0/setup.py` & `zdaemon-5.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 def read(*rnames):
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
 setup(
     name="zdaemon",
-    version='5.0',
+    version='5.1',
     url="https://github.com/zopefoundation/zdaemon",
     license="ZPL 2.1",
     description="Daemon process control library and tools for Unix-based systems",  # noqa: E501 line too long
     author="Zope Foundation and Contributors",
     author_email="zope-dev@zope.dev",
     long_description=(
         read('README.rst') +
@@ -61,14 +61,15 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Operating System :: POSIX',
         'Topic :: Utilities',
     ],
     zip_safe=False,
     entry_points=entry_points,
```

### Comparing `zdaemon-5.0/src/zdaemon/README.rst` & `zdaemon-5.1/src/zdaemon/README.rst`

 * *Files identical despite different names*

### Comparing `zdaemon-5.0/src/zdaemon/__init__.py` & `zdaemon-5.1/src/zdaemon/__init__.py`

 * *Files identical despite different names*

### Comparing `zdaemon-5.0/src/zdaemon/component.xml` & `zdaemon-5.1/src/zdaemon/component.xml`

 * *Files identical despite different names*

### Comparing `zdaemon-5.0/src/zdaemon/schema.xml` & `zdaemon-5.1/src/zdaemon/schema.xml`

 * *Files identical despite different names*

### Comparing `zdaemon-5.0/src/zdaemon/tests/parent.py` & `zdaemon-5.1/src/zdaemon/tests/parent.py`

 * *Files identical despite different names*

### Comparing `zdaemon-5.0/src/zdaemon/tests/tests.py` & `zdaemon-5.1/src/zdaemon/tests/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,36 @@
 
 
 def read(name):
     with open(name) as f:
         return f.read()
 
 
+def test_ChildExits():
+    """
+    ``_ChildExits`` is used to record the exit status for a
+    foreign process when it was captured by the ``SIGCHLD``handler
+    due to a race condition.
+
+    >>> from zdaemon.zdrun import _ChildExits
+    >>> exits = _ChildExits()
+
+    Initially, we have no exit status for a process.
+    >>> exits.fetch(5)
+
+    After we have recorded exit information, ``fetch`` will
+    retrieve and reset it.
+    >>> exits[5] = 0
+    >>> exits.fetch(5)
+    0
+    >>> exits.fetch(5)
+
+    """
+
+
 def make_sure_non_daemon_mode_doesnt_hang_when_program_exits():
     """
     The whole awhile bit that waits for a program to start
     whouldn't be used on non-daemon mode.
 
     >>> write('conf',
     ... '''
@@ -269,43 +291,66 @@
 
 
 def test_start_test_program():
     """
     >>> write('t.py',
     ... '''
     ... import time
-    ... time.sleep(1)
+    ... time.sleep(2)
     ... open('x', 'w').close()
     ... time.sleep(99)
     ... ''')
 
     >>> write('conf',
     ... '''
     ... <runner>
     ...   program %s t.py
     ...   start-test-program cat x
+    ...   daemon on
     ... </runner>
+    ... <eventlog>
+    ...   level debug
+    ...   <logfile>
+    ...      path log
+    ...      level debug
+    ...   </logfile>
+    ... </eventlog>
     ... ''' % sys.executable)
 
     >>> import os
 
     >>> system("./zdaemon -Cconf start")
     . .
     daemon process started, pid=21446
 
     >>> os.path.exists('x')
     True
     >>> os.remove('x')
 
+    >>> with open("log") as f:
+    ...   logged = f.read()
+    >>> nfailed = logged.count("start test failed")
+    >>> nfailed > 0
+    True
+    >>> logged.count("start test succeeded")
+    1
+
     >>> system("./zdaemon -Cconf restart")
     . . .
     daemon process restarted, pid=19622
     >>> os.path.exists('x')
     True
 
+    >>> with open("log") as f:
+    ...   logged = f.read()
+    >>> nfailed < logged.count("start test failed")
+    True
+    >>> logged.count("start test succeeded")
+    2
+
     >>> system("./zdaemon -Cconf stop")
     <BLANKLINE>
     daemon process stopped
     """
 
 
 def test_start_timeout():
```

### Comparing `zdaemon-5.0/src/zdaemon/tests/testuser.py` & `zdaemon-5.1/src/zdaemon/tests/testuser.py`

 * *Files identical despite different names*

### Comparing `zdaemon-5.0/src/zdaemon/tests/testzdctl.py` & `zdaemon-5.1/src/zdaemon/tests/testzdctl.py`

 * *Files identical despite different names*

### Comparing `zdaemon-5.0/src/zdaemon/tests/testzdoptions.py` & `zdaemon-5.1/src/zdaemon/tests/testzdoptions.py`

 * *Files identical despite different names*

### Comparing `zdaemon-5.0/src/zdaemon/tests/testzdrun.py` & `zdaemon-5.1/src/zdaemon/tests/testzdrun.py`

 * *Files identical despite different names*

### Comparing `zdaemon-5.0/src/zdaemon/zdctl.py` & `zdaemon-5.1/src/zdaemon/zdctl.py`

 * *Files identical despite different names*

### Comparing `zdaemon-5.0/src/zdaemon/zdoptions.py` & `zdaemon-5.1/src/zdaemon/zdoptions.py`

 * *Files identical despite different names*

### Comparing `zdaemon-5.0/src/zdaemon/zdrun.py` & `zdaemon-5.1/src/zdaemon/zdrun.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self.schemafile = file
 
     def realize(self, *args, **kwds):
         RunnerOptions.realize(self, *args, **kwds)
         if self.args:
             self.program = self.args
         if not self.program:
-            self.usage("no program specified (use -C or positional args)")
+            self.usage("no program specified (use positional args)")
         if self.sockname:
             # Convert socket name to absolute path
             self.sockname = os.path.abspath(self.sockname)
         if self.config_logger is None:
             # This doesn't perform any configuration of the logging
             # package, but that's reasonable in this case.
             self.logger = logging.getLogger()
@@ -105,27 +105,28 @@
 
     """A class to manage a subprocess."""
 
     # Initial state; overridden by instance variables
     pid = 0  # Subprocess pid; 0 when not running
     lasttime = 0  # Last time the subprocess was started; 0 if never
 
-    def __init__(self, options, args=None):
+    def __init__(self, options, args=None, child_exits=None):
         """Constructor.
 
         Arguments are a ZDRunOptions instance and a list of program
         arguments; the latter's first item must be the program name.
         """
         if args is None:
             args = options.args
         if not args:
             options.usage("missing 'program' argument")
         self.options = options
         self.args = args
         self.testing = set()
+        self.child_exits = child_exits
         self._set_filename(args[0])
 
     def _set_filename(self, program):
         """Internal: turn a program name into a file name, using $PATH."""
         if "/" in program:
             filename = program
             try:
@@ -148,18 +149,37 @@
                                    (program, path))
         if not os.access(filename, os.X_OK):
             self.options.usage("no permission to run program %r" % filename)
         self.filename = filename
 
     def test(self, pid):
         starttestprogram = self.options.starttestprogram
+        logger = self.options.logger
         try:
             while self.pid == pid:
-                if not subprocess.call(starttestprogram):
-                    break
+                try:
+                    with subprocess.Popen(starttestprogram) as p:
+                        # uncomment the following line to force
+                        # (for testing purposes) a race between
+                        # the ``wait`` below and the ``SIGCHLD`` handler
+                        # import time; time.sleep(0.01)
+                        sts = p.wait()
+                        # ``sts`` is usually the return status.
+                        # However, the true return status may have been
+                        # captured by the ``SIGCHLD`` handler.
+                        # In this case, ``str == 0`` and the
+                        # true return status can be found via ``child_exits``.
+                        if not sts and not self.child_exits.fetch(p.pid):
+                            logger.debug("start test succeeded")
+                            break
+                        logger.debug("start test failed")
+                except Exception:  # pragma: nocover
+                    logger.critical("start test raised",
+                                    exc_info=True)
+                    break  # likely a permanent error
                 time.sleep(1)
         finally:
             self.testing.remove(pid)
 
     def spawn(self):
         """Start the subprocess.  It must not be running already.
 
@@ -230,21 +250,25 @@
     def main(self, args=None):
         self.options = ZDRunOptions()
         self.options.realize(args)
         self.logger = self.options.logger
         self.run()
 
     def run(self):
-        self.proc = Subprocess(self.options)
+        self.child_exits = _ChildExits()
+        self.proc = Subprocess(self.options, child_exits=self.child_exits)
         self.opensocket()
         try:
             self.setsignals()
             if self.options.daemon:
                 self.daemonize()
-            self.runforever()
+            try:
+                self.runforever()
+            except Exception:  # pragma: nocover
+                self.logger.critical("runforever raised", exc_info=True)
         finally:
             try:
                 os.unlink(self.options.sockname)
             except os.error:
                 pass
 
     mastersocket = None
@@ -322,15 +346,24 @@
 
     def sigchild(self, sig, frame):
         try:
             pid, sts = os.waitpid(-1, os.WNOHANG)
         except os.error:
             return
         if pid:
-            self.waitstatus = pid, sts
+            if pid == self.proc.pid:
+                self.logger.debug("controlled process %s exited", pid)
+                self.waitstatus = pid, sts
+            else:  # pragma: nocover
+                # this indicates a race between this ``SIGCHLD`` handler
+                # and a ``wait``.
+                # Record in ``child_exits`` to allow the ``wait`` caller
+                # to get the correct exit status
+                self.logger.debug("unknown process %s exited", pid)
+                self.child_exits[pid] = sts
 
     transcript = None
 
     def daemonize(self):
 
         # To daemonize, we need to become the leader of our own session
         # (process) group.  If we do not, signals sent to our
@@ -443,15 +476,15 @@
 
     def reportstatus(self):
         pid, sts = self.waitstatus
         self.waitstatus = None
         es, msg = decode_wait_status(sts)
         msg = "pid %d: " % pid + msg
         if pid != self.proc.pid:
-            msg = "unknown " + msg
+            msg = "unknown(!=%s) " % self.proc.pid + msg
             self.logger.warn(msg)
         else:
             killing = self.killing
             if killing:
                 self.killing = 0
                 self.delay = 0
             else:
@@ -728,14 +761,25 @@
     if "PATH" in os.environ:
         p = os.environ["PATH"]
         if p:
             path = p.split(os.pathsep)
     return path
 
 
+class _ChildExits(dict):
+    """map ``pid`` to exit status or ``None``."""
+    def fetch(self, pid):
+        """fetch and reset status for *pid*."""
+        st = self.get(pid)
+        if st is not None:
+            # there is only a negligable race risk
+            del self[pid]
+        return st
+
+
 # Main program
 
 def main(args=None):
     assert os.name == "posix", "This code makes many Unix-specific assumptions"
 
     d = Daemonizer()
     d.main(args)
```

### Comparing `zdaemon-5.0/src/zdaemon.egg-info/PKG-INFO` & `zdaemon-5.1/src/zdaemon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zdaemon
-Version: 5.0
+Version: 5.1
 Summary: Daemon process control library and tools for Unix-based systems
 Home-page: https://github.com/zopefoundation/zdaemon
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -12,21 +12,29 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
-Provides-Extra: test
 License-File: LICENSE.txt
+Requires-Dist: ZConfig
+Requires-Dist: setuptools
+Provides-Extra: test
+Requires-Dist: manuel; extra == "test"
+Requires-Dist: mock; extra == "test"
+Requires-Dist: zc.customdoctests; extra == "test"
+Requires-Dist: zope.testing; extra == "test"
+Requires-Dist: zope.testrunner; extra == "test"
 
 *****************************************************
 ``zdaemon`` process controller for Unix-based systems
 *****************************************************
 
 ``zdaemon`` is a Unix (Unix, Linux, Mac OS X) Python program that wraps
 commands to make them behave as proper daemons.
@@ -560,14 +568,24 @@
 Log output from zdaemon usually isn't very interesting but can be
 handy for debugging.
 
 ==========
 Change log
 ==========
 
+5.1 (2024-05-03)
+================
+
+- Add support for Python 3.12.
+
+- Fix ``SIGCHLD``/``wait`` raise condition associated with the
+  ``start-test-program`` option.
+  For details see `#33 <https://github.com/zopefoundation/zdaemon/pull/33>`_.
+
+
 5.0 (2023-05-24)
 ================
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 
 4.4 (2022-12-02)
```

### Comparing `zdaemon-5.0/src/zdaemon.egg-info/SOURCES.txt` & `zdaemon-5.1/src/zdaemon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zdaemon-5.0/tox.ini` & `zdaemon-5.1/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,59 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/buildout-recipe
 [tox]
 minversion = 3.18
 envlist =
+    release-check
     lint
     py37
     py38
     py39
     py310
     py311
+    py312
     pypy3
     coverage
 
 [testenv]
 usedevelop = true
 deps =
+setenv =
+    py312: VIRTUALENV_PIP=23.1.2
+    py312: PIP_REQUIRE_VIRTUALENV=0
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
 extras =
     test
+[testenv:release-check]
+description = ensure that the distribution is ready to release
+basepython = python3
+skip_install = true
+deps =
+    twine
+    build
+    check-manifest
+    check-python-versions >= 0.20.0
+    wheel
+commands_pre =
+commands =
+    check-manifest
+    check-python-versions --only setup.py,tox.ini,.github/workflows/tests.yml
+    python -m build --sdist --no-isolation
+    twine check dist/*
 
 [testenv:lint]
 basepython = python3
 skip_install = true
+deps =
+    isort
+    flake8
 commands =
     isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
     flake8 src setup.py
-    check-manifest
-    check-python-versions
-deps =
-    check-manifest
-    check-python-versions >= 0.19.1
-    wheel
-    flake8
-    isort
 
 [testenv:isort-apply]
 basepython = python3
 skip_install = true
 commands_pre =
 deps =
     isort
```


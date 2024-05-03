# Comparing `tmp/logging_tree-1.8.1.tar.gz` & `tmp/logging_tree-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/logging_tree-1.8.1.tar", last modified: Mon Jan 27 01:19:21 2020, max compression
+gzip compressed data, was "dist/logging_tree-1.9.tar", last modified: Sat Apr 10 10:08:26 2021, max compression
```

## Comparing `logging_tree-1.8.1.tar` & `logging_tree-1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2020-01-27 01:19:21.947834 logging_tree-1.8.1/
--rw-r-----   0 brandon   (1000) brandon   (1000)     1305 2019-08-14 22:44:22.538371 logging_tree-1.8.1/COPYRIGHT
--rw-r-----   0 brandon   (1000) brandon   (1000)     6604 2020-01-27 01:19:21.947834 logging_tree-1.8.1/PKG-INFO
-drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2020-01-27 01:19:21.947834 logging_tree-1.8.1/logging_tree/
--rw-r-----   0 brandon   (1000) brandon   (1000)     4659 2020-01-27 01:18:46.046597 logging_tree-1.8.1/logging_tree/__init__.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     6113 2019-08-14 22:44:22.542371 logging_tree-1.8.1/logging_tree/format.py
--rw-r-----   0 brandon   (1000) brandon   (1000)      791 2019-08-14 22:44:22.542371 logging_tree-1.8.1/logging_tree/nodes.py
-drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2020-01-27 01:19:21.947834 logging_tree-1.8.1/logging_tree/tests/
--rw-r-----   0 brandon   (1000) brandon   (1000)        0 2019-08-14 22:44:22.542371 logging_tree-1.8.1/logging_tree/tests/__init__.py
--rw-r-----   0 brandon   (1000) brandon   (1000)      450 2019-08-14 22:44:22.542371 logging_tree-1.8.1/logging_tree/tests/case.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     8219 2020-01-27 01:15:11.227196 logging_tree-1.8.1/logging_tree/tests/test_format.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     1408 2019-08-14 22:44:22.542371 logging_tree-1.8.1/logging_tree/tests/test_node.py
--rw-r-----   0 brandon   (1000) brandon   (1000)       26 2019-08-14 22:44:22.542371 logging_tree-1.8.1/setup.cfg
--rw-r-----   0 brandon   (1000) brandon   (1000)     1236 2020-01-27 01:15:59.128847 logging_tree-1.8.1/setup.py
+drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2021-04-10 10:08:26.663534 logging_tree-1.9/
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1305 2019-08-14 22:44:22.538371 logging_tree-1.9/COPYRIGHT
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)     7134 2021-04-10 10:08:26.663534 logging_tree-1.9/PKG-INFO
+drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2021-04-10 10:08:26.663534 logging_tree-1.9/logging_tree/
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)     5059 2021-04-10 10:07:11.335458 logging_tree-1.9/logging_tree/__init__.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     6480 2021-04-10 09:56:55.320950 logging_tree-1.9/logging_tree/format.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)      791 2019-08-14 22:44:22.542371 logging_tree-1.9/logging_tree/nodes.py
+drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2021-04-10 10:08:26.663534 logging_tree-1.9/logging_tree/tests/
+-rw-r-----   0 brandon   (1000) brandon   (1000)        0 2019-08-14 22:44:22.542371 logging_tree-1.9/logging_tree/tests/__init__.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)      575 2021-04-10 09:48:16.976343 logging_tree-1.9/logging_tree/tests/case.py
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)     7827 2021-04-10 09:52:42.975182 logging_tree-1.9/logging_tree/tests/test_format.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1408 2019-08-14 22:44:22.542371 logging_tree-1.9/logging_tree/tests/test_node.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)       26 2019-08-14 22:44:22.542371 logging_tree-1.9/setup.cfg
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)     1285 2021-04-10 08:26:36.120340 logging_tree-1.9/setup.py
```

### Comparing `logging_tree-1.8.1/COPYRIGHT` & `logging_tree-1.9/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `logging_tree-1.8.1/PKG-INFO` & `logging_tree-1.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: logging_tree
-Version: 1.8.1
+Version: 1.9
 Summary: Introspect and display the logger tree inside "logging"
 Home-page: https://github.com/brandon-rhodes/logging_tree
 Author: Brandon Rhodes
 Author-email: brandon@rhodesmill.org
 License: UNKNOWN
 Description: Introspection for the ``logging`` logger tree in the Standard Library.
         
@@ -33,14 +33,19 @@
                |       Level DEBUG
                |
                o<--[x]
                    |
                    o<--"x.c"
                        Level NOTSET so inherits level WARNING
         
+        If you instead want to write the tree diagram to a file, stream, or
+        other file-like object, use::
+        
+            file_object.write(logging_tree.format.build_description())
+        
         The logger tree should always print successfully, no matter how
         complicated.  A node whose ``[name]`` is in square brackets is a "place
         holder" that has never actually been named in a ``getLogger()`` call,
         but was created automatically to serve as the parent of loggers further
         down the tree.
         
         There are several interfaces that ``logging_tree`` supports, depending
@@ -81,14 +86,19 @@
         
         On older versions of Python you will instead have to install
         ``unittest2`` and use its ``unit2`` command line tool to run the tests.
         
         Changelog
         ---------
         
+        **Version 1.9** - 2021 April 10
+            Declare compatibility with Python 3.9.  Improve how the logging
+            module's built-in ``Formatter`` class is displayed under old Python
+            versions where the ``logging`` module uses old-style classes.
+        
         **Version 1.8.1** - 2020 January 26
             Adjust one test to make it pass under Python 3.8, and update the
             distribution classifiers to declare compatibility with Python
             versions through 3.8.
         
         **Version 1.8** - 2018 August 5
             Improve the output to better explain what happens if a "parent"
@@ -146,8 +156,9 @@
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Logging
```

### Comparing `logging_tree-1.8.1/logging_tree/__init__.py` & `logging_tree-1.9/logging_tree/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,19 @@
        |       Level DEBUG
        |
        o<--[x]
            |
            o<--"x.c"
                Level NOTSET so inherits level WARNING
 
+If you instead want to write the tree diagram to a file, stream, or
+other file-like object, use::
+
+    file_object.write(logging_tree.format.build_description())
+
 The logger tree should always print successfully, no matter how
 complicated.  A node whose ``[name]`` is in square brackets is a "place
 holder" that has never actually been named in a ``getLogger()`` call,
 but was created automatically to serve as the parent of loggers further
 down the tree.
 
 There are several interfaces that ``logging_tree`` supports, depending
@@ -73,14 +78,19 @@
 
 On older versions of Python you will instead have to install
 ``unittest2`` and use its ``unit2`` command line tool to run the tests.
 
 Changelog
 ---------
 
+**Version 1.9** - 2021 April 10
+    Declare compatibility with Python 3.9.  Improve how the logging
+    module's built-in ``Formatter`` class is displayed under old Python
+    versions where the ``logging`` module uses old-style classes.
+
 **Version 1.8.1** - 2020 January 26
     Adjust one test to make it pass under Python 3.8, and update the
     distribution classifiers to declare compatibility with Python
     versions through 3.8.
 
 **Version 1.8** - 2018 August 5
     Improve the output to better explain what happens if a "parent"
@@ -122,12 +132,12 @@
 **Version 0.6** - 2012 February 10
     Added a display format for every ``logging.handlers`` class.
 
 **Version 0.5** - 2012 February 8
     Initial release.
 
 """
-__version__ = '1.8.1'
+__version__ = '1.9'
 __all__ = ('tree', 'printout')
 
 from logging_tree.nodes import tree
 from logging_tree.format import printout
```

### Comparing `logging_tree-1.8.1/logging_tree/format.py` & `logging_tree-1.9/logging_tree/format.py`

 * *Files 6% similar despite different names*

```diff
@@ -152,19 +152,33 @@
     level = getattr(h, 'level', logging.NOTSET)
     if level != logging.NOTSET:
         yield '  Level ' + logging.getLevelName(level)
     for f in getattr(h, 'filters', ()):
         yield '  Filter %s' % describe_filter(f)
     formatter = getattr(h, 'formatter', None)
     if formatter is not None:
-        if type(formatter) is logging.Formatter:
+        if class_of(formatter) is logging.Formatter:
             yield '  Formatter fmt=%r datefmt=%r' % (
                 getattr(formatter, '_fmt', None),
                 getattr(formatter, 'datefmt', None))
         else:
             yield '  Formatter %r' % (formatter,)
     if t is logging.handlers.MemoryHandler and h.target is not None:
         yield '  Flushes output to:'
         g = describe_handler(h.target)
         yield '    Handler ' + next(g)
         for line in g:
             yield '    ' + line
+
+
+def class_of(obj):
+    """Try to learn the class of `obj`.
+
+    We perform the operation gingerly, as `obj` could be any kind of
+    user-supplied object: an old-style class, a new-style class, or a
+    built-in type that doesn't follow normal rules.
+
+    """
+    cls = getattr(obj, '__class__', None)
+    if cls is None:
+        cls = type(obj)
+    return cls
```

### Comparing `logging_tree-1.8.1/logging_tree/nodes.py` & `logging_tree-1.9/logging_tree/nodes.py`

 * *Files identical despite different names*

### Comparing `logging_tree-1.8.1/logging_tree/tests/test_format.py` & `logging_tree-1.9/logging_tree/tests/test_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 if sys.version_info >= (3,):
     from io import StringIO
 else:
     from StringIO import StringIO
 
 
 class FakeFile(StringIO):
-    def __init__(self, filename, mode, encoding=None):
+    def __init__(self, filename, *args, **kwargs):
         self.filename = filename
         StringIO.__init__(self)
 
     def __repr__(self):
         return '<file %r>' % self.filename
 
     def fileno(self):
@@ -150,27 +150,14 @@
         ah = logging.getLogger('').addHandler
         ah(logging.handlers.TimedRotatingFileHandler('/bar/two.txt'))
         expected = '''\
 <--""
    Level WARNING
    Handler TimedRotatingFile '/bar/two.txt' when='H' interval=3600 backupCount=0
 '''
-        if sys.version_info >= (3, 8):
-            # Apparently the design of the TimedRotatingFileHandler has
-            # become a bit more ambitious as of Python 3.8.
-            expected += '''\
-   |
-   o<--"asyncio"
-   |   Level NOTSET so inherits level WARNING
-   |
-   o<--[concurrent]
-       |
-       o<--"concurrent.futures"
-           Level NOTSET so inherits level WARNING
-'''
         self.assertEqual(build_description(), expected)
 
     def test_2_dot_6_handlers(self):
         if sys.version_info < (2, 6):
             return
         ah = logging.getLogger('').addHandler
         ah(logging.handlers.WatchedFileHandler('/bar/three.txt'))
```

### Comparing `logging_tree-1.8.1/logging_tree/tests/test_node.py` & `logging_tree-1.9/logging_tree/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `logging_tree-1.8.1/setup.py` & `logging_tree-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,11 +20,12 @@
         'Programming Language :: Python :: 3.2',
         'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Topic :: System :: Logging',
         ],
       packages=['logging_tree', 'logging_tree.tests'],
       )
```


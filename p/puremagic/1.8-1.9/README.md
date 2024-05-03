# Comparing `tmp/puremagic-1.8.tar.gz` & `tmp/puremagic-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/puremagic-1.8.tar", last modified: Tue Mar 24 19:48:33 2020, max compression
+gzip compressed data, was "dist/puremagic-1.9.tar", last modified: Mon Jun 15 17:02:43 2020, max compression
```

## Comparing `puremagic-1.8.tar` & `puremagic-1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 19:48:33.256181 puremagic-1.8/
--rw-r--r--   0 runner    (1001) docker     (115)      362 2020-03-24 19:48:26.000000 puremagic-1.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (115)     1762 2020-03-24 19:48:26.000000 puremagic-1.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (115)     1086 2020-03-24 19:48:26.000000 puremagic-1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (115)       82 2020-03-24 19:48:26.000000 puremagic-1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (115)     6059 2020-03-24 19:48:33.256181 puremagic-1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     4126 2020-03-24 19:48:26.000000 puremagic-1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 19:48:33.252181 puremagic-1.8/puremagic/
--rw-r--r--   0 runner    (1001) docker     (115)      126 2020-03-24 19:48:26.000000 puremagic-1.8/puremagic/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (115)      114 2020-03-24 19:48:26.000000 puremagic-1.8/puremagic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (115)    98494 2020-03-24 19:48:26.000000 puremagic-1.8/puremagic/magic_data.json
--rw-r--r--   0 runner    (1001) docker     (115)     8315 2020-03-24 19:48:26.000000 puremagic-1.8/puremagic/main.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 19:48:33.256181 puremagic-1.8/puremagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)     6059 2020-03-24 19:48:33.000000 puremagic-1.8/puremagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)      357 2020-03-24 19:48:33.000000 puremagic-1.8/puremagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-03-24 19:48:33.000000 puremagic-1.8/puremagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)        9 2020-03-24 19:48:33.000000 puremagic-1.8/puremagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)       10 2020-03-24 19:48:33.000000 puremagic-1.8/puremagic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (115)       74 2020-03-24 19:48:33.256181 puremagic-1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)     1376 2020-03-24 19:48:26.000000 puremagic-1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 19:48:33.256181 puremagic-1.8/test/
--rw-r--r--   0 runner    (1001) docker     (115)     6201 2020-03-24 19:48:26.000000 puremagic-1.8/test/test_common_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-15 17:02:43.770153 puremagic-1.9/
+-rw-r--r--   0 runner    (1001) docker     (116)      391 2020-06-15 17:02:36.000000 puremagic-1.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1884 2020-06-15 17:02:36.000000 puremagic-1.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1086 2020-06-15 17:02:36.000000 puremagic-1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       82 2020-06-15 17:02:36.000000 puremagic-1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     5956 2020-06-15 17:02:43.774153 puremagic-1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4047 2020-06-15 17:02:36.000000 puremagic-1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-15 17:02:43.770153 puremagic-1.9/puremagic/
+-rw-r--r--   0 runner    (1001) docker     (116)      126 2020-06-15 17:02:36.000000 puremagic-1.9/puremagic/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)      114 2020-06-15 17:02:36.000000 puremagic-1.9/puremagic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    98494 2020-06-15 17:02:36.000000 puremagic-1.9/puremagic/magic_data.json
+-rw-r--r--   0 runner    (1001) docker     (116)     9584 2020-06-15 17:02:36.000000 puremagic-1.9/puremagic/main.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-15 17:02:43.770153 puremagic-1.9/puremagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     5956 2020-06-15 17:02:43.000000 puremagic-1.9/puremagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      357 2020-06-15 17:02:43.000000 puremagic-1.9/puremagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-06-15 17:02:43.000000 puremagic-1.9/puremagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        9 2020-06-15 17:02:43.000000 puremagic-1.9/puremagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       10 2020-06-15 17:02:43.000000 puremagic-1.9/puremagic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       74 2020-06-15 17:02:43.774153 puremagic-1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1374 2020-06-15 17:02:36.000000 puremagic-1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-15 17:02:43.770153 puremagic-1.9/test/
+-rw-r--r--   0 runner    (1001) docker     (116)     6692 2020-06-15 17:02:36.000000 puremagic-1.9/test/test_common_extensions.py
```

### Comparing `puremagic-1.8/CHANGELOG.md` & `puremagic-1.9/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Changelog
 =========
 
+Version 1.9
+-----------
+
+- Adding new methods for stream handling (from_stream, magic_stream) (thanks to Robbert Korving)
+
 Version 1.8
 -----------
 
 - Adding support for various other files (thanks to Don Tsang)
 - Adding missing mime types (thanks to Oleksandr)
 
 Version 1.7
 -----------
 
 - Adding support for PCAPNG files (thanks to bannsec)
 - Adding support for numerous other files updated by Gary C. Kessler
 - Adding script for parsing FTK GCK sigs
-- Changing test suites to github workflows instead of TravisCI 
+- Changing test suites to github workflows instead of TravisCI
 - Removing official support, new packages and test for python 2
 
 Version 1.6
 -----------
 
 - Adding support for LZ4 and ZSTD archives (Thanks to Sergey Ponomarev)
 - Adding support for more office formats (Thanks to andrewpmk)
```

### Comparing `puremagic-1.8/LICENSE` & `puremagic-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `puremagic-1.8/PKG-INFO` & `puremagic-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: puremagic
-Version: 1.8
+Version: 1.9
 Summary: Pure python implementation of magic file detection
 Home-page: https://github.com/cdgriffith/puremagic
 Author: Chris Griffith
 Author-email: chris@cdgriffith.com
 License: MIT
 Description: puremagic
         =========
@@ -39,31 +39,28 @@
         -  Duplications due to small or reused magic numbers
         
         (Help fix the first two disadvantages by contributing!)
         
         Compatibility
         ~~~~~~~~~~~~~
         
-        -  Python 2.7+
-        -  Python 3.4+
+        -  Python 3.5+
         -  Pypy
         
         Using travis-ci to run continuous integration tests on listed platforms.
         
         Install
         -------
         
         In either a virtualenv or globally, simply run:
         
         .. code:: bash
         
                 $ python setup.py install
         
-        It has no dependencies (other than the 2.7+ built-in argparse)
-        
         Usage
         -----
         
         "from_file" will return the most likely file extension. "magic_file"
         will give you every possible result it finds, as well as the confidence.
         
         .. code:: python
```

### Comparing `puremagic-1.8/README.rst` & `puremagic-1.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -31,31 +31,28 @@
 -  Duplications due to small or reused magic numbers
 
 (Help fix the first two disadvantages by contributing!)
 
 Compatibility
 ~~~~~~~~~~~~~
 
--  Python 2.7+
--  Python 3.4+
+-  Python 3.5+
 -  Pypy
 
 Using travis-ci to run continuous integration tests on listed platforms.
 
 Install
 -------
 
 In either a virtualenv or globally, simply run:
 
 .. code:: bash
 
         $ python setup.py install
 
-It has no dependencies (other than the 2.7+ built-in argparse)
-
 Usage
 -----
 
 "from_file" will return the most likely file extension. "magic_file"
 will give you every possible result it finds, as well as the confidence.
 
 .. code:: python
```

### Comparing `puremagic-1.8/puremagic/magic_data.json` & `puremagic-1.9/puremagic/magic_data.json`

 * *Files identical despite different names*

### Comparing `puremagic-1.8/puremagic/main.py` & `puremagic-1.9/puremagic/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-# -*- coding: UTF-8 -*-
+# -*- coding: utf-8 -*-
 """
 puremagic is a pure python module that will identify a file based off it's
 magic numbers. It is designed to be minimalistic and inherently cross platform
 compatible, with no imports when used as a module.
 
 © 2013-2020 Chris Griffith - License: MIT (see LICENSE)
 
@@ -15,72 +15,78 @@
 import os
 import json
 import binascii
 from itertools import chain
 from collections import namedtuple
 
 __author__ = "Chris Griffith"
-__version__ = "1.8"
-__all__ = ['magic_file', 'magic_string', 'from_file', 'from_string',
-           'ext_from_filename', 'PureError', 'magic_footer_array',
-           'magic_header_array']
+__version__ = "1.9"
+__all__ = [
+    "magic_file",
+    "magic_string",
+    "magic_stream",
+    "from_file",
+    "from_string",
+    "from_stream",
+    "ext_from_filename",
+    "PureError",
+    "magic_footer_array",
+    "magic_header_array",
+]
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-MAGIC_INFO_TYPES = ('byte_match', 'offset', 'extension', 'mime_type', 'name',)
-PureMagic = namedtuple('PureMagic', MAGIC_INFO_TYPES)
-PureMagicWithConfidence = namedtuple('PureMagicWithConfidence',
-                                     (MAGIC_INFO_TYPES + ('confidence',)))
+MAGIC_INFO_TYPES = (
+    "byte_match",
+    "offset",
+    "extension",
+    "mime_type",
+    "name",
+)
+PureMagic = namedtuple("PureMagic", MAGIC_INFO_TYPES)  # type: ignore
+PureMagicWithConfidence = namedtuple("PureMagicWithConfidence", (MAGIC_INFO_TYPES + ("confidence",)))  # type: ignore
 
 
 class PureError(LookupError):
     """Do not have that type of file in our databanks"""
 
 
-def _magic_data(filename=os.path.join(here, 'magic_data.json')):
+def _magic_data(filename=os.path.join(here, "magic_data.json")):
     """ Read the magic file"""
     with open(filename) as f:
         data = json.load(f)
-    headers = sorted((_create_puremagic(x) for x in data['headers']),
-                     key=lambda x: x.byte_match)
-    footers = sorted((_create_puremagic(x) for x in data['footers']),
-                     key=lambda x: x.byte_match)
+    headers = sorted((_create_puremagic(x) for x in data["headers"]), key=lambda x: x.byte_match)
+    footers = sorted((_create_puremagic(x) for x in data["footers"]), key=lambda x: x.byte_match)
     return headers, footers
 
 
 def _create_puremagic(x):
-    return PureMagic(byte_match=binascii.unhexlify(x[0].encode('ascii')),
-                     offset=x[1],
-                     extension=x[2],
-                     mime_type=x[3],
-                     name=x[4])
+    return PureMagic(
+        byte_match=binascii.unhexlify(x[0].encode("ascii")), offset=x[1], extension=x[2], mime_type=x[3], name=x[4]
+    )
 
 
 magic_header_array, magic_footer_array = _magic_data()
 
 
 def _max_lengths():
     """ The length of the largest magic string + its offset"""
-    max_header_length = max([len(x.byte_match) + x.offset
-                             for x in magic_header_array])
-    max_footer_length = max([len(x.byte_match) + abs(x.offset)
-                             for x in magic_footer_array])
+    max_header_length = max([len(x.byte_match) + x.offset for x in magic_header_array])
+    max_footer_length = max([len(x.byte_match) + abs(x.offset) for x in magic_footer_array])
     return max_header_length, max_footer_length
 
 
 def _confidence(matches, ext=None):
     """ Rough confidence based on string length and file extension"""
     results = []
     for match in matches:
-        con = (0.8 if len(match.extension) > 9 else
-               float("0.{0}".format(len(match.extension))))
+        con = 0.8 if len(match.extension) > 9 else float("0.{0}".format(len(match.extension)))
         if ext == match.extension:
             con = 0.9
-        results.append(
-            PureMagicWithConfidence(confidence=con, **match._asdict()))
+        results.append(PureMagicWithConfidence(confidence=con, **match._asdict()))
     return sorted(results, key=lambda x: x.confidence, reverse=True)
 
 
 def _identify_all(header, footer, ext=None):
     """ Attempt to identify 'data' by its magic numbers"""
 
     # Capture the length of the data
@@ -107,16 +113,15 @@
 def _magic(header, footer, mime, ext=None):
     """ Discover what type of file it is based on the incoming string """
     if not header:
         raise ValueError("Input was empty")
     info = _identify_all(header, footer, ext)[0]
     if mime:
         return info.mime_type
-    return info.extension if not \
-        isinstance(info.extension, list) else info[0].extension
+    return info.extension if not isinstance(info.extension, list) else info[0].extension
 
 
 def _file_details(filename):
     """ Grab the start and end of the file"""
     max_head, max_foot = _max_lengths()
     with open(filename, "rb") as fin:
         head = fin.read(max_head)
@@ -130,27 +135,35 @@
 
 def _string_details(string):
     """ Grab the start and end of the string"""
     max_head, max_foot = _max_lengths()
     return string[:max_head], string[-max_foot:]
 
 
+def _stream_details(stream):
+    """ Grab the start and end of the stream"""
+    max_head, max_foot = _max_lengths()
+    head = stream.read(max_head)
+    stream.seek(-max_foot, os.SEEK_END)
+    foot = stream.read()
+    return head, foot
+
+
 def ext_from_filename(filename):
     """ Scan a filename for it's extension.
 
     :param filename: string of the filename
     :return: the extension off the end (empty string if it can't find one)
     """
     try:
         base, ext = filename.lower().rsplit(".", 1)
     except ValueError:
-        return ''
+        return ""
     ext = ".{0}".format(ext)
-    all_exts = [x.extension for x in chain(magic_header_array,
-                                           magic_footer_array)]
+    all_exts = [x.extension for x in chain(magic_header_array, magic_footer_array)]
 
     if base[-4:].startswith("."):
         # For double extensions like like .tar.gz
         long_ext = base[-4:] + ext
         if long_ext in all_exts:
             return long_ext
     return ext
@@ -182,14 +195,30 @@
     :return: guessed extension or mime
     """
     head, foot = _string_details(string)
     ext = ext_from_filename(filename) if filename else None
     return _magic(head, foot, mime, ext)
 
 
+def from_stream(stream, mime=False, filename=None):
+    """ Reads in stream, attempts to identify content based
+    off magic number and will return the file extension.
+    If mime is True it will return the mime type instead.
+    If filename is provided it will be used in the computation.
+
+    :param stream: stream representation to check
+    :param mime: Return mime, not extension
+    :param filename: original filename
+    :return: guessed extension or mime
+    """
+    head, foot = _stream_details(stream)
+    ext = ext_from_filename(filename) if filename else None
+    return _magic(head, foot, mime, ext)
+
+
 def magic_file(filename):
     """ Returns tuple of (num_of_matches, array_of_matches)
     arranged highest confidence match first.
 
     :param filename: path to file
     :return: list of possible matches, highest confidence first
     """
@@ -218,33 +247,53 @@
     head, foot = _string_details(string)
     ext = ext_from_filename(filename) if filename else None
     info = _identify_all(head, foot, ext)
     info.sort(key=lambda x: x.confidence, reverse=True)
     return info
 
 
+def magic_stream(stream, filename=None):
+    """ Returns tuple of (num_of_matches, array_of_matches)
+    arranged highest confidence match first
+    If filename is provided it will be used in the computation.
+
+    :param stream: stream representation to check
+    :param filename: original filename
+    :return: list of possible matches, highest confidence first
+    """
+    head, foot = _stream_details(stream)
+    if not head:
+        raise ValueError("Input was empty")
+    ext = ext_from_filename(filename) if filename else None
+    info = _identify_all(head, foot, ext)
+    info.sort(key=lambda x: x.confidence, reverse=True)
+    return info
+
+
 def command_line_entry(*args):
     from argparse import ArgumentParser
     import sys
-    desc = "puremagic is a pure python file identification module. \
-    It looks for matching magic numbers in the file to locate the file type. "
-    parser = ArgumentParser(description=desc)
-    parser.add_argument("-m",
-                        "--mime",
-                        action="store_true",
-                        dest="mime",
-                        help="Return the mime type instead of file type")
-    parser.add_argument('files', nargs="+")
+
+    parser = ArgumentParser(
+        description=(
+            "puremagic is a pure python file identification module."
+            "It looks for matching magic numbers in the file to locate the file type. "
+        )
+    )
+    parser.add_argument(
+        "-m", "--mime", action="store_true", dest="mime", help="Return the mime type instead of file type"
+    )
+    parser.add_argument("files", nargs="+")
     args = parser.parse_args(args if args else sys.argv[1:])
 
     for fn in args.files:
         if not os.path.exists(fn):
             print("File '{0}' does not exist!".format(fn))
             continue
         try:
             print("'{0}' : {1}".format(fn, from_file(fn, args.mime)))
         except PureError:
             print("'{0}' : could not be Identified".format(fn))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     command_line_entry()
```

### Comparing `puremagic-1.8/puremagic.egg-info/PKG-INFO` & `puremagic-1.9/puremagic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: puremagic
-Version: 1.8
+Version: 1.9
 Summary: Pure python implementation of magic file detection
 Home-page: https://github.com/cdgriffith/puremagic
 Author: Chris Griffith
 Author-email: chris@cdgriffith.com
 License: MIT
 Description: puremagic
         =========
@@ -39,31 +39,28 @@
         -  Duplications due to small or reused magic numbers
         
         (Help fix the first two disadvantages by contributing!)
         
         Compatibility
         ~~~~~~~~~~~~~
         
-        -  Python 2.7+
-        -  Python 3.4+
+        -  Python 3.5+
         -  Pypy
         
         Using travis-ci to run continuous integration tests on listed platforms.
         
         Install
         -------
         
         In either a virtualenv or globally, simply run:
         
         .. code:: bash
         
                 $ python setup.py install
         
-        It has no dependencies (other than the 2.7+ built-in argparse)
-        
         Usage
         -----
         
         "from_file" will return the most likely file extension. "magic_file"
         will give you every possible result it finds, as well as the confidence.
         
         .. code:: python
```

### Comparing `puremagic-1.8/setup.py` & `puremagic-1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,33 +13,33 @@
 
 attrs = dict(re.findall(r"__([a-z]+)__ *= *['\"](.+)['\"]", reuse_content))
 
 with open("README.rst", "r") as readme_file:
     long_description = readme_file.read()
 
 setup(
-    name='puremagic',
-    version=attrs['version'],
-    url='https://github.com/cdgriffith/puremagic',
-    license='MIT',
-    author=attrs['author'],
+    name="puremagic",
+    version=attrs["version"],
+    url="https://github.com/cdgriffith/puremagic",
+    license="MIT",
+    author=attrs["author"],
     install_requires=["argparse"],
-    author_email='chris@cdgriffith.com',
-    description='Pure python implementation of magic file detection',
+    author_email="chris@cdgriffith.com",
+    description="Pure python implementation of magic file detection",
     long_description=long_description,
-    package_data={'puremagic': ['*.json']},
-    packages=['puremagic'],
+    package_data={"puremagic": ["*.json"]},
+    packages=["puremagic"],
     include_package_data=True,
-    platforms='any',
+    platforms="any",
     classifiers=[
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: Implementation :: PyPy',
-        'Development Status :: 4 - Beta',
-        'Natural Language :: English',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Topic :: Utilities'
-        ]
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 2",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: Implementation :: PyPy",
+        "Development Status :: 4 - Beta",
+        "Natural Language :: English",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Topic :: Utilities",
+    ],
 )
```

### Comparing `puremagic-1.8/test/test_common_extensions.py` & `puremagic-1.9/test/test_common_extensions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+# -*- coding: utf-8 -*-
 import unittest
 from tempfile import NamedTemporaryFile
 import os
+from io import BytesIO
+import pytest
 
 import puremagic
 
 LOCAL_DIR = os.path.realpath(os.path.dirname(__file__))
 IMAGE_DIR = os.path.join(LOCAL_DIR, "resources", "images")
 VIDEO_DIR = os.path.join(LOCAL_DIR, "resources", "video")
 AUDIO_DIR = os.path.join(LOCAL_DIR, "resources", "audio")
@@ -22,15 +25,14 @@
         self.expect_ext = ".mp4"
         self.expect_mime = "video/mp4"
 
     def group_test(self, directory):
         failures = []
         ext_failures = []
         for item in os.listdir(directory):
-            print(item)
             try:
                 ext = puremagic.from_file(os.path.join(directory, item))
             except puremagic.PureError:
                 failures.append(item)
             else:
                 if not item.endswith(ext):
                     ext_failures.append((item, ext))
@@ -44,120 +46,139 @@
             raise AssertionError(
                 "The following files did not have the expected extensions: {}".format(
                     ", ".join(['"{}" expected "{}"'.format(item, ext) for item, ext in ext_failures])
                 )
             )
 
     def test_file(self):
-        """File identification                          |"""
+        """File identification """
         mp4file = NamedTemporaryFile(delete=False)
         mp4file.write(self.mp4magic)
         mp4file.close()
         ext = puremagic.from_file(mp4file.name)
         os.unlink(mp4file.name)
         self.assertEqual(self.expect_ext, ext)
 
     def test_hex_string(self):
-        """Hex string identification                    |"""
+        """Hex string identification """
         ext = puremagic.from_string(self.mp4magic)
         self.assertEqual(self.expect_ext, ext)
 
     def test_string(self):
-        """String identification                        |"""
+        """String identification """
         ext = puremagic.from_string(bytes(self.mp4magic))
         self.assertEqual(self.expect_ext, ext)
 
     def test_string_with_filename_hint(self):
-        """String identification with filename hint     |"""
+        """String identification with filename hint """
         filename = os.path.join(OFFICE_DIR, "test.xlsx")
         with open(filename, "rb") as f:
             data = f.read()
         ext = puremagic.from_string(data)
         # .docx and .xlsx have same signature
         self.assertEqual(".docx", ext)
         # with the hint from_string() shoud find the correct extension
         ext = puremagic.from_string(data, filename=filename)
         self.assertEqual(".xlsx", ext)
 
     def test_string_with_confidence(self):
-        """String identification: magic_string          |"""
+        """String identification: magic_string """
         ext = puremagic.magic_string(bytes(self.mp4magic))
         self.assertEqual(self.expect_ext, ext[0].extension)
         self.assertRaises(ValueError, puremagic.magic_string, "")
 
     def test_magic_string_with_filename_hint(self):
-        """String identification: magic_string with hint|"""
+        """String identification: magic_string with hint """
         filename = os.path.join(OFFICE_DIR, "test.xlsx")
         with open(filename, "rb") as f:
             data = f.read()
         ext = puremagic.magic_string(data, filename=filename)
         self.assertEqual(".xlsx", ext[0].extension)
 
     def test_not_found(self):
-        """Bad file type via string                     |"""
+        """Bad file type via string """
         try:
             with self.assertRaises(puremagic.PureError):
                 puremagic.from_string("not applicable string")
         except TypeError:
             # Python 2.6 doesn't support using
             # assertRaises as a context manager
             pass
 
     def test_magic_file(self):
-        """File identification with magic_file          |"""
+        """File identification with magic_file """
         self.assertEqual(puremagic.magic_file(TGA_FILE)[0].extension, ".tga")
         open("test_empty_file", "w").close()
         try:
             self.assertRaises(ValueError, puremagic.magic_file, "test_empty_file")
         finally:
             os.unlink("test_empty_file")
 
+    def test_stream(self):
+        """Stream identification """
+        ext = puremagic.from_stream(BytesIO(self.mp4magic))
+        self.assertEqual(self.expect_ext, ext)
+        self.assertRaises(ValueError, puremagic.from_stream, BytesIO(b""))
+
+    def test_magic_stream(self):
+        """File identification with magic_stream """
+        with open(TGA_FILE, "rb") as f:
+            stream = BytesIO(f.read())
+        result = puremagic.magic_stream(stream, TGA_FILE)
+        self.assertEqual(result[0].extension, ".tga")
+        self.assertRaises(ValueError, puremagic.magic_stream, BytesIO(b""))
+
     def test_mime(self):
-        """Identify mime type                           |"""
+        """Identify mime type """
         self.assertEqual(puremagic.from_file(TGA_FILE, True), "image/tga")
 
     def test_images(self):
-        """Test common image formats                    |"""
+        """Test common image formats """
         self.group_test(IMAGE_DIR)
 
     def test_video(self):
-        """Test common video formats                    |"""
+        """Test common video formats """
         self.group_test(VIDEO_DIR)
 
     def test_audio(self):
-        """Test common audio formats                    |"""
+        """Test common audio formats """
         self.group_test(AUDIO_DIR)
 
     def test_office(self):
-        """Test common office document formats          |"""
+        """Test common office document formats """
         # Office files have very similar magic numbers, and may overlap
         for item in os.listdir(OFFICE_DIR):
             puremagic.from_file(os.path.join(OFFICE_DIR, item))
 
     def test_archive(self):
-        """Test common compressed archive formats       |"""
+        """Test common compressed archive formats """
         # pcapng files from https://wiki.wireshark.org/Development/PcapNg
         self.group_test(ARCHIVE_DIR)
 
     def test_media(self):
-        """Test common media formats                    |"""
+        """Test common media formats """
         self.group_test(MEDIA_DIR)
 
     def test_system(self):
-        """Test common system formats                   |"""
+        """Test common system formats """
         self.group_test(SYSTEM_DIR)
 
     def test_ext(self):
-        """Test ext from filename                       |"""
+        """Test ext from filename """
         ext = puremagic.ext_from_filename("test.tar.bz2")
         assert ext == ".tar.bz2", ext
 
     def test_cmd_options(self):
-        """Test CLI options                             |"""
+        """Test CLI options """
         from puremagic.main import command_line_entry
 
         command_line_entry(__file__, "test.py")
 
+    def test_bad_magic_input(self):
+        """Test bad magic imput"""
+        with pytest.raises(ValueError):
+            puremagic.main._magic(None, None, None)
+
 
 if __name__ == "__main__":
     suite = unittest.TestLoader().loadTestsFromTestCase(TestMagic)
     unittest.TextTestRunner(verbosity=2).run(suite)
```


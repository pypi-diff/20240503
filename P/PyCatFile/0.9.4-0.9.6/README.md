# Comparing `tmp/pycatfile-0.9.4.tar.gz` & `tmp/pycatfile-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatfile-0.9.4.tar", last modified: Thu May  2 01:11:38 2024, max compression
+gzip compressed data, was "pycatfile-0.9.6.tar", last modified: Thu May  2 01:20:02 2024, max compression
```

## Comparing `pycatfile-0.9.4.tar` & `pycatfile-0.9.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:11:38.355999 pycatfile-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-02 01:11:29.000000 pycatfile-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-02 01:11:38.355999 pycatfile-0.9.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:11:38.355999 pycatfile-0.9.4/PyCatFile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-02 01:11:38.000000 pycatfile-0.9.4/PyCatFile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 01:11:38.000000 pycatfile-0.9.4/PyCatFile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 01:11:38.000000 pycatfile-0.9.4/PyCatFile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 01:11:38.000000 pycatfile-0.9.4/PyCatFile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 01:11:38.000000 pycatfile-0.9.4/PyCatFile.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 01:11:29.000000 pycatfile-0.9.4/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     9956 2024-05-02 01:11:29.000000 pycatfile-0.9.4/catfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4968 2024-05-02 01:11:29.000000 pycatfile-0.9.4/neocatfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   305547 2024-05-02 01:11:29.000000 pycatfile-0.9.4/pycatfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-02 01:11:38.355999 pycatfile-0.9.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     5450 2024-05-02 01:11:29.000000 pycatfile-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:20:02.152612 pycatfile-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-02 01:19:48.000000 pycatfile-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-02 01:20:02.152612 pycatfile-0.9.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:20:02.152612 pycatfile-0.9.6/PyCatFile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-02 01:20:02.000000 pycatfile-0.9.6/PyCatFile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 01:20:02.000000 pycatfile-0.9.6/PyCatFile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 01:20:02.000000 pycatfile-0.9.6/PyCatFile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 01:20:02.000000 pycatfile-0.9.6/PyCatFile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 01:20:02.000000 pycatfile-0.9.6/PyCatFile.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 01:19:48.000000 pycatfile-0.9.6/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9956 2024-05-02 01:19:48.000000 pycatfile-0.9.6/catfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4968 2024-05-02 01:19:48.000000 pycatfile-0.9.6/neocatfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   305902 2024-05-02 01:19:48.000000 pycatfile-0.9.6/pycatfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-02 01:20:02.152612 pycatfile-0.9.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5450 2024-05-02 01:19:48.000000 pycatfile-0.9.6/setup.py
```

### Comparing `pycatfile-0.9.4/LICENSE` & `pycatfile-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pycatfile-0.9.4/PKG-INFO` & `pycatfile-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCatFile
-Version: 0.9.4
+Version: 0.9.6
 Summary: A tar like file format name catfile after unix cat command (concatenate files) .
 Home-page: https://github.com/GameMaker2k/PyCatFile
 Download-URL: https://github.com/GameMaker2k/PyCatFile/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `pycatfile-0.9.4/PyCatFile.egg-info/PKG-INFO` & `pycatfile-0.9.6/PyCatFile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCatFile
-Version: 0.9.4
+Version: 0.9.6
 Summary: A tar like file format name catfile after unix cat command (concatenate files) .
 Home-page: https://github.com/GameMaker2k/PyCatFile
 Download-URL: https://github.com/GameMaker2k/PyCatFile/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `pycatfile-0.9.4/catfile.py` & `pycatfile-0.9.6/catfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: catfile.py - Last Update: 5/1/2024 Ver. 0.9.4 RC 1 - Author: cooldude2k $
+    $FileInfo: catfile.py - Last Update: 5/1/2024 Ver. 0.9.6 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import sys, argparse, pycatfile, binascii;
 
 rarfile_support = pycatfile.rarfile_support;
 py7zr_support = pycatfile.py7zr_support;
```

### Comparing `pycatfile-0.9.4/neocatfile.py` & `pycatfile-0.9.6/neocatfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: neocatfile.py - Last Update: 5/1/2024 Ver. 0.9.4 RC 1 - Author: cooldude2k $
+    $FileInfo: neocatfile.py - Last Update: 5/1/2024 Ver. 0.9.6 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 import argparse
 import pycatfile
 
 # Compatibility layer for Python 2 and 3 input
```

### Comparing `pycatfile-0.9.4/pycatfile.py` & `pycatfile-0.9.6/pycatfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: pycatfile.py - Last Update: 5/1/2024 Ver. 0.9.4 RC 1 - Author: cooldude2k $
+    $FileInfo: pycatfile.py - Last Update: 5/1/2024 Ver. 0.9.6 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import io, os, re, sys, time, stat, zlib, base64, shutil, socket, hashlib, datetime, logging, binascii, tempfile, zipfile, platform;
 from ftplib import FTP, FTP_TLS;
 if(sys.version[0]=="2"):
  from urlparse import urlparse, urlunparse;
@@ -170,19 +170,19 @@
 __file_format_ver__ = "001";
 __use_new_style__ = True;
 __use_advanced_list__ = True;
 __use_alt_inode__ = False;
 __file_format_list__ = [__file_format_name__, __file_format_magic__, __file_format_lower__, __file_format_len__, __file_format_hex__, __file_format_delimiter__, __file_format_ver__, __use_new_style__, __use_advanced_list__, __use_alt_inode__];
 __project__ = __program_name__;
 __project_url__ = "https://github.com/GameMaker2k/PyCatFile";
-__version_info__ = (0, 9, 4, "RC 1", 1);
+__version_info__ = (0, 9, 6, "RC 1", 1);
 __version_date_info__ = (2024, 5, 1, "RC 1", 1);
 __version_date__ = str(__version_date_info__[0]) + "." + str(__version_date_info__[1]).zfill(2) + "." + str(__version_date_info__[2]).zfill(2);
 __revision__ = __version_info__[3];
-__revision_id__ = "$Id: 2e466ee1526f58ea652f67d4f12337bf6d4eea67 $";
+__revision_id__ = "$Id: 4567eb777c3f1cb3b1adf49788eb5c726205e3a4 $";
 if(__version_info__[4] is not None):
  __version_date_plusrc__ = __version_date__ + "-" + str(__version_date_info__[4]);
 if(__version_info__[4] is None):
  __version_date_plusrc__ = __version_date__;
 if(__version_info__[3] is not None):
  __version__ = str(__version_info__[0]) + "." + str(__version_info__[1]) + "." + str(__version_info__[2]) + " " + str(__version_info__[3]);
 if(__version_info__[3] is None):
@@ -2536,15 +2536,16 @@
   catfileoutstr = AppendNullByte(catheaersize, formatspecs[5]) + catfileoutstr;
   catfileheadercshex = GetFileChecksum(catfileoutstr, checksumtype, True, formatspecs);
   catfileoutstr = catfileoutstr + AppendNullBytes([catfileheadercshex, catfilecontentcshex], formatspecs[5]);
   catfhend = (catfp.tell() - 1) + len(catfileoutstr);
   catfcontentstart = catfp.tell() + len(catfileoutstr);
   catfileoutstrecd = catfileoutstr.encode('UTF-8');
   nullstrecd = formatspecs[5].encode('UTF-8');
-  catfileout = catfileoutstrecd + fcontents + nullstrecd;
+  fcontents.seek(0, 0);
+  catfileout = catfileoutstrecd + fcontents.read() + nullstrecd;
   catfcontentend = (catfp.tell() - 1) + len(catfileout);
   catfp.write(catfileout);
   try:
    catfp.flush();
    os.fsync(catfp.fileno());
   except io.UnsupportedOperation:
    pass;
@@ -2773,15 +2774,16 @@
   tmpfileoutstr = catfileoutstr + AppendNullBytes([catfileheadercshex, catfilecontentcshex], formatspecs[5]);
   catheaersize = format(int(len(tmpfileoutstr) - 1), 'x').lower();
   catfileoutstr = AppendNullByte(catheaersize, formatspecs[5]) + catfileoutstr;
   catfileheadercshex = GetFileChecksum(catfileoutstr, checksumtype, True, formatspecs);
   catfileoutstr = catfileoutstr + AppendNullBytes([catfileheadercshex, catfilecontentcshex], formatspecs[5]);
   catfileoutstrecd = catfileoutstr.encode('UTF-8');
   nullstrecd = formatspecs[5].encode('UTF-8');
-  catfileout = catfileoutstrecd + fcontents + nullstrecd;
+  fcontents.seek(0, 0);
+  catfileout = catfileoutstrecd + fcontents.read() + nullstrecd;
   catfcontentend = (catfp.tell() - 1) + len(catfileout);
   catfp.write(catfileout);
   try:
    catfp.flush();
    os.fsync(catfp.fileno());
   except io.UnsupportedOperation:
    pass;
@@ -3020,15 +3022,16 @@
   tmpfileoutstr = catfileoutstr + AppendNullBytes([catfileheadercshex, catfilecontentcshex], formatspecs[5]);
   catheaersize = format(int(len(tmpfileoutstr) - 1), 'x').lower();
   catfileoutstr = AppendNullByte(catheaersize, formatspecs[5]) + catfileoutstr;
   catfileheadercshex = GetFileChecksum(catfileoutstr, checksumtype, True, formatspecs);
   catfileoutstr = catfileoutstr + AppendNullBytes([catfileheadercshex, catfilecontentcshex], formatspecs[5]);
   catfileoutstrecd = catfileoutstr.encode('UTF-8');
   nullstrecd = formatspecs[5].encode('UTF-8');
-  catfileout = catfileoutstrecd + fcontents + nullstrecd;
+  fcontents.seek(0, 0);
+  catfileout = catfileoutstrecd + fcontents.read() + nullstrecd;
   catfcontentend = (catfp.tell() - 1) + len(catfileout);
   catfp.write(catfileout);
   try:
    catfp.flush();
    os.fsync(catfp.fileno());
   except io.UnsupportedOperation:
    pass;
@@ -3283,19 +3286,20 @@
    fcontents.seek(0, 0);
    catfilecontentcshex = GetFileChecksum(fcontents.read(), checksumtype, False, formatspecs);
    tmpfileoutstr = catfileoutstr + AppendNullBytes([catfileheadercshex, catfilecontentcshex], formatspecs[5]);
    catheaersize = format(int(len(tmpfileoutstr) - 1), 'x').lower();
    catfileoutstr = AppendNullByte(catheaersize, formatspecs[5]) + catfileoutstr;
    catfileheadercshex = GetFileChecksum(catfileoutstr, checksumtype, True, formatspecs);
    catfileoutstr = catfileoutstr + AppendNullBytes([catfileheadercshex, catfilecontentcshex], formatspecs[5])
-   catfileoutstrecd = catfileoutstr.encode('UTF-8')
-   nullstrecd = formatspecs[5].encode('UTF-8')
-   catfileout = catfileoutstrecd + fcontents + nullstrecd
-   catfcontentend = (catfp.tell() - 1) + len(catfileout)
-   catfp.write(catfileout)
+   catfileoutstrecd = catfileoutstr.encode('UTF-8');
+   nullstrecd = formatspecs[5].encode('UTF-8');
+   fcontents.seek(0, 0);
+   catfileout = catfileoutstrecd + fcontents.read() + nullstrecd;
+   catfcontentend = (catfp.tell() - 1) + len(catfileout);
+   catfp.write(catfileout);
    try:
     catfp.flush();
     os.fsync(catfp.fileno());
    except io.UnsupportedOperation:
     pass
    except AttributeError:
     pass
@@ -3495,19 +3499,20 @@
    fcontents.seek(0, 0);
    catfilecontentcshex = GetFileChecksum(fcontents.read(), checksumtype, False, formatspecs);
    tmpfileoutstr = catfileoutstr + AppendNullBytes([catfileheadercshex, catfilecontentcshex], formatspecs[5]);
    catheaersize = format(int(len(tmpfileoutstr) - 1), 'x').lower();
    catfileoutstr = AppendNullByte(catheaersize, formatspecs[5]) + catfileoutstr;
    catfileheadercshex = GetFileChecksum(catfileoutstr, checksumtype, True, formatspecs);
    catfileoutstr = catfileoutstr + AppendNullBytes([catfileheadercshex, catfilecontentcshex], formatspecs[5])
-   catfileoutstrecd = catfileoutstr.encode('UTF-8')
-   nullstrecd = formatspecs[5].encode('UTF-8')
-   catfileout = catfileoutstrecd + fcontents + nullstrecd
-   catfcontentend = (catfp.tell() - 1) + len(catfileout)
-   catfp.write(catfileout)
+   catfileoutstrecd = catfileoutstr.encode('UTF-8');
+   nullstrecd = formatspecs[5].encode('UTF-8');
+   fcontents.seek(0, 0);
+   catfileout = catfileoutstrecd + fcontents.read() + nullstrecd;
+   catfcontentend = (catfp.tell() - 1) + len(catfileout);
+   catfp.write(catfileout);
    try:
     catfp.flush();
     os.fsync(catfp.fileno());
    except io.UnsupportedOperation:
     pass
    except AttributeError:
     pass
@@ -4732,15 +4737,16 @@
   catfileoutstr = AppendNullByte(catheaersize, formatspecs[5]) + catfileoutstr;
   catfileheadercshex = GetFileChecksum(catfileoutstr, checksumtype, True, formatspecs);
   catfileoutstr = catfileoutstr + AppendNullBytes([catfileheadercshex, catfilecontentcshex], formatspecs[5]);
   catfileoutstrecd = catfileoutstr.encode('UTF-8');
   nullstrecd = formatspecs[5].encode('UTF-8');
   fheadtell += len(catfileoutstr) + 1;
   catfcontentend = fheadtell - 1;
-  catfileout = catfileoutstrecd + fcontents + nullstrecd;
+  fcontents.seek(0, 0);
+  catfileout = catfileoutstrecd + fcontents.read() + nullstrecd;
   pyhascontents = False;
   if(int(fsize)>0 and not listonly):
    pyhascontents = True;
   if(int(fsize)>0 and listonly):
    fcontents = BytesIO();
    pyhascontents = False;
   fcontents.seek(0, 0);
@@ -4905,15 +4911,16 @@
   catfileoutstr = AppendNullByte(catheaersize, formatspecs[5]) + catfileoutstr;
   catfileheadercshex = GetFileChecksum(catfileoutstr, checksumtype, True, formatspecs);
   catfileoutstr = catfileoutstr + AppendNullBytes([catfileheadercshex, catfilecontentcshex], formatspecs[5]);
   catfileoutstrecd = catfileoutstr.encode('UTF-8');
   nullstrecd = formatspecs[5].encode('UTF-8');
   fheadtell += len(catfileoutstr) + 1;
   catfcontentend = fheadtell - 1;
-  catfileout = catfileoutstrecd + fcontents + nullstrecd;
+  fcontents.seek(0, 0);
+  catfileout = catfileoutstrecd + fcontents.read() + nullstrecd;
   pyhascontents = False;
   if(int(fsize)>0 and not listonly):
    pyhascontents = True;
   if(int(fsize)>0 and listonly):
    fcontents = "";
    pyhascontents = False;
   fcontents.seek(0, 0);
@@ -5096,15 +5103,16 @@
   catfileoutstr = AppendNullByte(catheaersize, formatspecs[5]) + catfileoutstr;
   catfileheadercshex = GetFileChecksum(catfileoutstr, checksumtype, True, formatspecs);
   catfileoutstr = catfileoutstr + AppendNullBytes([catfileheadercshex, catfilecontentcshex], formatspecs[5]);
   catfileoutstrecd = catfileoutstr.encode('UTF-8');
   nullstrecd = formatspecs[5].encode('UTF-8');
   fheadtell += len(catfileoutstr) + 1;
   catfcontentend = fheadtell - 1;
-  catfileout = catfileoutstrecd + fcontents + nullstrecd;
+  fcontents.seek(0, 0);
+  catfileout = catfileoutstrecd + fcontents.read() + nullstrecd;
   pyhascontents = False;
   if(int(fsize)>0 and not listonly):
    pyhascontents = True;
   if(int(fsize)>0 and listonly):
    fcontents = BytesIO();
    pyhascontents = False;
   fcontents.seek(0, 0);
@@ -5305,15 +5313,16 @@
    catfileoutstr = AppendNullByte(catheaersize, formatspecs[5]) + catfileoutstr;
    catfileheadercshex = GetFileChecksum(catfileoutstr, checksumtype, True, formatspecs);
    catfileoutstr = catfileoutstr + AppendNullBytes([catfileheadercshex, catfilecontentcshex], formatspecs[5]);
    catfileoutstrecd = catfileoutstr.encode('UTF-8');
    nullstrecd = formatspecs[5].encode('UTF-8');
    fheadtell += len(catfileoutstr) + 1;
    catfcontentend = fheadtell - 1;
-   catfileout = catfileoutstrecd + fcontents + nullstrecd;
+   fcontents.seek(0, 0);
+   catfileout = catfileoutstrecd + fcontents.read() + nullstrecd;
    pyhascontents = False;
    if(int(fsize)>0 and not listonly):
     pyhascontents = True;
    if(int(fsize)>0 and listonly):
     fcontents = BytesIO();
     pyhascontents = False;
    fcontents.seek(0, 0);
@@ -5459,15 +5468,16 @@
    catfileoutstr = AppendNullByte(catheaersize, formatspecs[5]) + catfileoutstr;
    catfileheadercshex = GetFileChecksum(catfileoutstr, checksumtype, True, formatspecs);
    catfileoutstr = catfileoutstr + AppendNullBytes([catfileheadercshex, catfilecontentcshex], formatspecs[5]);
    catfileoutstrecd = catfileoutstr.encode('UTF-8');
    nullstrecd = formatspecs[5].encode('UTF-8');
    fheadtell += len(catfileoutstr) + 1;
    catfcontentend = fheadtell - 1;
-   catfileout = catfileoutstrecd + fcontents + nullstrecd;
+   fcontents.seek(0, 0);
+   catfileout = catfileoutstrecd + fcontents.read() + nullstrecd;
    pyhascontents = False;
    if(int(fsize)>0 and not listonly):
     pyhascontents = True;
    if(int(fsize)>0 and listonly):
     fcontents = "";
     pyhascontents = False;
    fcontents.seek(0, 0);
@@ -6057,15 +6067,16 @@
   tmpfileoutstr = catfileoutstr + AppendNullBytes([catfileheadercshex, catfilecontentcshex], formatspecs[5]);
   catheaersize = format(int(len(tmpfileoutstr) - 1), 'x').lower();
   catfileoutstr = AppendNullByte(catheaersize, formatspecs[5]) + catfileoutstr;
   catfileheadercshex = GetFileChecksum(catfileoutstr, checksumtype, True, formatspecs);
   catfileoutstr = catfileoutstr + AppendNullBytes([catfileheadercshex, catfilecontentcshex], formatspecs[5]);
   catfileoutstrecd = catfileoutstr.encode('UTF-8');
   nullstrecd = formatspecs[5].encode('UTF-8');
-  catfileout = catfileoutstrecd + fcontents + nullstrecd;
+  fcontents.seek(0, 0);
+  catfileout = catfileoutstrecd + fcontents.read() + nullstrecd;
   catfcontentend = (catfp.tell() - 1) + len(catfileout);
   catfp.write(catfileout);
   try:
    catfp.flush();
    os.fsync(catfp.fileno());
   except io.UnsupportedOperation:
    pass;
```

### Comparing `pycatfile-0.9.4/setup.py` & `pycatfile-0.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2016-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2016-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2016-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: setup.py - Last Update: 5/1/2024 Ver. 0.9.4 RC 1 - Author: cooldude2k $
+    $FileInfo: setup.py - Last Update: 5/1/2024 Ver. 0.9.6 RC 1 - Author: cooldude2k $
 '''
 
 import os, re, sys, pkg_resources;
 from setuptools import setup;
 
 verinfofilename = os.path.realpath("."+os.path.sep+os.path.sep+"pycatfile.py");
 verinfofile = open(verinfofilename, "r");
```


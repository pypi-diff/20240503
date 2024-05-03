# Comparing `tmp/kidiff-2.5.3.tar.gz` & `tmp/kidiff-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kidiff-2.5.3.tar", last modified: Wed Jan 10 13:19:35 2024, max compression
+gzip compressed data, was "kidiff-2.5.4.tar", last modified: Fri May  3 16:03:48 2024, max compression
```

## Comparing `kidiff-2.5.3.tar` & `kidiff-2.5.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 13:19:35.432518 kidiff-2.5.3/
--rw-r--r--   0 root         (0) root         (0)    14276 2024-01-10 13:19:35.432518 kidiff-2.5.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    10982 2024-01-10 13:17:05.000000 kidiff-2.5.3/README.md
--rwxrwxr-x   0 root         (0) root         (0)     4934 2024-01-10 13:17:05.000000 kidiff-2.5.3/kicad-diff-init.py
--rwxrwxr-x   0 root         (0) root         (0)    37116 2024-01-10 13:17:05.000000 kidiff-2.5.3/kicad-diff.py
--rwxrwxr-x   0 root         (0) root         (0)     3865 2024-01-10 13:17:05.000000 kidiff-2.5.3/kicad-git-diff.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 13:19:35.432518 kidiff-2.5.3/kidiff.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14276 2024-01-10 13:19:35.000000 kidiff-2.5.3/kidiff.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      228 2024-01-10 13:19:35.000000 kidiff-2.5.3/kidiff.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-10 13:19:35.000000 kidiff-2.5.3/kidiff.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-01-10 13:19:35.000000 kidiff-2.5.3/kidiff.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-10 13:19:35.000000 kidiff-2.5.3/kidiff.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)     1120 2024-01-10 13:19:35.436518 kidiff-2.5.3/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1430 2024-01-10 13:17:05.000000 kidiff-2.5.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:03:48.623359 kidiff-2.5.4/
+-rw-r--r--   0 root         (0) root         (0)    14451 2024-05-03 16:03:48.623359 kidiff-2.5.4/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    11117 2024-05-03 16:00:35.000000 kidiff-2.5.4/README.md
+-rwxrwxr-x   0 root         (0) root         (0)     4934 2024-05-03 16:00:35.000000 kidiff-2.5.4/kicad-diff-init.py
+-rwxrwxr-x   0 root         (0) root         (0)    37355 2024-05-03 16:00:35.000000 kidiff-2.5.4/kicad-diff.py
+-rwxrwxr-x   0 root         (0) root         (0)     3865 2024-05-03 16:00:35.000000 kidiff-2.5.4/kicad-git-diff.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:03:48.623359 kidiff-2.5.4/kidiff.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14451 2024-05-03 16:03:48.000000 kidiff-2.5.4/kidiff.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      228 2024-05-03 16:03:48.000000 kidiff-2.5.4/kidiff.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 16:03:48.000000 kidiff-2.5.4/kidiff.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-03 16:03:48.000000 kidiff-2.5.4/kidiff.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 16:03:48.000000 kidiff-2.5.4/kidiff.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     1120 2024-05-03 16:03:48.623359 kidiff-2.5.4/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1630 2024-05-03 16:00:35.000000 kidiff-2.5.4/setup.py
```

### Comparing `kidiff-2.5.3/PKG-INFO` & `kidiff-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kidiff
-Version: 2.5.3
+Version: 2.5.4
 Summary: KiCad PCB/SCH Diff
 Home-page: https://github.com/INTI-CMNB/KiDiff/
 Author: Salvador E. Tropea
 Author-email: salvador@inti.gob.ar
 License: GPL-2
 Description: 
         # KiDiff (kicad-diff or kicad_pcb-diff)
@@ -86,14 +86,19 @@
         ```shell
         # make prefix=/usr install
         ```
         
         Note: if you are using Debian, or some derived distro like Ubuntu, you can
         find a Debian package in the releases section.
         
+        ## Docker image
+        
+        You can find a docker image containing KiDiff and other KiCad tools
+        [here](https://github.com/INTI-CMNB/kicad_auto).
+        
         ## Git plug-in
         
         1. Install the scripts
         2. To initialize a repo just run the *kicad_pcb-diff-init.py* script from the
            root of the repo.\
            This will configure the repo to read extra configuration
            from the *.gitconfig* file.\
```

### Comparing `kidiff-2.5.3/README.md` & `kidiff-2.5.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,19 @@
 ```shell
 # make prefix=/usr install
 ```
 
 Note: if you are using Debian, or some derived distro like Ubuntu, you can
 find a Debian package in the releases section.
 
+## Docker image
+
+You can find a docker image containing KiDiff and other KiCad tools
+[here](https://github.com/INTI-CMNB/kicad_auto).
+
 ## Git plug-in
 
 1. Install the scripts
 2. To initialize a repo just run the *kicad_pcb-diff-init.py* script from the
    root of the repo.\
    This will configure the repo to read extra configuration
    from the *.gitconfig* file.\
```

### Comparing `kidiff-2.5.3/kicad-diff-init.py` & `kidiff-2.5.4/kicad-diff-init.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 This program initializes a repo to use the kicad-git-diff plug-in.
 """
 __author__ = 'Salvador E. Tropea'
 __copyright__ = 'Copyright 2020, INTI'
 __credits__ = ['Salvador E. Tropea']
 __license__ = 'GPL 2.0'
-__version__ = '2.5.3'
+__version__ = '2.5.4'
 __email__ = 'stopea@inti.gob.ar'
 __status__ = 'beta'
 __url__ = 'https://github.com/INTI-CMNB/KiDiff/'
 
 import argparse
 import logging
 from os.path import isfile, isdir, basename, sep
```

### Comparing `kidiff-2.5.3/kicad-diff.py` & `kidiff-2.5.4/kicad-diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 For the SCHs we use KiAuto.
 
 """
 __author__ = 'Salvador E. Tropea'
 __copyright__ = 'Copyright 2020-2024, INTI/'+__author__
 __credits__ = ['Salvador E. Tropea', 'Jesse Vincent']
 __license__ = 'GPL 2.0'
-__version__ = '2.5.3'
+__version__ = '2.5.4'
 __email__ = 'salvador@inti.gob.ar'
 __status__ = 'beta'
 __url__ = 'https://github.com/INTI-CMNB/KiDiff/'
 
 import argparse
 import atexit
 import csv
@@ -155,14 +155,18 @@
     logger.debug('Options for cache entry `{}` are the same as current: {}'.format(name, res))
     return res
 
 
 def GenPCBImages(file, file_hash, hash_dir, file_no_ext, layer_names, wanted_layers, kiri_mode, zones_ops):
     # Setup the KiCad plotter
     board = LoadBoard(file)
+    if hasattr(pcbnew, 'LAYER_HIDDEN_TEXT'):
+        # KiCad 8.0.2 crazyness: hidden text affects scaling, even when not plotted
+        # So a PRL can affect the plot mechanism
+        board.SetElementVisibility(pcbnew.LAYER_HIDDEN_TEXT, False)
     pctl = PLOT_CONTROLLER(board)
     popt = pctl.GetPlotOptions()
     popt.SetOutputDirectory(abspath(hash_dir))  # abspath: Otherwise it will be relative to the file
     # Options
     # KiCad 5 only
     if kicad_version_major == 5:
         popt.SetLineWidth(FromMM(0.35))
@@ -490,18 +494,18 @@
     return include
 
 
 def create_diff_stat(old_name, new_name, diff_name, font_size, layer, resolution, name_layer, only_different):
     wn, hn = png_size(new_name)
     wo, ho = png_size(old_name)
     if wn != wo or hn != ho:
-        extent = ' -extent {}x{}'.format(max(wn, wo), max(hn, ho))
+        # extent = ' -extent {}x{}'.format(max(wn, wo), max(hn, ho))
         extra_name = ' [diff page size]'
     else:
-        extra_name = extent = ''
+        extra_name = ''
     # Compare both
     cmd = ['compare',
            # Tolerate 5 % error in color (configurable)
            '-fuzz', str(args.fuzz)+'%',
            # Count how many pixels differ
            '-metric', 'AE',
            new_name,
@@ -786,16 +790,16 @@
     parser.add_argument('--removed_2color', help='Color used for removed stuff in 2color mode', type=str, default='red')
     parser.add_argument('--resolution', help='Image resolution in DPIs [%(default)s]', type=int, default=150)
     parser.add_argument('--threshold', help='Error threshold for diff stats mode, 0 is no error [%(default)s]',
                         type=thre_type, default=0, metavar='[0-1000000]')
     parser.add_argument('--verbose', '-v', action='count', default=0)
     parser.add_argument('--version', action='version', version='%(prog)s '+__version__+' - ' +
                         __copyright__+' - License: '+__license__)
-    parser.add_argument('--zones', help='Un/Fill zones before creating the images', type=str, choices=('fill', 'unfill', 'none'),
-                        default='none')
+    parser.add_argument('--zones', help='Un/Fill zones before creating the images', type=str,
+                        choices=('fill', 'unfill', 'none'), default='none')
 
     args = parser.parse_args()
 
     # Fill the names for the inner layers
     for i in range(1, 30):
         name = 'In'+str(i)+'.Cu'
         DEFAULT_LAYER_NAMES[pcbnew.In1_Cu+i-1] = name
```

### Comparing `kidiff-2.5.3/kicad-git-diff.py` & `kidiff-2.5.4/kicad-git-diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 This program is a git plug-in to generate diffs between two KiCad PCBs.
 It relies on kicad-diff.py script (where the real work is done).
 """
 __author__ = 'Salvador E. Tropea'
 __copyright__ = 'Copyright 2020, INTI'
 __credits__ = ['Salvador E. Tropea', 'Jesse Vincent']
 __license__ = 'GPL 2.0'
-__version__ = '2.5.3'
+__version__ = '2.5.4'
 __email__ = 'salvador@inti.gob.ar'
 __status__ = 'beta'
 __url__ = 'https://github.com/INTI-CMNB/KiDiff/'
 
 import argparse
 import logging
 from os.path import isfile, isdir, basename, sep, dirname, realpath
```

### Comparing `kidiff-2.5.3/kidiff.egg-info/PKG-INFO` & `kidiff-2.5.4/kidiff.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kidiff
-Version: 2.5.3
+Version: 2.5.4
 Summary: KiCad PCB/SCH Diff
 Home-page: https://github.com/INTI-CMNB/KiDiff/
 Author: Salvador E. Tropea
 Author-email: salvador@inti.gob.ar
 License: GPL-2
 Description: 
         # KiDiff (kicad-diff or kicad_pcb-diff)
@@ -86,14 +86,19 @@
         ```shell
         # make prefix=/usr install
         ```
         
         Note: if you are using Debian, or some derived distro like Ubuntu, you can
         find a Debian package in the releases section.
         
+        ## Docker image
+        
+        You can find a docker image containing KiDiff and other KiCad tools
+        [here](https://github.com/INTI-CMNB/kicad_auto).
+        
         ## Git plug-in
         
         1. Install the scripts
         2. To initialize a repo just run the *kicad_pcb-diff-init.py* script from the
            root of the repo.\
            This will configure the repo to read extra configuration
            from the *.gitconfig* file.\
```

### Comparing `kidiff-2.5.3/setup.cfg` & `kidiff-2.5.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `kidiff-2.5.3/setup.py` & `kidiff-2.5.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 #!/usr/bin/python3
+import re
 from setuptools import setup, find_packages
-import importlib
-kidiff = importlib.import_module("kicad-diff")
+
+
+with open("kicad-diff.py", 'rt') as f:
+    txt = f.read()
+    version = re.search(r"__version__ = '(.*)'", txt).group(1)
+    author = re.search(r"__author__ = '(.*)'", txt).group(1)
+    email = re.search(r"__email__ = '(.*)'", txt).group(1)
+    url = re.search(r"__url__ = '(.*)'", txt).group(1)
 
 # Use the README.md as a long description.
 # Note this is also included in the MANIFEST.in
 with open('README.md', encoding='utf-8') as f:
     long_description = '\n' + f.read()
 
 setup(name='kidiff',
-      version=kidiff.__version__,
+      version=version,
       description='KiCad PCB/SCH Diff',
       long_description=long_description,
       long_description_content_type='text/markdown',
-      author=kidiff.__author__,
-      author_email=kidiff.__email__,
-      url=kidiff.__url__,
+      author=author,
+      author_email=email,
+      url=url,
       # Packages are marked using __init__.py
       packages=find_packages(),
       scripts=['kicad-diff-init.py', 'kicad-diff.py', 'kicad-git-diff.py'],
       install_requires=['kiauto'],
       include_package_data=True,
       classifiers=['Development Status :: 5 - Production/Stable',
                    'Environment :: Console',
```


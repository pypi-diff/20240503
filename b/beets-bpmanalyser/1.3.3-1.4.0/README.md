# Comparing `tmp/beets-bpmanalyser-1.3.3.tar.gz` & `tmp/beets-bpmanalyser-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/beets-bpmanalyser-1.3.3.tar", last modified: Mon Mar  2 23:21:43 2020, max compression
+gzip compressed data, was "dist/beets-bpmanalyser-1.4.0.tar", last modified: Fri May  3 20:31:27 2024, max compression
```

## Comparing `beets-bpmanalyser-1.3.3.tar` & `beets-bpmanalyser-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-02 23:21:43.000000 beets-bpmanalyser-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (115)     1067 2020-03-02 23:21:36.000000 beets-bpmanalyser-1.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (115)       49 2020-03-02 23:21:36.000000 beets-bpmanalyser-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (115)     6273 2020-03-02 23:21:43.000000 beets-bpmanalyser-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     4801 2020-03-02 23:21:36.000000 beets-bpmanalyser-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-02 23:21:43.000000 beets-bpmanalyser-1.3.3/beets_bpmanalyser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)     6273 2020-03-02 23:21:43.000000 beets-bpmanalyser-1.3.3/beets_bpmanalyser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)      394 2020-03-02 23:21:43.000000 beets-bpmanalyser-1.3.3/beets_bpmanalyser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-03-02 23:21:43.000000 beets-bpmanalyser-1.3.3/beets_bpmanalyser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)       25 2020-03-02 23:21:43.000000 beets-bpmanalyser-1.3.3/beets_bpmanalyser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)       10 2020-03-02 23:21:43.000000 beets-bpmanalyser-1.3.3/beets_bpmanalyser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-02 23:21:43.000000 beets-bpmanalyser-1.3.3/beetsplug/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-02 23:21:43.000000 beets-bpmanalyser-1.3.3/beetsplug/bpmanalyser/
--rw-r--r--   0 runner    (1001) docker     (115)      685 2020-03-02 23:21:36.000000 beets-bpmanalyser-1.3.3/beetsplug/bpmanalyser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     6226 2020-03-02 23:21:36.000000 beets-bpmanalyser-1.3.3/beetsplug/bpmanalyser/command.py
--rw-r--r--   0 runner    (1001) docker     (115)     1350 2020-03-02 23:21:36.000000 beets-bpmanalyser-1.3.3/beetsplug/bpmanalyser/get_song_bpm.py
--rw-r--r--   0 runner    (1001) docker     (115)      175 2020-03-02 23:21:36.000000 beets-bpmanalyser-1.3.3/beetsplug/bpmanalyser/version.py
--rw-r--r--   0 runner    (1001) docker     (115)      193 2020-03-02 23:21:43.000000 beets-bpmanalyser-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)     1472 2020-03-02 23:21:36.000000 beets-bpmanalyser-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1067 2024-05-03 20:31:16.000000 beets-bpmanalyser-1.4.0/LICENSE.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-05-03 20:31:16.000000 beets-bpmanalyser-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5766 2024-05-03 20:31:16.000000 beets-bpmanalyser-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/beets_bpmanalyser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/beets_bpmanalyser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/beets_bpmanalyser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/beets_bpmanalyser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/beets_bpmanalyser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/beets_bpmanalyser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/beetsplug/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/beetsplug/bpmanalyser/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1293 2024-05-03 20:31:16.000000 beets-bpmanalyser-1.4.0/beetsplug/bpmanalyser/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6278 2024-05-03 20:31:16.000000 beets-bpmanalyser-1.4.0/beetsplug/bpmanalyser/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2038 2024-05-03 20:31:16.000000 beets-bpmanalyser-1.4.0/beetsplug/bpmanalyser/get_song_bpm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-05-03 20:31:16.000000 beets-bpmanalyser-1.4.0/beetsplug/bpmanalyser/version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      193 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1489 2024-05-03 20:31:16.000000 beets-bpmanalyser-1.4.0/setup.py
```

### Comparing `beets-bpmanalyser-1.3.3/LICENSE.txt` & `beets-bpmanalyser-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beets-bpmanalyser-1.3.3/PKG-INFO` & `beets-bpmanalyser-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: beets-bpmanalyser
-Version: 1.3.3
+Version: 1.4.0
 Summary: A beets plugin for analysing tempo of songs and storing it in the bpm tag.
 Home-page: https://github.com/adamjakab/BeetsPluginBpmAnalyser
 Author: Adam Jakab
 Author-email: adam@jakab.pro
 License: MIT
 Description: [![Build Status](https://travis-ci.org/adamjakab/BeetsPluginBpmAnalyser.svg?branch=master)](https://travis-ci.org/adamjakab/BeetsPluginBpmAnalyser)
         [![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginBpmAnalyser/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginBpmAnalyser?branch=master)
         [![PyPi](https://img.shields.io/pypi/v/beets-bpmanalyser.svg)](https://pypi.org/project/beets-bpmanalyser/)
+        [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
         
-        
-        # BPM Analyser (beets plugin)
-        
-        *A [beets](https://github.com/beetbox/beets) plugin for insane obsessive-compulsive music geeks.*
+        # BPM Analyser (Beets Plugin)
         
         The *beets-bpmanalyser* plugin lets you analyse the tempo of the songs you have in your library and write the bpm information on the bpm tag of your media files.
         
+        This plugin has a more powerful big brother which does much more than just extracting bpm: [beets-xtractor plugin](https://github.com/adamjakab/BeetsPluginXtractor).
+        
         
         ## Installation
         The plugin can be installed via:
         
         ```shell script
         $ pip install beets-bpmanalyser
         ```
@@ -46,15 +46,15 @@
           dry-run: no
           write: yes
           threads: 2
           force: no
           quiet: no
         ```
         
-        Heads up! THe `auto` option is NOT YET IMPLEMENTED! It will be used to execute the analysis during import.
+        You can set the `auto` option if you would like to execute the analysis during import. In this case, the `threads` option is ignored (beets import is already multithreaded).
         
         
         The other configuration options can also be set from the command line when running the plugin. 
         Here are the options explained:
         
         *-d, --dry-run*     : Do not update the library or the media files. Only display the bpm values.
         
@@ -109,21 +109,39 @@
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/05. Soul Stripper.mp3] bpm: 132
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/06. You Ain't Got a Hold on Me.mp3] bpm: 128
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/07. Love Song.mp3] bpm: 125
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/08. Show Business.mp3] bpm: 139
         ```
          
         
-        ## Development Notes 
-        Read the [development](./DEVELOPMENT.md) docs.
+        ## Issues
+        If something is not working as expected please use the Issue tracker.
+        If the documentation is not clear please use the Issue tracker.
+        If you have a feature request please use the Issue tracker.
+        In any other situation please use the Issue tracker.
+        
+        
+        ## Other plugins by the same author
+        - [beets-goingrunning](https://github.com/adamjakab/BeetsPluginGoingRunning)
+        - [beets-xtractor](https://github.com/adamjakab/BeetsPluginXtractor)
+        - [beets-yearfixer](https://github.com/adamjakab/BeetsPluginYearFixer)
+        - [beets-autofix](https://github.com/adamjakab/BeetsPluginAutofix)
+        - [beets-describe](https://github.com/adamjakab/BeetsPluginDescribe)
+        - [beets-bpmanalyser](https://github.com/adamjakab/BeetsPluginBpmAnalyser)
+        - [beets-template](https://github.com/adamjakab/BeetsPluginTemplate)
         
         
         ## Acknowledgements
         Many thanks to the developers and contributors of the [beets check plugin](https://github.com/geigerzaehler/beets-check). Some structural concepts and best practices were adopted to start on this plugin. 
         
+        
+        ## Final Remarks
+        Enjoy!
+        
+        
 Platform: ALL
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
```

### Comparing `beets-bpmanalyser-1.3.3/README.md` & `beets-bpmanalyser-1.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [![Build Status](https://travis-ci.org/adamjakab/BeetsPluginBpmAnalyser.svg?branch=master)](https://travis-ci.org/adamjakab/BeetsPluginBpmAnalyser)
 [![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginBpmAnalyser/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginBpmAnalyser?branch=master)
 [![PyPi](https://img.shields.io/pypi/v/beets-bpmanalyser.svg)](https://pypi.org/project/beets-bpmanalyser/)
+[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
 
-
-# BPM Analyser (beets plugin)
-
-*A [beets](https://github.com/beetbox/beets) plugin for insane obsessive-compulsive music geeks.*
+# BPM Analyser (Beets Plugin)
 
 The *beets-bpmanalyser* plugin lets you analyse the tempo of the songs you have in your library and write the bpm information on the bpm tag of your media files.
 
+This plugin has a more powerful big brother which does much more than just extracting bpm: [beets-xtractor plugin](https://github.com/adamjakab/BeetsPluginXtractor).
+
 
 ## Installation
 The plugin can be installed via:
 
 ```shell script
 $ pip install beets-bpmanalyser
 ```
@@ -38,15 +38,15 @@
   dry-run: no
   write: yes
   threads: 2
   force: no
   quiet: no
 ```
 
-Heads up! THe `auto` option is NOT YET IMPLEMENTED! It will be used to execute the analysis during import.
+You can set the `auto` option if you would like to execute the analysis during import. In this case, the `threads` option is ignored (beets import is already multithreaded).
 
 
 The other configuration options can also be set from the command line when running the plugin. 
 Here are the options explained:
 
 *-d, --dry-run*     : Do not update the library or the media files. Only display the bpm values.
 
@@ -101,13 +101,31 @@
 bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/05. Soul Stripper.mp3] bpm: 132
 bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/06. You Ain't Got a Hold on Me.mp3] bpm: 128
 bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/07. Love Song.mp3] bpm: 125
 bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/08. Show Business.mp3] bpm: 139
 ```
  
 
-## Development Notes 
-Read the [development](./DEVELOPMENT.md) docs.
+## Issues
+If something is not working as expected please use the Issue tracker.
+If the documentation is not clear please use the Issue tracker.
+If you have a feature request please use the Issue tracker.
+In any other situation please use the Issue tracker.
+
+
+## Other plugins by the same author
+- [beets-goingrunning](https://github.com/adamjakab/BeetsPluginGoingRunning)
+- [beets-xtractor](https://github.com/adamjakab/BeetsPluginXtractor)
+- [beets-yearfixer](https://github.com/adamjakab/BeetsPluginYearFixer)
+- [beets-autofix](https://github.com/adamjakab/BeetsPluginAutofix)
+- [beets-describe](https://github.com/adamjakab/BeetsPluginDescribe)
+- [beets-bpmanalyser](https://github.com/adamjakab/BeetsPluginBpmAnalyser)
+- [beets-template](https://github.com/adamjakab/BeetsPluginTemplate)
 
 
 ## Acknowledgements
 Many thanks to the developers and contributors of the [beets check plugin](https://github.com/geigerzaehler/beets-check). Some structural concepts and best practices were adopted to start on this plugin. 
+
+
+## Final Remarks
+Enjoy!
+
```

### Comparing `beets-bpmanalyser-1.3.3/beets_bpmanalyser.egg-info/PKG-INFO` & `beets-bpmanalyser-1.4.0/beets_bpmanalyser.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: beets-bpmanalyser
-Version: 1.3.3
+Version: 1.4.0
 Summary: A beets plugin for analysing tempo of songs and storing it in the bpm tag.
 Home-page: https://github.com/adamjakab/BeetsPluginBpmAnalyser
 Author: Adam Jakab
 Author-email: adam@jakab.pro
 License: MIT
 Description: [![Build Status](https://travis-ci.org/adamjakab/BeetsPluginBpmAnalyser.svg?branch=master)](https://travis-ci.org/adamjakab/BeetsPluginBpmAnalyser)
         [![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginBpmAnalyser/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginBpmAnalyser?branch=master)
         [![PyPi](https://img.shields.io/pypi/v/beets-bpmanalyser.svg)](https://pypi.org/project/beets-bpmanalyser/)
+        [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
         
-        
-        # BPM Analyser (beets plugin)
-        
-        *A [beets](https://github.com/beetbox/beets) plugin for insane obsessive-compulsive music geeks.*
+        # BPM Analyser (Beets Plugin)
         
         The *beets-bpmanalyser* plugin lets you analyse the tempo of the songs you have in your library and write the bpm information on the bpm tag of your media files.
         
+        This plugin has a more powerful big brother which does much more than just extracting bpm: [beets-xtractor plugin](https://github.com/adamjakab/BeetsPluginXtractor).
+        
         
         ## Installation
         The plugin can be installed via:
         
         ```shell script
         $ pip install beets-bpmanalyser
         ```
@@ -46,15 +46,15 @@
           dry-run: no
           write: yes
           threads: 2
           force: no
           quiet: no
         ```
         
-        Heads up! THe `auto` option is NOT YET IMPLEMENTED! It will be used to execute the analysis during import.
+        You can set the `auto` option if you would like to execute the analysis during import. In this case, the `threads` option is ignored (beets import is already multithreaded).
         
         
         The other configuration options can also be set from the command line when running the plugin. 
         Here are the options explained:
         
         *-d, --dry-run*     : Do not update the library or the media files. Only display the bpm values.
         
@@ -109,21 +109,39 @@
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/05. Soul Stripper.mp3] bpm: 132
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/06. You Ain't Got a Hold on Me.mp3] bpm: 128
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/07. Love Song.mp3] bpm: 125
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/08. Show Business.mp3] bpm: 139
         ```
          
         
-        ## Development Notes 
-        Read the [development](./DEVELOPMENT.md) docs.
+        ## Issues
+        If something is not working as expected please use the Issue tracker.
+        If the documentation is not clear please use the Issue tracker.
+        If you have a feature request please use the Issue tracker.
+        In any other situation please use the Issue tracker.
+        
+        
+        ## Other plugins by the same author
+        - [beets-goingrunning](https://github.com/adamjakab/BeetsPluginGoingRunning)
+        - [beets-xtractor](https://github.com/adamjakab/BeetsPluginXtractor)
+        - [beets-yearfixer](https://github.com/adamjakab/BeetsPluginYearFixer)
+        - [beets-autofix](https://github.com/adamjakab/BeetsPluginAutofix)
+        - [beets-describe](https://github.com/adamjakab/BeetsPluginDescribe)
+        - [beets-bpmanalyser](https://github.com/adamjakab/BeetsPluginBpmAnalyser)
+        - [beets-template](https://github.com/adamjakab/BeetsPluginTemplate)
         
         
         ## Acknowledgements
         Many thanks to the developers and contributors of the [beets check plugin](https://github.com/geigerzaehler/beets-check). Some structural concepts and best practices were adopted to start on this plugin. 
         
+        
+        ## Final Remarks
+        Enjoy!
+        
+        
 Platform: ALL
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
```

### Comparing `beets-bpmanalyser-1.3.3/beetsplug/bpmanalyser/__init__.py` & `beets-bpmanalyser-1.4.0/beetsplug/bpmanalyser/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,43 @@
 #  Copyright: Copyright (c) 2020., Adam Jakab
 #
 #  Author: Adam Jakab <adam at jakab dot pro>
 #  Created: 2/23/20, 10:50 PM
 #  License: See LICENSE.txt
 
+import logging
 
 from beets.plugins import BeetsPlugin
 from beets.util import cpu_count
+from beetsplug.bpmanalyser.command import BpmAnalyserCommand
 
-from beetsplug.bpmanalyser.command import BpmAnayserCommand
+log = logging.getLogger('beets.bpmanalyser')
 
 
 class BpmAnalyserPlugin(BeetsPlugin):
     def __init__(self):
         super(BpmAnalyserPlugin, self).__init__()
         self.config.add({
             'auto': False,
             'dry-run': False,
             'write': True,
             'threads': cpu_count(),
             'force': False,
             'quiet': False
         })
 
+        # On-import analysis.
+        if self.config['auto']:
+            self.import_stages = [self.imported]
+
     def commands(self):
-        return [BpmAnayserCommand(self.config)]
+        return [BpmAnalyserCommand(self.config)]
+
+    def imported(self, session, task):
+        # Add BPM for imported items.
+        for item in task.imported_items():
+            if not self.config['force'] and item['bpm'] != 0:
+                item_path = item.get("path").decode("utf-8")
+                log.debug("Skipping item with existing BPM[{0}]...".format(item_path))
+                return
+            else:
+                BpmAnalyserCommand(self.config).analyse(item)
```

### Comparing `beets-bpmanalyser-1.3.3/beetsplug/bpmanalyser/command.py` & `beets-bpmanalyser-1.4.0/beetsplug/bpmanalyser/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,45 +2,43 @@
 #
 #  Author: Adam Jakab <adam at jakab dot pro>
 #  Created: 2/23/20, 10:53 PM
 #  License: See LICENSE.txt
 
 import logging
 import os
+import sys
 from concurrent import futures
 from optparse import OptionParser
 from subprocess import Popen, PIPE
-import sys
 
-from beets.library import Library as BeatsLibrary
+from beets.library import Library as BeatsLibrary, Item
 from beets.ui import Subcommand, decargs
 
 # Module methods
 log = logging.getLogger('beets.bpmanalyser')
 
 
-class BpmAnayserCommand(Subcommand):
+class BpmAnalyserCommand(Subcommand):
     config = None
     lib = None
     query = None
     parser = None
 
-    cfg_auto = False
     cfg_dry_run = False
     cfg_write = True
     cfg_threads = 1
     cfg_force = False
     cfg_quiet = False
 
     analyser_script_path = None
 
     def __init__(self, cfg):
         self.config = cfg.flatten()
 
-        self.cfg_auto = self.config.get("auto")
         self.cfg_dry_run = self.config.get("dry-run")
         self.cfg_write = self.config.get("write")
         self.cfg_threads = self.config.get("threads")
         self.cfg_force = self.config.get("force")
         self.cfg_version = False
         self.cfg_quiet = self.config.get("quiet")
 
@@ -88,15 +86,15 @@
         self.parser.add_option(
             '-v', '--version',
             action='store_true', dest='version', default=self.cfg_version,
             help=u'show plugin version'
         )
 
         # Keep this at the end
-        super(BpmAnayserCommand, self).__init__(
+        super(BpmAnalyserCommand, self).__init__(
             parser=self.parser,
             name='bpmanalyser',
             help=u'analyse your songs for tempo and write it into the bpm tag'
         )
 
     def func(self, lib: BeatsLibrary, options, arguments):
         self.cfg_dry_run = options.dryrun
@@ -117,52 +115,58 @@
 
     def show_version_information(self):
         from beetsplug.bpmanalyser.version import __version__
         self._say(
             "Bpm Analyser(beets-bpmanalyser) plugin for Beets: v{0}".format(
                 __version__))
 
-    def analyse_songs(self):
+    def find_analyser_script(self):
         module_path = os.path.dirname(__file__)
         self.analyser_script_path = os.path.join(module_path, "get_song_bpm.py")
         log.debug("External script path: {}".format(self.analyser_script_path))
         if not os.path.isfile(self.analyser_script_path):
             raise FileNotFoundError("Analyser script not found!")
 
+    def analyse(self, item: Item):
+        if not self.analyser_script_path:
+            self.find_analyser_script()
+
+        item_path = item.get("path").decode("utf-8")
+        log.debug("Analysing[{0}]...".format(item_path))
+
+        bpm, errors = self.get_bpm_from_analyser_script(item_path)
+
+        if bpm == 0:
+            self._say("Bpm[ERROR]: - {}".format(item_path))
+            # self._say("Bpm[ERROR]: - {}".format(errors))
+        else:
+            self._say("Bpm[{}]: {}".format(bpm, item_path))
+
+        if not self.cfg_dry_run:
+            if bpm != 0:
+                item['bpm'] = bpm
+                if self.cfg_write:
+                    item.try_write()
+                item.store()
+
+    def analyse_songs(self):
+        self.find_analyser_script()
+
         # Setup the query
         query = self.query
         if not self.cfg_force:
             query_element = "bpm:0"
             query.append(query_element)
 
         # Get the library items
         # @todo: implement a limit option so that user can decide to do only
         #  a limited number of items per run
         items = self.lib.items(self.query)
 
-        def analyse(item):
-            item_path = item.get("path").decode("utf-8")
-            log.debug("Analysing[{0}]...".format(item_path))
-
-            bpm, errors = self.get_bpm_from_analyser_script(item_path)
-
-            if bpm == 0:
-                self._say("Bpm[ERROR]: - {}".format(item_path))
-                # self._say("Bpm[ERROR]: - {}".format(errors))
-            else:
-                self._say("Bpm[{}]: {}".format(bpm, item_path))
-
-            if not self.cfg_dry_run:
-                if bpm != 0:
-                    item['bpm'] = bpm
-                    if self.cfg_write:
-                        item.try_write()
-                    item.store()
-
-        self.execute_on_items(items, analyse, msg='Analysing tempo...')
+        self.execute_on_items(items, self.analyse, msg='Analysing tempo...')
 
     def get_bpm_from_analyser_script(self, item_path):
         log.debug(
             "calling external script: {}".format(self.analyser_script_path))
 
         proc = Popen([sys.executable, self.analyser_script_path, item_path],
                      stdout=PIPE, stderr=PIPE)
```

### Comparing `beets-bpmanalyser-1.3.3/beetsplug/bpmanalyser/get_song_bpm.py` & `beets-bpmanalyser-1.4.0/beetsplug/bpmanalyser/get_song_bpm.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,24 +6,28 @@
 #
 # The aubio/ffmpeg can produce some really ugly output on stderr:
 # [mp3float @ 0x...] Could not update timestamps for skipped samples.
 # [mp3float @ 0x...] Could not update timestamps for discarded samples.
 
 import os
 import sys
+import hashlib
+import tempfile
 
 from aubio import source, tempo
 from numpy import diff, median
+from pydub import AudioSegment
 
-
+__FRAME_RATE__ = 44100
+    
 def _analyse_tempo(item_path):
-    sample_rate, win_s, hop_s = 44100, 1024, 512
+    sample_rate, win_s, hop_s = __FRAME_RATE__, 1024, 512
     src = source(item_path, sample_rate, hop_s)
-    sample_rate = src.samplerate
-    o = tempo("default", win_s, hop_s, sample_rate)
+    # sample_rate = src.samplerate
+    o = tempo("default", win_s, hop_s, __FRAME_RATE__)
 
     beats = []
     total_frames = 0
     while True:
         samples, read = src()
         is_beat = o(samples)
         if is_beat:
@@ -33,21 +37,37 @@
         if read < hop_s:
             break
 
     bpms = 60.0 / diff(beats)
 
     return int(median(bpms))
 
+def _convert_audio_to_wav(item_path):
+    tempdir = tempfile.gettempdir()
+    filename = hashlib.md5(item_path.encode('utf-8')).hexdigest()
+    wav_path = "{dir}/{file}.wav".format(dir=tempdir, file=filename)
+    
+    sound = AudioSegment.from_file(item_path)
+    if (sound.frame_rate != __FRAME_RATE__):
+        sound = sound.set_frame_rate(__FRAME_RATE__)
+    sound.export(wav_path, format="wav")
+    return wav_path
+
+def _convert_and_analyse(item_path):
+    wav_path = _convert_audio_to_wav(item_path)
+    bpm = _analyse_tempo(wav_path)
+    os.remove(wav_path)
+    return bpm
+
 
 if __name__ == '__main__':
     if len(sys.argv) != 2:
         sys.stderr.write("Usage: python get_song_bpm.py song_path" + "\n")
         sys.exit(1)
 
     file_name = sys.argv[1]
-
     if not os.path.isfile(file_name):
         sys.stderr.write("Audio file not found" + "\n")
         sys.exit(1)
 
-    bpm = _analyse_tempo(file_name)
+    bpm = _convert_and_analyse(file_name)
     print(bpm)
```

### Comparing `beets-bpmanalyser-1.3.3/setup.py` & `beets-bpmanalyser-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,17 @@
     include_package_data=True,
     test_suite='test',
 
     packages=['beetsplug.bpmanalyser'],
 
     install_requires=[
         'beets>=1.4.9',
+        'aubio',
         'numpy',
-        'aubio'
+        'pydub'
     ],
 
     tests_require=[
         'pytest', 'nose', 'coverage',
         'mock', 'six'
     ],
```


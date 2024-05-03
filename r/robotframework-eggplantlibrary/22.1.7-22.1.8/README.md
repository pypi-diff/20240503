# Comparing `tmp/robotframework-eggplantlibrary-22.1.7.tar.gz` & `tmp/robotframework_eggplantlibrary-22.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-eggplantlibrary-22.1.7.tar", last modified: Wed Feb 16 17:12:21 2022, max compression
+gzip compressed data, was "robotframework_eggplantlibrary-22.1.8.tar", last modified: Fri May  3 11:25:46 2024, max compression
```

## Comparing `robotframework-eggplantlibrary-22.1.7.tar` & `robotframework_eggplantlibrary-22.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 17:12:21.797821 robotframework-eggplantlibrary-22.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 17:12:21.793820 robotframework-eggplantlibrary-22.1.7/EggplantLibrary/
--rw-r--r--   0 runner    (1001) docker     (121)    11189 2022-02-16 17:12:15.000000 robotframework-eggplantlibrary-22.1.7/EggplantLibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    34303 2022-02-16 17:12:15.000000 robotframework-eggplantlibrary-22.1.7/EggplantLibrary/libcore.py
--rw-r--r--   0 runner    (1001) docker     (121)    11026 2022-02-16 17:12:15.000000 robotframework-eggplantlibrary-22.1.7/EggplantLibrary/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-02-16 17:12:15.000000 robotframework-eggplantlibrary-22.1.7/EggplantLibrary/version.py
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-02-16 17:12:15.000000 robotframework-eggplantlibrary-22.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-02-16 17:12:21.797821 robotframework-eggplantlibrary-22.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13511 2022-02-16 17:12:15.000000 robotframework-eggplantlibrary-22.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 17:12:21.793820 robotframework-eggplantlibrary-22.1.7/robotframework_eggplantlibrary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-02-16 17:12:21.000000 robotframework-eggplantlibrary-22.1.7/robotframework_eggplantlibrary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-02-16 17:12:21.000000 robotframework-eggplantlibrary-22.1.7/robotframework_eggplantlibrary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-16 17:12:21.000000 robotframework-eggplantlibrary-22.1.7/robotframework_eggplantlibrary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-02-16 17:12:21.000000 robotframework-eggplantlibrary-22.1.7/robotframework_eggplantlibrary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-16 17:12:21.000000 robotframework-eggplantlibrary-22.1.7/robotframework_eggplantlibrary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-16 17:12:21.797821 robotframework-eggplantlibrary-22.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-02-16 17:12:15.000000 robotframework-eggplantlibrary-22.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:46.571834 robotframework_eggplantlibrary-22.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:46.571834 robotframework_eggplantlibrary-22.1.8/EggplantLibrary/
+-rw-r--r--   0 runner    (1001) docker     (127)    11184 2024-05-03 11:25:39.000000 robotframework_eggplantlibrary-22.1.8/EggplantLibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34303 2024-05-03 11:25:39.000000 robotframework_eggplantlibrary-22.1.8/EggplantLibrary/libcore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-05-03 11:25:39.000000 robotframework_eggplantlibrary-22.1.8/EggplantLibrary/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 11:25:39.000000 robotframework_eggplantlibrary-22.1.8/EggplantLibrary/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 11:25:39.000000 robotframework_eggplantlibrary-22.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-03 11:25:46.571834 robotframework_eggplantlibrary-22.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13903 2024-05-03 11:25:39.000000 robotframework_eggplantlibrary-22.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:46.571834 robotframework_eggplantlibrary-22.1.8/robotframework_eggplantlibrary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-03 11:25:46.000000 robotframework_eggplantlibrary-22.1.8/robotframework_eggplantlibrary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-03 11:25:46.000000 robotframework_eggplantlibrary-22.1.8/robotframework_eggplantlibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:25:46.000000 robotframework_eggplantlibrary-22.1.8/robotframework_eggplantlibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 11:25:46.000000 robotframework_eggplantlibrary-22.1.8/robotframework_eggplantlibrary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 11:25:46.000000 robotframework_eggplantlibrary-22.1.8/robotframework_eggplantlibrary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:25:46.571834 robotframework_eggplantlibrary-22.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-03 11:25:39.000000 robotframework_eggplantlibrary-22.1.8/setup.py
```

### Comparing `robotframework-eggplantlibrary-22.1.7/EggplantLibrary/__init__.py` & `robotframework_eggplantlibrary-22.1.8/EggplantLibrary/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     So the scripts themselves have to be created in eggPlant, not in Robot Framework.        
 
     The eggPlant itself should be launched in eggDrive mode from outside.
 
     See the [https://github.com/amochin/robotframework-eggplant|Eggplant Library homepage] for more information.
     """
     ROBOT_LIBRARY_VERSION = VERSION
-    ROBOT_LIBRARY_SCOPE = 'TEST SUITE'
+    ROBOT_LIBRARY_SCOPE = 'SUITE'
 
     # ---------- static keywords ------------------------------
     @keyword
     def set_eggdrive_connection(self, host='http://127.0.0.1', port='5400'):
         """
         Defines connection to running instance of eggPlant in the eggDrive mode
         (XML RPC Server).
```

### Comparing `robotframework-eggplantlibrary-22.1.7/EggplantLibrary/libcore.py` & `robotframework_eggplantlibrary-22.1.8/EggplantLibrary/libcore.py`

 * *Files identical despite different names*

### Comparing `robotframework-eggplantlibrary-22.1.7/EggplantLibrary/utils.py` & `robotframework_eggplantlibrary-22.1.8/EggplantLibrary/utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-eggplantlibrary-22.1.7/LICENSE` & `robotframework_eggplantlibrary-22.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-eggplantlibrary-22.1.7/PKG-INFO` & `robotframework_eggplantlibrary-22.1.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: robotframework-eggplantlibrary
-Version: 22.1.7
+Version: 22.1.8
 Summary: Robot Framework eggPlant Library
 Home-page: https://github.com/amochin/robotframework-eggplant
 Author: Andrei Mochinin
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Framework :: Robot Framework :: Library
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: robotframework
+Requires-Dist: Pillow
 
 
 The Eggplant Library for [Robot Framework](https://robotframework.org/) allows calling
 [eggPlant Functional](https://www.eggplantsoftware.com/eggplant-functional-downloads) scripts via XML RPC
 using [eggDrive](http://docs.testplant.com/ePF/using/epf-about-eggdrive.htm).  
 It considers **eggPlant scripts as low level keywords** and exposes them for usage in **high level keywords and test cases in Robot Framework**.  
 So the scripts themselves have to be created in eggPlant, not in Robot Framework.        
 
 The eggPlant itself should be launched in eggDrive mode from outside.
 
 See the [Eggplant Library homepage](https://github.com/amochin/robotframework-eggplant) for more information.
-
-
```

### Comparing `robotframework-eggplantlibrary-22.1.7/README.md` & `robotframework_eggplantlibrary-22.1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 So the scripts themselves have to be created in eggPlant, not in Robot Framework.
 
 The eggPlant itself should be launched in eggDrive mode from outside -
 see the scripts `start_eggPlant.bat` and `stop_eggPlant.bat` for example.
 
 ![Architecture picture](Architecture.png)
 
+Watch my talk from [Robocon 2022](https://youtu.be/wOGVdWEzs_A)!
+
+[![Eggplant Library presentation at RoboCon 2022](http://img.youtube.com/vi/wOGVdWEzs_A/0.jpg)](https://youtu.be/wOGVdWEzs_A "Eggplant Library presentation at RoboCon 2022")
+
 - [Quick Start](#quick-start)
 - [eggPlant compatibility](#eggplant-compatibility)
 - [Importing library](#importing-library)
 - [Keywords](#keywords)
 - [Library usage in VS Code](#library-usage-in-vs-code)
 - [Running self-tests](#running-self-tests)
 ## Quick start
@@ -168,26 +172,18 @@
 
 ### Static keywords
 
 The library also contains several built in keywords (independent from actually available eggPlant scripts) for taking screenshots, opening and closing eggPlant sessions and connections to eggDrive and SUT.
 
 ### Creating keyword documentation
 
-You can use _libdoc_ to build the keyword documentation file:
-
-- Static keywords only
-
-  ```shell
-    libdoc EggplantLibrary docs_static_keywords.html
-  ```
-
-- All keywords - including eggPlant scripts and static keywords as well
+You can use _libdoc_ to build the keyword documentation file. This will include eggPlant scripts and static keywords as well:
 
   ```shell
-    libdoc EggplantLibrary::../tests/keywords/eggPlantScripts/SuiteOne.suite docs_example_with_eggplant_scripts.html
+    libdoc EggplantLibrary::<Full path to eggplant suite> keywords_docs.html
   ```
 
 ### Keywords accept arguments
 
 Use standard Robot Framework argument format:
 
 ```robotframework
@@ -251,15 +247,17 @@
     "robot.libraries.libdoc.needsArgs": ["EggplantLibrary"]
     ```
 2. Alternatively you can use the [config file](#config-file-example) to specify library parameters.
     - You don't have to change the existing library import with parameters in RF test suite files -
    VS code processes the import, but ignores the parameters.
     - Direct library import parameters in RF files always have a higher pirority than config file values.
     - You may use only some of import parameters - both in RF files and in a config file.  
-    - There is no need to reload VS Code after adding or changing eggplant script files - the Language Server extension should detect the changes and update the keyword names for code completion automatically.
+
+There is no need to reload VS Code after adding or changing eggplant script files - the Language Server extension should detect the changes and update the keyword names for code completion automatically.     
+If you're having issues with it, try to regenerate the library specification files - just delete the `EggplantLibrary<...>.libspec` and `EggplantLibrary<...>.libspec.m` files in the LanguageServer specs folder - usually located somewhere in `<user_profile>/.robotframework-ls/specs/<...>/user`.
 
 
 Note that importing library directly as a python file via path doesn't work for VS Code -
 instead you should use module name with the correct `robot.pythonpath` in the Language Server extension settings.  
 It shouldn't be a problem when installing library as a normal user,
 but might be necessary for library development and maintenance.
```

### Comparing `robotframework-eggplantlibrary-22.1.7/robotframework_eggplantlibrary.egg-info/PKG-INFO` & `robotframework_eggplantlibrary-22.1.8/robotframework_eggplantlibrary.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: robotframework-eggplantlibrary
-Version: 22.1.7
+Version: 22.1.8
 Summary: Robot Framework eggPlant Library
 Home-page: https://github.com/amochin/robotframework-eggplant
 Author: Andrei Mochinin
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Framework :: Robot Framework :: Library
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: robotframework
+Requires-Dist: Pillow
 
 
 The Eggplant Library for [Robot Framework](https://robotframework.org/) allows calling
 [eggPlant Functional](https://www.eggplantsoftware.com/eggplant-functional-downloads) scripts via XML RPC
 using [eggDrive](http://docs.testplant.com/ePF/using/epf-about-eggdrive.htm).  
 It considers **eggPlant scripts as low level keywords** and exposes them for usage in **high level keywords and test cases in Robot Framework**.  
 So the scripts themselves have to be created in eggPlant, not in Robot Framework.        
 
 The eggPlant itself should be launched in eggDrive mode from outside.
 
 See the [Eggplant Library homepage](https://github.com/amochin/robotframework-eggplant) for more information.
-
-
```

### Comparing `robotframework-eggplantlibrary-22.1.7/setup.py` & `robotframework_eggplantlibrary-22.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     url="https://github.com/amochin/robotframework-eggplant",
     license = 'Apache License 2.0',
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: Microsoft :: Windows",
         "License :: OSI Approved :: Apache Software License",
+        "Framework :: Robot Framework :: Library",
     ],
     install_requires=[
         'robotframework',
         'Pillow',
     ],
     python_requires='>=3.9',
-)
+)
```


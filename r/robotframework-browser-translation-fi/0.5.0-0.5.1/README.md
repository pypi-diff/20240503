# Comparing `tmp/robotframework_browser_translation_fi-0.5.0.tar.gz` & `tmp/robotframework_browser_translation_fi-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_browser_translation_fi-0.5.0.tar", last modified: Fri May  3 19:22:01 2024, max compression
+gzip compressed data, was "robotframework_browser_translation_fi-0.5.1.tar", last modified: Fri May  3 20:06:16 2024, max compression
```

## Comparing `robotframework_browser_translation_fi-0.5.0.tar` & `robotframework_browser_translation_fi-0.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:22:01.470982 robotframework_browser_translation_fi-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 19:21:17.000000 robotframework_browser_translation_fi-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16513 2024-05-03 19:22:01.470982 robotframework_browser_translation_fi-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-03 19:21:17.000000 robotframework_browser_translation_fi-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-03 19:21:57.000000 robotframework_browser_translation_fi-0.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:22:01.470982 robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi/
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-03 19:21:57.000000 robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   295024 2024-05-03 19:21:17.000000 robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi/translation.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:22:01.470982 robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16513 2024-05-03 19:22:01.000000 robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-03 19:22:01.000000 robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:22:01.000000 robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 19:22:01.000000 robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:22:01.000000 robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:22:01.474982 robotframework_browser_translation_fi-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:06:16.245405 robotframework_browser_translation_fi-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 20:05:32.000000 robotframework_browser_translation_fi-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17161 2024-05-03 20:06:16.245405 robotframework_browser_translation_fi-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-03 20:05:32.000000 robotframework_browser_translation_fi-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-03 20:06:12.000000 robotframework_browser_translation_fi-0.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:06:16.241405 robotframework_browser_translation_fi-0.5.1/robotframework_browser_translation_fi/
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-03 20:06:12.000000 robotframework_browser_translation_fi-0.5.1/robotframework_browser_translation_fi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   295024 2024-05-03 20:05:32.000000 robotframework_browser_translation_fi-0.5.1/robotframework_browser_translation_fi/translation.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:06:16.245405 robotframework_browser_translation_fi-0.5.1/robotframework_browser_translation_fi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17161 2024-05-03 20:06:16.000000 robotframework_browser_translation_fi-0.5.1/robotframework_browser_translation_fi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-03 20:06:16.000000 robotframework_browser_translation_fi-0.5.1/robotframework_browser_translation_fi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:06:16.000000 robotframework_browser_translation_fi-0.5.1/robotframework_browser_translation_fi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 20:06:16.000000 robotframework_browser_translation_fi-0.5.1/robotframework_browser_translation_fi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:06:16.000000 robotframework_browser_translation_fi-0.5.1/robotframework_browser_translation_fi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:06:16.245405 robotframework_browser_translation_fi-0.5.1/setup.cfg
```

### Comparing `robotframework_browser_translation_fi-0.5.0/LICENSE` & `robotframework_browser_translation_fi-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_browser_translation_fi-0.5.0/PKG-INFO` & `robotframework_browser_translation_fi-0.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-browser-translation-fi
-Version: 0.5.0
+Version: 0.5.1
 Summary: Robot Framework Browser library translation to Finnish languege
 Author-email: Tatu Aalto <aalto.tatu@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -253,14 +253,25 @@
 library is imported with:
 
 ```robotRobotFramework
 *** Settings ***
 Library    Browser    languege=fi
 ```
 
+## Detect changes in documentation
+The
+[translation.json](https://github.com/MarketSquare/robotframework-browser-translation-fi/blob/main/ robotframework_browser_translation_fi/translation.json)
+contains sha256 sum, which is generated by the Browser library. The sha356
+is the checksum of the original documentation of the Browser library documentation.
+The checksum is used by
+`fbrowser translation --compare robotframework_browser_translation_fi/translation.json`
+command to compare translation between the library and translation file. Command will
+display a list of keywords which needs updating or are missing from the translation.json
+file.
+
 ## Contributors
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
```

### Comparing `robotframework_browser_translation_fi-0.5.0/README.md` & `robotframework_browser_translation_fi-0.5.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -26,14 +26,25 @@
 library is imported with:
 
 ```robotRobotFramework
 *** Settings ***
 Library    Browser    languege=fi
 ```
 
+## Detect changes in documentation
+The
+[translation.json](https://github.com/MarketSquare/robotframework-browser-translation-fi/blob/main/ robotframework_browser_translation_fi/translation.json)
+contains sha256 sum, which is generated by the Browser library. The sha356
+is the checksum of the original documentation of the Browser library documentation.
+The checksum is used by
+`fbrowser translation --compare robotframework_browser_translation_fi/translation.json`
+command to compare translation between the library and translation file. Command will
+display a list of keywords which needs updating or are missing from the translation.json
+file.
+
 ## Contributors
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
```

#### html2text {}

```diff
@@ -15,11 +15,20 @@
 translation.json) file for the Browser library. Browser library searches Python
 plugins by using naming convention: `robotframework_browser_translation`. This
 module fulfils the Browser library translation API and provides `get_language`
 metghod. The method return a dictionry: ```Python {"language": "fi", "path": "/
 opath/to/translation.json")} ``` Which Browser library will use to match
 correct translation from all the found Python plugins. Languea search is
 enabled when Browser library is imported with: ```robotRobotFramework ***
-Settings *** Library Browser languege=fi ``` ## Contributors
+Settings *** Library Browser languege=fi ``` ## Detect changes in documentation
+The [translation.json](https://github.com/MarketSquare/robotframework-browser-
+translation-fi/blob/main/ robotframework_browser_translation_fi/
+translation.json) contains sha256 sum, which is generated by the Browser
+library. The sha356 is the checksum of the original documentation of the
+Browser library documentation. The checksum is used by `fbrowser translation --
+compare robotframework_browser_translation_fi/translation.json` command to
+compare translation between the library and translation file. Command will
+display a list of keywords which needs updating or are missing from the
+translation.json file. ## Contributors
 _[_T_a_t_u_ _A_a_l_t_o_]
  _TT_aa_tt_uu_ _AA_aa_ll_tt_oo
  _ð___» _ð___
```

### Comparing `robotframework_browser_translation_fi-0.5.0/pyproject.toml` & `robotframework_browser_translation_fi-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "robotframework-browser-translation-fi"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
   { name="Tatu Aalto", email="aalto.tatu@gmail.com" },
 ]
 license = {file = "LICENSE"}
 description = "Robot Framework Browser library translation to Finnish languege"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi/__init__.py` & `robotframework_browser_translation_fi-0.5.1/robotframework_browser_translation_fi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from pathlib import Path
 from typing import TypedDict
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 
 class Language(TypedDict):
     language: str
     path: str
```

### Comparing `robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi/translation.json` & `robotframework_browser_translation_fi-0.5.1/robotframework_browser_translation_fi/translation.json`

 * *Files identical despite different names*

### Comparing `robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi.egg-info/PKG-INFO` & `robotframework_browser_translation_fi-0.5.1/robotframework_browser_translation_fi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-browser-translation-fi
-Version: 0.5.0
+Version: 0.5.1
 Summary: Robot Framework Browser library translation to Finnish languege
 Author-email: Tatu Aalto <aalto.tatu@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -253,14 +253,25 @@
 library is imported with:
 
 ```robotRobotFramework
 *** Settings ***
 Library    Browser    languege=fi
 ```
 
+## Detect changes in documentation
+The
+[translation.json](https://github.com/MarketSquare/robotframework-browser-translation-fi/blob/main/ robotframework_browser_translation_fi/translation.json)
+contains sha256 sum, which is generated by the Browser library. The sha356
+is the checksum of the original documentation of the Browser library documentation.
+The checksum is used by
+`fbrowser translation --compare robotframework_browser_translation_fi/translation.json`
+command to compare translation between the library and translation file. Command will
+display a list of keywords which needs updating or are missing from the translation.json
+file.
+
 ## Contributors
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
```


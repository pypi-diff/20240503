# Comparing `tmp/ssm_svg-0.0.6.tar.gz` & `tmp/ssm_svg-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm_svg-0.0.6.tar", last modified: Fri May  3 04:01:11 2024, max compression
+gzip compressed data, was "ssm_svg-0.0.7.tar", last modified: Fri May  3 05:36:35 2024, max compression
```

## Comparing `ssm_svg-0.0.6.tar` & `ssm_svg-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:01:11.335826 ssm_svg-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 04:01:00.000000 ssm_svg-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-03 04:01:11.335826 ssm_svg-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-03 04:01:00.000000 ssm_svg-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 04:01:11.335826 ssm_svg-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-03 04:01:00.000000 ssm_svg-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:01:11.331826 ssm_svg-0.0.6/ssm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 04:01:00.000000 ssm_svg-0.0.6/ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 04:01:00.000000 ssm_svg-0.0.6/ssm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-03 04:01:00.000000 ssm_svg-0.0.6/ssm/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16283 2024-05-03 04:01:00.000000 ssm_svg-0.0.6/ssm/ssm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:01:11.331826 ssm_svg-0.0.6/ssm_svg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-03 04:01:11.000000 ssm_svg-0.0.6/ssm_svg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-03 04:01:11.000000 ssm_svg-0.0.6/ssm_svg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 04:01:11.000000 ssm_svg-0.0.6/ssm_svg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 04:01:11.000000 ssm_svg-0.0.6/ssm_svg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 04:01:11.000000 ssm_svg-0.0.6/ssm_svg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-03 04:01:11.000000 ssm_svg-0.0.6/ssm_svg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:01:11.331826 ssm_svg-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7499 2024-05-03 04:01:00.000000 ssm_svg-0.0.6/tests/test_ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:36:35.721920 ssm_svg-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 05:36:24.000000 ssm_svg-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-03 05:36:35.721920 ssm_svg-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-03 05:36:24.000000 ssm_svg-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 05:36:35.721920 ssm_svg-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-03 05:36:24.000000 ssm_svg-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:36:35.717920 ssm_svg-0.0.7/ssm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:36:24.000000 ssm_svg-0.0.7/ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 05:36:24.000000 ssm_svg-0.0.7/ssm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-03 05:36:24.000000 ssm_svg-0.0.7/ssm/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16283 2024-05-03 05:36:24.000000 ssm_svg-0.0.7/ssm/ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:36:35.721920 ssm_svg-0.0.7/ssm_svg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-03 05:36:35.000000 ssm_svg-0.0.7/ssm_svg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-03 05:36:35.000000 ssm_svg-0.0.7/ssm_svg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 05:36:35.000000 ssm_svg-0.0.7/ssm_svg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 05:36:35.000000 ssm_svg-0.0.7/ssm_svg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 05:36:35.000000 ssm_svg-0.0.7/ssm_svg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-03 05:36:35.000000 ssm_svg-0.0.7/ssm_svg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:36:35.721920 ssm_svg-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7499 2024-05-03 05:36:24.000000 ssm_svg-0.0.7/tests/test_ssm.py
```

### Comparing `ssm_svg-0.0.6/LICENSE` & `ssm_svg-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ssm_svg-0.0.6/PKG-INFO` & `ssm_svg-0.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-svg
-Version: 0.0.6
+Version: 0.0.7
 Summary: SVG spritesheet maker
 Home-page: https://github.com/obeezzy/ssm
 Author: Chronic Coder
 Author-email: efeoghene.obebeduo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,145 +14,145 @@
 Requires-Dist: lxml
 
 # ssm
 
 SVG spritesheet maker
 
 [![CI](https://github.com/obeezzy/ssm/actions/workflows/main.yml/badge.svg)](https://github.com/obeezzy/ssm/actions/workflows/main.yml)
-[![Deployment to PyPI](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml/badge.svg?branch=v0.0.6)](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml)
+[![Deployment to PyPI](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml/badge.svg?branch=v0.0.7)](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml)
 
 __ssm__ is a command-line tool for creating and managing SVG spritesheets. It has 5 main functions:
 
 * __create__: For creating spritesheets from a list of SVG sprites (i.e. SVG icons etc.).
 * __list__: For listing the SVG sprites stored in a spritesheet.
 * __add__: For adding SVG sprites to an existing spritesheet.
 * __remove__: For removing SVG sprites from an existing spritesheet.
 * __export__: For exporting SVG sprites from an existing spritesheet; Can be used for converting a `<symbol>` back into a standalone `<svg>` or to display a format suitable for use in HTML (using `<use>`).
 
-For more details, run `python -m ssm -h` after installation.
+For more details, run `ssm -h` after installation.
 
 ## Installation
 
 To install the most stable version of this package, run:
 ```bash
 $ pip install ssm-svg
 ```
 
 ## Usage example
 
 Create spritesheet `icons.svg` with `search.svg` and `menu.svg` as sprites:
 
 ```bash
-$ python -m ssm create -f icons.svg search.svg menu.svg
+$ ssm create -f icons.svg search.svg menu.svg
 $ cat icons.svg
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="menu" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 Create spritesheet and overwrite existing file:
 
 ```bash
-$ python -m ssm create -f icons.svg search.svg menu.svg -F
+$ ssm create -f icons.svg search.svg menu.svg -F
 ```
 
 Create spritesheet containing `search.svg` and `menu.svg`, with custom ID `hamburger-icon` for `menu.svg` (instead of defaulting to its file name):
 
 ```bash
-$ python -m ssm create -f icons.svg search.svg hamburger-icon=menu.svg
+$ ssm create -f icons.svg search.svg hamburger-icon=menu.svg
 $ cat icons.svg
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 List IDs of sprites in spritesheet:
 
 ```bash
-$ python -m ssm list -f icons.svg
+$ ssm list -f icons.svg
 menu
 search
 ```
 
 Add `facebook.svg` and `instagram.svg` to spritesheet:
 
 ```bash
-$ python -m ssm add -f icons.svg facebook.svg instagram.svg
+$ ssm add -f icons.svg facebook.svg instagram.svg
 $ cat icons.svg
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
     <symbol id="facebook" viewBox="0 0 24 24">...</symbol>
     <symbol id="instagram" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 Remove sprites with IDs `facebook` and `instagram` from spritesheet:
 
 ```bash
-$ python -m ssm remove -f icons.svg facebook instagram
+$ ssm remove -f icons.svg facebook instagram
 $ cat icons.svg
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 NOTE: Inserting the same ID more than once would cause an error.
 
 Add `facebook.svg` to spritesheet with custom ID `fb-icon` (instead of defaulting to its file name):
 
 ```bash
-$ python -m ssm add -f icons.svg fb-icon=facebook.svg
+$ ssm add -f icons.svg fb-icon=facebook.svg
 $ cat icons.svg
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
     <symbol id="fb-icon" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 Export sprite with ID `menu` from spritesheet:
 
 ```bash
-$ python -m ssm export -f icons.svg menu
+$ ssm export -f icons.svg menu
 <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
     <!-- "menu" SVG elements -->
 </svg>
 ```
 
 Export sprite with ID `menu` from spritesheet for use in HTML:
 
 ```bash
-$ python -m ssm export -f icons.svg menu --use
+$ ssm export -f icons.svg menu --use
 <svg><use href="icons.svg#menu"></use></svg>
 ```
 
 Export sprites with IDs `search` and `menu` from spritesheet as `exported_files/search.svg` and `exported_files/menu.svg` respectively:
 
 ```bash
-$ python -m ssm export -f icons.svg --dir exported_files search menu
-$ cat exported_files/menu.svg
-<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
-    <!-- "menu" SVG elements -->
-</svg>
+$ ssm export -f icons.svg --dir exported_files search menu
 $ cat exported_files/search.svg
 <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
     <!-- "search" SVG elements -->
 </svg>
+$ cat exported_files/menu.svg
+<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
+    <!-- "menu" SVG elements -->
+</svg>
 ```
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `ssm_svg-0.0.6/README.md` & `ssm_svg-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,143 +1,143 @@
 # ssm
 
 SVG spritesheet maker
 
 [![CI](https://github.com/obeezzy/ssm/actions/workflows/main.yml/badge.svg)](https://github.com/obeezzy/ssm/actions/workflows/main.yml)
-[![Deployment to PyPI](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml/badge.svg?branch=v0.0.6)](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml)
+[![Deployment to PyPI](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml/badge.svg?branch=v0.0.7)](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml)
 
 __ssm__ is a command-line tool for creating and managing SVG spritesheets. It has 5 main functions:
 
 * __create__: For creating spritesheets from a list of SVG sprites (i.e. SVG icons etc.).
 * __list__: For listing the SVG sprites stored in a spritesheet.
 * __add__: For adding SVG sprites to an existing spritesheet.
 * __remove__: For removing SVG sprites from an existing spritesheet.
 * __export__: For exporting SVG sprites from an existing spritesheet; Can be used for converting a `<symbol>` back into a standalone `<svg>` or to display a format suitable for use in HTML (using `<use>`).
 
-For more details, run `python -m ssm -h` after installation.
+For more details, run `ssm -h` after installation.
 
 ## Installation
 
 To install the most stable version of this package, run:
 ```bash
 $ pip install ssm-svg
 ```
 
 ## Usage example
 
 Create spritesheet `icons.svg` with `search.svg` and `menu.svg` as sprites:
 
 ```bash
-$ python -m ssm create -f icons.svg search.svg menu.svg
+$ ssm create -f icons.svg search.svg menu.svg
 $ cat icons.svg
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="menu" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 Create spritesheet and overwrite existing file:
 
 ```bash
-$ python -m ssm create -f icons.svg search.svg menu.svg -F
+$ ssm create -f icons.svg search.svg menu.svg -F
 ```
 
 Create spritesheet containing `search.svg` and `menu.svg`, with custom ID `hamburger-icon` for `menu.svg` (instead of defaulting to its file name):
 
 ```bash
-$ python -m ssm create -f icons.svg search.svg hamburger-icon=menu.svg
+$ ssm create -f icons.svg search.svg hamburger-icon=menu.svg
 $ cat icons.svg
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 List IDs of sprites in spritesheet:
 
 ```bash
-$ python -m ssm list -f icons.svg
+$ ssm list -f icons.svg
 menu
 search
 ```
 
 Add `facebook.svg` and `instagram.svg` to spritesheet:
 
 ```bash
-$ python -m ssm add -f icons.svg facebook.svg instagram.svg
+$ ssm add -f icons.svg facebook.svg instagram.svg
 $ cat icons.svg
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
     <symbol id="facebook" viewBox="0 0 24 24">...</symbol>
     <symbol id="instagram" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 Remove sprites with IDs `facebook` and `instagram` from spritesheet:
 
 ```bash
-$ python -m ssm remove -f icons.svg facebook instagram
+$ ssm remove -f icons.svg facebook instagram
 $ cat icons.svg
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 NOTE: Inserting the same ID more than once would cause an error.
 
 Add `facebook.svg` to spritesheet with custom ID `fb-icon` (instead of defaulting to its file name):
 
 ```bash
-$ python -m ssm add -f icons.svg fb-icon=facebook.svg
+$ ssm add -f icons.svg fb-icon=facebook.svg
 $ cat icons.svg
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
     <symbol id="fb-icon" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 Export sprite with ID `menu` from spritesheet:
 
 ```bash
-$ python -m ssm export -f icons.svg menu
+$ ssm export -f icons.svg menu
 <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
     <!-- "menu" SVG elements -->
 </svg>
 ```
 
 Export sprite with ID `menu` from spritesheet for use in HTML:
 
 ```bash
-$ python -m ssm export -f icons.svg menu --use
+$ ssm export -f icons.svg menu --use
 <svg><use href="icons.svg#menu"></use></svg>
 ```
 
 Export sprites with IDs `search` and `menu` from spritesheet as `exported_files/search.svg` and `exported_files/menu.svg` respectively:
 
 ```bash
-$ python -m ssm export -f icons.svg --dir exported_files search menu
-$ cat exported_files/menu.svg
-<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
-    <!-- "menu" SVG elements -->
-</svg>
+$ ssm export -f icons.svg --dir exported_files search menu
 $ cat exported_files/search.svg
 <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
     <!-- "search" SVG elements -->
 </svg>
+$ cat exported_files/menu.svg
+<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
+    <!-- "menu" SVG elements -->
+</svg>
 ```
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `ssm_svg-0.0.6/setup.py` & `ssm_svg-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (ROOT_DIR / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="ssm-svg",
-    version="0.0.6",
+    version="0.0.7",
     description="SVG spritesheet maker",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/obeezzy/ssm",
     author="Chronic Coder",
     author_email="efeoghene.obebeduo@gmail.com",
     license="MIT",
```

### Comparing `ssm_svg-0.0.6/ssm/ssm.py` & `ssm_svg-0.0.7/ssm/ssm.py`

 * *Files identical despite different names*

### Comparing `ssm_svg-0.0.6/ssm_svg.egg-info/PKG-INFO` & `ssm_svg-0.0.7/ssm_svg.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-svg
-Version: 0.0.6
+Version: 0.0.7
 Summary: SVG spritesheet maker
 Home-page: https://github.com/obeezzy/ssm
 Author: Chronic Coder
 Author-email: efeoghene.obebeduo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,145 +14,145 @@
 Requires-Dist: lxml
 
 # ssm
 
 SVG spritesheet maker
 
 [![CI](https://github.com/obeezzy/ssm/actions/workflows/main.yml/badge.svg)](https://github.com/obeezzy/ssm/actions/workflows/main.yml)
-[![Deployment to PyPI](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml/badge.svg?branch=v0.0.6)](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml)
+[![Deployment to PyPI](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml/badge.svg?branch=v0.0.7)](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml)
 
 __ssm__ is a command-line tool for creating and managing SVG spritesheets. It has 5 main functions:
 
 * __create__: For creating spritesheets from a list of SVG sprites (i.e. SVG icons etc.).
 * __list__: For listing the SVG sprites stored in a spritesheet.
 * __add__: For adding SVG sprites to an existing spritesheet.
 * __remove__: For removing SVG sprites from an existing spritesheet.
 * __export__: For exporting SVG sprites from an existing spritesheet; Can be used for converting a `<symbol>` back into a standalone `<svg>` or to display a format suitable for use in HTML (using `<use>`).
 
-For more details, run `python -m ssm -h` after installation.
+For more details, run `ssm -h` after installation.
 
 ## Installation
 
 To install the most stable version of this package, run:
 ```bash
 $ pip install ssm-svg
 ```
 
 ## Usage example
 
 Create spritesheet `icons.svg` with `search.svg` and `menu.svg` as sprites:
 
 ```bash
-$ python -m ssm create -f icons.svg search.svg menu.svg
+$ ssm create -f icons.svg search.svg menu.svg
 $ cat icons.svg
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="menu" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 Create spritesheet and overwrite existing file:
 
 ```bash
-$ python -m ssm create -f icons.svg search.svg menu.svg -F
+$ ssm create -f icons.svg search.svg menu.svg -F
 ```
 
 Create spritesheet containing `search.svg` and `menu.svg`, with custom ID `hamburger-icon` for `menu.svg` (instead of defaulting to its file name):
 
 ```bash
-$ python -m ssm create -f icons.svg search.svg hamburger-icon=menu.svg
+$ ssm create -f icons.svg search.svg hamburger-icon=menu.svg
 $ cat icons.svg
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 List IDs of sprites in spritesheet:
 
 ```bash
-$ python -m ssm list -f icons.svg
+$ ssm list -f icons.svg
 menu
 search
 ```
 
 Add `facebook.svg` and `instagram.svg` to spritesheet:
 
 ```bash
-$ python -m ssm add -f icons.svg facebook.svg instagram.svg
+$ ssm add -f icons.svg facebook.svg instagram.svg
 $ cat icons.svg
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
     <symbol id="facebook" viewBox="0 0 24 24">...</symbol>
     <symbol id="instagram" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 Remove sprites with IDs `facebook` and `instagram` from spritesheet:
 
 ```bash
-$ python -m ssm remove -f icons.svg facebook instagram
+$ ssm remove -f icons.svg facebook instagram
 $ cat icons.svg
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 NOTE: Inserting the same ID more than once would cause an error.
 
 Add `facebook.svg` to spritesheet with custom ID `fb-icon` (instead of defaulting to its file name):
 
 ```bash
-$ python -m ssm add -f icons.svg fb-icon=facebook.svg
+$ ssm add -f icons.svg fb-icon=facebook.svg
 $ cat icons.svg
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
     <symbol id="fb-icon" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 Export sprite with ID `menu` from spritesheet:
 
 ```bash
-$ python -m ssm export -f icons.svg menu
+$ ssm export -f icons.svg menu
 <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
     <!-- "menu" SVG elements -->
 </svg>
 ```
 
 Export sprite with ID `menu` from spritesheet for use in HTML:
 
 ```bash
-$ python -m ssm export -f icons.svg menu --use
+$ ssm export -f icons.svg menu --use
 <svg><use href="icons.svg#menu"></use></svg>
 ```
 
 Export sprites with IDs `search` and `menu` from spritesheet as `exported_files/search.svg` and `exported_files/menu.svg` respectively:
 
 ```bash
-$ python -m ssm export -f icons.svg --dir exported_files search menu
-$ cat exported_files/menu.svg
-<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
-    <!-- "menu" SVG elements -->
-</svg>
+$ ssm export -f icons.svg --dir exported_files search menu
 $ cat exported_files/search.svg
 <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
     <!-- "search" SVG elements -->
 </svg>
+$ cat exported_files/menu.svg
+<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
+    <!-- "menu" SVG elements -->
+</svg>
 ```
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `ssm_svg-0.0.6/tests/test_ssm.py` & `ssm_svg-0.0.7/tests/test_ssm.py`

 * *Files identical despite different names*


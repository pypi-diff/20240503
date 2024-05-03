# Comparing `tmp/ssm_svg-0.0.5.tar.gz` & `tmp/ssm_svg-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm_svg-0.0.5.tar", last modified: Thu May  2 20:29:41 2024, max compression
+gzip compressed data, was "ssm_svg-0.0.6.tar", last modified: Fri May  3 04:01:11 2024, max compression
```

## Comparing `ssm_svg-0.0.5.tar` & `ssm_svg-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:29:41.543870 ssm_svg-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-02 20:29:33.000000 ssm_svg-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-02 20:29:41.543870 ssm_svg-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-02 20:29:33.000000 ssm_svg-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 20:29:41.543870 ssm_svg-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-02 20:29:33.000000 ssm_svg-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:29:41.543870 ssm_svg-0.0.5/ssm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:29:33.000000 ssm_svg-0.0.5/ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 20:29:33.000000 ssm_svg-0.0.5/ssm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 20:29:33.000000 ssm_svg-0.0.5/ssm/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16473 2024-05-02 20:29:33.000000 ssm_svg-0.0.5/ssm/ssm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:29:41.543870 ssm_svg-0.0.5/ssm_svg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-02 20:29:41.000000 ssm_svg-0.0.5/ssm_svg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-02 20:29:41.000000 ssm_svg-0.0.5/ssm_svg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:29:41.000000 ssm_svg-0.0.5/ssm_svg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 20:29:41.000000 ssm_svg-0.0.5/ssm_svg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 20:29:41.000000 ssm_svg-0.0.5/ssm_svg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 20:29:41.000000 ssm_svg-0.0.5/ssm_svg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:29:41.543870 ssm_svg-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7499 2024-05-02 20:29:33.000000 ssm_svg-0.0.5/tests/test_ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:01:11.335826 ssm_svg-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 04:01:00.000000 ssm_svg-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-03 04:01:11.335826 ssm_svg-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-03 04:01:00.000000 ssm_svg-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 04:01:11.335826 ssm_svg-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-03 04:01:00.000000 ssm_svg-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:01:11.331826 ssm_svg-0.0.6/ssm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 04:01:00.000000 ssm_svg-0.0.6/ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 04:01:00.000000 ssm_svg-0.0.6/ssm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-03 04:01:00.000000 ssm_svg-0.0.6/ssm/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16283 2024-05-03 04:01:00.000000 ssm_svg-0.0.6/ssm/ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:01:11.331826 ssm_svg-0.0.6/ssm_svg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-03 04:01:11.000000 ssm_svg-0.0.6/ssm_svg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-03 04:01:11.000000 ssm_svg-0.0.6/ssm_svg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 04:01:11.000000 ssm_svg-0.0.6/ssm_svg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 04:01:11.000000 ssm_svg-0.0.6/ssm_svg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 04:01:11.000000 ssm_svg-0.0.6/ssm_svg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-03 04:01:11.000000 ssm_svg-0.0.6/ssm_svg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:01:11.331826 ssm_svg-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7499 2024-05-03 04:01:00.000000 ssm_svg-0.0.6/tests/test_ssm.py
```

### Comparing `ssm_svg-0.0.5/LICENSE` & `ssm_svg-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ssm_svg-0.0.5/PKG-INFO` & `ssm_svg-0.0.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,159 +1,143 @@
-Metadata-Version: 2.1
-Name: ssm-svg
-Version: 0.0.5
-Summary: SVG spritesheet maker
-Home-page: https://github.com/obeezzy/ssm
-Author: Chronic Coder
-Author-email: efeoghene.obebeduo@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: lxml
-
 # ssm
 
 SVG spritesheet maker
 
 [![CI](https://github.com/obeezzy/ssm/actions/workflows/main.yml/badge.svg)](https://github.com/obeezzy/ssm/actions/workflows/main.yml)
-[![Deployment to PyPI](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml/badge.svg?branch=v0.0.5)](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml)
+[![Deployment to PyPI](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml/badge.svg?branch=v0.0.6)](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml)
 
-__ssm__ is a simple approach to creating and managing SVG spritesheets. It has 5 main functions:
+__ssm__ is a command-line tool for creating and managing SVG spritesheets. It has 5 main functions:
 
-* __create__: For creating spritesheets from a list of SVG sprites (i.e. SVG icons etc.)
-* __list__: For listing the SVG sprites stored in a spritesheet
-* __add__: For adding SVG sprites to an existing spritesheet
-* __remove__: For removing SVG sprites from an existing spritesheet
-* __export__: For exporting SVG sprites from an existing spritesheet. Can be used for converting a `<symbol>` back into a standalone `<svg>` or to display a format suitable for HTML (using `<use>`).
+* __create__: For creating spritesheets from a list of SVG sprites (i.e. SVG icons etc.).
+* __list__: For listing the SVG sprites stored in a spritesheet.
+* __add__: For adding SVG sprites to an existing spritesheet.
+* __remove__: For removing SVG sprites from an existing spritesheet.
+* __export__: For exporting SVG sprites from an existing spritesheet; Can be used for converting a `<symbol>` back into a standalone `<svg>` or to display a format suitable for use in HTML (using `<use>`).
 
 For more details, run `python -m ssm -h` after installation.
 
 ## Installation
+
 To install the most stable version of this package, run:
 ```bash
 $ pip install ssm-svg
 ```
 
 ## Usage example
 
 Create spritesheet `icons.svg` with `search.svg` and `menu.svg` as sprites:
 
 ```bash
 $ python -m ssm create -f icons.svg search.svg menu.svg
 $ cat icons.svg
-<?xml version='1.0' encoding='UTF-8'?>
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
-    <symbol id="menu" viewBox="0 0 24 24">...</symbol>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
+    <symbol id="menu" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 Create spritesheet and overwrite existing file:
 
 ```bash
 $ python -m ssm create -f icons.svg search.svg menu.svg -F
 ```
 
-Create spritesheet with custom ID `hamburger-icon` instead of defaulting to its file name:
+Create spritesheet containing `search.svg` and `menu.svg`, with custom ID `hamburger-icon` for `menu.svg` (instead of defaulting to its file name):
 
 ```bash
 $ python -m ssm create -f icons.svg search.svg hamburger-icon=menu.svg
 $ cat icons.svg
-<?xml version='1.0' encoding='UTF-8'?>
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
-    <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
+    <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
-List IDs of SVG sprites in spritesheet:
+List IDs of sprites in spritesheet:
 
 ```bash
 $ python -m ssm list -f icons.svg
 menu
 search
 ```
 
-Add SVG sprites to spritesheet:
+Add `facebook.svg` and `instagram.svg` to spritesheet:
 
 ```bash
 $ python -m ssm add -f icons.svg facebook.svg instagram.svg
 $ cat icons.svg
-<?xml version='1.0' encoding='UTF-8'?>
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
-    <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
+    <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
     <symbol id="facebook" viewBox="0 0 24 24">...</symbol>
     <symbol id="instagram" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
-Remove SVG sprites with IDs `facebook` and `instagram` from spritesheet:
+Remove sprites with IDs `facebook` and `instagram` from spritesheet:
 
 ```bash
 $ python -m ssm remove -f icons.svg facebook instagram
 $ cat icons.svg
-<?xml version='1.0' encoding='UTF-8'?>
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
-    <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
+    <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 NOTE: Inserting the same ID more than once would cause an error.
 
-Add SVG sprites to spritesheet with custom ID `fb-icon` instead of defaulting to its file name:
+Add `facebook.svg` to spritesheet with custom ID `fb-icon` (instead of defaulting to its file name):
 
 ```bash
 $ python -m ssm add -f icons.svg fb-icon=facebook.svg
 $ cat icons.svg
-<?xml version='1.0' encoding='UTF-8'?>
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
-    <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
+    <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
     <symbol id="fb-icon" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 Export sprite with ID `menu` from spritesheet:
 
 ```bash
 $ python -m ssm export -f icons.svg menu
-<?xml version='1.0' encoding='utf-8'?>
-<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">...</svg>
+<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
+    <!-- "menu" SVG elements -->
+</svg>
 ```
 
 Export sprite with ID `menu` from spritesheet for use in HTML:
 
 ```bash
 $ python -m ssm export -f icons.svg menu --use
 <svg><use href="icons.svg#menu"></use></svg>
 ```
 
-Export sprite with IDs `search` and `menu` from spritesheet as `exported_files/search.svg` and `exported_files/menu.svg` respectively:
+Export sprites with IDs `search` and `menu` from spritesheet as `exported_files/search.svg` and `exported_files/menu.svg` respectively:
 
 ```bash
 $ python -m ssm export -f icons.svg --dir exported_files search menu
 $ cat exported_files/menu.svg
-<?xml version='1.0' encoding='utf-8'?>
-<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">...</svg>
+<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
+    <!-- "menu" SVG elements -->
+</svg>
 $ cat exported_files/search.svg
-<?xml version='1.0' encoding='utf-8'?>
-<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">...</svg>
+<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
+    <!-- "search" SVG elements -->
+</svg>
 ```
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `ssm_svg-0.0.5/setup.py` & `ssm_svg-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (ROOT_DIR / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="ssm-svg",
-    version="0.0.5",
+    version="0.0.6",
     description="SVG spritesheet maker",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/obeezzy/ssm",
     author="Chronic Coder",
     author_email="efeoghene.obebeduo@gmail.com",
     license="MIT",
```

### Comparing `ssm_svg-0.0.5/ssm/ssm.py` & `ssm_svg-0.0.6/ssm/ssm.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,17 +85,15 @@
         else:
             attrib = SVG_XMLNS
             attrib["viewBox"] = self._view_box
             svg = E("svg", attrib)
             for child in self._child_nodes:
                 svg.append(child)
         return etree.tostring(svg,
-                              pretty_print=True,
-                              xml_declaration=True,
-                              encoding="utf-8").decode()
+                              pretty_print=True).decode()
 
     @property
     def id(self) -> str:
         """ID.
         """
         return self._id
 
@@ -194,17 +192,15 @@
             s.getparent().remove(s)
 
     def update(self) -> None:
         """Saves changes to the spritesheet to a file.
         """
         self._tree = etree.ElementTree(self._root)
         self._tree.write(self._filename,
-                         pretty_print=True,
-                         encoding="utf-8",
-                         xml_declaration=True)
+                         pretty_print=True)
 
     @property
     def filename(self) -> str:
         """File name.
         """
         return self._filename
```

### Comparing `ssm_svg-0.0.5/tests/test_ssm.py` & `ssm_svg-0.0.6/tests/test_ssm.py`

 * *Files identical despite different names*


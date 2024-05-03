# Comparing `tmp/openpyxl_style_writer-1.1.2.tar.gz` & `tmp/openpyxl_style_writer-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpyxl_style_writer-1.1.2.tar", last modified: Thu Feb 29 08:37:30 2024, max compression
+gzip compressed data, was "openpyxl_style_writer-1.1.3.tar", last modified: Fri May  3 17:13:10 2024, max compression
```

## Comparing `openpyxl_style_writer-1.1.2.tar` & `openpyxl_style_writer-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:37:30.222741 openpyxl_style_writer-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-29 08:37:17.000000 openpyxl_style_writer-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9954 2024-02-29 08:37:30.222741 openpyxl_style_writer-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-02-29 08:37:17.000000 openpyxl_style_writer-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:37:30.218740 openpyxl_style_writer-1.1.2/openpyxl_style_writer/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-29 08:37:17.000000 openpyxl_style_writer-1.1.2/openpyxl_style_writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-02-29 08:37:17.000000 openpyxl_style_writer-1.1.2/openpyxl_style_writer/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-02-29 08:37:17.000000 openpyxl_style_writer-1.1.2/openpyxl_style_writer/wirter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:37:30.222741 openpyxl_style_writer-1.1.2/openpyxl_style_writer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9954 2024-02-29 08:37:30.000000 openpyxl_style_writer-1.1.2/openpyxl_style_writer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-02-29 08:37:30.000000 openpyxl_style_writer-1.1.2/openpyxl_style_writer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 08:37:30.000000 openpyxl_style_writer-1.1.2/openpyxl_style_writer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-29 08:37:30.000000 openpyxl_style_writer-1.1.2/openpyxl_style_writer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-29 08:37:30.000000 openpyxl_style_writer-1.1.2/openpyxl_style_writer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 08:37:30.222741 openpyxl_style_writer-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-02-29 08:37:17.000000 openpyxl_style_writer-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:13:10.660919 openpyxl_style_writer-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 17:13:06.000000 openpyxl_style_writer-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9954 2024-05-03 17:13:10.660919 openpyxl_style_writer-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-05-03 17:13:06.000000 openpyxl_style_writer-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:13:10.660919 openpyxl_style_writer-1.1.3/openpyxl_style_writer/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-03 17:13:06.000000 openpyxl_style_writer-1.1.3/openpyxl_style_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-05-03 17:13:06.000000 openpyxl_style_writer-1.1.3/openpyxl_style_writer/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-03 17:13:06.000000 openpyxl_style_writer-1.1.3/openpyxl_style_writer/wirter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:13:10.660919 openpyxl_style_writer-1.1.3/openpyxl_style_writer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9954 2024-05-03 17:13:10.000000 openpyxl_style_writer-1.1.3/openpyxl_style_writer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-03 17:13:10.000000 openpyxl_style_writer-1.1.3/openpyxl_style_writer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:13:10.000000 openpyxl_style_writer-1.1.3/openpyxl_style_writer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 17:13:10.000000 openpyxl_style_writer-1.1.3/openpyxl_style_writer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 17:13:10.000000 openpyxl_style_writer-1.1.3/openpyxl_style_writer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:13:10.660919 openpyxl_style_writer-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-03 17:13:06.000000 openpyxl_style_writer-1.1.3/setup.py
```

### Comparing `openpyxl_style_writer-1.1.2/LICENSE` & `openpyxl_style_writer-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openpyxl_style_writer-1.1.2/PKG-INFO` & `openpyxl_style_writer-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpyxl_style_writer
-Version: 1.1.2
+Version: 1.1.3
 Summary: A wrapper for openpyxl to create and use resualbe style in write only mode
 Home-page: https://github.com/Zncl2222/openpyxl_style_writer
 Author: Zncl2222
 Author-email: zwebapplication@gmail.com
 License: MIT
 Keywords: openpyxl,excel,style
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openpyxl_style_writer-1.1.2/README.md` & `openpyxl_style_writer-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `openpyxl_style_writer-1.1.2/openpyxl_style_writer/style.py` & `openpyxl_style_writer-1.1.3/openpyxl_style_writer/style.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,44 +5,44 @@
     # params
     font_params = None
     fill_params = None
     ali_params = None
     border_params = None
 
     # font
-    font_size = 14
+    font_size = 11
     font_name = 'Calibri'
     font_bold = False
     font_italic = False
     font_underline = 'none'
     font_strike = False
     font_vertAlign = None
     font_color = '000000'
 
     # fill
     fill_pattern = 'solid'
-    fill_color = 'fcfcfc'
+    fill_color = 'ffffff'
 
     # alignment
-    ali_horizontal = 'center'
-    ali_vertical = 'center'
+    ali_horizontal = None
+    ali_vertical = 'bottom'
     ali_text_rotation = 0
     ali_wrap_text = False
     ali_shrink_to_fit = False
     ali_indent = 0
 
     # border
-    border_style_top = None
-    border_style_right = None
-    border_style_left = None
-    border_style_bottom = None
-    border_color_top = 'ff000000'
-    border_color_right = 'ff000000'
-    border_color_left = 'ff000000'
-    border_color_bottom = 'ff000000'
+    border_style_top = 'thin'
+    border_style_right = 'thin'
+    border_style_left = 'thin'
+    border_style_bottom = 'thin'
+    border_color_top = 'C0C0C0'
+    border_color_right = 'C0C0C0'
+    border_color_left = 'C0C0C0'
+    border_color_bottom = 'C0C0C0'
 
     # protect
     protect = False
     protection = Protection(locked=False)
 
     # format
     number_format = 'General'
```

### Comparing `openpyxl_style_writer-1.1.2/openpyxl_style_writer/wirter.py` & `openpyxl_style_writer-1.1.3/openpyxl_style_writer/wirter.py`

 * *Files identical despite different names*

### Comparing `openpyxl_style_writer-1.1.2/openpyxl_style_writer.egg-info/PKG-INFO` & `openpyxl_style_writer-1.1.3/openpyxl_style_writer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpyxl_style_writer
-Version: 1.1.2
+Version: 1.1.3
 Summary: A wrapper for openpyxl to create and use resualbe style in write only mode
 Home-page: https://github.com/Zncl2222/openpyxl_style_writer
 Author: Zncl2222
 Author-email: zwebapplication@gmail.com
 License: MIT
 Keywords: openpyxl,excel,style
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openpyxl_style_writer-1.1.2/setup.py` & `openpyxl_style_writer-1.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 url = 'https://github.com/Zncl2222/openpyxl_style_writer'
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='openpyxl_style_writer',
-    version='1.1.2',
+    version='1.1.3',
     description='A wrapper for openpyxl to create and use resualbe style in write only mode',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url=url,
     author=author,
     author_email=email,
     license='MIT',
```


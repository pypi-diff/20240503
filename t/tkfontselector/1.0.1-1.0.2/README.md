# Comparing `tmp/tkfontselector-1.0.1.tar.gz` & `tmp/tkfontselector-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkfontselector-1.0.1.tar", max compression
+gzip compressed data, was "tkfontselector-1.0.2.tar", max compression
```

## Comparing `tkfontselector-1.0.1.tar` & `tkfontselector-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1095 2024-05-03 18:38:10.067204 tkfontselector-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0      380 2024-05-03 21:09:08.317421 tkfontselector-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2915 2024-05-03 20:48:08.645315 tkfontselector-1.0.1/README.md
--rw-r--r--   0        0        0       72 2024-05-03 19:02:54.386237 tkfontselector-1.0.1/tkfontselector/__init__.py
--rw-r--r--   0        0        0       22 2024-05-03 21:06:43.204801 tkfontselector-1.0.1/tkfontselector/_version.py
--rw-r--r--   0        0        0     1404 2024-05-03 21:10:32.587835 tkfontselector-1.0.1/tkfontselector/ask_font.py
--rw-r--r--   0        0        0    18418 2024-05-03 21:10:32.589837 tkfontselector-1.0.1/tkfontselector/tkfontselector.py
--rw-r--r--   0        0        0      861 2024-05-03 20:31:18.551933 tkfontselector-1.0.1/tkfontselector/translations/__init__.py
--rw-r--r--   0        0        0     3334 1970-01-01 00:00:00.000000 tkfontselector-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-05-03 18:38:10.067204 tkfontselector-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      979 2024-05-03 21:47:43.240510 tkfontselector-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2913 2024-05-03 21:12:12.176906 tkfontselector-1.0.2/README.md
+-rw-r--r--   0        0        0       72 2024-05-03 19:02:54.386237 tkfontselector-1.0.2/tkfontselector/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-03 21:12:57.402449 tkfontselector-1.0.2/tkfontselector/_version.py
+-rw-r--r--   0        0        0     1404 2024-05-03 21:10:32.587835 tkfontselector-1.0.2/tkfontselector/ask_font.py
+-rw-r--r--   0        0        0    18418 2024-05-03 21:13:43.402212 tkfontselector-1.0.2/tkfontselector/tkfontselector.py
+-rw-r--r--   0        0        0      861 2024-05-03 20:31:18.551933 tkfontselector-1.0.2/tkfontselector/translations/__init__.py
+-rw-r--r--   0        0        0     3816 1970-01-01 00:00:00.000000 tkfontselector-1.0.2/PKG-INFO
```

### Comparing `tkfontselector-1.0.1/LICENSE.txt` & `tkfontselector-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.1/README.md` & `tkfontselector-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ## Installation
 
 `pip install tkFontSelector`
 
 ## Documentation
 
 ```python
-from tk_font_selector import ask_font
+from tkfontselector import ask_font
 
 ask_font(master=None, text="Abcd", title="Font Chooser", **font_args)
 ```
 
 Open the font chooser and return a dictionary of the font properties. This
 dictionary is similar to the one returned by the `actual` method of a tkinter
 `Font` object.
```

### Comparing `tkfontselector-1.0.1/tkfontselector/ask_font.py` & `tkfontselector-1.0.2/tkfontselector/ask_font.py`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.1/tkfontselector/tkfontselector.py` & `tkfontselector-1.0.2/tkfontselector/tkfontselector.py`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.1/tkfontselector/translations/__init__.py` & `tkfontselector-1.0.2/tkfontselector/translations/__init__.py`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.1/PKG-INFO` & `tkfontselector-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 Metadata-Version: 2.1
 Name: tkfontselector
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tkinter Font Selector
 License: MIT
 Author: jlw4049
 Author-email: jlw_4049@hotmail.com
 Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Natural Language :: French
+Classifier: Natural Language :: Italian
+Classifier: Natural Language :: Russian
+Classifier: Natural Language :: Spanish
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: OS Independent
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
@@ -34,15 +45,15 @@
 ## Installation
 
 `pip install tkFontSelector`
 
 ## Documentation
 
 ```python
-from tk_font_selector import ask_font
+from tkfontselector import ask_font
 
 ask_font(master=None, text="Abcd", title="Font Chooser", **font_args)
 ```
 
 Open the font chooser and return a dictionary of the font properties. This
 dictionary is similar to the one returned by the `actual` method of a tkinter
 `Font` object.
```


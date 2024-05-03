# Comparing `tmp/tkFontSelector-1.0.0.tar.gz` & `tmp/tkfontselector-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkFontSelector-1.0.0.tar", last modified: Fri May  3 20:56:21 2024, max compression
+gzip compressed data, was "tkfontselector-1.0.1.tar", max compression
```

## Comparing `tkFontSelector-1.0.0.tar` & `tkfontselector-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,9 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 20:56:21.373110 tkFontSelector-1.0.0/
--rw-rw-rw-   0        0        0     1095 2024-05-03 18:38:10.000000 tkFontSelector-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3866 2024-05-03 20:56:21.373110 tkFontSelector-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2915 2024-05-03 20:48:08.000000 tkFontSelector-1.0.0/README.md
--rw-rw-rw-   0        0        0      378 2024-05-03 19:52:30.000000 tkFontSelector-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 20:56:21.373110 tkFontSelector-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1186 2024-05-03 20:31:06.000000 tkFontSelector-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 20:56:21.370112 tkFontSelector-1.0.0/tkFontSelector.egg-info/
--rw-rw-rw-   0        0        0     3866 2024-05-03 20:56:21.000000 tkFontSelector-1.0.0/tkFontSelector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2024-05-03 20:56:21.000000 tkFontSelector-1.0.0/tkFontSelector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 20:56:21.000000 tkFontSelector-1.0.0/tkFontSelector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-03 20:56:21.000000 tkFontSelector-1.0.0/tkFontSelector.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-03 20:56:21.372110 tkFontSelector-1.0.0/tk_font_selector/
--rw-rw-rw-   0        0        0       72 2024-05-03 19:02:54.000000 tkFontSelector-1.0.0/tk_font_selector/__init__.py
--rw-rw-rw-   0        0        0       22 2024-05-03 18:36:58.000000 tkFontSelector-1.0.0/tk_font_selector/_version.py
--rw-rw-rw-   0        0        0     1406 2024-05-03 19:08:23.000000 tkFontSelector-1.0.0/tk_font_selector/ask_font.py
--rw-rw-rw-   0        0        0    18420 2024-05-03 20:31:41.000000 tkFontSelector-1.0.0/tk_font_selector/tkfontselector.py
+-rw-r--r--   0        0        0     1095 2024-05-03 18:38:10.067204 tkfontselector-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0      380 2024-05-03 21:09:08.317421 tkfontselector-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2915 2024-05-03 20:48:08.645315 tkfontselector-1.0.1/README.md
+-rw-r--r--   0        0        0       72 2024-05-03 19:02:54.386237 tkfontselector-1.0.1/tkfontselector/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-03 21:06:43.204801 tkfontselector-1.0.1/tkfontselector/_version.py
+-rw-r--r--   0        0        0     1404 2024-05-03 21:10:32.587835 tkfontselector-1.0.1/tkfontselector/ask_font.py
+-rw-r--r--   0        0        0    18418 2024-05-03 21:10:32.589837 tkfontselector-1.0.1/tkfontselector/tkfontselector.py
+-rw-r--r--   0        0        0      861 2024-05-03 20:31:18.551933 tkfontselector-1.0.1/tkfontselector/translations/__init__.py
+-rw-r--r--   0        0        0     3334 1970-01-01 00:00:00.000000 tkfontselector-1.0.1/PKG-INFO
```

### Comparing `tkFontSelector-1.0.0/LICENSE.txt` & `tkfontselector-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkFontSelector-1.0.0/README.md` & `tkfontselector-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tkFontSelector-1.0.0/tk_font_selector/ask_font.py` & `tkfontselector-1.0.1/tkfontselector/ask_font.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tk_font_selector.tkfontselector import FontSelector
+from tkfontselector.tkfontselector import FontSelector
 
 
 def ask_font(
     master=None,
     text="Abcd",
     title="Font Selector",
     fixed_only: bool = False,
```

### Comparing `tkFontSelector-1.0.0/tk_font_selector/tkfontselector.py` & `tkfontselector-1.0.1/tkfontselector/tkfontselector.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from tkinter import Tk, Toplevel, Listbox, StringVar, BooleanVar, TclError
 from tkinter.ttk import Checkbutton, Frame, Label, Button, Scrollbar, Style, Entry
 from tkinter.font import families, Font
 from locale import getlocale
 from typing import Union, List
 
-from tk_font_selector.translations import LANGUAGES
+from tkfontselector.translations import LANGUAGES
 
 try:
     lang_code = getlocale()[0][:2]
     if lang_code in LANGUAGES:
         TR = LANGUAGES[lang_code]
     else:
         TR = LANGUAGES["en"]
```


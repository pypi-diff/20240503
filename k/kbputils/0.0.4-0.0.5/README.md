# Comparing `tmp/kbputils-0.0.4.tar.gz` & `tmp/kbputils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbputils-0.0.4.tar", last modified: Sun Apr 21 21:27:55 2024, max compression
+gzip compressed data, was "kbputils-0.0.5.tar", last modified: Fri May  3 18:35:39 2024, max compression
```

## Comparing `kbputils-0.0.4.tar` & `kbputils-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-21 21:27:55.166743 kbputils-0.0.4/
--rw-r--r--   0 matt      (1000) matt      (1000)     1305 2024-04-16 18:40:43.000000 kbputils-0.0.4/LICENSE
--rw-r--r--   0 matt      (1000) matt      (1000)     2199 2024-04-21 21:27:55.166743 kbputils-0.0.4/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)     1844 2024-04-16 19:00:17.000000 kbputils-0.0.4/README.md
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-21 21:27:55.166743 kbputils-0.0.4/kbputils/
--rw-r--r--   0 matt      (1000) matt      (1000)      132 2024-04-16 18:40:43.000000 kbputils-0.0.4/kbputils/__init__.py
--rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-04-16 18:40:43.000000 kbputils-0.0.4/kbputils/__main__.py
--rw-r--r--   0 matt      (1000) matt      (1000)     2051 2024-04-16 18:40:43.000000 kbputils-0.0.4/kbputils/cli.py
--rw-r--r--   0 matt      (1000) matt      (1000)    12411 2024-04-21 21:21:36.000000 kbputils-0.0.4/kbputils/converters.py
--rw-r--r--   0 matt      (1000) matt      (1000)    18086 2024-04-16 18:40:43.000000 kbputils-0.0.4/kbputils/kbp.py
--rw-r--r--   0 matt      (1000) matt      (1000)      773 2024-04-16 18:40:43.000000 kbputils-0.0.4/kbputils/kbs.py
--rw-r--r--   0 matt      (1000) matt      (1000)     6745 2024-04-16 18:40:43.000000 kbputils-0.0.4/kbputils/validators.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-21 21:27:55.166743 kbputils-0.0.4/kbputils.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)     2199 2024-04-21 21:27:55.000000 kbputils-0.0.4/kbputils.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)      362 2024-04-21 21:27:55.000000 kbputils-0.0.4/kbputils.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-04-21 21:27:55.000000 kbputils-0.0.4/kbputils.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       55 2024-04-21 21:27:55.000000 kbputils-0.0.4/kbputils.egg-info/entry_points.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        4 2024-04-21 21:27:55.000000 kbputils-0.0.4/kbputils.egg-info/requires.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        9 2024-04-21 21:27:55.000000 kbputils-0.0.4/kbputils.egg-info/top_level.txt
--rw-r--r--   0 matt      (1000) matt      (1000)      545 2024-04-21 21:27:44.000000 kbputils-0.0.4/pyproject.toml
--rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-04-21 21:27:55.166743 kbputils-0.0.4/setup.cfg
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-03 18:35:39.086653 kbputils-0.0.5/
+-rw-r--r--   0 matt      (1000) matt      (1000)     1305 2024-04-16 18:40:43.000000 kbputils-0.0.5/LICENSE
+-rw-r--r--   0 matt      (1000) matt      (1000)     2199 2024-05-03 18:35:39.086653 kbputils-0.0.5/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)     1844 2024-04-16 19:00:17.000000 kbputils-0.0.5/README.md
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-03 18:35:39.083320 kbputils-0.0.5/kbputils/
+-rw-r--r--   0 matt      (1000) matt      (1000)      154 2024-05-03 18:34:35.000000 kbputils-0.0.5/kbputils/__init__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-04-16 18:40:43.000000 kbputils-0.0.5/kbputils/__main__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     2563 2024-05-03 18:34:35.000000 kbputils-0.0.5/kbputils/cli.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    14187 2024-05-03 18:34:35.000000 kbputils-0.0.5/kbputils/converters.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    18086 2024-04-16 18:40:43.000000 kbputils-0.0.5/kbputils/kbp.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      773 2024-04-16 18:40:43.000000 kbputils-0.0.5/kbputils/kbs.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     6745 2024-04-16 18:40:43.000000 kbputils-0.0.5/kbputils/validators.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-03 18:35:39.086653 kbputils-0.0.5/kbputils.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)     2199 2024-05-03 18:35:39.000000 kbputils-0.0.5/kbputils.egg-info/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)      362 2024-05-03 18:35:39.000000 kbputils-0.0.5/kbputils.egg-info/SOURCES.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-05-03 18:35:39.000000 kbputils-0.0.5/kbputils.egg-info/dependency_links.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       55 2024-05-03 18:35:39.000000 kbputils-0.0.5/kbputils.egg-info/entry_points.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        4 2024-05-03 18:35:39.000000 kbputils-0.0.5/kbputils.egg-info/requires.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        9 2024-05-03 18:35:39.000000 kbputils-0.0.5/kbputils.egg-info/top_level.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)      627 2024-05-03 18:34:35.000000 kbputils-0.0.5/pyproject.toml
+-rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-05-03 18:35:39.086653 kbputils-0.0.5/setup.cfg
```

### Comparing `kbputils-0.0.4/LICENSE` & `kbputils-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kbputils-0.0.4/PKG-INFO` & `kbputils-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbputils
-Version: 0.0.4
+Version: 0.0.5
 Summary: Utilities to handle .kbp files created with Karaoke Builder Studio.
 Author-email: Matt M <code@itmightbekaraoke.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ass
```

### Comparing `kbputils-0.0.4/README.md` & `kbputils-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `kbputils-0.0.4/kbputils/converters.py` & `kbputils-0.0.5/kbputils/converters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,77 @@
 import ass
 import dataclasses
 import datetime
 import enum
 import types
+import typing
 import collections
 from . import kbp
 from . import validators
 from . import kbs
 
 class AssAlignment(enum.Enum):
+    DEFAULT = 0
     BOTTOM_LEFT = 1
     BOTTOM_CENTER = 2
     BOTTOM_RIGHT = 3
     MIDDLE_LEFT = 4
     MIDDLE_CENTER = 5
     MIDDLE_RIGHT = 6
     TOP_LEFT = 7
     L = 7 # Alias
     TOP_CENTER = 8
     C = 8 # Alias
     TOP_RIGHT = 9
     R = 9 # Alias
-    
+
+@validators.validated_instantiation
+class AssPosition(typing.NamedTuple):
+    rotation: int
+    alignment: AssAlignment
+    x: int | float
+    y: int | float
+
+    def __str__(self):
+        result = "{"
+        if self.alignment != AssAlignment.DEFAULT:
+            result += r"\an%d" % self.alignment.value
+        if self.rotation:
+            result += r"\frz%d" % self.rotation
+        # Yes, %s, so it will stringify either an int or float and display properly
+        result += r"\pos(%s,%s)}" % (self.x, self.y)
+        return result
+
+class AssOverflow(enum.Enum):
+    NO_WRAP = 2
+    EVEN_SPLIT = 0
+    TOP_SPLIT = 1
+    BOTTOM_SPLIT = 3
+
+    def __str__(self):
+        return self.name
+
 @validators.validated_instantiation(replace="__init__")
 @dataclasses.dataclass
 class AssOptions:
     #position: bool
     #wipe: bool
     border: bool = True # Add CDG-style borders to margins
     #display: int
     #remove: int
     float_font: bool = True # Allow floating point in output font sizes (well-supported)
-    float_pos: bool = False # Allow floating point in \pos coordinates (supported by recent libass)
+    float_pos: bool = False # Allow floating point in \pos and margins (supported by recent libass)
     target_x: int = 300 # Output resolution
     target_y: int = 216
     fade_in: int = 300 # Fade duration for line display/remove
     fade_out: int = 200
     transparency: bool = True
     offset: int | bool = True # False = disable offset (same as 0), True = pull from KBS config, int is offset in ms
+    overflow: AssOverflow = AssOverflow.EVEN_SPLIT
+    #overflow_spacing: float # TODO? spacing value in styles that will apply for overflow (default 0). Multiplied by font height or based on default style?
 
     @validators.validated_types
     @staticmethod
     def __assert_valid(key: str, value):
         if key in AssOptions._fields:
             if not isinstance(value, (t := AssOptions._fields[key].type)):
                 if callable(t):
@@ -115,38 +145,47 @@
     def rescale_scalar(size: float, target_x: int, target_y: int, allow_float: bool = True, border: bool = True, font: bool = False) -> int | float:
         cdg_res = (300, 216) if border else (288, 192)
         scale = min(target_x / cdg_res[0], target_y / cdg_res[1])
         res = size * scale * (1.4 if font else 1) # Find way to calculate line_height(fontsize) instead of using this constant
         return res if (allow_float and int(res) != res) else round(res)
 
     @validators.validated_types
-    def get_pos(self, line: kbp.KBPLine, num: int) -> str:
+    def get_pos(self, line: kbp.KBPLine, num: int) -> AssPosition:
         cdg_res_x = 300 if self.border else 288
         margins = self.kbpFile.margins
+        result = {}
         y = margins["top"] + line.down + num * (self.kbpFile.margins["spacing"] + 19) + (12 if self.border else 0)
 
-        if line.align == self.style_alignments[line.style]:
-            result = r"{"
-        else:
-            result = r"{\an%d" % AssAlignment[line.align].value
-
-        if line.rotation:
-            result += f"\\frz{line.rotation}"
+        result["alignment"] = AssAlignment.DEFAULT if line.align == self.style_alignments[line.style] else AssAlignment[line.align]
 
         if line.align == 'L':
             x = margins["left"] + line.right + (6 if self.border else 0)
         elif line.align == 'C':
             x = cdg_res_x / 2 + line.right
         else: #line.align == 'R' or the file is broken
             x = cdg_res_x - margins["right"] + line.right - (6 if self.border else 0)
 
-        # TODO: Adjust margin for line based on pos for better wrapping behavior?
-        # Yes, %s, so it will stringify either an int or float and display properly
-        return result + r"\pos(%s,%s)}" % AssConverter.rescale_coords(x, y, self.target_x, self.target_y, border=self.border, allow_float=self.float_pos)
+        result["x"], result["y"] = AssConverter.rescale_coords(x, y, self.target_x, self.target_y, border=self.border, allow_float=self.float_pos)
+
+        return AssPosition(**result, rotation=line.rotation)
 
+    @validators.validated_types
+    def get_line_margins(self, line: kbp.KBPLine, pos: AssPosition | types.NoneType = None, num: int = 1) -> tuple:
+        if pos is None:
+            pos = self.get_pos(line, num)
+
+        page_margins = self.kbpFile.margins
+
+        left = page_margins["left"] - (0 if line.align == 'L' or (line.align == 'C' and line.right > 0) else line.right)
+        right = page_margins["right"] + (0 if line.align == 'R' or (line.align == 'C' and line.right < 0) else line.right)
+        left, _ = AssConverter.rescale_coords(left, pos.y, self.target_x, self.target_y, border=self.border, allow_float=self.float_pos)
+        right, _ = AssConverter.rescale_coords(right, pos.y, self.target_x, self.target_y, border=self.border, allow_float=self.float_pos)
+
+        return (left, right)
+    
     # Determine the most-used line alignment for each style to minimize \anX tags in result
     # (since alignment is not part of the KBP style, but is part of the ASS style)
     def _calc_style_alignments(self):
         # dict of alpha-keyed style to dict of alignment to frequency
         # E.g.
         # { 'A' : {'C': 5, 'L': 2}}
         # would indicate style A was centered 5 times and left-aligned twice
@@ -160,16 +199,16 @@
 
     @validators.validated_types
     def fade(self) -> str:
         return r"{\fad(%d,%d)}" % (self.options.fade_in, self.options.fade_out)
 
     # Convert a line of syllables into the text of a dialogue event including wipe tags
     @validators.validated_types
-    def kbp2asstext(self, line: kbp.KBPLine, num: int):
-        result = self.get_pos(line, num) + self.fade()
+    def kbp2asstext(self, line: kbp.KBPLine, pos: AssPosition):
+        result = str(pos) + self.fade()
         if self.kbpFile.styles[line.style].fixed:
             return result + line.text()
         cur = line.start
         for (n, s) in enumerate(line.syllables):
             delay = s.start - cur
             dur = s.end - s.start
 
@@ -210,15 +249,15 @@
         return alpha + "".join(x+x for x in reversed(list(kbpcolor)))
 
     def ass_document(self):
         result = ass.Document()
         result.info.update(
             Title="",
             ScriptType="v4.00+",
-            WrapStyle=0,
+            WrapStyle=self.overflow.value,
             ScaledBorderAndShadow="yes",
             Collisions="Normal",
             PlayResX=self.options.target_x,
             PlayResY=self.options.target_y,
             ) 
 
         if self.options.offset is False:
@@ -229,21 +268,24 @@
 
         styles = self.kbpFile.styles
         self._calc_style_alignments()
         for page in self.kbpFile.pages:
             for num, line in enumerate(page.lines):
                 if line.isempty():
                     continue
+                pos = self.get_pos(line, num)
+                line_margins = self.get_line_margins(line, pos)
                 result.events.append(ass.Dialogue(
                     start=datetime.timedelta(milliseconds = line.start * 10 + self.options.offset),
                     end=datetime.timedelta(milliseconds = line.end * 10 + self.options.offset),
                     style=AssConverter.ass_style_name(kbp.KBPStyleCollection.alpha2key(line.style), styles[line.style].name),
                     effect="karaoke",
-                    text=self.kbp2asstext(line, num),
-                    # TODO: set margins for proper wrapping? Need to be modified for pos
+                    text=self.kbp2asstext(line, pos),
+                    margin_l=line_margins[0],
+                    margin_r=line_margins[1],
                     ))
         for idx in styles:
             style = styles[idx]
             result.styles.append(ass.Style(
                 name=AssConverter.ass_style_name(idx, style.name),
                 fontname=style.fontname,
                 fontsize=AssConverter.rescale_scalar(style.fontsize, self.target_x, self.target_y, font = True, border=self.border),
@@ -254,16 +296,16 @@
                 back_color=AssConverter.kbp2asscolor(style.outlinewipecolor, palette=self.kbpFile.colors, transparency=self.options.transparency),
                 bold = 'B' in style.fontstyle,
                 italic = 'I' in style.fontstyle,
                 underline = 'U' in style.fontstyle,
                 strike_out = 'S' in style.fontstyle,
                 outline = AssConverter.rescale_scalar(sum(style.outlines), self.target_x, self.target_y, border=self.border)/4, # NOTE: only one outline, but it's a float, so maybe averaging will be helpful
                 shadow = AssConverter.rescale_scalar(sum(style.shadows), self.target_x, self.target_y, border=self.border)/2,
-                margin_l = 0, # TODO: determine if these should be set and if page margins and line margins stack
-                margin_r = 0,
+                margin_l = 0, # TODO: Decide if these should be set (and overridden on lines only when different)
+                margin_r = 0, # TODO cont: Potentially could also be set by style like alignment based on most-used positions
                 margin_v = 0,
                 encoding = style.charset,
                 alignment=AssAlignment[self.style_alignments.get(kbp.KBPStyleCollection.key2alpha(idx), 'C')].value,
                 ))
             
         return result
```

### Comparing `kbputils-0.0.4/kbputils/kbp.py` & `kbputils-0.0.5/kbputils/kbp.py`

 * *Files identical despite different names*

### Comparing `kbputils-0.0.4/kbputils/kbs.py` & `kbputils-0.0.5/kbputils/kbs.py`

 * *Files identical despite different names*

### Comparing `kbputils-0.0.4/kbputils/validators.py` & `kbputils-0.0.5/kbputils/validators.py`

 * *Files identical despite different names*

### Comparing `kbputils-0.0.4/kbputils.egg-info/PKG-INFO` & `kbputils-0.0.5/kbputils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbputils
-Version: 0.0.4
+Version: 0.0.5
 Summary: Utilities to handle .kbp files created with Karaoke Builder Studio.
 Author-email: Matt M <code@itmightbekaraoke.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ass
```

### Comparing `kbputils-0.0.4/pyproject.toml` & `kbputils-0.0.5/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kbputils"
-version = "0.0.4"
+dynamic = ["version"]
 authors = [
   { name="Matt M", email="code@itmightbekaraoke.com" },
 ]
 description = "Utilities to handle .kbp files created with Karaoke Builder Studio."
 readme = "README.md"
 dependencies = [
     "ass"
@@ -12,11 +12,13 @@
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: BSD License"
 ]
 [project.scripts]
 KBPUtils = "kbputils.cli:convert_file"
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools >= 61.0.0"]
 build-backend = "setuptools.build_meta"
 [tool.setuptools.packages.find]
 include = ["kbputils"]
+[tool.setuptools.dynamic]
+version = {attr = "kbputils.__version__"}
```


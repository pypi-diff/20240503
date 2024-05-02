# Comparing `tmp/pdftext-0.3.3.tar.gz` & `tmp/pdftext-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdftext-0.3.3.tar", max compression
+gzip compressed data, was "pdftext-0.3.4.tar", max compression
```

## Comparing `pdftext-0.3.3.tar` & `pdftext-0.3.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11269 2024-05-02 17:27:01.276151 pdftext-0.3.3/LICENSE
--rw-r--r--   0        0        0     7170 2024-05-02 17:27:01.276151 pdftext-0.3.3/README.md
--rw-r--r--   0        0        0     1726 2024-05-02 17:27:01.276151 pdftext-0.3.3/extract_text.py
--rw-r--r--   0        0        0    14097 2024-05-02 17:27:01.280151 pdftext-0.3.3/models/dt.joblib
--rw-r--r--   0        0        0     2426 2024-05-02 17:27:01.280151 pdftext-0.3.3/pdftext/extraction.py
--rw-r--r--   0        0        0     7242 2024-05-02 17:27:01.280151 pdftext-0.3.3/pdftext/inference.py
--rw-r--r--   0        0        0      153 2024-05-02 17:27:01.280151 pdftext-0.3.3/pdftext/model.py
--rw-r--r--   0        0        0     3752 2024-05-02 17:27:01.280151 pdftext-0.3.3/pdftext/pdf/chars.py
--rw-r--r--   0        0        0     4653 2024-05-02 17:27:01.280151 pdftext-0.3.3/pdftext/pdf/utils.py
--rw-r--r--   0        0        0     3222 2024-05-02 17:27:01.280151 pdftext-0.3.3/pdftext/postprocessing.py
--rw-r--r--   0        0        0      579 2024-05-02 17:27:01.280151 pdftext-0.3.3/pdftext/settings.py
--rw-r--r--   0        0        0      856 2024-05-02 17:27:01.280151 pdftext-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     8146 1970-01-01 00:00:00.000000 pdftext-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    11269 2024-05-02 22:58:30.842906 pdftext-0.3.4/LICENSE
+-rw-r--r--   0        0        0     7170 2024-05-02 22:58:30.842906 pdftext-0.3.4/README.md
+-rw-r--r--   0        0        0     1726 2024-05-02 22:58:30.846906 pdftext-0.3.4/extract_text.py
+-rw-r--r--   0        0        0    14097 2024-05-02 22:58:30.846906 pdftext-0.3.4/models/dt.joblib
+-rw-r--r--   0        0        0     2426 2024-05-02 22:58:30.846906 pdftext-0.3.4/pdftext/extraction.py
+-rw-r--r--   0        0        0     7212 2024-05-02 22:58:30.846906 pdftext-0.3.4/pdftext/inference.py
+-rw-r--r--   0        0        0      153 2024-05-02 22:58:30.846906 pdftext-0.3.4/pdftext/model.py
+-rw-r--r--   0        0        0     3752 2024-05-02 22:58:30.846906 pdftext-0.3.4/pdftext/pdf/chars.py
+-rw-r--r--   0        0        0     4613 2024-05-02 22:58:30.846906 pdftext-0.3.4/pdftext/pdf/utils.py
+-rw-r--r--   0        0        0     3222 2024-05-02 22:58:30.846906 pdftext-0.3.4/pdftext/postprocessing.py
+-rw-r--r--   0        0        0      489 2024-05-02 22:58:30.846906 pdftext-0.3.4/pdftext/settings.py
+-rw-r--r--   0        0        0      856 2024-05-02 22:58:30.846906 pdftext-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     8146 1970-01-01 00:00:00.000000 pdftext-0.3.4/PKG-INFO
```

### Comparing `pdftext-0.3.3/LICENSE` & `pdftext-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.3/README.md` & `pdftext-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.3/extract_text.py` & `pdftext-0.3.4/extract_text.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.3/models/dt.joblib` & `pdftext-0.3.4/models/dt.joblib`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.3/pdftext/extraction.py` & `pdftext-0.3.4/pdftext/extraction.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.3/pdftext/inference.py` & `pdftext-0.3.4/pdftext/inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             # First item is probability of same line/block, second is probability of new line, third is probability of new block
             if prediction_probs[0] >= .5:
                 pass
             elif prediction_probs[2] > block_threshold:
                 span = update_span(line, span)
                 line = update_line(block, line)
                 block = update_block(blocks, block)
-            elif prev_char["char"] in LINE_BREAKS and prediction_probs[1] >= .5: # Look for newline character as a forcing signal for a new line
+            elif prev_char["char"] in LINE_BREAKS: # Look for newline character as a forcing signal for a new line
                 span = update_span(line, span)
                 line = update_line(block, line)
             elif prev_font_info != font_info:
                 span = update_span(line, span)
 
         span["chars"].append(char_info)
         update_current(line, char_info)
```

### Comparing `pdftext-0.3.3/pdftext/pdf/chars.py` & `pdftext-0.3.4/pdftext/pdf/chars.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.3/pdftext/pdf/utils.py` & `pdftext-0.3.4/pdftext/pdf/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,15 @@
 
 def get_fontname(textpage, char_index):
     n_bytes = pdfium_c.FPDFText_GetFontInfo(textpage, char_index, None, 0, None)
     buffer = ctypes.create_string_buffer(n_bytes)
     # Re-interpret the type from char to unsigned short as required by the function
     buffer_ptr = ctypes.cast(buffer, ctypes.POINTER(ctypes.c_ushort))
     flag_buffer = ctypes.c_int()
-    flag_ptr = ctypes.pointer(flag_buffer)
-    font_info = pdfium_c.FPDFText_GetFontInfo(textpage, char_index, buffer_ptr, n_bytes, flag_ptr)
+    font_info = pdfium_c.FPDFText_GetFontInfo(textpage, char_index, buffer_ptr, n_bytes, flag_buffer)
     if font_info == 0:
         return None, None
     try:
         decoded = buffer.value.decode("utf-8")
     except Exception as e:
         return None, None
     return decoded, flag_buffer.value
```

### Comparing `pdftext-0.3.3/pdftext/postprocessing.py` & `pdftext-0.3.4/pdftext/postprocessing.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.3/pyproject.toml` & `pdftext-0.3.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdftext"
-version = "0.3.3"
+version = "0.3.4"
 description = "Extract structured text from pdfs quickly"
 authors = ["Vik Paruchuri <vik.paruchuri@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/VikParuchuri/pdftext"
 keywords = ["pdf", "text", "extraction"]
 packages = [
```

### Comparing `pdftext-0.3.3/PKG-INFO` & `pdftext-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdftext
-Version: 0.3.3
+Version: 0.3.4
 Summary: Extract structured text from pdfs quickly
 Home-page: https://github.com/VikParuchuri/pdftext
 License: Apache-2.0
 Keywords: pdf,text,extraction
 Author: Vik Paruchuri
 Author-email: vik.paruchuri@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
```


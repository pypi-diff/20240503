# Comparing `tmp/txt-from-pdf-1.0.1.tar.gz` & `tmp/txt-from-pdf-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txt-from-pdf-1.0.1.tar", last modified: Thu Apr 18 16:21:39 2024, max compression
+gzip compressed data, was "txt-from-pdf-1.1.0.tar", last modified: Fri May  3 15:39:40 2024, max compression
```

## Comparing `txt-from-pdf-1.0.1.tar` & `txt-from-pdf-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 asafaya    (501) staff       (20)        0 2024-04-18 16:21:39.070612 txt-from-pdf-1.0.1/
--rw-r--r--   0 asafaya    (501) staff       (20)    11357 2024-04-18 13:31:13.000000 txt-from-pdf-1.0.1/LICENSE
--rw-r--r--   0 asafaya    (501) staff       (20)     2419 2024-04-18 16:21:39.070496 txt-from-pdf-1.0.1/PKG-INFO
--rw-r--r--   0 asafaya    (501) staff       (20)     1583 2024-04-18 13:50:49.000000 txt-from-pdf-1.0.1/README.md
--rw-r--r--   0 asafaya    (501) staff       (20)      672 2024-04-18 13:38:51.000000 txt-from-pdf-1.0.1/pyproject.toml
--rw-r--r--   0 asafaya    (501) staff       (20)       38 2024-04-18 16:21:39.070655 txt-from-pdf-1.0.1/setup.cfg
--rw-r--r--   0 asafaya    (501) staff       (20)     2301 2024-04-18 16:20:44.000000 txt-from-pdf-1.0.1/setup.py
-drwxr-xr-x   0 asafaya    (501) staff       (20)        0 2024-04-18 16:21:39.069269 txt-from-pdf-1.0.1/txt_from_pdf.egg-info/
--rw-r--r--   0 asafaya    (501) staff       (20)     2419 2024-04-18 16:21:39.000000 txt-from-pdf-1.0.1/txt_from_pdf.egg-info/PKG-INFO
--rw-r--r--   0 asafaya    (501) staff       (20)      394 2024-04-18 16:21:39.000000 txt-from-pdf-1.0.1/txt_from_pdf.egg-info/SOURCES.txt
--rw-r--r--   0 asafaya    (501) staff       (20)        1 2024-04-18 16:21:39.000000 txt-from-pdf-1.0.1/txt_from_pdf.egg-info/dependency_links.txt
--rw-r--r--   0 asafaya    (501) staff       (20)       62 2024-04-18 16:21:39.000000 txt-from-pdf-1.0.1/txt_from_pdf.egg-info/entry_points.txt
--rw-r--r--   0 asafaya    (501) staff       (20)       86 2024-04-18 16:21:39.000000 txt-from-pdf-1.0.1/txt_from_pdf.egg-info/requires.txt
--rw-r--r--   0 asafaya    (501) staff       (20)       11 2024-04-18 16:21:39.000000 txt-from-pdf-1.0.1/txt_from_pdf.egg-info/top_level.txt
-drwxr-xr-x   0 asafaya    (501) staff       (20)        0 2024-04-18 16:21:39.070196 txt-from-pdf-1.0.1/txtfrompdf/
--rw-r--r--   0 asafaya    (501) staff       (20)      255 2024-04-18 16:20:10.000000 txt-from-pdf-1.0.1/txtfrompdf/__init__.py
--rw-r--r--   0 asafaya    (501) staff       (20)     2361 2024-04-18 16:20:19.000000 txt-from-pdf-1.0.1/txtfrompdf/__main__.py
--rw-r--r--   0 asafaya    (501) staff       (20)     4902 2024-04-18 16:20:33.000000 txt-from-pdf-1.0.1/txtfrompdf/extract.py
--rw-r--r--   0 asafaya    (501) staff       (20)     6575 2024-04-18 13:38:56.000000 txt-from-pdf-1.0.1/txtfrompdf/filter.py
--rw-r--r--   0 asafaya    (501) staff       (20)     3296 2024-04-18 13:14:25.000000 txt-from-pdf-1.0.1/txtfrompdf/fix_unicode.py
--rw-r--r--   0 asafaya    (501) staff       (20)      511 2024-04-18 13:14:27.000000 txt-from-pdf-1.0.1/txtfrompdf/utils.py
+drwxr-xr-x   0 asafaya    (501) staff       (20)        0 2024-05-03 15:39:40.651329 txt-from-pdf-1.1.0/
+-rw-r--r--   0 asafaya    (501) staff       (20)    11357 2024-04-18 13:31:13.000000 txt-from-pdf-1.1.0/LICENSE
+-rw-r--r--   0 asafaya    (501) staff       (20)     2428 2024-05-03 15:39:40.651221 txt-from-pdf-1.1.0/PKG-INFO
+-rw-r--r--   0 asafaya    (501) staff       (20)     1592 2024-05-03 15:38:37.000000 txt-from-pdf-1.1.0/README.md
+-rw-r--r--   0 asafaya    (501) staff       (20)      672 2024-04-18 13:38:51.000000 txt-from-pdf-1.1.0/pyproject.toml
+-rw-r--r--   0 asafaya    (501) staff       (20)       38 2024-05-03 15:39:40.651373 txt-from-pdf-1.1.0/setup.cfg
+-rw-r--r--   0 asafaya    (501) staff       (20)     2301 2024-05-03 15:36:47.000000 txt-from-pdf-1.1.0/setup.py
+drwxr-xr-x   0 asafaya    (501) staff       (20)        0 2024-05-03 15:39:40.649738 txt-from-pdf-1.1.0/txt_from_pdf.egg-info/
+-rw-r--r--   0 asafaya    (501) staff       (20)     2428 2024-05-03 15:39:40.000000 txt-from-pdf-1.1.0/txt_from_pdf.egg-info/PKG-INFO
+-rw-r--r--   0 asafaya    (501) staff       (20)      394 2024-05-03 15:39:40.000000 txt-from-pdf-1.1.0/txt_from_pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 asafaya    (501) staff       (20)        1 2024-05-03 15:39:40.000000 txt-from-pdf-1.1.0/txt_from_pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 asafaya    (501) staff       (20)       62 2024-05-03 15:39:40.000000 txt-from-pdf-1.1.0/txt_from_pdf.egg-info/entry_points.txt
+-rw-r--r--   0 asafaya    (501) staff       (20)       86 2024-05-03 15:39:40.000000 txt-from-pdf-1.1.0/txt_from_pdf.egg-info/requires.txt
+-rw-r--r--   0 asafaya    (501) staff       (20)       11 2024-05-03 15:39:40.000000 txt-from-pdf-1.1.0/txt_from_pdf.egg-info/top_level.txt
+drwxr-xr-x   0 asafaya    (501) staff       (20)        0 2024-05-03 15:39:40.650937 txt-from-pdf-1.1.0/txtfrompdf/
+-rw-r--r--   0 asafaya    (501) staff       (20)      255 2024-05-03 15:36:29.000000 txt-from-pdf-1.1.0/txtfrompdf/__init__.py
+-rw-r--r--   0 asafaya    (501) staff       (20)     2361 2024-04-18 16:20:19.000000 txt-from-pdf-1.1.0/txtfrompdf/__main__.py
+-rw-r--r--   0 asafaya    (501) staff       (20)     4903 2024-04-30 20:35:51.000000 txt-from-pdf-1.1.0/txtfrompdf/extract.py
+-rw-r--r--   0 asafaya    (501) staff       (20)     6575 2024-04-18 13:38:56.000000 txt-from-pdf-1.1.0/txtfrompdf/filter.py
+-rw-r--r--   0 asafaya    (501) staff       (20)     3296 2024-04-30 20:26:33.000000 txt-from-pdf-1.1.0/txtfrompdf/fix_unicode.py
+-rw-r--r--   0 asafaya    (501) staff       (20)      511 2024-04-18 13:14:27.000000 txt-from-pdf-1.1.0/txtfrompdf/utils.py
```

### Comparing `txt-from-pdf-1.0.1/LICENSE` & `txt-from-pdf-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `txt-from-pdf-1.0.1/PKG-INFO` & `txt-from-pdf-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txt-from-pdf
-Version: 1.0.1
+Version: 1.1.0
 Summary: Extract clean text from PDFs.
 Home-page: https://github.com/alisafaya/txt-from-pdf
 Author: Ali Safaya
 Author-email: alisafaya@gmail.com
 License: Apache
 Keywords: pdf text extraction
 Classifier: Intended Audience :: Developers
@@ -39,15 +39,15 @@
 
 # Usage
 
 ```python
 from txtfrompdf import extract_txt_from_pdf
 
 pdf_path = "file.pdf"
-text = extract_pdf(pdf_path)
+text = extract_txt_from_pdf(pdf_path)
 print(text)
 ```
 
 # CLI Usage
 
 Single file:
```

### Comparing `txt-from-pdf-1.0.1/README.md` & `txt-from-pdf-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # Usage
 
 ```python
 from txtfrompdf import extract_txt_from_pdf
 
 pdf_path = "file.pdf"
-text = extract_pdf(pdf_path)
+text = extract_txt_from_pdf(pdf_path)
 print(text)
 ```
 
 # CLI Usage
 
 Single file:
```

### Comparing `txt-from-pdf-1.0.1/pyproject.toml` & `txt-from-pdf-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `txt-from-pdf-1.0.1/setup.py` & `txt-from-pdf-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 extras = {}
 extras["dev"] = ["black ~= 23.0", "ruff>=0.2"]
 
 setup(
     name="txt-from-pdf",
-    version="1.0.1",
+    version="1.1.0",
     description="Extract clean text from PDFs.",
     license_files=["LICENSE"],
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="pdf text extraction",
     license="Apache",
     author="Ali Safaya",
```

### Comparing `txt-from-pdf-1.0.1/txt_from_pdf.egg-info/PKG-INFO` & `txt-from-pdf-1.1.0/txt_from_pdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txt-from-pdf
-Version: 1.0.1
+Version: 1.1.0
 Summary: Extract clean text from PDFs.
 Home-page: https://github.com/alisafaya/txt-from-pdf
 Author: Ali Safaya
 Author-email: alisafaya@gmail.com
 License: Apache
 Keywords: pdf text extraction
 Classifier: Intended Audience :: Developers
@@ -39,15 +39,15 @@
 
 # Usage
 
 ```python
 from txtfrompdf import extract_txt_from_pdf
 
 pdf_path = "file.pdf"
-text = extract_pdf(pdf_path)
+text = extract_txt_from_pdf(pdf_path)
 print(text)
 ```
 
 # CLI Usage
 
 Single file:
```

### Comparing `txt-from-pdf-1.0.1/txtfrompdf/__main__.py` & `txt-from-pdf-1.1.0/txtfrompdf/__main__.py`

 * *Files identical despite different names*

### Comparing `txt-from-pdf-1.0.1/txtfrompdf/extract.py` & `txt-from-pdf-1.1.0/txtfrompdf/extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     retstr = BytesIO()
     layout = LAParams(all_texts=True)
     device = TextConverter(manager, retstr, laparams=layout)
     filepath = open(path, "rb")
     interpreter = PDFPageInterpreter(manager, device)
 
     try:
-        for page in PDFPage.get_pages(filepath, check_extractable=True):
+        for page in PDFPage.get_pages(filepath, check_extractable=False):
             interpreter.process_page(page)
 
     except (PDFSyntaxError, TypeError):
         logger.error(f"ERROR: Extraction failed for {path}")
 
     text = retstr.getvalue()
     filepath.close()
```

### Comparing `txt-from-pdf-1.0.1/txtfrompdf/filter.py` & `txt-from-pdf-1.1.0/txtfrompdf/filter.py`

 * *Files identical despite different names*

### Comparing `txt-from-pdf-1.0.1/txtfrompdf/fix_unicode.py` & `txt-from-pdf-1.1.0/txtfrompdf/fix_unicode.py`

 * *Files identical despite different names*


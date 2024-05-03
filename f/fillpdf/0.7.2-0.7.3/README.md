# Comparing `tmp/fillpdf-0.7.2.tar.gz` & `tmp/fillpdf-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/tyler/Desktop/School Stuff/Applied Programming/fillpdf/dist/tmpq75d_v1c/fillpdf-0.7.2.tar", last modified: Fri May 20 00:07:21 2022, max compression
+gzip compressed data, was "fillpdf-0.7.3.tar", last modified: Fri May  3 18:02:12 2024, max compression
```

## Comparing `fillpdf-0.7.2.tar` & `fillpdf-0.7.3.tar`

### file list

```diff
@@ -1,18 +1,24 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2022-05-20 00:07:21.863818 fillpdf-0.7.2/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1070 2021-02-18 23:46:14.000000 fillpdf-0.7.2/LICENSE
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    16894 2022-05-20 00:07:21.863818 fillpdf-0.7.2/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    16457 2022-05-20 00:04:55.000000 fillpdf-0.7.2/README.md
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2022-05-20 00:07:21.855817 fillpdf-0.7.2/fillpdf/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      577 2021-11-19 02:49:32.000000 fillpdf-0.7.2/fillpdf/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     4933 2021-11-19 02:49:32.000000 fillpdf-0.7.2/fillpdf/extractfillpdf.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    24354 2022-05-20 00:04:55.000000 fillpdf-0.7.2/fillpdf/fillpdfs.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     5718 2021-11-19 02:49:32.000000 fillpdf-0.7.2/fillpdf/insertfillpdf.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2022-05-20 00:07:21.859817 fillpdf-0.7.2/fillpdf.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    16894 2022-05-20 00:07:20.000000 fillpdf-0.7.2/fillpdf.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      315 2022-05-20 00:07:21.000000 fillpdf-0.7.2/fillpdf.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2022-05-20 00:07:20.000000 fillpdf-0.7.2/fillpdf.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      104 2022-05-20 00:07:21.000000 fillpdf-0.7.2/fillpdf.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       32 2022-05-20 00:07:21.000000 fillpdf-0.7.2/fillpdf.egg-info/requires.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2022-05-20 00:07:21.000000 fillpdf-0.7.2/fillpdf.egg-info/top_level.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      681 2022-05-20 00:07:21.863818 fillpdf-0.7.2/setup.cfg
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      817 2022-05-20 00:07:07.000000 fillpdf-0.7.2/setup.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-03 18:02:12.459356 fillpdf-0.7.3/
+-rw-r--r--   0 tyler      (501) staff       (20)     1070 2024-05-03 17:58:46.000000 fillpdf-0.7.3/LICENSE
+-rw-r--r--   0 tyler      (501) staff       (20)    15932 2024-05-03 18:02:12.459118 fillpdf-0.7.3/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)    15403 2024-05-03 17:58:46.000000 fillpdf-0.7.3/README.md
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-03 18:02:12.456768 fillpdf-0.7.3/fillpdf/
+-rw-r--r--   0 tyler      (501) staff       (20)      577 2024-05-03 17:58:46.000000 fillpdf-0.7.3/fillpdf/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4933 2024-05-03 17:58:46.000000 fillpdf-0.7.3/fillpdf/extractfillpdf.py
+-rw-r--r--   0 tyler      (501) staff       (20)    25126 2024-05-03 17:58:46.000000 fillpdf-0.7.3/fillpdf/fillpdfs.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5718 2024-05-03 17:58:46.000000 fillpdf-0.7.3/fillpdf/insertfillpdf.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-03 18:02:12.458081 fillpdf-0.7.3/fillpdf/utils/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2024-05-03 17:58:46.000000 fillpdf-0.7.3/fillpdf/utils/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)      744 2024-05-03 17:58:46.000000 fillpdf-0.7.3/fillpdf/utils/field_format.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-03 18:02:12.458761 fillpdf-0.7.3/fillpdf.egg-info/
+-rw-r--r--   0 tyler      (501) staff       (20)    15932 2024-05-03 18:02:12.000000 fillpdf-0.7.3/fillpdf.egg-info/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)      417 2024-05-03 18:02:12.000000 fillpdf-0.7.3/fillpdf.egg-info/SOURCES.txt
+-rw-r--r--   0 tyler      (501) staff       (20)        1 2024-05-03 18:02:12.000000 fillpdf-0.7.3/fillpdf.egg-info/dependency_links.txt
+-rw-r--r--   0 tyler      (501) staff       (20)      104 2024-05-03 18:02:12.000000 fillpdf-0.7.3/fillpdf.egg-info/entry_points.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       32 2024-05-03 18:02:12.000000 fillpdf-0.7.3/fillpdf.egg-info/requires.txt
+-rw-r--r--   0 tyler      (501) staff       (20)        8 2024-05-03 18:02:12.000000 fillpdf-0.7.3/fillpdf.egg-info/top_level.txt
+-rw-r--r--   0 tyler      (501) staff       (20)      681 2024-05-03 18:02:12.460149 fillpdf-0.7.3/setup.cfg
+-rw-r--r--   0 tyler      (501) staff       (20)      818 2024-05-03 17:58:46.000000 fillpdf-0.7.3/setup.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-03 18:02:12.458439 fillpdf-0.7.3/tests/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2024-05-03 17:58:46.000000 fillpdf-0.7.3/tests/test_myfunctions.py
+-rw-r--r--   0 tyler      (501) staff       (20)      644 2024-05-03 17:58:46.000000 fillpdf-0.7.3/tests/test_utils.py
```

### Comparing `fillpdf-0.7.2/LICENSE` & `fillpdf-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fillpdf-0.7.2/PKG-INFO` & `fillpdf-0.7.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: fillpdf
-Version: 0.7.2
-Summary: A Library to fill and flatten pdfs
-Home-page: https://github.com/t-houssian/fillpdf
-Author: Tyler Houssian
-Author-email: tylerhoussian@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # fillpdf
 https://pypi.org/project/fillpdf/
 
 # Documentation:
 [View The Documentation](https://fillpdf.readthedocs.io/en/latest/)
 
 ![GitHub](https://img.shields.io/github/license/t-houssian/fillpdf) ![PyPI](https://img.shields.io/pypi/v/fillpdf) ![GitHub last commit](https://img.shields.io/github/last-commit/t-houssian/fillpdf) [![Documentation Status](https://readthedocs.org/projects/fillpdf/badge/?version=latest)](https://fillpdf.readthedocs.io/en/latest/?badge=latest)
@@ -56,45 +42,25 @@
 ##### write_fillable_pdf
     write_fillable_pdf(input_pdf_path, output_pdf_path, data_dict, flatten=False)
 - input_pdf_path- path to your pdf you want to alter (including the pdf name could just leave as 'blank.pdf' if the pdf is in your current directory)
 - output_pdf_path- path of where you want your pdf to write to (including the pdf name could just leave as 'new.pdf' to write to current directory)
 - data_dict- dictionary that contains the fields to write to as your key and what to write to it as your value (get this from the get_form_fields function)
 - flatten (default=False)- If True, then the fields will become uneditable when you write to the pdf.
 ###### For Example:
-    data_dict = {'Address # Useful Websites
-
-* [List PDF Fields pdfrw](https://github.com/pmaupin/pdfrw/issues/165)
-* [List PDF Fields](https://stackoverflow.com/questions/3984003/how-to-extract-pdf-fields-from-a-filled-out-form-in-python)
-* [Fill PDF Fields](https://stackoverflow.com/questions/60082481/how-to-edit-checkboxes-and-save-changes-in-an-editable-pdf-using-the-python-pdfr)
-* [Flatten PDFs](https://stackoverflow.com/questions/27023043/generate-flattened-pdf-with-python)
-* [pdfrw2](https://pypi.org/project/pdfrw2/)
-
-# Credit
-- [dvska](https://stackoverflow.com/users/1303068/dvska)
-- [gbroiles](https://github.com/pmaupin/pdfrw/issues/165)
-- [tomatoeshift](https://stackoverflow.com/users/11998874/tomatoeshift)
-- [Tyler Houssian](https://stackoverflow.com/users/13537359/tyler-houssian)
-- [jtplaarj](https://github.com/jtplaarj)
-- [WestHealth](https://github.com/WestHealth/pdf-form-filler)
-- [sarnold](https://github.com/sarnold)
-- [Patrick Maupin](https://github.com/pmaupin)
-
-# Future Work
-* give option to place text by coordinate
-* alter or view pdf versions
-1 Text Box': '500 West Main Street',
+    data_dict = {'Address1 Text Box': '500 West Main Street',
     'Driving License Check Box': 'Yes',
     'Language 1 Check Box': 'Off',}
     
     fillpdfs.write_fillable_pdf('blank.pdf', 'new.pdf', data_dict)
 - For radio boxes ('Off' = not filled, 'Yes' = filled)
 - For check boxes ('Off' or '' = not filled, 'Yes' = filled)
 - For drop downs (Enter the name of the desired drop down option)
 - For radio groups ('0' = The first option, '1' = The second option, '2' = the third option, etc.)
 
+
 ##### flatten_pdf
     flatten_pdf(input_pdf_path, output_pdf_path, as_images=False)
 - input_pdf_path- path to your pdf you want to alter (including the pdf name could just leave as 'blank.pdf' if the pdf is in your current directory)
 - output_pdf_path- path of where you want your pdf to write to (including the pdf name could just leave as 'new.pdf' to write to current directory)
 - as_images=False- Default is False meaning it will update each individual annotation and set
         it to False. True means it will convert to images and then reinsert into the
         pdf. Try this if the first is not working. (this image technique requires poppler.)
```

### Comparing `fillpdf-0.7.2/README.md` & `fillpdf-0.7.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: fillpdf
+Version: 0.7.3
+Summary: A Library to fill and flatten pdfs
+Home-page: https://github.com/t-houssian/fillpdf
+Author: Tyler Houssian
+Author-email: tylerhoussian@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pdfrw2
+Requires-Dist: pdf2image
+Requires-Dist: Pillow
+Requires-Dist: pymupdf
+
 # fillpdf
 https://pypi.org/project/fillpdf/
 
 # Documentation:
 [View The Documentation](https://fillpdf.readthedocs.io/en/latest/)
 
 ![GitHub](https://img.shields.io/github/license/t-houssian/fillpdf) ![PyPI](https://img.shields.io/pypi/v/fillpdf) ![GitHub last commit](https://img.shields.io/github/last-commit/t-houssian/fillpdf) [![Documentation Status](https://readthedocs.org/projects/fillpdf/badge/?version=latest)](https://fillpdf.readthedocs.io/en/latest/?badge=latest)
@@ -42,45 +60,25 @@
 ##### write_fillable_pdf
     write_fillable_pdf(input_pdf_path, output_pdf_path, data_dict, flatten=False)
 - input_pdf_path- path to your pdf you want to alter (including the pdf name could just leave as 'blank.pdf' if the pdf is in your current directory)
 - output_pdf_path- path of where you want your pdf to write to (including the pdf name could just leave as 'new.pdf' to write to current directory)
 - data_dict- dictionary that contains the fields to write to as your key and what to write to it as your value (get this from the get_form_fields function)
 - flatten (default=False)- If True, then the fields will become uneditable when you write to the pdf.
 ###### For Example:
-    data_dict = {'Address # Useful Websites
-
-* [List PDF Fields pdfrw](https://github.com/pmaupin/pdfrw/issues/165)
-* [List PDF Fields](https://stackoverflow.com/questions/3984003/how-to-extract-pdf-fields-from-a-filled-out-form-in-python)
-* [Fill PDF Fields](https://stackoverflow.com/questions/60082481/how-to-edit-checkboxes-and-save-changes-in-an-editable-pdf-using-the-python-pdfr)
-* [Flatten PDFs](https://stackoverflow.com/questions/27023043/generate-flattened-pdf-with-python)
-* [pdfrw2](https://pypi.org/project/pdfrw2/)
-
-# Credit
-- [dvska](https://stackoverflow.com/users/1303068/dvska)
-- [gbroiles](https://github.com/pmaupin/pdfrw/issues/165)
-- [tomatoeshift](https://stackoverflow.com/users/11998874/tomatoeshift)
-- [Tyler Houssian](https://stackoverflow.com/users/13537359/tyler-houssian)
-- [jtplaarj](https://github.com/jtplaarj)
-- [WestHealth](https://github.com/WestHealth/pdf-form-filler)
-- [sarnold](https://github.com/sarnold)
-- [Patrick Maupin](https://github.com/pmaupin)
-
-# Future Work
-* give option to place text by coordinate
-* alter or view pdf versions
-1 Text Box': '500 West Main Street',
+    data_dict = {'Address1 Text Box': '500 West Main Street',
     'Driving License Check Box': 'Yes',
     'Language 1 Check Box': 'Off',}
     
     fillpdfs.write_fillable_pdf('blank.pdf', 'new.pdf', data_dict)
 - For radio boxes ('Off' = not filled, 'Yes' = filled)
 - For check boxes ('Off' or '' = not filled, 'Yes' = filled)
 - For drop downs (Enter the name of the desired drop down option)
 - For radio groups ('0' = The first option, '1' = The second option, '2' = the third option, etc.)
 
+
 ##### flatten_pdf
     flatten_pdf(input_pdf_path, output_pdf_path, as_images=False)
 - input_pdf_path- path to your pdf you want to alter (including the pdf name could just leave as 'blank.pdf' if the pdf is in your current directory)
 - output_pdf_path- path of where you want your pdf to write to (including the pdf name could just leave as 'new.pdf' to write to current directory)
 - as_images=False- Default is False meaning it will update each individual annotation and set
         it to False. True means it will convert to images and then reinsert into the
         pdf. Try this if the first is not working. (this image technique requires poppler.)
```

### Comparing `fillpdf-0.7.2/fillpdf/__init__.py` & `fillpdf-0.7.3/fillpdf/__init__.py`

 * *Files identical despite different names*

### Comparing `fillpdf-0.7.2/fillpdf/extractfillpdf.py` & `fillpdf-0.7.3/fillpdf/extractfillpdf.py`

 * *Files identical despite different names*

### Comparing `fillpdf-0.7.2/fillpdf/fillpdfs.py` & `fillpdf-0.7.3/fillpdf/fillpdfs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import fitz
 import math
 import pdfrw
 from pdf2image import convert_from_path # Needs conda install -c conda-forge poppler
 from PIL import Image
 from collections import OrderedDict
 
+from fillpdf.utils.field_format import is_text_field_multiline, make_read_only
 ANNOT_KEY = '/Annots'               # key for all annotations within a page
 ANNOT_FIELD_KEY = '/T'              # Name of field. i.e. given ID of field
 ANNOT_FORM_type = '/FT'             # Form type (e.g. text/button)
 ANNOT_FORM_button = '/Btn'          # ID for buttons, i.e. a checkbox
 ANNOT_FORM_text = '/Tx'             # ID for textbox
 ANNOT_FORM_options = '/Opt'
 ANNOT_FORM_combo = '/Ch'
@@ -287,44 +288,46 @@
                             annotation.update(pdfrw.PdfDict(V=pdfstr, AS=pdfstr))
                         elif target[ANNOT_FORM_type] == ANNOT_FORM_text:
                             # regular text field
                             target.update( pdfrw.PdfDict( V=data_dict[key], AP=data_dict[key]) )
                             if target[ANNOT_FIELD_KIDS_KEY]:
                                 target[ANNOT_FIELD_KIDS_KEY][0].update( pdfrw.PdfDict( V=data_dict[key], AP=data_dict[key]) )
                 if flatten == True:
-                    annotation.update(pdfrw.PdfDict(Ff=1))
+                    annotation.update(pdfrw.PdfDict(Ff=make_read_only(target["/Ff"])))
     template_pdf.Root.AcroForm.update(pdfrw.PdfDict(NeedAppearances=pdfrw.PdfObject('true')))
     pdfrw.PdfWriter().write(output_pdf_path, template_pdf)
 
 
-def rotate_page(deg, input_pdf_path, output_map_path, page_number):
+def rotate_page(deg, input_pdf_path, output_map_path, page_number, **kwargs):
     """
     Rotate a page within the pdf document.
     Parameters
     ---------
     deg: float
         The x coordinate of the top left corner of the text.
     input_pdf_path: str
         Path to the pdf you want the fields from.
     output_map_path: str
         Path of the new pdf that is generated.
     page_number: float
         Number of the page to get the map of.
+    kwargs: Dict
+        Additional arguments to pass to fitz save method.
     Returns
     ---------
     """
     doc = fitz.open(input_pdf_path)
     page = doc[page_number-1]
     
     page.set_rotation(deg)
         
-    doc.save(output_map_path)
+    doc.save(output_map_path, **kwargs)
 
 
-def place_radiobutton(field_name, x, y, input_pdf_path, output_map_path, page_number, width=10, height=10, font_size=12, font_name=None, fill_color=(0.8,0.8,0.8), font_color=(0,0,0)):
+def place_radiobutton(field_name, x, y, input_pdf_path, output_map_path, page_number, width=10, height=10, font_size=12, font_name=None, fill_color=(0.8,0.8,0.8), font_color=(0,0,0), **kwargs):
     """
     Place a radio box in the pdf document. Use the get_coordinate_map
     function to help with placement.
     Parameters
     ---------
     field_name: str
         The name you want attatched to the field
@@ -347,14 +350,16 @@
     font_name: str
         The name of the font type you are using.
         https://github.com/t-houssian/fillpdf/blob/main/README.md#fonts
     fill_color: tuple
         The color to use (0,0,0) = white, (1,1,1) = black
     font_color: tuple
         The color to use (0,0,0) = white, (1,1,1) = black
+    kwargs: Dict
+        Additional arguments to pass to fitz save method.
     Returns
     ---------
     """
     doc = fitz.open(input_pdf_path)
     page = doc[page_number-1]
     
     widget = fitz.Widget()
@@ -364,18 +369,18 @@
     widget.text_color = font_color
     widget.text_font = font_name
     widget.fill_color = fill_color
     widget.field_name = field_name
     
     page.add_widget(widget)
         
-    doc.save(output_map_path)
+    doc.save(output_map_path, **kwargs)
 
 
-def place_dropdown(field_name, values, x, y, input_pdf_path, output_map_path, page_number, width=10, height=10, font_size=12, font_name=None, fill_color=(0.8,0.8,0.8), font_color=(0,0,0)):
+def place_dropdown(field_name, values, x, y, input_pdf_path, output_map_path, page_number, width=10, height=10, font_size=12, font_name=None, fill_color=(0.8,0.8,0.8), font_color=(0,0,0), **kwargs):
     """
     Place a dropdown box widget in the pdf document. Use the get_coordinate_map
     function to help with placement.
     Parameters
     ---------
     field_name: str
         The name you want attatched to the field
@@ -400,14 +405,16 @@
     font_name: str
         The name of the font type you are using.
         https://github.com/t-houssian/fillpdf/blob/main/README.md#fonts
     fill_color: tuple
         The color to use (0,0,0) = white, (1,1,1) = black
     font_color: tuple
         The color to use (0,0,0) = white, (1,1,1) = black
+    kwargs: Dict
+        Additional arguments to pass to fitz save method.
     Returns
     ---------
     """
     doc = fitz.open(input_pdf_path)
     page = doc[page_number-1]
     widget = fitz.Widget()
     widget.field_name = field_name
@@ -418,18 +425,18 @@
     widget.field_flags = fitz.PDF_CH_FIELD_IS_COMMIT_ON_SEL_CHANGE
     widget.choice_values = values
     widget.rect = fitz.Rect(x, y, x+width, y+height)
     widget.text_fontsize = font_size
     widget.field_value = widget.choice_values[-1]
     page.add_widget(widget)
     
-    doc.save(output_map_path)
+    doc.save(output_map_path, **kwargs)
 
 
-def place_text_box(field_name, prefilled_text, x, y, input_pdf_path, output_map_path, page_number, width=10, height=10, font_size=12, font_name=None, fill_color=(0.8,0.8,0.8), font_color=(0,0,0)):
+def place_text_box(field_name, prefilled_text, x, y, input_pdf_path, output_map_path, page_number, width=10, height=10, font_size=12, font_name=None, fill_color=(0.8,0.8,0.8), font_color=(0,0,0), **kwargs):
     """
     Place a fillable text box widget in the pdf document. Use the get_coordinate_map
     function to help with placement.
     Parameters
     ---------
     field_name: str
         The name you want attatched to the field
@@ -454,14 +461,16 @@
     font_name: str
         The name of the font type you are using.
         https://github.com/t-houssian/fillpdf/blob/main/README.md#fonts
     fill_color: tuple
         The color to use (0,0,0) = white, (1,1,1) = black
     font_color: tuple
         The color to use (0,0,0) = white, (1,1,1) = black
+    kwargs: Dict
+        Additional arguments to pass to fitz save method.
     Returns
     ---------
     """
     doc = fitz.open(input_pdf_path)
     page = doc[page_number-1]
     
     widget = fitz.Widget()
@@ -475,18 +484,18 @@
     widget.field_value = prefilled_text
     widget.field_label = "arbitrary text - e.g. to help filling the field"
     
     page.add_widget(widget)
     field = page.first_widget
     assert field.field_type_string == "Text"
     
-    doc.save(output_map_path)
+    doc.save(output_map_path, **kwargs)
 
 
-def place_image(file_name, x, y, input_pdf_path, output_map_path, page_number, width=10, height=10):
+def place_image(file_name, x, y, input_pdf_path, output_map_path, page_number, width=10, height=10, **kwargs):
     """
     Place image on the pdf document. Use the get_coordinate_map
     function to help with placement.
     Parameters
     ---------
     file_name: str
         The path of the file to be placed in the image
@@ -500,25 +509,27 @@
         Path of the new pdf that is generated.
     page_number: float
         Number of the page to get the map of.
     width: float
         The width of the image
     height: float
         The height of the image
+    kwargs: Dict
+        Additional arguments to pass to fitz save method.
     Returns
     ---------
     """
     doc = fitz.open(input_pdf_path)
     page = doc[page_number-1]
     
     page.insert_image(fitz.Rect(x, y, x+width, y+height), filename=file_name)
-    doc.save(output_map_path)
+    doc.save(output_map_path, **kwargs)
 
 
-def place_text(text, x, y, input_pdf_path, output_map_path, page_number, font_size=12, font_name="helv", color=None):
+def place_text(text, x, y, input_pdf_path, output_map_path, page_number, font_size=12, font_name="helv", color=None, **kwargs):
     """
     Place Text on the pdf document. Use the get_coordinate_map
     function to help with placement.
     Parameters
     ---------
     text: str
         The string you want to be place in the document
@@ -535,35 +546,39 @@
     font_size: float
         Size of the text being inserted.
     font_name: str
         The name of the font type you are using.
         https://github.com/t-houssian/fillpdf/blob/main/README.md#fonts
     color: tuple
         The color to use (0,0,0) = white, (1,1,1) = black
+    kwargs: Dict
+        Additional arguments to pass to fitz save method.
     Returns
     ---------
     """
     doc = fitz.open(input_pdf_path)
     page = doc[page_number-1]
     page.insert_text(fitz.Point(x, y), str(text), fontname=font_name, color=color, fontsize=font_size)
-    doc.save(output_map_path)
+    doc.save(output_map_path, **kwargs)
 
 
-def get_coordinate_map(input_pdf_path, output_map_path, page_number=1):
+def get_coordinate_map(input_pdf_path, output_map_path, page_number=1, **kwargs):
     """
     Creates a map on the pdf page to help in the placement of text, photos,
     and widgets.
     Parameters
     ---------
     input_pdf_path: str
         Path to the pdf you want the fields from.
     output_map_path: str
         Path of the new pdf that is generated.
     page_number: float
         Number of the page to get the map of.
+    kwargs: Dict
+        Additional arguments to pass to fitz save method.
     Returns
     ---------
     A dictionary of form fields and their filled values.
     """
     doc = fitz.open(input_pdf_path)
     page = doc[page_number-1]
     max_x = page.rect[2]
@@ -573,8 +588,8 @@
         page.insert_text(fitz.Point(0 , y), str(y), fontsize=12, fontname="times-bold", color=(1, 0, 0))
         page.draw_line(fitz.Point(0 , y), fitz.Point(max_x , y), color=(1, 0, 0))
         
     for x in range(0, int(math.ceil(max_x / 50.0)) * 50, 50):
         page.insert_text(fitz.Point(x , 12), str(x), fontsize=12, fontname="times-bold", color=(1, 0, 0))
         page.draw_line(fitz.Point(x , 12), fitz.Point(x , max_y), color=(1, 0, 0))
     
-    doc.save(output_map_path)
+    doc.save(output_map_path, **kwargs)
```

### Comparing `fillpdf-0.7.2/fillpdf/insertfillpdf.py` & `fillpdf-0.7.3/fillpdf/insertfillpdf.py`

 * *Files identical despite different names*

### Comparing `fillpdf-0.7.2/fillpdf.egg-info/PKG-INFO` & `fillpdf-0.7.3/fillpdf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: fillpdf
-Version: 0.7.2
+Version: 0.7.3
 Summary: A Library to fill and flatten pdfs
 Home-page: https://github.com/t-houssian/fillpdf
 Author: Tyler Houssian
 Author-email: tylerhoussian@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pdfrw2
+Requires-Dist: pdf2image
+Requires-Dist: Pillow
+Requires-Dist: pymupdf
 
 # fillpdf
 https://pypi.org/project/fillpdf/
 
 # Documentation:
 [View The Documentation](https://fillpdf.readthedocs.io/en/latest/)
 
@@ -56,45 +60,25 @@
 ##### write_fillable_pdf
     write_fillable_pdf(input_pdf_path, output_pdf_path, data_dict, flatten=False)
 - input_pdf_path- path to your pdf you want to alter (including the pdf name could just leave as 'blank.pdf' if the pdf is in your current directory)
 - output_pdf_path- path of where you want your pdf to write to (including the pdf name could just leave as 'new.pdf' to write to current directory)
 - data_dict- dictionary that contains the fields to write to as your key and what to write to it as your value (get this from the get_form_fields function)
 - flatten (default=False)- If True, then the fields will become uneditable when you write to the pdf.
 ###### For Example:
-    data_dict = {'Address # Useful Websites
-
-* [List PDF Fields pdfrw](https://github.com/pmaupin/pdfrw/issues/165)
-* [List PDF Fields](https://stackoverflow.com/questions/3984003/how-to-extract-pdf-fields-from-a-filled-out-form-in-python)
-* [Fill PDF Fields](https://stackoverflow.com/questions/60082481/how-to-edit-checkboxes-and-save-changes-in-an-editable-pdf-using-the-python-pdfr)
-* [Flatten PDFs](https://stackoverflow.com/questions/27023043/generate-flattened-pdf-with-python)
-* [pdfrw2](https://pypi.org/project/pdfrw2/)
-
-# Credit
-- [dvska](https://stackoverflow.com/users/1303068/dvska)
-- [gbroiles](https://github.com/pmaupin/pdfrw/issues/165)
-- [tomatoeshift](https://stackoverflow.com/users/11998874/tomatoeshift)
-- [Tyler Houssian](https://stackoverflow.com/users/13537359/tyler-houssian)
-- [jtplaarj](https://github.com/jtplaarj)
-- [WestHealth](https://github.com/WestHealth/pdf-form-filler)
-- [sarnold](https://github.com/sarnold)
-- [Patrick Maupin](https://github.com/pmaupin)
-
-# Future Work
-* give option to place text by coordinate
-* alter or view pdf versions
-1 Text Box': '500 West Main Street',
+    data_dict = {'Address1 Text Box': '500 West Main Street',
     'Driving License Check Box': 'Yes',
     'Language 1 Check Box': 'Off',}
     
     fillpdfs.write_fillable_pdf('blank.pdf', 'new.pdf', data_dict)
 - For radio boxes ('Off' = not filled, 'Yes' = filled)
 - For check boxes ('Off' or '' = not filled, 'Yes' = filled)
 - For drop downs (Enter the name of the desired drop down option)
 - For radio groups ('0' = The first option, '1' = The second option, '2' = the third option, etc.)
 
+
 ##### flatten_pdf
     flatten_pdf(input_pdf_path, output_pdf_path, as_images=False)
 - input_pdf_path- path to your pdf you want to alter (including the pdf name could just leave as 'blank.pdf' if the pdf is in your current directory)
 - output_pdf_path- path of where you want your pdf to write to (including the pdf name could just leave as 'new.pdf' to write to current directory)
 - as_images=False- Default is False meaning it will update each individual annotation and set
         it to False. True means it will convert to images and then reinsert into the
         pdf. Try this if the first is not working. (this image technique requires poppler.)
```

### Comparing `fillpdf-0.7.2/setup.cfg` & `fillpdf-0.7.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `fillpdf-0.7.2/setup.py` & `fillpdf-0.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,22 @@
     'Pillow',
     'pymupdf'
     ]
 
 setup(
     name='fillpdf',
     packages=find_packages(exclude=['tests']),
-    version='0.7.2',
+    version='0.7.3',
     install_requires=install_requires,
     description='A Library to fill and flatten pdfs',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Tyler Houssian',
     author_email="tylerhoussian@gmail.com",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     url='https://github.com/t-houssian/fillpdf',
-)
+)
```


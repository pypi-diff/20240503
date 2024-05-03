# Comparing `tmp/mailbagit-0.7.1.tar.gz` & `tmp/mailbagit-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailbagit-0.7.1.tar", last modified: Wed Feb  7 20:51:01 2024, max compression
+gzip compressed data, was "mailbagit-0.7.2.tar", last modified: Fri May  3 16:49:26 2024, max compression
```

## Comparing `mailbagit-0.7.1.tar` & `mailbagit-0.7.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-02-07 20:51:01.468746 mailbagit-0.7.1/
--rw-rw-rw-   0        0        0     1145 2022-03-31 19:54:35.000000 mailbagit-0.7.1/LICENSE
--rw-rw-rw-   0        0        0     7359 2024-02-07 20:51:01.467776 mailbagit-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     5857 2024-02-07 20:36:48.000000 mailbagit-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-07 20:51:01.395749 mailbagit-0.7.1/mailbagit/
--rw-rw-rw-   0        0        0    12594 2024-02-07 20:36:48.000000 mailbagit-0.7.1/mailbagit/__init__.py
--rw-rw-rw-   0        0        0    13942 2023-02-14 18:29:58.000000 mailbagit-0.7.1/mailbagit/controller.py
--rw-rw-rw-   0        0        0     3205 2023-01-27 22:21:41.000000 mailbagit-0.7.1/mailbagit/derivative.py
-drwxrwxrwx   0        0        0        0 2024-02-07 20:51:01.429747 mailbagit-0.7.1/mailbagit/derivatives/
--rw-rw-rw-   0        0        0     8658 2023-02-14 18:20:25.000000 mailbagit-0.7.1/mailbagit/derivatives/eml.py
--rw-rw-rw-   0        0        0      914 2023-02-14 18:20:25.000000 mailbagit-0.7.1/mailbagit/derivatives/example.py
--rw-rw-rw-   0        0        0     2773 2023-06-22 15:09:33.000000 mailbagit-0.7.1/mailbagit/derivatives/html.py
--rw-rw-rw-   0        0        0     7945 2023-02-14 18:29:58.000000 mailbagit-0.7.1/mailbagit/derivatives/mbox.py
--rw-rw-rw-   0        0        0     5297 2023-02-14 18:20:25.000000 mailbagit-0.7.1/mailbagit/derivatives/pdf.py
--rw-rw-rw-   0        0        0     4861 2023-02-14 18:20:25.000000 mailbagit-0.7.1/mailbagit/derivatives/pdf_chrome.py
--rw-rw-rw-   0        0        0     2150 2023-02-14 18:20:25.000000 mailbagit-0.7.1/mailbagit/derivatives/txt.py
--rw-rw-rw-   0        0        0    17293 2024-02-07 20:36:48.000000 mailbagit-0.7.1/mailbagit/derivatives/warc.py
--rw-rw-rw-   0        0        0     3136 2023-02-14 18:29:58.000000 mailbagit-0.7.1/mailbagit/email_account.py
-drwxrwxrwx   0        0        0        0 2024-02-07 20:51:01.440746 mailbagit-0.7.1/mailbagit/formats/
--rw-rw-rw-   0        0        0     6989 2023-02-14 18:29:58.000000 mailbagit-0.7.1/mailbagit/formats/eml.py
--rw-rw-rw-   0        0        0      744 2023-02-14 18:29:58.000000 mailbagit-0.7.1/mailbagit/formats/example.py
--rw-rw-rw-   0        0        0     7378 2023-06-15 20:22:51.000000 mailbagit-0.7.1/mailbagit/formats/mbox.py
--rw-rw-rw-   0        0        0    11273 2024-02-07 20:36:48.000000 mailbagit-0.7.1/mailbagit/formats/msg.py
--rw-rw-rw-   0        0        0    20554 2024-02-07 20:36:48.000000 mailbagit-0.7.1/mailbagit/formats/pst.py
--rw-rw-rw-   0        0        0      245 2023-02-14 18:20:25.000000 mailbagit-0.7.1/mailbagit/globals.py
--rw-rw-rw-   0        0        0     9765 2023-02-14 18:29:58.000000 mailbagit-0.7.1/mailbagit/guided.py
-drwxrwxrwx   0        0        0        0 2024-02-07 20:51:01.446746 mailbagit-0.7.1/mailbagit/helper/
--rw-rw-rw-   0        0        0        0 2022-05-25 17:40:41.000000 mailbagit-0.7.1/mailbagit/helper/__init__.py
--rw-rw-rw-   0        0        0     3787 2023-07-25 14:30:15.000000 mailbagit-0.7.1/mailbagit/helper/common.py
--rw-rw-rw-   0        0        0     5606 2024-02-05 21:07:20.000000 mailbagit-0.7.1/mailbagit/helper/controller.py
--rw-rw-rw-   0        0        0     8499 2024-02-07 20:36:48.000000 mailbagit-0.7.1/mailbagit/helper/derivative.py
--rw-rw-rw-   0        0        0    16767 2024-02-07 20:36:48.000000 mailbagit-0.7.1/mailbagit/helper/format.py
--rw-rw-rw-   0        0        0     3888 2023-02-14 18:20:25.000000 mailbagit-0.7.1/mailbagit/loggerx.py
--rw-rw-rw-   0        0        0     6320 2023-02-14 18:20:25.000000 mailbagit-0.7.1/mailbagit/models.py
-drwxrwxrwx   0        0        0        0 2024-02-07 20:51:01.464749 mailbagit-0.7.1/mailbagit.egg-info/
--rw-rw-rw-   0        0        0     7359 2024-02-07 20:51:01.000000 mailbagit-0.7.1/mailbagit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-02-07 20:51:01.000000 mailbagit-0.7.1/mailbagit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-07 20:51:01.000000 mailbagit-0.7.1/mailbagit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2024-02-07 20:51:01.000000 mailbagit-0.7.1/mailbagit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      452 2024-02-07 20:51:01.000000 mailbagit-0.7.1/mailbagit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2024-02-07 20:51:01.000000 mailbagit-0.7.1/mailbagit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       30 2022-05-12 18:35:05.000000 mailbagit-0.7.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-07 20:51:01.468746 mailbagit-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1648 2024-02-07 20:36:48.000000 mailbagit-0.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-07 20:51:01.463746 mailbagit-0.7.1/tests/
--rw-rw-rw-   0        0        0        0 2022-05-12 18:35:05.000000 mailbagit-0.7.1/tests/__init__.py
--rw-rw-rw-   0        0        0     3443 2022-05-16 18:54:07.000000 mailbagit-0.7.1/tests/test_controller.py
--rw-rw-rw-   0        0        0     8452 2023-02-14 18:29:58.000000 mailbagit-0.7.1/tests/test_formats.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:49:26.125853 mailbagit-0.7.2/
+-rw-rw-rw-   0        0        0     1145 2022-03-31 19:54:35.000000 mailbagit-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0     7359 2024-05-03 16:49:26.124884 mailbagit-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5857 2024-02-07 20:36:48.000000 mailbagit-0.7.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 16:49:26.047851 mailbagit-0.7.2/mailbagit/
+-rw-rw-rw-   0        0        0    12594 2024-05-03 16:43:22.000000 mailbagit-0.7.2/mailbagit/__init__.py
+-rw-rw-rw-   0        0        0    13942 2024-04-12 20:58:29.000000 mailbagit-0.7.2/mailbagit/controller.py
+-rw-rw-rw-   0        0        0     3205 2023-01-27 22:21:41.000000 mailbagit-0.7.2/mailbagit/derivative.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:49:26.082855 mailbagit-0.7.2/mailbagit/derivatives/
+-rw-rw-rw-   0        0        0     8658 2023-02-14 18:20:25.000000 mailbagit-0.7.2/mailbagit/derivatives/eml.py
+-rw-rw-rw-   0        0        0      914 2023-02-14 18:20:25.000000 mailbagit-0.7.2/mailbagit/derivatives/example.py
+-rw-rw-rw-   0        0        0     2773 2023-06-22 15:09:33.000000 mailbagit-0.7.2/mailbagit/derivatives/html.py
+-rw-rw-rw-   0        0        0     7945 2023-02-14 18:29:58.000000 mailbagit-0.7.2/mailbagit/derivatives/mbox.py
+-rw-rw-rw-   0        0        0     5297 2023-02-14 18:20:25.000000 mailbagit-0.7.2/mailbagit/derivatives/pdf.py
+-rw-rw-rw-   0        0        0     4876 2024-05-03 16:43:22.000000 mailbagit-0.7.2/mailbagit/derivatives/pdf_chrome.py
+-rw-rw-rw-   0        0        0     2150 2023-02-14 18:20:25.000000 mailbagit-0.7.2/mailbagit/derivatives/txt.py
+-rw-rw-rw-   0        0        0    17293 2024-02-07 20:36:48.000000 mailbagit-0.7.2/mailbagit/derivatives/warc.py
+-rw-rw-rw-   0        0        0     3136 2023-02-14 18:29:58.000000 mailbagit-0.7.2/mailbagit/email_account.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:49:26.096870 mailbagit-0.7.2/mailbagit/formats/
+-rw-rw-rw-   0        0        0     6989 2023-02-14 18:29:58.000000 mailbagit-0.7.2/mailbagit/formats/eml.py
+-rw-rw-rw-   0        0        0      744 2023-02-14 18:29:58.000000 mailbagit-0.7.2/mailbagit/formats/example.py
+-rw-rw-rw-   0        0        0     7378 2023-06-15 20:22:51.000000 mailbagit-0.7.2/mailbagit/formats/mbox.py
+-rw-rw-rw-   0        0        0    11273 2024-02-07 20:36:48.000000 mailbagit-0.7.2/mailbagit/formats/msg.py
+-rw-rw-rw-   0        0        0    21674 2024-05-03 16:43:22.000000 mailbagit-0.7.2/mailbagit/formats/pst.py
+-rw-rw-rw-   0        0        0      245 2023-02-14 18:20:25.000000 mailbagit-0.7.2/mailbagit/globals.py
+-rw-rw-rw-   0        0        0     9765 2023-02-14 18:29:58.000000 mailbagit-0.7.2/mailbagit/guided.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:49:26.102852 mailbagit-0.7.2/mailbagit/helper/
+-rw-rw-rw-   0        0        0        0 2022-05-25 17:40:41.000000 mailbagit-0.7.2/mailbagit/helper/__init__.py
+-rw-rw-rw-   0        0        0     3787 2023-07-25 14:30:15.000000 mailbagit-0.7.2/mailbagit/helper/common.py
+-rw-rw-rw-   0        0        0     5598 2024-05-03 16:43:22.000000 mailbagit-0.7.2/mailbagit/helper/controller.py
+-rw-rw-rw-   0        0        0     8499 2024-05-02 17:39:53.000000 mailbagit-0.7.2/mailbagit/helper/derivative.py
+-rw-rw-rw-   0        0        0    16767 2024-04-12 20:48:24.000000 mailbagit-0.7.2/mailbagit/helper/format.py
+-rw-rw-rw-   0        0        0     3888 2023-02-14 18:20:25.000000 mailbagit-0.7.2/mailbagit/loggerx.py
+-rw-rw-rw-   0        0        0     6320 2023-02-14 18:20:25.000000 mailbagit-0.7.2/mailbagit/models.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:49:26.122859 mailbagit-0.7.2/mailbagit.egg-info/
+-rw-rw-rw-   0        0        0     7359 2024-05-03 16:49:25.000000 mailbagit-0.7.2/mailbagit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-03 16:49:26.000000 mailbagit-0.7.2/mailbagit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 16:49:25.000000 mailbagit-0.7.2/mailbagit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2024-05-03 16:49:25.000000 mailbagit-0.7.2/mailbagit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      452 2024-05-03 16:49:25.000000 mailbagit-0.7.2/mailbagit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2024-05-03 16:49:25.000000 mailbagit-0.7.2/mailbagit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       30 2022-05-12 18:35:05.000000 mailbagit-0.7.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 16:49:26.125853 mailbagit-0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     1648 2024-05-03 16:43:22.000000 mailbagit-0.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:49:26.120853 mailbagit-0.7.2/tests/
+-rw-rw-rw-   0        0        0        0 2022-05-12 18:35:05.000000 mailbagit-0.7.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     3443 2022-05-16 18:54:07.000000 mailbagit-0.7.2/tests/test_controller.py
+-rw-rw-rw-   0        0        0     8452 2023-02-14 18:29:58.000000 mailbagit-0.7.2/tests/test_formats.py
```

### Comparing `mailbagit-0.7.1/LICENSE` & `mailbagit-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/PKG-INFO` & `mailbagit-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailbagit
-Version: 0.7.1
+Version: 0.7.2
 Summary: A tool for preserving email in multiple preservation formats.
 Home-page: https://github.com/UAlbanyArchives/mailbag
 Author: Gregory Wiedeman
 Author-email: gwiedeman@albany.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mailbagit-0.7.1/README.md` & `mailbagit-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit/__init__.py` & `mailbagit-0.7.2/mailbagit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # __init__.py
 
 # Version of the mailbagit package
-__version__ = "0.7.1"
+__version__ = "0.7.2"
 
 import os
 from pathlib import Path
 from bagit import _make_parser, Bag, BagHeaderAction, DEFAULT_CHECKSUMS
 import importlib
 from mailbagit.loggerx import setup_logging, get_logger
 from argparse import ArgumentParser, FileType
```

### Comparing `mailbagit-0.7.1/mailbagit/controller.py` & `mailbagit-0.7.2/mailbagit/controller.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit/derivative.py` & `mailbagit-0.7.2/mailbagit/derivative.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit/derivatives/eml.py` & `mailbagit-0.7.2/mailbagit/derivatives/eml.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit/derivatives/example.py` & `mailbagit-0.7.2/mailbagit/derivatives/example.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit/derivatives/html.py` & `mailbagit-0.7.2/mailbagit/derivatives/html.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit/derivatives/mbox.py` & `mailbagit-0.7.2/mailbagit/derivatives/mbox.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit/derivatives/pdf.py` & `mailbagit-0.7.2/mailbagit/derivatives/pdf.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit/derivatives/pdf_chrome.py` & `mailbagit-0.7.2/mailbagit/derivatives/pdf_chrome.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import mailbagit.helper.derivative as derivative
 import mailbagit.helper.common as common
 
 
 skip_registry = False
 
 try:
-    chromes = ["google-chrome", "chrome.exe", "chrome"]
+    chromes = ["google-chrome", "Google Chrome", "chrome.exe", "chrome"]
     chrome = next((c for c in chromes if distutils.spawn.find_executable(c)), None)
     skip_registry = True if chrome is None else False
 
 except:
     skip_registry = True
 
 log = get_logger()
@@ -68,15 +68,15 @@
                                 write_html.write(html_formatted)
                                 write_html.close()
                             command = [
                                 chrome,
                                 "--headless",
                                 "--run-all-compositor-stages-before-draw",
                                 "--disable-gpu",
-                                "--print-to-pdf-no-header",
+                                "--no-pdf-header-footer",
                                 "--print-to-pdf=" + os.path.abspath(pdf_name),
                                 os.path.abspath(html_name),
                             ]
 
                             # Adds --no-sandbox arg to run as root in docker container if env variable set
                             if os.environ.get("IN_CONTAINER", "").upper() == "TRUE":
                                 command.insert(4, "--no-sandbox")
```

### Comparing `mailbagit-0.7.1/mailbagit/derivatives/txt.py` & `mailbagit-0.7.2/mailbagit/derivatives/txt.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit/derivatives/warc.py` & `mailbagit-0.7.2/mailbagit/derivatives/warc.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit/email_account.py` & `mailbagit-0.7.2/mailbagit/email_account.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit/formats/eml.py` & `mailbagit-0.7.2/mailbagit/formats/eml.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit/formats/example.py` & `mailbagit-0.7.2/mailbagit/formats/example.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit/formats/mbox.py` & `mailbagit-0.7.2/mailbagit/formats/mbox.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit/formats/msg.py` & `mailbagit-0.7.2/mailbagit/formats/msg.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit/formats/pst.py` & `mailbagit-0.7.2/mailbagit/formats/pst.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,38 +41,40 @@
             self.dry_run = args.dry_run
             self.keep = args.keep
             self.mailbag_name = mailbag_name
             self.mailbag_dir = mailbag_dir
             self.source_parent_dir = source_parent_dir
             self.companion_files = args.companion_files
             log.info("Reading: " + self.path)
+            self.count = 0
 
         @property
         def account_data(self):
             return self._account_data
 
         @property
         def number_of_messages(self):
             count = 0
             for _ in self.messages(iteration_only=True):
                 count += 1
             return count
 
-        def folders(self, folder, path, originalFile, errors, iteration_only=False):
+        def folders(self, folder, path, originalFile, iteration_only=False):
             # recursive function that calls itself on any subfolders and
             # returns a generator of messages
             # path is the email folder path of the message, separated by "/"
             if folder.number_of_sub_messages:
                 log.debug("Reading folder: " + folder.name)
                 for index in range(folder.number_of_sub_messages):
 
                     if iteration_only:
                         yield None
                         continue
                     attachments = []
+                    errors = []
                     try:
                         messageObj = folder.get_sub_message(index)
 
                         try:
                             headerParser = email.parser.HeaderParser()
                             if messageObj.transport_headers:
                                 headers = headerParser.parsestr(messageObj.transport_headers)
@@ -120,19 +122,36 @@
                                     # HT to extract_msg for this https://github.com/TeamMsgExtractor/msg-extractor/blob/3cffc2e0d82a0301cfaca2b05c5ef35bfc96a8cb/extract_msg/message_base.py#L958
                                     rtf_body = messageObj.rtf_body
                                     # I dunno why this needs a len of 125 ¯\_(ツ)_/¯
                                     while rtf_body and rtf_body[-1] != 125:
                                         rtf_body = rtf_body[:-1]
                                     # decode it before using DeEncapsulator
                                     rtf_string, html_encoding, errors = format.safely_decode("HTML", rtf_body, encodings, errors)
-                                    deencapsulated_body = DeEncapsulator(rtf_string)
-                                    deencapsulated_body.deencapsulate()
-                                    html_body = deencapsulated_body.html
-                            except:
-                                pass
+
+                                    # Some sort of encoding issue can cause multiple EOF characters which is malformed RTF
+                                    """
+                                    eof_index = rtf_string.find('\x1a')
+                                    self.count += 1
+                                    if eof_index != -1:
+                                        print (rtf_string.count('\x1a'))
+                                    """
+
+                                    try:
+                                        deencapsulated_body = DeEncapsulator(rtf_body)
+                                        deencapsulated_body.deencapsulate()
+                                        html_body, html_encoding, errors = format.safely_decode(
+                                            "HTML", deencapsulated_body.html, encodings, errors
+                                        )
+                                        # html_body = deencapsulated_body.html.decode(html_encoding)
+                                    except Exception as e:
+                                        desc = "Error parsing RTF body"
+                                        errors = common.handle_error(errors, e, desc)
+                            except Exception as e:
+                                desc = "Error parsing HTML or RTF body"
+                                errors = common.handle_error(errors, e, desc)
                             if messageObj.plain_text_body:
                                 encodings[len(encodings.keys()) + 1] = {
                                     "name": "utf-8",
                                     "label": "manual",
                                 }
                                 encodings[len(encodings.keys()) + 2] = {
                                     "name": chardet.detect(messageObj.plain_text_body)["encoding"],
@@ -278,15 +297,15 @@
 
                     yield message
 
             # iterate over any subfolders too
             if folder.number_of_sub_folders:
                 for folder_index in range(folder.number_of_sub_folders):
                     subfolder = folder.get_sub_folder(folder_index)
-                    yield from self.folders(subfolder, path + "/" + subfolder.name, originalFile, errors, iteration_only=iteration_only)
+                    yield from self.folders(subfolder, path + "/" + subfolder.name, originalFile, iteration_only=iteration_only)
             else:
                 if not iteration_only:
                     if not folder.number_of_sub_messages:
                         # This is an email folder that does not contain any messages.
                         # Add it to self.account_data['empty_folder_paths']
                         if not "empty_folder_paths" in self.account_data:
                             self.account_data["empty_folder_paths"] = []
@@ -316,19 +335,18 @@
                 else:
                     originalFile = Path(os.path.normpath(rel_path)).as_posix()
                 # original file is now the relative path to the PST from the provided path
 
                 pst = pypff.file()
                 pst.open(filePath)
                 root = pst.get_root_folder()
-                errors = []
                 for folder in root.sub_folders:
                     if folder.number_of_sub_folders:
                         # call recursive function to parse email folder
-                        yield from self.folders(folder, folder.name, originalFile, errors, iteration_only=iteration_only)
+                        yield from self.folders(folder, folder.name, originalFile, iteration_only=iteration_only)
                     else:
                         if not iteration_only:
                             # This is an email folder that does not contain any messages.
                             # Add it to self.account_data['empty_folder_paths']
                             if not "empty_folder_paths" in self.account_data:
                                 self.account_data["empty_folder_paths"] = []
                             self.account_data["empty_folder_paths"].append(os.path.splitext(originalFile)[0] + "/" + folder.name)
```

### Comparing `mailbagit-0.7.1/mailbagit/guided.py` & `mailbagit-0.7.2/mailbagit/guided.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit/helper/common.py` & `mailbagit-0.7.2/mailbagit/helper/common.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit/helper/controller.py` & `mailbagit-0.7.2/mailbagit/helper/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     for i, attachment in enumerate(message.Attachments):
         if attachment.Name:
             # Need to handle filename conflicts with attachments.csv
             # The format parsers raise a warning about this
             if attachment.Name.lower() == "attachments.csv":
                 writtenName = attachment.WrittenName + os.path.splitext(attachment.Name)[1]
                 desc = ""
-                errors = common.handle_error(errors, None, desc, "warn")
+                errors = common.handle_error([], None, desc, "warn")
             else:
                 writtenName = attachment.WrittenName
             attachment_row = [attachment.Name, writtenName, attachment.MimeType, attachment.Content_ID]
         else:
             # If there is no filename available, just use and integer
             # The format parsers raise an error about this
             writtenName = attachment.WrittenName
@@ -110,15 +110,15 @@
                 f.write(attachment.File)
                 f.close()
             except Exception as e:
                 random_name = "".join(random.choices(string.ascii_letters + string.digits, k=8))
                 desc = (
                     f"Failed to write attachment {attachment.Name} even as normalized name {writtenName}. Instead writing as {random_name}."
                 )
-                errors = common.handle_error(errors, None, desc, "error")
+                errors = common.handle_error([], None, desc, "error")
                 attachment_row = [attachment.Name, random_name, attachment.MimeType, attachment.Content_ID]
                 attachment_path = os.path.join(message_attachments_dir, random_name)
                 f = open(attachment_path, "wb")
                 f.write(attachment.File)
                 f.close()
 
         # add line to CSV for attachment
```

### Comparing `mailbagit-0.7.1/mailbagit/helper/derivative.py` & `mailbagit-0.7.2/mailbagit/helper/derivative.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit/helper/format.py` & `mailbagit-0.7.2/mailbagit/helper/format.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit/loggerx.py` & `mailbagit-0.7.2/mailbagit/loggerx.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit/models.py` & `mailbagit-0.7.2/mailbagit/models.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/mailbagit.egg-info/PKG-INFO` & `mailbagit-0.7.2/mailbagit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailbagit
-Version: 0.7.1
+Version: 0.7.2
 Summary: A tool for preserving email in multiple preservation formats.
 Home-page: https://github.com/UAlbanyArchives/mailbag
 Author: Gregory Wiedeman
 Author-email: gwiedeman@albany.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mailbagit-0.7.1/mailbagit.egg-info/SOURCES.txt` & `mailbagit-0.7.2/mailbagit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/setup.py` & `mailbagit-0.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mailbagit",
-    version="0.7.1",
+    version="0.7.2",
     author="Gregory Wiedeman",
     author_email="gwiedeman@albany.edu",
     description="A tool for preserving email in multiple preservation formats.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/UAlbanyArchives/mailbag",
     packages=setuptools.find_namespace_packages(exclude=("tests")),
```

### Comparing `mailbagit-0.7.1/tests/test_controller.py` & `mailbagit-0.7.2/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.7.1/tests/test_formats.py` & `mailbagit-0.7.2/tests/test_formats.py`

 * *Files identical despite different names*


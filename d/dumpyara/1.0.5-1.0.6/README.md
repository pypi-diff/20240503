# Comparing `tmp/dumpyara-1.0.5.tar.gz` & `tmp/dumpyara-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumpyara-1.0.5.tar", max compression
+gzip compressed data, was "dumpyara-1.0.6.tar", max compression
```

## Comparing `dumpyara-1.0.5.tar` & `dumpyara-1.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1304 2024-04-10 18:38:03.743982 dumpyara-1.0.5/README.md
--rw-r--r--   0        0        0      215 2024-04-13 19:54:43.719360 dumpyara-1.0.5/dumpyara/__init__.py
--rw-r--r--   0        0        0      166 2022-02-24 11:26:29.453827 dumpyara-1.0.5/dumpyara/__main__.py
--rw-r--r--   0        0        0     2273 2024-04-10 10:30:16.574915 dumpyara-1.0.5/dumpyara/dumpyara.py
--rw-r--r--   0        0        0      249 2024-02-22 14:20:03.637781 dumpyara-1.0.5/dumpyara/lib/liberofs/__init__.py
--rw-r--r--   0        0        0     1061 2022-04-13 02:01:29.000000 dumpyara-1.0.5/dumpyara/lib/libpayload/LICENSE
--rw-r--r--   0        0        0     4190 2022-04-13 13:16:39.682675 dumpyara-1.0.5/dumpyara/lib/libpayload/__init__.py
--rw-r--r--   0        0        0     7291 2022-06-29 23:18:10.039907 dumpyara-1.0.5/dumpyara/lib/libpayload/update_metadata_pb2.py
--rw-r--r--   0        0        0     5148 2022-02-25 10:28:46.742568 dumpyara-1.0.5/dumpyara/lib/libsdat2img/__init__.py
--rw-r--r--   0        0        0      336 2024-04-10 10:30:16.614915 dumpyara-1.0.5/dumpyara/lib/libsevenzip/__init__.py
--rw-r--r--   0        0        0     1131 2024-04-13 19:58:24.279471 dumpyara-1.0.5/dumpyara/main.py
--rw-r--r--   0        0        0      112 2023-03-13 23:23:23.165706 dumpyara-1.0.5/dumpyara/steps/__init__.py
--rw-r--r--   0        0        0     1831 2024-04-10 16:48:32.161503 dumpyara-1.0.5/dumpyara/steps/extract_archive.py
--rw-r--r--   0        0        0     1725 2024-04-10 10:30:16.614915 dumpyara-1.0.5/dumpyara/steps/extract_images.py
--rw-r--r--   0        0        0     1622 2024-04-10 16:50:48.741049 dumpyara-1.0.5/dumpyara/steps/prepare_images.py
--rw-r--r--   0        0        0      961 2024-02-22 14:38:13.604100 dumpyara-1.0.5/dumpyara/utils/bootimg.py
--rw-r--r--   0        0        0     1137 2023-03-13 23:30:07.843483 dumpyara-1.0.5/dumpyara/utils/files.py
--rw-r--r--   0        0        0     1107 2024-04-10 18:32:49.324963 dumpyara-1.0.5/dumpyara/utils/multipartitions.py
--rw-r--r--   0        0        0     4957 2024-04-10 18:29:47.692186 dumpyara-1.0.5/dumpyara/utils/partitions.py
--rw-r--r--   0        0        0     2257 2024-04-10 18:35:00.421223 dumpyara-1.0.5/dumpyara/utils/raw_image.py
--rw-r--r--   0        0        0      696 2024-04-10 15:32:58.328024 dumpyara-1.0.5/dumpyara/utils/shutil.py
--rw-r--r--   0        0        0     1100 2023-03-13 23:55:49.868282 dumpyara-1.0.5/dumpyara/utils/sparsed_images.py
--rw-r--r--   0        0        0      597 2024-04-13 19:54:40.169358 dumpyara-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     2289 1970-01-01 00:00:00.000000 dumpyara-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1304 2024-05-02 14:07:31.448264 dumpyara-1.0.6/README.md
+-rw-r--r--   0        0        0      215 2024-05-03 10:52:19.330425 dumpyara-1.0.6/dumpyara/__init__.py
+-rw-r--r--   0        0        0      166 2024-02-23 13:42:11.844459 dumpyara-1.0.6/dumpyara/__main__.py
+-rw-r--r--   0        0        0     2273 2024-05-02 14:07:31.448264 dumpyara-1.0.6/dumpyara/dumpyara.py
+-rw-r--r--   0        0        0      249 2024-02-23 13:42:11.844459 dumpyara-1.0.6/dumpyara/lib/liberofs/__init__.py
+-rw-r--r--   0        0        0     1061 2024-02-23 13:42:11.844459 dumpyara-1.0.6/dumpyara/lib/libpayload/LICENSE
+-rw-r--r--   0        0        0     4190 2024-02-23 13:42:11.844459 dumpyara-1.0.6/dumpyara/lib/libpayload/__init__.py
+-rw-r--r--   0        0        0     7291 2024-02-23 13:42:11.847792 dumpyara-1.0.6/dumpyara/lib/libpayload/update_metadata_pb2.py
+-rw-r--r--   0        0        0     5148 2024-02-23 13:42:11.847792 dumpyara-1.0.6/dumpyara/lib/libsdat2img/__init__.py
+-rw-r--r--   0        0        0      336 2024-05-02 14:07:31.448264 dumpyara-1.0.6/dumpyara/lib/libsevenzip/__init__.py
+-rw-r--r--   0        0        0     1131 2024-05-02 14:07:31.448264 dumpyara-1.0.6/dumpyara/main.py
+-rw-r--r--   0        0        0      112 2024-02-23 13:42:11.847792 dumpyara-1.0.6/dumpyara/steps/__init__.py
+-rw-r--r--   0        0        0     1831 2024-05-02 14:07:31.448264 dumpyara-1.0.6/dumpyara/steps/extract_archive.py
+-rw-r--r--   0        0        0     1725 2024-05-02 14:07:31.451597 dumpyara-1.0.6/dumpyara/steps/extract_images.py
+-rw-r--r--   0        0        0     1622 2024-05-02 14:07:31.451597 dumpyara-1.0.6/dumpyara/steps/prepare_images.py
+-rw-r--r--   0        0        0      987 2024-05-02 14:32:26.307433 dumpyara-1.0.6/dumpyara/utils/bootimg.py
+-rw-r--r--   0        0        0     1137 2024-02-23 13:42:11.847792 dumpyara-1.0.6/dumpyara/utils/files.py
+-rw-r--r--   0        0        0     1107 2024-05-02 14:07:31.451597 dumpyara-1.0.6/dumpyara/utils/multipartitions.py
+-rw-r--r--   0        0        0     4957 2024-02-23 13:42:11.847792 dumpyara-1.0.6/dumpyara/utils/partitions.py
+-rw-r--r--   0        0        0     2257 2024-05-02 14:07:31.451597 dumpyara-1.0.6/dumpyara/utils/raw_image.py
+-rw-r--r--   0        0        0      696 2024-05-02 14:07:31.451597 dumpyara-1.0.6/dumpyara/utils/shutil.py
+-rw-r--r--   0        0        0     1100 2024-02-23 13:42:11.847792 dumpyara-1.0.6/dumpyara/utils/sparsed_images.py
+-rw-r--r--   0        0        0      597 2024-05-03 10:52:13.653658 dumpyara-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2289 1970-01-01 00:00:00.000000 dumpyara-1.0.6/PKG-INFO
```

### Comparing `dumpyara-1.0.5/README.md` & `dumpyara-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.5/dumpyara/dumpyara.py` & `dumpyara-1.0.6/dumpyara/dumpyara.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.5/dumpyara/lib/libpayload/LICENSE` & `dumpyara-1.0.6/dumpyara/lib/libpayload/LICENSE`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.5/dumpyara/lib/libpayload/__init__.py` & `dumpyara-1.0.6/dumpyara/lib/libpayload/__init__.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.5/dumpyara/lib/libpayload/update_metadata_pb2.py` & `dumpyara-1.0.6/dumpyara/lib/libpayload/update_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.5/dumpyara/lib/libsdat2img/__init__.py` & `dumpyara-1.0.6/dumpyara/lib/libsdat2img/__init__.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.5/dumpyara/main.py` & `dumpyara-1.0.6/dumpyara/main.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.5/dumpyara/steps/extract_archive.py` & `dumpyara-1.0.6/dumpyara/steps/extract_archive.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.5/dumpyara/steps/extract_images.py` & `dumpyara-1.0.6/dumpyara/steps/extract_images.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.5/dumpyara/steps/prepare_images.py` & `dumpyara-1.0.6/dumpyara/steps/prepare_images.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.5/dumpyara/utils/bootimg.py` & `dumpyara-1.0.6/dumpyara/utils/bootimg.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 # Copyright (C) 2022 Dumpyara Project
 #
 # SPDX-License-Identifier: GPL-3.0
 #
 
-from distutils.dir_util import copy_tree
 from pathlib import Path
+from sebaubuntu_libs.libcompat.distutils.dir_util import copy_tree
 from sebaubuntu_libs.libaik import AIKManager
 
 def extract_bootimg(file: Path, output_path: Path):
 	aik_manager = AIKManager()
 
 	image_info = aik_manager.unpackimg(file, ignore_ramdisk_errors=True)
```

### Comparing `dumpyara-1.0.5/dumpyara/utils/files.py` & `dumpyara-1.0.6/dumpyara/utils/files.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.5/dumpyara/utils/multipartitions.py` & `dumpyara-1.0.6/dumpyara/utils/multipartitions.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.5/dumpyara/utils/partitions.py` & `dumpyara-1.0.6/dumpyara/utils/partitions.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.5/dumpyara/utils/raw_image.py` & `dumpyara-1.0.6/dumpyara/utils/raw_image.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.5/dumpyara/utils/shutil.py` & `dumpyara-1.0.6/dumpyara/utils/shutil.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.5/dumpyara/utils/sparsed_images.py` & `dumpyara-1.0.6/dumpyara/utils/sparsed_images.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.5/pyproject.toml` & `dumpyara-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "dumpyara"
-version = "1.0.5"
+version = "1.0.6"
 description = "Android firmware extractor"
 authors = ["Sebastiano Barezzi <seba@sebaubuntu.dev>"]
 license = "GPL-3.0"
 readme = "README.md"
 repository = "https://github.com/sebaubuntu-python/dumpyara"
 
 [tool.poetry.scripts]
 dumpyara = 'dumpyara.main:main'
 
 [tool.poetry.dependencies]
 python = "^3.8"
 Brotli = "^1.0.9"
 protobuf = ">=4.22.1,<6.0.0"
-sebaubuntu-libs = "^1.4.2"
+sebaubuntu-libs = "^1.4.4"
 liblp = "^1.0.2"
 py7zr = "^0.21.0"
 lz4 = "^4.3.3"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
```

### Comparing `dumpyara-1.0.5/PKG-INFO` & `dumpyara-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dumpyara
-Version: 1.0.5
+Version: 1.0.6
 Summary: Android firmware extractor
 Home-page: https://github.com/sebaubuntu-python/dumpyara
 License: GPL-3.0
 Author: Sebastiano Barezzi
 Author-email: seba@sebaubuntu.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Brotli (>=1.0.9,<2.0.0)
 Requires-Dist: liblp (>=1.0.2,<2.0.0)
 Requires-Dist: lz4 (>=4.3.3,<5.0.0)
 Requires-Dist: protobuf (>=4.22.1,<6.0.0)
 Requires-Dist: py7zr (>=0.21.0,<0.22.0)
-Requires-Dist: sebaubuntu-libs (>=1.4.2,<2.0.0)
+Requires-Dist: sebaubuntu-libs (>=1.4.4,<2.0.0)
 Project-URL: Repository, https://github.com/sebaubuntu-python/dumpyara
 Description-Content-Type: text/markdown
 
 # dumpyara
 
 [![PyPI version](https://img.shields.io/pypi/v/dumpyara)](https://pypi.org/project/dumpyara/)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/85d2c39edbed4dc38f680db01f7b83af)](https://www.codacy.com/gh/sebaubuntu-python/dumpyara/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=sebaubuntu-python/dumpyara&amp;utm_campaign=Badge_Grade)
```


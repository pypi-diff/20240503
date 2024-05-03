# Comparing `tmp/streamlit_datatables_net-0.0.3-py3-none-any.whl.zip` & `tmp/streamlit_datatables_net-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 770708 bytes, number of entries: 12
--rw-r--r--  2.0 unx     4820 b- defN 24-May-03 13:46 streamlit_datatables_net/__init__.py
--rw-r--r--  2.0 unx      369 b- defN 24-May-03 13:46 streamlit_datatables_net/frontend/build/asset-manifest.json
--rw-r--r--  2.0 unx      502 b- defN 24-May-03 13:46 streamlit_datatables_net/frontend/build/index.html
--rw-r--r--  2.0 unx    23791 b- defN 24-May-03 13:46 streamlit_datatables_net/frontend/build/static/css/main.7cdd006b.css
--rw-r--r--  2.0 unx    34601 b- defN 24-May-03 13:46 streamlit_datatables_net/frontend/build/static/css/main.7cdd006b.css.map
--rw-r--r--  2.0 unx   516885 b- defN 24-May-03 13:46 streamlit_datatables_net/frontend/build/static/js/main.b8fdd4b1.js
--rw-r--r--  2.0 unx     1733 b- defN 24-May-03 13:46 streamlit_datatables_net/frontend/build/static/js/main.b8fdd4b1.js.LICENSE.txt
--rw-r--r--  2.0 unx  2295954 b- defN 24-May-03 13:46 streamlit_datatables_net/frontend/build/static/js/main.b8fdd4b1.js.map
--rw-r--r--  2.0 unx      694 b- defN 24-May-03 13:46 streamlit_datatables_net-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-03 13:46 streamlit_datatables_net-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 24-May-03 13:46 streamlit_datatables_net-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1325 b- defN 24-May-03 13:46 streamlit_datatables_net-0.0.3.dist-info/RECORD
-12 files, 2880791 bytes uncompressed, 768384 bytes compressed:  73.3%
+Zip file size: 770683 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     4783 b- defN 24-May-03 14:16 streamlit_datatables_net/__init__.py
+-rw-r--r--  2.0 unx      374 b- defN 24-May-03 14:16 streamlit_datatables_net/frontend/build/asset-manifest.json
+-rw-r--r--  2.0 unx      504 b- defN 24-May-03 14:16 streamlit_datatables_net/frontend/build/index.html
+-rw-r--r--  2.0 unx    23791 b- defN 24-May-03 14:16 streamlit_datatables_net/frontend/build/static/css/main.7cdd006b.css
+-rw-r--r--  2.0 unx    34601 b- defN 24-May-03 14:16 streamlit_datatables_net/frontend/build/static/css/main.7cdd006b.css.map
+-rw-r--r--  2.0 unx   516885 b- defN 24-May-03 14:16 streamlit_datatables_net/frontend/build/static/js/main.b8fdd4b1.js
+-rw-r--r--  2.0 unx     1733 b- defN 24-May-03 14:16 streamlit_datatables_net/frontend/build/static/js/main.b8fdd4b1.js.LICENSE.txt
+-rw-r--r--  2.0 unx  2295954 b- defN 24-May-03 14:16 streamlit_datatables_net/frontend/build/static/js/main.b8fdd4b1.js.map
+-rw-r--r--  2.0 unx      694 b- defN 24-May-03 14:16 streamlit_datatables_net-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-03 14:16 streamlit_datatables_net-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       25 b- defN 24-May-03 14:16 streamlit_datatables_net-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1325 b- defN 24-May-03 14:16 streamlit_datatables_net-0.0.4.dist-info/RECORD
+12 files, 2880761 bytes uncompressed, 768359 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: streamlit_datatables_net/frontend/build/static/js/main.b8fdd4b1.js.LICENSE.txt
 Comment: 
 
 Filename: streamlit_datatables_net/frontend/build/static/js/main.b8fdd4b1.js.map
 Comment: 
 
-Filename: streamlit_datatables_net-0.0.3.dist-info/METADATA
+Filename: streamlit_datatables_net-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: streamlit_datatables_net-0.0.3.dist-info/WHEEL
+Filename: streamlit_datatables_net-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: streamlit_datatables_net-0.0.3.dist-info/top_level.txt
+Filename: streamlit_datatables_net-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: streamlit_datatables_net-0.0.3.dist-info/RECORD
+Filename: streamlit_datatables_net-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamlit_datatables_net/__init__.py

```diff
@@ -1,17 +1,13 @@
 import os
 import streamlit.components.v1 as components
 import streamlit as st
 import json
 from typing import List, Dict
 
-
-st.set_page_config(layout="wide")
-
-
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
 # release process.)
 _RELEASE = True
 
 # Declare a Streamlit component. `declare_component` returns a function
```

## streamlit_datatables_net/frontend/build/asset-manifest.json

### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'files'": "{'main.css': './static/css/main.7cdd006b.css', 'main.js': "*

 * *            "'./static/js/main.b8fdd4b1.js', 'index.html': './index.html', "*

 * *            "'main.7cdd006b.css.map': './static/css/main.7cdd006b.css.map', "*

 * *            "'main.b8fdd4b1.js.map': './static/js/main.b8fdd4b1.js.map'}"}*

```diff
@@ -1,13 +1,13 @@
 {
     "entrypoints": [
         "static/css/main.7cdd006b.css",
         "static/js/main.b8fdd4b1.js"
     ],
     "files": {
-        "index.html": "/index.html",
-        "main.7cdd006b.css.map": "/static/css/main.7cdd006b.css.map",
-        "main.b8fdd4b1.js.map": "/static/js/main.b8fdd4b1.js.map",
-        "main.css": "/static/css/main.7cdd006b.css",
-        "main.js": "/static/js/main.b8fdd4b1.js"
+        "index.html": "./index.html",
+        "main.7cdd006b.css.map": "./static/css/main.7cdd006b.css.map",
+        "main.b8fdd4b1.js.map": "./static/js/main.b8fdd4b1.js.map",
+        "main.css": "./static/css/main.7cdd006b.css",
+        "main.js": "./static/js/main.b8fdd4b1.js"
     }
 }
```

## streamlit_datatables_net/frontend/build/index.html

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><script defer="defer" src="/static/js/main.b8fdd4b1.js"></script><link href="/static/css/main.7cdd006b.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><script defer="defer" src="./static/js/main.b8fdd4b1.js"></script><link href="./static/css/main.7cdd006b.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

## Comparing `streamlit_datatables_net-0.0.3.dist-info/METADATA` & `streamlit_datatables_net-0.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-datatables-net
-Version: 0.0.3
+Version: 0.0.4
 Summary: Streamlit component for Datatables.net
 Home-page: 
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit >=0.63
 Provides-Extra: devel
 Requires-Dist: wheel ; extra == 'devel'
```

## Comparing `streamlit_datatables_net-0.0.3.dist-info/RECORD` & `streamlit_datatables_net-0.0.4.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-streamlit_datatables_net/__init__.py,sha256=Pr1toX0ZmivG2Y3LhNop0Vv_9kizH7l_7-ddrKTqp6M,4820
-streamlit_datatables_net/frontend/build/asset-manifest.json,sha256=GkIqP0RMdhJ6JAhwm4uT2VXGasjF6CfzhYcMmAxC-o8,369
-streamlit_datatables_net/frontend/build/index.html,sha256=OekrlIwh1TSjfX1yh_g8a57xelcpMTYfhxPWgSmt8MY,502
+streamlit_datatables_net/__init__.py,sha256=hH_pS3gWuUAj0-F0VjzAipvWEdtMEpVv9Nqqqc8P_Rw,4783
+streamlit_datatables_net/frontend/build/asset-manifest.json,sha256=yIt9d_kB4IQfSOMzvSlXLW0Vv_Ap4EOTVJUW3_9j71E,374
+streamlit_datatables_net/frontend/build/index.html,sha256=uuW167i2vyd_q5tBJR5t9OVYUeAjB--7gF-uHVwEip4,504
 streamlit_datatables_net/frontend/build/static/css/main.7cdd006b.css,sha256=6Mh2TajVmR6bWdtr3nnbxvg03PIzCSzZrH-2lt7GrEI,23791
 streamlit_datatables_net/frontend/build/static/css/main.7cdd006b.css.map,sha256=zbvlyIMi4EeiobsDb1fFIaM2OPFqmpR2Jot8mGZGCWs,34601
 streamlit_datatables_net/frontend/build/static/js/main.b8fdd4b1.js,sha256=tACNyZAD8Nxjo4iXa168D7VSUywczHMyo4rHTttgyVk,516885
 streamlit_datatables_net/frontend/build/static/js/main.b8fdd4b1.js.LICENSE.txt,sha256=bTYq7VRKyl-jTmYxV2CI1g581D7g1ceDjgZlhyqrkyI,1733
 streamlit_datatables_net/frontend/build/static/js/main.b8fdd4b1.js.map,sha256=Hvw89sumAzKztlSNKsEFhG2MwDinHiZLUk717A_75WU,2295954
-streamlit_datatables_net-0.0.3.dist-info/METADATA,sha256=QTPtZTxfSRoiQ9OkUceoZDsIXJ-QQuyudjqgucW-KrQ,694
-streamlit_datatables_net-0.0.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-streamlit_datatables_net-0.0.3.dist-info/top_level.txt,sha256=Juuw4Qlrxc1-5dsiE0hd5oJipjTUgbBY7WriIvID17A,25
-streamlit_datatables_net-0.0.3.dist-info/RECORD,,
+streamlit_datatables_net-0.0.4.dist-info/METADATA,sha256=EgaqegtCNK0cUEdKBSx01Z60faEGiM_XQfehFPnjCw4,694
+streamlit_datatables_net-0.0.4.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+streamlit_datatables_net-0.0.4.dist-info/top_level.txt,sha256=Juuw4Qlrxc1-5dsiE0hd5oJipjTUgbBY7WriIvID17A,25
+streamlit_datatables_net-0.0.4.dist-info/RECORD,,
```


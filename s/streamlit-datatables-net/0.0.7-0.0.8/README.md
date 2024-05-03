# Comparing `tmp/streamlit_datatables_net-0.0.7-py3-none-any.whl.zip` & `tmp/streamlit_datatables_net-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 771888 bytes, number of entries: 12
--rw-r--r--  2.0 unx     5213 b- defN 24-May-03 20:42 streamlit_datatables_net/__init__.py
--rw-r--r--  2.0 unx      374 b- defN 24-May-03 20:42 streamlit_datatables_net/frontend/build/asset-manifest.json
--rw-r--r--  2.0 unx      521 b- defN 24-May-03 20:42 streamlit_datatables_net/frontend/build/index.html
--rw-r--r--  2.0 unx    23791 b- defN 24-May-03 20:42 streamlit_datatables_net/frontend/build/static/css/main.7cdd006b.css
--rw-r--r--  2.0 unx    34601 b- defN 24-May-03 20:42 streamlit_datatables_net/frontend/build/static/css/main.7cdd006b.css.map
--rw-r--r--  2.0 unx   517718 b- defN 24-May-03 20:42 streamlit_datatables_net/frontend/build/static/js/main.28784b13.js
--rw-r--r--  2.0 unx     1733 b- defN 24-May-03 20:42 streamlit_datatables_net/frontend/build/static/js/main.28784b13.js.LICENSE.txt
--rw-r--r--  2.0 unx  2299006 b- defN 24-May-03 20:42 streamlit_datatables_net/frontend/build/static/js/main.28784b13.js.map
--rw-r--r--  2.0 unx      694 b- defN 24-May-03 20:42 streamlit_datatables_net-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-03 20:42 streamlit_datatables_net-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 24-May-03 20:42 streamlit_datatables_net-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1325 b- defN 24-May-03 20:42 streamlit_datatables_net-0.0.7.dist-info/RECORD
-12 files, 2885093 bytes uncompressed, 769564 bytes compressed:  73.3%
+Zip file size: 771890 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     5214 b- defN 24-May-03 20:48 streamlit_datatables_net/__init__.py
+-rw-r--r--  2.0 unx      374 b- defN 24-May-03 20:48 streamlit_datatables_net/frontend/build/asset-manifest.json
+-rw-r--r--  2.0 unx      521 b- defN 24-May-03 20:48 streamlit_datatables_net/frontend/build/index.html
+-rw-r--r--  2.0 unx    23791 b- defN 24-May-03 20:48 streamlit_datatables_net/frontend/build/static/css/main.7cdd006b.css
+-rw-r--r--  2.0 unx    34601 b- defN 24-May-03 20:48 streamlit_datatables_net/frontend/build/static/css/main.7cdd006b.css.map
+-rw-r--r--  2.0 unx   517718 b- defN 24-May-03 20:48 streamlit_datatables_net/frontend/build/static/js/main.28784b13.js
+-rw-r--r--  2.0 unx     1733 b- defN 24-May-03 20:48 streamlit_datatables_net/frontend/build/static/js/main.28784b13.js.LICENSE.txt
+-rw-r--r--  2.0 unx  2299006 b- defN 24-May-03 20:48 streamlit_datatables_net/frontend/build/static/js/main.28784b13.js.map
+-rw-r--r--  2.0 unx      694 b- defN 24-May-03 20:48 streamlit_datatables_net-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-03 20:48 streamlit_datatables_net-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       25 b- defN 24-May-03 20:48 streamlit_datatables_net-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1325 b- defN 24-May-03 20:48 streamlit_datatables_net-0.0.8.dist-info/RECORD
+12 files, 2885094 bytes uncompressed, 769566 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: streamlit_datatables_net/frontend/build/static/js/main.28784b13.js.LICENSE.txt
 Comment: 
 
 Filename: streamlit_datatables_net/frontend/build/static/js/main.28784b13.js.map
 Comment: 
 
-Filename: streamlit_datatables_net-0.0.7.dist-info/METADATA
+Filename: streamlit_datatables_net-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: streamlit_datatables_net-0.0.7.dist-info/WHEEL
+Filename: streamlit_datatables_net-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: streamlit_datatables_net-0.0.7.dist-info/top_level.txt
+Filename: streamlit_datatables_net-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: streamlit_datatables_net-0.0.7.dist-info/RECORD
+Filename: streamlit_datatables_net-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamlit_datatables_net/__init__.py

```diff
@@ -71,15 +71,15 @@
     # Call through to our private component function. Arguments we pass here
     # will be sent to the frontend, where they'll be available in an "args"
     # dictionary.
     #
     # "default" is a special argument that specifies the initial return
     # value of the component before the user has interacted with it.
     component_value = _component_func(
-        props=props, table_id=table_id, class_name=class_name, stylesheets=stylesheets, key=key, default=0)
+        props=props, table_id=table_id, class_name=class_name, stylesheets=stylesheets, key=key, default={})
 
     # We could modify the value returned from the component if we wanted.
     # There's no need to do this in our simple example - but it's an option.
     return component_value
 
 
 if not _RELEASE:
```

## Comparing `streamlit_datatables_net-0.0.7.dist-info/METADATA` & `streamlit_datatables_net-0.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-datatables-net
-Version: 0.0.7
+Version: 0.0.8
 Summary: Streamlit component for Datatables.net
 Home-page: 
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit >=0.63
 Provides-Extra: devel
 Requires-Dist: wheel ; extra == 'devel'
```

## Comparing `streamlit_datatables_net-0.0.7.dist-info/RECORD` & `streamlit_datatables_net-0.0.8.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-streamlit_datatables_net/__init__.py,sha256=bhE9cgkYoz7MKDSeWNq694LnLCqgmU8Za1CM9-akZik,5213
+streamlit_datatables_net/__init__.py,sha256=dzbx0dW3pkdTQNI3H4FVmEI3NLXSPApiBGXBhH-HAu8,5214
 streamlit_datatables_net/frontend/build/asset-manifest.json,sha256=XW5sg1SLE_u7W34MjwLNnNN5ZC_0DPNtkZItPARcBmo,374
 streamlit_datatables_net/frontend/build/index.html,sha256=lsov8LV3nsrjtoYO1Gq_fCUxm1pb7K_wL_EyHpzKiyo,521
 streamlit_datatables_net/frontend/build/static/css/main.7cdd006b.css,sha256=6Mh2TajVmR6bWdtr3nnbxvg03PIzCSzZrH-2lt7GrEI,23791
 streamlit_datatables_net/frontend/build/static/css/main.7cdd006b.css.map,sha256=zbvlyIMi4EeiobsDb1fFIaM2OPFqmpR2Jot8mGZGCWs,34601
 streamlit_datatables_net/frontend/build/static/js/main.28784b13.js,sha256=2TuBFn2dugboI7SFmdm9jqXbQM483TP70uwPL22J2G4,517718
 streamlit_datatables_net/frontend/build/static/js/main.28784b13.js.LICENSE.txt,sha256=bTYq7VRKyl-jTmYxV2CI1g581D7g1ceDjgZlhyqrkyI,1733
 streamlit_datatables_net/frontend/build/static/js/main.28784b13.js.map,sha256=ZVq8JBtWwjRWjNhGFXh403Vhmzf051VUwgJLFxcULlQ,2299006
-streamlit_datatables_net-0.0.7.dist-info/METADATA,sha256=jOiDAWNsi_7snWYTrqsAGIRT2lLwP62HrypjCaWJp_k,694
-streamlit_datatables_net-0.0.7.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-streamlit_datatables_net-0.0.7.dist-info/top_level.txt,sha256=Juuw4Qlrxc1-5dsiE0hd5oJipjTUgbBY7WriIvID17A,25
-streamlit_datatables_net-0.0.7.dist-info/RECORD,,
+streamlit_datatables_net-0.0.8.dist-info/METADATA,sha256=_ki7IsVtC_oasv2hCnbl-xCH9Za3rnxi3ghMYQc4PYE,694
+streamlit_datatables_net-0.0.8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+streamlit_datatables_net-0.0.8.dist-info/top_level.txt,sha256=Juuw4Qlrxc1-5dsiE0hd5oJipjTUgbBY7WriIvID17A,25
+streamlit_datatables_net-0.0.8.dist-info/RECORD,,
```


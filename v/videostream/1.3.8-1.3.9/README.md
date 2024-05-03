# Comparing `tmp/videostream-1.3.8-py3-none-any.whl.zip` & `tmp/videostream-1.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 13601 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      425 b- defN 23-Aug-16 19:51 deepview/videostream/__init__.py
--rw-rw-r--  2.0 unx     2849 b- defN 23-Aug-16 19:51 deepview/videostream/client.py
--rw-rw-r--  2.0 unx     7029 b- defN 23-Aug-16 19:51 deepview/videostream/frame.py
--rw-rw-r--  2.0 unx     3500 b- defN 23-Aug-16 19:51 deepview/videostream/host.py
--rw-rw-r--  2.0 unx     6744 b- defN 23-Aug-16 19:51 deepview/videostream/library.py
--rw-rw-r--  2.0 unx    11710 b- defN 23-Aug-16 19:54 videostream-1.3.8.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      243 b- defN 23-Aug-16 19:54 videostream-1.3.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Aug-16 19:54 videostream-1.3.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Aug-16 19:54 videostream-1.3.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      843 b- defN 23-Aug-16 19:54 videostream-1.3.8.dist-info/RECORD
-10 files, 33444 bytes uncompressed, 12153 bytes compressed:  63.7%
+Zip file size: 13600 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx      425 b- defN 23-Oct-23 17:13 deepview/videostream/__init__.py
+-rw-rw-r--  2.0 unx     2849 b- defN 23-Oct-23 17:13 deepview/videostream/client.py
+-rw-rw-r--  2.0 unx     7029 b- defN 23-Oct-23 17:13 deepview/videostream/frame.py
+-rw-rw-r--  2.0 unx     3500 b- defN 23-Oct-23 17:13 deepview/videostream/host.py
+-rw-rw-r--  2.0 unx     6744 b- defN 23-Oct-23 17:13 deepview/videostream/library.py
+-rw-rw-r--  2.0 unx    11710 b- defN 23-Oct-23 17:16 videostream-1.3.9.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      243 b- defN 23-Oct-23 17:16 videostream-1.3.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Oct-23 17:16 videostream-1.3.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Oct-23 17:16 videostream-1.3.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      843 b- defN 23-Oct-23 17:16 videostream-1.3.9.dist-info/RECORD
+10 files, 33444 bytes uncompressed, 12152 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: deepview/videostream/host.py
 Comment: 
 
 Filename: deepview/videostream/library.py
 Comment: 
 
-Filename: videostream-1.3.8.dist-info/LICENSE.txt
+Filename: videostream-1.3.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: videostream-1.3.8.dist-info/METADATA
+Filename: videostream-1.3.9.dist-info/METADATA
 Comment: 
 
-Filename: videostream-1.3.8.dist-info/WHEEL
+Filename: videostream-1.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: videostream-1.3.8.dist-info/top_level.txt
+Filename: videostream-1.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: videostream-1.3.8.dist-info/RECORD
+Filename: videostream-1.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `videostream-1.3.8.dist-info/LICENSE.txt` & `videostream-1.3.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `videostream-1.3.8.dist-info/RECORD` & `videostream-1.3.9.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 deepview/videostream/__init__.py,sha256=z2TPx9-OdcG0xyIluZjzuXZoYGtx2kv4pCnYel0uCoU,425
 deepview/videostream/client.py,sha256=SAKJ5FkmBU7LyTSzaRR37VHssoqfdzvuI54AzYuTr6Y,2849
 deepview/videostream/frame.py,sha256=xrXa7FqauvkcytvIJK4njTUxz4ssDICNptQk3breDns,7029
 deepview/videostream/host.py,sha256=Oc_u3ZQUd6VBmB-IiZS4_yGin4jxIUeCG4q9n4inhU4,3500
 deepview/videostream/library.py,sha256=sSFoWZtztFDez8F-b-3rYxIMIzNwpI72zmgkW1VvV2Q,6744
-videostream-1.3.8.dist-info/LICENSE.txt,sha256=tRF0H4BBjc7hxfxRe2Y573C-tye_wJQBFdZu_wG_rLQ,11710
-videostream-1.3.8.dist-info/METADATA,sha256=HLtjdFLUKUm_TC7Mi_w2Px1ePhkmLZnEkO0oT-cssrM,243
-videostream-1.3.8.dist-info/WHEEL,sha256=nvhOrkn7_9sGzJjxuUFjoJ6OkO7SJJqHSjq9VNu0Elc,92
-videostream-1.3.8.dist-info/top_level.txt,sha256=FZ_uj5ZExs9dTNq5lw196yb-XR3VHKi6vS0EWgTQtXk,9
-videostream-1.3.8.dist-info/RECORD,,
+videostream-1.3.9.dist-info/LICENSE.txt,sha256=tRF0H4BBjc7hxfxRe2Y573C-tye_wJQBFdZu_wG_rLQ,11710
+videostream-1.3.9.dist-info/METADATA,sha256=iSXEAf-nkMz0frGlyAg-_acHmaqLme19m9TGjBZ8CPU,243
+videostream-1.3.9.dist-info/WHEEL,sha256=nvhOrkn7_9sGzJjxuUFjoJ6OkO7SJJqHSjq9VNu0Elc,92
+videostream-1.3.9.dist-info/top_level.txt,sha256=FZ_uj5ZExs9dTNq5lw196yb-XR3VHKi6vS0EWgTQtXk,9
+videostream-1.3.9.dist-info/RECORD,,
```


# Comparing `tmp/lyrpy-2024.0.2.tar.gz` & `tmp/lyrpy-2024.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyrpy-2024.0.2.tar", last modified: Fri May  3 11:21:20 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


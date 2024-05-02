# Comparing `tmp/aladdinsdk-0.0.1a3.post0.tar.gz` & `tmp/aladdinsdk-0.0.1a4.post0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aladdinsdk-0.0.1a3.post0.tar", last modified: Wed Apr 24 18:50:23 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


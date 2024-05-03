# Comparing `tmp/badkeys-0.0.8.tar.gz` & `tmp/badkeys-0.0.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badkeys-0.0.8.tar", last modified: Fri Apr 26 13:22:35 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


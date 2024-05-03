# Comparing `tmp/arolla-0.0.0.tar.gz` & `tmp/arolla-0.0.0.post1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arolla-0.0.0.tar", last modified: Sat Mar  9 11:33:09 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


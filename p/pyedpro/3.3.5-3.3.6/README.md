# Comparing `tmp/pyedpro-3.3.5.tar.gz` & `tmp/pyedpro-3.3.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyedpro-3.3.5.tar", last modified: Wed Apr 10 06:50:43 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


# Comparing `tmp/pedantic-2.1.4.tar.gz` & `tmp/pedantic-2.1.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pedantic-2.1.4.tar", last modified: Sat Dec 30 07:43:39 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


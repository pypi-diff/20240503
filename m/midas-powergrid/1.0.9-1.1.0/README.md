# Comparing `tmp/midas-powergrid-1.0.9.tar.gz` & `tmp/midas_powergrid-1.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midas-powergrid-1.0.9.tar", last modified: Thu Aug 11 10:40:03 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


# Comparing `tmp/sbot-1.1.1.tar.gz` & `tmp/sbot-1.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbot-1.1.1.tar", last modified: Sun Aug  6 16:08:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


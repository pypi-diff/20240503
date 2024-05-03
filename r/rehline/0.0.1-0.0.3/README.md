# Comparing `tmp/rehline-0.0.1.tar.gz` & `tmp/rehline-0.0.3-pp310-pypy310_pp73-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rehline-0.0.1.tar", last modified: Wed Oct 18 08:32:28 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


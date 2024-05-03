# Comparing `tmp/lusid_sdk-2.1.81.tar.gz` & `tmp/lusid_sdk-2.1.86-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_sdk-2.1.81.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


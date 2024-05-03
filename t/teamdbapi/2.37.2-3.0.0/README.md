# Comparing `tmp/teamdbapi-2.37.2.tar.gz` & `tmp/teamdbapi-3.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teamdbapi-2.37.2.tar", last modified: Wed Oct 18 11:02:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


# Comparing `tmp/pokernow-0.5.8.tar.gz` & `tmp/pokernow-0.5.9.win-amd64.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokernow-0.5.8.tar", last modified: Thu May  2 23:52:29 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


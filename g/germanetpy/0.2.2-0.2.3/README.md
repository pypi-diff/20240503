# Comparing `tmp/germanetpy-0.2.2.tar.gz` & `tmp/germanetpy-0.2.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/bcmpbell/Documents/germanetpy/dist/tmp42n_ds6t/germanetpy-0.2.2.tar", last modified: Fri May  6 13:55:11 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


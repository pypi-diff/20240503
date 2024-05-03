# Comparing `tmp/pychomp2-1.0.2.tar.gz` & `tmp/pychomp2-1.0.3-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychomp2-1.0.2.tar", last modified: Mon Mar 25 00:19:03 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


# Comparing `tmp/botocore-a-la-carte-iot1click-devices-1.34.96.tar.gz` & `tmp/botocore_a_la_carte_iot1click_devices-1.34.97-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-iot1click-devices-1.34.96.tar", last modified: Thu May  2 01:01:20 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


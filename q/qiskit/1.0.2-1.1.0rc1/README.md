# Comparing `tmp/qiskit-1.0.2.tar.gz` & `tmp/qiskit-1.1.0rc1-cp38-abi3-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-1.0.2.tar", last modified: Thu Mar  7 23:06:07 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


# Comparing `tmp/conversion_utils-0.1.0.tar.gz` & `tmp/conversion_utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conversion_utils-0.1.0.tar", max compression
+gzip compressed data, was "conversion_utils-0.1.1.tar", max compression
```

## Comparing `conversion_utils-0.1.0.tar` & `conversion_utils-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-05-03 02:03:14.438799 conversion_utils-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-03 02:03:14.438799 conversion_utils-0.1.0/conversion_utils/__init__.py
--rw-r--r--   0        0        0      845 2024-05-03 02:51:47.193121 conversion_utils-0.1.0/conversion_utils/conversion.py
--rw-r--r--   0        0        0      311 2024-05-03 02:55:25.355485 conversion_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      455 1970-01-01 00:00:00.000000 conversion_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-03 02:03:14.438799 conversion_utils-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 02:03:14.438799 conversion_utils-0.1.1/conversion_utils/__init__.py
+-rw-r--r--   0        0        0      696 2024-05-03 03:34:10.820099 conversion_utils-0.1.1/conversion_utils/conversion.py
+-rw-r--r--   0        0        0      311 2024-05-03 03:34:38.252346 conversion_utils-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      455 1970-01-01 00:00:00.000000 conversion_utils-0.1.1/PKG-INFO
```


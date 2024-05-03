# Comparing `tmp/release_action_testing-0.1.0.tar.gz` & `tmp/release_action_testing-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "release_action_testing-0.1.0.tar", max compression
+gzip compressed data, was "release_action_testing-0.2.0.tar", max compression
```

## Comparing `release_action_testing-0.1.0.tar` & `release_action_testing-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       41 2024-05-03 03:38:15.350284 release_action_testing-0.1.0/README.md
--rw-r--r--   0        0        0      310 2024-05-03 03:38:15.350284 release_action_testing-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-03 03:38:15.350284 release_action_testing-0.1.0/release_action_testing/__init__.py
--rw-r--r--   0        0        0       65 2024-05-03 03:38:15.350284 release_action_testing-0.1.0/release_action_testing/bruh.py
--rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 release_action_testing-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       41 2024-05-03 03:47:01.162416 release_action_testing-0.2.0/README.md
+-rw-r--r--   0        0        0      310 2024-05-03 03:47:01.162416 release_action_testing-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-03 03:47:01.162416 release_action_testing-0.2.0/release_action_testing/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-03 03:47:01.162416 release_action_testing-0.2.0/release_action_testing/bruh.py
+-rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 release_action_testing-0.2.0/PKG-INFO
```


# Comparing `tmp/rosa_python_client-1.0.87.tar.gz` & `tmp/rosa_python_client-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosa_python_client-1.0.87.tar", max compression
+gzip compressed data, was "rosa_python_client-1.0.9.tar", max compression
```

## Comparing `rosa_python_client-1.0.87.tar` & `rosa_python_client-1.0.9.tar`

### file list

```diff
@@ -1,9 +1,5 @@
--rw-r--r--   0        0        0      865 2024-05-03 21:24:54.698247 rosa_python_client-1.0.87/README.md
--rw-r--r--   0        0        0     1412 2024-05-03 21:24:59.369216 rosa_python_client-1.0.87/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-03 21:24:54.699247 rosa_python_client-1.0.87/rosa/__init__.py
--rw-r--r--   0        0        0    11119 2024-05-03 21:24:54.699247 rosa_python_client-1.0.87/rosa/cli.py
--rw-r--r--   0        0        0        0 2024-05-03 21:24:54.699247 rosa_python_client-1.0.87/rosa/tests/__init__.py
--rw-r--r--   0        0        0      843 2024-05-03 21:24:54.699247 rosa_python_client-1.0.87/rosa/tests/conftest.py
--rw-r--r--   0        0        0       30 2024-05-03 21:24:54.699247 rosa_python_client-1.0.87/rosa/tests/const.py
--rw-r--r--   0        0        0     1031 2024-05-03 21:24:54.700247 rosa_python_client-1.0.87/rosa/tests/test_parse_command.py
--rw-r--r--   0        0        0     2033 1970-01-01 00:00:00.000000 rosa_python_client-1.0.87/PKG-INFO
+-rw-r--r--   0        0        0      511 2023-06-14 13:03:12.785023 rosa_python_client-1.0.9/README.md
+-rw-r--r--   0        0        0      353 2023-06-14 13:03:12.785023 rosa_python_client-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-14 13:03:12.785023 rosa_python_client-1.0.9/rosa/__init__.py
+-rw-r--r--   0        0        0     8586 2023-06-14 13:03:12.785023 rosa_python_client-1.0.9/rosa/cli.py
+-rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 rosa_python_client-1.0.9/PKG-INFO
```


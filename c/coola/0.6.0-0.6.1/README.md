# Comparing `tmp/coola-0.6.0.tar.gz` & `tmp/coola-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coola-0.6.0.tar", max compression
+gzip compressed data, was "coola-0.6.1.tar", max compression
```

## Comparing `coola-0.6.0.tar` & `coola-0.6.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1501 2024-04-02 04:09:13.904312 coola-0.6.0/LICENSE
--rw-r--r--   0        0        0    11161 2024-04-02 04:09:13.904312 coola-0.6.0/README.md
--rw-r--r--   0        0        0     6864 2024-04-02 04:09:13.904312 coola-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      553 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/__init__.py
--rw-r--r--   0        0        0     3628 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/comparison.py
--rw-r--r--   0        0        0      266 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/__init__.py
--rw-r--r--   0        0        0     1935 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/__init__.py
--rw-r--r--   0        0        0     2426 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/base.py
--rw-r--r--   0        0        0     4122 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/collection.py
--rw-r--r--   0        0        0     2123 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/default.py
--rw-r--r--   0        0        0     2998 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/jax_.py
--rw-r--r--   0        0        0     4481 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/numpy_.py
--rw-r--r--   0        0        0     4208 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/pandas_.py
--rw-r--r--   0        0        0     4262 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/polars_.py
--rw-r--r--   0        0        0     2130 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/scalar.py
--rw-r--r--   0        0        0     4631 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/torch_.py
--rw-r--r--   0        0        0     1493 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/utils.py
--rw-r--r--   0        0        0     6502 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/xarray_.py
--rw-r--r--   0        0        0      488 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/config.py
--rw-r--r--   0        0        0     2074 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/__init__.py
--rw-r--r--   0        0        0     4973 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/base.py
--rw-r--r--   0        0        0     2098 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/data.py
--rw-r--r--   0        0        0     2256 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/dtype.py
--rw-r--r--   0        0        0     2849 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/equal.py
--rw-r--r--   0        0        0     2827 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/jax_.py
--rw-r--r--   0        0        0     3820 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/mapping.py
--rw-r--r--   0        0        0     9512 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/native.py
--rw-r--r--   0        0        0     2790 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/numpy_.py
--rw-r--r--   0        0        0     5624 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/pandas_.py
--rw-r--r--   0        0        0     6173 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/polars_.py
--rw-r--r--   0        0        0     3630 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/scalar.py
--rw-r--r--   0        0        0     2129 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/sequence.py
--rw-r--r--   0        0        0     2306 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/shape.py
--rw-r--r--   0        0        0     4186 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/torch_.py
--rw-r--r--   0        0        0      319 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/testers/__init__.py
--rw-r--r--   0        0        0     1348 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/testers/base.py
--rw-r--r--   0        0        0     9794 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/testers/default.py
--rw-r--r--   0        0        0      502 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/formatters/__init__.py
--rw-r--r--   0        0        0     3485 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/formatters/base.py
--rw-r--r--   0        0        0    11668 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/formatters/default.py
--rw-r--r--   0        0        0     3543 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/formatters/numpy_.py
--rw-r--r--   0        0        0     3577 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/formatters/torch_.py
--rw-r--r--   0        0        0      445 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/nested/__init__.py
--rw-r--r--   0        0        0     1780 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/nested/conversion.py
--rw-r--r--   0        0        0     4100 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/nested/mapping.py
--rw-r--r--   0        0        0      875 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/random/__init__.py
--rw-r--r--   0        0        0     1822 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/random/base.py
--rw-r--r--   0        0        0     5605 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/random/default.py
--rw-r--r--   0        0        0     1397 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/random/functional.py
--rw-r--r--   0        0        0     2858 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/random/numpy_.py
--rw-r--r--   0        0        0     1363 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/random/random_.py
--rw-r--r--   0        0        0     2953 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/random/torch_.py
--rw-r--r--   0        0        0      826 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/random/utils.py
--rw-r--r--   0        0        0      555 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/reducers/__init__.py
--rw-r--r--   0        0        0     8056 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/reducers/base.py
--rw-r--r--   0        0        0     1605 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/reducers/native.py
--rw-r--r--   0        0        0     2381 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/reducers/numpy_.py
--rw-r--r--   0        0        0     2802 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/reducers/registry.py
--rw-r--r--   0        0        0     2441 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/reducers/torch_.py
--rw-r--r--   0        0        0      909 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/reducers/utils.py
--rw-r--r--   0        0        0     1722 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/reduction.py
--rw-r--r--   0        0        0     1535 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/summarization.py
--rw-r--r--   0        0        0      322 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/summarizers/__init__.py
--rw-r--r--   0        0        0     2983 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/summarizers/base.py
--rw-r--r--   0        0        0    12758 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/summarizers/summarizer.py
--rw-r--r--   0        0        0     1302 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/testing.py
--rw-r--r--   0        0        0      573 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/types.py
--rw-r--r--   0        0        0      871 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/utils/__init__.py
--rw-r--r--   0        0        0     1189 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/utils/array.py
--rw-r--r--   0        0        0     5837 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/utils/format.py
--rw-r--r--   0        0        0    11275 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/utils/imports.py
--rw-r--r--   0        0        0     1070 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/utils/stats.py
--rw-r--r--   0        0        0     2632 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/utils/tensor.py
--rw-r--r--   0        0        0    12656 1970-01-01 00:00:00.000000 coola-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1501 2024-05-03 18:19:02.044378 coola-0.6.1/LICENSE
+-rw-r--r--   0        0        0    11649 2024-05-03 18:19:02.044378 coola-0.6.1/README.md
+-rw-r--r--   0        0        0     6990 2024-05-03 18:19:02.044378 coola-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      553 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/__init__.py
+-rw-r--r--   0        0        0     3628 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/comparison.py
+-rw-r--r--   0        0        0      266 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/equality/__init__.py
+-rw-r--r--   0        0        0     1935 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/equality/comparators/__init__.py
+-rw-r--r--   0        0        0     2426 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/equality/comparators/base.py
+-rw-r--r--   0        0        0     4122 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/equality/comparators/collection.py
+-rw-r--r--   0        0        0     2123 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/equality/comparators/default.py
+-rw-r--r--   0        0        0     2998 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/equality/comparators/jax_.py
+-rw-r--r--   0        0        0     4481 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/equality/comparators/numpy_.py
+-rw-r--r--   0        0        0     4208 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/equality/comparators/pandas_.py
+-rw-r--r--   0        0        0     4262 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/equality/comparators/polars_.py
+-rw-r--r--   0        0        0     2130 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/equality/comparators/scalar.py
+-rw-r--r--   0        0        0     4631 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/equality/comparators/torch_.py
+-rw-r--r--   0        0        0     1493 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/equality/comparators/utils.py
+-rw-r--r--   0        0        0     6502 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/equality/comparators/xarray_.py
+-rw-r--r--   0        0        0      488 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/equality/config.py
+-rw-r--r--   0        0        0     2074 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/equality/handlers/__init__.py
+-rw-r--r--   0        0        0     4973 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/equality/handlers/base.py
+-rw-r--r--   0        0        0     2098 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/equality/handlers/data.py
+-rw-r--r--   0        0        0     2256 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/equality/handlers/dtype.py
+-rw-r--r--   0        0        0     2849 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/equality/handlers/equal.py
+-rw-r--r--   0        0        0     2827 2024-05-03 18:19:02.044378 coola-0.6.1/src/coola/equality/handlers/jax_.py
+-rw-r--r--   0        0        0     3820 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/equality/handlers/mapping.py
+-rw-r--r--   0        0        0     9512 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/equality/handlers/native.py
+-rw-r--r--   0        0        0     3850 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/equality/handlers/numpy_.py
+-rw-r--r--   0        0        0     5624 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/equality/handlers/pandas_.py
+-rw-r--r--   0        0        0     6173 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/equality/handlers/polars_.py
+-rw-r--r--   0        0        0     3630 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/equality/handlers/scalar.py
+-rw-r--r--   0        0        0     2129 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/equality/handlers/sequence.py
+-rw-r--r--   0        0        0     2306 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/equality/handlers/shape.py
+-rw-r--r--   0        0        0     4186 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/equality/handlers/torch_.py
+-rw-r--r--   0        0        0      319 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/equality/testers/__init__.py
+-rw-r--r--   0        0        0     1348 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/equality/testers/base.py
+-rw-r--r--   0        0        0     9794 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/equality/testers/default.py
+-rw-r--r--   0        0        0      502 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/formatters/__init__.py
+-rw-r--r--   0        0        0     3485 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/formatters/base.py
+-rw-r--r--   0        0        0    11668 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/formatters/default.py
+-rw-r--r--   0        0        0     3543 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/formatters/numpy_.py
+-rw-r--r--   0        0        0     3577 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/formatters/torch_.py
+-rw-r--r--   0        0        0      445 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/nested/__init__.py
+-rw-r--r--   0        0        0     1780 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/nested/conversion.py
+-rw-r--r--   0        0        0     4100 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/nested/mapping.py
+-rw-r--r--   0        0        0      875 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/random/__init__.py
+-rw-r--r--   0        0        0     1822 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/random/base.py
+-rw-r--r--   0        0        0     5605 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/random/default.py
+-rw-r--r--   0        0        0     1397 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/random/functional.py
+-rw-r--r--   0        0        0     2858 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/random/numpy_.py
+-rw-r--r--   0        0        0     1363 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/random/random_.py
+-rw-r--r--   0        0        0     2953 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/random/torch_.py
+-rw-r--r--   0        0        0      826 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/random/utils.py
+-rw-r--r--   0        0        0      555 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/reducers/__init__.py
+-rw-r--r--   0        0        0     8056 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/reducers/base.py
+-rw-r--r--   0        0        0     1605 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/reducers/native.py
+-rw-r--r--   0        0        0     2381 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/reducers/numpy_.py
+-rw-r--r--   0        0        0     2802 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/reducers/registry.py
+-rw-r--r--   0        0        0     2441 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/reducers/torch_.py
+-rw-r--r--   0        0        0      909 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/reducers/utils.py
+-rw-r--r--   0        0        0     1722 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/reduction.py
+-rw-r--r--   0        0        0     1535 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/summarization.py
+-rw-r--r--   0        0        0      322 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/summarizers/__init__.py
+-rw-r--r--   0        0        0     2983 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/summarizers/base.py
+-rw-r--r--   0        0        0    12758 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/summarizers/summarizer.py
+-rw-r--r--   0        0        0     1302 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/testing.py
+-rw-r--r--   0        0        0      573 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/types.py
+-rw-r--r--   0        0        0      871 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/utils/__init__.py
+-rw-r--r--   0        0        0     1189 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/utils/array.py
+-rw-r--r--   0        0        0     5837 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/utils/format.py
+-rw-r--r--   0        0        0    11275 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/utils/imports.py
+-rw-r--r--   0        0        0     1070 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/utils/stats.py
+-rw-r--r--   0        0        0     2632 2024-05-03 18:19:02.048378 coola-0.6.1/src/coola/utils/tensor.py
+-rw-r--r--   0        0        0    13261 1970-01-01 00:00:00.000000 coola-0.6.1/PKG-INFO
```

### Comparing `coola-0.6.0/LICENSE` & `coola-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/README.md` & `coola-0.6.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -158,29 +158,32 @@
 
 Please check the [get started page](https://durandtibo.github.io/coola/get_started) to see how to
 install only some specific dependencies or other alternatives to install the library.
 The following is the corresponding `coola` versions and tested dependencies.
 
 | `coola` | `jax`<sup>*</sup> | `numpy`<sup>*</sup> | `pandas`<sup>*</sup> | `polars`<sup>*</sup> | `torch`<sup>*</sup> | `xarray`<sup>*</sup> | `python`      |
 |---------|-------------------|---------------------|----------------------|----------------------|---------------------|----------------------|---------------|
-| `main`  | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
+| `main`  | `>=0.4.1,<1.0`    | `>=1.21,<2.0`       | `>=1.3,<3.0`         | `>=0.18.3,<1.0`      | `>=1.10,<3.0`       | `>=2023.1`           | `>=3.9,<3.13` |
+| `0.6.1` | `>=0.4.1,<1.0`    | `>=1.21,<2.0`       | `>=1.3,<3.0`         | `>=0.18.3,<1.0`      | `>=1.10,<3.0`       | `>=2023.1`           | `>=3.9,<3.13` |
+| `0.6.0` | `>=0.4.1,<1.0`    | `>=1.21,<2.0`       | `>=1.3,<3.0`         | `>=0.18.3,<1.0`      | `>=1.10,<3.0`       | `>=2023.1`           | `>=3.9,<3.13` |
+| `0.5.0` | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
 | `0.4.0` | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
-| `0.3.1` | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
-| `0.3.0` | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
-| `0.2.2` | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
-| `0.2.1` | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
-| `0.2.0` | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
 
 <sup>*</sup> indicates an optional dependency
 
 <details>
     <summary>older versions</summary>
 
 | `coola`  | `jax`<sup>*</sup> | `numpy`<sup>*</sup> | `pandas`<sup>*</sup> | `polars`<sup>*</sup> | `torch`<sup>*</sup> | `xarray`<sup>*</sup> | `python`      |
 |----------|-------------------|---------------------|----------------------|----------------------|---------------------|----------------------|---------------|
+| `0.3.1`  | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
+| `0.3.0`  | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
+| `0.2.2`  | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
+| `0.2.1`  | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
+| `0.2.0`  | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
 | `0.1.2`  | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<0.21`     | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
 | `0.1.1`  | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<0.20`     | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
 | `0.1.0`  | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<0.20`     | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.12` |
 | `0.0.26` | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<0.20`     | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.12` |
 | `0.0.25` | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<0.20`     | `>=1.10,<2.2`       | `>=2023.4,<2023.11`  | `>=3.9,<3.12` |
 | `0.0.24` | `>=0.3,<0.5`      | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<0.20`     | `>=1.10,<2.2`       | `>=2023.3,<2023.9`   | `>=3.9,<3.12` |
 | `0.0.23` | `>=0.3,<0.5`      | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<0.20`     | `>=1.10,<2.1`       | `>=2023.3,<2023.9`   | `>=3.9,<3.12` |
```

#### html2text {}

```diff
@@ -57,32 +57,37 @@
 install coola[all] ``` Please check the [get started page](https://
 durandtibo.github.io/coola/get_started) to see how to install only some
 specific dependencies or other alternatives to install the library. The
 following is the corresponding `coola` versions and tested dependencies. |
 `coola` | `jax`* | `numpy`* | `pandas`* | `polars`* | `torch`* | `xarray`* |
 `python` | |---------|-------------------|---------------------|---------------
 -------|----------------------|---------------------|----------------------|---
-------------| | `main` | `>=0.4.1,<0.5` | `>=1.21,<1.27` | `>=1.3,<2.2` |
-`>=0.18.3,<1.0` | `>=1.10,<2.2` | `>=2023.1,<2023.13` | `>=3.9,<3.13` | |
-`0.4.0` | `>=0.4.1,<0.5` | `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` |
-`>=1.10,<2.2` | `>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.3.1` |
-`>=0.4.1,<0.5` | `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` |
-`>=1.10,<2.2` | `>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.3.0` |
-`>=0.4.1,<0.5` | `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` |
-`>=1.10,<2.2` | `>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.2.2` |
-`>=0.4.1,<0.5` | `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` |
-`>=1.10,<2.2` | `>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.2.1` |
-`>=0.4.1,<0.5` | `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` |
-`>=1.10,<2.2` | `>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.2.0` |
+------------| | `main` | `>=0.4.1,<1.0` | `>=1.21,<2.0` | `>=1.3,<3.0` |
+`>=0.18.3,<1.0` | `>=1.10,<3.0` | `>=2023.1` | `>=3.9,<3.13` | | `0.6.1` |
+`>=0.4.1,<1.0` | `>=1.21,<2.0` | `>=1.3,<3.0` | `>=0.18.3,<1.0` | `>=1.10,<3.0`
+| `>=2023.1` | `>=3.9,<3.13` | | `0.6.0` | `>=0.4.1,<1.0` | `>=1.21,<2.0` |
+`>=1.3,<3.0` | `>=0.18.3,<1.0` | `>=1.10,<3.0` | `>=2023.1` | `>=3.9,<3.13` | |
+`0.5.0` | `>=0.4.1,<0.5` | `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` |
+`>=1.10,<2.2` | `>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.4.0` |
 `>=0.4.1,<0.5` | `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` |
 `>=1.10,<2.2` | `>=2023.1,<2023.13` | `>=3.9,<3.13` | * indicates an optional
 dependency older versions | `coola` | `jax`* | `numpy`* | `pandas`* | `polars`*
 | `torch`* | `xarray`* | `python` | |----------|-------------------|-----------
 ----------|----------------------|----------------------|---------------------
-|----------------------|---------------| | `0.1.2` | `>=0.4.1,<0.5` |
+|----------------------|---------------| | `0.3.1` | `>=0.4.1,<0.5` |
+`>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` | `>=1.10,<2.2` |
+`>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.3.0` | `>=0.4.1,<0.5` |
+`>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` | `>=1.10,<2.2` |
+`>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.2.2` | `>=0.4.1,<0.5` |
+`>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` | `>=1.10,<2.2` |
+`>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.2.1` | `>=0.4.1,<0.5` |
+`>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` | `>=1.10,<2.2` |
+`>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.2.0` | `>=0.4.1,<0.5` |
+`>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` | `>=1.10,<2.2` |
+`>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.1.2` | `>=0.4.1,<0.5` |
 `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<0.21` | `>=1.10,<2.2` |
 `>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.1.1` | `>=0.4.1,<0.5` |
 `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<0.20` | `>=1.10,<2.2` |
 `>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.1.0` | `>=0.4.1,<0.5` |
 `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<0.20` | `>=1.10,<2.2` |
 `>=2023.1,<2023.13` | `>=3.9,<3.12` | | `0.0.26` | `>=0.4.1,<0.5` |
 `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<0.20` | `>=1.10,<2.2` |
```

### Comparing `coola-0.6.0/pyproject.toml` & `coola-0.6.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coola"
-version = "0.6.0"
+version = "0.6.1"
 description = "A library to check if two complex/nested objects are equal or not"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/coola"
 repository = "https://github.com/durandtibo/coola"
 keywords = [
     "complex/nested objects",
@@ -44,38 +44,41 @@
 # Optional dependencies
 jax = { version = ">=0.4.1,<1.0", optional = true }
 jaxlib = { version = ">=0.4.1,<1.0", optional = true }
 numpy = { version = ">=1.21,<2.0", optional = true }
 pandas = { version = ">=1.3,<3.0", optional = true }
 # polars: 0.18.3 is the minimal version because of https://github.com/pola-rs/polars/issues/9358
 polars = { version = ">=0.18.3,<1.0", optional = true }
-torch = { version = ">=1.10,<3.0", optional = true }
+torch = [
+    { version = ">=1.10,<2.3", optional = true, markers="sys_platform == 'darwin' and platform_machine != 'arm64'" },
+    { version = ">=1.10,<3.0", optional = true }
+]
 xarray = { version = ">=2023.1", optional = true }
 
 [tool.poetry.extras]
 all = ["jax", "jaxlib", "numpy", "pandas", "polars", "torch", "xarray"]
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-mike = "^2.0"
+mike = "^2.1"
 mkdocs-material = "^9.5"
-mkdocstrings = { extras = ["python"], version = "^0.24" }
+mkdocstrings = { extras = ["python"], version = "^0.25" }
 
 [tool.poetry.group.dev.dependencies]
-black = ">=24.3"
-coverage = { extras = ["toml"], version = "^7.4" }
+black = ">=24.4"
+coverage = { extras = ["toml"], version = "^7.5" }
 docformatter = { extras = ["tomli"], version = "^1.7" }
 pre-commit = "^3.7"
 pygments = "^2.17"
-pytest = "^8.1"
+pytest = "^8.2"
 pytest-cov = "^5.0"
 pytest-timeout = "^2.3"
-ruff = ">=0.3.0,<1.0"
+ruff = ">=0.4.0,<1.0"
 xdoctest = "^1.1"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `coola-0.6.0/src/coola/__init__.py` & `coola-0.6.1/src/coola/__init__.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/comparison.py` & `coola-0.6.1/src/coola/comparison.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/comparators/__init__.py` & `coola-0.6.1/src/coola/equality/comparators/__init__.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/comparators/base.py` & `coola-0.6.1/src/coola/equality/comparators/base.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/comparators/collection.py` & `coola-0.6.1/src/coola/equality/comparators/collection.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/comparators/default.py` & `coola-0.6.1/src/coola/equality/comparators/default.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/comparators/jax_.py` & `coola-0.6.1/src/coola/equality/comparators/jax_.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/comparators/numpy_.py` & `coola-0.6.1/src/coola/equality/comparators/numpy_.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/comparators/pandas_.py` & `coola-0.6.1/src/coola/equality/comparators/pandas_.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/comparators/polars_.py` & `coola-0.6.1/src/coola/equality/comparators/polars_.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/comparators/scalar.py` & `coola-0.6.1/src/coola/equality/comparators/scalar.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/comparators/torch_.py` & `coola-0.6.1/src/coola/equality/comparators/torch_.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/comparators/utils.py` & `coola-0.6.1/src/coola/equality/comparators/utils.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/comparators/xarray_.py` & `coola-0.6.1/src/coola/equality/comparators/xarray_.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/handlers/__init__.py` & `coola-0.6.1/src/coola/equality/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/handlers/base.py` & `coola-0.6.1/src/coola/equality/handlers/base.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/handlers/data.py` & `coola-0.6.1/src/coola/equality/handlers/data.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/handlers/dtype.py` & `coola-0.6.1/src/coola/equality/handlers/dtype.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/handlers/equal.py` & `coola-0.6.1/src/coola/equality/handlers/equal.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/handlers/jax_.py` & `coola-0.6.1/src/coola/equality/handlers/jax_.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/handlers/mapping.py` & `coola-0.6.1/src/coola/equality/handlers/mapping.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/handlers/native.py` & `coola-0.6.1/src/coola/equality/handlers/native.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/handlers/numpy_.py` & `coola-0.6.1/src/coola/equality/handlers/numpy_.py`

 * *Files 26% similar despite different names*

```diff
@@ -76,15 +76,56 @@
 
     Args:
         array1: Specifies the first array to compare.
         array2: Specifies the second array to compare.
         config: Specifies the equality configuration.
 
     Returns:
-        ``True``if the two arrays are equal within a tolerance,
+        ``True` `if the two arrays are equal within a tolerance,
             otherwise ``False``.
+
+    Example usage:
+
+    ```pycon
+
+    >>> import numpy as np
+    >>> from coola.equality import EqualityConfig
+    >>> from coola.equality.handlers.numpy_ import array_equal
+    >>> from coola.equality.testers import EqualityTester
+    >>> config = EqualityConfig(tester=EqualityTester())
+    >>> array_equal(np.ones((2, 3)), np.ones((2, 3)), config)
+    True
+    >>> array_equal(np.ones((2, 3)), np.zeros((2, 3)), config)
+    False
+
+    ```
     """
-    if config.atol > 0 or config.rtol > 0:
+    if (config.atol > 0 or config.rtol > 0) and is_numeric_array(array1):
         return np.allclose(
             array1, array2, rtol=config.rtol, atol=config.atol, equal_nan=config.equal_nan
         )
     return np.array_equal(array1, array2, equal_nan=config.equal_nan)
+
+
+def is_numeric_array(array: np.ndarray) -> bool:
+    r"""Indicate if the input array is a numeric array or not.
+
+    Args:
+        array: The input array.
+
+    Returns:
+        ``True`` if the input array is a numeric array, otherwise ``False``.
+
+    Example usage:
+
+    ```pycon
+
+    >>> import numpy as np
+    >>> from coola.equality.handlers.numpy_ import is_numeric_array
+    >>> is_numeric_array(np.ones((2, 3)))
+    True
+    >>> is_numeric_array(np.array(["polar", "bear", "meow"]))
+    False
+
+    ```
+    """
+    return array.dtype.kind in {"?", "b", "B", "i", "u", "f", "c"}
```

### Comparing `coola-0.6.0/src/coola/equality/handlers/pandas_.py` & `coola-0.6.1/src/coola/equality/handlers/pandas_.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/handlers/polars_.py` & `coola-0.6.1/src/coola/equality/handlers/polars_.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/handlers/scalar.py` & `coola-0.6.1/src/coola/equality/handlers/scalar.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/handlers/sequence.py` & `coola-0.6.1/src/coola/equality/handlers/sequence.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/handlers/shape.py` & `coola-0.6.1/src/coola/equality/handlers/shape.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/handlers/torch_.py` & `coola-0.6.1/src/coola/equality/handlers/torch_.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/testers/base.py` & `coola-0.6.1/src/coola/equality/testers/base.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/equality/testers/default.py` & `coola-0.6.1/src/coola/equality/testers/default.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/formatters/base.py` & `coola-0.6.1/src/coola/formatters/base.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/formatters/default.py` & `coola-0.6.1/src/coola/formatters/default.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/formatters/numpy_.py` & `coola-0.6.1/src/coola/formatters/numpy_.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/formatters/torch_.py` & `coola-0.6.1/src/coola/formatters/torch_.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/nested/conversion.py` & `coola-0.6.1/src/coola/nested/conversion.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/nested/mapping.py` & `coola-0.6.1/src/coola/nested/mapping.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/random/__init__.py` & `coola-0.6.1/src/coola/random/__init__.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/random/base.py` & `coola-0.6.1/src/coola/random/base.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/random/default.py` & `coola-0.6.1/src/coola/random/default.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/random/functional.py` & `coola-0.6.1/src/coola/random/functional.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/random/numpy_.py` & `coola-0.6.1/src/coola/random/numpy_.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/random/random_.py` & `coola-0.6.1/src/coola/random/random_.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/random/torch_.py` & `coola-0.6.1/src/coola/random/torch_.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/random/utils.py` & `coola-0.6.1/src/coola/random/utils.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/reducers/__init__.py` & `coola-0.6.1/src/coola/reducers/__init__.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/reducers/base.py` & `coola-0.6.1/src/coola/reducers/base.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/reducers/native.py` & `coola-0.6.1/src/coola/reducers/native.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/reducers/numpy_.py` & `coola-0.6.1/src/coola/reducers/numpy_.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/reducers/registry.py` & `coola-0.6.1/src/coola/reducers/registry.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/reducers/torch_.py` & `coola-0.6.1/src/coola/reducers/torch_.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/reducers/utils.py` & `coola-0.6.1/src/coola/reducers/utils.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/reduction.py` & `coola-0.6.1/src/coola/reduction.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/summarization.py` & `coola-0.6.1/src/coola/summarization.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/summarizers/base.py` & `coola-0.6.1/src/coola/summarizers/base.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/summarizers/summarizer.py` & `coola-0.6.1/src/coola/summarizers/summarizer.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/testing.py` & `coola-0.6.1/src/coola/testing.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/types.py` & `coola-0.6.1/src/coola/types.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/utils/__init__.py` & `coola-0.6.1/src/coola/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/utils/array.py` & `coola-0.6.1/src/coola/utils/array.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/utils/format.py` & `coola-0.6.1/src/coola/utils/format.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/utils/imports.py` & `coola-0.6.1/src/coola/utils/imports.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/utils/stats.py` & `coola-0.6.1/src/coola/utils/stats.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/src/coola/utils/tensor.py` & `coola-0.6.1/src/coola/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `coola-0.6.0/PKG-INFO` & `coola-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coola
-Version: 0.6.0
+Version: 0.6.1
 Summary: A library to check if two complex/nested objects are equal or not
 Home-page: https://github.com/durandtibo/coola
 License: BSD-3-Clause
 Keywords: complex/nested objects,equality,jax,numpy,pandas,polars,pytorch,xarray
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<3.13
@@ -23,14 +23,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: all
 Requires-Dist: jax (>=0.4.1,<1.0) ; extra == "all"
 Requires-Dist: jaxlib (>=0.4.1,<1.0) ; extra == "all"
 Requires-Dist: numpy (>=1.21,<2.0) ; extra == "all"
 Requires-Dist: pandas (>=1.3,<3.0) ; extra == "all"
 Requires-Dist: polars (>=0.18.3,<1.0) ; extra == "all"
+Requires-Dist: torch (>=1.10,<2.3) ; (sys_platform == "darwin" and platform_machine != "arm64") and (extra == "all")
 Requires-Dist: torch (>=1.10,<3.0) ; extra == "all"
 Requires-Dist: xarray (>=2023.1) ; extra == "all"
 Project-URL: Repository, https://github.com/durandtibo/coola
 Description-Content-Type: text/markdown
 
 # coola
 
@@ -192,29 +193,32 @@
 
 Please check the [get started page](https://durandtibo.github.io/coola/get_started) to see how to
 install only some specific dependencies or other alternatives to install the library.
 The following is the corresponding `coola` versions and tested dependencies.
 
 | `coola` | `jax`<sup>*</sup> | `numpy`<sup>*</sup> | `pandas`<sup>*</sup> | `polars`<sup>*</sup> | `torch`<sup>*</sup> | `xarray`<sup>*</sup> | `python`      |
 |---------|-------------------|---------------------|----------------------|----------------------|---------------------|----------------------|---------------|
-| `main`  | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
+| `main`  | `>=0.4.1,<1.0`    | `>=1.21,<2.0`       | `>=1.3,<3.0`         | `>=0.18.3,<1.0`      | `>=1.10,<3.0`       | `>=2023.1`           | `>=3.9,<3.13` |
+| `0.6.1` | `>=0.4.1,<1.0`    | `>=1.21,<2.0`       | `>=1.3,<3.0`         | `>=0.18.3,<1.0`      | `>=1.10,<3.0`       | `>=2023.1`           | `>=3.9,<3.13` |
+| `0.6.0` | `>=0.4.1,<1.0`    | `>=1.21,<2.0`       | `>=1.3,<3.0`         | `>=0.18.3,<1.0`      | `>=1.10,<3.0`       | `>=2023.1`           | `>=3.9,<3.13` |
+| `0.5.0` | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
 | `0.4.0` | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
-| `0.3.1` | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
-| `0.3.0` | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
-| `0.2.2` | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
-| `0.2.1` | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
-| `0.2.0` | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
 
 <sup>*</sup> indicates an optional dependency
 
 <details>
     <summary>older versions</summary>
 
 | `coola`  | `jax`<sup>*</sup> | `numpy`<sup>*</sup> | `pandas`<sup>*</sup> | `polars`<sup>*</sup> | `torch`<sup>*</sup> | `xarray`<sup>*</sup> | `python`      |
 |----------|-------------------|---------------------|----------------------|----------------------|---------------------|----------------------|---------------|
+| `0.3.1`  | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
+| `0.3.0`  | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
+| `0.2.2`  | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
+| `0.2.1`  | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
+| `0.2.0`  | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<1.0`      | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
 | `0.1.2`  | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<0.21`     | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
 | `0.1.1`  | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<0.20`     | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.13` |
 | `0.1.0`  | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<0.20`     | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.12` |
 | `0.0.26` | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<0.20`     | `>=1.10,<2.2`       | `>=2023.1,<2023.13`  | `>=3.9,<3.12` |
 | `0.0.25` | `>=0.4.1,<0.5`    | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<0.20`     | `>=1.10,<2.2`       | `>=2023.4,<2023.11`  | `>=3.9,<3.12` |
 | `0.0.24` | `>=0.3,<0.5`      | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<0.20`     | `>=1.10,<2.2`       | `>=2023.3,<2023.9`   | `>=3.9,<3.12` |
 | `0.0.23` | `>=0.3,<0.5`      | `>=1.21,<1.27`      | `>=1.3,<2.2`         | `>=0.18.3,<0.20`     | `>=1.10,<2.1`       | `>=2023.3,<2023.9`   | `>=3.9,<3.12` |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coola Version: 0.6.0 Summary: A library to check if
+Metadata-Version: 2.1 Name: coola Version: 0.6.1 Summary: A library to check if
 two complex/nested objects are equal or not Home-page: https://github.com/
 durandtibo/coola License: BSD-3-Clause Keywords: complex/nested
 objects,equality,jax,numpy,pandas,polars,pytorch,xarray Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com Requires-Python: >=3.9,<3.13 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: BSD License
@@ -11,17 +11,19 @@
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Software Development ::
 Libraries Provides-Extra: all Requires-Dist: jax (>=0.4.1,<1.0) ; extra ==
 "all" Requires-Dist: jaxlib (>=0.4.1,<1.0) ; extra == "all" Requires-Dist:
 numpy (>=1.21,<2.0) ; extra == "all" Requires-Dist: pandas (>=1.3,<3.0) ; extra
 == "all" Requires-Dist: polars (>=0.18.3,<1.0) ; extra == "all" Requires-Dist:
-torch (>=1.10,<3.0) ; extra == "all" Requires-Dist: xarray (>=2023.1) ; extra
-== "all" Project-URL: Repository, https://github.com/durandtibo/coola
-Description-Content-Type: text/markdown # coola
+torch (>=1.10,<2.3) ; (sys_platform == "darwin" and platform_machine !=
+"arm64") and (extra == "all") Requires-Dist: torch (>=1.10,<3.0) ; extra ==
+"all" Requires-Dist: xarray (>=2023.1) ; extra == "all" Project-URL:
+Repository, https://github.com/durandtibo/coola Description-Content-Type: text/
+markdown # coola
                   _[_C_I_]_[_N_i_g_h_t_l_y_ _T_e_s_t_s_]_[_N_i_g_h_t_l_y_ _P_a_c_k_a_g_e_ _T_e_s_t_s_]
                         _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]
      _[_C_o_d_e_c_o_v_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_8_3_e_b_b_5_0_e_6_c_6_f_6_7_b_0_5_7_0_d_/
  _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_8_3_e_b_b_5_0_e_6_c_6_f_6_7_b_0_5_7_0_d_/
                                 _t_e_s_t___c_o_v_e_r_a_g_e_]
         _[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_D_o_c_ _s_t_y_l_e_:_ _g_o_o_g_l_e_]_[_R_u_f_f_]_[_D_o_c_ _s_t_y_l_e_:_ _g_o_o_g_l_e_]
                      _[_P_Y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_B_S_D_-_3_-_C_l_a_u_s_e_]
@@ -76,32 +78,37 @@
 install coola[all] ``` Please check the [get started page](https://
 durandtibo.github.io/coola/get_started) to see how to install only some
 specific dependencies or other alternatives to install the library. The
 following is the corresponding `coola` versions and tested dependencies. |
 `coola` | `jax`* | `numpy`* | `pandas`* | `polars`* | `torch`* | `xarray`* |
 `python` | |---------|-------------------|---------------------|---------------
 -------|----------------------|---------------------|----------------------|---
-------------| | `main` | `>=0.4.1,<0.5` | `>=1.21,<1.27` | `>=1.3,<2.2` |
-`>=0.18.3,<1.0` | `>=1.10,<2.2` | `>=2023.1,<2023.13` | `>=3.9,<3.13` | |
-`0.4.0` | `>=0.4.1,<0.5` | `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` |
-`>=1.10,<2.2` | `>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.3.1` |
-`>=0.4.1,<0.5` | `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` |
-`>=1.10,<2.2` | `>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.3.0` |
-`>=0.4.1,<0.5` | `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` |
-`>=1.10,<2.2` | `>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.2.2` |
-`>=0.4.1,<0.5` | `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` |
-`>=1.10,<2.2` | `>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.2.1` |
-`>=0.4.1,<0.5` | `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` |
-`>=1.10,<2.2` | `>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.2.0` |
+------------| | `main` | `>=0.4.1,<1.0` | `>=1.21,<2.0` | `>=1.3,<3.0` |
+`>=0.18.3,<1.0` | `>=1.10,<3.0` | `>=2023.1` | `>=3.9,<3.13` | | `0.6.1` |
+`>=0.4.1,<1.0` | `>=1.21,<2.0` | `>=1.3,<3.0` | `>=0.18.3,<1.0` | `>=1.10,<3.0`
+| `>=2023.1` | `>=3.9,<3.13` | | `0.6.0` | `>=0.4.1,<1.0` | `>=1.21,<2.0` |
+`>=1.3,<3.0` | `>=0.18.3,<1.0` | `>=1.10,<3.0` | `>=2023.1` | `>=3.9,<3.13` | |
+`0.5.0` | `>=0.4.1,<0.5` | `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` |
+`>=1.10,<2.2` | `>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.4.0` |
 `>=0.4.1,<0.5` | `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` |
 `>=1.10,<2.2` | `>=2023.1,<2023.13` | `>=3.9,<3.13` | * indicates an optional
 dependency older versions | `coola` | `jax`* | `numpy`* | `pandas`* | `polars`*
 | `torch`* | `xarray`* | `python` | |----------|-------------------|-----------
 ----------|----------------------|----------------------|---------------------
-|----------------------|---------------| | `0.1.2` | `>=0.4.1,<0.5` |
+|----------------------|---------------| | `0.3.1` | `>=0.4.1,<0.5` |
+`>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` | `>=1.10,<2.2` |
+`>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.3.0` | `>=0.4.1,<0.5` |
+`>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` | `>=1.10,<2.2` |
+`>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.2.2` | `>=0.4.1,<0.5` |
+`>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` | `>=1.10,<2.2` |
+`>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.2.1` | `>=0.4.1,<0.5` |
+`>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` | `>=1.10,<2.2` |
+`>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.2.0` | `>=0.4.1,<0.5` |
+`>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<1.0` | `>=1.10,<2.2` |
+`>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.1.2` | `>=0.4.1,<0.5` |
 `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<0.21` | `>=1.10,<2.2` |
 `>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.1.1` | `>=0.4.1,<0.5` |
 `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<0.20` | `>=1.10,<2.2` |
 `>=2023.1,<2023.13` | `>=3.9,<3.13` | | `0.1.0` | `>=0.4.1,<0.5` |
 `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<0.20` | `>=1.10,<2.2` |
 `>=2023.1,<2023.13` | `>=3.9,<3.12` | | `0.0.26` | `>=0.4.1,<0.5` |
 `>=1.21,<1.27` | `>=1.3,<2.2` | `>=0.18.3,<0.20` | `>=1.10,<2.2` |
```


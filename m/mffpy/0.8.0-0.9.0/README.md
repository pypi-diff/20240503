# Comparing `tmp/mffpy-0.8.0.tar.gz` & `tmp/mffpy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mffpy-0.8.0.tar", last modified: Fri Nov  4 19:40:17 2022, max compression
+gzip compressed data, was "mffpy-0.9.0.tar", last modified: Fri Apr 26 19:54:49 2024, max compression
```

## Comparing `mffpy-0.8.0.tar` & `mffpy-0.9.0.tar`

### file list

```diff
@@ -1,82 +1,81 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-11-04 19:40:17.715655 mffpy-0.8.0/
--rw-r--r--   0 admin      (501) staff       (20)      514 2020-01-29 20:48:12.000000 mffpy-0.8.0/LICENSE
--rw-r--r--   0 admin      (501) staff       (20)      124 2020-12-01 01:34:17.000000 mffpy-0.8.0/MANIFEST.in
--rw-r--r--   0 admin      (501) staff       (20)     8454 2022-11-04 19:40:17.715860 mffpy-0.8.0/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     7882 2022-11-04 19:37:14.000000 mffpy-0.8.0/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-11-04 19:40:17.319120 mffpy-0.8.0/bin/
--rw-r--r--   0 admin      (501) staff       (20)     2168 2021-02-03 23:13:40.000000 mffpy-0.8.0/bin/mff2json.py
--rw-r--r--   0 admin      (501) staff       (20)     1251 2020-01-30 01:14:20.000000 mffpy-0.8.0/bin/mff2mfz.py
--rw-r--r--   0 admin      (501) staff       (20)     3174 2022-02-11 23:45:32.000000 mffpy-0.8.0/bin/mffdiff.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-11-04 19:40:17.418892 mffpy-0.8.0/mffpy/
--rw-r--r--   0 admin      (501) staff       (20)      671 2020-11-11 17:46:24.000000 mffpy-0.8.0/mffpy/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     2939 2020-08-22 00:53:21.000000 mffpy-0.8.0/mffpy/bin_files.py
--rw-r--r--   0 admin      (501) staff       (20)     6997 2021-02-05 17:31:57.000000 mffpy-0.8.0/mffpy/bin_writer.py
--rw-r--r--   0 admin      (501) staff       (20)     1460 2020-11-04 17:04:24.000000 mffpy-0.8.0/mffpy/cached_property.py
--rw-r--r--   0 admin      (501) staff       (20)      927 2020-01-30 01:14:20.000000 mffpy-0.8.0/mffpy/devices.py
--rw-r--r--   0 admin      (501) staff       (20)     2248 2020-01-30 01:14:20.000000 mffpy-0.8.0/mffpy/dict2xml.py
--rw-r--r--   0 admin      (501) staff       (20)     2214 2020-09-16 00:35:14.000000 mffpy-0.8.0/mffpy/epoch.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-11-04 19:40:17.465052 mffpy-0.8.0/mffpy/header_block/
--rw-r--r--   0 admin      (501) staff       (20)      554 2021-02-05 17:31:57.000000 mffpy-0.8.0/mffpy/header_block/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     6069 2021-02-05 17:31:57.000000 mffpy-0.8.0/mffpy/header_block/header_block.py
--rw-r--r--   0 admin      (501) staff       (20)      655 2021-02-05 17:31:57.000000 mffpy-0.8.0/mffpy/header_block/helpers.py
--rw-r--r--   0 admin      (501) staff       (20)     2445 2021-05-13 20:54:55.000000 mffpy-0.8.0/mffpy/header_block/optional_header_block.py
--rw-r--r--   0 admin      (501) staff       (20)     6183 2022-01-27 18:33:48.000000 mffpy-0.8.0/mffpy/mffdir.py
--rw-r--r--   0 admin      (501) staff       (20)     9050 2022-05-05 22:45:56.000000 mffpy-0.8.0/mffpy/raw_bin_files.py
--rw-r--r--   0 admin      (501) staff       (20)    13401 2022-01-27 18:33:48.000000 mffpy-0.8.0/mffpy/reader.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-11-04 19:40:17.283062 mffpy-0.8.0/mffpy/resources/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-11-04 19:40:17.546860 mffpy-0.8.0/mffpy/resources/coordinates/
--rw-r--r--   0 admin      (501) staff       (20)    31543 2022-11-04 19:37:14.000000 mffpy-0.8.0/mffpy/resources/coordinates/Geodesic Head Web 130 1.0.xml
--rw-r--r--   0 admin      (501) staff       (20)    66445 2022-11-04 19:37:14.000000 mffpy-0.8.0/mffpy/resources/coordinates/Geodesic Head Web 280 1.0.xml
--rw-r--r--   0 admin      (501) staff       (20)    30884 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/coordinates/Geodesic Sensor Net 128 2.1.xml
--rw-r--r--   0 admin      (501) staff       (20)    60240 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/coordinates/Geodesic Sensor Net 256 2.1.xml
--rw-r--r--   0 admin      (501) staff       (20)    16275 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/coordinates/Geodesic Sensor Net 64 2.0.xml
--rw-r--r--   0 admin      (501) staff       (20)    30874 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/coordinates/HydroCel GSN 128 1.0.xml
--rw-r--r--   0 admin      (501) staff       (20)    60304 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/coordinates/HydroCel GSN 256 1.0.xml
--rw-r--r--   0 admin      (501) staff       (20)     8925 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/coordinates/HydroCel GSN 32 1.0.xml
--rw-r--r--   0 admin      (501) staff       (20)    16213 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/coordinates/HydroCel GSN 64 1.0.xml
--rw-r--r--   0 admin      (501) staff       (20)    30878 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/coordinates/MicroCel GSN 100 128 1.0.xml
--rw-r--r--   0 admin      (501) staff       (20)    60308 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/coordinates/MicroCel GSN 100 256 1.0.xml
--rw-r--r--   0 admin      (501) staff       (20)     8929 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/coordinates/MicroCel GSN 100 32 1.0.xml
--rw-r--r--   0 admin      (501) staff       (20)    16217 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/coordinates/MicroCel GSN 100 64 1.0.xml
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-11-04 19:40:17.642526 mffpy-0.8.0/mffpy/resources/sensorLayout/
--rw-r--r--   0 admin      (501) staff       (20)    72318 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/sensorLayout/Amp Sample.xml
--rw-r--r--   0 admin      (501) staff       (20)    29682 2022-11-04 19:37:14.000000 mffpy-0.8.0/mffpy/resources/sensorLayout/Geodesic Head Web 130 1.0.xml
--rw-r--r--   0 admin      (501) staff       (20)    63351 2022-11-04 19:37:14.000000 mffpy-0.8.0/mffpy/resources/sensorLayout/Geodesic Head Web 280 1.0.xml
--rw-r--r--   0 admin      (501) staff       (20)    43938 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/sensorLayout/Geodesic Sensor Net 128 2.1.xml
--rw-r--r--   0 admin      (501) staff       (20)    87397 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/sensorLayout/Geodesic Sensor Net 256 2.1.xml
--rw-r--r--   0 admin      (501) staff       (20)    24363 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/sensorLayout/Geodesic Sensor Net 64 2.0.xml
--rw-r--r--   0 admin      (501) staff       (20)    39498 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/sensorLayout/HydroCel GSN 128 1.0.xml
--rw-r--r--   0 admin      (501) staff       (20)    78886 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/sensorLayout/HydroCel GSN 256 1.0.xml
--rw-r--r--   0 admin      (501) staff       (20)    37888 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/sensorLayout/HydroCel GSN 32 1.0.xml
--rw-r--r--   0 admin      (501) staff       (20)    38206 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/sensorLayout/HydroCel GSN 64 1.0.xml
--rw-r--r--   0 admin      (501) staff       (20)    39502 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/sensorLayout/MicroCel GSN 100 128 1.0.xml
--rw-r--r--   0 admin      (501) staff       (20)    78890 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/sensorLayout/MicroCel GSN 100 256 1.0.xml
--rw-r--r--   0 admin      (501) staff       (20)    37892 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/sensorLayout/MicroCel GSN 100 32 1.0.xml
--rw-r--r--   0 admin      (501) staff       (20)    38210 2020-01-29 20:48:13.000000 mffpy-0.8.0/mffpy/resources/sensorLayout/MicroCel GSN 100 64 1.0.xml
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-11-04 19:40:17.715165 mffpy-0.8.0/mffpy/tests/
--rw-r--r--   0 admin      (501) staff       (20)      501 2020-12-01 01:34:17.000000 mffpy-0.8.0/mffpy/tests/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1102 2022-01-27 18:33:48.000000 mffpy-0.8.0/mffpy/tests/conftest.py
--rw-r--r--   0 admin      (501) staff       (20)     2105 2020-11-04 17:04:24.000000 mffpy-0.8.0/mffpy/tests/test_cached_property.py
--rw-r--r--   0 admin      (501) staff       (20)     1841 2022-11-04 19:37:14.000000 mffpy-0.8.0/mffpy/tests/test_devices.py
--rw-r--r--   0 admin      (501) staff       (20)     1142 2022-01-27 18:33:48.000000 mffpy-0.8.0/mffpy/tests/test_dict2xml.py
--rw-r--r--   0 admin      (501) staff       (20)     1921 2021-02-05 17:31:57.000000 mffpy-0.8.0/mffpy/tests/test_header_block.py
--rw-r--r--   0 admin      (501) staff       (20)     2200 2020-01-30 01:14:20.000000 mffpy-0.8.0/mffpy/tests/test_mffdir.py
--rw-r--r--   0 admin      (501) staff       (20)     3695 2022-05-05 22:45:56.000000 mffpy-0.8.0/mffpy/tests/test_raw_bin_files.py
--rw-r--r--   0 admin      (501) staff       (20)     8412 2022-07-05 21:15:34.000000 mffpy-0.8.0/mffpy/tests/test_reader.py
--rw-r--r--   0 admin      (501) staff       (20)    11073 2022-05-10 21:19:42.000000 mffpy-0.8.0/mffpy/tests/test_writer.py
--rw-r--r--   0 admin      (501) staff       (20)    19984 2022-11-04 19:37:14.000000 mffpy-0.8.0/mffpy/tests/test_xml_files.py
--rw-r--r--   0 admin      (501) staff       (20)     1968 2020-01-30 01:14:20.000000 mffpy-0.8.0/mffpy/tests/test_zipfile.py
--rw-r--r--   0 admin      (501) staff       (20)       22 2022-11-04 19:37:14.000000 mffpy-0.8.0/mffpy/version.py
--rw-r--r--   0 admin      (501) staff       (20)     5013 2022-05-10 21:19:42.000000 mffpy-0.8.0/mffpy/writer.py
--rw-r--r--   0 admin      (501) staff       (20)    46824 2022-11-04 19:37:14.000000 mffpy-0.8.0/mffpy/xml_files.py
--rw-r--r--   0 admin      (501) staff       (20)     3631 2020-10-30 20:40:15.000000 mffpy-0.8.0/mffpy/zipfile.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-11-04 19:40:17.436412 mffpy-0.8.0/mffpy.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     8454 2022-11-04 19:40:17.000000 mffpy-0.8.0/mffpy.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     2538 2022-11-04 19:40:17.000000 mffpy-0.8.0/mffpy.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2022-11-04 19:40:17.000000 mffpy-0.8.0/mffpy.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       58 2022-11-04 19:40:17.000000 mffpy-0.8.0/mffpy.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)        6 2022-11-04 19:40:17.000000 mffpy-0.8.0/mffpy.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)      104 2021-02-05 17:49:31.000000 mffpy-0.8.0/pyproject.toml
--rw-r--r--   0 admin      (501) staff       (20)       58 2022-07-05 21:15:34.000000 mffpy-0.8.0/requirements.txt
--rw-r--r--   0 admin      (501) staff       (20)      564 2022-11-04 19:40:17.723187 mffpy-0.8.0/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1192 2022-04-25 16:45:19.000000 mffpy-0.8.0/setup.py
+drwxrwxr-x   0 damian    (1000) damian    (1000)        0 2024-04-26 19:54:49.305913 mffpy-0.9.0/
+-rw-rw-r--   0 damian    (1000) damian    (1000)      514 2020-11-19 22:10:40.000000 mffpy-0.9.0/LICENSE
+-rw-rw-r--   0 damian    (1000) damian    (1000)      124 2021-02-04 20:42:15.000000 mffpy-0.9.0/MANIFEST.in
+-rw-r--r--   0 damian    (1000) damian    (1000)     8525 2024-04-26 19:54:49.305913 mffpy-0.9.0/PKG-INFO
+-rw-rw-r--   0 damian    (1000) damian    (1000)     7882 2024-04-11 18:18:54.000000 mffpy-0.9.0/README.md
+drwxrwxr-x   0 damian    (1000) damian    (1000)        0 2024-04-26 19:54:49.273913 mffpy-0.9.0/bin/
+-rw-rw-r--   0 damian    (1000) damian    (1000)     2168 2021-02-04 20:42:15.000000 mffpy-0.9.0/bin/mff2json.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     1251 2020-11-19 22:10:40.000000 mffpy-0.9.0/bin/mff2mfz.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     3174 2022-05-06 17:12:03.000000 mffpy-0.9.0/bin/mffdiff.py
+drwxrwxr-x   0 damian    (1000) damian    (1000)        0 2024-04-26 19:54:49.277913 mffpy-0.9.0/mffpy/
+-rw-rw-r--   0 damian    (1000) damian    (1000)      671 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/__init__.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     2939 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/bin_files.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     6997 2021-02-04 20:42:15.000000 mffpy-0.9.0/mffpy/bin_writer.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     1460 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/cached_property.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)      927 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/devices.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     2248 2024-03-21 20:31:28.000000 mffpy-0.9.0/mffpy/dict2xml.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     2214 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/epoch.py
+drwxrwxr-x   0 damian    (1000) damian    (1000)        0 2024-04-26 19:54:49.281913 mffpy-0.9.0/mffpy/header_block/
+-rw-rw-r--   0 damian    (1000) damian    (1000)      554 2021-02-04 20:42:15.000000 mffpy-0.9.0/mffpy/header_block/__init__.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     6069 2021-02-04 20:42:15.000000 mffpy-0.9.0/mffpy/header_block/header_block.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)      655 2021-02-04 20:42:15.000000 mffpy-0.9.0/mffpy/header_block/helpers.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     2445 2021-02-19 00:58:54.000000 mffpy-0.9.0/mffpy/header_block/optional_header_block.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     6183 2022-08-24 21:58:20.000000 mffpy-0.9.0/mffpy/mffdir.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     9050 2022-05-06 17:12:03.000000 mffpy-0.9.0/mffpy/raw_bin_files.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)    13401 2022-05-06 17:12:03.000000 mffpy-0.9.0/mffpy/reader.py
+drwxrwxr-x   0 damian    (1000) damian    (1000)        0 2024-04-26 19:54:49.273913 mffpy-0.9.0/mffpy/resources/
+drwxrwxr-x   0 damian    (1000) damian    (1000)        0 2024-04-26 19:54:49.289913 mffpy-0.9.0/mffpy/resources/coordinates/
+-rw-rw-r--   0 damian    (1000) damian    (1000)    31543 2022-10-28 15:53:57.000000 mffpy-0.9.0/mffpy/resources/coordinates/Geodesic Head Web 130 1.0.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    66445 2022-10-28 15:53:57.000000 mffpy-0.9.0/mffpy/resources/coordinates/Geodesic Head Web 280 1.0.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    30884 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/coordinates/Geodesic Sensor Net 128 2.1.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    60240 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/coordinates/Geodesic Sensor Net 256 2.1.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    16275 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/coordinates/Geodesic Sensor Net 64 2.0.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    30874 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/coordinates/HydroCel GSN 128 1.0.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    60304 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/coordinates/HydroCel GSN 256 1.0.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)     8925 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/coordinates/HydroCel GSN 32 1.0.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    16213 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/coordinates/HydroCel GSN 64 1.0.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    30878 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/coordinates/MicroCel GSN 100 128 1.0.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    60308 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/coordinates/MicroCel GSN 100 256 1.0.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)     8929 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/coordinates/MicroCel GSN 100 32 1.0.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    16217 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/coordinates/MicroCel GSN 100 64 1.0.xml
+drwxrwxr-x   0 damian    (1000) damian    (1000)        0 2024-04-26 19:54:49.293913 mffpy-0.9.0/mffpy/resources/sensorLayout/
+-rw-rw-r--   0 damian    (1000) damian    (1000)    72318 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/sensorLayout/Amp Sample.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    29682 2022-10-28 15:53:57.000000 mffpy-0.9.0/mffpy/resources/sensorLayout/Geodesic Head Web 130 1.0.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    63351 2022-10-28 15:53:57.000000 mffpy-0.9.0/mffpy/resources/sensorLayout/Geodesic Head Web 280 1.0.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    43938 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/sensorLayout/Geodesic Sensor Net 128 2.1.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    87397 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/sensorLayout/Geodesic Sensor Net 256 2.1.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    24363 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/sensorLayout/Geodesic Sensor Net 64 2.0.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    39498 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/sensorLayout/HydroCel GSN 128 1.0.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    78886 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/sensorLayout/HydroCel GSN 256 1.0.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    37888 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/sensorLayout/HydroCel GSN 32 1.0.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    38206 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/sensorLayout/HydroCel GSN 64 1.0.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    39502 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/sensorLayout/MicroCel GSN 100 128 1.0.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    78890 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/sensorLayout/MicroCel GSN 100 256 1.0.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    37892 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/sensorLayout/MicroCel GSN 100 32 1.0.xml
+-rw-rw-r--   0 damian    (1000) damian    (1000)    38210 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/resources/sensorLayout/MicroCel GSN 100 64 1.0.xml
+drwxrwxr-x   0 damian    (1000) damian    (1000)        0 2024-04-26 19:54:49.305913 mffpy-0.9.0/mffpy/tests/
+-rw-rw-r--   0 damian    (1000) damian    (1000)      501 2021-02-04 20:42:15.000000 mffpy-0.9.0/mffpy/tests/__init__.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     2395 2024-04-11 18:18:55.000000 mffpy-0.9.0/mffpy/tests/conftest.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     2105 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/tests/test_cached_property.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     1841 2022-10-28 15:53:57.000000 mffpy-0.9.0/mffpy/tests/test_devices.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     1142 2021-09-02 20:52:32.000000 mffpy-0.9.0/mffpy/tests/test_dict2xml.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     1921 2021-02-04 20:42:15.000000 mffpy-0.9.0/mffpy/tests/test_header_block.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     2200 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/tests/test_mffdir.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     3695 2022-05-06 17:12:03.000000 mffpy-0.9.0/mffpy/tests/test_raw_bin_files.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     8412 2024-03-13 06:20:19.000000 mffpy-0.9.0/mffpy/tests/test_reader.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)    11504 2024-04-11 18:18:55.000000 mffpy-0.9.0/mffpy/tests/test_writer.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)    20552 2024-04-11 18:18:55.000000 mffpy-0.9.0/mffpy/tests/test_xml_files.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     1968 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/tests/test_zipfile.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)       22 2024-04-11 18:18:55.000000 mffpy-0.9.0/mffpy/version.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     5013 2022-05-06 17:12:03.000000 mffpy-0.9.0/mffpy/writer.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)    53473 2024-04-11 18:18:55.000000 mffpy-0.9.0/mffpy/xml_files.py
+-rw-rw-r--   0 damian    (1000) damian    (1000)     3631 2020-11-19 22:10:41.000000 mffpy-0.9.0/mffpy/zipfile.py
+drwxrwxr-x   0 damian    (1000) damian    (1000)        0 2024-04-26 19:54:49.305913 mffpy-0.9.0/mffpy.egg-info/
+-rw-r--r--   0 damian    (1000) damian    (1000)     8525 2024-04-26 19:54:49.000000 mffpy-0.9.0/mffpy.egg-info/PKG-INFO
+-rw-rw-r--   0 damian    (1000) damian    (1000)     2513 2024-04-26 19:54:49.000000 mffpy-0.9.0/mffpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 damian    (1000) damian    (1000)        1 2024-04-26 19:54:49.000000 mffpy-0.9.0/mffpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 damian    (1000) damian    (1000)       58 2024-04-26 19:54:49.000000 mffpy-0.9.0/mffpy.egg-info/requires.txt
+-rw-rw-r--   0 damian    (1000) damian    (1000)        6 2024-04-26 19:54:49.000000 mffpy-0.9.0/mffpy.egg-info/top_level.txt
+-rw-rw-r--   0 damian    (1000) damian    (1000)       58 2022-10-28 15:53:57.000000 mffpy-0.9.0/requirements.txt
+-rw-rw-r--   0 damian    (1000) damian    (1000)       38 2024-04-26 19:54:49.305913 mffpy-0.9.0/setup.cfg
+-rw-rw-r--   0 damian    (1000) damian    (1000)     1192 2021-09-02 20:52:21.000000 mffpy-0.9.0/setup.py
```

### Comparing `mffpy-0.8.0/LICENSE` & `mffpy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/PKG-INFO` & `mffpy-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: mffpy
-Version: 0.8.0
+Version: 0.9.0
 Summary: Reader and Writer for Philips' MFF file format.
-Home-page: https://github.com/BEL-Public/mffpy
 Author: Justus Schwabedal, Wayne Manselle
 Author-email: jschwabedal@belco.tech, wayne.manselle@belco.tech
 Maintainer: Evan Hathaway
 Maintainer-email: evan.hathaway@belco.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: lxml>=4.8.0
+Requires-Dist: pytz>=2019.2
+Requires-Dist: numpy>=1.15.1
+Requires-Dist: Deprecated>=1.2.12
 
 # Introduction
 
 [![Github Actions](https://github.com/BEL-Public/mffpy/workflows/lint-and-test/badge.svg)
 ](https://github.com/BEL-Public/mffpy/actions)
 
 `mffpy` is a lean reader for EGI's MFF file format.  These files are
@@ -48,26 +51,26 @@
 ### Test Coverage
 
 ```
 ============================= test session starts ==============================
 platform linux -- Python 3.6.7, pytest-7.0.1, pluggy-1.0.0
 rootdir: /home/runner/work/mffpy/mffpy
 plugins: cov-4.0.0
-collected 122 items
+collected 123 items
 
 mffpy/tests/test_cached_property.py ..                                   [  1%]
 mffpy/tests/test_devices.py .............                                [ 12%]
 mffpy/tests/test_dict2xml.py .                                           [ 13%]
 mffpy/tests/test_header_block.py ..                                      [ 14%]
-mffpy/tests/test_mffdir.py ....                                          [ 18%]
+mffpy/tests/test_mffdir.py ....                                          [ 17%]
 mffpy/tests/test_raw_bin_files.py ..................                     [ 32%]
 mffpy/tests/test_reader.py ......................                        [ 50%]
 mffpy/tests/test_writer.py ...........                                   [ 59%]
-mffpy/tests/test_xml_files.py .......................................... [ 94%]
-..                                                                       [ 95%]
+mffpy/tests/test_xml_files.py .......................................... [ 93%]
+...                                                                      [ 95%]
 mffpy/tests/test_zipfile.py .....                                        [100%]
 
 ----------- coverage: platform linux, python 3.6.7-final-0 -----------
 Name                                          Stmts   Miss  Cover
 -----------------------------------------------------------------
 mffpy/__init__.py                                 4      0   100%
 mffpy/bin_files.py                               40      2    95%
@@ -80,31 +83,31 @@
 mffpy/header_block/header_block.py               48      2    96%
 mffpy/header_block/helpers.py                    15      0   100%
 mffpy/header_block/optional_header_block.py      32      1    97%
 mffpy/mffdir.py                                  92      7    92%
 mffpy/raw_bin_files.py                          113      0   100%
 mffpy/reader.py                                 110      2    98%
 mffpy/tests/__init__.py                           0      0   100%
-mffpy/tests/conftest.py                          11      0   100%
+mffpy/tests/conftest.py                          15      0   100%
 mffpy/tests/test_cached_property.py              33      0   100%
 mffpy/tests/test_devices.py                      12      0   100%
 mffpy/tests/test_dict2xml.py                     16      0   100%
 mffpy/tests/test_header_block.py                 33      0   100%
 mffpy/tests/test_mffdir.py                       30      0   100%
 mffpy/tests/test_raw_bin_files.py                63      0   100%
 mffpy/tests/test_reader.py                       96      0   100%
-mffpy/tests/test_writer.py                      204      0   100%
-mffpy/tests/test_xml_files.py                   202      1    99%
+mffpy/tests/test_writer.py                      212      0   100%
+mffpy/tests/test_xml_files.py                   214      1    99%
 mffpy/tests/test_zipfile.py                      34      0   100%
 mffpy/version.py                                  1      0   100%
 mffpy/writer.py                                  71      0   100%
-mffpy/xml_files.py                              554     18    97%
+mffpy/xml_files.py                              607     22    96%
 mffpy/zipfile.py                                 47      0   100%
 -----------------------------------------------------------------
-TOTAL                                          2023     40    98%
+TOTAL                                          2100     44    98%
 
 
 ============================= 122 passed in 7.19s ==============================
 ```
 
 ## View the Docs
```

### Comparing `mffpy-0.8.0/README.md` & `mffpy-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,26 +32,26 @@
 ### Test Coverage
 
 ```
 ============================= test session starts ==============================
 platform linux -- Python 3.6.7, pytest-7.0.1, pluggy-1.0.0
 rootdir: /home/runner/work/mffpy/mffpy
 plugins: cov-4.0.0
-collected 122 items
+collected 123 items
 
 mffpy/tests/test_cached_property.py ..                                   [  1%]
 mffpy/tests/test_devices.py .............                                [ 12%]
 mffpy/tests/test_dict2xml.py .                                           [ 13%]
 mffpy/tests/test_header_block.py ..                                      [ 14%]
-mffpy/tests/test_mffdir.py ....                                          [ 18%]
+mffpy/tests/test_mffdir.py ....                                          [ 17%]
 mffpy/tests/test_raw_bin_files.py ..................                     [ 32%]
 mffpy/tests/test_reader.py ......................                        [ 50%]
 mffpy/tests/test_writer.py ...........                                   [ 59%]
-mffpy/tests/test_xml_files.py .......................................... [ 94%]
-..                                                                       [ 95%]
+mffpy/tests/test_xml_files.py .......................................... [ 93%]
+...                                                                      [ 95%]
 mffpy/tests/test_zipfile.py .....                                        [100%]
 
 ----------- coverage: platform linux, python 3.6.7-final-0 -----------
 Name                                          Stmts   Miss  Cover
 -----------------------------------------------------------------
 mffpy/__init__.py                                 4      0   100%
 mffpy/bin_files.py                               40      2    95%
@@ -64,31 +64,31 @@
 mffpy/header_block/header_block.py               48      2    96%
 mffpy/header_block/helpers.py                    15      0   100%
 mffpy/header_block/optional_header_block.py      32      1    97%
 mffpy/mffdir.py                                  92      7    92%
 mffpy/raw_bin_files.py                          113      0   100%
 mffpy/reader.py                                 110      2    98%
 mffpy/tests/__init__.py                           0      0   100%
-mffpy/tests/conftest.py                          11      0   100%
+mffpy/tests/conftest.py                          15      0   100%
 mffpy/tests/test_cached_property.py              33      0   100%
 mffpy/tests/test_devices.py                      12      0   100%
 mffpy/tests/test_dict2xml.py                     16      0   100%
 mffpy/tests/test_header_block.py                 33      0   100%
 mffpy/tests/test_mffdir.py                       30      0   100%
 mffpy/tests/test_raw_bin_files.py                63      0   100%
 mffpy/tests/test_reader.py                       96      0   100%
-mffpy/tests/test_writer.py                      204      0   100%
-mffpy/tests/test_xml_files.py                   202      1    99%
+mffpy/tests/test_writer.py                      212      0   100%
+mffpy/tests/test_xml_files.py                   214      1    99%
 mffpy/tests/test_zipfile.py                      34      0   100%
 mffpy/version.py                                  1      0   100%
 mffpy/writer.py                                  71      0   100%
-mffpy/xml_files.py                              554     18    97%
+mffpy/xml_files.py                              607     22    96%
 mffpy/zipfile.py                                 47      0   100%
 -----------------------------------------------------------------
-TOTAL                                          2023     40    98%
+TOTAL                                          2100     44    98%
 
 
 ============================= 122 passed in 7.19s ==============================
 ```
 
 ## View the Docs
```

### Comparing `mffpy-0.8.0/bin/mff2json.py` & `mffpy-0.9.0/bin/mff2json.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/bin/mff2mfz.py` & `mffpy-0.9.0/bin/mff2mfz.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/bin/mffdiff.py` & `mffpy-0.9.0/bin/mffdiff.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/__init__.py` & `mffpy-0.9.0/mffpy/__init__.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/bin_files.py` & `mffpy-0.9.0/mffpy/bin_files.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/bin_writer.py` & `mffpy-0.9.0/mffpy/bin_writer.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/cached_property.py` & `mffpy-0.9.0/mffpy/cached_property.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/devices.py` & `mffpy-0.9.0/mffpy/devices.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/dict2xml.py` & `mffpy-0.9.0/mffpy/dict2xml.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/epoch.py` & `mffpy-0.9.0/mffpy/epoch.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/header_block/__init__.py` & `mffpy-0.9.0/mffpy/header_block/__init__.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/header_block/header_block.py` & `mffpy-0.9.0/mffpy/header_block/header_block.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/header_block/helpers.py` & `mffpy-0.9.0/mffpy/header_block/helpers.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/header_block/optional_header_block.py` & `mffpy-0.9.0/mffpy/header_block/optional_header_block.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/mffdir.py` & `mffpy-0.9.0/mffpy/mffdir.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/raw_bin_files.py` & `mffpy-0.9.0/mffpy/raw_bin_files.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/reader.py` & `mffpy-0.9.0/mffpy/reader.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/coordinates/Geodesic Head Web 130 1.0.xml` & `mffpy-0.9.0/mffpy/resources/coordinates/Geodesic Head Web 130 1.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/coordinates/Geodesic Head Web 280 1.0.xml` & `mffpy-0.9.0/mffpy/resources/coordinates/Geodesic Head Web 280 1.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/coordinates/Geodesic Sensor Net 128 2.1.xml` & `mffpy-0.9.0/mffpy/resources/coordinates/Geodesic Sensor Net 128 2.1.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/coordinates/Geodesic Sensor Net 256 2.1.xml` & `mffpy-0.9.0/mffpy/resources/coordinates/Geodesic Sensor Net 256 2.1.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/coordinates/Geodesic Sensor Net 64 2.0.xml` & `mffpy-0.9.0/mffpy/resources/coordinates/Geodesic Sensor Net 64 2.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/coordinates/HydroCel GSN 128 1.0.xml` & `mffpy-0.9.0/mffpy/resources/coordinates/HydroCel GSN 128 1.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/coordinates/HydroCel GSN 256 1.0.xml` & `mffpy-0.9.0/mffpy/resources/coordinates/HydroCel GSN 256 1.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/coordinates/HydroCel GSN 32 1.0.xml` & `mffpy-0.9.0/mffpy/resources/coordinates/HydroCel GSN 32 1.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/coordinates/HydroCel GSN 64 1.0.xml` & `mffpy-0.9.0/mffpy/resources/coordinates/HydroCel GSN 64 1.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/coordinates/MicroCel GSN 100 128 1.0.xml` & `mffpy-0.9.0/mffpy/resources/coordinates/MicroCel GSN 100 128 1.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/coordinates/MicroCel GSN 100 256 1.0.xml` & `mffpy-0.9.0/mffpy/resources/coordinates/MicroCel GSN 100 256 1.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/coordinates/MicroCel GSN 100 32 1.0.xml` & `mffpy-0.9.0/mffpy/resources/coordinates/MicroCel GSN 100 32 1.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/coordinates/MicroCel GSN 100 64 1.0.xml` & `mffpy-0.9.0/mffpy/resources/coordinates/MicroCel GSN 100 64 1.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/sensorLayout/Amp Sample.xml` & `mffpy-0.9.0/mffpy/resources/sensorLayout/Amp Sample.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/sensorLayout/Geodesic Head Web 130 1.0.xml` & `mffpy-0.9.0/mffpy/resources/sensorLayout/Geodesic Head Web 130 1.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/sensorLayout/Geodesic Head Web 280 1.0.xml` & `mffpy-0.9.0/mffpy/resources/sensorLayout/Geodesic Head Web 280 1.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/sensorLayout/Geodesic Sensor Net 128 2.1.xml` & `mffpy-0.9.0/mffpy/resources/sensorLayout/Geodesic Sensor Net 128 2.1.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/sensorLayout/Geodesic Sensor Net 256 2.1.xml` & `mffpy-0.9.0/mffpy/resources/sensorLayout/Geodesic Sensor Net 256 2.1.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/sensorLayout/Geodesic Sensor Net 64 2.0.xml` & `mffpy-0.9.0/mffpy/resources/sensorLayout/Geodesic Sensor Net 64 2.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/sensorLayout/HydroCel GSN 128 1.0.xml` & `mffpy-0.9.0/mffpy/resources/sensorLayout/HydroCel GSN 128 1.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/sensorLayout/HydroCel GSN 256 1.0.xml` & `mffpy-0.9.0/mffpy/resources/sensorLayout/HydroCel GSN 256 1.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/sensorLayout/HydroCel GSN 32 1.0.xml` & `mffpy-0.9.0/mffpy/resources/sensorLayout/HydroCel GSN 32 1.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/sensorLayout/HydroCel GSN 64 1.0.xml` & `mffpy-0.9.0/mffpy/resources/sensorLayout/HydroCel GSN 64 1.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/sensorLayout/MicroCel GSN 100 128 1.0.xml` & `mffpy-0.9.0/mffpy/resources/sensorLayout/MicroCel GSN 100 128 1.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/sensorLayout/MicroCel GSN 100 256 1.0.xml` & `mffpy-0.9.0/mffpy/resources/sensorLayout/MicroCel GSN 100 256 1.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/sensorLayout/MicroCel GSN 100 32 1.0.xml` & `mffpy-0.9.0/mffpy/resources/sensorLayout/MicroCel GSN 100 32 1.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/resources/sensorLayout/MicroCel GSN 100 64 1.0.xml` & `mffpy-0.9.0/mffpy/resources/sensorLayout/MicroCel GSN 100 64 1.0.xml`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/tests/test_cached_property.py` & `mffpy-0.9.0/mffpy/tests/test_cached_property.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/tests/test_devices.py` & `mffpy-0.9.0/mffpy/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/tests/test_dict2xml.py` & `mffpy-0.9.0/mffpy/tests/test_dict2xml.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/tests/test_header_block.py` & `mffpy-0.9.0/mffpy/tests/test_header_block.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/tests/test_mffdir.py` & `mffpy-0.9.0/mffpy/tests/test_mffdir.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/tests/test_raw_bin_files.py` & `mffpy-0.9.0/mffpy/tests/test_raw_bin_files.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/tests/test_reader.py` & `mffpy-0.9.0/mffpy/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/tests/test_writer.py` & `mffpy-0.9.0/mffpy/tests/test_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,24 +161,24 @@
     W2.write()
 
     for p in [mffpath, mfzpath]:
         R2 = Reader(p)
         assert R2.startdatetime == time2
 
 
-def test_writer_writes_multple_bins(tmpdir):
+def test_writer_writes_multple_bins(tmpdir, sensors):
     """test that `mffpy.Writer` can write multiple binary files"""
     dirname = join(str(tmpdir), 'multiple_bins.mff')
     device = 'HydroCel GSN 256 1.0'
     # create some data and add it to binary writers
     num_samples = 10
     sampling_rate = 128
     num_channels_dict = {
         'EEG': 256,
-        'PNSData': 16
+        'PNSData': 2
     }
     data = {
         dtype: np.random.randn(
             num_channels, num_samples).astype(np.float32)
         for dtype, num_channels in num_channels_dict.items()
     }
     bin_writers = {
@@ -188,14 +188,20 @@
     for dtype, bin_writer in bin_writers.items():
         bin_writer.add_block(data[dtype])
     # create an mffpy.Writer and add a file info, and the binary file
     W = Writer(dirname)
     startdatetime = datetime.strptime(
         '1984-02-18T14:00:10.000000+0100', XML._time_format)
     W.addxml('fileInfo', recordTime=startdatetime)
+    W.addxml(
+        'PNSSet',
+        name='Physio 16 set 60hz 1.0',
+        amp_series='400',
+        sensors=sensors,
+    )
     W.add_coordinates_and_sensor_layout(device)
     for b in bin_writers.values():
         W.addbin(b)
 
     W.write()
     # read it again; compare the result
     R = Reader(dirname)
@@ -208,14 +214,22 @@
         assert t0 == 0.0
         assert written == pytest.approx(expected)
 
     layout = R.directory.filepointer('sensorLayout')
     layout = XML.from_file(layout)
     assert layout.name == device
 
+    pns_set = R.directory.filepointer('pnsSet')
+    pns_set = XML.from_file(pns_set)
+    assert pns_set.name == 'Physio 16 set 60hz 1.0'
+    assert pns_set.amp_series == '400'
+    for key, val in pns_set.sensors.items():
+        for k, v in val.items():
+            assert v == sensors[key][k]
+
 
 def test_write_multiple_blocks():
     """check that BinWriter correctly handles adding multiple blocks"""
     B = BinWriter(sampling_rate=250)
     data = np.random.randn(257, 10).astype(np.float32)
     B.add_block(data)
     B.add_block(data, offset_us=None)
```

### Comparing `mffpy-0.8.0/mffpy/tests/test_xml_files.py` & `mffpy-0.9.0/mffpy/tests/test_xml_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from ..dict2xml import dict2xml
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 examples_path = join(dirname(__file__), '..', '..', 'examples')
 mff_path = join(examples_path, 'example_1.mff')
+mffpath_3 = join(examples_path, 'example_3.mff')
 
 """
 Here are several fixtures that parse example xml files
 to be tested.  The files parsed are located in `mff_path`.
 """
 
 
@@ -142,14 +143,16 @@
     assert category_names == expected_names
 
 
 def test_FileInfo(file_info):
     assert file_info.mffVersion == '3'
     assert file_info.acquisitionVersion == '5.4.1.2 (r28337)'
     assert file_info.ampType == 'NA400'
+    assert file_info.ampSerialNumber == 'M13010030'
+    assert file_info.ampFirmwareVersion == '1.6.23'
     expected_rt = datetime.strptime(
         '2019-05-01T10:58:31.236065-0700', "%Y-%m-%dT%H:%M:%S.%f%z")
     assert file_info.recordTime == expected_rt, f"""
     found record time {file_info.recordTime} [expected {expected_rt}]"""
 
 
 def test_fileInfo_fails():
@@ -512,14 +515,26 @@
         [64, 120, 150],
         [68, 120, 150],
         [69, 120, 150],
         [61, 130, 150]
     ], dtype=np.float32))
 
 
+def test_pnsSet(sensors):
+    """test parsing of `pnsSet.xml`"""
+    filepath = join(mffpath_3, 'pnsSet.xml')
+    assert exists(filepath), f"Not found: '{filepath}'"
+    pns_set = XML.from_file(filepath)
+    assert pns_set.name == 'Physio 16 set 60hz 1.0'
+    assert pns_set.amp_series == '400'
+    for key, val in pns_set.sensors.items():
+        for k, v in val.items():
+            assert v == sensors[key][k]
+
+
 @pytest.mark.parametrize("idx,expected", [
     ('name', 'Noise_30Seconds'),
     ('method', 'Segmentation'),
     ('version', '5.4.1.2'),
     ('beginTime', XML._parse_time_str('2019-10-25T12:09:57.639365-07:00')),
     ('endTime', XML._parse_time_str('2019-10-25T12:09:57.897929-07:00')),
     ('sourceFiles', ['/Volumes/PARTYONWAYN/NoiseTest_2.mff']),
```

### Comparing `mffpy-0.8.0/mffpy/tests/test_zipfile.py` & `mffpy-0.9.0/mffpy/tests/test_zipfile.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/writer.py` & `mffpy-0.9.0/mffpy/writer.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy/xml_files.py` & `mffpy-0.9.0/mffpy/xml_files.py`

 * *Files 5% similar despite different names*

```diff
@@ -179,23 +179,37 @@
     @cached_property
     def ampType(self):
         """return content of ampType field"""
         el = self.find('ampType')
         return None if el is None else el.text
 
     @cached_property
+    def ampSerialNumber(self):
+        """return content of ampSerialNumber field"""
+        el = self.find('ampSerialNumber')
+        return None if el is None else el.text
+
+    @cached_property
+    def ampFirmwareVersion(self):
+        """return content of ampFirmwareVersion field"""
+        el = self.find('ampFirmwareVersion')
+        return None if el is None else el.text
+
+    @cached_property
     def recordTime(self):
         el = self.find('recordTime')
         return self._parse_time_str(el.text) if el is not None else None
 
     @classmethod
     def content(cls, recordTime: datetime,  # type: ignore
                 mffVersion: str = '3',
                 acquisitionVersion: str = None,
-                ampType: str = None) -> dict:
+                ampType: str = None,
+                ampSerialNumber: str = None,
+                ampFirmwareVersion: str = None) -> dict:
         """returns MFF file information
 
         Only Version '3' is supported.
         """
         assert mffVersion in cls._supported_versions, f"""
         version {mffVersion} not supported"""
         content = {
@@ -208,35 +222,49 @@
         }
         if acquisitionVersion:
             content.update(acquisitionVersion={TEXT: acquisitionVersion})
 
         if ampType:
             content.update(ampType={TEXT: ampType})
 
+        if ampSerialNumber:
+            content.update(ampSerialNumber={TEXT: ampSerialNumber})
+
+        if ampFirmwareVersion:
+            content.update(ampFirmwareVersion={TEXT: ampFirmwareVersion})
+
         return content
 
     def get_content(self):
         """return dictionary of MFF file information
 
         The info are comprised of:
         - MFF version number
         - time of start of recording
         - acquisition version (optional)
         - amplifier type (optional)
+        - amplifier serial number (optional)
+        - amplifier firmware version (optional)
         """
         content = {
             'mffVersion': self.mffVersion,
             'recordTime': self.recordTime
         }
         if self.acquisitionVersion:
             content.update(acquisitionVersion=self.acquisitionVersion)
 
         if self.ampType:
             content.update(ampType=self.ampType)
 
+        if self.ampSerialNumber:
+            content.update(ampSerialNumber=self.ampSerialNumber)
+
+        if self.ampFirmwareVersion:
+            content.update(ampFirmwareVersion=self.ampFirmwareVersion)
+
         return content
 
     def get_serializable_content(self):
         """return serializable dictionary of MFF file information"""
         content = copy.deepcopy(self.get_content())
         content['recordTime'] = XML._dump_datetime(content['recordTime'])
         return content
@@ -1262,14 +1290,179 @@
         content['dipoles'] = {
             key: value.tolist()
             for key, value in content['dipoles'].items()
         }
         return content
 
 
+class PNSSet(XML):
+    """Parser for 'pnsSet.xml' file
+
+    These files have the following structure:
+    ```
+    <?xml version="1.0" encoding="UTF-8" standalone="yes" ?>
+    <PNSSet xmlns="http://www.egi.com/pnsSet_mff"
+    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
+        <name>Physio 16 set 60hz 1.0</name>
+        <ampSeries>400</ampSeries>
+        <sensors>
+            <sensor>
+                <name>ECG</name>
+                <number>0</number>
+                <unit>uV</unit>
+                <psgType>0</psgType>
+                <mapping>1</mapping>
+                <samplingRate>0</samplingRate>
+                <sensorType>ECG</sensorType>
+                <highpass>0.3000000119</highpass>
+                <lowpass>70</lowpass>
+                <notch>60</notch>
+                <groupNumber>1</groupNumber>
+                <gain>1</gain>
+                <defaultDisplayAmplitude>7.5</defaultDisplayAmplitude>
+                <highpassDisplay>0.3000000119</highpassDisplay>
+                <lowpassDisplay>70</lowpassDisplay>
+                <notchDisplay>60</notchDisplay>
+                <color>0.0000,0.0000,0.0000,1.0000</color>
+                <positiveUp>false</positiveUp>
+            </sensor>
+            <sensor>
+                <name>EMG</name>
+                <number>1</number>
+                <unit>uV</unit>
+                <psgType>0</psgType>
+                <mapping>2</mapping>
+                <samplingRate>0</samplingRate>
+                <sensorType>EMG</sensorType>
+                <highpass>10</highpass>
+                <lowpass>100</lowpass>
+                <notch>60</notch>
+                <groupNumber>1</groupNumber>
+                <gain>1</gain>
+                <defaultDisplayAmplitude>7.5</defaultDisplayAmplitude>
+                <highpassDisplay>10</highpassDisplay>
+                <lowpassDisplay>100</lowpassDisplay>
+                <notchDisplay>60</notchDisplay>
+                <color>0.0000,0.0000,0.0000,1.0000</color>
+                <positiveUp>false</positiveUp>
+            ...
+    ```
+    """
+
+    _xmlns = r'{http://www.egi.com/pnsSet_mff}'
+    _xmlroottag = r'PNSSet'
+    _default_filename = 'pnsSet.xml'
+    _sensor_type_reverter = {
+        'name': str,
+        'number': str,
+        'unit': str,
+        'psgType': str,
+        'mapping': str,
+        'samplingRate': str,
+        'sensorType': str,
+        'highpass': str,
+        'lowpass': str,
+        'notch': str,
+        'groupNumber': str,
+        'gain': str,
+        'defaultDisplayAmplitude': str,
+        'highpassDisplay': str,
+        'lowpassDisplay': str,
+        'notchDisplay': str,
+        'color': lambda color: ','.join(
+            ["{:.4f}".format(c) for c in color]
+        ),
+        'positiveUp': str
+    }
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._sensor_type_converter = {
+            'name': str,
+            'number': int,
+            'unit': str,
+            'psgType': int,
+            'mapping': int,
+            'samplingRate': int,
+            'sensorType': str,
+            'highpass': float,
+            'lowpass': float,
+            'notch': int,
+            'groupNumber': int,
+            'gain': int,
+            'defaultDisplayAmplitude': float,
+            'highpassDisplay': float,
+            'lowpassDisplay': float,
+            'notchDisplay': int,
+            'color': lambda s: list(map(float, s.split(","))),
+            'positiveUp': str,
+        }
+
+    @cached_property
+    def sensors(self) -> Dict[int, Any]:
+        return dict([
+            self._parse_sensor(sensor)
+            for sensor in self.find('sensors')
+        ])
+
+    def _parse_sensor(self, el) -> Tuple[int, Any]:
+        assert self.nsstrip(el.tag) == 'sensor', f"""
+        Unknown sensor with tag '{self.nsstrip(el.tag)}'"""
+        ans = {}
+        for e in el:
+            tag = self.nsstrip(e.tag)
+            ans[tag] = self._sensor_type_converter[tag](e.text)
+        return ans['number'], ans
+
+    @cached_property
+    def name(self) -> str:
+        """return value of the name tag"""
+        return self.find('name').text
+
+    @cached_property
+    def amp_series(self) -> str:
+        """return value of the ampSeries tag"""
+        return self.find('ampSeries').text
+
+    def get_content(self) -> Dict[str, Any]:
+        """return properties of the sensor
+        set read from the .xml"""
+        return {
+            'name': self.name,
+            'ampSeries': self.amp_series,
+            'sensors': self.sensors
+        }
+
+    def get_serializable_content(self) -> Dict[str, Any]:
+        """return a serializable object containing the
+        properties of the sensor set read from the .xml"""
+        return copy.deepcopy(self.get_content())
+
+    @classmethod
+    def content(cls, name: str, amp_series: str,  # type: ignore
+                sensors: Dict[int, Any]) -> Dict[str, Any]:
+        """return content in xml-convertible json format"""
+        formatted_sensors = []
+        for sensor in sensors.values():
+            formatted = {}
+            for k, v in sensor.items():
+                assert k in cls._sensor_type_reverter, "sensor property "
+                f"'{k}' not serializable. Needs to be on of "
+                "{list(cls._sensor_type_reverter.keys())}"
+                formatted[k] = {
+                    TEXT: cls._sensor_type_reverter[k](v)  # type: ignore
+                }
+            formatted_sensors.append({TEXT: formatted})
+        return {
+            'name': {TEXT: name},
+            'ampSeries': {TEXT: amp_series},
+            'sensors': {TEXT: {'sensor': formatted_sensors}},
+        }
+
+
 class History(XML):
     """Parser for 'history.xml' files
 
     These files have the following structure:
     ```
     <?xml version="1.0" encoding="UTF-8" standalone="yes" ?>
     <historyEntries xmlns="http://www.egi.com/history_mff"
```

### Comparing `mffpy-0.8.0/mffpy/zipfile.py` & `mffpy-0.9.0/mffpy/zipfile.py`

 * *Files identical despite different names*

### Comparing `mffpy-0.8.0/mffpy.egg-info/PKG-INFO` & `mffpy-0.9.0/mffpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: mffpy
-Version: 0.8.0
+Version: 0.9.0
 Summary: Reader and Writer for Philips' MFF file format.
-Home-page: https://github.com/BEL-Public/mffpy
 Author: Justus Schwabedal, Wayne Manselle
 Author-email: jschwabedal@belco.tech, wayne.manselle@belco.tech
 Maintainer: Evan Hathaway
 Maintainer-email: evan.hathaway@belco.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: lxml>=4.8.0
+Requires-Dist: pytz>=2019.2
+Requires-Dist: numpy>=1.15.1
+Requires-Dist: Deprecated>=1.2.12
 
 # Introduction
 
 [![Github Actions](https://github.com/BEL-Public/mffpy/workflows/lint-and-test/badge.svg)
 ](https://github.com/BEL-Public/mffpy/actions)
 
 `mffpy` is a lean reader for EGI's MFF file format.  These files are
@@ -48,26 +51,26 @@
 ### Test Coverage
 
 ```
 ============================= test session starts ==============================
 platform linux -- Python 3.6.7, pytest-7.0.1, pluggy-1.0.0
 rootdir: /home/runner/work/mffpy/mffpy
 plugins: cov-4.0.0
-collected 122 items
+collected 123 items
 
 mffpy/tests/test_cached_property.py ..                                   [  1%]
 mffpy/tests/test_devices.py .............                                [ 12%]
 mffpy/tests/test_dict2xml.py .                                           [ 13%]
 mffpy/tests/test_header_block.py ..                                      [ 14%]
-mffpy/tests/test_mffdir.py ....                                          [ 18%]
+mffpy/tests/test_mffdir.py ....                                          [ 17%]
 mffpy/tests/test_raw_bin_files.py ..................                     [ 32%]
 mffpy/tests/test_reader.py ......................                        [ 50%]
 mffpy/tests/test_writer.py ...........                                   [ 59%]
-mffpy/tests/test_xml_files.py .......................................... [ 94%]
-..                                                                       [ 95%]
+mffpy/tests/test_xml_files.py .......................................... [ 93%]
+...                                                                      [ 95%]
 mffpy/tests/test_zipfile.py .....                                        [100%]
 
 ----------- coverage: platform linux, python 3.6.7-final-0 -----------
 Name                                          Stmts   Miss  Cover
 -----------------------------------------------------------------
 mffpy/__init__.py                                 4      0   100%
 mffpy/bin_files.py                               40      2    95%
@@ -80,31 +83,31 @@
 mffpy/header_block/header_block.py               48      2    96%
 mffpy/header_block/helpers.py                    15      0   100%
 mffpy/header_block/optional_header_block.py      32      1    97%
 mffpy/mffdir.py                                  92      7    92%
 mffpy/raw_bin_files.py                          113      0   100%
 mffpy/reader.py                                 110      2    98%
 mffpy/tests/__init__.py                           0      0   100%
-mffpy/tests/conftest.py                          11      0   100%
+mffpy/tests/conftest.py                          15      0   100%
 mffpy/tests/test_cached_property.py              33      0   100%
 mffpy/tests/test_devices.py                      12      0   100%
 mffpy/tests/test_dict2xml.py                     16      0   100%
 mffpy/tests/test_header_block.py                 33      0   100%
 mffpy/tests/test_mffdir.py                       30      0   100%
 mffpy/tests/test_raw_bin_files.py                63      0   100%
 mffpy/tests/test_reader.py                       96      0   100%
-mffpy/tests/test_writer.py                      204      0   100%
-mffpy/tests/test_xml_files.py                   202      1    99%
+mffpy/tests/test_writer.py                      212      0   100%
+mffpy/tests/test_xml_files.py                   214      1    99%
 mffpy/tests/test_zipfile.py                      34      0   100%
 mffpy/version.py                                  1      0   100%
 mffpy/writer.py                                  71      0   100%
-mffpy/xml_files.py                              554     18    97%
+mffpy/xml_files.py                              607     22    96%
 mffpy/zipfile.py                                 47      0   100%
 -----------------------------------------------------------------
-TOTAL                                          2023     40    98%
+TOTAL                                          2100     44    98%
 
 
 ============================= 122 passed in 7.19s ==============================
 ```
 
 ## View the Docs
```

### Comparing `mffpy-0.8.0/mffpy.egg-info/SOURCES.txt` & `mffpy-0.9.0/mffpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
-pyproject.toml
 requirements.txt
-setup.cfg
 setup.py
 ./bin/mff2json.py
 ./bin/mff2mfz.py
 ./bin/mffdiff.py
 mffpy/__init__.py
 mffpy/bin_files.py
 mffpy/bin_writer.py
```

### Comparing `mffpy-0.8.0/setup.py` & `mffpy-0.9.0/setup.py`

 * *Files identical despite different names*


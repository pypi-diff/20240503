# Comparing `tmp/alyx_registrator-0.0.3.tar.gz` & `tmp/alyx_registrator-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alyx_registrator-0.0.3.tar", last modified: Tue Apr 23 09:49:27 2024, max compression
+gzip compressed data, was "alyx_registrator-0.0.4.tar", last modified: Fri May  3 09:58:13 2024, max compression
```

## Comparing `alyx_registrator-0.0.3.tar` & `alyx_registrator-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6234 2024-04-23 09:49:18.258678 alyx_registrator-0.0.3/one_registrator/README.md
--rw-r--r--   0        0        0       51 2024-04-23 09:49:18.258678 alyx_registrator-0.0.3/one_registrator/__init__.py
--rw-r--r--   0        0        0    28212 2024-04-23 09:49:18.262678 alyx_registrator-0.0.3/one_registrator/registration.py
--rw-r--r--   0        0        0    11125 2024-04-23 09:49:18.262678 alyx_registrator-0.0.3/one_registrator/rules.json
--rw-r--r--   0        0        0     2904 2024-04-23 09:49:18.262678 alyx_registrator-0.0.3/one_registrator/utils.py
--rw-r--r--   0        0        0      660 2024-04-23 09:49:27.506533 alyx_registrator-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      342 1970-01-01 00:00:00.000000 alyx_registrator-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6234 2024-05-03 09:58:04.603888 alyx_registrator-0.0.4/one_registrator/README.md
+-rw-r--r--   0        0        0       51 2024-05-03 09:58:04.603888 alyx_registrator-0.0.4/one_registrator/__init__.py
+-rw-r--r--   0        0        0    28212 2024-05-03 09:58:04.603888 alyx_registrator-0.0.4/one_registrator/registration.py
+-rw-r--r--   0        0        0    12095 2024-05-03 09:58:04.603888 alyx_registrator-0.0.4/one_registrator/rules.json
+-rw-r--r--   0        0        0     2904 2024-05-03 09:58:04.603888 alyx_registrator-0.0.4/one_registrator/utils.py
+-rw-r--r--   0        0        0      660 2024-05-03 09:58:13.759749 alyx_registrator-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      342 1970-01-01 00:00:00.000000 alyx_registrator-0.0.4/PKG-INFO
```

### Comparing `alyx_registrator-0.0.3/one_registrator/README.md` & `alyx_registrator-0.0.4/one_registrator/README.md`

 * *Files identical despite different names*

### Comparing `alyx_registrator-0.0.3/one_registrator/registration.py` & `alyx_registrator-0.0.4/one_registrator/registration.py`

 * *Files identical despite different names*

### Comparing `alyx_registrator-0.0.3/one_registrator/rules.json` & `alyx_registrator-0.0.4/one_registrator/rules.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9942978395061729%*

 * *Differences: {"'rules'": "{'intrinsic_imaging_vessels_rule1': {'if': {'object': {'contain': {insert: [(1, "*

 * *            "'green'), (2, 'Green'), (3, 'FOV'), (4, 'fov')]}}}}, "*

 * *            "'intrinsic_imaging_exclude_versions_rule1': {'overrides': {insert: [(3, "*

 * *            "'intrinsic_imaging_alredy_renamed_versions_rule1')]}}, "*

 * *            "'intrinsic_imaging_alredy_renamed_versions_rule1': OrderedDict([('if', "*

 * *            "OrderedDict([('collection', OrderedDict([('exact', ['intrinsic_optical_imaging'])])), "*

 * *      […]*

```diff
@@ -270,14 +270,48 @@
             "on": {
                 "match": "include"
             },
             "overrides": [
                 "imaging_data_rule1"
             ]
         },
+        "intrinsic_imaging_alredy_renamed_versions_rule1": {
+            "if": {
+                "attribute": {
+                    "exact": [
+                        "delta_stim_images",
+                        "bin_delta_stim_images",
+                        "vessels_reference"
+                    ]
+                },
+                "collection": {
+                    "exact": [
+                        "intrinsic_optical_imaging"
+                    ]
+                },
+                "extension": {
+                    "exact": [
+                        "binlv",
+                        "tdms",
+                        "tiff"
+                    ]
+                },
+                "object": {
+                    "exact": "imaging_intrinsic"
+                }
+            },
+            "on": {
+                "match": "include"
+            },
+            "overrides": [
+                "intrinsic_imaging_binaries_rule1",
+                "intrinsic_imaging_vessels_rule1",
+                "intrinsic_imaging_tdms_rule1"
+            ]
+        },
         "intrinsic_imaging_binaries_rule1": {
             "if": {
                 "collection": {
                     "exact": [
                         "intrinsic_optical_imaging",
                         "IOI"
                     ]
@@ -320,15 +354,16 @@
             },
             "on": {
                 "match": "exclude"
             },
             "overrides": [
                 "intrinsic_imaging_binaries_rule1",
                 "intrinsic_imaging_vessels_rule1",
-                "intrinsic_imaging_tdms_rule1"
+                "intrinsic_imaging_tdms_rule1",
+                "intrinsic_imaging_alredy_renamed_versions_rule1"
             ]
         },
         "intrinsic_imaging_tdms_rule1": {
             "if": {
                 "collection": {
                     "exact": [
                         "intrinsic_optical_imaging",
@@ -361,15 +396,19 @@
                 },
                 "extension": [
                     "",
                     "tiff"
                 ],
                 "object": {
                     "contain": [
-                        "reference"
+                        "reference",
+                        "green",
+                        "Green",
+                        "FOV",
+                        "fov"
                     ]
                 }
             },
             "on": {
                 "match": "rename"
             },
             "rename": {
```

### Comparing `alyx_registrator-0.0.3/one_registrator/utils.py` & `alyx_registrator-0.0.4/one_registrator/utils.py`

 * *Files identical despite different names*

### Comparing `alyx_registrator-0.0.3/pyproject.toml` & `alyx_registrator-0.0.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 dependencies = [
     "numpy>=1.23",
     "alyx-connector>=1.16",
     "pandas>=1.4",
 ]
 requires-python = ">=3.11"
 dynamic = []
-version = "0.0.3"
+version = "0.0.4"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```


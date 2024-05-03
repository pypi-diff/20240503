# Comparing `tmp/nmuwd-0.0.3.tar.gz` & `tmp/nmuwd-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmuwd-0.0.3.tar", last modified: Fri May  3 07:04:59 2024, max compression
+gzip compressed data, was "nmuwd-0.0.4.tar", last modified: Fri May  3 07:06:36 2024, max compression
```

## Comparing `nmuwd-0.0.3.tar` & `nmuwd-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:04:59.118918 nmuwd-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 07:04:53.000000 nmuwd-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-03 07:04:59.118918 nmuwd-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 07:04:53.000000 nmuwd-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:04:59.118918 nmuwd-0.0.3/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:04:53.000000 nmuwd-0.0.3/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-03 07:04:53.000000 nmuwd-0.0.3/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-03 07:04:53.000000 nmuwd-0.0.3/backend/persister.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-03 07:04:53.000000 nmuwd-0.0.3/backend/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-03 07:04:53.000000 nmuwd-0.0.3/backend/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-03 07:04:53.000000 nmuwd-0.0.3/backend/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:04:59.118918 nmuwd-0.0.3/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:04:53.000000 nmuwd-0.0.3/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-03 07:04:53.000000 nmuwd-0.0.3/frontend/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-03 07:04:53.000000 nmuwd-0.0.3/frontend/unifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:04:59.118918 nmuwd-0.0.3/nmuwd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-03 07:04:59.000000 nmuwd-0.0.3/nmuwd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-03 07:04:59.000000 nmuwd-0.0.3/nmuwd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 07:04:59.000000 nmuwd-0.0.3/nmuwd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 07:04:59.000000 nmuwd-0.0.3/nmuwd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 07:04:59.000000 nmuwd-0.0.3/nmuwd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 07:04:59.118918 nmuwd-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-03 07:04:53.000000 nmuwd-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:06:36.265829 nmuwd-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 07:06:32.000000 nmuwd-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 07:06:36.265829 nmuwd-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 07:06:32.000000 nmuwd-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:06:36.265829 nmuwd-0.0.4/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:06:32.000000 nmuwd-0.0.4/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-03 07:06:32.000000 nmuwd-0.0.4/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-03 07:06:32.000000 nmuwd-0.0.4/backend/persister.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-03 07:06:32.000000 nmuwd-0.0.4/backend/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-03 07:06:32.000000 nmuwd-0.0.4/backend/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-03 07:06:32.000000 nmuwd-0.0.4/backend/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:06:36.265829 nmuwd-0.0.4/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:06:32.000000 nmuwd-0.0.4/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-03 07:06:32.000000 nmuwd-0.0.4/frontend/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-03 07:06:32.000000 nmuwd-0.0.4/frontend/unifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:06:36.265829 nmuwd-0.0.4/nmuwd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 07:06:36.000000 nmuwd-0.0.4/nmuwd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-03 07:06:36.000000 nmuwd-0.0.4/nmuwd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 07:06:36.000000 nmuwd-0.0.4/nmuwd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 07:06:36.000000 nmuwd-0.0.4/nmuwd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 07:06:36.000000 nmuwd-0.0.4/nmuwd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 07:06:36.265829 nmuwd-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-03 07:06:32.000000 nmuwd-0.0.4/setup.py
```

### Comparing `nmuwd-0.0.3/LICENSE` & `nmuwd-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.3/backend/config.py` & `nmuwd-0.0.4/backend/config.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.3/backend/persister.py` & `nmuwd-0.0.4/backend/persister.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.3/backend/record.py` & `nmuwd-0.0.4/backend/record.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,23 +34,25 @@
             return v
 
         return [get(k) for k in self.keys]
 
     def __getattr__(self, k):
         return self._payload.get(k)
 
+
 class WaterLevelRecord(BaseRecord):
     keys = (
         "source",
         "id",
         "depth_to_water_below_ground_surface_ft",
         "date_measured",
-        "time_measured"
+        "time_measured",
     )
-    defaults ={}
+    defaults = {}
+
 
 class SiteRecord(BaseRecord):
     keys = (
         "source",
         "id",
         "name",
         "latitude",
@@ -76,9 +78,8 @@
         "vertical_datum": "",
         "usgs_site_id": "",
         "alternate_site_id": "",
         "formation": "",
     }
 
 
-
 # ============= EOF =============================================
```

### Comparing `nmuwd-0.0.3/backend/source.py` & `nmuwd-0.0.4/backend/source.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.3/backend/transformer.py` & `nmuwd-0.0.4/backend/transformer.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.3/frontend/cli.py` & `nmuwd-0.0.4/frontend/cli.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.3/frontend/unifier.py` & `nmuwd-0.0.4/frontend/unifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,22 +67,20 @@
                 persister.records.append(wl)
 
     if config.use_source_nwis:
         pass
 
     persister.save(config.output_path)
 
-
     # if config.use_source_isc_seven_rivers:
     #     isc = ISCSevenRiversSiteSource()
     #     persister.load(isc.read(config))
     #
     # if config.use_source_nwis:
     #     nwis = USGSSiteSource()
     #     persister.load(nwis.read(config))
 
 
-
 if __name__ == "__main__":
     unify_sites()
 
 # ============= EOF =============================================
```

### Comparing `nmuwd-0.0.3/setup.py` & `nmuwd-0.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="nmuwd",
-    version="0.0.3",
+    version="0.0.4",
     author="Jake Ross",
     description="New Mexico Water Data Integration Engine",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/PychronLabsLLC/pcm",
+    url="https://github.com/DataIntegrationGroup/PyWeaver",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     install_requires=[],
     entry_points={
         "console_scripts": [
```


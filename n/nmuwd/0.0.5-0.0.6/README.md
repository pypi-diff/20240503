# Comparing `tmp/nmuwd-0.0.5.tar.gz` & `tmp/nmuwd-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmuwd-0.0.5.tar", last modified: Fri May  3 15:24:26 2024, max compression
+gzip compressed data, was "nmuwd-0.0.6.tar", last modified: Fri May  3 15:42:08 2024, max compression
```

## Comparing `nmuwd-0.0.5.tar` & `nmuwd-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:24:26.623248 nmuwd-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 15:24:21.000000 nmuwd-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 15:24:26.619248 nmuwd-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 15:24:21.000000 nmuwd-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:24:26.619248 nmuwd-0.0.5/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:24:21.000000 nmuwd-0.0.5/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-03 15:24:21.000000 nmuwd-0.0.5/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-03 15:24:21.000000 nmuwd-0.0.5/backend/persister.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-03 15:24:21.000000 nmuwd-0.0.5/backend/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-03 15:24:21.000000 nmuwd-0.0.5/backend/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-03 15:24:21.000000 nmuwd-0.0.5/backend/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:24:26.619248 nmuwd-0.0.5/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:24:21.000000 nmuwd-0.0.5/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-03 15:24:21.000000 nmuwd-0.0.5/frontend/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-03 15:24:21.000000 nmuwd-0.0.5/frontend/unifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:24:26.619248 nmuwd-0.0.5/nmuwd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 15:24:26.000000 nmuwd-0.0.5/nmuwd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-03 15:24:26.000000 nmuwd-0.0.5/nmuwd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:24:26.000000 nmuwd-0.0.5/nmuwd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 15:24:26.000000 nmuwd-0.0.5/nmuwd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 15:24:26.000000 nmuwd-0.0.5/nmuwd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:24:26.623248 nmuwd-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-03 15:24:21.000000 nmuwd-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:42:08.147935 nmuwd-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 15:42:04.000000 nmuwd-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 15:42:08.147935 nmuwd-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 15:42:04.000000 nmuwd-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:42:08.143935 nmuwd-0.0.6/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:42:04.000000 nmuwd-0.0.6/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-03 15:42:04.000000 nmuwd-0.0.6/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-03 15:42:04.000000 nmuwd-0.0.6/backend/persister.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-03 15:42:04.000000 nmuwd-0.0.6/backend/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-03 15:42:04.000000 nmuwd-0.0.6/backend/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-03 15:42:04.000000 nmuwd-0.0.6/backend/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:42:08.147935 nmuwd-0.0.6/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:42:04.000000 nmuwd-0.0.6/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-03 15:42:04.000000 nmuwd-0.0.6/frontend/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-03 15:42:04.000000 nmuwd-0.0.6/frontend/unifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:42:08.147935 nmuwd-0.0.6/nmuwd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 15:42:08.000000 nmuwd-0.0.6/nmuwd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-03 15:42:08.000000 nmuwd-0.0.6/nmuwd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:42:08.000000 nmuwd-0.0.6/nmuwd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 15:42:08.000000 nmuwd-0.0.6/nmuwd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 15:42:08.000000 nmuwd-0.0.6/nmuwd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:42:08.147935 nmuwd-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-03 15:42:04.000000 nmuwd-0.0.6/setup.py
```

### Comparing `nmuwd-0.0.5/LICENSE` & `nmuwd-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.5/backend/config.py` & `nmuwd-0.0.6/backend/config.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.5/backend/persister.py` & `nmuwd-0.0.6/backend/persister.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.5/backend/record.py` & `nmuwd-0.0.6/backend/record.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,15 +39,17 @@
         return self._payload.get(k)
 
 
 class WaterLevelRecord(BaseRecord):
     keys = (
         "source",
         "id",
-        "depth_to_water_below_ground_surface_ft",
+        "surface_elevation_ft",
+        "well_depth_ft_below_ground_surface",
+        "depth_to_water_ft_below_ground_surface",
         "date_measured",
         "time_measured",
     )
     defaults = {}
 
 
 class SiteRecord(BaseRecord):
```

### Comparing `nmuwd-0.0.5/backend/source.py` & `nmuwd-0.0.6/backend/source.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.5/backend/transformer.py` & `nmuwd-0.0.6/backend/transformer.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===============================================================================
 
 
 class BaseTransformer:
-    def transform(self, record, config, *args, **kw):
+    def transform(self, *args, **kw):
         raise NotImplementedError
 
 
 # ============= EOF =============================================
```

### Comparing `nmuwd-0.0.5/frontend/cli.py` & `nmuwd-0.0.6/frontend/cli.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.5/frontend/unifier.py` & `nmuwd-0.0.6/frontend/unifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===============================================================================
 from backend.config import Config
 from backend.connectors.ampapi.source import AMPAPISiteSource, AMPAPIWaterLevelSource
-from backend.connectors.isc_seven_rivers.source import ISCSevenRiversSiteSource, ISCSevenRiversWaterLevelSource
+from backend.connectors.isc_seven_rivers.source import (
+    ISCSevenRiversSiteSource,
+    ISCSevenRiversWaterLevelSource,
+)
 from backend.connectors.usgs.source import USGSSiteSource
 from backend.persister import CSVPersister, GeoJSONPersister
 from backend.record import SiteRecord, WaterLevelRecord
 
 
 def perister_factory(config, record_klass):
     persister_klass = CSVPersister
@@ -80,10 +83,10 @@
     #     nwis = USGSSiteSource()
     #     persister.load(nwis.read(config))
 
 
 if __name__ == "__main__":
     cfg = Config()
     cfg.bbox = "-106.5 32.5, -106.0 33.0"
-    unify_sites(cfg)
+    unify_waterlevels(cfg)
 
 # ============= EOF =============================================
```

### Comparing `nmuwd-0.0.5/setup.py` & `nmuwd-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="nmuwd",
-    version="0.0.5",
+    version="0.0.6",
     author="Jake Ross",
     description="New Mexico Water Data Integration Engine",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DataIntegrationGroup/PyWeaver",
     classifiers=[
         "Programming Language :: Python :: 3",
```


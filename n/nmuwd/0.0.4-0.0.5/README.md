# Comparing `tmp/nmuwd-0.0.4.tar.gz` & `tmp/nmuwd-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmuwd-0.0.4.tar", last modified: Fri May  3 07:06:36 2024, max compression
+gzip compressed data, was "nmuwd-0.0.5.tar", last modified: Fri May  3 15:24:26 2024, max compression
```

## Comparing `nmuwd-0.0.4.tar` & `nmuwd-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:06:36.265829 nmuwd-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 07:06:32.000000 nmuwd-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 07:06:36.265829 nmuwd-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 07:06:32.000000 nmuwd-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:06:36.265829 nmuwd-0.0.4/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:06:32.000000 nmuwd-0.0.4/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-03 07:06:32.000000 nmuwd-0.0.4/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-03 07:06:32.000000 nmuwd-0.0.4/backend/persister.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-03 07:06:32.000000 nmuwd-0.0.4/backend/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-03 07:06:32.000000 nmuwd-0.0.4/backend/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-03 07:06:32.000000 nmuwd-0.0.4/backend/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:06:36.265829 nmuwd-0.0.4/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:06:32.000000 nmuwd-0.0.4/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-03 07:06:32.000000 nmuwd-0.0.4/frontend/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-03 07:06:32.000000 nmuwd-0.0.4/frontend/unifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:06:36.265829 nmuwd-0.0.4/nmuwd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 07:06:36.000000 nmuwd-0.0.4/nmuwd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-03 07:06:36.000000 nmuwd-0.0.4/nmuwd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 07:06:36.000000 nmuwd-0.0.4/nmuwd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 07:06:36.000000 nmuwd-0.0.4/nmuwd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 07:06:36.000000 nmuwd-0.0.4/nmuwd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 07:06:36.265829 nmuwd-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-03 07:06:32.000000 nmuwd-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:24:26.623248 nmuwd-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 15:24:21.000000 nmuwd-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 15:24:26.619248 nmuwd-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 15:24:21.000000 nmuwd-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:24:26.619248 nmuwd-0.0.5/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:24:21.000000 nmuwd-0.0.5/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-03 15:24:21.000000 nmuwd-0.0.5/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-03 15:24:21.000000 nmuwd-0.0.5/backend/persister.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-03 15:24:21.000000 nmuwd-0.0.5/backend/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-03 15:24:21.000000 nmuwd-0.0.5/backend/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-03 15:24:21.000000 nmuwd-0.0.5/backend/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:24:26.619248 nmuwd-0.0.5/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:24:21.000000 nmuwd-0.0.5/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-03 15:24:21.000000 nmuwd-0.0.5/frontend/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-03 15:24:21.000000 nmuwd-0.0.5/frontend/unifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:24:26.619248 nmuwd-0.0.5/nmuwd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 15:24:26.000000 nmuwd-0.0.5/nmuwd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-03 15:24:26.000000 nmuwd-0.0.5/nmuwd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:24:26.000000 nmuwd-0.0.5/nmuwd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 15:24:26.000000 nmuwd-0.0.5/nmuwd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 15:24:26.000000 nmuwd-0.0.5/nmuwd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:24:26.623248 nmuwd-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-03 15:24:21.000000 nmuwd-0.0.5/setup.py
```

### Comparing `nmuwd-0.0.4/LICENSE` & `nmuwd-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.4/backend/config.py` & `nmuwd-0.0.5/backend/config.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.4/backend/persister.py` & `nmuwd-0.0.5/backend/persister.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.4/backend/record.py` & `nmuwd-0.0.5/backend/record.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.4/backend/source.py` & `nmuwd-0.0.5/backend/source.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.4/backend/transformer.py` & `nmuwd-0.0.5/backend/transformer.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.4/frontend/cli.py` & `nmuwd-0.0.5/frontend/cli.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.4/frontend/unifier.py` & `nmuwd-0.0.5/frontend/unifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===============================================================================
+from backend.config import Config
 from backend.connectors.ampapi.source import AMPAPISiteSource, AMPAPIWaterLevelSource
-from backend.connectors.isc_seven_rivers.source import ISCSevenRiversSiteSource
+from backend.connectors.isc_seven_rivers.source import ISCSevenRiversSiteSource, ISCSevenRiversWaterLevelSource
 from backend.connectors.usgs.source import USGSSiteSource
 from backend.persister import CSVPersister, GeoJSONPersister
 from backend.record import SiteRecord, WaterLevelRecord
 
 
 def perister_factory(config, record_klass):
     persister_klass = CSVPersister
@@ -77,10 +78,12 @@
     #
     # if config.use_source_nwis:
     #     nwis = USGSSiteSource()
     #     persister.load(nwis.read(config))
 
 
 if __name__ == "__main__":
-    unify_sites()
+    cfg = Config()
+    cfg.bbox = "-106.5 32.5, -106.0 33.0"
+    unify_sites(cfg)
 
 # ============= EOF =============================================
```

### Comparing `nmuwd-0.0.4/setup.py` & `nmuwd-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="nmuwd",
-    version="0.0.4",
+    version="0.0.5",
     author="Jake Ross",
     description="New Mexico Water Data Integration Engine",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DataIntegrationGroup/PyWeaver",
     classifiers=[
         "Programming Language :: Python :: 3",
```


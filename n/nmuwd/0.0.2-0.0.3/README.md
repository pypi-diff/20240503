# Comparing `tmp/nmuwd-0.0.2.tar.gz` & `tmp/nmuwd-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmuwd-0.0.2.tar", last modified: Fri May  3 05:35:45 2024, max compression
+gzip compressed data, was "nmuwd-0.0.3.tar", last modified: Fri May  3 07:04:59 2024, max compression
```

## Comparing `nmuwd-0.0.2.tar` & `nmuwd-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:35:45.290938 nmuwd-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 05:35:40.000000 nmuwd-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-03 05:35:45.290938 nmuwd-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 05:35:40.000000 nmuwd-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:35:45.286938 nmuwd-0.0.2/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:35:40.000000 nmuwd-0.0.2/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-03 05:35:40.000000 nmuwd-0.0.2/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-03 05:35:40.000000 nmuwd-0.0.2/backend/persister.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-03 05:35:40.000000 nmuwd-0.0.2/backend/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-03 05:35:40.000000 nmuwd-0.0.2/backend/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-03 05:35:40.000000 nmuwd-0.0.2/backend/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:35:45.286938 nmuwd-0.0.2/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:35:40.000000 nmuwd-0.0.2/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-03 05:35:40.000000 nmuwd-0.0.2/frontend/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-03 05:35:40.000000 nmuwd-0.0.2/frontend/unifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:35:45.290938 nmuwd-0.0.2/nmuwd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-03 05:35:45.000000 nmuwd-0.0.2/nmuwd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-03 05:35:45.000000 nmuwd-0.0.2/nmuwd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 05:35:45.000000 nmuwd-0.0.2/nmuwd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 05:35:45.000000 nmuwd-0.0.2/nmuwd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 05:35:45.000000 nmuwd-0.0.2/nmuwd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 05:35:45.290938 nmuwd-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-03 05:35:40.000000 nmuwd-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:04:59.118918 nmuwd-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 07:04:53.000000 nmuwd-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-03 07:04:59.118918 nmuwd-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 07:04:53.000000 nmuwd-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:04:59.118918 nmuwd-0.0.3/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:04:53.000000 nmuwd-0.0.3/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-03 07:04:53.000000 nmuwd-0.0.3/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-03 07:04:53.000000 nmuwd-0.0.3/backend/persister.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-03 07:04:53.000000 nmuwd-0.0.3/backend/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-03 07:04:53.000000 nmuwd-0.0.3/backend/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-03 07:04:53.000000 nmuwd-0.0.3/backend/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:04:59.118918 nmuwd-0.0.3/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:04:53.000000 nmuwd-0.0.3/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-03 07:04:53.000000 nmuwd-0.0.3/frontend/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-03 07:04:53.000000 nmuwd-0.0.3/frontend/unifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:04:59.118918 nmuwd-0.0.3/nmuwd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-03 07:04:59.000000 nmuwd-0.0.3/nmuwd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-03 07:04:59.000000 nmuwd-0.0.3/nmuwd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 07:04:59.000000 nmuwd-0.0.3/nmuwd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 07:04:59.000000 nmuwd-0.0.3/nmuwd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 07:04:59.000000 nmuwd-0.0.3/nmuwd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 07:04:59.118918 nmuwd-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-03 07:04:53.000000 nmuwd-0.0.3/setup.py
```

### Comparing `nmuwd-0.0.2/LICENSE` & `nmuwd-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.2/backend/config.py` & `nmuwd-0.0.3/backend/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,16 +17,20 @@
 
 class Config:
     bbox = None
     output_path = "output"
     use_csv = True
     use_geojson = False
     use_source_ampapi = True
-    use_source_isc_seven_rivers = True
-    use_source_nwis = True
+
+    # use_source_isc_seven_rivers = True
+    # use_source_nwis = True
+
+    use_source_isc_seven_rivers = False
+    use_source_nwis = False
 
     def bounding_points(self):
         p1, p2 = self.bbox.split(",")
         x1, y1 = [float(a) for a in p1.strip().split(" ")]
         x2, y2 = [float(a) for a in p2.strip().split(" ")]
 
         if x1 > x2:
```

### Comparing `nmuwd-0.0.2/backend/persister.py` & `nmuwd-0.0.3/backend/persister.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,19 @@
     def log(self, msg, fg="yellow"):
         click.secho(f"{self.__class__.__name__:30s}{msg}", fg=fg)
 
 
 class BasePersister(Loggable):
     extension = None
 
-    def __init__(self):
+    def __init__(self, record_klass):
         self.records = []
 
+        self.keys = record_klass.keys
+
     def load(self, records):
         self.records.extend(records)
 
     def save(self, path):
         path = self.add_extension(path)
         self.log(f"saving to {path}")
         self._save(path)
@@ -59,24 +61,24 @@
 class CSVPersister(BasePersister):
     extension = "csv"
 
     def _save(self, path):
         path = self.add_extension(path)
         with open(path, "w") as f:
             writer = csv.writer(f)
-            writer.writerow(SiteRecord.keys)
+            writer.writerow(self.keys)
             for record in self.records:
                 writer.writerow(record.to_row())
 
 
 class GeoJSONPersister(BasePersister):
     extension = "geojson"
 
     def _save(self, path):
-        df = pd.DataFrame([r.to_row() for r in self.records], columns=SiteRecord.keys)
+        df = pd.DataFrame([r.to_row() for r in self.records], columns=self.keys)
 
         gdf = gpd.GeoDataFrame(
             df, geometry=gpd.points_from_xy(df.longitude, df.latitude), crs="EPSG:4326"
         )
         gdf.to_file(path, driver="GeoJSON")
```

### Comparing `nmuwd-0.0.2/backend/record.py` & `nmuwd-0.0.3/backend/record.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,42 @@
 # ===============================================================================
 
 
 class BaseRecord:
     def to_csv(self):
         raise NotImplementedError
 
+    def __init__(self, payload):
+        self._payload = payload
+
+    def to_row(self):
+
+        def get(attr):
+            v = self._payload.get(attr)
+            if attr == "elevation" and v is not None:
+                v = round(v, 2)
+
+            if v is None:
+                v = self.defaults.get(attr)
+            return v
+
+        return [get(k) for k in self.keys]
+
+    def __getattr__(self, k):
+        return self._payload.get(k)
+
+class WaterLevelRecord(BaseRecord):
+    keys = (
+        "source",
+        "id",
+        "depth_to_water_below_ground_surface_ft",
+        "date_measured",
+        "time_measured"
+    )
+    defaults ={}
 
 class SiteRecord(BaseRecord):
     keys = (
         "source",
         "id",
         "name",
         "latitude",
@@ -47,25 +75,10 @@
         "horizontal_datum": "",
         "vertical_datum": "",
         "usgs_site_id": "",
         "alternate_site_id": "",
         "formation": "",
     }
 
-    def __init__(self, payload):
-        self._payload = payload
-
-    def to_row(self):
-
-        def get(attr):
-            v = self._payload.get(attr)
-            if attr == "elevation" and v is not None:
-                v = round(v, 2)
-
-            if v is None:
-                v = self.defaults.get(attr)
-            return v
-
-        return [get(k) for k in self.keys]
 
 
 # ============= EOF =============================================
```

### Comparing `nmuwd-0.0.2/backend/source.py` & `nmuwd-0.0.3/backend/source.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,23 +24,23 @@
 
     def __init__(self):
         self.transformer = self.transformer_klass()
 
     def log(self, msg):
         click.secho(f"{self.__class__.__name__:30s} {msg}", fg="yellow")
 
-    def read(self, config):
+    def read(self, config, *args, **kw):
         self.log("Gathering records")
         n = 0
         for record in self.get_records(config):
             record = self.transformer.transform(record, config)
             if record:
                 n += 1
                 yield record
 
         self.log(f"nrecords={n}")
 
-    def get_records(self, config):
+    def get_records(self, *args, **kw):
         raise NotImplementedError
 
 
 # ============= EOF =============================================
```

### Comparing `nmuwd-0.0.2/backend/transformer.py` & `nmuwd-0.0.3/backend/transformer.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===============================================================================
 
 
 class BaseTransformer:
-    def transform(self, record, config):
+    def transform(self, record, config, *args, **kw):
         raise NotImplementedError
 
 
 # ============= EOF =============================================
```

### Comparing `nmuwd-0.0.2/frontend/cli.py` & `nmuwd-0.0.3/frontend/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 @cli.command()
 @click.option(
     "--bbox",
     default="",
     help="Bounding box in the form 'x1 y1, x2 y2'",
 )
-def locations(bbox):
+def wells(bbox):
     """
     Get locations
     """
 
     click.echo(f"Getting locations for bounding box {bbox}")
 
     config = Config()
@@ -50,14 +50,16 @@
     default="",
     help="Bounding box in the form 'x1 y1, x2 y2'",
 )
 def waterlevels(bbox):
     click.echo(f"Getting waterlevels for bounding box {bbox}")
 
     config = Config()
+    # bbox = -107.468262,33.979809,-107.053528,34.191358
     # bbox = -105.396826 36.219290, -106.024162 35.384307
+    # bbox = -107.266538 34.098781,-107.233107 34.114967
     config.bbox = bbox
 
     unify_waterlevels(config)
 
 
 # ============= EOF =============================================
```

### Comparing `nmuwd-0.0.2/setup.py` & `nmuwd-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="nmuwd",
-    version="0.0.2",
+    version="0.0.3",
     author="Jake Ross",
     description="New Mexico Water Data Integration Engine",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PychronLabsLLC/pcm",
     classifiers=[
         "Programming Language :: Python :: 3",
```


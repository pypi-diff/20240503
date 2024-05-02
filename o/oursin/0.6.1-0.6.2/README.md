# Comparing `tmp/oursin-0.6.1.tar.gz` & `tmp/oursin-0.6.2.tar.gz`

## Comparing `oursin-0.6.1.tar` & `oursin-0.6.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oursin-0.6.1/setup.cfg
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/__about__.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/__init__.py
--rw-r--r--   0        0        0    11473 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/camera.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/client.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/custom.py
--rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/dock.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/lines.py
--rw-r--r--   0        0        0     8293 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/meshes.py
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/particles.py
--rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/probes.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/renderer.py
--rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/text.py
--rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/texture.py
--rw-r--r--   0        0        0    15261 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/ui.py
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/utils.py
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/volumes.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/atlas/__init__.py
--rw-r--r--   0        0        0    11979 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/atlas/ontology.py
--rw-r--r--   0        0        0   138106 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/atlas/data/ccf25.structures.json
--rw-r--r--   0        0        0    51097 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/atlas/data/waxholm39.structures.json
--rw-r--r--   0        0        0    51097 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/atlas/data/waxholm78.structures.json
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/colors/__init__.py
--rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/colors/colors.py
--rw-r--r--   0        0        0    36410 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin/colors/xkcd_rgb.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin.egg-info/PKG-INFO
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 oursin-0.6.1/oursin.egg-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oursin-0.6.1/tests/__init__.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 oursin-0.6.1/tests/test_urchin_core.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 oursin-0.6.1/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 oursin-0.6.1/LICENSE
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 oursin-0.6.1/README.md
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 oursin-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 oursin-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oursin-0.6.2/setup.cfg
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/__about__.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/__init__.py
+-rw-r--r--   0        0        0    11473 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/camera.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/client.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/custom.py
+-rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/dock.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/lines.py
+-rw-r--r--   0        0        0     8293 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/meshes.py
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/particles.py
+-rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/probes.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/renderer.py
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/text.py
+-rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/texture.py
+-rw-r--r--   0        0        0    15261 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/ui.py
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/utils.py
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/volumes.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/atlas/__init__.py
+-rw-r--r--   0        0        0    11979 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/atlas/ontology.py
+-rw-r--r--   0        0        0   138106 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/atlas/data/ccf25.structures.json
+-rw-r--r--   0        0        0    51097 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/atlas/data/waxholm39.structures.json
+-rw-r--r--   0        0        0    51097 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/atlas/data/waxholm78.structures.json
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/colors/__init__.py
+-rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/colors/colors.py
+-rw-r--r--   0        0        0    36410 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin/colors/xkcd_rgb.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 oursin-0.6.2/oursin.egg-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oursin-0.6.2/tests/__init__.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 oursin-0.6.2/tests/test_urchin_core.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 oursin-0.6.2/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 oursin-0.6.2/LICENSE
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 oursin-0.6.2/README.md
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 oursin-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 oursin-0.6.2/PKG-INFO
```

### Comparing `oursin-0.6.1/oursin/__init__.py` & `oursin-0.6.2/oursin/__init__.py`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin/camera.py` & `oursin-0.6.2/oursin/camera.py`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin/client.py` & `oursin-0.6.2/oursin/client.py`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin/custom.py` & `oursin-0.6.2/oursin/custom.py`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin/dock.py` & `oursin-0.6.2/oursin/dock.py`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin/lines.py` & `oursin-0.6.2/oursin/lines.py`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin/meshes.py` & `oursin-0.6.2/oursin/meshes.py`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin/particles.py` & `oursin-0.6.2/oursin/particles.py`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin/probes.py` & `oursin-0.6.2/oursin/probes.py`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin/renderer.py` & `oursin-0.6.2/oursin/renderer.py`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin/text.py` & `oursin-0.6.2/oursin/text.py`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin/texture.py` & `oursin-0.6.2/oursin/texture.py`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin/ui.py` & `oursin-0.6.2/oursin/ui.py`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin/utils.py` & `oursin-0.6.2/oursin/utils.py`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin/volumes.py` & `oursin-0.6.2/oursin/volumes.py`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin/atlas/ontology.py` & `oursin-0.6.2/oursin/atlas/ontology.py`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin/atlas/data/ccf25.structures.json` & `oursin-0.6.2/oursin/atlas/data/ccf25.structures.json`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin/atlas/data/waxholm39.structures.json` & `oursin-0.6.2/oursin/atlas/data/waxholm39.structures.json`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin/atlas/data/waxholm78.structures.json` & `oursin-0.6.2/oursin/atlas/data/waxholm78.structures.json`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin/colors/colors.py` & `oursin-0.6.2/oursin/colors/colors.py`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin/colors/xkcd_rgb.py` & `oursin-0.6.2/oursin/colors/xkcd_rgb.py`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/oursin.egg-info/SOURCES.txt` & `oursin-0.6.2/oursin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/tests/test_urchin_core.py` & `oursin-0.6.2/tests/test_urchin_core.py`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/.gitignore` & `oursin-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/LICENSE` & `oursin-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oursin-0.6.1/pyproject.toml` & `oursin-0.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   "Intended Audience :: Science/Research",
 ]
 dependencies = [
   "pydantic==2.6.4",
   "python-socketio[client]>=5.8, <5.11",
   "numpy>=1.23.3, <1.27.0",
   "Pillow>=9.5, <10.2",
-  "vbl-aquarium>=0.0.11",
+  "vbl-aquarium>=0.0.12",
 ]
 
 [tool.hatch.version]
 path = "oursin/__about__.py"
 
 [project.urls]
 Documentation = "https://virtualbrainlab.org/urchin/installation_and_use.html"
```

### Comparing `oursin-0.6.1/PKG-INFO` & `oursin-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: oursin
-Version: 0.6.1
+Version: 0.6.2
 Summary: Urchin - Universal Renderer Creating Helpful Images for Neuroscience Python API
 Project-URL: Documentation, https://virtualbrainlab.org/urchin/installation_and_use.html
 Project-URL: Issues, https://github.com/VirtualBrainLab/Urchin/issues
 Project-URL: Source, https://github.com/VirtualBrainLab/Urchin
 Author-email: Daniel Birman <dbirman@uw.edu>
 License-Expression: MIT
 License-File: LICENSE
@@ -21,13 +21,13 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: <3.13,>=3.8
 Requires-Dist: numpy<1.27.0,>=1.23.3
 Requires-Dist: pillow<10.2,>=9.5
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: python-socketio[client]<5.11,>=5.8
-Requires-Dist: vbl-aquarium>=0.0.11
+Requires-Dist: vbl-aquarium>=0.0.12
 Description-Content-Type: text/markdown
 
 # Urchin - Unity Renderer Creating Helpful Images for Neuroscience (Python API)
 
 More details can be found on [our website](https://virtualbrainlab.org/03_unity_neuro/01_urn_intro.html)
```


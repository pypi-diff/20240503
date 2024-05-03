# Comparing `tmp/raugraf-0.0.1.tar.gz` & `tmp/raugraf-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raugraf-0.0.1.tar", last modified: Fri May  3 10:02:49 2024, max compression
+gzip compressed data, was "raugraf-0.0.4.tar", last modified: Fri May  3 10:33:23 2024, max compression
```

## Comparing `raugraf-0.0.1.tar` & `raugraf-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 kevin     (3112) kevin     (3112)        0 2024-05-03 10:02:49.812365 raugraf-0.0.1/
-drwxrwxr-x   0 kevin     (3112) kevin     (3112)        0 2024-05-03 10:02:49.808365 raugraf-0.0.1/.github/
-drwxrwxr-x   0 kevin     (3112) kevin     (3112)        0 2024-05-03 10:02:49.808365 raugraf-0.0.1/.github/workflows/
--rw-rw-r--   0 kevin     (3112) kevin     (3112)     1189 2024-05-03 09:45:58.000000 raugraf-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 kevin     (3112) kevin     (3112)     3098 2024-04-15 16:32:48.000000 raugraf-0.0.1/.gitignore
--rw-r--r--   0 kevin     (3112) kevin     (3112)    16725 2024-01-29 16:03:49.000000 raugraf-0.0.1/LICENSE
--rw-r--r--   0 kevin     (3112) kevin     (3112)      965 2024-05-03 10:02:49.812365 raugraf-0.0.1/PKG-INFO
--rw-rw-r--   0 kevin     (3112) kevin     (3112)      381 2024-05-03 10:01:02.000000 raugraf-0.0.1/README.md
--rw-r--r--   0 kevin     (3112) kevin     (3112)      870 2024-05-03 09:55:15.000000 raugraf-0.0.1/pyproject.toml
-drwxrwxr-x   0 kevin     (3112) kevin     (3112)        0 2024-05-03 10:02:49.808365 raugraf-0.0.1/raugraf/
--rw-rw-r--   0 kevin     (3112) kevin     (3112)     1134 2024-05-03 09:57:16.000000 raugraf-0.0.1/raugraf/__init__.py
--rw-rw-r--   0 kevin     (3112) kevin     (3112)      142 2024-05-03 10:02:49.000000 raugraf-0.0.1/raugraf/_version.py
-drwxrwxr-x   0 kevin     (3112) kevin     (3112)        0 2024-05-03 10:02:49.808365 raugraf-0.0.1/raugraf/draft/
--rw-rw-r--   0 kevin     (3112) kevin     (3112)        0 2024-05-03 09:47:02.000000 raugraf-0.0.1/raugraf/draft/__init__.py
--rw-r--r--   0 kevin     (3112) kevin     (3112)     6228 2024-04-15 16:39:02.000000 raugraf-0.0.1/raugraf/draft/minimizer_diversity.py
--rw-r--r--   0 kevin     (3112) kevin     (3112)     2903 2024-03-27 13:28:07.000000 raugraf-0.0.1/raugraf/draft/syntenic_anchors.py
--rw-r--r--   0 kevin     (3112) kevin     (3112)     3960 2024-04-15 16:39:47.000000 raugraf-0.0.1/raugraf/noderadius.py
-drwxrwxr-x   0 kevin     (3112) kevin     (3112)        0 2024-05-03 10:02:49.808365 raugraf-0.0.1/raugraf.egg-info/
--rw-r--r--   0 kevin     (3112) kevin     (3112)      965 2024-05-03 10:02:49.000000 raugraf-0.0.1/raugraf.egg-info/PKG-INFO
--rw-rw-r--   0 kevin     (3112) kevin     (3112)      427 2024-05-03 10:02:49.000000 raugraf-0.0.1/raugraf.egg-info/SOURCES.txt
--rw-rw-r--   0 kevin     (3112) kevin     (3112)        1 2024-05-03 10:02:49.000000 raugraf-0.0.1/raugraf.egg-info/dependency_links.txt
--rw-rw-r--   0 kevin     (3112) kevin     (3112)       41 2024-05-03 10:02:49.000000 raugraf-0.0.1/raugraf.egg-info/entry_points.txt
--rw-rw-r--   0 kevin     (3112) kevin     (3112)       13 2024-05-03 10:02:49.000000 raugraf-0.0.1/raugraf.egg-info/requires.txt
--rw-rw-r--   0 kevin     (3112) kevin     (3112)        8 2024-05-03 10:02:49.000000 raugraf-0.0.1/raugraf.egg-info/top_level.txt
--rw-rw-r--   0 kevin     (3112) kevin     (3112)       38 2024-05-03 10:02:49.812365 raugraf-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:33:23.603609 raugraf-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:33:23.599609 raugraf-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:33:23.599609 raugraf-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-03 10:33:18.000000 raugraf-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-03 10:33:18.000000 raugraf-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-03 10:33:18.000000 raugraf-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-03 10:33:23.603609 raugraf-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-03 10:33:18.000000 raugraf-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-03 10:33:18.000000 raugraf-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:33:23.603609 raugraf-0.0.4/raugraf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-03 10:33:18.000000 raugraf-0.0.4/raugraf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 10:33:23.000000 raugraf-0.0.4/raugraf/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:33:23.603609 raugraf-0.0.4/raugraf/draft/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:33:18.000000 raugraf-0.0.4/raugraf/draft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-05-03 10:33:18.000000 raugraf-0.0.4/raugraf/draft/minimizer_diversity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-03 10:33:18.000000 raugraf-0.0.4/raugraf/draft/syntenic_anchors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-03 10:33:18.000000 raugraf-0.0.4/raugraf/noderadius.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:33:23.603609 raugraf-0.0.4/raugraf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-03 10:33:23.000000 raugraf-0.0.4/raugraf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-03 10:33:23.000000 raugraf-0.0.4/raugraf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:33:23.000000 raugraf-0.0.4/raugraf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-03 10:33:23.000000 raugraf-0.0.4/raugraf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 10:33:23.000000 raugraf-0.0.4/raugraf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 10:33:23.000000 raugraf-0.0.4/raugraf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 10:33:23.603609 raugraf-0.0.4/setup.cfg
```

### Comparing `raugraf-0.0.1/.github/workflows/python-publish.yml` & `raugraf-0.0.4/.github/workflows/python-publish.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,37 @@
-# This workflow will upload a Python Package using Twine when a release is created
-# For more information see: https://help.github.com/en/actions/language-and-framework-guides/using-python-with-github-actions#publishing-to-package-registries
-
 name: Upload Python Package
 
 on:
   push: {}
 
 jobs:
-  deploy:
+  pypi-publish:
+    name: Upload to PyPI
     runs-on: ubuntu-latest
+    environment:
+      name: pypi
+      url: https://pypi.org/project/raugraf/
+    permissions:
+      id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
     steps:
-
-    - uses: actions/checkout@v2
-      with:
-        fetch-depth: 0
-
-    - name: Set up Python
-      uses: actions/setup-python@v2
-      with:
-        python-version: '3.x'
-
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip setuptools wheel build
-
-    - name: Build and publish
-      run: |
-        python -m build --sdist --wheel --outdir dist/
-
-    - name: Publish distribution to Test PyPI
-      uses: pypa/gh-action-pypi-publish@release/v1
-      if: "!startsWith(github.ref, 'refs/tags')"
-      with:
-        password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-        repository_url: https://test.pypi.org/legacy/
-
-    - name: Publish distribution to PyPI
-      if: startsWith(github.ref, 'refs/tags')
-      uses: pypa/gh-action-pypi-publish@master
-      with:
-        password: ${{ secrets.PYPI_API_TOKEN }}
+      - name: Clone
+        uses: actions/checkout@v2
+      - name: Set up Python
+        uses: actions/setup-python@v2
+        with:
+          python-version: '3.x'
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip setuptools wheel build
+      - name: Build and publish
+        run: |
+          python -m build --sdist --wheel --outdir dist/
+      - name: Publish distribution to Test PyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
+        if: "!startsWith(github.ref, 'refs/tags')"
+        with:
+          repository_url: https://test.pypi.org/legacy/
+      - name: Publish distribution to PyPI
+        if: startsWith(github.ref, 'refs/tags')
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          print_hash: true
```

### Comparing `raugraf-0.0.1/.gitignore` & `raugraf-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `raugraf-0.0.1/LICENSE` & `raugraf-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `raugraf-0.0.1/PKG-INFO` & `raugraf-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raugraf
-Version: 0.0.1
+Version: 0.0.4
 Author-email: "K.D. Murray" <foss@kdmurray.id.au>
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Environment :: Console
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX
@@ -15,15 +15,23 @@
 Requires-Dist: tqdm
 Requires-Dist: natsort
 
 # Raugraf
 
 Pangenomic diversity metrics
 
-# Local Complexity/Node Radius
+# Install
+
+```
+pipx install raugraf
+```
+
+# Tools
+
+## Local Complexity/Node Radius
 
 ```
 raugraf local-complexity \
 	--graph mygraph.gfa \        # GFA from PGGB (or at least passed thru smooothxg and odgi)
 	--jumps 20 \                 # Traverse up to 20 nodes away from the focal node
 	--node-bed out.bedGraph      # Bedgraph of local complexity per node for each path in the pangenome
 ```
```

### Comparing `raugraf-0.0.1/pyproject.toml` & `raugraf-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `raugraf-0.0.1/raugraf/__init__.py` & `raugraf-0.0.4/raugraf/__init__.py`

 * *Files identical despite different names*

### Comparing `raugraf-0.0.1/raugraf/draft/minimizer_diversity.py` & `raugraf-0.0.4/raugraf/draft/minimizer_diversity.py`

 * *Files identical despite different names*

### Comparing `raugraf-0.0.1/raugraf/draft/syntenic_anchors.py` & `raugraf-0.0.4/raugraf/draft/syntenic_anchors.py`

 * *Files identical despite different names*

### Comparing `raugraf-0.0.1/raugraf/noderadius.py` & `raugraf-0.0.4/raugraf/noderadius.py`

 * *Files identical despite different names*

### Comparing `raugraf-0.0.1/raugraf.egg-info/PKG-INFO` & `raugraf-0.0.4/raugraf.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raugraf
-Version: 0.0.1
+Version: 0.0.4
 Author-email: "K.D. Murray" <foss@kdmurray.id.au>
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Environment :: Console
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX
@@ -15,15 +15,23 @@
 Requires-Dist: tqdm
 Requires-Dist: natsort
 
 # Raugraf
 
 Pangenomic diversity metrics
 
-# Local Complexity/Node Radius
+# Install
+
+```
+pipx install raugraf
+```
+
+# Tools
+
+## Local Complexity/Node Radius
 
 ```
 raugraf local-complexity \
 	--graph mygraph.gfa \        # GFA from PGGB (or at least passed thru smooothxg and odgi)
 	--jumps 20 \                 # Traverse up to 20 nodes away from the focal node
 	--node-bed out.bedGraph      # Bedgraph of local complexity per node for each path in the pangenome
 ```
```


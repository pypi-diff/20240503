# Comparing `tmp/catalog_builder-0.3.tar.gz` & `tmp/catalog_builder-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalog_builder-0.3.tar", last modified: Tue Mar 19 14:59:48 2024, max compression
+gzip compressed data, was "catalog_builder-0.4.tar", last modified: Fri May  3 09:29:05 2024, max compression
```

## Comparing `catalog_builder-0.3.tar` & `catalog_builder-0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-03-19 14:59:48.242787 catalog_builder-0.3/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1064 2024-03-06 14:29:44.000000 catalog_builder-0.3/LICENSE
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7214 2024-03-19 14:59:48.241787 catalog_builder-0.3/PKG-INFO
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     6551 2024-03-19 13:44:29.000000 catalog_builder-0.3/README.md
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-03-19 14:59:48.238787 catalog_builder-0.3/catalog_builder/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     4049 2024-03-19 12:53:57.000000 catalog_builder-0.3/catalog_builder/catalogs.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     4296 2024-03-19 14:59:29.000000 catalog_builder-0.3/catalog_builder/cli.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     2461 2024-03-12 15:34:10.000000 catalog_builder-0.3/catalog_builder/utils.py
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-03-19 14:59:48.240787 catalog_builder-0.3/catalog_builder.egg-info/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7214 2024-03-19 14:59:48.000000 catalog_builder-0.3/catalog_builder.egg-info/PKG-INFO
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      338 2024-03-19 14:59:48.000000 catalog_builder-0.3/catalog_builder.egg-info/SOURCES.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        1 2024-03-19 14:59:48.000000 catalog_builder-0.3/catalog_builder.egg-info/dependency_links.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       52 2024-03-19 14:59:48.000000 catalog_builder-0.3/catalog_builder.egg-info/entry_points.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       92 2024-03-19 14:59:48.000000 catalog_builder-0.3/catalog_builder.egg-info/requires.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       16 2024-03-19 14:59:48.000000 catalog_builder-0.3/catalog_builder.egg-info/top_level.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       38 2024-03-19 14:59:48.242787 catalog_builder-0.3/setup.cfg
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1040 2024-03-19 14:59:36.000000 catalog_builder-0.3/setup.py
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-03 09:29:05.537030 catalog_builder-0.4/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1064 2024-03-06 14:29:44.000000 catalog_builder-0.4/LICENSE
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7214 2024-05-03 09:29:05.536030 catalog_builder-0.4/PKG-INFO
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     6551 2024-03-19 13:44:29.000000 catalog_builder-0.4/README.md
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-03 09:29:05.533030 catalog_builder-0.4/catalog_builder/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     4400 2024-05-03 09:22:20.000000 catalog_builder-0.4/catalog_builder/catalogs.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     5698 2024-05-03 09:23:52.000000 catalog_builder-0.4/catalog_builder/cli.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     2461 2024-03-12 15:34:10.000000 catalog_builder-0.4/catalog_builder/utils.py
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-03 09:29:05.535030 catalog_builder-0.4/catalog_builder.egg-info/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7214 2024-05-03 09:29:05.000000 catalog_builder-0.4/catalog_builder.egg-info/PKG-INFO
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      338 2024-05-03 09:29:05.000000 catalog_builder-0.4/catalog_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        1 2024-05-03 09:29:05.000000 catalog_builder-0.4/catalog_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       52 2024-05-03 09:29:05.000000 catalog_builder-0.4/catalog_builder.egg-info/entry_points.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       92 2024-05-03 09:29:05.000000 catalog_builder-0.4/catalog_builder.egg-info/requires.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       16 2024-05-03 09:29:05.000000 catalog_builder-0.4/catalog_builder.egg-info/top_level.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       38 2024-05-03 09:29:05.537030 catalog_builder-0.4/setup.cfg
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1040 2024-05-03 09:25:30.000000 catalog_builder-0.4/setup.py
```

### Comparing `catalog_builder-0.3/LICENSE` & `catalog_builder-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `catalog_builder-0.3/PKG-INFO` & `catalog_builder-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: catalog_builder
-Version: 0.3
+Version: 0.4
 Summary: Data Catalogs Made Easy
-Download-URL: https://github.com/unytics/catalog_builder/archive/refs/tags/v0.3.tar.gz
+Download-URL: https://github.com/unytics/catalog_builder/archive/refs/tags/v0.4.tar.gz
 Author: Unytics
 Author-email: paul.marcombes@unytics.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `catalog_builder-0.3/README.md` & `catalog_builder-0.4/README.md`

 * *Files identical despite different names*

### Comparing `catalog_builder-0.3/catalog_builder/catalogs.py` & `catalog_builder-0.4/catalog_builder/catalogs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import shutil
 import os
+import shutil
 
 import jinja2
 import pandas as pd
 
 from .utils import CatalogException
 
-
-CATALOGS_CONF_FOLDER = 'catalogs'
+CATALOGS_CONF_FOLDER = "catalogs"
 
 
-FOLDER_TEMPLATE = jinja2.Template('''---
+FOLDER_TEMPLATE = jinja2.Template(
+    """---
 search:
   exclude: true
 ---
 
 {{ content }}
 
 {% if files_and_folders %}
@@ -28,85 +28,91 @@
     :material-folder: [{{ obj.name }}]({{ obj.name }}/index.md)<br>
     {% endif %}
     {% endfor %}
 
 </div>
 
 {% endif %}
-''')
-
+"""
+)
 
 
 class Catalog:
 
     def __init__(self, name):
         self.name = name
-        self.folder = f'{CATALOGS_CONF_FOLDER}/{name}'
-        self.generated_docs_folder = f'{self.folder}/docs'
+        self.folder = f"{CATALOGS_CONF_FOLDER}/{name}"
+        self.generated_docs_folder = f"{self.folder}/docs"
         self.load_templates()
         self._assets = None
 
     def load_templates(self):
-        template_folder = f'{self.folder}/templates'
+        template_folder = f"{self.folder}/templates"
         self.templates = {}
         if not os.path.isdir(template_folder):
             os.makedirs(template_folder)
             return
         for root, folders, files in os.walk(template_folder):
             for file in files:
-                template = open(f'{root}/{file}', encoding='utf-8').read()
+                template = open(f"{root}/{file}", encoding="utf-8").read()
                 template = jinja2.Template(template)
-                filename = f'{root}/{file}'.replace(template_folder + '/', '')
-                asset_type =  filename.replace('.md', '')
+                filename = f"{root}/{file}".replace(template_folder + "/", "")
+                asset_type = filename.replace(".md", "")
                 self.templates[asset_type] = template
 
     @property
     def assets(self):
         if self._assets is not None:
             return self._assets
-        if os.path.isfile(f'{self.folder}/assets.parquet'):
-            self._assets = pd.read_parquet(f'{self.folder}/assets.parquet')
-        elif os.path.isfile(f'{self.folder} /assets.jsonl'):
-            self._assets = pd.read_json(f'{self.folder}/assets.jsonl', lines=True)
+        if os.path.isfile(f"{self.folder}/assets.parquet"):
+            self._assets = pd.read_parquet(f"{self.folder}/assets.parquet")
+        elif os.path.isfile(f"{self.folder} /assets.jsonl"):
+            self._assets = pd.read_json(f"{self.folder}/assets.jsonl", lines=True)
         else:
-            raise CatalogException(f'Could not find any assets file. Neither `{self.folder}/assets.parquet` nor `{self.folder}/assets.jsonl` exist. Please generate the file by running `{self.folder}/generate_assets_file.py`.')
+            raise CatalogException(
+                f"Could not find any assets file. Neither `{self.folder}/assets.parquet` nor `{self.folder}/assets.jsonl` exist. Please generate the file by running `{self.folder}/generate_assets_file.py`."
+            )
         return self._assets
 
-    def generate_markdown(self):
+    def generate_markdown(self, markdown_folder_paths_to_include=None, add_children_in_folder_pages=False):
         shutil.rmtree(self.generated_docs_folder, ignore_errors=True)
-        if os.path.isdir(f'{self.folder}/source_docs'):
-            shutil.copytree(f'{self.folder}/source_docs', self.generated_docs_folder)
+        if markdown_folder_paths_to_include:
+            assert isinstance(markdown_folder_paths_to_include, list), 'markdown_folder_paths_to_include must be a list'
+            for folder in markdown_folder_paths_to_include:
+                if os.path.isdir(folder):
+                    shutil.copytree(folder, self.generated_docs_folder)
         self._generate_markdown_of_assets()
-        self._generate_markdown_of_folders()
+        if add_children_in_folder_pages:
+            self._generate_markdown_of_folders()
 
     def _generate_markdown_of_assets(self):
-        for asset in self.assets.to_dict(orient='records'):
-            if not asset['path'] or asset['asset_type'] not in self.templates:
+        for asset in self.assets.to_dict(orient="records"):
+            if not asset["path"] or asset["asset_type"] not in self.templates:
                 continue
-            template = self.templates[asset['asset_type']]
-            content = template.render(**asset['data'])
-            path = asset['path'].replace('\\', '/')
-            path = f'{self.generated_docs_folder}/{path}'
-            if not path.endswith('.md'):
-                path += '.md'
-            folder = '/'.join(path.split('/')[:-1])
+            template = self.templates[asset["asset_type"]]
+            content = template.render(**asset["data"])
+            path = asset["path"].replace("\\", "/")
+            path = f"{self.generated_docs_folder}/{path}"
+            if not path.endswith(".md"):
+                path += ".md"
+            folder = "/".join(path.split("/")[:-1])
             os.makedirs(folder, exist_ok=True)
-            with open(path, 'w', encoding='utf8') as out:
+            with open(path, "w", encoding="utf8") as out:
                 out.write(content)
 
     def _generate_markdown_of_folders(self):
         for root, folders, files in os.walk(self.generated_docs_folder):
-            if 'index.md' in files:
-                content = open(f'{root}/index.md', encoding='utf-8').read()
+            if "index.md" in files:
+                content = open(f"{root}/index.md", encoding="utf-8").read()
             else:
-                content = '# ' + os.path.basename(root).replace('_', ' ').title()
+                content = "# " + os.path.basename(root).replace("_", " ").title()
             if root == self.generated_docs_folder:
                 files_and_folders = None
             else:
-                files = [{'name': f, 'type': 'file'} for f in files if f != 'index.md']
-                folders = [{'name': f, 'type': 'folder'} for f in folders]
-                files_and_folders = sorted(files + folders, key=lambda x: x['name'])
+                files = [{"name": f, "type": "file"} for f in files if f != "index.md"]
+                folders = [{"name": f, "type": "folder"} for f in folders]
+                files_and_folders = sorted(files + folders, key=lambda x: x["name"])
             content = FOLDER_TEMPLATE.render(
                 files_and_folders=files_and_folders,
                 content=content,
             )
-            open(f'{root}/index.md', 'w', encoding='utf-8').write(content)
+            open(f"{root}/index.md", "w", encoding="utf-8").write(content)
```

### Comparing `catalog_builder-0.3/catalog_builder/utils.py` & `catalog_builder-0.4/catalog_builder/utils.py`

 * *Files identical despite different names*

### Comparing `catalog_builder-0.3/catalog_builder.egg-info/PKG-INFO` & `catalog_builder-0.4/catalog_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: catalog_builder
-Version: 0.3
+Version: 0.4
 Summary: Data Catalogs Made Easy
-Download-URL: https://github.com/unytics/catalog_builder/archive/refs/tags/v0.3.tar.gz
+Download-URL: https://github.com/unytics/catalog_builder/archive/refs/tags/v0.4.tar.gz
 Author: Unytics
 Author-email: paul.marcombes@unytics.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `catalog_builder-0.3/setup.py` & `catalog_builder-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-VERSION = '0.3'
+VERSION = '0.4'
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
```


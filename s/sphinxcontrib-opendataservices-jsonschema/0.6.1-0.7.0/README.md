# Comparing `tmp/sphinxcontrib-opendataservices-jsonschema-0.6.1.tar.gz` & `tmp/sphinxcontrib-opendataservices-jsonschema-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-opendataservices-jsonschema-0.6.1.tar", last modified: Mon Oct 23 12:29:09 2023, max compression
+gzip compressed data, was "sphinxcontrib-opendataservices-jsonschema-0.7.0.tar", last modified: Fri May  3 13:57:13 2024, max compression
```

## Comparing `sphinxcontrib-opendataservices-jsonschema-0.6.1.tar` & `sphinxcontrib-opendataservices-jsonschema-0.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-10-23 12:29:09.608865 sphinxcontrib-opendataservices-jsonschema-0.6.1/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1418 2023-08-30 14:59:22.000000 sphinxcontrib-opendataservices-jsonschema-0.6.1/LICENSE
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)       55 2023-08-30 14:59:22.000000 sphinxcontrib-opendataservices-jsonschema-0.6.1/MANIFEST.in
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2038 2023-10-23 12:29:09.608865 sphinxcontrib-opendataservices-jsonschema-0.6.1/PKG-INFO
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1013 2023-08-30 14:59:22.000000 sphinxcontrib-opendataservices-jsonschema-0.6.1/README.rst
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      266 2023-10-23 12:29:09.612865 sphinxcontrib-opendataservices-jsonschema-0.6.1/setup.cfg
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1533 2023-10-23 12:29:05.000000 sphinxcontrib-opendataservices-jsonschema-0.6.1/setup.py
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-10-23 12:29:09.608865 sphinxcontrib-opendataservices-jsonschema-0.6.1/sphinxcontrib/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)       80 2023-08-30 14:59:22.000000 sphinxcontrib-opendataservices-jsonschema-0.6.1/sphinxcontrib/__init__.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    19198 2023-10-23 12:29:05.000000 sphinxcontrib-opendataservices-jsonschema-0.6.1/sphinxcontrib/jsonschema.py
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-10-23 12:29:09.608865 sphinxcontrib-opendataservices-jsonschema-0.6.1/sphinxcontrib_opendataservices_jsonschema.egg-info/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2038 2023-10-23 12:29:09.000000 sphinxcontrib-opendataservices-jsonschema-0.6.1/sphinxcontrib_opendataservices_jsonschema.egg-info/PKG-INFO
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      632 2023-10-23 12:29:09.000000 sphinxcontrib-opendataservices-jsonschema-0.6.1/sphinxcontrib_opendataservices_jsonschema.egg-info/SOURCES.txt
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        1 2023-10-23 12:29:09.000000 sphinxcontrib-opendataservices-jsonschema-0.6.1/sphinxcontrib_opendataservices_jsonschema.egg-info/dependency_links.txt
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)       14 2023-10-23 12:29:09.000000 sphinxcontrib-opendataservices-jsonschema-0.6.1/sphinxcontrib_opendataservices_jsonschema.egg-info/namespace_packages.txt
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        1 2023-08-31 10:02:13.000000 sphinxcontrib-opendataservices-jsonschema-0.6.1/sphinxcontrib_opendataservices_jsonschema.egg-info/not-zip-safe
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)       70 2023-10-23 12:29:09.000000 sphinxcontrib-opendataservices-jsonschema-0.6.1/sphinxcontrib_opendataservices_jsonschema.egg-info/requires.txt
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)       20 2023-10-23 12:29:09.000000 sphinxcontrib-opendataservices-jsonschema-0.6.1/sphinxcontrib_opendataservices_jsonschema.egg-info/top_level.txt
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-10-23 12:29:09.608865 sphinxcontrib-opendataservices-jsonschema-0.6.1/tests/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      121 2023-08-30 14:59:22.000000 sphinxcontrib-opendataservices-jsonschema-0.6.1/tests/__init__.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2789 2023-08-30 14:59:22.000000 sphinxcontrib-opendataservices-jsonschema-0.6.1/tests/test_directive.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    16201 2023-08-30 14:59:22.000000 sphinxcontrib-opendataservices-jsonschema-0.6.1/tests/test_jsonschema.py
+drwxr-xr-x   0 odsc      (1000) odsc      (1000)        0 2024-05-03 13:57:13.321850 sphinxcontrib-opendataservices-jsonschema-0.7.0/
+-rw-r--r--   0 odsc      (1000) odsc      (1000)     1418 2024-04-30 14:16:47.000000 sphinxcontrib-opendataservices-jsonschema-0.7.0/LICENSE
+-rw-r--r--   0 odsc      (1000) odsc      (1000)       55 2024-04-30 14:16:47.000000 sphinxcontrib-opendataservices-jsonschema-0.7.0/MANIFEST.in
+-rw-r--r--   0 odsc      (1000) odsc      (1000)     2038 2024-05-03 13:57:13.321850 sphinxcontrib-opendataservices-jsonschema-0.7.0/PKG-INFO
+-rw-r--r--   0 odsc      (1000) odsc      (1000)     1013 2024-04-30 14:16:47.000000 sphinxcontrib-opendataservices-jsonschema-0.7.0/README.rst
+-rw-r--r--   0 odsc      (1000) odsc      (1000)      266 2024-05-03 13:57:13.321850 sphinxcontrib-opendataservices-jsonschema-0.7.0/setup.cfg
+-rw-r--r--   0 odsc      (1000) odsc      (1000)     1685 2024-05-03 13:29:38.000000 sphinxcontrib-opendataservices-jsonschema-0.7.0/setup.py
+drwxr-xr-x   0 odsc      (1000) odsc      (1000)        0 2024-05-03 13:57:13.315183 sphinxcontrib-opendataservices-jsonschema-0.7.0/sphinxcontrib/
+-rw-r--r--   0 odsc      (1000) odsc      (1000)       80 2024-04-30 14:16:47.000000 sphinxcontrib-opendataservices-jsonschema-0.7.0/sphinxcontrib/__init__.py
+-rw-r--r--   0 odsc      (1000) odsc      (1000)    20776 2024-05-03 08:00:19.000000 sphinxcontrib-opendataservices-jsonschema-0.7.0/sphinxcontrib/jsonschema.py
+drwxr-xr-x   0 odsc      (1000) odsc      (1000)        0 2024-05-03 13:57:13.318517 sphinxcontrib-opendataservices-jsonschema-0.7.0/sphinxcontrib_opendataservices_jsonschema.egg-info/
+-rw-r--r--   0 odsc      (1000) odsc      (1000)     2038 2024-05-03 13:57:13.000000 sphinxcontrib-opendataservices-jsonschema-0.7.0/sphinxcontrib_opendataservices_jsonschema.egg-info/PKG-INFO
+-rw-r--r--   0 odsc      (1000) odsc      (1000)      632 2024-05-03 13:57:13.000000 sphinxcontrib-opendataservices-jsonschema-0.7.0/sphinxcontrib_opendataservices_jsonschema.egg-info/SOURCES.txt
+-rw-r--r--   0 odsc      (1000) odsc      (1000)        1 2024-05-03 13:57:13.000000 sphinxcontrib-opendataservices-jsonschema-0.7.0/sphinxcontrib_opendataservices_jsonschema.egg-info/dependency_links.txt
+-rw-r--r--   0 odsc      (1000) odsc      (1000)       14 2024-05-03 13:57:13.000000 sphinxcontrib-opendataservices-jsonschema-0.7.0/sphinxcontrib_opendataservices_jsonschema.egg-info/namespace_packages.txt
+-rw-r--r--   0 odsc      (1000) odsc      (1000)        1 2024-05-01 12:54:02.000000 sphinxcontrib-opendataservices-jsonschema-0.7.0/sphinxcontrib_opendataservices_jsonschema.egg-info/not-zip-safe
+-rw-r--r--   0 odsc      (1000) odsc      (1000)       98 2024-05-03 13:57:13.000000 sphinxcontrib-opendataservices-jsonschema-0.7.0/sphinxcontrib_opendataservices_jsonschema.egg-info/requires.txt
+-rw-r--r--   0 odsc      (1000) odsc      (1000)       20 2024-05-03 13:57:13.000000 sphinxcontrib-opendataservices-jsonschema-0.7.0/sphinxcontrib_opendataservices_jsonschema.egg-info/top_level.txt
+drwxr-xr-x   0 odsc      (1000) odsc      (1000)        0 2024-05-03 13:57:13.321850 sphinxcontrib-opendataservices-jsonschema-0.7.0/tests/
+-rw-r--r--   0 odsc      (1000) odsc      (1000)      121 2024-04-30 14:16:47.000000 sphinxcontrib-opendataservices-jsonschema-0.7.0/tests/__init__.py
+-rw-r--r--   0 odsc      (1000) odsc      (1000)     2789 2024-04-30 14:16:47.000000 sphinxcontrib-opendataservices-jsonschema-0.7.0/tests/test_directive.py
+-rw-r--r--   0 odsc      (1000) odsc      (1000)    16201 2024-04-30 14:16:47.000000 sphinxcontrib-opendataservices-jsonschema-0.7.0/tests/test_jsonschema.py
```

### Comparing `sphinxcontrib-opendataservices-jsonschema-0.6.1/LICENSE` & `sphinxcontrib-opendataservices-jsonschema-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-opendataservices-jsonschema-0.6.1/PKG-INFO` & `sphinxcontrib-opendataservices-jsonschema-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-opendataservices-jsonschema
-Version: 0.6.1
+Version: 0.7.0
 Summary: Sphinx extension to define data structure using JSON Schema
 Home-page: https://github.com/OpenDataServices/sphinxcontrib-opendataservices-jsonschema
 Author: Takeshi KOMIYA & Open Data Services Co-operative
 Author-email: code@opendataservices.coop
 License: BSD
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sphinxcontrib-opendataservices-jsonschema-0.6.1/README.rst` & `sphinxcontrib-opendataservices-jsonschema-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-opendataservices-jsonschema-0.6.1/setup.py` & `sphinxcontrib-opendataservices-jsonschema-0.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 long_desc = open('README.rst').read()
 
 setup(
     name='sphinxcontrib-opendataservices-jsonschema',
-    version='0.6.1',
+    version='0.7.0',
     url='https://github.com/OpenDataServices/sphinxcontrib-opendataservices-jsonschema',
     license='BSD',
     author='Takeshi KOMIYA & Open Data Services Co-operative',
     author_email='code@opendataservices.coop',
     description='Sphinx extension to define data structure using JSON Schema',
     long_description=long_desc,
     zip_safe=False,
@@ -34,17 +34,20 @@
     include_package_data=True,
     python_requires='>=3.8',
     install_requires=[
         'docutils',
         'jsonref',
         'jsonpointer',
         'myst-parser',
+        'referencing',
+        'jscc',
     ],
     extras_require={
         'test': [
             'flake8<6',
             'lxml',
+            'defusedxml',  # Not directly used, but require because of issue with sphinx.testing.fixtures plugin
             'pytest',
         ],
     },
     namespace_packages=['sphinxcontrib'],
 )
```

### Comparing `sphinxcontrib-opendataservices-jsonschema-0.6.1/sphinxcontrib/jsonschema.py` & `sphinxcontrib-opendataservices-jsonschema-0.7.0/sphinxcontrib/jsonschema.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 import io
 import os
 import jsonref
 from jsonpointer import resolve_pointer
 from docutils import nodes
 from docutils.parsers.rst import directives, Directive
 from pathlib import Path
+from urllib import parse as urlparse
+from referencing import Registry, Resource
+from referencing.jsonschema import DRAFT202012
+from jscc.schema import is_json_schema
+from jscc.testing.filesystem import walk_json_data
 
 import json
 from collections import OrderedDict
 
 
 try:
     from myst_parser.main import to_docutils
@@ -34,25 +39,47 @@
         return parser.render(text)
 
 
 def custom_jsonref_jsonloader(uri, **kwargs):
     return {}
 
 
+def build_custom_schema_loader(schema_path):
+    """
+    Builds a callable which handles a URN if provided (e.g. resolves part
+    before hash in 'urn:components#/$defs/UnspecifiedRecord' to components.json
+    in schema_path dircetory), else calls default JSON loader.
+    """
+    schemas = []
+    for _, _, _, data in walk_json_data(top=schema_path):
+        if is_json_schema(data):
+            schemas.append((data.get("$id"), Resource(contents=data, specification=DRAFT202012)))
+    registry = Registry().with_resources(schemas)
+
+    def custom_loader(uri, **kwargs):
+        scheme = urlparse.urlsplit(uri).scheme
+        if scheme == "urn":
+            return registry.contents(uri.split("#")[0])
+        else:
+            return jsonref.jsonloader(uri, **kwargs)
+    return custom_loader
+
+
 class JSONSchemaDirective(Directive):
     has_content = True
     required_arguments = 1
     option_spec = {
         'include': directives.unchanged,
         'collapse': directives.unchanged,
         'pointer': directives.unchanged,
         'nocrossref': directives.flag,
         'addtargets': directives.flag,
         'externallinks': directives.unchanged,
         'allowexternalrefs': directives.flag,
+        'allowurnrefs': directives.flag,
     }
     # Add a rollup option here
 
     headers = ['Title', 'Description', 'Type', 'Format', 'Required']
     widths = [1, 1, 1, 1, 1]
     include = []
     include_used = set()
@@ -83,19 +110,26 @@
                 relpath = os.path.join(dirname, self.arguments[0])
                 abspath = os.path.join(env.srcdir, relpath)
                 if not os.access(abspath, os.R_OK):
                     raise self.warning('JSON Schema file not readable: %s' %
                                        self.arguments[0])
                 env.note_dependency(relpath)
 
-                schema = JSONSchema.loadfromfile(abspath, allow_external_refs=('allowexternalrefs' in self.options))
+                schema = JSONSchema.loadfromfile(
+                    abspath,
+                    allow_external_refs=('allowexternalrefs' in self.options),
+                    loader=(build_custom_schema_loader(abspath.rsplit("/", 1)[0])
+                            if 'allowurnrefs' in self.options else None)
+                )
             else:
                 schema = JSONSchema.loadfromfile(
                     ''.join(self.content),
-                    allow_external_refs=('allowexternalrefs' in self.options)
+                    allow_external_refs=('allowexternalrefs' in self.options),
+                    loader=(build_custom_schema_loader(abspath.rsplit("/", 1)[0])
+                            if 'allowurnrefs' in self.options else None)
                 )
         except ValueError as exc:
             raise self.error('Failed to parse JSON Schema: %s' % exc)
 
         if self.options.get('pointer'):
             schema = JSONSchema.instantiate(None, resolve_pointer(schema.attributes, self.options.get('pointer')))
 
@@ -238,33 +272,37 @@
             return str(type)
     else:
         return json.dumps(obj)
 
 
 class JSONSchema(object):
     @classmethod
-    def load(cls, reader, allow_external_refs=False, base_uri=""):
+    def load(cls, reader, allow_external_refs=False, base_uri="", loader=None):
         args = {}
         if not allow_external_refs:
             args['loader'] = custom_jsonref_jsonloader
+        if loader:
+            args['loader'] = loader
         obj = jsonref.load(reader, object_pairs_hook=OrderedDict, base_uri=base_uri, **args)
         return cls.instantiate(None, obj)
 
     @classmethod
     def loads(cls, string):
         obj = jsonref.loads(string, object_pairs_hook=OrderedDict, loader=custom_jsonref_jsonloader)
         return cls.instantiate(None, obj)
 
     @classmethod
-    def loadfromfile(cls, filename, allow_external_refs=False):
+    def loadfromfile(cls, filename, allow_external_refs=False, loader=None):
         with io.open(filename, 'rt', encoding='utf-8') as reader:
             args = {}
             if allow_external_refs:
                 args['allow_external_refs'] = True
                 args['base_uri'] = Path(os.path.realpath(filename)).as_uri()
+                if loader:
+                    args['loader'] = loader
             return cls.load(reader, **args)
 
     @classmethod
     def instantiate(cls, name, obj, required=False, parent=None, rollup=True):
         return get_class_for(obj)(name, obj, required, parent, rollup)
```

### Comparing `sphinxcontrib-opendataservices-jsonschema-0.6.1/sphinxcontrib_opendataservices_jsonschema.egg-info/PKG-INFO` & `sphinxcontrib-opendataservices-jsonschema-0.7.0/sphinxcontrib_opendataservices_jsonschema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-opendataservices-jsonschema
-Version: 0.6.1
+Version: 0.7.0
 Summary: Sphinx extension to define data structure using JSON Schema
 Home-page: https://github.com/OpenDataServices/sphinxcontrib-opendataservices-jsonschema
 Author: Takeshi KOMIYA & Open Data Services Co-operative
 Author-email: code@opendataservices.coop
 License: BSD
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sphinxcontrib-opendataservices-jsonschema-0.6.1/sphinxcontrib_opendataservices_jsonschema.egg-info/SOURCES.txt` & `sphinxcontrib-opendataservices-jsonschema-0.7.0/sphinxcontrib_opendataservices_jsonschema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-opendataservices-jsonschema-0.6.1/tests/test_directive.py` & `sphinxcontrib-opendataservices-jsonschema-0.7.0/tests/test_directive.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-opendataservices-jsonschema-0.6.1/tests/test_jsonschema.py` & `sphinxcontrib-opendataservices-jsonschema-0.7.0/tests/test_jsonschema.py`

 * *Files identical despite different names*


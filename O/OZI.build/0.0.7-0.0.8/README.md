# Comparing `tmp/OZI.build-0.0.7.tar.gz` & `tmp/OZI.build-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OZI.build-0.0.7.tar", last modified: Thu May  2 02:06:11 2024, max compression
+gzip compressed data, was "OZI.build-0.0.8.tar", last modified: Fri May  3 04:17:20 2024, max compression
```

## Comparing `OZI.build-0.0.7.tar` & `OZI.build-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-02 02:06:11.841250 OZI.build-0.0.7/
--rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-02 02:06:01.000000 OZI.build-0.0.7/.gitignore
--rw-rw-r--   0 ross      (1000) ross      (1000)      422 2024-05-02 02:06:01.000000 OZI.build-0.0.7/.gitlab-ci.yml
--rw-rw-r--   0 ross      (1000) ross      (1000)    11359 2024-05-02 02:06:01.000000 OZI.build-0.0.7/COPYING
--rw-rw-r--   0 ross      (1000) ross      (1000)      482 2024-05-02 02:06:01.000000 OZI.build-0.0.7/README.rst
--rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-02 02:06:01.000000 OZI.build-0.0.7/__init__.py
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-02 02:06:11.841250 OZI.build-0.0.7/doc/
--rwxrwxr-x   0 ross      (1000) ross      (1000)      651 2024-05-02 02:06:01.000000 OZI.build-0.0.7/doc/generate_doc.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1105 2024-05-02 02:06:01.000000 OZI.build-0.0.7/doc/index.md
--rw-rw-r--   0 ross      (1000) ross      (1000)      623 2024-05-02 02:06:01.000000 OZI.build-0.0.7/doc/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     3388 2024-05-02 02:06:01.000000 OZI.build-0.0.7/doc/pyproject-gen.md
--rw-rw-r--   0 ross      (1000) ross      (1000)     4171 2024-05-02 02:06:01.000000 OZI.build-0.0.7/doc/pyproject.md
--rw-rw-r--   0 ross      (1000) ross      (1000)     1339 2024-05-02 02:06:01.000000 OZI.build-0.0.7/doc/pyproject.md.in
--rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-02 02:06:01.000000 OZI.build-0.0.7/doc/sitemap.txt
--rw-rw-r--   0 ross      (1000) ross      (1000)      164 2024-05-02 02:06:01.000000 OZI.build-0.0.7/meson.build
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-02 02:06:11.841250 OZI.build-0.0.7/ozi_build/
--rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-02 02:06:01.000000 OZI.build-0.0.7/ozi_build/__init__.py
--rw-rw-r--   0 ross      (1000) ross      (1000)    14882 2024-05-02 02:06:01.000000 OZI.build-0.0.7/ozi_build/buildapi.py
--rw-rw-r--   0 ross      (1000) ross      (1000)      230 2024-05-02 02:06:01.000000 OZI.build-0.0.7/ozi_build/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     4297 2024-05-02 02:06:01.000000 OZI.build-0.0.7/ozi_build/pep425tags.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     3509 2024-05-02 02:06:01.000000 OZI.build-0.0.7/ozi_build/schema.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1070 2024-05-02 02:06:01.000000 OZI.build-0.0.7/pyproject.toml
--rwxrwxr-x   0 ross      (1000) ross      (1000)       73 2024-05-02 02:06:01.000000 OZI.build-0.0.7/release
--rw-rw-r--   0 ross      (1000) ross      (1000)     1353 2024-05-02 02:06:11.849250 OZI.build-0.0.7/PKG-INFO
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-03 04:17:20.774603 OZI.build-0.0.8/
+-rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-03 04:17:05.000000 OZI.build-0.0.8/.gitignore
+-rw-rw-r--   0 ross      (1000) ross      (1000)      422 2024-05-03 04:17:05.000000 OZI.build-0.0.8/.gitlab-ci.yml
+-rw-rw-r--   0 ross      (1000) ross      (1000)    11359 2024-05-03 04:17:05.000000 OZI.build-0.0.8/COPYING
+-rw-rw-r--   0 ross      (1000) ross      (1000)      482 2024-05-03 04:17:05.000000 OZI.build-0.0.8/README.rst
+-rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-03 04:17:05.000000 OZI.build-0.0.8/__init__.py
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-03 04:17:20.770603 OZI.build-0.0.8/doc/
+-rwxrwxr-x   0 ross      (1000) ross      (1000)      651 2024-05-03 04:17:05.000000 OZI.build-0.0.8/doc/generate_doc.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1105 2024-05-03 04:17:05.000000 OZI.build-0.0.8/doc/index.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)      623 2024-05-03 04:17:05.000000 OZI.build-0.0.8/doc/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     3388 2024-05-03 04:17:05.000000 OZI.build-0.0.8/doc/pyproject-gen.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)     4171 2024-05-03 04:17:05.000000 OZI.build-0.0.8/doc/pyproject.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1339 2024-05-03 04:17:05.000000 OZI.build-0.0.8/doc/pyproject.md.in
+-rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-03 04:17:05.000000 OZI.build-0.0.8/doc/sitemap.txt
+-rw-rw-r--   0 ross      (1000) ross      (1000)      164 2024-05-03 04:17:05.000000 OZI.build-0.0.8/meson.build
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-03 04:17:20.774603 OZI.build-0.0.8/ozi_build/
+-rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-03 04:17:05.000000 OZI.build-0.0.8/ozi_build/__init__.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)    15087 2024-05-03 04:17:05.000000 OZI.build-0.0.8/ozi_build/buildapi.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)      230 2024-05-03 04:17:05.000000 OZI.build-0.0.8/ozi_build/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     4297 2024-05-03 04:17:05.000000 OZI.build-0.0.8/ozi_build/pep425tags.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     3509 2024-05-03 04:17:05.000000 OZI.build-0.0.8/ozi_build/schema.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1070 2024-05-03 04:17:05.000000 OZI.build-0.0.8/pyproject.toml
+-rwxrwxr-x   0 ross      (1000) ross      (1000)       73 2024-05-03 04:17:05.000000 OZI.build-0.0.8/release
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1353 2024-05-03 04:17:20.786603 OZI.build-0.0.8/PKG-INFO
```

### Comparing `OZI.build-0.0.7/COPYING` & `OZI.build-0.0.8/COPYING`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.7/doc/generate_doc.py` & `OZI.build-0.0.8/doc/generate_doc.py`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.7/doc/index.md` & `OZI.build-0.0.8/doc/index.md`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.7/doc/meson.build` & `OZI.build-0.0.8/doc/meson.build`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.7/doc/pyproject-gen.md` & `OZI.build-0.0.8/doc/pyproject-gen.md`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.7/doc/pyproject.md` & `OZI.build-0.0.8/doc/pyproject.md`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.7/doc/pyproject.md.in` & `OZI.build-0.0.8/doc/pyproject.md.in`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.7/ozi_build/buildapi.py` & `OZI.build-0.0.8/ozi_build/buildapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,22 @@
         meta = {
             'name': self['module'],
             'version': self['version'],
         }
 
         if 'pkg-info-file' in self:
             res = '\n'.join(PKG_INFO.split('\n')[:3]).format(**meta) + '\n'
-            with open(self['pkg-info-file'], 'r') as f:
+            with open(
+                (
+                    self['pkg-info-file']
+                    if Path(self['pkg-info-file']).exists()
+                    else Path(self.builddir) / 'PKG-INFO'
+                ),
+                'r',
+            ) as f:
                 orig_lines = f.readlines()
                 for line in orig_lines:
                     if line.startswith(
                         'Metadata-Version:'
                     ) or line.startswith('Version:'):
                         continue
                     res += line
```

### Comparing `OZI.build-0.0.7/ozi_build/pep425tags.py` & `OZI.build-0.0.8/ozi_build/pep425tags.py`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.7/ozi_build/schema.py` & `OZI.build-0.0.8/ozi_build/schema.py`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.7/pyproject.toml` & `OZI.build-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.7/PKG-INFO` & `OZI.build-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OZI.build
-Version: 0.0.7
+Version: 0.0.8
 Summary: Create pep517 compliant packages from the meson build system, OZI-maintained fork.
 Home-page: https://github.com/OZI-Project/OZI.build
 Author: Thibault Saunier
 Author-email: tsaunier@gnome.org
 Maintainer: Eden Rose Duff MSc
 Maintainer-email: help@oziproject.dev
 Requires-Dist: wheel>0.33
```


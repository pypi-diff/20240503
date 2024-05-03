# Comparing `tmp/neo4py-1.1.7b0.tar.gz` & `tmp/neo4py-1.1.8b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo4py-1.1.7b0.tar", last modified: Fri May  3 04:57:55 2024, max compression
+gzip compressed data, was "neo4py-1.1.8b0.tar", last modified: Fri May  3 05:03:26 2024, max compression
```

## Comparing `neo4py-1.1.7b0.tar` & `neo4py-1.1.8b0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)        0 2024-05-03 04:57:55.510933 neo4py-1.1.7b0/
--rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)    11558 2024-03-14 07:44:25.000000 neo4py-1.1.7b0/LICENSE
--rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)     2173 2024-05-03 04:57:55.509943 neo4py-1.1.7b0/PKG-INFO
-drwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)        0 2024-05-03 04:57:55.500078 neo4py-1.1.7b0/neo4py/
--rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)        0 2024-03-14 07:10:59.000000 neo4py-1.1.7b0/neo4py/__init__.py
--rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)     3895 2024-04-30 09:16:01.000000 neo4py-1.1.7b0/neo4py/neo4py.py
--rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)     1644 2024-05-03 04:03:07.000000 neo4py-1.1.7b0/neo4py/sloth.py
-drwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)        0 2024-05-03 04:57:55.509051 neo4py-1.1.7b0/neo4py.egg-info/
--rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)     2173 2024-05-03 04:57:55.000000 neo4py-1.1.7b0/neo4py.egg-info/PKG-INFO
--rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)      251 2024-05-03 04:57:55.000000 neo4py-1.1.7b0/neo4py.egg-info/SOURCES.txt
--rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)        1 2024-05-03 04:57:55.000000 neo4py-1.1.7b0/neo4py.egg-info/dependency_links.txt
--rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)       14 2024-05-03 04:57:55.000000 neo4py-1.1.7b0/neo4py.egg-info/requires.txt
--rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)        7 2024-05-03 04:57:55.000000 neo4py-1.1.7b0/neo4py.egg-info/top_level.txt
--rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)      612 2024-05-03 04:49:24.000000 neo4py-1.1.7b0/pyproject.toml
--rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)     1755 2024-03-29 17:13:56.000000 neo4py-1.1.7b0/readme.md
--rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)       38 2024-05-03 04:57:55.511108 neo4py-1.1.7b0/setup.cfg
-drwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)        0 2024-05-03 04:57:55.507806 neo4py-1.1.7b0/tests/
--rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)      274 2024-04-30 09:15:28.000000 neo4py-1.1.7b0/tests/test_neo.py
+drwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)        0 2024-05-03 05:03:26.338987 neo4py-1.1.8b0/
+-rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)    11558 2024-03-14 07:44:25.000000 neo4py-1.1.8b0/LICENSE
+-rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)     2171 2024-05-03 05:03:26.337773 neo4py-1.1.8b0/PKG-INFO
+drwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)        0 2024-05-03 05:03:26.324942 neo4py-1.1.8b0/neo4py/
+-rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)        0 2024-03-14 07:10:59.000000 neo4py-1.1.8b0/neo4py/__init__.py
+-rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)     3895 2024-04-30 09:16:01.000000 neo4py-1.1.8b0/neo4py/neo4py.py
+-rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)     1644 2024-05-03 04:03:07.000000 neo4py-1.1.8b0/neo4py/sloth.py
+drwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)        0 2024-05-03 05:03:26.336652 neo4py-1.1.8b0/neo4py.egg-info/
+-rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)     2171 2024-05-03 05:03:26.000000 neo4py-1.1.8b0/neo4py.egg-info/PKG-INFO
+-rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)      251 2024-05-03 05:03:26.000000 neo4py-1.1.8b0/neo4py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)        1 2024-05-03 05:03:26.000000 neo4py-1.1.8b0/neo4py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)       12 2024-05-03 05:03:26.000000 neo4py-1.1.8b0/neo4py.egg-info/requires.txt
+-rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)        7 2024-05-03 05:03:26.000000 neo4py-1.1.8b0/neo4py.egg-info/top_level.txt
+-rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)      610 2024-05-03 05:02:51.000000 neo4py-1.1.8b0/pyproject.toml
+-rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)     1755 2024-03-29 17:13:56.000000 neo4py-1.1.8b0/readme.md
+-rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)       38 2024-05-03 05:03:26.339163 neo4py-1.1.8b0/setup.cfg
+drwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)        0 2024-05-03 05:03:26.335047 neo4py-1.1.8b0/tests/
+-rwxrwxrwx   0 atharnaveed  (1000) atharnaveed  (1000)      274 2024-04-30 09:15:28.000000 neo4py-1.1.8b0/tests/test_neo.py
```

### Comparing `neo4py-1.1.7b0/LICENSE` & `neo4py-1.1.8b0/LICENSE`

 * *Files identical despite different names*

### Comparing `neo4py-1.1.7b0/PKG-INFO` & `neo4py-1.1.8b0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: neo4py
-Version: 1.1.7b0
+Version: 1.1.8b0
 Summary: Neo4py is a better alternative to py2neo.
 Author-email: Athar Naveed <asphaltlegends24@gmail.com>
 Project-URL: Homepage, https://github.com/Athar-Naveed/neo4py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: neo4j==5.20.0
+Requires-Dist: neo4j==5.20
 
 ## Neo4py
 A proper documentation to __neo4py__ will be available soon.
 ## Introduction
 Neo4py is an alternative to __py2neo__. I am trying my best to make it a perfect and better clone of the py2neo package.
 
 ### How to run a query in neo4py
```

### Comparing `neo4py-1.1.7b0/neo4py/neo4py.py` & `neo4py-1.1.8b0/neo4py/neo4py.py`

 * *Files identical despite different names*

### Comparing `neo4py-1.1.7b0/neo4py/sloth.py` & `neo4py-1.1.8b0/neo4py/sloth.py`

 * *Files identical despite different names*

### Comparing `neo4py-1.1.7b0/neo4py.egg-info/PKG-INFO` & `neo4py-1.1.8b0/neo4py.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: neo4py
-Version: 1.1.7b0
+Version: 1.1.8b0
 Summary: Neo4py is a better alternative to py2neo.
 Author-email: Athar Naveed <asphaltlegends24@gmail.com>
 Project-URL: Homepage, https://github.com/Athar-Naveed/neo4py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: neo4j==5.20.0
+Requires-Dist: neo4j==5.20
 
 ## Neo4py
 A proper documentation to __neo4py__ will be available soon.
 ## Introduction
 Neo4py is an alternative to __py2neo__. I am trying my best to make it a perfect and better clone of the py2neo package.
 
 ### How to run a query in neo4py
```

### Comparing `neo4py-1.1.7b0/pyproject.toml` & `neo4py-1.1.8b0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neo4py"
-version = "1.1.7-beta"
+version = "1.1.8-beta"
 authors = [
   { name="Athar Naveed", email="asphaltlegends24@gmail.com" },
 ]
 description = "Neo4py is a better alternative to py2neo."
 readme = "readme.md"
 requires-python = ">=3.8"
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 dependencies =[
-  "neo4j==5.20.0"
+  "neo4j==5.20"
 ]
 
 
 [project.urls]
 Homepage = "https://github.com/Athar-Naveed/neo4py"
```

### Comparing `neo4py-1.1.7b0/readme.md` & `neo4py-1.1.8b0/readme.md`

 * *Files identical despite different names*


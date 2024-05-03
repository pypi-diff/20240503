# Comparing `tmp/couchdb_client-1.0.1.tar.gz` & `tmp/couchdb_client-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "couchdb_client-1.0.1.tar", last modified: Mon Apr 29 13:23:57 2024, max compression
+gzip compressed data, was "couchdb_client-1.0.3.tar", last modified: Fri May  3 12:17:30 2024, max compression
```

## Comparing `couchdb_client-1.0.1.tar` & `couchdb_client-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:23:57.447132 couchdb_client-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-29 13:23:53.000000 couchdb_client-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-29 13:23:57.447132 couchdb_client-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-29 13:23:53.000000 couchdb_client-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-29 13:23:53.000000 couchdb_client-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:23:57.447132 couchdb_client-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:23:57.443132 couchdb_client-1.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:23:53.000000 couchdb_client-1.0.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:23:57.443132 couchdb_client-1.0.1/src/couchdb_client/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-29 13:23:53.000000 couchdb_client-1.0.1/src/couchdb_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-29 13:23:53.000000 couchdb_client-1.0.1/src/couchdb_client/couchdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-29 13:23:53.000000 couchdb_client-1.0.1/src/couchdb_client/document.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-29 13:23:53.000000 couchdb_client-1.0.1/src/couchdb_client/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:23:57.447132 couchdb_client-1.0.1/src/couchdb_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-29 13:23:57.000000 couchdb_client-1.0.1/src/couchdb_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-29 13:23:57.000000 couchdb_client-1.0.1/src/couchdb_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:23:57.000000 couchdb_client-1.0.1/src/couchdb_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 13:23:57.000000 couchdb_client-1.0.1/src/couchdb_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 13:23:57.000000 couchdb_client-1.0.1/src/couchdb_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:30.158091 couchdb_client-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-03 12:17:19.000000 couchdb_client-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-03 12:17:30.158091 couchdb_client-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-03 12:17:19.000000 couchdb_client-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-03 12:17:19.000000 couchdb_client-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:17:30.158091 couchdb_client-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:30.154091 couchdb_client-1.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:19.000000 couchdb_client-1.0.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:30.154091 couchdb_client-1.0.3/src/couchdb_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-03 12:17:19.000000 couchdb_client-1.0.3/src/couchdb_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-03 12:17:19.000000 couchdb_client-1.0.3/src/couchdb_client/couchdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-03 12:17:19.000000 couchdb_client-1.0.3/src/couchdb_client/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-03 12:17:19.000000 couchdb_client-1.0.3/src/couchdb_client/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:30.158091 couchdb_client-1.0.3/src/couchdb_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-03 12:17:30.000000 couchdb_client-1.0.3/src/couchdb_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-03 12:17:30.000000 couchdb_client-1.0.3/src/couchdb_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:17:30.000000 couchdb_client-1.0.3/src/couchdb_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 12:17:30.000000 couchdb_client-1.0.3/src/couchdb_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 12:17:30.000000 couchdb_client-1.0.3/src/couchdb_client.egg-info/top_level.txt
```

### Comparing `couchdb_client-1.0.1/LICENSE` & `couchdb_client-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `couchdb_client-1.0.1/PKG-INFO` & `couchdb_client-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: couchdb_client
-Version: 1.0.1
+Version: 1.0.3
 Summary: Very simple CouchDB client
 Author-email: Enzo PB <enzo.puiroux@mail.com>
 Project-URL: Homepage, https://github.com/EnzoPB/couchdb-client
 Project-URL: Issues, https://github.com/EnzoPB/couchdb-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `couchdb_client-1.0.1/README.md` & `couchdb_client-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `couchdb_client-1.0.1/pyproject.toml` & `couchdb_client-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "couchdb_client"
-version = "1.0.1"
+version = "1.0.3"
 authors = [
   { name="Enzo PB", email="enzo.puiroux@mail.com" },
 ]
 description = "Very simple CouchDB client"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `couchdb_client-1.0.1/src/couchdb_client/couchdb.py` & `couchdb_client-1.0.3/src/couchdb_client/couchdb.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,30 @@
         data = requests.request(
             method,
             self.base_url + self.db_name + '/' + endpoint + params,
             json=data if data is not None else {})
         data.raise_for_status()
         return json.loads(data.text)
 
+    def get_all_documents(self, skip: int | None = None, limit: int | None = None):
+        params = {
+            'include_docs': True
+        }
+        if skip is not None:
+            params['skip'] = skip
+        if limit is not None:
+            params['limit'] = limit
+
+        result = []
+        for doc in self.req('_all_docs', 'GET', query_params=params)['rows']:
+            if not doc['id'].startswith('_design'):  # ignore design documents
+                result.append(Document(self, doc['doc']))
+        return result
+
+
     def get_document(self, document_id: str):
         try:
             return Document(self, self.req(document_id, 'GET'))
         except requests.exceptions.HTTPError as e:
             if e.response.status_code == 404:
                 return None
             else:
```

### Comparing `couchdb_client-1.0.1/src/couchdb_client/document.py` & `couchdb_client-1.0.3/src/couchdb_client/document.py`

 * *Files identical despite different names*

### Comparing `couchdb_client-1.0.1/src/couchdb_client/example.py` & `couchdb_client-1.0.3/src/couchdb_client/example.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,7 +19,9 @@
 # get the document again to the the updated data
 print(db.get_document(doc.id))
 
 # delete the document
 doc.delete()
 
 print(db.get_document(doc.id))  # should return none since the document was deleted
+
+print(db.get_all_documents(skip=100, limit=10))  # get 10 documents, starting from the 100th
```

### Comparing `couchdb_client-1.0.1/src/couchdb_client.egg-info/PKG-INFO` & `couchdb_client-1.0.3/src/couchdb_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: couchdb_client
-Version: 1.0.1
+Version: 1.0.3
 Summary: Very simple CouchDB client
 Author-email: Enzo PB <enzo.puiroux@mail.com>
 Project-URL: Homepage, https://github.com/EnzoPB/couchdb-client
 Project-URL: Issues, https://github.com/EnzoPB/couchdb-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


# Comparing `tmp/es_wait-0.5.5.tar.gz` & `tmp/es_wait-0.5.6.tar.gz`

## Comparing `es_wait-0.5.5.tar` & `es_wait-0.5.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 es_wait-0.5.5/.coveragerc
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 es_wait-0.5.5/src/es_wait/__init__.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 es_wait-0.5.5/src/es_wait/_base.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 es_wait-0.5.5/src/es_wait/exceptions.py
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 es_wait-0.5.5/src/es_wait/exists.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 es_wait-0.5.5/src/es_wait/health.py
--rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 es_wait-0.5.5/src/es_wait/ilm.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 es_wait-0.5.5/src/es_wait/relocate.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 es_wait-0.5.5/src/es_wait/restore.py
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 es_wait-0.5.5/src/es_wait/snapshot.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 es_wait-0.5.5/src/es_wait/task.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 es_wait-0.5.5/.gitignore
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.5.5/LICENSE
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.5.5/README.md
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 es_wait-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 es_wait-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 es_wait-0.5.6/.coveragerc
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 es_wait-0.5.6/src/es_wait/__init__.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 es_wait-0.5.6/src/es_wait/_base.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 es_wait-0.5.6/src/es_wait/exceptions.py
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 es_wait-0.5.6/src/es_wait/exists.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 es_wait-0.5.6/src/es_wait/health.py
+-rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 es_wait-0.5.6/src/es_wait/ilm.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 es_wait-0.5.6/src/es_wait/relocate.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 es_wait-0.5.6/src/es_wait/restore.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 es_wait-0.5.6/src/es_wait/snapshot.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 es_wait-0.5.6/src/es_wait/task.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 es_wait-0.5.6/.gitignore
+-rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.5.6/LICENSE
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.5.6/README.md
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 es_wait-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 es_wait-0.5.6/PKG-INFO
```

### Comparing `es_wait-0.5.5/src/es_wait/_base.py` & `es_wait-0.5.6/src/es_wait/_base.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.5/src/es_wait/exists.py` & `es_wait-0.5.6/src/es_wait/exists.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.5/src/es_wait/health.py` & `es_wait-0.5.6/src/es_wait/health.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.5/src/es_wait/ilm.py` & `es_wait-0.5.6/src/es_wait/ilm.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     def get_explain_data(self) -> t.Union[t.Dict, None]:
         """
         Calls `client.indices.`
         :py:meth:`~.elasticsearch.client.IlmClient.explain_lifecycle` with an index
         name and returns the resulting response.
         """
         try:
-            resp = self.client.ilm.explain_lifecycle(index=self.name)
+            resp = dict(self.client.ilm.explain_lifecycle(index=self.name))
             logger.debug('ILM Explain response: %s', self.prettystr(resp))
         except NotFoundError as exc:
             msg = (
                 f'Datastream/Index Name changed. {self.name} was not found. '
                 f'This is likely due to the index name suddenly changing, as with '
                 f'searchable snapshot mounts.'
             )
```

### Comparing `es_wait-0.5.5/src/es_wait/relocate.py` & `es_wait-0.5.6/src/es_wait/relocate.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.5/src/es_wait/restore.py` & `es_wait-0.5.6/src/es_wait/restore.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.5/src/es_wait/snapshot.py` & `es_wait-0.5.6/src/es_wait/snapshot.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.5/src/es_wait/task.py` & `es_wait-0.5.6/src/es_wait/task.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.5/.gitignore` & `es_wait-0.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.5/LICENSE` & `es_wait-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.5/pyproject.toml` & `es_wait-0.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.5/PKG-INFO` & `es_wait-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: es-wait
-Version: 0.5.5
+Version: 0.5.6
 Summary: Helping you wait for certain Elasticsearch tasks and API calls to finish
 Project-URL: Documentation, https://github.com/untergeek/es-wait#readme
 Project-URL: Issues, https://github.com/untergeek/es-wait/issues
 Project-URL: Source, https://github.com/untergeek/es-wait
 Author-email: Aaron Mildenstein <untergeek@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
```


# Comparing `tmp/es_wait-0.5.6.tar.gz` & `tmp/es_wait-0.5.7.tar.gz`

## Comparing `es_wait-0.5.6.tar` & `es_wait-0.5.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 es_wait-0.5.6/.coveragerc
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 es_wait-0.5.6/src/es_wait/__init__.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 es_wait-0.5.6/src/es_wait/_base.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 es_wait-0.5.6/src/es_wait/exceptions.py
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 es_wait-0.5.6/src/es_wait/exists.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 es_wait-0.5.6/src/es_wait/health.py
--rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 es_wait-0.5.6/src/es_wait/ilm.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 es_wait-0.5.6/src/es_wait/relocate.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 es_wait-0.5.6/src/es_wait/restore.py
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 es_wait-0.5.6/src/es_wait/snapshot.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 es_wait-0.5.6/src/es_wait/task.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 es_wait-0.5.6/.gitignore
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.5.6/LICENSE
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.5.6/README.md
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 es_wait-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 es_wait-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 es_wait-0.5.7/.coveragerc
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 es_wait-0.5.7/src/es_wait/__init__.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 es_wait-0.5.7/src/es_wait/_base.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 es_wait-0.5.7/src/es_wait/exceptions.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 es_wait-0.5.7/src/es_wait/exists.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 es_wait-0.5.7/src/es_wait/health.py
+-rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 es_wait-0.5.7/src/es_wait/ilm.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 es_wait-0.5.7/src/es_wait/relocate.py
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 es_wait-0.5.7/src/es_wait/restore.py
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 es_wait-0.5.7/src/es_wait/snapshot.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 es_wait-0.5.7/src/es_wait/task.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 es_wait-0.5.7/.gitignore
+-rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.5.7/LICENSE
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.5.7/README.md
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 es_wait-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 es_wait-0.5.7/PKG-INFO
```

### Comparing `es_wait-0.5.6/src/es_wait/_base.py` & `es_wait-0.5.7/src/es_wait/_base.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.6/src/es_wait/exists.py` & `es_wait-0.5.7/src/es_wait/exists.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
         super().__init__(client=client, pause=pause, timeout=timeout)
         self.name = name
         self.kind = kind
         self.empty_check('name')
         self.empty_check('kind')
         self.waitstr = f'for {self.kindmap} "{name}" to exist'
+        logger.debug('Waiting %s...', self.waitstr)
 
     @property
     def check(self) -> bool:
         """
         Check if the named entity exists, based on kind
         """
         doit = {
```

### Comparing `es_wait-0.5.6/src/es_wait/health.py` & `es_wait-0.5.7/src/es_wait/health.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
             'allocation', 'cluster_routing', 'mount', 'replicas', 'shrink'
         ] = None,
     ) -> None:
         super().__init__(client=client, pause=pause, timeout=timeout)
         self.action = action
         self.empty_check('action')
         self.waitstr = self.getwaitstr
+        logger.debug('Waiting %s...', self.waitstr)
 
     def argmap(self) -> t.Union[t.Dict[str, int], t.Dict[str, str]]:
         """This is a little way to ensure many possibilities come down to one"""
         if self.action in self.RELO_ACTIONS:
             return self.RELO_ARGS
         if self.action in self.STATUS_ACTIONS:
             return self.STATUS_ARGS
```

### Comparing `es_wait-0.5.6/src/es_wait/ilm.py` & `es_wait-0.5.7/src/es_wait/ilm.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         self.logger = logging.getLogger('es_wait.IlmPhase')
         super().__init__(client=client, pause=pause, timeout=timeout, name=name)
         self.phase = phase
         self.empty_check('phase')
         self.waitstr = (
             f'for "{self.name}" to complete ILM transition to phase "{self.phase}"'
         )
+        logger.debug('Waiting %s...', self.waitstr)
 
     @property
     def check(self) -> bool:
         """
         Check for ILM phase change completion.  It will return ``True`` if the expected
         phase and the actually collected phase match.
```

### Comparing `es_wait-0.5.6/src/es_wait/relocate.py` & `es_wait-0.5.7/src/es_wait/relocate.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         timeout: float = -1,
         name: str = None,
     ) -> None:
         super().__init__(client=client, pause=pause, timeout=timeout)
         self.name = name
         self.empty_check('name')
         self.waitstr = f'for index "{self.name}" to finish relocating'
+        logger.debug('Waiting %s...', self.waitstr)
 
     @property
     def check(self) -> bool:
         """
         This function calls `client.cluster.`
         :py:meth:`~.elasticsearch.client.ClusterClient.state` with a given index to
         check if all of the shards for that index are in the ``STARTED`` state. It will
```

### Comparing `es_wait-0.5.6/src/es_wait/restore.py` & `es_wait-0.5.7/src/es_wait/restore.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         timeout: float = -1,
         index_list: t.Sequence[str] = None,
     ) -> None:
         super().__init__(client=client, pause=pause, timeout=timeout)
         self.index_list = index_list
         self.empty_check('index_list')
         self.waitstr = 'for indices in index_list to be restored from snapshot'
+        logger.debug('Waiting %s...', self.waitstr)
 
     @property
     def check(self) -> bool:
         """
         Calls `client.indices.`
         :py:meth:`~.elasticsearch.client.IndicesClient.recovery` with a list of indices
         to check for complete recovery.  It will return ``True`` if recovery of those
```

### Comparing `es_wait-0.5.6/src/es_wait/snapshot.py` & `es_wait-0.5.7/src/es_wait/snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     ) -> None:
         super().__init__(client=client, pause=pause, timeout=timeout)
         self.snapshot = snapshot
         self.repository = repository
         self.empty_check('snapshot')
         self.empty_check('repository')
         self.waitstr = f'for snapshot "{self.snapshot}" to complete'
+        logger.debug('Waiting %s...', self.waitstr)
 
     @property
     def check(self) -> bool:
         """
         This function calls `client.snapshot.`
         :py:meth:`~.elasticsearch.client.SnapshotClient.get` and tests to see whether
         the snapshot is complete, and if so, with what status. It will log errors
```

### Comparing `es_wait-0.5.6/src/es_wait/task.py` & `es_wait-0.5.7/src/es_wait/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         self.action = action
         self.task_id = task_id
         self.empty_check('action')
         self.empty_check('task_id')
         self.task_data = None
         self.task = None
         self.waitstr = f'for the "{self.action}" task to complete'
+        logger.debug('Waiting %s...', self.waitstr)
 
     @property
     def check(self) -> bool:
         """
         This function calls `client.tasks.`
         :py:meth:`~.elasticsearch.client.TasksClient.get` with the provided
         ``task_id``.  If the task data contains ``'completed': True``, then it will
```

### Comparing `es_wait-0.5.6/.gitignore` & `es_wait-0.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.6/LICENSE` & `es_wait-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.6/pyproject.toml` & `es_wait-0.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.6/PKG-INFO` & `es_wait-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: es-wait
-Version: 0.5.6
+Version: 0.5.7
 Summary: Helping you wait for certain Elasticsearch tasks and API calls to finish
 Project-URL: Documentation, https://github.com/untergeek/es-wait#readme
 Project-URL: Issues, https://github.com/untergeek/es-wait/issues
 Project-URL: Source, https://github.com/untergeek/es-wait
 Author-email: Aaron Mildenstein <untergeek@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
```


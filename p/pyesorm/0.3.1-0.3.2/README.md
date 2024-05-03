# Comparing `tmp/pyesorm-0.3.1.tar.gz` & `tmp/pyesorm-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyesorm-0.3.1.tar", last modified: Mon Apr 29 12:27:40 2024, max compression
+gzip compressed data, was "pyesorm-0.3.2.tar", last modified: Fri May  3 19:07:13 2024, max compression
```

## Comparing `pyesorm-0.3.1.tar` & `pyesorm-0.3.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-04-29 12:27:40.930554 pyesorm-0.3.1/
--rw-r--r--   0 wallner    (501) staff       (20)    16725 2023-10-30 16:10:12.000000 pyesorm-0.3.1/LICENSE
--rw-r--r--   0 wallner    (501) staff       (20)    22773 2024-04-29 12:27:40.929481 pyesorm-0.3.1/PKG-INFO
--rw-r--r--   0 wallner    (501) staff       (20)    21136 2024-04-29 12:11:29.000000 pyesorm-0.3.1/README.md
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-04-29 12:27:40.909202 pyesorm-0.3.1/docs/
--rw-r--r--   0 wallner    (501) staff       (20)        0 2024-01-17 15:06:14.000000 pyesorm-0.3.1/docs/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     1484 2024-01-17 15:18:18.000000 pyesorm-0.3.1/docs/changelog.py
--rw-r--r--   0 wallner    (501) staff       (20)     1462 2024-01-17 15:10:11.000000 pyesorm-0.3.1/docs/conf.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-04-29 12:27:40.921892 pyesorm-0.3.1/esorm/
--rw-r--r--   0 wallner    (501) staff       (20)      666 2024-04-29 11:40:09.000000 pyesorm-0.3.1/esorm/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     3132 2024-01-22 17:32:29.000000 pyesorm-0.3.1/esorm/aggs.py
--rw-r--r--   0 wallner    (501) staff       (20)     2046 2024-04-29 10:57:43.000000 pyesorm-0.3.1/esorm/bulk.py
--rw-r--r--   0 wallner    (501) staff       (20)      470 2023-10-30 16:10:12.000000 pyesorm-0.3.1/esorm/error.py
--rw-r--r--   0 wallner    (501) staff       (20)     1943 2023-10-31 19:12:30.000000 pyesorm-0.3.1/esorm/esorm.py
--rw-r--r--   0 wallner    (501) staff       (20)     3500 2024-01-24 09:39:22.000000 pyesorm-0.3.1/esorm/fastapi.py
--rw-r--r--   0 wallner    (501) staff       (20)    11640 2023-10-31 19:12:30.000000 pyesorm-0.3.1/esorm/fields.py
--rw-r--r--   0 wallner    (501) staff       (20)       52 2023-10-30 16:10:12.000000 pyesorm-0.3.1/esorm/logger.py
--rw-r--r--   0 wallner    (501) staff       (20)    37485 2024-04-29 12:18:45.000000 pyesorm-0.3.1/esorm/model.py
--rw-r--r--   0 wallner    (501) staff       (20)     9605 2024-01-18 19:16:18.000000 pyesorm-0.3.1/esorm/query.py
--rw-r--r--   0 wallner    (501) staff       (20)     1315 2024-01-18 19:06:35.000000 pyesorm-0.3.1/esorm/response.py
--rw-r--r--   0 wallner    (501) staff       (20)      996 2024-01-23 07:15:23.000000 pyesorm-0.3.1/esorm/utils.py
--rw-r--r--   0 wallner    (501) staff       (20)     5538 2023-10-30 16:10:12.000000 pyesorm-0.3.1/esorm/watcher.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-04-29 12:27:40.927252 pyesorm-0.3.1/pyesorm.egg-info/
--rw-r--r--   0 wallner    (501) staff       (20)    22773 2024-04-29 12:27:40.000000 pyesorm-0.3.1/pyesorm.egg-info/PKG-INFO
--rw-r--r--   0 wallner    (501) staff       (20)      514 2024-04-29 12:27:40.000000 pyesorm-0.3.1/pyesorm.egg-info/SOURCES.txt
--rw-r--r--   0 wallner    (501) staff       (20)        1 2024-04-29 12:27:40.000000 pyesorm-0.3.1/pyesorm.egg-info/dependency_links.txt
--rw-r--r--   0 wallner    (501) staff       (20)      272 2024-04-29 12:27:40.000000 pyesorm-0.3.1/pyesorm.egg-info/requires.txt
--rw-r--r--   0 wallner    (501) staff       (20)       17 2024-04-29 12:27:40.000000 pyesorm-0.3.1/pyesorm.egg-info/top_level.txt
--rw-r--r--   0 wallner    (501) staff       (20)       87 2023-10-31 20:33:56.000000 pyesorm-0.3.1/pyproject.toml
--rw-r--r--   0 wallner    (501) staff       (20)     1306 2024-04-29 12:27:40.931225 pyesorm-0.3.1/setup.cfg
--rw-r--r--   0 wallner    (501) staff       (20)       37 2023-10-30 16:10:12.000000 pyesorm-0.3.1/setup.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-04-29 12:27:40.926196 pyesorm-0.3.1/tests/
--rw-r--r--   0 wallner    (501) staff       (20)        0 2023-10-30 16:10:12.000000 pyesorm-0.3.1/tests/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     6472 2024-04-29 11:47:14.000000 pyesorm-0.3.1/tests/conftest.py
--rw-r--r--   0 wallner    (501) staff       (20)    23736 2024-04-29 11:47:54.000000 pyesorm-0.3.1/tests/test_esorm.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-03 19:07:13.139805 pyesorm-0.3.2/
+-rw-r--r--   0 wallner    (501) staff       (20)    16725 2023-10-30 16:10:12.000000 pyesorm-0.3.2/LICENSE
+-rw-r--r--   0 wallner    (501) staff       (20)    22773 2024-05-03 19:07:13.139577 pyesorm-0.3.2/PKG-INFO
+-rw-r--r--   0 wallner    (501) staff       (20)    21136 2024-04-29 12:11:29.000000 pyesorm-0.3.2/README.md
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-03 19:07:13.127076 pyesorm-0.3.2/docs/
+-rw-r--r--   0 wallner    (501) staff       (20)        0 2024-01-17 15:06:14.000000 pyesorm-0.3.2/docs/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1484 2024-01-17 15:18:18.000000 pyesorm-0.3.2/docs/changelog.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1462 2024-01-17 15:10:11.000000 pyesorm-0.3.2/docs/conf.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-03 19:07:13.132816 pyesorm-0.3.2/esorm/
+-rw-r--r--   0 wallner    (501) staff       (20)      666 2024-04-29 11:40:09.000000 pyesorm-0.3.2/esorm/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     3132 2024-01-22 17:32:29.000000 pyesorm-0.3.2/esorm/aggs.py
+-rw-r--r--   0 wallner    (501) staff       (20)     2028 2024-05-03 18:04:45.000000 pyesorm-0.3.2/esorm/bulk.py
+-rw-r--r--   0 wallner    (501) staff       (20)      470 2023-10-30 16:10:12.000000 pyesorm-0.3.2/esorm/error.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1943 2023-10-31 19:12:30.000000 pyesorm-0.3.2/esorm/esorm.py
+-rw-r--r--   0 wallner    (501) staff       (20)     3500 2024-01-24 09:39:22.000000 pyesorm-0.3.2/esorm/fastapi.py
+-rw-r--r--   0 wallner    (501) staff       (20)    11640 2023-10-31 19:12:30.000000 pyesorm-0.3.2/esorm/fields.py
+-rw-r--r--   0 wallner    (501) staff       (20)       52 2023-10-30 16:10:12.000000 pyesorm-0.3.2/esorm/logger.py
+-rw-r--r--   0 wallner    (501) staff       (20)    38189 2024-05-03 17:24:16.000000 pyesorm-0.3.2/esorm/model.py
+-rw-r--r--   0 wallner    (501) staff       (20)     9605 2024-01-18 19:16:18.000000 pyesorm-0.3.2/esorm/query.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1315 2024-01-18 19:06:35.000000 pyesorm-0.3.2/esorm/response.py
+-rw-r--r--   0 wallner    (501) staff       (20)      996 2024-01-23 07:15:23.000000 pyesorm-0.3.2/esorm/utils.py
+-rw-r--r--   0 wallner    (501) staff       (20)     5538 2023-10-30 16:10:12.000000 pyesorm-0.3.2/esorm/watcher.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-03 19:07:13.137446 pyesorm-0.3.2/pyesorm.egg-info/
+-rw-r--r--   0 wallner    (501) staff       (20)    22773 2024-05-03 19:07:13.000000 pyesorm-0.3.2/pyesorm.egg-info/PKG-INFO
+-rw-r--r--   0 wallner    (501) staff       (20)      514 2024-05-03 19:07:13.000000 pyesorm-0.3.2/pyesorm.egg-info/SOURCES.txt
+-rw-r--r--   0 wallner    (501) staff       (20)        1 2024-05-03 19:07:13.000000 pyesorm-0.3.2/pyesorm.egg-info/dependency_links.txt
+-rw-r--r--   0 wallner    (501) staff       (20)      272 2024-05-03 19:07:13.000000 pyesorm-0.3.2/pyesorm.egg-info/requires.txt
+-rw-r--r--   0 wallner    (501) staff       (20)       17 2024-05-03 19:07:13.000000 pyesorm-0.3.2/pyesorm.egg-info/top_level.txt
+-rw-r--r--   0 wallner    (501) staff       (20)       87 2023-10-31 20:33:56.000000 pyesorm-0.3.2/pyproject.toml
+-rw-r--r--   0 wallner    (501) staff       (20)     1306 2024-05-03 19:07:13.140502 pyesorm-0.3.2/setup.cfg
+-rw-r--r--   0 wallner    (501) staff       (20)       37 2023-10-30 16:10:12.000000 pyesorm-0.3.2/setup.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-03 19:07:13.136293 pyesorm-0.3.2/tests/
+-rw-r--r--   0 wallner    (501) staff       (20)        0 2023-10-30 16:10:12.000000 pyesorm-0.3.2/tests/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     7056 2024-05-03 18:47:40.000000 pyesorm-0.3.2/tests/conftest.py
+-rw-r--r--   0 wallner    (501) staff       (20)    25009 2024-05-03 19:04:15.000000 pyesorm-0.3.2/tests/test_esorm.py
```

### Comparing `pyesorm-0.3.1/LICENSE` & `pyesorm-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.1/PKG-INFO` & `pyesorm-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyesorm
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python ElasticSearch ORM based on Pydantic
 Home-page: https://github.com/wallneradam/esorm
 Author: Adam Wallner
 Author-email: Adam.wallner@gmail.com
 License: MPL-2.0
 Project-URL: Bug Tracker, https://github.com/wallneradam/esorm/issues
 Project-URL: Documentation, https://esorm.readthedocs.io/en/latest/
```

### Comparing `pyesorm-0.3.1/README.md` & `pyesorm-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.1/docs/changelog.py` & `pyesorm-0.3.2/docs/changelog.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.1/docs/conf.py` & `pyesorm-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.1/esorm/__init__.py` & `pyesorm-0.3.2/esorm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.1/esorm/aggs.py` & `pyesorm-0.3.2/esorm/aggs.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.1/esorm/bulk.py` & `pyesorm-0.3.2/esorm/bulk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Bulk operation for ElasticSearch
 """
-from datetime import datetime, UTC
+from .utils import utcnow
 
 from .model import TModel, ESModelTimestamp
 from .esorm import es
 
 
 class ESBulk:
     """
@@ -47,15 +47,15 @@
             '_id': model.__id__
         }
         routing = model.__routing__
         if routing is not None:
             index['routing'] = routing
 
         if isinstance(model, ESModelTimestamp):
-            document['modified_at'] = datetime.now(UTC)
+            document['modified_at'] = utcnow()
 
         self._actions.append({'index': index, })
         self._actions.append(document)
 
     async def delete(self, model: TModel):
         """
         Add the model to the bulk for deletion
```

### Comparing `pyesorm-0.3.1/esorm/esorm.py` & `pyesorm-0.3.2/esorm/esorm.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.1/esorm/fastapi.py` & `pyesorm-0.3.2/esorm/fastapi.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.1/esorm/fields.py` & `pyesorm-0.3.2/esorm/fields.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.1/esorm/model.py` & `pyesorm-0.3.2/esorm/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,70 +159,103 @@
     # All model classes collected
     __models__: Dict[str, Type['ESModel']] = {}
 
     # noinspection PyUnresolvedReferences
     def __new__(cls: Type[ModelMetaclass], name: str, bases: Tuple[type, ...],
                 namespace: Dict[str, Any], **kwds: Any):
         model: Type[BaseModel] = super().__new__(cls, name, bases, namespace, **kwds)
-        if name not in ("ESModel", "ESModelTimestamp"):
+        if name not in ("ESModel", "ESModelTimestamp", "ESBaseModel"):
+            is_model = issubclass(model, ESModel)
+
             # ESConfig inheritance
             m_dict = {k: v for k, v in ESModel.ESConfig.__dict__.items() if k[0] != '_'}
             if bases and 'ESConfig' in bases[0].__dict__:
                 m_dict.update({k: v for k, v in bases[0].ESConfig.__dict__.items() if k[0] != '_'})
             del m_dict['index']  # It is only allowed to be set on the actual model class
             if 'ESConfig' in model.__dict__:
                 m_dict.update({k: v for k, v in model.ESConfig.__dict__.items() if k[0] != '_'})
             m_dict['_lazy_properties'] = {}
 
             # Create (new) ESConfig class inside the class
             model.ESConfig = type('ESConfig', (object,), dict(m_dict))
 
             # Set default index name if not already set
-            if not getattr(model.ESConfig, 'index', None):
+            if is_model and not getattr(model.ESConfig, 'index', None):
                 # Default index is the name of the class in snake_case
                 model.ESConfig.index = _default_index_prefix + '-' + snake_case(name)
 
             # If there is an 'id' field, set it as id_field
-            if 'id' in model.model_fields.keys():
+            if is_model and 'id' in model.model_fields.keys():
                 model.ESConfig.id_field = 'id'
 
             # Add to models
-            cls.__models__[model.ESConfig.index] = model
+            if is_model:
+                cls.__models__[model.ESConfig.index] = model
 
             # Collect lazy properties
             for attr_name, attr in namespace.items():
                 # Support computed fields
                 if attr.__class__.__name__ == 'PydanticDescriptorProxy':
                     attr = getattr(attr, 'wrapped')
                 # Is it a lazy property?
                 if isinstance(attr, property) and hasattr(attr.fget, '__lazy_property__'):
                     # noinspection PyProtectedMember
                     model.ESConfig._lazy_properties[attr_name] = getattr(attr.fget, '__lazy_property__')
 
         return model
 
 
-class ESBaseModel(BaseModel):
+class ESBaseModel(BaseModel, metaclass=_ESModelMeta):
     """
     Base class for Elastic
 
     It is useful for nested models, if you don't need the model in ES mappings
     """
 
+    class ESConfig:
+        """
+        ESBaseModel Config
+
+        This is just for lazy properties, to make ESBasemodel compatible with them
+        """
+
+        lazy_property_max_recursion_depth: int = 1
+        """ Maximum recursion depth of lazy properties """
+
+        _lazy_properties: Dict[str, Callable[[], Awaitable[Any]]] = {}
+        """ Lazy property async function definitions """
+
     model_config = ConfigDict(
         str_strip_whitespace=True,
         extra="forbid",
         populate_by_name=True,
         arbitrary_types_allowed=True,
         ser_json_bytes='base64',
         validate_assignment=True,
     )
 
+    async def calc_lazy_properties(self):
+        """
+        (re)Calculate lazy properties
+        """
+        _lazy_semaphore = _lazy_property_semaphore.get()
+        # noinspection PyProtectedMember
+        for attr_name, attr in self.ESConfig._lazy_properties.items():
+            async with _lazy_semaphore:
+                # If we use create_task, this creates a new context, so changed contextvars live only upward
+                res = await asyncio.create_task(attr(self))
+                setattr(self, '_' + attr_name, res)
+
+        # Calc lazy properties for nested models
+        for k, v in self.__dict__.items():
+            if isinstance(v, ESBaseModel):
+                await v.calc_lazy_properties()
 
-class ESModel(ESBaseModel, metaclass=_ESModelMeta):
+
+class ESModel(ESBaseModel):
     """
     ElasticSearch Base Model
     """
 
     _id: Optional[str] = PrivateAttr(None)
     """ The ES id of the document """
 
@@ -365,26 +398,14 @@
 
         # Set routing field
         _routing = data.get("_routing", None)
         setattr(obj, '_routing', _routing)
 
         return obj
 
-    async def calc_lazy_properties(self):
-        """
-        (re)Calculate lazy properties
-        """
-        _lazy_semaphore = _lazy_property_semaphore.get()
-        # noinspection PyProtectedMember
-        for attr_name, attr in self.ESConfig._lazy_properties.items():
-            async with _lazy_semaphore:
-                # If we use create_task, this creates a new context, so changed contextvars live only upward
-                res = await asyncio.create_task(attr(self))
-                setattr(self, '_' + attr_name, res)
-
     async def save(self, *, wait_for=False, pipeline: Optional[str] = None, routing: Optional[str] = None) -> str:
         """
         Save document into elasticsearch.
 
         If document already exists, existing document will be updated as per native elasticsearch index operation.
         If model has id (Config.id_field or __id__), this will be used as the elasticsearch _id. The id field will be
         removed from the document before indexing.
@@ -716,15 +737,15 @@
     Process the results of ES query to calculate lazy properties recursively
 
     :param res: The result of the endpoint
     :return: The result of the endpoint
     """
     tasks = []
 
-    if isinstance(res, ESModel):
+    if isinstance(res, ESBaseModel):
         tasks.append(asyncio.create_task(res.calc_lazy_properties()))
 
     elif isinstance(res, list):
         for r in res:
             tasks.append(asyncio.create_task(r.calc_lazy_properties()))
 
     elif isinstance(res, dict):
```

### Comparing `pyesorm-0.3.1/esorm/query.py` & `pyesorm-0.3.2/esorm/query.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.1/esorm/response.py` & `pyesorm-0.3.2/esorm/response.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.1/esorm/utils.py` & `pyesorm-0.3.2/esorm/utils.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.1/esorm/watcher.py` & `pyesorm-0.3.2/esorm/watcher.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.1/pyesorm.egg-info/PKG-INFO` & `pyesorm-0.3.2/pyesorm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyesorm
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python ElasticSearch ORM based on Pydantic
 Home-page: https://github.com/wallneradam/esorm
 Author: Adam Wallner
 Author-email: Adam.wallner@gmail.com
 License: MPL-2.0
 Project-URL: Bug Tracker, https://github.com/wallneradam/esorm/issues
 Project-URL: Documentation, https://esorm.readthedocs.io/en/latest/
```

### Comparing `pyesorm-0.3.1/pyesorm.egg-info/SOURCES.txt` & `pyesorm-0.3.2/pyesorm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.1/setup.cfg` & `pyesorm-0.3.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyesorm
-version = 0.3.1
+version = 0.3.2
 author = Adam Wallner
 author_email = Adam.wallner@gmail.com
 description = Python ElasticSearch ORM based on Pydantic
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = ElasticSearch, ORM, Pydantic
 license = MPL-2.0
```

### Comparing `pyesorm-0.3.1/tests/conftest.py` & `pyesorm-0.3.2/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,18 +40,18 @@
 @pytest.fixture(scope="class")
 async def esorm():
     """
     Simply import esorm module
     This way it can be removed too
     """
     esorm = importlib.import_module('esorm')
-    esorm_model = importlib.import_module('esorm.model')
     # It should be empty for every class
-    assert len(esorm_model._ESModelMeta.__models__) == 0
+    assert len(esorm.model._ESModelMeta.__models__) == 0
     yield esorm
+    esorm.model._ESModelMeta.__models__.clear()
     for module_name in list(sys.modules):
         if module_name.startswith('esorm'):
             del sys.modules[module_name]
 
 
 @pytest.fixture(scope="class")  # Test both ES 8.x and 7.x
 def docker_es(service):
@@ -254,20 +254,45 @@
 
 # noinspection PyUnresolvedReferences
 @pytest.fixture(scope="class")
 async def model_nested_binary(esorm):
     """
     Model to test nested binary fields
     """
-    from pydantic import BaseModel
 
     class BinaryModel(esorm.ESBaseModel):
         f_binary: Optional[esorm.fields.binary] = esorm.Field(None, index=False)
 
     class NestedBinaryModel(esorm.ESModel):
         f_nested: BinaryModel
 
     await esorm.setup_mappings()
 
     yield BinaryModel, NestedBinaryModel
     del BinaryModel
     del NestedBinaryModel
+
+
+@pytest.fixture(scope="class")
+async def model_nested_base_model(esorm):
+    """
+    Model to test nested base model
+    """
+    from asyncio import sleep
+
+    class NestedBaseModel(esorm.ESBaseModel):
+        f_str: str
+        f_int: int
+
+        @esorm.lazy_property
+        async def lazy_prop(self) -> str:
+            await sleep(0.1)
+            return f'lazy(f_str={self.f_str}, f_int={self.f_int})'
+
+    class NestedBaseModelModel(esorm.ESModel):
+        f_nested: NestedBaseModel
+
+    await esorm.setup_mappings()
+
+    yield NestedBaseModel, NestedBaseModelModel
+    del NestedBaseModel
+    del NestedBaseModelModel
```

### Comparing `pyesorm-0.3.1/tests/test_esorm.py` & `pyesorm-0.3.2/tests/test_esorm.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,32 @@
 
     async def test_connect(self, es):
         """
         Test connection
         """
         assert es is not None
 
+    async def test_create_basemodel(self, es, esorm):
+        """
+        Test create base model
+        """
+
+        class BaseModel(esorm.ESBaseModel):
+            f_str: str
+            f_int: int
+
+        class BaseChild(BaseModel):
+            f_float: float
+
+        # Basemodels should not be registered as models they should not be created in the DB as indexes
+        # TODO: This is not working in the 2nd run, this is only test issue
+        # assert len(esorm.model._ESModelMeta.__models__) == 0
+        assert not hasattr(BaseModel.ESConfig, 'index')
+        assert not hasattr(BaseChild.ESConfig, 'index')
+
     async def test_create_model_with_python_fields(self, es, esorm, model_python):
         """
         Test model with python fields
         """
         assert model_python is not None
         assert model_python.ESConfig.index == 'esorm-python_field_model'
 
@@ -412,16 +430,15 @@
         assert res[0].f_nested.f_str == 'nested_test4'
         assert res[1].f_nested.f_str == 'nested_test5'
 
     async def test_sort(self, es, esorm, model_nested):
         """
         Test sort
         """
-        from esorm.model import set_max_lazy_property_concurrency
-        set_max_lazy_property_concurrency(2)
+        esorm.model.set_max_lazy_property_concurrency(2)
 
         sort = esorm.Sort(sort=[{'f_nested.f_int': {'order': 'asc'}}])
         res = await sort(model_nested).all()
         assert len(res) == 4
         assert res[0].f_nested.f_int == 2
         assert res[1].f_nested.f_int == 3
         assert res[2].f_nested.f_int == 4
@@ -569,7 +586,25 @@
         Test nested binary fields
         """
         binary_model, nested_binary_model = model_nested_binary
         doc = nested_binary_model(f_nested=binary_model())
         doc.f_nested.f_binary = b'\x01\x02\x03\x04'
         doc_id = await doc.save()
         assert doc_id is not None
+
+    async def test_nested_base_model_lazy_prop(self, es, esorm, model_nested_base_model):
+        """
+        Test nested base model
+        """
+        nested_base_model, nested_base_model_model = model_nested_base_model
+
+        assert nested_base_model.ESConfig._lazy_properties['lazy_prop'] is not None
+
+        doc = nested_base_model_model(f_nested=nested_base_model(f_str='test', f_int=1))
+        doc_id = await doc.save()
+        assert doc_id is not None
+
+        doc = await nested_base_model_model.get(doc_id)
+        assert doc is not None
+        assert doc.f_nested.f_str == 'test'
+        assert doc.f_nested.f_int == 1
+        assert doc.f_nested.lazy_prop == 'lazy(f_str=test, f_int=1)'
```


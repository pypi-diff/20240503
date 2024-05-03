# Comparing `tmp/sqlmodel_filters-0.0.6.tar.gz` & `tmp/sqlmodel_filters-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmodel_filters-0.0.6.tar", max compression
+gzip compressed data, was "sqlmodel_filters-0.0.7.tar", max compression
```

## Comparing `sqlmodel_filters-0.0.6.tar` & `sqlmodel_filters-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-04-26 00:40:51.787604 sqlmodel_filters-0.0.6/LICENSE
--rw-r--r--   0        0        0     8442 2024-04-26 00:40:51.787604 sqlmodel_filters-0.0.6/README.md
--rw-r--r--   0        0        0     1022 2024-04-26 00:41:05.451602 sqlmodel_filters-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       82 2024-04-26 00:40:51.787604 sqlmodel_filters-0.0.6/sqlmodel_filters/__init__.py
--rw-r--r--   0        0        0     7467 2024-04-26 00:40:51.787604 sqlmodel_filters-0.0.6/sqlmodel_filters/builder.py
--rw-r--r--   0        0        0     6802 2024-04-26 00:40:51.787604 sqlmodel_filters-0.0.6/sqlmodel_filters/components.py
--rw-r--r--   0        0        0      165 2024-04-26 00:40:51.787604 sqlmodel_filters-0.0.6/sqlmodel_filters/exceptions.py
--rw-r--r--   0        0        0      777 2024-04-26 00:40:51.787604 sqlmodel_filters-0.0.6/sqlmodel_filters/utils.py
--rw-r--r--   0        0        0     9027 1970-01-01 00:00:00.000000 sqlmodel_filters-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-03 00:29:09.341392 sqlmodel_filters-0.0.7/LICENSE
+-rw-r--r--   0        0        0     8433 2024-05-03 00:29:09.341392 sqlmodel_filters-0.0.7/README.md
+-rw-r--r--   0        0        0     1022 2024-05-03 00:29:25.205609 sqlmodel_filters-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       82 2024-05-03 00:29:09.341392 sqlmodel_filters-0.0.7/sqlmodel_filters/__init__.py
+-rw-r--r--   0        0        0     7467 2024-05-03 00:29:09.341392 sqlmodel_filters-0.0.7/sqlmodel_filters/builder.py
+-rw-r--r--   0        0        0     6941 2024-05-03 00:29:09.341392 sqlmodel_filters-0.0.7/sqlmodel_filters/components.py
+-rw-r--r--   0        0        0      165 2024-05-03 00:29:09.341392 sqlmodel_filters-0.0.7/sqlmodel_filters/exceptions.py
+-rw-r--r--   0        0        0      391 2024-05-03 00:29:09.341392 sqlmodel_filters-0.0.7/sqlmodel_filters/utils.py
+-rw-r--r--   0        0        0     9018 1970-01-01 00:00:00.000000 sqlmodel_filters-0.0.7/PKG-INFO
```

### Comparing `sqlmodel_filters-0.0.6/LICENSE` & `sqlmodel_filters-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmodel_filters-0.0.6/README.md` & `sqlmodel_filters-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -206,24 +206,22 @@
 ```py
 >>> tree = parse("name:*")
 >>> statement = builder(tree, entities=func.count(Hero.id))
 >>> session.scalar(statement)
 3
 ```
 
-## Default Fields
+### Default Fields
 
-Default fields are used if you don't set a field in a query.
+Default fields, all of the fields in a model by default, are used when you don't set a field in a query.
 
 | Query    | SQL (Where Clause)                                                    |
 | -------- | --------------------------------------------------------------------- |
 | `Spider` | `WHERE hero.name LIKE '%Spider%' OR hero.secret_name LIKE '%Spider%'` |
 
-The default fields are fields of a model by default.
-
 You can override the default by setting `default_fields`.
 
 ```py
 builder = SelectBuilder(Hero, default_fields={"name": Hero.model_fields["name"]})
 ```
 
 ### Helper Function
```

### Comparing `sqlmodel_filters-0.0.6/pyproject.toml` & `sqlmodel_filters-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlmodel-filters"
-version = "0.0.6"
+version = "0.0.7"
 description = "A Lucene query like fliltering for SQLModel"
 authors = ["Manabu Niseki <manabu.niseki@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -14,15 +14,15 @@
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.9"
 pre-commit = "^3.7"
 pytest = "^8.1"
 pytest-pretty = "^1.2"
 pytest-randomly = "^3.15"
 pyupgrade = "^3.15"
-ruff = "^0.3"
+ruff = "^0.4"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `sqlmodel_filters-0.0.6/sqlmodel_filters/builder.py` & `sqlmodel_filters-0.0.7/sqlmodel_filters/builder.py`

 * *Files identical despite different names*

### Comparing `sqlmodel_filters-0.0.6/sqlmodel_filters/components.py` & `sqlmodel_filters-0.0.7/sqlmodel_filters/components.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import contextlib
 from functools import cached_property
 from types import MappingProxyType
-from typing import TypeVar
+from typing import Annotated, Any, TypeVar
 
 from luqum.tree import From, Item, Phrase, Range, Regex, To, Word
+from pydantic import TypeAdapter
 from pydantic.fields import FieldInfo
 from sqlalchemy.orm.attributes import InstrumentedAttribute
 from sqlalchemy.sql._typing import _ColumnExpressionArgument
 from sqlmodel import SQLModel, and_
 
 from .exceptions import IllegalFieldError, IllegalFilterError
-from .utils import cast_by_annotation, dequote, deslash
+from .utils import dequote, deslash
 
 ModelType = TypeVar("ModelType", bound=SQLModel)
 
 
 def replace_wildcards(s: str, *, mapping: MappingProxyType[str, str]):
     for k, v in mapping.items():
         s = s.replace(k, v)
@@ -51,34 +52,34 @@
 
 class ModelField:
     def __init__(
         self,
         model: type[ModelType],
         name: str,
         *,
-        relationships: MappingProxyType[str, type[SQLModel]],
+        relationships: MappingProxyType[str, type[SQLModel]] | None = None,
     ):
         self.name = name
         self.model = model
-        self.relationships = relationships
+        self.relationships = relationships or MappingProxyType({})
 
     @cached_property
     def chains(self):
         return self.name.split(".")
 
     @property
     def is_chained(self) -> bool:
         return len(self.chains) > 1
 
     @cached_property
     def last_name(self) -> str:
         return self.chains[-1]
 
-    @property
-    def _model(self):
+    @cached_property
+    def chained_model(self):
         if not self.is_chained:
             return self.model
 
         model = self.model
         for chain in self.chains[:-2]:
             if chain not in model.__sqlmodel_relationships__:
                 raise IllegalFieldError(f"{model.__name__} does not have field:{chain}")
@@ -90,79 +91,82 @@
             return self.relationships[relationship_name]
         except KeyError as e:
             raise IllegalFieldError(f"{model.__name__} does not have field:{relationship_name}") from e
 
     @property
     def field(self) -> InstrumentedAttribute:
         try:
-            return getattr(self._model, self.last_name)
+            return getattr(self.chained_model, self.last_name)
         except AttributeError as e:
-            raise IllegalFieldError(f"{self._model.__name__} does not have field:{self.last_name}") from e
+            raise IllegalFieldError(f"{self.chained_model.__name__} does not have field:{self.last_name}") from e
 
-    @property
-    def annotation(self) -> type:
-        return self._model.model_fields[self.last_name].annotation  # type: ignore
+    @cached_property
+    def field_info(self) -> FieldInfo:
+        return self.chained_model.model_fields[self.last_name]
+
+    @cached_property
+    def type_adapter(self) -> TypeAdapter[Any]:
+        return TypeAdapter(Annotated[self.field_info.annotation, self.field_info])  # type: ignore
+
+    def cast(self, obj: Any) -> Any:
+        return self.type_adapter.validate_python(obj)
 
 
 class SearchFieldNode:
     def __init__(
         self, node: Item, *, model: type[ModelType], name: str, relationships: MappingProxyType[str, type[SQLModel]]
     ):
         self.node = node
         self.model_field = ModelField(model, name, relationships=relationships)
 
     @property
     def field(self):
         return self.model_field.field
 
-    @property
-    def annotation(self):
-        return self.model_field.annotation
-
     def _phrase_expression(self, phrase: Phrase):
-        yield self.field == cast_by_annotation(dequote(phrase.value), self.annotation)
+        yield self.field == self.model_field.cast(dequote(phrase.value))
 
     def _word_expression(self, word: Word):
         if word.value == "*":
             yield self.field.isnot(None)
         else:
-            casted = cast_by_annotation(word.value, self.annotation)
+            casted = self.model_field.cast(word.value)
             if isinstance(casted, str):
                 yield self.field.like(str(LikeWord(casted)))
             else:
                 yield self.field == casted
 
     def _range_expressions(self, range: Range):
         expressions: list[_ColumnExpressionArgument] = []
 
         if range.include_high:
-            expressions.append(self.field <= cast_by_annotation(range.high.value, self.annotation))
+            expressions.append(self.field <= self.model_field.cast(range.high.value))
         else:
-            expressions.append(self.field < cast_by_annotation(range.high.value, self.annotation))
+            expressions.append(self.field < self.model_field.cast(range.high.value))
 
         if range.include_low:
-            expressions.append(self.field >= cast_by_annotation(range.low.value, self.annotation))
+            expressions.append(self.field >= self.model_field.cast(range.low.value))
         else:
-            expressions.append(self.field > cast_by_annotation(range.low.value, self.annotation))
+            expressions.append(self.field > self.model_field.cast(range.low.value))
 
         yield and_(*expressions)
 
     def _from_expression(self, from_: From):
         child: Word = from_.children[0]
         if from_.include:
-            yield self.field >= cast_by_annotation(child.value, self.annotation)
+            yield self.field >= self.model_field.cast(child.value)
         else:
-            yield self.field > cast_by_annotation(child.value, self.annotation)
+            yield self.field > self.model_field.cast(child.value)
 
     def _to_expression(self, to: To):
         child: Word = to.children[0]
         if to.include:
-            yield self.field <= cast_by_annotation(child.value, self.annotation)
+            yield self.field <= self.model_field.cast(child.value)
         else:
-            yield self.field < cast_by_annotation(child.value, self.annotation)
+            yield self.field < self.model_field.cast(child.value)
 
     def _regex_expression(self, regex: Regex):
         yield self.field.regexp_match(deslash(regex.value))
 
     def get_expressions(self):
         match self.node:
             case Phrase():
@@ -187,19 +191,20 @@
         self.model = model
         self.default_fields = default_fields or model.model_fields
 
     def get_field(self, name) -> InstrumentedAttribute:
         return getattr(self.model, name)
 
     def get_expressions(self):
-        for name, field_info in self.default_fields.items():
+        for name in self.default_fields:
+            model_field = ModelField(self.model, name=name)
             with contextlib.suppress(Exception):
                 field = self.get_field(name)
 
                 if self.node.value == "*":
                     yield field.isnot(None)
                 else:
-                    casted = cast_by_annotation(self.node.value, field_info.annotation)
+                    casted = model_field.cast(self.node.value)
                     if isinstance(casted, str):
                         yield field.like(str(LikeWord(casted)))
                     else:
                         yield field == casted
```

### Comparing `sqlmodel_filters-0.0.6/PKG-INFO` & `sqlmodel_filters-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmodel-filters
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Lucene query like fliltering for SQLModel
 License: MIT
 Author: Manabu Niseki
 Author-email: manabu.niseki@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -223,24 +223,22 @@
 ```py
 >>> tree = parse("name:*")
 >>> statement = builder(tree, entities=func.count(Hero.id))
 >>> session.scalar(statement)
 3
 ```
 
-## Default Fields
+### Default Fields
 
-Default fields are used if you don't set a field in a query.
+Default fields, all of the fields in a model by default, are used when you don't set a field in a query.
 
 | Query    | SQL (Where Clause)                                                    |
 | -------- | --------------------------------------------------------------------- |
 | `Spider` | `WHERE hero.name LIKE '%Spider%' OR hero.secret_name LIKE '%Spider%'` |
 
-The default fields are fields of a model by default.
-
 You can override the default by setting `default_fields`.
 
 ```py
 builder = SelectBuilder(Hero, default_fields={"name": Hero.model_fields["name"]})
 ```
 
 ### Helper Function
```


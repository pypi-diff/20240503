# Comparing `tmp/clickhouse-query-0.0.7.tar.gz` & `tmp/clickhouse_query-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse-query-0.0.7.tar", last modified: Thu Mar 28 14:25:28 2024, max compression
+gzip compressed data, was "clickhouse_query-0.1.0.tar", last modified: Fri May  3 12:12:15 2024, max compression
```

## Comparing `clickhouse-query-0.0.7.tar` & `clickhouse_query-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:25:28.817286 clickhouse-query-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-28 14:25:19.000000 clickhouse-query-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-28 14:25:28.817286 clickhouse-query-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-03-28 14:25:19.000000 clickhouse-query-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:25:28.817286 clickhouse-query-0.0.7/clickhouse_query/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-28 14:25:19.000000 clickhouse-query-0.0.7/clickhouse_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-03-28 14:25:19.000000 clickhouse-query-0.0.7/clickhouse_query/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-28 14:25:19.000000 clickhouse-query-0.0.7/clickhouse_query/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    15182 2024-03-28 14:25:19.000000 clickhouse-query-0.0.7/clickhouse_query/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-03-28 14:25:19.000000 clickhouse-query-0.0.7/clickhouse_query/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:25:28.817286 clickhouse-query-0.0.7/clickhouse_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-28 14:25:28.000000 clickhouse-query-0.0.7/clickhouse_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-28 14:25:28.000000 clickhouse-query-0.0.7/clickhouse_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 14:25:28.000000 clickhouse-query-0.0.7/clickhouse_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-28 14:25:28.000000 clickhouse-query-0.0.7/clickhouse_query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-28 14:25:19.000000 clickhouse-query-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 14:25:28.817286 clickhouse-query-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-28 14:25:19.000000 clickhouse-query-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:25:28.817286 clickhouse-query-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-28 14:25:19.000000 clickhouse-query-0.0.7/tests/test_clickhouse_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:12:15.836703 clickhouse_query-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-03 12:12:07.000000 clickhouse_query-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-03 12:12:15.836703 clickhouse_query-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-03 12:12:07.000000 clickhouse_query-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:12:15.836703 clickhouse_query-0.1.0/clickhouse_query/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-03 12:12:07.000000 clickhouse_query-0.1.0/clickhouse_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-03 12:12:07.000000 clickhouse_query-0.1.0/clickhouse_query/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-03 12:12:07.000000 clickhouse_query-0.1.0/clickhouse_query/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-05-03 12:12:07.000000 clickhouse_query-0.1.0/clickhouse_query/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-03 12:12:07.000000 clickhouse_query-0.1.0/clickhouse_query/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:12:15.836703 clickhouse_query-0.1.0/clickhouse_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-03 12:12:15.000000 clickhouse_query-0.1.0/clickhouse_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-03 12:12:15.000000 clickhouse_query-0.1.0/clickhouse_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:12:15.000000 clickhouse_query-0.1.0/clickhouse_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 12:12:15.000000 clickhouse_query-0.1.0/clickhouse_query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-03 12:12:07.000000 clickhouse_query-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:12:15.836703 clickhouse_query-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-03 12:12:07.000000 clickhouse_query-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:12:15.836703 clickhouse_query-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-03 12:12:07.000000 clickhouse_query-0.1.0/tests/test_clickhouse_query.py
```

### Comparing `clickhouse-query-0.0.7/LICENSE` & `clickhouse_query-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clickhouse-query-0.0.7/PKG-INFO` & `clickhouse_query-0.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 Metadata-Version: 2.1
 Name: clickhouse-query
-Version: 0.0.7
+Version: 0.1.0
 Summary: clickhouse query
 Home-page: https://github.com/mehrh8/clickhouse-query
 Author: Mehrshad Hosseini
 Author-email: mehrh8@gmail.com
 Project-URL: Bug Tracker, https://github.com/mehrh8/clickhouse-query/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ClickHouse Query
-**!!! This repository is not complete, so the following codes may not work in current version. !!!**
 
-Clickhouse Query is a Python library for building complex ClickHouse queries by a fluent API and a set of functions.
+**ClickHouse Query** is a Python library designed to simplify the construction of complex ClickHouse queries. It provides a fluent API and a comprehensive set of functions for this purpose.
+
 
 ## Installation
 
+You can install the ClickHouse Query library using pip. Run the following command in your terminal:
+
+
 ```bash
 pip install clickhouse-query
 ```
 
 ## Usage
 
-**!!! This repository is not complete, so the following codes may not work in current version. !!!**
+Here’s an example of how to use the ClickHouse Query library:
 
 ```python
 import clickhouse_query as ch
+from clickhouse_query import functions as chf
 
+# Create a QuerySet instance for your table
 q = (
-    ch.QuerySet()
-    .from_("my_table")
-    .prewhere(date__year__gte="2024")
-    .select(count=ch.Count())
-    .limit(10)
+    ch.QuerySet("my_table", clickhouse_client=...)
+    .prewhere(date__year__gte=2020)  # Add a prewhere condition
+    .group_by("status")  # Group by status
+    .select("status", s=chf.sum("price"))  # Select status and sum
+    .order_by("-s")  # Order by sum in descending order
+    .limit(10)  # Limit the results to 10
 )
 
+# Get the SQL query and parameters
 sql, sql_params  = ch.get_sql(q)
-# sql = 'SELECT count() AS count FROM click PREWHERE (greaterOrEquals(toYear(date), %(__U_1)s)) LIMIT %(__U_2)f'
-# sql_params = {'__U_1': 2024, '__U_2': 10}
+# sql = 'SELECT status, sum(price) AS cnt FROM my_table PREWHERE (greaterOrEquals(toYear(date), %(__U_1)f)) GROUP BY status ORDER BY cnt DESC LIMIT %(__U_2)f'
+# sql_params = {'__U_1': 2020, '__U_2': 10}
 
+# Execute the query
 data = q.execute()
-# data = [{'count': 100}]
+# data = [{"status": "status1", "s": 200}, {"status": "status2", "s": 100}, ...]
 ```
 
-## Custom Functions
+In this example, `sql` will contain the generated SQL query and `sql_params` will contain its parameters. The `execute` method will execute the query and return the data.
 
-If there is not a function that you need, you can easily create it by extending the `Function` class. like this:
 
-```python
-class MyFunction(ch.Function):
-    function = "my_function"
-```
 
-## Custom Aggregation Functions
+## Docs
+
+For more detailed information on how to use the ClickHouse Query library, please refer to the documentation in the [docs](docs/doc.md) directory.
 
-If there is not a aggregation function that you need, you can easily create it by extending the `AggregationFunction` class. like this:
 
-```python
-class MyAggregationFunction(ch.AggregationFunction):
-    function = "my_aggregation_function"
-```
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `clickhouse-query-0.0.7/clickhouse_query/mixins.py` & `clickhouse_query-0.1.0/clickhouse_query/mixins.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,39 +28,39 @@
         return ""
 
 
 class ArithmeticMixin:
     def __add__(self, other):
         from clickhouse_query import functions
 
-        return functions.Plus(self, other)
+        return functions.plus(self, other)
 
     def __sub__(self, other):
         from clickhouse_query import functions
 
-        return functions.Minus(self, other)
+        return functions.minus(self, other)
 
     def __mul__(self, other):
         from clickhouse_query import functions
 
-        return functions.Multiply(self, other)
+        return functions.multiply(self, other)
 
     def __truediv__(self, other):
         from clickhouse_query import functions
 
-        return functions.Divide(self, other)
+        return functions.divide(self, other)
 
     def __floordiv__(self, other):
         from clickhouse_query import functions
 
         # TODO: cast self to Float64
-        return functions.IntDiv(self, other)
+        return functions.intDiv(self, other)
 
     def __mod__(self, other):
         from clickhouse_query import functions
 
-        return functions.Modulo(self, other)
+        return functions.modulo(self, other)
 
     def __neg__(self):
         from clickhouse_query import functions
 
-        return functions.Negate(self)
+        return functions.negate(self)
```

### Comparing `clickhouse-query-0.0.7/clickhouse_query/models.py` & `clickhouse_query-0.1.0/clickhouse_query/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 import datetime
 from zoneinfo import ZoneInfo
 
 from clickhouse_query import Function, mixins, utils
 
 
 class QuerySet:
-    def __init__(self, inplace=False):
+    def __init__(self, _from=None, inplace=False, clickhouse_client=None):
         self._from = None
         self._select = []
         self._distinct = None
         self._prewhere = []
         self._where = []
         self._group_by = []
         self._having = []
         self._order_by = []
         self._limit = None
         self._limit_by = None
 
         self.inplace = inplace
+        self.clickhouse_client = clickhouse_client
+
+        self.enable_inplace().from_(_from).disable_inplace()
 
     def _clone(self):
         if not self.inplace:
             self = copy.deepcopy(self)
         return self
 
     def disable_inplace(self):
@@ -42,15 +45,15 @@
 
         self._select = []
         for item in args:
             expression = utils.get_expression(item, str_is_field=True)
             self._select.append(expression)
         for as_, item in kwargs.items():
             expression = utils.get_expression(item, str_is_field=True)
-            expression.as_(as_)
+            expression = expression.as_(as_)
             self._select.append(expression)
         return self
 
     def distinct(self, *args):
         self = self._clone()
 
         if args and args[0] is None:
@@ -341,15 +344,21 @@
             having=having_sql,
             order_by=order_by_sql,
             limit_by=limit_by_sql,
             limit=limit_sql,
         )
         return sql, sql_params
 
-    def execute(self, clickhouse_client):
+    def execute(self, clickhouse_client=None):
+        if clickhouse_client is None:
+            clickhouse_client = self.clickhouse_client
+
+        if callable(clickhouse_client):
+            clickhouse_client = clickhouse_client()
+
         sql, sql_params = utils.get_sql(self)
 
         values_list, column__type = clickhouse_client.execute(sql, params=sql_params, with_column_types=True)
 
         data = []
         for values in values_list:
             data.append({column: value for (column, type), value in zip(column__type, values)})  # noqa: B905
```

### Comparing `clickhouse-query-0.0.7/clickhouse_query/utils.py` & `clickhouse_query-0.1.0/clickhouse_query/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,83 +34,83 @@
     from clickhouse_query import functions, models
 
     *_field, op = item.split("__")
 
     field = models.F(_field)
     if op == "exact":
         if value is None:
-            condition = functions.IsNull(field)
+            condition = functions.isNull(field)
         else:
-            condition = functions.Equals(field, value)
+            condition = functions.equals(field, value)
     elif op == "iexact":
         if value is None:
-            condition = functions.IsNull(field)
+            condition = functions.isNull(field)
         else:
-            condition = functions.ILike(field, value)
+            condition = functions.iLike(field, value)
     elif op == "contains":
-        condition = functions.Like(field, functions.Concat(models.Value("%"), value, models.Value("%")))
+        condition = functions.like(field, functions.concat(models.Value("%"), value, models.Value("%")))
     elif op == "icontains":
-        condition = functions.ILike(field, functions.Concat(models.Value("%"), value, models.Value("%")))
+        condition = functions.iLike(field, functions.concat(models.Value("%"), value, models.Value("%")))
     elif op == "in":
-        condition = functions.In(field, value)
+        condition = functions.in_(field, value)
     elif op == "gt":
-        condition = functions.Greater(field, value)
+        condition = functions.greater(field, value)
     elif op == "gte":
-        condition = functions.GreaterOrEquals(field, value)
+        condition = functions.greaterOrEquals(field, value)
     elif op == "lt":
-        condition = functions.Less(field, value)
+        condition = functions.less(field, value)
     elif op == "lte":
-        condition = functions.LessOrEquals(field, value)
+        condition = functions.lessOrEquals(field, value)
     elif op == "startswith":
-        condition = functions.Like(field, functions.Concat(value, models.Value("%")))
+        condition = functions.like(field, functions.concat(value, models.Value("%")))
     elif op == "istartswith":
-        condition = functions.ILike(field, functions.Concat(value, models.Value("%")))
+        condition = functions.iLike(field, functions.concat(value, models.Value("%")))
     elif op == "endswith":
-        condition = functions.Like(field, functions.Concat(models.Value("%"), value))
+        condition = functions.like(field, functions.concat(models.Value("%"), value))
     elif op == "iendswith":
-        condition = functions.ILike(field, functions.Concat(models.Value("%"), value))
+        condition = functions.iLike(field, functions.concat(models.Value("%"), value))
     elif op == "isnull":
         if value.arg is True:
-            condition = functions.IsNull(field)
+            condition = functions.isNull(field)
         elif value.arg is False:
-            condition = functions.IsNotNull(field)
+            condition = functions.isNotNull(field)
         else:
             raise ValueError("isnull value should be True or False")
     else:  # equals
         field = models.F(_field + [op])
-        condition = functions.Equals(field, value)
+        condition = functions.equals(field, value)
 
     return condition
 
 
 def _apply_operator(field, op):
     from clickhouse_query import functions
 
     if op[0] == "_":  # nested
         field = field._arg_extend("." + op[1:])
     elif op == "year":
-        field = functions.ToYear(field)
+        field = functions.toYear(field)
     elif op == "month":
-        field = functions.ToMonth(field)
+        field = functions.toMonth(field)
     elif op == "day":
-        field = functions.ToDayOfYear(field)
+        field = functions.toDayOfYear(field)
     elif op == "week":
-        field = functions.ToWeek(field)
+        field = functions.toWeek(field)
     elif op == "week_day":
-        field = functions.ToDayOfWeek(field)
+        field = functions.toDayOfWeek(field)
     elif op == "quarter":
-        field = functions.ToQuarter(field)
+        field = functions.toQuarter(field)
     elif op == "time":
-        field = functions.ToTime(field)
+        field = functions.toTime(field)
     elif op == "hour":
-        field = functions.ToHour(field)
+        field = functions.toHour(field)
     elif op == "minute":
-        field = functions.ToMinute(field)
+        field = functions.toMinute(field)
     elif op == "second":
-        field = functions.ToSecond(field)
+        field = functions.toSecond(field)
     else:
         # not changed
         return field._arg_extend("__" + op)
 
     return field
```

### Comparing `clickhouse-query-0.0.7/clickhouse_query.egg-info/PKG-INFO` & `clickhouse_query-0.1.0/clickhouse_query.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 Metadata-Version: 2.1
 Name: clickhouse-query
-Version: 0.0.7
+Version: 0.1.0
 Summary: clickhouse query
 Home-page: https://github.com/mehrh8/clickhouse-query
 Author: Mehrshad Hosseini
 Author-email: mehrh8@gmail.com
 Project-URL: Bug Tracker, https://github.com/mehrh8/clickhouse-query/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ClickHouse Query
-**!!! This repository is not complete, so the following codes may not work in current version. !!!**
 
-Clickhouse Query is a Python library for building complex ClickHouse queries by a fluent API and a set of functions.
+**ClickHouse Query** is a Python library designed to simplify the construction of complex ClickHouse queries. It provides a fluent API and a comprehensive set of functions for this purpose.
+
 
 ## Installation
 
+You can install the ClickHouse Query library using pip. Run the following command in your terminal:
+
+
 ```bash
 pip install clickhouse-query
 ```
 
 ## Usage
 
-**!!! This repository is not complete, so the following codes may not work in current version. !!!**
+Here’s an example of how to use the ClickHouse Query library:
 
 ```python
 import clickhouse_query as ch
+from clickhouse_query import functions as chf
 
+# Create a QuerySet instance for your table
 q = (
-    ch.QuerySet()
-    .from_("my_table")
-    .prewhere(date__year__gte="2024")
-    .select(count=ch.Count())
-    .limit(10)
+    ch.QuerySet("my_table", clickhouse_client=...)
+    .prewhere(date__year__gte=2020)  # Add a prewhere condition
+    .group_by("status")  # Group by status
+    .select("status", s=chf.sum("price"))  # Select status and sum
+    .order_by("-s")  # Order by sum in descending order
+    .limit(10)  # Limit the results to 10
 )
 
+# Get the SQL query and parameters
 sql, sql_params  = ch.get_sql(q)
-# sql = 'SELECT count() AS count FROM click PREWHERE (greaterOrEquals(toYear(date), %(__U_1)s)) LIMIT %(__U_2)f'
-# sql_params = {'__U_1': 2024, '__U_2': 10}
+# sql = 'SELECT status, sum(price) AS cnt FROM my_table PREWHERE (greaterOrEquals(toYear(date), %(__U_1)f)) GROUP BY status ORDER BY cnt DESC LIMIT %(__U_2)f'
+# sql_params = {'__U_1': 2020, '__U_2': 10}
 
+# Execute the query
 data = q.execute()
-# data = [{'count': 100}]
+# data = [{"status": "status1", "s": 200}, {"status": "status2", "s": 100}, ...]
 ```
 
-## Custom Functions
+In this example, `sql` will contain the generated SQL query and `sql_params` will contain its parameters. The `execute` method will execute the query and return the data.
 
-If there is not a function that you need, you can easily create it by extending the `Function` class. like this:
 
-```python
-class MyFunction(ch.Function):
-    function = "my_function"
-```
 
-## Custom Aggregation Functions
+## Docs
+
+For more detailed information on how to use the ClickHouse Query library, please refer to the documentation in the [docs](docs/doc.md) directory.
 
-If there is not a aggregation function that you need, you can easily create it by extending the `AggregationFunction` class. like this:
 
-```python
-class MyAggregationFunction(ch.AggregationFunction):
-    function = "my_aggregation_function"
-```
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `clickhouse-query-0.0.7/pyproject.toml` & `clickhouse_query-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clickhouse-query-0.0.7/setup.py` & `clickhouse_query-0.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="clickhouse-query",
-    version="0.0.7",
+    version="0.1.0",
     author="Mehrshad Hosseini",
     author_email="mehrh8@gmail.com",
     description="clickhouse query",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mehrh8/clickhouse-query",
     project_urls={
         "Bug Tracker": "https://github.com/mehrh8/clickhouse-query/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    packages=setuptools.find_packages(".", exclude=["tests*"]),
+    packages=["clickhouse_query"],
     python_requires=">=3.6",
 )
```


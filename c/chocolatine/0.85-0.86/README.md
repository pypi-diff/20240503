# Comparing `tmp/chocolatine-0.85.tar.gz` & `tmp/chocolatine-0.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chocolatine-0.85.tar", last modified: Thu Apr 25 12:32:05 2024, max compression
+gzip compressed data, was "chocolatine-0.86.tar", last modified: Fri May  3 09:17:05 2024, max compression
```

## Comparing `chocolatine-0.85.tar` & `chocolatine-0.86.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:32:05.607129 chocolatine-0.85/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-25 12:31:52.000000 chocolatine-0.85/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-25 12:32:05.607129 chocolatine-0.85/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-25 12:31:52.000000 chocolatine-0.85/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:32:05.603129 chocolatine-0.85/chocolatine/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/agg_function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:32:05.607129 chocolatine-0.85/chocolatine/expr/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/choc_expr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/choc_expr_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/col.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/col_when.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/delete_from.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/expr.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/from_expr.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/group_by.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/having.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/join.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/limit.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/order_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/select.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/select_from.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/table.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/update.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/update_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/when.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/expr/where.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/join_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/query_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/shortcut.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/sql_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/type.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-25 12:31:52.000000 chocolatine-0.85/chocolatine/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:32:05.607129 chocolatine-0.85/chocolatine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-25 12:32:05.000000 chocolatine-0.85/chocolatine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-25 12:32:05.000000 chocolatine-0.85/chocolatine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:32:05.000000 chocolatine-0.85/chocolatine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 12:32:05.000000 chocolatine-0.85/chocolatine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 12:32:05.000000 chocolatine-0.85/chocolatine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-25 12:31:52.000000 chocolatine-0.85/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-25 12:32:05.607129 chocolatine-0.85/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:32:05.607129 chocolatine-0.85/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13748 2024-04-25 12:31:52.000000 chocolatine-0.85/tests/test_sakila_challenge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:17:05.473028 chocolatine-0.86/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-03 09:16:52.000000 chocolatine-0.86/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-03 09:17:05.473028 chocolatine-0.86/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-03 09:16:52.000000 chocolatine-0.86/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:17:05.469028 chocolatine-0.86/chocolatine/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/agg_function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:17:05.473028 chocolatine-0.86/chocolatine/expr/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/col.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/col_when.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/delete_from.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/from_expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/group_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/having.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/order_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/select_from.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/union.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/update_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/when.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/expr/where.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/join_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/query_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/shortcut.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/sql_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-03 09:16:52.000000 chocolatine-0.86/chocolatine/view_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:17:05.473028 chocolatine-0.86/chocolatine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-03 09:17:05.000000 chocolatine-0.86/chocolatine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-03 09:17:05.000000 chocolatine-0.86/chocolatine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:17:05.000000 chocolatine-0.86/chocolatine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-03 09:17:05.000000 chocolatine-0.86/chocolatine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-03 09:17:05.000000 chocolatine-0.86/chocolatine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-03 09:16:52.000000 chocolatine-0.86/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-03 09:17:05.473028 chocolatine-0.86/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:17:05.473028 chocolatine-0.86/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14337 2024-05-03 09:16:52.000000 chocolatine-0.86/tests/test_sakila_challenge.py
```

### Comparing `chocolatine-0.85/LICENSE` & `chocolatine-0.86/LICENSE`

 * *Files identical despite different names*

### Comparing `chocolatine-0.85/PKG-INFO` & `chocolatine-0.86/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 Metadata-Version: 2.1
 Name: chocolatine
-Version: 0.85
+Version: 0.86
 Summary: A lightweight Python library to easily generate SQL queries
 Home-page: https://github.com/pe-brian/chocolatine
 Author: Pierre-Emmanuel Brian
 Author-email: pebrian@outlook.fr
 Project-URL: Bug Tracker, https://github.com/pe-brian/chocolatine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typeguard==4.1.5
+Requires-Dist: choc-expr==1.0
+
+[![PyPI version](https://badge.fury.io/py/chocolatine.svg)](https://badge.fury.io/py/chocolatine) ![Licence badge](https://img.shields.io/pypi/l/chocolatine) ![Python version](https://img.shields.io/pypi/pyversions/chocolatine)
+[![Actions Status](https://github.com/pe-brian/chocolatine/workflows/validate-dev-push/badge.svg)](https://github.com/pe-brian/chocolatine/actions)
+![Dependencies](https://img.shields.io/badge/dependencies-typeguard-yellowgreen)
+![Dependencies](https://img.shields.io/badge/dependencies-choc_expr-yellowgreen)
+![Downloads per month](https://img.shields.io/pypi/dm/chocolatine)
+![Last commit](https://img.shields.io/github/last-commit/pe-brian/chocolatine)
 
 # chocolatine
 
 ![Image](logo.jpg)
 
 Chocolatine is a lightweight python library designed to easily generate SQL queries.
 
 # Why Chocolatine ?
 
-If you know Python programming langage but you are not at your ease with SQL (or you don't want to manage SQL requests by yourself), you can use Chocolatine to generate some SQL queries for you.
+If you know Python programming langage but you are not at your ease with SQL (or you don't want to manage SQL queries by yourself), you can use Chocolatine to generate some SQL queries for you.
 Of course, there are many other open source projects to do that, but honestly, they are more complex than most people expects from them (SQLAlchemy, Django ORM, etc...).
 
+# Installation
+
+```pip install chocolatine```
+
 # Examples
 
 __Concatenation & filtering__ :
 ```python
 from chocolatine import Query, Col as _
 
 query = Query().table("customer")\
@@ -101,52 +113,48 @@
 # SQL dialect
 
 For now, Chocolatine is only designed to generate MySQL queries.
 It is not excluded that in the future it will be compatible with Sqlite3, SqlServer or postgreSQL
 
 # Basic functionnalities
 
-- Select requests
+- Select, Update & delete queries
 - Distinct
-- Aliases (for columns & tables)
-- Ordering
-- Group by
-- Aggregation functions
+- Names aliases
+- Columns ordering
+- Group by & aggregations
 - Joins
 - SQL functions
 - Concatenations
+- Unions
+- Case-When
 
 # Advanced functionnalities
 
 - Dynamic type checking
 - Use of : or @ in col or table name directly for alias
 - Protection against SQL injection attacks
 - Calls orders doesn't matter (except for join clauses)
 - Compact or extended SQL expressions
 - Whole system to deal with conditions (logical operators, boolean operators, priority order)
 - Automatic handling of filter conditions to fill the having or where clause depending on the given columns
 - Shortcut functions : Asc, Desc, Sum, Count, Upper, Lower, Concat, Second, Minute, Hour, Day, Month, Year
 - \>: or <: at first position in column name (or alias) in select to set the ordering
 - \>\> operator to perform a "like" condition on a column
 - << operator to perform a "in" condition on a column
-- Limit clause
-- Nested requests
-- "ChocExpr" mini langage for SQL requests templating :
+- Nested queries
+- "ChocExpr" mini langage for SQL queries templating :
     - Conditions
     - Basic loops (with unpacking lists)
-- Case When
-- Update requests
-- Delete requests
 
 # To-do
 
-- Tables union
+- Equality evaluation in ChocExpr if statements
 - Option to disable dynamic type checking (for performance concerns)
-- Create requests
-- Pypi package (to install with pip install)
+- Create queries
 - SQLServer compatibility
 - PostGreSQL compatibility
 - SQLite3 compatibility
 
 # Tests
 
 ```python pytest```
```

### Comparing `chocolatine-0.85/README.md` & `chocolatine-0.86/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,29 @@
+[![PyPI version](https://badge.fury.io/py/chocolatine.svg)](https://badge.fury.io/py/chocolatine) ![Licence badge](https://img.shields.io/pypi/l/chocolatine) ![Python version](https://img.shields.io/pypi/pyversions/chocolatine)
+[![Actions Status](https://github.com/pe-brian/chocolatine/workflows/validate-dev-push/badge.svg)](https://github.com/pe-brian/chocolatine/actions)
+![Dependencies](https://img.shields.io/badge/dependencies-typeguard-yellowgreen)
+![Dependencies](https://img.shields.io/badge/dependencies-choc_expr-yellowgreen)
+![Downloads per month](https://img.shields.io/pypi/dm/chocolatine)
+![Last commit](https://img.shields.io/github/last-commit/pe-brian/chocolatine)
+
 # chocolatine
 
 ![Image](logo.jpg)
 
 Chocolatine is a lightweight python library designed to easily generate SQL queries.
 
 # Why Chocolatine ?
 
-If you know Python programming langage but you are not at your ease with SQL (or you don't want to manage SQL requests by yourself), you can use Chocolatine to generate some SQL queries for you.
+If you know Python programming langage but you are not at your ease with SQL (or you don't want to manage SQL queries by yourself), you can use Chocolatine to generate some SQL queries for you.
 Of course, there are many other open source projects to do that, but honestly, they are more complex than most people expects from them (SQLAlchemy, Django ORM, etc...).
 
+# Installation
+
+```pip install chocolatine```
+
 # Examples
 
 __Concatenation & filtering__ :
 ```python
 from chocolatine import Query, Col as _
 
 query = Query().table("customer")\
@@ -85,52 +96,48 @@
 # SQL dialect
 
 For now, Chocolatine is only designed to generate MySQL queries.
 It is not excluded that in the future it will be compatible with Sqlite3, SqlServer or postgreSQL
 
 # Basic functionnalities
 
-- Select requests
+- Select, Update & delete queries
 - Distinct
-- Aliases (for columns & tables)
-- Ordering
-- Group by
-- Aggregation functions
+- Names aliases
+- Columns ordering
+- Group by & aggregations
 - Joins
 - SQL functions
 - Concatenations
+- Unions
+- Case-When
 
 # Advanced functionnalities
 
 - Dynamic type checking
 - Use of : or @ in col or table name directly for alias
 - Protection against SQL injection attacks
 - Calls orders doesn't matter (except for join clauses)
 - Compact or extended SQL expressions
 - Whole system to deal with conditions (logical operators, boolean operators, priority order)
 - Automatic handling of filter conditions to fill the having or where clause depending on the given columns
 - Shortcut functions : Asc, Desc, Sum, Count, Upper, Lower, Concat, Second, Minute, Hour, Day, Month, Year
 - \>: or <: at first position in column name (or alias) in select to set the ordering
 - \>\> operator to perform a "like" condition on a column
 - << operator to perform a "in" condition on a column
-- Limit clause
-- Nested requests
-- "ChocExpr" mini langage for SQL requests templating :
+- Nested queries
+- "ChocExpr" mini langage for SQL queries templating :
     - Conditions
     - Basic loops (with unpacking lists)
-- Case When
-- Update requests
-- Delete requests
 
 # To-do
 
-- Tables union
+- Equality evaluation in ChocExpr if statements
 - Option to disable dynamic type checking (for performance concerns)
-- Create requests
-- Pypi package (to install with pip install)
+- Create queries
 - SQLServer compatibility
 - PostGreSQL compatibility
 - SQLite3 compatibility
 
 # Tests
 
 ```python pytest```
```

### Comparing `chocolatine-0.85/chocolatine/expr/__init__.py` & `chocolatine-0.86/chocolatine/expr/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from .choc_expr import ChocExpr  # noqa
 from .table import Table  # noqa
 from .from_expr import FromExpr  # noqa
 from .select_from import SelectFrom  # noqa
 from .select import Select  # noqa
 from .limit import Limit  # noqa
 from .query import Query  # noqa
 from .col import Col  # noqa
 from .col_when import ColWhen  # noqa
 from .when import When  # noqa
 from .condition import Condition  # noqa
 from .where import Where  # noqa
 from .having import Having  # noqa
-from .choc_expr_attr import ChocExprAttr  # noqa
 from .group_by import GroupBy  # noqa
 from .order_by import OrderBy  # noqa
 from .join import Join  # noqa
 from .set import Set  # noqa
 from .update import Update  # noqa
 from .update_set import UpdateSet  # noqa
 from .delete import Delete  # noqa
 from .delete_from import DeleteFrom  # noqa
+from .union import Union  # noqa
+from .view import View  # noqa
```

### Comparing `chocolatine-0.85/chocolatine/expr/col.py` & `chocolatine-0.86/chocolatine/expr/col.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from typing import Iterable, Self, TYPE_CHECKING
 
 
 if TYPE_CHECKING:
     from .query import Query
 
 from typeguard import typechecked
+from choc_expr import Expr as ChocExpr
 
 from .when import When
-from .choc_expr import ChocExpr
 from .condition import Condition
 from ..operator import Operator
 from ..ordering import Ordering
 from ..agg_function import AggFunction
 from ..sql_function import SqlFunction
```

### Comparing `chocolatine-0.85/chocolatine/expr/col_when.py` & `chocolatine-0.86/chocolatine/expr/col_when.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable
 
 from typeguard import typechecked
+from choc_expr import Expr as ChocExpr
 
-from .choc_expr import ChocExpr
 from .col import Col
 from ..utils import quote_expr
 
 
 @typechecked
 class ColWhen(ChocExpr):
     """ 'Case When' expression  """
```

### Comparing `chocolatine-0.85/chocolatine/expr/condition.py` & `chocolatine-0.86/chocolatine/expr/condition.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from typing import Self, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from .col import Col
     from .when import When
 
 from typeguard import typechecked
+from choc_expr import Expr as ChocExpr
 
 from ..utils import quote_expr
-from . import ChocExpr
 from ..operator import Operator
 
 
 @typechecked
 class Condition(ChocExpr):
     """ SQL condition """
     def __init__(
```

### Comparing `chocolatine-0.85/chocolatine/expr/delete_from.py` & `chocolatine-0.86/chocolatine/expr/select_from.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Iterable
 
 if TYPE_CHECKING:
     from .table import Table
+    from .col import Col
 
 from typeguard import typechecked
+from choc_expr import Expr as ChocExpr
 
 from .from_expr import FromExpr
-from .delete import Delete
-
-from .choc_expr import ChocExpr
+from .select import Select
 
 
 @typechecked
-class DeleteFrom(ChocExpr):
-    """ Delete expression """
+class SelectFrom(ChocExpr):
+    """ Select expression """
     def __init__(
             self,
             table: str | Table | None = None,
+            cols: Iterable[str | Col] | None = None,
+            unique: bool = False,
             compact: bool = True
     ) -> None:
-        self._delete = Delete(compact=compact)
+        self._select = Select(cols=cols, unique=unique, compact=compact)
         self._from_expr = FromExpr(table=table, compact=compact)
-        super().__init__("{delete~}{from_expr}", compact=compact)
+        super().__init__("{select~}{from_expr}", compact=compact)
 
     @property
-    def delete(self):
-        return self._delete
+    def select(self):
+        return self._select
 
     @property
     def from_expr(self):
         return self._from_expr
 
     @property
     def buildable(self) -> bool:
```

### Comparing `chocolatine-0.85/chocolatine/expr/from_expr.py` & `chocolatine-0.86/chocolatine/expr/update.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typeguard import typechecked
+from choc_expr import Expr as ChocExpr
 
-from .choc_expr import ChocExpr
 from .table import Table
 
 
 @typechecked
-class FromExpr(ChocExpr):
-    """ From expression """
+class Update(ChocExpr):
+    """ Update expression """
     def __init__(
             self,
             table: Table | str | None = None,
             compact: bool = True
     ) -> None:
         self.table = table
-        super().__init__("FROM {table}", compact=compact)
+        super().__init__("UPDATE {table}", compact=compact)
 
     @property
     def table(self):
         return self._table
 
     @table.setter
     def table(self, value):
```

### Comparing `chocolatine-0.85/chocolatine/expr/group_by.py` & `chocolatine-0.86/chocolatine/expr/limit.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,24 @@
-from typing import Iterable
 from typeguard import typechecked
-
-from .col import Col
-from .choc_expr import ChocExpr
+from choc_expr import Expr as ChocExpr
 
 
 @typechecked
-class GroupBy(ChocExpr):
-    """ GroupBy expression """
+class Limit(ChocExpr):
+    """ Limit expression """
     def __init__(
             self,
-            cols: Iterable[Col | str] | None = None,
+            length: int | None,
             compact: bool = True
     ) -> None:
-        self.cols = cols
-        super().__init__("GROUP BY {$(cols)}", compact=compact)
+        if length is not None and length < 1:
+            raise ValueError("Length cannot be lower than 1")
+        self._length = length
+        super().__init__("LIMIT {length}", compact=compact)
 
     @property
-    def cols(self):
-        return self._cols
-
-    @cols.setter
-    def cols(self, value: Iterable[Col | str] | None):
-        if value is not None and len(value) < 1:
-            raise ValueError("The number of cols must be at least 1")
-        self._cols = [Col(col) if type(col) is str else col for col in (value or [])]
+    def length(self) -> int:
+        return self._length
 
     @property
-    def buildable(self):
-        return self.cols is not None and len(self.cols) > 0
+    def buildable(self) -> bool:
+        return self._length is not None and self._length > 0
```

### Comparing `chocolatine-0.85/chocolatine/expr/having.py` & `chocolatine-0.86/chocolatine/expr/where.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typeguard import typechecked
+from choc_expr import Expr as ChocExpr
 
 from .condition import Condition
-from .choc_expr import ChocExpr
 
 
 @typechecked
-class Having(ChocExpr):
-    """ Having expression """
+class Where(ChocExpr):
+    """ Where expression """
     def __init__(
             self,
             condition: Condition | None = None,
             compact: bool = True
     ) -> None:
         self.condition = condition
-        super().__init__("HAVING {condition}", compact=compact)
+        super().__init__("WHERE {condition}", compact=compact)
 
     @property
     def condition(self) -> Condition | None:
         return self._condition
 
     @condition.setter
     def condition(self, value: Condition | None) -> None:
```

### Comparing `chocolatine-0.85/chocolatine/expr/join.py` & `chocolatine-0.86/chocolatine/expr/join.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Iterable
+
 from typeguard import typechecked
+from choc_expr import Expr as ChocExpr
 
 from ..join_type import JoinType
 from .table import Table
-from .choc_expr import ChocExpr
 from .condition import Condition
 
 
 @typechecked
 class Join(ChocExpr):
     """ Select expression """
     def __init__(
```

### Comparing `chocolatine-0.85/chocolatine/expr/order_by.py` & `chocolatine-0.86/chocolatine/expr/order_by.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Iterable
+
 from typeguard import typechecked
+from choc_expr import Expr as ChocExpr
 
 from .select import Select
 from .col import Col
-from .choc_expr import ChocExpr
 
 
 @typechecked
 class OrderBy(ChocExpr):
     """ OrderBy expression """
     def __init__(
             self,
```

### Comparing `chocolatine-0.85/chocolatine/expr/query.py` & `chocolatine-0.86/chocolatine/expr/query.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from typing import Iterable, Self, Tuple
 
 from typeguard import typechecked
+from choc_expr import Expr as ChocExpr
 
 from .delete_from import DeleteFrom
 from ..query_mode import QueryMode
 from .join import Join
 from .order_by import OrderBy
 from .group_by import GroupBy
 from .having import Having
 from .where import Where
 from .select_from import SelectFrom
 from .limit import Limit
 from ..agg_function import AggFunction
-from .choc_expr import ChocExpr
 from ..join_type import JoinType
 from .condition import Condition
 from .col import Col
 from .table import Table
 from .update_set import UpdateSet
+from .union import Union
 
 
 @typechecked
 class Query(ChocExpr):
     """ Handler to generate a SQL query """
     def __init__(
             self,
@@ -129,14 +130,25 @@
 
     def group_by(self, *cols_names: str) -> Self:
         """ Group the rows of the specified columns """
         self._group_by.cols = cols_names
         return self
 
     def join(self, table: str | Table, condition: Condition | str | Iterable[str], join_type: JoinType | None = JoinType.Inner) -> Self:
+        """ Join two tables together """
         self._joins.append(Join(table=table if isinstance(table, Table) else Table(name=table), condition=condition, join_type=join_type, compact=self._compact))
         return self
 
     def join_many(self, *joins_params: Tuple[str | Table, Condition | str | Iterable[str]] | Tuple[str | Table, Condition | str | Iterable[str], JoinType | None]) -> Self:
+        """ Join more than two tables together """
         for join_params in joins_params:
             self.join(*join_params)
         return self
+
+    def union(self, other_request: Self) -> Union:
+        return Union(self, other_request, compact=self._compact)
+
+    def __and__(self, other_request: Self) -> Union:
+        return self.union(other_request)
+
+    def __rand__(self, other_request: Self) -> Union:
+        return self.__and__(other_request)
```

### Comparing `chocolatine-0.85/chocolatine/expr/select.py` & `chocolatine-0.86/chocolatine/expr/select.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Iterable
+
 from typeguard import typechecked
+from choc_expr import Expr as ChocExpr
 
 from .col import Col
-from .choc_expr import ChocExpr
 
 
 @typechecked
 class Select(ChocExpr):
     """ Select expression """
     def __init__(
             self,
```

### Comparing `chocolatine-0.85/chocolatine/expr/select_from.py` & `chocolatine-0.86/chocolatine/expr/delete_from.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING, Iterable
+from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from .table import Table
-    from .col import Col
 
 from typeguard import typechecked
+from choc_expr import Expr as ChocExpr
 
 from .from_expr import FromExpr
-from .select import Select
-
-from .choc_expr import ChocExpr
+from .delete import Delete
 
 
 @typechecked
-class SelectFrom(ChocExpr):
-    """ Select expression """
+class DeleteFrom(ChocExpr):
+    """ Delete expression """
     def __init__(
             self,
             table: str | Table | None = None,
-            cols: Iterable[str | Col] | None = None,
-            unique: bool = False,
             compact: bool = True
     ) -> None:
-        self._select = Select(cols=cols, unique=unique, compact=compact)
+        self._delete = Delete(compact=compact)
         self._from_expr = FromExpr(table=table, compact=compact)
-        super().__init__("{select~}{from_expr}", compact=compact)
+        super().__init__("{delete~}{from_expr}", compact=compact)
 
     @property
-    def select(self):
-        return self._select
+    def delete(self):
+        return self._delete
 
     @property
     def from_expr(self):
         return self._from_expr
 
     @property
     def buildable(self) -> bool:
```

### Comparing `chocolatine-0.85/chocolatine/expr/set.py` & `chocolatine-0.86/chocolatine/expr/update_set.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from typing import Iterable
+from __future__ import annotations
+from typing import TYPE_CHECKING, Iterable
+
+if TYPE_CHECKING:
+    from .table import Table
+    from .condition import Condition
+
 from typeguard import typechecked
+from choc_expr import Expr as ChocExpr
 
-from .col import Col
-from .choc_expr import ChocExpr
-from .condition import Condition
+from .update import Update
+from .set import Set
 
 
 @typechecked
-class Set(ChocExpr):
-    """ Set expression """
+class UpdateSet(ChocExpr):
+    """ UpdateSet expression """
     def __init__(
             self,
+            table: str | Table | None = None,
             assignations: Iterable[Condition] | None = None,
             compact: bool = True
     ) -> None:
-        self.assignations = assignations or []
-        super().__init__("SET {$(assignations)}", compact=compact)
-
-    @property
-    def assignations(self):
-        return self._cols
-
-    @assignations.setter
-    def assignations(self, value):
-        self._cols = [Col(col) if type(col) is str else col for col in (value or [])]
+        self._update = Update(table=table, compact=compact)
+        self._set = Set(assignations=assignations, compact=compact)
+        super().__init__("{_update~}{_set}", compact=compact)
 
     @property
-    def buildable(self):
-        return len(self.assignations) > 0
+    def buildable(self) -> bool:
+        return self._update.buildable and self._set.buildable
```

### Comparing `chocolatine-0.85/chocolatine/expr/table.py` & `chocolatine-0.86/chocolatine/expr/table.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
-
 from typing import Self
-from typeguard import typechecked
 
-from .choc_expr import ChocExpr
+from typeguard import typechecked
+from choc_expr import Expr as ChocExpr
 
 
 @typechecked
 class Table(ChocExpr):
     """ Represent a SQL table name """
 
     def __init__(
```

### Comparing `chocolatine-0.85/chocolatine/expr/update.py` & `chocolatine-0.86/chocolatine/expr/from_expr.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typeguard import typechecked
+from choc_expr import Expr as ChocExpr
 
-from .choc_expr import ChocExpr
 from .table import Table
 
 
 @typechecked
-class Update(ChocExpr):
-    """ Update expression """
+class FromExpr(ChocExpr):
+    """ From expression """
     def __init__(
             self,
             table: Table | str | None = None,
             compact: bool = True
     ) -> None:
         self.table = table
-        super().__init__("UPDATE {table}", compact=compact)
+        super().__init__("FROM {table}", compact=compact)
 
     @property
     def table(self):
         return self._table
 
     @table.setter
     def table(self, value):
```

### Comparing `chocolatine-0.85/chocolatine/expr/when.py` & `chocolatine-0.86/chocolatine/expr/when.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable
 
 from typeguard import typechecked
+from choc_expr import Expr as ChocExpr
 
-from .choc_expr import ChocExpr
 from .condition import Condition
 from ..utils import quote_expr
 
 
 @typechecked
 class When(ChocExpr):
     """ Conditional 'Case When' expression """
```

### Comparing `chocolatine-0.85/chocolatine/expr/where.py` & `chocolatine-0.86/chocolatine/expr/having.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typeguard import typechecked
+from choc_expr import Expr as ChocExpr
 
 from .condition import Condition
-from .choc_expr import ChocExpr
 
 
 @typechecked
-class Where(ChocExpr):
-    """ Where expression """
+class Having(ChocExpr):
+    """ Having expression """
     def __init__(
             self,
             condition: Condition | None = None,
             compact: bool = True
     ) -> None:
         self.condition = condition
-        super().__init__("WHERE {condition}", compact=compact)
+        super().__init__("HAVING {condition}", compact=compact)
 
     @property
     def condition(self) -> Condition | None:
         return self._condition
 
     @condition.setter
     def condition(self, value: Condition | None) -> None:
```

### Comparing `chocolatine-0.85/chocolatine/shortcut.py` & `chocolatine-0.86/chocolatine/shortcut.py`

 * *Files identical despite different names*

### Comparing `chocolatine-0.85/chocolatine/sql_function.py` & `chocolatine-0.86/chocolatine/sql_function.py`

 * *Files identical despite different names*

### Comparing `chocolatine-0.85/chocolatine.egg-info/PKG-INFO` & `chocolatine-0.86/chocolatine.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 Metadata-Version: 2.1
 Name: chocolatine
-Version: 0.85
+Version: 0.86
 Summary: A lightweight Python library to easily generate SQL queries
 Home-page: https://github.com/pe-brian/chocolatine
 Author: Pierre-Emmanuel Brian
 Author-email: pebrian@outlook.fr
 Project-URL: Bug Tracker, https://github.com/pe-brian/chocolatine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typeguard==4.1.5
+Requires-Dist: choc-expr==1.0
+
+[![PyPI version](https://badge.fury.io/py/chocolatine.svg)](https://badge.fury.io/py/chocolatine) ![Licence badge](https://img.shields.io/pypi/l/chocolatine) ![Python version](https://img.shields.io/pypi/pyversions/chocolatine)
+[![Actions Status](https://github.com/pe-brian/chocolatine/workflows/validate-dev-push/badge.svg)](https://github.com/pe-brian/chocolatine/actions)
+![Dependencies](https://img.shields.io/badge/dependencies-typeguard-yellowgreen)
+![Dependencies](https://img.shields.io/badge/dependencies-choc_expr-yellowgreen)
+![Downloads per month](https://img.shields.io/pypi/dm/chocolatine)
+![Last commit](https://img.shields.io/github/last-commit/pe-brian/chocolatine)
 
 # chocolatine
 
 ![Image](logo.jpg)
 
 Chocolatine is a lightweight python library designed to easily generate SQL queries.
 
 # Why Chocolatine ?
 
-If you know Python programming langage but you are not at your ease with SQL (or you don't want to manage SQL requests by yourself), you can use Chocolatine to generate some SQL queries for you.
+If you know Python programming langage but you are not at your ease with SQL (or you don't want to manage SQL queries by yourself), you can use Chocolatine to generate some SQL queries for you.
 Of course, there are many other open source projects to do that, but honestly, they are more complex than most people expects from them (SQLAlchemy, Django ORM, etc...).
 
+# Installation
+
+```pip install chocolatine```
+
 # Examples
 
 __Concatenation & filtering__ :
 ```python
 from chocolatine import Query, Col as _
 
 query = Query().table("customer")\
@@ -101,52 +113,48 @@
 # SQL dialect
 
 For now, Chocolatine is only designed to generate MySQL queries.
 It is not excluded that in the future it will be compatible with Sqlite3, SqlServer or postgreSQL
 
 # Basic functionnalities
 
-- Select requests
+- Select, Update & delete queries
 - Distinct
-- Aliases (for columns & tables)
-- Ordering
-- Group by
-- Aggregation functions
+- Names aliases
+- Columns ordering
+- Group by & aggregations
 - Joins
 - SQL functions
 - Concatenations
+- Unions
+- Case-When
 
 # Advanced functionnalities
 
 - Dynamic type checking
 - Use of : or @ in col or table name directly for alias
 - Protection against SQL injection attacks
 - Calls orders doesn't matter (except for join clauses)
 - Compact or extended SQL expressions
 - Whole system to deal with conditions (logical operators, boolean operators, priority order)
 - Automatic handling of filter conditions to fill the having or where clause depending on the given columns
 - Shortcut functions : Asc, Desc, Sum, Count, Upper, Lower, Concat, Second, Minute, Hour, Day, Month, Year
 - \>: or <: at first position in column name (or alias) in select to set the ordering
 - \>\> operator to perform a "like" condition on a column
 - << operator to perform a "in" condition on a column
-- Limit clause
-- Nested requests
-- "ChocExpr" mini langage for SQL requests templating :
+- Nested queries
+- "ChocExpr" mini langage for SQL queries templating :
     - Conditions
     - Basic loops (with unpacking lists)
-- Case When
-- Update requests
-- Delete requests
 
 # To-do
 
-- Tables union
+- Equality evaluation in ChocExpr if statements
 - Option to disable dynamic type checking (for performance concerns)
-- Create requests
-- Pypi package (to install with pip install)
+- Create queries
 - SQLServer compatibility
 - PostGreSQL compatibility
 - SQLite3 compatibility
 
 # Tests
 
 ```python pytest```
```

### Comparing `chocolatine-0.85/chocolatine.egg-info/SOURCES.txt` & `chocolatine-0.86/chocolatine.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,37 +8,37 @@
 chocolatine/operator.py
 chocolatine/ordering.py
 chocolatine/query_mode.py
 chocolatine/shortcut.py
 chocolatine/sql_function.py
 chocolatine/type.py
 chocolatine/utils.py
+chocolatine/view_mode.py
 chocolatine.egg-info/PKG-INFO
 chocolatine.egg-info/SOURCES.txt
 chocolatine.egg-info/dependency_links.txt
 chocolatine.egg-info/requires.txt
 chocolatine.egg-info/top_level.txt
 chocolatine/expr/__init__.py
-chocolatine/expr/choc_expr.py
-chocolatine/expr/choc_expr_attr.py
 chocolatine/expr/col.py
 chocolatine/expr/col_when.py
 chocolatine/expr/condition.py
 chocolatine/expr/delete.py
 chocolatine/expr/delete_from.py
-chocolatine/expr/expr.py
 chocolatine/expr/from_expr.py
 chocolatine/expr/group_by.py
 chocolatine/expr/having.py
 chocolatine/expr/join.py
 chocolatine/expr/limit.py
 chocolatine/expr/order_by.py
 chocolatine/expr/query.py
 chocolatine/expr/select.py
 chocolatine/expr/select_from.py
 chocolatine/expr/set.py
 chocolatine/expr/table.py
+chocolatine/expr/union.py
 chocolatine/expr/update.py
 chocolatine/expr/update_set.py
+chocolatine/expr/view.py
 chocolatine/expr/when.py
 chocolatine/expr/where.py
 tests/test_sakila_challenge.py
```

### Comparing `chocolatine-0.85/setup.cfg` & `chocolatine-0.86/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chocolatine
-version = 0.85
+version = 0.86
 author = Pierre-Emmanuel Brian
 author_email = pebrian@outlook.fr
 description = A lightweight Python library to easily generate SQL queries
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pe-brian/chocolatine
 project_urls = 
@@ -14,12 +14,13 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 python_requires = >=3.12.2
 install_requires = 
 	typeguard == 4.1.5
+	choc-expr == 1.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `chocolatine-0.85/tests/test_sakila_challenge.py` & `chocolatine-0.86/tests/test_sakila_challenge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from chocolatine import Query, Col as _, month, year, sum, count, QueryMode, When
+from chocolatine import Query, Col as _, month, year, sum, count, QueryMode, When, View, ViewMode
 
 
 def test_query_1a():
     """ How to display the first and last names of all actors from the table `actor` ? """
     assert str(Query(
         compact=False,
         table="actor",
@@ -418,33 +418,58 @@
 INNER JOIN category
 USING category_id
 GROUP BY name
 ORDER BY total_amount DESC
 """
 
 
-# 8a. In your new role as an executive, you would like to have an easy way of viewing the Top five genres by gross revenue. Use the
-# solution from the problem above to create a view. If you havent solved 7h, you can substitute another query to create a view.
-
-#   CREATE VIEW top_five_genres AS
-#   SELECT SUM(amount) AS "Total Sales", c.name AS "Genre"
-#   FROM payment p
-#   JOIN rental r
-#   ON (p.rental_id = r.rental_id)
-#   JOIN inventory i
-#   ON (r.inventory_id = i.inventory_id)
-#   JOIN film_category fc
-#   ON (i.film_id = fc.film_id)
-#   JOIN category c
-#   ON (fc.category_id = c.category_id)
-#   GROUP BY c.name
-#   ORDER BY SUM(amount) DESC
-#   LIMIT 5;
+def test_query_8a():
+    """ In your new role as an executive, you would like to have an easy way of viewing the Top five genres by gross revenue. Use the
+        solution from the problem above to create a view. If you havent solved 7h, you can substitute another query to create a view. """
+    assert str(View(
+        name="top_five_genres",
+        compact=False,
+        query=Query(
+            compact=False,
+            table="payment",
+            cols=(sum("amount").alias("<:total_sales"), "name:genre"),
+            joins=(("rental", "rental_id"), ("inventory", "inventory_id"), ("film_category", "film_id"), ("category", "category_id")),
+            groups=("name",),
+            limit=5
+        ))) == """\
+CREATE VIEW top_five_genres AS
+SELECT SUM(amount) AS total_sales, name AS genre
+FROM payment
+INNER JOIN rental
+USING rental_id
+INNER JOIN inventory
+USING inventory_id
+INNER JOIN film_category
+USING film_id
+INNER JOIN category
+USING category_id
+GROUP BY name
+ORDER BY total_sales DESC
+LIMIT 5
+"""
 
-# 8b. How would you display the view that you created in 8a?
 
-#   SELECT *
-#   FROM top_five_genres;
+def test_query_8b():
+    """ How would you display the view that you created in 8a? """
+    assert str(Query(
+        compact=False,
+        table="top_five_genres"
+    )) == """\
+SELECT *
+FROM top_five_genres
+"""
 
-# 8c. You find that you no longer need the view `top_five_genres`. Write a query to delete it.
 
-#   DROP VIEW top_five_genres;
+def test_query_8c():
+    """ How would you display the view that you created in 8a? """
+    assert str(View(
+        name="top_five_genres",
+        mode=ViewMode.Drop,
+        compact=False,
+    )) == """\
+DROP VIEW top_five_genres
+"""
```


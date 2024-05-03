# Comparing `tmp/sru_queryer-1.0.3.tar.gz` & `tmp/sru_queryer-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sru_queryer-1.0.3.tar", last modified: Fri Apr 26 16:40:53 2024, max compression
+gzip compressed data, was "sru_queryer-2.0.0.tar", last modified: Fri May  3 13:53:10 2024, max compression
```

## Comparing `sru_queryer-1.0.3.tar` & `sru_queryer-2.0.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-04-26 16:40:53.463308 sru_queryer-1.0.3/
--rw-r--r--   0 ejones99   (505) staff       (20)    11354 2024-04-17 20:20:30.000000 sru_queryer-1.0.3/LICENSE
--rw-r--r--   0 ejones99   (505) staff       (20)    39386 2024-04-26 16:40:53.463013 sru_queryer-1.0.3/PKG-INFO
--rw-r--r--   0 ejones99   (505) staff       (20)      512 2024-04-26 16:35:01.000000 sru_queryer-1.0.3/pyproject.toml
--rw-r--r--   0 ejones99   (505) staff       (20)    38890 2024-04-17 17:20:50.000000 sru_queryer-1.0.3/readme.md
--rw-r--r--   0 ejones99   (505) staff       (20)       38 2024-04-26 16:40:53.463366 sru_queryer-1.0.3/setup.cfg
-drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-04-26 16:40:53.452228 sru_queryer-1.0.3/src/
-drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-04-26 16:40:53.454314 sru_queryer-1.0.3/src/sru_queryer/
--rw-r--r--   0 ejones99   (505) staff       (20)      165 2024-04-17 17:18:26.000000 sru_queryer-1.0.3/src/sru_queryer/__init__.py
-drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-04-26 16:40:53.458911 sru_queryer-1.0.3/src/sru_queryer/_base/
--rw-r--r--   0 ejones99   (505) staff       (20)        0 2024-04-17 17:18:54.000000 sru_queryer-1.0.3/src/sru_queryer/_base/__init__.py
--rw-r--r--   0 ejones99   (505) staff       (20)     5619 2024-04-22 13:47:27.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_cql_boolean_operators.py
--rw-r--r--   0 ejones99   (505) staff       (20)      463 2024-04-22 13:47:27.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_cql_literal.py
--rw-r--r--   0 ejones99   (505) staff       (20)     4653 2024-04-22 13:47:27.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_cql_modifiers.py
--rw-r--r--   0 ejones99   (505) staff       (20)     3107 2024-04-17 17:18:54.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_drivers.py
--rw-r--r--   0 ejones99   (505) staff       (20)     3657 2024-04-22 13:47:27.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_query.py
--rw-r--r--   0 ejones99   (505) staff       (20)     3464 2024-04-22 13:47:27.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_search_index_config.py
--rw-r--r--   0 ejones99   (505) staff       (20)     2961 2024-04-22 13:47:27.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_sort_key.py
--rw-r--r--   0 ejones99   (505) staff       (20)     5125 2024-04-22 13:47:27.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_sru_aux_formatter.py
--rw-r--r--   0 ejones99   (505) staff       (20)     1205 2024-04-22 13:47:27.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_sru_configuration.py
--rw-r--r--   0 ejones99   (505) staff       (20)    13516 2024-04-22 13:47:27.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_sru_explain_xml_parser.py
--rw-r--r--   0 ejones99   (505) staff       (20)     6060 2024-04-22 13:47:27.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_sru_util.py
--rw-r--r--   0 ejones99   (505) staff       (20)    11334 2024-04-26 16:17:40.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_sru_validator.py
--rw-r--r--   0 ejones99   (505) staff       (20)      441 2024-04-17 17:18:26.000000 sru_queryer-1.0.3/src/sru_queryer/cql.py
--rw-r--r--   0 ejones99   (505) staff       (20)       67 2024-04-17 17:18:26.000000 sru_queryer-1.0.3/src/sru_queryer/drivers.py
--rw-r--r--   0 ejones99   (505) staff       (20)      223 2024-04-17 17:18:37.000000 sru_queryer-1.0.3/src/sru_queryer/sru.py
-drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-04-26 16:40:53.462516 sru_queryer-1.0.3/src/sru_queryer.egg-info/
--rw-r--r--   0 ejones99   (505) staff       (20)    39386 2024-04-26 16:40:53.000000 sru_queryer-1.0.3/src/sru_queryer.egg-info/PKG-INFO
--rw-r--r--   0 ejones99   (505) staff       (20)     1137 2024-04-26 16:40:53.000000 sru_queryer-1.0.3/src/sru_queryer.egg-info/SOURCES.txt
--rw-r--r--   0 ejones99   (505) staff       (20)        1 2024-04-26 16:40:53.000000 sru_queryer-1.0.3/src/sru_queryer.egg-info/dependency_links.txt
--rw-r--r--   0 ejones99   (505) staff       (20)       35 2024-04-26 16:40:53.000000 sru_queryer-1.0.3/src/sru_queryer.egg-info/requires.txt
--rw-r--r--   0 ejones99   (505) staff       (20)       12 2024-04-26 16:40:53.000000 sru_queryer-1.0.3/src/sru_queryer.egg-info/top_level.txt
-drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-04-26 16:40:53.462129 sru_queryer-1.0.3/tests/
--rw-r--r--   0 ejones99   (505) staff       (20)    10836 2024-04-17 17:20:07.000000 sru_queryer-1.0.3/tests/test_cql_boolean_operators.py
--rw-r--r--   0 ejones99   (505) staff       (20)     1130 2024-04-17 17:20:07.000000 sru_queryer-1.0.3/tests/test_cql_literal.py
--rw-r--r--   0 ejones99   (505) staff       (20)     5583 2024-04-17 17:20:07.000000 sru_queryer-1.0.3/tests/test_cql_modifiers.py
--rw-r--r--   0 ejones99   (505) staff       (20)     4457 2024-04-17 17:20:07.000000 sru_queryer-1.0.3/tests/test_search_index_config.py
--rw-r--r--   0 ejones99   (505) staff       (20)     3439 2024-04-17 17:20:07.000000 sru_queryer-1.0.3/tests/test_sort_key.py
--rw-r--r--   0 ejones99   (505) staff       (20)     8162 2024-04-17 17:20:07.000000 sru_queryer-1.0.3/tests/test_sru_aux_formatter.py
--rw-r--r--   0 ejones99   (505) staff       (20)    20854 2024-04-17 17:20:07.000000 sru_queryer-1.0.3/tests/test_sru_explain_xml_parser.py
--rw-r--r--   0 ejones99   (505) staff       (20)     9898 2024-04-17 17:20:07.000000 sru_queryer-1.0.3/tests/test_sru_query.py
--rw-r--r--   0 ejones99   (505) staff       (20)     7909 2024-04-17 17:20:07.000000 sru_queryer-1.0.3/tests/test_sru_util.py
--rw-r--r--   0 ejones99   (505) staff       (20)    10488 2024-04-17 17:20:07.000000 sru_queryer-1.0.3/tests/test_sru_validator.py
+drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-05-03 13:53:10.428948 sru_queryer-2.0.0/
+-rw-r--r--   0 ejones99   (505) staff       (20)    11354 2024-04-17 20:20:30.000000 sru_queryer-2.0.0/LICENSE
+-rw-r--r--   0 ejones99   (505) staff       (20)    43463 2024-05-03 13:53:10.428667 sru_queryer-2.0.0/PKG-INFO
+-rw-r--r--   0 ejones99   (505) staff       (20)      512 2024-05-03 13:26:19.000000 sru_queryer-2.0.0/pyproject.toml
+-rw-r--r--   0 ejones99   (505) staff       (20)    42967 2024-05-03 13:30:15.000000 sru_queryer-2.0.0/readme.md
+-rw-r--r--   0 ejones99   (505) staff       (20)       38 2024-05-03 13:53:10.429012 sru_queryer-2.0.0/setup.cfg
+drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-05-03 13:53:10.418255 sru_queryer-2.0.0/src/
+drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-05-03 13:53:10.420340 sru_queryer-2.0.0/src/sru_queryer/
+-rw-r--r--   0 ejones99   (505) staff       (20)      131 2024-05-01 20:21:50.000000 sru_queryer-2.0.0/src/sru_queryer/__init__.py
+drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-05-03 13:53:10.425018 sru_queryer-2.0.0/src/sru_queryer/_base/
+-rw-r--r--   0 ejones99   (505) staff       (20)        0 2024-04-17 17:18:54.000000 sru_queryer-2.0.0/src/sru_queryer/_base/__init__.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     5630 2024-04-29 14:29:44.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_cql_boolean_operators.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     4982 2024-05-02 17:42:23.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_cql_modifiers.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     1210 2024-05-01 15:58:54.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_exceptions.py
+-rw-r--r--   0 ejones99   (505) staff       (20)      462 2024-04-29 14:29:44.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_raw_cql.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     3306 2024-05-02 17:17:10.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_search_clause.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     3808 2024-05-02 16:27:34.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_search_retrieve.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     2961 2024-04-22 13:47:27.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_sort_key.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     4368 2024-05-01 21:01:01.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_sru_aux_formatter.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     1159 2024-04-29 14:29:44.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_sru_configuration.py
+-rw-r--r--   0 ejones99   (505) staff       (20)    12230 2024-05-02 16:27:34.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_sru_explain_auto_parser.py
+-rw-r--r--   0 ejones99   (505) staff       (20)    11729 2024-05-03 12:56:00.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_sru_queryer.py
+-rw-r--r--   0 ejones99   (505) staff       (20)    10887 2024-05-02 19:42:22.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_sru_validator.py
+-rw-r--r--   0 ejones99   (505) staff       (20)      433 2024-04-29 14:29:44.000000 sru_queryer-2.0.0/src/sru_queryer/cql.py
+-rw-r--r--   0 ejones99   (505) staff       (20)      241 2024-05-01 16:02:27.000000 sru_queryer-2.0.0/src/sru_queryer/exceptions.py
+-rw-r--r--   0 ejones99   (505) staff       (20)      191 2024-05-01 20:21:50.000000 sru_queryer-2.0.0/src/sru_queryer/sru.py
+drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-05-03 13:53:10.428322 sru_queryer-2.0.0/src/sru_queryer.egg-info/
+-rw-r--r--   0 ejones99   (505) staff       (20)    43463 2024-05-03 13:53:10.000000 sru_queryer-2.0.0/src/sru_queryer.egg-info/PKG-INFO
+-rw-r--r--   0 ejones99   (505) staff       (20)     1147 2024-05-03 13:53:10.000000 sru_queryer-2.0.0/src/sru_queryer.egg-info/SOURCES.txt
+-rw-r--r--   0 ejones99   (505) staff       (20)        1 2024-05-03 13:53:10.000000 sru_queryer-2.0.0/src/sru_queryer.egg-info/dependency_links.txt
+-rw-r--r--   0 ejones99   (505) staff       (20)       35 2024-05-03 13:53:10.000000 sru_queryer-2.0.0/src/sru_queryer.egg-info/requires.txt
+-rw-r--r--   0 ejones99   (505) staff       (20)       12 2024-05-03 13:53:10.000000 sru_queryer-2.0.0/src/sru_queryer.egg-info/top_level.txt
+drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-05-03 13:53:10.427891 sru_queryer-2.0.0/tests/
+-rw-r--r--   0 ejones99   (505) staff       (20)    10310 2024-05-02 17:42:23.000000 sru_queryer-2.0.0/tests/test_cql_boolean_operators.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     5670 2024-05-02 17:42:23.000000 sru_queryer-2.0.0/tests/test_cql_modifiers.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     1087 2024-04-29 14:29:44.000000 sru_queryer-2.0.0/tests/test_raw_cql.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     4852 2024-05-02 17:42:23.000000 sru_queryer-2.0.0/tests/test_search_clause.py
+-rw-r--r--   0 ejones99   (505) staff       (20)    10206 2024-05-02 17:17:10.000000 sru_queryer-2.0.0/tests/test_search_retrieve.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     3439 2024-04-17 17:20:07.000000 sru_queryer-2.0.0/tests/test_sort_key.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     8096 2024-05-02 15:32:04.000000 sru_queryer-2.0.0/tests/test_sru_aux_formatter.py
+-rw-r--r--   0 ejones99   (505) staff       (20)    13475 2024-05-02 16:27:34.000000 sru_queryer-2.0.0/tests/test_sru_explain_auto_parser.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     9367 2024-05-02 18:07:43.000000 sru_queryer-2.0.0/tests/test_sru_queryer.py
+-rw-r--r--   0 ejones99   (505) staff       (20)    11356 2024-05-02 19:38:45.000000 sru_queryer-2.0.0/tests/test_sru_validator.py
```

### Comparing `sru_queryer-1.0.3/LICENSE` & `sru_queryer-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.3/PKG-INFO` & `sru_queryer-2.0.0/readme.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,503 +1,558 @@
-Metadata-Version: 2.1
-Name: sru-queryer
-Version: 1.0.3
-Summary: A utility for integrating SRU queries into your applications.
-Author-email: Erik Jones <ejones99@umd.edu>
-Maintainer-email: USMAI <libclas@umd.edu>
-Keywords: sru,library,api
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7.17
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.27.1
-Requires-Dist: xmltodict>=0.13.0
-
 # USMAI SRU Queryer
 
 Welcome to SRU Queryer, a library for working with Search/Retrieval via URL (SRU) created by the USMAI Library Consortium. This package is designed to make working with SRU simple and accurate!
 
 Using this utility has a few big benefits, such as:
 
 1. It handles validating much of the searchRetrieve request. This is particularly helpful because many SRU servers don't have good error messages.
 2. It handles formatting the searchRetrieve request for you. This makes queries much less prone to human mistakes.
-3. It provides functions to see which indexes are available to search in the SRU server.
+3. Programmatically access the capabilities of the SRU server in your program.
 
 ## TABLE OF CONTENTS
 
 1. [Setting Up The Environment](#setting-up-the-environment)
 2. [Basic Usage](#basic-usage)
 3. [Quick Overview of Important Components](#quick-overview-of-important-components)
    1. [Initializing SRU Functionality](#initializing-sru-functionality)
-   2. [Basic Query Component](#basic-query-component-indexquery)
-   3. [Configuration Service](#configuration-service-sruutil)
-   4. [Query class](#creating-queries---the-query-class)
-   5. [Boolean Operators for Queries](#constructing-more-advanced-queries-boolean-operators)
+   2. [Basic Query Component](#basic-query-component-searchclause)
+   3. [Searching using SRUQueryer](#searching-using-sruqueryer)
+   4. [Boolean Operators for Queries](#constructing-more-advanced-queries-boolean-operators)
 4. [Full Overview of Different Components](#full-overview-of-different-components)
-   1. [IndexQuery](#basic-query-component-indexquery-1)
-   2. [SRUUtil](#sruutil)
-   3. [Boolean Operators (AND, OR, NOT, PROX)](#constructing-more-advanced-queries-boolean-operators-1)
-   4. [Query](#query-class)
-   5. [LITERAL](#custom-queries-literal)
-   6. [Modifiers](#modifiying-operators---modifiers)
-   7. [Sorting in v1.2](#sorting-in-12-sortby-clauses)
-   8. [Sorting in v1.1](#sorting-in-11-SortKey)
+   1. [SearchClause](#basic-query-component-searchclause-1)
+   2. [SRUQueryer](#sruqueryer)
+   3. [Boolean Operators (AND, OR, NOT, PROX)](#boolean-operators)
+   4. [RawCQL](#custom-queries-rawcql)
+   5. [Modifiers](#modifiying-operators---modifiers)
+   6. [Sorting in v1.2](#sorting-in-12-sortby-clauses)
+   7. [Sorting in v1.1](#sorting-in-11-SortKey)
+5. [Known Incompatibilities](#known-incompatibilities)
 
 ## Setting Up The Environment
 
-This python script was developed using python 3.10 and tested on python 3.11.1.
-
 To install sru-queryer, just run `pip install sru-queryer`
 
+Note that you may have to specify pip3 if you have python2 installed. The install will fail if you try to use python2's PIP.
+
 ## Basic Usage
 
 Here's just a basic usage example:
 
 ```
 # Create a configuration object for the SRU server, allowing you to validate and send queries.
-sru_configuration = SRUUtil.create_configuration_for_server("https://path-to-sru-server-base", "https://path-to-sru-server-base", "1.2")
-
-# Configure a query - in this case, find records where the creator includes Abraham, sorted alphabetically & ascending.
-query_obj = Query(sru_configuration, IndexQuery(
-        "alma", "creator", "=", "Abraham"), sort_queries=[{
-            "index_set": "alma",
-            "index_name": "creator",
-            "sort_order": "ascending"
-        }])
+queryer = SRUQueryer("https://path-to-sru-server-base")
 
-# Validate the query to see whether it's valid
-query_obj.validate()
-
-# Construct the request (just a python PreparedRequest object)
-request = query_obj.construct_request()
-
-s = Session()
-response = s.send(request)
+# Configure a SearchRetrieve query - in this case, find records where the creator includes Abraham, sorted alphabetically & ascending.
+response_content = queryer.search_retrieve(SearchClause("alma", "creator", "=", "Abraham"),
+                     sort_queries=[{
+                           "index_set": "alma",
+                           "index_name": "creator",
+                           "sort_order": "ascending"
+                     }])
 ```
 
 This code will send the following query:
 https://path-to-sru-server-base/?version=1.2&operation=searchRetrieve&recordSchema=marcxml&maximumRecords=10&query=alma.creator=%22Abraham%22%20sortBy%20alma.creator/sort.ascending
 
 You can also create a query with boolean conditions:
 
 ```
 # Find records where the creator includes Abraham AND the material type is 'book'
-query_obj = Query(sru_configuration, AND(IndexQuery("alma", "creator", "=", "Abraham"), IndexQuery("alma", "materialType", "==", "BOOK")))
+queryer.search_retrieve(sru_configuration, AND(SearchClause("alma", "creator", "=", "Abraham"), SearchClause("alma", "materialType", "==", "BOOK")))
 ```
 
 ## Quick Overview of Important Components:
 
 ### Initializing SRU functionality
 
-Before you can validate or send searchRetrieve requests, you must create an SRU configuration for your server. The configuration of this server will be in the form of an SRUConfiguration class.
-
-An instance is created through the SRUUtil.create_configuration_for_server() function, and all you have to do is to pass the created instance to the functions that need it. You can read information from it if you want to integrate SRU querying more deeply into your application.
+Before you can validate or send searchRetrieve requests, you must create a queryer. Upon initialization, the queryer will contact your SRU server and set up everything it needs to validate and format your SRU queries.
 
 ```
-from sru_queryer.drivers import alma_driver
-sru_configuration = SRUUtil.create_configuration_for_server("https://path-to-sru-server-base", "https://path-to-sru-server-base", "1.2", driver=alma_driver)
+queryer = SRUQueryer("https://path-to-sru-server-base")
 ```
 
-This is the most basic way to create a configuration object. The first argument is the SRU explain URL, the second is the searchRetrieve URL, the third is the SRU version, and the final one is the driver. This function takes many other optional arguments, which can do things like configure the default record schemas, default context sets, change validation settings, etc.
+This is the most basic way to create a queryer. This function takes many other optional arguments, which can do things like configure the default record schemas, default context sets, change validation settings, etc.
 
-A very important argument is 'driver'. This takes a dict which tells the program how to parse explainResponses. This program already includes drivers for ExLibris Alma, LOC, and gapines SRU servers. The default is set to 'alma' (ExLibris Alma), which is why you won't see it in some examples. The drivers are straightforward - you can follow the template of the included drivers to create one for your own server. Drivers serve to tell the program where to find the information it needs in the SRU explainResponse and which information is available.
+### Basic Query Component: SearchClause
 
-### Basic Query Component: IndexQuery
+`from sru_queryer.cql import SearchClause`
 
-`from sru_queryer import IndexQuery`
+This is officially known as a 'CQL search clause': https://www.loc.gov/standards/sru/cql/spec.html <br>
+A standard CQL search clause looks like: `alma.title="Harry Potter"`. This same query with the SearchClause class would look like: `SearchClause("alma", "title", "=", "Harry Potter")`. Pretty straightforward! See more in the extended SearchClause section below - there's rules for which of these arguments are required.
 
-This would more officially be known as a 'CQL search clause': https://www.loc.gov/standards/sru/cql/spec.html.\
-A standard CQL search clause looks like: `alma.title="Harry Potter"`. This same query with the IndexQuery class would look like: `IndexQuery("alma", "title", "=", "Harry Potter")`
+### Searching using SRUQueryer
 
-https://www.loc.gov/standards/sru/cql/spec.html
+`from sru_queryer import SRUQueryer`
 
-### Creating queries - the Query class
+There's two options for conducting searchRetrieve requests with the SRUQueryer class. <br>
 
-`from sru_queryer import Query`
+First, you can have the queryer send the request for you and return the content. Once the querier is initialized, you can do so in this way (this is only an example search, it doesn't have to look exactly like this):
 
-Use the Query class to actually construct and validate a query.\
-This class takes the SRU configuration as an argument, followed by the actual CQL query made up of boolean operators, Literals, and IndexQueries. You can also set certain values that you might want to change between queries while keeping the same SRUConfiguration - record format, start record, maximum records, etc. It also takes sort queries.
+```
+response_content = queryer.search_retrieve(SearchClause("alma", "creator", "=", "Abraham"),
+         sort_queries=[{
+            "index_set": "alma",
+            "index_name": "creator",
+            "sort_order": "ascending"
+        }])
+```
+
+Alternately, you can construct a requests.Request object that you can then send yourself. This allows for a bit more flexibility, like adding a custom authentication header:
 
 ```
-query_obj = Query(sru_configuration, IndexQuery(
+request = queryer.construct_search_retrieve_request(SearchClause(
         "alma", "creator", "=", "Abraham"), sort_queries=[{
             "index_set": "alma",
             "index_name": "creator",
             "sort_order": "ascending"
         }])
 ```
 
+Both of these options take the same arguments. The first is the CQL query made up of boolean operators, RawCQL classes, and/or SearchClauses. You can also set certain values that you might want to change between queries while keeping the same queryer - record format, start record, maximum records, etc. It also takes sort queries.
+
 ### Constructing more advanced queries: Boolean Operators
 
 `from sru_queryer.cql import AND, OR, NOT, PROX`
 
-Boolean Operators are used to construct queries with one or more IndexQueries. Their usage is extrememly simply by design, and should be familiar to people working with logic-based programming.
+Boolean Operators are used to construct queries with one or more SearchClauses. Their usage is extrememly simply by design, and should be familiar to people working with logic-based programming.
 
 For example, the query:
-`OR(IndexQuery("alma", "title", "=", "Harry"), IndexQuery("alma", "title", "=", "Potter"))`
+`OR(SearchClause("alma", "title", "=", "Harry"), SearchClause("alma", "title", "=", "Potter"))`
 will produce the following string, when formatted:
 `alma.title="Harry" or alma.title="Potter"` (except spaces will be replaced with '%20')
 
+<br>
+<br>
+
 ---
 
 ## Full Overview of Different Components
 
 This section will give a deep dive on each different component in sru_queryer. Check here if you can't figure something out!
 
-### Basic Query Component: IndexQuery
+<br>
 
-`from sru_queryer import IndexQuery`
+### Basic Query Component: SearchClause
 
-A SRU query, written in CQL, is made up of one or more queries on Indexes - here called an IndexQuery. Formatted, an index query looks like:
+`from sru_queryer import SearchClause`
+
+A SRU query, written in CQL, is made up of one or more search clauses. Formatted, a search clause looks like:
 
 `alma.title="Harry Potter"`
 
-The four components of this query are the context_set (`alma`), the index (`title`), the operation(`=`, called 'relation' officially), and the value (`Harry Potter`, called 'search term' officially). For more information, please see https://www.loc.gov/standards/sru/cql/spec.html. I won't explain the nuances of SRU/CQL here, just my implementation of it.
+The four components of this query are the context_set (`alma`), the index (`title`), the relation(`=`), and the search term (`Harry Potter`). For more information, please see https://www.loc.gov/standards/sru/cql/spec.html. I won't explain the nuances of SRU/CQL here, just my implementation of it.
 
 #### USAGE
 
-All of the options for initializing an IndexQuery are keyword arguments, but are listed in an order that's the same as a standard index query (aside from modifiers).
-This means you can initialize an IndexQuery in a human-readable way without including any keywords:
-`IndexQuery("alma", "title", "=", "Harry Potter")`
+All of the options for initializing a SearchClause are keyword arguments, but are listed in order.
+This means you can initialize a SearchClause in a human-readable way without including any keywords:
+`SearchClause("alma", "title", "=", "Harry Potter")`
 which looks like the formatted query:
 `alma.title="Harry Potter"`.
 
-For queries without all options, you have to include the option name for each option OR include 'None' where the option would be.
-Query with only a value:
-`IndexQuery(value="Harry Potter")` or `IndexQuery(None, None, None, "Harry Potter")`
-Query without a context_set:
-`IndexQuery(index_name="title", operation="=", value="Harry Potter")` or
-`IndexQuery(None, "title", "=", "Harry Potter")`
+For SearchClauses without all options, you have to include the option name for each option OR include 'None' where the option would be.<br>
+SearchClause with only a search term:<br>
+`SearchClause(search_term="Harry Potter")` or `SearchClause(None, None, None, "Harry Potter")`<br>
+SearchClause without a context_set:<br>
+`SearchClause(index_name="title", relation="=", search_term="Harry Potter")` or <br>
+`SearchClause(None, "title", "=", "Harry Potter")`
 
-Keep in mind, if a context_set or index_name is not provided, the defaults must be set manually though SRUUtil for validation to work. This is because the explainResponse does not include the default context set or index. If you do not know them, there are options to disable validation for IndexQueries that use defaults.
+Keep in mind, if a context_set or index_name is not provided, the defaults must be set manually during initialization of SRUQueryer for validation to work. This is because the explainResponse does not always include the default context set or index. If you do not know them, there are options to disable validation for SearchClauses that use defaults.
 
 #### AVAILABLE FUNCTIONS
 
-You don't need to use any functions on an IndexQuery as a general user. For instance, the Query.validate() function will also run the validate() function for all included IndexQueries.
+You don't need to use any functions on a SearchClause as a general user. For instance, SRUQueryer will run the validate() function for all included SearchClauses.
 
 #### INITIALIZATION OPTIONS
 
-Internal variables are private once initialized - if you change them, you will bypass some validation and likely cause errors. It's easy to create a new instance of IndexQuery if you need different options, so do that instead of modifying an existing one.
+Internal variables are private once initialized - if you change them, you will bypass some validation and likely cause errors. It's easy to create a new instance of SearchClause if you need different options, so do that instead of modifying an existing one.
 
-| Option      | Data Type                 | Mandatory | Description                                                                          |
-| ----------- | ------------------------- | --------- | ------------------------------------------------------------------------------------ |
-| context_set | string / None             | No        | The context set to search in.                                                        |
-| index_name  | string / None             | No        | The index you want to search.                                                        |
-| operation   | string / None             | No        | The operator ("=", ">", etc) you want to search with.                                |
-| value       | string                    | Yes       | The value you're looking for.                                                        |
-| modifiers   | list of RelationModifiers | No        | A list of relation modifiers for the operation. More information on modifiers below. |
+| Option      | Data Type                 | Mandatory | Description                                                                         |
+| ----------- | ------------------------- | --------- | ----------------------------------------------------------------------------------- |
+| context_set | string / None             | No        | The context set to search in.                                                       |
+| index_name  | string / None             | No        | The index you want to search.                                                       |
+| relation    | string / None             | No        | The operator ("=", ">", etc) you want to search with.                               |
+| search_term | string                    | Yes       | The value you're looking for.                                                       |
+| modifiers   | list of RelationModifiers | No        | A list of relation modifiers for the relation. More information on modifiers below. |
 
-COMBINATIONS OF INITIALIZATION PROPERTIES (according to LOC standards):
+COMBINATIONS OF INITIALIZATION PROPERTIES (according to LOC standards):<br>
 You MUST include either:
 
-1. a value,
-2. an index_name, operation, and value,
-3. a context_set, index_name, operation, and value.
+1. a search term,
+2. an index_name, relation, and search term,
+3. a context_set, index_name, relation, and search term.
 
-- RelationModifiers can be set for all combinations, but will only added to the final query on combinations with an operation.
+- RelationModifiers can be set for all combinations, but will only added to the final query on combinations with an relation.
 
-### SRUUtil
+<br>
+<br>
 
-`from sru_queryer import SRUUtil`
+### SRUQueryer
 
-The SRUUtil static class handles core configuration for this utility, as well as providing an interface for reading the configuration information.
+`from sru_queryer import SRUQueryer`
 
-#### AVAILABLE FUNCTIONS:
+The SRUQueryer is the most important class of this library, as it handles configuring the utility as well as constructing, validating, and sending requests.
 
-There are two functions that the general user would want to use:
+The SRUQueryer stores all its configuration information in an SRUConfiguration object in the property sru_configuration. If you want your program to know the capabilites of the SRU server, it can read the properties of queryer.sru_configuration. For instance, you can access the available record schemas with:<br>
 
-1. `format_available_indexes` - This function nicely formats all the indexes availabe for an SRU server, as well as their information. It then prints this information to the console, to a text file, or both. It only prints to the console by default. You can filter the indexes based on their human-readable title.
+`queryer.sru_configuration.available_record_schemas`<br>
 
-`format_available_indexes(sru_configuration, filename: str | None = None, print_to_console: bool = True, title_filter: str | None = None)`
+It is HIGHLY recommended not to change any of these values.
 
-2. `create_configuration_for_server` - This function creates an SRUConfiguration object by reading you provide as arguments to the function, pulling values found by contacting the SRU server, and reconciling them. Many arguments are optional and are used for improved validation of the SRU queries. Be aware that any option you specify manually will override the corresponding value returned by the explainResponse, if the explainResponse contains this value.
+#### INITIALIZATION OPTIONS
 
-Arguments for create_configuration_for_server:
+This function configures settings (stored in an SRUConfiguration object) by reading the arguments you provide, pulling values from the SRU server, and reconciling them. Many arguments are optional and are used for improved validation of the SRU queries. Be aware that any option you specify manually will override the corresponding value returned by the explainResponse, if the explainResponse contains this value.
 
-`explain_url`
-| Mandatory | Data Type | Description |
-| ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| Yes | url string | The base URL for the explainResponse. This must not include any query params - they will be added by the utility. |
+If the SRU server returns a different SRU version than you the one you specify, the library will use that version. If you do not provide a version, it will default to version 1.2 or whatever the server is capable of.
 
-`search_retrieve_url`
+`server_url`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| Yes | url string | The base URL for the searchRetrieve query. This must not include any query params - they will be added by the utility. |
+| Yes | url string | The base URL for the server. This must not include any query params - they will be added by the utility. |
 
 `sru_version`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| Yes, but defaults to 1.2 | string | The SRU version to use.|
-
-`driver`
-| Mandatory | Data Type | Description |
-| --- | --- | --- |
-| Yes, but defaults to Alma driver | dict | The driver for parsing the xml explainResponse. This is needed because different SRU servers have their data located in different XML paths. The driver tells the program where to look. The drivers are arrays of strings, each string representing a key in a higherarchical dictionary. The drivers will be run on the explainResponse AFTER it's been parsed by the xmltodict library. Additional drivers can be imported from `sru_queryer.drivers` |
+| No - defaults to 1.2 | string | The SRU version to use. If the SRU server returns a different SRU version than you specify, the tool will use that version. If you do not provide a version, it will default to version 1.2. |
 
 `username`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
 | No | string | The username for the SRU server, if the server requires authentication. This is sent in Basic Access Authentication format. |
 
 `password`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
 | No (unless there's a username) | string | The password for the SRU server, if the server requires authentication. This is sent in Basic Access Authentication format. |
 
 `default_cql_context_set`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| No | string | The default context set for indexes if one is not provided. Adding a default enables validation for IndexQueries without context sets. For example, if the default context set is set to 'alma', this will validate the query `title="Harry Potter"` as if it were `alma.title="Harry Potter"`. The default MUST be the same as the default context set for your SRU server. Some SRU servers return this information in the explainResponse; others don't.|
+| No | string | The default context set for indexes if one is not provided. Adding a default enables validation for SearchClauses without context sets. For example, if the default context set is set to 'alma', this will validate the query `title="Harry Potter"` as if it were `alma.title="Harry Potter"`. The default MUST be the same as the default context set for your SRU server. Some SRU servers return this information in the explainResponse; others don't.|
 
 `default_cql_index`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| No | string |The default index for an IndexQuery if only a value is provided. If you have a default_cql_index, you must also have a default_cql_context_set. For example, if the default context set is 'alma' and the default index is 'title', the query `"Harry Potter"` will be validated as `alma.title "Harry Potter"`. |
+| No | string |The default index for a SearchClause if only a search term is provided. If you have a default_cql_index, you must also have a default_cql_context_set. For example, if the default context set is 'alma' and the default index is 'title', the query `"Harry Potter"` will be validated as `alma.title "Harry Potter"`. |
 
 `default_cql_relation`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| No | string |The default relation for an IndexQuery if only a value is provided. If you have a default_cql_relation, you must also have a default_cql_context_set and index. For example, if the default context set is 'alma' and the default index is 'title', the query `"Harry Potter"` will be validated as `alma.title="Harry Potter"`. Not all SRU servers list valid relations for index queries, so this is ONLY NECCESARY when validating defaults for servers that do. If you server does not, you can safely ignore this even if you don't disable validation for cql defaults.|
+| No | string |The default relation for a SearchClause if only a search term is provided. If you have a default_cql_relation, you must also have a default_cql_context_set and index. For example, if the default context set is 'alma' and the default index is 'title', the query `"Harry Potter"` will be validated as `alma.title="Harry Potter"`. Not all SRU servers list valid relations for SearchClauses, so this is ONLY NECCESARY when validating defaults for servers that do. If you server does not, you can safely ignore this even if you don't disable validation for cql defaults.|
 
 `disable_validation_for_cql_defaults`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| No | boolean | If you don't know the default context set, index, and relation (if relation information for indexes is specified) for your SRU server, yet you still want to send IndexQueries with default values, this setting will allow for that. It will disable any validation for indexQuery defaults, but allow validation for non-defaults. |
+| No | boolean | If you don't know the default context set, index, and relation (if relation information for indexes is specified) for your SRU server, yet you still want to send SearchClauses with defaults, this setting will allow for that. It will disable any validation for SearchClause defaults, but allow validation for non-defaults. |
 
 `max_records_supported`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
 | No | int | This indicates the maximum number of records a searchRetrieve response is capable of returning. This is often returned by the explainResponse. If your server's maximum is not included in its explainResponse, it is recommended to include this value. Without it, the number of records requested in a query will not be validated correctly. |
 
 `default_records_returned`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| No | int | This indicates the default maximum number of records that the searchRetrieve will return. It must be equal to or less than the max_records_supported. If set, every query will return a maximum of this number of records. By default, it is set to whatever SRUUtil finds in the explainResponse OR, if not specified in the explainResponse, will not be included. |
+| No | int | This indicates the default maximum number of records that the searchRetrieve will return. It must be equal to or less than the max_records_supported. If set, every query will return a maximum of this number of records. By default, it is set to whatever is in the explainResponse OR, if not specified in the explainResponse, will not be included. |
 
 `default_record_schema`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
 | No | string | The default record schema that's returned by the searchRetrieve operation. If you don't specify what record schema you want in an individual query, the default record schema (if set) will be used in that query. If the explainResponse includes a default record schema and you don't specify one, the explainResponse's record schema will be included in all queries. |
 
 `default_sort_schema`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
 | No | string | The default schema that sort operations are run on. I don't know too much about this. I use it for validating sortKeys, which are only for version 1.1. If the sort schema is not included in a sort key, this value will be used to validate the sort key (not all schemas can sort).|
 
-### Constructing more advanced queries: Boolean Operators
+#### AVAILABLE FUNCTIONS:
+
+There are three functions that the general user would want to use:
+
+##### `search_retrieve`
+
+This function sends a search retrieve request, using the values you provide and the information parsed from the SRU ExplainResponse.
+
+##### USAGE
+
+After initializing your SRUQueryer class: <br>
+`response_content = queryer.search_retrieve(OR(SearchClause("alma", "title", "=", "Harry"), SearchClause("alma", "title", "=", "Potter")), record_schema="marcxml")`
+
+There are additional options to you can set to modify the request. They will be discussed below.
+
+This will validate and send the request. You will receive whatever content the SRU server sends back - it may be a searchRetrieveResponse, or it might be an error. This library does not currently validate or parse the response.
+
+##### INPUT PARAMETERS
+
+| Option          | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                           |
+| --------------- | --------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| cql_query       | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                    |
+| start_record    | int                                                             | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                     |
+| maximum_records | int                                                             | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUQueryer initialization.create_configuration_for_server, by the explainResponse, or is set to 5.                                                     |
+| record_schema   | string                                                          | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse. |
+| sort_queries    | list[dict] or list[SortKey]                                     | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                              |
+| record_packing  | string                                                          | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                         |
+| validate        | boolean (default True)                                          | No        | Whether or not to validate the query before sending it. You can disable validation if you think the library is falsely failing a query.                                                                                                                               |
+
+<br>
+
+##### `construct_search_retrieve_request`
+
+This does the same thing as the previous function, however instead of running request.prepare() and sending the request, it returns the requests.Request object. This allows you to be more flexible by modifying the request - for instance, if you want to use a shared requests.Session between multiple requests, or add a custom authentication header.
+
+##### USAGE
+
+After initializing your SRUQueryer class: <br>
+`request = queryer.construct_search_retrieve_request(OR(SearchClause("alma", "title", "=", "Harry"), SearchClause("alma", "title", "=", "Potter")), record_schema="marcxml")`
+
+This will validate the request and return a requests.Request object.
+
+##### INPUT PARAMETERS
+
+| Option          | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                           |
+| --------------- | --------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| cql_query       | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                    |
+| start_record    | int                                                             | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                     |
+| maximum_records | int                                                             | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUQueryer initialization.create_configuration_for_server, by the explainResponse, or is set to 5.                                                     |
+| record_schema   | string                                                          | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse. |
+| sort_queries    | list[dict] or list[SortKey]                                     | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                              |
+| record_packing  | string                                                          | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                         |
+| validate        | boolean (default True)                                          | No        | Whether or not to validate the query before returning the requests.Request object. You can disable validation if you think the library is falsely failing a query.                                                                                                    |
+
+##### `format_available_indexes`
+
+This function nicely formats all the indexes availabe for an SRU server, as well as their information. It then prints this information to the console, to a text file, or both. It only prints to the console by default. You can filter the indexes based on their human-readable title.
+
+`format_available_indexes(sru_configuration, filename: str | None = None, print_to_console: bool = True, title_filter: str | None = None)`
+
+<br>
+<br>
+
+### Boolean Operators
 
 `from sru_queryer.cql import AND, OR, NOT, PROX`
 
-Boolean Operators are used to construct queries with one or more IndexQueries. Their usage is extrememly simply by design, and should be familiar to people working with logic-based programming.
+Boolean Operators are used to construct queries with one or more SearchClauses. Their usage is extrememly simply by design, and should be familiar to people working with logic-based programming.
 
 #### USAGE
 
-Each operator takes an unlimited quantity of arguments, each of which represents a logical condition. Each condition can be an IndexQuery, a Literal (discussed below), or another nested Boolean Operator.
+Each operator takes an unlimited quantity of arguments, each of which represents a logical condition. Each condition can be a SearchClause, a RawCQL class (discussed below), or another nested Boolean Operator.
 
 For example, the query:
-`OR(IndexQuery("alma", "title", "=", "Harry"), IndexQuery("alma", "title", "=", "Potter"))`
+`OR(SearchClause("alma", "title", "=", "Harry"), SearchClause("alma", "title", "=", "Potter"))`
 will produce the following string, when formatted:
 `alma.title="Harry" or alma.title="Potter"` (except spaces will be replaced with '%20')
 
 If you nest one Boolean Operator within another, the resultant behavior will depend on whether the nested boolean operator has one condition or whether it has multiple conditions.
 
 1. If the nested operator has one condition, it will REPLACE the preceeding boolean operator of the parent. This allows you to create a long query with alternating boolean operators:
-   `AND(IndexQuery("alma", "title", "=", "Maryland"), OR(IndexQuery("alma", "materialType", "==", "BOOK")), IndexQuery("alma", "main_pub_date", ">", "1975"))`
+   `AND(SearchClause("alma", "title", "=", "Maryland"), OR(SearchClause("alma", "materialType", "==", "BOOK")), SearchClause("alma", "main_pub_date", ">", "1975"))`
    Procduces:
    `alma.title="Maryland" or alma.materialType=="BOOK" and alma.main_pub_date>"1975"` (again, spaces replaced with '%20')
 
    \*\* KEEP IN MIND that you can't have an operator with one condition as the first condition of a parent operator (or as the top condition). This wouldn't make sense because all operators require 2 conditions (none are unary operators, even NOT. Not is treated as 'and-not'). Here, I allow operators with one conditions so that a parent's operator can be overridden - this makes formatting simpler.
 
 2. If the nested operator has more than one condition, it will be surrounded by parenthesis and the parent's operator will be placed before the parenthesis:
-   `AND(IndexQuery("alma", "title", "=", "Maryland"), OR(IndexQuery("alma", "materialType", "==", "BOOK"), IndexQuery("alma", "materialType", "==", "DVD")))`
+   `AND(SearchClause("alma", "title", "=", "Maryland"), OR(SearchClause("alma", "materialType", "==", "BOOK"), SearchClause("alma", "materialType", "==", "DVD")))`
    Produces:
    `alma.title="Maryland" and (alma.materialType=="BOOK" or alma.materialType=="DVD")`
 
 You may add modifiers to the Boolean Operator with the 'modifiers' keyword argument. Please use the correct modifier type for the boolean operator you've chosen - for example, the PROX modifier should use ProxModifier, whereas AND, OR, and NOT should use the AndOrNotModifier. You may create custom modifiers by extending the CQLModifierBase class. More on Modifiers later.
 
 #### AVAILABLE FUNCTIONS
 
-As with the IndexQuery, the functions on the CQL Boolean Operators are not indended to be used by the general person. For example, Query.construct_request() will call format() for all boolean operators.
+As with the SearchClause, the functions on the CQL Boolean Operators are not indended to be used by the general person. For example, SRUQueryer.search_retrieve will call format() for all boolean operators.
 
 #### INITIALIZATION OPTIONS
 
 Any options not marked as MANDATORY are optional. It is not recommended to change any options manually after initializing a CQL Boolean Operator, as this will bypass some validation. It's easy to create a new instance of CQL Boolean Operator if you need different options.
 
-| Option                   | Data Type                                                      | Mandatory | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
-| ------------------------ | -------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| Positional arguments 1-n | IndexQuery, class extending CQLBooleanOperatorBase, or LITERAL | Yes       | Search clauses, which will be joined by the boolean operator. Must have at least one, or two if it is the outermost condition or first condition in a parent operator.                                                                                                                                                                                                                                                                                                                                                                                                                  |
-| modifiers                | list[Class extending CQLModifierBase]                          | No        | A list of modifiers for the boolean operator, which will be tacked on to the end of the operator. Keep in mind that modifiers will be added to each instance of the formatted operator - if there's 3 conditions in the operator, leading to two 'and' conditions, this list will be included for both 'and's. To get around this, you may use a nested Boolean Operator with one condition and add the modifiers to that operator. In this case, it will replace the parent's operator with its own, which has the modifiers. The rest of the parent's operators will not be affected. |
-
-Note: Literals may work in place of modifiers, however, this has not been tested.
-
-### Query class
-
-`from sru_queryer import Query`
-
-Now, for the class which you'll likely use the most - the Query class. Whereas SRUUtil deals with configuration, Query only deals with one specific query. It takes an instance of SRUUtil for the purposes of validation.
-
-#### USAGE
-
-Use the Query class to construct your request.
-Instantiate the SRUUtil class:
-`configuration = SRUUtil.construct_configuration_for_server(...)`
-Create the query class with the desired request:
-`query_util = Query(configuration, OR(IndexQuery("alma", "title", "=", "Harry"), IndexQuery("alma", "title", "=", "Potter")), record_schema="marcxml")`
-
-There are additional options to you can set to modify the request. They will be discussed below.
-
-You can then validate the request with the validate() function, which will throw an error for the first issue it finds:
-`query_util.validate()`
-
-After this, you can get a PreparedRequest and send it:
-`from requests import Session`
-`request_to_send = query_util.construct_request()`
-`s = Session()`
-`response = s.send(request_to_send)`
+| Option                   | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| ------------------------ | --------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| Positional arguments 1-n | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | Search clauses, which will be joined by the boolean operator. Must have at least one, or two if it is the outermost condition or first condition in a parent operator.                                                                                                                                                                                                                                                                                                                                                                                                                  |
+| modifiers                | list[Class extending CQLModifierBase]                           | No        | A list of modifiers for the boolean operator, which will be tacked on to the end of the operator. Keep in mind that modifiers will be added to each instance of the formatted operator - if there's 3 conditions in the operator, leading to two 'and' conditions, this list will be included for both 'and's. To get around this, you may use a nested Boolean Operator with one condition and add the modifiers to that operator. In this case, it will replace the parent's operator with its own, which has the modifiers. The rest of the parent's operators will not be affected. |
 
-This will return an XML response, which might be a searchRetrieve response, or might be an error.
-
-#### AVAILABLE FUNCTIONS
-
-validate: Validates all components of the searchRetrieve request that can be validated. For the query itself, this is a recursive function that validates all CQLBooleanOperators / IndexQueries and their children. It will throw a ValueError an error for the first issue it finds. It returns nothing when successful.
-
-construct_request: Uses all components of the query to construct a searchRetrieve request. It pulls some of the information from the SRUConfiguration, including the base URL, username, password, and version, as well as other defaults that have been specified. Returns a requests.PreparedRequest object.
-
-#### INITIALIZATION OPTIONS
+Note: RawCQL classes may work in place of modifiers, however, this has not been tested.
 
-Unlike many other classes, it is safe to modify variables after instantiating. This is because no validation occurs in the constructor. If you do change something, you'd just have to remember to run validate() again.
+<br>
+<br>
 
-| Option            | Data Type                                                      | Mandatory | Description                                                                                                                                                                                                                                                           |
-| ----------------- | -------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| sru_configuration | SRUConfiguration                                               | Yes       | The configuration of the SRU server, which is used to construct and validate queries. Create a configuration with SRUUtil's create_configuration_for_server()                                                                                                         |
-| index_search      | IndexQuery, class extending CQLBooleanOperatorBase, or LITERAL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                    |
-| start_record      | int                                                            | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                     |
-| maximum_records   | int                                                            | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUUtil.create_configuration_for_server, by the explainResponse, or is set to 5.                                                                       |
-| record_schema     | string                                                         | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse. |
-| sort_queries      | list[dict] or list[SortKey]                                    | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                              |
-| record_packing    | string                                                         | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                         |
+### Custom queries: RawCQL
 
-### Custom queries: LITERAL
+`from sru_queryer.cql import RawCQL`
 
-`from sru_queryer.cql import LITERAL`
+USE ONLY WHEN NEEDED! The RawCQL class allows you to pass a string directly to the CQL query. THE STRING WILL NOT BE VALIDATED.
 
-USE ONLY WHEN NEEDED! The LITERAL class allows you to pass a string directly to the SRU query. THE STRING WILL NOT BE VALIDATED.
+RawCQL is intended for cases in which this library does not support a certain SRU feature OR to bypass a bugged output format.
 
-Literals are intended for cases in which this library does not support a certain SRU feature OR to bypass a bugged output format.
+Using raw cql allows you to insert whatever search condition you need, while still validating the rest of the query. You can use a RawCQL class to replace the entire search query, replace a boolean conditional, or replace a SearchClause.
 
-Using a literal allows you to insert whatever search condition you need, while still validating the rest of the query. You can use a literal to replace the entire search query, replace a boolean conditional, or replace an IndexQuery.
-
-You don't have to worry about creating the string in exact URL notation (e.g., replacing ' ' with %20 or '"' with %22). Characters will be encoded automatically by Query.construct_request().
+You don't have to worry about creating the string in exact URL notation (e.g., replacing ' ' with %20 or '"' with %22). Characters will be encoded automatically by SRUQueryer.search_retrieve().
 
 #### USAGE
 
-Use a literal in place of an IndexQuery or class extending CQLBooleanOperatorBase (AND, OR, NOT, PROX).
+Use a RawCQL class in place of a SearchClause or class extending CQLBooleanOperatorBase (AND, OR, NOT, PROX).
 
-Here's an example of a literal being used instead of an IndexQuery in an AND boolean operator:
-`AND(IndexQuery("alma", "title", "=", "Maryland"), LITERAL("alma.materialType==BOOK"))`
+Here's an example of a RawCQL class being used instead of a SearchClause in an AND boolean operator:
+`AND(SearchClause("alma", "title", "=", "Maryland"), RawCQL("alma.materialType==BOOK"))`
 
-Here's an example of a literal replacing a CQLBooleanOperator and its IndexQueries:
-`LITERAL('alma.title="Maryland" and (alma.materialType=="BOOK" or alma.materialType=="DVD")')`
+Here's an example of a RawCQL class replacing a CQLBooleanOperator and its SearchClauses:
+`RawCQL('alma.title="Maryland" and (alma.materialType=="BOOK" or alma.materialType=="DVD")')`
 
-You can't pass an IndexQuery or a CQLBooleanOperator to a literal and have them be nested inside of it, in the way you can nest CQLBooleanOperators/IndexQueries inside CQLBooleanOperators. You COULD format them in when constructing the literal using string formatting:
-`LITERAL(f'{index_query_1.format()} and {cql_boolean_operator.format()}')`
-...where index_query_1 and cql_boolean_operator are instantiated IndexQuery and CQLBooleanOperatorBase objects.
+You can't pass a SearchClause or a CQLBooleanOperator to a RawCQL class and have them be nested inside of it, in the way you can nest CQLBooleanOperators/SearchClauses inside CQLBooleanOperators. You COULD format them in when constructing the RawCQL class using string formatting:
+`RawCQL(f'{search_clause_1.format()} and {cql_boolean_operator.format()}')`
+...where search_clause_1 and cql_boolean_operator are instantiated SearchClause and CQLBooleanOperatorBase objects.
 
 However, keep in mind that this will disable validation for those inner objects.
 
 #### AVAILABLE FUNCTIONS
 
-There's nothing here that you would want to use. This class is essentially a wrapper around a string which allows it to be interchangable with IndexQueries and CQLBooleanOperators.
+There's nothing here that you would want to use. This class is essentially a wrapper around a string which allows it to be interchangable with SearchClauses and CQLBooleanOperators.
 
 #### INITIALIZATION OPTIONS
 
-| Option         | Data Type              | Mandatory | Description                                                                                                                                                                                                                           |
-| -------------- | ---------------------- | --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| literal_string | string (should be CQL) | Yes       | The string that you want to be executed. Again, you don't have to provide it in a url-exact format, spaces and other special characters will be replaced by their compability characters later on if you're using the provided tools. |
-| add_padding    | boolean                | No        | Whether or not to add a space (%20) before and after the string upon formatting. Set to false by default.                                                                                                                             |
+| Option         | Data Type              | Mandatory | Description                                                                                                                                                                                                           |
+| -------------- | ---------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| raw_cql_string | string (should be CQL) | Yes       | A CQL query as a string. Again, you don't have to provide it in a url-exact format, spaces and other special characters will be replaced by their compability characters later on if you're using the provided tools. |
+| add_padding    | boolean                | No        | Whether or not to add a space (%20) before and after the string upon formatting. Set to false by default.                                                                                                             |
+
+<br>
+<br>
 
 ### Modifiying operators - Modifiers
 
-Modifiers are conditions which modify the search query operators (AND, "all", OR, etc). As indicated above, in version 1.2, they can either modify IndexQuery operators or Boolean Operators.
+Modifiers are conditions which modify the search query operators (AND, "all", OR, etc). As indicated above, in version 1.2, they can either modify SearchClause relations or Boolean Operators.
 
-Each modifier is preceeded by a '/' and optional spacing. One or many modifiers may be included. Modifiers must include a base_name, but MAY include a context_set, operator, and value.
+Each modifier is preceeded by a '/' and optional spacing. One or many modifiers may be included. Modifiers must include a base_name, but MAY include a context_set, comparison symbol, and value.
 
-From the LOC website, a modifier on a Boolean Operator looks like: `dc.title any fish or/rel.combine=sum dc.creator any sanderson`.
-A modifier on an IndexQuery looks like `any /relevant /cql.string`
+From the LOC website, a modifier on a Boolean Operator looks like: <br>
+`dc.title=fish or[/rel.combine=sum] dc.creator=sanderson`.<br>
+A modifier on a SearchClause relation looks like:<br> `any /relevant /cql.string`
 
-One thought of interest - it may be possible to include a LITERAL instead of a modifier for custom modifiers / modifier formats not available through this program. I've not tested it, but it's likely to work.
+One thought of interest - it may be possible to include a RawCQL instead of a modifier if you want to create custom modifiers or modifier formats not available through this program. I've not tested it, but it's likely to work.
 
 #### USAGE
 
-This utility comes with 3 standard modifiers - AndOrNotModifier (for CQL Boolean Operators AND, OR, and NOT), ProxModifier (for CQL Boolean Operator PROX), and RelationModifier (for any IndexQuery relation).
+This utility comes with 3 standard modifiers - AndOrNotModifier (for CQL Boolean Operators AND, OR, and NOT), ProxModifier (for CQL Boolean Operator PROX), and RelationModifier (for any SearchClause relation).
 
 These modifiers differ mainly in validation. The ProxModifier limits the base_name to either 'unit' or 'distance', as these are the base names used by prox, and limits the values for the 'unit' base name in the CQL context set to the values specified in the LOC documentation. Upon validation, an error will be raised if these values are not correct.
 
-This program will NOT validate modifiers in relation to one another - e.g., even though a prox must have one 'unit' and one 'distance' modifier, this is not enforced through validation. You could extend the CQLBooleanOperatorBase or PROX class to create this custom validation, if desired.
+This program will NOT validate combinations of modifiers - e.g., even though a 'PROX' boolean operator must have one 'unit' and one 'distance' modifier, this is not enforced through validation. You could extend the CQLBooleanOperatorBase or PROX class to create this custom validation, if desired.
 
 Example prox modifier:
-`ProxModifier('unit', "=", "sentence", context_set="cql")`
-\*Using the keyword for context set here is optional. I'm just showing it to make the order clear - it's rearranged slightly as compared to an IndexQuery.
+`ProxModifier('cql', 'unit', "=", "sentence")`
+\*Using the keyword for context set here is optional. I'm just showing it to make the order clear - it's rearranged slightly as compared to a SearchClause.
 
 The RelationModifier works in the same way.
 
-Modifiers are added as an array to either IndexQueries or CQLBooleanOperatorBase classes.
+Modifiers are added as an array to either SearchClauses or CQLBooleanOperatorBase classes.
 
 #### AVAILABLE FUNCTIONS
 
 There are no functions here that the general user should need to use.
 
 #### INITIALIZATION OPTIONS
 
 It is not recommended to change any options manually after initializing a Modifier, as this will bypass some validation. It's easy and not resource intensive to create a new instance of a modifier if you need different options.
 
-| Option      | Data Type      | Mandatory | Description                                                                                                             |
-| ----------- | -------------- | --------- | ----------------------------------------------------------------------------------------------------------------------- |
-| base_name   | string         | Yes       | The base name of the modifier (e.g, 'relevant' in `/relevant`). Validated against the whitelist 'supported_base_names'. |
-| operator    | string or None | No        | The operator used in the modifier condition.                                                                            |
-| value       | string or None | No        | The value used in the modifier condition.                                                                               |
-| context_set | string or None | No        | The context set that the base_name should be pulled from.                                                               |
+| Option            | Data Type      | Mandatory | Description                                                     |
+| ----------------- | -------------- | --------- | --------------------------------------------------------------- |
+| context_set       | string or None | No        | The context set that the base_name should be pulled from.       |
+| base_name         | string         | Yes       | The base name of the modifier (e.g, 'relevant' in `/relevant`). |
+| comparison_symbol | string or None | No        | The comparison symbol used in the modifier condition.           |
+| value             | string or None | No        | The value used in the modifier condition.                       |
 
-COMBINATIONS OF INITIALIZATION PROPERTIES (implied from LOC standards):
+COMBINATIONS OF INITIALIZATION PROPERTIES (implied from LOC standards):<br>
 You MUST include either:
 
 1. a base_name,
-2. a context_set, base_name
-3. a base_name, operation, and value,
-4. a context_set, base_name, operation, and value.
+2. a context_set and base_name
+3. a base_name, comparison_symbol, and value,
+4. a context_set, base_name, comparison_symbol, and value.
+
+<br>
+<br>
 
 ### Sorting in 1.2: SortBy clauses
 
 sortBy clauses are simply Python dictionaries with the form:
 `{ "index_set": "alma", "index_name": "creator", "sort_order": "ascending" }`
 Which will be formatted to:
 `sortBy%20alma.creator/sort.ascending`
 
 All values are required. The sort_order can either be "ascending" or "descending."
 
-You should add all desired sortBy clauses to the Query object in an array with the keyword argument 'sort_queries='
+You should add all desired sortBy clauses to the SRUQueryer.search_retrieve or SRUQueryer.construct_search_retrieve_request in an array with the keyword argument 'sort_queries='
+
+<br>
+<br>
 
 ### Sorting in 1.1: SortKey
 
 `from sru_queryer.sru import SortKey`
 
-SortKeys are used to sort results returned by a searchRetrieve request ins SRU version 1.1. SRU 1.1 doesn't specify whether sorting is allow per-index like 1.2 does; rather, it specifies this per record schema.
+SortKeys are used to sort results returned by a searchRetrieve request in SRU version 1.1. SRU 1.1 doesn't specify whether sorting is allow per-index like 1.2 does; rather, it specifies this per record schema.
 
-Note that this isn't imported from CQL. It's actually not part of the CQL query - it's another URL query string parameter.
+Note that this isn't imported from sru_queryer.cql but rather sru_queryer.sru. This is because it's actually not part of the CQL query.
 
 #### USAGE
 
-Simply include a list of SortKeys in the 'sort_queries' parameter of your Query object. They will be automatically validated and formatted.
+Simply include a list of SortKeys in the 'sort_queries' parameter of your SearchRetrieve object. They will be automatically validated and formatted.
 
 #### AVAILABLE FUNCTIONS
 
-There's nothing here that you would need to use; the built-in functions are used by other parts of the SRUUtil program.
+There's nothing here that you would need to use; the built-in functions are used by other parts of the sru_queryer library.
 
 #### INITIALIZATION OPTIONS
 
 | Option         | Data Type | Mandatory | Description                                                                                            |
 | -------------- | --------- | --------- | ------------------------------------------------------------------------------------------------------ |
 | xpath          | string    | Yes       | The xpath of the index you want to sort by. It's just the index name prefixed by the context set.      |
 | schema         | string    | No        | The record schema you want to search by                                                                |
 | ascending      | boolean   | No        | Whether you want the results to be ascending. Default is True, False will set results to be descending |
 | case_sensitive | boolean   | No        | If case should be important during the search. Default is False.                                       |
+
+<br>
+<br>
+
+---
+
+## Known Incompatibilities
+
+Different SRU servers have quirks to their default behaviors, and don't all fully implement the Library of Congress standard on SRU.
+
+Additionally, I haven't been able to test some of the more advanced features of this library, namely the PROX modifier, relation modifiers, and boolean operator modifiers successfully on an SRU server. I've tried to test with 3 SRU servers, and I've never gotten the queries to work properly, even when trying them by hand in the browser URL bar. Even when I use the exact sample from the Library of Congress SRU documentation on the Library of Congress SRU server, it returns errors. However, all the queries that this library creates meet up to the documentation, so I'm hopeful that these features will work if there's a SRU server that supports them. Thankfully, I've been able to test most of the core functionality of the library.
+
+If you know of a valid RelationModifier, BooleanOperatorModifier, or PROX request and have the capability to test it, it would be much appreciated! Part of my issue simply comes from the fact that I don't really know all the use cases for these features, which limits my testing to only one or two. We also need the SRU version 1.1 SortKey functionality to be tested, but again don't have the capability.
+
+Below are a few of the issues I've found.
+
+<br>
+
+### ExLibris Alma SRU server
+
+❌ PROX boolean operator <br>
+❌ NOT boolean operator <br>
+❌ Multiple sort queries (only one supported)
+
+❓ Boolean Operator Modifiers <br>
+❓ RelationModifiers
+
+### Library of Congress SRU server
+
+❌ PROX boolean operator <br>
+❌ Sorting (in either version 1.1 or 1.2) <br>
+❌ Default context set
+
+⚠️ You must include maximum_records in a searchRetrieve query to get any records in return <br>
+⚠️ This server lists BIBFRAME as an available record schema, but fails when requesting it
+
+❓ RelationModifiers <br>
+❓ Boolean Operator Modifiers
+
+### Georgia Public Library 'Public Information Network for Electronic Services' (GAPINES)
+
+⚠️ PROX boolean operator doesn't return an error, but doesn't seem to affect results <br>
+⚠️ Sorting doesn't return an error, but doesn't seem to affect results
+
+❓ RelationModifiers <br>
+❓ Boolean Operator Modifiers
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sru_queryer-1.0.3/pyproject.toml` & `sru_queryer-2.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sru-queryer"
-version = "1.0.3"
+version = "2.0.0"
 description = "A utility for integrating SRU queries into your applications."
 readme = "readme.md"
 requires-python = ">=3.7.17"
 keywords = ["sru", "library", "api"]
 
 authors = [
     {name = "Erik Jones", email = "ejones99@umd.edu"},
```

### Comparing `sru_queryer-1.0.3/readme.md` & `sru_queryer-2.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,488 +1,573 @@
+Metadata-Version: 2.1
+Name: sru-queryer
+Version: 2.0.0
+Summary: A utility for integrating SRU queries into your applications.
+Author-email: Erik Jones <ejones99@umd.edu>
+Maintainer-email: USMAI <libclas@umd.edu>
+Keywords: sru,library,api
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.7.17
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.27.1
+Requires-Dist: xmltodict>=0.13.0
+
 # USMAI SRU Queryer
 
 Welcome to SRU Queryer, a library for working with Search/Retrieval via URL (SRU) created by the USMAI Library Consortium. This package is designed to make working with SRU simple and accurate!
 
 Using this utility has a few big benefits, such as:
 
 1. It handles validating much of the searchRetrieve request. This is particularly helpful because many SRU servers don't have good error messages.
 2. It handles formatting the searchRetrieve request for you. This makes queries much less prone to human mistakes.
-3. It provides functions to see which indexes are available to search in the SRU server.
+3. Programmatically access the capabilities of the SRU server in your program.
 
 ## TABLE OF CONTENTS
 
 1. [Setting Up The Environment](#setting-up-the-environment)
 2. [Basic Usage](#basic-usage)
 3. [Quick Overview of Important Components](#quick-overview-of-important-components)
    1. [Initializing SRU Functionality](#initializing-sru-functionality)
-   2. [Basic Query Component](#basic-query-component-indexquery)
-   3. [Configuration Service](#configuration-service-sruutil)
-   4. [Query class](#creating-queries---the-query-class)
-   5. [Boolean Operators for Queries](#constructing-more-advanced-queries-boolean-operators)
+   2. [Basic Query Component](#basic-query-component-searchclause)
+   3. [Searching using SRUQueryer](#searching-using-sruqueryer)
+   4. [Boolean Operators for Queries](#constructing-more-advanced-queries-boolean-operators)
 4. [Full Overview of Different Components](#full-overview-of-different-components)
-   1. [IndexQuery](#basic-query-component-indexquery-1)
-   2. [SRUUtil](#sruutil)
-   3. [Boolean Operators (AND, OR, NOT, PROX)](#constructing-more-advanced-queries-boolean-operators-1)
-   4. [Query](#query-class)
-   5. [LITERAL](#custom-queries-literal)
-   6. [Modifiers](#modifiying-operators---modifiers)
-   7. [Sorting in v1.2](#sorting-in-12-sortby-clauses)
-   8. [Sorting in v1.1](#sorting-in-11-SortKey)
+   1. [SearchClause](#basic-query-component-searchclause-1)
+   2. [SRUQueryer](#sruqueryer)
+   3. [Boolean Operators (AND, OR, NOT, PROX)](#boolean-operators)
+   4. [RawCQL](#custom-queries-rawcql)
+   5. [Modifiers](#modifiying-operators---modifiers)
+   6. [Sorting in v1.2](#sorting-in-12-sortby-clauses)
+   7. [Sorting in v1.1](#sorting-in-11-SortKey)
+5. [Known Incompatibilities](#known-incompatibilities)
 
 ## Setting Up The Environment
 
-This python script was developed using python 3.10 and tested on python 3.11.1.
-
 To install sru-queryer, just run `pip install sru-queryer`
 
+Note that you may have to specify pip3 if you have python2 installed. The install will fail if you try to use python2's PIP.
+
 ## Basic Usage
 
 Here's just a basic usage example:
 
 ```
 # Create a configuration object for the SRU server, allowing you to validate and send queries.
-sru_configuration = SRUUtil.create_configuration_for_server("https://path-to-sru-server-base", "https://path-to-sru-server-base", "1.2")
-
-# Configure a query - in this case, find records where the creator includes Abraham, sorted alphabetically & ascending.
-query_obj = Query(sru_configuration, IndexQuery(
-        "alma", "creator", "=", "Abraham"), sort_queries=[{
-            "index_set": "alma",
-            "index_name": "creator",
-            "sort_order": "ascending"
-        }])
+queryer = SRUQueryer("https://path-to-sru-server-base")
 
-# Validate the query to see whether it's valid
-query_obj.validate()
-
-# Construct the request (just a python PreparedRequest object)
-request = query_obj.construct_request()
-
-s = Session()
-response = s.send(request)
+# Configure a SearchRetrieve query - in this case, find records where the creator includes Abraham, sorted alphabetically & ascending.
+response_content = queryer.search_retrieve(SearchClause("alma", "creator", "=", "Abraham"),
+                     sort_queries=[{
+                           "index_set": "alma",
+                           "index_name": "creator",
+                           "sort_order": "ascending"
+                     }])
 ```
 
 This code will send the following query:
 https://path-to-sru-server-base/?version=1.2&operation=searchRetrieve&recordSchema=marcxml&maximumRecords=10&query=alma.creator=%22Abraham%22%20sortBy%20alma.creator/sort.ascending
 
 You can also create a query with boolean conditions:
 
 ```
 # Find records where the creator includes Abraham AND the material type is 'book'
-query_obj = Query(sru_configuration, AND(IndexQuery("alma", "creator", "=", "Abraham"), IndexQuery("alma", "materialType", "==", "BOOK")))
+queryer.search_retrieve(sru_configuration, AND(SearchClause("alma", "creator", "=", "Abraham"), SearchClause("alma", "materialType", "==", "BOOK")))
 ```
 
 ## Quick Overview of Important Components:
 
 ### Initializing SRU functionality
 
-Before you can validate or send searchRetrieve requests, you must create an SRU configuration for your server. The configuration of this server will be in the form of an SRUConfiguration class.
-
-An instance is created through the SRUUtil.create_configuration_for_server() function, and all you have to do is to pass the created instance to the functions that need it. You can read information from it if you want to integrate SRU querying more deeply into your application.
+Before you can validate or send searchRetrieve requests, you must create a queryer. Upon initialization, the queryer will contact your SRU server and set up everything it needs to validate and format your SRU queries.
 
 ```
-from sru_queryer.drivers import alma_driver
-sru_configuration = SRUUtil.create_configuration_for_server("https://path-to-sru-server-base", "https://path-to-sru-server-base", "1.2", driver=alma_driver)
+queryer = SRUQueryer("https://path-to-sru-server-base")
 ```
 
-This is the most basic way to create a configuration object. The first argument is the SRU explain URL, the second is the searchRetrieve URL, the third is the SRU version, and the final one is the driver. This function takes many other optional arguments, which can do things like configure the default record schemas, default context sets, change validation settings, etc.
+This is the most basic way to create a queryer. This function takes many other optional arguments, which can do things like configure the default record schemas, default context sets, change validation settings, etc.
 
-A very important argument is 'driver'. This takes a dict which tells the program how to parse explainResponses. This program already includes drivers for ExLibris Alma, LOC, and gapines SRU servers. The default is set to 'alma' (ExLibris Alma), which is why you won't see it in some examples. The drivers are straightforward - you can follow the template of the included drivers to create one for your own server. Drivers serve to tell the program where to find the information it needs in the SRU explainResponse and which information is available.
+### Basic Query Component: SearchClause
 
-### Basic Query Component: IndexQuery
+`from sru_queryer.cql import SearchClause`
 
-`from sru_queryer import IndexQuery`
+This is officially known as a 'CQL search clause': https://www.loc.gov/standards/sru/cql/spec.html <br>
+A standard CQL search clause looks like: `alma.title="Harry Potter"`. This same query with the SearchClause class would look like: `SearchClause("alma", "title", "=", "Harry Potter")`. Pretty straightforward! See more in the extended SearchClause section below - there's rules for which of these arguments are required.
 
-This would more officially be known as a 'CQL search clause': https://www.loc.gov/standards/sru/cql/spec.html.\
-A standard CQL search clause looks like: `alma.title="Harry Potter"`. This same query with the IndexQuery class would look like: `IndexQuery("alma", "title", "=", "Harry Potter")`
+### Searching using SRUQueryer
 
-https://www.loc.gov/standards/sru/cql/spec.html
+`from sru_queryer import SRUQueryer`
 
-### Creating queries - the Query class
+There's two options for conducting searchRetrieve requests with the SRUQueryer class. <br>
 
-`from sru_queryer import Query`
+First, you can have the queryer send the request for you and return the content. Once the querier is initialized, you can do so in this way (this is only an example search, it doesn't have to look exactly like this):
 
-Use the Query class to actually construct and validate a query.\
-This class takes the SRU configuration as an argument, followed by the actual CQL query made up of boolean operators, Literals, and IndexQueries. You can also set certain values that you might want to change between queries while keeping the same SRUConfiguration - record format, start record, maximum records, etc. It also takes sort queries.
+```
+response_content = queryer.search_retrieve(SearchClause("alma", "creator", "=", "Abraham"),
+         sort_queries=[{
+            "index_set": "alma",
+            "index_name": "creator",
+            "sort_order": "ascending"
+        }])
+```
+
+Alternately, you can construct a requests.Request object that you can then send yourself. This allows for a bit more flexibility, like adding a custom authentication header:
 
 ```
-query_obj = Query(sru_configuration, IndexQuery(
+request = queryer.construct_search_retrieve_request(SearchClause(
         "alma", "creator", "=", "Abraham"), sort_queries=[{
             "index_set": "alma",
             "index_name": "creator",
             "sort_order": "ascending"
         }])
 ```
 
+Both of these options take the same arguments. The first is the CQL query made up of boolean operators, RawCQL classes, and/or SearchClauses. You can also set certain values that you might want to change between queries while keeping the same queryer - record format, start record, maximum records, etc. It also takes sort queries.
+
 ### Constructing more advanced queries: Boolean Operators
 
 `from sru_queryer.cql import AND, OR, NOT, PROX`
 
-Boolean Operators are used to construct queries with one or more IndexQueries. Their usage is extrememly simply by design, and should be familiar to people working with logic-based programming.
+Boolean Operators are used to construct queries with one or more SearchClauses. Their usage is extrememly simply by design, and should be familiar to people working with logic-based programming.
 
 For example, the query:
-`OR(IndexQuery("alma", "title", "=", "Harry"), IndexQuery("alma", "title", "=", "Potter"))`
+`OR(SearchClause("alma", "title", "=", "Harry"), SearchClause("alma", "title", "=", "Potter"))`
 will produce the following string, when formatted:
 `alma.title="Harry" or alma.title="Potter"` (except spaces will be replaced with '%20')
 
+<br>
+<br>
+
 ---
 
 ## Full Overview of Different Components
 
 This section will give a deep dive on each different component in sru_queryer. Check here if you can't figure something out!
 
-### Basic Query Component: IndexQuery
+<br>
 
-`from sru_queryer import IndexQuery`
+### Basic Query Component: SearchClause
 
-A SRU query, written in CQL, is made up of one or more queries on Indexes - here called an IndexQuery. Formatted, an index query looks like:
+`from sru_queryer import SearchClause`
+
+A SRU query, written in CQL, is made up of one or more search clauses. Formatted, a search clause looks like:
 
 `alma.title="Harry Potter"`
 
-The four components of this query are the context_set (`alma`), the index (`title`), the operation(`=`, called 'relation' officially), and the value (`Harry Potter`, called 'search term' officially). For more information, please see https://www.loc.gov/standards/sru/cql/spec.html. I won't explain the nuances of SRU/CQL here, just my implementation of it.
+The four components of this query are the context_set (`alma`), the index (`title`), the relation(`=`), and the search term (`Harry Potter`). For more information, please see https://www.loc.gov/standards/sru/cql/spec.html. I won't explain the nuances of SRU/CQL here, just my implementation of it.
 
 #### USAGE
 
-All of the options for initializing an IndexQuery are keyword arguments, but are listed in an order that's the same as a standard index query (aside from modifiers).
-This means you can initialize an IndexQuery in a human-readable way without including any keywords:
-`IndexQuery("alma", "title", "=", "Harry Potter")`
+All of the options for initializing a SearchClause are keyword arguments, but are listed in order.
+This means you can initialize a SearchClause in a human-readable way without including any keywords:
+`SearchClause("alma", "title", "=", "Harry Potter")`
 which looks like the formatted query:
 `alma.title="Harry Potter"`.
 
-For queries without all options, you have to include the option name for each option OR include 'None' where the option would be.
-Query with only a value:
-`IndexQuery(value="Harry Potter")` or `IndexQuery(None, None, None, "Harry Potter")`
-Query without a context_set:
-`IndexQuery(index_name="title", operation="=", value="Harry Potter")` or
-`IndexQuery(None, "title", "=", "Harry Potter")`
+For SearchClauses without all options, you have to include the option name for each option OR include 'None' where the option would be.<br>
+SearchClause with only a search term:<br>
+`SearchClause(search_term="Harry Potter")` or `SearchClause(None, None, None, "Harry Potter")`<br>
+SearchClause without a context_set:<br>
+`SearchClause(index_name="title", relation="=", search_term="Harry Potter")` or <br>
+`SearchClause(None, "title", "=", "Harry Potter")`
 
-Keep in mind, if a context_set or index_name is not provided, the defaults must be set manually though SRUUtil for validation to work. This is because the explainResponse does not include the default context set or index. If you do not know them, there are options to disable validation for IndexQueries that use defaults.
+Keep in mind, if a context_set or index_name is not provided, the defaults must be set manually during initialization of SRUQueryer for validation to work. This is because the explainResponse does not always include the default context set or index. If you do not know them, there are options to disable validation for SearchClauses that use defaults.
 
 #### AVAILABLE FUNCTIONS
 
-You don't need to use any functions on an IndexQuery as a general user. For instance, the Query.validate() function will also run the validate() function for all included IndexQueries.
+You don't need to use any functions on a SearchClause as a general user. For instance, SRUQueryer will run the validate() function for all included SearchClauses.
 
 #### INITIALIZATION OPTIONS
 
-Internal variables are private once initialized - if you change them, you will bypass some validation and likely cause errors. It's easy to create a new instance of IndexQuery if you need different options, so do that instead of modifying an existing one.
+Internal variables are private once initialized - if you change them, you will bypass some validation and likely cause errors. It's easy to create a new instance of SearchClause if you need different options, so do that instead of modifying an existing one.
 
-| Option      | Data Type                 | Mandatory | Description                                                                          |
-| ----------- | ------------------------- | --------- | ------------------------------------------------------------------------------------ |
-| context_set | string / None             | No        | The context set to search in.                                                        |
-| index_name  | string / None             | No        | The index you want to search.                                                        |
-| operation   | string / None             | No        | The operator ("=", ">", etc) you want to search with.                                |
-| value       | string                    | Yes       | The value you're looking for.                                                        |
-| modifiers   | list of RelationModifiers | No        | A list of relation modifiers for the operation. More information on modifiers below. |
+| Option      | Data Type                 | Mandatory | Description                                                                         |
+| ----------- | ------------------------- | --------- | ----------------------------------------------------------------------------------- |
+| context_set | string / None             | No        | The context set to search in.                                                       |
+| index_name  | string / None             | No        | The index you want to search.                                                       |
+| relation    | string / None             | No        | The operator ("=", ">", etc) you want to search with.                               |
+| search_term | string                    | Yes       | The value you're looking for.                                                       |
+| modifiers   | list of RelationModifiers | No        | A list of relation modifiers for the relation. More information on modifiers below. |
 
-COMBINATIONS OF INITIALIZATION PROPERTIES (according to LOC standards):
+COMBINATIONS OF INITIALIZATION PROPERTIES (according to LOC standards):<br>
 You MUST include either:
 
-1. a value,
-2. an index_name, operation, and value,
-3. a context_set, index_name, operation, and value.
+1. a search term,
+2. an index_name, relation, and search term,
+3. a context_set, index_name, relation, and search term.
 
-- RelationModifiers can be set for all combinations, but will only added to the final query on combinations with an operation.
+- RelationModifiers can be set for all combinations, but will only added to the final query on combinations with an relation.
 
-### SRUUtil
+<br>
+<br>
 
-`from sru_queryer import SRUUtil`
+### SRUQueryer
 
-The SRUUtil static class handles core configuration for this utility, as well as providing an interface for reading the configuration information.
+`from sru_queryer import SRUQueryer`
 
-#### AVAILABLE FUNCTIONS:
+The SRUQueryer is the most important class of this library, as it handles configuring the utility as well as constructing, validating, and sending requests.
 
-There are two functions that the general user would want to use:
+The SRUQueryer stores all its configuration information in an SRUConfiguration object in the property sru_configuration. If you want your program to know the capabilites of the SRU server, it can read the properties of queryer.sru_configuration. For instance, you can access the available record schemas with:<br>
 
-1. `format_available_indexes` - This function nicely formats all the indexes availabe for an SRU server, as well as their information. It then prints this information to the console, to a text file, or both. It only prints to the console by default. You can filter the indexes based on their human-readable title.
+`queryer.sru_configuration.available_record_schemas`<br>
 
-`format_available_indexes(sru_configuration, filename: str | None = None, print_to_console: bool = True, title_filter: str | None = None)`
+It is HIGHLY recommended not to change any of these values.
 
-2. `create_configuration_for_server` - This function creates an SRUConfiguration object by reading you provide as arguments to the function, pulling values found by contacting the SRU server, and reconciling them. Many arguments are optional and are used for improved validation of the SRU queries. Be aware that any option you specify manually will override the corresponding value returned by the explainResponse, if the explainResponse contains this value.
+#### INITIALIZATION OPTIONS
 
-Arguments for create_configuration_for_server:
+This function configures settings (stored in an SRUConfiguration object) by reading the arguments you provide, pulling values from the SRU server, and reconciling them. Many arguments are optional and are used for improved validation of the SRU queries. Be aware that any option you specify manually will override the corresponding value returned by the explainResponse, if the explainResponse contains this value.
 
-`explain_url`
-| Mandatory | Data Type | Description |
-| ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| Yes | url string | The base URL for the explainResponse. This must not include any query params - they will be added by the utility. |
+If the SRU server returns a different SRU version than you the one you specify, the library will use that version. If you do not provide a version, it will default to version 1.2 or whatever the server is capable of.
 
-`search_retrieve_url`
+`server_url`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| Yes | url string | The base URL for the searchRetrieve query. This must not include any query params - they will be added by the utility. |
+| Yes | url string | The base URL for the server. This must not include any query params - they will be added by the utility. |
 
 `sru_version`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| Yes, but defaults to 1.2 | string | The SRU version to use.|
-
-`driver`
-| Mandatory | Data Type | Description |
-| --- | --- | --- |
-| Yes, but defaults to Alma driver | dict | The driver for parsing the xml explainResponse. This is needed because different SRU servers have their data located in different XML paths. The driver tells the program where to look. The drivers are arrays of strings, each string representing a key in a higherarchical dictionary. The drivers will be run on the explainResponse AFTER it's been parsed by the xmltodict library. Additional drivers can be imported from `sru_queryer.drivers` |
+| No - defaults to 1.2 | string | The SRU version to use. If the SRU server returns a different SRU version than you specify, the tool will use that version. If you do not provide a version, it will default to version 1.2. |
 
 `username`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
 | No | string | The username for the SRU server, if the server requires authentication. This is sent in Basic Access Authentication format. |
 
 `password`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
 | No (unless there's a username) | string | The password for the SRU server, if the server requires authentication. This is sent in Basic Access Authentication format. |
 
 `default_cql_context_set`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| No | string | The default context set for indexes if one is not provided. Adding a default enables validation for IndexQueries without context sets. For example, if the default context set is set to 'alma', this will validate the query `title="Harry Potter"` as if it were `alma.title="Harry Potter"`. The default MUST be the same as the default context set for your SRU server. Some SRU servers return this information in the explainResponse; others don't.|
+| No | string | The default context set for indexes if one is not provided. Adding a default enables validation for SearchClauses without context sets. For example, if the default context set is set to 'alma', this will validate the query `title="Harry Potter"` as if it were `alma.title="Harry Potter"`. The default MUST be the same as the default context set for your SRU server. Some SRU servers return this information in the explainResponse; others don't.|
 
 `default_cql_index`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| No | string |The default index for an IndexQuery if only a value is provided. If you have a default_cql_index, you must also have a default_cql_context_set. For example, if the default context set is 'alma' and the default index is 'title', the query `"Harry Potter"` will be validated as `alma.title "Harry Potter"`. |
+| No | string |The default index for a SearchClause if only a search term is provided. If you have a default_cql_index, you must also have a default_cql_context_set. For example, if the default context set is 'alma' and the default index is 'title', the query `"Harry Potter"` will be validated as `alma.title "Harry Potter"`. |
 
 `default_cql_relation`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| No | string |The default relation for an IndexQuery if only a value is provided. If you have a default_cql_relation, you must also have a default_cql_context_set and index. For example, if the default context set is 'alma' and the default index is 'title', the query `"Harry Potter"` will be validated as `alma.title="Harry Potter"`. Not all SRU servers list valid relations for index queries, so this is ONLY NECCESARY when validating defaults for servers that do. If you server does not, you can safely ignore this even if you don't disable validation for cql defaults.|
+| No | string |The default relation for a SearchClause if only a search term is provided. If you have a default_cql_relation, you must also have a default_cql_context_set and index. For example, if the default context set is 'alma' and the default index is 'title', the query `"Harry Potter"` will be validated as `alma.title="Harry Potter"`. Not all SRU servers list valid relations for SearchClauses, so this is ONLY NECCESARY when validating defaults for servers that do. If you server does not, you can safely ignore this even if you don't disable validation for cql defaults.|
 
 `disable_validation_for_cql_defaults`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| No | boolean | If you don't know the default context set, index, and relation (if relation information for indexes is specified) for your SRU server, yet you still want to send IndexQueries with default values, this setting will allow for that. It will disable any validation for indexQuery defaults, but allow validation for non-defaults. |
+| No | boolean | If you don't know the default context set, index, and relation (if relation information for indexes is specified) for your SRU server, yet you still want to send SearchClauses with defaults, this setting will allow for that. It will disable any validation for SearchClause defaults, but allow validation for non-defaults. |
 
 `max_records_supported`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
 | No | int | This indicates the maximum number of records a searchRetrieve response is capable of returning. This is often returned by the explainResponse. If your server's maximum is not included in its explainResponse, it is recommended to include this value. Without it, the number of records requested in a query will not be validated correctly. |
 
 `default_records_returned`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| No | int | This indicates the default maximum number of records that the searchRetrieve will return. It must be equal to or less than the max_records_supported. If set, every query will return a maximum of this number of records. By default, it is set to whatever SRUUtil finds in the explainResponse OR, if not specified in the explainResponse, will not be included. |
+| No | int | This indicates the default maximum number of records that the searchRetrieve will return. It must be equal to or less than the max_records_supported. If set, every query will return a maximum of this number of records. By default, it is set to whatever is in the explainResponse OR, if not specified in the explainResponse, will not be included. |
 
 `default_record_schema`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
 | No | string | The default record schema that's returned by the searchRetrieve operation. If you don't specify what record schema you want in an individual query, the default record schema (if set) will be used in that query. If the explainResponse includes a default record schema and you don't specify one, the explainResponse's record schema will be included in all queries. |
 
 `default_sort_schema`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
 | No | string | The default schema that sort operations are run on. I don't know too much about this. I use it for validating sortKeys, which are only for version 1.1. If the sort schema is not included in a sort key, this value will be used to validate the sort key (not all schemas can sort).|
 
-### Constructing more advanced queries: Boolean Operators
+#### AVAILABLE FUNCTIONS:
+
+There are three functions that the general user would want to use:
+
+##### `search_retrieve`
+
+This function sends a search retrieve request, using the values you provide and the information parsed from the SRU ExplainResponse.
+
+##### USAGE
+
+After initializing your SRUQueryer class: <br>
+`response_content = queryer.search_retrieve(OR(SearchClause("alma", "title", "=", "Harry"), SearchClause("alma", "title", "=", "Potter")), record_schema="marcxml")`
+
+There are additional options to you can set to modify the request. They will be discussed below.
+
+This will validate and send the request. You will receive whatever content the SRU server sends back - it may be a searchRetrieveResponse, or it might be an error. This library does not currently validate or parse the response.
+
+##### INPUT PARAMETERS
+
+| Option          | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                           |
+| --------------- | --------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| cql_query       | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                    |
+| start_record    | int                                                             | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                     |
+| maximum_records | int                                                             | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUQueryer initialization.create_configuration_for_server, by the explainResponse, or is set to 5.                                                     |
+| record_schema   | string                                                          | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse. |
+| sort_queries    | list[dict] or list[SortKey]                                     | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                              |
+| record_packing  | string                                                          | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                         |
+| validate        | boolean (default True)                                          | No        | Whether or not to validate the query before sending it. You can disable validation if you think the library is falsely failing a query.                                                                                                                               |
+
+<br>
+
+##### `construct_search_retrieve_request`
+
+This does the same thing as the previous function, however instead of running request.prepare() and sending the request, it returns the requests.Request object. This allows you to be more flexible by modifying the request - for instance, if you want to use a shared requests.Session between multiple requests, or add a custom authentication header.
+
+##### USAGE
+
+After initializing your SRUQueryer class: <br>
+`request = queryer.construct_search_retrieve_request(OR(SearchClause("alma", "title", "=", "Harry"), SearchClause("alma", "title", "=", "Potter")), record_schema="marcxml")`
+
+This will validate the request and return a requests.Request object.
+
+##### INPUT PARAMETERS
+
+| Option          | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                           |
+| --------------- | --------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| cql_query       | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                    |
+| start_record    | int                                                             | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                     |
+| maximum_records | int                                                             | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUQueryer initialization.create_configuration_for_server, by the explainResponse, or is set to 5.                                                     |
+| record_schema   | string                                                          | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse. |
+| sort_queries    | list[dict] or list[SortKey]                                     | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                              |
+| record_packing  | string                                                          | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                         |
+| validate        | boolean (default True)                                          | No        | Whether or not to validate the query before returning the requests.Request object. You can disable validation if you think the library is falsely failing a query.                                                                                                    |
+
+##### `format_available_indexes`
+
+This function nicely formats all the indexes availabe for an SRU server, as well as their information. It then prints this information to the console, to a text file, or both. It only prints to the console by default. You can filter the indexes based on their human-readable title.
+
+`format_available_indexes(sru_configuration, filename: str | None = None, print_to_console: bool = True, title_filter: str | None = None)`
+
+<br>
+<br>
+
+### Boolean Operators
 
 `from sru_queryer.cql import AND, OR, NOT, PROX`
 
-Boolean Operators are used to construct queries with one or more IndexQueries. Their usage is extrememly simply by design, and should be familiar to people working with logic-based programming.
+Boolean Operators are used to construct queries with one or more SearchClauses. Their usage is extrememly simply by design, and should be familiar to people working with logic-based programming.
 
 #### USAGE
 
-Each operator takes an unlimited quantity of arguments, each of which represents a logical condition. Each condition can be an IndexQuery, a Literal (discussed below), or another nested Boolean Operator.
+Each operator takes an unlimited quantity of arguments, each of which represents a logical condition. Each condition can be a SearchClause, a RawCQL class (discussed below), or another nested Boolean Operator.
 
 For example, the query:
-`OR(IndexQuery("alma", "title", "=", "Harry"), IndexQuery("alma", "title", "=", "Potter"))`
+`OR(SearchClause("alma", "title", "=", "Harry"), SearchClause("alma", "title", "=", "Potter"))`
 will produce the following string, when formatted:
 `alma.title="Harry" or alma.title="Potter"` (except spaces will be replaced with '%20')
 
 If you nest one Boolean Operator within another, the resultant behavior will depend on whether the nested boolean operator has one condition or whether it has multiple conditions.
 
 1. If the nested operator has one condition, it will REPLACE the preceeding boolean operator of the parent. This allows you to create a long query with alternating boolean operators:
-   `AND(IndexQuery("alma", "title", "=", "Maryland"), OR(IndexQuery("alma", "materialType", "==", "BOOK")), IndexQuery("alma", "main_pub_date", ">", "1975"))`
+   `AND(SearchClause("alma", "title", "=", "Maryland"), OR(SearchClause("alma", "materialType", "==", "BOOK")), SearchClause("alma", "main_pub_date", ">", "1975"))`
    Procduces:
    `alma.title="Maryland" or alma.materialType=="BOOK" and alma.main_pub_date>"1975"` (again, spaces replaced with '%20')
 
    \*\* KEEP IN MIND that you can't have an operator with one condition as the first condition of a parent operator (or as the top condition). This wouldn't make sense because all operators require 2 conditions (none are unary operators, even NOT. Not is treated as 'and-not'). Here, I allow operators with one conditions so that a parent's operator can be overridden - this makes formatting simpler.
 
 2. If the nested operator has more than one condition, it will be surrounded by parenthesis and the parent's operator will be placed before the parenthesis:
-   `AND(IndexQuery("alma", "title", "=", "Maryland"), OR(IndexQuery("alma", "materialType", "==", "BOOK"), IndexQuery("alma", "materialType", "==", "DVD")))`
+   `AND(SearchClause("alma", "title", "=", "Maryland"), OR(SearchClause("alma", "materialType", "==", "BOOK"), SearchClause("alma", "materialType", "==", "DVD")))`
    Produces:
    `alma.title="Maryland" and (alma.materialType=="BOOK" or alma.materialType=="DVD")`
 
 You may add modifiers to the Boolean Operator with the 'modifiers' keyword argument. Please use the correct modifier type for the boolean operator you've chosen - for example, the PROX modifier should use ProxModifier, whereas AND, OR, and NOT should use the AndOrNotModifier. You may create custom modifiers by extending the CQLModifierBase class. More on Modifiers later.
 
 #### AVAILABLE FUNCTIONS
 
-As with the IndexQuery, the functions on the CQL Boolean Operators are not indended to be used by the general person. For example, Query.construct_request() will call format() for all boolean operators.
+As with the SearchClause, the functions on the CQL Boolean Operators are not indended to be used by the general person. For example, SRUQueryer.search_retrieve will call format() for all boolean operators.
 
 #### INITIALIZATION OPTIONS
 
 Any options not marked as MANDATORY are optional. It is not recommended to change any options manually after initializing a CQL Boolean Operator, as this will bypass some validation. It's easy to create a new instance of CQL Boolean Operator if you need different options.
 
-| Option                   | Data Type                                                      | Mandatory | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
-| ------------------------ | -------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| Positional arguments 1-n | IndexQuery, class extending CQLBooleanOperatorBase, or LITERAL | Yes       | Search clauses, which will be joined by the boolean operator. Must have at least one, or two if it is the outermost condition or first condition in a parent operator.                                                                                                                                                                                                                                                                                                                                                                                                                  |
-| modifiers                | list[Class extending CQLModifierBase]                          | No        | A list of modifiers for the boolean operator, which will be tacked on to the end of the operator. Keep in mind that modifiers will be added to each instance of the formatted operator - if there's 3 conditions in the operator, leading to two 'and' conditions, this list will be included for both 'and's. To get around this, you may use a nested Boolean Operator with one condition and add the modifiers to that operator. In this case, it will replace the parent's operator with its own, which has the modifiers. The rest of the parent's operators will not be affected. |
-
-Note: Literals may work in place of modifiers, however, this has not been tested.
-
-### Query class
-
-`from sru_queryer import Query`
-
-Now, for the class which you'll likely use the most - the Query class. Whereas SRUUtil deals with configuration, Query only deals with one specific query. It takes an instance of SRUUtil for the purposes of validation.
-
-#### USAGE
-
-Use the Query class to construct your request.
-Instantiate the SRUUtil class:
-`configuration = SRUUtil.construct_configuration_for_server(...)`
-Create the query class with the desired request:
-`query_util = Query(configuration, OR(IndexQuery("alma", "title", "=", "Harry"), IndexQuery("alma", "title", "=", "Potter")), record_schema="marcxml")`
-
-There are additional options to you can set to modify the request. They will be discussed below.
-
-You can then validate the request with the validate() function, which will throw an error for the first issue it finds:
-`query_util.validate()`
-
-After this, you can get a PreparedRequest and send it:
-`from requests import Session`
-`request_to_send = query_util.construct_request()`
-`s = Session()`
-`response = s.send(request_to_send)`
+| Option                   | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| ------------------------ | --------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| Positional arguments 1-n | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | Search clauses, which will be joined by the boolean operator. Must have at least one, or two if it is the outermost condition or first condition in a parent operator.                                                                                                                                                                                                                                                                                                                                                                                                                  |
+| modifiers                | list[Class extending CQLModifierBase]                           | No        | A list of modifiers for the boolean operator, which will be tacked on to the end of the operator. Keep in mind that modifiers will be added to each instance of the formatted operator - if there's 3 conditions in the operator, leading to two 'and' conditions, this list will be included for both 'and's. To get around this, you may use a nested Boolean Operator with one condition and add the modifiers to that operator. In this case, it will replace the parent's operator with its own, which has the modifiers. The rest of the parent's operators will not be affected. |
 
-This will return an XML response, which might be a searchRetrieve response, or might be an error.
-
-#### AVAILABLE FUNCTIONS
-
-validate: Validates all components of the searchRetrieve request that can be validated. For the query itself, this is a recursive function that validates all CQLBooleanOperators / IndexQueries and their children. It will throw a ValueError an error for the first issue it finds. It returns nothing when successful.
-
-construct_request: Uses all components of the query to construct a searchRetrieve request. It pulls some of the information from the SRUConfiguration, including the base URL, username, password, and version, as well as other defaults that have been specified. Returns a requests.PreparedRequest object.
-
-#### INITIALIZATION OPTIONS
+Note: RawCQL classes may work in place of modifiers, however, this has not been tested.
 
-Unlike many other classes, it is safe to modify variables after instantiating. This is because no validation occurs in the constructor. If you do change something, you'd just have to remember to run validate() again.
+<br>
+<br>
 
-| Option            | Data Type                                                      | Mandatory | Description                                                                                                                                                                                                                                                           |
-| ----------------- | -------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| sru_configuration | SRUConfiguration                                               | Yes       | The configuration of the SRU server, which is used to construct and validate queries. Create a configuration with SRUUtil's create_configuration_for_server()                                                                                                         |
-| index_search      | IndexQuery, class extending CQLBooleanOperatorBase, or LITERAL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                    |
-| start_record      | int                                                            | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                     |
-| maximum_records   | int                                                            | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUUtil.create_configuration_for_server, by the explainResponse, or is set to 5.                                                                       |
-| record_schema     | string                                                         | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse. |
-| sort_queries      | list[dict] or list[SortKey]                                    | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                              |
-| record_packing    | string                                                         | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                         |
+### Custom queries: RawCQL
 
-### Custom queries: LITERAL
+`from sru_queryer.cql import RawCQL`
 
-`from sru_queryer.cql import LITERAL`
+USE ONLY WHEN NEEDED! The RawCQL class allows you to pass a string directly to the CQL query. THE STRING WILL NOT BE VALIDATED.
 
-USE ONLY WHEN NEEDED! The LITERAL class allows you to pass a string directly to the SRU query. THE STRING WILL NOT BE VALIDATED.
+RawCQL is intended for cases in which this library does not support a certain SRU feature OR to bypass a bugged output format.
 
-Literals are intended for cases in which this library does not support a certain SRU feature OR to bypass a bugged output format.
+Using raw cql allows you to insert whatever search condition you need, while still validating the rest of the query. You can use a RawCQL class to replace the entire search query, replace a boolean conditional, or replace a SearchClause.
 
-Using a literal allows you to insert whatever search condition you need, while still validating the rest of the query. You can use a literal to replace the entire search query, replace a boolean conditional, or replace an IndexQuery.
-
-You don't have to worry about creating the string in exact URL notation (e.g., replacing ' ' with %20 or '"' with %22). Characters will be encoded automatically by Query.construct_request().
+You don't have to worry about creating the string in exact URL notation (e.g., replacing ' ' with %20 or '"' with %22). Characters will be encoded automatically by SRUQueryer.search_retrieve().
 
 #### USAGE
 
-Use a literal in place of an IndexQuery or class extending CQLBooleanOperatorBase (AND, OR, NOT, PROX).
+Use a RawCQL class in place of a SearchClause or class extending CQLBooleanOperatorBase (AND, OR, NOT, PROX).
 
-Here's an example of a literal being used instead of an IndexQuery in an AND boolean operator:
-`AND(IndexQuery("alma", "title", "=", "Maryland"), LITERAL("alma.materialType==BOOK"))`
+Here's an example of a RawCQL class being used instead of a SearchClause in an AND boolean operator:
+`AND(SearchClause("alma", "title", "=", "Maryland"), RawCQL("alma.materialType==BOOK"))`
 
-Here's an example of a literal replacing a CQLBooleanOperator and its IndexQueries:
-`LITERAL('alma.title="Maryland" and (alma.materialType=="BOOK" or alma.materialType=="DVD")')`
+Here's an example of a RawCQL class replacing a CQLBooleanOperator and its SearchClauses:
+`RawCQL('alma.title="Maryland" and (alma.materialType=="BOOK" or alma.materialType=="DVD")')`
 
-You can't pass an IndexQuery or a CQLBooleanOperator to a literal and have them be nested inside of it, in the way you can nest CQLBooleanOperators/IndexQueries inside CQLBooleanOperators. You COULD format them in when constructing the literal using string formatting:
-`LITERAL(f'{index_query_1.format()} and {cql_boolean_operator.format()}')`
-...where index_query_1 and cql_boolean_operator are instantiated IndexQuery and CQLBooleanOperatorBase objects.
+You can't pass a SearchClause or a CQLBooleanOperator to a RawCQL class and have them be nested inside of it, in the way you can nest CQLBooleanOperators/SearchClauses inside CQLBooleanOperators. You COULD format them in when constructing the RawCQL class using string formatting:
+`RawCQL(f'{search_clause_1.format()} and {cql_boolean_operator.format()}')`
+...where search_clause_1 and cql_boolean_operator are instantiated SearchClause and CQLBooleanOperatorBase objects.
 
 However, keep in mind that this will disable validation for those inner objects.
 
 #### AVAILABLE FUNCTIONS
 
-There's nothing here that you would want to use. This class is essentially a wrapper around a string which allows it to be interchangable with IndexQueries and CQLBooleanOperators.
+There's nothing here that you would want to use. This class is essentially a wrapper around a string which allows it to be interchangable with SearchClauses and CQLBooleanOperators.
 
 #### INITIALIZATION OPTIONS
 
-| Option         | Data Type              | Mandatory | Description                                                                                                                                                                                                                           |
-| -------------- | ---------------------- | --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| literal_string | string (should be CQL) | Yes       | The string that you want to be executed. Again, you don't have to provide it in a url-exact format, spaces and other special characters will be replaced by their compability characters later on if you're using the provided tools. |
-| add_padding    | boolean                | No        | Whether or not to add a space (%20) before and after the string upon formatting. Set to false by default.                                                                                                                             |
+| Option         | Data Type              | Mandatory | Description                                                                                                                                                                                                           |
+| -------------- | ---------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| raw_cql_string | string (should be CQL) | Yes       | A CQL query as a string. Again, you don't have to provide it in a url-exact format, spaces and other special characters will be replaced by their compability characters later on if you're using the provided tools. |
+| add_padding    | boolean                | No        | Whether or not to add a space (%20) before and after the string upon formatting. Set to false by default.                                                                                                             |
+
+<br>
+<br>
 
 ### Modifiying operators - Modifiers
 
-Modifiers are conditions which modify the search query operators (AND, "all", OR, etc). As indicated above, in version 1.2, they can either modify IndexQuery operators or Boolean Operators.
+Modifiers are conditions which modify the search query operators (AND, "all", OR, etc). As indicated above, in version 1.2, they can either modify SearchClause relations or Boolean Operators.
 
-Each modifier is preceeded by a '/' and optional spacing. One or many modifiers may be included. Modifiers must include a base_name, but MAY include a context_set, operator, and value.
+Each modifier is preceeded by a '/' and optional spacing. One or many modifiers may be included. Modifiers must include a base_name, but MAY include a context_set, comparison symbol, and value.
 
-From the LOC website, a modifier on a Boolean Operator looks like: `dc.title any fish or/rel.combine=sum dc.creator any sanderson`.
-A modifier on an IndexQuery looks like `any /relevant /cql.string`
+From the LOC website, a modifier on a Boolean Operator looks like: <br>
+`dc.title=fish or[/rel.combine=sum] dc.creator=sanderson`.<br>
+A modifier on a SearchClause relation looks like:<br> `any /relevant /cql.string`
 
-One thought of interest - it may be possible to include a LITERAL instead of a modifier for custom modifiers / modifier formats not available through this program. I've not tested it, but it's likely to work.
+One thought of interest - it may be possible to include a RawCQL instead of a modifier if you want to create custom modifiers or modifier formats not available through this program. I've not tested it, but it's likely to work.
 
 #### USAGE
 
-This utility comes with 3 standard modifiers - AndOrNotModifier (for CQL Boolean Operators AND, OR, and NOT), ProxModifier (for CQL Boolean Operator PROX), and RelationModifier (for any IndexQuery relation).
+This utility comes with 3 standard modifiers - AndOrNotModifier (for CQL Boolean Operators AND, OR, and NOT), ProxModifier (for CQL Boolean Operator PROX), and RelationModifier (for any SearchClause relation).
 
 These modifiers differ mainly in validation. The ProxModifier limits the base_name to either 'unit' or 'distance', as these are the base names used by prox, and limits the values for the 'unit' base name in the CQL context set to the values specified in the LOC documentation. Upon validation, an error will be raised if these values are not correct.
 
-This program will NOT validate modifiers in relation to one another - e.g., even though a prox must have one 'unit' and one 'distance' modifier, this is not enforced through validation. You could extend the CQLBooleanOperatorBase or PROX class to create this custom validation, if desired.
+This program will NOT validate combinations of modifiers - e.g., even though a 'PROX' boolean operator must have one 'unit' and one 'distance' modifier, this is not enforced through validation. You could extend the CQLBooleanOperatorBase or PROX class to create this custom validation, if desired.
 
 Example prox modifier:
-`ProxModifier('unit', "=", "sentence", context_set="cql")`
-\*Using the keyword for context set here is optional. I'm just showing it to make the order clear - it's rearranged slightly as compared to an IndexQuery.
+`ProxModifier('cql', 'unit', "=", "sentence")`
+\*Using the keyword for context set here is optional. I'm just showing it to make the order clear - it's rearranged slightly as compared to a SearchClause.
 
 The RelationModifier works in the same way.
 
-Modifiers are added as an array to either IndexQueries or CQLBooleanOperatorBase classes.
+Modifiers are added as an array to either SearchClauses or CQLBooleanOperatorBase classes.
 
 #### AVAILABLE FUNCTIONS
 
 There are no functions here that the general user should need to use.
 
 #### INITIALIZATION OPTIONS
 
 It is not recommended to change any options manually after initializing a Modifier, as this will bypass some validation. It's easy and not resource intensive to create a new instance of a modifier if you need different options.
 
-| Option      | Data Type      | Mandatory | Description                                                                                                             |
-| ----------- | -------------- | --------- | ----------------------------------------------------------------------------------------------------------------------- |
-| base_name   | string         | Yes       | The base name of the modifier (e.g, 'relevant' in `/relevant`). Validated against the whitelist 'supported_base_names'. |
-| operator    | string or None | No        | The operator used in the modifier condition.                                                                            |
-| value       | string or None | No        | The value used in the modifier condition.                                                                               |
-| context_set | string or None | No        | The context set that the base_name should be pulled from.                                                               |
+| Option            | Data Type      | Mandatory | Description                                                     |
+| ----------------- | -------------- | --------- | --------------------------------------------------------------- |
+| context_set       | string or None | No        | The context set that the base_name should be pulled from.       |
+| base_name         | string         | Yes       | The base name of the modifier (e.g, 'relevant' in `/relevant`). |
+| comparison_symbol | string or None | No        | The comparison symbol used in the modifier condition.           |
+| value             | string or None | No        | The value used in the modifier condition.                       |
 
-COMBINATIONS OF INITIALIZATION PROPERTIES (implied from LOC standards):
+COMBINATIONS OF INITIALIZATION PROPERTIES (implied from LOC standards):<br>
 You MUST include either:
 
 1. a base_name,
-2. a context_set, base_name
-3. a base_name, operation, and value,
-4. a context_set, base_name, operation, and value.
+2. a context_set and base_name
+3. a base_name, comparison_symbol, and value,
+4. a context_set, base_name, comparison_symbol, and value.
+
+<br>
+<br>
 
 ### Sorting in 1.2: SortBy clauses
 
 sortBy clauses are simply Python dictionaries with the form:
 `{ "index_set": "alma", "index_name": "creator", "sort_order": "ascending" }`
 Which will be formatted to:
 `sortBy%20alma.creator/sort.ascending`
 
 All values are required. The sort_order can either be "ascending" or "descending."
 
-You should add all desired sortBy clauses to the Query object in an array with the keyword argument 'sort_queries='
+You should add all desired sortBy clauses to the SRUQueryer.search_retrieve or SRUQueryer.construct_search_retrieve_request in an array with the keyword argument 'sort_queries='
+
+<br>
+<br>
 
 ### Sorting in 1.1: SortKey
 
 `from sru_queryer.sru import SortKey`
 
-SortKeys are used to sort results returned by a searchRetrieve request ins SRU version 1.1. SRU 1.1 doesn't specify whether sorting is allow per-index like 1.2 does; rather, it specifies this per record schema.
+SortKeys are used to sort results returned by a searchRetrieve request in SRU version 1.1. SRU 1.1 doesn't specify whether sorting is allow per-index like 1.2 does; rather, it specifies this per record schema.
 
-Note that this isn't imported from CQL. It's actually not part of the CQL query - it's another URL query string parameter.
+Note that this isn't imported from sru_queryer.cql but rather sru_queryer.sru. This is because it's actually not part of the CQL query.
 
 #### USAGE
 
-Simply include a list of SortKeys in the 'sort_queries' parameter of your Query object. They will be automatically validated and formatted.
+Simply include a list of SortKeys in the 'sort_queries' parameter of your SearchRetrieve object. They will be automatically validated and formatted.
 
 #### AVAILABLE FUNCTIONS
 
-There's nothing here that you would need to use; the built-in functions are used by other parts of the SRUUtil program.
+There's nothing here that you would need to use; the built-in functions are used by other parts of the sru_queryer library.
 
 #### INITIALIZATION OPTIONS
 
 | Option         | Data Type | Mandatory | Description                                                                                            |
 | -------------- | --------- | --------- | ------------------------------------------------------------------------------------------------------ |
 | xpath          | string    | Yes       | The xpath of the index you want to sort by. It's just the index name prefixed by the context set.      |
 | schema         | string    | No        | The record schema you want to search by                                                                |
 | ascending      | boolean   | No        | Whether you want the results to be ascending. Default is True, False will set results to be descending |
 | case_sensitive | boolean   | No        | If case should be important during the search. Default is False.                                       |
+
+<br>
+<br>
+
+---
+
+## Known Incompatibilities
+
+Different SRU servers have quirks to their default behaviors, and don't all fully implement the Library of Congress standard on SRU.
+
+Additionally, I haven't been able to test some of the more advanced features of this library, namely the PROX modifier, relation modifiers, and boolean operator modifiers successfully on an SRU server. I've tried to test with 3 SRU servers, and I've never gotten the queries to work properly, even when trying them by hand in the browser URL bar. Even when I use the exact sample from the Library of Congress SRU documentation on the Library of Congress SRU server, it returns errors. However, all the queries that this library creates meet up to the documentation, so I'm hopeful that these features will work if there's a SRU server that supports them. Thankfully, I've been able to test most of the core functionality of the library.
+
+If you know of a valid RelationModifier, BooleanOperatorModifier, or PROX request and have the capability to test it, it would be much appreciated! Part of my issue simply comes from the fact that I don't really know all the use cases for these features, which limits my testing to only one or two. We also need the SRU version 1.1 SortKey functionality to be tested, but again don't have the capability.
+
+Below are a few of the issues I've found.
+
+<br>
+
+### ExLibris Alma SRU server
+
+❌ PROX boolean operator <br>
+❌ NOT boolean operator <br>
+❌ Multiple sort queries (only one supported)
+
+❓ Boolean Operator Modifiers <br>
+❓ RelationModifiers
+
+### Library of Congress SRU server
+
+❌ PROX boolean operator <br>
+❌ Sorting (in either version 1.1 or 1.2) <br>
+❌ Default context set
+
+⚠️ You must include maximum_records in a searchRetrieve query to get any records in return <br>
+⚠️ This server lists BIBFRAME as an available record schema, but fails when requesting it
+
+❓ RelationModifiers <br>
+❓ Boolean Operator Modifiers
+
+### Georgia Public Library 'Public Information Network for Electronic Services' (GAPINES)
+
+⚠️ PROX boolean operator doesn't return an error, but doesn't seem to affect results <br>
+⚠️ Sorting doesn't return an error, but doesn't seem to affect results
+
+❓ RelationModifiers <br>
+❓ Boolean Operator Modifiers
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sru_queryer-1.0.3/src/sru_queryer/_base/_cql_boolean_operators.py` & `sru_queryer-2.0.0/src/sru_queryer/_base/_cql_boolean_operators.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
-from ._search_index_config import IndexQuery
-from ._cql_literal import LITERAL
+from ._search_clause import SearchClause
+from ._raw_cql import RawCQL
 from ._cql_modifiers import AndOrNotModifier, CQLModifierBase
 
 
 class CQLBooleanOperatorBase:
     operator = None
     unary_operator_error = "Error during formatting: Operator cannot have one argument AND the first condition of a parent operator (including if it's used by itself). No operators are unary, even NOT."
 
     def __init__(self, *args, modifiers: list[AndOrNotModifier] = None):
         self.conditions = []
 
         for condition in args:
-            if isinstance(condition, IndexQuery) or isinstance(condition, CQLBooleanOperatorBase) or isinstance(condition, LITERAL):
+            if isinstance(condition, SearchClause) or isinstance(condition, CQLBooleanOperatorBase) or isinstance(condition, RawCQL):
                 self.conditions.append(condition)
             else:
                 raise ValueError(
                     f"Condition '{condition.__str__()}' is not valid")
 
         if not self.conditions:
             raise ValueError(
@@ -32,33 +32,33 @@
         is_unary_operator = len(self.conditions) == 1
 
         if is_first_condition_of_parent and is_unary_operator:
             raise ValueError(self.unary_operator_error)
 
         formatted_conditional = ""
         is_first_condition_of_conditions = True
-        for operator_index_or_literal in self.conditions:
+        for operator_is_index_or_raw_cql in self.conditions:
 
             parent_is_first_condition_of_parent = is_first_condition_of_parent
             # For clarity, I've set this variable name here. This means,
             # "the parent of this condition (which is 'self', the object
             # that this function is in) is the first condition in its
             # parent operator (or, its the first level operator)"
 
             parent_is_unary_operator = is_unary_operator
             # Same deal as above. Now referring to the parent of this conditional in
             # the loop, which is 'self'
 
             condition_is_operator = isinstance(
-                operator_index_or_literal, CQLBooleanOperatorBase)
-            condition_is_index_or_literal = isinstance(
-                operator_index_or_literal, IndexQuery) or isinstance(operator_index_or_literal, LITERAL)
+                operator_is_index_or_raw_cql, CQLBooleanOperatorBase)
+            condition_is_index_or_raw_cql = isinstance(
+                operator_is_index_or_raw_cql, SearchClause) or isinstance(operator_is_index_or_raw_cql, RawCQL)
 
             if condition_is_operator:
-                operator = operator_index_or_literal
+                operator = operator_is_index_or_raw_cql
                 # Renaming to operator because we checked above whether it's an operator.
 
                 condition_is_unary_operator = len(
                     operator.conditions) == 1
 
                 # Different conditions we're testing for, varies whether the operator is included or not.
 
@@ -74,24 +74,24 @@
                 # If the operator has multiple conditions (which means it's surrounded by parenthesis),
                 # and it isn't the first condition of this (self)'s conditions, we should add self's
                 # boolean operator beforehand
 
                 if operator_is_unary_and_parent_is_not_first_condition or operator_has_multiple_conditions_and_is_not_first_condition_of_conditions:
                     formatted_conditional += self.format_operator()
 
-            elif condition_is_index_or_literal:
+            elif condition_is_index_or_raw_cql:
                 # Now we check whether we should append self's operator given the condition is an index
 
                 is_first_condition_and_parent_is_unary_operator_and_parent_not_first_condition = (
                     not parent_is_first_condition_of_parent and is_first_condition_of_conditions and parent_is_unary_operator)
 
                 if not is_first_condition_of_conditions or is_first_condition_and_parent_is_unary_operator_and_parent_not_first_condition:
                     formatted_conditional += self.format_operator()
 
-            formatted_conditional += f"{operator_index_or_literal._format(nested_condition=True, is_first_condition_of_parent=is_first_condition_of_conditions)}"
+            formatted_conditional += f"{operator_is_index_or_raw_cql._format(nested_condition=True, is_first_condition_of_parent=is_first_condition_of_conditions)}"
             is_first_condition_of_conditions = False
 
         if nested_condition and not is_unary_operator:
             formatted_conditional = f"({formatted_conditional})"
         return formatted_conditional
 
     def format_operator(self):
```

### Comparing `sru_queryer-1.0.3/src/sru_queryer/_base/_cql_modifiers.py` & `sru_queryer-2.0.0/src/sru_queryer/_base/_cql_modifiers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,70 @@
 from __future__ import annotations
 
 # I know this is bad coupling, but it would take too refactoring work to fix.
 from ._sru_validator import SRUValidator
 
 class CQLModifierBase:
     # Pulled from Library of Congress docs.
-    supported_operators = ["=", "<", "<=", ">", ">=", "<>"]
+    supported_comparison_symbols = ["=", "<", "<=", ">", ">=", "<>"]
 
     # Functions as whitelist. The string "any" will allow any value
     supported_base_names: str | list[str] = "any"
 
     # Functions as a blacklist. See class 'prox' below for an example.
     base_name_value_limitations_per_context: dict | None = None
     modifier_type = "Generic"
 
     # Will probably be the same for all modifiers. But override if you want.
     default_context_set_for_modifier = "cql"
 
-    def __init__(self, base_name: str, operator: str | None = None, value: str | None = None, context_set: str | None = None):
+    def __init__(self, context_set: str | None = None, base_name: str = None, comparison_symbol: str | None = None, value: str | None = None):
+        if not base_name:
+            raise ValueError("You must include a base name.")
         self.base_name = base_name
         self.context_set = context_set
 
-        if operator and not value:
+        if comparison_symbol and not value:
             raise ValueError(
-                "If you include an operator, you must include a value.")
-        if value and not operator:
+                "If you include an comparison_symbol, you must include a value.")
+        if value and not comparison_symbol:
             raise ValueError(
-                "If you include a value, you must include an operator.")
-        if operator and operator not in self.supported_operators:
-            raise ValueError(f"Operator '{operator}' is not supported.")
-        self.operator = operator
+                "If you include a value, you must include an comparison_symbol.")
+        if comparison_symbol and comparison_symbol not in self.supported_comparison_symbols:
+            raise ValueError(f"Operator '{comparison_symbol}' is not supported.")
+        self.comparison_symbol = comparison_symbol
         self.value = value
 
         self._validate_base_name(
             base_name, self.supported_base_names, self.modifier_type)
-        if operator != None:
-            self._validate_operator(operator, self.supported_operators)
+        if comparison_symbol != None:
+            self._validate_comparison_symbol(comparison_symbol, self.supported_comparison_symbols)
 
     def format(self):
         return self._format()
 
     def _format(self, **kwargs) -> str:
         formatted_modifier = "/"
         if self.context_set:
             formatted_modifier += f'{self.context_set}.'
 
         formatted_modifier += f'{self.base_name}'
 
-        if self.operator and self.value:
-            formatted_modifier += f'{self.operator}"{self.value}"'
+        if self.comparison_symbol and self.value:
+            formatted_modifier += f'{self.comparison_symbol}"{self.value}"'
 
         return formatted_modifier
 
     @staticmethod
     def format_modifier_array(modifiers):
         """Returns formatted modifiers."""
         formatted_modifiers = ''
         if modifiers:
-            for boolean_operator_modifier in modifiers:
-                formatted_modifiers += f'{boolean_operator_modifier.format()}%20'
+            for boolean_comparison_symbol_modifier in modifiers:
+                formatted_modifiers += f'{boolean_comparison_symbol_modifier.format()}%20'
         return formatted_modifiers
 
     def validate(self, sru_configuration):
 
         context_set_to_check = self.context_set
         if context_set_to_check is None:
             context_set_to_check = self.default_context_set_for_modifier
@@ -75,17 +77,17 @@
             SRUValidator.validate_context_set(sru_configuration, self.context_set)
 
         if self.value != None:
             self._check_if_value_allowed_for_base_name_in_context_set(
                 context_set_to_check, self.base_name, self.value, self.base_name_value_limitations_per_context)
 
     @staticmethod
-    def _validate_operator(operator, supported_operators):
-        if operator not in supported_operators:
-            raise ValueError(f"Operator '{operator}' is not supported.")
+    def _validate_comparison_symbol(comparison_symbol, supported_comparison_symbols):
+        if comparison_symbol not in supported_comparison_symbols:
+            raise ValueError(f"Operator '{comparison_symbol}' is not supported.")
 
     @staticmethod
     def _validate_base_name(base_name: str, supported_base_names: str | list[str], modifier_type):
         if supported_base_names != "any":
             if base_name not in supported_base_names:
                 raise ValueError(
                     f"Base name '{base_name}' is not valid for modifier type '{modifier_type}.'")
```

### Comparing `sru_queryer-1.0.3/src/sru_queryer/_base/_query.py` & `sru_queryer-2.0.0/src/sru_queryer/_base/_search_retrieve.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,71 @@
 from __future__ import annotations
-from requests import Request, PreparedRequest
+from requests import Request
 
-from ._search_index_config import IndexQuery
-from ._cql_literal import LITERAL
+from ._search_clause import SearchClause
+from ._raw_cql import RawCQL
 from ._cql_boolean_operators import CQLBooleanOperatorBase
 from ._sru_configuration import SRUConfiguration
 from ._sru_validator import SRUValidator
 from ._sru_aux_formatter import SRUAuxiliaryFormatter
 from ._sort_key import SortKey
 
-class Query:
+class SearchRetrieve:
 
-    def __init__(self, sru_configuration: SRUConfiguration, index_search: IndexQuery | CQLBooleanOperatorBase | LITERAL, start_record: int | None = None, maximum_records: int | None = None, record_schema: str | None = None, sort_queries: list[dict] | list[SortKey] | None = None, record_packing: str | None = None):
+    def __init__(self, sru_configuration: SRUConfiguration, cql_query: SearchClause | CQLBooleanOperatorBase | RawCQL, start_record: int | None = None, maximum_records: int | None = None, record_schema: str | None = None, sort_queries: list[dict] | list[SortKey] | None = None, record_packing: str | None = None):
         self.sru_configuration = sru_configuration
-        self.index_search = index_search
+        self.cql_query = cql_query
         self.start_record = start_record
         self.maximum_records = maximum_records
         self.record_schema = record_schema
         self.record_packing = record_packing
 
         if sru_configuration.sru_version == "1.2":
             if sort_queries and isinstance(sort_queries[0], SortKey):
                 raise ValueError("You cannot use SortKeys with SRU version 1.2. Please see documentation on constructing a SortBy request.")
         if sru_configuration.sru_version == "1.1":
             if sort_queries and not isinstance(sort_queries[0], SortKey):
                 raise ValueError("You must use SortKeys for sorting with SRU version 1.1. Please see documentation on SortKey objects.")
         self.sort_queries = sort_queries
 
     def validate(self):
-        """Validates the query. 
-        Keep in mind that not all facets of the query are validated."""
+        """Validates the searchRetrieve request. 
+        Keep in mind that not all facets of the request are validated."""
+
+        SRUValidator.validate_defaults(self.sru_configuration)
 
         SRUValidator.validate_base_query(self.sru_configuration,
             self.start_record, self.maximum_records, self.record_schema, self.record_packing)
 
-        self.index_search.validate(self.sru_configuration)
+        self.cql_query.validate(self.sru_configuration)
 
         SRUValidator.validate_sort(self.sru_configuration, self.sort_queries, self.record_schema)
 
-    def construct_request(self) -> PreparedRequest:
+    def construct_request(self) -> Request:
         """Constructs the searchRetrieve request.
 
         Constructs the searchRetrieve request, including the base request, CQL query, and sortBy.
 
-        If you added a username and password when initializing the SRUUtil, it will be added to the
+        If you added a username and password when initializing SRUQueryer, it will be added to the
         headers of the request using the 'Basic access authentication' protocol.
 
-        Returns a PreparedRequest object. You can execute it using an instance of requests.Session:\n
+        Returns a Request object. You can execute it using an instance of requests.Session:\n
+            request = request.prepare()\n
             s = requests.Session()\n
             response = s.send(request)\n"""
         search_retrieve_query = SRUAuxiliaryFormatter.format_base_search_retrieve_query(self.sru_configuration,
             self.start_record, self.maximum_records, self.record_schema, self.record_packing)
 
-        if isinstance(self.index_search, IndexQuery) and not (self.index_search.get_index_name() and self.index_search.get_operation()):
-            # If it's just a single value (search term) as the query, without anything else, append an equals sign.
-            search_retrieve_query += "="
-        search_retrieve_query += self.index_search.format()
+        # if isinstance(self.cql_query, SearchClause) and not (self.cql_query.get_index_name() and self.cql_query.get_relation()):
+        #     # If it's just a single value (search term) as the query, without anything else, append an equals sign.
+        #     search_retrieve_query += "="
+        # This ^ caused the query to fail. I'm not sure why I put it here, but I'm leaving it here just in case.
+        search_retrieve_query += self.cql_query.format()
 
         search_retrieve_query += SRUAuxiliaryFormatter.format_sort_query(self.sort_queries)
 
         # Create the actual request object
         request = Request("GET", search_retrieve_query)
         if self.sru_configuration.username and self.sru_configuration.password:
             request.headers["Authorization"] = SRUAuxiliaryFormatter.format_basic_access_authentication_header_payload(self.sru_configuration.username, self.sru_configuration.password)
 
-        request = request.prepare()
-
         return request
```

### Comparing `sru_queryer-1.0.3/src/sru_queryer/_base/_search_index_config.py` & `sru_queryer-2.0.0/src/sru_queryer/_base/_search_clause.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,97 +1,94 @@
 from __future__ import annotations
 
 from ._sru_configuration import SRUConfiguration
 from ._sru_validator import SRUValidator
 from ._cql_modifiers import CQLModifierBase, RelationModifier
 
-class IndexQuery:
-    """A query of an index.
+class SearchClause:
+    """A CQL clause.
 
-    Supports validation of context set, index_name, operation, and whether 
-    or not an empty string is allowed as a value for a particular index.
+    Supports validation of context set, index_name, relation, and whether 
+    or not an empty string is allowed as a search_term for a particular index.
 
-    To create a valid query, you must use:\n
-        a value,\n
-        index_name + operation + value,\n
-        OR context_set + index_name + operation + value.\n
+    To create a valid search clause, you must use:\n
+        a search_term,\n
+        index_name + relation + search_term,\n
+        OR context_set + index_name + relation + search_term.\n
 
-    Modifiers will only be included if there's an operation.
+    Modifiers will only be included if there's an relation.
         """
 
-    def __init__(self, context_set: str | None = None, index_name: str | None = None, operation: str | None = None, value: str | None = None, modifiers: list[RelationModifier] | None = None):
+    def __init__(self, context_set: str | None = None, index_name: str | None = None, relation: str | None = None, search_term: str | None = None, modifiers: list[RelationModifier] | None = None):
         self._context_set: str = context_set
         self._index_name: str = index_name
-        self._operation: str = operation
-        self._value: str = value
+        self._relation: str = relation
+        self._search_term: str = search_term
         self._modifiers = modifiers
 
-        value_exists = value != None
-        if not value_exists:
-            raise ValueError("You must provide a search term (value)")
+        search_term_exists = search_term != None
+        if not search_term_exists:
+            raise ValueError("You must provide a search term (search_term)")
 
-        if index_name and not operation:
+        if index_name and not relation:
             raise ValueError(
-                "If you include an index, you must include an operation")
-        if operation and not index_name:
+                "If you include an index, you must include an relation")
+        if relation and not index_name:
             raise ValueError(
-                "If you include an operation, you must include an index")
+                "If you include an relation, you must include an index")
         if context_set and not index_name:
             raise ValueError(
                 "If you have a context set, you must include an index.")
 
     def get_index_name(self):
         return self._index_name
 
-    def get_operation(self):
-        return self._operation
+    def get_relation(self):
+        return self._relation
 
     def format(self):
         return self._format()
 
-    def _format_operation(self) -> str:
-        """Formats the relational operation
+    def _format_relation(self) -> str:
+        """Formats the relational relation
 
-        For non-word relational operators (==, >, <>, etc), there should be no spacing, E.G.:\n
-            ==\n
-        For relational operators that are words (E.G., 'any'), append a space before and AFTER IF THERE'S NO MODIFIERS:\n
+        append a space before and AFTER IF there's no modifiers:\n
             %20any%20 (no modifiers)\n
             %20and    (with modifiers)\n
         """
-        formatted_operation = ""
+        formatted_relation = ""
 
-        if self._operation:
-            formatted_operation = self._operation
-            if formatted_operation in ["all"]:
-                formatted_operation = f'%20{formatted_operation}'
-
-                # add padding for the operations that are words
-                if not self._modifiers:
-                    formatted_operation += "%20"
+        if self._relation:
+            formatted_relation = self._relation
+            formatted_relation = f'%20{formatted_relation}'
 
-        return formatted_operation
+            # add padding for the relations that are words
+            if not self._modifiers:
+                formatted_relation += "%20"
+
+        return formatted_relation
 
     def _format(self, **kwargs):
-        formatted_index_query = ""
+        formatted_search_clause = ""
 
         if self._context_set:
-            formatted_index_query += f'{self._context_set}.'
+            formatted_search_clause += f'{self._context_set}.'
 
         if self._index_name:
-            formatted_index_query += f'{self._index_name}{self._format_operation()}'
+            formatted_search_clause += f'{self._index_name}{self._format_relation()}'
 
         # Format the modifiers
-        formatted_index_query += CQLModifierBase.format_modifier_array(
+        formatted_search_clause += CQLModifierBase.format_modifier_array(
             self._modifiers)
 
-        # The index value will always be added
-        formatted_index_query += f'"{self._value}"'
+        # The index search_term will always be added
+        formatted_search_clause += f'"{self._search_term}"'
 
-        return formatted_index_query
+        return formatted_search_clause
 
     def validate(self, sru_configuration: SRUConfiguration):
         SRUValidator.validate_cql(sru_configuration, self._context_set,
-            self._index_name, self._operation, self._value)
+            self._index_name, self._relation, self._search_term)
 
         if self._modifiers:
             for modifier in self._modifiers:
                 modifier.validate(sru_configuration)
```

### Comparing `sru_queryer-1.0.3/src/sru_queryer/_base/_sort_key.py` & `sru_queryer-2.0.0/src/sru_queryer/_base/_sort_key.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.3/src/sru_queryer/_base/_sru_aux_formatter.py` & `sru_queryer-2.0.0/src/sru_queryer/_base/_sru_aux_formatter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,20 @@
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
 from base64 import b64encode
 
 from ._sru_configuration import SRUConfiguration
 from ._sort_key import SortKey
 
-class SRUAuxiliaryFormatterAbstract(ABC):
 
-    @staticmethod
-    @abstractmethod
-    def format_available_indexes(available_context_sets_and_indexes: dict, filename: str | None = None, print_to_console: bool = True):
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def format_base_explain_query(base_explain_url: str, version: str) -> str:
-        pass
-    
-    @staticmethod
-    @abstractmethod
-    def format_base_search_retrieve_query(sru_configuration: SRUConfiguration, start_record: int | None = None, maximum_records: int | None = None, record_schema: str | None = None, record_packing: str |  None = None) -> str:
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def format_sort_query(sort_queries: list[dict] | list[SortKey] | None) -> str:
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def format_basic_access_authentication_header_payload(username: str, password: str):
-        pass
-
-
-class SRUAuxiliaryFormatter(SRUAuxiliaryFormatterAbstract):
+class SRUAuxiliaryFormatter():
+    """
+    This class handles formatting that isn't handled by Objects. For example, the SortKeys abstraction is a class and can
+    self-format, while sort queries are not their own class. So, this class will format them. 
+    """
 
     @staticmethod
     def format_available_indexes(available_context_sets_and_indexes: dict, filename: str | None = None, print_to_console: bool = True):
         formatted_string = ""
 
         for context_set in available_context_sets_and_indexes:
             formatted_string += f"------INDEX SET: {context_set}------\n\n"
@@ -49,36 +25,37 @@
 
                 if index_data["id"]:
                     formatted_string += f"     Index ID:               | {index_data['id']}\n"
 
                 formatted_string += f"     Index Set:              | {context_set}\n"
                 formatted_string += f"     Index Code:             | {index_code}\n"
 
-                if index_data["supported_operations"]:
-                    formatted_string += f"     Supported Operations:   | {index_data['supported_operations'].__str__()}\n"
+                if index_data["supported_relations"]:
+                    formatted_string += f"     Supported Operations:   | {index_data['supported_relations'].__str__()}\n"
 
                 sort = index_data['sort']
                 if sort != None:
                     formatted_string += f"     Sortable:               | {sort}\n\n"
                 formatted_string += "\n"
 
         if print_to_console:
             print(formatted_string)
 
         if filename:
             with open(filename, "w") as f:
                 f.write(formatted_string)
 
     @staticmethod
-    def format_base_explain_query(base_explain_url: str, version: str) -> str:
-        return f'{base_explain_url}?version={str(version)}&operation=explain'
+    def format_base_explain_query(server_url: str, version: str) -> str:
+        url = f'{server_url}?version={str(version)}&operation=explain'
+        return url
     
     @staticmethod
     def format_base_search_retrieve_query(sru_configuration: SRUConfiguration, start_record: int | None = None, maximum_records: int | None = None, record_schema: str | None = None, record_packing: str | None = None) -> str:
-        search_retrieve_base_query = f"{sru_configuration.search_retrieve_url}?version={sru_configuration.sru_version}&operation=searchRetrieve"
+        search_retrieve_base_query = f"{sru_configuration.server_url}?version={sru_configuration.sru_version}&operation=searchRetrieve"
 
         record_schema_to_include = record_schema
         if not record_schema:
             if sru_configuration.default_record_schema:
                 record_schema_to_include = sru_configuration.default_record_schema
         if record_schema_to_include:
             search_retrieve_base_query += f'&recordSchema={record_schema_to_include}'
```

### Comparing `sru_queryer-1.0.3/src/sru_queryer/_base/_sru_configuration.py` & `sru_queryer-2.0.0/src/sru_queryer/_base/_sru_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,13 +18,12 @@
         self.default_records_returned: int | None = None
         self.max_records_supported: int | None = None
 
         # Hard-coded limits from documentation
         self.available_record_packing_values = ["string", "xml"]
 
         # Values set by user
-        self.explain_url: str = None
-        self.search_retrieve_url: str = None
+        self.server_url: str = None
         self.sru_version: str = None
         self.username: str | None = None
         self.password: str | None = None
         self.disable_validation_for_cql_defaults: bool = False
```

### Comparing `sru_queryer-1.0.3/src/sru_queryer/_base/_sru_explain_xml_parser.py` & `sru_queryer-2.0.0/src/sru_queryer/_base/_sru_explain_auto_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,293 +1,254 @@
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
-import sys
-
 from ._sru_configuration import SRUConfiguration
+from ._exceptions import NoExplainResponseException
 
-class SRUExplainXMLParserAbstract(ABC):
-
-    def __init__(self, sru_explain_dict: dict, driver: dict):
-        self.sru_explain_dict = sru_explain_dict
-        self.driver = driver
-
-    @abstractmethod
-    def get_sru_configuration_from_explain_response(self) -> SRUConfiguration:
-        pass
+generic_driver = {
+    "name": "Generic Driver for auto-detect",
+    "version": {
+        "location": ["explainResponse", "version"]
+    },
+    "index": {
+        'location': ["explainResponse", "record", "recordData", "explain", "index", "index"],
+        # Relative to the index info location above
+        "sortLocation": ["@sort"],
+        "idLocation": ["@id"], 
+        "titleLocation": ["title"],
+        "supportedRelationsLocation": ["configInfo", "supports"],
+        # Below is relative to map location (hard-coded to ...index["map"])
+        "nameLocation": ["name", "#text"],
+        "setLocation": ["name", "@set"]
+    },
+    "schema": {
+        "location": ["explainResponse", "record", "recordData", "explain", "schemaInfo", "schema"]
+    },
+    "defaults": {
+        "location": ["explainResponse", "record", "recordData", "explain", "configInfo", "default"]
+    },
+    "settings": {
+        "location": ["explainResponse", "record", "recordData", "explain", "configInfo", "setting"]
+    },
+    "supports": {
+        "location": ["explainResponse", "record", "recordData", "explain", "configInfo", "supports"]
+    }
+}
 
-class SRUExplainXMLParser(SRUExplainXMLParserAbstract):
+class SRUExplainAutoParser():
 
-    def __init__(self, sru_explain_dict: dict, driver: dict):
+    def __init__(self, sru_explain_dict: dict):
         self.sru_explain_dict = sru_explain_dict
-        self.driver = driver
-    
-    def get_sru_configuration_from_explain_response(self) -> SRUConfiguration:
-        sru_configuration = SRUConfiguration()
-
-        raw_index_info = self._parse_raw_index_info_from_xml()
-        sru_configuration.available_context_sets_and_indexes = self._parse_available_context_sets_and_index_info(raw_index_info)
-        
-        raw_schema_info = self._parse_raw_schema_info_from_xml()
-        sru_configuration.available_record_schemas = self._parse_schema_info(raw_schema_info)
-
-        raw_config_info = self._parse_raw_config_info_from_xml()
-        config_info = self._parse_config_info(raw_config_info)
-
-        if config_info:
-            sru_configuration.supported_relation_modifiers = config_info["supported_relation_modifiers"]
-            sru_configuration.default_context_set = config_info["default_context_set"]
-            sru_configuration.default_index = config_info["default_index"]
-            sru_configuration.default_relation = config_info["default_relation"]
-            sru_configuration.default_record_schema = config_info["default_record_schema"]
-            sru_configuration.default_sort_schema = config_info["default_sort_schema"]
-            sru_configuration.default_records_returned = config_info["default_records_returned"]
-            sru_configuration.max_records_supported = config_info["max_records_supported"]
+        self.sru_config: SRUConfiguration = None
 
-        return sru_configuration
-
-    def _parse_raw_index_info_from_xml(self) -> list[dict] | None:
-        path_to_index_info = self.driver["indexInfo"]["indexInfoLocation"]
-        
-        return self._pull_data_from_dict(self.sru_explain_dict, path_to_index_info)
-    
-    def _parse_raw_schema_info_from_xml(self) -> list[dict] | None:
-        path_to_schema_info = self.driver["schemaInfo"]["schemaInfoLocation"]
-        
-        return self._pull_data_from_dict(self.sru_explain_dict, path_to_schema_info)
+    def get_sru_configuration_from_explain_response(self) -> SRUConfiguration:
 
-    def _parse_raw_config_info_from_xml(self) -> dict | None:
-        path_to_config_info = self.driver["configInfo"]["configInfoLocation"]
-
-        return self._pull_data_from_dict(self.sru_explain_dict, path_to_config_info)
-    
-    def _parse_available_context_sets_and_index_info(self, raw_index_info) -> dict | None:
-        if raw_index_info is None:
-            return None
-
-        available_context_sets_and_indexes = {}
-        driver_base = self.driver["indexInfo"]
-
-        try:
-            path_to_sort = driver_base["sortLocation"]
-            path_to_id = driver_base["idLocation"]
-            path_to_title = driver_base["titleLocation"]
-            path_to_supported_operations = driver_base["supportedOperationsLocation"]
-            path_to_name = driver_base["nameLocation"]
-            path_to_set = driver_base["setLocation"]
-        except KeyError:
-            sys.exit(f"One or more indexInfo paths for driver '{self.driver}' are not specified.\nPlease add them to config.py.")
-
-        # Checks if sort info is included in the index info.
-        sort_information_included_in_index_info = self._evaluate_if_sort_info_included_in_index_info(raw_index_info, path_to_sort)
-
-        for raw_index in raw_index_info:
-            id = self._pull_data_from_dict(raw_index, path_to_id)
-            title = self._pull_data_from_dict(raw_index, path_to_title)
-            
-            raw_supported_operations: list = self._pull_data_from_dict(raw_index, path_to_supported_operations, throw_error_if_not_found=False)
-            empty_term_supported, supported_operations = self._parse_raw_supported_operations(raw_supported_operations)
-
-            sort = self._parse_sort_info(raw_index, path_to_sort, sort_information_included_in_index_info)
-
-            maps = raw_index["map"]
-            if isinstance(maps, dict):
-                maps = [maps]
-
-            for map in maps:
-                name = self._remove_set_from_index_name(self._pull_data_from_dict(map, path_to_name))
-                set = self._pull_data_from_dict(map, path_to_set)
+        # Raise exception if the explainResponse can't be parsed.
+        # Check validity - invalid ones will not contain explainResponse 
+        contains_explain_response = self._find_property_value(self.sru_explain_dict, ["explainResponse"])
+        if not contains_explain_response:
+            raise NoExplainResponseException("ExplainResponse could not be parsed", self.sru_explain_dict)
+
+        self.sru_config = SRUConfiguration()
+        self.sru_config.sru_version = self._find_property_value(self.sru_explain_dict, generic_driver["version"]["location"])
+        self._parse_context_set_and_index_info()
+        self._parse_config_info()
+        self._parse_schema_info()
+       
+        return self.sru_config
+    
+    def _parse_context_set_and_index_info(self):
+        """Parses the context set and index information from the explainResponse.
+        
+        Relies on the sru_explain_dict and sru_config property."""
+        index_information = self._find_property_value(self.sru_explain_dict, generic_driver["index"]["location"])
+        self.sru_config.available_context_sets_and_indexes = {}
+        for index in index_information:
+            id = self._find_property_value(index, generic_driver["index"]["idLocation"])
+            title = self._find_property_value(index, generic_driver["index"]["titleLocation"])
+            empty_term_supported, supported_relations = self._get_supported_relations_for_index(index)
+
+            # Get the sort information
+            sortable = None
+            sort_info_included_in_indexes = self._evaluate_if_sort_info_included_in_index_info()
+            if sort_info_included_in_indexes:
+                sort = self._find_property_value(index, generic_driver["index"]["sortLocation"])
+                if sort == "true":
+                    sortable = True
+                else:
+                    sortable = False
+
+
+            context_sets_that_include_this_index = index["map"]
+            if isinstance(context_sets_that_include_this_index, dict):
+                # A few indexes are part of multiple context sets, so
+                # I'll just loop over them. This means turning dicts into
+                # a list. 
+                context_sets_that_include_this_index = [context_sets_that_include_this_index]
+
+            for context_set in context_sets_that_include_this_index:
+                name = self._remove_set_from_index_name(context_set["name"]["#text"])
+                set = context_set["name"]["@set"]
 
                 # If the set is not in the index and config info, add it
-                if set not in available_context_sets_and_indexes:
-                    available_context_sets_and_indexes[set] = {}
+                if set not in self.sru_config.available_context_sets_and_indexes:
+                    self.sru_config.available_context_sets_and_indexes[set] = {}
 
                 # Add the index to its set.
-                index_config = self._generate_index_config(title, id=id, sort=sort, supported_operations=supported_operations, empty_term_supported=empty_term_supported)
-                available_context_sets_and_indexes[set][name] = index_config
+                index_config = self._generate_index_config(title, id=id, sort=sortable, supported_relations=supported_relations, empty_term_supported=empty_term_supported)
+                self.sru_config.available_context_sets_and_indexes[set][name] = index_config
 
-        return available_context_sets_and_indexes
-    
-    def _parse_config_info(self, raw_config_info) -> dict | None:
-        if raw_config_info is None:
-            return None
-        
-        driver_base = self.driver["configInfo"]
-
-        try:
-            path_to_defaults = driver_base["defaultsLocation"]
-            path_to_settings = driver_base["settingsLocation"]
-            path_to_supports = driver_base["supportsLocation"]
-        except KeyError:
-            sys.exit(f"One or more configInfo paths for driver '{self.driver.name}' are not specified.\nPlease add them to config.py.")
-
-        parsed_config_info = {
-            "default_context_set": None,
-            "default_index": None,
-            "default_relation": None,
-            "default_record_schema": None,
-            "default_sort_schema": None,
-            "default_records_returned": None,
-            "max_records_supported": None,
-            "supported_relation_modifiers": []
-        }
+    def _parse_config_info(self):
+        """Parses the configuration info from the explainResponse."""
 
-        default_information = self._pull_data_from_dict(raw_config_info, path_to_defaults)
+        default_information = self._find_property_value(self.sru_explain_dict, generic_driver["defaults"]["location"])
         if default_information:
             if isinstance(default_information, dict):
                 default_information = [default_information]
 
             for default in default_information:
                 def_type = default["@type"]
                 value = default["#text"]
                 if def_type == "numberOfRecords":
-                    parsed_config_info["default_records_returned"] = int(value)
+                    self.sru_config.default_records_returned = int(value)
                 elif def_type == "contextSet":
-                    parsed_config_info["default_context_set"] = value
+                    self.sru_config.default_context_set = value
                 elif def_type == "index":
-                    parsed_config_info["default_index"] = value
+                    self.sru_config.default_index = value
                 elif def_type == "relation":
-                    parsed_config_info["default_relation"] = value
+                    self.sru_config.default_relation = value
                 elif def_type == "retrieveSchema":
-                    parsed_config_info["default_record_schema"] = value
+                    self.sru_config.default_record_schema = value
                 elif def_type == "sortSchema":
-                    parsed_config_info["default_sort_schema"] = value
+                    self.sru_config.default_sort_schema = value
 
-        settings_information = self._pull_data_from_dict(raw_config_info, path_to_settings)
+        settings_information = self._find_property_value(self.sru_explain_dict, generic_driver["settings"]["location"])
         if settings_information:
             if isinstance(settings_information, dict):
                 settings_information = [settings_information]
 
             for setting in settings_information:
                 setting_name = setting["@type"]
                 value = setting["#text"]
 
                 if setting_name == "maximumRecords":
-                    parsed_config_info["max_records_supported"] = int(value)
+                    self.sru_config.max_records_supported = int(value)
 
-        supports_information = self._pull_data_from_dict(raw_config_info, path_to_supports)
+        supports_information = self._find_property_value(self.sru_explain_dict, generic_driver["supports"]["location"])
         if supports_information:
+            self.sru_config.supported_relation_modifiers = []
             if isinstance(supports_information, dict):
                 supports_information = [supports_information]
 
             for support_setting in supports_information:
-                support_type = support_setting["@type"]
+                if support_setting["@type"] == "relationModifier":
+                    self.sru_config.supported_relation_modifiers.append(support_setting["#text"])
 
-                if support_type == "relationModifier":
-                    value = support_setting["#text"]
-                    parsed_config_info["supported_relation_modifiers"].append(value)
 
-        return parsed_config_info
-    
-    def _parse_schema_info(self, raw_schema_info) -> dict | None :
-        if raw_schema_info is None:
-            return None
+    def _parse_schema_info(self):
+        """Parse the record schema information from the explainResponse.
+        
+        This will add a list of available schemas to sru_configuration.available_record_schemas.
         
+        It counts both the identifier and the official name of the schema as a available record schemas.
+        While this is technically duplication, they're both valid ways to write a schema in an SRU query.
+        I didn't know this until I had already defined the available_record_schemas as a simple list, and
+        didn't want to rip my program apart to fix this. So, for now, the record schemas are all duplicated
+        if they have identifiers so that validation will work with those identifier names."""
+        schema_information = self._find_property_value(self.sru_explain_dict, generic_driver["schema"]["location"])
         cleaned_record_schema_info: dict = {}
         
         # Turn dict to list so we can interate through it 
         # (just simplifies logic)
-        if isinstance(raw_schema_info, dict):
-            raw_schema_info = [raw_schema_info]
+        if isinstance(schema_information, dict):
+            schema_information = [schema_information]
 
-        for schema in raw_schema_info:
+        for schema in schema_information:
             sort = True
             if schema["@sort"] == "false":
                 sort = False
 
             schema_name = schema["@name"]
-            # The schema identifier can be used in place of the
-            # name in a query
-            alternate_schema_name = self._pull_data_from_dict(schema, ["@identifier"])
+            schema_identifier = schema["@identifier"]
 
             cleaned_record_schema_info[schema_name] = {
-                "sort": sort
+                "sort": sort,
+                "identifier": schema_identifier
             }
-
-            if alternate_schema_name:
-                cleaned_record_schema_info[alternate_schema_name] = {
-                    "sort": sort
-                }
         
-        return cleaned_record_schema_info
-    
+        self.sru_config.available_record_schemas = cleaned_record_schema_info
+
     @staticmethod
-    def _parse_sort_info(raw_index: dict, path_to_sort: list, sort_information_included_in_index_info: bool) -> bool:
-        """Parses whether an index can be sorted
-        
-        For any index, 'sort' will either be None, or 'true'. This is because when sort is 'false', the
-        sort information is not included.
-        
-        We need also need the boolean 'sort_information_included_in_index_info', as indexes in explainResponses that have
-        no sort information look the same as ones where sort=false (they both have no sort key). 
-        When a response DOES incude sort info on at least one index, we interpret missing sort info as meaning 
-        the index cannot be sorted. Else, we will include 'None,' which indicates that the information is not available.
-        
-        We also, of course, need to convert the string 'true' to Python's boolean 'True'"""
-        sort = SRUExplainXMLParser._pull_data_from_dict(raw_index, path_to_sort, throw_error_if_not_found=False)
-        if sort is None and sort_information_included_in_index_info:
-            sort = False
-        elif sort == "true":
-            sort = True
+    def _find_property_value(input_dict: dict, location: list[str]) -> any | None:
+        """This method takes a location in a dict and returns the value at that location.
+
+        The input 'location' is a list of strings that represents the dictionary path to the value
+        we want. 
+
+        It's designed to work with different namespaces, so it checks the keys of the dictionary
+        to see if any of them INCLUDE the term (rather than exact match). It will then use that
+        term.
+
+        If it finds nothing, it will return None. Else, it will return whatever it finds. 
+        """
+        data = input_dict
+        for path_segment in location:
+            # Get the available keys and try to find a match
+            keys = data.keys()
+            actual_key = None
+            for key in keys:
+                if path_segment in key:
+                    actual_key = key
+
+            if actual_key:
+                data = data[actual_key]
+            else:
+                return None
 
-        return sort
+        return data
     
-    @staticmethod
-    def _evaluate_if_sort_info_included_in_index_info(raw_index_info, path_to_sort) -> bool:
+    def _evaluate_if_sort_info_included_in_index_info(self) -> bool:
         sort_information_included_in_index_info = False
-        for index in raw_index_info:
-            sort_info = SRUExplainXMLParser._pull_data_from_dict(index, path_to_sort, throw_error_if_not_found=False)
+        for index in self._find_property_value(self.sru_explain_dict, generic_driver["index"]["location"]):
+            sort_info = self._find_property_value(index, generic_driver["index"]["sortLocation"])
             if sort_info != None:
                 sort_information_included_in_index_info = True
                 break
 
         return sort_information_included_in_index_info
-    
-    @staticmethod
-    def _parse_raw_supported_operations(raw_supported_operations, ):
-        supported_operations = []
-        empty_term_supported = None
-        if raw_supported_operations:
-            empty_term_supported = False
-            for operation in raw_supported_operations:
-                if operation["@type"] == "emptyTerm":
-                    empty_term_supported = True
-                elif operation["@type"] == "relation":
-                    supported_operations.append(operation["#text"])
-        
-        return empty_term_supported, supported_operations
         
-    @staticmethod
-    def _pull_data_from_dict(dict, path_to_data: list[str], throw_error_if_not_found: bool=True) -> dict | list | None:
-        """Given a dictionary and an array of property names, goes down the chain to
-        find the property you're looking for. Returns -1 if not found."""
-        if not path_to_data:
-            return None
-
-        data = dict
-        try:
-            for path_segment in path_to_data:
-                data = data[path_segment]
-        except KeyError as ke:
-            if throw_error_if_not_found:
-                raise ke
-            
-            return None
 
-        return data
-    
-    @staticmethod
-    def _generate_index_config(title: str, id: str | None = None, sort: bool | None = None, supported_operations: list[str] = None, empty_term_supported: bool | None = None) -> dict:
-        if supported_operations is None: 
-            supported_operations = []
+    def _get_supported_relations_for_index(self, index) -> tuple[bool, list[str]]:
+        """Get the relations supported by a CQL index.
+        
+        This takes a CQL index from the explainResponse after being parsed from xmltodict,
+        and returns whether empty terms are supported and the other terms that are supported"""
+        raw_supported_relations = self._find_property_value(index, generic_driver["index"]["supportedRelationsLocation"])
+
+        if not raw_supported_relations:
+            return None, None
+        
+        supported_relations: dict = []
+        empty_term_supported = False
+        for relation in raw_supported_relations:
+            if relation["@type"] == "emptyTerm":
+                empty_term_supported = True
+            elif relation["@type"] == "relation":
+                supported_relations.append(relation["#text"])
+
+        return empty_term_supported, supported_relations
+    
+    @staticmethod
+    def _generate_index_config(title: str, id: str | None = None, sort: bool | None = None, supported_relations: list[str] = None, empty_term_supported: bool | None = None) -> dict:
+        if supported_relations is None: 
+            supported_relations = []
         index_config_dict = {
             "id": id,
             "title": title,
             "sort": sort,
-            "supported_operations": supported_operations,
+            "supported_relations": supported_relations,
             "empty_term_supported": empty_term_supported
         }
 
         return index_config_dict
     
     @staticmethod
     def _remove_set_from_index_name(index_name: str) -> str:
```

### Comparing `sru_queryer-1.0.3/src/sru_queryer/_base/_sru_validator.py` & `sru_queryer-2.0.0/src/sru_queryer/_base/_sru_validator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,43 @@
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
-
 from ._sru_configuration import SRUConfiguration
 from ._sort_key import SortKey
 
-class SRUValidatorAbstract(ABC):
-    @staticmethod
-    @abstractmethod
-    def validate_defaults(sru_configuration: SRUConfiguration, default_context_set: str | None, default_index: str | None, default_relation: str | None, default_record_schema: str | None, default_sort_schema: str | None):
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def validate_cql(sru_configuration: SRUConfiguration, context_set: str | None = None, index_name: str | None = None, relation: str | None = None, value: str | None = None, evaluate_can_sort: bool = False) -> None:
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def validate_base_query(sru_configuration: SRUConfiguration, start_record: str | None, maximum_record: str | None, record_schema: str | None, record_packing: str | None) -> None:
-        pass 
-
-    @staticmethod
-    @abstractmethod
-    def validate_context_set(sru_configuration: SRUConfiguration, context_set: str) -> None:
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def validate_sort(sru_configuration: SRUConfiguration, sort_queries: list[dict] | list[SortKey], record_schema: str | None = None) -> None:
-        pass
-
-class SRUValidator(SRUValidatorAbstract):
+class SRUValidator():
+    """Handles most validation tasks. Some things are validated when they are initialized, however."""
 
     @staticmethod
     def validate_defaults(sru_configuration: SRUConfiguration):
         # Validate default index, context set, and relation
-        information_exists_for_cql_defaults = sru_configuration.default_context_set != None
-        if not sru_configuration.disable_validation_for_cql_defaults and information_exists_for_cql_defaults:
-            SRUValidator.validate_cql(sru_configuration, sru_configuration.default_context_set, sru_configuration.default_index, sru_configuration.default_relation)
+        if not sru_configuration.disable_validation_for_cql_defaults:
+            if sru_configuration.default_context_set and sru_configuration.default_index:
+                SRUValidator.validate_cql(sru_configuration, sru_configuration.default_context_set, sru_configuration.default_index, sru_configuration.default_relation)
+            elif sru_configuration.default_context_set and not sru_configuration.default_index:
+                SRUValidator.validate_context_set(sru_configuration, sru_configuration.default_context_set)
 
         # Validate default record schema
-        record_schema_valid = SRUValidator._validate_record_schema(sru_configuration.available_record_schemas, sru_configuration.default_record_schema)
-        if not record_schema_valid:
-            raise ValueError(f"Record schema '{sru_configuration.default_record_schema}' is not available.")
+        if sru_configuration.default_record_schema:
+            record_schema_valid = SRUValidator._validate_record_schema(sru_configuration.available_record_schemas, sru_configuration.default_record_schema)
+            if not record_schema_valid:
+                raise ValueError(f"Record schema '{sru_configuration.default_record_schema}' is not available.")
         
-        # Validate default sort schema
+        # If there is a default sort schema, check that it exists and that it can sort
         default_sort_schema = sru_configuration.default_sort_schema
-        sort_schema_valid = SRUValidator._validate_record_schema(sru_configuration.available_record_schemas, default_sort_schema)
-        if not sort_schema_valid:
-            raise ValueError(f"Sort schema '{default_sort_schema}' is not available.")
-        
         if default_sort_schema:
+            sort_schema_valid = SRUValidator._validate_record_schema(sru_configuration.available_record_schemas, default_sort_schema)
+            if not sort_schema_valid:
+                raise ValueError(f"Sort schema '{default_sort_schema}' is not available.")
             sort_schema_info = sru_configuration.available_record_schemas[default_sort_schema]
             if sort_schema_info["sort"] is False:
                 raise ValueError(f"Schema {default_sort_schema} cannot sort.")
 
     
     @staticmethod
-    def validate_cql(sru_configuration: SRUConfiguration, context_set: str | None = None, index_name: str | None = None, relation: str | None = None, value: str | None = None, evaluate_can_sort: bool = False) -> None:
+    def validate_cql(sru_configuration: SRUConfiguration, context_set: str | None = None, index_name: str | None = None, relation: str | None = None, search_term: str | None = None, evaluate_can_sort: bool = False) -> None:
         no_context_set = context_set is None
         no_index = index_name is None
         no_relation = relation is None
         no_default_context_set = sru_configuration.default_context_set is None
         no_default_index = sru_configuration.default_index is None
         no_default_relation = sru_configuration.default_relation is None
         validation_for_defaults_enabled = sru_configuration.disable_validation_for_cql_defaults is False
@@ -71,20 +46,19 @@
         index_to_evaluate = index_name
         relation_to_evaluate = relation
 
         no_context_set_info = no_context_set and no_default_context_set
         no_index_info = no_index and no_default_index
         no_relation_info = no_relation and no_default_relation
 
-        if (no_context_set_info or no_index_info) and validation_for_defaults_enabled:
-            if no_context_set_info:
-                raise ValueError("Cannot validate context set 'None'; ensure you have set a default context set or have disabled validation for cql defaults.")
+        if no_context_set_info and validation_for_defaults_enabled:
+            raise ValueError("Cannot validate context set 'None'; ensure you have set a default context set or have disabled validation for cql defaults.")
             
-            if no_index_info:
-                raise ValueError("Cannot validate index 'None'; ensure you have set a default index or have disabled validation for cql defaults.")
+        if no_index_info and validation_for_defaults_enabled:
+            raise ValueError("Cannot validate index 'None'; ensure you have set a default index or have disabled validation for cql defaults.")
 
         if no_context_set:
             if not validation_for_defaults_enabled:
                 return
             context_set_to_evaluate = sru_configuration.default_context_set
         SRUValidator.validate_context_set(sru_configuration, context_set_to_evaluate)
         
@@ -100,40 +74,40 @@
         # Evaluate whether the index can sort.
         if evaluate_can_sort:
             if index_info["sort"] is False:
                 raise ValueError(f"Index '{index_to_evaluate}' in context set '{context_set_to_evaluate}' does not support sorting.")
             return
         
         # Evaluate the relation, if specified
-        relation_info_included_in_index = index_info["supported_operations"]
+        relation_info_included_in_index = index_info["supported_relations"]
         if relation_info_included_in_index and no_relation_info:
             raise ValueError("Cannot validate relation 'None'; ensure you have set a default relation or have disabled validation for cql defaults.")
             
         relation_is_valid = SRUValidator._validate_relation(relation_to_evaluate, index_info)
         if not relation_is_valid:
             raise ValueError(f"Relation '{relation_to_evaluate}' is not supported on index '{index_to_evaluate}' in context set '{context_set_to_evaluate}'")
             
-        # Evaluate the value. This checks for 'empty term supported'. So if the value is an empty 
+        # Evaluate the search_term. This checks for 'empty term supported'. So if the search_term is an empty 
         # string and empty term is not supported, this will raise an error. 
-        value_is_valid = SRUValidator._validate_value(value, index_info)
-        if not value_is_valid:
+        search_term_is_valid = SRUValidator._validate_search_term(search_term, index_info)
+        if not search_term_is_valid:
             raise ValueError(f"Index '{index_to_evaluate}' in context set '{context_set_to_evaluate}' does not support empty terms.")
                 
             
     @staticmethod
     def validate_base_query(sru_configuration: SRUConfiguration, start_record: str | None, maximum_record: str | None, record_schema: str | None, record_packing: str | None) -> None:
         if start_record and start_record < 1:
             raise ValueError("Start record must be greater than 0.")
 
         if maximum_record and sru_configuration.max_records_supported:
             if maximum_record > sru_configuration.max_records_supported:
                 raise ValueError(f"Maximum records returned must be less than {str(sru_configuration.max_records_supported)}.") 
         
         if record_schema:
-            if record_schema not in sru_configuration.available_record_schemas:
+            if SRUValidator._validate_record_schema(sru_configuration.available_record_schemas, record_schema) == False:
                 raise ValueError(f"Record schema '{record_schema}' is not available.")
             
         if record_packing:
             if record_packing not in sru_configuration.available_record_packing_values:
                 raise ValueError(f"Record packing value '{record_packing}' is not available.")
 
     @staticmethod
@@ -152,36 +126,38 @@
             return
         else:
             SRUValidator._validate_1_2_sort(sru_configuration, sort_queries)
 
 
     @staticmethod
     def _validate_record_schema(available_record_schemas: dict, schema: str) -> bool:
-        if schema:
-            if schema not in available_record_schemas:
-                return False
-        return True
+        for schema_name in available_record_schemas.keys():
+            if schema == schema_name:
+                return True
+            if schema == available_record_schemas[schema_name]["identifier"]:
+                raise ValueError(f"You cannot use the schema identifier in the schema argument. Please use '{schema_name}' instead of '{available_record_schemas[schema_name]["identifier"]}'.")
+        return False
     
     @staticmethod
     def _validate_relation(relation: str | None, index_info: dict) -> bool:
         if relation != None:
-            relation_information_included_in_index = index_info["supported_operations"]
+            relation_information_included_in_index = index_info["supported_relations"]
             
             if relation_information_included_in_index:
-                if relation not in index_info["supported_operations"]:
+                if relation not in index_info["supported_relations"]:
                     return False
         return True
     
     @staticmethod
-    def _validate_value(value: str | None, index_info: dict) -> bool:
-        if value != None:
-            index_info_contains_value_info = index_info["empty_term_supported"] != None
+    def _validate_search_term(search_term: str | None, index_info: dict) -> bool:
+        if search_term != None:
+            index_info_contains_search_term_info = index_info["empty_term_supported"] != None
 
-            if index_info_contains_value_info:
-                if value == "" and index_info["empty_term_supported"] is False:
+            if index_info_contains_search_term_info:
+                if search_term == "" and index_info["empty_term_supported"] is False:
                     return False
         
         return True
     
     @staticmethod
     def _validate_1_1_sort(available_record_schemas: dict, sort_keys: list[SortKey], record_schema: str):
         # Here, we want to see whether the SCHEMA is available to
```

### Comparing `sru_queryer-1.0.3/src/sru_queryer.egg-info/PKG-INFO` & `sru_queryer-2.0.0/src/sru_queryer.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sru-queryer
-Version: 1.0.3
+Version: 2.0.0
 Summary: A utility for integrating SRU queries into your applications.
 Author-email: Erik Jones <ejones99@umd.edu>
 Maintainer-email: USMAI <libclas@umd.edu>
 Keywords: sru,library,api
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7.17
@@ -17,487 +17,557 @@
 
 Welcome to SRU Queryer, a library for working with Search/Retrieval via URL (SRU) created by the USMAI Library Consortium. This package is designed to make working with SRU simple and accurate!
 
 Using this utility has a few big benefits, such as:
 
 1. It handles validating much of the searchRetrieve request. This is particularly helpful because many SRU servers don't have good error messages.
 2. It handles formatting the searchRetrieve request for you. This makes queries much less prone to human mistakes.
-3. It provides functions to see which indexes are available to search in the SRU server.
+3. Programmatically access the capabilities of the SRU server in your program.
 
 ## TABLE OF CONTENTS
 
 1. [Setting Up The Environment](#setting-up-the-environment)
 2. [Basic Usage](#basic-usage)
 3. [Quick Overview of Important Components](#quick-overview-of-important-components)
    1. [Initializing SRU Functionality](#initializing-sru-functionality)
-   2. [Basic Query Component](#basic-query-component-indexquery)
-   3. [Configuration Service](#configuration-service-sruutil)
-   4. [Query class](#creating-queries---the-query-class)
-   5. [Boolean Operators for Queries](#constructing-more-advanced-queries-boolean-operators)
+   2. [Basic Query Component](#basic-query-component-searchclause)
+   3. [Searching using SRUQueryer](#searching-using-sruqueryer)
+   4. [Boolean Operators for Queries](#constructing-more-advanced-queries-boolean-operators)
 4. [Full Overview of Different Components](#full-overview-of-different-components)
-   1. [IndexQuery](#basic-query-component-indexquery-1)
-   2. [SRUUtil](#sruutil)
-   3. [Boolean Operators (AND, OR, NOT, PROX)](#constructing-more-advanced-queries-boolean-operators-1)
-   4. [Query](#query-class)
-   5. [LITERAL](#custom-queries-literal)
-   6. [Modifiers](#modifiying-operators---modifiers)
-   7. [Sorting in v1.2](#sorting-in-12-sortby-clauses)
-   8. [Sorting in v1.1](#sorting-in-11-SortKey)
+   1. [SearchClause](#basic-query-component-searchclause-1)
+   2. [SRUQueryer](#sruqueryer)
+   3. [Boolean Operators (AND, OR, NOT, PROX)](#boolean-operators)
+   4. [RawCQL](#custom-queries-rawcql)
+   5. [Modifiers](#modifiying-operators---modifiers)
+   6. [Sorting in v1.2](#sorting-in-12-sortby-clauses)
+   7. [Sorting in v1.1](#sorting-in-11-SortKey)
+5. [Known Incompatibilities](#known-incompatibilities)
 
 ## Setting Up The Environment
 
-This python script was developed using python 3.10 and tested on python 3.11.1.
-
 To install sru-queryer, just run `pip install sru-queryer`
 
+Note that you may have to specify pip3 if you have python2 installed. The install will fail if you try to use python2's PIP.
+
 ## Basic Usage
 
 Here's just a basic usage example:
 
 ```
 # Create a configuration object for the SRU server, allowing you to validate and send queries.
-sru_configuration = SRUUtil.create_configuration_for_server("https://path-to-sru-server-base", "https://path-to-sru-server-base", "1.2")
-
-# Configure a query - in this case, find records where the creator includes Abraham, sorted alphabetically & ascending.
-query_obj = Query(sru_configuration, IndexQuery(
-        "alma", "creator", "=", "Abraham"), sort_queries=[{
-            "index_set": "alma",
-            "index_name": "creator",
-            "sort_order": "ascending"
-        }])
-
-# Validate the query to see whether it's valid
-query_obj.validate()
+queryer = SRUQueryer("https://path-to-sru-server-base")
 
-# Construct the request (just a python PreparedRequest object)
-request = query_obj.construct_request()
-
-s = Session()
-response = s.send(request)
+# Configure a SearchRetrieve query - in this case, find records where the creator includes Abraham, sorted alphabetically & ascending.
+response_content = queryer.search_retrieve(SearchClause("alma", "creator", "=", "Abraham"),
+                     sort_queries=[{
+                           "index_set": "alma",
+                           "index_name": "creator",
+                           "sort_order": "ascending"
+                     }])
 ```
 
 This code will send the following query:
 https://path-to-sru-server-base/?version=1.2&operation=searchRetrieve&recordSchema=marcxml&maximumRecords=10&query=alma.creator=%22Abraham%22%20sortBy%20alma.creator/sort.ascending
 
 You can also create a query with boolean conditions:
 
 ```
 # Find records where the creator includes Abraham AND the material type is 'book'
-query_obj = Query(sru_configuration, AND(IndexQuery("alma", "creator", "=", "Abraham"), IndexQuery("alma", "materialType", "==", "BOOK")))
+queryer.search_retrieve(sru_configuration, AND(SearchClause("alma", "creator", "=", "Abraham"), SearchClause("alma", "materialType", "==", "BOOK")))
 ```
 
 ## Quick Overview of Important Components:
 
 ### Initializing SRU functionality
 
-Before you can validate or send searchRetrieve requests, you must create an SRU configuration for your server. The configuration of this server will be in the form of an SRUConfiguration class.
-
-An instance is created through the SRUUtil.create_configuration_for_server() function, and all you have to do is to pass the created instance to the functions that need it. You can read information from it if you want to integrate SRU querying more deeply into your application.
+Before you can validate or send searchRetrieve requests, you must create a queryer. Upon initialization, the queryer will contact your SRU server and set up everything it needs to validate and format your SRU queries.
 
 ```
-from sru_queryer.drivers import alma_driver
-sru_configuration = SRUUtil.create_configuration_for_server("https://path-to-sru-server-base", "https://path-to-sru-server-base", "1.2", driver=alma_driver)
+queryer = SRUQueryer("https://path-to-sru-server-base")
 ```
 
-This is the most basic way to create a configuration object. The first argument is the SRU explain URL, the second is the searchRetrieve URL, the third is the SRU version, and the final one is the driver. This function takes many other optional arguments, which can do things like configure the default record schemas, default context sets, change validation settings, etc.
+This is the most basic way to create a queryer. This function takes many other optional arguments, which can do things like configure the default record schemas, default context sets, change validation settings, etc.
+
+### Basic Query Component: SearchClause
 
-A very important argument is 'driver'. This takes a dict which tells the program how to parse explainResponses. This program already includes drivers for ExLibris Alma, LOC, and gapines SRU servers. The default is set to 'alma' (ExLibris Alma), which is why you won't see it in some examples. The drivers are straightforward - you can follow the template of the included drivers to create one for your own server. Drivers serve to tell the program where to find the information it needs in the SRU explainResponse and which information is available.
+`from sru_queryer.cql import SearchClause`
 
-### Basic Query Component: IndexQuery
+This is officially known as a 'CQL search clause': https://www.loc.gov/standards/sru/cql/spec.html <br>
+A standard CQL search clause looks like: `alma.title="Harry Potter"`. This same query with the SearchClause class would look like: `SearchClause("alma", "title", "=", "Harry Potter")`. Pretty straightforward! See more in the extended SearchClause section below - there's rules for which of these arguments are required.
 
-`from sru_queryer import IndexQuery`
+### Searching using SRUQueryer
 
-This would more officially be known as a 'CQL search clause': https://www.loc.gov/standards/sru/cql/spec.html.\
-A standard CQL search clause looks like: `alma.title="Harry Potter"`. This same query with the IndexQuery class would look like: `IndexQuery("alma", "title", "=", "Harry Potter")`
+`from sru_queryer import SRUQueryer`
 
-https://www.loc.gov/standards/sru/cql/spec.html
+There's two options for conducting searchRetrieve requests with the SRUQueryer class. <br>
 
-### Creating queries - the Query class
+First, you can have the queryer send the request for you and return the content. Once the querier is initialized, you can do so in this way (this is only an example search, it doesn't have to look exactly like this):
 
-`from sru_queryer import Query`
+```
+response_content = queryer.search_retrieve(SearchClause("alma", "creator", "=", "Abraham"),
+         sort_queries=[{
+            "index_set": "alma",
+            "index_name": "creator",
+            "sort_order": "ascending"
+        }])
+```
 
-Use the Query class to actually construct and validate a query.\
-This class takes the SRU configuration as an argument, followed by the actual CQL query made up of boolean operators, Literals, and IndexQueries. You can also set certain values that you might want to change between queries while keeping the same SRUConfiguration - record format, start record, maximum records, etc. It also takes sort queries.
+Alternately, you can construct a requests.Request object that you can then send yourself. This allows for a bit more flexibility, like adding a custom authentication header:
 
 ```
-query_obj = Query(sru_configuration, IndexQuery(
+request = queryer.construct_search_retrieve_request(SearchClause(
         "alma", "creator", "=", "Abraham"), sort_queries=[{
             "index_set": "alma",
             "index_name": "creator",
             "sort_order": "ascending"
         }])
 ```
 
+Both of these options take the same arguments. The first is the CQL query made up of boolean operators, RawCQL classes, and/or SearchClauses. You can also set certain values that you might want to change between queries while keeping the same queryer - record format, start record, maximum records, etc. It also takes sort queries.
+
 ### Constructing more advanced queries: Boolean Operators
 
 `from sru_queryer.cql import AND, OR, NOT, PROX`
 
-Boolean Operators are used to construct queries with one or more IndexQueries. Their usage is extrememly simply by design, and should be familiar to people working with logic-based programming.
+Boolean Operators are used to construct queries with one or more SearchClauses. Their usage is extrememly simply by design, and should be familiar to people working with logic-based programming.
 
 For example, the query:
-`OR(IndexQuery("alma", "title", "=", "Harry"), IndexQuery("alma", "title", "=", "Potter"))`
+`OR(SearchClause("alma", "title", "=", "Harry"), SearchClause("alma", "title", "=", "Potter"))`
 will produce the following string, when formatted:
 `alma.title="Harry" or alma.title="Potter"` (except spaces will be replaced with '%20')
 
+<br>
+<br>
+
 ---
 
 ## Full Overview of Different Components
 
 This section will give a deep dive on each different component in sru_queryer. Check here if you can't figure something out!
 
-### Basic Query Component: IndexQuery
+<br>
+
+### Basic Query Component: SearchClause
 
-`from sru_queryer import IndexQuery`
+`from sru_queryer import SearchClause`
 
-A SRU query, written in CQL, is made up of one or more queries on Indexes - here called an IndexQuery. Formatted, an index query looks like:
+A SRU query, written in CQL, is made up of one or more search clauses. Formatted, a search clause looks like:
 
 `alma.title="Harry Potter"`
 
-The four components of this query are the context_set (`alma`), the index (`title`), the operation(`=`, called 'relation' officially), and the value (`Harry Potter`, called 'search term' officially). For more information, please see https://www.loc.gov/standards/sru/cql/spec.html. I won't explain the nuances of SRU/CQL here, just my implementation of it.
+The four components of this query are the context_set (`alma`), the index (`title`), the relation(`=`), and the search term (`Harry Potter`). For more information, please see https://www.loc.gov/standards/sru/cql/spec.html. I won't explain the nuances of SRU/CQL here, just my implementation of it.
 
 #### USAGE
 
-All of the options for initializing an IndexQuery are keyword arguments, but are listed in an order that's the same as a standard index query (aside from modifiers).
-This means you can initialize an IndexQuery in a human-readable way without including any keywords:
-`IndexQuery("alma", "title", "=", "Harry Potter")`
+All of the options for initializing a SearchClause are keyword arguments, but are listed in order.
+This means you can initialize a SearchClause in a human-readable way without including any keywords:
+`SearchClause("alma", "title", "=", "Harry Potter")`
 which looks like the formatted query:
 `alma.title="Harry Potter"`.
 
-For queries without all options, you have to include the option name for each option OR include 'None' where the option would be.
-Query with only a value:
-`IndexQuery(value="Harry Potter")` or `IndexQuery(None, None, None, "Harry Potter")`
-Query without a context_set:
-`IndexQuery(index_name="title", operation="=", value="Harry Potter")` or
-`IndexQuery(None, "title", "=", "Harry Potter")`
+For SearchClauses without all options, you have to include the option name for each option OR include 'None' where the option would be.<br>
+SearchClause with only a search term:<br>
+`SearchClause(search_term="Harry Potter")` or `SearchClause(None, None, None, "Harry Potter")`<br>
+SearchClause without a context_set:<br>
+`SearchClause(index_name="title", relation="=", search_term="Harry Potter")` or <br>
+`SearchClause(None, "title", "=", "Harry Potter")`
 
-Keep in mind, if a context_set or index_name is not provided, the defaults must be set manually though SRUUtil for validation to work. This is because the explainResponse does not include the default context set or index. If you do not know them, there are options to disable validation for IndexQueries that use defaults.
+Keep in mind, if a context_set or index_name is not provided, the defaults must be set manually during initialization of SRUQueryer for validation to work. This is because the explainResponse does not always include the default context set or index. If you do not know them, there are options to disable validation for SearchClauses that use defaults.
 
 #### AVAILABLE FUNCTIONS
 
-You don't need to use any functions on an IndexQuery as a general user. For instance, the Query.validate() function will also run the validate() function for all included IndexQueries.
+You don't need to use any functions on a SearchClause as a general user. For instance, SRUQueryer will run the validate() function for all included SearchClauses.
 
 #### INITIALIZATION OPTIONS
 
-Internal variables are private once initialized - if you change them, you will bypass some validation and likely cause errors. It's easy to create a new instance of IndexQuery if you need different options, so do that instead of modifying an existing one.
+Internal variables are private once initialized - if you change them, you will bypass some validation and likely cause errors. It's easy to create a new instance of SearchClause if you need different options, so do that instead of modifying an existing one.
 
-| Option      | Data Type                 | Mandatory | Description                                                                          |
-| ----------- | ------------------------- | --------- | ------------------------------------------------------------------------------------ |
-| context_set | string / None             | No        | The context set to search in.                                                        |
-| index_name  | string / None             | No        | The index you want to search.                                                        |
-| operation   | string / None             | No        | The operator ("=", ">", etc) you want to search with.                                |
-| value       | string                    | Yes       | The value you're looking for.                                                        |
-| modifiers   | list of RelationModifiers | No        | A list of relation modifiers for the operation. More information on modifiers below. |
+| Option      | Data Type                 | Mandatory | Description                                                                         |
+| ----------- | ------------------------- | --------- | ----------------------------------------------------------------------------------- |
+| context_set | string / None             | No        | The context set to search in.                                                       |
+| index_name  | string / None             | No        | The index you want to search.                                                       |
+| relation    | string / None             | No        | The operator ("=", ">", etc) you want to search with.                               |
+| search_term | string                    | Yes       | The value you're looking for.                                                       |
+| modifiers   | list of RelationModifiers | No        | A list of relation modifiers for the relation. More information on modifiers below. |
 
-COMBINATIONS OF INITIALIZATION PROPERTIES (according to LOC standards):
+COMBINATIONS OF INITIALIZATION PROPERTIES (according to LOC standards):<br>
 You MUST include either:
 
-1. a value,
-2. an index_name, operation, and value,
-3. a context_set, index_name, operation, and value.
+1. a search term,
+2. an index_name, relation, and search term,
+3. a context_set, index_name, relation, and search term.
 
-- RelationModifiers can be set for all combinations, but will only added to the final query on combinations with an operation.
+- RelationModifiers can be set for all combinations, but will only added to the final query on combinations with an relation.
 
-### SRUUtil
+<br>
+<br>
 
-`from sru_queryer import SRUUtil`
+### SRUQueryer
 
-The SRUUtil static class handles core configuration for this utility, as well as providing an interface for reading the configuration information.
+`from sru_queryer import SRUQueryer`
 
-#### AVAILABLE FUNCTIONS:
+The SRUQueryer is the most important class of this library, as it handles configuring the utility as well as constructing, validating, and sending requests.
 
-There are two functions that the general user would want to use:
+The SRUQueryer stores all its configuration information in an SRUConfiguration object in the property sru_configuration. If you want your program to know the capabilites of the SRU server, it can read the properties of queryer.sru_configuration. For instance, you can access the available record schemas with:<br>
 
-1. `format_available_indexes` - This function nicely formats all the indexes availabe for an SRU server, as well as their information. It then prints this information to the console, to a text file, or both. It only prints to the console by default. You can filter the indexes based on their human-readable title.
+`queryer.sru_configuration.available_record_schemas`<br>
 
-`format_available_indexes(sru_configuration, filename: str | None = None, print_to_console: bool = True, title_filter: str | None = None)`
+It is HIGHLY recommended not to change any of these values.
 
-2. `create_configuration_for_server` - This function creates an SRUConfiguration object by reading you provide as arguments to the function, pulling values found by contacting the SRU server, and reconciling them. Many arguments are optional and are used for improved validation of the SRU queries. Be aware that any option you specify manually will override the corresponding value returned by the explainResponse, if the explainResponse contains this value.
+#### INITIALIZATION OPTIONS
 
-Arguments for create_configuration_for_server:
+This function configures settings (stored in an SRUConfiguration object) by reading the arguments you provide, pulling values from the SRU server, and reconciling them. Many arguments are optional and are used for improved validation of the SRU queries. Be aware that any option you specify manually will override the corresponding value returned by the explainResponse, if the explainResponse contains this value.
 
-`explain_url`
-| Mandatory | Data Type | Description |
-| ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| Yes | url string | The base URL for the explainResponse. This must not include any query params - they will be added by the utility. |
+If the SRU server returns a different SRU version than you the one you specify, the library will use that version. If you do not provide a version, it will default to version 1.2 or whatever the server is capable of.
 
-`search_retrieve_url`
+`server_url`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| Yes | url string | The base URL for the searchRetrieve query. This must not include any query params - they will be added by the utility. |
+| Yes | url string | The base URL for the server. This must not include any query params - they will be added by the utility. |
 
 `sru_version`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| Yes, but defaults to 1.2 | string | The SRU version to use.|
-
-`driver`
-| Mandatory | Data Type | Description |
-| --- | --- | --- |
-| Yes, but defaults to Alma driver | dict | The driver for parsing the xml explainResponse. This is needed because different SRU servers have their data located in different XML paths. The driver tells the program where to look. The drivers are arrays of strings, each string representing a key in a higherarchical dictionary. The drivers will be run on the explainResponse AFTER it's been parsed by the xmltodict library. Additional drivers can be imported from `sru_queryer.drivers` |
+| No - defaults to 1.2 | string | The SRU version to use. If the SRU server returns a different SRU version than you specify, the tool will use that version. If you do not provide a version, it will default to version 1.2. |
 
 `username`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
 | No | string | The username for the SRU server, if the server requires authentication. This is sent in Basic Access Authentication format. |
 
 `password`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
 | No (unless there's a username) | string | The password for the SRU server, if the server requires authentication. This is sent in Basic Access Authentication format. |
 
 `default_cql_context_set`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| No | string | The default context set for indexes if one is not provided. Adding a default enables validation for IndexQueries without context sets. For example, if the default context set is set to 'alma', this will validate the query `title="Harry Potter"` as if it were `alma.title="Harry Potter"`. The default MUST be the same as the default context set for your SRU server. Some SRU servers return this information in the explainResponse; others don't.|
+| No | string | The default context set for indexes if one is not provided. Adding a default enables validation for SearchClauses without context sets. For example, if the default context set is set to 'alma', this will validate the query `title="Harry Potter"` as if it were `alma.title="Harry Potter"`. The default MUST be the same as the default context set for your SRU server. Some SRU servers return this information in the explainResponse; others don't.|
 
 `default_cql_index`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| No | string |The default index for an IndexQuery if only a value is provided. If you have a default_cql_index, you must also have a default_cql_context_set. For example, if the default context set is 'alma' and the default index is 'title', the query `"Harry Potter"` will be validated as `alma.title "Harry Potter"`. |
+| No | string |The default index for a SearchClause if only a search term is provided. If you have a default_cql_index, you must also have a default_cql_context_set. For example, if the default context set is 'alma' and the default index is 'title', the query `"Harry Potter"` will be validated as `alma.title "Harry Potter"`. |
 
 `default_cql_relation`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| No | string |The default relation for an IndexQuery if only a value is provided. If you have a default_cql_relation, you must also have a default_cql_context_set and index. For example, if the default context set is 'alma' and the default index is 'title', the query `"Harry Potter"` will be validated as `alma.title="Harry Potter"`. Not all SRU servers list valid relations for index queries, so this is ONLY NECCESARY when validating defaults for servers that do. If you server does not, you can safely ignore this even if you don't disable validation for cql defaults.|
+| No | string |The default relation for a SearchClause if only a search term is provided. If you have a default_cql_relation, you must also have a default_cql_context_set and index. For example, if the default context set is 'alma' and the default index is 'title', the query `"Harry Potter"` will be validated as `alma.title="Harry Potter"`. Not all SRU servers list valid relations for SearchClauses, so this is ONLY NECCESARY when validating defaults for servers that do. If you server does not, you can safely ignore this even if you don't disable validation for cql defaults.|
 
 `disable_validation_for_cql_defaults`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| No | boolean | If you don't know the default context set, index, and relation (if relation information for indexes is specified) for your SRU server, yet you still want to send IndexQueries with default values, this setting will allow for that. It will disable any validation for indexQuery defaults, but allow validation for non-defaults. |
+| No | boolean | If you don't know the default context set, index, and relation (if relation information for indexes is specified) for your SRU server, yet you still want to send SearchClauses with defaults, this setting will allow for that. It will disable any validation for SearchClause defaults, but allow validation for non-defaults. |
 
 `max_records_supported`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
 | No | int | This indicates the maximum number of records a searchRetrieve response is capable of returning. This is often returned by the explainResponse. If your server's maximum is not included in its explainResponse, it is recommended to include this value. Without it, the number of records requested in a query will not be validated correctly. |
 
 `default_records_returned`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
-| No | int | This indicates the default maximum number of records that the searchRetrieve will return. It must be equal to or less than the max_records_supported. If set, every query will return a maximum of this number of records. By default, it is set to whatever SRUUtil finds in the explainResponse OR, if not specified in the explainResponse, will not be included. |
+| No | int | This indicates the default maximum number of records that the searchRetrieve will return. It must be equal to or less than the max_records_supported. If set, every query will return a maximum of this number of records. By default, it is set to whatever is in the explainResponse OR, if not specified in the explainResponse, will not be included. |
 
 `default_record_schema`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
 | No | string | The default record schema that's returned by the searchRetrieve operation. If you don't specify what record schema you want in an individual query, the default record schema (if set) will be used in that query. If the explainResponse includes a default record schema and you don't specify one, the explainResponse's record schema will be included in all queries. |
 
 `default_sort_schema`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
 | No | string | The default schema that sort operations are run on. I don't know too much about this. I use it for validating sortKeys, which are only for version 1.1. If the sort schema is not included in a sort key, this value will be used to validate the sort key (not all schemas can sort).|
 
-### Constructing more advanced queries: Boolean Operators
+#### AVAILABLE FUNCTIONS:
+
+There are three functions that the general user would want to use:
+
+##### `search_retrieve`
+
+This function sends a search retrieve request, using the values you provide and the information parsed from the SRU ExplainResponse.
+
+##### USAGE
+
+After initializing your SRUQueryer class: <br>
+`response_content = queryer.search_retrieve(OR(SearchClause("alma", "title", "=", "Harry"), SearchClause("alma", "title", "=", "Potter")), record_schema="marcxml")`
+
+There are additional options to you can set to modify the request. They will be discussed below.
+
+This will validate and send the request. You will receive whatever content the SRU server sends back - it may be a searchRetrieveResponse, or it might be an error. This library does not currently validate or parse the response.
+
+##### INPUT PARAMETERS
+
+| Option          | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                           |
+| --------------- | --------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| cql_query       | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                    |
+| start_record    | int                                                             | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                     |
+| maximum_records | int                                                             | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUQueryer initialization.create_configuration_for_server, by the explainResponse, or is set to 5.                                                     |
+| record_schema   | string                                                          | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse. |
+| sort_queries    | list[dict] or list[SortKey]                                     | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                              |
+| record_packing  | string                                                          | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                         |
+| validate        | boolean (default True)                                          | No        | Whether or not to validate the query before sending it. You can disable validation if you think the library is falsely failing a query.                                                                                                                               |
+
+<br>
+
+##### `construct_search_retrieve_request`
+
+This does the same thing as the previous function, however instead of running request.prepare() and sending the request, it returns the requests.Request object. This allows you to be more flexible by modifying the request - for instance, if you want to use a shared requests.Session between multiple requests, or add a custom authentication header.
+
+##### USAGE
+
+After initializing your SRUQueryer class: <br>
+`request = queryer.construct_search_retrieve_request(OR(SearchClause("alma", "title", "=", "Harry"), SearchClause("alma", "title", "=", "Potter")), record_schema="marcxml")`
+
+This will validate the request and return a requests.Request object.
+
+##### INPUT PARAMETERS
+
+| Option          | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                           |
+| --------------- | --------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| cql_query       | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                    |
+| start_record    | int                                                             | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                     |
+| maximum_records | int                                                             | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUQueryer initialization.create_configuration_for_server, by the explainResponse, or is set to 5.                                                     |
+| record_schema   | string                                                          | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse. |
+| sort_queries    | list[dict] or list[SortKey]                                     | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                              |
+| record_packing  | string                                                          | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                         |
+| validate        | boolean (default True)                                          | No        | Whether or not to validate the query before returning the requests.Request object. You can disable validation if you think the library is falsely failing a query.                                                                                                    |
+
+##### `format_available_indexes`
+
+This function nicely formats all the indexes availabe for an SRU server, as well as their information. It then prints this information to the console, to a text file, or both. It only prints to the console by default. You can filter the indexes based on their human-readable title.
+
+`format_available_indexes(sru_configuration, filename: str | None = None, print_to_console: bool = True, title_filter: str | None = None)`
+
+<br>
+<br>
+
+### Boolean Operators
 
 `from sru_queryer.cql import AND, OR, NOT, PROX`
 
-Boolean Operators are used to construct queries with one or more IndexQueries. Their usage is extrememly simply by design, and should be familiar to people working with logic-based programming.
+Boolean Operators are used to construct queries with one or more SearchClauses. Their usage is extrememly simply by design, and should be familiar to people working with logic-based programming.
 
 #### USAGE
 
-Each operator takes an unlimited quantity of arguments, each of which represents a logical condition. Each condition can be an IndexQuery, a Literal (discussed below), or another nested Boolean Operator.
+Each operator takes an unlimited quantity of arguments, each of which represents a logical condition. Each condition can be a SearchClause, a RawCQL class (discussed below), or another nested Boolean Operator.
 
 For example, the query:
-`OR(IndexQuery("alma", "title", "=", "Harry"), IndexQuery("alma", "title", "=", "Potter"))`
+`OR(SearchClause("alma", "title", "=", "Harry"), SearchClause("alma", "title", "=", "Potter"))`
 will produce the following string, when formatted:
 `alma.title="Harry" or alma.title="Potter"` (except spaces will be replaced with '%20')
 
 If you nest one Boolean Operator within another, the resultant behavior will depend on whether the nested boolean operator has one condition or whether it has multiple conditions.
 
 1. If the nested operator has one condition, it will REPLACE the preceeding boolean operator of the parent. This allows you to create a long query with alternating boolean operators:
-   `AND(IndexQuery("alma", "title", "=", "Maryland"), OR(IndexQuery("alma", "materialType", "==", "BOOK")), IndexQuery("alma", "main_pub_date", ">", "1975"))`
+   `AND(SearchClause("alma", "title", "=", "Maryland"), OR(SearchClause("alma", "materialType", "==", "BOOK")), SearchClause("alma", "main_pub_date", ">", "1975"))`
    Procduces:
    `alma.title="Maryland" or alma.materialType=="BOOK" and alma.main_pub_date>"1975"` (again, spaces replaced with '%20')
 
    \*\* KEEP IN MIND that you can't have an operator with one condition as the first condition of a parent operator (or as the top condition). This wouldn't make sense because all operators require 2 conditions (none are unary operators, even NOT. Not is treated as 'and-not'). Here, I allow operators with one conditions so that a parent's operator can be overridden - this makes formatting simpler.
 
 2. If the nested operator has more than one condition, it will be surrounded by parenthesis and the parent's operator will be placed before the parenthesis:
-   `AND(IndexQuery("alma", "title", "=", "Maryland"), OR(IndexQuery("alma", "materialType", "==", "BOOK"), IndexQuery("alma", "materialType", "==", "DVD")))`
+   `AND(SearchClause("alma", "title", "=", "Maryland"), OR(SearchClause("alma", "materialType", "==", "BOOK"), SearchClause("alma", "materialType", "==", "DVD")))`
    Produces:
    `alma.title="Maryland" and (alma.materialType=="BOOK" or alma.materialType=="DVD")`
 
 You may add modifiers to the Boolean Operator with the 'modifiers' keyword argument. Please use the correct modifier type for the boolean operator you've chosen - for example, the PROX modifier should use ProxModifier, whereas AND, OR, and NOT should use the AndOrNotModifier. You may create custom modifiers by extending the CQLModifierBase class. More on Modifiers later.
 
 #### AVAILABLE FUNCTIONS
 
-As with the IndexQuery, the functions on the CQL Boolean Operators are not indended to be used by the general person. For example, Query.construct_request() will call format() for all boolean operators.
+As with the SearchClause, the functions on the CQL Boolean Operators are not indended to be used by the general person. For example, SRUQueryer.search_retrieve will call format() for all boolean operators.
 
 #### INITIALIZATION OPTIONS
 
 Any options not marked as MANDATORY are optional. It is not recommended to change any options manually after initializing a CQL Boolean Operator, as this will bypass some validation. It's easy to create a new instance of CQL Boolean Operator if you need different options.
 
-| Option                   | Data Type                                                      | Mandatory | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
-| ------------------------ | -------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| Positional arguments 1-n | IndexQuery, class extending CQLBooleanOperatorBase, or LITERAL | Yes       | Search clauses, which will be joined by the boolean operator. Must have at least one, or two if it is the outermost condition or first condition in a parent operator.                                                                                                                                                                                                                                                                                                                                                                                                                  |
-| modifiers                | list[Class extending CQLModifierBase]                          | No        | A list of modifiers for the boolean operator, which will be tacked on to the end of the operator. Keep in mind that modifiers will be added to each instance of the formatted operator - if there's 3 conditions in the operator, leading to two 'and' conditions, this list will be included for both 'and's. To get around this, you may use a nested Boolean Operator with one condition and add the modifiers to that operator. In this case, it will replace the parent's operator with its own, which has the modifiers. The rest of the parent's operators will not be affected. |
-
-Note: Literals may work in place of modifiers, however, this has not been tested.
-
-### Query class
-
-`from sru_queryer import Query`
-
-Now, for the class which you'll likely use the most - the Query class. Whereas SRUUtil deals with configuration, Query only deals with one specific query. It takes an instance of SRUUtil for the purposes of validation.
-
-#### USAGE
-
-Use the Query class to construct your request.
-Instantiate the SRUUtil class:
-`configuration = SRUUtil.construct_configuration_for_server(...)`
-Create the query class with the desired request:
-`query_util = Query(configuration, OR(IndexQuery("alma", "title", "=", "Harry"), IndexQuery("alma", "title", "=", "Potter")), record_schema="marcxml")`
-
-There are additional options to you can set to modify the request. They will be discussed below.
-
-You can then validate the request with the validate() function, which will throw an error for the first issue it finds:
-`query_util.validate()`
-
-After this, you can get a PreparedRequest and send it:
-`from requests import Session`
-`request_to_send = query_util.construct_request()`
-`s = Session()`
-`response = s.send(request_to_send)`
+| Option                   | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| ------------------------ | --------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| Positional arguments 1-n | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | Search clauses, which will be joined by the boolean operator. Must have at least one, or two if it is the outermost condition or first condition in a parent operator.                                                                                                                                                                                                                                                                                                                                                                                                                  |
+| modifiers                | list[Class extending CQLModifierBase]                           | No        | A list of modifiers for the boolean operator, which will be tacked on to the end of the operator. Keep in mind that modifiers will be added to each instance of the formatted operator - if there's 3 conditions in the operator, leading to two 'and' conditions, this list will be included for both 'and's. To get around this, you may use a nested Boolean Operator with one condition and add the modifiers to that operator. In this case, it will replace the parent's operator with its own, which has the modifiers. The rest of the parent's operators will not be affected. |
 
-This will return an XML response, which might be a searchRetrieve response, or might be an error.
-
-#### AVAILABLE FUNCTIONS
-
-validate: Validates all components of the searchRetrieve request that can be validated. For the query itself, this is a recursive function that validates all CQLBooleanOperators / IndexQueries and their children. It will throw a ValueError an error for the first issue it finds. It returns nothing when successful.
-
-construct_request: Uses all components of the query to construct a searchRetrieve request. It pulls some of the information from the SRUConfiguration, including the base URL, username, password, and version, as well as other defaults that have been specified. Returns a requests.PreparedRequest object.
-
-#### INITIALIZATION OPTIONS
+Note: RawCQL classes may work in place of modifiers, however, this has not been tested.
 
-Unlike many other classes, it is safe to modify variables after instantiating. This is because no validation occurs in the constructor. If you do change something, you'd just have to remember to run validate() again.
+<br>
+<br>
 
-| Option            | Data Type                                                      | Mandatory | Description                                                                                                                                                                                                                                                           |
-| ----------------- | -------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| sru_configuration | SRUConfiguration                                               | Yes       | The configuration of the SRU server, which is used to construct and validate queries. Create a configuration with SRUUtil's create_configuration_for_server()                                                                                                         |
-| index_search      | IndexQuery, class extending CQLBooleanOperatorBase, or LITERAL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                    |
-| start_record      | int                                                            | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                     |
-| maximum_records   | int                                                            | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUUtil.create_configuration_for_server, by the explainResponse, or is set to 5.                                                                       |
-| record_schema     | string                                                         | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse. |
-| sort_queries      | list[dict] or list[SortKey]                                    | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                              |
-| record_packing    | string                                                         | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                         |
+### Custom queries: RawCQL
 
-### Custom queries: LITERAL
+`from sru_queryer.cql import RawCQL`
 
-`from sru_queryer.cql import LITERAL`
+USE ONLY WHEN NEEDED! The RawCQL class allows you to pass a string directly to the CQL query. THE STRING WILL NOT BE VALIDATED.
 
-USE ONLY WHEN NEEDED! The LITERAL class allows you to pass a string directly to the SRU query. THE STRING WILL NOT BE VALIDATED.
+RawCQL is intended for cases in which this library does not support a certain SRU feature OR to bypass a bugged output format.
 
-Literals are intended for cases in which this library does not support a certain SRU feature OR to bypass a bugged output format.
+Using raw cql allows you to insert whatever search condition you need, while still validating the rest of the query. You can use a RawCQL class to replace the entire search query, replace a boolean conditional, or replace a SearchClause.
 
-Using a literal allows you to insert whatever search condition you need, while still validating the rest of the query. You can use a literal to replace the entire search query, replace a boolean conditional, or replace an IndexQuery.
-
-You don't have to worry about creating the string in exact URL notation (e.g., replacing ' ' with %20 or '"' with %22). Characters will be encoded automatically by Query.construct_request().
+You don't have to worry about creating the string in exact URL notation (e.g., replacing ' ' with %20 or '"' with %22). Characters will be encoded automatically by SRUQueryer.search_retrieve().
 
 #### USAGE
 
-Use a literal in place of an IndexQuery or class extending CQLBooleanOperatorBase (AND, OR, NOT, PROX).
+Use a RawCQL class in place of a SearchClause or class extending CQLBooleanOperatorBase (AND, OR, NOT, PROX).
 
-Here's an example of a literal being used instead of an IndexQuery in an AND boolean operator:
-`AND(IndexQuery("alma", "title", "=", "Maryland"), LITERAL("alma.materialType==BOOK"))`
+Here's an example of a RawCQL class being used instead of a SearchClause in an AND boolean operator:
+`AND(SearchClause("alma", "title", "=", "Maryland"), RawCQL("alma.materialType==BOOK"))`
 
-Here's an example of a literal replacing a CQLBooleanOperator and its IndexQueries:
-`LITERAL('alma.title="Maryland" and (alma.materialType=="BOOK" or alma.materialType=="DVD")')`
+Here's an example of a RawCQL class replacing a CQLBooleanOperator and its SearchClauses:
+`RawCQL('alma.title="Maryland" and (alma.materialType=="BOOK" or alma.materialType=="DVD")')`
 
-You can't pass an IndexQuery or a CQLBooleanOperator to a literal and have them be nested inside of it, in the way you can nest CQLBooleanOperators/IndexQueries inside CQLBooleanOperators. You COULD format them in when constructing the literal using string formatting:
-`LITERAL(f'{index_query_1.format()} and {cql_boolean_operator.format()}')`
-...where index_query_1 and cql_boolean_operator are instantiated IndexQuery and CQLBooleanOperatorBase objects.
+You can't pass a SearchClause or a CQLBooleanOperator to a RawCQL class and have them be nested inside of it, in the way you can nest CQLBooleanOperators/SearchClauses inside CQLBooleanOperators. You COULD format them in when constructing the RawCQL class using string formatting:
+`RawCQL(f'{search_clause_1.format()} and {cql_boolean_operator.format()}')`
+...where search_clause_1 and cql_boolean_operator are instantiated SearchClause and CQLBooleanOperatorBase objects.
 
 However, keep in mind that this will disable validation for those inner objects.
 
 #### AVAILABLE FUNCTIONS
 
-There's nothing here that you would want to use. This class is essentially a wrapper around a string which allows it to be interchangable with IndexQueries and CQLBooleanOperators.
+There's nothing here that you would want to use. This class is essentially a wrapper around a string which allows it to be interchangable with SearchClauses and CQLBooleanOperators.
 
 #### INITIALIZATION OPTIONS
 
-| Option         | Data Type              | Mandatory | Description                                                                                                                                                                                                                           |
-| -------------- | ---------------------- | --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| literal_string | string (should be CQL) | Yes       | The string that you want to be executed. Again, you don't have to provide it in a url-exact format, spaces and other special characters will be replaced by their compability characters later on if you're using the provided tools. |
-| add_padding    | boolean                | No        | Whether or not to add a space (%20) before and after the string upon formatting. Set to false by default.                                                                                                                             |
+| Option         | Data Type              | Mandatory | Description                                                                                                                                                                                                           |
+| -------------- | ---------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| raw_cql_string | string (should be CQL) | Yes       | A CQL query as a string. Again, you don't have to provide it in a url-exact format, spaces and other special characters will be replaced by their compability characters later on if you're using the provided tools. |
+| add_padding    | boolean                | No        | Whether or not to add a space (%20) before and after the string upon formatting. Set to false by default.                                                                                                             |
+
+<br>
+<br>
 
 ### Modifiying operators - Modifiers
 
-Modifiers are conditions which modify the search query operators (AND, "all", OR, etc). As indicated above, in version 1.2, they can either modify IndexQuery operators or Boolean Operators.
+Modifiers are conditions which modify the search query operators (AND, "all", OR, etc). As indicated above, in version 1.2, they can either modify SearchClause relations or Boolean Operators.
 
-Each modifier is preceeded by a '/' and optional spacing. One or many modifiers may be included. Modifiers must include a base_name, but MAY include a context_set, operator, and value.
+Each modifier is preceeded by a '/' and optional spacing. One or many modifiers may be included. Modifiers must include a base_name, but MAY include a context_set, comparison symbol, and value.
 
-From the LOC website, a modifier on a Boolean Operator looks like: `dc.title any fish or/rel.combine=sum dc.creator any sanderson`.
-A modifier on an IndexQuery looks like `any /relevant /cql.string`
+From the LOC website, a modifier on a Boolean Operator looks like: <br>
+`dc.title=fish or[/rel.combine=sum] dc.creator=sanderson`.<br>
+A modifier on a SearchClause relation looks like:<br> `any /relevant /cql.string`
 
-One thought of interest - it may be possible to include a LITERAL instead of a modifier for custom modifiers / modifier formats not available through this program. I've not tested it, but it's likely to work.
+One thought of interest - it may be possible to include a RawCQL instead of a modifier if you want to create custom modifiers or modifier formats not available through this program. I've not tested it, but it's likely to work.
 
 #### USAGE
 
-This utility comes with 3 standard modifiers - AndOrNotModifier (for CQL Boolean Operators AND, OR, and NOT), ProxModifier (for CQL Boolean Operator PROX), and RelationModifier (for any IndexQuery relation).
+This utility comes with 3 standard modifiers - AndOrNotModifier (for CQL Boolean Operators AND, OR, and NOT), ProxModifier (for CQL Boolean Operator PROX), and RelationModifier (for any SearchClause relation).
 
 These modifiers differ mainly in validation. The ProxModifier limits the base_name to either 'unit' or 'distance', as these are the base names used by prox, and limits the values for the 'unit' base name in the CQL context set to the values specified in the LOC documentation. Upon validation, an error will be raised if these values are not correct.
 
-This program will NOT validate modifiers in relation to one another - e.g., even though a prox must have one 'unit' and one 'distance' modifier, this is not enforced through validation. You could extend the CQLBooleanOperatorBase or PROX class to create this custom validation, if desired.
+This program will NOT validate combinations of modifiers - e.g., even though a 'PROX' boolean operator must have one 'unit' and one 'distance' modifier, this is not enforced through validation. You could extend the CQLBooleanOperatorBase or PROX class to create this custom validation, if desired.
 
 Example prox modifier:
-`ProxModifier('unit', "=", "sentence", context_set="cql")`
-\*Using the keyword for context set here is optional. I'm just showing it to make the order clear - it's rearranged slightly as compared to an IndexQuery.
+`ProxModifier('cql', 'unit', "=", "sentence")`
+\*Using the keyword for context set here is optional. I'm just showing it to make the order clear - it's rearranged slightly as compared to a SearchClause.
 
 The RelationModifier works in the same way.
 
-Modifiers are added as an array to either IndexQueries or CQLBooleanOperatorBase classes.
+Modifiers are added as an array to either SearchClauses or CQLBooleanOperatorBase classes.
 
 #### AVAILABLE FUNCTIONS
 
 There are no functions here that the general user should need to use.
 
 #### INITIALIZATION OPTIONS
 
 It is not recommended to change any options manually after initializing a Modifier, as this will bypass some validation. It's easy and not resource intensive to create a new instance of a modifier if you need different options.
 
-| Option      | Data Type      | Mandatory | Description                                                                                                             |
-| ----------- | -------------- | --------- | ----------------------------------------------------------------------------------------------------------------------- |
-| base_name   | string         | Yes       | The base name of the modifier (e.g, 'relevant' in `/relevant`). Validated against the whitelist 'supported_base_names'. |
-| operator    | string or None | No        | The operator used in the modifier condition.                                                                            |
-| value       | string or None | No        | The value used in the modifier condition.                                                                               |
-| context_set | string or None | No        | The context set that the base_name should be pulled from.                                                               |
+| Option            | Data Type      | Mandatory | Description                                                     |
+| ----------------- | -------------- | --------- | --------------------------------------------------------------- |
+| context_set       | string or None | No        | The context set that the base_name should be pulled from.       |
+| base_name         | string         | Yes       | The base name of the modifier (e.g, 'relevant' in `/relevant`). |
+| comparison_symbol | string or None | No        | The comparison symbol used in the modifier condition.           |
+| value             | string or None | No        | The value used in the modifier condition.                       |
 
-COMBINATIONS OF INITIALIZATION PROPERTIES (implied from LOC standards):
+COMBINATIONS OF INITIALIZATION PROPERTIES (implied from LOC standards):<br>
 You MUST include either:
 
 1. a base_name,
-2. a context_set, base_name
-3. a base_name, operation, and value,
-4. a context_set, base_name, operation, and value.
+2. a context_set and base_name
+3. a base_name, comparison_symbol, and value,
+4. a context_set, base_name, comparison_symbol, and value.
+
+<br>
+<br>
 
 ### Sorting in 1.2: SortBy clauses
 
 sortBy clauses are simply Python dictionaries with the form:
 `{ "index_set": "alma", "index_name": "creator", "sort_order": "ascending" }`
 Which will be formatted to:
 `sortBy%20alma.creator/sort.ascending`
 
 All values are required. The sort_order can either be "ascending" or "descending."
 
-You should add all desired sortBy clauses to the Query object in an array with the keyword argument 'sort_queries='
+You should add all desired sortBy clauses to the SRUQueryer.search_retrieve or SRUQueryer.construct_search_retrieve_request in an array with the keyword argument 'sort_queries='
+
+<br>
+<br>
 
 ### Sorting in 1.1: SortKey
 
 `from sru_queryer.sru import SortKey`
 
-SortKeys are used to sort results returned by a searchRetrieve request ins SRU version 1.1. SRU 1.1 doesn't specify whether sorting is allow per-index like 1.2 does; rather, it specifies this per record schema.
+SortKeys are used to sort results returned by a searchRetrieve request in SRU version 1.1. SRU 1.1 doesn't specify whether sorting is allow per-index like 1.2 does; rather, it specifies this per record schema.
 
-Note that this isn't imported from CQL. It's actually not part of the CQL query - it's another URL query string parameter.
+Note that this isn't imported from sru_queryer.cql but rather sru_queryer.sru. This is because it's actually not part of the CQL query.
 
 #### USAGE
 
-Simply include a list of SortKeys in the 'sort_queries' parameter of your Query object. They will be automatically validated and formatted.
+Simply include a list of SortKeys in the 'sort_queries' parameter of your SearchRetrieve object. They will be automatically validated and formatted.
 
 #### AVAILABLE FUNCTIONS
 
-There's nothing here that you would need to use; the built-in functions are used by other parts of the SRUUtil program.
+There's nothing here that you would need to use; the built-in functions are used by other parts of the sru_queryer library.
 
 #### INITIALIZATION OPTIONS
 
 | Option         | Data Type | Mandatory | Description                                                                                            |
 | -------------- | --------- | --------- | ------------------------------------------------------------------------------------------------------ |
 | xpath          | string    | Yes       | The xpath of the index you want to sort by. It's just the index name prefixed by the context set.      |
 | schema         | string    | No        | The record schema you want to search by                                                                |
 | ascending      | boolean   | No        | Whether you want the results to be ascending. Default is True, False will set results to be descending |
 | case_sensitive | boolean   | No        | If case should be important during the search. Default is False.                                       |
+
+<br>
+<br>
+
+---
+
+## Known Incompatibilities
+
+Different SRU servers have quirks to their default behaviors, and don't all fully implement the Library of Congress standard on SRU.
+
+Additionally, I haven't been able to test some of the more advanced features of this library, namely the PROX modifier, relation modifiers, and boolean operator modifiers successfully on an SRU server. I've tried to test with 3 SRU servers, and I've never gotten the queries to work properly, even when trying them by hand in the browser URL bar. Even when I use the exact sample from the Library of Congress SRU documentation on the Library of Congress SRU server, it returns errors. However, all the queries that this library creates meet up to the documentation, so I'm hopeful that these features will work if there's a SRU server that supports them. Thankfully, I've been able to test most of the core functionality of the library.
+
+If you know of a valid RelationModifier, BooleanOperatorModifier, or PROX request and have the capability to test it, it would be much appreciated! Part of my issue simply comes from the fact that I don't really know all the use cases for these features, which limits my testing to only one or two. We also need the SRU version 1.1 SortKey functionality to be tested, but again don't have the capability.
+
+Below are a few of the issues I've found.
+
+<br>
+
+### ExLibris Alma SRU server
+
+❌ PROX boolean operator <br>
+❌ NOT boolean operator <br>
+❌ Multiple sort queries (only one supported)
+
+❓ Boolean Operator Modifiers <br>
+❓ RelationModifiers
+
+### Library of Congress SRU server
+
+❌ PROX boolean operator <br>
+❌ Sorting (in either version 1.1 or 1.2) <br>
+❌ Default context set
+
+⚠️ You must include maximum_records in a searchRetrieve query to get any records in return <br>
+⚠️ This server lists BIBFRAME as an available record schema, but fails when requesting it
+
+❓ RelationModifiers <br>
+❓ Boolean Operator Modifiers
+
+### Georgia Public Library 'Public Information Network for Electronic Services' (GAPINES)
+
+⚠️ PROX boolean operator doesn't return an error, but doesn't seem to affect results <br>
+⚠️ Sorting doesn't return an error, but doesn't seem to affect results
+
+❓ RelationModifiers <br>
+❓ Boolean Operator Modifiers
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sru_queryer-1.0.3/src/sru_queryer.egg-info/SOURCES.txt` & `sru_queryer-2.0.0/src/sru_queryer.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 LICENSE
 pyproject.toml
 readme.md
 src/sru_queryer/__init__.py
 src/sru_queryer/cql.py
-src/sru_queryer/drivers.py
+src/sru_queryer/exceptions.py
 src/sru_queryer/sru.py
 src/sru_queryer.egg-info/PKG-INFO
 src/sru_queryer.egg-info/SOURCES.txt
 src/sru_queryer.egg-info/dependency_links.txt
 src/sru_queryer.egg-info/requires.txt
 src/sru_queryer.egg-info/top_level.txt
 src/sru_queryer/_base/__init__.py
 src/sru_queryer/_base/_cql_boolean_operators.py
-src/sru_queryer/_base/_cql_literal.py
 src/sru_queryer/_base/_cql_modifiers.py
-src/sru_queryer/_base/_drivers.py
-src/sru_queryer/_base/_query.py
-src/sru_queryer/_base/_search_index_config.py
+src/sru_queryer/_base/_exceptions.py
+src/sru_queryer/_base/_raw_cql.py
+src/sru_queryer/_base/_search_clause.py
+src/sru_queryer/_base/_search_retrieve.py
 src/sru_queryer/_base/_sort_key.py
 src/sru_queryer/_base/_sru_aux_formatter.py
 src/sru_queryer/_base/_sru_configuration.py
-src/sru_queryer/_base/_sru_explain_xml_parser.py
-src/sru_queryer/_base/_sru_util.py
+src/sru_queryer/_base/_sru_explain_auto_parser.py
+src/sru_queryer/_base/_sru_queryer.py
 src/sru_queryer/_base/_sru_validator.py
 tests/test_cql_boolean_operators.py
-tests/test_cql_literal.py
 tests/test_cql_modifiers.py
-tests/test_search_index_config.py
+tests/test_raw_cql.py
+tests/test_search_clause.py
+tests/test_search_retrieve.py
 tests/test_sort_key.py
 tests/test_sru_aux_formatter.py
-tests/test_sru_explain_xml_parser.py
-tests/test_sru_query.py
-tests/test_sru_util.py
+tests/test_sru_explain_auto_parser.py
+tests/test_sru_queryer.py
 tests/test_sru_validator.py
```

### Comparing `sru_queryer-1.0.3/tests/test_cql_modifiers.py` & `sru_queryer-2.0.0/tests/test_cql_modifiers.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,39 +4,39 @@
 from src.sru_queryer.cql import CQLModifierBase
 
 from tests.testData.test_data import get_alma_sru_configuration
 
 class TestCQLModifiers(unittest.TestCase):
 
     def test_format_cql_modifier_base_only(self):
-        cql_modifier = CQLModifierBase("relevant")
+        cql_modifier = CQLModifierBase(base_name="relevant")
 
         self.assertEqual(cql_modifier.format(), "/relevant")
 
     def test_format_cql_modifier_with_context_set(self):
-        cql_modifier = CQLModifierBase("unit", context_set="alma")
+        cql_modifier = CQLModifierBase("alma", "unit")
 
         self.assertEqual(cql_modifier.format(), "/alma.unit")
 
     def test_format_cql_modifier_with_operator_and_value(self):
-        cql_modifier = CQLModifierBase("unit", "<>", "street")
+        cql_modifier = CQLModifierBase(None, "unit", "<>", "street")
 
         self.assertEqual(cql_modifier.format(), '/unit<>"street"')
 
     def test_initializing_cql_modifier_operator_no_value_throws_error(self):
         with self.assertRaises(ValueError) as ve:
-            cql_modifier = CQLModifierBase("unit", "=")
+            cql_modifier = CQLModifierBase(None, "unit", "=", None)
 
     def test_initializing_cql_modifier_value_no_operator_throws_error(self):
         with self.assertRaises(ValueError) as ve:
-            cql_modifier = CQLModifierBase("unit", value="3")
+            cql_modifier = CQLModifierBase(None, "unit", None, value="3")
 
     def test_initializing_cql_modifier_unsupported_operator(self):
         with self.assertRaises(ValueError) as ve:
-            cql_modifier = CQLModifierBase("unit", "+", "Hippo")
+            cql_modifier = CQLModifierBase(None, "unit", "+", "Hippo")
 
         self.assertEqual(ve.exception.__str__(),
                          "Operator '+' is not supported.")
 
     def test_validate_base_name_invalid_name_raises_error(self):
         with self.assertRaises(ValueError) as ve:
             CQLModifierBase._validate_base_name(
@@ -47,15 +47,15 @@
 
     def test_validate_base_name_no_restriction_no_error(self):
         CQLModifierBase._validate_base_name(
             "not_unit_or_distance", "any", "Boom")
 
     def test_invalid_operator_raises_error(self):
         with self.assertRaises(ValueError) as ve:
-            CQLModifierBase._validate_operator(
+            CQLModifierBase._validate_comparison_symbol(
                 "++", [">", "=="])
 
         self.assertEqual(ve.exception.__str__(),
                          "Operator '++' is not supported.")
 
     def test_value_allowed_for_base_name_in_context_set_no_limitations(self):
         CQLModifierBase._check_if_value_allowed_for_base_name_in_context_set(
@@ -101,43 +101,43 @@
         CQLModifierBase._check_if_value_allowed_for_base_name_in_context_set(
             "test_set", "texture", None, limitations)
 
     def test_prox_modifier_restrict_unit_values_in_default_context_invalid_value_raises_error(self):
         """Integration test"""
         sru_configuration = get_alma_sru_configuration()
         
-        prox_modifier = ProxModifier(
+        prox_modifier = ProxModifier(None,
             "unit", "=", "invalid value")
 
         with self.assertRaises(ValueError) as ve:
             prox_modifier.validate(sru_configuration)
 
         self.assertIn("invalid value", ve.exception.__str__())
 
     def test_prox_modifier_restrict_unit_values_in_valid_context_not_specified_no_error(self):
         """Integration test"""
         sru_configuration = get_alma_sru_configuration()
-        prox_modifier = ProxModifier(
-            "unit", "=", "invalid value", "alma")
+        prox_modifier = ProxModifier("alma",
+            "unit", "=", "invalid value")
 
         prox_modifier.validate(sru_configuration)
 
     def test_proper_format_two_simple_modifiers(self):
-        modifiers = [AndOrNotModifier("relevant"), AndOrNotModifier("simple")]
+        modifiers = [AndOrNotModifier(base_name="relevant"), AndOrNotModifier(base_name="simple")]
 
         actual_formatted_operator = CQLModifierBase.format_modifier_array(
             modifiers)
 
         expected_formatted_operator = '/relevant%20/simple%20'
 
         self.assertEqual(actual_formatted_operator,
                          expected_formatted_operator)
 
     def test_proper_format_two_simple_modifier_with_padding(self):
-        modifiers = [AndOrNotModifier("relevant"), AndOrNotModifier("simple")]
+        modifiers = [AndOrNotModifier(base_name="relevant"), AndOrNotModifier(base_name="simple")]
 
         actual_formatted_operator = CQLModifierBase.format_modifier_array(
             modifiers)
 
         expected_formatted_operator = '/relevant%20/simple%20'
 
         self.assertEqual(actual_formatted_operator,
```

### Comparing `sru_queryer-1.0.3/tests/test_search_index_config.py` & `sru_queryer-2.0.0/tests/test_search_clause.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,105 +1,114 @@
 import unittest
 
-from src.sru_queryer.cql import IndexQuery
+from src.sru_queryer.cql import SearchClause
 from src.sru_queryer.cql import RelationModifier
 from tests.testData.test_data import get_alma_sru_configuration
 
-class TestIndexQuery(unittest.TestCase):
+class TestSearchClause(unittest.TestCase):
 
     def test_format_with_all_query(self):
-        search_index_config = IndexQuery("alma", "test_attribute", "all", "")
+        search_index_config = SearchClause("alma", "test_attribute", "all", "")
 
-        formatted_search_index_config = search_index_config.format()
+        formatted_search_clause = search_index_config.format()
 
-        self.assertEqual(formatted_search_index_config,
+        self.assertEqual(formatted_search_clause,
                          'alma.test_attribute%20all%20""')
 
-    def test_create_index_query_index_no_operator_throws_error(self):
+    def test_create_search_clause_index_no_operator_throws_error(self):
         with self.assertRaises(ValueError):
-            IndexQuery(value="", index_name="test_attribute",
+            SearchClause(search_term="", index_name="test_attribute",
                        context_set="alma")
 
-    def test_create_index_query_operator_no_index_throws_error(self):
+    def test_create_search_clause_operator_no_index_throws_error(self):
         with self.assertRaises(ValueError):
-            IndexQuery(value="", operation="=", context_set="alma")
+            SearchClause(search_term="", relation="=", context_set="alma")
 
-    def test_create_index_query_context_set_no_index_name_throws_error(self):
+    def test_create_search_clause_context_set_no_index_name_throws_error(self):
         with self.assertRaises(ValueError):
-            IndexQuery(value="", context_set="alma")
+            SearchClause(search_term="", context_set="alma")
 
-    def test_create_index_query_value_none_throws_error(self):
+    def test_create_search_clause_no_search_term_throws_error(self):
         with self.assertRaises(ValueError):
-            IndexQuery(value=None, index_name="test_attribute",
-                       operation="all", context_set="alma")
+            SearchClause(search_term=None, index_name="test_attribute",
+                       relation="all", context_set="alma")
 
     def test_format_with_all_query_2(self):
-        search_index_config = IndexQuery(
-            context_set="alma", index_name="test_attribute", operation="all", value="hello*")
+        search_index_config = SearchClause(
+            context_set="alma", index_name="test_attribute", relation="all", search_term="hello*")
 
-        formatted_search_index_config = search_index_config.format()
+        formatted_search_clause = search_index_config.format()
 
-        self.assertEqual(formatted_search_index_config,
+        self.assertEqual(formatted_search_clause,
                          'alma.test_attribute%20all%20"hello*"')
+        
+    def test_format_with_any_keyword(self):
+        search_index_config = SearchClause(
+            context_set="alma", index_name="test_attribute", relation="any", search_term="hello*")
+
+        formatted_search_clause = search_index_config.format()
+
+        self.assertEqual(formatted_search_clause,
+                         'alma.test_attribute%20any%20"hello*"')
 
     def test_format_with_default_context(self):
-        search_index_config = IndexQuery(
-            value="10", index_name="bib_count", operation="==")
+        search_index_config = SearchClause(
+            search_term="10", index_name="bib_count", relation="==")
 
-        formatted_search_index_config = search_index_config.format()
+        formatted_search_clause = search_index_config.format()
 
-        self.assertEqual(formatted_search_index_config, 'bib_count=="10"')
+        self.assertEqual(formatted_search_clause, 'bib_count%20==%20"10"')
 
-    def test_format_with_only_value(self):
-        search_index_config = IndexQuery(value="10")
+    def test_format_with_only_search_term(self):
+        search_index_config = SearchClause(search_term="10")
 
-        formatted_search_index_config = search_index_config.format()
+        formatted_search_clause = search_index_config.format()
 
-        self.assertEqual(formatted_search_index_config, '"10"')
+        self.assertEqual(formatted_search_clause, '"10"')
 
     def test_validate_invalid_set(self):
         sru_configuration = get_alma_sru_configuration()
 
         with self.assertRaises(ValueError) as ve:
-            IndexQuery("puma", "bib_holding_count", ">", "15").validate(sru_configuration)
+            SearchClause("puma", "bib_holding_count", ">", "15").validate(sru_configuration)
 
         self.assertIn("'puma'", ve.exception.__str__())
         self.assertIn("not available", ve.exception.__str__())
 
     def test_validate_unsupported_index(self):
         sru_configuration = get_alma_sru_configuration()
         with self.assertRaises(ValueError) as ve:
-            IndexQuery("alma", "bib_count", "==", "10").validate(sru_configuration)
+            SearchClause("alma", "bib_count", "==", "10").validate(sru_configuration)
             
-    def test_validate_unsupported_operation(self):
+    def test_validate_unsupported_relation(self):
         sru_configuration = get_alma_sru_configuration()
 
         with self.assertRaises(ValueError) as ve:
-            IndexQuery("alma", "mms_id", "?", "10").validate(sru_configuration)
+            SearchClause("alma", "mms_id", "?", "10").validate(sru_configuration)
         
         self.assertIn("relation '?'", ve.exception.__str__().lower())
 
     def test_format_with_simple_modifier(self):
-        search_index_config = IndexQuery("alma", "test_attribute", "all", "hello", [RelationModifier("relevant")])
+        search_index_config = SearchClause("alma", "test_attribute", "all", "hello", [RelationModifier(base_name="relevant")])
 
-        formatted_search_index_config = search_index_config.format()
+        formatted_search_clause = search_index_config.format()
 
-        self.assertEqual(formatted_search_index_config, 'alma.test_attribute%20all/relevant%20"hello"')
+        self.assertEqual(formatted_search_clause, 'alma.test_attribute%20all/relevant%20"hello"')
 
     def test_validate_with_valid_modifier_integration(self):
         """Integration test."""
         sru_configuration = get_alma_sru_configuration()
 
-        search_index_config = IndexQuery("alma", "title", "all", "hello", [RelationModifier("relevant", context_set="alma")])
+        search_index_config = SearchClause("alma", "title", "all", "hello", [RelationModifier("alma", "relevant")])
 
         search_index_config.validate(sru_configuration)
 
     def test_validate_with_invalid_modifier_raises_error_integration(self):
         """Integration test."""
         sru_configuration = get_alma_sru_configuration()
         with self.assertRaises(ValueError) as ve:
-            search_index_config = IndexQuery("alma", "title", "all", "hello", [
-                                                RelationModifier("relevant", context_set="invalid_set_on_modifier")])
+            search_index_config = SearchClause("alma", "title", "all", "hello", [
+                                                RelationModifier("invalid_set_on_modifier", "relevant")])
             search_index_config.validate(sru_configuration)
 
         self.assertIn("'invalid_set_on_modifier'", ve.exception.__str__())
         self.assertIn("not available", ve.exception.__str__())
```

### Comparing `sru_queryer-1.0.3/tests/test_sort_key.py` & `sru_queryer-2.0.0/tests/test_sort_key.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.3/tests/test_sru_aux_formatter.py` & `sru_queryer-2.0.0/tests/test_sru_aux_formatter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+import logging
 
 from tests.testData.test_data import get_gapines_sru_configuration, get_alma_sru_configuration
 from src.sru_queryer._base._sru_aux_formatter import SRUAuxiliaryFormatter
 
 class TestSRUAuxiliaryFormatter(unittest.TestCase):
     def test_format_basic_access_authentication_header_payload(self, *args):
         username = "testusername01"
@@ -40,110 +41,110 @@
 
         actual_url = SRUAuxiliaryFormatter.format_base_explain_query(base_url, "1.1")
 
         self.assertEqual(expected_url, actual_url)
 
     def test_format_search_retrieve_query_start_record_not_default(self):
         sru_configuration = get_gapines_sru_configuration()
-        sru_configuration.search_retrieve_url = "https://example.com"
+        sru_configuration.server_url = "https://example.com"
         sru_configuration.sru_version = "1.2"
 
         actual_query = SRUAuxiliaryFormatter.format_base_search_retrieve_query(sru_configuration,
             start_record=7, maximum_records=10, record_schema="marcxml")
 
         expected_query = "https://example.com?version=1.2&operation=searchRetrieve&recordSchema=marcxml&startRecord=7&maximumRecords=10&query="
 
         self.assertEqual(actual_query, expected_query)
 
     def test_format_search_retrieve_query_maximum_records_not_default(self):
         sru_configuration = get_gapines_sru_configuration()
-        sru_configuration.search_retrieve_url = "https://example.com"
+        sru_configuration.server_url = "https://example.com"
         sru_configuration.sru_version = "1.2"
 
         actual_query = SRUAuxiliaryFormatter.format_base_search_retrieve_query(sru_configuration,
             start_record=1, maximum_records=7, record_schema="marcxml")
 
         expected_query = "https://example.com?version=1.2&operation=searchRetrieve&recordSchema=marcxml&startRecord=1&maximumRecords=7&query="
 
         self.assertEqual(actual_query, expected_query)
 
     def test_format_search_retrieve_query_version_1_1(self):
         sru_configuration = get_gapines_sru_configuration()
-        sru_configuration.search_retrieve_url = "https://example.com"
+        sru_configuration.server_url = "https://example.com"
         sru_configuration.sru_version = "1.1"
 
         actual_query = SRUAuxiliaryFormatter.format_base_search_retrieve_query(sru_configuration,
             start_record=1, maximum_records=10, record_schema="marcxml")
 
         expected_query = "https://example.com?version=1.1&operation=searchRetrieve&recordSchema=marcxml&startRecord=1&maximumRecords=10&query="
 
         self.assertEqual(actual_query, expected_query)
 
     def test_format_search_retrieve_query_default_record_schema(self):
         sru_configuration = get_gapines_sru_configuration()
-        sru_configuration.search_retrieve_url = "https://example.com"
+        sru_configuration.server_url = "https://example.com"
         sru_configuration.sru_version = "1.1"
 
         actual_query = SRUAuxiliaryFormatter.format_base_search_retrieve_query(sru_configuration,
             start_record=1, maximum_records=10)
 
         expected_query = "https://example.com?version=1.1&operation=searchRetrieve&recordSchema=marcxml&startRecord=1&maximumRecords=10&query="
 
         self.assertEqual(actual_query, expected_query)
 
     def test_format_search_retrieve_query_no_default_record_schema_or_user_defined_record_schema(self):
         sru_configuration = get_gapines_sru_configuration()
-        sru_configuration.search_retrieve_url = "https://example.com"
+        sru_configuration.server_url = "https://example.com"
         sru_configuration.sru_version = "1.1"
         sru_configuration.default_record_schema = None
 
         actual_query = SRUAuxiliaryFormatter.format_base_search_retrieve_query(sru_configuration,
             start_record=1, maximum_records=10)
 
         expected_query = "https://example.com?version=1.1&operation=searchRetrieve&startRecord=1&maximumRecords=10&query="
 
         self.assertEqual(actual_query, expected_query)
 
     def test_format_search_retrieve_query_no_user_defined_start_record(self):
         sru_configuration = get_gapines_sru_configuration()
-        sru_configuration.search_retrieve_url = "https://example.com"
+        sru_configuration.server_url = "https://example.com"
         sru_configuration.sru_version = "1.1"
 
         actual_query = SRUAuxiliaryFormatter.format_base_search_retrieve_query(sru_configuration, maximum_records=10)
 
         expected_query = "https://example.com?version=1.1&operation=searchRetrieve&recordSchema=marcxml&maximumRecords=10&query="
 
         self.assertEqual(actual_query, expected_query)
 
     def test_format_search_retrieve_query_no_user_defined_maximum_record_default_maximum_record(self):
         sru_configuration = get_gapines_sru_configuration()
-        sru_configuration.search_retrieve_url = "https://example.com"
+        sru_configuration.server_url = "https://example.com"
         sru_configuration.sru_version = "1.1"
 
         actual_query = SRUAuxiliaryFormatter.format_base_search_retrieve_query(sru_configuration)
 
         expected_query = "https://example.com?version=1.1&operation=searchRetrieve&recordSchema=marcxml&maximumRecords=10&query="
 
         self.assertEqual(actual_query, expected_query)
 
     def test_format_search_retrieve_query_no_user_defined_maximum_record_no_default_maximum_record(self):
         sru_configuration = get_gapines_sru_configuration()
-        sru_configuration.search_retrieve_url = "https://example.com"
+        sru_configuration.server_url = "https://example.com"
         sru_configuration.sru_version = "1.1"
         sru_configuration.default_records_returned = None
 
         actual_query = SRUAuxiliaryFormatter.format_base_search_retrieve_query(sru_configuration)
 
         expected_query = "https://example.com?version=1.1&operation=searchRetrieve&recordSchema=marcxml&query="
 
         self.assertEqual(actual_query, expected_query)
 
     def test_format_search_retrieve_query_record_packing(self):
         sru_configuration = get_alma_sru_configuration()
-        sru_configuration.search_retrieve_url = "https://example.com"
+        sru_configuration.server_url = "https://example.com"
         sru_configuration.sru_version = "1.1"
         sru_configuration.default_records_returned = None
 
         actual_query = SRUAuxiliaryFormatter.format_base_search_retrieve_query(sru_configuration, record_packing="xml")
 
         expected_query = "https://example.com?version=1.1&operation=searchRetrieve&recordPacking=xml&query="
```

### Comparing `sru_queryer-1.0.3/tests/test_sru_explain_xml_parser.py` & `sru_queryer-2.0.0/tests/test_sru_explain_auto_parser.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import unittest
 import xmltodict
 import json
-from unittest.mock import patch
 
-from src.sru_queryer._base._sru_explain_xml_parser import SRUExplainXMLParser
-from tests.testData.test_data import TestFiles, test_available_record_schemas, mock_searchable_indexes_and_descriptions
+from src.sru_queryer._base._exceptions import NoExplainResponseException
+from src.sru_queryer._base._sru_explain_auto_parser import SRUExplainAutoParser
+from tests.testData.test_data import TestFiles, test_available_record_schemas
 
-from src.sru_queryer.drivers import alma_driver, loc_driver, gapines_driver
-
-# Format returned by SRUExplainXMLParser's '_parse_config_info'
 gapines_test_parsed_config_info = {
     "default_context_set": "eg",
     "default_index": "keyword",
     "default_relation": "all",
     "default_record_schema": "marcxml",
     "default_sort_schema": "marcxml",
     "default_records_returned": 10,
@@ -26,376 +23,226 @@
     "default_record_schema": None,
     "default_sort_schema": None,
     "default_records_returned": 10,
     "max_records_supported": 50,
     "supported_relation_modifiers": []
 }
 
-class TestSRUExplainXMLParser(unittest.TestCase):
+class TestSRUExplainAutoParser(unittest.TestCase):
 
-    def test_parse_context_set_and_index_info_from_xml_alma(self):
+    def test_parse_context_set_and_index_info_from_alma(self):
         with open (TestFiles.explain_response_alma, "rb") as f:
 
             xml_unprocessed_dict = xmltodict.parse(f.read())
 
-            sru_xml_parser = SRUExplainXMLParser(xml_unprocessed_dict, driver=alma_driver)
-            xml_dict = sru_xml_parser._parse_raw_index_info_from_xml()
+            sru_dict_parser = SRUExplainAutoParser(xml_unprocessed_dict)
+            sru_configuration = sru_dict_parser.get_sru_configuration_from_explain_response()
 
-            with open (TestFiles.alma_raw_indexes, "r") as f:
+            with open (TestFiles.alma_available_context_sets_and_indexes, "r") as f:
                 expected_dict = json.loads(f.read())
 
-                self.assertListEqual(xml_dict, expected_dict)
+            self.assertDictEqual(sru_configuration.available_context_sets_and_indexes["alma"]["accompanying_material"], expected_dict["alma"]["accompanying_material"])
+            self.assertDictEqual(sru_configuration.available_context_sets_and_indexes, expected_dict)
 
-    def test_parse_context_set_and_index_info_from_xml_loc(self):
+    def test_parse_context_set_and_index_info_from_loc(self):
         with open (TestFiles.explain_response_loc, "rb") as f:
 
             xml_unprocessed_dict = xmltodict.parse(f.read())
 
-            sru_xml_parser = SRUExplainXMLParser(xml_unprocessed_dict, driver=loc_driver)
-            xml_dict = sru_xml_parser._parse_raw_index_info_from_xml()
+            sru_dict_parser = SRUExplainAutoParser(xml_unprocessed_dict)
+            sru_configuration = sru_dict_parser.get_sru_configuration_from_explain_response()
 
-            with open (TestFiles.loc_raw_indexes, "r") as f:
+            with open (TestFiles.loc_available_context_sets_and_indexes, "r") as f:
                 expected_dict = json.loads(f.read())
 
-                self.assertListEqual(xml_dict, expected_dict)
+            self.assertDictEqual(sru_configuration.available_context_sets_and_indexes["dc"]["author"], expected_dict["dc"]["author"])
+            self.assertDictEqual(sru_configuration.available_context_sets_and_indexes, expected_dict)
 
-    def test_parse_context_set_and_index_info_from_xml_gapines(self):
+    def test_parse_context_set_and_index_info_from_gapines(self):
         with open (TestFiles.explain_response_gapines, "rb") as f:
 
             xml_unprocessed_dict = xmltodict.parse(f.read())
 
-            sru_xml_parser = SRUExplainXMLParser(xml_unprocessed_dict, driver=gapines_driver)
-            xml_dict = sru_xml_parser._parse_raw_index_info_from_xml()
+            sru_dict_parser = SRUExplainAutoParser(xml_unprocessed_dict)
+            sru_configuration = sru_dict_parser.get_sru_configuration_from_explain_response()
 
-            with open (TestFiles.gapines_raw_indexes, "r") as f:
+            with open (TestFiles.gapines_available_context_sets_and_indexes, "r") as f:
                 expected_dict = json.loads(f.read())
 
-                self.assertListEqual(xml_dict, expected_dict)
-
-    def test_parse_schema_info_from_xml_gapines(self):
-        with open (TestFiles.explain_response_gapines, "rb") as f:
-
-            xml_unprocessed_dict = xmltodict.parse(f.read())
+            self.assertDictEqual(sru_configuration.available_context_sets_and_indexes["eg"]["author"], expected_dict["eg"]["author"])
+            self.assertDictEqual(sru_configuration.available_context_sets_and_indexes, expected_dict)
 
-            sru_xml_parser = SRUExplainXMLParser(xml_unprocessed_dict, driver=gapines_driver)
-            xml_dict = sru_xml_parser._parse_raw_schema_info_from_xml()
-            xml_dict = sru_xml_parser._parse_schema_info(xml_dict)
-
-    def test_parse_schema_info_from_xml_alma(self):
+    def test_parse_sru_version_from_dict_alma(self):
         with open (TestFiles.explain_response_alma, "rb") as f:
 
             xml_unprocessed_dict = xmltodict.parse(f.read())
 
-            sru_xml_parser = SRUExplainXMLParser(xml_unprocessed_dict, driver=alma_driver)
-            xml_dict = sru_xml_parser._parse_raw_schema_info_from_xml()
-
-            with open (TestFiles.alma_raw_schemas, "r") as f:
-                expected_dict = json.loads(f.read())
+            sru_dict_parser = SRUExplainAutoParser(xml_unprocessed_dict)
+            sc = sru_dict_parser.get_sru_configuration_from_explain_response()
 
-                self.assertListEqual(xml_dict, expected_dict)
+            self.assertEqual(sc.sru_version, "1.2")
 
-    def test_parse_schema_info_from_xml_loc(self):
+    def test_parse_sru_version_from_dict_loc(self):
         with open (TestFiles.explain_response_loc, "rb") as f:
 
             xml_unprocessed_dict = xmltodict.parse(f.read())
 
-            sru_xml_parser = SRUExplainXMLParser(xml_unprocessed_dict, driver=loc_driver)
-            xml_dict = sru_xml_parser._parse_raw_schema_info_from_xml()
-
-            with open (TestFiles.loc_raw_schemas, "r") as f:
-                expected_dict = json.loads(f.read())
-
-                self.assertListEqual(xml_dict, expected_dict)
-
-    def test_parse_config_info_from_xml_alma(self):
-        with open (TestFiles.explain_response_alma, "rb") as f:
-
-            xml_unprocessed_dict = xmltodict.parse(f.read())
-
-            sru_xml_parser = SRUExplainXMLParser(xml_unprocessed_dict, driver=alma_driver)
-            xml_dict = sru_xml_parser._parse_raw_config_info_from_xml()
+            sru_dict_parser = SRUExplainAutoParser(xml_unprocessed_dict)
+            sc = sru_dict_parser.get_sru_configuration_from_explain_response()
 
-            with open (TestFiles.alma_raw_config_info, "r") as f:
-                expected_dict = json.loads(f.read())
-
-                self.assertDictEqual(xml_dict, expected_dict)
+            self.assertEqual(sc.sru_version, "1.1")
 
-    def test_parse_config_info_from_xml_alma(self):
-        with open (TestFiles.explain_response_loc, "rb") as f:
-
-            xml_unprocessed_dict = xmltodict.parse(f.read())
-
-            sru_xml_parser = SRUExplainXMLParser(xml_unprocessed_dict, driver=loc_driver)
-            xml_dict = sru_xml_parser._parse_raw_config_info_from_xml()
-
-            self.assertIsNone(xml_dict)
-
-    def test_parse_config_info_from_xml_gapines(self):
+    def test_parse_sru_version_from_dict_gapines(self):
         with open (TestFiles.explain_response_gapines, "rb") as f:
 
             xml_unprocessed_dict = xmltodict.parse(f.read())
 
-            sru_xml_parser = SRUExplainXMLParser(xml_unprocessed_dict, driver=gapines_driver)
-            xml_dict = sru_xml_parser._parse_raw_config_info_from_xml()
-
-            with open (TestFiles.gapines_raw_config_info, "r") as f:
-                expected_dict = json.loads(f.read())
-
-                self.assertDictEqual(xml_dict, expected_dict)
+            sru_dict_parser = SRUExplainAutoParser(xml_unprocessed_dict)
+            sc = sru_dict_parser.get_sru_configuration_from_explain_response()
 
-    @staticmethod
-    def create_index_config(title, id, sort, supported_operations, empty_term_supported) -> dict:
-        return {
-                "id": id,
-                "title": title,
-                "sort": sort,
-                "supported_operations": supported_operations,
-                "empty_term_supported": empty_term_supported
-        }
-
-    def verify_index_config_info(self, index, expected_index):
-        self.assertEqual(index["title"], expected_index["title"], "Title Incorrect!")
-        self.assertEqual(index["id"], expected_index["id"], "ID Incorrect! ")
-        self.assertEqual(index["sort"], expected_index["sort"], "Sort Incorrect!")
-        self.assertListEqual(index["supported_operations"], expected_index["supported_operations"], "Supported Operations incorrect!")
-        self.assertEqual(index["empty_term_supported"], expected_index["empty_term_supported"], "Empty Term Supported Incorrect!")
-
-    def test_parse_available_context_set_and_index_info_from_xml_dict_alma(self):
-        with open (TestFiles.alma_raw_indexes, "r") as f:
-            explain_index_json = json.loads(f.read())
-
-            sru_xml_parser = SRUExplainXMLParser({}, driver=alma_driver)
-            available_context_set_and_index_info = sru_xml_parser._parse_available_context_sets_and_index_info(explain_index_json)
-            
-            self.verify_index_config_info(available_context_set_and_index_info["alma"]["bib_level"], {
-                "id": None,
-                "title": "Bibliographic Level",
-                "sort": False,
-                "supported_operations": ["==", "<>", "=", "all"],
-                "empty_term_supported": True
-            })
-
-            self.verify_index_config_info(available_context_set_and_index_info["alma"]["serviceType"], {
-                "id": None,
-                "title": "Service Type",
-                "sort": False,
-                "supported_operations": ["==", "<>", "=", "all"],
-                "empty_term_supported": True
-            })
-
-            self.verify_index_config_info(available_context_set_and_index_info["alma"]["main_pub_date"], {
-                "id": None,
-                "title": "Publication Year",
-                "sort": True,
-                "supported_operations": ["==", ">", ">=", "<", "<=", "<>", "=", "all"],
-                "empty_term_supported": False
-            })
-    
-    def test_parse_available_context_set_and_index_info_from_xml_dict_alma_different_set(self):
-        with open (TestFiles.alma_raw_indexes, "r") as f:
-            explain_index_json = json.loads(f.read())
-
-            sru_xml_parser = SRUExplainXMLParser({}, driver=alma_driver)
-            available_context_set_and_index_info = sru_xml_parser._parse_available_context_sets_and_index_info(explain_index_json)
-
-            index = available_context_set_and_index_info["rec"]["id"]
-            expected_index = self.create_index_config("Record Identifier (MMS ID)", None, False, ["==", ">", ">=", "<", "<=", "<>", "=", "all"], False)
-
-            self.verify_index_config_info(index, expected_index)
-
-    def test_parse_available_context_set_and_index_info_from_xml_dict_gapines(self):
-        with open(TestFiles.gapines_raw_indexes, "r") as f:
-            explain_index_json = json.loads(f.read())
-
-            sru_xml_parser = SRUExplainXMLParser({}, driver=gapines_driver)
-            available_context_set_and_index_info = sru_xml_parser._parse_available_context_sets_and_index_info(explain_index_json)
-
-            index = available_context_set_and_index_info["bib"]["nameconference"]
-            expected_index = self.create_index_config(title="nameconference", id="bib.nameconference", sort=None, supported_operations=[], empty_term_supported=None)
-
-            self.verify_index_config_info(index, expected_index=expected_index)
-
-    def test_parse_available_context_set_and_index_info_from_xml_dict_loc(self):
-        with open(TestFiles.loc_raw_indexes, "r") as f:
-            explain_index_json = json.loads(f.read())
-
-            sru_xml_parser = SRUExplainXMLParser({}, driver=loc_driver)
-            available_context_set_and_index_info = sru_xml_parser._parse_available_context_sets_and_index_info(explain_index_json)
-
-            index = available_context_set_and_index_info["cql"]["anywhere"]
-            expected_index = self.create_index_config("Keyword Anywhere", "1016", None, [], None)
-
-            self.verify_index_config_info(index, expected_index=expected_index)
+            self.assertEqual(sc.sru_version, "1.1")
 
     def test_parse_config_info_alma(self):
-        with open(TestFiles.alma_raw_config_info, "r") as f:
-            explain_index_json = json.loads(f.read())
+        with open(TestFiles.explain_response_alma, "rb") as f:
+            explain_response = xmltodict.parse(f.read())
 
-            sru_xml_parser = SRUExplainXMLParser({}, driver=alma_driver)
-            config_info = sru_xml_parser._parse_config_info(explain_index_json)
+            sru_dict_parser = SRUExplainAutoParser(explain_response)
+            sc = sru_dict_parser.get_sru_configuration_from_explain_response()
 
-            self.assertDictEqual(config_info, alma_test_parsed_config_info)
+            self.assertEqual(sc.default_context_set, alma_test_parsed_config_info["default_context_set"])
+            self.assertEqual(sc.default_index, alma_test_parsed_config_info["default_index"])
+            self.assertEqual(sc.default_relation, alma_test_parsed_config_info["default_relation"])
+            self.assertEqual(sc.default_record_schema, alma_test_parsed_config_info["default_record_schema"])
+            self.assertEqual(sc.default_records_returned, alma_test_parsed_config_info["default_records_returned"])
+            self.assertEqual(sc.max_records_supported, alma_test_parsed_config_info["max_records_supported"])
+            self.assertListEqual(sc.supported_relation_modifiers, alma_test_parsed_config_info["supported_relation_modifiers"])
 
     def test_parse_config_info_gapines(self):
-        with open(TestFiles.gapines_raw_config_info, "r") as f:
-            explain_index_json = json.loads(f.read())
+        with open(TestFiles.explain_response_gapines, "rb") as f:
+            explain_response = xmltodict.parse(f.read())
 
-            sru_xml_parser = SRUExplainXMLParser({}, driver=gapines_driver)
-            config_info = sru_xml_parser._parse_config_info(explain_index_json)
+            sru_dict_parser = SRUExplainAutoParser(explain_response)
+            sc = sru_dict_parser.get_sru_configuration_from_explain_response()
 
-            self.assertDictEqual(config_info, gapines_test_parsed_config_info)
+            self.assertEqual(sc.default_context_set, gapines_test_parsed_config_info["default_context_set"])
+            self.assertEqual(sc.default_index, gapines_test_parsed_config_info["default_index"])
+            self.assertEqual(sc.default_relation, gapines_test_parsed_config_info["default_relation"])
+            self.assertEqual(sc.default_record_schema, gapines_test_parsed_config_info["default_record_schema"])
+            self.assertEqual(sc.default_records_returned, gapines_test_parsed_config_info["default_records_returned"])
+            self.assertEqual(sc.max_records_supported, gapines_test_parsed_config_info["max_records_supported"])
+            self.assertListEqual(sc.supported_relation_modifiers, gapines_test_parsed_config_info["supported_relation_modifiers"])
 
-    def test_parse_config_info_loc(self):
-        sru_xml_parser = SRUExplainXMLParser({}, driver=loc_driver)
-        config_info = sru_xml_parser._parse_config_info(None)
+    def test_parse_schema_info_alma(self):
+        with open(TestFiles.explain_response_alma, "rb") as f:
+            alma_dict = xmltodict.parse(f.read())
 
-        self.assertIsNone(config_info)
+            sru_dict_parser = SRUExplainAutoParser(alma_dict)
+            sc = sru_dict_parser.get_sru_configuration_from_explain_response()
 
-    def test_parse_schema_info_alma(self):
-        with open(TestFiles.alma_raw_schemas, "r") as f:
-            record_schema_info = json.loads(f.read())
+            for record_schema_name in test_available_record_schemas.keys():
+                self.assertTrue(record_schema_name in sc.available_record_schemas.keys(), "Parsed record schemas are missing an expected record schema.")
+                self.assertDictEqual(test_available_record_schemas[record_schema_name], sc.available_record_schemas[record_schema_name], "An expected record schema does not match an actual record schema.")
 
-            sru_xml_parser = SRUExplainXMLParser({}, driver=alma_driver)
+            self.assertEqual(len(sc.available_record_schemas), 8)
+
+    def test_parse_schema_info_loc(self):
+        with open(TestFiles.explain_response_loc, "rb") as f:
+            loc_dict = xmltodict.parse(f.read())
 
-            parsed_record_schema_info = sru_xml_parser._parse_schema_info(record_schema_info)
+            sru_dict_parser = SRUExplainAutoParser(loc_dict)
+            sc = sru_dict_parser.get_sru_configuration_from_explain_response()
 
-            parsed_stringified_available_record_schemas = json.dumps(parsed_record_schema_info)
-            for record_schema in test_available_record_schemas:
-                stringified_record_schema = json.dumps(record_schema)
-                self.assertTrue(stringified_record_schema in parsed_stringified_available_record_schemas)
+            self.assertEqual(len(sc.available_record_schemas), 4)
 
-            self.assertEqual(len(parsed_record_schema_info), 16)
+    def test_bad_explain_response_loc_raises_exception(self):
+        with open(TestFiles.loc_bad_explain_response, "rb") as f:
+            bad_response_dict = xmltodict.parse(f.read())
 
-    def test_parse_schema_info_loc(self):
-        with open(TestFiles.loc_raw_schemas, "r") as f:
-            record_schema_info = json.loads(f.read())
+            sru_dict_parser = SRUExplainAutoParser(bad_response_dict)
 
-            sru_xml_parser = SRUExplainXMLParser({}, driver=loc_driver)
+            with self.assertRaises(NoExplainResponseException) as e:
+                sc = sru_dict_parser.get_sru_configuration_from_explain_response()
 
-            parsed_record_schema_info = sru_xml_parser._parse_schema_info(record_schema_info)
+    def test_bad_explain_response_alma_raises_exception(self):
+        with open(TestFiles.alma_bad_explain_response, "rb") as f:
+            bad_response_dict = xmltodict.parse(f.read())
 
-            self.assertEqual(len(parsed_record_schema_info), 8)
+            sru_dict_parser = SRUExplainAutoParser(bad_response_dict)
 
-    @patch('src.sru_queryer._base._sru_explain_xml_parser.SRUExplainXMLParser._parse_raw_index_info_from_xml')
-    @patch('src.sru_queryer._base._sru_explain_xml_parser.SRUExplainXMLParser._parse_raw_schema_info_from_xml')
-    @patch('src.sru_queryer._base._sru_explain_xml_parser.SRUExplainXMLParser._parse_raw_config_info_from_xml')
-    @patch('src.sru_queryer._base._sru_explain_xml_parser.SRUExplainXMLParser._parse_schema_info')
-    @patch('src.sru_queryer._base._sru_explain_xml_parser.SRUExplainXMLParser._parse_available_context_sets_and_index_info')
-    @patch('src.sru_queryer._base._sru_explain_xml_parser.SRUExplainXMLParser._parse_config_info')
-    def test_construct_sru_configuration_alma(self, mock_parse_config_info, mock_parse_index_info, mock_parse_schema_info, *args):
-        mock_parse_config_info.return_value = alma_test_parsed_config_info
-        # The following two mock values aren't exactly what Alma returns, but should approximate it.
-        mock_parse_index_info.return_value = mock_searchable_indexes_and_descriptions
-        mock_parse_schema_info.return_value = test_available_record_schemas
-
-        sru_xml_parser = SRUExplainXMLParser({}, driver=alma_driver)
-
-        configuration = sru_xml_parser.get_sru_configuration_from_explain_response()
-
-        self.assertDictEqual(configuration.available_context_sets_and_indexes, mock_searchable_indexes_and_descriptions)
-        self.assertDictEqual(configuration.available_record_schemas, test_available_record_schemas)
-        self.assertListEqual(configuration.supported_relation_modifiers, [])
-        self.assertEqual(configuration.default_context_set, None)
-        self.assertEqual(configuration.default_index, None)
-        self.assertEqual(configuration.default_relation, None)
-        self.assertEqual(configuration.default_record_schema, None)
-        self.assertEqual(configuration.default_sort_schema, None)
-        self.assertEqual(configuration.default_records_returned, 10)
-        self.assertEqual(configuration.max_records_supported, 50)
-
-    @patch('src.sru_queryer._base._sru_explain_xml_parser.SRUExplainXMLParser._parse_raw_index_info_from_xml')
-    @patch('src.sru_queryer._base._sru_explain_xml_parser.SRUExplainXMLParser._parse_raw_schema_info_from_xml')
-    @patch('src.sru_queryer._base._sru_explain_xml_parser.SRUExplainXMLParser._parse_raw_config_info_from_xml')
-    @patch('src.sru_queryer._base._sru_explain_xml_parser.SRUExplainXMLParser._parse_schema_info')
-    @patch('src.sru_queryer._base._sru_explain_xml_parser.SRUExplainXMLParser._parse_available_context_sets_and_index_info')
-    @patch('src.sru_queryer._base._sru_explain_xml_parser.SRUExplainXMLParser._parse_config_info')
-    def test_construct_sru_configuration_gapines_config_info(self, mock_parse_config_info, mock_parse_index_info, mock_parse_schema_info, *args):
-        # Only tests properly parsing the Gapines CONFIG info. Other stuff is
-        # simply there to allow the test to work
-        mock_parse_config_info.return_value = gapines_test_parsed_config_info
-        mock_parse_index_info.return_value = mock_searchable_indexes_and_descriptions
-        mock_parse_schema_info.return_value = test_available_record_schemas
-
-        sru_xml_parser = SRUExplainXMLParser({}, driver=gapines_driver)
-
-        configuration = sru_xml_parser.get_sru_configuration_from_explain_response()
-
-        self.assertListEqual(configuration.supported_relation_modifiers, ["relevant", "stem", "fuzzy", "word"])
-        self.assertEqual(configuration.default_context_set, "eg")
-        self.assertEqual(configuration.default_index, "keyword")
-        self.assertEqual(configuration.default_relation, "all")
-        self.assertEqual(configuration.default_record_schema, "marcxml")
-        self.assertEqual(configuration.default_sort_schema, "marcxml")
-        self.assertEqual(configuration.default_records_returned, 10)
-        self.assertEqual(configuration.max_records_supported, 50)
+            with self.assertRaises(NoExplainResponseException) as e:
+                sc = sru_dict_parser.get_sru_configuration_from_explain_response()
 
     def test_construct_sru_configuration_integration_alma(self):
         with open(TestFiles.explain_response_alma, "rb") as f:
             xml_dict = xmltodict.parse(f.read())
-            sru_xml_parser = SRUExplainXMLParser(xml_dict, driver=alma_driver)
-            configuration = sru_xml_parser.get_sru_configuration_from_explain_response()
+            sru_dict_parser = SRUExplainAutoParser(xml_dict)
+            configuration = sru_dict_parser.get_sru_configuration_from_explain_response()
 
             # Check if each record schema is in the parsed record schemas
             # (The test_available_record_schemas are a subset of what's included in 
             # explain_response_alma)
-            parsed_stringified_available_record_schemas = json.dumps(configuration.available_record_schemas)
-            for record_schema in test_available_record_schemas:
-                stringified_record_schema = json.dumps(record_schema)
-                self.assertTrue(stringified_record_schema in parsed_stringified_available_record_schemas)
+            for record_schema_name in test_available_record_schemas.keys():
+                self.assertTrue(record_schema_name in configuration.available_record_schemas.keys(), "Parsed record schemas are missing an expected record schema.")
+                self.assertDictEqual(test_available_record_schemas[record_schema_name], configuration.available_record_schemas[record_schema_name], "An expected record schema does not match an actual record schema.")
 
             self.assertListEqual(configuration.supported_relation_modifiers, [])
             self.assertEqual(configuration.default_context_set, None)
             self.assertEqual(configuration.default_index, None)
             self.assertEqual(configuration.default_relation, None)
             self.assertEqual(configuration.default_record_schema, None)
             self.assertEqual(configuration.default_sort_schema, None)
             self.assertEqual(configuration.default_records_returned, 10)
             self.assertEqual(configuration.max_records_supported, 50)
+            self.assertEqual(configuration.sru_version, "1.2")
 
             with open(TestFiles.alma_available_context_sets_and_indexes, "r") as f2:
                 expected_indexes = json.loads(f2.read())
 
                 self.assertDictEqual(configuration.available_context_sets_and_indexes, expected_indexes)
 
     def test_construct_sru_configuration_integration_gapines(self):
         with open(TestFiles.explain_response_gapines, "rb") as f:
             with open(TestFiles.gapines_available_context_sets_and_indexes, "r") as f2:
                 expected_indexes = json.loads(f2.read())
 
                 xml_dict = xmltodict.parse(f.read())
-                sru_xml_parser = SRUExplainXMLParser(xml_dict, driver=gapines_driver)
-                configuration = sru_xml_parser.get_sru_configuration_from_explain_response()
+                sru_dict_parser = SRUExplainAutoParser(xml_dict)
+                configuration = sru_dict_parser.get_sru_configuration_from_explain_response()
 
-                self.assertDictEqual({'marcxml': {'sort': True}, 'info:srw/schema/1/marcxml-v1.1': {'sort': True}}, configuration.available_record_schemas)
+                self.assertDictEqual({'marcxml': {'sort': True, "identifier": "info:srw/schema/1/marcxml-v1.1"}}, configuration.available_record_schemas)
                 self.assertDictEqual(configuration.available_context_sets_and_indexes, expected_indexes)
                 self.assertListEqual(configuration.supported_relation_modifiers, ["relevant", "stem", "fuzzy", "word"])
                 self.assertEqual(configuration.default_context_set, "eg")
                 self.assertEqual(configuration.default_index, "keyword")
                 self.assertEqual(configuration.default_relation, "all")
                 self.assertEqual(configuration.default_record_schema, "marcxml")
                 self.assertEqual(configuration.default_sort_schema, "marcxml")
                 self.assertEqual(configuration.default_records_returned, 10)
                 self.assertEqual(configuration.max_records_supported, 50)
+                self.assertEqual(configuration.sru_version, "1.1")
 
     def test_construct_sru_configuration_integration_loc(self):
         with open(TestFiles.explain_response_loc, "rb") as f:
             xml_dict = xmltodict.parse(f.read())
-            sru_xml_parser = SRUExplainXMLParser(xml_dict, driver=loc_driver)
-            configuration = sru_xml_parser.get_sru_configuration_from_explain_response()
+            sru_dict_parser = SRUExplainAutoParser(xml_dict)
+            configuration = sru_dict_parser.get_sru_configuration_from_explain_response()
+
 
-            stringified_available_record_schemas = json.dumps(configuration.available_record_schemas)
-            self.assertTrue(json.dumps({"marcxml": {"sort": False}}).strip("{}") in stringified_available_record_schemas)
-            self.assertTrue(json.dumps({"http://www.loc.gov/MARC21/slim": {"sort": False}}).strip("{}") in stringified_available_record_schemas)
+            self.assertTrue("marcxml" in configuration.available_record_schemas.keys(), "Parsed record schemas are missing an expected record schema.")
+            self.assertDictEqual({"sort": False, "identifier": "http://www.loc.gov/MARC21/slim"}, configuration.available_record_schemas["marcxml"], "An expected record schema does not match an actual record schema.")
 
             self.assertListEqual(configuration.supported_relation_modifiers, [])
             self.assertEqual(configuration.default_context_set, None)
             self.assertEqual(configuration.default_index, None)
             self.assertEqual(configuration.default_relation, None)
             self.assertEqual(configuration.default_record_schema, None)
             self.assertEqual(configuration.default_sort_schema, None)
             self.assertEqual(configuration.default_records_returned, None)
             self.assertEqual(configuration.max_records_supported, None)
+            self.assertEqual(configuration.sru_version, "1.1")
 
             with open (TestFiles.loc_available_context_sets_and_indexes, "r") as f:
                 expected_indexes = json.loads(f.read())
 
-                self.assertEqual(configuration.available_context_sets_and_indexes, expected_indexes)
+                self.assertEqual(configuration.available_context_sets_and_indexes, expected_indexes)
+
+
```

### Comparing `sru_queryer-1.0.3/tests/test_sru_query.py` & `sru_queryer-2.0.0/tests/test_search_retrieve.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,186 +1,198 @@
 from unittest.mock import patch
 import unittest
 from requests import Request
 
-from src.sru_queryer import Query
-from src.sru_queryer.sru import SRUUtil
-from src.sru_queryer.cql import IndexQuery
-from src.sru_queryer.cql import AND, OR, LITERAL
+from src.sru_queryer._base._search_retrieve import SearchRetrieve
+from src.sru_queryer import SRUQueryer
+from src.sru_queryer.cql import SearchClause
+from src.sru_queryer.cql import AND, RawCQL
 from src.sru_queryer.sru import SortKey
 from tests.testData.test_data import TestFiles, get_alma_sru_configuration
-from src.sru_queryer.drivers import gapines_driver, alma_driver, loc_driver
 
 
-class TestSRUQuery(unittest.TestCase):
+class TestSearchRetrieve(unittest.TestCase):
 
     def test_construct_request(self):
         sru_configuration = get_alma_sru_configuration()
-        sru_configuration.search_retrieve_url = "https://example.com"
+        sru_configuration.server_url = "https://example.com"
         sru_configuration.sru_version = "1.2"
         sru_configuration.default_records_returned = None
 
-        constructed_search_retrieve_request = Query(sru_configuration, IndexQuery("alma", "bib_holding_count", "==", "10"), record_schema="marcxml").construct_request()
+        constructed_search_retrieve_request = SearchRetrieve(sru_configuration, SearchClause("alma", "bib_holding_count", "==", "10"), record_schema="marcxml").construct_request()
 
         expected_request = Request(
-            "GET", f'https://example.com?version=1.2&operation=searchRetrieve&recordSchema=marcxml&query=alma.bib_holding_count==%2210%22').prepare()
+            "GET", f'https://example.com?version=1.2&operation=searchRetrieve&recordSchema=marcxml&query=alma.bib_holding_count%20==%20"10"')
 
         self.assertEqual(
             constructed_search_retrieve_request.method, expected_request.method)
         self.assertEqual(
             constructed_search_retrieve_request.url, expected_request.url)
         self.assertEqual(
             constructed_search_retrieve_request.headers, expected_request.headers)
 
     def test_construct_request_complex(self):
         sru_configuration = get_alma_sru_configuration()
-        sru_configuration.search_retrieve_url = "https://example.com"
+        sru_configuration.server_url = "https://example.com"
         sru_configuration.sru_version = "1.2"
         sru_configuration.default_records_returned = None
         sru_configuration.default_record_schema = "marcxml"
 
-        constructed_search_retrieve_request = Query(sru_configuration, AND(
-            IndexQuery("alma", "bib_holding_count", ">", "15"),
-            IndexQuery("rec", "mms_id",  "==", "112233")
+        constructed_search_retrieve_request = SearchRetrieve(sru_configuration, AND(
+            SearchClause("alma", "bib_holding_count", ">", "15"),
+            SearchClause("rec", "mms_id",  "==", "112233")
         )).construct_request()
 
         expected_request = Request(
-            "GET", f'https://example.com/?version=1.2&operation=searchRetrieve&recordSchema=marcxml&query=alma.bib_holding_count%3E%2215%22%20and%20rec.mms_id==%22112233%22').prepare()
+            "GET", f'https://example.com?version=1.2&operation=searchRetrieve&recordSchema=marcxml&query=alma.bib_holding_count%20>%20"15"%20and%20rec.mms_id%20==%20"112233"')
 
         self.assertEqual(
             constructed_search_retrieve_request.method, expected_request.method)
         self.assertEqual(
             constructed_search_retrieve_request.url, expected_request.url)
         self.assertEqual(
             constructed_search_retrieve_request.headers, expected_request.headers)
 
     def test_construct_request_with_credentials(self):
         sru_configuration = get_alma_sru_configuration()
-        sru_configuration.search_retrieve_url = "https://example.com"
+        sru_configuration.server_url = "https://example.com"
         sru_configuration.sru_version = "1.2"
         sru_configuration.default_records_returned = None
         sru_configuration.username = "test_user"
         sru_configuration.password = "test_password"
 
-        constructed_search_retrieve_request = Query(sru_configuration, AND(
-            IndexQuery("alma", "bib_holding_count", ">", "15"),
-            IndexQuery("rec", "mms_id",  "==", "112233")
+        constructed_search_retrieve_request = SearchRetrieve(sru_configuration, AND(
+            SearchClause("alma", "bib_holding_count", ">", "15"),
+            SearchClause("rec", "mms_id",  "==", "112233")
         ), record_schema="marcxml").construct_request()
 
         credentials_encoded = "dGVzdF91c2VyOnRlc3RfcGFzc3dvcmQ="
         expected_request = Request(
-            "GET", f'https://example.com/?version=1.2&operation=searchRetrieve&recordSchema=marcxml&query=alma.bib_holding_count%3E%2215%22%20and%20rec.mms_id==%22112233%22', headers={
+            "GET", f'https://example.com?version=1.2&operation=searchRetrieve&recordSchema=marcxml&query=alma.bib_holding_count%20>%20"15"%20and%20rec.mms_id%20==%20"112233"', headers={
                 "Authorization": f'Basic {credentials_encoded}'
             })
 
         self.assertEqual(
             constructed_search_retrieve_request.method, expected_request.method)
         self.assertEqual(
             constructed_search_retrieve_request.url, expected_request.url)
         self.assertEqual(
             constructed_search_retrieve_request.headers, expected_request.headers)
 
     def test_construct_request_with_sort_by(self):
         sru_configuration = get_alma_sru_configuration()
-        sru_configuration.search_retrieve_url = "https://example.com"
+        sru_configuration.server_url = "https://example.com"
         sru_configuration.sru_version = "1.2"
         sru_configuration.default_records_returned = None
 
-        constructed_search_retrieve_request = Query(sru_configuration,
-                                                    IndexQuery("alma", "bib_holding_count", "==", '10'), record_schema="marcxml", sort_queries=[{"index_set": "alma", "index_name": "bib_holding_count", "sort_order": "ascending"}, {"index_set": "alma", "index_name": "title", "sort_order": "descending"}]).construct_request()
+        constructed_search_retrieve_request = SearchRetrieve(sru_configuration,
+                                                    SearchClause("alma", "bib_holding_count", "==", '10'), record_schema="marcxml", sort_queries=[{"index_set": "alma", "index_name": "bib_holding_count", "sort_order": "ascending"}, {"index_set": "alma", "index_name": "title", "sort_order": "descending"}]).construct_request()
 
         expected_request = Request(
-            "GET", f'https://example.com/?version=1.2&operation=searchRetrieve&recordSchema=marcxml&query=alma.bib_holding_count==%2210%22%20sortBy%20alma.bib_holding_count/sort.ascending%20alma.title/sort.descending')
+            "GET", f'https://example.com?version=1.2&operation=searchRetrieve&recordSchema=marcxml&query=alma.bib_holding_count%20==%20"10"%20sortBy%20alma.bib_holding_count/sort.ascending%20alma.title/sort.descending')
 
         self.assertEqual(
             constructed_search_retrieve_request.method, expected_request.method)
         self.assertEqual(
             constructed_search_retrieve_request.url, expected_request.url)
         self.assertEqual(
             constructed_search_retrieve_request.headers, expected_request.headers)
 
-    def test_validate_query_with_base_query_error(self):
+    def test_validate_query_with_bad_record_schema_raises_error(self):
         sru_configuration = get_alma_sru_configuration()
-        sru_configuration.search_retrieve_url = "https://example.com"
+        sru_configuration.server_url = "https://example.com"
         sru_configuration.sru_version = "1.2"
         sru_configuration.default_records_returned = None
 
         with self.assertRaises(ValueError) as ve:
-            Query(sru_configuration, IndexQuery("alma", "bib_holding_count", "==", "10"), record_schema='fakefake').validate()
+            SearchRetrieve(sru_configuration, SearchClause("alma", "action_note_note", "==", "10"), record_schema='fakefake').validate()
+
+        self.assertIn("'fakefake'", ve.exception.__str__())
+        self.assertIn("not available", ve.exception.__str__())
+
+    def test_validate_query_with_bad_default_record_schema_raises_error(self):
+        sru_configuration = get_alma_sru_configuration()
+        sru_configuration.server_url = "https://example.com"
+        sru_configuration.sru_version = "1.2"
+        sru_configuration.default_records_returned = None
+        sru_configuration.default_record_schema = "fakefake"
+
+        with self.assertRaises(ValueError) as ve:
+            SearchRetrieve(sru_configuration, SearchClause("alma", "action_note_note", "==", "10")).validate()
 
         self.assertIn("'fakefake'", ve.exception.__str__())
         self.assertIn("not available", ve.exception.__str__())
 
     def test_validate_query_with_index_error_raises_error_query(self):
         """Integration Test"""
         sru_configuration = get_alma_sru_configuration()
-        sru_configuration.search_retrieve_url = "https://example.com"
+        sru_configuration.server_url = "https://example.com"
         sru_configuration.sru_version = "1.2"
         sru_configuration.default_records_returned = None
 
         with self.assertRaises(ValueError) as ve:
-            Query(sru_configuration, IndexQuery(
+            SearchRetrieve(sru_configuration, SearchClause(
                 "alma", "fake_index", "==", "10"), record_schema="marcxml").validate()
 
         self.assertIn("'fake_index'", ve.exception.__str__())
                 
 class TestQueryWithXMLData(unittest.TestCase):
-    @patch("src.sru_queryer._base._sru_util.requests.get")
+    @patch("src.sru_queryer._base._sru_queryer.requests.get")
     def test_construct_request_gapines_data_default_schema_returned_by_explain(self, mock_get):
         """Integration"""
         with open(TestFiles.explain_response_gapines, "rb") as f:
             mock_get.return_value.content = f.read()
 
             # Initialize the gapines configuration
-            sru_configuration = SRUUtil.create_configuration_for_server("https://example.com", "https://example.com", sru_version="1.1", driver=gapines_driver)
+            sru_configuration = SRUQueryer("https://example.com").sru_configuration
 
-            constructed_search_retrieve_request = Query(sru_configuration, IndexQuery("alma", "bib_holding_count", "==", "10")).construct_request()
+            constructed_search_retrieve_request = SearchRetrieve(sru_configuration, SearchClause("alma", "bib_holding_count", "==", "10")).construct_request()
 
             expected_request = Request(
-                "GET", f'https://example.com?version=1.1&operation=searchRetrieve&recordSchema=marcxml&maximumRecords=10&query=alma.bib_holding_count==%2210%22').prepare()
+                "GET", f'https://example.com?version=1.1&operation=searchRetrieve&recordSchema=marcxml&maximumRecords=10&query=alma.bib_holding_count%20==%20"10"')
             
             self.assertEqual(
                 constructed_search_retrieve_request.url, expected_request.url)
             
-    @patch("src.sru_queryer._base._sru_util.requests.get")
+    @patch("src.sru_queryer._base._sru_queryer.requests.get")
     def test_initialize_1_2_query_with_invalid_sort_type_raises_error(self, mock_get):
-         with open(TestFiles.explain_response_gapines, "rb") as f:
+         with open(TestFiles.explain_response_alma, "rb") as f:
             mock_get.return_value.content = f.read()
 
             with self.assertRaises(ValueError) as ve:
-                sru_configuration = SRUUtil.create_configuration_for_server("https://example.com", "https://example.com", sru_version="1.2", driver=gapines_driver)
-                Query(sru_configuration, IndexQuery(value="dummyval"), record_schema="marcxml", sort_queries=[SortKey("example_xpath")])
+                sru_configuration = SRUQueryer("https://example.com").sru_configuration
+                SearchRetrieve(sru_configuration, SearchClause(search_term="dummyval"), record_schema="marcxml", sort_queries=[SortKey("example_xpath")])
 
             self.assertIn("SortKeys", ve.exception.__str__())
             self.assertIn("1.2", ve.exception.__str__())
 
-    @patch("src.sru_queryer._base._sru_util.requests.get")
+    @patch("src.sru_queryer._base._sru_queryer.requests.get")
     def test_initialize_1_1_query_with_invalid_sort_type_raises_error(self, mock_get):
         with open(TestFiles.explain_response_gapines, "rb") as f:
             mock_get.return_value.content = f.read()
 
             with self.assertRaises(ValueError) as ve:
-                sru_configuration = SRUUtil.create_configuration_for_server("https://example.com", "https://example.com", sru_version="1.1", driver=gapines_driver)
-                Query(sru_configuration, IndexQuery(value="dummyval"), sort_queries=[{"index_set": "alma", "index_name": "bib_holding_count", "sort_order": "ascending"}])
+                sru_configuration = SRUQueryer("https://example.com").sru_configuration
+                SearchRetrieve(sru_configuration, SearchClause(search_term="dummyval"), sort_queries=[{"index_set": "alma", "index_name": "bib_holding_count", "sort_order": "ascending"}])
             
             self.assertIn("SortKeys", ve.exception.__str__())
             self.assertIn("1.1", ve.exception.__str__())
 
-    @patch('src.sru_queryer._base._sru_util.requests.get')
+    @patch('src.sru_queryer._base._sru_queryer.requests.get')
     def test_initialize_and_format_base_query_no_schema_no_error(self, mock_get):
         """Integration"""
         with open(TestFiles.explain_response_loc, "rb") as f:
             mock_get.return_value.content = f.read()
 
-            sru_configuration = SRUUtil.create_configuration_for_server("https://example.com", "https://example2.com", sru_version="1.1", driver=loc_driver)
+            sru_configuration = SRUQueryer("https://example.com").sru_configuration
 
-            Query(sru_configuration, LITERAL("pass")).validate()
+            SearchRetrieve(sru_configuration, RawCQL("pass")).validate()
     
-    @patch('src.sru_queryer._base._sru_util.requests.get')
+    @patch('src.sru_queryer._base._sru_queryer.requests.get')
     def test_initialize_query_default_schema_raises_no_error(self, mock_get):
         """Integration"""
         with open(TestFiles.explain_response_gapines, "rb") as f:
             mock_get.return_value.content = f.read() 
 
-            sru_configuration = SRUUtil.create_configuration_for_server("https://example.com", "https://example2.com", sru_version="1.1", driver=gapines_driver)
+            sru_configuration = SRUQueryer("https://example.com").sru_configuration
 
-            Query(sru_configuration, LITERAL("pass"))
+            SearchRetrieve(sru_configuration, RawCQL("pass"))
```

### Comparing `sru_queryer-1.0.3/tests/test_sru_util.py` & `sru_queryer-2.0.0/tests/test_sru_queryer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,155 +1,186 @@
 import unittest
 from unittest.mock import patch
 
-from src.sru_queryer.sru import SRUUtil
-from tests.testData.test_data import get_alma_sru_configuration, get_gapines_sru_configuration, mock_searchable_indexes_and_descriptions
-
-@patch("src.sru_queryer.sru.SRUUtil._retrieve_explain_response_xml")
-@patch("src.sru_queryer.sru.SRUUtil._parse_explain_response_configuration")
-class TestSRUUtilCreateConfiguration(unittest.TestCase):
+from src.sru_queryer import SRUQueryer
+from src.sru_queryer._base._exceptions import ExplainResponseContentTypeException
+from src.sru_queryer.cql import SearchClause
+from tests.testData.test_data import get_alma_sru_configuration, get_gapines_sru_configuration, mock_searchable_indexes_and_descriptions, TestFiles
+
+@patch("src.sru_queryer.SRUQueryer._retrieve_explain_response_xml")
+@patch("src.sru_queryer.SRUQueryer._parse_explain_response_configuration")
+class TestSRUQueryerInitialization(unittest.TestCase):
 
     def test_merge_config_and_user_settings_urls_set_correctly(self, mock_parse_explain_response, *args):
         mock_parse_explain_response.return_value = get_alma_sru_configuration()
 
-        updated_config = SRUUtil.create_configuration_for_server("testurl2.com", "testurl.com")
+        updated_config = SRUQueryer("testurl2.com").sru_configuration
 
-        self.assertEqual(updated_config.explain_url, "testurl2.com")
-        self.assertEqual(updated_config.search_retrieve_url, "testurl.com")
+        self.assertEqual(updated_config.server_url, "testurl2.com")
 
-    def test_merge_config_and_user_settings_version_set_correctly(self, mock_parse_explain_response, *args):
+    def test_merge_config_and_user_settings_version_updates_based_on_explain(self, mock_parse_explain_response, *args):
         mock_parse_explain_response.return_value = get_alma_sru_configuration()
 
-        updated_config = SRUUtil.create_configuration_for_server("testurl2.com", "testurl.com", sru_version="1.1")
+        updated_config = SRUQueryer("testurl2.com", sru_version="1.1").sru_configuration
 
-        self.assertEqual(updated_config.sru_version, "1.1")
+        self.assertEqual(updated_config.sru_version, "1.2")
 
     def test_merge_config_and_user_settings_set_record_numbers_returned_correctly(self, mock_parse_explain_response, *args):
         mock_parse_explain_response.return_value = get_alma_sru_configuration()
 
-        updated_config = SRUUtil.create_configuration_for_server("testurl2.com", "testurl.com", default_records_returned=15, max_records_supported=40)
+        updated_config = SRUQueryer("testurl2.com", default_records_returned=15, max_records_supported=40).sru_configuration
 
         self.assertEqual(updated_config.default_records_returned, 15)
         self.assertEqual(updated_config.max_records_supported, 40)
 
     def test_merge_config_and_user_settings_set_username_password_returned_correctly(self, mock_parse_explain_response, *args):
         mock_parse_explain_response.return_value = get_alma_sru_configuration()
 
-        updated_config = SRUUtil.create_configuration_for_server("testurl2.com", "testurl.com", username="testusername", password="testpassword")
+        updated_config = SRUQueryer("testurl2.com", username="testusername", password="testpassword").sru_configuration
 
         self.assertEqual(updated_config.username, "testusername")
         self.assertEqual(updated_config.password, "testpassword")
 
     def test_merge_config_and_user_settings_set_cql_defaults_returned_correctly(self, mock_parse_explain_response, *args):
         mock_parse_explain_response.return_value = get_alma_sru_configuration()
 
-        updated_config = SRUUtil.create_configuration_for_server("testurl2.com", "testurl.com", default_cql_context_set="alma", default_cql_index="all_for_ui", default_cql_relation="all")
+        updated_config = SRUQueryer("testurl2.com", default_cql_context_set="alma", default_cql_index="all_for_ui", default_cql_relation="all").sru_configuration
 
         self.assertEqual(updated_config.default_context_set, "alma")
         self.assertEqual(updated_config.default_index, "all_for_ui")
         self.assertEqual(updated_config.default_relation, "all")
 
     def test_merge_config_and_user_settings_set_default_schemas_returned_correctly(self, mock_parse_explain_response, *args):
         mock_parse_explain_response.return_value = get_alma_sru_configuration()
 
-        updated_config = SRUUtil.create_configuration_for_server("testurl2.com", "testurl.com", default_record_schema="marcxml", default_sort_schema="marcxml")
+        updated_config = SRUQueryer("testurl2.com", default_record_schema="marcxml", default_sort_schema="marcxml").sru_configuration
 
         self.assertEqual(updated_config.default_record_schema, "marcxml")
         self.assertEqual(updated_config.default_sort_schema, "marcxml")
 
     def test_merge_config_and_user_settings_set_disable_validation_for_cql_defaults_returned_correctly(self, mock_parse_explain_response, *args):
         mock_parse_explain_response.return_value = get_alma_sru_configuration()
 
-        updated_config = SRUUtil.create_configuration_for_server("testurl2.com", "testurl.com", disable_validation_for_cql_defaults=True)
+        updated_config = SRUQueryer("testurl2.com", disable_validation_for_cql_defaults=True).sru_configuration
 
         self.assertEqual(updated_config.disable_validation_for_cql_defaults, True)
 
     def test_merge_config_and_user_settings_full_configuration_no_user_changes_stays_original(self, mock_parse_explain_response, *args):
         configuration_parsed_from_explain_response = get_gapines_sru_configuration()
         mock_parse_explain_response.return_value = configuration_parsed_from_explain_response
 
-        updated_config = SRUUtil.create_configuration_for_server("testurl2.com", "testurl.com")
+        updated_config = SRUQueryer("testurl2.com").sru_configuration
 
         self.assertEqual(updated_config.disable_validation_for_cql_defaults, False)
         self.assertEqual(updated_config.default_context_set, "eg")
         self.assertEqual(updated_config.default_index, "keyword")
         self.assertEqual(updated_config.default_relation, "all")
         self.assertEqual(updated_config.default_record_schema, "marcxml")
         self.assertEqual(updated_config.default_sort_schema, "marcxml")
         self.assertEqual(updated_config.default_records_returned, 10)
         self.assertEqual(updated_config.max_records_supported, 50)
+        self.assertEqual(updated_config.sru_version, "1.1")
 
     @staticmethod
-    def create_index_config(title, id, sort, supported_operations, empty_term_supported) -> dict:
+    def create_index_info(title, id, sort, supported_relations, empty_term_supported) -> dict:
         return {
                 "id": id,
                 "title": title,
                 "sort": sort,
-                "supported_operations": supported_operations,
+                "supported_relations": supported_relations,
                 "empty_term_supported": empty_term_supported
     }
 
     def verify_index_config_info(self, index, expected_index):
         self.assertEqual(index["title"], expected_index["title"], "Title Incorrect!")
         self.assertEqual(index["id"], expected_index["id"], "ID Incorrect! ")
         self.assertEqual(index["sort"], expected_index["sort"], "Sort Incorrect!")
-        self.assertListEqual(index["supported_operations"], expected_index["supported_operations"], "Supported Operations incorrect!")
+        self.assertListEqual(index["supported_relations"], expected_index["supported_relations"], "Supported Operations incorrect!")
         self.assertEqual(index["empty_term_supported"], expected_index["empty_term_supported"], "Empty Term Supported Incorrect!")
 
 
     def test_filter_available_context_sets_and_indexes_different_capitalization(self, *args):
-        filtered_dict = SRUUtil._filter_available_context_sets_and_indexes(
+        filtered_dict = SRUQueryer._filter_available_context_sets_and_indexes(
             mock_searchable_indexes_and_descriptions, title="library")
 
         self.assertDictEqual(filtered_dict, {
             "alma": {
                 "library": {
                     "id": None,
                     "title": "Library Code",
                     "sort": False,
-                    "supported_operations": ["==", "all"],
+                    "supported_relations": ["==", "all"],
                     "empty_term_supported": True
                 },
                 "library_status": {
                     "id": None,
                     "title": "Library Status",
                     "sort": False,
-                    "supported_operations": ["==", "all"],
+                    "supported_relations": ["==", "all"],
                     "empty_term_supported": True
                 },
             },
         })
 
     def test_filter_available_context_sets_and_indexes_different_set(self, *args):
-        filtered_dict = SRUUtil._filter_available_context_sets_and_indexes(
+        filtered_dict = SRUQueryer._filter_available_context_sets_and_indexes(
             mock_searchable_indexes_and_descriptions, title="mms")
         
-        expected_index = self.create_index_config("Bib MMS ID", None, False, ["==", "all"], True)
+        expected_index = self.create_index_info("Bib MMS ID", None, False, ["==", "all"], True)
 
         self.verify_index_config_info(filtered_dict["rec"]["mms_id"], expected_index)
 
 
     def test_filter_available_context_sets_and_indexes_two_sets(self, *args):
-        filtered_dict = SRUUtil._filter_available_context_sets_and_indexes(
+        filtered_dict = SRUQueryer._filter_available_context_sets_and_indexes(
             mock_searchable_indexes_and_descriptions, title="bib")
 
         self.assertDictEqual(filtered_dict, {
             "alma": {
                 "bib_holding_count": {
                     "id": None,
                     "title": "Bib Holding Count (Alma)",
                     "sort": True,
-                    "supported_operations": [">", ">=", "==", "<", "<="],
+                    "supported_relations": [">", ">=", "==", "<", "<="],
                     "empty_term_supported": True
                 },
             },
             "rec": {
                 "mms_id": {
                     "id": None,
                     "title": "Bib MMS ID",
                     "sort": False,
-                    "supported_operations": ["==", "all"],
+                    "supported_relations": ["==", "all"],
                     "empty_term_supported": True
                 },
             },
         })
 
+class TestSRUQUeryerExplainResponseXMLParse(unittest.TestCase):
+
+    @patch("src.sru_queryer.SRUQueryer._get_request_contents")
+    def test_parse_html_raises_parser_failure_exception(self, mock_request_contents):
+        with open(TestFiles.gapines_html_response, "rb") as f:
+            mock_request_contents.return_value = f.read()
+
+        with self.assertRaises(ExplainResponseContentTypeException) as pe:
+            SRUQueryer._retrieve_explain_response_xml("blahblah", None, None)
+        
+        print(pe.exception)
+
+class TestInitializeSRUQueryerIntegration(unittest.TestCase):
+    @patch("src.sru_queryer.SRUQueryer._get_request_contents")
+    def test_construct_search_retrieve_request_not_validated_no_error(self, mock_request_contents):
+        with open(TestFiles.explain_response_alma, "rb") as f:
+            mock_request_contents.return_value = f.read()
+
+        sc = SRUQueryer("https://server.com")
+        request = sc.construct_search_retrieve_request(SearchClause("fakecontextset", "bib", "=", "Radeon"), validate=False)
+
+    @patch("src.sru_queryer._base._sru_queryer.requests.Session.send")
+    @patch("src.sru_queryer.SRUQueryer._get_request_contents")
+    def test_search_retrieve_not_validated_no_error(self, mock_request_contents, *args):
+        with open(TestFiles.explain_response_alma, "rb") as f:
+            mock_request_contents.return_value = f.read()
+
+        sc = SRUQueryer("https://server.com")
+        content = sc.search_retrieve(SearchClause("fakecontextset", "bib", "=", "Radeon"), validate=False)
```

### Comparing `sru_queryer-1.0.3/tests/test_sru_validator.py` & `sru_queryer-2.0.0/tests/test_sru_validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 
 from src.sru_queryer._base._sru_validator import SRUValidator
-from tests.testData.test_data import get_gapines_sru_configuration, get_alma_sru_configuration, get_test_sru_configuration_no_sort_or_supported_operations_or_config, test_available_record_schemas_one_false
+from tests.testData.test_data import get_gapines_sru_configuration, get_alma_sru_configuration, get_test_sru_configuration_no_sort_or_supported_relations_or_config, test_available_record_schemas_one_false, test_available_record_schemas
 from src.sru_queryer.sru import SortKey
 
 class TestSRUValidator(unittest.TestCase):
 
     def test_validate_context_set_invalid_set_throws_error(self):
         sru_configuration = get_gapines_sru_configuration()
 
@@ -44,41 +44,53 @@
         sru_configuration = get_alma_sru_configuration()
 
         with self.assertRaises(ValueError) as ve:
             SRUValidator.validate_cql(sru_configuration, "alma", "all_for_ui", relation="***")
 
         self.assertIn("***", ve.exception.__str__())
 
-    def test_validate_index_invalid_value_raises_error(self):
+    def test_validate_index_invalid_search_term_raises_error(self):
         sru_configuration = get_alma_sru_configuration()
 
         with self.assertRaises(ValueError) as ve:
-            SRUValidator.validate_cql(sru_configuration, "alma", "alternate_complete_edition", "=", value="")
+            SRUValidator.validate_cql(sru_configuration, "alma", "alternate_complete_edition", "=", search_term="")
 
         self.assertIn("empty", ve.exception.__str__())
 
     def test_validate_index_can_sort_invalid_sort_raises_error(self):
         sru_configuration = get_alma_sru_configuration()
         sru_configuration.disable_validation_for_cql_defaults = True
 
         with self.assertRaises(ValueError) as ve:
             SRUValidator.validate_cql(sru_configuration, "alma", "alternate_complete_edition", "=", evaluate_can_sort=True)
 
         self.assertIn("sort", ve.exception.__str__())
 
-    def test_validate_index_no_value_sort_or_supported_operations_info(self):
-        sru_configuration = get_test_sru_configuration_no_sort_or_supported_operations_or_config()
+    def test_validate_index_no_search_term_sort_or_supported_relations_info(self):
+        sru_configuration = get_test_sru_configuration_no_sort_or_supported_relations_or_config()
 
         SRUValidator.validate_cql(sru_configuration, "dc", "title", "all", "", evaluate_can_sort=True)
 
     def test_validate_index_with_default_context_set(self):
         sru_configuration = get_gapines_sru_configuration()
 
         SRUValidator.validate_cql(sru_configuration, index_name="keyword")
 
+    def test_validate_defaults_context_set_only_no_error(self):
+        sru_configuration = get_alma_sru_configuration()
+        sru_configuration.default_context_set = "alma"
+
+        SRUValidator.validate_defaults(sru_configuration)
+
+    def test_validate_defaults_relation_only_no_error(self):
+        sru_configuration = get_alma_sru_configuration()
+        sru_configuration.default_relation = "="
+
+        SRUValidator.validate_defaults(sru_configuration)
+
     def test_validate_invalid_index_with_default_context_set_throws_error(self):
         sru_configuration = get_gapines_sru_configuration()
 
         with self.assertRaises(ValueError) as ve:
             SRUValidator.validate_cql(sru_configuration, index_name="invalid_index")
 
         self.assertIn("'eg'", ve.exception.__str__())
@@ -88,30 +100,30 @@
         sru_configuration = get_alma_sru_configuration()
 
         with self.assertRaises(ValueError) as ve:
             SRUValidator.validate_cql(sru_configuration, index_name="all_for_ui")
 
         self.assertIn("ensure", ve.exception.__str__())
 
-    def test_validate_value_with_all_defaults_set_no_error(self):
+    def test_validate_search_term_with_all_defaults_set_no_error(self):
         sru_configuration = get_alma_sru_configuration()
         sru_configuration.default_context_set = "alma"
         sru_configuration.default_index = "all_for_ui"
         sru_configuration.default_relation = "=="
 
-        SRUValidator.validate_cql(sru_configuration, value="hello")
+        SRUValidator.validate_cql(sru_configuration, search_term="hello")
 
-    def test_validate_invalid_value_with_all_defaults_set_throws_error(self):
+    def test_validate_invalid_search_term_with_all_defaults_set_throws_error(self):
         sru_configuration = get_alma_sru_configuration()
         sru_configuration.default_context_set = "alma"
         sru_configuration.default_index = "alternate_complete_edition"
         sru_configuration.default_relation = "=="
 
         with self.assertRaises(ValueError) as ve:
-            SRUValidator.validate_cql(sru_configuration, value="")
+            SRUValidator.validate_cql(sru_configuration, search_term="")
 
         self.assertIn("empty", ve.exception.__str__())
 
     def test_validate_all_defaults_set_no_error(self):
         sru_configuration = get_alma_sru_configuration()
         sru_configuration.default_context_set = "alma"
         sru_configuration.default_index = "alternate_complete_edition"
@@ -184,14 +196,20 @@
         sru_configuration.default_record_schema = "invalid_record_schema"
 
         with self.assertRaises(ValueError) as ve:
             SRUValidator.validate_defaults(sru_configuration)
 
         self.assertIn("invalid_record_schema", ve.exception.__str__())
 
+    def test_validate_record_schema_using_identifier_throws_error(self):
+        with self.assertRaises(ValueError) as ve:
+            SRUValidator._validate_record_schema(test_available_record_schemas, "http://www.loc.gov/standards/iso20775/")
+
+        self.assertIn("http://www.loc.gov/standards/iso20775/", ve.exception.__str__())
+
     def test_validate_configuration_defaults_throws_error_invalid_sort_schema(self):
         sru_configuration = get_alma_sru_configuration()
         sru_configuration.default_record_schema = "invalid_sort_schema"
 
         with self.assertRaises(ValueError) as ve:
             SRUValidator.validate_defaults(sru_configuration)
```


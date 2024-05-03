# Comparing `tmp/core-db-2.0.2.tar.gz` & `tmp/core_db-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core-db-2.0.2.tar", last modified: Fri Mar 29 01:24:57 2024, max compression
+gzip compressed data, was "core_db-2.0.3.tar", last modified: Fri May  3 02:26:20 2024, max compression
```

## Comparing `core-db-2.0.2.tar` & `core_db-2.0.3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 01:24:57.891749 core-db-2.0.2/
--rw-r--r--   0 root         (0) root         (0)     4406 2024-03-29 01:24:57.890749 core-db-2.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2675 2024-03-29 01:24:34.000000 core-db-2.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 01:24:57.883749 core-db-2.0.2/core_db/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 01:24:34.000000 core-db-2.0.2/core_db/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 01:24:57.887749 core-db-2.0.2/core_db/engines/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 01:24:34.000000 core-db-2.0.2/core_db/engines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10000 2024-03-29 01:24:34.000000 core-db-2.0.2/core_db/engines/mongo.py
--rw-rw-rw-   0 root         (0) root         (0)     1714 2024-03-29 01:24:34.000000 core-db-2.0.2/core_db/engines/mssql.py
--rw-rw-rw-   0 root         (0) root         (0)     2795 2024-03-29 01:24:34.000000 core-db-2.0.2/core_db/engines/mysql.py
--rw-rw-rw-   0 root         (0) root         (0)     1341 2024-03-29 01:24:34.000000 core-db-2.0.2/core_db/engines/oracle.py
--rw-rw-rw-   0 root         (0) root         (0)     1849 2024-03-29 01:24:34.000000 core-db-2.0.2/core_db/engines/postgre.py
--rw-rw-rw-   0 root         (0) root         (0)     4725 2024-03-29 01:24:34.000000 core-db-2.0.2/core_db/engines/snowflake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 01:24:57.887749 core-db-2.0.2/core_db/etls/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 01:24:34.000000 core-db-2.0.2/core_db/etls/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2477 2024-03-29 01:24:34.000000 core-db-2.0.2/core_db/etls/database_based.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 01:24:57.888749 core-db-2.0.2/core_db/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 01:24:34.000000 core-db-2.0.2/core_db/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1526 2024-03-29 01:24:34.000000 core-db-2.0.2/core_db/interfaces/base.py
--rw-rw-rw-   0 root         (0) root         (0)     6319 2024-03-29 01:24:34.000000 core-db-2.0.2/core_db/interfaces/sql_based.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 01:24:57.888749 core-db-2.0.2/core_db.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4406 2024-03-29 01:24:57.000000 core-db-2.0.2/core_db.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      538 2024-03-29 01:24:57.000000 core-db-2.0.2/core_db.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-29 01:24:57.000000 core-db-2.0.2/core_db.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      387 2024-03-29 01:24:57.000000 core-db-2.0.2/core_db.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-29 01:24:57.000000 core-db-2.0.2/core_db.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1830 2024-03-29 01:24:34.000000 core-db-2.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-29 01:24:57.891749 core-db-2.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       64 2024-03-29 01:24:34.000000 core-db-2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 02:26:20.060478 core_db-2.0.3/
+-rw-r--r--   0 root         (0) root         (0)     6122 2024-05-03 02:26:20.060478 core_db-2.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2024-05-03 02:26:02.000000 core_db-2.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 02:26:20.053478 core_db-2.0.3/core_db/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 02:26:02.000000 core_db-2.0.3/core_db/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 02:26:20.057478 core_db-2.0.3/core_db/engines/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 02:26:02.000000 core_db-2.0.3/core_db/engines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2393 2024-05-03 02:26:02.000000 core_db-2.0.3/core_db/engines/db2.py
+-rw-rw-rw-   0 root         (0) root         (0)    10000 2024-05-03 02:26:02.000000 core_db-2.0.3/core_db/engines/mongo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2024-05-03 02:26:02.000000 core_db-2.0.3/core_db/engines/mssql.py
+-rw-rw-rw-   0 root         (0) root         (0)     3043 2024-05-03 02:26:02.000000 core_db-2.0.3/core_db/engines/mysql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2024-05-03 02:26:02.000000 core_db-2.0.3/core_db/engines/oracle.py
+-rw-rw-rw-   0 root         (0) root         (0)     2097 2024-05-03 02:26:02.000000 core_db-2.0.3/core_db/engines/postgre.py
+-rw-rw-rw-   0 root         (0) root         (0)     4725 2024-05-03 02:26:02.000000 core_db-2.0.3/core_db/engines/snowflake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 02:26:20.057478 core_db-2.0.3/core_db/etls/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 02:26:02.000000 core_db-2.0.3/core_db/etls/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2024-05-03 02:26:02.000000 core_db-2.0.3/core_db/etls/database_based.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 02:26:20.058478 core_db-2.0.3/core_db/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 02:26:02.000000 core_db-2.0.3/core_db/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2024-05-03 02:26:02.000000 core_db-2.0.3/core_db/interfaces/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6319 2024-05-03 02:26:02.000000 core_db-2.0.3/core_db/interfaces/sql_based.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 02:26:20.058478 core_db-2.0.3/core_db.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6122 2024-05-03 02:26:20.000000 core_db-2.0.3/core_db.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      561 2024-05-03 02:26:20.000000 core_db-2.0.3/core_db.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 02:26:20.000000 core_db-2.0.3/core_db.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2024-05-03 02:26:20.000000 core_db-2.0.3/core_db.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-03 02:26:20.000000 core_db-2.0.3/core_db.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2024-05-03 02:26:02.000000 core_db-2.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 02:26:20.060478 core_db-2.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       64 2024-05-03 02:26:02.000000 core_db-2.0.3/setup.py
```

### Comparing `core-db-2.0.2/PKG-INFO` & `core_db-2.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-db
-Version: 2.0.2
+Version: 2.0.3
 Summary: This project/library contains common elements and clients related to database engines...
 Author-email: Alejandro Cora González <alek.cora.glez@gmail.com>
 Maintainer: Alejandro Cora González
 License: MIT
 Project-URL: Homepage, https://gitlab.com/bytecode-solutions/core/core-db
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -35,19 +35,22 @@
 Requires-Dist: oracledb==2.0.1; extra == "oracle"
 Provides-Extra: mssql
 Requires-Dist: pyodbc==5.1.0; extra == "mssql"
 Provides-Extra: mongo
 Requires-Dist: pymongo==4.6.0; extra == "mongo"
 Provides-Extra: snowflake
 Requires-Dist: snowflake-connector-python==3.7.1; extra == "snowflake"
+Provides-Extra: db2
+Requires-Dist: pyodbc==5.1.0; extra == "db2"
 
 # core-db
 _______________________________________________________________________________
 
-This project/library contains common elements related to database engines...
+This project/library contains common elements related to database engines and 
+provides clients to simplify the connections...
 
 ## Execution Environment
 
 ### Install libraries
 ```shell
 pip install --upgrade pip 
 pip install virtualenv
@@ -73,22 +76,80 @@
 pip install '.[all]'  # For all...
 pip install '.[mysql]'
 pip install '.[postgre]'
 pip install '.[oracle]'
 pip install '.[mongo]'
 pip install '.[mssql]'
 pip install '.[snowflake]'
+pip install '.[db2]'
 ```
 
 ### Check tests and coverage...
 ```shell
 python manager.py run-tests
 python manager.py run-coverage
 ```
 
+## Clients
+
+### Postgre
+```python
+from core_db.engines.postgre import PostgreClient
+
+with PostgreClient(conninfo=f"postgresql://postgres:postgres@localhost:5432/test") as client:
+    client.execute("SELECT version() AS version;")
+    print(client.fetch_one()[0])
+```
+
+### Mongo
+```python
+from core_db.engines.mongo import MongoClient
+
+client = MongoClient(**{"host": "host", "database": "db"})
+client.connect()
+print(client.test_connection())
+```
+
+### MsSql
+```python
+from core_db.engines.mssql import MsSqlClient
+
+with MsSqlClient(
+        dsn="DRIVER={ODBC Driver 18 for SQL Server};SERVER=localhost;DATABASE=master;UID=SA;PWD=sOm3str0ngP@33w0rd;Encrypt=no",
+        autocommit=True, timeout=5) as client:
+    
+    client.execute("SELECT @@VERSION AS 'version';")
+    print(list(client.fetch_records()))
+```
+
+### Oracle
+```python
+from core_db.engines.oracle import OracleClient
+
+with OracleClient(user="...", password="...", dsn=f"{host}:{port}/{service_name}") as client:
+    res = client.execute("SELECT * FROM ...")
+    for x in client.fetch_all():
+        print(x)
+```
+
+### MySQL
+```python
+from core_db.engines.mysql import MySQLClient
+
+with MySQLClient(host="localhost", user="root", password="SomePassword") as client:
+    client.execute("SELECT * FROM ...;")
+    for x in client.fetch_all():
+        print(x)
+```
+
+### Snowflake
+```python
+...
+```
+
 ### Testing clients...
 We can test the clients by executing the below command. It will perform a series of
 query execution in the database engine to ensure it's working as expected. We
 must have the database engine up and running...
 
 Example PostgreSQL:
 ```commandline
@@ -123,7 +184,14 @@
   mcr.microsoft.com/mssql/server:2022-latest
 
 docker start MsSQL
 
 sudo /bin/bash ./scripts/install_mssql_driver.sh
 python manager.py run-database-test -db MsSqlClient -params '{"dsn": "DRIVER={ODBC Driver 18 for SQL Server};SERVER=localhost;DATABASE=master;UID=SA;PWD=sOm3str0ngP@33w0rd;Encrypt=no"}'
 ```
+
+Example DB2:
+```shell
+curl https://public.dhe.ibm.com/software/ibmi/products/odbc/debs/dists/1.1.0/ibmi-acs-1.1.0.list | sudo tee /etc/apt/sources.list.d/ibmi-acs-1.1.0.list
+sudo apt update
+sudo apt install ibm-iaccess
+```
```

### Comparing `core-db-2.0.2/core_db/engines/mongo.py` & `core_db-2.0.3/core_db/engines/mongo.py`

 * *Files identical despite different names*

### Comparing `core-db-2.0.2/core_db/engines/mssql.py` & `core_db-2.0.3/core_db/engines/mssql.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,21 @@
 from core_db.interfaces.sql_based import SqlDatabaseClient
 
 
 class MsSqlClient(SqlDatabaseClient):
     """
     Client for Microsoft MsSQL connection...
 
-    Example WITH context manager:
+    ===================================================
+    How to use
+    ===================================================
+
+    WITH Context Manager
+    ---------------------------------------------------
+
         with MsSqlClient(
             dsn="DRIVER={ODBC Driver 18 for SQL Server};SERVER=localhost;DATABASE=master;UID=SA;PWD=sOm3str0ngP@33w0rd;Encrypt=no",
             autocommit=True,
             timeout=5
         ) as client:
             client.execute("SELECT @@VERSION AS 'version';")
             print(list(client.fetch_records()))
```

### Comparing `core-db-2.0.2/core_db/engines/mysql.py` & `core_db-2.0.3/core_db/engines/mysql.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,21 +10,29 @@
 from core_db.interfaces.sql_based import SqlDatabaseClient
 
 
 class MySQLClient(SqlDatabaseClient):
     """
     Client for MySQL connection...
 
-    Example WITH context manager:
+    ===================================================
+    How to use
+    ===================================================
+
+    WITH Context Manager
+    ---------------------------------------------------
+
         with MySQLClient(host="localhost", user="root", password="SomePassword") as client:
             client.execute("SELECT * FROM ...;")
             for x in client.fetch_all():
                 print(x)
 
-    Example:
+    WITHOUT Context Manager
+    ---------------------------------------------------
+
         client = MySQLClient(host="localhost", user="root", password="SomePassword")
         client.connect()
 
         res = client.execute("SELECT * FROM ...;")
         for x in client.fetch_all():
             print(x)
         client.close()
```

### Comparing `core-db-2.0.2/core_db/engines/oracle.py` & `core_db-2.0.3/core_db/engines/oracle.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,25 +5,33 @@
 from core_db.interfaces.sql_based import SqlDatabaseClient
 
 
 class OracleClient(SqlDatabaseClient):
     """
     Client for Oracle connection...
 
-    Example:
+    ===================================================
+    How to use
+    ===================================================
+
+    WITHOUT Context Manager
+    ---------------------------------------------------
+
         client = OracleClient(user="...", password="...", dsn=f"{host}:{port}/{service_name}")
         client.connect()
 
         res = client.execute("SELECT * FROM ...")
         for x in client.fetch_all():
             print(x)
         client.close()
 
 
-    Example WITH context manager:
+    WITH Context Manager
+    ---------------------------------------------------
+
         with OracleClient(user="...", password="...", dsn=f"{host}:{port}/{service_name}") as client:
             res = client.execute("SELECT * FROM ...")
             for x in client.fetch_all():
                 print(x)
     """
 
     def __init__(self, **kwargs):
```

### Comparing `core-db-2.0.2/core_db/engines/postgre.py` & `core_db-2.0.3/core_db/engines/postgre.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,22 +8,31 @@
 from core_db.interfaces.sql_based import SqlDatabaseClient
 
 
 class PostgreClient(SqlDatabaseClient):
     """
     Client for PostgreSQL connection...
 
-    Example WITH context manager:
-        with PostgreLClient(conninfo=f"postgresql://postgres:postgres@localhost:5432/test") as client:
+    ===================================================
+    How to use
+    ===================================================
+
+    WITH Context Manager
+    ---------------------------------------------------
+
+        with PostgreClient(conninfo=f"postgresql://postgres:postgres@localhost:5432/test") as client:
             client.execute("SELECT version() AS version;")
             print(client.fetch_one()[0])
 
-    Example:
+    WITHOUT Context Manager
+    ---------------------------------------------------
+
         client = PostgreClient(conninfo=f"postgresql://postgres:postgres@localhost:5432/test")
         client.connect()
+
         client.execute("SELECT version();")
         print(list(client.fetch_records()))
         client.close()
     """
 
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
```

### Comparing `core-db-2.0.2/core_db/engines/snowflake.py` & `core_db-2.0.3/core_db/engines/snowflake.py`

 * *Files identical despite different names*

### Comparing `core-db-2.0.2/core_db/etls/database_based.py` & `core_db-2.0.3/core_db/etls/database_based.py`

 * *Files identical despite different names*

### Comparing `core-db-2.0.2/core_db/interfaces/base.py` & `core_db-2.0.3/core_db/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `core-db-2.0.2/core_db/interfaces/sql_based.py` & `core_db-2.0.3/core_db/interfaces/sql_based.py`

 * *Files identical despite different names*

### Comparing `core-db-2.0.2/core_db.egg-info/PKG-INFO` & `core_db-2.0.3/core_db.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-db
-Version: 2.0.2
+Version: 2.0.3
 Summary: This project/library contains common elements and clients related to database engines...
 Author-email: Alejandro Cora González <alek.cora.glez@gmail.com>
 Maintainer: Alejandro Cora González
 License: MIT
 Project-URL: Homepage, https://gitlab.com/bytecode-solutions/core/core-db
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -35,19 +35,22 @@
 Requires-Dist: oracledb==2.0.1; extra == "oracle"
 Provides-Extra: mssql
 Requires-Dist: pyodbc==5.1.0; extra == "mssql"
 Provides-Extra: mongo
 Requires-Dist: pymongo==4.6.0; extra == "mongo"
 Provides-Extra: snowflake
 Requires-Dist: snowflake-connector-python==3.7.1; extra == "snowflake"
+Provides-Extra: db2
+Requires-Dist: pyodbc==5.1.0; extra == "db2"
 
 # core-db
 _______________________________________________________________________________
 
-This project/library contains common elements related to database engines...
+This project/library contains common elements related to database engines and 
+provides clients to simplify the connections...
 
 ## Execution Environment
 
 ### Install libraries
 ```shell
 pip install --upgrade pip 
 pip install virtualenv
@@ -73,22 +76,80 @@
 pip install '.[all]'  # For all...
 pip install '.[mysql]'
 pip install '.[postgre]'
 pip install '.[oracle]'
 pip install '.[mongo]'
 pip install '.[mssql]'
 pip install '.[snowflake]'
+pip install '.[db2]'
 ```
 
 ### Check tests and coverage...
 ```shell
 python manager.py run-tests
 python manager.py run-coverage
 ```
 
+## Clients
+
+### Postgre
+```python
+from core_db.engines.postgre import PostgreClient
+
+with PostgreClient(conninfo=f"postgresql://postgres:postgres@localhost:5432/test") as client:
+    client.execute("SELECT version() AS version;")
+    print(client.fetch_one()[0])
+```
+
+### Mongo
+```python
+from core_db.engines.mongo import MongoClient
+
+client = MongoClient(**{"host": "host", "database": "db"})
+client.connect()
+print(client.test_connection())
+```
+
+### MsSql
+```python
+from core_db.engines.mssql import MsSqlClient
+
+with MsSqlClient(
+        dsn="DRIVER={ODBC Driver 18 for SQL Server};SERVER=localhost;DATABASE=master;UID=SA;PWD=sOm3str0ngP@33w0rd;Encrypt=no",
+        autocommit=True, timeout=5) as client:
+    
+    client.execute("SELECT @@VERSION AS 'version';")
+    print(list(client.fetch_records()))
+```
+
+### Oracle
+```python
+from core_db.engines.oracle import OracleClient
+
+with OracleClient(user="...", password="...", dsn=f"{host}:{port}/{service_name}") as client:
+    res = client.execute("SELECT * FROM ...")
+    for x in client.fetch_all():
+        print(x)
+```
+
+### MySQL
+```python
+from core_db.engines.mysql import MySQLClient
+
+with MySQLClient(host="localhost", user="root", password="SomePassword") as client:
+    client.execute("SELECT * FROM ...;")
+    for x in client.fetch_all():
+        print(x)
+```
+
+### Snowflake
+```python
+...
+```
+
 ### Testing clients...
 We can test the clients by executing the below command. It will perform a series of
 query execution in the database engine to ensure it's working as expected. We
 must have the database engine up and running...
 
 Example PostgreSQL:
 ```commandline
@@ -123,7 +184,14 @@
   mcr.microsoft.com/mssql/server:2022-latest
 
 docker start MsSQL
 
 sudo /bin/bash ./scripts/install_mssql_driver.sh
 python manager.py run-database-test -db MsSqlClient -params '{"dsn": "DRIVER={ODBC Driver 18 for SQL Server};SERVER=localhost;DATABASE=master;UID=SA;PWD=sOm3str0ngP@33w0rd;Encrypt=no"}'
 ```
+
+Example DB2:
+```shell
+curl https://public.dhe.ibm.com/software/ibmi/products/odbc/debs/dists/1.1.0/ibmi-acs-1.1.0.list | sudo tee /etc/apt/sources.list.d/ibmi-acs-1.1.0.list
+sudo apt update
+sudo apt install ibm-iaccess
+```
```

### Comparing `core-db-2.0.2/core_db.egg-info/SOURCES.txt` & `core_db-2.0.3/core_db.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 core_db/__init__.py
 core_db.egg-info/PKG-INFO
 core_db.egg-info/SOURCES.txt
 core_db.egg-info/dependency_links.txt
 core_db.egg-info/requires.txt
 core_db.egg-info/top_level.txt
 core_db/engines/__init__.py
+core_db/engines/db2.py
 core_db/engines/mongo.py
 core_db/engines/mssql.py
 core_db/engines/mysql.py
 core_db/engines/oracle.py
 core_db/engines/postgre.py
 core_db/engines/snowflake.py
 core_db/etls/__init__.py
```

### Comparing `core-db-2.0.2/pyproject.toml` & `core_db-2.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "core-db"
 description = "This project/library contains common elements and clients related to database engines..."
-version = "2.0.2"
+version = "2.0.3"
 
 authors = [
     {name = "Alejandro Cora González", email = "alek.cora.glez@gmail.com"}
 ]
 
 maintainers = [
     {name = "Alejandro Cora González"}
@@ -82,7 +82,11 @@
 mongo = [
     "pymongo==4.6.0"
 ]
 
 snowflake = [
     "snowflake-connector-python==3.7.1"
 ]
+
+db2 = [
+    "pyodbc==5.1.0"
+]
```


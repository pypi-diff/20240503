# Comparing `tmp/database-factory-1.0.6.tar.gz` & `tmp/database-factory-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/database-factory-1.0.6.tar", last modified: Mon May 15 05:12:40 2023, max compression
+gzip compressed data, was "database-factory-1.1.0.tar", last modified: Fri May  3 13:04:36 2024, max compression
```

## Comparing `database-factory-1.0.6.tar` & `database-factory-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-05-15 05:12:40.126346 database-factory-1.0.6/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     1117 2021-03-16 10:53:13.000000 database-factory-1.0.6/LICENSE
--rw-rw-r--   0 ankit     (1001) ankit     (1001)      233 2021-03-16 12:44:42.000000 database-factory-1.0.6/MANIFEST.in
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     8061 2023-05-15 05:12:40.126346 database-factory-1.0.6/PKG-INFO
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     5355 2023-05-15 05:12:34.000000 database-factory-1.0.6/README.md
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-05-15 05:12:40.122346 database-factory-1.0.6/database_factory/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)       45 2023-05-15 05:12:39.000000 database-factory-1.0.6/database_factory/.version
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/__init__.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-05-15 05:12:40.126346 database-factory-1.0.6/database_factory/cloud/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/cloud/__init__.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-05-15 05:12:40.126346 database-factory-1.0.6/database_factory/cloud/aws/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/cloud/aws/__init__.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     3204 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/cloud/aws/auth.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     3888 2021-08-10 05:53:56.000000 database-factory-1.0.6/database_factory/cloud/aws/secrete_manager.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-05-15 05:12:40.126346 database-factory-1.0.6/database_factory/cloud/gcp/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/cloud/gcp/__init__.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     5800 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/cloud/gcp/auth.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     5435 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/cloud/gcp/resource_manager.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     3876 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/cloud/gcp/secrete_manager.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-05-15 05:12:40.126346 database-factory-1.0.6/database_factory/common/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/common/__init__.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     4217 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/common/common.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)    17304 2023-04-14 13:57:53.000000 database-factory-1.0.6/database_factory/manager.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     5435 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/operations.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-05-15 05:12:40.126346 database-factory-1.0.6/database_factory.egg-info/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     8061 2023-05-15 05:12:40.000000 database-factory-1.0.6/database_factory.egg-info/PKG-INFO
--rw-rw-r--   0 ankit     (1001) ankit     (1001)      753 2023-05-15 05:12:40.000000 database-factory-1.0.6/database_factory.egg-info/SOURCES.txt
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        1 2023-05-15 05:12:40.000000 database-factory-1.0.6/database_factory.egg-info/dependency_links.txt
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     1139 2023-05-15 05:12:40.000000 database-factory-1.0.6/database_factory.egg-info/requires.txt
--rw-rw-r--   0 ankit     (1001) ankit     (1001)       17 2023-05-15 05:12:40.000000 database-factory-1.0.6/database_factory.egg-info/top_level.txt
--rw-rw-r--   0 ankit     (1001) ankit     (1001)       67 2023-05-15 05:12:40.126346 database-factory-1.0.6/setup.cfg
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     7026 2023-05-15 05:12:34.000000 database-factory-1.0.6/setup.py
+drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-03 13:04:36.101024 database-factory-1.1.0/
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     1117 2024-05-02 14:18:14.000000 database-factory-1.1.0/LICENSE
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)      233 2024-05-02 14:18:14.000000 database-factory-1.1.0/MANIFEST.in
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     7190 2024-05-03 13:04:36.101024 database-factory-1.1.0/PKG-INFO
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     5940 2024-05-03 06:37:08.000000 database-factory-1.1.0/README.md
+drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-03 13:04:36.101024 database-factory-1.1.0/database_factory/
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)       45 2024-05-03 13:04:35.000000 database-factory-1.1.0/database_factory/.version
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)        0 2024-05-02 14:18:14.000000 database-factory-1.1.0/database_factory/__init__.py
+drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-03 13:04:36.101024 database-factory-1.1.0/database_factory/cloud/
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)        0 2024-05-02 14:18:14.000000 database-factory-1.1.0/database_factory/cloud/__init__.py
+drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-03 13:04:36.101024 database-factory-1.1.0/database_factory/cloud/aws/
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)        0 2024-05-02 14:18:14.000000 database-factory-1.1.0/database_factory/cloud/aws/__init__.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     3204 2024-05-02 14:18:14.000000 database-factory-1.1.0/database_factory/cloud/aws/auth.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     3888 2024-05-02 14:18:14.000000 database-factory-1.1.0/database_factory/cloud/aws/secrete_manager.py
+drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-03 13:04:36.101024 database-factory-1.1.0/database_factory/cloud/gcp/
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)        0 2024-05-02 14:18:14.000000 database-factory-1.1.0/database_factory/cloud/gcp/__init__.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     5800 2024-05-02 14:18:14.000000 database-factory-1.1.0/database_factory/cloud/gcp/auth.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     5435 2024-05-02 14:18:14.000000 database-factory-1.1.0/database_factory/cloud/gcp/resource_manager.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     3876 2024-05-02 14:18:14.000000 database-factory-1.1.0/database_factory/cloud/gcp/secrete_manager.py
+drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-03 13:04:36.101024 database-factory-1.1.0/database_factory/common/
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)        0 2024-05-02 14:18:14.000000 database-factory-1.1.0/database_factory/common/__init__.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     4217 2024-05-02 14:18:14.000000 database-factory-1.1.0/database_factory/common/common.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)    17304 2024-05-02 14:18:14.000000 database-factory-1.1.0/database_factory/manager.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     5435 2024-05-02 14:18:14.000000 database-factory-1.1.0/database_factory/operations.py
+drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-03 13:04:36.101024 database-factory-1.1.0/database_factory.egg-info/
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     7190 2024-05-03 13:04:36.000000 database-factory-1.1.0/database_factory.egg-info/PKG-INFO
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)      753 2024-05-03 13:04:36.000000 database-factory-1.1.0/database_factory.egg-info/SOURCES.txt
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)        1 2024-05-03 13:04:36.000000 database-factory-1.1.0/database_factory.egg-info/dependency_links.txt
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     2489 2024-05-03 13:04:36.000000 database-factory-1.1.0/database_factory.egg-info/requires.txt
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)       17 2024-05-03 13:04:36.000000 database-factory-1.1.0/database_factory.egg-info/top_level.txt
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)       67 2024-05-03 13:04:36.101024 database-factory-1.1.0/setup.cfg
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     8009 2024-05-03 06:37:08.000000 database-factory-1.1.0/setup.py
```

### Comparing `database-factory-1.0.6/LICENSE` & `database-factory-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.6/PKG-INFO` & `database-factory-1.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,220 +1,249 @@
 Metadata-Version: 2.1
 Name: database-factory
-Version: 1.0.6
+Version: 1.1.0
 Summary: Database Factory;
 Home-page: https://github.com/shrivastava-v-ankit/database-factory
 Author: Ankit Shrivastava
 License: MIT
 Project-URL: Source, https://github.com/shrivastava-v-ankit/database-factory/
 Project-URL: Tracker, https://github.com/shrivastava-v-ankit/database-factory/issues
-Description: # database-factory
-        
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-        [![PyPI](https://img.shields.io/pypi/v/database-factory.svg)](https://pypi.org/project/database-factory)
-        [![CircleCI](https://circleci.com/gh/shrivastava-v-ankit/database-factory.svg?style=svg)](https://circleci.com/gh/shrivastava-v-ankit/database-factory)
-        
-        
-        
-        Database factory is used to manage/create database connection with execute queries using the connection.
-        The concept of having single source to connect various databases and perform database operations.
-        
-        User need not to worry on the crafting the connection string and to identify the methods for the database operations.
-        Database factory supports DML / DDL executions and have support of Pandas DataFrame to create or replace existing tables.
-        
-        Database factory is wrapper on sqlalchemy for crafting the connection and supports below databases:
-        
-        ```bash
-        * Sqlite3
-        * PostgreSQl
-        * BigQuery
-        * Snowflake
-        * MariaDB
-        * MySQL
-        ```
-        Database factory can be enhanced for all the sqlalchemy supported database.
-        
-        ## Getting Started
-        
-        ```bash
-        pip install database-factory
-        ```
-        
-        ### Using database-factory
-        -----
-        ```python
-        from database_factory.manager import DatabaseManager
-        import tempfile
-        temp_dir = tempfile.gettempdir()
-        db = DatabaseManager(engine_type="sqlite", database="test_db", sqlite_db_path=temp_dir)
-        db.create_session()
-        
-        db.execute_sql(sql="create table test (id int PRIMARY KEY)")
-        db.execute_sql(sql="insert into test values (1)")
-        db.execute_sql(sql="insert into test values (2)")
-        
-        rows = db.execute_sql(sql="select * from test")
-        if rows:
-          print(rows)
-        
-        
-        df = db.get_df(sql="select * from test")
-        print(df)
-        
-        db.execute_df(panda_df=df, table_name=copy_test, exist_action="replace")
-        # db.execute_df(panda_df=df, table_name=copy_test, exist_action="replace", chunk_size=100)
-        db.execute_sql(sql="insert into copy_test values (3)")
-        rows_copy = db.execute_sql(sql="select * from copy_test")
-        if rows_copy:
-          print(rows_copy)
-        ```
-        
-        ## Appendix
-        ### Supported database type:
-        ----
-        ```
-        *   sqlite `default`
-        *   postgres
-        *   mysql
-        *   mariadb
-        *   snowflake
-        ```
-        
-        ### Connection parameters for sqlite:
-        -----
-        ```python
-        * engine_type: sqlite
-        * database: <name of database>
-        * sqlite_db_path: <path where database will be created>
-        ```
-        
-        ### Connection parameters for postgres:
-        -----
-        ```python
-        * engine_type: postgres
-        * database: <name of database>
-        * username: <postgres user>
-        * password: <user password>
-        * host: <host of postgres service>
-        * port: <port of postgres service>
-        ```
-        
-        ### Connection parameters for mysql:
-        -----
-        ```python
-        * engine_type: mysql
-        * database: <name of database>
-        * username: <mysql user>
-        * password: <user password>
-        * host: <host of mysql service>
-        * port: <port of mysql servic\>
-        ```
-        
-        ### Connection parameters for mariadb:
-        -----
-        ```python
-        * engine_type: mariadb
-        * database: <name of database>
-        * username: <mariadb user>
-        * password: <user password>
-        * host: <host of mariadb service>
-        * port: <port of mariadb service>
-        ```
-        
-        ### Connection parameters for snowflake:
-        -----
-        ```python
-        * engine_type: snowflake
-        * database: <name of database>
-        * username: <snowflake user>
-        * password: <user password>
-        * schema: <schema name>
-        * snowflake_role: <snowflake role>
-        * snowflake_warehouse: <snowflake warehouse>
-        * snowflake_account: <snowflake account>
-        ```
-        
-        ### Connection parameters for bigquery:
-        -----
-        ```python
-        * engine_type: bigquery
-        * database: <name of database>
-        ```
-        
-        ### Getting connection properties from AWS / GCP Secret Manager Service:
-        -----
-        Note:
-        * GCP: 
-           * On Cloud Server:
-               * Set server to execute the all cloud api services
-               * Attach following permissions
-                  * Project Viewer
-                  * Secret Manager Secret Accessor
-           * On Premises:
-               * Attach following permissions to user service account and download service account file for authentication:
-                  * Project Viewer
-                  * Secret Manager Secret Accessor
-               * Set environment variable "GOOGLE_APPLICATION_CREDENTIALS" pointing to service account file.
-        * AWS:
-           * On Cloud Server:
-              * Set execution profile with "secretsmanager:GetSecretValue" policy
-           * On Premises:
-              * AWS should be configured
-              * User should have permissions of "secretsmanager:GetSecretValue" policy.
-        
-        ```python
-        * engine_type: bigquery
-        * database: <name of database>
-        * secret_id: <Secret name of AWS / GCP Secret Manager Service>
-        * secrete_manager_cloud: <aws or gcp as per cloud>
-        * aws_region: <aws region: default=> us-east-1>
-        ```
-        
-        
-        ### Development Setup
-        
-        #### Using virtualenv
-        
-        ```bash
-        python3 -m venv venv
-        source env/bin/activate
-        pip install .
-        ```
-        
-        ### Contributing
-        
-        1. Fork repo- https://github.com/shrivastava-v-ankit/database-factory.git
-        2. Create your feature branch - `git checkout -b feature/name`
-        3. Install Python packages
-           * sqlalchemy==1.4.47
-           * pandas==1.5.3
-           * GitPython
-           * coverage==7.2.3
-           * exceptiongroup==1.1.1
-           * iniconfig==2.0.0
-           * pluggy==1.0.0
-           * pytest==7.3.0
-           * pytest-cov==4.0.0
-           * tomli==2.0.1
-        4. Run Python test (pytest)
-           * pytest -v --cov --cov-report html --cov-report xml --junitxml=test-results/database_factory_test/results.xml
-        5. Add Python test (pytest) and covrage report for new/changed feature.
-        4. Commit your changes - `git commit -am "Added name"`
-        5. Push to the branch - `git push origin feature/name`
-        6. Create a new pull request
-        
-        
 Keywords: python,os independent,database,sqlalchemy,sqlite3,sqlite,postgres,mysql,maridb,snowflake,bigquery,secret manager
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Version Control :: Git
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.8, >=3.9, <3.10
 Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: aws
+Provides-Extra: gcp
+Provides-Extra: snowflake
+Provides-Extra: postgres
+Provides-Extra: mysql
+License-File: LICENSE
+
+# database-factory
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI](https://img.shields.io/pypi/v/database-factory.svg)](https://pypi.org/project/database-factory)
+[![CircleCI](https://circleci.com/gh/shrivastava-v-ankit/database-factory.svg?style=svg)](https://circleci.com/gh/shrivastava-v-ankit/database-factory)
+
+
+
+Database factory is used to manage/create database connection with execute queries using the connection.
+The concept of having single source to connect various databases and perform database operations.
+
+User need not to worry on the crafting the connection string and to identify the methods for the database operations.
+Database factory supports DML / DDL executions and have support of Pandas DataFrame to create or replace existing tables.
+
+Database factory is wrapper on sqlalchemy for crafting the connection and supports below databases:
+
+```bash
+* Sqlite3
+* PostgreSQl
+* BigQuery
+* Snowflake
+* MariaDB
+* MySQL
+```
+Database factory can be enhanced for all the sqlalchemy supported database.
+
+## Getting Started
+
+```bash
+pip install database-factory
+```
+Note: Default installation for database factory is to support Sqlite3. For other database/cloud support it can be installed with compinations of extra libraries
+
+### Sqite3 with AWS cloud support
+```bash
+pip install database-factory["aws"]
+```
+
+### Snowflake with AWS cloud support
+```bash
+pip install database-factory["snowflake,aws"]
+```
+
+### Following options are supported
+   * Secret manager cloud support
+      * aws
+      * gcp
+   * Databases
+      * snowflake
+      * postgres
+      * mysql
+   * all: Will install with libraries of all supported cloud and supported databases.
+
+### Using database-factory
+-----
+```python
+from database_factory.manager import DatabaseManager
+import tempfile
+temp_dir = tempfile.gettempdir()
+db = DatabaseManager(engine_type="sqlite", database="test_db", sqlite_db_path=temp_dir)
+db.create_session()
+
+db.execute_sql(sql="create table test (id int PRIMARY KEY)")
+db.execute_sql(sql="insert into test values (1)")
+db.execute_sql(sql="insert into test values (2)")
+
+rows = db.execute_sql(sql="select * from test")
+if rows:
+  print(rows)
+
+
+df = db.get_df(sql="select * from test")
+print(df)
+
+db.execute_df(panda_df=df, table_name=copy_test, exist_action="replace")
+# db.execute_df(panda_df=df, table_name=copy_test, exist_action="replace", chunk_size=100)
+db.execute_sql(sql="insert into copy_test values (3)")
+rows_copy = db.execute_sql(sql="select * from copy_test")
+if rows_copy:
+  print(rows_copy)
+```
+
+## Appendix
+### Supported database type:
+----
+```
+*   sqlite `default`
+*   postgres
+*   mysql
+*   mariadb
+*   snowflake
+```
+
+### Connection parameters for sqlite:
+-----
+```python
+* engine_type: sqlite
+* database: <name of database>
+* sqlite_db_path: <path where database will be created>
+```
+
+### Connection parameters for postgres:
+-----
+```python
+* engine_type: postgres
+* database: <name of database>
+* username: <postgres user>
+* password: <user password>
+* host: <host of postgres service>
+* port: <port of postgres service>
+```
+
+### Connection parameters for mysql:
+-----
+```python
+* engine_type: mysql
+* database: <name of database>
+* username: <mysql user>
+* password: <user password>
+* host: <host of mysql service>
+* port: <port of mysql servic\>
+```
+
+### Connection parameters for mariadb:
+-----
+```python
+* engine_type: mariadb
+* database: <name of database>
+* username: <mariadb user>
+* password: <user password>
+* host: <host of mariadb service>
+* port: <port of mariadb service>
+```
+
+### Connection parameters for snowflake:
+-----
+```python
+* engine_type: snowflake
+* database: <name of database>
+* username: <snowflake user>
+* password: <user password>
+* schema: <schema name>
+* snowflake_role: <snowflake role>
+* snowflake_warehouse: <snowflake warehouse>
+* snowflake_account: <snowflake account>
+```
+
+### Connection parameters for bigquery:
+-----
+```python
+* engine_type: bigquery
+* database: <name of database>
+```
+
+### Getting connection properties from AWS / GCP Secret Manager Service:
+-----
+Note:
+* GCP: 
+   * On Cloud Server:
+       * Set server to execute the all cloud api services
+       * Attach following permissions
+          * Project Viewer
+          * Secret Manager Secret Accessor
+   * On Premises:
+       * Attach following permissions to user service account and download service account file for authentication:
+          * Project Viewer
+          * Secret Manager Secret Accessor
+       * Set environment variable "GOOGLE_APPLICATION_CREDENTIALS" pointing to service account file.
+* AWS:
+   * On Cloud Server:
+      * Set execution profile with "secretsmanager:GetSecretValue" policy
+   * On Premises:
+      * AWS should be configured
+      * User should have permissions of "secretsmanager:GetSecretValue" policy.
+
+```python
+* engine_type: bigquery
+* database: <name of database>
+* secret_id: <Secret name of AWS / GCP Secret Manager Service>
+* secrete_manager_cloud: <aws or gcp as per cloud>
+* aws_region: <aws region: default=> us-east-1>
+```
+
+
+### Development Setup
+
+#### Using virtualenv
+
+```bash
+python3 -m venv venv
+source env/bin/activate
+pip install .
+```
+
+### Contributing
+
+1. Fork repo- https://github.com/shrivastava-v-ankit/database-factory.git
+2. Create your feature branch - `git checkout -b feature/name`
+3. Install Python packages
+   * sqlalchemy==1.4.47
+   * pandas==1.5.3
+   * GitPython
+   * coverage==7.2.3
+   * exceptiongroup==1.1.1
+   * iniconfig==2.0.0
+   * pluggy==1.0.0
+   * pytest==7.3.0
+   * pytest-cov==4.0.0
+   * tomli==2.0.1
+4. Run Python test (pytest)
+   * pytest -v --cov --cov-report html --cov-report xml --junitxml=test-results/database_factory_test/results.xml
+5. Add Python test (pytest) and covrage report for new/changed feature.
+4. Commit your changes - `git commit -am "Added name"`
+5. Push to the branch - `git push origin feature/name`
+6. Create a new pull request
+
+
+
```

### Comparing `database-factory-1.0.6/README.md` & `database-factory-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,35 @@
 Database factory can be enhanced for all the sqlalchemy supported database.
 
 ## Getting Started
 
 ```bash
 pip install database-factory
 ```
+Note: Default installation for database factory is to support Sqlite3. For other database/cloud support it can be installed with compinations of extra libraries
+
+### Sqite3 with AWS cloud support
+```bash
+pip install database-factory["aws"]
+```
+
+### Snowflake with AWS cloud support
+```bash
+pip install database-factory["snowflake,aws"]
+```
+
+### Following options are supported
+   * Secret manager cloud support
+      * aws
+      * gcp
+   * Databases
+      * snowflake
+      * postgres
+      * mysql
+   * all: Will install with libraries of all supported cloud and supported databases.
 
 ### Using database-factory
 -----
 ```python
 from database_factory.manager import DatabaseManager
 import tempfile
 temp_dir = tempfile.gettempdir()
```

### Comparing `database-factory-1.0.6/database_factory/cloud/aws/auth.py` & `database-factory-1.1.0/database_factory/cloud/aws/auth.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.6/database_factory/cloud/aws/secrete_manager.py` & `database-factory-1.1.0/database_factory/cloud/aws/secrete_manager.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.6/database_factory/cloud/gcp/auth.py` & `database-factory-1.1.0/database_factory/cloud/gcp/auth.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.6/database_factory/cloud/gcp/resource_manager.py` & `database-factory-1.1.0/database_factory/cloud/gcp/resource_manager.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.6/database_factory/cloud/gcp/secrete_manager.py` & `database-factory-1.1.0/database_factory/cloud/gcp/secrete_manager.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.6/database_factory/common/common.py` & `database-factory-1.1.0/database_factory/common/common.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.6/database_factory/manager.py` & `database-factory-1.1.0/database_factory/manager.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.6/database_factory/operations.py` & `database-factory-1.1.0/database_factory/operations.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.6/database_factory.egg-info/PKG-INFO` & `database-factory-1.1.0/database_factory.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,220 +1,249 @@
 Metadata-Version: 2.1
 Name: database-factory
-Version: 1.0.6
+Version: 1.1.0
 Summary: Database Factory;
 Home-page: https://github.com/shrivastava-v-ankit/database-factory
 Author: Ankit Shrivastava
 License: MIT
 Project-URL: Source, https://github.com/shrivastava-v-ankit/database-factory/
 Project-URL: Tracker, https://github.com/shrivastava-v-ankit/database-factory/issues
-Description: # database-factory
-        
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-        [![PyPI](https://img.shields.io/pypi/v/database-factory.svg)](https://pypi.org/project/database-factory)
-        [![CircleCI](https://circleci.com/gh/shrivastava-v-ankit/database-factory.svg?style=svg)](https://circleci.com/gh/shrivastava-v-ankit/database-factory)
-        
-        
-        
-        Database factory is used to manage/create database connection with execute queries using the connection.
-        The concept of having single source to connect various databases and perform database operations.
-        
-        User need not to worry on the crafting the connection string and to identify the methods for the database operations.
-        Database factory supports DML / DDL executions and have support of Pandas DataFrame to create or replace existing tables.
-        
-        Database factory is wrapper on sqlalchemy for crafting the connection and supports below databases:
-        
-        ```bash
-        * Sqlite3
-        * PostgreSQl
-        * BigQuery
-        * Snowflake
-        * MariaDB
-        * MySQL
-        ```
-        Database factory can be enhanced for all the sqlalchemy supported database.
-        
-        ## Getting Started
-        
-        ```bash
-        pip install database-factory
-        ```
-        
-        ### Using database-factory
-        -----
-        ```python
-        from database_factory.manager import DatabaseManager
-        import tempfile
-        temp_dir = tempfile.gettempdir()
-        db = DatabaseManager(engine_type="sqlite", database="test_db", sqlite_db_path=temp_dir)
-        db.create_session()
-        
-        db.execute_sql(sql="create table test (id int PRIMARY KEY)")
-        db.execute_sql(sql="insert into test values (1)")
-        db.execute_sql(sql="insert into test values (2)")
-        
-        rows = db.execute_sql(sql="select * from test")
-        if rows:
-          print(rows)
-        
-        
-        df = db.get_df(sql="select * from test")
-        print(df)
-        
-        db.execute_df(panda_df=df, table_name=copy_test, exist_action="replace")
-        # db.execute_df(panda_df=df, table_name=copy_test, exist_action="replace", chunk_size=100)
-        db.execute_sql(sql="insert into copy_test values (3)")
-        rows_copy = db.execute_sql(sql="select * from copy_test")
-        if rows_copy:
-          print(rows_copy)
-        ```
-        
-        ## Appendix
-        ### Supported database type:
-        ----
-        ```
-        *   sqlite `default`
-        *   postgres
-        *   mysql
-        *   mariadb
-        *   snowflake
-        ```
-        
-        ### Connection parameters for sqlite:
-        -----
-        ```python
-        * engine_type: sqlite
-        * database: <name of database>
-        * sqlite_db_path: <path where database will be created>
-        ```
-        
-        ### Connection parameters for postgres:
-        -----
-        ```python
-        * engine_type: postgres
-        * database: <name of database>
-        * username: <postgres user>
-        * password: <user password>
-        * host: <host of postgres service>
-        * port: <port of postgres service>
-        ```
-        
-        ### Connection parameters for mysql:
-        -----
-        ```python
-        * engine_type: mysql
-        * database: <name of database>
-        * username: <mysql user>
-        * password: <user password>
-        * host: <host of mysql service>
-        * port: <port of mysql servic\>
-        ```
-        
-        ### Connection parameters for mariadb:
-        -----
-        ```python
-        * engine_type: mariadb
-        * database: <name of database>
-        * username: <mariadb user>
-        * password: <user password>
-        * host: <host of mariadb service>
-        * port: <port of mariadb service>
-        ```
-        
-        ### Connection parameters for snowflake:
-        -----
-        ```python
-        * engine_type: snowflake
-        * database: <name of database>
-        * username: <snowflake user>
-        * password: <user password>
-        * schema: <schema name>
-        * snowflake_role: <snowflake role>
-        * snowflake_warehouse: <snowflake warehouse>
-        * snowflake_account: <snowflake account>
-        ```
-        
-        ### Connection parameters for bigquery:
-        -----
-        ```python
-        * engine_type: bigquery
-        * database: <name of database>
-        ```
-        
-        ### Getting connection properties from AWS / GCP Secret Manager Service:
-        -----
-        Note:
-        * GCP: 
-           * On Cloud Server:
-               * Set server to execute the all cloud api services
-               * Attach following permissions
-                  * Project Viewer
-                  * Secret Manager Secret Accessor
-           * On Premises:
-               * Attach following permissions to user service account and download service account file for authentication:
-                  * Project Viewer
-                  * Secret Manager Secret Accessor
-               * Set environment variable "GOOGLE_APPLICATION_CREDENTIALS" pointing to service account file.
-        * AWS:
-           * On Cloud Server:
-              * Set execution profile with "secretsmanager:GetSecretValue" policy
-           * On Premises:
-              * AWS should be configured
-              * User should have permissions of "secretsmanager:GetSecretValue" policy.
-        
-        ```python
-        * engine_type: bigquery
-        * database: <name of database>
-        * secret_id: <Secret name of AWS / GCP Secret Manager Service>
-        * secrete_manager_cloud: <aws or gcp as per cloud>
-        * aws_region: <aws region: default=> us-east-1>
-        ```
-        
-        
-        ### Development Setup
-        
-        #### Using virtualenv
-        
-        ```bash
-        python3 -m venv venv
-        source env/bin/activate
-        pip install .
-        ```
-        
-        ### Contributing
-        
-        1. Fork repo- https://github.com/shrivastava-v-ankit/database-factory.git
-        2. Create your feature branch - `git checkout -b feature/name`
-        3. Install Python packages
-           * sqlalchemy==1.4.47
-           * pandas==1.5.3
-           * GitPython
-           * coverage==7.2.3
-           * exceptiongroup==1.1.1
-           * iniconfig==2.0.0
-           * pluggy==1.0.0
-           * pytest==7.3.0
-           * pytest-cov==4.0.0
-           * tomli==2.0.1
-        4. Run Python test (pytest)
-           * pytest -v --cov --cov-report html --cov-report xml --junitxml=test-results/database_factory_test/results.xml
-        5. Add Python test (pytest) and covrage report for new/changed feature.
-        4. Commit your changes - `git commit -am "Added name"`
-        5. Push to the branch - `git push origin feature/name`
-        6. Create a new pull request
-        
-        
 Keywords: python,os independent,database,sqlalchemy,sqlite3,sqlite,postgres,mysql,maridb,snowflake,bigquery,secret manager
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Version Control :: Git
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.8, >=3.9, <3.10
 Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: aws
+Provides-Extra: gcp
+Provides-Extra: snowflake
+Provides-Extra: postgres
+Provides-Extra: mysql
+License-File: LICENSE
+
+# database-factory
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI](https://img.shields.io/pypi/v/database-factory.svg)](https://pypi.org/project/database-factory)
+[![CircleCI](https://circleci.com/gh/shrivastava-v-ankit/database-factory.svg?style=svg)](https://circleci.com/gh/shrivastava-v-ankit/database-factory)
+
+
+
+Database factory is used to manage/create database connection with execute queries using the connection.
+The concept of having single source to connect various databases and perform database operations.
+
+User need not to worry on the crafting the connection string and to identify the methods for the database operations.
+Database factory supports DML / DDL executions and have support of Pandas DataFrame to create or replace existing tables.
+
+Database factory is wrapper on sqlalchemy for crafting the connection and supports below databases:
+
+```bash
+* Sqlite3
+* PostgreSQl
+* BigQuery
+* Snowflake
+* MariaDB
+* MySQL
+```
+Database factory can be enhanced for all the sqlalchemy supported database.
+
+## Getting Started
+
+```bash
+pip install database-factory
+```
+Note: Default installation for database factory is to support Sqlite3. For other database/cloud support it can be installed with compinations of extra libraries
+
+### Sqite3 with AWS cloud support
+```bash
+pip install database-factory["aws"]
+```
+
+### Snowflake with AWS cloud support
+```bash
+pip install database-factory["snowflake,aws"]
+```
+
+### Following options are supported
+   * Secret manager cloud support
+      * aws
+      * gcp
+   * Databases
+      * snowflake
+      * postgres
+      * mysql
+   * all: Will install with libraries of all supported cloud and supported databases.
+
+### Using database-factory
+-----
+```python
+from database_factory.manager import DatabaseManager
+import tempfile
+temp_dir = tempfile.gettempdir()
+db = DatabaseManager(engine_type="sqlite", database="test_db", sqlite_db_path=temp_dir)
+db.create_session()
+
+db.execute_sql(sql="create table test (id int PRIMARY KEY)")
+db.execute_sql(sql="insert into test values (1)")
+db.execute_sql(sql="insert into test values (2)")
+
+rows = db.execute_sql(sql="select * from test")
+if rows:
+  print(rows)
+
+
+df = db.get_df(sql="select * from test")
+print(df)
+
+db.execute_df(panda_df=df, table_name=copy_test, exist_action="replace")
+# db.execute_df(panda_df=df, table_name=copy_test, exist_action="replace", chunk_size=100)
+db.execute_sql(sql="insert into copy_test values (3)")
+rows_copy = db.execute_sql(sql="select * from copy_test")
+if rows_copy:
+  print(rows_copy)
+```
+
+## Appendix
+### Supported database type:
+----
+```
+*   sqlite `default`
+*   postgres
+*   mysql
+*   mariadb
+*   snowflake
+```
+
+### Connection parameters for sqlite:
+-----
+```python
+* engine_type: sqlite
+* database: <name of database>
+* sqlite_db_path: <path where database will be created>
+```
+
+### Connection parameters for postgres:
+-----
+```python
+* engine_type: postgres
+* database: <name of database>
+* username: <postgres user>
+* password: <user password>
+* host: <host of postgres service>
+* port: <port of postgres service>
+```
+
+### Connection parameters for mysql:
+-----
+```python
+* engine_type: mysql
+* database: <name of database>
+* username: <mysql user>
+* password: <user password>
+* host: <host of mysql service>
+* port: <port of mysql servic\>
+```
+
+### Connection parameters for mariadb:
+-----
+```python
+* engine_type: mariadb
+* database: <name of database>
+* username: <mariadb user>
+* password: <user password>
+* host: <host of mariadb service>
+* port: <port of mariadb service>
+```
+
+### Connection parameters for snowflake:
+-----
+```python
+* engine_type: snowflake
+* database: <name of database>
+* username: <snowflake user>
+* password: <user password>
+* schema: <schema name>
+* snowflake_role: <snowflake role>
+* snowflake_warehouse: <snowflake warehouse>
+* snowflake_account: <snowflake account>
+```
+
+### Connection parameters for bigquery:
+-----
+```python
+* engine_type: bigquery
+* database: <name of database>
+```
+
+### Getting connection properties from AWS / GCP Secret Manager Service:
+-----
+Note:
+* GCP: 
+   * On Cloud Server:
+       * Set server to execute the all cloud api services
+       * Attach following permissions
+          * Project Viewer
+          * Secret Manager Secret Accessor
+   * On Premises:
+       * Attach following permissions to user service account and download service account file for authentication:
+          * Project Viewer
+          * Secret Manager Secret Accessor
+       * Set environment variable "GOOGLE_APPLICATION_CREDENTIALS" pointing to service account file.
+* AWS:
+   * On Cloud Server:
+      * Set execution profile with "secretsmanager:GetSecretValue" policy
+   * On Premises:
+      * AWS should be configured
+      * User should have permissions of "secretsmanager:GetSecretValue" policy.
+
+```python
+* engine_type: bigquery
+* database: <name of database>
+* secret_id: <Secret name of AWS / GCP Secret Manager Service>
+* secrete_manager_cloud: <aws or gcp as per cloud>
+* aws_region: <aws region: default=> us-east-1>
+```
+
+
+### Development Setup
+
+#### Using virtualenv
+
+```bash
+python3 -m venv venv
+source env/bin/activate
+pip install .
+```
+
+### Contributing
+
+1. Fork repo- https://github.com/shrivastava-v-ankit/database-factory.git
+2. Create your feature branch - `git checkout -b feature/name`
+3. Install Python packages
+   * sqlalchemy==1.4.47
+   * pandas==1.5.3
+   * GitPython
+   * coverage==7.2.3
+   * exceptiongroup==1.1.1
+   * iniconfig==2.0.0
+   * pluggy==1.0.0
+   * pytest==7.3.0
+   * pytest-cov==4.0.0
+   * tomli==2.0.1
+4. Run Python test (pytest)
+   * pytest -v --cov --cov-report html --cov-report xml --junitxml=test-results/database_factory_test/results.xml
+5. Add Python test (pytest) and covrage report for new/changed feature.
+4. Commit your changes - `git commit -am "Added name"`
+5. Push to the branch - `git push origin feature/name`
+6. Create a new pull request
+
+
+
```

### Comparing `database-factory-1.0.6/database_factory.egg-info/SOURCES.txt` & `database-factory-1.1.0/database_factory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.6/setup.py` & `database-factory-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 
 """
 Prerequesites -
   Python Packages:
     * setuptools
+    * wheel
     * GitPython
   System Packages:
     * make
     * Python 3
 Commands: python setup.py [bdist_wheel / [sdist [--format=[gztar][,tar]]]
 Ex:
   * python setup.py bdist_wheel
@@ -20,36 +21,50 @@
 """
 
 """
 distutils/setuptools install script.
 """
 
 
-from setuptools import setup, find_packages
+import sys
+from setuptools import setup
+from setuptools import find_packages
+from setuptools import Command
+from textwrap import wrap
 import traceback
 import shutil
 import re
 import os
 __NAME__ = "database-factory"
 
 ROOT = os.path.dirname(os.path.abspath(__file__))
 VERSION_FILE = os.path.join(ROOT, __NAME__.replace("-", "_"), ".version")
 VERSION_RE = re.compile(r'''__version__ = ['"]([0-9.]+)['"]''')
 
 base = [
     # Database Abstraction Library
     "sqlalchemy==1.4.47",
     # Powerful data structures for data analysis, time series, and statistics
-    "pandas==1.5.3"
-
+    "pandas==1.5.3",
+    "greenlet==2.0.2",
+    "python-dateutil==2.8.2",
+    "pytz==2023.3",
+    "six==1.16.0",
+    "numpy==1.24.2",
+    "pyarrow==6.0.1",
+    "pycparser==2.21"
 ]
 
 aws = [
     # The AWS SDK for Python
-    "boto3==1.26.113"
+    "boto3==1.26.113",
+    "botocore==1.29.113",
+    "jmespath==1.0.1",
+    "s3transfer==0.6.0",
+    "urllib3==1.26.15"
 ]
 
 gcp = [
     # This library simplifies using Google’s various server-to-server authentication mechanisms to access Google APIs.
     "google-auth==2.17.3",
     # This library provides an httplib2 transport for google-auth.
     "google-auth-httplib2==0.1.0",
@@ -58,84 +73,88 @@
     # Google API Client Library for Python
     "google-api-python-client==2.85.0",
     # Google Secret Manager API API client library
     "google-cloud-secret-manager==2.16.1",
     # Google Cloud Resource Manager API client lib
     "google-cloud-resource-manager==1.9.1",
     # SQLAlchemy dialect for BigQuery
-    "pybigquery==0.10.2"
-]
-
-snowflake = [
-    # Snowflake Connector Library
-    "snowflake-connector-python==2.7.9",
-    # Snowflake SQLAlchemy Dialect
-    "snowflake-sqlalchemy==1.4.7"
-]
-
-postgres = [
-    # PostgreSQL interface library.
-    "pg8000==1.29.4"
-]
-
-mysql = [
-    # Pure Python MySQL Driver
-    "pymysql==1.0.3"
-]
-
-dependencies = [
-    "asn1crypto==1.5.1",
-    "botocore==1.29.113",
-    "cachetools==5.3.0",
-    "certifi==2022.12.7",
-    "cffi==1.15.1",
-    "charset-normalizer==2.0.12",
-    "cryptography==36.0.2",
-    "future==0.18.3",
+    "pybigquery==0.10.2",
     "google-api-core==2.11.0",
     "google-cloud-bigquery-storage==2.19.1",
     "google-cloud-core==2.3.2",
     "google-crc32c==1.5.0",
     "google-resumable-media==2.4.1",
     "googleapis-common-protos==1.59.0",
-    "greenlet==2.0.2",
     "grpc-google-iam-v1==0.12.6",
     "grpcio==1.53.0",
     "httplib2==0.22.0",
+    "cachetools==5.3.0",
+    "certifi==2022.12.7",
+    "charset-normalizer==2.0.12",
+    "future==0.18.3",
     "idna==3.4",
-    "jmespath==1.0.1",
-    "numpy==1.24.2",
-    "oscrypto==1.3.0",
     "packaging==23.1",
     "proto-plus==1.22.2",
     "protobuf==3.20.3",
-    "pyarrow==6.0.1",
     "pyasn1==0.4.8",
     "pyasn1-modules==0.2.8",
-    "pycparser==2.21",
-    "pycryptodomex==3.17",
-    "pyjwt==2.6.0",
-    "pymysql==1.0.3",
-    "pyopenssl==22.0.0",
     "pyparsing==3.0.9",
-    "python-dateutil==2.8.2",
-    "pytz==2023.3",
     "requests==2.28.2",
     "rsa==4.9",
-    "s3transfer==0.6.0",
-    "scramp==1.4.4",
-    "six==1.16.0",
     "uritemplate==4.1.1",
+    "grpcio-status==1.48.2",
     "urllib3==1.26.15"
 ]
 
-setups = []
+snowflake = [
+    # Snowflake Connector Library
+    "snowflake-connector-python==2.7.9",
+    # Snowflake SQLAlchemy Dialect
+    "snowflake-sqlalchemy==1.4.7",
+    "pyjwt==2.6.0",
+    "asn1crypto==1.5.1",
+    "certifi==2022.12.7",
+    "cffi==1.15.1",
+    "charset-normalizer==2.0.12",
+    "cryptography==36.0.2",
+    "idna==3.4",
+    "oscrypto==1.3.0",
+    "pyopenssl==22.0.0",
+    "pyparsing==3.0.9",
+    "pycryptodomex==3.17",
+    "requests==2.28.2",
+    "urllib3==1.26.15"
+]
 
-ir = (base + aws + gcp + snowflake + postgres + mysql + dependencies)
-requires = ir
+postgres = [
+    # PostgreSQL interface library.
+    "pg8000==1.29.4",
+    "asn1crypto==1.5.1",
+    "scramp==1.4.4",
+]
+
+mysql = [
+    # Pure Python MySQL Driver
+    "pymysql==1.0.3"
+]
+
+setups = [
+    'gitpython',
+    'setuptools',
+    'wheel'
+]
+
+extras = {
+    "all": (aws + gcp + snowflake + postgres + mysql),
+    "aws": aws,
+    "gcp": gcp,
+    "snowflake": snowflake,
+    "postgres": postgres,
+    "mysql": mysql
+}
 
 
 def delete(path):
     if os.path.exists(path=path):
         try:
             if os.path.isfile(path=path):
                 os.remove(path=path)
@@ -185,14 +204,34 @@
     return version
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
+class List_Extras(Command):
+    """
+    List all available extras
+    Registered as cmdclass in setup() so it can be called with ``python setup.py list_extras``.
+    """
+
+    description = "List available extras"
+    user_options = []
+
+    def initialize_options(self):
+        """Set default values for options."""
+
+    def finalize_options(self):
+        """Set final values for options."""
+
+    def run(self):
+        """List extras."""
+        print("\n".join(wrap(", ".join(extras.keys()), 100)))
+
+
 def do_setup():
     setup(
         name=__NAME__,
         version=get_version(filename=VERSION_FILE),
         description="Database Factory;",
         long_description=long_description,
         long_description_content_type="text/markdown",
@@ -200,30 +239,33 @@
                   'sqlite3', 'sqlite', 'postgres', 'mysql', 'maridb',
                   'snowflake', 'bigquery', 'secret manager'],
         author="Ankit Shrivastava",
         url="https://github.com/shrivastava-v-ankit/database-factory",
         packages=find_packages(include=[__NAME__.replace("-", "_")]),
         include_package_data=True,
         setup_requires=setups,
-        install_requires=requires,
+        install_requires=base,
+        extras_require=extras,
         license="MIT",
-        python_requires=">=3.7, <4",
+        python_requires=">=3.8, >=3.9, <3.10",
         platforms='any',
+        cmdclass={
+            'list_extras': List_Extras,
+        },
         project_urls={
             'Source': 'https://github.com/shrivastava-v-ankit/database-factory/',
             'Tracker': 'https://github.com/shrivastava-v-ankit/database-factory/issues',
         },
         classifiers=[
             'Development Status :: 5 - Production/Stable',
             'Environment :: Web Environment',
             'Intended Audience :: Developers',
             'Natural Language :: English',
             'License :: OSI Approved :: MIT License',
             'Operating System :: OS Independent',
-            'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Topic :: Software Development :: Libraries :: Python Modules',
             'Topic :: Software Development :: Version Control :: Git',
         ],
     )
```


# Comparing `tmp/odbms-0.3.2.tar.gz` & `tmp/odbms-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odbms-0.3.2.tar", last modified: Wed May  1 15:03:19 2024, max compression
+gzip compressed data, was "odbms-0.3.3.tar", last modified: Fri May  3 18:41:48 2024, max compression
```

## Comparing `odbms-0.3.2.tar` & `odbms-0.3.3.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:03:19.969566 odbms-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-01 15:03:15.000000 odbms-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 15:03:15.000000 odbms-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-01 15:03:19.965566 odbms-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-01 15:03:15.000000 odbms-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:03:19.965566 odbms-0.3.2/odbms/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/dbms.py
--rw-r--r--   0 runner    (1001) docker     (127)    16733 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:03:19.965566 odbms-0.3.2/odbms/orms/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/orms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/orms/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/orms/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/orms/mysqldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/orms/postgresqldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/orms/sqlitedb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:03:19.965566 odbms-0.3.2/odbms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-01 15:03:19.000000 odbms-0.3.2/odbms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-01 15:03:19.000000 odbms-0.3.2/odbms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:03:19.000000 odbms-0.3.2/odbms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-01 15:03:19.000000 odbms-0.3.2/odbms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 15:03:19.000000 odbms-0.3.2/odbms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 15:03:19.969566 odbms-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-01 15:03:15.000000 odbms-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:41:48.844536 odbms-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-03 18:41:45.000000 odbms-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 18:41:45.000000 odbms-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-03 18:41:48.844536 odbms-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 18:41:45.000000 odbms-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:41:48.840536 odbms-0.3.3/odbms/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-03 18:41:45.000000 odbms-0.3.3/odbms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-03 18:41:45.000000 odbms-0.3.3/odbms/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-03 18:41:45.000000 odbms-0.3.3/odbms/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-03 18:41:45.000000 odbms-0.3.3/odbms/dbms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-03 18:41:45.000000 odbms-0.3.3/odbms/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19321 2024-05-03 18:41:45.000000 odbms-0.3.3/odbms/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:41:48.844536 odbms-0.3.3/odbms/orms/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-03 18:41:45.000000 odbms-0.3.3/odbms/orms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-03 18:41:45.000000 odbms-0.3.3/odbms/orms/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-03 18:41:45.000000 odbms-0.3.3/odbms/orms/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-03 18:41:45.000000 odbms-0.3.3/odbms/orms/mysqldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9009 2024-05-03 18:41:45.000000 odbms-0.3.3/odbms/orms/postgresqldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-03 18:41:45.000000 odbms-0.3.3/odbms/orms/sqlitedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-03 18:41:45.000000 odbms-0.3.3/odbms/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:41:48.844536 odbms-0.3.3/odbms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-03 18:41:48.000000 odbms-0.3.3/odbms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-03 18:41:48.000000 odbms-0.3.3/odbms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 18:41:48.000000 odbms-0.3.3/odbms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 18:41:48.000000 odbms-0.3.3/odbms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 18:41:48.000000 odbms-0.3.3/odbms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 18:41:48.844536 odbms-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-03 18:41:45.000000 odbms-0.3.3/setup.py
```

### Comparing `odbms-0.3.2/LICENSE` & `odbms-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `odbms-0.3.2/PKG-INFO` & `odbms-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbms
-Version: 0.3.2
+Version: 0.3.3
 Summary: Database client for Mysql, MongoDB and Sqlite
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/odbms/
 Project-URL: Tracker, https://github.com/theonlyamos/odbms/issues
 Keywords: python3 runit developer serverless architecture docker sqlite mysql mongodb
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `odbms-0.3.2/odbms/database.py` & `odbms-0.3.3/odbms/database.py`

 * *Files identical despite different names*

### Comparing `odbms-0.3.2/odbms/dbms.py` & `odbms-0.3.3/odbms/dbms.py`

 * *Files identical despite different names*

### Comparing `odbms-0.3.2/odbms/model.py` & `odbms-0.3.3/odbms/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import json
 
 from bson.objectid import ObjectId
 from .dbms import DBMS
 
 class Model():
     '''A model class'''
-    TABLE_NAME = ''
+    TABLE_NAME: str = ''
     SELECTED_COLUMNS = []
     WHERE_CLAUSE = []
-    GROUP_BY = ''
+    GROUP_BY: str = ''
     ORDER_BY = ()
     LIMIT = 0
 
     def __init__(self, created_at: Optional[str] = None, updated_at: Optional[str] = None, id: Optional[str] = None):
         self.created_at = (datetime.now()).strftime("%a %b %d %Y %H:%M:%S") \
             if not created_at else created_at
         self.updated_at = (datetime.now()).strftime("%a %b %d %Y %H:%M:%S") \
@@ -105,31 +105,77 @@
             bool: "BOOLEAN",
             list: "TEXT",
             dict: "TEXT"
             # Add more mappings as needed
         }
         return type_mapping.get(attr_type, "TEXT")
 
+    @classmethod
+    def alter_table(cls, changes: dict):
+        """
+        Alter the table structure by adding, modifying, or dropping columns.
+
+        @param changes: A dictionary mapping column names to their new data types.
+        """
+        if DBMS.Database.dbms != 'mongodb':
+            # Fetch existing columns from the database
+            fetch_columns_sql = f"SELECT column_name FROM information_schema.columns WHERE table_name='{cls.TABLE_NAME}';"
+            existing_columns = {row['column_name'] for row in DBMS.Database.execute(fetch_columns_sql)}
+            default_columns = {'id', 'created_at', 'updated_at'}
+            # Determine columns to add or modify and columns to drop
+            specified_columns = set(changes.keys())
+            specified_columns.update(default_columns)
+            columns_to_drop = existing_columns - specified_columns
+            columns_to_add_or_modify = specified_columns - existing_columns
+            
+            alter_statements = []
+
+            # Handle adding or modifying columns
+            for column, data_type in changes.items():
+                column_type = cls.get_column_type(data_type)
+                if column in columns_to_add_or_modify:
+                    alter_statements.append(f"ADD COLUMN {column} {column_type}")
+                else:
+                    # Modify existing column
+                    if DBMS.Database.dbms in ['mysql', 'postgresql']:
+                        alter_statements.append(f"ALTER COLUMN {column} TYPE {column_type}")
+                    elif DBMS.Database.dbms == 'sqlite':
+                        # SQLite does not support MODIFY COLUMN directly, needs table recreation
+                        continue  # Handle SQLite modifications separately if needed
+
+            # Handle dropping columns
+            for column in columns_to_drop:
+                if DBMS.Database.dbms in ['mysql', 'postgresql']:
+                    alter_statements.append(f"DROP COLUMN {column}")
+                elif DBMS.Database.dbms == 'sqlite':
+                    # SQLite does not support DROP COLUMN directly, needs table recreation
+                    continue  # Handle SQLite drops separately if needed
+
+            # Execute all alter statements
+            for statement in alter_statements:
+                alter_sql = f"ALTER TABLE {cls.TABLE_NAME} {statement};"
+                DBMS.Database.execute(alter_sql)
+
     def save(self):
         '''
         Instance Method for saving Model instance to database
 
         @params None
         @return None
         '''
 
         data = self.__dict__.copy()
         
         if DBMS.Database.dbms != 'mongodb':
             data['updated_at'] = (datetime.now()).strftime("%a %b %d %Y %H:%M:%S")
             del data["created_at"]
             del data["updated_at"]
-
+            
         if isinstance(self.id, ObjectId):
-            return DBMS.Database.insert(self.TABLE_NAME, Model.normalise(data, 'params'))
+            return DBMS.Database.insert(self.TABLE_NAME, self.normalise(data, 'params'))
         
         # Update the existing record in database
         data.pop('id', None)
         return DBMS.Database.update(self.TABLE_NAME, self.normalise({'id': self.id}, 'params'), self.normalise(data, 'params'))
 
     @staticmethod
     def insert(document):
@@ -231,20 +277,18 @@
         Class Method for retrieving \n
         model data from database
 
         @param _id ID of Model
         @return Model instance(s)
         '''
 
-        result = DBMS.Database.find_one(cls.TABLE_NAME, cls.normalise({'id': id}, 'params'))
-        
-        if isinstance(result, dict):
-            return cls(**cls.normalise(result)) if len(result.keys()) else None
-        elif isinstance(result, list) or isinstance(result, tuple):
-            return cls(*result) if len(result) else None
+        result = cls.normalise(DBMS.Database.find_one(cls.TABLE_NAME, cls.normalise({'id': id}, 'params'))) # type: ignore
+
+        return cls(**result) if len(result.keys()) else None
+    
         
         # query = 'SELECT '
         # if cls.SELECTED_COLUMNS:
         #     query += cls.SELECTED_COLUMNS if type(cls.SELECTED_COLUMNS) is str \
         #         else ', '.join(cls.SELECTED_COLUMNS)
         # else:
         #     query += "*"
@@ -324,15 +368,15 @@
         Class Method for retrieving one model
         imstance by provided parameters
 
         @param params
         @return List[Model]
         '''
 
-        result = cls.normalise(DBMS.Database.find_one(cls.TABLE_NAME, cls.normalise(params, 'params'), projection))
+        result = cls.normalise(DBMS.Database.find_one(cls.TABLE_NAME, cls.normalise(params, 'params'), projection)) # type: ignore
 
         return cls(**result) if len(result.keys()) else None
     
     @classmethod
     def query(cls, column: str, search: str):
         '''
         Class Method for retrieving products
@@ -433,16 +477,19 @@
 
         @paramas None
         @return dict() format of Function instance
         '''
         
         data = self.__dict__.copy()
         
-        data['created_at'] = data['created_at'].strftime("%a %b %d %Y %H:%M:%S")
-        data['updated_at'] = data['updated_at'].strftime("%a %b %d %Y %H:%M:%S")
+        if isinstance(data['created_at'], datetime):
+            data['created_at'] = data['created_at'].strftime("%a %b %d %Y %H:%M:%S")
+            
+        if isinstance(data['updated_at'], datetime):
+            data['updated_at'] = data['updated_at'].strftime("%a %b %d %Y %H:%M:%S")
 
         data.pop('password', None)
 
         return data
     
     @classmethod
     def normalise(cls, content: dict|None, optype: str = 'dbresult')-> dict:
@@ -479,24 +526,27 @@
                 for key, value in content.items():
                     if type(value) == list:
                         content[key] = '::'.join([str(v) for v in value])
                 normalized = content
             return normalized
         else:
             if optype == 'params':
-                if 'id' in content.keys():
-                    content['id'] = str(content['id'])
+                if '_id' in content.keys():
+                    content['id'] = str(content['_id'])
+                    del content['_id']
                 for key, value in content.items():
-                    if type(value) == list:
+                    if isinstance(value, ObjectId):
+                        content[key] = str(value)
+                    elif type(value) == list:
                         content[key] = '::'.join([str(v) for v in value])
-
                     elif type(value) == datetime:
                         content[key] = value.strftime("%a %b %d %Y %H:%M:%S")
                     elif type(value) == dict:
                         content[key] = json.dumps(value) # type: ignore
+                
             else:
                 init_signatures = inspect.signature(cls.__init__)
             
                 init_parameters = [param for param in init_signatures.parameters.values()
                                 if param.name != 'self']
                 
                 all_parameters = init_parameters
```

### Comparing `odbms-0.3.2/odbms/orms/base.py` & `odbms-0.3.3/odbms/orms/base.py`

 * *Files identical despite different names*

### Comparing `odbms-0.3.2/odbms/orms/mongodb.py` & `odbms-0.3.3/odbms/orms/mongodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
             client = MongoClient(host, int(port))
         else:
             client = MongoClient(host)
         MongoDB.db = client[database]
 
     @staticmethod
     def insert(collection: str, data: dict):
-        return MongoDB.db[collection].insert_one(data)
+        result = MongoDB.db[collection].insert_one(data)
+        return result.inserted_id
 
     @staticmethod
     def insert_many(collection: str, data: dict):
         return MongoDB.db[collection].insert_many(data)
 
     @staticmethod
     def find(collection: str, filter: dict = {}, projection: Union[list,dict] = []):
```

### Comparing `odbms-0.3.2/odbms/orms/mysqldb.py` & `odbms-0.3.3/odbms/orms/mysqldb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!python3
 # -*- coding: utf-8 -*-
 # @Date    : 2022-07-22 11:42:39
 # @Author  : Amos Amissah (theonlyamos@gmai.com)
 # @Link    : link
 # @Version : 1.0.0
 
+import logging
 import os
 from mysql import connector
 from sys import exit
 
 from .base import ORM
 
 class MysqlDB(ORM):
@@ -60,15 +61,16 @@
         try:
             MysqlDB.cursor.execute(query)
             MysqlDB.db.commit()
 
             return str(MysqlDB.cursor.lastrowid)
 
         except Exception as e:
-            return {'status': 'Error', 'message': str(e)}
+            logging.error(f"Error: {str(e)}")
+            return 0
     
     @staticmethod
     def update(table: str, filter: dict, data: dict):
 
         query = f'UPDATE {table} SET'
         for key in data.keys():
             query += f" {key}= ?,"
@@ -125,15 +127,16 @@
         try:
             MysqlDB.cursor.execute(query, tuple(filter.values()))
             MysqlDB.db.commit()
 
             return MysqlDB.cursor.fetchone()
 
         except Exception as e:
-            return {'status': 'Error', 'message': str(e)}
+            logging.error(f"Error: {str(e)}")
+            return {}
     
     @staticmethod
     def count(table: str, filter: dict = {}, columns: list = ['*'])-> int:
         columns = ', '.join(columns)
         query = f'SELECT {columns} FROM {table}'
 
         if len(filter.keys()):
```

### Comparing `odbms-0.3.2/odbms/orms/postgresqldb.py` & `odbms-0.3.3/odbms/orms/postgresqldb.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,27 +45,34 @@
                 password=password
             )
             PostgresqlDB.db.set_session(autocommit=False)
             PostgresqlDB.cursor = PostgresqlDB.db.cursor()
             
         except (Exception, psycopg2.Error) as error:
             logging.error("Error connecting to PostgreSQL database:", error)
-
+    
     @staticmethod
     def execute(query, params=None):
         try:
             if params:
                 PostgresqlDB.cursor.execute(query, params)
             else:
                 PostgresqlDB.cursor.execute(query)
-                PostgresqlDB.db.commit()
-
+                if PostgresqlDB.cursor.description:  # Check if description is not None
+                    column_names = [desc.name for desc in PostgresqlDB.cursor.description]
+                    result = [dict(zip(column_names, row)) for row in PostgresqlDB.cursor.fetchall()]
+                    PostgresqlDB.db.commit()
+                    return result
+                else:
+                    PostgresqlDB.db.commit()
+                    return []  # Return an empty list or appropriate value for queries that do not return rows
         except (Exception, psycopg2.Error) as error:
             logging.exception(error)
             PostgresqlDB.db.rollback()
+            return []
 
     @staticmethod
     def insert(table: str, data: Dict):
         columns = sql.SQL(', ').join(sql.Identifier(col) for col in data.keys())
         values = ', '.join(['%s'] * len(data))
         sql_query = sql.SQL("INSERT INTO {} ({}) VALUES ({}) RETURNING id").format(
             sql.Identifier(table),
@@ -73,15 +80,15 @@
             sql.SQL(values)
         )
         try:
             PostgresqlDB.cursor.execute(sql_query, list(data.values()))
             PostgresqlDB.db.commit()
             new_inserts = PostgresqlDB.cursor.fetchone()
             insert_id =   new_inserts[0] if new_inserts else 0
-            return insert_id
+            return str(insert_id)
         except (Exception, psycopg2.Error) as error:
             print("Error inserting data:", error)
             PostgresqlDB.db.rollback()
             return 0
 
     @staticmethod
     def insert_many(table: str, data: List[Dict]):
```

### Comparing `odbms-0.3.2/odbms/orms/sqlitedb.py` & `odbms-0.3.3/odbms/orms/sqlitedb.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,16 @@
         try:
             SqliteDB.cursor.execute(query)
             SqliteDB.db.commit()
 
             return str(SqliteDB.cursor.lastrowid)
 
         except Exception as e:
-            return {'status': 'Error', 'message': str(e)}
+            logging.error(f"Error: {str(e)}")
+            return 0
     
     @staticmethod
     def insert_many(tale: str, data: list[dict]):
         return {}
     
     @staticmethod
     def update(table: str, params: dict, data: dict)-> Union[int, None]:
@@ -106,15 +107,16 @@
             query = query.rstrip(',')
         
         try:
             SqliteDB.cursor.execute(query, tuple(params.values()))
             SqliteDB.db.commit()
 
             resp = [x for x in SqliteDB.cursor.fetchall()]
-            return resp[0] if len(resp) else resp
+            
+            return resp[0] if len(resp) else {}
 
         except Exception as e:
             logging.error({'status': 'Error', 'message': str(e)})
             return []
     
     @staticmethod
     def count(table: str, params: dict = {})-> int:
```

### Comparing `odbms-0.3.2/odbms.egg-info/PKG-INFO` & `odbms-0.3.3/odbms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbms
-Version: 0.3.2
+Version: 0.3.3
 Summary: Database client for Mysql, MongoDB and Sqlite
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/odbms/
 Project-URL: Tracker, https://github.com/theonlyamos/odbms/issues
 Keywords: python3 runit developer serverless architecture docker sqlite mysql mongodb
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `odbms-0.3.2/setup.py` & `odbms-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from importlib.metadata import entry_points
 from setuptools import setup, find_packages
 
-VERSION = '0.3.2'
+VERSION = '0.3.3'
 
 with open('README.md', 'rt') as file:
     description = file.read()
 
 setup(
     name='odbms',
     version=VERSION,
```


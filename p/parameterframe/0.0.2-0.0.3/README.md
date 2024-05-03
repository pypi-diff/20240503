# Comparing `tmp/parameterframe-0.0.2.tar.gz` & `tmp/parameterframe-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parameterframe-0.0.2.tar", last modified: Wed May  1 00:04:14 2024, max compression
+gzip compressed data, was "parameterframe-0.0.3.tar", last modified: Fri May  3 10:28:18 2024, max compression
```

## Comparing `parameterframe-0.0.2.tar` & `parameterframe-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:04:14.798398 parameterframe-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-01 00:01:16.000000 parameterframe-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    38966 2024-05-01 00:04:14.798398 parameterframe-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-01 00:01:16.000000 parameterframe-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:04:14.798398 parameterframe-0.0.2/parameterframe/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-01 00:04:14.000000 parameterframe-0.0.2/parameterframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    69559 2024-05-01 00:04:14.000000 parameterframe-0.0.2/parameterframe/parameterframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-01 00:04:14.000000 parameterframe-0.0.2/parameterframe/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:04:14.798398 parameterframe-0.0.2/parameterframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    38966 2024-05-01 00:04:14.000000 parameterframe-0.0.2/parameterframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-01 00:04:14.000000 parameterframe-0.0.2/parameterframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:04:14.000000 parameterframe-0.0.2/parameterframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-01 00:04:14.000000 parameterframe-0.0.2/parameterframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 00:04:14.000000 parameterframe-0.0.2/parameterframe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:04:14.798398 parameterframe-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:28:18.392570 parameterframe-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-03 10:24:29.000000 parameterframe-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    39020 2024-05-03 10:28:18.392570 parameterframe-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-03 10:24:29.000000 parameterframe-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:28:18.392570 parameterframe-0.0.3/parameterframe/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 10:28:17.000000 parameterframe-0.0.3/parameterframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79272 2024-05-03 10:28:17.000000 parameterframe-0.0.3/parameterframe/parameterframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-03 10:28:18.000000 parameterframe-0.0.3/parameterframe/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:28:18.392570 parameterframe-0.0.3/parameterframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    39020 2024-05-03 10:28:18.000000 parameterframe-0.0.3/parameterframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-03 10:28:18.000000 parameterframe-0.0.3/parameterframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:28:18.000000 parameterframe-0.0.3/parameterframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-03 10:28:18.000000 parameterframe-0.0.3/parameterframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 10:28:18.000000 parameterframe-0.0.3/parameterframe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 10:28:18.392570 parameterframe-0.0.3/setup.cfg
```

### Comparing `parameterframe-0.0.2/LICENSE` & `parameterframe-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `parameterframe-0.0.2/PKG-INFO` & `parameterframe-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parameterframe
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','parameter storage']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -25,15 +25,15 @@
 
 
 ```python
 import sys
 import pandas as pd
 import os
 sys.path.append('../')
-from python_modules.parameterframe import FileTypeHandler, ParameterFrame, DatabaseConnector
+from python_modules.parameterframe import FileTypeHandler, ParameterFrame, MockerDatabaseConnector, SqlAlchemyDatabaseManager
 
 ```
 
 ## Content
 
 1. Processing and reconstructing yaml and txt with FileTypeHandler
 2. Assembling parameter sets and adding to solution with ParameterFrame
@@ -42,15 +42,17 @@
 ### 1. Processing and reconstructing yaml and txt with FileTypeHandler
 
 
 ```python
 params_path = "../tests/parameterframe/example_configs"
 
 pf = ParameterFrame(
-    params_path = params_path
+    params_path = params_path,
+    database_connector = SqlAlchemyDatabaseManager(connection_details = {
+    'base_url' : 'postgresql+psycopg2://postgres:mysecretpassword@localhost:5432/mytestdb'})
 )
 
 pf.process_parameters_from_files()
 ```
 
 ### 2. Assembling parameter sets and adding to solution with ParameterFrame
 
@@ -78,15 +80,15 @@
 
 
     {'solution_id': 'ffb2fa4d1f14786e7a11641a870c3db55f08f375fb7ac00c9a2127f7cd801a60',
      'solution_description': {'solution_id': 'ffb2fa4d1f14786e7a11641a870c3db55f08f375fb7ac00c9a2127f7cd801a60',
       'solution_name': 'example_solution',
       'solution_description': 'example solution for test',
       'deployment_date': None,
-      'deprication_date': None,
+      'deprecation_date': None,
       'maintainers': None}}
 
 
 
 
 ```python
 pf.add_parameter_set_to_solution(solution_name="example_solution",
@@ -127,15 +129,15 @@
   </thead>
   <tbody>
     <tr>
       <th>0</th>
       <td>ffb2fa4d1f14786e7a11641a870c3db55f08f375fb7ac0...</td>
       <td>a54f04d2ff154294309403206e059aec556cdcfa511206...</td>
       <td>STAGING</td>
-      <td>2024-04-21 23:18:22</td>
+      <td>2024-05-02 18:36:32</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
@@ -175,15 +177,15 @@
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>solution_id</th>
       <th>solution_name</th>
       <th>solution_description</th>
       <th>deployment_date</th>
-      <th>deprication_date</th>
+      <th>deprecation_date</th>
       <th>maintainers</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <th>0</th>
       <td>ffb2fa4d1f14786e7a11641a870c3db55f08f375fb7ac0...</td>
@@ -237,15 +239,15 @@
   </thead>
   <tbody>
     <tr>
       <th>0</th>
       <td>ffb2fa4d1f14786e7a11641a870c3db55f08f375fb7ac0...</td>
       <td>a54f04d2ff154294309403206e059aec556cdcfa511206...</td>
       <td>STAGING</td>
-      <td>2024-04-21 23:18:22</td>
+      <td>2024-05-02 18:36:32</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
@@ -1061,54 +1063,48 @@
 
 
 ```python
 pf.push_solution(solution_id='ffb2fa4d1f14786e7a11641a870c3db55f08f375fb7ac00c9a2127f7cd801a60',
                  parameter_set_ids=['a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5'])
 ```
 
-    HTTP Request: POST http://localhost:8000/insert "HTTP/1.1 200 OK"
-
-
 
 
 
     True
 
 
 
 ### 5. Pulling solution with DatabaseConnector
 
 
 ```python
 params_path = "../tests/parameterframe/example_configs"
 
 pf2 = ParameterFrame(
-    params_path = params_path
+    params_path = params_path,
+    database_connector = SqlAlchemyDatabaseManager(connection_details = {
+    'base_url' : 'postgresql+psycopg2://postgres:mysecretpassword@localhost:5432/mytestdb'})
 )
 
 pf2.pull_solution(solution_id='ffb2fa4d1f14786e7a11641a870c3db55f08f375fb7ac00c9a2127f7cd801a60',
                  parameter_set_id='a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5')
 ```
 
-    HTTP Request: POST http://localhost:8000/search "HTTP/1.1 200 OK"
-    HTTP Request: POST http://localhost:8000/search "HTTP/1.1 200 OK"
-    HTTP Request: POST http://localhost:8000/search "HTTP/1.1 200 OK"
-
-
 ### 6. Reconstructing files
 
 
 ```python
 os.listdir("../tests/parameterframe/reconstructed_files")
 ```
 
 
 
 
-    ['.gitignore']
+    []
 
 
 
 
 ```python
 pf2.reconstruct_parameter_set(
     solution_name = "example_solution",
@@ -1123,13 +1119,12 @@
 ```
 
 
 
 
     ['param_2.yaml',
      'param_11.dill',
-     '.gitignore',
      'param_1.yaml',
      'param_10.txt',
      'param_21.ipynb']
```

### Comparing `parameterframe-0.0.2/README.md` & `parameterframe-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `parameterframe-0.0.2/parameterframe/parameterframe.py` & `parameterframe-0.0.3/parameterframe/parameterframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 from datetime import datetime
 from mocker_db import MockerDB, MockerConnector #==0.1.1
 import yaml
 from collections import defaultdict
 import logging
 import ast
 
+from sqlalchemy import create_engine, Column, String, Text, ForeignKey, DateTime
+from sqlalchemy.orm import relationship, sessionmaker, declarative_base
+from sqlalchemy.exc import SQLAlchemyError, IntegrityError, DBAPIError
+from sqlalchemy import inspect
+
 __design_choices__ = {
     "FileTypeHandler" : ['prepares one parameter file and reconstructs one parameter file at a time',
                          'txt and yaml files can be processed',
                          'yaml files are not reconstructed 1to1 but are first make into python dictionary, with python type mapping'],
     "ParameterFrame" : ['parameter_names and paramer_description are optional'],
     "DatabaseConnector" : ['connector is an external component that includes handling of connection to some database',
                            'default connector is meant for MockerDB',
@@ -35,15 +40,15 @@
     "author": "Kyrylo Mordan",
     "author_email": "parachute.repo@gmail.com",
     "description": "A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.",
     "keywords" : ['python', 'parameter storage']
 }
 
 @attr.s
-class DatabaseConnector:
+class MockerDatabaseConnector:
 
     db_handler = attr.ib(default=MockerDB)
     db_remote_handler = attr.ib(default=MockerConnector)
     db_handler_params = attr.ib(default = {
         'file_path' : "./parameterframe_storage",
          'persist' : True})
     connection_details = attr.ib(default = {
@@ -245,14 +250,235 @@
             parameter_set_descriptions,
             parameter_descriptions,
             parameter_attributes,
             attribute_values
         )
 
 
+@attr.s
+class SqlAlchemyDatabaseManager:
+
+
+    connection_details = attr.ib(default = {
+        'base_url' : "http://localhost:8000"})
+
+    _instance = None
+    Base = declarative_base()
+
+    logger = attr.ib(default=None)
+    logger_name = attr.ib(default='SqlAlchemy Database Connector')
+    loggerLvl = attr.ib(default=logging.INFO)
+    logger_format = attr.ib(default=None)
+
+
+    def __new__(cls, *args, **kwargs):
+        if not cls._instance:
+            cls._instance = super(SqlAlchemyDatabaseManager, cls).__new__(cls)
+        return cls._instance
+
+    def __attrs_post_init__(self):
+
+        if not hasattr(self, 'engine'):
+            self.engine = create_engine(self.connection_details['base_url'])
+            self.Session = sessionmaker(bind=self.engine)
+
+        self._initialize_logger()
+
+    def _initialize_logger(self):
+
+        """
+        Initialize a logger for the class instance based on the specified logging level and logger name.
+        """
+
+        if self.logger is None:
+            logging.basicConfig(level=self.loggerLvl, format=self.logger_format)
+            logger = logging.getLogger(self.logger_name)
+            logger.setLevel(self.loggerLvl)
+
+            self.logger = logger
+
+    class AttributeValues(Base):
+        __tablename__ = 'attribute_values'
+        attribute_id = Column(String, primary_key=True)
+        previous_attribute_id = Column(String, nullable=True)
+        attribute_name = Column(String)
+        attribute_value = Column(String)
+        attribute_value_type = Column(String)
+
+    class ParameterDescription(Base):
+        __tablename__ = 'parameter_description'
+        parameter_id = Column(String, primary_key=True)
+        parameter_name = Column(String)
+        parameter_description = Column(Text)
+        file_name = Column(String)
+        file_type = Column(String)
+
+    class ParameterAttribute(Base):
+        __tablename__ = 'parameter_attribute'
+        parameter_id = Column(String, ForeignKey('parameter_description.parameter_id'), primary_key=True)
+        attribute_id = Column(String, ForeignKey('attribute_values.attribute_id'), primary_key=True)
+        previous_attribute_id = Column(String, nullable=True)
+        attribute_values = relationship("AttributeValues")
+        parameter_description = relationship("ParameterDescription")
+
+    class ParameterSet(Base):
+        __tablename__ = 'parameter_set'
+        parameter_set_id = Column(String, primary_key=True)
+        parameter_id = Column(String,primary_key=True)
+        #parameter_description = relationship("ParameterDescription")
+        # If ParameterAttribute should be related here, it needs adjustment.
+
+    class SolutionParameterSet(Base):
+        __tablename__ = 'solution_parameter_set'
+        solution_id = Column(String, primary_key=True)
+        parameter_set_id = Column(String, primary_key=True)
+        #parameter_set = relationship("ParameterSet")
+        deployment_status = Column(String)
+        insertion_datetime = Column(String)
+
+
+    class ParameterSetDescription(Base):
+        __tablename__ = 'parameter_set_description'
+        parameter_set_id = Column(String, primary_key=True)
+        parameter_set_name = Column(String)
+        parameter_set_description = Column(Text)
+        # This should not have parameter_id as primary key if it's not part of ParameterSet primary key.
+
+    class SolutionDescription(Base):
+        __tablename__ = 'solution_description'
+        solution_id = Column(String, primary_key=True)
+        solution_name = Column(String)
+        solution_description = Column(Text)
+        deployment_date = Column(String)
+        deprecation_date = Column(String, nullable=True)
+        maintainers = Column(Text)
+
+    # Define other models similarly
+
+    def create_tables(self):
+        self.Base.metadata.create_all(self.engine)
+
+    def drop_tables(self):
+        self.Base.metadata.drop_all(self.engine)
+
+
+    def _merge_entries(self, entries):
+        with self.Session() as session:
+            try:
+                for entry in entries:
+                    session.merge(entry)  # Merges based on primary key
+                session.commit()
+            except SQLAlchemyError as e:
+                session.rollback()
+                self.logger.error(f"SQLAlchemy Error: {e}")
+
+
+    def _as_dict(self, obj, with_relationships=False):
+        data = {c.key: getattr(obj, c.key) for c in inspect(obj).mapper.column_attrs}
+        if with_relationships:
+            for relationship in inspect(obj).mapper.relationships:
+                related_data = getattr(obj, relationship.key)
+                if related_data is not None:
+                    if isinstance(related_data, list):
+                        data[relationship.key] = [self._as_dict(child, True) for child in related_data]
+                    else:
+                        data[relationship.key] = self._as_dict(related_data, True)
+        return data
+
+    def push_tables(self,
+                      solution_description : list,
+                      solution_parameter_set : list,
+                      parameter_set : list,
+                      parameter_set_description : list,
+                      parameter_description : list,
+                      parameter_attribute : list,
+                      attribute_values : list):
+
+        """
+        Pushes tables with database handler
+        """
+
+
+        solution_description = [self.SolutionDescription(**data)
+                                for data in solution_description]
+
+        parameter_description = [self.ParameterDescription(**data)
+                                for data in parameter_description]
+
+        parameter_set_description = [self.ParameterSetDescription(**data)
+                                for data in parameter_set_description]
+
+        solution_parameter_set = [self.SolutionParameterSet(**data)
+                                for data in solution_parameter_set]
+
+        parameter_set = [self.ParameterSet(**data)
+                                for data in parameter_set]
+
+        parameter_attribute = [self.ParameterAttribute(**data)
+                                for data in parameter_attribute]
+
+        attribute_values = [self.AttributeValues(**data)
+                                for data in attribute_values]
+
+
+        inserts = solution_description + parameter_description + parameter_set +\
+             solution_parameter_set + parameter_set_description + \
+                attribute_values + parameter_attribute
+
+        self._merge_entries(entries = inserts)
+
+        return True
+
+    def pull_tables(self, solution_id=None, parameter_set_id=None):
+        if solution_id is None or parameter_set_id is None:
+            raise ValueError("Provide both solution_id and parameter_set_id!")
+
+        session = self.Session()
+        try:
+            # Fetch related entries based on solution_id and parameter_set_id
+            solution_descriptions = session.query(self.SolutionDescription).filter(
+                self.SolutionDescription.solution_id == solution_id).all()
+            solution_parameter_sets = session.query(self.SolutionParameterSet).filter(
+                self.SolutionParameterSet.solution_id == solution_id,
+                self.SolutionParameterSet.parameter_set_id == parameter_set_id).all()
+            parameter_sets = session.query(self.ParameterSet).filter(
+                self.ParameterSet.parameter_set_id == parameter_set_id).all()
+            parameter_set_descriptions = session.query(self.ParameterSetDescription).filter(
+                self.ParameterSetDescription.parameter_set_id == parameter_set_id).all()
+
+            # Fetch parameter_id from parameter_sets for further queries
+            param_ids = [param.parameter_id for param in parameter_sets]
+
+            # Continue to fetch related entries based on parameter_id
+            parameter_descriptions = session.query(self.ParameterDescription).filter(
+                self.ParameterDescription.parameter_id.in_(param_ids)).all()
+            parameter_attributes = session.query(self.ParameterAttribute).filter(
+                self.ParameterAttribute.parameter_id.in_(param_ids)).all()
+
+            # Get attribute_ids for fetching attribute values
+            attribute_ids = [attr.attribute_id for attr in parameter_attributes]
+            attribute_values = session.query(self.AttributeValues).filter(
+                self.AttributeValues.attribute_id.in_(attribute_ids)).all()
+
+            return (
+                [self._as_dict(data) for data in solution_descriptions],
+                [self._as_dict(data) for data in solution_parameter_sets],
+                [self._as_dict(data) for data in parameter_sets],
+                [self._as_dict(data) for data in parameter_set_descriptions],
+                [self._as_dict(data) for data in parameter_descriptions],
+                [self._as_dict(data) for data in parameter_attributes],
+                [self._as_dict(data) for data in attribute_values]
+            )
+
+        except Exception as e:
+            session.rollback()
+            print(f"An error occurred: {e}")
+        finally:
+            session.close()
+
 
 @attr.s
 class FileTypeHandler:
 
     """
     Handles raw files, processes them for storage
     and reconstructs when pulling from storage.
@@ -943,16 +1169,19 @@
 
     # optional
     solution_id = attr.ib(default=None, type=str)
     param_names = attr.ib(default=None, type=dict)
     param_descriptions = attr.ib(default=None, type=dict)
     seed = attr.ib(default=None, type=int)
 
+    connection_details = attr.ib(default = {
+        'base_url' : "http://localhost:8000"})
+
     # dependancies
-    database_connector = attr.ib(default=None, type=DatabaseConnector)
+    database_connector = attr.ib(default=None, type=MockerDatabaseConnector)
     file_type_handler = attr.ib(default=FileTypeHandler)
     name_generator = attr.ib(default=ComplexNameGenerator)
 
     # inner
     solutions = attr.ib(default={})
     param_sets = attr.ib(default={})
     param_attributes = attr.ib(default={})
@@ -966,15 +1195,17 @@
     logger_format = attr.ib(default=None)
 
 
     def __attrs_post_init__(self):
         self._initialize_logger()
 
         if self.database_connector is None:
-            self.database_connector = DatabaseConnector()
+            self.database_connector = MockerDatabaseConnector(connection_details = self.connection_details)
+
+
 
         self.commited_tables = {}
 
 
     def _initialize_logger(self):
 
         """
@@ -1076,15 +1307,15 @@
         self.param_sets[parameter_set_name] = {'parameter_set' : parameter_set,
                                                'parameter_set_description' : parameter_set_description}
 
 
     def add_solution_description(self,
                                     solution_name : str,
                                     deployment_date : str = None,
-                                    deprication_date : str = None,
+                                    deprecation_date : str = None,
                                     solution_description : str = None,
                                     solution_id : str = None,
                                     maintainers : list = None):
 
         """
         Add new solution and its description.
         """
@@ -1109,15 +1340,15 @@
             self.solutions[solution_name]['solution_id'] = solution_id
 
         self.solutions[solution_name]['solution_description'] = {
             'solution_id' : solution_id,
             'solution_name' : solution_name,
             'solution_description' : solution_description,
             'deployment_date' : deployment_date,
-            'deprication_date' : deprication_date,
+            'deprecation_date' : deprecation_date,
             'maintainers' : maintainers
         }
 
     def _get_solution_name_from_memory(self, solution_id : str) -> str:
 
         """
         Get solution name from memory from solution id.
@@ -1162,15 +1393,15 @@
         return parameter_set_id
 
 
     def update_solution_description(self,
                                     solution_id : str,
                                     solution_name : str = None,
                                     deployment_date : str = None,
-                                    deprication_date : str = None,
+                                    deprecation_date : str = None,
                                     solution_description : str = None,
                                     maintainers : list = None):
 
         """
         Update solution description.
         """
 
@@ -1178,16 +1409,16 @@
         solution_name = self._get_solution_name_from_memory(solution_id = solution_id)
 
         # update description parameters
         if solution_name is not None:
             self.solutions[solution_name]['solution_description']['solution_name'] = solution_name
         if deployment_date is not None:
             self.solutions[solution_name]['solution_description']['deployment_date'] = deployment_date
-        if deprication_date is not None:
-            self.solutions[solution_name]['solution_description']['deprication_date'] = deprication_date
+        if deprecation_date is not None:
+            self.solutions[solution_name]['solution_description']['deprecation_date'] = deprecation_date
         if solution_description is not None:
             self.solutions[solution_name]['solution_description']['solution_description'] = solution_description
         if maintainers is not None:
             self.solutions[solution_name]['solution_description']['maintainers'] = maintainers
 
 
     def add_parameter_set_to_solution(self,
@@ -1518,21 +1749,22 @@
             parameter_attribute,
             attribute_values) = self._prep_tables_for_pushing(
                 solution_id = solution_id,
                 parameter_set_ids = parameter_set_ids
             )
 
         self.database_connector.push_tables(
-            solution_description,
-            solution_parameter_set,
-            parameter_set,
-            parameter_set_description,
-            parameter_description,
-            parameter_attribute,
-            attribute_values
+
+            solution_description = solution_description,
+            solution_parameter_set = solution_parameter_set,
+            parameter_set = parameter_set,
+            parameter_set_description = parameter_set_description,
+            parameter_description = parameter_description,
+            parameter_attribute = parameter_attribute,
+            attribute_values = attribute_values
         )
 
         return True
 
     def _rebuild_tables_from_pulled_data(self,
                                      solution_id: str,
                                      parameter_set_ids: list,
```

### Comparing `parameterframe-0.0.2/parameterframe/setup.py` & `parameterframe-0.0.3/parameterframe/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,14 @@
       long_description = fh.read()
 else:
   long_description = ''
 
 setup(
     name="parameterframe",
     packages=["parameterframe"],
-    install_requires=['### parameterframe.py', 'attrs', 'mocker_db==0.1.1', 'pyyaml', 'dill'],
+    install_requires=['### parameterframe.py', 'mocker_db==0.1.1', 'pyyaml', 'attrs', 'dill', 'sqlalchemy'],
     classifiers=['Development Status :: 3 - Alpha', 'Intended Audience :: Developers', 'Intended Audience :: Science/Research', 'Programming Language :: Python :: 3', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11', 'License :: OSI Approved :: MIT License', 'Topic :: Scientific/Engineering'],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.", keywords="['python', 'parameter storage']", version="0.0.2"
+    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.", keywords="['python', 'parameter storage']", version="0.0.3"
 )
```

### Comparing `parameterframe-0.0.2/parameterframe.egg-info/PKG-INFO` & `parameterframe-0.0.3/parameterframe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parameterframe
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','parameter storage']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -25,15 +25,15 @@
 
 
 ```python
 import sys
 import pandas as pd
 import os
 sys.path.append('../')
-from python_modules.parameterframe import FileTypeHandler, ParameterFrame, DatabaseConnector
+from python_modules.parameterframe import FileTypeHandler, ParameterFrame, MockerDatabaseConnector, SqlAlchemyDatabaseManager
 
 ```
 
 ## Content
 
 1. Processing and reconstructing yaml and txt with FileTypeHandler
 2. Assembling parameter sets and adding to solution with ParameterFrame
@@ -42,15 +42,17 @@
 ### 1. Processing and reconstructing yaml and txt with FileTypeHandler
 
 
 ```python
 params_path = "../tests/parameterframe/example_configs"
 
 pf = ParameterFrame(
-    params_path = params_path
+    params_path = params_path,
+    database_connector = SqlAlchemyDatabaseManager(connection_details = {
+    'base_url' : 'postgresql+psycopg2://postgres:mysecretpassword@localhost:5432/mytestdb'})
 )
 
 pf.process_parameters_from_files()
 ```
 
 ### 2. Assembling parameter sets and adding to solution with ParameterFrame
 
@@ -78,15 +80,15 @@
 
 
     {'solution_id': 'ffb2fa4d1f14786e7a11641a870c3db55f08f375fb7ac00c9a2127f7cd801a60',
      'solution_description': {'solution_id': 'ffb2fa4d1f14786e7a11641a870c3db55f08f375fb7ac00c9a2127f7cd801a60',
       'solution_name': 'example_solution',
       'solution_description': 'example solution for test',
       'deployment_date': None,
-      'deprication_date': None,
+      'deprecation_date': None,
       'maintainers': None}}
 
 
 
 
 ```python
 pf.add_parameter_set_to_solution(solution_name="example_solution",
@@ -127,15 +129,15 @@
   </thead>
   <tbody>
     <tr>
       <th>0</th>
       <td>ffb2fa4d1f14786e7a11641a870c3db55f08f375fb7ac0...</td>
       <td>a54f04d2ff154294309403206e059aec556cdcfa511206...</td>
       <td>STAGING</td>
-      <td>2024-04-21 23:18:22</td>
+      <td>2024-05-02 18:36:32</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
@@ -175,15 +177,15 @@
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>solution_id</th>
       <th>solution_name</th>
       <th>solution_description</th>
       <th>deployment_date</th>
-      <th>deprication_date</th>
+      <th>deprecation_date</th>
       <th>maintainers</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <th>0</th>
       <td>ffb2fa4d1f14786e7a11641a870c3db55f08f375fb7ac0...</td>
@@ -237,15 +239,15 @@
   </thead>
   <tbody>
     <tr>
       <th>0</th>
       <td>ffb2fa4d1f14786e7a11641a870c3db55f08f375fb7ac0...</td>
       <td>a54f04d2ff154294309403206e059aec556cdcfa511206...</td>
       <td>STAGING</td>
-      <td>2024-04-21 23:18:22</td>
+      <td>2024-05-02 18:36:32</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
@@ -1061,54 +1063,48 @@
 
 
 ```python
 pf.push_solution(solution_id='ffb2fa4d1f14786e7a11641a870c3db55f08f375fb7ac00c9a2127f7cd801a60',
                  parameter_set_ids=['a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5'])
 ```
 
-    HTTP Request: POST http://localhost:8000/insert "HTTP/1.1 200 OK"
-
-
 
 
 
     True
 
 
 
 ### 5. Pulling solution with DatabaseConnector
 
 
 ```python
 params_path = "../tests/parameterframe/example_configs"
 
 pf2 = ParameterFrame(
-    params_path = params_path
+    params_path = params_path,
+    database_connector = SqlAlchemyDatabaseManager(connection_details = {
+    'base_url' : 'postgresql+psycopg2://postgres:mysecretpassword@localhost:5432/mytestdb'})
 )
 
 pf2.pull_solution(solution_id='ffb2fa4d1f14786e7a11641a870c3db55f08f375fb7ac00c9a2127f7cd801a60',
                  parameter_set_id='a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5')
 ```
 
-    HTTP Request: POST http://localhost:8000/search "HTTP/1.1 200 OK"
-    HTTP Request: POST http://localhost:8000/search "HTTP/1.1 200 OK"
-    HTTP Request: POST http://localhost:8000/search "HTTP/1.1 200 OK"
-
-
 ### 6. Reconstructing files
 
 
 ```python
 os.listdir("../tests/parameterframe/reconstructed_files")
 ```
 
 
 
 
-    ['.gitignore']
+    []
 
 
 
 
 ```python
 pf2.reconstruct_parameter_set(
     solution_name = "example_solution",
@@ -1123,13 +1119,12 @@
 ```
 
 
 
 
     ['param_2.yaml',
      'param_11.dill',
-     '.gitignore',
      'param_1.yaml',
      'param_10.txt',
      'param_21.ipynb']
```


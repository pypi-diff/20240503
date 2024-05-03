# Comparing `tmp/cdklabs.aws_data_solutions_framework-1.6.0.tar.gz` & `tmp/cdklabs.aws_data_solutions_framework-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.aws_data_solutions_framework-1.6.0.tar", last modified: Mon Apr 29 17:40:15 2024, max compression
+gzip compressed data, was "cdklabs.aws_data_solutions_framework-1.7.0.tar", last modified: Fri May  3 16:49:18 2024, max compression
```

## Comparing `cdklabs.aws_data_solutions_framework-1.6.0.tar` & `cdklabs.aws_data_solutions_framework-1.7.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.666992 cdklabs.aws_data_solutions_framework-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-29 17:40:15.666992 cdklabs.aws_data_solutions_framework-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 17:40:15.666992 cdklabs.aws_data_solutions_framework-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.658992 cdklabs.aws_data_solutions_framework-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.658992 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.658992 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.662992 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  3947535 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/_jsii/aws-data-solutions-framework@1.6.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.666992 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/consumption/
--rw-r--r--   0 runner    (1001) docker     (127)   249288 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/consumption/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.666992 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/governance/
--rw-r--r--   0 runner    (1001) docker     (127)    45726 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/governance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.666992 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/processing/
--rw-r--r--   0 runner    (1001) docker     (127)   259729 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.666992 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/storage/
--rw-r--r--   0 runner    (1001) docker     (127)    86274 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.666992 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)    93221 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/streaming/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.666992 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    97649 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.658992 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs.aws_data_solutions_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-29 17:40:15.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs.aws_data_solutions_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-29 17:40:15.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs.aws_data_solutions_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:40:15.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs.aws_data_solutions_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-29 17:40:15.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs.aws_data_solutions_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 17:40:15.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs.aws_data_solutions_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.480687 cdklabs.aws_data_solutions_framework-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-03 16:49:18.480687 cdklabs.aws_data_solutions_framework-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:49:18.480687 cdklabs.aws_data_solutions_framework-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.472687 cdklabs.aws_data_solutions_framework-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.472687 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.476687 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.476687 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  3976219 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/_jsii/aws-data-solutions-framework@1.7.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.480687 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/consumption/
+-rw-r--r--   0 runner    (1001) docker     (127)   263926 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/consumption/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.480687 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/governance/
+-rw-r--r--   0 runner    (1001) docker     (127)    45726 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/governance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.480687 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)   259729 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.480687 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)    86274 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.480687 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)    93221 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/streaming/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.480687 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    97649 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.472687 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs.aws_data_solutions_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-03 16:49:18.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs.aws_data_solutions_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-03 16:49:18.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs.aws_data_solutions_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:49:18.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs.aws_data_solutions_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 16:49:18.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs.aws_data_solutions_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 16:49:18.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs.aws_data_solutions_framework.egg-info/top_level.txt
```

### Comparing `cdklabs.aws_data_solutions_framework-1.6.0/LICENSE` & `cdklabs.aws_data_solutions_framework-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.aws_data_solutions_framework-1.6.0/PKG-INFO` & `cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs.aws_data_solutions_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cdklabs.aws_data_solutions_framework
-Version: 1.6.0
+Name: cdklabs.aws-data-solutions-framework
+Version: 1.7.0
 Summary: L3 CDK Constructs used to build data solutions with AWS
 Home-page: https://awslabs.github.io/data-solutions-framework-on-aws/
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/data-solutions-framework-on-aws.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.aws_data_solutions_framework-1.6.0/setup.py` & `cdklabs.aws_data_solutions_framework-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.aws_data_solutions_framework",
-    "version": "1.6.0",
+    "version": "1.7.0",
     "description": "L3 CDK Constructs used to build data solutions with AWS",
     "license": "Apache-2.0",
     "url": "https://awslabs.github.io/data-solutions-framework-on-aws/",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -28,15 +28,15 @@
         "cdklabs.aws_data_solutions_framework.processing",
         "cdklabs.aws_data_solutions_framework.storage",
         "cdklabs.aws_data_solutions_framework.streaming",
         "cdklabs.aws_data_solutions_framework.utils"
     ],
     "package_data": {
         "cdklabs.aws_data_solutions_framework._jsii": [
-            "aws-data-solutions-framework@1.6.0.jsii.tgz"
+            "aws-data-solutions-framework@1.7.0.jsii.tgz"
         ],
         "cdklabs.aws_data_solutions_framework": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/__init__.py` & `cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/_jsii/__init__.py` & `cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import aws_cdk.lambda_layer_kubectl_v27._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@cdklabs/aws-data-solutions-framework",
-    "1.6.0",
+    "1.7.0",
     __name__[0:-6],
-    "aws-data-solutions-framework@1.6.0.jsii.tgz",
+    "aws-data-solutions-framework@1.7.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/consumption/__init__.py` & `cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/consumption/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,40 +100,37 @@
 
 ```python
 workgroup = dsf.consumption.RedshiftServerlessWorkgroup(self, "DefaultRedshiftServerlessWorkgroup",
     name="default",
     namespace=namespace
 )
 
-# Initialize the Redshift Data API
-data_access = workgroup.access_data("DataApi", True)
-
 # Run a custom SQL to create a customer table
-create_table = data_access.run_custom_sQL("CreateCustomerTable", "defaultdb", """
+create_table = workgroup.run_custom_sQL("CreateCustomerTable", "defaultdb", """
           CREATE TABLE customer(
             customer_id varchar(50),
             salutation varchar(5),
             first_name varchar(50),
             last_name varchar(50),
             email_address varchar(100)
           )
           diststyle even
           """, "drop table customer")
 
 # Run a COPY command to load data into the customer table
-ingestion = data_access.ingest_data("ExampleCopy", "defaultdb", "customer", bucket, "data-products/customer/", "csv ignoreheader 1")
+ingestion = workgroup.ingest_data("ExampleCopy", "defaultdb", "customer", bucket, "data-products/customer/", "csv ignoreheader 1")
 
 # Add dependencies between Redshift Data API commands because CDK cannot infer them
 ingestion.node.add_dependency(create_table)
 
 # Create an engineering role in the defaultdb
-db_role = data_access.create_db_role("EngineeringRole", "defaultdb", "engineering")
+db_role = workgroup.create_db_role("EngineeringRole", "defaultdb", "engineering")
 
 # Grant the engineering role full access to the public schema in the defaultdb
-db_schema = data_access.grant_db_schema_to_role("EngineeringGrant", "defaultdb", "public", "engineering")
+db_schema = workgroup.grant_db_schema_to_role("EngineeringGrant", "defaultdb", "public", "engineering")
 
 # Enforce dependencies
 db_schema.node.add_dependency(db_role)
 ```
 
 ## Cataloging Redshift Serverless Tables
 
@@ -200,16 +197,15 @@
         consumer_workgroup = RedshiftServerlessWorkgroup(self, "ConsumerRSWorkgroup",
             name="consumer-workgroup",
             namespace=consumer_namespace
         )
 
         share_name = "testshare"
 
-        producer_data_access = producer_workgroup.access_data("ProducerDataAccess")
-        create_customers_table = producer_data_access.run_custom_sQL("CreateCustomerTable", db_name, "create table public.customers (id varchar(100) not null, first_name varchar(50) not null, last_name varchar(50) not null, email varchar(100) not null)", "drop table public.customers")
+        create_customers_table = producer_workgroup.run_custom_sQL("CreateCustomerTable", db_name, "create table public.customers (id varchar(100) not null, first_name varchar(50) not null, last_name varchar(50) not null, email varchar(100) not null)", "drop table public.customers")
 
         new_share = producer_workgroup.create_share("producer-share", db_name, share_name, "public", ["public.customers"])
         new_share.new_share_custom_resource.node.add_dependency(create_customers_table)
 
         grant_to_consumer = producer_workgroup.grant_access_to_share("GrantToConsumer", new_share, consumer_namespace.namespace_id)
 
         grant_to_consumer.resource.node.add_dependency(new_share)
@@ -237,16 +233,15 @@
         producer_workgroup = RedshiftServerlessWorkgroup(self, "ProducerRSWorkgroup",
             name="producer-workgroup",
             namespace=producer_namespace
         )
 
         share_name = "testshare"
 
-        producer_data_access = producer_workgroup.access_data("ProducerDataAccess")
-        create_customers_table = producer_data_access.run_custom_sQL("CreateCustomerTable", db_name, "create table public.customers (id varchar(100) not null, first_name varchar(50) not null, last_name varchar(50) not null, email varchar(100) not null)", "drop table public.customers")
+        create_customers_table = producer_workgroup.run_custom_sQL("CreateCustomerTable", db_name, "create table public.customers (id varchar(100) not null, first_name varchar(50) not null, last_name varchar(50) not null, email varchar(100) not null)", "drop table public.customers")
 
         new_share = producer_workgroup.create_share("producer-share", db_name, share_name, "public", ["public.customers"])
         new_share.new_share_custom_resource.node.add_dependency(create_customers_table)
 
         grant_to_consumer = producer_workgroup.grant_access_to_share("GrantToConsumer", new_share, undefined, "<CONSUMER-ACCOUNT-ID>", True)
 
         grant_to_consumer.resource.node.add_dependency(new_share)
@@ -3846,29 +3841,50 @@
     @jsii.member(jsii_name="accessData")
     def access_data(
         self,
         id: builtins.str,
         create_vpc_endpoint: typing.Optional[builtins.bool] = None,
         existing_interface_vpc_endpoint: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IInterfaceVpcEndpoint] = None,
     ) -> RedshiftData:
-        '''Creates an instance of ``RedshiftData`` to send custom SQLs to the workgroup.
+        '''(deprecated) Creates an instance of ``RedshiftData`` to send custom SQLs to the workgroup.
 
         :param id: The CDK ID of the resource.
         :param create_vpc_endpoint: if set to true, create interface VPC endpoint for Redshift Data API.
         :param existing_interface_vpc_endpoint: if ``createVpcEndpoint`` is false, and if this is populated, then the Lambda function's security group would be added in the existing VPC endpoint's security group.
 
         :return: ``RedshiftData``
+
+        :deprecated: Use the convenience methods directly from the ``RedshiftServerlessWorkgroup`` construct.
+
+        :stability: deprecated
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__656d5ccac3be5498f4c9424d9535dc359e8d9f55ffcaf649ad7cfc1b2de647d4)
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument create_vpc_endpoint", value=create_vpc_endpoint, expected_type=type_hints["create_vpc_endpoint"])
             check_type(argname="argument existing_interface_vpc_endpoint", value=existing_interface_vpc_endpoint, expected_type=type_hints["existing_interface_vpc_endpoint"])
         return typing.cast(RedshiftData, jsii.invoke(self, "accessData", [id, create_vpc_endpoint, existing_interface_vpc_endpoint]))
 
+    @jsii.member(jsii_name="assignDbRolesToIAMRole")
+    def assign_db_roles_to_iam_role(
+        self,
+        db_roles: typing.Sequence[builtins.str],
+        target_role: _aws_cdk_aws_iam_ceddda9d.IRole,
+    ) -> None:
+        '''Assigns Redshift DB roles to IAM role vs the ``RedshiftDbRoles`` tag.
+
+        :param db_roles: List of Redshift DB roles to assign to IAM role.
+        :param target_role: The IAM role to assign the Redshift DB roles to.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__274a1c47474a72a173b6aa1ea8f194624cfca935b741372a44d5145e2c0268e2)
+            check_type(argname="argument db_roles", value=db_roles, expected_type=type_hints["db_roles"])
+            check_type(argname="argument target_role", value=target_role, expected_type=type_hints["target_role"])
+        return typing.cast(None, jsii.invoke(self, "assignDbRolesToIAMRole", [db_roles, target_role]))
+
     @jsii.member(jsii_name="catalogTables")
     def catalog_tables(
         self,
         id: builtins.str,
         catalog_db_name: builtins.str,
         path_to_crawl: typing.Optional[builtins.str] = None,
     ) -> _DataCatalogDatabase_925dcbbb:
@@ -3916,14 +3932,36 @@
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument new_database_name", value=new_database_name, expected_type=type_hints["new_database_name"])
             check_type(argname="argument producer_data_share_name", value=producer_data_share_name, expected_type=type_hints["producer_data_share_name"])
             check_type(argname="argument producer_namespace_id", value=producer_namespace_id, expected_type=type_hints["producer_namespace_id"])
             check_type(argname="argument producer_account_id", value=producer_account_id, expected_type=type_hints["producer_account_id"])
         return typing.cast(RedshiftDataSharingCreateDbFromShareProps, jsii.invoke(self, "createDatabaseFromShare", [id, new_database_name, producer_data_share_name, producer_namespace_id, producer_account_id]))
 
+    @jsii.member(jsii_name="createDbRole")
+    def create_db_role(
+        self,
+        id: builtins.str,
+        database_name: builtins.str,
+        role_name: builtins.str,
+    ) -> _aws_cdk_ceddda9d.CustomResource:
+        '''Creates a new DB role.
+
+        :param id: The CDK Construct ID.
+        :param database_name: The name of the database to run this command.
+        :param role_name: The name of the role to create.
+
+        :return: ``CustomResource``
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ffd90f090e5decf054755d4d34db25c9506e74ac2990171d30d286da23fbde0a)
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument database_name", value=database_name, expected_type=type_hints["database_name"])
+            check_type(argname="argument role_name", value=role_name, expected_type=type_hints["role_name"])
+        return typing.cast(_aws_cdk_ceddda9d.CustomResource, jsii.invoke(self, "createDbRole", [id, database_name, role_name]))
+
     @jsii.member(jsii_name="createShare")
     def create_share(
         self,
         id: builtins.str,
         database_name: builtins.str,
         data_share_name: builtins.str,
         schema: builtins.str,
@@ -3974,19 +4012,186 @@
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument data_share_details", value=data_share_details, expected_type=type_hints["data_share_details"])
             check_type(argname="argument consumer_namespace_id", value=consumer_namespace_id, expected_type=type_hints["consumer_namespace_id"])
             check_type(argname="argument consumer_account_id", value=consumer_account_id, expected_type=type_hints["consumer_account_id"])
             check_type(argname="argument auto_authorized", value=auto_authorized, expected_type=type_hints["auto_authorized"])
         return typing.cast(RedshiftDataSharingGrantedProps, jsii.invoke(self, "grantAccessToShare", [id, data_share_details, consumer_namespace_id, consumer_account_id, auto_authorized]))
 
+    @jsii.member(jsii_name="grantDbAllPrivilegesToRole")
+    def grant_db_all_privileges_to_role(
+        self,
+        id: builtins.str,
+        database_name: builtins.str,
+        schema: builtins.str,
+        role_name: builtins.str,
+    ) -> _aws_cdk_ceddda9d.CustomResource:
+        '''Grants both read and write permissions on all the tables in the ``schema`` to the DB role.
+
+        :param id: The CDK Construct ID.
+        :param database_name: The name of the database to run this command.
+        :param schema: The schema where the tables are located in.
+        :param role_name: The DB role to grant the permissions to.
+
+        :return: ``CustomResource``
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__44c0a0a30c1e3e0f45aac36fa07c8a0b1426550b5f557e03fe782092f459620f)
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument database_name", value=database_name, expected_type=type_hints["database_name"])
+            check_type(argname="argument schema", value=schema, expected_type=type_hints["schema"])
+            check_type(argname="argument role_name", value=role_name, expected_type=type_hints["role_name"])
+        return typing.cast(_aws_cdk_ceddda9d.CustomResource, jsii.invoke(self, "grantDbAllPrivilegesToRole", [id, database_name, schema, role_name]))
+
+    @jsii.member(jsii_name="grantDbSchemaToRole")
+    def grant_db_schema_to_role(
+        self,
+        id: builtins.str,
+        database_name: builtins.str,
+        schema: builtins.str,
+        role_name: builtins.str,
+    ) -> _aws_cdk_ceddda9d.CustomResource:
+        '''Grants access to the schema to the DB role.
+
+        :param id: The CDK Construct ID.
+        :param database_name: The name of the database to run this command.
+        :param schema: The schema where the tables are located in.
+        :param role_name: The DB role to grant the permissions to.
+
+        :return: ``CustomResource``
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__5f71eb71eb7f7dd7216af3dc20d9b6906e806742b531d956dd6bd1bd9949e625)
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument database_name", value=database_name, expected_type=type_hints["database_name"])
+            check_type(argname="argument schema", value=schema, expected_type=type_hints["schema"])
+            check_type(argname="argument role_name", value=role_name, expected_type=type_hints["role_name"])
+        return typing.cast(_aws_cdk_ceddda9d.CustomResource, jsii.invoke(self, "grantDbSchemaToRole", [id, database_name, schema, role_name]))
+
+    @jsii.member(jsii_name="grantSchemaReadToRole")
+    def grant_schema_read_to_role(
+        self,
+        id: builtins.str,
+        database_name: builtins.str,
+        schema: builtins.str,
+        role_name: builtins.str,
+    ) -> _aws_cdk_ceddda9d.CustomResource:
+        '''Grants read permission on all the tables in the ``schema`` to the DB role.
+
+        :param id: -
+        :param database_name: The name of the database to run this command.
+        :param schema: The schema where the tables are located in.
+        :param role_name: The DB role to grant the permissions to.
+
+        :return: ``CustomResource``
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__1b6639981684a4360e50ba57963d7af9f370fc6b052cec18de467dfc77599d8d)
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument database_name", value=database_name, expected_type=type_hints["database_name"])
+            check_type(argname="argument schema", value=schema, expected_type=type_hints["schema"])
+            check_type(argname="argument role_name", value=role_name, expected_type=type_hints["role_name"])
+        return typing.cast(_aws_cdk_ceddda9d.CustomResource, jsii.invoke(self, "grantSchemaReadToRole", [id, database_name, schema, role_name]))
+
+    @jsii.member(jsii_name="ingestData")
+    def ingest_data(
+        self,
+        id: builtins.str,
+        database_name: builtins.str,
+        target_table: builtins.str,
+        source_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+        source_prefix: builtins.str,
+        ingest_additional_options: typing.Optional[builtins.str] = None,
+        role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+    ) -> _aws_cdk_ceddda9d.CustomResource:
+        '''Ingest data from S3 into a Redshift table.
+
+        :param id: The CDK Construct ID.
+        :param database_name: The name of the database to run this command.
+        :param target_table: The target table to load the data into.
+        :param source_bucket: The bucket where the source data would be coming from.
+        :param source_prefix: The location inside the bucket where the data would be ingested from.
+        :param ingest_additional_options: Optional. Additional options to pass to the ``COPY`` command. For example, ``delimiter '|'`` or ``ignoreheader 1``
+        :param role: Optional. The IAM Role to use to access the data in S3. If not provided, it would use the default IAM role configured in the Redshift Namespace
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__0c51af318125fc00003c4631af5211b0ca4110e65b4dd14747f1bb0cd6497a0a)
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument database_name", value=database_name, expected_type=type_hints["database_name"])
+            check_type(argname="argument target_table", value=target_table, expected_type=type_hints["target_table"])
+            check_type(argname="argument source_bucket", value=source_bucket, expected_type=type_hints["source_bucket"])
+            check_type(argname="argument source_prefix", value=source_prefix, expected_type=type_hints["source_prefix"])
+            check_type(argname="argument ingest_additional_options", value=ingest_additional_options, expected_type=type_hints["ingest_additional_options"])
+            check_type(argname="argument role", value=role, expected_type=type_hints["role"])
+        return typing.cast(_aws_cdk_ceddda9d.CustomResource, jsii.invoke(self, "ingestData", [id, database_name, target_table, source_bucket, source_prefix, ingest_additional_options, role]))
+
+    @jsii.member(jsii_name="mergeToTargetTable")
+    def merge_to_target_table(
+        self,
+        id: builtins.str,
+        database_name: builtins.str,
+        source_table: builtins.str,
+        target_table: builtins.str,
+        source_column_id: typing.Optional[builtins.str] = None,
+        target_column_id: typing.Optional[builtins.str] = None,
+    ) -> _aws_cdk_ceddda9d.CustomResource:
+        '''Run the ``MERGE`` query using simplified mode.
+
+        This command would do an upsert into the target table.
+
+        :param id: The CDK Construct ID.
+        :param database_name: The name of the database to run this command.
+        :param source_table: The source table name. Schema can also be included using the following format: ``schemaName.tableName``
+        :param target_table: The target table name. Schema can also be included using the following format: ``schemaName.tableName``
+        :param source_column_id: The column in the source table that's used to determine whether the rows in the ``sourceTable`` can be matched with rows in the ``targetTable``. Default is ``id``
+        :param target_column_id: The column in the target table that's used to determine whether the rows in the ``sourceTable`` can be matched with rows in the ``targetTable``. Default is ``id``
+
+        :return: ``CustomResource``
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__fa028c96754f9f984481434a31ccaaec5289a009cc31f17849f3eac21feb9704)
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument database_name", value=database_name, expected_type=type_hints["database_name"])
+            check_type(argname="argument source_table", value=source_table, expected_type=type_hints["source_table"])
+            check_type(argname="argument target_table", value=target_table, expected_type=type_hints["target_table"])
+            check_type(argname="argument source_column_id", value=source_column_id, expected_type=type_hints["source_column_id"])
+            check_type(argname="argument target_column_id", value=target_column_id, expected_type=type_hints["target_column_id"])
+        return typing.cast(_aws_cdk_ceddda9d.CustomResource, jsii.invoke(self, "mergeToTargetTable", [id, database_name, source_table, target_table, source_column_id, target_column_id]))
+
     @jsii.member(jsii_name="retrieveVersion")
     def retrieve_version(self) -> typing.Any:
         '''Retrieve DSF package.json version.'''
         return typing.cast(typing.Any, jsii.invoke(self, "retrieveVersion", []))
 
+    @jsii.member(jsii_name="runCustomSQL")
+    def run_custom_sql(
+        self,
+        id: builtins.str,
+        database_name: builtins.str,
+        sql: builtins.str,
+        delete_sql: typing.Optional[builtins.str] = None,
+    ) -> _aws_cdk_ceddda9d.CustomResource:
+        '''Runs a custom SQL.
+
+        Once the custom resource finishes execution, the attribute ``Data`` contains an attribute ``execId`` which contains the Redshift Data API execution ID. You can then use this to retrieve execution results via the ``GetStatementResult`` API.
+
+        :param id: The CDK Construct ID.
+        :param database_name: The name of the database to run this command.
+        :param sql: The sql to run.
+        :param delete_sql: Optional. The sql to run when this resource gets deleted
+
+        :return: ``CustomResource``
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__f7039acbf64106fcfc7e263695ba5592494b32eeef7b9afbda78e216ec8bf630)
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument database_name", value=database_name, expected_type=type_hints["database_name"])
+            check_type(argname="argument sql", value=sql, expected_type=type_hints["sql"])
+            check_type(argname="argument delete_sql", value=delete_sql, expected_type=type_hints["delete_sql"])
+        return typing.cast(_aws_cdk_ceddda9d.CustomResource, jsii.invoke(self, "runCustomSQL", [id, database_name, sql, delete_sql]))
+
     @jsii.python.classproperty
     @jsii.member(jsii_name="DSF_OWNED_TAG")
     def DSF_OWNED_TAG(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "DSF_OWNED_TAG"))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="DSF_TRACKING_CODE")
@@ -4706,14 +4911,21 @@
     id: builtins.str,
     create_vpc_endpoint: typing.Optional[builtins.bool] = None,
     existing_interface_vpc_endpoint: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IInterfaceVpcEndpoint] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__274a1c47474a72a173b6aa1ea8f194624cfca935b741372a44d5145e2c0268e2(
+    db_roles: typing.Sequence[builtins.str],
+    target_role: _aws_cdk_aws_iam_ceddda9d.IRole,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__1732f80b1debc82beaf28365ccb5311f0a9de55e9b841b2a6932b124a8b0b979(
     id: builtins.str,
     catalog_db_name: builtins.str,
     path_to_crawl: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
@@ -4724,14 +4936,22 @@
     producer_data_share_name: builtins.str,
     producer_namespace_id: typing.Optional[builtins.str] = None,
     producer_account_id: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__ffd90f090e5decf054755d4d34db25c9506e74ac2990171d30d286da23fbde0a(
+    id: builtins.str,
+    database_name: builtins.str,
+    role_name: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__bb7d745f44f06dc1511932c5b2a7566dc46ab9fe97deaf5bdb0768eef6f679ef(
     id: builtins.str,
     database_name: builtins.str,
     data_share_name: builtins.str,
     schema: builtins.str,
     tables: typing.Sequence[builtins.str],
 ) -> None:
@@ -4744,14 +4964,73 @@
     consumer_namespace_id: typing.Optional[builtins.str] = None,
     consumer_account_id: typing.Optional[builtins.str] = None,
     auto_authorized: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__44c0a0a30c1e3e0f45aac36fa07c8a0b1426550b5f557e03fe782092f459620f(
+    id: builtins.str,
+    database_name: builtins.str,
+    schema: builtins.str,
+    role_name: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__5f71eb71eb7f7dd7216af3dc20d9b6906e806742b531d956dd6bd1bd9949e625(
+    id: builtins.str,
+    database_name: builtins.str,
+    schema: builtins.str,
+    role_name: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__1b6639981684a4360e50ba57963d7af9f370fc6b052cec18de467dfc77599d8d(
+    id: builtins.str,
+    database_name: builtins.str,
+    schema: builtins.str,
+    role_name: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__0c51af318125fc00003c4631af5211b0ca4110e65b4dd14747f1bb0cd6497a0a(
+    id: builtins.str,
+    database_name: builtins.str,
+    target_table: builtins.str,
+    source_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+    source_prefix: builtins.str,
+    ingest_additional_options: typing.Optional[builtins.str] = None,
+    role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__fa028c96754f9f984481434a31ccaaec5289a009cc31f17849f3eac21feb9704(
+    id: builtins.str,
+    database_name: builtins.str,
+    source_table: builtins.str,
+    target_table: builtins.str,
+    source_column_id: typing.Optional[builtins.str] = None,
+    target_column_id: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__f7039acbf64106fcfc7e263695ba5592494b32eeef7b9afbda78e216ec8bf630(
+    id: builtins.str,
+    database_name: builtins.str,
+    sql: builtins.str,
+    delete_sql: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__83581aad2a8ffe9885f335ae9f8efd43c1cb14783aad8eb61311a8a99788bd1f(
     *,
     name: builtins.str,
     namespace: RedshiftServerlessNamespace,
     base_capacity: typing.Optional[jsii.Number] = None,
     extra_security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.SecurityGroup]] = None,
     port: typing.Optional[jsii.Number] = None,
```

### Comparing `cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/governance/__init__.py` & `cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/governance/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/processing/__init__.py` & `cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/storage/__init__.py` & `cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/streaming/__init__.py` & `cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/utils/__init__.py` & `cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs.aws_data_solutions_framework.egg-info/PKG-INFO` & `cdklabs.aws_data_solutions_framework-1.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cdklabs.aws-data-solutions-framework
-Version: 1.6.0
+Name: cdklabs.aws_data_solutions_framework
+Version: 1.7.0
 Summary: L3 CDK Constructs used to build data solutions with AWS
 Home-page: https://awslabs.github.io/data-solutions-framework-on-aws/
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/data-solutions-framework-on-aws.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs.aws_data_solutions_framework.egg-info/SOURCES.txt` & `cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs.aws_data_solutions_framework.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 src/cdklabs.aws_data_solutions_framework.egg-info/SOURCES.txt
 src/cdklabs.aws_data_solutions_framework.egg-info/dependency_links.txt
 src/cdklabs.aws_data_solutions_framework.egg-info/requires.txt
 src/cdklabs.aws_data_solutions_framework.egg-info/top_level.txt
 src/cdklabs/aws_data_solutions_framework/__init__.py
 src/cdklabs/aws_data_solutions_framework/py.typed
 src/cdklabs/aws_data_solutions_framework/_jsii/__init__.py
-src/cdklabs/aws_data_solutions_framework/_jsii/aws-data-solutions-framework@1.6.0.jsii.tgz
+src/cdklabs/aws_data_solutions_framework/_jsii/aws-data-solutions-framework@1.7.0.jsii.tgz
 src/cdklabs/aws_data_solutions_framework/consumption/__init__.py
 src/cdklabs/aws_data_solutions_framework/governance/__init__.py
 src/cdklabs/aws_data_solutions_framework/processing/__init__.py
 src/cdklabs/aws_data_solutions_framework/storage/__init__.py
 src/cdklabs/aws_data_solutions_framework/streaming/__init__.py
 src/cdklabs/aws_data_solutions_framework/utils/__init__.py
```


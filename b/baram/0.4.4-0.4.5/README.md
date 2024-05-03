# Comparing `tmp/baram-0.4.4.tar.gz` & `tmp/baram-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baram-0.4.4.tar", max compression
+gzip compressed data, was "baram-0.4.5.tar", max compression
```

## Comparing `baram-0.4.4.tar` & `baram-0.4.5.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0      660 2023-08-14 00:49:22.722376 baram-0.4.4/baram/airflow_manager.py
--rw-r--r--   0        0        0     1161 2022-05-31 00:21:03.987264 baram-0.4.4/baram/async_crawler.py
--rw-r--r--   0        0        0      644 2023-02-13 00:11:32.025035 baram-0.4.4/baram/conf_manager.py
--rw-r--r--   0        0        0    14117 2023-08-07 01:33:48.528999 baram-0.4.4/baram/ec2_manager.py
--rw-r--r--   0        0        0      773 2022-05-24 00:56:46.354660 baram-0.4.4/baram/ecr_manager.py
--rw-r--r--   0        0        0     2385 2023-03-15 07:55:06.640970 baram-0.4.4/baram/efs_manager.py
--rw-r--r--   0        0        0     8439 2024-02-27 06:29:18.350049 baram-0.4.4/baram/glue_manager.py
--rw-r--r--   0        0        0     3525 2024-01-19 07:14:47.762432 baram-0.4.4/baram/iam_manager.py
--rw-r--r--   0        0        0     1098 2022-05-04 05:35:56.208476 baram-0.4.4/baram/kms_manager.py
--rw-r--r--   0        0        0     2064 2022-05-06 01:06:54.382347 baram-0.4.4/baram/lambda_manager.py
--rw-r--r--   0        0        0      477 2022-05-06 01:06:54.382534 baram-0.4.4/baram/log_manager.py
--rw-r--r--   0        0        0      605 2022-05-04 05:35:56.213543 baram-0.4.4/baram/poetry_manager.py
--rw-r--r--   0        0        0      560 2022-05-04 05:23:44.845922 baram-0.4.4/baram/process_manager.py
--rw-r--r--   0        0        0      679 2023-02-13 00:11:32.025599 baram-0.4.4/baram/requests_manager.py
--rw-r--r--   0        0        0    10266 2024-01-19 07:15:36.000000 baram-0.4.4/baram/s3_manager.py
--rw-r--r--   0        0        0    12557 2024-03-22 06:24:08.547056 baram-0.4.4/baram/sagemaker_manager.py
--rw-r--r--   0        0        0      552 2024-03-22 06:24:11.075326 baram-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      224 2022-05-03 23:39:58.553478 baram-0.4.4/readme.md
--rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 baram-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      660 2023-08-14 00:49:22.722376 baram-0.4.5/baram/airflow_manager.py
+-rw-r--r--   0        0        0     1161 2022-05-31 00:21:03.987264 baram-0.4.5/baram/async_crawler.py
+-rw-r--r--   0        0        0     8669 2024-05-03 04:01:34.273726 baram-0.4.5/baram/athena_manager.py
+-rw-r--r--   0        0        0      644 2023-02-13 00:11:32.025035 baram-0.4.5/baram/conf_manager.py
+-rw-r--r--   0        0        0    14117 2024-05-03 04:01:29.979992 baram-0.4.5/baram/ec2_manager.py
+-rw-r--r--   0        0        0     1263 2024-05-03 04:01:34.274110 baram-0.4.5/baram/ecr_manager.py
+-rw-r--r--   0        0        0     2385 2024-05-02 05:14:52.449770 baram-0.4.5/baram/efs_manager.py
+-rw-r--r--   0        0        0    16478 2024-05-03 04:01:34.274572 baram-0.4.5/baram/glue_manager.py
+-rw-r--r--   0        0        0     3525 2024-01-19 07:14:47.762432 baram-0.4.5/baram/iam_manager.py
+-rw-r--r--   0        0        0     1098 2022-05-04 05:35:56.208476 baram-0.4.5/baram/kms_manager.py
+-rw-r--r--   0        0        0     2064 2022-05-06 01:06:54.382347 baram-0.4.5/baram/lambda_manager.py
+-rw-r--r--   0        0        0      477 2022-05-06 01:06:54.382534 baram-0.4.5/baram/log_manager.py
+-rw-r--r--   0        0        0      605 2022-05-04 05:35:56.213543 baram-0.4.5/baram/poetry_manager.py
+-rw-r--r--   0        0        0      560 2022-05-04 05:23:44.845922 baram-0.4.5/baram/process_manager.py
+-rw-r--r--   0        0        0     8684 2024-05-03 04:01:34.275062 baram-0.4.5/baram/quicksight_manager.py
+-rw-r--r--   0        0        0      679 2023-02-13 00:11:32.025599 baram-0.4.5/baram/requests_manager.py
+-rw-r--r--   0        0        0    12852 2024-05-03 04:01:34.275540 baram-0.4.5/baram/s3_manager.py
+-rw-r--r--   0        0        0    16688 2024-05-03 04:01:34.275853 baram-0.4.5/baram/sagemaker_manager.py
+-rw-r--r--   0        0        0      585 2024-05-03 04:01:34.277207 baram-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1674 2024-05-03 04:01:34.277552 baram-0.4.5/readme.md
+-rw-r--r--   0        0        0     2513 1970-01-01 00:00:00.000000 baram-0.4.5/PKG-INFO
```

### Comparing `baram-0.4.4/baram/airflow_manager.py` & `baram-0.4.5/baram/airflow_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.4.4/baram/async_crawler.py` & `baram-0.4.5/baram/async_crawler.py`

 * *Files identical despite different names*

### Comparing `baram-0.4.4/baram/conf_manager.py` & `baram-0.4.5/baram/conf_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.4.4/baram/ec2_manager.py` & `baram-0.4.5/baram/ec2_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.4.4/baram/ecr_manager.py` & `baram-0.4.5/baram/ecr_manager.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 import boto3
 
 
 class ECRManager(object):
     def __init__(self):
         self.cli = boto3.client('ecr')
 
-    def describe_images(self, name: str, max_result: int = 100):
+    def describe_repositories(self,
+                              max_results=100,
+                              **kwargs):
+        response = self.cli.describe_repositories(maxResults=max_results,
+                                                  **kwargs)
+        return response
+
+    def describe_images(self,
+                        repo_name: str,
+                        max_results: int = 100,
+                        **kwargs):
         '''
 
-        :param name: repo name
-        :param max_result: default 100
+        :param repo_name: repo name
+        :param max_results: default 100
         :return:
         '''
-        response = self.cli.describe_images(
-            repositoryName=name,
-            maxResults=max_result,
-        )
+        response = self.cli.describe_images(repositoryName=repo_name,
+                                            maxResults=max_results,
+                                            **kwargs)
         return response['imageDetails']
 
-    def list_images(self, name: str, max_result: int = 100):
+    def list_images(self, repo_name: str,
+                    max_results: int = 100):
         '''
 
-        :param name: repo name
-        :param max_result: default 100
+        :param repo_name: repo name
+        :param max_results: default 100
         :return:
         '''
-        response = self.cli.list_images(
-            repositoryName=name,
-            maxResults=max_result
-        )
+        response = self.cli.list_images(repositoryName=repo_name,
+                                        maxResults=max_results)
         return response['imageIds']
```

### Comparing `baram-0.4.4/baram/efs_manager.py` & `baram-0.4.5/baram/efs_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.4.4/baram/glue_manager.py` & `baram-0.4.5/baram/athena_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,261 +1,227 @@
-import os
-from pathlib import Path
+from pprint import pprint
+from typing import Optional, Union, Dict, Any, List, Literal
 
-import boto3
 import fire
+import boto3
+import awswrangler as wr
+from awswrangler.athena._utils import _QUERY_WAIT_POLLING_DELAY
 
-from baram.iam_manager import IAMManager
-from baram.log_manager import LogManager
 from baram.s3_manager import S3Manager
+from baram.log_manager import LogManager
+from baram.glue_manager import GlueManager
 
 
-class GlueManager(object):
-    def __init__(self, s3_bucket_name: str, table_path_prefix='table'):
+class AthenaManager(object):
+    def __init__(self,
+                 query_result_bucket_name: str,
+                 output_bucket_name: str,
+                 workgroup: str = 'primary'):
+        self.logger = LogManager.get_logger()
+        self.QUERY_RESULT_BUCKET = query_result_bucket_name
+        self.OUTPUT_BUCKET = output_bucket_name
+        self.ATHENA_WORKGROUP = workgroup
+
+    def create_external_table(self,
+                              db_name: str,
+                              table_name: str,
+                              column_def: dict,
+                              location: str,
+                              s3_output: str,
+                              column_comments: Optional[dict] = None,
+                              table_comment: Optional[str] = None,
+                              partition_cols: dict = None):
+        '''
+        Create Glue External Table with s3 file
+
+        :param db_name: target glue database name
+        :param table_name: target glue table name
+        :param column_def: definition for columns. each key means column name, and its value means column type
+        :param location: s3 location of data for table
+        :param s3_output: s3 location for query saving
+        :param column_comments: comments for columns. each key means column name, and its value means comment
+        :param table_comment: comment for table
+        :param partition_cols: same with column_def when do partitioning, None when don't.
+        :return:
+        '''
+        columns = ', '.join([f"{k} {column_def[k]} comment '{column_comments[k]}'"
+                             if k in column_comments.keys() else f"{k} {column_def[k]}" for k in column_def])
+        partitions = 'partitioned by (' + ', '.join([f"{k} {partition_cols[k]}"
+                                                    for k in partition_cols]) + ')' if partition_cols else ''
+
+        sql = f"create external table if not exists {db_name}.{table_name}("\
+              f"{columns}) "\
+              f"comment '{table_comment}' "\
+              f"{partitions} " \
+              f"row format delimited fields terminated by ',' "\
+              f"stored as textfile "\
+              f"location '{location}' "\
+              f"tblproperties ('classification'='csv', 'skip.header.line.count'='1');"
+
+        self.fetch_query(sql=sql,
+                         db_name=db_name,
+                         s3_output=s3_output)
+
+    def create_iceberg_table_with_query(self):
+        # TODO
+        pass
+
+    def create_iceberg_table_with_dataframe(self):
+        # TODO
+        pass
+
+    def delete_table(self, db_name: str, table_name: str):
+        '''
+        Delete Glue Table.
+
+        :param db_name: target glue database name
+        :param table_name: target glue table name
+        :param table_path:
+        :return:
         '''
+        sm = S3Manager(self.OUTPUT_BUCKET)
+        gm = GlueManager(self.OUTPUT_BUCKET)
 
-        :param s3_bucket_name: s3 bucket name where Glue uses as default.
-        '''
+        try:
+            table = gm.get_table(db_name=db_name, table_name=table_name)
+            location = table['StorageDescriptor']['Location'].replace(f's3://{gm.s3_bucket_name}/', '')
 
-        self.logger = LogManager.get_logger()
-        self.cli = boto3.client('glue')
-        self.im = IAMManager()
+            wr.catalog.delete_table_if_exists(database=db_name, table=table_name)
+            print(f'{db_name}.{table_name} is deleted, on athena')
 
-        self.worker_type = 'G.1X'
-        self.workers_num = 2
-        self.timeout = 2880
-        self.max_concurrent_runs = 123
-        self.max_retries = 0
-        self.python_ver = '3'
-        self.glue_ver = '3.0'
-        self.s3_path = f's3://{s3_bucket_name}'
-        self.sm = S3Manager(s3_bucket_name)
-        self.TABLE_PATH_PREFIX = table_path_prefix
-        self.MAX_RESULTS = 1000
-
-        # See https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-glue-arguments.html
-        self.default_args = {
-            '--job-language': 'scala',
-            '--TempDir': os.path.join(self.s3_path, 'temp'),
-            '--enable-continuous-cloudwatch-log': 'true',
-            '--enable-glue-datacatalog': 'true',
-            '--enable-job-insights': 'true',
-            '--enable-metrics': 'true',
-            '--enable-spark-ui': 'true',
-            '--job-bookmark-option': 'job-bookmark-enable',
-            '--spark-event-logs-path': os.path.join(self.s3_path, 'events/'),
-            '--encryption-type': 'sse-kms'
-        }
+            sm.delete_dir(s3_dir_path=location)
+            print(f'data of {table_name} in its location {location} is deleted, on s3')
 
-    def start_job_run(self, name: str):
-        '''
+        except Exception as e:
+            self.logger.info(e)
+            raise e
 
-        :param name: job name
-        :return:
+    def fetch_query(self,
+                    sql: str,
+                    db_name: Optional[str] = None,
+                    params: Union[Dict[str, Any], List[str], None] = None,
+                    paramstyle: Literal['qmark', 'named'] = 'qmark',
+                    s3_output: Optional[str] = None,
+                    athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY):
         '''
-        return self.cli.start_job_run(
-            JobName=name
-        )
+        Fetch query result.
 
-    def _get_command(self, name: str):
+        :param sql: sql
+        :param db_name: database name
+        :param params: for parametrized query.
+                       This should be dictionary for "named" paramstyle and list for "qmark" paramstyle.
+        :param paramstyle: "named" or "qmark"
+        :param s3_output: You can choose output bucket for query result. default is workgroup s3 bucket.
+        :param athena_query_wait_polling_delay: float, default: 0.25 seconds
+        Interval in seconds for how often the function will check if the Athena query has completed.
+        :return: Dictionary with the get_query_execution response. You can obtain query result as csv on S3.
         '''
+        pprint(sql)
+        query_execution_id = wr.athena.start_query_execution(sql=sql,
+                                                             workgroup=self.ATHENA_WORKGROUP,
+                                                             params=params,
+                                                             paramstyle=paramstyle,
+                                                             s3_output=s3_output,
+                                                             database=db_name)
 
-        :param name: get command object when you create or update glue job.
-        :return:
+        res = wr.athena.wait_query(query_execution_id=query_execution_id,
+                                   athena_query_wait_polling_delay=athena_query_wait_polling_delay)
+
+        arr = str(res['ResultConfiguration']['OutputLocation']).replace('s3://', '').split('/')
+
+        sm = S3Manager(self.QUERY_RESULT_BUCKET)
+        print(f"fetch_result_path={sm.get_s3_web_url(arr[0], '/'.join(arr[1:]))}")
+        return res
+
+    def count_rows_from_table(self, db_name: str, table_name: str):
         '''
+        Return rows from table.
 
-        return {
-            'Name': 'glueetl',
-            'ScriptLocation': os.path.join(self.s3_path, "scripts", f'{name}.scala'),
-            'PythonVersion': self.python_ver
-        }
-
-    def create_job(self,
-                   name: str,
-                   package_name: str,
-                   role_name: str,
-                   extra_jars: str,
-                   security_configuration: str):
-        '''
-
-        :param name: glue job name
-        :param package_name: glue jar package name
-        :param role_name:  role name
-        :param extra_jars: extra jar path in s3
-        :param security_configuration:  security configuration
+        :param table_name:
         :return:
         '''
+        df = self.from_athena_to_df(sql=f'SELECT count(*) as cnt FROM {table_name}', db_name=db_name)
+        return int(df['cnt'])
 
-        self.default_args['--class'] = f'{package_name}.{name}'
-        self.default_args['--extra-jars'] = extra_jars
+    def optimize_and_vacumm_iceberg_table(self, db_name: str, table_name: str):
+        '''
+        Optimize and Vacumm iceberg table in database.
 
-        try:
-            self.cli.create_job(
-                Name=name,
-                Description='',
-                Role=self.im.get_role_arn(role_name),
-                ExecutionProperty={
-                    'MaxConcurrentRuns': self.max_concurrent_runs
-                },
-                Command=self._get_command(name),
-                DefaultArguments=self.default_args,
-                MaxRetries=self.max_retries,
-                Timeout=self.timeout,
-                SecurityConfiguration=security_configuration,
-                GlueVersion=self.glue_ver,
-                NumberOfWorkers=self.workers_num,
-                WorkerType=self.worker_type
-            )
-        except self.cli.exceptions.IdempotentParameterMismatchException as e:
-            self.logger.error(str(e))
-
-    def get_job(self, job_name: str):
-        '''
-
-        :param job_name: glue job name.
-        :return: glue job
-        '''
-        return self.cli.get_job(JobName=job_name)
-
-    def update_job(self,
-                   name: str,
-                   package_name: str,
-                   role_name: str,
-                   extra_jars: str,
-                   security_configuration: str):
-        '''
-
-        :param name: job name
-        :param package_name: glue jar package name
-        :param role_name:  role name
-        :param extra_jars: extra jar path in s3
-        :param security_configuration:  security configuration
+        :param db_name:
+        :param table_name:
         :return:
         '''
 
-        self.default_args['--class'] = f'{package_name}.{name}'
-        self.default_args['--extra-jars'] = extra_jars
+        print(f"{table_name} optimize start")
+        self.optimize_table(table_name, db_name)
 
-        return self.cli.update_job(
-            JobName=name,
-            JobUpdate={
-                'Role': self.im.get_role_arn(role_name),
-                'ExecutionProperty': {
-                    'MaxConcurrentRuns': self.max_concurrent_runs
-                },
-                'Command': self._get_command(name),
-                'DefaultArguments': self.default_args,
-                'MaxRetries': self.max_retries,
-                'Timeout': self.timeout,
-                'WorkerType': self.worker_type,
-                'NumberOfWorkers': self.workers_num,
-                'SecurityConfiguration': security_configuration,
-                'GlueVersion': self.glue_ver
-            }
-        )
+        print(f"{table_name} vacumm start")
+        self.vacumm_table(table_name, db_name)
 
-    def delete_job(self, name: str):
+    def optimize_iceberg_table(self, db_name: str, table_name: str):
         '''
+        Optimize iceberg table.
 
-        :param name: job name
+        :param db_name: database name
+        :param table_name: table name
         :return:
         '''
-        return self.cli.delete_job(JobName=name)
 
-    def delete_table(self, db_name: str, table_name: str, include_s3: bool = False):
+        return self.fetch_query(f"OPTIMIZE {table_name} REWRITE DATA USING BIN_PACK", db_name)
+
+    def vacumm_iceberg_table(self, db_name: str, table_name: str):
         '''
+        Vacumm iceberg table.
 
         :param db_name: database name
-        :param table_name: job name
-        :param include_s3: delete table including s3 or not
+        :param table_name: table name
         :return:
         '''
-        try:
-            self.cli.delete_table(
-                DatabaseName=db_name,
-                Name=table_name
-            )
-        except Exception as e:
-            pass
-        finally:
-            if include_s3:
-                print(f'delete {os.path.join(self.TABLE_PATH_PREFIX, db_name, table_name)}')
-                self.sm.delete_dir(os.path.join(self.TABLE_PATH_PREFIX, db_name, table_name))
 
-    def get_table(self, db_name: str, table_name: str):
+        return self.fetch_query(f"VACUUM {table_name}", db_name)
+
+    def check_table_exists(self, db_name: str, table_name: str):
         '''
+        Return table exists or not.
 
         :param db_name: database name
         :param table_name: table name
         :return:
         '''
-        return self.cli.get_table(
-            DatabaseName=db_name,
-            Name=table_name
-        )
-
-    def list_job_names(self,
-                       max_results: int = 50,
-                       name_filter: str = ''):
+        return wr.catalog.does_table_exist(db_name, table_name)
+
+    def read_query_txt(self,
+                       bucket_name: str,
+                       filepath: str,
+                       replacements: Optional[dict] = None):
         '''
-        List glue jobs
+        Read txt sql file from s3 and fetch it via Athena.
 
-        :param max_results:
-        :param name_filter:
-        :return:
+        :param bucket_name: the name of s3 bucket containing file
+        :param filepath: prefix of file
+        :param replacements: specified replacements for specific purpose of query
+        :return: string, a line of query
         '''
-        max_results = max_results if max_results else self.MAX_RESULTS
-        jobs = self.cli.list_jobs(MaxResults=max_results)['JobNames']
+        pass
 
-        return [job for job in jobs if name_filter in jobs]
+    def from_athena_to_df(self, sql: str, db_name: str, workgroup: Optional[str] = None):
+        '''
+        run query and return data frame.
 
-    def refresh_job(self,
-                    code_path: str,
-                    exclude_names: list,
-                    package_name: str,
-                    role_name: str,
-                    extra_jars: str,
-                    security_configuration: str):
-        '''
-
-        :param code_path: code path
-        :param exclude_names: job names to be excluded
-        :param package_name: glue jar package name
-        :param role_name: glue role name
-        :param extra_jars: extra jar path in s3
-        :param security_configuration: security configuraton
+        :param sql: sql
+        :param db_name: database name
+        :param workgroup: athena workgroup
         :return:
         '''
+        workgroup = workgroup if workgroup else self.ATHENA_WORKGROUP
 
-        glue_jobs = set([f'{jn}.scala' for jn in self.list_job_names()])
-        git_jobs = set([f for f in os.listdir(code_path)])
+        df = wr.athena.read_sql_query(sql=sql,
+                                      ctas_approach=False,
+                                      database=db_name,
+                                      workgroup=workgroup)
+        return df
 
-        rest_in_glue = glue_jobs - git_jobs
-        for f in rest_in_glue:
-            name = Path(f).stem
-            self.delete_job(name)
-            self.logger.info(f'{name} deleted.')
-
-        rest_in_git = git_jobs - glue_jobs
-        for f in rest_in_git:
-            name = Path(f).stem
-            if name in exclude_names:
-                continue
-            self.create_job(name, package_name, role_name, extra_jars, security_configuration)
-            self.logger.info(f'{name} created.')
-
-    def summary(self):
-        jobs = self.cli.list_jobs()
-        if 'JobNames' in jobs:
-            for j in jobs['JobNames']:
-                r = self.cli.get_job_runs(JobName=j)
-                if 'JobRuns' in r and len(r['JobRuns']) > 0:
-                    last_run = r['JobRuns'][0]
-                    last_run['StartedOn']
-
-                    duration = int((last_run['CompletedOn'] - last_run['StartedOn']).total_seconds())
-                    print(
-                        f"{last_run['JobName']}\t{last_run['AllocatedCapacity']}\t{last_run['StartedOn']}\t{last_run['CompletedOn']}\t{duration}")
+    # TODO: Add a method that dumps athena query result into s3 directly.
 
 
 if __name__ == '__main__':
-    fire.Fire(GlueManager)
+    fire.Fire(AthenaManager)
```

### Comparing `baram-0.4.4/baram/iam_manager.py` & `baram-0.4.5/baram/iam_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.4.4/baram/kms_manager.py` & `baram-0.4.5/baram/kms_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.4.4/baram/lambda_manager.py` & `baram-0.4.5/baram/lambda_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.4.4/baram/poetry_manager.py` & `baram-0.4.5/baram/poetry_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.4.4/baram/process_manager.py` & `baram-0.4.5/baram/process_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.4.4/baram/requests_manager.py` & `baram-0.4.5/baram/requests_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.4.4/baram/s3_manager.py` & `baram-0.4.5/baram/s3_manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import os
 from typing import Optional
 
+import awswrangler as wr
 import boto3
+import botocore
 from botocore.client import Config
 
 from baram.kms_manager import KMSManager
 from baram.log_manager import LogManager
 
 
 class S3Manager(object):
@@ -101,45 +103,59 @@
         '''
         self.logger.info('Uploading results to s3 initiated...')
         self.logger.info(f'local_path:{local_dir_path}, s3_path:{s3_dir_path}')
         try:
             for path, subdirs, files in os.walk(local_dir_path):
                 for file in files:
                     dest_path = path.replace(local_dir_path, '')
-                    s3file_path = os.path.normpath(s3_dir_path + '/' + dest_path + '/' + file)
+                    s3_file_path = os.path.normpath(s3_dir_path + '/' + dest_path + '/' + file)
                     local_file_path = os.path.join(path, file)
 
                     extra_args = {'ServerSideEncryption': self.kms_algorithm,
                                   'SSEKMSKeyId': self.kms_id} if self.kms_id else None
-                    self.cli.upload_file(local_file_path,
-                                         self.bucket_name,
-                                         s3file_path,
-                                         ExtraArgs=extra_args)
+                    self.cli.upload_file(local_file_path, self.bucket_name, s3_file_path, ExtraArgs=extra_args)
                     self.logger.info(
-                        f'upload : {local_file_path} to Target: s3://{self.bucket_name}/{s3file_path} Success.')
+                        f'upload : {local_file_path} to Target: s3://{self.bucket_name}/{s3_file_path} Success.')
         except Exception as e:
             self.logger.info(e)
             raise e
 
-    def upload_file(self, local_file_path: str, s3file_path: str):
+    def write_and_upload_file(self, content: str, local_file_path: str, s3_file_path: str, do_remove: bool = False):
         '''
         Upload file.
+
+        :param content: the content of file. ex) 'col1,col2\nname,height'
         :param local_file_path: local file path. ex) /Users/lks21c/repo/sli-aflow/a.csv
-        :param s3_dir_path: s3 path. ex) nylon-detector/crawl_data/a.csv
+        :param s3_file_path: s3 path. ex) nylon-detector/crawl_data/a.csv
+        :param do_remove: remove written file
+        :return: response
+        '''
+
+        with open(local_file_path, 'w') as f:
+            f.write(content)
+        assert os.path.exists(local_file_path)
+        self.upload_file(local_file_path, s3_file_path)
+
+        if do_remove:
+            os.remove(local_file_path)
+
+    def upload_file(self, local_file_path: str, s3_file_path: str):
+        '''
+        Upload file.
+
+        :param local_file_path: local file path. ex) /Users/lks21c/repo/sli-aflow/a.csv
+        :param s3_file_path: s3 path. ex) nylon-detector/crawl_data/a.csv
         :return: response
         '''
 
         try:
             extra_args = {'ServerSideEncryption': self.kms_algorithm,
                           'SSEKMSKeyId': self.kms_id} if self.kms_id else None
-            self.cli.upload_file(local_file_path,
-                                 self.bucket_name,
-                                 s3file_path,
-                                 ExtraArgs=extra_args)
-            self.logger.info(f'upload : {local_file_path} to Target: s3://{self.bucket_name}/{s3file_path} Success.')
+            self.cli.upload_file(local_file_path, self.bucket_name, s3_file_path, ExtraArgs=extra_args)
+            self.logger.info(f'upload : {local_file_path} to Target: s3://{self.bucket_name}/{s3_file_path} Success.')
         except Exception as e:
             self.logger.info(e)
             raise e
 
     def download_dir(self, s3_dir_path: str, local_dir_path: str = os.getcwd()):
         '''
         Download directory from s3.
@@ -263,7 +279,75 @@
         :return:
         '''
         self.cli.copy_object(
             Bucket=self.bucket_name,
             CopySource=f'{self.bucket_name}/{from_key}',
             Key=to_key
         )
+
+    def get_s3_web_url(self, s3_bucket_name, path: str, region: str = 'ap-northeast-2'):
+        '''
+        get s3 web url
+
+        :param s3_bucket_name: s3 bucket name
+        :param path: s3 path
+        :param region: s3 region
+        :return:
+        '''
+        return f'https://s3.console.aws.amazon.com/s3/buckets/{s3_bucket_name}?region={region}&prefix={path}'
+
+    def convert_s3_path_to_web_url(self, s3_path: str):
+        '''
+        Convert s3 url to web url
+
+        :param s3_path:
+        :return:
+        '''
+        token = s3_path.replace('s3://', '').split('/')
+        return self.get_s3_web_url(token[0], '/'.join(token[1:]))
+
+    def get_s3_full_path(self, s3_bucket_name: str, path: str):
+        '''
+        Get s3 full path.
+
+        :param s3_bucket_name: bucket name
+        :param path: path
+        :return:
+        '''
+        return f's3://{s3_bucket_name}/{path}'
+
+    def check_s3_object_exists(self, s3_bucket_name: str, path: str):
+        '''
+        Check if s3 object exists.
+
+        :param s3_bucket_name: s3 bucket name
+        :param path:  path
+        :return:
+        '''
+        try:
+            self.cli.head_object(Bucket=s3_bucket_name,
+                                 Key=path)
+            return True
+        except botocore.exceptions.ClientError as e:
+            pass
+        return False
+
+    def rename_file(self, from_file_path: str, to_file_path: str):
+        '''
+        Rename s3 obj.
+
+        :param from_file_path:
+        :param to_file_path:
+        :return:
+        '''
+        self.copy_object(from_key=from_file_path, to_key=to_file_path)
+        self.delete_dir(from_file_path)
+
+    def count_csv_row_count(self, csv_path: str, distinct_col_name: Optional[str] = None):
+        df = wr.s3.read_csv(path=f's3://{self.bucket_name}/{csv_path}', index_col=False,
+                            keep_default_na=False)
+        import pandas as pd
+
+        if distinct_col_name:
+            return len(pd.unique(df[distinct_col_name]))
+        else:
+            return df.shape[0]
```

### Comparing `baram-0.4.4/pyproject.toml` & `baram-0.4.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "baram"
-version = "0.4.4"
+version = "0.4.5"
 description = "AWS Framework for python"
 authors = ["Kwangsik Lee <lks21c@gmail.com>"]
 readme = "readme.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fire = "^0.4.0"
@@ -12,14 +12,16 @@
 boto3 = "1.28.62"
 aiohttp = "^3.8.1"
 nest-asyncio = "^1.5.5"
 toml = "^0.10.2"
 ujson = "^5.5.0"
 requests = "^2.28.1"
 awswrangler = { version = "3.5.2", extras = ["modin"] }
+tzlocal = "^5.2"
+six = "^1.16.0"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```


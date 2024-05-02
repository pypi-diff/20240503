# Comparing `tmp/ng_data_pipelines_sdk-0.5.0.tar.gz` & `tmp/ng_data_pipelines_sdk-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-0.5.0.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-0.6.0.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-0.5.0.tar` & `ng_data_pipelines_sdk-0.6.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-04-30 20:39:04.002808 ng_data_pipelines_sdk-0.5.0/README.md
--rw-r--r--   0        0        0        0 2024-04-30 20:39:04.025808 ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     9155 2024-04-30 20:39:04.003808 ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-04-30 20:39:04.003808 ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    26500 2024-04-30 20:39:04.003808 ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0    15420 2024-04-30 20:39:04.003808 ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     4648 2024-04-30 20:39:04.003808 ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     1453 2024-04-30 20:39:04.003808 ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      672 2024-04-30 20:39:04.004808 ng_data_pipelines_sdk-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-05-02 22:26:22.376910 ng_data_pipelines_sdk-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 22:26:22.401909 ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     9155 2024-05-02 22:26:22.377910 ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-05-02 22:26:22.377910 ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    27485 2024-05-02 22:26:22.377910 ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0    15573 2024-05-02 22:26:22.377910 ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     5093 2024-05-02 22:26:22.377910 ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     1453 2024-05-02 22:26:22.377910 ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      672 2024-05-02 22:26:22.378910 ng_data_pipelines_sdk-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.6.0/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,39 +58,43 @@
         self.completed_steps = []
         logger.info("DataFrameManager initialized.")
 
     def _get_bucket_url(self, bucket_params: S3BucketParams) -> str:
         return f"{self.file_system}://{bucket_params.bucket_name}"
 
     def _get_processing_date_partition_path(
-        self, df_params: Union[DataFrameReadWriteParams, DataFrameReadWriteParams]
-    ) -> str:
-        if df_params.processing_date_partitions is None:
+        self, processing_date, processing_date_partitions
+    ) -> Union[str, List[str]]:
+        if processing_date_partitions is None:
             return ""
 
-        if not isinstance(df_params.processing_date, datetime):
+        if not isinstance(processing_date, datetime):
             raise ValueError(
-                f"processing_date must be a datetime object to calculate partition path. Received: '{df_params.processing_date}'"
+                f"processing_date must be a datetime object to calculate partition path. Received: '{processing_date}'"
             )
 
         partition_path_segments = [
-            f"{date_part.value}={DATE_FORMATTER[date_part.value.replace('part_', '')](df_params.processing_date)}"
-            for date_part in df_params.processing_date_partitions
+            f"{date_part.value}={DATE_FORMATTER[date_part.value.replace('part_', '')](processing_date)}"
+            for date_part in processing_date_partitions
         ]
 
         processing_date_partition_path = "/".join(partition_path_segments)
 
         return processing_date_partition_path
 
     def _get_dataframe_path_with_date_partitions(
         self, df_params: DataFrameReadWriteParams
-    ) -> str:
-        dataframe_path_with_date_partitions = f"{df_params.path_to_dataframe_root}/{self._get_processing_date_partition_path(df_params)}"
-
-        return dataframe_path_with_date_partitions.strip("/")
+    ) -> Union[str, List[str]]:
+        if isinstance(df_params.processing_date, list):
+            return [
+                f"{df_params.path_to_dataframe_root}/{self._get_processing_date_partition_path(processing_date, df_params.processing_date_partitions)}"
+                for processing_date in df_params.processing_date
+            ]
+        else:
+            return f"{df_params.path_to_dataframe_root}/{self._get_processing_date_partition_path(df_params.processing_date, df_params.processing_date_partitions)}"
 
     def convert_schema_object_to_pyspark_schema(
         self, schema_object: Dict[str, Any]
     ) -> StructType:
         logger.debug("Converting schema object to PySpark StructType...")
         pyspark_schema = StructType.fromJson(schema_object)
         pyspark_schema = handle_pyspark_timestamp_in_schema(pyspark_schema)
@@ -162,17 +166,28 @@
         Returns:
             DataFrame: The read DataFrame.
 
         """
         read_params = df_params.df_params
         bucket_url = self._get_bucket_url(read_params.bucket_params)
         if read_params.specific_path:
-            path = f"{bucket_url}/{read_params.specific_path}"
+            if isinstance(read_params.specific_path, list):
+                path = [f"{bucket_url}/{path}" for path in read_params.specific_path]
+            else:
+                path = f"{bucket_url}/{read_params.specific_path}"
         else:
-            path = f"{bucket_url}/{self._get_dataframe_path_with_date_partitions(read_params)}"
+            if isinstance(read_params.processing_date, list):
+                path = [
+                    f"{bucket_url}/{path_with_date_partitions}"
+                    for path_with_date_partitions in self._get_dataframe_path_with_date_partitions(
+                        read_params
+                    )
+                ]
+            else:
+                path = f"{bucket_url}/{self._get_dataframe_path_with_date_partitions(read_params)}"
 
         if df_params.pyspark_schema_struct:
             schema = self.convert_schema_object_to_pyspark_schema(
                 schema_object=df_params.pyspark_schema_struct
             )
         elif df_params.s3_schema_path_params:
             schema = self.retrieve_schema_from_s3(df_params.s3_schema_path_params)
@@ -205,14 +220,18 @@
         pyspark_schema_json = df.schema.jsonValue()
         bucket_name = write_params.bucket_params.bucket_name
 
         if bucket_name is None:
             raise ValueError("bucket_name must be provided to write schema to S3")
 
         if write_params.specific_path:
+            if isinstance(write_params.specific_path, list):
+                raise ValueError(
+                    "Specific path is set as a list. Only a single path is allowed for writing the schema."
+                )
             logger.warning(
                 "Specific path is set for writing the schema. Schema will be written to the same path."
             )
             path_to_schema = write_params.specific_path
         else:
             if write_params.path_to_dataframe_root is None:
                 raise ValueError(
```

### Comparing `ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/interfaces.py`

 * *Files 3% similar despite different names*

```diff
@@ -198,29 +198,28 @@
 
 class DataFrameReadWriteParams(BaseModelJsonDumps):
     """
     Represents the parameters for reading and writing a DataFrame.
 
     Attributes:
         bucket_params (S3BucketParams): The parameters for the S3 bucket.
-        specific_path (str, optional): The specific path within the bucket. Defaults to None.
-        path_to_dataframe_root (str, optional): The path to the root folder of the DataFrame. Defaults to None.
+        specific_path (Optional[Union[List[str], str]]): The specific path to the data within the bucket.
+        path_to_dataframe_root (Optional[str]): The path to the root folder of the DataFrame within the bucket.
         file_type (FileType): The type of file to read or write.
-        processing_date (Union[datetime, Literal["{{processing_date}}"], Literal["{{processing_date_previous}}"]], optional):
-            The processing date for the DataFrame. Defaults to "{{processing_date}}".
-        processing_date_partitions (List[DatePartition], optional): The processing date partitions. Defaults to None.
-        processing_date_partitions_first (bool): Flag indicating whether to use processing date partitions first. Defaults to True.
-        column_partitions (List[str], optional): The column partitions. Defaults to None.
+        processing_date (Union[List[datetime], datetime, Literal["{{processing_date}}"], Literal["{{processing_date_previous}}"]]): The processing date or dates to use for partitioning.
+        processing_date_partitions (Optional[List[DatePartition]]): The list of date partitions to use for filtering.
+        processing_date_partitions_first (bool): Flag indicating whether to process date partitions first.
+        column_partitions (Optional[List[str]]): The list of column partitions to use for filtering.
     """
-
     bucket_params: S3BucketParams
-    specific_path: Optional[str] = None
+    specific_path: Optional[Union[List[str], str]] = None
     path_to_dataframe_root: Optional[str] = None
     file_type: FileType
     processing_date: Union[
+        List[datetime],
         datetime,
         Literal["{{processing_date}}"],
         Literal["{{processing_date_previous}}"],
     ] = "{{processing_date}}"
     processing_date_partitions: Optional[List[DatePartition]] = None
     processing_date_partitions_first: bool = True
     column_partitions: Optional[List[str]] = None
@@ -251,26 +250,29 @@
             raise ValueError(
                 "Either 'specific_path' or 'path_to_dataframe_root' should be passed"
             )
 
         return data
 
     @field_validator("path_to_dataframe_root", "specific_path")
-    def strip_slashes(cls, v: str) -> str:
+    def strip_slashes(cls, v: Union[str, List[str]]) -> str:
         """
         Strips leading and trailing slashes from the input string.
 
         Args:
             v (str): The input string.
 
         Returns:
             str: The input string with leading and trailing slashes stripped.
         """
         if v is not None:
-            return v.strip("/")
+            if isinstance(v, list):
+                return [x.strip("/") for x in v] # type: ignore
+            else:
+                return v.strip("/")
 
     @field_validator("path_to_dataframe_root")
     def ensure_dataframe_root_parent_folder(cls, v: str) -> str:
         """
         Ensures that 'path_to_dataframe_root' has at least one parent folder inside the bucket.
 
         Args:
```

### Comparing `ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/spark_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Union
 
 from pyspark.conf import SparkConf
 from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql.types import StructType
 
 from ng_data_pipelines_sdk.interfaces import AWSCredentials, Env, FileType
 
@@ -77,30 +77,40 @@
             )
 
         return config
 
     def read(
         self,
         env: Env,
-        path: str,
+        path: Union[str, List[str]],
         file_type: FileType,
         schema: Optional[StructType] = None,
     ):
         """
         Reads data from a specified path using the specified file type and optional schema.
 
         Args:
             env (Env): The environment to use for setting AWS credentials.
-            path (str): The path to the data source.
+            path (Union[str, List[str]]): The path or list of paths to the data source.
             file_type (FileType): The type of the data source.
             schema (Optional[StructType], optional): The schema to use for reading the data. Defaults to None.
 
         Returns:
             DataFrame: The loaded data as a DataFrame.
 
+        Raises:
+            None
+
+        Examples:
+            >>> env = Env()
+            >>> path = "/path/to/data"
+            >>> file_type = FileType.CSV
+            >>> schema = StructType([StructField("name", StringType()), StructField("age", IntegerType())])
+            >>> spark_manager = SparkManager()
+            >>> df = spark_manager.read(env, path, file_type, schema)
         """
         self._set_aws_credentials(env)
 
         if schema:
             return self.spark.read.format(file_type).schema(schema).load(path)
         else:
             return self.spark.read.format(file_type).load(path)
```

### Comparing `ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.5.0/pyproject.toml` & `ng_data_pipelines_sdk-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "0.5.0"
+version = "0.6.0"
 description = "A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airflow 2.8.1."
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `ng_data_pipelines_sdk-0.5.0/PKG-INFO` & `ng_data_pipelines_sdk-0.6.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 0.5.0
+Version: 0.6.0
 Summary: A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airflow 2.8.1.
 Author: ng.cash
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


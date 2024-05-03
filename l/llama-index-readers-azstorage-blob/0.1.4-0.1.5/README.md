# Comparing `tmp/llama_index_readers_azstorage_blob-0.1.4.tar.gz` & `tmp/llama_index_readers_azstorage_blob-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_azstorage_blob-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_readers_azstorage_blob-0.1.5.tar", max compression
```

## Comparing `llama_index_readers_azstorage_blob-0.1.4.tar` & `llama_index_readers_azstorage_blob-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3573 2024-03-26 18:14:34.683385 llama_index_readers_azstorage_blob-0.1.4/README.md
--rw-r--r--   0        0        0      107 2024-03-26 18:14:34.683385 llama_index_readers_azstorage_blob-0.1.4/llama_index/readers/azstorage_blob/__init__.py
--rw-r--r--   0        0        0     7471 2024-03-26 18:14:34.683385 llama_index_readers_azstorage_blob-0.1.4/llama_index/readers/azstorage_blob/base.py
--rw-r--r--   0        0        0     1603 2024-03-26 18:14:34.683385 llama_index_readers_azstorage_blob-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4307 1970-01-01 00:00:00.000000 llama_index_readers_azstorage_blob-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3497 2024-05-03 14:42:30.194296 llama_index_readers_azstorage_blob-0.1.5/README.md
+-rw-r--r--   0        0        0      107 2024-05-03 14:42:30.194296 llama_index_readers_azstorage_blob-0.1.5/llama_index/readers/azstorage_blob/__init__.py
+-rw-r--r--   0        0        0     7627 2024-05-03 14:42:30.194296 llama_index_readers_azstorage_blob-0.1.5/llama_index/readers/azstorage_blob/base.py
+-rw-r--r--   0        0        0     1603 2024-05-03 14:42:30.194296 llama_index_readers_azstorage_blob-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4231 1970-01-01 00:00:00.000000 llama_index_readers_azstorage_blob-0.1.5/PKG-INFO
```

### Comparing `llama_index_readers_azstorage_blob-0.1.4/README.md` & `llama_index_readers_azstorage_blob-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     account_url="https://<storage account name>.blob.core.windows.net",
     credential=default_credential,
 )
 
 documents = loader.load_data()
 ```
 
-This loader is designed to be used as a way to load data into [LlamaIndex](https://github.com/run-llama/llama_index/tree/main/llama_index) and/or subsequently used as a Tool in a [LangChain](https://github.com/hwchase17/langchain) Agent. See [here](https://github.com/emptycrown/llama-hub/tree/main) for examples.
+This loader is designed to be used as a way to load data into [LlamaIndex](https://github.com/run-llama/llama_index/tree/main/llama_index) and/or subsequently used as a Tool in a [LangChain](https://github.com/hwchase17/langchain) Agent.
 
 ### Updates
 
 #### [2023-12-14] by [JAlexMcGraw](https://github.com/JAlexMcGraw) (#765)
 
 - Added functionality to allow user to connect to blob storage with connection string
 - Changed temporary file names from random to back to original names
```

### Comparing `llama_index_readers_azstorage_blob-0.1.4/llama_index/readers/azstorage_blob/base.py` & `llama_index_readers_azstorage_blob-0.1.5/llama_index/readers/azstorage_blob/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,15 +78,16 @@
         total_download_start_time = time.time()
         blob_meta = {}
 
         with tempfile.TemporaryDirectory() as temp_dir:
             if self.blob:
                 blob_client = container_client.get_blob_client(self.blob)
                 stream = blob_client.download_blob()
-                download_file_path = os.path.join(temp_dir, stream.name)
+                sanitized_file_name = stream.name.replace("/", "-")
+                download_file_path = os.path.join(temp_dir, sanitized_file_name)
                 logger.info(f"Start download of {self.blob}")
                 start_time = time.time()
                 with open(file=download_file_path, mode="wb") as download_file:
                     stream.readinto(download_file)
                 blob_meta[download_file_path] = blob_client.get_blob_properties()
                 end_time = time.time()
                 logger.info(
@@ -96,15 +97,16 @@
             # Needed because the loading of a container can take some time, and if everything is already pickled into local environment, loading it from there will be much faster.
             else:
                 logger.info("Listing blobs")
                 blobs_list = container_client.list_blobs(
                     self.name_starts_with, self.include
                 )
                 for obj in blobs_list:
-                    download_file_path = os.path.join(temp_dir, obj.name)
+                    sanitized_file_name = obj.name.replace("/", "-")
+                    download_file_path = os.path.join(temp_dir, sanitized_file_name)
                     logger.info(f"Start download of {obj.name}")
                     start_time = time.time()
                     blob_client = container_client.get_blob_client(obj)
                     stream = blob_client.download_blob()
                     with open(file=download_file_path, mode="wb") as download_file:
                         stream.readinto(download_file)
                     blob_meta[download_file_path] = blob_client.get_blob_properties()
```

### Comparing `llama_index_readers_azstorage_blob-0.1.4/pyproject.toml` & `llama_index_readers_azstorage_blob-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 description = "llama-index readers azstorage_blob integration"
 exclude = ["**/BUILD"]
 keywords = ["azure storage", "azure", "blob", "container"]
 license = "MIT"
 maintainers = ["rivms"]
 name = "llama-index-readers-azstorage-blob"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 azure-storage-blob = "^12.19.0"
 azure-identity = "^1.15.0"
```

### Comparing `llama_index_readers_azstorage_blob-0.1.4/PKG-INFO` & `llama_index_readers_azstorage_blob-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-azstorage-blob
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index readers azstorage_blob integration
 License: MIT
 Keywords: azure storage,azure,blob,container
 Author: Your Name
 Author-email: you@example.com
 Maintainer: rivms
 Requires-Python: >=3.8.1,<4.0
@@ -88,15 +88,15 @@
     account_url="https://<storage account name>.blob.core.windows.net",
     credential=default_credential,
 )
 
 documents = loader.load_data()
 ```
 
-This loader is designed to be used as a way to load data into [LlamaIndex](https://github.com/run-llama/llama_index/tree/main/llama_index) and/or subsequently used as a Tool in a [LangChain](https://github.com/hwchase17/langchain) Agent. See [here](https://github.com/emptycrown/llama-hub/tree/main) for examples.
+This loader is designed to be used as a way to load data into [LlamaIndex](https://github.com/run-llama/llama_index/tree/main/llama_index) and/or subsequently used as a Tool in a [LangChain](https://github.com/hwchase17/langchain) Agent.
 
 ### Updates
 
 #### [2023-12-14] by [JAlexMcGraw](https://github.com/JAlexMcGraw) (#765)
 
 - Added functionality to allow user to connect to blob storage with connection string
 - Changed temporary file names from random to back to original names
```


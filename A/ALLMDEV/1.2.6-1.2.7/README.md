# Comparing `tmp/ALLMDEV-1.2.6-py3-none-any.whl.zip` & `tmp/ALLMDEV-1.2.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,56 @@
-Zip file size: 13622 bytes, number of entries: 15
+Zip file size: 40611 bytes, number of entries: 54
 -rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-17 06:01 ALLMDEV/__init__.py
 -rw-rw-rw-  2.0 fat     3096 b- defN 24-Apr-27 08:57 ALLMDEV/agent_rag.py
 -rw-rw-rw-  2.0 fat     3440 b- defN 24-Apr-27 08:48 ALLMDEV/agent_ragrun.py
 -rw-rw-rw-  2.0 fat      757 b- defN 24-Apr-17 06:35 ALLMDEV/cli.py
+-rw-rw-rw-  2.0 fat      981 b- defN 24-May-03 13:33 ALLMDEV/cloud.py
+-rw-rw-rw-  2.0 fat     1851 b- defN 24-May-03 13:47 ALLMDEV/cloudrag.py
 -rw-rw-rw-  2.0 fat     1945 b- defN 24-Apr-26 04:23 ALLMDEV/fasty.py
 -rw-rw-rw-  2.0 fat     2579 b- defN 24-Apr-20 10:27 ALLMDEV/generate.py
 -rw-rw-rw-  2.0 fat    10334 b- defN 24-Apr-19 14:10 ALLMDEV/instruct.py
 -rw-rw-rw-  2.0 fat     1985 b- defN 24-Apr-25 11:09 ALLMDEV/rag.py
 -rw-rw-rw-  2.0 fat     3016 b- defN 24-Apr-25 07:21 ALLMDEV/ragrun.py
 -rw-rw-rw-  2.0 fat     3490 b- defN 24-Apr-27 09:53 ALLMDEV/ragserve.py
--rw-rw-rw-  2.0 fat     3268 b- defN 24-Apr-27 09:56 ALLMDEV-1.2.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-27 09:56 ALLMDEV-1.2.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      201 b- defN 24-Apr-27 09:56 ALLMDEV-1.2.6.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-27 09:56 ALLMDEV-1.2.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1141 b- defN 24-Apr-27 09:56 ALLMDEV-1.2.6.dist-info/RECORD
-15 files, 35391 bytes uncompressed, 11764 bytes compressed:  66.8%
+-rw-rw-rw-  2.0 fat      683 b- defN 24-May-03 07:37 ALLMDEV/test.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/chains/__init__.py
+-rw-rw-rw-  2.0 fat     4880 b- defN 24-Apr-30 08:27 ALLMDEV/allmutils/chains/long_text_processing_chain.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/constants/__init__.py
+-rw-rw-rw-  2.0 fat      575 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/constants/azure.py
+-rw-rw-rw-  2.0 fat      877 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/constants/input_data.py
+-rw-rw-rw-  2.0 fat      258 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/constants/prompt.py
+-rw-rw-rw-  2.0 fat      270 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/constants/vertex_ai.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/defaults/__init__.py
+-rw-rw-rw-  2.0 fat      666 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/defaults/azure_defaults.py
+-rw-rw-rw-  2.0 fat      117 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/defaults/general_defaults.py
+-rw-rw-rw-  2.0 fat      469 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/defaults/long_text_chain.py
+-rw-rw-rw-  2.0 fat      676 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/defaults/vertex_ai.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/domain/__init__.py
+-rw-rw-rw-  2.0 fat      471 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/domain/configuration.py
+-rw-rw-rw-  2.0 fat      777 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/domain/enumerables.py
+-rw-rw-rw-  2.0 fat      229 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/domain/input_data.py
+-rw-rw-rw-  2.0 fat      444 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/domain/prompt_dto.py
+-rw-rw-rw-  2.0 fat      730 b- defN 24-Apr-30 08:25 ALLMDEV/allmutils/domain/response.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/exceptions/__init__.py
+-rw-rw-rw-  2.0 fat     1548 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/exceptions/validation_input_data_exceptions.py
+-rw-rw-rw-  2.0 fat     1166 b- defN 24-Apr-30 07:59 ALLMDEV/allmutils/models/__init__.py
+-rw-rw-rw-  2.0 fat    16616 b- defN 24-Apr-30 08:28 ALLMDEV/allmutils/models/abstract.py
+-rw-rw-rw-  2.0 fat      935 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/models/azure_base.py
+-rw-rw-rw-  2.0 fat     2275 b- defN 24-Apr-30 08:24 ALLMDEV/allmutils/models/azure_llama2.py
+-rw-rw-rw-  2.0 fat     2190 b- defN 24-Apr-30 08:03 ALLMDEV/allmutils/models/azure_mistral.py
+-rw-rw-rw-  2.0 fat     1856 b- defN 24-Apr-30 08:03 ALLMDEV/allmutils/models/azure_openai.py
+-rw-rw-rw-  2.0 fat     3898 b- defN 24-Apr-30 08:03 ALLMDEV/allmutils/models/vertexai_base.py
+-rw-rw-rw-  2.0 fat     1985 b- defN 24-Apr-30 08:03 ALLMDEV/allmutils/models/vertexai_gemini.py
+-rw-rw-rw-  2.0 fat     2148 b- defN 24-Apr-30 08:04 ALLMDEV/allmutils/models/vertexai_gemma.py
+-rw-rw-rw-  2.0 fat     1967 b- defN 24-Apr-30 08:04 ALLMDEV/allmutils/models/vertexai_palm.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/utils/__init__.py
+-rw-rw-rw-  2.0 fat     1264 b- defN 24-Apr-30 08:29 ALLMDEV/allmutils/utils/io_utils.py
+-rw-rw-rw-  2.0 fat      291 b- defN 24-Apr-18 13:17 ALLMDEV/allmutils/utils/logger_utils.py
+-rw-rw-rw-  2.0 fat     4843 b- defN 24-Apr-30 07:58 ALLMDEV/allmutils/utils/long_text_processing_utils.py
+-rw-rw-rw-  2.0 fat     2611 b- defN 24-Apr-30 08:29 ALLMDEV/allmutils/utils/response_parsing_utils.py
+-rw-rw-rw-  2.0 fat     3268 b- defN 24-May-03 13:48 ALLMDEV-1.2.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-03 13:48 ALLMDEV-1.2.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      273 b- defN 24-May-03 13:48 ALLMDEV-1.2.7.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 24-May-03 13:48 ALLMDEV-1.2.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     4842 b- defN 24-May-03 13:48 ALLMDEV-1.2.7.dist-info/RECORD
+54 files, 99711 bytes uncompressed, 32759 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -6,14 +6,20 @@
 
 Filename: ALLMDEV/agent_ragrun.py
 Comment: 
 
 Filename: ALLMDEV/cli.py
 Comment: 
 
+Filename: ALLMDEV/cloud.py
+Comment: 
+
+Filename: ALLMDEV/cloudrag.py
+Comment: 
+
 Filename: ALLMDEV/fasty.py
 Comment: 
 
 Filename: ALLMDEV/generate.py
 Comment: 
 
 Filename: ALLMDEV/instruct.py
@@ -24,23 +30,134 @@
 
 Filename: ALLMDEV/ragrun.py
 Comment: 
 
 Filename: ALLMDEV/ragserve.py
 Comment: 
 
-Filename: ALLMDEV-1.2.6.dist-info/METADATA
+Filename: ALLMDEV/test.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/__init__.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/chains/__init__.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/chains/long_text_processing_chain.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/constants/__init__.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/constants/azure.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/constants/input_data.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/constants/prompt.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/constants/vertex_ai.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/defaults/__init__.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/defaults/azure_defaults.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/defaults/general_defaults.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/defaults/long_text_chain.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/defaults/vertex_ai.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/domain/__init__.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/domain/configuration.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/domain/enumerables.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/domain/input_data.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/domain/prompt_dto.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/domain/response.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/exceptions/__init__.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/exceptions/validation_input_data_exceptions.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/models/__init__.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/models/abstract.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/models/azure_base.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/models/azure_llama2.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/models/azure_mistral.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/models/azure_openai.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/models/vertexai_base.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/models/vertexai_gemini.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/models/vertexai_gemma.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/models/vertexai_palm.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/utils/__init__.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/utils/io_utils.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/utils/logger_utils.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/utils/long_text_processing_utils.py
+Comment: 
+
+Filename: ALLMDEV/allmutils/utils/response_parsing_utils.py
+Comment: 
+
+Filename: ALLMDEV-1.2.7.dist-info/METADATA
 Comment: 
 
-Filename: ALLMDEV-1.2.6.dist-info/WHEEL
+Filename: ALLMDEV-1.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: ALLMDEV-1.2.6.dist-info/entry_points.txt
+Filename: ALLMDEV-1.2.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: ALLMDEV-1.2.6.dist-info/top_level.txt
+Filename: ALLMDEV-1.2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: ALLMDEV-1.2.6.dist-info/RECORD
+Filename: ALLMDEV-1.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ALLMDEV-1.2.6.dist-info/METADATA` & `ALLMDEV-1.2.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALLMDEV
-Version: 1.2.6
+Version: 1.2.7
 Summary: A simple and efficient python library for fast inference of GGUF Large Language Models.
 Author: All Advance AI
 Author-email: allmdev@allaai.com
 Maintainer: Soham Ghadge
 Maintainer-email: soham.ghadge@allaai.com
 Keywords: GGUF,GGUF Large Language Model,GGUF Large Language Models,GGUF Large Language Modeling,GGUF Large Language Modeling Library
 Description-Content-Type: text/markdown
```


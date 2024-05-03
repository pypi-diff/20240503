# Comparing `tmp/bpm_ai-1.7.1.tar.gz` & `tmp/bpm_ai-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai-1.7.1.tar", max compression
+gzip compressed data, was "bpm_ai-1.7.2.tar", max compression
```

## Comparing `bpm_ai-1.7.1.tar` & `bpm_ai-1.7.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      726 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/README.md
--rw-r--r--   0        0        0        0 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/common/__init__.py
--rw-r--r--   0        0        0      195 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/common/errors.py
--rw-r--r--   0        0        0     1668 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/common/multimodal.py
--rw-r--r--   0        0        0        0 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/compose/__init__.py
--rw-r--r--   0        0        0     1595 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/compose/compose.anthropic.prompt
--rw-r--r--   0        0        0     1369 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/compose/compose.openai.prompt
--rw-r--r--   0        0        0     1699 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/compose/compose.prompt
--rw-r--r--   0        0        0     3644 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/compose/compose.py
--rw-r--r--   0        0        0      950 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/compose/util.py
--rw-r--r--   0        0        0        0 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/decide/__init__.py
--rw-r--r--   0        0        0     8786 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/decide/decide.anthropic.prompt
--rw-r--r--   0        0        0     8181 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/decide/decide.openai.prompt
--rw-r--r--   0        0        0     8459 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/decide/decide.prompt
--rw-r--r--   0        0        0     6221 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/decide/decide.py
--rw-r--r--   0        0        0     3044 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/decide/schema.py
--rw-r--r--   0        0        0        0 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/extract/__init__.py
--rw-r--r--   0        0        0     1485 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/extract/extract.anthropic.prompt
--rw-r--r--   0        0        0     1286 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/extract/extract.openai.prompt
--rw-r--r--   0        0        0     1466 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/extract/extract.prompt
--rw-r--r--   0        0        0     7495 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/extract/extract.py
--rw-r--r--   0        0        0     2578 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/extract/util.py
--rw-r--r--   0        0        0        0 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/generic/__init__.py
--rw-r--r--   0        0        0      690 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/generic/generic.anthropic.prompt
--rw-r--r--   0        0        0      544 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/generic/generic.openai.prompt
--rw-r--r--   0        0        0      738 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/generic/generic.prompt
--rw-r--r--   0        0        0     1631 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/generic/generic.py
--rw-r--r--   0        0        0        0 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/translate/__init__.py
--rw-r--r--   0        0        0      632 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/translate/translate.anthropic.prompt
--rw-r--r--   0        0        0      611 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/translate/translate.openai.prompt
--rw-r--r--   0        0        0      688 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/translate/translate.prompt
--rw-r--r--   0        0        0     3138 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/translate/translate.py
--rw-r--r--   0        0        0      680 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/translate/util.py
--rw-r--r--   0        0        0      900 2024-04-30 09:46:16.008526 bpm_ai-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 bpm_ai-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0      726 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/common/__init__.py
+-rw-r--r--   0        0        0      195 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/common/errors.py
+-rw-r--r--   0        0        0     1961 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/common/multimodal.py
+-rw-r--r--   0        0        0        0 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/compose/__init__.py
+-rw-r--r--   0        0        0     1595 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/compose/compose.anthropic.prompt
+-rw-r--r--   0        0        0     1369 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/compose/compose.openai.prompt
+-rw-r--r--   0        0        0     1699 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/compose/compose.prompt
+-rw-r--r--   0        0        0     3644 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/compose/compose.py
+-rw-r--r--   0        0        0      950 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/compose/util.py
+-rw-r--r--   0        0        0        0 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/decide/__init__.py
+-rw-r--r--   0        0        0     8786 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/decide/decide.anthropic.prompt
+-rw-r--r--   0        0        0     8181 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/decide/decide.openai.prompt
+-rw-r--r--   0        0        0     8459 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/decide/decide.prompt
+-rw-r--r--   0        0        0     6247 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/decide/decide.py
+-rw-r--r--   0        0        0     3044 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/decide/schema.py
+-rw-r--r--   0        0        0        0 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/extract/__init__.py
+-rw-r--r--   0        0        0     1485 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/extract/extract.anthropic.prompt
+-rw-r--r--   0        0        0     1286 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/extract/extract.openai.prompt
+-rw-r--r--   0        0        0     1466 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/extract/extract.prompt
+-rw-r--r--   0        0        0     7565 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/extract/extract.py
+-rw-r--r--   0        0        0     2578 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/extract/util.py
+-rw-r--r--   0        0        0        0 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/generic/__init__.py
+-rw-r--r--   0        0        0      690 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/generic/generic.anthropic.prompt
+-rw-r--r--   0        0        0      544 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/generic/generic.openai.prompt
+-rw-r--r--   0        0        0      738 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/generic/generic.prompt
+-rw-r--r--   0        0        0     1631 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/generic/generic.py
+-rw-r--r--   0        0        0        0 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/translate/__init__.py
+-rw-r--r--   0        0        0      632 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/translate/translate.anthropic.prompt
+-rw-r--r--   0        0        0      611 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/translate/translate.openai.prompt
+-rw-r--r--   0        0        0      688 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/translate/translate.prompt
+-rw-r--r--   0        0        0     3164 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/translate/translate.py
+-rw-r--r--   0        0        0      680 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/translate/util.py
+-rw-r--r--   0        0        0      900 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 bpm_ai-1.7.2/PKG-INFO
```

### Comparing `bpm_ai-1.7.1/README.md` & `bpm_ai-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/common/multimodal.py` & `bpm_ai-1.7.2/bpm_ai/common/multimodal.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from bpm_ai_core.llm.common.blob import Blob
 from bpm_ai_core.ocr.ocr import OCR
 from bpm_ai_core.speech_recognition.asr import ASRModel
 from bpm_ai_core.util.file import is_supported_audio_file, is_file, is_supported_text_file
 from bpm_ai_core.util.file import is_supported_img_file
 
 from bpm_ai.common.errors import FileNotSupportedError
 
@@ -41,11 +42,19 @@
     return {
         k: f"[# blob {v} #]"
         if (isinstance(v, str) and is_supported_text_file(v))
         else v for k, v in input_data.items()
     }
 
 
+async def replace_text_blobs(input_data: dict):
+    return {
+        k: (await Blob.from_path_or_url(v).as_bytes()).decode("utf-8")
+        if (isinstance(v, str) and is_supported_text_file(v))
+        else v for k, v in input_data.items()
+    }
+
+
 def assert_all_files_processed(input_data: dict):
     for v in input_data.values():
         if v and isinstance(v, str) and is_file(v):
             raise FileNotSupportedError(v)
```

### Comparing `bpm_ai-1.7.1/bpm_ai/compose/compose.anthropic.prompt` & `bpm_ai-1.7.2/bpm_ai/compose/compose.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/compose/compose.openai.prompt` & `bpm_ai-1.7.2/bpm_ai/compose/compose.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/compose/compose.prompt` & `bpm_ai-1.7.2/bpm_ai/compose/compose.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/compose/compose.py` & `bpm_ai-1.7.2/bpm_ai/compose/compose.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/compose/util.py` & `bpm_ai-1.7.2/bpm_ai/compose/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/decide/decide.anthropic.prompt` & `bpm_ai-1.7.2/bpm_ai/decide/decide.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/decide/decide.openai.prompt` & `bpm_ai-1.7.2/bpm_ai/decide/decide.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/decide/decide.prompt` & `bpm_ai-1.7.2/bpm_ai/decide/decide.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/decide/decide.py` & `bpm_ai-1.7.2/bpm_ai/decide/decide.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from bpm_ai_core.text_classification.text_classifier import TextClassifier
 from bpm_ai_core.tracing.decorators import trace
 from bpm_ai_core.util.file import is_supported_img_file
 from bpm_ai_core.util.markdown import dict_to_md
 
 from bpm_ai.common.errors import MissingParameterError
 from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_documents, prepare_text_blobs, \
-    assert_all_files_processed
+    assert_all_files_processed, replace_text_blobs
 from bpm_ai.decide.schema import get_cot_decision_output_schema, get_decision_output_schema, remove_order_prefix_from_keys
 
 
 @trace("bpm-ai-decide", ["llm"])
 async def decide_llm(
     llm: LLM,
     input_data: dict[str, str | dict | None],
@@ -114,15 +114,15 @@
             hypothesis_template=hypothesis_template,
             confidence_threshold=0.1,
         )
 
     else:  # text classifier
         input_data = await ocr_documents(input_data, ocr)
         input_data = await transcribe_audio(input_data, asr)
-        input_data = prepare_text_blobs(input_data)
+        input_data = await replace_text_blobs(input_data)
         assert_all_files_processed(input_data)
 
         input_md = dict_to_md(input_data).strip()
 
         hypothesis_template = "In this example the question '" + question + "' should be answered with '{}'" \
             if question else "This example is {}."
```

### Comparing `bpm_ai-1.7.1/bpm_ai/decide/schema.py` & `bpm_ai-1.7.2/bpm_ai/decide/schema.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/extract/extract.anthropic.prompt` & `bpm_ai-1.7.2/bpm_ai/extract/extract.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/extract/extract.openai.prompt` & `bpm_ai-1.7.2/bpm_ai/extract/extract.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/extract/extract.prompt` & `bpm_ai-1.7.2/bpm_ai/extract/extract.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/extract/extract.py` & `bpm_ai-1.7.2/bpm_ai/extract/extract.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from bpm_ai_core.tracing.decorators import trace
 from bpm_ai_core.util.file import is_supported_img_file
 from bpm_ai_core.util.json_schema import expand_simplified_json_schema
 from bpm_ai_core.util.markdown import dict_to_md
 
 from bpm_ai.common.errors import MissingParameterError
 from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_documents, prepare_text_blobs, \
-    assert_all_files_processed
+    assert_all_files_processed, replace_text_blobs
 from bpm_ai.extract.util import merge_dicts, strip_non_numeric_chars, create_json_object
 
 
 @trace("bpm-ai-extract", ["llm"])
 async def extract_llm(
     llm: LLM,
     input_data: dict[str, str | dict | None],
@@ -90,15 +90,15 @@
 
     if vqa:
         input_img_data = {k: v for k, v in input_data.items() if (isinstance(v, str) and is_supported_img_file(v))}
         input_data = {k: v for k, v in input_data.items() if k not in input_img_data.keys()}
     else:
         input_data = await ocr_documents(input_data, ocr)
     input_data = await transcribe_audio(input_data, asr)
-    input_data = prepare_text_blobs(input_data)
+    input_data = await replace_text_blobs(input_data)
     assert_all_files_processed(input_data)
 
     if not output_schema:
         return input_data
 
     input_md = dict_to_md(input_data).strip()
     output_schema = expand_simplified_json_schema(output_schema)["properties"]
@@ -127,15 +127,15 @@
         qa_result = await model.answer(context, question, confidence_threshold=0.01 if not vqa else 0.1)
 
         if qa_result is None or qa_result.answer is None:
             return None
 
         if field_type == "integer":
             try:
-                return int(strip_non_numeric_chars(qa_result.answer))
+                return int(strip_non_numeric_chars(qa_result.answer))  # todo should also accept and round floats
             except ValueError:
                 return None
         elif field_type == "number":
             try:
                 return float(strip_non_numeric_chars(qa_result.answer))
             except ValueError:
                 return None
```

### Comparing `bpm_ai-1.7.1/bpm_ai/extract/util.py` & `bpm_ai-1.7.2/bpm_ai/extract/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/generic/generic.anthropic.prompt` & `bpm_ai-1.7.2/bpm_ai/generic/generic.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/generic/generic.openai.prompt` & `bpm_ai-1.7.2/bpm_ai/generic/generic.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/generic/generic.prompt` & `bpm_ai-1.7.2/bpm_ai/generic/generic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/generic/generic.py` & `bpm_ai-1.7.2/bpm_ai/generic/generic.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/translate/translate.anthropic.prompt` & `bpm_ai-1.7.2/bpm_ai/translate/translate.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/translate/translate.openai.prompt` & `bpm_ai-1.7.2/bpm_ai/translate/translate.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/translate/translate.prompt` & `bpm_ai-1.7.2/bpm_ai/translate/translate.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/bpm_ai/translate/translate.py` & `bpm_ai-1.7.2/bpm_ai/translate/translate.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from bpm_ai_core.prompt.prompt import Prompt
 from bpm_ai_core.speech_recognition.asr import ASRModel
 from bpm_ai_core.tracing.decorators import trace
 from bpm_ai_core.translation.nmt import NMTModel
 
 from bpm_ai.common.errors import MissingParameterError, LanguageNotFoundError
 from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_documents, prepare_text_blobs, \
-    assert_all_files_processed
+    assert_all_files_processed, replace_text_blobs
 from bpm_ai.translate.util import get_translation_output_schema, get_lang_code
 
 
 @trace("bpm-ai-translate", ["llm"])
 async def translate_llm(
         llm: LLM,
         input_data: dict[str, str | dict | None],
@@ -65,15 +65,15 @@
         return input_data
 
     if not target_language or target_language.isspace():
         raise MissingParameterError("target language is required")
 
     input_items = await ocr_documents(input_items, ocr)
     input_items = await transcribe_audio(input_items, asr)
-    input_data = prepare_text_blobs(input_data)
+    input_data = await replace_text_blobs(input_data)
     assert_all_files_processed(input_data)
 
     try:
         target_language_code = get_lang_code(target_language)
     except LookupError:
         raise LanguageNotFoundError(f"Could not identify target language '{target_language}'.")
```

### Comparing `bpm_ai-1.7.1/bpm_ai/translate/util.py` & `bpm_ai-1.7.2/bpm_ai/translate/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.1/pyproject.toml` & `bpm_ai-1.7.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpm-ai"
-version = "1.7.1"
+version = "1.7.2"
 description = "AI task automation for BPM engines."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai"
 homepage = "https://www.holisticon.de/"
 license = "Apache-2.0"
 readme = "README.md"
 
@@ -18,15 +18,15 @@
 aiobotocore = "^2.12.3"
 azure-storage-blob = "^12.19.1"
 azure-ai-translation-text = "^1.0.0b1"
 azure-ai-documentintelligence = "^1.0.0b2"
 av = "^11.0.0"
 
 [tool.poetry.group.dev.dependencies]
-bpm-ai-inference = "0.3.0"
+bpm-ai-inference = "0.3.3"
 ctranslate2 = "4.1.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.2"
 pytest-asyncio = "^0.23.5"
 pytest-dotenv = "^0.5.2"
```

### Comparing `bpm_ai-1.7.1/PKG-INFO` & `bpm_ai-1.7.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpm-ai
-Version: 1.7.1
+Version: 1.7.2
 Summary: AI task automation for BPM engines.
 Home-page: https://www.holisticon.de/
 License: Apache-2.0
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```


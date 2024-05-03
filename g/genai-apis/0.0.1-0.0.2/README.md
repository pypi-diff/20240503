# Comparing `tmp/genai_apis-0.0.1-py3-none-any.whl.zip` & `tmp/genai_apis-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7869 bytes, number of entries: 11
--rw-r--r--  2.0 unx       95 b- defN 24-May-03 04:29 genai_apis/__init__.py
+Zip file size: 8145 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       95 b- defN 24-May-03 05:23 genai_apis/__init__.py
 -rw-r--r--  2.0 unx      265 b- defN 24-May-03 04:28 genai_apis/abstract.py
--rw-r--r--  2.0 unx      532 b- defN 24-May-03 04:28 genai_apis/anthropic_api.py
--rw-r--r--  2.0 unx     1384 b- defN 24-May-03 04:28 genai_apis/factory.py
--rw-r--r--  2.0 unx      428 b- defN 24-May-03 04:28 genai_apis/gemini_api.py
+-rw-r--r--  2.0 unx      532 b- defN 24-May-03 05:23 genai_apis/anthropic_api.py
+-rw-r--r--  2.0 unx     2905 b- defN 24-May-03 05:23 genai_apis/factory.py
+-rw-r--r--  2.0 unx      813 b- defN 24-May-03 05:23 genai_apis/gemini_api.py
 -rw-r--r--  2.0 unx      542 b- defN 24-May-03 04:28 genai_apis/openai_api.py
--rw-r--r--  2.0 unx    11357 b- defN 24-May-03 04:32 genai_apis-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      734 b- defN 24-May-03 04:32 genai_apis-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-03 04:32 genai_apis-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-May-03 04:32 genai_apis-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      877 b- defN 24-May-03 04:32 genai_apis-0.0.1.dist-info/RECORD
-11 files, 16317 bytes uncompressed, 6383 bytes compressed:  60.9%
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-03 05:23 genai_apis-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1025 b- defN 24-May-03 05:23 genai_apis-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-03 05:23 genai_apis-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-03 05:23 genai_apis-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      878 b- defN 24-May-03 05:23 genai_apis-0.0.2.dist-info/RECORD
+11 files, 18515 bytes uncompressed, 6659 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: genai_apis/gemini_api.py
 Comment: 
 
 Filename: genai_apis/openai_api.py
 Comment: 
 
-Filename: genai_apis-0.0.1.dist-info/LICENSE
+Filename: genai_apis-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: genai_apis-0.0.1.dist-info/METADATA
+Filename: genai_apis-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: genai_apis-0.0.1.dist-info/WHEEL
+Filename: genai_apis-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: genai_apis-0.0.1.dist-info/top_level.txt
+Filename: genai_apis-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: genai_apis-0.0.1.dist-info/RECORD
+Filename: genai_apis-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genai_apis/__init__.py

```diff
@@ -1,5 +1,5 @@
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 from src.genai_apis.factory import APIFactory
 
 __all__ = ["APIFactory"]
```

## genai_apis/factory.py

```diff
@@ -1,9 +1,9 @@
 from .openai_api import OpenAIAPI
-from .gemini_api import GeminiAPI
+from .gemini_api import GeminiAPI, GeminiVertexAPI
 from .anthropic_api import AnthropicAPI
 
 
 class APIFactory:
     @staticmethod
     def get_api_client(api_name, **kwargs):
         if api_name == "openai":
@@ -21,18 +21,56 @@
 
                 genai.configure(api_key=kwargs["api_key"])
                 return GeminiAPI()
             except ImportError:
                 raise ImportError(
                     "Google GenerativeAI library is not installed. Please install the package before proceeding."
                 )
+        elif api_name == "gemini-vertex":
+            try:
+                import vertexai
+
+                vertexai.init(
+                    project=kwargs["GCP_PROJECT_ID"],
+                    location=kwargs["GCP_PROJECT_LOCATION"],
+                )
+                return GeminiVertexAPI()
+            except ImportError:
+                raise ImportError(
+                    "Google google-cloud-aiplatform library is not installed. Please install the package before proceeding."
+                )
         elif api_name == "anthropic":
             try:
                 from anthropic import AsyncAnthropic
 
                 return AnthropicAPI(AsyncAnthropic(api_key=kwargs["api_key"]))
             except ImportError:
                 raise ImportError(
                     "Anthropic library is not installed. Please install the package before proceeding."
                 )
+        elif api_name == "anthropic-vertex":
+            try:
+                from anthropic import AsyncAnthropicVertex
+
+                return AnthropicAPI(
+                    AsyncAnthropicVertex(
+                        project_id=kwargs["GCP_PROJECT_ID"],
+                        region=kwargs["GCP_PROJECT_LOCATION"],
+                    )
+                )
+            except ImportError:
+                raise ImportError(
+                    "Anthropic library is not installed. Please install the package before proceeding."
+                )
+        elif api_name == "anthropic-bedrock":
+            try:
+                from anthropic import AsyncAnthropicBedrock
+
+                return AnthropicAPI(
+                    AsyncAnthropicBedrock(aws_region=kwargs["AWS_REGION"])
+                )
+            except ImportError:
+                raise ImportError(
+                    "Anthropic library is not installed. Please install the package before proceeding."
+                )
         else:
             raise ValueError("Unsupported API")
```

## genai_apis/gemini_api.py

```diff
@@ -6,7 +6,16 @@
         import google.generativeai as genai
 
         model = genai.GenerativeModel(
             model_name=model, system_instruction=system_instruction
         )
         response = await model.generate_content_async([prompt], **kwargs)
         return response.text
+
+
+class GeminiVertexAPI(TextGenerationAPI):
+    async def generate_text(self, model, prompt, system_instruction=None, **kwargs):
+        from vertexai.generative_models import GenerativeModel
+
+        model = GenerativeModel(model_name=model, system_instruction=system_instruction)
+        response = await model.generate_content_async([prompt], **kwargs)
+        return response.text
```

## Comparing `genai_apis-0.0.1.dist-info/LICENSE` & `genai_apis-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `genai_apis-0.0.1.dist-info/METADATA` & `genai_apis-0.0.2.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 2.1
 Name: genai-apis
-Version: 0.0.1
+Version: 0.0.2
 Summary: GenAI APIs provides a unified API callers to Gemini API, OpenAI API, and Anthropic API.
 Home-page: https://github.com/deep-diver/genai-apis
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: genai
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asyncio
 Provides-Extra: anthropic
 Requires-Dist: anthropic ; extra == 'anthropic'
-Provides-Extra: google
-Requires-Dist: google-generativeai ; extra == 'google'
+Provides-Extra: anthropic-bedrock
+Requires-Dist: anthropic[bedrock] ; extra == 'anthropic-bedrock'
+Provides-Extra: anthropic-vertex
+Requires-Dist: anthropic[vertex] ; extra == 'anthropic-vertex'
+Provides-Extra: gemini
+Requires-Dist: google-generativeai ; extra == 'gemini'
+Provides-Extra: gemini-vertex
+Requires-Dist: google-cloud-aiplatform ; extra == 'gemini-vertex'
 Provides-Extra: openai
 Requires-Dist: openai ; extra == 'openai'
 
 # genai-apis
```

## Comparing `genai_apis-0.0.1.dist-info/RECORD` & `genai_apis-0.0.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-genai_apis/__init__.py,sha256=la1532jtOz3ZSCuNPTl7UX_B-VNSnuLp_qyHZ4pLMs4,95
+genai_apis/__init__.py,sha256=OYQBtvZT9Kt0CS6bXzpjczmQmR0iX6IjZHjySrC0xs0,95
 genai_apis/abstract.py,sha256=a54RxTFFfSWuoO2r8-rIjRpcXcD3LBmEchwPZNCzP7U,265
 genai_apis/anthropic_api.py,sha256=Bkm9tR9pbyNS_AEqLhy64Nu5BQDbMVPZvSwZLUnOxX4,532
-genai_apis/factory.py,sha256=6jAA76gFVd_XJIHJUBE2fUWshp57aHq2e-JqEv4cjW4,1384
-genai_apis/gemini_api.py,sha256=qjOPkbdESWwjBSgpvixe71cXyhRyyaFuWNMvHiCyMTw,428
+genai_apis/factory.py,sha256=sJgX-cUGVb5c-i7bYjofYAVbEVXqWVnFflURO5C9PIA,2905
+genai_apis/gemini_api.py,sha256=HOnUpKsf-axZ99hFAyZewJoBPyaYFQWEyPT9ijtsb0E,813
 genai_apis/openai_api.py,sha256=dEouN2rQjNQE8SJkortGA9bQcr6R0UyOYkQKKsBDGSQ,542
-genai_apis-0.0.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-genai_apis-0.0.1.dist-info/METADATA,sha256=WSjaB58FADrMJFv0KFdS-X1l2Z3iIO7NTyHkuxZdE9g,734
-genai_apis-0.0.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-genai_apis-0.0.1.dist-info/top_level.txt,sha256=lxy-j5IOQHvkO1zMVLruWLnxQapKtnD_0P9_F_z8cKc,11
-genai_apis-0.0.1.dist-info/RECORD,,
+genai_apis-0.0.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+genai_apis-0.0.2.dist-info/METADATA,sha256=mhDLvkEJ3UU_9sviLVfHWVhdh9EgJgR922S_7cNrvBw,1025
+genai_apis-0.0.2.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+genai_apis-0.0.2.dist-info/top_level.txt,sha256=lxy-j5IOQHvkO1zMVLruWLnxQapKtnD_0P9_F_z8cKc,11
+genai_apis-0.0.2.dist-info/RECORD,,
```


# Comparing `tmp/prometheus_eval-0.1.8.tar.gz` & `tmp/prometheus_eval-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus_eval-0.1.8.tar", max compression
+gzip compressed data, was "prometheus_eval-0.1.9.tar", max compression
```

## Comparing `prometheus_eval-0.1.8.tar` & `prometheus_eval-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-05-01 11:39:59.068594 prometheus_eval-0.1.8/README.md
--rw-r--r--   0        0        0      230 2024-05-01 13:51:32.126311 prometheus_eval-0.1.8/prometheus_eval/__init__.py
--rw-r--r--   0        0        0     9355 2024-05-01 14:42:02.809346 prometheus_eval-0.1.8/prometheus_eval/judge.py
--rw-r--r--   0        0        0     5786 2024-05-01 13:42:46.303450 prometheus_eval-0.1.8/prometheus_eval/prompts.py
--rw-r--r--   0        0        0     7448 2024-05-01 13:42:57.411514 prometheus_eval-0.1.8/prometheus_eval/utils.py
--rw-r--r--   0        0        0     2113 2024-05-01 14:52:44.731804 prometheus_eval-0.1.8/prometheus_eval/vllm.py
--rw-r--r--   0        0        0      595 2024-05-01 14:52:48.063817 prometheus_eval-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 prometheus_eval-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-01 11:39:59.068594 prometheus_eval-0.1.9/README.md
+-rw-r--r--   0        0        0      230 2024-05-02 13:38:22.456706 prometheus_eval-0.1.9/prometheus_eval/__init__.py
+-rw-r--r--   0        0        0     9668 2024-05-02 14:20:46.021529 prometheus_eval-0.1.9/prometheus_eval/judge.py
+-rw-r--r--   0        0        0     5786 2024-05-02 13:38:22.456706 prometheus_eval-0.1.9/prometheus_eval/prompts.py
+-rw-r--r--   0        0        0     7448 2024-05-02 13:38:22.456706 prometheus_eval-0.1.9/prometheus_eval/utils.py
+-rw-r--r--   0        0        0     2116 2024-05-02 14:12:09.224101 prometheus_eval-0.1.9/prometheus_eval/vllm.py
+-rw-r--r--   0        0        0      595 2024-05-02 14:22:21.013804 prometheus_eval-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 prometheus_eval-0.1.9/PKG-INFO
```

### Comparing `prometheus_eval-0.1.8/prometheus_eval/judge.py` & `prometheus_eval-0.1.9/prometheus_eval/judge.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def __init__(
         self,
         model_id: str = "prometheus-eval/prometheus-7b-v2.0",
         num_gpus: int = 1,
         download_dir: str = None,
         absolute_grade_template: str = ABSOLUTE_PROMPT_WO_REF,
         relative_grade_template: str = RELATIVE_PROMPT_WO_REF,
-        is_test: bool = False,
+        is_test: bool = False,  # For debugging purposes
         dtype: str = "auto",
         **kwargs,
     ):
         self.model_id = model_id
         self.num_gpus = num_gpus
         self.download_dir = download_dir
         if "###Reference Answer (Score 5):" not in absolute_grade_template:
@@ -40,15 +40,21 @@
             warnings.warn(
                 "Reference answer was not given in Relative Grading mode. This might lead to nonoptimal performances."
             )
 
         self.absolute_grade_template = absolute_grade_template
         self.relative_grade_template = relative_grade_template
         self.model = (
-            VLLM(model_id, num_gpus=num_gpus, download_dir=download_dir, dtype=dtype, **kwargs)
+            VLLM(
+                model_id,
+                num_gpus=num_gpus,
+                download_dir=download_dir,
+                dtype=dtype,
+                **kwargs,
+            )
             if not is_test
             else MockVLLM()
         )
 
     def _get_conversation_prompt(self, messages: List[Dict[str, str]]):
         """
         From filled prompt, convert it into llama-2 conversation prompt
@@ -62,204 +68,200 @@
                 conv.append_message(conv.roles[0], message["content"])
 
         conv.append_message(conv.roles[1], None)
         prompt = conv.get_prompt()
         return prompt
 
     def single_absolute_grade(
-        self, instruction: str, response: str, rubric: str, reference_answer: str | None
+        self,
+        instruction: str,
+        response: str,
+        rubric: str,
+        reference_answer: str = None,
+        params: Dict[str, Any] = {},
     ) -> Tuple[str, int]:
-        content = self.absolute_grade_template.format(
-            instruction=instruction,
-            response=response,
-            score_rubric=rubric_,
-            reference_answer=reference_answer,
-        )
-
-        messages = [
-            {"role": "user", "content": ABS_SYSTEM_PROMPT + "\n\n" + content},
-        ]
-        input_ = self.tokenizer.apply_chat_template(
-            messages, tokenize=False, add_generation_prompt=True
-        )
+        """
+        Grades a single response absolutely based on the provided instruction and response.
 
-        feedbacks, scores = batch_completions_with_retries(
-            self.model, [input_], mode="absolute", params=None
+        :param instruction: The instruction for the response.
+        :param response: The response to grade.
+        :param rubric: The rubric to use for grading.
+        :param reference_answer: Optional reference answer to aid in grading.
+        :param params: Additional parameters for the model completion requests.
+        :return: A tuple containing the feedback and score.
+        """
+        feedbacks, scores = self.absolute_grade(
+            instructions=[instruction],
+            responses=[response],
+            rubric=[rubric],
+            reference_answers=[reference_answer] if reference_answer else [None],
+            params=params,
         )
-
-        return feedbacks, scores
+        return feedbacks[0], scores[0]
 
     def single_relative_grade(
         self,
         instruction: str,
         response_A: str,
         response_B: str,
         rubric: str,
-        reference_answer: str | None,
+        reference_answers: Tuple[str, str] = (None, None),
+        params: Dict[str, Any] = {},
     ) -> Tuple[str, int]:
-        content = self.relative_grade_template.format(
-            instruction=instruction,
-            response_A=response_a,
-            response_B=response_b,
-            score_rubric=rubric_,
-            reference_answer=reference_answer,
-        )
-
-        messages = [
-            {"role": "user", "content": REL_SYSTEM_PROMPT + "\n\n" + content},
-        ]
-        input_ = self.tokenizer.apply_chat_template(
-            messages, tokenize=False, add_generation_prompt=True
-        )
+        """
+        Grades two responses relatively based on a single instruction.
 
-        feedbacks, scores = batch_completions_with_retries(
-            self.model, [inputs], mode="relative", params=None
+        :param instruction: The instruction for the paired responses.
+        :param response_A: First response to compare.
+        :param response_B: Second response to compare.
+        :param rubric: The rubric to use for grading.
+        :param reference_answers: Optional tuple of reference answers for each response.
+        :param params: Additional parameters for the model completion requests.
+        :return: A tuple containing the feedbacks and scores.
+        """
+        feedbacks, scores = self.relative_grade(
+            instructions=[instruction],
+            responses_A=[response_A],
+            responses_B=[response_B],
+            rubric=[rubric],
+            reference_answers=list(reference_answers),
+            params=params,
         )
-
-        return feedbacks, scores
+        return feedbacks[0], scores[0]
 
     def absolute_grade(
         self,
         *,
-        data: List[Dict[str, str]],
+        instructions: List[str],
+        responses: List[str],
         params: Dict[str, Any],
         rubric: List[str] | str,
-        reference_answers: List[str] = None
+        reference_answers: List[str] = None,
     ) -> Tuple[List[str], List[int]]:
         """
-        Grades a batch of responses absolutely based on the provided data.
+        Grades a batch of responses absolutely based on the provided instructions and responses.
 
-        :param data: A list of dictionaries, each containing 'instruction' and 'response'.
+        :param instructions: List of instructions corresponding to each response.
+        :param responses: List of responses to grade.
         :param params: Parameters for the model completion requests.
         :return: A tuple containing lists of feedbacks and scores.
         """
-        # Validate the input data format
-        for entry in data:
-            if (
-                not isinstance(entry, dict)
-                or "instruction" not in entry
-                or "response" not in entry
-            ):
-                raise ValueError(
-                    "Each entry in the data list must be a dictionary with 'instruction' and 'response' keys"
-                )
-
-        # If rubric is a list, assume its a entry-wise rubric
-        if isinstance(rubric, list):
-            if len(rubric) != len(data):
-                raise ValueError("Length of rubric must match the length of data")
-        else:
-            rubric = [rubric] * len(data)
+        if len(instructions) != len(responses):
+            raise ValueError(
+                "Length of instructions must match the length of responses"
+            )
 
-        # If reference answer is given, assume its a entry-wise reference answer
-        if isinstance(reference_answers, list):
-            if len(reference_answers) != len(data):
-                raise ValueError(
-                    "Length of reference_answers must match the length of data"
-                )
+        # If rubric is a list, check its length matches the length of instructions
+        if isinstance(rubric, list) and len(rubric) != len(instructions):
+            raise ValueError("Length of rubric must match the length of instructions")
         else:
-            reference_answers = [None] * len(data)
+            rubric = [rubric] * len(
+                instructions
+            )  # Apply the same rubric to all if it's not a list
+
+        # Handle reference answers
+        if isinstance(reference_answers, list) and len(reference_answers) != len(
+            instructions
+        ):
+            raise ValueError(
+                "Length of reference answers must match the length of instructions"
+            )
+        else:
+            reference_answers = [None] * len(
+                instructions
+            )  # Default to None if not provided
 
         inputs = []
-        for idx, entry in enumerate(data):
-            instruction = entry["instruction"]
-            response = entry["response"]
+        for idx, (instruction, response) in enumerate(zip(instructions, responses)):
             rubric_ = rubric[idx]
             reference_answer = reference_answers[idx]
-
             content = self.absolute_grade_template.format(
                 instruction=instruction,
                 response=response,
                 rubric=rubric_,
                 reference_answer=reference_answer,
             )
-
             messages = [
                 {"role": "system", "content": ABS_SYSTEM_PROMPT},
                 {"role": "user", "content": content},
             ]
             input_ = self._get_conversation_prompt(messages)
             inputs.append(input_)
 
-        # TODO: Ensure no parsing errors by running the batch_absolute_grade in the last run
         feedbacks, scores = batch_completions_with_retries(
             self.model,
             inputs,
             mode="absolute",
             params=params,
         )
 
         return feedbacks, scores
 
     def relative_grade(
         self,
         *,
-        data: List[Dict[str, str]],
+        instructions: List[str],
+        responses_A: List[str],
+        responses_B: List[str],
         params: Dict[str, Any],
         rubric: List[str] | str,
-        reference_answers: List[str] = None
+        reference_answers: List[str] = None,
     ) -> Tuple[List[str], List[int]]:
         """
-        Grades a batch of responses relatively based on the provided data.
+        Grades a batch of responses relatively based on the provided instructions and paired responses.
 
-        :param data: A list of dictionaries, each containing 'instruction', 'response_A', and 'response_B'.
+        :param instructions: List of instructions for each paired responses.
+        :param responses_A: List of first responses in each pair.
+        :param responses_B: List of second responses in each pair.
         :param params: Additional parameters for the model completion requests.
         :return: A tuple containing lists of feedbacks and scores.
         """
-        # Validate the input data format
-        for entry in data:
-            if (
-                not isinstance(entry, dict)
-                or "instruction" not in entry
-                or "response_A" not in entry
-                or "response_B" not in entry
-            ):
-                raise ValueError(
-                    "Each entry in the data list must be a dictionary with 'instruction', 'response_A', and 'response_B' keys"
-                )
-
-        # If rubric is a list, assume its a entry-wise rubric
-        if isinstance(rubric, list):
-            if len(rubric) != len(data):
-                raise ValueError("Length of rubric must match the length of data")
+        if len(instructions) != len(responses_A) or len(responses_A) != len(
+            responses_B
+        ):
+            raise ValueError(
+                "Length of instructions, responses_A, and responses_B must all match"
+            )
+
+        # Handle rubric and reference answers similar to absolute_grade
+        if isinstance(rubric, list) and len(rubric) != len(instructions):
+            raise ValueError("Length of rubric must match the length of instructions")
         else:
-            rubric = [rubric] * len(data)
+            rubric = [rubric] * len(instructions)
 
-        # If reference answer is given, assume its a entry-wise reference answer
-        if isinstance(reference_answers, list):
-            if len(reference_answers) != len(data):
-                raise ValueError(
-                    "Length of reference_answers must match the length of data"
-                )
+        if isinstance(reference_answers, list) and len(reference_answers) != len(
+            instructions
+        ):
+            raise ValueError(
+                "Length of reference answers must match the length of instructions"
+            )
         else:
-            reference_answers = [None] * len(data)
+            reference_answers = [None] * len(instructions)
 
         inputs = []
-        for idx, entry in enumerate(data):
-            instruction = entry["instruction"]
-            response_a = entry["response_A"]
-            response_b = entry["response_B"]
+        for idx, (instruction, response_a, response_b) in enumerate(
+            zip(instructions, responses_A, responses_B)
+        ):
             rubric_ = rubric[idx]
             reference_answer = reference_answers[idx]
-
-            # Formatting the input for the relative grading
             content = self.relative_grade_template.format(
                 instruction=instruction,
                 response_A=response_a,
                 response_B=response_b,
                 rubric=rubric_,
                 reference_answer=reference_answer,
             )
-
             messages = [
                 {"role": "system", "content": REL_SYSTEM_PROMPT},
                 {"role": "user", "content": content},
             ]
             input_ = self._get_conversation_prompt(messages)
             inputs.append(input_)
 
-        # TODO: Ensure no parsing errors by running the batch_absolute_grade in the last run
         feedbacks, scores = batch_completions_with_retries(
-            self.model, inputs, mode="relative", params=params
+            self.model,
+            inputs,
+            mode="relative",
+            params=params,
         )
 
         return feedbacks, scores
```

### Comparing `prometheus_eval-0.1.8/prometheus_eval/prompts.py` & `prometheus_eval-0.1.9/prometheus_eval/prompts.py`

 * *Files identical despite different names*

### Comparing `prometheus_eval-0.1.8/prometheus_eval/utils.py` & `prometheus_eval-0.1.9/prometheus_eval/utils.py`

 * *Files identical despite different names*

### Comparing `prometheus_eval-0.1.8/prometheus_eval/vllm.py` & `prometheus_eval-0.1.9/prometheus_eval/vllm.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,35 +17,35 @@
 
         self.model: LLM = LLM(
             model=self.name,
             tensor_parallel_size=num_gpus,
             dtype=dtype,
             gpu_memory_utilization=gpu_memory_utilization,
             download_dir=download_dir,
-            **kwargs
+            **kwargs,
         )
 
     def completions(
         self,
         prompts: List[str],
         use_tqdm: bool = False,
-        **kwargs: Union[int, float, str]
+        **kwargs: Union[int, float, str],
     ) -> List[str]:
         prompts = [prompt.strip() for prompt in prompts]
         params = SamplingParams(**kwargs)
 
         outputs = self.model.generate(prompts, params, use_tqdm=use_tqdm)
         outputs = [output.outputs[0].text for output in outputs]
         return outputs
 
     def generate(
         self,
         prompts: List[str],
         use_tqdm: bool = False,
-        **kwargs: Union[int, float, str]
+        **kwargs: Union[int, float, str],
     ) -> List[str]:
         params = SamplingParams(**kwargs)
         return self.model.generate(prompts, params, use_tqdm=use_tqdm)
 
 
 class MockVLLM:
     def __init__(
```

### Comparing `prometheus_eval-0.1.8/pyproject.toml` & `prometheus_eval-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prometheus-eval"
-version = "0.1.8"
+version = "0.1.9"
 description = "A package for evaluating the performance of language models with Prometheus"
 authors = ["Juyoung Suk <juyoung@kaist.ac.kr>", "Seungone Kim <seungone@cmu.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 vllm = "<0.4.0"
```

### Comparing `prometheus_eval-0.1.8/PKG-INFO` & `prometheus_eval-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-eval
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package for evaluating the performance of language models with Prometheus
 Author: Juyoung Suk
 Author-email: juyoung@kaist.ac.kr
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


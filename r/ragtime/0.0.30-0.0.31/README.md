# Comparing `tmp/ragtime-0.0.30.tar.gz` & `tmp/ragtime-0.0.31.tar.gz`

## Comparing `ragtime-0.0.30.tar` & `ragtime-0.0.31.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 ragtime-0.0.30/CHANGELOG.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 ragtime-0.0.30/CONTRIBUTING.md
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ragtime-0.0.30/deploy/deploy.py
--rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 ragtime-0.0.30/img/Ragtime_logo.png
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ragtime-0.0.30/src/ragtime/__init__.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 ragtime-0.0.30/src/ragtime/api.py
--rw-r--r--   0        0        0     8839 2020-02-02 00:00:00.000000 ragtime-0.0.30/src/ragtime/config.py
--rw-r--r--   0        0        0    19134 2020-02-02 00:00:00.000000 ragtime-0.0.30/src/ragtime/expe.py
--rw-r--r--   0        0        0    38999 2020-02-02 00:00:00.000000 ragtime-0.0.30/src/ragtime/generators.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ragtime-0.0.30/src/ragtime/base_folder/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragtime-0.0.30/src/ragtime/base_folder/LICENSE
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ragtime-0.0.30/src/ragtime/base_folder/README.md
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 ragtime-0.0.30/src/ragtime/base_folder/classes.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 ragtime-0.0.30/src/ragtime/base_folder/main.py
--rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 ragtime-0.0.30/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 ragtime-0.0.30/src/ragtime/base_folder/res/html_templates/basic_template.jinja
--rw-r--r--   0        0        0    91060 2020-02-02 00:00:00.000000 ragtime-0.0.30/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx
--rw-r--r--   0        0        0    31095 2020-02-02 00:00:00.000000 ragtime-0.0.30/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx
--rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 ragtime-0.0.30/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx
--rw-r--r--   0        0        0    33387 2020-02-02 00:00:00.000000 ragtime-0.0.30/src/ragtime/base_folder/res/spreadsheet_templates/spreadsheet_rich_template.xlsx
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 ragtime-0.0.30/tests/full_test.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 ragtime-0.0.30/tests/run_tests.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragtime-0.0.30/tests/test_quest.json
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ragtime-0.0.30/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 ragtime-0.0.30/LICENSE
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 ragtime-0.0.30/README.md
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 ragtime-0.0.30/pyproject.toml
--rw-r--r--   0        0        0     7067 2020-02-02 00:00:00.000000 ragtime-0.0.30/PKG-INFO
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 ragtime-0.0.31/CHANGELOG.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 ragtime-0.0.31/CONTRIBUTING.md
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ragtime-0.0.31/deploy/deploy.py
+-rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 ragtime-0.0.31/img/Ragtime_logo.png
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/__init__.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/api.py
+-rw-r--r--   0        0        0     8840 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/config.py
+-rw-r--r--   0        0        0    20347 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/expe.py
+-rw-r--r--   0        0        0    39001 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/generators.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/LICENSE
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/README.md
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/classes.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/main.py
+-rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/res/html_templates/basic_template.jinja
+-rw-r--r--   0        0        0    91060 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx
+-rw-r--r--   0        0        0    31095 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx
+-rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx
+-rw-r--r--   0        0        0    33387 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/res/spreadsheet_templates/spreadsheet_rich_template.xlsx
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 ragtime-0.0.31/tests/full_test.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 ragtime-0.0.31/tests/run_tests.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragtime-0.0.31/tests/test_quest.json
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ragtime-0.0.31/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 ragtime-0.0.31/LICENSE
+-rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 ragtime-0.0.31/README.md
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 ragtime-0.0.31/pyproject.toml
+-rw-r--r--   0        0        0     7184 2020-02-02 00:00:00.000000 ragtime-0.0.31/PKG-INFO
```

### Comparing `ragtime-0.0.30/CONTRIBUTING.md` & `ragtime-0.0.31/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.30/img/Ragtime_logo.png` & `ragtime-0.0.31/img/Ragtime_logo.png`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.30/src/ragtime/__init__.py` & `ragtime-0.0.31/src/ragtime/__init__.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.30/src/ragtime/api.py` & `ragtime-0.0.31/src/ragtime/api.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.30/src/ragtime/config.py` & `ragtime-0.0.31/src/ragtime/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,16 +78,16 @@
     DEFAULT_HTML_TEMPLATE = FOLDER_HTML_TEMPLATES / 'basic_template.jinja'
     # # # Spreadheet
     DEFAULT_SPREADSHEET_TEMPLATE = FOLDER_SST_TEMPLATES / 'basic_template.xlsx'
     DEFAULT_WORKSHEET = "Expe"
     DEFAULT_HEADER_SIZE = 2
     DEFAULT_QUESTION_COL = 2
     DEFAULT_FACTS_COL = 4
-    DEFAULT_ANSWERS_COL = 9
-    DEFAULT_HUMAN_EVAL_COL = 15
+    DEFAULT_ANSWERS_COL = 11
+    DEFAULT_HUMAN_EVAL_COL = 25
     # # # LLMs
     DEFAULT_LITELLM_RETRIES = 3
     DEFAULT_LITELLM_TEMP = 0
 
     ####################
     # LOGGING
     # You can choose the file where the logs are written in "log_conf" dict, key "handlers"/"file"/"filename" - default is "logs/logs.txt"
```

### Comparing `ragtime-0.0.30/src/ragtime/expe.py` & `ragtime-0.0.31/src/ragtime/expe.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import defaultdict
-from enum import Enum
+from enum import Enum, IntEnum
 import json
 from pathlib import Path
 import re
 import shutil
 from openpyxl import load_workbook, Workbook
 from openpyxl.worksheet.worksheet import Worksheet
 from copy import copy
@@ -130,14 +130,18 @@
                 except:
                     b_return_None = True
             if b_return_None:
                 return None
 
         return result
 
+class UpdateTypes(IntEnum):
+    human_eval = 0
+    facts = 1
+
 class Expe(RagtimeList[QA]):
     meta:Optional[dict] = {}
     json_path:Path = Field(None, exclude=True)
 
     def __init__(self, json_path:Path=None):
         super().__init__()
         if json_path:
@@ -159,15 +163,21 @@
     def get_name(self) -> str:
         """Returns the name of the Expe based on the number of questions, answers..."""
         date_to_time_format:str = "%Y-%m-%d_%Hh%M,%S"
         stats:dict = self.stats()
         name:str = f'{stats["questions"]}Q_{stats["chunks"]}C_{stats["facts"]}F_{stats["models"]}M_{stats["answers"]}A_{stats["human eval"]}HE_{stats["auto eval"]}AE_{datetime.now().strftime(date_to_time_format)}'
         return name
 
-    def _file_check_before_writing(self, path:Path, b_overwrite:bool=False, b_add_suffix:bool = True, force_ext:str=None) -> Path:
+    def _file_check_before_writing(self, path:Path=None, b_overwrite:bool=False, b_add_suffix:bool = True, force_ext:str=None) -> Path:
+        if not path:
+            if self.json_path:
+                path = Path(self.json_path.parent) / self.json_path.stem
+            else:
+                raise RagtimeException(f'Cannot save since no json_path is stored in expe and no path has been provided')        
+
         # Make sure at least 1 QA is here
         if len(self) == 0:
             raise Exception("""The Expe object you're trying to write is empty! Please add at least one QA""")
         
         # Check and prepare the destination file path
         if not(path):
             raise Exception("""No file defined - please specify a file name to save the Expe into""")
@@ -220,90 +230,97 @@
             if 'meta' in data:
                 self.meta = data['meta']
                 qa_list = data['items']
             for json_qa in qa_list:
                 qa:QA = QA(**json_qa)
                 self.append(qa)
    
-    def update_from_spreadsheet(self, path:Path, sheet_name:str = DEFAULT_WORKSHEET,
-                                question_col:int=DEFAULT_QUESTION_COL,
-                                facts_col:int=DEFAULT_FACTS_COL,
-                                answers_col:int=DEFAULT_ANSWERS_COL,
-                                human_eval_col:int=DEFAULT_HUMAN_EVAL_COL):
-        # Load Human Evaluations from a Spreadsheet
-        # Assumes a spreadhseet formatted like "spreadsheet_multi_rows_template.xlsx", so:
-        # Question column is B
-        # Facts column is D
-        # LLM name column is J
-        # Human eval column is O
-        def find_row(ws:Worksheet, row:int, column:int, val_to_find:str):
-            return next((r+1 for r in range(row, ws.max_row) if ws.cell(row=r+1, column=column).value.lower() == val_to_find.lower()), None)
-        
-        def find_next(ws:Worksheet, row:int, column:int):
-            return next((r+1 for r in range(row, ws.max_row) if ws.cell(row=r+1, column=column).value), None)
+    def update_from_spreadsheet(self, path:Path, update_type:UpdateTypes, data_col:int=None, 
+                                question_col:int = DEFAULT_QUESTION_COL-1, answer_col:int = DEFAULT_ANSWERS_COL-1,
+                                sheet_name:str = DEFAULT_WORKSHEET, header_size:int=DEFAULT_HEADER_SIZE):
+        """Updates data from a spreadsheet, e.g. human evaluation or facts
+        Args:
+        - data_col (int): indicates the column number (starts at 0) from where the data will be imported in the spreadsheet
+        if None (default), default column values are used, i.e. DEFAULT_FACTS_COL if update_type==Facts and
+        DEFAULT_HUMAN_EVAL_COL if update_type==human_eval
+        - update_type (UpdateTypes): can be "human_eval" or "facts"
+        - question_col (int): indicates the column number (starts at 0) where the questions are - default: DEFAULT_QUESTION_COL-1 (0 based)
+        - answer_col (in): used if update_type==human_eval, since the eval entered in the spreadsheet has to be matched with a specific answer
+        """
+        def starts_with_num(fact:str) -> bool:
+            result:bool = False
+            if "." in fact:
+                try:
+                    dummy:int = int(fact[:fact.find('.')])
+                    result = True
+                except (TypeError, ValueError): pass
+            return result
+
 
         wb:Workbook = load_workbook(path)
         ws:Worksheet = wb[sheet_name]
-
-        # For each question in the current Expe object
-        for qa in self:
-            # find the corresponding question in the spreadsheet
-            q_row:int = find_row(ws=ws, row=1, column=question_col, val_to_find=qa.question.text)
-            if q_row:
-                # update human evaluations
-                for ans in qa.answers:
-                    ans_row:int = find_row(ws=ws, row=q_row, column=answers_col, val_to_find=ans.text)
-                    if ans_row:
-                        human_eval:int = int(ws.cell(row=ans_row, column=human_eval_col).value)
-                        ans.eval.human = human_eval
-                # update facts list 
+        cur_qa:QA = None
+        if not data_col:
+            data_cols:dict = {UpdateTypes.facts: DEFAULT_FACTS_COL, UpdateTypes.human_eval: DEFAULT_HUMAN_EVAL_COL}
+            data_col = data_cols[update_type]-1
+
+        new_facts:Facts = Facts() # the new facts to replace the old ones in the current QA
+
+        # For each row in the worksheet
+        for i, row in enumerate(ws.iter_rows(min_row=header_size+1), start=1):
+            if row[question_col].value: # a question is in the current row, so a new question starts
+                if cur_qa: # not first question
+                    cur_qa.facts = new_facts
+                cur_qa = next((qa for qa in self if qa.question.text.lower() == row[question_col].value.lower()), None) # get the corresponding QA in the Expe
                 new_facts:Facts = Facts()
-                for fact in qa.facts:
-                    fact_row:int = find_row(ws=ws, row=q_row, column=facts_col, val_to_find=fact.text)
-                    if fact_row: # fact still exists -> keep it
-                        new_facts.append(fact)
-                qa.facts = new_facts
-                # add facts added in the spreadsheet
-                next_q_row:int = find_next(ws=ws, row=q_row, column=question_col)
-                if not next_q_row: next_q_row = ws.max_row
-                fact_list:list[str] = [f.text.lower() for f in qa.facts]
-                for r in range(q_row, next_q_row):
-                    fact_text:str = ws.cell(row=r, column=facts_col).value
-                    if fact_text.lower() not in fact_list:
-                        qa.facts.append(Fact(text=fact_text))
+            
+            if cur_qa: # QA and question in the worksheet is made
+                data_in_ws = row[data_col].value
+                if data_in_ws:
+                    if update_type == UpdateTypes.facts: # Update FACTS
+                        if not starts_with_num(data_in_ws): # if the fact in the ws does not start with a number, add it
+                            data_in_ws = f'{len(new_facts) + 1}. {data_in_ws}'
+                        new_facts.append(Fact(text=data_in_ws))
+                    elif update_type == UpdateTypes.human_eval: # Update HUMAN EVAL
+                        answer_text:str = row[answer_col].value
+                        cur_ans:Answer = next((a for a in cur_qa.answers if a.text == answer_text), None)
+                        if cur_ans: # corresponding Answer has been found
+                            try:
+                                human_eval:int = int(data_in_ws)
+                            except (TypeError, ValueError):
+                                logger.warn(f'Human eval should be a value between 0 and 1 - cannot use "{data_in_ws}" as found in line {i}')
+                            cur_ans.eval.human = human_eval
+                        else:
+                            logger.warn(f'Cannot find Answer corresponding with the human eval "{data_in_ws}" - Answer should contain the text "{answer_text}"')
+                        
 
     def save_to_json(self, path:Path=None, b_overwrite:bool=False, b_add_suffix:bool = True) -> Path:
         """Saves Expe to JSON - can generate a suffix for the filename
         Returns the Path of the file actually saved"""
-        if not path:
-            if self.json_path:
-                path = Path(self.json_path.parent) / self.json_path.stem
-            else:
-                raise RagtimeException(f'Cannot save to JSON since no json_path is stored in expe and not path has been provided in argument.')        
         path:Path = self._file_check_before_writing(path, b_overwrite=b_overwrite, 
                                                     b_add_suffix=b_add_suffix, force_ext='.json')
         with open(path, mode='w', encoding='utf-8') as file:
             file.write(self.model_dump_json(indent=2))
         logger.info(f'Expe saved as JSON to {path}')
         return path
 
-    def save_to_html(self, path:Path, render_params:dict[str,bool]=DEFAULT_HTML_RENDERING,
+    def save_to_html(self, path:Path=None, render_params:dict[str,bool]=DEFAULT_HTML_RENDERING,
                      template_path:Path=DEFAULT_HTML_TEMPLATE, b_overwrite:bool=False, b_add_suffix:bool = True):
         """Saves Expe to an HTML file from a Jinja template - can generate a suffix for the filename
         Returns the Path of the file actually saved"""
         path:Path = self._file_check_before_writing(path, b_overwrite=b_overwrite, b_add_suffix=b_add_suffix, force_ext='.html')
         environment = Environment(loader=FileSystemLoader(searchpath=template_path.parent,encoding='utf-8'))
         template = environment.get_template(template_path.name)
         context = {"expe": self, **render_params, "report_name": self.get_name(), "sub": (lambda pattern, repl, s: re.sub(pattern, repl, s))}
         with open(path, mode='w', encoding='utf-8') as file:
             file.write(template.render(context))
         logger.info(f'Expe saved as HTML to {path}')
         return path
 
-    def save_to_spreadsheet(self, path:Path, template_path:Path=DEFAULT_SPREADSHEET_TEMPLATE,
+    def save_to_spreadsheet(self, path:Path=None, template_path:Path=DEFAULT_SPREADSHEET_TEMPLATE,
                             header_size:int=DEFAULT_HEADER_SIZE, sheet_name:str = DEFAULT_WORKSHEET,
                             b_overwrite:bool=False, b_add_suffix:bool = True):
         """Saves Expe to a spreadsheet - can generate a suffix for the filename
         Returns the Path of the file actually saved"""
         path:Path = self._file_check_before_writing(path, b_overwrite=b_overwrite, b_add_suffix=b_add_suffix, force_ext='.xlsx')
         
         # Prepare the result file
@@ -332,15 +349,16 @@
                 # get the first non empty value in the required column
                 val = next((qa.get_attr(p) for qa in self if qa.get_attr(p)), "")
                 ws.cell(row=row, column=cell.column, value=val)
 
         qa:QA
         row:int = header_size+1
         col_with_formulas:dict[int, str] = {c: ws.cell(column=c, row=row).value
-                                            for c in range(1, ws.max_column) if ws.cell(column=c, row=row).value[0] == "="}
+                                            for c in range(1, ws.max_column) 
+                                            if ws.cell(column=c, row=row).value and str(ws.cell(column=c, row=row).value)[0] == "="}
         for num_q, qa in enumerate(self, start=1): # write each row in expe
             next_row:int = 0
             for col, p in enumerate(ws_conf, start=1):
                 if p == "#": # special token # used to indicate question number
                     val = [num_q]
                 elif p[0] == "=": # if a formula is here, write it as is in the formula field
                     continue
```

### Comparing `ragtime-0.0.30/src/ragtime/generators.py` & `ragtime-0.0.31/src/ragtime/generators.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,28 +46,28 @@
     def get_prompt(self) -> Prompt:
         raise NotImplementedError('Must implement this!')
 
     @abstractmethod
     def post_process(self, qa:QA, cur_obj:WithLLMAnswer) -> WithLLMAnswer:
         raise NotImplementedError('Must implement this!')
 
-class PptrBase(Prompter):
+class PptrBaseAns(Prompter):
     """This simple prompter just send the question as is to the LLM
     and does not perform any post-processing"""
     def get_prompt(self, question:Question, chunks:Optional[Chunks] = None) -> Prompt:
         result:Prompt = Prompt()
         result.user = f'{question.text}'
         result.system = ""
         return result
     
     def post_process(self, qa:QA=None, cur_obj:Answer=None):
         """Does not do anything by default, but can be overridden to add fields in meta data for instance"""
         cur_obj.text = cur_obj.llm_answer.text
 
-class PptrRichAnsFR(Prompter):
+class PptrRAGAnsFR(Prompter):
     """This prompter uses a prompt asking the LLM to generate a JSON structure
     and includes chunks in its prompt. It performs post-processing to exploit
     the JSON structure the LLM is supposed to generate."""
     FLD_QUEST_OK:str = "q_ok"
     FLD_CHUNKS_OK:str = "chunks_ok"
     FLD_ANSWER:str = "answer"
```

### Comparing `ragtime-0.0.30/src/ragtime/base_folder/.gitignore` & `ragtime-0.0.31/src/ragtime/base_folder/.gitignore`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.30/src/ragtime/base_folder/LICENSE` & `ragtime-0.0.31/src/ragtime/base_folder/LICENSE`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.30/src/ragtime/base_folder/classes.py` & `ragtime-0.0.31/src/ragtime/base_folder/classes.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.30/src/ragtime/base_folder/main.py` & `ragtime-0.0.31/src/ragtime/base_folder/main.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.30/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx` & `ragtime-0.0.31/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.30/src/ragtime/base_folder/res/html_templates/basic_template.jinja` & `ragtime-0.0.31/src/ragtime/base_folder/res/html_templates/basic_template.jinja`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.30/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx` & `ragtime-0.0.31/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.30/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx` & `ragtime-0.0.31/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.30/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx` & `ragtime-0.0.31/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.30/src/ragtime/base_folder/res/spreadsheet_templates/spreadsheet_rich_template.xlsx` & `ragtime-0.0.31/src/ragtime/base_folder/res/spreadsheet_templates/spreadsheet_rich_template.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.30/tests/full_test.py` & `ragtime-0.0.31/tests/full_test.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.30/tests/run_tests.py` & `ragtime-0.0.31/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.30/tests/test_quest.json` & `ragtime-0.0.31/tests/test_quest.json`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.30/.gitignore` & `ragtime-0.0.31/.gitignore`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.30/LICENSE` & `ragtime-0.0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.30/README.md` & `ragtime-0.0.31/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 In Ragtime 🎹, a *RAG* is made of, optionally, a *Retriever*, and always, one or several *Large Language Model* (*LLM*).
 - A *Retriever* takes a *question* in input and returns one or several *chunks* or *paragraphs* retrieved from a documents knowledge base
 - A *LLM* is a text to text generator taking in input a *prompt*, made of a question and optional chunks, and returning an *LLMAnswer*
 
 You can specify how *prompts* are generated and how the *LLMAnswer* has to be post-processed to return an *answer*.
 
 # How does it work?
-The main idea in Ragtime 🎹 is to evaluate answers returned by a RAG based on **Facts** that you define. Indeed, it is very difficult to evaluate RAGs and/or LLMs because you cannot define a "good" answer. Indeed a LLM can return many equialent answers expressed in different ways, making impossible a simple string comparison to determine whether an answer is right or wrong. Even though many proxies have been created, counting the number of common words like in ROUGE for instance is not very precise.
+The main idea in Ragtime 🎹 is to evaluate answers returned by a RAG based on **Facts** that you define. Indeed, it is very difficult to evaluate RAGs and/or LLMs because you cannot define a "good" answer. A LLM can return many equivalent answers expressed in different ways, making impossible a simple string comparison to determine whether an answer is right or wrong. Even though many proxies have been created, counting the number of common words like in ROUGE for instance is not very precise (see [HuggingFace's `lighteval`](https://github.com/huggingface/lighteval?tab=readme-ov-file#metrics-for-generative-tasks))
 
 In Ragtime 🎹, answers returned by a RAG or a LLM are evaluated against a set of facts. If the answer validates all the facts, then the answer is deemed correct. Conversely, if some facts are not validated, the answer is considered wrong. The number of validated facts compared to the total number of facts to validate defines a score.
 
 You can either define facts manually, or have a LLM define them for you. **The evaluation of facts against answers is done automatically with another LLM**.
 
 # Main objects
 The main objects used in Ragtime 🎹 are:
```

### Comparing `ragtime-0.0.30/pyproject.toml` & `ragtime-0.0.31/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ragtime"
-version = "0.0.30"
+version = "0.0.31"
 
 authors = [
   { name="Gilles Moyse", email="gilles@recital.ai" },
 ]
 maintainers = [
   { name="reciTAL", email="ragtime@recital.ai" },
 ]
```

### Comparing `ragtime-0.0.30/PKG-INFO` & `ragtime-0.0.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragtime
-Version: 0.0.30
+Version: 0.0.31
 Summary: Ragtime 🎹 is an LLMOps framework to automatically evaluate Retrieval Augmented Generation (RAG) systems and compare different RAGs / LLMs
 Project-URL: Homepage, https://github.com/recitalAI/ragtime-package
 Project-URL: Issues, https://github.com/recitalAI/ragtime-package/issues
 Author-email: Gilles Moyse <gilles@recital.ai>
 Maintainer-email: reciTAL <ragtime@recital.ai>
 License: MIT License
         
@@ -60,15 +60,15 @@
 In Ragtime 🎹, a *RAG* is made of, optionally, a *Retriever*, and always, one or several *Large Language Model* (*LLM*).
 - A *Retriever* takes a *question* in input and returns one or several *chunks* or *paragraphs* retrieved from a documents knowledge base
 - A *LLM* is a text to text generator taking in input a *prompt*, made of a question and optional chunks, and returning an *LLMAnswer*
 
 You can specify how *prompts* are generated and how the *LLMAnswer* has to be post-processed to return an *answer*.
 
 # How does it work?
-The main idea in Ragtime 🎹 is to evaluate answers returned by a RAG based on **Facts** that you define. Indeed, it is very difficult to evaluate RAGs and/or LLMs because you cannot define a "good" answer. Indeed a LLM can return many equialent answers expressed in different ways, making impossible a simple string comparison to determine whether an answer is right or wrong. Even though many proxies have been created, counting the number of common words like in ROUGE for instance is not very precise.
+The main idea in Ragtime 🎹 is to evaluate answers returned by a RAG based on **Facts** that you define. Indeed, it is very difficult to evaluate RAGs and/or LLMs because you cannot define a "good" answer. A LLM can return many equivalent answers expressed in different ways, making impossible a simple string comparison to determine whether an answer is right or wrong. Even though many proxies have been created, counting the number of common words like in ROUGE for instance is not very precise (see [HuggingFace's `lighteval`](https://github.com/huggingface/lighteval?tab=readme-ov-file#metrics-for-generative-tasks))
 
 In Ragtime 🎹, answers returned by a RAG or a LLM are evaluated against a set of facts. If the answer validates all the facts, then the answer is deemed correct. Conversely, if some facts are not validated, the answer is considered wrong. The number of validated facts compared to the total number of facts to validate defines a score.
 
 You can either define facts manually, or have a LLM define them for you. **The evaluation of facts against answers is done automatically with another LLM**.
 
 # Main objects
 The main objects used in Ragtime 🎹 are:
```


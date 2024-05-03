# Comparing `tmp/text_lloom-0.7.2.tar.gz` & `tmp/text_lloom-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_lloom-0.7.2.tar", max compression
+gzip compressed data, was "text_lloom-0.7.3.tar", max compression
```

## Comparing `text_lloom-0.7.2.tar` & `text_lloom-0.7.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       39 2024-02-02 13:27:07.282735 text_lloom-0.7.2/README.md
--rw-r--r--   0        0        0      546 2024-04-26 11:54:39.443185 text_lloom-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     2019 2024-04-16 10:45:54.173463 text_lloom-0.7.2/src/text_lloom/__init__.py
--rw-r--r--   0        0        0      738 2024-02-28 09:09:42.891236 text_lloom-0.7.2/src/text_lloom/concept.py
--rw-r--r--   0        0        0    58656 2024-04-26 11:32:12.086284 text_lloom-0.7.2/src/text_lloom/concept_induction.py
--rw-r--r--   0        0        0     8216 2024-04-26 11:49:39.075606 text_lloom-0.7.2/src/text_lloom/llm.py
--rw-r--r--   0        0        0     8416 2024-04-13 23:28:08.093682 text_lloom-0.7.2/src/text_lloom/prompts.py
--rw-r--r--   0        0        0     1263 2024-04-15 01:19:42.816858 text_lloom-0.7.2/src/text_lloom/static/index.css
--rw-r--r--   0        0        0   455935 2024-04-15 01:19:42.816860 text_lloom-0.7.2/src/text_lloom/static/index.js
--rw-r--r--   0        0        0      707 2024-04-15 01:19:38.799003 text_lloom-0.7.2/src/text_lloom/static/index_select.css
--rw-r--r--   0        0        0    11241 2024-04-15 01:19:38.799013 text_lloom-0.7.2/src/text_lloom/static/index_select.js
--rw-r--r--   0        0        0    30201 2024-04-26 11:47:07.423672 text_lloom-0.7.2/src/text_lloom/workbench.py
--rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 text_lloom-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-02-02 13:27:07.282735 text_lloom-0.7.3/README.md
+-rw-r--r--   0        0        0      546 2024-05-03 06:10:31.780251 text_lloom-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     2019 2024-05-02 04:55:04.265643 text_lloom-0.7.3/src/text_lloom/__init__.py
+-rw-r--r--   0        0        0      805 2024-05-02 04:59:53.695827 text_lloom-0.7.3/src/text_lloom/concept.py
+-rw-r--r--   0        0        0    59691 2024-05-03 05:48:19.215334 text_lloom-0.7.3/src/text_lloom/concept_induction.py
+-rw-r--r--   0        0        0     8216 2024-05-02 04:55:04.668679 text_lloom-0.7.3/src/text_lloom/llm.py
+-rw-r--r--   0        0        0     8911 2024-05-03 05:35:05.419656 text_lloom-0.7.3/src/text_lloom/prompts.py
+-rw-r--r--   0        0        0     1263 2024-04-15 01:19:42.816858 text_lloom-0.7.3/src/text_lloom/static/index.css
+-rw-r--r--   0        0        0   455935 2024-04-15 01:19:42.816860 text_lloom-0.7.3/src/text_lloom/static/index.js
+-rw-r--r--   0        0        0      707 2024-04-15 01:19:38.799003 text_lloom-0.7.3/src/text_lloom/static/index_select.css
+-rw-r--r--   0        0        0    11241 2024-04-15 01:19:38.799013 text_lloom-0.7.3/src/text_lloom/static/index_select.js
+-rw-r--r--   0        0        0    32809 2024-05-03 06:05:16.532556 text_lloom-0.7.3/src/text_lloom/workbench.py
+-rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 text_lloom-0.7.3/PKG-INFO
```

### Comparing `text_lloom-0.7.2/pyproject.toml` & `text_lloom-0.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "text_lloom"
-version = "0.7.2"
+version = "0.7.3"
 description = "Concept Induction to analyze unstructured text"
 authors = ["Michelle Lam <mlam4@cs.stanford.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 hdbscan = "^0.8.33"
```

### Comparing `text_lloom-0.7.2/src/text_lloom/__init__.py` & `text_lloom-0.7.3/src/text_lloom/__init__.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.7.2/src/text_lloom/concept_induction.py` & `text_lloom-0.7.3/src/text_lloom/concept_induction.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     from .prompts import *
     from .concept import Concept
     from .__init__ import MatrixWidget, ConceptSelectWidget
 
 # CONSTANTS ================================
 NAN_SCORE = 0  # Numerical score to use in place of NaN values for matrix viz
 OUTLIER_CRITERIA = "Did the example not match any of the above concepts?"
-SCORE_DF_OUT_COLS = ["doc_id", "text", "concept_id", "concept_name", "concept_prompt", "score", "rationale", "highlight"]
+SCORE_DF_OUT_COLS = ["doc_id", "text", "concept_id", "concept_name", "concept_prompt", "score", "rationale", "highlight", "concept_seed"]
 
 
 # HELPER functions ================================
 
 def json_load(s, top_level_key=None):
     # Attempts to safely load a JSON from a string response from the LLM
     if s is None:
@@ -123,16 +123,16 @@
         sess.time[k] = elapsed
 
 def calc_cost(results, model_name, step_name, sess, debug=False):
     # Calculate cost with API results and model name
     if results is None:
         return
     # Cost estimation
-    in_tokens = np.sum([res.usage.prompt_tokens for res in results])
-    out_tokens = np.sum([res.usage.completion_tokens for res in results])
+    in_tokens = np.sum([(res.usage.prompt_tokens) if res is not None else 0 for res in results])
+    out_tokens = np.sum([(res.usage.completion_tokens) if res is not None else 0 for res in results])
     in_token_cost, out_token_cost = calc_cost_by_tokens(model_name, in_tokens, out_tokens)
     total_cost = in_token_cost + out_token_cost
     if debug:
         print(f"\nTotal: {total_cost} | In: {in_token_cost} | Out: {out_token_cost}")
     if sess is not None:
         # Save to session if provided
         sess.tokens["in_tokens"].append(in_tokens)
@@ -147,15 +147,15 @@
 
 # CORE functions ================================
 
 # Input: 
 # - text_df: DataFrame (columns: doc_id, doc)
 # Parameters: model_name, n_quotes, seed
 # Output: quote_df (columns: doc_id, quote)
-async def distill_filter(text_df, doc_col, doc_id_col, model_name, n_quotes=3, seed=None, sess=None):
+async def distill_filter(text_df, doc_col, doc_id_col, model_name, n_quotes=3, prompt_template=None, seed=None, sess=None):
     # Filtering operates on provided text
     start = time.time()
 
     # Filter to non-empty rows
     text_df = filter_empty_rows(text_df, doc_col)
 
     # Prepare prompts
@@ -170,15 +170,16 @@
             "ex": ex, 
             "n_quotes": n_quotes, 
             "seeding_phrase": seeding_phrase.upper()
         } for ex in text_df[doc_col].tolist()
     ]
     
     # Run prompts
-    prompt_template = filter_prompt
+    if prompt_template is None:
+        prompt_template = filter_prompt
     if sess is not None:
         rate_limits = sess.rate_limits
     else:
         rate_limits = None
     res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name, rate_limits=rate_limits)
 
     # Process results
@@ -195,15 +196,15 @@
     return quote_df
 
 
 # Input: text_df (columns: doc_id, doc) 
 #   --> text could be original or filtered (quotes)
 # Parameters: n_bullets, n_words_per_bullet, seed
 # Output: bullet_df (columns: doc_id, bullet)
-async def distill_summarize(text_df, doc_col, doc_id_col, model_name, n_bullets="2-4", n_words_per_bullet="5-8", seed=None, sess=None):
+async def distill_summarize(text_df, doc_col, doc_id_col, model_name, n_bullets="2-4", n_words_per_bullet="5-8", prompt_template=None, seed=None, sess=None):
     # Summarization operates on text_col
     start = time.time()
 
     # Filter to non-empty rows
     text_df = filter_empty_rows(text_df, doc_col)
 
     # Prepare prompts
@@ -228,15 +229,17 @@
             "n_bullets": n_bullets, 
             "n_words": n_words_per_bullet
         }
         arg_dicts.append(arg_dict)
         all_ex_ids.append(ex_id)
     
     # Run prompts
-    prompt_template = summarize_prompt
+    if prompt_template is None:
+        prompt_template = summarize_prompt
+        
     if sess is not None:
         rate_limits = sess.rate_limits
     else:
         rate_limits = None
     res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name, rate_limits=rate_limits)
 
     # Process results
@@ -297,15 +300,15 @@
     return examples_json
 
 # Input: cluster_df (columns: doc_id, doc, cluster_id)
 # Parameters: n_concepts
 # Output: 
 # - concepts: dict (concept_id -> concept dict)
 # - concept_df: DataFrame (columns: doc_id, doc, concept_id, concept_name, concept_prompt)
-async def synthesize(cluster_df, doc_col, doc_id_col, model_name, cluster_id_col="cluster_id", concept_col_prefix="concept", n_concepts=None, batch_size=None, verbose=False, pattern_phrase="unifying pattern", dedupe=True, seed=None, sess=None, return_logs=False):
+async def synthesize(cluster_df, doc_col, doc_id_col, model_name, cluster_id_col="cluster_id", concept_col_prefix="concept", n_concepts=None, batch_size=None, verbose=False, pattern_phrase="unifying pattern", dedupe=True, prompt_template=None, seed=None, sess=None, return_logs=False):
     # Synthesis operates on "doc" column for each cluster_id
     # Concept object is created for each concept
     start = time.time()
     
     # Filter to non-empty rows
     cluster_df = filter_empty_rows(cluster_df, doc_col)
 
@@ -319,17 +322,19 @@
             return f"up to {cur_n_concepts} {pattern_phrase}s"
         else:
             return f"{cur_n_concepts} {pattern_phrase}"
     
     # Prepare prompts
     # Create prompt arg dictionary with example IDs
     if seed is not None:
-        seed_phrase = f"If possible, please make the patterns RELATED TO {seed.upper()}."
+        seeding_phrase = f"If possible, please make the patterns RELATED TO {seed.upper()}."
     else:
-        seed_phrase = ""
+        seeding_phrase = ""
+
+    seed_label = seed
     arg_dicts = []
     cluster_ids = cluster_df[cluster_id_col].unique()
     cluster_dfs = {}  # Store each cluster's dataframe by cluster_id
     ex_id_to_ex = {(str(row[doc_id_col]), row[cluster_id_col]): row[doc_col] for _, row in cluster_df.iterrows()}  # Map example IDs to example text
     for cluster_id in cluster_ids:
         # Iterate over cluster IDs to get example sets
         cur_df = cluster_df[cluster_df[cluster_id_col] == cluster_id]
@@ -340,30 +345,31 @@
             for i in range(n_batches):
                 cur_batch_df = cur_df.iloc[i*batch_size:(i+1)*batch_size]
                 ex_dicts = [{"example_id": row[doc_id_col], "example": row[doc_col]} for _, row in cur_batch_df.iterrows()]
                 ex_dicts_json = dict_to_json(ex_dicts)
                 arg_dict = {
                     "examples": ex_dicts_json,
                     "n_concepts_phrase": get_n_concepts_phrase(cur_df),
-                    "seed_phrase": seed_phrase
+                    "seeding_phrase": seeding_phrase
                 }
                 arg_dicts.append(arg_dict)
         else:
             # Handle unbatched case
             ex_dicts = [{"example_id": row[doc_id_col], "example": row[doc_col]} for _, row in cur_df.iterrows()]
             ex_dicts_json = dict_to_json(ex_dicts)
             arg_dict = {
                 "examples": ex_dicts_json,
                 "n_concepts_phrase": get_n_concepts_phrase(cur_df),
-                "seed_phrase": seed_phrase
+                "seeding_phrase": seeding_phrase
             }
             arg_dicts.append(arg_dict)
 
     # Run prompts
-    prompt_template = synthesize_prompt
+    if prompt_template is None:
+        prompt_template = synthesize_prompt
     if sess is not None:
         rate_limits = sess.rate_limits
     else:
         rate_limits = None
     res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name, rate_limits=rate_limits)
 
     # Process results
@@ -377,32 +383,33 @@
                 ex_ids = concept_dict["example_ids"]
                 ex_ids = set(ex_ids) # remove duplicates
                 concept = Concept(
                     name=concept_dict["name"],
                     prompt=concept_dict["prompt"],
                     example_ids=ex_ids,
                     active=False,
+                    seed=seed_label
                 )
                 concepts[concept.id] = concept
                 
                 for ex_id in ex_ids:
                     # doc_id, text, concept_id, concept_name, concept_prompt
                     cur_key = (ex_id, cur_cluster_id)
                     if cur_key in ex_id_to_ex:
-                        row = [ex_id, ex_id_to_ex[cur_key], concept.id, concept.name, concept.prompt]
+                        row = [ex_id, ex_id_to_ex[cur_key], concept.id, concept.name, concept.prompt, concept.seed]
                         rows.append(row)
             # Print intermediate results
             examples = cluster_dfs[cur_cluster_id][doc_col].tolist()
             concepts_formatted = pretty_print_dict_list(cur_concepts)
             cur_log = f"\n\nInput examples: {examples}\nOutput concepts: {concepts_formatted}"
             logs += cur_log
             if verbose:
                 print(cur_log)
     # doc_id, text, concept_id, concept_name, concept_prompt
-    concept_df = pd.DataFrame(rows, columns=[doc_id_col, doc_col, concept_col_prefix, f"{concept_col_prefix}_name", f"{concept_col_prefix}_prompt"])
+    concept_df = pd.DataFrame(rows, columns=[doc_id_col, doc_col, concept_col_prefix, f"{concept_col_prefix}_name", f"{concept_col_prefix}_prompt", "seed"])
 
     concept_df[f"{concept_col_prefix}_namePrompt"] = concept_df[f"{concept_col_prefix}_name"] + ": " + concept_df[f"{concept_col_prefix}_prompt"]
     if dedupe:
         concept_df = dedupe_concepts(concept_df, concept_col=f"{concept_col_prefix}_namePrompt")
 
     save_progress(sess, concept_df, step_name="Synthesize", start=start, res=res_full, model_name=model_name)
     # Save to session if provided
@@ -469,15 +476,15 @@
     concepts = concepts.copy()  # Make a copy of the concepts dict to avoid modifying the original
     start = time.time()
     concept_name_col = f"{concept_col_prefix}_name"
 
     concepts_list = [f"- Name: {c.name}, Prompt: {c.prompt}" for c in concepts.values()]
     concepts_list_str = "\n".join(concepts_list)
     arg_dicts = [{
-        "themes": concepts_list_str,
+        "concepts": concepts_list_str,
     }]
 
     # Run prompts
     prompt_template = review_remove_prompt
     if sess is not None:
         rate_limits = sess.rate_limits
     else:
@@ -521,15 +528,15 @@
     concept_col = concept_col_prefix
     concept_name_col = f"{concept_col_prefix}_name"
     concept_prompt_col = f"{concept_col_prefix}_prompt"
 
     concepts_list = [f"- Name: {c.name}, Prompt: {c.prompt}" for c in concepts.values()]
     concepts_list_str = "\n".join(concepts_list)
     arg_dicts = [{
-        "themes": concepts_list_str,
+        "concepts": concepts_list_str,
     }]
 
     # Run prompts
     prompt_template = review_merge_prompt
     if sess is not None:
         rate_limits = sess.rate_limits
     else:
@@ -593,15 +600,15 @@
 # Input: concepts (concept_id -> Concept)
 # Parameters: max_concepts, model_name
 # Output: selected_concepts: dict (concept_id -> Concept)
 async def review_select(concepts, max_concepts, model_name, rate_limits=None):
     concepts_list = [f"- Name: {c.name}, Prompt: {c.prompt}" for c in concepts.values()]
     concepts_list_str = "\n".join(concepts_list)
     arg_dicts = [{
-        "themes": concepts_list_str,
+        "concepts": concepts_list_str,
         "max_concepts": max_concepts,
     }]
 
     # Run prompts
     prompt_template = review_select_prompt
     res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name, rate_limits=rate_limits)
 
@@ -620,16 +627,16 @@
 
 
 def get_ex_batch_args(df, text_col, doc_id_col, concept_name, concept_prompt):
     ex = get_examples_dict(df, text_col, doc_id_col)
     examples_json = dict_to_json(ex)
     arg_dict = {
         "examples_json": examples_json,
-        "pattern_name": concept_name,
-        "pattern_prompt": concept_prompt,
+        "concept_name": concept_name,
+        "concept_prompt": concept_prompt,
         "example_ids": list(df[doc_id_col])
     }
     return arg_dict
 
 def get_examples_dict(cur_df, text_col, doc_id_col):
     # Helper to get examples from cur_df in dictionary form for JSON in prompt
     ex_list = []
@@ -659,14 +666,15 @@
     return answer_scores[x]
 
 def get_score_df(res, in_df, concept, concept_id, text_col, doc_id_col, get_highlights):
     # Cols: doc_id, text, concept_id, concept_name, concept_prompt, score, highlight
     res_dict = json_load(res, top_level_key="pattern_results")
     concept_name = concept.name
     concept_prompt = concept.prompt
+    concept_seed = concept.seed
     if res_dict is not None:
         rows = []
         for ex in res_dict:
             if "answer" in ex:
                 ans = parse_bucketed_score(ex["answer"])
             else:
                 ans = NAN_SCORE
@@ -680,38 +688,40 @@
 
                     if "rationale" in ex:
                         rationale = ex["rationale"]
                     else:
                         rationale = ""   # Set rationale to empty string
 
                     if get_highlights and ("quote" in ex):
-                        row = [doc_id, text, concept_id, concept_name, concept_prompt, ans, rationale, ex["quote"]]
+                        row = [doc_id, text, concept_id, concept_name, concept_prompt, ans, rationale, ex["quote"], concept_seed]
                     else:
-                        row = [doc_id, text, concept_id, concept_name, concept_prompt, ans, rationale, ""]  # Set quote to empty string
+                        row = [doc_id, text, concept_id, concept_name, concept_prompt, ans, rationale, "", concept_seed]  # Set quote to empty string
                     rows.append(row)
         
         out_df = pd.DataFrame(rows, columns=SCORE_DF_OUT_COLS)
         return out_df
     else:
         out_df = get_empty_score_df(in_df, concept, concept_id, text_col, doc_id_col)
         return out_df[SCORE_DF_OUT_COLS]
 
 def get_empty_score_df(in_df, concept, concept_id, text_col, doc_id_col):
     # Cols: doc_id, text, concept_id, concept_name, concept_prompt, score, highlight
     concept_name = concept.name
     concept_prompt = concept.prompt
+    concept_seed = concept.seed
     out_df = in_df.copy()
     out_df["doc_id"] = out_df[doc_id_col]
     out_df["text"] = out_df[text_col]
     out_df["concept_id"] = concept_id
     out_df["concept_name"] = concept_name
     out_df["concept_prompt"] = concept_prompt
     out_df["score"] = NAN_SCORE
     out_df["rationale"] = ""
     out_df["highlight"] = ""
+    out_df["concept_seed"] = concept.seed
     return out_df[SCORE_DF_OUT_COLS]
 
 # Performs scoring for one concept
 async def score_helper(concept, batch_i, concept_id, df, text_col, doc_id_col, model_name, batch_size, get_highlights, sess, threshold):
     # TODO: add support for only a sample of examples
     # TODO: set consistent concept IDs for reference
 
@@ -882,15 +892,15 @@
     return doc_ids
 
 # Returns ids of covered-by-generic documents
 def get_covered_by_generic(score_df, doc_id_col, threshold=1.0, generic_threshold=0.5, debug=False):
     # Determines generic concepts
     df = score_df.copy()
     df["score"] = df["score"].apply(lambda x: 1 if x >= threshold else 0)
-    df_generic = df.groupby("concept_id").mean().reset_index()
+    df_generic = df.groupby("concept_id")['score'].mean().reset_index()
     df_generic.rename(columns={"score": "pos_frac"}, inplace=True)
     df_generic = df_generic[df_generic["pos_frac"] >= generic_threshold]
     generic_concepts = df_generic["concept_id"].unique().tolist()
     if debug:
         display(df_generic)
         print(generic_concepts)
 
@@ -911,15 +921,14 @@
 def loop(score_df, doc_col, doc_id_col, debug=False):
     # Check for not-covered and covered-by-generic documents
     # Not-covered: examples that don't match any concepts
     # Covered-by-generic: examples that only match generic concepts (those which cover the majority of examples)
     # TODO: Allow users to decide on custom filtering conditions
     # TODO: Save generic concepts to session (to avoid later)
     n_initial = len(score_df[doc_id_col].unique())
-
     underrep_ids = get_not_covered(score_df, doc_id_col)
     generic_ids = get_covered_by_generic(score_df, doc_id_col)
     ids_to_include = underrep_ids + generic_ids
     ids_to_include = set(ids_to_include)
     if debug:
         print(f"ids_to_include ({len(ids_to_include)}): {ids_to_include}")
 
@@ -928,15 +937,14 @@
 
     # Stopping condition: if text_df is empty or has the same number of docs as the original df
     n_final = len(text_df[doc_id_col].unique())
     if (n_final == n_initial) or (len(text_df) == 0):
         return None
     return text_df
 
-
 def trace():
     # Input: concept_df (columns: doc_id, text, concept_id, ...), text_dfs (columns: doc_id, text)
     # Output: trace_df (columns: doc_id, text, concept_id, score, text1, text2)
 
     # Joins the score_df with other text dfs that share the same doc_id column
     # To trace from the final concepts and scores to the original text
     pass
@@ -1438,7 +1446,24 @@
     if new_ex_ids is not None:
         cur_concept["example_ids"] = new_ex_ids
         # TODO: differentiate between replacing and appending example IDs
     concepts[concept_id] = cur_concept
 
     # TODO: handle concept_df
     return concepts
+
+async def check_concept_seed(concepts, seed, model_name="gpt-3.5-turbo"):
+    concepts_prompts_str = str(concepts)
+    seed_str = str(seed)
+    arg_dicts = [
+        {
+            "concepts": concepts_prompts_str,
+            "seed": seed_str,
+        }
+    ]
+
+    # Run prompts
+    prompt_template = match_concept_prompt
+    res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name)
+    res = res_text[0]
+    concepts_to_remove = json_load(res, top_level_key="remove")
+    return concepts_to_remove
```

### Comparing `text_lloom-0.7.2/src/text_lloom/llm.py` & `text_lloom-0.7.3/src/text_lloom/llm.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.7.2/src/text_lloom/prompts.py` & `text_lloom-0.7.3/src/text_lloom/prompts.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,27 +22,27 @@
 """
 
 # Synthesize ========================
 synthesize_prompt = """
 I have this set of bullet point summaries of text examples:
 {examples}
 
-Please write a summary of {n_concepts_phrase} for these examples {seed_phrase} For each high-level pattern, write a 2-4 word NAME for the pattern and an associated 1-sentence ChatGPT PROMPT that could take in a new text example and determine whether the relevant pattern applies. Also include 1-2 example_ids for items that BEST exemplify the pattern. Please respond ONLY with a valid JSON in the following format:
+Please write a summary of {n_concepts_phrase} for these examples. {seeding_phrase} For each high-level pattern, write a 2-4 word NAME for the pattern and an associated 1-sentence ChatGPT PROMPT that could take in a new text example and determine whether the relevant pattern applies. Also include 1-2 example_ids for items that BEST exemplify the pattern. Please respond ONLY with a valid JSON in the following format:
 {{
     "patterns": [ 
         {{"name": "<PATTERN_NAME_1>", "prompt": "<PATTERN_PROMPT_1>", "example_ids": ["<EXAMPLE_ID_1>", "<EXAMPLE_ID_2>"]}},
         {{"name": "<PATTERN_NAME_2>", "prompt": "<PATTERN_PROMPT_2>", "example_ids": ["<EXAMPLE_ID_1>", "<EXAMPLE_ID_2>"]}},
     ]
 }}
 """
 
 # Review ========================
 review_remove_prompt = """
 I have this set of themes generated from text examples:
-{themes}
+{concepts}
 
 Please identify any themes that should be REMOVED because they are either:
 (1) Too specific/narrow and would only describe a few examples, or 
 (2) Too generic/broad and would describe nearly all examples.
 If there no such themes, please leave the list empty.
 Please respond ONLY with a valid JSON in the following format:
 
@@ -52,15 +52,15 @@
         "<THEME_NAME_6>",
     ]
 }}
 """
 
 review_merge_prompt = """
 I have this set of themes generated from text examples:
-{themes}
+{concepts}
 
 Please identify any PAIRS of themes that are similar or overlapping that should be MERGED together. 
 Please respond ONLY with a valid JSON in the following format with the original themes and a new name and prompt for the merged theme. Do NOT simply combine the prior theme names or prompts, but come up with a new 2-3 word name and 1-sentence ChatGPT prompt. If there no similar themes, please leave the list empty.
 
 {{
     "merge": [ 
         {{
@@ -75,15 +75,15 @@
         }}
     ]
 }}
 """
 
 review_select_prompt = """
 I have this set of themes generated from text examples:
-{themes}
+{concepts}
 
 Please select AT MOST {max_concepts} themes to include in the final set of themes. These themes should be the highest quality themes in the set: (1) NOT too generic or vague (should not describe most examples), (2) NOT too specific (should not only describe a small set of examples), and (3) NOT overlapping with other selected themes (they should capture a range of different patterns).
 Please respond ONLY with a valid JSON in the following format:
 
 {{
     "selected": [ 
         "<THEME_NAME_1>",
@@ -94,16 +94,16 @@
 
 # Score ========================
 score_no_highlight_prompt = """
 CONTEXT: 
     I have the following text examples in a JSON:
     {examples_json}
 
-    I also have a pattern named {pattern_name} with the following PROMPT: 
-    {pattern_prompt}
+    I also have a pattern named {concept_name} with the following PROMPT: 
+    {concept_prompt}
 
 TASK:
     For each example, please evaluate the PROMPT by generating a 1-sentence RATIONALE of your thought process and providing a resulting ANSWER of ONE of the following multiple-choice options, including just the letter: 
     - A: Strongly agree
     - B: Agree
     - C: Neither agree nor disagree
     - D: Disagree
@@ -121,16 +121,16 @@
 """
 
 score_highlight_prompt = """
 CONTEXT: 
     I have the following text examples in a JSON:
     {examples_json}
 
-    I also have a pattern named {pattern_name} with the following PROMPT: 
-    {pattern_prompt}
+    I also have a pattern named {concept_name} with the following PROMPT: 
+    {concept_prompt}
 
 TASK:
     For each example, please evaluate the PROMPT by generating a 1-sentence RATIONALE of your thought process and providing a resulting ANSWER of ONE of the following multiple-choice options, including just the letter: 
     - A: Strongly agree
     - B: Agree
     - C: Neither agree nor disagree
     - D: Disagree
@@ -216,7 +216,26 @@
             "concept_id": "<concept_id_number>",
             "item_id": "<item_id_number or NONE>",
             "rationale": "<rationale for match>",
         }}
     ]
 }}
 """
+
+# Match Concept ========================
+match_concept_prompt = """
+I have this dict of CONCEPTS (keys) and their corresponding inclusion criteria (values), as follows:
+{concepts}
+
+I have the following theme:
+{seed}
+
+Please identify any CONCEPTS that do not match the THEME. If there no such concepts, please leave the list empty.
+Please respond ONLY with a valid JSON in the following format:
+
+{{
+    "remove": [ 
+        "<CONCEPT_NAME_5>",
+        "<CONCEPT_NAME_6>",
+    ]
+}}
+"""
```

### Comparing `text_lloom-0.7.2/src/text_lloom/static/index.css` & `text_lloom-0.7.3/src/text_lloom/static/index.css`

 * *Files identical despite different names*

### Comparing `text_lloom-0.7.2/src/text_lloom/static/index.js` & `text_lloom-0.7.3/src/text_lloom/static/index.js`

 * *Files identical despite different names*

### Comparing `text_lloom-0.7.2/src/text_lloom/static/index_select.css` & `text_lloom-0.7.3/src/text_lloom/static/index_select.css`

 * *Files identical despite different names*

### Comparing `text_lloom-0.7.2/src/text_lloom/static/index_select.js` & `text_lloom-0.7.3/src/text_lloom/static/index_select.js`

 * *Files identical despite different names*

### Comparing `text_lloom-0.7.2/src/text_lloom/workbench.py` & `text_lloom-0.7.3/src/text_lloom/workbench.py`

 * *Files 8% similar despite different names*

```diff
@@ -294,74 +294,119 @@
         print(f"\n\n{self.bold_txt('Tokens')}: total={total_tokens}, in={in_tokens}, out={out_tokens}")
 
     def show_selected(self):
         active_concepts = self.__get_active_concepts()
         print(f"\n\n{self.bold_txt('Active concepts')} (n={len(active_concepts)}):")
         for c_id, c in active_concepts.items():
             print(f"- {self.bold_txt(c.name)}: {c.prompt}")
+    
+    def show_prompt(self, step_name):
+        # Displays the default prompt for the specified step.
+        steps_to_prompts = {
+            "distill_filter": filter_prompt,
+            "distill_summarize": summarize_prompt,
+            "synthesize": synthesize_prompt,
+        }
+        if step_name in steps_to_prompts:
+            return steps_to_prompts[step_name]
+        else:
+            raise Exception(f"Operator `{step_name}` not found. The available operators for custom prompts are: {list(steps_to_prompts.keys())}")
+    
+    def validate_prompt(self, step_name, prompt):
+        # Validate prompt for a given step to ensure that it includes the necessary template fields.
+        # Raises an exception if any required field is missing.
+        prompt_reqs = {
+            "distill_filter": ["ex", "n_quotes", "seeding_phrase"],
+            "distill_summarize": ["ex", "n_bullets", "seeding_phrase", "n_words"],
+            "synthesize": ["examples", "n_concepts_phrase", "seeding_phrase"],
+        }
+        reqs = prompt_reqs[step_name]
+        for req in reqs:
+            template_str = f"{{{req}}}"  # Check for {req} in the prompt
+            if template_str not in prompt:
+                raise Exception(f"Custom prompt for `{step_name}` is missing required template field: `{req}`. All required fields: {reqs}. For example, this is the default prompt template:\n{self.show_prompt(step_name)}")
+        
 
     # HELPER FUNCTIONS ================================
-    async def gen(self, seed=None, params=None, n_synth=1, auto_review=True, debug=True):
+    async def gen(self, seed=None, params=None, n_synth=1, custom_prompts=None, auto_review=True, debug=True):
         if params is None:
             params = self.auto_suggest_parameters(debug=debug)
             if debug:
                 print(f"{self.bold_txt('Auto-suggested parameters')}: {params}")
+        if custom_prompts is None:
+            # Use default prompts
+            custom_prompts = {
+                "distill_filter": self.show_prompt("distill_filter"),
+                "distill_summarize": self.show_prompt("distill_summarize"),
+                "synthesize": self.show_prompt("synthesize"),
+            }
+        else:
+            # Validate that prompts are formatted correctly
+            for step_name, prompt in custom_prompts.items():
+                if prompt is not None:
+                    self.validate_prompt(step_name, prompt)
         
         # Run cost estimation
         self.estimate_gen_cost(params)
         
         # Confirm to proceed
         print(f"\n\n{self.bold_highlight_txt('Action required')}")
         user_input = input("Proceed with generation? (y/n): ")
         if user_input.lower() != "y":
             print("Cancelled generation")
             return
 
         # Run concept generation
         filter_n_quotes = params["filter_n_quotes"]
-        if filter_n_quotes > 1:
+        if (filter_n_quotes > 1) and (custom_prompts["distill_filter"] is not None):
             step_name = "Distill-filter"
             self.print_step_name(step_name)
             with self.spinner_wrapper() as spinner:
                 df_filtered = await distill_filter(
                     text_df=self.in_df, 
                     doc_col=self.doc_col,
                     doc_id_col=self.doc_id_col,
                     model_name=self.distill_model_name,
                     n_quotes=params["filter_n_quotes"],
+                    prompt_template=custom_prompts["distill_filter"],
                     seed=seed,
                     sess=self,
                 )
                 self.df_to_score = df_filtered  # Change to use filtered df for concept scoring
                 self.df_filtered = df_filtered
                 spinner.text = "Done"
                 spinner.ok("✅")
             if debug:
                 display(df_filtered)
         else:
             # Just use original df to generate bullets
-            self.df_filtered = self.in_df
+            self.df_filtered = self.in_df[[self.doc_id_col, self.doc_col]]
         
-        step_name = "Distill-summarize"
-        self.print_step_name(step_name)
-        with self.spinner_wrapper() as spinner:
-            df_bullets = await distill_summarize(
-                text_df=self.df_filtered, 
-                doc_col=self.doc_col,
-                doc_id_col=self.doc_id_col,
-                model_name=self.distill_model_name,
-                n_bullets=params["summ_n_bullets"],
-                seed=seed,
-                sess=self,
-            )
-            self.df_bullets = df_bullets
-            spinner.text = "Done"
-            spinner.ok("✅")
-        if debug:
-            display(df_bullets)
+        if (custom_prompts["distill_summarize"] is not None):
+            step_name = "Distill-summarize"
+            self.print_step_name(step_name)
+            with self.spinner_wrapper() as spinner:
+                df_bullets = await distill_summarize(
+                    text_df=self.df_filtered, 
+                    doc_col=self.doc_col,
+                    doc_id_col=self.doc_id_col,
+                    model_name=self.distill_model_name,
+                    n_bullets=params["summ_n_bullets"],
+                    prompt_template=custom_prompts["distill_summarize"],
+                    seed=seed,
+                    sess=self,
+                )
+                self.df_bullets = df_bullets
+                spinner.text = "Done"
+                spinner.ok("✅")
+            if debug:
+                display(df_bullets)
+        else:
+            # Just use filtered df to generate concepts
+            self.df_bullets = self.df_filtered
         
         df_cluster_in = df_bullets
         synth_doc_col = self.doc_col
         synth_n_concepts = params["synth_n_concepts"]
         concept_col_prefix = "concept"
         # Perform synthesize step n_synth times
         for i in range(n_synth):
@@ -389,14 +434,15 @@
                     cluster_df=df_cluster, 
                     doc_col=synth_doc_col,
                     doc_id_col=self.doc_id_col,
                     model_name=self.synth_model_name,
                     concept_col_prefix=concept_col_prefix,
                     n_concepts=synth_n_concepts,
                     pattern_phrase="unique topic",
+                    prompt_template=custom_prompts["synthesize"],
                     seed=seed,
                     sess=self,
                     return_logs=True,
                 )
                 spinner.text = "Done"
                 spinner.ok("✅")
             if debug:
@@ -666,19 +712,20 @@
                 spinner.fail("❌")
                 print(f"Error: {e}")
 
     async def gen_auto(
         self,
         max_concepts=8,
         seed=None, params=None, n_synth=1,
+        custom_prompts=None,
         debug=True
     ):
         # Runs gen(), select(), and score() all at once
         # Run generation
-        await self.gen(seed=seed, params=params, n_synth=n_synth, auto_review=True, debug=debug)
+        await self.gen(seed=seed, params=params, n_synth=n_synth, custom_prompts=custom_prompts, auto_review=True, debug=debug)
 
         # Select the best concepts
         await self.select_auto(max_concepts=max_concepts)
         self.show_selected()
 
         # Run scoring
         score_df = await self.score()
```

### Comparing `text_lloom-0.7.2/PKG-INFO` & `text_lloom-0.7.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text_lloom
-Version: 0.7.2
+Version: 0.7.3
 Summary: Concept Induction to analyze unstructured text
 Author: Michelle Lam
 Author-email: mlam4@cs.stanford.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


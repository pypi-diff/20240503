# Comparing `tmp/uptrain-0.6.9.tar.gz` & `tmp/uptrain-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uptrain-0.6.9.tar", last modified: Wed Mar 20 18:23:13 2024, max compression
+gzip compressed data, was "uptrain-0.7.0.tar", last modified: Fri May  3 06:34:31 2024, max compression
```

## Comparing `uptrain-0.6.9.tar` & `uptrain-0.7.0.tar`

### file list

```diff
@@ -1,121 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.271146 uptrain-0.6.9/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-20 18:23:01.000000 uptrain-0.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    29448 2024-03-20 18:23:13.271146 uptrain-0.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    28085 2024-03-20 18:23:01.000000 uptrain-0.6.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-03-20 18:23:01.000000 uptrain-0.6.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 18:23:13.271146 uptrain-0.6.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.255146 uptrain-0.6.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    30080 2024-03-20 18:23:01.000000 uptrain-0.6.9/tests/test_builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-20 18:23:01.000000 uptrain-0.6.9/tests/test_custom_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-03-20 18:23:01.000000 uptrain-0.6.9/tests/test_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.255146 uptrain-0.6.9/uptrain/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.251146 uptrain-0.6.9/uptrain/dashboard/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.259146 uptrain-0.6.9/uptrain/dashboard/backend/
--rw-r--r--   0 runner    (1001) docker     (127)    32102 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/dashboard/backend/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/dashboard/backend/nest_asyncio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.259146 uptrain-0.6.9/uptrain/framework/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/framework/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11050 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/framework/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/framework/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    12355 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/framework/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    20910 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/framework/evalllm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/framework/evals.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/framework/rca_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    28392 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/framework/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/framework/signal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.259146 uptrain-0.6.9/uptrain/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/integrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/integrations/llama_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/integrations/promptfoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/integrations/promptfoo_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.263146 uptrain-0.6.9/uptrain/operators/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7980 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14860 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.263146 uptrain-0.6.9/uptrain/operators/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/code/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/code/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/drift.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.263146 uptrain-0.6.9/uptrain/operators/embedding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/embedding/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/embedding/vector_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    11415 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/embs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.263146 uptrain-0.6.9/uptrain/operators/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/io/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/io/bq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/io/duck.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/io/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/io/mongodb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.267146 uptrain-0.6.9/uptrain/operators/language/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)    26151 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/context_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/factual_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13521 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7501 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/guideline.py
--rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/jailbreak.py
--rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/language_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/meteor.py
--rw-r--r--   0 runner    (1001) docker     (127)    20512 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/model_grade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.255146 uptrain-0.6.9/uptrain/operators/language/openai_eval_custom/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.267146 uptrain-0.6.9/uptrain/operators/language/openai_eval_custom/completion_fns/
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/openai_eval_custom/completion_fns/dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.267146 uptrain-0.6.9/uptrain/operators/language/openai_eval_custom/elsuite/
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/openai_eval_custom/elsuite/model_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/openai_evals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.267146 uptrain-0.6.9/uptrain/operators/language/prompts/
--rw-r--r--   0 runner    (1001) docker     (127)    19906 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/prompts/classic.py
--rw-r--r--   0 runner    (1001) docker     (127)    41167 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/prompts/few_shots.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/prompts/instructions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/prompts/output_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/question_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)    36147 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/response_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/rouge.py
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/subquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/tone.py
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.267146 uptrain-0.6.9/uptrain/operators/rca/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/rca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/rca/rag_with_citation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.271146 uptrain-0.6.9/uptrain/st_classic/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/st_classic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/st_classic/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/st_classic/st_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/st_classic/st_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/st_classic/st_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.271146 uptrain-0.6.9/uptrain/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/utilities/app_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/utilities/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/utilities/prompt_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/utilities/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/utilities/sql_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/utilities/sqlglot_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.271146 uptrain-0.6.9/uptrain/validation_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/validation_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/validation_wrapper/validation_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.271146 uptrain-0.6.9/uptrain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    29448 2024-03-20 18:23:13.000000 uptrain-0.6.9/uptrain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-03-20 18:23:13.000000 uptrain-0.6.9/uptrain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 18:23:13.000000 uptrain-0.6.9/uptrain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-20 18:23:13.000000 uptrain-0.6.9/uptrain.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-20 18:23:13.000000 uptrain-0.6.9/uptrain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-20 18:23:13.000000 uptrain-0.6.9/uptrain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.707733 uptrain-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 06:34:26.000000 uptrain-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    32522 2024-05-03 06:34:31.707733 uptrain-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    31084 2024-05-03 06:34:26.000000 uptrain-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-03 06:34:26.000000 uptrain-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 06:34:31.707733 uptrain-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.687733 uptrain-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    31890 2024-05-03 06:34:26.000000 uptrain-0.7.0/tests/test_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-03 06:34:26.000000 uptrain-0.7.0/tests/test_custom_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-03 06:34:26.000000 uptrain-0.7.0/tests/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.691733 uptrain-0.7.0/uptrain/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.687733 uptrain-0.7.0/uptrain/dashboard/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.691733 uptrain-0.7.0/uptrain/dashboard/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)    37470 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/dashboard/backend/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/dashboard/backend/nest_asyncio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.691733 uptrain-0.7.0/uptrain/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/framework/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11264 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/framework/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/framework/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12355 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/framework/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.695733 uptrain-0.7.0/uptrain/framework/eval_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/framework/eval_assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/framework/eval_assistant/assistant_evals_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/framework/eval_assistant/assistant_evals_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/framework/eval_assistant/parse_files_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21531 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/framework/evalllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/framework/evals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/framework/rca_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29079 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/framework/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/framework/signal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.695733 uptrain-0.7.0/uptrain/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/integrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/integrations/llama_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/integrations/promptfoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/integrations/promptfoo_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.695733 uptrain-0.7.0/uptrain/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7980 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14860 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.695733 uptrain-0.7.0/uptrain/operators/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/code/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/code/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/drift.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.695733 uptrain-0.7.0/uptrain/operators/embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/embedding/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/embedding/vector_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11415 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/embs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.699733 uptrain-0.7.0/uptrain/operators/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/io/bq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/io/duck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/io/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/io/mongodb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.703733 uptrain-0.7.0/uptrain/operators/language/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26151 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/context_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/factual_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13521 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/guideline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/jailbreak.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21526 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/language_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11175 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/meteor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20512 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/model_grade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/multiquery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.687733 uptrain-0.7.0/uptrain/operators/language/openai_eval_custom/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.703733 uptrain-0.7.0/uptrain/operators/language/openai_eval_custom/completion_fns/
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/openai_eval_custom/completion_fns/dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.703733 uptrain-0.7.0/uptrain/operators/language/openai_eval_custom/elsuite/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/openai_eval_custom/elsuite/model_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/openai_evals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.703733 uptrain-0.7.0/uptrain/operators/language/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)    25375 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/prompts/classic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45880 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/prompts/few_shots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/prompts/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/prompts/output_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/question_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36138 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/response_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/subquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/tone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/language/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.703733 uptrain-0.7.0/uptrain/operators/rca/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/rca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/rca/rag_with_citation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/operators/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.703733 uptrain-0.7.0/uptrain/st_classic/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/st_classic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/st_classic/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/st_classic/st_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/st_classic/st_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/st_classic/st_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.703733 uptrain-0.7.0/uptrain/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/utilities/app_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/utilities/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/utilities/prompt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/utilities/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/utilities/sql_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/utilities/sqlglot_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.703733 uptrain-0.7.0/uptrain/validation_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/validation_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-03 06:34:26.000000 uptrain-0.7.0/uptrain/validation_wrapper/validation_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:34:31.707733 uptrain-0.7.0/uptrain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    32522 2024-05-03 06:34:31.000000 uptrain-0.7.0/uptrain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-03 06:34:31.000000 uptrain-0.7.0/uptrain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 06:34:31.000000 uptrain-0.7.0/uptrain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-03 06:34:31.000000 uptrain-0.7.0/uptrain.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-03 06:34:31.000000 uptrain-0.7.0/uptrain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 06:34:31.000000 uptrain-0.7.0/uptrain.egg-info/top_level.txt
```

### Comparing `uptrain-0.6.9/LICENSE` & `uptrain-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/PKG-INFO` & `uptrain-0.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,7 @@
-Metadata-Version: 2.1
-Name: uptrain
-Version: 0.6.9
-Summary: UpTrain - tool to evaluate LLM applications on aspects like factual accuracy, response quality, retrieval quality, tonality, etc.
-Maintainer-email: UpTrain AI Team <oss@uptrain.ai>
-License: Apache-2.0
-Project-URL: Homepage, https://uptrain.ai
-Project-URL: Repository, https://github.com/uptrain-ai/uptrain
-Keywords: uptrain,ai,LLM,evaluation,hallucinations,observability,response quality
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pydantic
-Requires-Dist: pydantic-settings
-Requires-Dist: loguru
-Requires-Dist: lazy_loader
-Requires-Dist: networkx
-Requires-Dist: polars>=0.18
-Requires-Dist: pandas
-Requires-Dist: numpy>=1.23.0
-Requires-Dist: httpx>=0.24.1
-Requires-Dist: plotly>=5.0.0
-Requires-Dist: aiolimiter>=1.1
-Requires-Dist: openai>=1.6.1
-Requires-Dist: fsspec
-Requires-Dist: litellm
-Requires-Dist: pyyaml
-Requires-Dist: json5
-Provides-Extra: test
-Requires-Dist: pytest>=7.0; extra == "test"
-
 <h4 align="center">
   <a href="https://uptrain.ai">
    <img alt="Logo of UpTrain - an open-source platform to evaluate and improve LLM applications" src="https://github.com/uptrain-ai/uptrain/assets/108270398/b6a4905f-63fd-47ab-a894-1026a6669c86"/>
   </a>
 </h4>
 
 <p align="center">
@@ -49,15 +12,18 @@
         <img alt="Read Docs" src="https://img.shields.io/badge/Read%20Docs-uptrain?logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAAGQAAABkCAYAAABw4pVUAAAACXBIWXMAAAsTAAALEwEAmpwYAAAC%2FklEQVR4nO3dO2sUURiH8SPipVAhKngJWggKolZ%2BAEGQIFiaL2CICNoLBmJAsBAbKxEREcTAYq%2BFYKGx8orxFkmhEltNY6P4yIEjs5FlJ4k7s%2B975v%2BD6ZJhD0%2FenZnsMhOCiIiIiIhIQwFbgFHgCjAJtPq83QF2hqYBNgNXgZ%2FYMwvsCE0B7E2LtuwjMBga8hb1CR9mso8C3MWXGWB7yBFwAPiNP2%2FjZIfcABfw6z2wLeQEuIdv74CtIRfA85IFv%2BnDdceTJUZ5FU%2FZQw6A6ZLFTvThNQ2zdC%2BBTcG7jIJEL9xHySzI3ygbg1cZBiEdF31GyTRI9AwYCN5kHIR0trYheJJ5kGgKWB%2B8aECQ6HHfogBHgJvpX%2BlPF%2FHzTQgSnat7EYPAAxaaXsTvNSXIRJ0L2APMdXgRClJ3kHgWAXygMwXpQ5Bu%2Fz73GmQAOLjEbbbv6wBWA99zC7IcJtaRzqi6UZCag5ymOwWpOcg43SlIzUEm6E5BCgrSxIO6JiRRkIXfBz5b8TYSSihIAuyjej6OhRbeslAQBelEE5JoQtroLaugCUk0IW00IQVNSALsip%2FdV7y1QgkFMUZBjFEQYxTEGAVJdNrbRqe9BU1IoglpowkpaEISTUgbTUhBE5JoQtpoQgqakIXfvh%2BueBsKJRTEGAUxRkGMURBjFMQYBTFGQYzJKcjrkn20arjO6MX2uWQd416CPKQZTnkJco1mOOwlyDHy9w1Y5SXIykUcR7w7X3mMXgVJ%2Bzlk9IkIvboD9jpXQdK%2BRoBf5OULsLvaChUFSfsbcvSUhDL3a78Nea%2BDpH2uBU6mW5DPOZqaH%2Bn5IjdqOaOqK4j8BwUxRkGMURBjFMQYBTFGQYxREGPi3ZpLrkPmDTw2tbWM7UzwCDhBni4Fj4D95Ol48Co9RS0n864eL%2FGv%2BNdEXsaCd8B18jAFrAnexUWkB9F79iibh0NGwApgFPiKv2PGWLyPfchRmpajwEXgloFrilaH7TZwOX3BrZ7Pu0VERERERIJ9fwBA%2FZMtFhwT0AAAAABJRU5ErkJggg%3D%3D&labelColor=976DA5&color=6A6A6A">
     </a>
     </a>
     <a href="https://join.slack.com/t/uptraincommunity/shared_invite/zt-1yih3aojn-CEoR_gAh6PDSknhFmuaJeg">
         <img alt="Slack Community" src="https://img.shields.io/badge/Slack%20Community-uptrain?logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAAGQAAABkCAYAAABw4pVUAAAACXBIWXMAAAsTAAALEwEAmpwYAAADFklEQVR4nO2cPW4TURSFLaWBhg6xACs9YhEsISiLiIzoUkGNRIV3kDSxhJVVBArKrCBUSCnCTyTc8KGRphomjsfv3vGBdz7JpY%2Bu5iQz9v3kN5kYY4wxxhhjjDHG%2FAXwGDgGPgJfgRXwBfgAHAJ7u8yrCuAI%2BM56LoFnu8irCuA9m3MLPB8zryrav%2BSh3AD7Y%2BRVRXuP%2F8Z2nGfnVUf7wC1hmplXHcBF4QWcZeZVB3BdeAHnmXnVAfwqvIBnnbzfkXnVAVwVXsBFJ4%2FIvOoAli5EiHZ94f8QFZpdUru%2B8C1LBeAp8NPPECGaXVK7vhiKH%2BqJpew36wtciBbAFHjZbmwX97xedd5bSt0fe6PBhWiBC9GC2gvpcdbRrIY48OxCpB39hs46mst1DjyzEGlHP9BZR3N7lwPPKkTa0W%2FprKO56XPgGYVIO%2FpCZx3NeXYh8o4%2BwFlHM00uRNvRBzjraGbJhWg7%2BgBnHc08uRBtRx%2FgwKM56czXfC8o4TTY0Z%2BoO%2FBo3gbP180LnU%2FRgUdzEDxfNy90PkUHHskP4FHgfH15ofMpOvBIXgfP15cXOp%2BiA4%2FiM%2FAwcL7evIz51Bx4BJ%2BAJ4Hz3ZmXNZ%2BSAy%2B9J78BHgTNd29e5nwqDnzo6xR4B7zY9gHZmW9Q3hjzGWNMrWzh1Ed11og5f0WnPpqzRtD5Kzr1UZw1os5f0amnO2uEnb%2BiU0911og7%2F4xCjpWdNeLOP6OQC2VnjbjzzyjkWtlZI%2B78FZ16tLM%2BC54vGnmnHu2sF8HzRSPv1A%2BSC1mihbRTj3bWfYVIO%2F%2BMQpScdV8h0s4%2FqxQFZ73um7%2B0888qZZfOepPdmLTzT2EHznro9lja%2BadR6KzTf6SJuPOXYoxCzABciBgu5D8vhH%2FJgSuyg0K6%2BOx3sUIafPa7WCENPvtdrJAGn%2F1OOYvgW2D1Z7%2BrFTKb1IxgIfNJzST8rnwl7cDVSXD0V5F51ZHg6JeRedWR4OgPI%2FOqI8HR70XmVUmko8%2FIq5IoR5%2BVVyURjj4zr1oocPRj5BljjDHGGGOMMcYYY8xElT9jEHRBpJyhuQAAAABJRU5ErkJggg%3D%3D&labelColor=6565d8&color=6A6A6A">
     </a>
     <a href="https://github.com/uptrain-ai/uptrain/issues/new?assignees=&labels=enhancement&template=feature_request.md&title=">
-        <img alt="Request New Feature" src="https://img.shields.io/badge/Request%20New%20Feature-uptrain?logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAAGQAAABkCAYAAABw4pVUAAAACXBIWXMAAAsTAAALEwEAmpwYAAAG%2BElEQVR4nO2da6gWRRjHN1NLKy1Tu2B5CjEsMiO0wEiqoxhmZQUJ5YfyQ5FhdLEiIiItLQtRIswiMIvKNDOTCosyCzsVGWiXLykVdrESQz1aXn7xcObAsmdmdvc9715md37wftAzszuz%2F3eemX3mmecNAo%2FH4%2FF4PKUF6AmMBxYDG4E1wLii21VXEZYAf9KV%2F4BLim5n3UWIsqboNlcO0osQ5sui218J6J4IYRYX3RdnAY4ELgYWAr%2FRHFqL7pdTkI0IncjI6ll0H%2BsuQpjn8ujIWGAacA9wf0GfmcCwBuaEVnlI3ZwTOtkNvAq8YCkzPishzlQ3%2FoviaAdWADcAxxQswrVAH3UP%2BXc%2B5kp16EngX%2BotwmvAdZ0ihO7VR%2F1dx5Jmi3EC8AHFsAd4ADi%2BbCJE7isjJXtzBfQCPqIYfgHOSTif5S5CpA35mCu1%2BiiCfcDIHEXYk1aE3M0VMAI4GNORA8BmYFuCTsuy8mtgf4KyszXt6VGECMD54hgE%2Bhr%2BLvVzMVfSWBubwktOYAKw0yDaLaFyA4G1luseAk6KtGU48B05jgRgMPBpqK58CS5N8ZyaZ67UMNxr6dgB3fpfHrym7HxNuX7A74Zrf6MpL%2BLnZo7kCwF8a3jIfYswV5NiOrnZUE%2B%2B%2FVG0mzPA64Zrr46UG0K%2Bc4KIscVy7XFFmKs7Yzq8zVDvDE3ZSYayaw3XXh8pd6IyY0mR0TsbGNRAv%2BPEEM7L1VypGz2RoOMTNPXmasq9pSk3XL3s6djZwHymQxYPS4HRTRTjk4Tmqrm%2BK%2BCZBB3eqeaMgWpkzLWsypYBZwP9gasSrMouirTnWLVH3ainoE353Y6yTOBxYsjfB%2BdurlIIkiXvWL7F4lT8qcHr%2FgHMA4ZGxJClu43vgVMSzoGZ%2BK6KFkS4LcaDIH6tDTTGAeUbm5xwZESX4X1zM1clEuQgMD1BW0cBz1vmpO7QRYwE5qq1qoJ08n6SuCZgADAL2EqGYuS6uiqpIJ38oJbjVvd7yMUiAWqHaYwuc0ZCc5VNIENJBenkH%2BXPGpGgH8PUJK5z6aQWQ13zekvdy5suRowg69W3rwyfy0wOP01%2FjgNmJPSHTY65lslc7cgskMEiyPLAYYAjlJirLOZshaV%2BvqurqgsSRoliWt0NLY25qpEgrZaHO8dQJ7%2BXwboJIlje0GU%2BODooenVVQ0FmWEbJtFKYK9cFoSPyZApwl0QlJlh9yTJaR1vhqyvXBaHDrHweafOimDqLLN%2F8MYWuriogyEOGdo%2B11DnLsgRemtZ3JRExWXTMVUHeNrT77ph64i8zbXINSmOu5IU1i465KshCQ7uviaknbngTc9Qefay5Uhtp87PomKuCnK7xW22Mm3SVQ3KrZe8kqbmaKs8ui445KYgAnKZGymrgwRShP%2FeSDp25WlkbQejYar1dPeRRGVx%2FQEwsWhJz1V4LQejYFZT98LC%2F6dYM7mM7dJPEXFEXQT7UtGVvUvd7SuEbNVcr6iTILkN7Rmdwrw3dMFe1EaTNkK5icAb3kmiWtOYqXMddQYALgPtkPpAgOku5KzXLT62LvAltkhCj7Q2aK3cFoeOo2qHIiakWS%2FkLVbiPnFaa2qx2GO71cIPmyk1BZEcOfdjpsqAEACdbwlZt5spZQaYYrr8lKAkqlrhL%2B6LOw4i5claQkYbrd4mULwqJ%2F1LmsdOsfhU9pKSOSrQ7L4hhf7pdzvMFJUO9wZuC5h7RPCNnBemltlDfBJ6VMyOBQ6gV4r7KCOI6lj2S8gmiDnVKYpjHgKslQC2oGMByJwRRXtkfI%2FVerJooOCSI6XyiNQLENVwS5F1D3TuCCoFDgixIemrXZVwSZIjyS4WR%2FQw%2FhxS4yhJf0KPAS2KqgN5BxcCVEVIX8IKUCy9IyfCClIzSC6I2nU4NagJlFUQlnvkissRtevBB2SizIJ9pyq0MKg5lFEQ5Ek1h%2FJV793BBkH6GbG9y2qhHUGEooyCq7Bu5NKpklFmQ%2FipIeZdK0r8gbeJJFymtIKE6lXIelk2Qp9IKUjcw7%2FvMy%2BJmEubpBbEfgfvV8IxmBs0GuMIL0lDkpTAxaDZqotbFHNXeZAEtlt%2Br2h3NkdJMUXS%2FiVFbQYDewI2Ro3VRXsmyAedqItS1gqjELBI49rJpyKqFwjpHP22WnCjhA0TZRl8CT8cJYlgA3KwpV9Qv9eRF8xMGGIap5Fk0uU56G%2FLlbq%2BZIOty%2B%2BFIlcLoY3XjVZpD%2BjoOaxKA6bzCVeA923G8LHNQPS4nVDVJJXXn8TZprvEz1WK%2FyoPS%2FOw%2FaXKJaP5vYiQ5y9%2BaXzdo6UZS47KxQ%2BUN1ibKLFPSFzlJO92QK32MSmjs6mcWcJM6eFrciPB4PB6Px%2BPxeDwej8fj8XiCYvgfmdGLzXmrOA4AAAAASUVORK5CYII%3D&labelColor=3E93C4&color=6A6A6A">
+        <img alt="Request New Feature" src="https://img.shields.io/badge/Request%20New%20Feature-uptrain?logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAAGQAAABkCAYAAABw4pVUAAAACXBIWXMAAAsTAAALEwEAmpwYAAAG%2BElEQVR4nO2da6gWRRjHN1NLKy1Tu2B5CjEsMiO0wEiqoxhmZQUJ5YfyQ5FhdLEiIiItLQtRIswiMIvKNDOTCosyCzsVGWiXLykVdrESQz1aXn7xcObAsmdmdvc9715md37wftAzszuz%2F3eemX3mmecNAo%2FH4%2FF4PKUF6AmMBxYDG4E1wLii21VXEZYAf9KV%2F4BLim5n3UWIsqboNlcO0osQ5sui218J6J4IYRYX3RdnAY4ELgYWAr%2FRHFqL7pdTkI0IncjI6ll0H%2BsuQpjn8ujIWGAacA9wf0GfmcCwBuaEVnlI3ZwTOtkNvAq8YCkzPishzlQ3%2FoviaAdWADcAxxQswrVAH3UP%2BXc%2B5kp16EngX%2BotwmvAdZ0ihO7VR%2F1dx5Jmi3EC8AHFsAd4ADi%2BbCJE7isjJXtzBfQCPqIYfgHOSTif5S5CpA35mCu1%2BiiCfcDIHEXYk1aE3M0VMAI4GNORA8BmYFuCTsuy8mtgf4KyszXt6VGECMD54hgE%2Bhr%2BLvVzMVfSWBubwktOYAKw0yDaLaFyA4G1luseAk6KtGU48B05jgRgMPBpqK58CS5N8ZyaZ67UMNxr6dgB3fpfHrym7HxNuX7A74Zrf6MpL%2BLnZo7kCwF8a3jIfYswV5NiOrnZUE%2B%2B%2FVG0mzPA64Zrr46UG0K%2Bc4KIscVy7XFFmKs7Yzq8zVDvDE3ZSYayaw3XXh8pd6IyY0mR0TsbGNRAv%2BPEEM7L1VypGz2RoOMTNPXmasq9pSk3XL3s6djZwHymQxYPS4HRTRTjk4Tmqrm%2BK%2BCZBB3eqeaMgWpkzLWsypYBZwP9gasSrMouirTnWLVH3ainoE353Y6yTOBxYsjfB%2BdurlIIkiXvWL7F4lT8qcHr%2FgHMA4ZGxJClu43vgVMSzoGZ%2BK6KFkS4LcaDIH6tDTTGAeUbm5xwZESX4X1zM1clEuQgMD1BW0cBz1vmpO7QRYwE5qq1qoJ08n6SuCZgADAL2EqGYuS6uiqpIJ38oJbjVvd7yMUiAWqHaYwuc0ZCc5VNIENJBenkH%2BXPGpGgH8PUJK5z6aQWQ13zekvdy5suRowg69W3rwyfy0wOP01%2FjgNmJPSHTY65lslc7cgskMEiyPLAYYAjlJirLOZshaV%2BvqurqgsSRoliWt0NLY25qpEgrZaHO8dQJ7%2BXwboJIlje0GU%2BODooenVVQ0FmWEbJtFKYK9cFoSPyZApwl0QlJlh9yTJaR1vhqyvXBaHDrHweafOimDqLLN%2F8MYWuriogyEOGdo%2B11DnLsgRemtZ3JRExWXTMVUHeNrT77ph64i8zbXINSmOu5IU1i465KshCQ7uviaknbngTc9Qefay5Uhtp87PomKuCnK7xW22Mm3SVQ3KrZe8kqbmaKs8ui445KYgAnKZGymrgwRShP%2FeSDp25WlkbQejYar1dPeRRGVx%2FQEwsWhJz1V4LQejYFZT98LC%2F6dYM7mM7dJPEXFEXQT7UtGVvUvd7SuEbNVcr6iTILkN7Rmdwrw3dMFe1EaTNkK5icAb3kmiWtOYqXMddQYALgPtkPpAgOku5KzXLT62LvAltkhCj7Q2aK3cFoeOo2qHIiakWS%2FkLVbiPnFaa2qx2GO71cIPmyk1BZEcOfdjpsqAEACdbwlZt5spZQaYYrr8lKAkqlrhL%2B6LOw4i5claQkYbrd4mULwqJ%2F1LmsdOsfhU9pKSOSrQ7L4hhf7pdzvMFJUO9wZuC5h7RPCNnBemltlDfBJ6VMyOBQ6gV4r7KCOI6lj2S8gmiDnVKYpjHgKslQC2oGMByJwRRXtkfI%2FVerJooOCSI6XyiNQLENVwS5F1D3TuCCoFDgixIemrXZVwSZIjyS4WR%2FQw%2FhxS4yhJf0KPAS2KqgN5BxcCVEVIX8IKUCy9IyfCClIzSC6I2nU4NagJlFUQlnvkissRtevBB2SizIJ9pyq0MKg5lFEQ5Ek1h%2FJV793BBkH6GbG9y2qhHUGEooyCq7Bu5NKpklFmQ%2FipIeZdK0r8gbeJJFymtIKE6lXIelk2Qp9IKUjcw7%2FvMy%2BJmEubpBbEfgfvV8IxmBs0GuMIL0lDkpTAxaDZqotbFHNXeZAEtlt%2Br2h3NkdJMUXS%2FiVFbQYDewI2Ro3VRXsmyAedqItS1gqjELBI49rJpyKqFwjpHP22WnCjhA0TZRl8CT8cJYlgA3KwpV9Qv9eRF8xMGGIap5Fk0uU56G%2FLlbq%2BZIOty%2B%2BFIlcLoY3XjVZpD%2BjoOaxKA6bzCVeA923G8LHNQPS4nVDVJJXXn8TZprvEz1WK%2FyoPS%2FOw%2FaXKJaP5vYiQ5y9%2BaXzdo6UZS47KxQ%2BUN1ibKLFPSFzlJO92QK32MSmjs6mcWcJM6eFrciPB4PB6Px%2BPxeDwej8fj8XiCYvgfmdGLzXmrOA4AAAAASUVORK5CYII%3D&labelColor=5B92E9&color=6A6A6A">
+    </a>
+    <a href="https://demo.uptrain.ai/benchmark">
+      <img alt="Daily Monitoring" src="https://img.shields.io/badge/Daily%20Monitoring-uptrain?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAGQAAABkCAYAAABw4pVUAAAACXBIWXMAAAsTAAALEwEAmpwYAAAFUUlEQVR4nO2daahVVRTHt2WDls3RQDYXRUZBkRkRjdAraPjSAJUUKVSE0QuiQZ4FmRj2lMwwqGgitZTq5cvEIipKpGgymogwCrKs7IOkDf5i9ZYorzvsM+99zvrB/XjWXfv+z9ln7zXs65xhGIZhGIZhGIZRCsD2wOXAIuA94P2MH7HxLHBBOSOoEcBewJsUx/PATlWPMxqAQYpnXtXjjALgDMrhb+CwqscbPMAMymNy1eMNHuDxEgXpq3q8wQP0lSjIPVWPN3iAY4HNJkhAAHNMkIAAdgBml/Ck2JSVBOAo4HbgYWD+sM9KEyQQZP8ArDVBAgDYDfjUpqwAAEYCy+0dEgjAPHupBwJwq62yAgHo0WCgLXurBjgOWG/7kAAA9gfW2MYwAIDRwKoUYkiq9pdG7NQZSq3eD3wCrANWAwuBOyRXDRyU0/dsB7yQQoxvgf2AH2svCHCO50BFqBXALGAicCKwY8Lvmp5CjN+BcXp9fQXRu3VqxlXOn8DHwFNAL3AusG+b7xMRkyK+9Wxj42vP625zMQHsAyyjOH4AXtW07RXAZcCmFHZuHub3y57XxVMSBEwAviN85rbw/SKP62T1NtLFADBFp5nQWdbuRwWe6HDdRqlucZFEUqWILAZWi79d3n13tdhUfgSMd6EDnAB8RRys9a2pAnbRWq+Lt6zCgge4BthAHPwBnObqCLCzpkNjYTNwlasjwNG6N8jCr/opi2mujuh8+lvGH2cVcKjaO1A3e1N08/dZAeFyaUsY4eqEhDC0vCbrtDFLSnU8XqbjpX5Wq0be0fBGGt6V6dXVCWCsRkKzsB64NIMPI4DDxYZMP8AS4Jsu9VeDnZa3UQKcD/ycUYwPgSML3P+cDtykT5NMT/3Aea5O6B0phWb/ZBRD3gujqx5P1Ghg8LUc1vzXVz2W6AGO0GRNFr4AjneRA+ypwcZrgbOS5mby6l6VeE0WJAs4xsVfVDddA4nb8n2WhUkaRy7JIMSm4bmFWAGe6TBOWdVdGXpvxZoooqAeABd6jFciDHu4ogEeTSGGrPX3djWBoWWzDxNDK7mU8MbdkjtwNQL/GN2MMpw5RJer3ZDKjLNdDQG+9BRkdlkO3dLFkbckIOhqCqEJok5NalHBt0HTmnEk9+skiDq2q1YUTtaA3u6uARCqIE0FEyQsTJDAaIwgDFWWS/X7B5pYegO4ofSAXRcaIYiWlq5rM7CVIe30ay+I5lZ+6jK4V1wgNEEQ3yOTTnEB0ARB3vYc4J0uAJogyOcxDZAGCCLpXB/muAAwQbZigtTpCWGobUCqIhcAD0pRQko7NmVlEUSDoFLF2IqBpEFREyS7IC/SmUETpKQpCzjT03ZP9FOWtglcJ/sDzYmMDVCQfk/b86MVRBse723R8y2dtQ8kzRgWLMgiT9uDMQvSn9fdVoIgSzxtL49SEKnH9ax2PzWBTRMkLcB9ed/NJkgGgOc8BVmawKY9IWkBFnsKsiKBTRMkLSaIC+6lbk8IJsgWbNlrT8j/sSdkK/aEtLg7JJeQdyhCTiH1YWaB/g4U4G8p/SEzPZ15JIFN3zMMbyzwb/IeSmDzpWD+Nk9CIp7OeJ+SAFztYe8v4IAU/p7s6a/3kXzS0Olhb2O7k1FzR09e6MRAkpN1tNX69S42p2bw97EuthekiHZ3OzSh15UFMAp4uo0ji9P0oOup1kvb9ClOy9KnKH8ULFNom0No5DDLUSlsjtF++1ZPRnliDHPqJA02PqlF0hNymhL75HhWPRT54Hy8/c/2MXps+Vzt9BqXU/S7V3+HSaVNU4ZhGIZhGIZhGIZhGIbhquVfiiAaCf/Kq/8AAAAASUVORK5CYII=&labelColor=35B9D2&color=6A6A6A">
     </a>
 </p>
 
 <p align="center">
   <a href="https://github.com/uptrain-ai/uptrain/releases">
     <img alt="GitHub Release" src="https://img.shields.io/github/v/release/uptrain-ai/uptrain?labelColor=6A6A6A&color=CC766E">
   </a>
@@ -73,18 +39,14 @@
 </p>
 
 <h4 align="center">
   <video src="https://github.com/uptrain-ai/uptrain/assets/43818888/68a3b169-2217-446b-93b2-96b48ec7201d" alt="Demo of UpTrain's LLM evaluations with scores for hallucinations, retrieved-context quality, response tonality for a customer support chatbot" autoplay>
 </h4>
 
 
-
-
-
-
 **[UpTrain](https://uptrain.ai)** is an open-source unified platform to evaluate and improve Generative AI applications. We provide grades for [20+ preconfigured evaluations](https://github.com/uptrain-ai/uptrain?tab=readme-ov-file#pre-built-evaluations-we-offer-) (covering language, code, embedding use cases), perform [root cause analysis](https://github.com/uptrain-ai/uptrain/blob/main/examples/root_cause_analysis/rag_with_citation.ipynb) on failure cases and give insights on how to resolve them.    
 
 <br />
 
 # Key Features 🔑
 
 <img width="1088" alt="Interactive Dashboards" src="https://github.com/uptrain-ai/uptrain/assets/36454110/eb1c8239-dd99-4e66-ba8a-cbaee2beec10">
@@ -249,14 +211,16 @@
 |[Jailbreak Detection](https://docs.uptrain.ai/predefined-evaluations/safeguarding/jailbreak) | Grades whether the user's prompt is an attempt to jailbreak (i.e. generate illegal or harmful responses). |
 
 <img width="1088" alt="evaluate the clarity of user queries" src="https://github.com/uptrain-ai/uptrain/assets/36454110/50ed622f-0b92-468c-af48-2391ff6ab8e0">
 
 | Eval | Description |
 | ---- | ----------- |
 |[Sub-Query Completeness](https://docs.uptrain.ai/predefined-evaluations/query-quality/sub-query-completeness) | Evaluate whether all of the sub-questions generated from a user's query, taken together, cover all aspects of the user's query or not |
+| [Multi-Query Accuracy](https://docs.uptrain.ai/predefined-evaluations/query-quality/multi-query-accuracy) | Evaluate whether the variants generated accurately represent the original query |
+
 
 <br />
 
 # Integrations 🤝
 
 | Eval Frameworks  | LLM Providers | LLM Packages | Serving frameworks | LLM Observability | Vector DBs |
 | ------------- | ------------- | ------------- | ------------- | ------------- |  ------------- |
@@ -266,14 +230,23 @@
 | | [Mistral](https://docs.uptrain.ai/llms/mistral) | | Replicate  |
 | |  | |  HuggingFace  |
 
 More integrations are coming soon. If you have a specific integration in mind, please let us know by [creating an issue](https://github.com/uptrain-ai/uptrain/issues).
 
 <br />
 
+# Monitoring Prompt Drift in LLMs: Benchmark by UpTrain
+
+Most popular LLMs like GPT-4, GPT-3.5-turbo, Claude-2.1 etc., are closed-source, i.e. exposed via an API with very little visibility on what happens under the hood. There are many reported instances of prompt drift (or GPT-4 becoming lazy) and research work exploring the degradation in model quality. This benchmark is an attempt to track the change in model behaviour by evaluating its response on a fixed dataset.
+
+<img width="1316" alt="image" src="https://github.com/uptrain-ai/uptrain/assets/43818888/65b7e8c3-3f5e-48bb-98c1-88208520945b">
+
+You can find the benchmark [here](https://demo.uptrain.ai/benchmark).
+
+
 # Resources 💡
 
 1. [How to evaluate your LLM application](https://blog.uptrain.ai/how-to-evaluate-your-llm-applications)
 1. [How to detect jailbreaks](https://blog.uptrain.ai/llm-jailbreak/)
 1. [Dealing with hallucinations](https://blog.uptrain.ai/dealing-with-hallucinations-in-llms-a-deep-dive/)
 
 <br />
```

#### html2text {}

```diff
@@ -1,29 +1,11 @@
-Metadata-Version: 2.1 Name: uptrain Version: 0.6.9 Summary: UpTrain - tool to
-evaluate LLM applications on aspects like factual accuracy, response quality,
-retrieval quality, tonality, etc. Maintainer-email: UpTrain AI Team
-uptrain.ai> License: Apache-2.0 Project-URL: Homepage, https://uptrain.ai
-Project-URL: Repository, https://github.com/uptrain-ai/uptrain Keywords:
-uptrain,ai,LLM,evaluation,hallucinations,observability,response quality
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Developers Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist: pydantic
-Requires-Dist: pydantic-settings Requires-Dist: loguru Requires-Dist:
-lazy_loader Requires-Dist: networkx Requires-Dist: polars>=0.18 Requires-Dist:
-pandas Requires-Dist: numpy>=1.23.0 Requires-Dist: httpx>=0.24.1 Requires-Dist:
-plotly>=5.0.0 Requires-Dist: aiolimiter>=1.1 Requires-Dist: openai>=1.6.1
-Requires-Dist: fsspec Requires-Dist: litellm Requires-Dist: pyyaml Requires-
-Dist: json5 Provides-Extra: test Requires-Dist: pytest>=7.0; extra == "test"
   ****** _[[_LL_oo_gg_oo_ _oo_ff_ _UU_pp_TT_rr_aa_ii_nn_ _--_ _aa_nn_ _oo_pp_ee_nn_--_ss_oo_uu_rr_cc_ee_ _pp_ll_aa_tt_ff_oo_rr_mm_ _tt_oo_ _ee_vv_aa_ll_uu_aa_tt_ee_ _aa_nn_dd_ _ii_mm_pp_rr_oo_vv_ee_ _LL_LL_MM
                                _aa_pp_pp_ll_ii_cc_aa_tt_ii_oo_nn_ss_]] ******
                         _[_T_r_y_ _o_u_t_ _E_v_a_l_u_a_t_i_o_n_]_[_R_e_a_d_ _D_o_c_s_]
-_[_S_l_a_c_k_ _C_o_m_m_u_n_i_t_y_]_[_R_e_q_u_e_s_t_ _N_e_w_ _F_e_a_t_u_r_e_]
+_[_S_l_a_c_k_ _C_o_m_m_u_n_i_t_y_]_[_R_e_q_u_e_s_t_ _N_e_w_ _F_e_a_t_u_r_e_]_[_D_a_i_l_y_ _M_o_n_i_t_o_r_i_n_g_]
   _[_G_i_t_H_u_b_ _R_e_l_e_a_s_e_]_[_G_i_t_H_u_b_ _c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]_[_G_i_t_H_u_b_ _L_i_c_e_n_s_e_]_[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]
 **[UpTrain](https://uptrain.ai)** is an open-source unified platform to
 evaluate and improve Generative AI applications. We provide grades for [20+
 preconfigured evaluations](https://github.com/uptrain-ai/uptrain?tab=readme-ov-
 file#pre-built-evaluations-we-offer-) (covering language, code, embedding use
 cases), perform [root cause analysis](https://github.com/uptrain-ai/uptrain/
 blob/main/examples/root_cause_analysis/rag_with_citation.ipynb) on failure
@@ -152,15 +134,18 @@
 LLM reveal its system prompts. | |[Jailbreak Detection](https://
 docs.uptrain.ai/predefined-evaluations/safeguarding/jailbreak) | Grades whether
 the user's prompt is an attempt to jailbreak (i.e. generate illegal or harmful
 responses). | [evaluate the clarity of user queries]| Eval | Description | | --
 -- | ----------- | |[Sub-Query Completeness](https://docs.uptrain.ai/
 predefined-evaluations/query-quality/sub-query-completeness) | Evaluate whether
 all of the sub-questions generated from a user's query, taken together, cover
-all aspects of the user's query or not |
+all aspects of the user's query or not | | [Multi-Query Accuracy](https://
+docs.uptrain.ai/predefined-evaluations/query-quality/multi-query-accuracy) |
+Evaluate whether the variants generated accurately represent the original query
+|
 # Integrations ð¤ | Eval Frameworks | LLM Providers | LLM Packages | Serving
 frameworks | LLM Observability | Vector DBs | | ------------- | ------------- |
 ------------- | ------------- | ------------- | ------------- | | [OpenAI
 Evals](https://docs.uptrain.ai/tutorials/openai-evals) | [OpenAI](https://
 docs.uptrain.ai/llms/openai) | [LlamaIndex](https://docs.uptrain.ai/
 integrations/framework/llamaindex-methods/overview) | [Ollama](https://
 docs.uptrain.ai/llms/ollama) | [Langfuse](https://docs.uptrain.ai/integrations/
@@ -172,15 +157,22 @@
 docs.uptrain.ai/llms/claude) | | [Anyscale](https://docs.uptrain.ai/llms/
 anyscale) | [Zeno](https://docs.uptrain.ai/integrations/observation-tools/zeno)
 | [Chroma](https://docs.uptrain.ai/integrations/vector_db/chroma) | | |
 [Mistral](https://docs.uptrain.ai/llms/mistral) | | Replicate | | | | |
 HuggingFace | More integrations are coming soon. If you have a specific
 integration in mind, please let us know by [creating an issue](https://
 github.com/uptrain-ai/uptrain/issues).
-# Resources ð¡ 1. [How to evaluate your LLM application](https://
+# Monitoring Prompt Drift in LLMs: Benchmark by UpTrain Most popular LLMs like
+GPT-4, GPT-3.5-turbo, Claude-2.1 etc., are closed-source, i.e. exposed via an
+API with very little visibility on what happens under the hood. There are many
+reported instances of prompt drift (or GPT-4 becoming lazy) and research work
+exploring the degradation in model quality. This benchmark is an attempt to
+track the change in model behaviour by evaluating its response on a fixed
+dataset. [image]You can find the benchmark [here](https://demo.uptrain.ai/
+benchmark). # Resources ð¡ 1. [How to evaluate your LLM application](https://
 blog.uptrain.ai/how-to-evaluate-your-llm-applications) 1. [How to detect
 jailbreaks](https://blog.uptrain.ai/llm-jailbreak/) 1. [Dealing with
 hallucinations](https://blog.uptrain.ai/dealing-with-hallucinations-in-llms-a-
 deep-dive/)
 # Why we are building UpTrain ð¤ Having worked with ML and NLP models for the
 last 8 years, we were continuosly frustated with numerous hidden failures in
 our models which led to us building UpTrain. UpTrain was initially started as
```

### Comparing `uptrain-0.6.9/README.md` & `uptrain-0.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,47 @@
+Metadata-Version: 2.1
+Name: uptrain
+Version: 0.7.0
+Summary: UpTrain - tool to evaluate LLM applications on aspects like factual accuracy, response quality, retrieval quality, tonality, etc.
+Maintainer-email: UpTrain AI Team <oss@uptrain.ai>
+License: Apache-2.0
+Project-URL: Homepage, https://uptrain.ai
+Project-URL: Repository, https://github.com/uptrain-ai/uptrain
+Keywords: uptrain,ai,LLM,evaluation,hallucinations,observability,response quality
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pydantic
+Requires-Dist: pydantic-settings
+Requires-Dist: loguru
+Requires-Dist: lazy_loader
+Requires-Dist: networkx
+Requires-Dist: polars>=0.18
+Requires-Dist: pandas
+Requires-Dist: numpy>=1.23.0
+Requires-Dist: httpx>=0.24.1
+Requires-Dist: plotly>=5.0.0
+Requires-Dist: aiolimiter>=1.1
+Requires-Dist: openai>=1.6.1
+Requires-Dist: fsspec
+Requires-Dist: litellm
+Requires-Dist: pyyaml
+Requires-Dist: json5
+Requires-Dist: python-docx
+Requires-Dist: pymupdf
+Requires-Dist: faiss-cpu
+Provides-Extra: test
+Requires-Dist: pytest>=7.0; extra == "test"
+
 <h4 align="center">
   <a href="https://uptrain.ai">
    <img alt="Logo of UpTrain - an open-source platform to evaluate and improve LLM applications" src="https://github.com/uptrain-ai/uptrain/assets/108270398/b6a4905f-63fd-47ab-a894-1026a6669c86"/>
   </a>
 </h4>
 
 <p align="center">
@@ -12,15 +52,18 @@
         <img alt="Read Docs" src="https://img.shields.io/badge/Read%20Docs-uptrain?logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAAGQAAABkCAYAAABw4pVUAAAACXBIWXMAAAsTAAALEwEAmpwYAAAC%2FklEQVR4nO3dO2sUURiH8SPipVAhKngJWggKolZ%2BAEGQIFiaL2CICNoLBmJAsBAbKxEREcTAYq%2BFYKGx8orxFkmhEltNY6P4yIEjs5FlJ4k7s%2B975v%2BD6ZJhD0%2FenZnsMhOCiIiIiIhIQwFbgFHgCjAJtPq83QF2hqYBNgNXgZ%2FYMwvsCE0B7E2LtuwjMBga8hb1CR9mso8C3MWXGWB7yBFwAPiNP2%2FjZIfcABfw6z2wLeQEuIdv74CtIRfA85IFv%2BnDdceTJUZ5FU%2FZQw6A6ZLFTvThNQ2zdC%2BBTcG7jIJEL9xHySzI3ygbg1cZBiEdF31GyTRI9AwYCN5kHIR0trYheJJ5kGgKWB%2B8aECQ6HHfogBHgJvpX%2BlPF%2FHzTQgSnat7EYPAAxaaXsTvNSXIRJ0L2APMdXgRClJ3kHgWAXygMwXpQ5Bu%2Fz73GmQAOLjEbbbv6wBWA99zC7IcJtaRzqi6UZCag5ymOwWpOcg43SlIzUEm6E5BCgrSxIO6JiRRkIXfBz5b8TYSSihIAuyjej6OhRbeslAQBelEE5JoQtroLaugCUk0IW00IQVNSALsip%2FdV7y1QgkFMUZBjFEQYxTEGAVJdNrbRqe9BU1IoglpowkpaEISTUgbTUhBE5JoQtpoQgqakIXfvh%2BueBsKJRTEGAUxRkGMURBjFMQYBTFGQYzJKcjrkn20arjO6MX2uWQd416CPKQZTnkJco1mOOwlyDHy9w1Y5SXIykUcR7w7X3mMXgVJ%2Bzlk9IkIvboD9jpXQdK%2BRoBf5OULsLvaChUFSfsbcvSUhDL3a78Nea%2BDpH2uBU6mW5DPOZqaH%2Bn5IjdqOaOqK4j8BwUxRkGMURBjFMQYBTFGQYxREGPi3ZpLrkPmDTw2tbWM7UzwCDhBni4Fj4D95Ol48Co9RS0n864eL%2FGv%2BNdEXsaCd8B18jAFrAnexUWkB9F79iibh0NGwApgFPiKv2PGWLyPfchRmpajwEXgloFrilaH7TZwOX3BrZ7Pu0VERERERIJ9fwBA%2FZMtFhwT0AAAAABJRU5ErkJggg%3D%3D&labelColor=976DA5&color=6A6A6A">
     </a>
     </a>
     <a href="https://join.slack.com/t/uptraincommunity/shared_invite/zt-1yih3aojn-CEoR_gAh6PDSknhFmuaJeg">
         <img alt="Slack Community" src="https://img.shields.io/badge/Slack%20Community-uptrain?logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAAGQAAABkCAYAAABw4pVUAAAACXBIWXMAAAsTAAALEwEAmpwYAAADFklEQVR4nO2cPW4TURSFLaWBhg6xACs9YhEsISiLiIzoUkGNRIV3kDSxhJVVBArKrCBUSCnCTyTc8KGRphomjsfv3vGBdz7JpY%2Bu5iQz9v3kN5kYY4wxxhhjjDHG%2FAXwGDgGPgJfgRXwBfgAHAJ7u8yrCuAI%2BM56LoFnu8irCuA9m3MLPB8zryrav%2BSh3AD7Y%2BRVRXuP%2F8Z2nGfnVUf7wC1hmplXHcBF4QWcZeZVB3BdeAHnmXnVAfwqvIBnnbzfkXnVAVwVXsBFJ4%2FIvOoAli5EiHZ94f8QFZpdUru%2B8C1LBeAp8NPPECGaXVK7vhiKH%2BqJpew36wtciBbAFHjZbmwX97xedd5bSt0fe6PBhWiBC9GC2gvpcdbRrIY48OxCpB39hs46mst1DjyzEGlHP9BZR3N7lwPPKkTa0W%2FprKO56XPgGYVIO%2FpCZx3NeXYh8o4%2BwFlHM00uRNvRBzjraGbJhWg7%2BgBnHc08uRBtRx%2FgwKM56czXfC8o4TTY0Z%2BoO%2FBo3gbP180LnU%2FRgUdzEDxfNy90PkUHHskP4FHgfH15ofMpOvBIXgfP15cXOp%2BiA4%2FiM%2FAwcL7evIz51Bx4BJ%2BAJ4Hz3ZmXNZ%2BSAy%2B9J78BHgTNd29e5nwqDnzo6xR4B7zY9gHZmW9Q3hjzGWNMrWzh1Ed11og5f0WnPpqzRtD5Kzr1UZw1os5f0amnO2uEnb%2BiU0911og7%2F4xCjpWdNeLOP6OQC2VnjbjzzyjkWtlZI%2B78FZ16tLM%2BC54vGnmnHu2sF8HzRSPv1A%2BSC1mihbRTj3bWfYVIO%2F%2BMQpScdV8h0s4%2FqxQFZ73um7%2B0888qZZfOepPdmLTzT2EHznro9lja%2BadR6KzTf6SJuPOXYoxCzABciBgu5D8vhH%2FJgSuyg0K6%2BOx3sUIafPa7WCENPvtdrJAGn%2F1OOYvgW2D1Z7%2BrFTKb1IxgIfNJzST8rnwl7cDVSXD0V5F51ZHg6JeRedWR4OgPI%2FOqI8HR70XmVUmko8%2FIq5IoR5%2BVVyURjj4zr1oocPRj5BljjDHGGGOMMcYYY8xElT9jEHRBpJyhuQAAAABJRU5ErkJggg%3D%3D&labelColor=6565d8&color=6A6A6A">
     </a>
     <a href="https://github.com/uptrain-ai/uptrain/issues/new?assignees=&labels=enhancement&template=feature_request.md&title=">
-        <img alt="Request New Feature" src="https://img.shields.io/badge/Request%20New%20Feature-uptrain?logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAAGQAAABkCAYAAABw4pVUAAAACXBIWXMAAAsTAAALEwEAmpwYAAAG%2BElEQVR4nO2da6gWRRjHN1NLKy1Tu2B5CjEsMiO0wEiqoxhmZQUJ5YfyQ5FhdLEiIiItLQtRIswiMIvKNDOTCosyCzsVGWiXLykVdrESQz1aXn7xcObAsmdmdvc9715md37wftAzszuz%2F3eemX3mmecNAo%2FH4%2FF4PKUF6AmMBxYDG4E1wLii21VXEZYAf9KV%2F4BLim5n3UWIsqboNlcO0osQ5sui218J6J4IYRYX3RdnAY4ELgYWAr%2FRHFqL7pdTkI0IncjI6ll0H%2BsuQpjn8ujIWGAacA9wf0GfmcCwBuaEVnlI3ZwTOtkNvAq8YCkzPishzlQ3%2FoviaAdWADcAxxQswrVAH3UP%2BXc%2B5kp16EngX%2BotwmvAdZ0ihO7VR%2F1dx5Jmi3EC8AHFsAd4ADi%2BbCJE7isjJXtzBfQCPqIYfgHOSTif5S5CpA35mCu1%2BiiCfcDIHEXYk1aE3M0VMAI4GNORA8BmYFuCTsuy8mtgf4KyszXt6VGECMD54hgE%2Bhr%2BLvVzMVfSWBubwktOYAKw0yDaLaFyA4G1luseAk6KtGU48B05jgRgMPBpqK58CS5N8ZyaZ67UMNxr6dgB3fpfHrym7HxNuX7A74Zrf6MpL%2BLnZo7kCwF8a3jIfYswV5NiOrnZUE%2B%2B%2FVG0mzPA64Zrr46UG0K%2Bc4KIscVy7XFFmKs7Yzq8zVDvDE3ZSYayaw3XXh8pd6IyY0mR0TsbGNRAv%2BPEEM7L1VypGz2RoOMTNPXmasq9pSk3XL3s6djZwHymQxYPS4HRTRTjk4Tmqrm%2BK%2BCZBB3eqeaMgWpkzLWsypYBZwP9gasSrMouirTnWLVH3ainoE353Y6yTOBxYsjfB%2BdurlIIkiXvWL7F4lT8qcHr%2FgHMA4ZGxJClu43vgVMSzoGZ%2BK6KFkS4LcaDIH6tDTTGAeUbm5xwZESX4X1zM1clEuQgMD1BW0cBz1vmpO7QRYwE5qq1qoJ08n6SuCZgADAL2EqGYuS6uiqpIJ38oJbjVvd7yMUiAWqHaYwuc0ZCc5VNIENJBenkH%2BXPGpGgH8PUJK5z6aQWQ13zekvdy5suRowg69W3rwyfy0wOP01%2FjgNmJPSHTY65lslc7cgskMEiyPLAYYAjlJirLOZshaV%2BvqurqgsSRoliWt0NLY25qpEgrZaHO8dQJ7%2BXwboJIlje0GU%2BODooenVVQ0FmWEbJtFKYK9cFoSPyZApwl0QlJlh9yTJaR1vhqyvXBaHDrHweafOimDqLLN%2F8MYWuriogyEOGdo%2B11DnLsgRemtZ3JRExWXTMVUHeNrT77ph64i8zbXINSmOu5IU1i465KshCQ7uviaknbngTc9Qefay5Uhtp87PomKuCnK7xW22Mm3SVQ3KrZe8kqbmaKs8ui445KYgAnKZGymrgwRShP%2FeSDp25WlkbQejYar1dPeRRGVx%2FQEwsWhJz1V4LQejYFZT98LC%2F6dYM7mM7dJPEXFEXQT7UtGVvUvd7SuEbNVcr6iTILkN7Rmdwrw3dMFe1EaTNkK5icAb3kmiWtOYqXMddQYALgPtkPpAgOku5KzXLT62LvAltkhCj7Q2aK3cFoeOo2qHIiakWS%2FkLVbiPnFaa2qx2GO71cIPmyk1BZEcOfdjpsqAEACdbwlZt5spZQaYYrr8lKAkqlrhL%2B6LOw4i5claQkYbrd4mULwqJ%2F1LmsdOsfhU9pKSOSrQ7L4hhf7pdzvMFJUO9wZuC5h7RPCNnBemltlDfBJ6VMyOBQ6gV4r7KCOI6lj2S8gmiDnVKYpjHgKslQC2oGMByJwRRXtkfI%2FVerJooOCSI6XyiNQLENVwS5F1D3TuCCoFDgixIemrXZVwSZIjyS4WR%2FQw%2FhxS4yhJf0KPAS2KqgN5BxcCVEVIX8IKUCy9IyfCClIzSC6I2nU4NagJlFUQlnvkissRtevBB2SizIJ9pyq0MKg5lFEQ5Ek1h%2FJV793BBkH6GbG9y2qhHUGEooyCq7Bu5NKpklFmQ%2FipIeZdK0r8gbeJJFymtIKE6lXIelk2Qp9IKUjcw7%2FvMy%2BJmEubpBbEfgfvV8IxmBs0GuMIL0lDkpTAxaDZqotbFHNXeZAEtlt%2Br2h3NkdJMUXS%2FiVFbQYDewI2Ro3VRXsmyAedqItS1gqjELBI49rJpyKqFwjpHP22WnCjhA0TZRl8CT8cJYlgA3KwpV9Qv9eRF8xMGGIap5Fk0uU56G%2FLlbq%2BZIOty%2B%2BFIlcLoY3XjVZpD%2BjoOaxKA6bzCVeA923G8LHNQPS4nVDVJJXXn8TZprvEz1WK%2FyoPS%2FOw%2FaXKJaP5vYiQ5y9%2BaXzdo6UZS47KxQ%2BUN1ibKLFPSFzlJO92QK32MSmjs6mcWcJM6eFrciPB4PB6Px%2BPxeDwej8fj8XiCYvgfmdGLzXmrOA4AAAAASUVORK5CYII%3D&labelColor=3E93C4&color=6A6A6A">
+        <img alt="Request New Feature" src="https://img.shields.io/badge/Request%20New%20Feature-uptrain?logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAAGQAAABkCAYAAABw4pVUAAAACXBIWXMAAAsTAAALEwEAmpwYAAAG%2BElEQVR4nO2da6gWRRjHN1NLKy1Tu2B5CjEsMiO0wEiqoxhmZQUJ5YfyQ5FhdLEiIiItLQtRIswiMIvKNDOTCosyCzsVGWiXLykVdrESQz1aXn7xcObAsmdmdvc9715md37wftAzszuz%2F3eemX3mmecNAo%2FH4%2FF4PKUF6AmMBxYDG4E1wLii21VXEZYAf9KV%2F4BLim5n3UWIsqboNlcO0osQ5sui218J6J4IYRYX3RdnAY4ELgYWAr%2FRHFqL7pdTkI0IncjI6ll0H%2BsuQpjn8ujIWGAacA9wf0GfmcCwBuaEVnlI3ZwTOtkNvAq8YCkzPishzlQ3%2FoviaAdWADcAxxQswrVAH3UP%2BXc%2B5kp16EngX%2BotwmvAdZ0ihO7VR%2F1dx5Jmi3EC8AHFsAd4ADi%2BbCJE7isjJXtzBfQCPqIYfgHOSTif5S5CpA35mCu1%2BiiCfcDIHEXYk1aE3M0VMAI4GNORA8BmYFuCTsuy8mtgf4KyszXt6VGECMD54hgE%2Bhr%2BLvVzMVfSWBubwktOYAKw0yDaLaFyA4G1luseAk6KtGU48B05jgRgMPBpqK58CS5N8ZyaZ67UMNxr6dgB3fpfHrym7HxNuX7A74Zrf6MpL%2BLnZo7kCwF8a3jIfYswV5NiOrnZUE%2B%2B%2FVG0mzPA64Zrr46UG0K%2Bc4KIscVy7XFFmKs7Yzq8zVDvDE3ZSYayaw3XXh8pd6IyY0mR0TsbGNRAv%2BPEEM7L1VypGz2RoOMTNPXmasq9pSk3XL3s6djZwHymQxYPS4HRTRTjk4Tmqrm%2BK%2BCZBB3eqeaMgWpkzLWsypYBZwP9gasSrMouirTnWLVH3ainoE353Y6yTOBxYsjfB%2BdurlIIkiXvWL7F4lT8qcHr%2FgHMA4ZGxJClu43vgVMSzoGZ%2BK6KFkS4LcaDIH6tDTTGAeUbm5xwZESX4X1zM1clEuQgMD1BW0cBz1vmpO7QRYwE5qq1qoJ08n6SuCZgADAL2EqGYuS6uiqpIJ38oJbjVvd7yMUiAWqHaYwuc0ZCc5VNIENJBenkH%2BXPGpGgH8PUJK5z6aQWQ13zekvdy5suRowg69W3rwyfy0wOP01%2FjgNmJPSHTY65lslc7cgskMEiyPLAYYAjlJirLOZshaV%2BvqurqgsSRoliWt0NLY25qpEgrZaHO8dQJ7%2BXwboJIlje0GU%2BODooenVVQ0FmWEbJtFKYK9cFoSPyZApwl0QlJlh9yTJaR1vhqyvXBaHDrHweafOimDqLLN%2F8MYWuriogyEOGdo%2B11DnLsgRemtZ3JRExWXTMVUHeNrT77ph64i8zbXINSmOu5IU1i465KshCQ7uviaknbngTc9Qefay5Uhtp87PomKuCnK7xW22Mm3SVQ3KrZe8kqbmaKs8ui445KYgAnKZGymrgwRShP%2FeSDp25WlkbQejYar1dPeRRGVx%2FQEwsWhJz1V4LQejYFZT98LC%2F6dYM7mM7dJPEXFEXQT7UtGVvUvd7SuEbNVcr6iTILkN7Rmdwrw3dMFe1EaTNkK5icAb3kmiWtOYqXMddQYALgPtkPpAgOku5KzXLT62LvAltkhCj7Q2aK3cFoeOo2qHIiakWS%2FkLVbiPnFaa2qx2GO71cIPmyk1BZEcOfdjpsqAEACdbwlZt5spZQaYYrr8lKAkqlrhL%2B6LOw4i5claQkYbrd4mULwqJ%2F1LmsdOsfhU9pKSOSrQ7L4hhf7pdzvMFJUO9wZuC5h7RPCNnBemltlDfBJ6VMyOBQ6gV4r7KCOI6lj2S8gmiDnVKYpjHgKslQC2oGMByJwRRXtkfI%2FVerJooOCSI6XyiNQLENVwS5F1D3TuCCoFDgixIemrXZVwSZIjyS4WR%2FQw%2FhxS4yhJf0KPAS2KqgN5BxcCVEVIX8IKUCy9IyfCClIzSC6I2nU4NagJlFUQlnvkissRtevBB2SizIJ9pyq0MKg5lFEQ5Ek1h%2FJV793BBkH6GbG9y2qhHUGEooyCq7Bu5NKpklFmQ%2FipIeZdK0r8gbeJJFymtIKE6lXIelk2Qp9IKUjcw7%2FvMy%2BJmEubpBbEfgfvV8IxmBs0GuMIL0lDkpTAxaDZqotbFHNXeZAEtlt%2Br2h3NkdJMUXS%2FiVFbQYDewI2Ro3VRXsmyAedqItS1gqjELBI49rJpyKqFwjpHP22WnCjhA0TZRl8CT8cJYlgA3KwpV9Qv9eRF8xMGGIap5Fk0uU56G%2FLlbq%2BZIOty%2B%2BFIlcLoY3XjVZpD%2BjoOaxKA6bzCVeA923G8LHNQPS4nVDVJJXXn8TZprvEz1WK%2FyoPS%2FOw%2FaXKJaP5vYiQ5y9%2BaXzdo6UZS47KxQ%2BUN1ibKLFPSFzlJO92QK32MSmjs6mcWcJM6eFrciPB4PB6Px%2BPxeDwej8fj8XiCYvgfmdGLzXmrOA4AAAAASUVORK5CYII%3D&labelColor=5B92E9&color=6A6A6A">
+    </a>
+    <a href="https://demo.uptrain.ai/benchmark">
+      <img alt="Daily Monitoring" src="https://img.shields.io/badge/Daily%20Monitoring-uptrain?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAGQAAABkCAYAAABw4pVUAAAACXBIWXMAAAsTAAALEwEAmpwYAAAFUUlEQVR4nO2daahVVRTHt2WDls3RQDYXRUZBkRkRjdAraPjSAJUUKVSE0QuiQZ4FmRj2lMwwqGgitZTq5cvEIipKpGgymogwCrKs7IOkDf5i9ZYorzvsM+99zvrB/XjWXfv+z9ln7zXs65xhGIZhGIZhGIZRCsD2wOXAIuA94P2MH7HxLHBBOSOoEcBewJsUx/PATlWPMxqAQYpnXtXjjALgDMrhb+CwqscbPMAMymNy1eMNHuDxEgXpq3q8wQP0lSjIPVWPN3iAY4HNJkhAAHNMkIAAdgBml/Ck2JSVBOAo4HbgYWD+sM9KEyQQZP8ArDVBAgDYDfjUpqwAAEYCy+0dEgjAPHupBwJwq62yAgHo0WCgLXurBjgOWG/7kAAA9gfW2MYwAIDRwKoUYkiq9pdG7NQZSq3eD3wCrANWAwuBOyRXDRyU0/dsB7yQQoxvgf2AH2svCHCO50BFqBXALGAicCKwY8Lvmp5CjN+BcXp9fQXRu3VqxlXOn8DHwFNAL3AusG+b7xMRkyK+9Wxj42vP625zMQHsAyyjOH4AXtW07RXAZcCmFHZuHub3y57XxVMSBEwAviN85rbw/SKP62T1NtLFADBFp5nQWdbuRwWe6HDdRqlucZFEUqWILAZWi79d3n13tdhUfgSMd6EDnAB8RRys9a2pAnbRWq+Lt6zCgge4BthAHPwBnObqCLCzpkNjYTNwlasjwNG6N8jCr/opi2mujuh8+lvGH2cVcKjaO1A3e1N08/dZAeFyaUsY4eqEhDC0vCbrtDFLSnU8XqbjpX5Wq0be0fBGGt6V6dXVCWCsRkKzsB64NIMPI4DDxYZMP8AS4Jsu9VeDnZa3UQKcD/ycUYwPgSML3P+cDtykT5NMT/3Aea5O6B0phWb/ZBRD3gujqx5P1Ghg8LUc1vzXVz2W6AGO0GRNFr4AjneRA+ypwcZrgbOS5mby6l6VeE0WJAs4xsVfVDddA4nb8n2WhUkaRy7JIMSm4bmFWAGe6TBOWdVdGXpvxZoooqAeABd6jFciDHu4ogEeTSGGrPX3djWBoWWzDxNDK7mU8MbdkjtwNQL/GN2MMpw5RJer3ZDKjLNdDQG+9BRkdlkO3dLFkbckIOhqCqEJok5NalHBt0HTmnEk9+skiDq2q1YUTtaA3u6uARCqIE0FEyQsTJDAaIwgDFWWS/X7B5pYegO4ofSAXRcaIYiWlq5rM7CVIe30ay+I5lZ+6jK4V1wgNEEQ3yOTTnEB0ARB3vYc4J0uAJogyOcxDZAGCCLpXB/muAAwQbZigtTpCWGobUCqIhcAD0pRQko7NmVlEUSDoFLF2IqBpEFREyS7IC/SmUETpKQpCzjT03ZP9FOWtglcJ/sDzYmMDVCQfk/b86MVRBse723R8y2dtQ8kzRgWLMgiT9uDMQvSn9fdVoIgSzxtL49SEKnH9ax2PzWBTRMkLcB9ed/NJkgGgOc8BVmawKY9IWkBFnsKsiKBTRMkLSaIC+6lbk8IJsgWbNlrT8j/sSdkK/aEtLg7JJeQdyhCTiH1YWaB/g4U4G8p/SEzPZ15JIFN3zMMbyzwb/IeSmDzpWD+Nk9CIp7OeJ+SAFztYe8v4IAU/p7s6a/3kXzS0Olhb2O7k1FzR09e6MRAkpN1tNX69S42p2bw97EuthekiHZ3OzSh15UFMAp4uo0ji9P0oOup1kvb9ClOy9KnKH8ULFNom0No5DDLUSlsjtF++1ZPRnliDHPqJA02PqlF0hNymhL75HhWPRT54Hy8/c/2MXps+Vzt9BqXU/S7V3+HSaVNU4ZhGIZhGIZhGIZhGIbhquVfiiAaCf/Kq/8AAAAASUVORK5CYII=&labelColor=35B9D2&color=6A6A6A">
     </a>
 </p>
 
 <p align="center">
   <a href="https://github.com/uptrain-ai/uptrain/releases">
     <img alt="GitHub Release" src="https://img.shields.io/github/v/release/uptrain-ai/uptrain?labelColor=6A6A6A&color=CC766E">
   </a>
@@ -36,18 +79,14 @@
 </p>
 
 <h4 align="center">
   <video src="https://github.com/uptrain-ai/uptrain/assets/43818888/68a3b169-2217-446b-93b2-96b48ec7201d" alt="Demo of UpTrain's LLM evaluations with scores for hallucinations, retrieved-context quality, response tonality for a customer support chatbot" autoplay>
 </h4>
 
 
-
-
-
-
 **[UpTrain](https://uptrain.ai)** is an open-source unified platform to evaluate and improve Generative AI applications. We provide grades for [20+ preconfigured evaluations](https://github.com/uptrain-ai/uptrain?tab=readme-ov-file#pre-built-evaluations-we-offer-) (covering language, code, embedding use cases), perform [root cause analysis](https://github.com/uptrain-ai/uptrain/blob/main/examples/root_cause_analysis/rag_with_citation.ipynb) on failure cases and give insights on how to resolve them.    
 
 <br />
 
 # Key Features 🔑
 
 <img width="1088" alt="Interactive Dashboards" src="https://github.com/uptrain-ai/uptrain/assets/36454110/eb1c8239-dd99-4e66-ba8a-cbaee2beec10">
@@ -212,14 +251,16 @@
 |[Jailbreak Detection](https://docs.uptrain.ai/predefined-evaluations/safeguarding/jailbreak) | Grades whether the user's prompt is an attempt to jailbreak (i.e. generate illegal or harmful responses). |
 
 <img width="1088" alt="evaluate the clarity of user queries" src="https://github.com/uptrain-ai/uptrain/assets/36454110/50ed622f-0b92-468c-af48-2391ff6ab8e0">
 
 | Eval | Description |
 | ---- | ----------- |
 |[Sub-Query Completeness](https://docs.uptrain.ai/predefined-evaluations/query-quality/sub-query-completeness) | Evaluate whether all of the sub-questions generated from a user's query, taken together, cover all aspects of the user's query or not |
+| [Multi-Query Accuracy](https://docs.uptrain.ai/predefined-evaluations/query-quality/multi-query-accuracy) | Evaluate whether the variants generated accurately represent the original query |
+
 
 <br />
 
 # Integrations 🤝
 
 | Eval Frameworks  | LLM Providers | LLM Packages | Serving frameworks | LLM Observability | Vector DBs |
 | ------------- | ------------- | ------------- | ------------- | ------------- |  ------------- |
@@ -229,14 +270,23 @@
 | | [Mistral](https://docs.uptrain.ai/llms/mistral) | | Replicate  |
 | |  | |  HuggingFace  |
 
 More integrations are coming soon. If you have a specific integration in mind, please let us know by [creating an issue](https://github.com/uptrain-ai/uptrain/issues).
 
 <br />
 
+# Monitoring Prompt Drift in LLMs: Benchmark by UpTrain
+
+Most popular LLMs like GPT-4, GPT-3.5-turbo, Claude-2.1 etc., are closed-source, i.e. exposed via an API with very little visibility on what happens under the hood. There are many reported instances of prompt drift (or GPT-4 becoming lazy) and research work exploring the degradation in model quality. This benchmark is an attempt to track the change in model behaviour by evaluating its response on a fixed dataset.
+
+<img width="1316" alt="image" src="https://github.com/uptrain-ai/uptrain/assets/43818888/65b7e8c3-3f5e-48bb-98c1-88208520945b">
+
+You can find the benchmark [here](https://demo.uptrain.ai/benchmark).
+
+
 # Resources 💡
 
 1. [How to evaluate your LLM application](https://blog.uptrain.ai/how-to-evaluate-your-llm-applications)
 1. [How to detect jailbreaks](https://blog.uptrain.ai/llm-jailbreak/)
 1. [Dealing with hallucinations](https://blog.uptrain.ai/dealing-with-hallucinations-in-llms-a-deep-dive/)
 
 <br />
```

#### html2text {}

```diff
@@ -1,11 +1,30 @@
+Metadata-Version: 2.1 Name: uptrain Version: 0.7.0 Summary: UpTrain - tool to
+evaluate LLM applications on aspects like factual accuracy, response quality,
+retrieval quality, tonality, etc. Maintainer-email: UpTrain AI Team
+uptrain.ai> License: Apache-2.0 Project-URL: Homepage, https://uptrain.ai
+Project-URL: Repository, https://github.com/uptrain-ai/uptrain Keywords:
+uptrain,ai,LLM,evaluation,hallucinations,observability,response quality
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Description-
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: pydantic
+Requires-Dist: pydantic-settings Requires-Dist: loguru Requires-Dist:
+lazy_loader Requires-Dist: networkx Requires-Dist: polars>=0.18 Requires-Dist:
+pandas Requires-Dist: numpy>=1.23.0 Requires-Dist: httpx>=0.24.1 Requires-Dist:
+plotly>=5.0.0 Requires-Dist: aiolimiter>=1.1 Requires-Dist: openai>=1.6.1
+Requires-Dist: fsspec Requires-Dist: litellm Requires-Dist: pyyaml Requires-
+Dist: json5 Requires-Dist: python-docx Requires-Dist: pymupdf Requires-Dist:
+faiss-cpu Provides-Extra: test Requires-Dist: pytest>=7.0; extra == "test"
   ****** _[[_LL_oo_gg_oo_ _oo_ff_ _UU_pp_TT_rr_aa_ii_nn_ _--_ _aa_nn_ _oo_pp_ee_nn_--_ss_oo_uu_rr_cc_ee_ _pp_ll_aa_tt_ff_oo_rr_mm_ _tt_oo_ _ee_vv_aa_ll_uu_aa_tt_ee_ _aa_nn_dd_ _ii_mm_pp_rr_oo_vv_ee_ _LL_LL_MM
                                _aa_pp_pp_ll_ii_cc_aa_tt_ii_oo_nn_ss_]] ******
                         _[_T_r_y_ _o_u_t_ _E_v_a_l_u_a_t_i_o_n_]_[_R_e_a_d_ _D_o_c_s_]
-_[_S_l_a_c_k_ _C_o_m_m_u_n_i_t_y_]_[_R_e_q_u_e_s_t_ _N_e_w_ _F_e_a_t_u_r_e_]
+_[_S_l_a_c_k_ _C_o_m_m_u_n_i_t_y_]_[_R_e_q_u_e_s_t_ _N_e_w_ _F_e_a_t_u_r_e_]_[_D_a_i_l_y_ _M_o_n_i_t_o_r_i_n_g_]
   _[_G_i_t_H_u_b_ _R_e_l_e_a_s_e_]_[_G_i_t_H_u_b_ _c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]_[_G_i_t_H_u_b_ _L_i_c_e_n_s_e_]_[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]
 **[UpTrain](https://uptrain.ai)** is an open-source unified platform to
 evaluate and improve Generative AI applications. We provide grades for [20+
 preconfigured evaluations](https://github.com/uptrain-ai/uptrain?tab=readme-ov-
 file#pre-built-evaluations-we-offer-) (covering language, code, embedding use
 cases), perform [root cause analysis](https://github.com/uptrain-ai/uptrain/
 blob/main/examples/root_cause_analysis/rag_with_citation.ipynb) on failure
@@ -134,15 +153,18 @@
 LLM reveal its system prompts. | |[Jailbreak Detection](https://
 docs.uptrain.ai/predefined-evaluations/safeguarding/jailbreak) | Grades whether
 the user's prompt is an attempt to jailbreak (i.e. generate illegal or harmful
 responses). | [evaluate the clarity of user queries]| Eval | Description | | --
 -- | ----------- | |[Sub-Query Completeness](https://docs.uptrain.ai/
 predefined-evaluations/query-quality/sub-query-completeness) | Evaluate whether
 all of the sub-questions generated from a user's query, taken together, cover
-all aspects of the user's query or not |
+all aspects of the user's query or not | | [Multi-Query Accuracy](https://
+docs.uptrain.ai/predefined-evaluations/query-quality/multi-query-accuracy) |
+Evaluate whether the variants generated accurately represent the original query
+|
 # Integrations ð¤ | Eval Frameworks | LLM Providers | LLM Packages | Serving
 frameworks | LLM Observability | Vector DBs | | ------------- | ------------- |
 ------------- | ------------- | ------------- | ------------- | | [OpenAI
 Evals](https://docs.uptrain.ai/tutorials/openai-evals) | [OpenAI](https://
 docs.uptrain.ai/llms/openai) | [LlamaIndex](https://docs.uptrain.ai/
 integrations/framework/llamaindex-methods/overview) | [Ollama](https://
 docs.uptrain.ai/llms/ollama) | [Langfuse](https://docs.uptrain.ai/integrations/
@@ -154,15 +176,22 @@
 docs.uptrain.ai/llms/claude) | | [Anyscale](https://docs.uptrain.ai/llms/
 anyscale) | [Zeno](https://docs.uptrain.ai/integrations/observation-tools/zeno)
 | [Chroma](https://docs.uptrain.ai/integrations/vector_db/chroma) | | |
 [Mistral](https://docs.uptrain.ai/llms/mistral) | | Replicate | | | | |
 HuggingFace | More integrations are coming soon. If you have a specific
 integration in mind, please let us know by [creating an issue](https://
 github.com/uptrain-ai/uptrain/issues).
-# Resources ð¡ 1. [How to evaluate your LLM application](https://
+# Monitoring Prompt Drift in LLMs: Benchmark by UpTrain Most popular LLMs like
+GPT-4, GPT-3.5-turbo, Claude-2.1 etc., are closed-source, i.e. exposed via an
+API with very little visibility on what happens under the hood. There are many
+reported instances of prompt drift (or GPT-4 becoming lazy) and research work
+exploring the degradation in model quality. This benchmark is an attempt to
+track the change in model behaviour by evaluating its response on a fixed
+dataset. [image]You can find the benchmark [here](https://demo.uptrain.ai/
+benchmark). # Resources ð¡ 1. [How to evaluate your LLM application](https://
 blog.uptrain.ai/how-to-evaluate-your-llm-applications) 1. [How to detect
 jailbreaks](https://blog.uptrain.ai/llm-jailbreak/) 1. [Dealing with
 hallucinations](https://blog.uptrain.ai/dealing-with-hallucinations-in-llms-a-
 deep-dive/)
 # Why we are building UpTrain ð¤ Having worked with ML and NLP models for the
 last 8 years, we were continuosly frustated with numerous hidden failures in
 our models which led to us building UpTrain. UpTrain was initially started as
```

### Comparing `uptrain-0.6.9/pyproject.toml` & `uptrain-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "uptrain"
-version = "0.6.9"
+version = "0.7.0"
 description = "UpTrain - tool to evaluate LLM applications on aspects like factual accuracy, response quality, retrieval quality, tonality, etc."
 readme = "README.md"
 maintainers = [{ name = "UpTrain AI Team", email = "oss@uptrain.ai" }]
 license = {text = "Apache-2.0"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -30,15 +30,18 @@
     "httpx>=0.24.1",
     "plotly>=5.0.0",
     "aiolimiter>=1.1",
     "openai>=1.6.1",
     "fsspec",
     "litellm",
     "pyyaml",
-    "json5"
+    "json5",
+    "python-docx",
+    "pymupdf",
+    "faiss-cpu",
 ]
 
 [project.urls]
 Homepage = "https://uptrain.ai"
 Repository = "https://github.com/uptrain-ai/uptrain"
 
 [project.scripts]
```

### Comparing `uptrain-0.6.9/tests/test_builtins.py` & `uptrain-0.7.0/tests/test_builtins.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     CheckCodeHallucination,
     CheckConversationSatisfaction,
     CheckGuidelineAdherence,
     CheckResponseMatching,
     CheckPromptInjection,
     CheckJailbreakDetection,
     CheckSubQueryCompleteness,
+    CheckMultiQueryAccuracy,
 )
 
 # Enter your OpenAI API key here if it is not already set as an environment variable
 openai_api_key = os.environ.get("OPENAI_API_KEY")
 
 settings = Settings(openai_api_key=openai_api_key)
 
@@ -194,21 +195,21 @@
 
 
 def test_check_response_matching():
     check = CheckResponseMatching()
     output = check.setup(settings).run(response_matching_dataset)
     assert isinstance(output, pl.DataFrame)
     assert (
-        "score_response_matching" in output.columns
+        "score_response_match" in output.columns
         and "explanation_response_matching" in output.columns
     )
     assert (
-        output["score_response_matching"].dtype == pl.Float64
-        and len(output["score_response_matching"])
-        - output["score_response_matching"].null_count()
+        output["score_response_match"].dtype == pl.Float64
+        and len(output["score_response_match"])
+        - output["score_response_match"].null_count()
         > 0
     )
     assert (
         output["explanation_response_matching"].dtype == pl.Utf8
         and len(output["explanation_response_matching"])
         - output["explanation_response_matching"].null_count()
         > 0
@@ -524,49 +525,50 @@
 
 # -----------------------------------------------------------
 # Custom Evaluations
 # -----------------------------------------------------------
 
 
 def test_check_guideline_adherence():
+    guideline_name = "No Numbers"
     check = CheckGuidelineAdherence(
         guideline="The response should not contain any numbers or statistic",
-        guideline_name="guideline",
+        guideline_name=guideline_name,
         response_schema=None,
     )
     output = check.setup(settings).run(dataset)
     assert isinstance(output, pl.DataFrame)
     assert (
-        "score_guideline_adherence" in output.columns
-        and "explanation_guideline_adherence" in output.columns
+        f"score_{guideline_name}_adherence" in output.columns
+        and f"explanation_{guideline_name}_adherence" in output.columns
     )
     assert (
-        output["score_guideline_adherence"].dtype == pl.Float64
-        and len(output["score_guideline_adherence"])
-        - output["score_guideline_adherence"].null_count()
+        output[f"score_{guideline_name}_adherence"].dtype == pl.Float64
+        and len(output[f"score_{guideline_name}_adherence"])
+        - output[f"score_{guideline_name}_adherence"].null_count()
         > 0
     )
     assert (
-        output["explanation_guideline_adherence"].dtype == pl.Utf8
-        and len(output["explanation_guideline_adherence"])
-        - output["explanation_guideline_adherence"].null_count()
+        output[f"explanation_{guideline_name}_adherence"].dtype == pl.Utf8
+        and len(output[f"explanation_{guideline_name}_adherence"])
+        - output[f"explanation_{guideline_name}_adherence"].null_count()
         > 0
     )
 
 
 # # -----------------------------------------------------------
 # # Compare response with ground truth
 # # -----------------------------------------------------------
 
 # def test_check_response_matching():
 #     check = CheckResponseMatching()
 #     output = check.setup(settings).run(dataset)
 #     assert isinstance(output, pl.DataFrame)
-#     assert "score_response_matching" in output.columns and "explanation_response_matching" in output.columns
-#     assert output["score_response_matching"].dtype == pl.Float64 and len(output["score_response_matching"]) - output["score_response_matching"].null_count() > 0
+#     assert "score_response_match" in output.columns and "explanation_response_matching" in output.columns
+#     assert output["score_response_match"].dtype == pl.Float64 and len(output["score_response_match"]) - output["score_response_match"].null_count() > 0
 #     assert output["explanation_response_matching"].dtype == pl.Utf8 and len(output["explanation_response_matching"]) - output["explanation_response_matching"].null_count() > 0
 
 
 # -----------------------------------------------------------
 # Security
 # -----------------------------------------------------------
 
@@ -674,7 +676,60 @@
     )
     assert (
         output["explanation_sub_query_completeness"].dtype == pl.Utf8
         and len(output["explanation_sub_query_completeness"])
         - output["explanation_sub_query_completeness"].null_count()
         > 0
     )
+
+
+# -----------------------------------------------------------
+# Multi Query
+# -----------------------------------------------------------
+    
+multi_query_dataset = pl.DataFrame(
+    {
+        "question": [
+            "What are the main causes of climate change?",
+            "What are the benefits of AI?",
+            "What are the differences between Python and Java?",
+        ],
+        "variants": [
+            """
+            1. What are the main causes of climate change?
+            2. What are the effects of climate change?
+            3. What are the solutions to climate change?
+            """,
+            """
+            1. What are the benefits of AI?
+            2. What is AI?
+            3. What are the regulations of AI?
+            """,
+            """
+            1. What are the differences between Python and Java?
+            2. What are the similarities between Python and Java?
+            """,
+        ],
+    }
+)
+
+
+def test_check_multi_query_accuracy():
+    check = CheckMultiQueryAccuracy()
+    output = check.setup(settings).run(multi_query_dataset)
+    assert isinstance(output, pl.DataFrame)
+    assert (
+        "score_multi_query_accuracy" in output.columns
+        and "explanation_multi_query_accuracy" in output.columns
+    )
+    assert (
+        output["score_multi_query_accuracy"].dtype == pl.Float64
+        and len(output["score_multi_query_accuracy"])
+        - output["score_multi_query_accuracy"].null_count()
+        > 0
+    )
+    assert (
+        output["explanation_multi_query_accuracy"].dtype == pl.Utf8
+        and len(output["explanation_multi_query_accuracy"])
+        - output["explanation_multi_query_accuracy"].null_count()
+        > 0
+    )
```

### Comparing `uptrain-0.6.9/tests/test_custom_ops.py` & `uptrain-0.7.0/tests/test_custom_ops.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/tests/test_operators.py` & `uptrain-0.7.0/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/__init__.pyi` & `uptrain-0.7.0/uptrain/__init__.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     "ResponseMatching",
     "Settings",
     "EvalLlamaIndex",
     "EvalPromptfoo",
     "CustomPromptEval",
     "RcaTemplate",
     "JailbreakDetection",
+    "EvalAssistant"
 ]
 
 from .framework.base import Settings
 from .framework.remote import APIClient
 from .framework.evals import (
     Evals,
     CritiqueTone,
@@ -25,7 +26,9 @@
     CustomPromptEval,
     JailbreakDetection,
 )
 from .framework.evalllm import EvalLLM
 from .framework.rca_templates import RcaTemplate
 from .integrations.llama_index import EvalLlamaIndex
 from .integrations.promptfoo import EvalPromptfoo
+
+from .framework.eval_assistant.assistant_evals_utils import EvalAssistant
```

### Comparing `uptrain-0.6.9/uptrain/cli.py` & `uptrain-0.7.0/uptrain/cli.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/dashboard/backend/app.py` & `uptrain-0.7.0/uptrain/dashboard/backend/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,26 +3,29 @@
  
 NOTE: Make sure all public api methods make use of `user_name` to only 
 work with rows specific to the user.
 """
 
 from __future__ import annotations
 from contextlib import contextmanager
-from datetime import datetime, timedelta
 import datetime as dt
 import json
 import io
 import os
 import typing as t
+import copy 
+import random
 import uvicorn
 import polars as pl
 import sys
 
-from uptrain.framework import Settings, EvalLLM
-from uptrain.operators import ColumnOp, ColumnOp, Table, LineChart, Histogram
+from uptrain.operators import JsonReader, JsonWriter
+
+from uptrain import Settings as UserSettings
+from uptrain import EvalLLM
 
 import pandas as pd
 import dateutil.parser
 
 from fastapi import (
     APIRouter,
     Depends,
@@ -33,36 +36,38 @@
     File,
     Security,
     Request,
 )
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.security.api_key import APIKeyHeader
 
+def get_uuid():
+    import uuid
+    return str(uuid.uuid4().hex)
 
 from loguru import logger
 from sqlalchemy.orm import Session
 
-from uptrain.utilities.db import create_database, ModelDataset, ModelUser, ModelPrompt
+from uptrain.utilities.db import create_database, ModelUser, ModelPrompt, ModelProject, ModelProjectDataset, ModelProjectRun
 from uptrain.utilities.utils import (
-    get_sqlite_utils_db,
     _get_fsspec_filesystem,
-    convert_project_to_polars,
-    convert_project_to_dicts,
     checks_mapping,
     create_dirs,
-    get_current_datetime,
 )
-from uptrain.utilities import polars_to_pandas
 
 from uptrain.utilities import app_schema
 
 
 def _row_to_dict(row):
     return {k: v for k, v in row.__dict__.items() if not k.startswith("_")}
 
+def intersection(lst1, lst2):
+    lst3 = [value for value in lst1 if value in lst2]
+    return lst3
+
 
 # -----------------------------------------------------------
 # Dependencies
 # -----------------------------------------------------------
 
 DATABASE_PATH = "/data/uptrain_data/"
 # security
@@ -134,29 +139,29 @@
 # -----------------------------------------------------------
 # Routers
 # -----------------------------------------------------------
 
 router_public = APIRouter(dependencies=[Depends(validate_api_key_public)])
 router_internal = APIRouter()
 
-# -----------------------------------------------------------
-# Internal API
-# -----------------------------------------------------------
+# # -----------------------------------------------------------
+# # Internal API
+# # -----------------------------------------------------------
 
 
-@router_internal.post("/user")
-def add_user(user: app_schema.UserCreate, db: Session = Depends(get_db)):
-    """Add a new user."""
-    name = user.name
-    try:
-        db_user = _create_user(db, name)
-        return db_user
-    except Exception as exc:
-        logger.exception(exc)
-        raise HTTPException(status_code=400, detail=f"Error creating user: {name}")
+# @router_internal.post("/user")
+# def add_user(user: app_schema.UserCreate, db: Session = Depends(get_db)):
+#     """Add a new user."""
+#     name = user.name
+#     try:
+#         db_user = _create_user(db, name)
+#         return db_user
+#     except Exception as exc:
+#         logger.exception(exc)
+#         raise HTTPException(status_code=400, detail=f"Error creating user: {name}")
 
 
 # -----------------------------------------------------------
 # Public API
 # -----------------------------------------------------------
 
 # -----------------------------------------------------------
@@ -175,508 +180,445 @@
     else:
         return {
             "id": user_id,
             "user_name": "open-source user",
             "api_key": "default_key",
         }
 
-
-@router_public.get("/get_project_data", response_model=app_schema.ProjectData)
-def get_project_data(
-    project_name: str,
-    num_days: int = 7,
+@router_public.get("/get_data", response_model=app_schema.ProjectData)
+def get_data(
+    evaluation_id: str,
     db: Session = Depends(get_db),
     user_id: str = Depends(validate_api_key_public),
 ):
-    """Get all the data for a particular project_name for the given user."""
-    projects = get_projects_list(num_days=num_days, db=db, user_id=user_id)
+    """Get all the data for a particular evaluation for the given user.
+    """
+    user = db.query(ModelUser).filter_by(id=user_id).first()
+    if user is None:
+        raise HTTPException(status_code=403, detail="Invalid user name")
+    else:
+        user_name = user.name
 
-    for project in projects.data:
-        if project["project"] == project_name:
-            run_via = project["run_via"]
-            if run_via == "project" or run_via == "experiment":
-                if run_via == "project":
-                    query = f"""
-                        SELECT *
-                        FROM results
-                        WHERE project = '{project_name}' AND metadata NOT LIKE '%prompt_version%' AND metadata NOT LIKE '%uptrain_experiment_columns%' AND timestamp > datetime('now', '-{num_days} days')
-                        """
-                else:
-                    query = f"""
-                        SELECT *
-                        FROM results
-                        WHERE project = '{project_name}' AND metadata LIKE '%uptrain_experiment_columns%' AND timestamp > datetime('now', '-{num_days} days')
-                        """
-                fpath = os.path.join(
-                    DATABASE_PATH, "uptrain-eval-results", f"{user_id}.db"
-                )
-                if not os.path.exists(fpath):
-                    raise HTTPException(
-                        status_code=404, detail="No evaluations run yet for this user"
-                    )
-                DB = get_sqlite_utils_db(fpath)
-
-                buffer = io.StringIO()
-                for row in DB.query(query):
-                    buffer.write(json.dumps(row) + "\n")
-                buffer.seek(0)
-                data = []
-                for line in buffer:
-                    details = json.loads(line)
-                    for key in details:
-                        try:
-                            details[key] = json.loads(details[key])
-                        except Exception:
-                            pass
-                    data.append(details)
-                scores = [
-                    col[6:]
-                    for col in data[0]["checks"].keys()
-                    if col.startswith("score_")
-                ]
-                if run_via == "project":
-                    return app_schema.ProjectData(
-                        data=[
-                            data,
-                            None,
-                            project["latest_timestamp"][:10],
-                            None,
-                            scores,
-                        ],
-                        project_name=project_name,
-                    )
-                else:
-                    exp_data = convert_project_to_polars(data)
-                    exp_column = str(exp_data["uptrain_experiment_columns"][0][0])
-
-                    plot_data = {}
-                    for col in scores:
-                        col_name = "score_" + col
-                        plot_data.update(
-                            {
-                                col: exp_data.group_by(
-                                    [exp_column], maintain_order=True
-                                )
-                                .agg(pl.col(col_name))
-                                .to_dicts()
-                            }
-                        )
-
-                    columns = exp_data.columns
-                    columns.remove("question")
-                    display_data = (
-                        exp_data.group_by(["question"], maintain_order=True)
-                        .agg(pl.col(col) for col in columns)
-                        .to_dicts()
-                    )
-                    unqiue_values = list(set(exp_data[exp_column].to_list()))
-                    return app_schema.ProjectData(
-                        data=[
-                            display_data,
-                            None,
-                            project["latest_timestamp"][:10],
-                            None,
-                            scores,
-                            unqiue_values,
-                            exp_column,
-                            plot_data,
-                        ],
-                        project_name=project_name,
-                    )
-
-
-@router_public.get("/get_prompt_data", response_model=app_schema.ProjectData)
-def get_prompt_data(
-    project_name: str,
-    num_days: int = 7,
-    db: Session = Depends(get_db),
-    user_id: str = Depends(validate_api_key_public),
-):
-    """Get all the data for a particular project_name for the given user."""
-    projects = get_projects_list(num_days=num_days, db=db, user_id=user_id)
+    project_run = db.query(ModelProjectRun).filter_by(id=evaluation_id).first()
 
-    for project in projects.data:
-        if project["project"] == project_name:
-            run_via = project["run_via"]
-            if run_via == "prompt":
-                query = f"""
-                    SELECT *
-                    FROM results
-                    WHERE project = '{project_name}' AND metadata like '%prompt_version%' AND metadata NOT LIKE '%uptrain_experiment_columns%' AND timestamp > datetime('now', '-{num_days} days')
-                    """
-                fpath = os.path.join(
-                    DATABASE_PATH, "uptrain-eval-results", f"{user_id}.db"
-                )
-                if not os.path.exists(fpath):
-                    raise HTTPException(
-                        status_code=404, detail="No evaluations run yet for this user"
-                    )
-                DB = get_sqlite_utils_db(fpath)
-
-                buffer = io.StringIO()
-                for row in DB.query(query):
-                    buffer.write(json.dumps(row) + "\n")
-                buffer.seek(0)
-                data = []
-                for line in buffer:
-                    details = json.loads(line)
-                    for key in details:
-                        try:
-                            details[key] = json.loads(details[key])
-                        except Exception:
-                            pass
-                    data.append(details)
-
-                exp_data, checks_mapping = convert_project_to_dicts(data)
-
-                columns = exp_data.columns
-                columns.remove("prompt_name")
-                columns.remove("prompt_version")
-                data = exp_data.group_by(
-                    ["prompt_name", "prompt_version"], maintain_order=True
-                ).agg(pl.col(col) for col in columns)
-                columns = data.columns
-                columns.remove("prompt_name")
-                data = (
-                    data.group_by(["prompt_name"], maintain_order=True)
-                    .agg(pl.col(col) for col in columns)
-                    .to_dicts()
-                )
-
-                for row in data:
-                    row["scores"] = []
-                    uuid_tags_version = row["uuid_tag"]
-                    for uuid_tags in uuid_tags_version:
-                        scores = []
-                        for uuid in uuid_tags:
-                            score = checks_mapping[uuid]
-                            scores.append(score)
-                        row["scores"].append(pl.DataFrame(scores).mean().to_dicts()[0])
-
-                res = []
-                for prompt in data:
-                    prompt_data = []
-                    num_versions = len(prompt["prompt_version"])
-                    for i in range(num_versions):
-                        prompt_v = {}
-                        for key, value in prompt.items():
-                            # Return only one string instead of a list of strings
-                            if key == "prompt":
-                                value = value[i]
-                            # Remove the explanations from the scores
-                            elif key == "scores":
-                                try:
-                                    value = [
-                                        {
-                                            k: round(float(v), 3)
-                                            for k, v in score.items()
-                                            if not k.startswith("explanation")
-                                        }
-                                        for score in value
-                                    ]
-                                except Exception:
-                                    value = [
-                                        {
-                                            k: v
-                                            for k, v in score.items()
-                                            if not k.startswith("explanation")
-                                        }
-                                        for score in value
-                                    ]
-                            # Handle cases where the value is a list or a string
-                            if isinstance(value, list):
-                                prompt_v[key] = value[i]
-                            else:
-                                prompt_v[key] = value
-                        prompt_data.append(prompt_v)
-                    res.append(
-                        {"prompt_name": prompt["prompt_name"], "prompts": prompt_data}
-                    )
-                return app_schema.ProjectData(data=res, project_name=project_name)
+    address = project_run.address
+    exp_column = project_run.exp_column
+    run_type = project_run.run_type
+    created_at = project_run.created_at
+    checks = project_run.checks
+
+    data = JsonReader(fpath = address).setup(UserSettings()).run()['output'].to_dicts()
+
+    if run_type == "evaluation" or run_type == "experiment" or run_type == "prompt":
+        scores = [col[6:] for col in data[0].keys() if (col.startswith("score_") and 'confidence' not in col)]
+        if run_type == "evaluation" or run_type == "prompt":
+            return app_schema.ProjectData(data=[data, created_at, scores, checks], id=evaluation_id)
+        else:
+            plot_data = {}
+            exp_data = pl.DataFrame(data)
+            for col in scores:
+                col_name = 'score_' + col
+                plot_data.update({col : exp_data.group_by([exp_column], maintain_order=True).agg(pl.col(col_name)).to_dicts()})
+
+            columns = exp_data.columns
+            columns.remove('question')
+            display_data = exp_data.group_by(["question"], maintain_order=True).agg(pl.col(col) for col in columns).to_dicts()
+            unqiue_values  = list(set(exp_data[exp_column].to_list()))
+            return app_schema.ProjectData(data = [display_data, created_at, scores, unqiue_values, exp_column, plot_data, checks], id = evaluation_id)
 
 
-@router_public.post("/add_project_data")
-async def add_project_data(
-    eval_args: app_schema.EvaluateV2,
-    user_id: str = Depends(validate_api_key_public),
-    db: Session = Depends(get_db),
-):
-
-    fpath = os.path.join(DATABASE_PATH, "uptrain-eval-results", f"{user_id}.db")
-    DB = get_sqlite_utils_db(fpath)
 
-    metadata = eval_args.metadata
-    schema = eval_args.schema_dict
-    results = eval_args.data
-    checks = eval_args.checks
-    project = eval_args.project
-    timestamp = get_current_datetime()
-    try:
-        DB["results"].insert_all(
-            [
-                {
-                    "data": row_data,
-                    "checks": row_check,
-                    "metadata": metadata,
-                    "schema": schema,
-                    "project": project,
-                    "timestamp": timestamp,
-                }
-                for row_data, row_check in zip(results, checks)
-            ]
-        )
-    except Exception as e:
-        logger.exception(f"Error running the eval: {e}")
-        raise HTTPException(
-            status_code=500, detail=f"Error saving the data for the project: {e}"
-        )
+def _save_log_and_eval(
+        project_name: str, 
+        evaluation_name: str, 
+        metadata: dict,
+        user_id: str, 
+        source_data: list[dict],
+        sink_data: list[dict],
+        checks: list[dict], 
+        db: Session,
+        exp_column: t.Optional[str] = None
+    ):
+    existing_project = (
+        db.query(ModelProject)
+        .filter_by(name=project_name, user_id=user_id)
+        .first()
+    )
+    if existing_project is not None:
+        project_id = existing_project.id
+    else:
+        project_id = get_uuid()
+    
 
+    if "dataset_id" not in metadata:
+        ######    
+        if "dataset_name" in metadata:
+            dataset_name = metadata["dataset_name"]
+        else:
+            dataset_name = project_name + "__" + evaluation_name
+        dataset_id = get_uuid()
 
-@router_public.get("/get_projects_list", response_model=app_schema.ProjectsList)
-def get_projects_list(
-    num_days: int = 200,
-    active_only: bool = True,
-    limit: int = 10,
-    db: Session = Depends(get_db),
-    user_id: str = Depends(validate_api_key_public),
-):
-    """Get all the project names associated with the user."""
-    user = db.query(ModelUser).filter_by(id=user_id).first()
-    if user is None:
-        raise HTTPException(status_code=403, detail="Invalid user name")
-    else:
-        user_name = user.name
-    try:
-        query = f"""
-        SELECT project, MAX(timestamp) AS latest_timestamp
-        FROM results
-        WHERE metadata LIKE '%uptrain_experiment_columns%' AND timestamp > datetime('now', '-{num_days} days')
-        GROUP BY project
-        ORDER BY latest_timestamp DESC
-        LIMIT {limit}
-        """
-        fpath = os.path.join(DATABASE_PATH, "uptrain-eval-results", f"{user_id}.db")
-        if not os.path.exists(fpath):
-            raise HTTPException(
-                status_code=404, detail="No evaluations run yet for this user"
+        existing_dataset = (
+            db.query(ModelProjectDataset)
+            .filter_by(name=dataset_name, user_id=user_id)
+            .order_by(ModelProjectDataset.version.desc())
+            .first()
+        )
+        if existing_dataset is not None:
+            version = existing_dataset.version + 1
+        else:
+            version = 1
+        #####    
+        try:
+            name_w_version = os.path.join(user_id, dataset_name)
+            address = os.path.join(DATABASE_PATH, "uptrain-datasets", name_w_version)
+            os.makedirs(address, exist_ok=True)
+            address = os.path.join(address, f"v_{version}")
+            JsonWriter(fpath=address).setup(UserSettings()).run(pl.DataFrame(source_data))
+            rows_count = len(source_data)
+            db_item = ModelProjectDataset(
+                id=dataset_id,
+                project_id=project_id,
+                user_id=user_id,
+                name=dataset_name,
+                version=version,
+                address=address,
+                rows_count=rows_count
             )
-        DB = get_sqlite_utils_db(fpath)
-
-        experiment_runs = DB.query(query)
-    except Exception:
-        experiment_runs = []
-
-    try:
-        query = f"""
-        SELECT project, MAX(timestamp) AS latest_timestamp
-        FROM results
-        WHERE metadata NOT LIKE '%prompt_version%' AND metadata NOT LIKE '%uptrain_experiment_columns%' AND timestamp > datetime('now', '-{num_days} days')
-        GROUP BY project
-        ORDER BY latest_timestamp DESC
-        LIMIT {limit}
-        """
-        fpath = os.path.join(DATABASE_PATH, "uptrain-eval-results", f"{user_id}.db")
-        if not os.path.exists(fpath):
+            db.add(db_item)
+            db.commit()
+        except Exception as exc:
+            logger.exception("Error adding/updating dataset to platform")
+            db.rollback()
             raise HTTPException(
-                status_code=404, detail="No evaluations run yet for this user"
+                status_code=400, detail="Error adding/updating dataset to platform"
             )
-        DB = get_sqlite_utils_db(fpath)
-
-        project_runs = DB.query(query)
-    except Exception:
-        project_runs = []
-
-    try:
-        prompts_runs = get_prompts_list(
-            num_days=num_days, limit=limit, db=db, user_id=user_id
+    else:
+        existing_dataset = (
+            db.query(ModelProjectDataset)
+            .filter_by(id=metadata["dataset_id"], user_id=user_id)
+            .order_by(ModelProjectDataset.version.desc())
+            .first()
         )
-    except Exception:
-        prompts_runs = []
+        dataset_id = existing_dataset.id
 
-    out = []
+    for check in checks:
+        for key, value in check.copy().items():
+            ## to remove scenario description
+            if value is None:
+                del check[key]
+    try:
+        if existing_project is None:
+            db_item = ModelProject(
+                id=project_id,
+                name=project_name,
+                user_id=user_id,
+                dataset_id=dataset_id,
+                checks=json.dumps({"checks": checks})
+            )
+            db.add(db_item)
+            db.commit()
+    except Exception as exc:
+        logger.exception("Error adding project to platform")
+        db.rollback()
+        raise HTTPException(
+            status_code=400, detail="Error adding project to platform"
+        )       
+    
+    evaluation_id = get_uuid()
+
+    name_w_version = os.path.join("uptrain-eval-results", evaluation_id)
+    address = os.path.join(DATABASE_PATH, name_w_version)
+
+    JsonWriter(fpath=address).setup(UserSettings()).run(pl.DataFrame(sink_data))
+    run_type = "evaluation"
+    if exp_column is not None:
+        run_type = "experiment"
+    elif "prompt_id" in metadata:
+        run_type = "prompt"
+    add_project_run(
+        app_schema.EvalCreate(
+            evaluation_id=evaluation_id, 
+            evaluation_name=evaluation_name,
+            dataset_id=dataset_id,
+            project_id=project_id,
+            address=address,
+            user_id=user_id,
+            run_type=run_type,
+            checks={"checks": checks},
+            exp_column=exp_column,
+            prompt_id = metadata.get("prompt_id", None)
+        ),
+        db
+    )
+    return 
 
-    for run in project_runs:
-        out.append(
-            {
-                "project": run["project"],
-                "latest_timestamp": run["latest_timestamp"],
-                "run_via": "project",
-            }
-        )
+def _create_evaluation(db: Session, evaluation_id: str, evaluation_name: str, address: str,  project_id: str, dataset_id: str, user_id: str, run_type: str, checks: dict, exp_column: str=None, prompt_id: str=None):
+    """Create a new evaluation."""
+    if exp_column is not None:
+        db_eval = ModelProjectRun(id=evaluation_id, name=evaluation_name, address=address, project_id=project_id, dataset_id=dataset_id, user_id=user_id, run_type=run_type, exp_column=exp_column, checks=checks)
+    else:
+        if prompt_id is not None:
+            db_eval = ModelProjectRun(id=evaluation_id, name=evaluation_name, address=address, project_id=project_id, dataset_id=dataset_id, user_id=user_id, run_type=run_type, prompt_id=prompt_id, checks=checks)
+        else:
+            db_eval = ModelProjectRun(id=evaluation_id, name=evaluation_name, address=address, project_id=project_id, dataset_id=dataset_id, user_id=user_id, run_type=run_type, checks=checks)
+    try:
+        db.add(db_eval)
+        db.commit()
+        return db_eval
+    except Exception as exc:
+        db.rollback()
+        raise exc
+    
 
-    for run in experiment_runs:
-        out.append(
-            {
-                "project": run["project"],
-                "latest_timestamp": run["latest_timestamp"],
-                "run_via": "experiment",
-            }
+@router_internal.post("/evaluation")
+def add_project_run(
+    evaluation: app_schema.EvalCreate,
+    db: Session = Depends(get_db)
+):
+    try:
+        db_eval = _create_evaluation(
+            db, 
+            evaluation.evaluation_id, 
+            evaluation.evaluation_name, 
+            evaluation.address, 
+            evaluation.project_id, 
+            evaluation.dataset_id, 
+            evaluation.user_id, 
+            evaluation.run_type,
+            evaluation.checks,
+            evaluation.exp_column,
+            evaluation.prompt_id
         )
+        return db_eval
+    except Exception as exc:
+        logger.exception(exc)
+        raise HTTPException(status_code=400, detail=f"Error creating the evaluation: {evaluation.evaluation_name}")
+    
+@router_public.post("/add_project_data")
+async def add_project_data(
+    eval_args: app_schema.EvaluateV2,
+    user_id: str = Depends(validate_api_key_public),
+    db: Session = Depends(get_db),
+):
 
-    for run in prompts_runs.data:
-        out.append(
-            {
-                "project": run["project"],
-                "latest_timestamp": run["latest_timestamp"],
-                "run_via": "prompt",
-            }
-        )
+    project_name = eval_args.project
+    evaluation_name = eval_args.evaluation
+    sink_data = eval_args.sink_data
+    exp_column = eval_args.exp_column
+    metadata = eval_args.metadata
 
-    out.sort(reverse=True, key=lambda x: x["latest_timestamp"])
-    return app_schema.ProjectsList(data=out, user_name=user_name)
+    _save_log_and_eval(
+                project_name=project_name, 
+                evaluation_name=evaluation_name, 
+                metadata = metadata,
+                user_id=user_id,
+                source_data=eval_args.data,
+                sink_data=sink_data,
+                checks=eval_args.checks,
+                db=db,
+                exp_column=exp_column
+            )
+    return
 
 
-@router_public.get("/get_evaluations_list", response_model=app_schema.ProjectsList)
-def get_evaluations_list(
-    num_days: int = 200,
-    active_only: bool = True,
-    limit: int = 10,
+@router_public.get("/projects", response_model=list[app_schema.Project])
+def list_projects(
+    num: int = 10,
+    num_days: int = 7,
     db: Session = Depends(get_db),
     user_id: str = Depends(validate_api_key_public),
 ):
-    """Get all the project names associated with the user."""
-    user = db.query(ModelUser).filter_by(id=user_id).first()
-    if user is None:
-        raise HTTPException(status_code=403, detail="Invalid user name")
-    else:
-        user_name = user.name
-
-    try:
-        query = f"""
-        SELECT project, MAX(timestamp) AS latest_timestamp
-        FROM results
-        WHERE metadata NOT LIKE '%prompt_version%' AND metadata NOT LIKE '%uptrain_experiment_columns%' AND timestamp > datetime('now', '-{num_days} days')
-        GROUP BY project
-        ORDER BY latest_timestamp DESC
-        LIMIT {limit}
-        """
+    """Get the last N runs for the user (non-scheduled). Optionally filter by status."""
+    query = (
+        db.query(ModelProject)
+        .filter(ModelProject.user_id == user_id)
+    )
+    
+    projects = query.order_by(ModelProject.created_at.desc()).limit(num).all()
 
-        fpath = os.path.join(DATABASE_PATH, "uptrain-eval-results", f"{user_id}.db")
-        if not os.path.exists(fpath):
-            raise HTTPException(
-                status_code=404, detail="No evaluations run yet for this user"
+    # Convert to list of dicts for easier serialization
+    results = []
+    ### This will include evaluations, experiments and prompts run. 
+    for project in projects:
+        results.append(
+            app_schema.Project(
+                project_type="project",
+                project_id=project.id,
+                created_at=project.created_at,
+                project_name=project.name,
+                dataset_id=project.dataset_id,
+                checks=eval(project.checks)
             )
-        DB = get_sqlite_utils_db(fpath)
+        )
+    return results
+
 
-        project_runs = DB.query(query)
-    except Exception:
-        project_runs = []
+@router_public.get("/project_runs", response_model=list[app_schema.ProjectRun])
+def list_project_runs(
+    project_id: str,
+    num_days: int = 7,
+    num: int = 10,
+    db: Session = Depends(get_db),
+    user_id: str = Depends(validate_api_key_public),
+):
+    """Get the last N runs for the user (non-scheduled). Optionally filter by status."""
+    query = (
+        db.query(ModelProjectRun)
+        .filter(ModelProjectRun.user_id == user_id, ModelProjectRun.project_id == project_id)
+    )
 
-    out = []
+    project_runs = query.order_by(ModelProjectRun.created_at.desc()).limit(num).all()
 
+    # Convert to list of dicts for easier serialization
+    results = []
     for run in project_runs:
-        out.append(
-            {
-                "project": run["project"],
-                "latest_timestamp": run["latest_timestamp"],
-                "run_via": "project",
-            }
+        results.append(
+            app_schema.ProjectRun(
+                evaluation_id=run.id,
+                evaluation_name=run.name,
+                project_id=run.project_id,
+                created_at=run.created_at,
+                dataset_id=run.dataset_id,
+                run_type=run.run_type,
+                exp_column=run.exp_column
+            )
         )
 
-    out.sort(reverse=True, key=lambda x: x["latest_timestamp"])
-    return app_schema.ProjectsList(data=out, user_name=user_name)
+    return results
 
 
-@router_public.get("/get_experiments_list", response_model=app_schema.ProjectsList)
-def get_experiments_list(
-    num_days: int = 7,
-    limit: int = 10,
+@router_public.get("/prompt_runs", response_model=list[app_schema.PromptRun])
+def prompt_runs(
+    project_id: str,
+    num: int = 10,
     db: Session = Depends(get_db),
     user_id: str = Depends(validate_api_key_public),
 ):
-    """Get all the experiment names associated with the user."""
-    user = db.query(ModelUser).filter_by(id=user_id).first()
-    if user is None:
-        raise HTTPException(status_code=403, detail="Invalid user name")
-    else:
-        user_name = user.name
+    """Get the last N runs for the user (non-scheduled). Optionally filter by status."""
+    query = (
+        db.query(ModelPrompt)
+        .filter(ModelPrompt.user_id == user_id, ModelPrompt.project_id == project_id)
+    )
 
-    try:
-        query = f"""
-        SELECT project, MAX(timestamp) AS latest_timestamp
-        FROM results
-        WHERE metadata LIKE '%uptrain_experiment_columns%' AND timestamp > datetime('now', '-{num_days} days')
-        GROUP BY project
-        ORDER BY latest_timestamp DESC
-        LIMIT {limit}
-        """
+    prompt_runs = query.order_by(ModelPrompt.created_at.asc()).limit(num).all()
 
-        fpath = os.path.join(DATABASE_PATH, "uptrain-eval-results", f"{user_id}.db")
-        if not os.path.exists(fpath):
-            raise HTTPException(
-                status_code=404, detail="No evaluations run yet for this user"
+    results = []
+    prompts = []
+    for run in prompt_runs:
+        prompt_id = run.id
+        prompt_name = run.name
+        prompt_version = run.version
+        prompt = run.prompt
+        prompt_dict = {'prompt_id': prompt_id, 'prompt_name': prompt_name, 'prompt_version': prompt_version, 'prompt': prompt}
+        query_prompt_data = db.query(ModelProjectRun).filter(ModelProjectRun.prompt_id == prompt_id, ModelProjectRun.user_id == user_id).first()
+
+        if query_prompt_data is None: #or not len(list(query_prompt_data)):
+            continue
+        prompt_run = query_prompt_data
+        
+        evaluation_id = prompt_run.id 
+        prompt_dict['evaluation_id'] = evaluation_id
+        prompt_dict['created_at'] = prompt_run.created_at
+        prompt_dict['dataset_id'] = prompt_run.dataset_id
+        address = prompt_run.address
+        data = JsonReader(fpath = address).setup(UserSettings()).run()['output'].to_dicts()
+        data_df = pl.DataFrame(data)
+        scores = [col for col in data[0].keys() if (col.startswith("score_") and "confidence" not in col)]
+        scores_dict = {}
+        mean_values = data_df.mean().to_dicts()[0]
+        for score in scores:
+            scores_dict[score] = round(mean_values[score], 2)
+        prompt_dict['scores'] = scores_dict
+        prompts.append(copy.deepcopy(prompt_dict))
+     
+    for run in prompts:
+        results.append(
+            app_schema.PromptRun(
+                evaluation_id=run['evaluation_id'],
+                prompt_id=run['prompt_id'],
+                prompt_name=run['prompt_name'],
+                prompt_version=run['prompt_version'],
+                prompt=run['prompt'],
+                created_at=run['created_at'],
+                dataset_id=run['dataset_id'],
+                scores=run['scores']
             )
-        DB = get_sqlite_utils_db(fpath)
-
-        project_runs = DB.query(query)
-    except Exception:
-        project_runs = []
-
-    out = []
-
-    for run in project_runs:
-        out.append(
-            {
-                "project": run["project"],
-                "latest_timestamp": run["latest_timestamp"],
-                "run_via": "experiment",
-            }
         )
+    return results
 
-    out.sort(reverse=True, key=lambda x: x["latest_timestamp"])
-    return app_schema.ProjectsList(data=out, user_name=user_name)
 
-
-@router_public.get("/get_prompts_list", response_model=app_schema.ProjectsList)
-def get_prompts_list(
-    num_days: int = 7,
-    limit: int = 10,
+@router_public.get("/compare_prompt", response_model=app_schema.ProjectData)
+def compare_prompt(
+    evaluation_id_1: str,
+    evaluation_id_2: str,
+    version_1: t.Union[str, int],
+    version_2: t.Union[str, int],
     db: Session = Depends(get_db),
     user_id: str = Depends(validate_api_key_public),
 ):
-    """Get all the experiment names associated with the user."""
+    """Get all the data for a particular evaluation for the given user.
+    """
     user = db.query(ModelUser).filter_by(id=user_id).first()
     if user is None:
         raise HTTPException(status_code=403, detail="Invalid user name")
     else:
         user_name = user.name
 
-    try:
-        query = f"""
-        SELECT project, MAX(timestamp) AS latest_timestamp
-        FROM results
-        WHERE metadata like '%prompt_version%' AND metadata NOT LIKE '%uptrain_experiment_columns%' AND timestamp > datetime('now', '-{num_days} days')
-        GROUP BY project
-        ORDER BY latest_timestamp DESC
-        LIMIT {limit}
-        """
-        fpath = os.path.join(DATABASE_PATH, "uptrain-eval-results", f"{user_id}.db")
-        if not os.path.exists(fpath):
-            raise HTTPException(
-                status_code=404, detail="No evaluations run yet for this user"
-            )
-        DB = get_sqlite_utils_db(fpath)
-
-        prompts_runs = DB.query(query)
-    except Exception:
-        prompts_runs = []
-
-    out = []
+    project_run_1 = db.query(ModelProjectRun).filter_by(id=evaluation_id_1).first()
+    project_run_2 = db.query(ModelProjectRun).filter_by(id=evaluation_id_2).first()
 
-    for run in prompts_runs:
-        out.append(
-            {
-                "project": run["project"],
-                "latest_timestamp": run["latest_timestamp"],
-                "run_via": "prompt",
-            }
-        )
-
-    out.sort(reverse=True, key=lambda x: x["latest_timestamp"])
-    return app_schema.ProjectsList(data=out, user_name=user_name)
+    address_1 = project_run_1.address
+    address_2 = project_run_2.address
+    created_at_1 = project_run_1.created_at
+    created_at_2 = project_run_2.created_at
+
+    
+    data_1 = JsonReader(fpath = address_1).setup(UserSettings()).run()['output'].with_columns(
+        experiment_column = pl.lit(str(version_1))
+    ).to_dicts()
+    data_2 = JsonReader(fpath = address_2).setup(UserSettings()).run()['output'].with_columns(
+        experiment_column = pl.lit(str(version_2))
+    ).to_dicts()
+
+    combined_data = pl.concat([pl.DataFrame(data_1), pl.DataFrame(data_2)], how="diagonal").to_dicts()
+    
+    scores_1 = [col[6:] for col in data_1[0].keys() if (col.startswith("score_") and 'confidence' not in col)]
+    scores_2 = [col[6:] for col in data_2[0].keys() if (col.startswith("score_") and 'confidence' not in col)]
+    common_scores = intersection(scores_1, scores_2)
+
+    plot_data = {}
+    exp_column = 'experiment_column'
+    exp_data = pl.DataFrame(combined_data)
+    for col in common_scores:
+        col_name = 'score_' + col
+        plot_data.update({col : exp_data.group_by([exp_column], maintain_order=True).agg(pl.col(col_name)).to_dicts()})
+
+    columns = exp_data.columns
+    columns.remove('question')
+    display_data = exp_data.group_by(["question"], maintain_order=True).agg(pl.col(col) for col in columns).to_dicts()
+    unqiue_values  = list(set(exp_data[exp_column].to_list()))
+    return app_schema.ProjectData(data = [display_data, created_at_1, common_scores, unqiue_values, exp_column, plot_data], id = evaluation_id_1)
+
+
+@router_public.get("/project_datasets", response_model=list[app_schema.ProjectDataset])
+def list_project_datasets(
+    project_id: str, 
+    db: Session = Depends(get_db),
+    user_id: str = Depends(validate_api_key_public),
+):
+    datasets = (
+        db.query(ModelProjectDataset)
+        .filter_by(user_id=user_id, project_id=project_id)
+        .all()
+    )
+    return [
+        app_schema.ProjectDataset(name=db_item.name, version=db_item.version, id=db_item.id)
+        for db_item in datasets
+    ]
 
 
 @router_public.post("/find_common_topic")
 async def find_common_topic(
     args: app_schema.TopicGenerate,
     db: Session = Depends(get_db),
     user_id: str = Depends(validate_api_key_public),
@@ -696,261 +638,495 @@
         map(
             lambda x: {"question": x, "cluster_index": 0, "cluster_index_distance": 0},
             refined_items,
         )
     )
 
     from uptrain.operators import TopicGenerator
-
     user = db.query(ModelUser).filter_by(id=user_id).first()
     if user is None:
         raise HTTPException(status_code=403, detail="Invalid user name")
     else:
         user_name = user.name
 
     user_headers = {"openai_api_key": user_name}
 
     try:
         result = (
             TopicGenerator()
-            .setup(Settings(**user_headers))
+            .setup(UserSettings(**user_headers))
             .run(pl.DataFrame(data))["output"]
         )
         return {"common_topic": result.to_dicts()[0]["topic"]}
     except Exception as exc:
         logger.exception("Error creating run")
         db.rollback()
         raise HTTPException(status_code=400, detail="Error finding common topic")
 
 
-@router_public.post("/add_evaluation")
-async def add_evaluation(
+@router_public.post("/create_project")
+async def create_project(
     model: str = Form(...),
     project_name: str = Form(...),
     dataset_name: str = Form(...),
     checks: list = Form(...),
     data_file: UploadFile = File(...),
     metadata: str = Form(...),
     user_id: str = Depends(validate_api_key_public),
     db: Session = Depends(get_db),
     fsspec_fs: t.Any = Depends(get_fsspec_fs),
 ):
     ## project key would be present in the eval_args.metadata
 
-    existing_dataset = (
-        db.query(ModelDataset)
-        .filter_by(name=dataset_name, user_id=user_id)
-        .order_by(ModelDataset.version.desc())
+    existing_project = (
+        db.query(ModelProject)
+        .filter_by(name=project_name, user_id=user_id)
         .first()
     )
-    if existing_dataset is not None:
-        version = existing_dataset.version + 1
+    if existing_project is not None:
+        raise HTTPException(
+            status_code=400, detail="cannot create a project with the same name."
+        )
+    
+    evaluation_name = "default_run"
+    version = str(random.random()).split('.')[-1][:2]
+    name_w_version = os.path.join(user_id, dataset_name, f"v_{version}")
+    address = os.path.join("temp-datasets", name_w_version)
+    with fsspec_fs.open(address, "wb") as f:
+        f.write(data_file.file.read())
+
+    checks = eval(checks[0])
+    checks_1 = []
+    metadata = eval(metadata)
+
+    for check in checks:
+        if check in metadata:
+            final_check = checks_mapping(check, metadata[check])
+        else:
+            final_check = checks_mapping(check)
+
+        if final_check is not None:
+            checks_1.append(final_check)
+
+    settings_data = {}
+    settings_data["model"] = model
+    settings_data["uptrain_local_url"] = os.environ["UPTRAIN_LOCAL_URL"]
+    settings_data.update(metadata[model])
+
+    if "exp_column" in metadata:
+        exp_column = metadata["exp_column"]
     else:
-        version = 1
+        exp_column = None
+    
     try:
-        name_w_version = os.path.join(user_id, dataset_name, f"v_{version}")
-        address = os.path.join("uptrain-datasets", name_w_version)
-        with fsspec_fs.open(address, "wb") as f:
-            f.write(data_file.file.read())
-
-        data_file.file.seek(0, 0)
-        rows_count = len(data_file.file.readlines())
-        db_item = ModelDataset(
-            user_id=user_id,
-            name=dataset_name,
-            version=version,
-            address=address,
-            rows_count=rows_count,
+        user_client = EvalLLM(UserSettings(**settings_data))
+        data = (
+            JsonReader(
+                fpath=os.path.join(DATABASE_PATH, "temp-datasets", name_w_version)
+            )
+            .setup(UserSettings())
+            .run()["output"]
+            .to_dicts()
         )
-        db.add(db_item)
-        db.commit()
-    except Exception as exc:
-        logger.exception("Error adding/updating dataset to platform")
-        db.rollback()
+        metadata = {'dataset_name': dataset_name}
+        if exp_column is None:
+            results = user_client.evaluate(
+                data=data, checks=checks_1, project_name=project_name, evaluation_name=evaluation_name, metadata=metadata
+            )
+        else:
+            results = user_client.evaluate_experiments(
+                data=data, checks=checks_1, project_name=project_name, evaluation_name=evaluation_name, exp_columns=[exp_column], metadata=metadata
+            )
+        return {"message": f"Evaluation has been queued up"}
+    except Exception as e:
+        logger.exception(f"Error running the eval: {e}")
         raise HTTPException(
-            status_code=400, detail="Error adding/updating dataset to platform"
+            status_code=500, detail=f"Error running the evaluation: {e}"
         )
-    from uptrain.operators import JsonReader
-    from uptrain import Settings
 
+
+
+@router_public.post("/new_run")
+async def new_run(
+    model: str = Form(...),
+    dataset_name: str = Form(...),
+    evaluation_name: str = Form(...),
+    checks: list = Form(...),
+    project_id: str = Form(...),
+    data_file: UploadFile = File(...),
+    metadata: str = Form(...),
+    user_id: str = Depends(validate_api_key_public),
+    db: Session = Depends(get_db),
+    fsspec_fs: t.Any = Depends(get_fsspec_fs),
+):
+    ## project key would be present in the eval_args.metadata
+
+    existing_project = (
+        db.query(ModelProject)
+        .filter_by(id=project_id)
+        .first()
+    )
+    
     checks = eval(checks[0])
     checks_1 = []
     metadata = eval(metadata)
 
+    version = str(random.random()).split('.')[-1][:2]
+    name_w_version = os.path.join(user_id, dataset_name, f"v_{version}")
+    address = os.path.join("temp-datasets", name_w_version)
+    with fsspec_fs.open(address, "wb") as f:
+        f.write(data_file.file.read())
+
     for check in checks:
         if check in metadata:
             final_check = checks_mapping(check, metadata[check])
         else:
             final_check = checks_mapping(check)
 
         if final_check is not None:
             checks_1.append(final_check)
 
     settings_data = {}
     settings_data["model"] = model
+    settings_data["uptrain_local_url"] = os.environ["UPTRAIN_LOCAL_URL"]
     settings_data.update(metadata[model])
 
-    try:
-        from uptrain import EvalLLM
+    if "exp_column" in metadata:
+        exp_column = metadata["exp_column"]
+    else:
+        exp_column = None
 
-        user_client = EvalLLM(Settings(**settings_data))
+    try:
+        user_client = EvalLLM(UserSettings(**settings_data))
         data = (
             JsonReader(
-                fpath=os.path.join(DATABASE_PATH, "uptrain-datasets", name_w_version)
+                fpath=os.path.join(DATABASE_PATH, "temp-datasets", name_w_version)
             )
-            .setup(Settings())
+            .setup(UserSettings())
             .run()["output"]
             .to_dicts()
         )
-        results = user_client.evaluate(
-            data=data, checks=checks_1, project_name=project_name
+        metadata = {'dataset_name': dataset_name}
+        if exp_column is None:
+            results = user_client.evaluate(
+                data=data, checks=checks_1, project_name=existing_project.name, evaluation_name=evaluation_name, metadata=metadata
+            )
+        else:
+            results = user_client.evaluate_experiments(
+                data=data, checks=checks_1, project_name=existing_project.name, evaluation_name=evaluation_name, exp_columns=[exp_column], metadata=metadata
+            )
+        return {"message": f"Evaluation has been queued up"}
+    except Exception as e:
+        logger.exception(f"Error running the eval: {e}")
+        raise HTTPException(
+            status_code=500, detail=f"Error running the evaluation: {e}"
+        )
+    
+
+
+@router_public.post("/add_default_run")
+async def add_default_run(
+    eval_args: app_schema.DefaultRun,
+    user_id: str = Depends(validate_api_key_public),
+    db: Session = Depends(get_db)
+):
+    ## project key would be present in the eval_args.metadata
+    dataset_id = eval_args.dataset_id
+    project_id = eval_args.project_id
+
+    existing_project = (
+        db.query(ModelProject)
+        .filter_by(id=project_id)
+        .first()
+    )
+
+
+    existing_dataset = (
+        db.query(ModelProjectDataset)
+        .filter_by(id=dataset_id, user_id=user_id)
+        .order_by(ModelProjectDataset.version.desc())
+        .first()
+    )
+
+    if existing_dataset is None:
+        raise HTTPException(status_code=500, detail="Invalid dataset provided")
+
+    dataset_name = existing_dataset.name
+    version = existing_dataset.version
+
+    name_w_version = os.path.join(user_id, dataset_name, f"v_{version}")
+    address = os.path.join('uptrain-datasets', name_w_version)
+    
+    checks = eval_args.checks
+    checks_1 = []
+    metadata = eval_args.metadata
+            
+    for check in checks:
+        if check in metadata:
+            final_check = checks_mapping(check, metadata[check])
+        else:
+            final_check = checks_mapping(check)
+        if final_check is not None:
+            checks_1.append(final_check)
+
+    settings_data = {}
+    settings_data["model"] = eval_args.model
+    settings_data["uptrain_local_url"] = os.environ["UPTRAIN_LOCAL_URL"]
+    settings_data.update(metadata[eval_args.model])
+
+    if "exp_column" in metadata:
+        exp_column = metadata["exp_column"]
+    else:
+        exp_column = None
+
+    try:
+        user_client = EvalLLM(UserSettings(**settings_data))
+        data = (
+            JsonReader(
+                fpath=os.path.join(DATABASE_PATH, address)
+            )
+            .setup(UserSettings())
+            .run()["output"]
+            .to_dicts()
         )
+        metadata = {'dataset_name': dataset_name, 'dataset_id': dataset_id}
+        if exp_column is None:
+            results = user_client.evaluate(
+                data=data, checks=checks_1, project_name=existing_project.name, evaluation_name=eval_args.evaluation_name, metadata=metadata
+            )
+        else:
+            results = user_client.evaluate_experiments(
+                data=data, checks=checks_1, project_name=existing_project.name, evaluation_name=eval_args.evaluation_name, exp_columns=[exp_column], metadata=metadata
+            )
         return {"message": f"Evaluation has been queued up"}
     except Exception as e:
         logger.exception(f"Error running the eval: {e}")
         raise HTTPException(
             status_code=500, detail=f"Error running the evaluation: {e}"
         )
 
 
 @router_public.post("/add_prompts")
-async def add_prompts(
+async def add_prompts(  
+    project_id: str = Form(...),
     model: str = Form(...),
-    project_name: str = Form(...),
     dataset_name: str = Form(...),
     prompt: str = Form(...),
     checks: list = Form(...),
     metadata: str = Form(...),
     prompt_name: str = Form(...),
     data_file: UploadFile = File(...),
     user_id: str = Depends(validate_api_key_public),
     db: Session = Depends(get_db),
     fsspec_fs: t.Any = Depends(get_fsspec_fs),
 ):
     ## project key would be present in the eval_args.metadata
 
-    user = db.query(ModelUser).filter_by(id=user_id).first()
-    if user is None:
-        raise HTTPException(status_code=403, detail="Invalid user name")
-    else:
-        user_name = user.name
+    # user = db.query(ModelUser).filter_by(id=user_id).first()
+    # if user is None:
+    #     raise HTTPException(status_code=403, detail="Invalid user name")
+    # else:
+    #     user_name = user.name
+
+    existing_project = (
+        db.query(ModelProject)
+        .filter_by(id=project_id)
+        .first()
+    )
+    
+    checks = eval(checks[0])
+    checks_1 = []
+    metadata = eval(metadata)
 
-    existing_dataset = (
-        db.query(ModelDataset)
-        .filter_by(name=dataset_name, user_id=user_id)
-        .order_by(ModelDataset.version.desc())
+    version = str(random.random()).split('.')[-1][:2]
+    name_w_version = os.path.join(user_id, dataset_name, f"v_{version}")
+    address = os.path.join("temp-datasets", name_w_version)
+    with fsspec_fs.open(address, "wb") as f:
+        f.write(data_file.file.read())
+
+    for check in checks:
+        if check in metadata:
+            final_check = checks_mapping(check, metadata[check])
+        else:
+            final_check = checks_mapping(check)
+
+        if final_check is not None:
+            checks_1.append(final_check)
+
+    settings_data = {}
+    settings_data["model"] = model
+    settings_data["uptrain_local_url"] = os.environ["UPTRAIN_LOCAL_URL"]
+    settings_data.update(metadata[model])
+    prompt_id = get_uuid()
+
+    existing_prompt = (
+        db.query(ModelPrompt)
+        .filter_by(name=prompt_name, user_id=user_id)
+        .order_by(ModelPrompt.version.desc())
         .first()
     )
-    if existing_dataset is not None:
-        version = existing_dataset.version + 1
+    if existing_prompt is not None:
+        version = existing_prompt.version + 1
     else:
         version = 1
-    try:
-        name_w_version = os.path.join(user_id, dataset_name, f"v_{version}")
-        address = os.path.join("uptrain-datasets", name_w_version)
-        with fsspec_fs.open(address, "wb") as f:
-            f.write(data_file.file.read())
-
-        data_file.file.seek(0, 0)
-        rows_count = len(data_file.file.readlines())
 
-        db_item = ModelDataset(
-            user_id=user_id,
-            name=dataset_name,
-            version=version,
-            address=address,
-            rows_count=rows_count,
+    try:
+        db_item = ModelPrompt(
+            id=prompt_id, user_id=user_id, name=prompt_name, version=version, prompt=prompt, project_id=project_id
         )
         db.add(db_item)
         db.commit()
     except Exception as exc:
-        logger.exception("Error adding/updating dataset to platform")
+        logger.exception("Error adding/updating prompts to platform")
         db.rollback()
         raise HTTPException(
-            status_code=400, detail="Error adding/updating dataset to platform"
+            status_code=400, detail="Error adding/updating prompts to platform"
+        )
+
+    metadata = {
+        "dataset_name": dataset_name,
+        "prompt_id": prompt_id,
+        "model": model,
+    }
+
+    try:
+        user_client = EvalLLM(UserSettings(**settings_data))
+        data = (
+            JsonReader(
+                fpath=os.path.join(DATABASE_PATH, "temp-datasets", name_w_version)
+            )
+            .setup(UserSettings())
+            .run()["output"]
+            .to_dicts()
+        )
+        results = user_client.evaluate_prompts(
+            project_name=existing_project.name,
+            data=data,
+            checks=checks_1,
+            prompt=prompt,
+            metadata=metadata,
+        )
+        return {"message": f"Evaluation has been queued up"}
+    except Exception as e:
+        logger.exception(f"Error running the eval: {e}")
+        raise HTTPException(
+            status_code=500, detail=f"Error running the evaluation: {e}"
         )
 
+
+
+
+@router_public.post("/add_default_prompt")
+async def add_default_prompt(
+    eval_args: app_schema.DefaultPrompt,
+    user_id: str = Depends(validate_api_key_public),
+    db: Session = Depends(get_db)
+):
+    ## project key would be present in the eval_args.metadata
+    prompt_id = get_uuid()
+
+    dataset_id = eval_args.dataset_id
+    project_id = eval_args.project_id
+
+    prompt_name = eval_args.prompt_name
+    prompt = eval_args.prompt
+
+    existing_project = (
+        db.query(ModelProject)
+        .filter_by(id=project_id)
+        .first()
+    )
+
+
+    existing_dataset = (
+        db.query(ModelProjectDataset)
+        .filter_by(id=dataset_id, user_id=user_id)
+        .order_by(ModelProjectDataset.version.desc())
+        .first()
+    )
+
+    if existing_dataset is None:
+        raise HTTPException(status_code=500, detail="Invalid dataset provided")
+
+    dataset_name = existing_dataset.name
+    version = existing_dataset.version
+
+    name_w_version = os.path.join(user_id, dataset_name, f"v_{version}")
+    address = os.path.join('uptrain-datasets', name_w_version)
+    
     existing_prompt = (
         db.query(ModelPrompt)
         .filter_by(name=prompt_name, user_id=user_id)
         .order_by(ModelPrompt.version.desc())
         .first()
     )
     if existing_prompt is not None:
         version = existing_prompt.version + 1
     else:
         version = 1
     try:
         db_item = ModelPrompt(
-            user_id=user_id, name=prompt_name, version=version, prompt=prompt
+            id=prompt_id,
+            project_id=project_id,
+            user_id=user_id,
+            name=prompt_name,
+            version=version,
+            prompt=prompt
         )
         db.add(db_item)
         db.commit()
     except Exception as exc:
         logger.exception("Error adding/updating prompts to platform")
         db.rollback()
         raise HTTPException(
             status_code=400, detail="Error adding/updating prompts to platform"
         )
-
-    checks = eval(checks[0])
+    
+    checks = eval_args.checks
     checks_1 = []
-    metadata = eval(metadata)
-
+    metadata = eval_args.metadata
+            
     for check in checks:
         if check in metadata:
             final_check = checks_mapping(check, metadata[check])
         else:
             final_check = checks_mapping(check)
-
         if final_check is not None:
             checks_1.append(final_check)
 
     settings_data = {}
-    settings_data["model"] = model
-    settings_data.update(metadata[model])
+    settings_data["model"] = eval_args.model
+    settings_data["uptrain_local_url"] = os.environ["UPTRAIN_LOCAL_URL"]
+    settings_data.update(metadata[eval_args.model])
 
-    from uptrain.operators import JsonReader
-    from uptrain import Settings as UserSettings
 
-    metadata = None
     metadata = {
-        "project": project_name,
-        "prompt": prompt,
-        "prompt_name": prompt_name,
-        "prompt_version": version,
-        "model": model,
+        "dataset_id": dataset_id,
+        "prompt_id": prompt_id,
+        "model": eval_args.model,
     }
 
+    data = JsonReader(fpath=os.path.join(DATABASE_PATH, address)).setup(UserSettings()).run()['output'].to_dicts()
+    
     try:
-        from uptrain import EvalLLM
-
-        user_client = EvalLLM(Settings(**settings_data))
-        data = (
-            JsonReader(
-                fpath=os.path.join(DATABASE_PATH, "uptrain-datasets", name_w_version)
-            )
-            .setup(UserSettings())
-            .run()["output"]
-            .to_dicts()
-        )
+        user_client = EvalLLM(UserSettings(**settings_data))
         results = user_client.evaluate_prompts(
-            project_name=project_name,
+            project_name=existing_project.name,
             data=data,
             checks=checks_1,
             prompt=prompt,
             metadata=metadata,
         )
         return {"message": f"Evaluation has been queued up"}
     except Exception as e:
         logger.exception(f"Error running the eval: {e}")
         raise HTTPException(
             status_code=500, detail=f"Error running the evaluation: {e}"
         )
-
+    
 
 # -----------------------------------------------------------
 # FastAPI app
 # -----------------------------------------------------------
 
 app = FastAPI()
 app.add_middleware(
```

### Comparing `uptrain-0.6.9/uptrain/dashboard/backend/nest_asyncio.py` & `uptrain-0.7.0/uptrain/dashboard/backend/nest_asyncio.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/framework/__init__.pyi` & `uptrain-0.7.0/uptrain/framework/__init__.pyi`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/framework/base.py` & `uptrain-0.7.0/uptrain/framework/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,36 +45,42 @@
 
     azure_api_key: t.Optional[str] = Field(None, env="AZURE_API_KEY")
     azure_api_base: t.Optional[str] = Field(None, env="AZURE_API_BASE")
     azure_api_version: t.Optional[str] = Field(
         None, env="AZURE_API_VERSION"
     )
 
+    custom_llm_provider: t.Optional[str] = None
+    api_base: t.Optional[str] = None
+
     rpm_limit: int = 100
     tpm_limit: int = 90_000
     embedding_compute_method: t.Literal["local", "replicate", "api"] = "local"
 
     # uptrain managed service related
     uptrain_access_token: t.Optional[str] = Field(
         None, env="UPTRAIN_ACCESS_TOKEN"
     )
     uptrain_server_url: str = Field(
         "https://demo.uptrain.ai/", env="UPTRAIN_SERVER_URL"
     )
-
+    # uptrain open-source related
+    uptrain_local_url: str = Field(
+        "http://localhost:4300/", env="UPTRAIN_LOCAL_URL"
+    )
     # Embedding model related, applicable if embedding_compute_method is api.
     embedding_model_url: t.Optional[str] = Field(
         None, env="EMBEDDING_MODEL_URL"
     )
     embedding_model_api_token: t.Optional[str] = Field(
         None, env="EMBEDDING_MODEL_API_TOKEN"
     )
 
     # LLM model to run the evaluations
-    model: str = "gpt-3.5-turbo-1106"
+    model: str = "gpt-3.5-turbo"
     seed: t.Union[int, None] = None
     response_format: t.Union[dict, None] = None
 
     evaluate_locally: bool = True
 
     # Cot -> We will use chain of thought prompting to evaluate and get the grade
     # basic -> We will simply prompt the LLM to return the grade without any reasoning
```

### Comparing `uptrain-0.6.9/uptrain/framework/builtins.py` & `uptrain-0.7.0/uptrain/framework/builtins.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     ResponseMatchingScore,
     ConversationSatisfactionScore,
     CodeHallucinationScore,
     JailbreakDetectionScore,
     SubQueryCompleteness,
     ContextReranking,
     ContextConciseness,
+    MultiQueryAccuracy,
 )
 
 
 # -----------------------------------------------------------
 # Response Quality
 # -----------------------------------------------------------
 
@@ -71,15 +72,15 @@
     )
 
 
 def CheckResponseMatching(method="llm"):
     return Check(
         name="response_matching_score",
         operators=[ResponseMatchingScore(method=method)],
-        plots=[Histogram(x="score_response_matching")],
+        plots=[Histogram(x="score_response_match")],
     )
 
 
 # -----------------------------------------------------------
 # Context Quality
 # -----------------------------------------------------------
 
@@ -224,7 +225,19 @@
 
 def CheckSubQueryCompleteness():
     return Check(
         name="sub_query_completeness_score",
         operators=[SubQueryCompleteness()],
         plots=[Histogram(x="score_sub_query_completeness")],
     )
+
+
+# -----------------------------------------------------------
+# MultiQuery
+# -----------------------------------------------------------
+
+def CheckMultiQueryAccuracy():
+    return Check(
+        name="multi_query_accuracy_score",
+        operators=[MultiQueryAccuracy()],
+        plots=[Histogram(x="score_multi_query_accuracy")],
+    )
```

### Comparing `uptrain-0.6.9/uptrain/framework/checks.py` & `uptrain-0.7.0/uptrain/framework/checks.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/framework/evalllm.py` & `uptrain-0.7.0/uptrain/framework/evalllm.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,29 +10,28 @@
 import polars as pl
 import pandas as pd
 import pydantic
 import copy
 import os
 import httpx
 from uptrain.operators.base import ColumnOp
-from uptrain.utilities.utils import get_current_datetime, parse_prompt, check_openai_api_key
+from uptrain.utilities.utils import parse_prompt, check_openai_api_key
 from uptrain.framework.remote import APIClientWithoutAuth, DataSchema
 from uptrain.framework.base import Settings
 from uptrain.framework.checks import Check
 from uptrain.framework.evals import (
     Evals,
     JailbreakDetection,
     ParametricEval,
     CritiqueTone,
     GuidelineAdherence,
     ResponseMatching,
     ConversationSatisfaction,
 )
 from uptrain.operators import (
-    TransformOp,
     ResponseFactualScore,
     ContextRelevance,
     ResponseCompleteness,
     ResponseCompletenessWrtContext,
     ResponseConciseness,
     ResponseConsistency,
     ResponseMatchingScore,
@@ -44,14 +43,17 @@
     LanguageCritique,
     ToneCritique,
     ResponseRelevance,
     ContextConciseness,
     ContextReranking,
     SubQueryCompleteness,
     CodeHallucinationScore,
+    CustomPromptEvalScore,
+    MultiQueryAccuracy,
+    ValidQuestionScore
 )
 
 from uptrain.framework.rca_templates import RcaTemplate
 from uptrain.operators import RagWithCitation
 
 RCA_TEMPLATE_TO_OPERATOR_MAPPING = {RcaTemplate.RAG_WITH_CITATION: RagWithCitation()}
 
@@ -66,38 +68,45 @@
     Evals.RESPONSE_CONSISTENCY: ResponseConsistency(),
     Evals.RESPONSE_RELEVANCE: ResponseRelevance(),
     Evals.VALID_RESPONSE: ValidResponseScore(),
     Evals.PROMPT_INJECTION: PromptInjectionScore(),
     Evals.CRITIQUE_LANGUAGE: LanguageCritique(),
     Evals.SUB_QUERY_COMPLETENESS: SubQueryCompleteness(),
     Evals.CODE_HALLUCINATION: CodeHallucinationScore(),
+    Evals.MULTI_QUERY_ACCURACY: MultiQueryAccuracy(),
+    Evals.QUESTION_COMPLETENESS: ValidQuestionScore(),
 }
 
 PARAMETRIC_EVAL_TO_OPERATOR_MAPPING = {
     "JailbreakDetection": JailbreakDetectionScore,
     "GuidelineAdherence": GuidelineAdherenceScore,
     "ConversationSatisfaction": ConversationSatisfactionScore,
     "CritiqueTone": ToneCritique,
     "ResponseMatching": ResponseMatchingScore,
+    "CustomPromptEval": CustomPromptEvalScore,
 }
 
 
+def get_uuid():
+    import uuid
+    return str(uuid.uuid4().hex)
+
 class EvalLLM:
     def __init__(self, settings: Settings = None, openai_api_key: str = None) -> None:
         if (openai_api_key is None) and (settings is None):
             raise Exception("Please provide OpenAI API Key")
 
         if settings is None:
             self.settings = Settings(openai_api_key=openai_api_key)
         else:
             self.settings = settings
         if self.settings.openai_api_key is not None and len(self.settings.openai_api_key):
             response = check_openai_api_key(self.settings.openai_api_key)
             if not response:
-                raise Exception("OpenAI API Key is invalid")
+                raise ValueError("OpenAI API Key is invalid")
 
         self.executor = APIClientWithoutAuth(self.settings)
 
     ####
     def perform_root_cause_analysis(
         self,
         data: t.Union[list[dict], pl.DataFrame, pd.DataFrame],
@@ -170,14 +179,15 @@
         return results
 
     def evaluate(
         self,
         data: t.Union[list[dict], pl.DataFrame, pd.DataFrame],
         checks: list[t.Union[str, Evals, ParametricEval]],
         project_name: str = "Project - " + str(datetime.utcnow()),
+        evaluation_name: t.Optional[str] = None,
         scenario_description: t.Optional[str] = None,
         schema: t.Union[DataSchema, dict[str, str], None] = None,
         metadata: t.Optional[dict[str, str]] = None,
     ):
         """Run an evaluation on the UpTrain server using user's openai keys.
         NOTE: This api doesn't log any data.
 
@@ -186,15 +196,17 @@
             data: Data to evaluate on. Either a Pandas DataFrame or a list of dicts.
             checks: List of checks to evaluate on.
             schema: Schema of the data. Only required if the data attributes aren't typical (question, response, context).
             metadata: Attributes to attach to this dataset. Useful for filtering and grouping in the UI.
         Returns:
             results: List of dictionaries with each data point and corresponding evaluation results.
         """
-
+        if evaluation_name is None:
+            evaluation_name = "Eval - " + str(datetime.utcnow())
+        
         if isinstance(data, pl.DataFrame):
             data = data.to_dicts()
         elif isinstance(data, pd.DataFrame):
             data = data.to_dict(orient="records")
 
         if schema is None:
             schema = DataSchema()
@@ -202,16 +214,18 @@
             schema = DataSchema(**schema)
 
         if metadata is None:
             metadata = {}
 
         checks = [Evals(m) if isinstance(m, str) else m for m in checks]
         for m in checks:
-            assert isinstance(m, (Evals, ParametricEval, TransformOp, ColumnOp, list))
-            # TODO: Check type of each element in the list - should be transformOp
+            assert isinstance(m, (Evals, ParametricEval, ColumnOp, list))
+            if isinstance(m, list):
+                for op in m:
+                    assert isinstance(op, ColumnOp)
 
         req_attrs, ser_checks = set(), []
         for idx, m in enumerate(checks):
             if m in [Evals.SUB_QUERY_COMPLETENESS]:
                 req_attrs.update([schema.sub_questions, schema.question])
             elif m in [Evals.CONTEXT_CONCISENESS]:
                 req_attrs.update(
@@ -261,31 +275,28 @@
             if isinstance(m, ParametricEval):
                 dictm = m.model_dump()
                 dictm.update({"scenario_description": this_scenario_description})
                 ser_checks.append({"check_name": m.__class__.__name__, **dictm})
             elif isinstance(m, Evals):
                 dictm = {"scenario_description": this_scenario_description}
                 ser_checks.append({"check_name": m.value, **dictm})
-            elif isinstance(m, TransformOp):
-                dictm = m.model_dump()
-                ser_checks.append({"check_name": m.__class__.__name__, **dictm})
             elif isinstance(m, ColumnOp):
                 dictm = m.model_dump()
                 ser_checks.append({"check_name": m.__class__.__name__, **dictm})
             elif isinstance(m, list):
                 ser_checks.append({"check_name": "dummy_list_ops"})
             else:
                 raise ValueError(f"Invalid metric: {m}")
 
         for idx, row in enumerate(data):
             if not req_attrs.issubset(row.keys()):
                 raise ValueError(
                     f"Row {idx} is missing required all required attributes for evaluation: {req_attrs}"
                 )
-
+        server_checks = copy.deepcopy(ser_checks)
         if self.settings.evaluate_locally:
             results = copy.deepcopy(data)
             for idx, check in enumerate(checks):
                 if (
                     isinstance(check, ParametricEval)
                     and ser_checks[idx]["check_name"]
                     in PARAMETRIC_EVAL_TO_OPERATOR_MAPPING
@@ -307,21 +318,14 @@
                         else scenario_description[idx]
                     )
                     res = (
                         op.setup(self.settings)
                         .run(pl.DataFrame(data))["output"]
                         .to_dicts()
                     )
-                elif isinstance(check, TransformOp):
-                    op = check
-                    res = (
-                        op.setup(self.settings)
-                        .run(pl.DataFrame(data))["output"]
-                        .to_dicts()
-                    )
                 elif isinstance(check, ColumnOp):
                     op = Check(name = "dummy", operators = [check])
                     res = (
                         op.setup(self.settings)
                         .run(pl.DataFrame(data))
                     ).to_dicts()
                 elif isinstance(check, list):
@@ -334,43 +338,45 @@
                     res = self.evaluate_on_server(data, [ser_checks[idx]], schema)
                 for idx, row in enumerate(res):
                     results[idx].update(row)
         else:
             results = self.evaluate_on_server(data, ser_checks, schema)
         ## local server calls
         try:
-            url = "http://localhost:4300/api/public/user"
             client = httpx.Client(
                 headers={"uptrain-access-token": "default_key"},
                 timeout=httpx.Timeout(7200, connect=5),
             )
-            response = client.post(url, json={"name": "default_key"})
 
-            user_id = response.json()["id"]
-            checks = []
-            for res in results:
-                row_check = {}
-                for key in res:
-                    if key.startswith("score") or key.startswith("explanation"):
-                        row_check.update({key: res[key]})
-                checks.append(row_check)
+            sink_data = copy.deepcopy(results)
+            for idx, data_point in enumerate(sink_data):
+                row_uuid= get_uuid()
+                data_point["row_uuid"] = row_uuid
+                for key_dict in list(data_point.keys()):
+                    if "confidence" in key_dict:
+                        data_point['score_confidence' + '_' + key_dict.split("confidence_")[-1]] = data_point[key_dict]
+                    if key_dict.startswith("score") and "confidence" not in key_dict:
+                        data_point["status_" + key_dict] = "not updated"
 
-            url = "http://localhost:4300/api/public/add_project_data"
+            url = self.settings.uptrain_local_url + "/api/public/add_project_data"
             response = client.post(
                 url,
                 json={
-                    "data": results,
-                    "checks": checks,
+                    "data": data,
+                    "sink_data": sink_data,
+                    "checks": server_checks,
                     "metadata": metadata,
                     "schema_dict": schema.model_dump(),
                     "project": project_name,
+                    "evaluation": evaluation_name,
+                    "exp_column": None if metadata.get("uptrain_experiment_columns", None) is None else metadata.get("uptrain_experiment_columns", None)[0]
                 },
             )
         except Exception:
-            user_id = "default_key"
+            #user_id = "default_key"
             logger.info("Local server not running, start the server to log data and visualize in the dashboard!")
         return results
 
     def evaluate_on_server(self, data, ser_checks, schema):
         # send in chunks of 50, so the connection doesn't time out waiting for the server
         results = []
         NUM_TRIES, BATCH_SIZE = 3, 50
@@ -401,14 +407,15 @@
 
     def evaluate_experiments(
         self,
         project_name: str,
         data: t.Union[list[dict], pl.DataFrame],
         checks: list[t.Union[str, Evals, ParametricEval]],
         exp_columns: list[str],
+        evaluation_name: t.Optional[str] = None,
         schema: t.Union[DataSchema, dict[str, str], None] = None,
         metadata: t.Optional[dict[str, t.Any]] = None,
     ):
         """Evaluate experiments on the given data.
 
         Args:
             project_name: Name of the project.
@@ -419,24 +426,27 @@
             metadata: Attributes to attach to this dataset. Useful for filtering and grouping in the UI.
 
         Returns:
             results: List of dictionaries with each data point and corresponding evaluation results for all the experiments.
         """
         if metadata is None:
             metadata = {}
-
+        if evaluation_name is None:
+            evaluation_name = "Expt - " + str(datetime.utcnow())
+        
         metadata.update({"uptrain_experiment_columns": exp_columns})
 
         if schema is None:
             schema = DataSchema()
         elif isinstance(schema, dict):
             schema = DataSchema(**schema)
 
         results = self.evaluate(
             project_name=project_name,
+            evaluation_name=evaluation_name,
             data=data,
             checks=checks,
             schema=schema,
             metadata=metadata,
         )
 
         results = pl.DataFrame(results)
```

### Comparing `uptrain-0.6.9/uptrain/framework/evals.py` & `uptrain-0.7.0/uptrain/framework/evals.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     RESPONSE_ALIGNMENT_WITH_SCENARIO = "response_alignment_with_scenario"
     RESPONSE_SINCERITY_WITH_SCENARIO = "response_sincerity_with_scenario"
     PROMPT_INJECTION = "prompt_injection"
     CODE_HALLUCINATION = "code_hallucination"
     SUB_QUERY_COMPLETENESS = "sub_query_completeness"
     CONTEXT_RERANKING = "context_reranking"
     CONTEXT_CONCISENESS = "context_conciseness"
+    MULTI_QUERY_ACCURACY = "multi_query_accuracy"
+    QUESTION_COMPLETENESS = "question_completeness"
 
 
 class ParametricEval(BaseModel):
     model_config = ConfigDict(protected_namespaces=())
 
 
 class CritiqueTone(ParametricEval):
```

### Comparing `uptrain-0.6.9/uptrain/framework/remote.py` & `uptrain-0.7.0/uptrain/framework/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import typing as t
 
 from loguru import logger
 from pydantic import BaseModel
 import httpx
 import polars as pl
+from datetime import datetime
 import pandas as pd
 
 from uptrain.framework.checks import CheckSet, ExperimentArgs
 from uptrain.framework.base import Settings
 from uptrain.framework.evals import (
     Evals,
     JailbreakDetection,
@@ -43,14 +44,15 @@
     scenario: str = "scenario"
     objective: str = "objective"
 
     ##rag_evals
     sub_questions: str = "sub_questions"
     reranked_context: str = "reranked_context"
     concise_context: str = "concise_context"
+    variants: str = "variants"
 
 
 def raise_or_return(response: httpx.Response):
     if not response.is_success:
         logger.error(response.text)
         response.raise_for_status()
     else:
@@ -548,33 +550,37 @@
         return results
 
     def log_and_evaluate(
         self,
         project_name: str,
         data: t.Union[list[dict], pl.DataFrame, pd.DataFrame],
         checks: list[t.Union[str, Evals, ParametricEval]],
+        evaluation_name: t.Optional[str] = None,
         scenario_description: t.Optional[str] = None,
         schema: t.Union[DataSchema, dict[str, str], None] = None,
         metadata: t.Optional[dict[str, t.Any]] = None,
     ):
         """Run an evaluation on the server and log the results.
         NOTE: This api is a bit different than the regular `evaluate` call.
 
         Args:
-            project_name: Name of the project to evaluate on.
+            project_name: Name of the project.
+            evaluation_name: Name of the Run to evaluate on.
             data: Data to evaluate on. Either a Pandas DataFrame or a list of dicts.
             checks: List of checks to evaluate on.
             schema: Schema of the data. Only required if the data attributes aren't typical (question, response, context).
             metadata: Attributes to attach to this dataset. Useful for filtering and grouping in the UI.
 
         Returns:
             results: List of dictionaries with each data point and corresponding evaluation results.
         """
+        if evaluation_name is None:
+            evaluation_name = "Eval - " + str(datetime.utcnow())
+        
         url = f"{self.base_url}/log_and_evaluate"
-
         if isinstance(data, pl.DataFrame):
             data = data.to_dicts()
         elif isinstance(data, pd.DataFrame):
             data = data.to_dict(orient="records")
 
         if schema is None:
             schema = DataSchema()
@@ -588,14 +594,16 @@
         for m in checks:
             assert isinstance(m, (Evals, ParametricEval))
 
         req_attrs, ser_checks = set(), []
         for m in checks:
             if m in [Evals.SUB_QUERY_COMPLETENESS]:
                 req_attrs.update([schema.sub_questions, schema.question])
+            elif m in [Evals.MULTI_QUERY_ACCURACY]:
+                req_attrs.update([schema.question, schema.variants])
             elif m in [Evals.CONTEXT_CONCISENESS]:
                 req_attrs.update(
                     [schema.question, schema.context, schema.concise_context]
                 )
             elif m in [Evals.CONTEXT_RERANKING]:
                 req_attrs.update(
                     [schema.question, schema.context, schema.reranked_context]
@@ -672,14 +680,15 @@
                     response = self.client.post(
                         url,
                         json={
                             "data": data[i : i + BATCH_SIZE],
                             "checks": ser_checks,
                             "metadata": {
                                 "project": project_name,
+                                "evaluation": evaluation_name,
                                 "schema": schema.model_dump(),
                                 **metadata,
                                 "uptrain_settings": self.settings.model_dump(),
                             },
                         },
                     )
                     response_json = raise_or_return(response)
@@ -693,46 +702,51 @@
             if response_json is not None:
                 results.extend(response_json)
 
         return results
 
     def evaluate_experiments(
         self,
-        project_name: str,
         data: t.Union[list[dict], pl.DataFrame],
         checks: list[t.Union[str, Evals, ParametricEval]],
         exp_columns: list[str],
+        project_name: str,
+        evaluation_name: t.Optional[str] = None,
         schema: t.Union[DataSchema, dict[str, str], None] = None,
         metadata: t.Optional[dict[str, t.Any]] = None,
     ):
         """Evaluate experiments on the server and log the results.
 
         Args:
-            project_name: Name of the experiment to evaluate on.
             data: Data to evaluate on. Either a Pandas DataFrame or a list of dicts.
             checks: List of checks to evaluate on.
             exp_columns: List of columns/keys which denote different experiment configurations.
+            project_name: Name of the project.
+            evaluation_name: Name of the Run to evaluate on.
             schema: Schema of the data. Only required if the data attributes aren't typical (question, response, context).
             metadata: Attributes to attach to this dataset. Useful for filtering and grouping in the UI.
 
         Returns:
             results: List of dictionaries with each data point and corresponding evaluation results for all the experiments.
         """
+        if evaluation_name is None:
+            evaluation_name = "Expt - " + str(datetime.utcnow())
         if metadata is None:
             metadata = {}
 
         metadata.update({"uptrain_experiment_columns": exp_columns})
 
         if schema is None:
             schema = DataSchema()
         elif isinstance(schema, dict):
             schema = DataSchema(**schema)
 
         results = self.log_and_evaluate(
             project_name=project_name,
+            evaluation_name=evaluation_name,
             data=data,
             checks=checks,
             schema=schema,
             metadata=metadata,
         )
 
         results = pl.DataFrame(results)
```

### Comparing `uptrain-0.6.9/uptrain/framework/signal.py` & `uptrain-0.7.0/uptrain/framework/signal.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/integrations/llama_index.py` & `uptrain-0.7.0/uptrain/integrations/llama_index.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/integrations/promptfoo.py` & `uptrain-0.7.0/uptrain/integrations/promptfoo.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,17 +25,17 @@
             logger.error("Try running npx promptfoo@" + pr_u.PROMPTFOO_version)
 
     def evaluate(
         self,
         evals_list: t.Union[list],
         evals_weight: t.Union[list],
         input_data: t.Union[list[dict], pl.DataFrame, pd.DataFrame],
-        threshold: t.Union[float],
         prompts: t.Union[str],
         providers: t.Union[list],
+        threshold: t.Optional[float] = 0.5,
         output_file: t.Optional[str] = "results_" + timestr + ".csv",
         port: t.Optional[int] = pr_u.generate_open_port(),
         eval_model: t.Optional[str] = "gpt-3.5-turbo-1106",
         project_name: t.Optional[str] = "EvalPromptfoo " + str(timestr),
         kill_process_on_exit: t.Optional[bool] = True,
     ) -> None:
         try:
@@ -93,25 +93,67 @@
                             "promptfoo@" + pr_u.PROMPTFOO_version,
                             "view",
                             "-y",
                             "-p",
                             str(port),
                         ]
                     )
-                    subprocess.run(
-                        ["npx", "promptfoo@latest", "view", "-y", "-p", str(port)]
-                    )
                 except Exception as e:
                     logger.error(
                         "Something failed: Try running !npx promptfoo@latest view" + e
                     )
 
             except Exception as e:
                 logger.error(f"Evaluation failed with error: {e}")
                 raise e
+        except Exception:
+            if kill_process_on_exit:
+                try:
+                    pid = subprocess.check_output(["lsof", "-t", "-i:" + str(port)])
+                    pids_str = pid.decode()
+                    pids = [
+                        int(pid)
+                        for pid in pids_str.split("\n")
+                        if pid.strip().isdigit()
+                    ]
+                    try:
+                        for pid in pids:
+                            subprocess.run(["kill", str(pid)])
+                        print(
+                            f"Closed application at http://localhost:{port} successfully"
+                        )
+                        print("To reopen it try running view method in EvalPromptfoo")
+                    except subprocess.CalledProcessError:
+                        pass
+                except Exception:
+                    print("No running process to close")
+            else:
+                return None
+
+    def view(
+        self, port: t.Optional[int] = pr_u.generate_open_port(),
+        kill_process_on_exit: t.Optional[bool] = True,
+        ) -> None:
+        try:
+            try:
+                subprocess.run(
+                    [
+                        "npx",
+                        "promptfoo@" + pr_u.PROMPTFOO_version,
+                        "view",
+                        "-y",
+                        "-p",
+                        str(port),
+                    ]
+                )
+            except Exception as e:
+                logger.error(
+                    "Something failed: Try running !npx promptfoo@latest view" + e
+                )
+        
         except:
             if kill_process_on_exit:
                 try:
                     pid = subprocess.check_output(["lsof", "-t", "-i:" + str(port)])
                     pids_str = pid.decode()
                     pids = [
                         int(pid)
@@ -128,27 +170,12 @@
                     except subprocess.CalledProcessError as e:
                         pass
                 except:
                     print("No running process to close")
             else:
                 return None
 
-    def view(self, port: t.Optional[int] = pr_u.generate_open_port()):
-        try:
-            subprocess.run(
-                [
-                    "npx",
-                    "promptfoo@" + pr_u.PROMPTFOO_version,
-                    "view",
-                    "-y",
-                    "-p",
-                    str(port),
-                ]
-            )
-        except Exception as e:
-            logger.error("Something failed: Try running !npx promptfoo@latest view" + e)
-
     def custom(self, command: t.Union[str] = "init"):
         try:
             subprocess.run(["npx", "promptfoo@" + pr_u.PROMPTFOO_version, command])
         except Exception as e:
             logger.error("Something failed: " + e)
```

### Comparing `uptrain-0.6.9/uptrain/integrations/promptfoo_utils.py` & `uptrain-0.7.0/uptrain/integrations/promptfoo_utils.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/__init__.pyi` & `uptrain-0.7.0/uptrain/operators/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -56,28 +56,31 @@
     "ContextRelevance",
     "ResponseRelevance",
     "ResponseCompleteness",
     "ResponseCompletenessWrtContext",
     "ResponseConsistency",
     "ResponseConciseness",
     "ValidQuestionScore",
+    "QueryRewrite",
     "LanguageCritique",
     "ToneCritique",
     "GuidelineAdherenceScore",
     "PromptInjectionScore",
     "ConversationSatisfactionScore",
     "ResponseMatchingScore",
     "ValidResponseScore",
     "TopicAssignmentviaCluster",
     "JailbreakDetectionScore",
     "PromptInjectionScore",
     "ResponseCoherence",
     "SubQueryCompleteness",
     "ContextReranking",
     "ContextConciseness",
+    "CustomPromptEvalScore",
+    "MultiQueryAccuracy",
     # io - also include all the subimports
     "io",
     "ExcelReader",
     "CsvReader",
     "JsonReader",
     "JsonWriter",
     "DeltaReader",
@@ -149,32 +152,34 @@
 from .language.context_quality import (
     ContextRelevance,
     ResponseCompletenessWrtContext,
     ContextConciseness,
     ContextReranking,
 )
 from .language.subquery import SubQueryCompleteness
+from .language.multiquery import MultiQueryAccuracy
 from .language.response_quality import (
     ResponseCompleteness,
     ResponseConsistency,
     ResponseConciseness,
     ValidResponseScore,
     ResponseRelevance,
     ResponseMatchingScore,
 )
-from .language.question_quality import ValidQuestionScore
+from .language.question_quality import ValidQuestionScore, QueryRewrite
 from .language.language_quality import LanguageCritique, ResponseCoherence
 from .language.tone import ToneCritique
 from .language.guideline import GuidelineAdherenceScore
 from .language.conversation import ConversationSatisfactionScore
 from .language.topic import TopicAssignmentviaCluster
 from .language.jailbreak import (
     PromptInjectionScore,
     JailbreakDetectionScore,
 )
+from .language.custom import CustomPromptEvalScore
 
 from . import io
 from .io.base import CsvReader, JsonReader, DeltaReader, JsonWriter, DeltaWriter
 from .io.excel import ExcelReader
 from .io.bq import BigQueryReader, BigQueryWriter
 from .io.mongodb import MongoDBReader
 from .io.duck import DuckDBReader
```

### Comparing `uptrain-0.6.9/uptrain/operators/base.py` & `uptrain-0.7.0/uptrain/operators/base.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/chart.py` & `uptrain-0.7.0/uptrain/operators/chart.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/clustering.py` & `uptrain-0.7.0/uptrain/operators/clustering.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/code/detection.py` & `uptrain-0.7.0/uptrain/operators/code/detection.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/code/sql.py` & `uptrain-0.7.0/uptrain/operators/code/sql.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/drift.py` & `uptrain-0.7.0/uptrain/operators/drift.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/embedding/embedding.py` & `uptrain-0.7.0/uptrain/operators/embedding/embedding.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,10 +213,10 @@
                                 logger.error(f"Error while computing embeddings: {e}")
                                 if len(run_res) != 0:
                                     run_res.append(run_res[-1])
                                 else:
                                     run_res.append([0] * emb_length)
             results.extend(run_res)
             logger.info(
-                f"Running batch: {idx} out of {int(np.ceil(len(inputs)/BATCH_SIZE))} for operator Embedding"
+                f"Running batch: {idx + 1} out of {int(np.ceil(len(inputs)/BATCH_SIZE))} for operator Embedding"
             )
         return {"output": data.with_columns([pl.Series(results).alias(self.col_out)])}
```

### Comparing `uptrain-0.6.9/uptrain/operators/embedding/vector_search.py` & `uptrain-0.7.0/uptrain/operators/embedding/vector_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,30 +25,33 @@
 
 @register_op
 class VectorSearch(TransformOp):
     """
 
      Attributes:
         col_in_query (str): Column name for the input query to be used for retrieval
-        documents (str): List of documents for vector database.
-        embeddings_model (str): Name of the embeddings model
+        colk_in_document (str): Column name for the input document to be used for retrieval
         col_out (str): Column name for the retrieved_context
+        documents (t.Union[list[str], str, JsonReader, CsvReader]): List of documents or path to the file containing the documents
+        embeddings_model (str): Name of the embeddings model
         top_k (int): Top K documents will be retrieved.
         distance_metric (str): One of ['cosine_similarity', 'l2_distance']
+        embedding_batch_size (int): Batch size for the embeddings model
+
     Raises:
         Exception: Raises exception for any failed evaluation attempts
 
     """
 
     col_in_query: str = "question"
+    col_in_document: str = ""
+    col_out: str = "context"
     documents: t.Union[list[str], str, JsonReader, CsvReader] = None
     embeddings_model: str = ""
-    col_out: str = "context"
     top_k: int = 1
-    col_in_document: str = ""
     distance_metric: str = t.Literal["cosine_similarity", "l2_distance"]
     embedding_batch_size: int = 128
 
     def setup(self, settings: t.Optional[Settings] = None):
         read_op = None
         if isinstance(self.documents, list):
             documents_table = pl.DataFrame({"document": self.documents})
```

### Comparing `uptrain-0.6.9/uptrain/operators/embs.py` & `uptrain-0.7.0/uptrain/operators/embs.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/io/base.py` & `uptrain-0.7.0/uptrain/operators/io/base.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/io/bq.py` & `uptrain-0.7.0/uptrain/operators/io/bq.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/io/duck.py` & `uptrain-0.7.0/uptrain/operators/io/duck.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/io/excel.py` & `uptrain-0.7.0/uptrain/operators/io/excel.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/io/mongodb.py` & `uptrain-0.7.0/uptrain/operators/io/mongodb.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/language/bleu.py` & `uptrain-0.7.0/uptrain/operators/language/bleu.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/language/context_quality.py` & `uptrain-0.7.0/uptrain/operators/language/context_quality.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/language/conversation.py` & `uptrain-0.7.0/uptrain/operators/language/conversation.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/language/factual_accuracy.py` & `uptrain-0.7.0/uptrain/operators/language/factual_accuracy.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/language/generation.py` & `uptrain-0.7.0/uptrain/operators/language/generation.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/language/grammar.py` & `uptrain-0.7.0/uptrain/operators/language/grammar.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/language/guideline.py` & `uptrain-0.7.0/uptrain/operators/language/guideline.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     score_mapping: dict = {"A": 1.0, "B": 0.0}
 
     def setup(self, settings: t.Optional[Settings] = None):
         from uptrain.framework.remote import APIClient
 
         assert settings is not None
         self.settings = settings
+        self.col_out = f"score_{self.guideline_name}_adherence"
         if self.settings.evaluate_locally and (
             self.settings.uptrain_access_token is None
             or not len(self.settings.uptrain_access_token)
         ):
             self._api_client = LLMMulticlient(settings)
         else:
             self._api_client = APIClient(settings)
@@ -174,23 +175,23 @@
         )
 
         results = []
 
         for res in output_payloads:
             idx = res.metadata["index"]
             output = {
-                "score_guideline_adherence": None,
-                "explanation_guideline_adherence": None,
+                f"score_{self.guideline_name}_adherence": None,
+                f"explanation_{self.guideline_name}_adherence": None,
             }
             try:
                 score = self.score_mapping[
                     json.loads(res.response.choices[0].message.content)["Choice"]
                 ]
-                output["score_guideline_adherence"] = float(score)
-                output["explanation_guideline_adherence"] = res.response.choices[
+                output[f"score_{self.guideline_name}_adherence"] = float(score)
+                output[f"explanation_{self.guideline_name}_adherence"] = res.response.choices[
                     0
                 ].message.content
             except Exception:
                 logger.error(
                     f"Error when processing payload at index {idx}: {res.error}"
                 )
             results.append((idx, output))
```

### Comparing `uptrain-0.6.9/uptrain/operators/language/jailbreak.py` & `uptrain-0.7.0/uptrain/operators/language/jailbreak.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/language/llm.py` & `uptrain-0.7.0/uptrain/operators/language/llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -211,39 +211,47 @@
                 self.aclient = AsyncOpenAI(
                     api_key=settings.together_api_key,
                     base_url="https://api.together.xyz/v1",
                 )
             if (
                 settings.model.startswith("ollama")
             ):
-                self.aclient = None
+                self.aclient = None        
             self._rpm_limit = settings.check_and_get("rpm_limit")
             self._tpm_limit = settings.check_and_get("tpm_limit")
 
     def make_payload(
         self,
         index: int,
         prompt: str,
         temperature: float = 0.1,
     ) -> Payload:
         model = self.settings.model
         seed = self.settings.seed
         response_format = self.settings.response_format
 
+        # For vllm
+        custom_llm_provider = self.settings.custom_llm_provider
+        api_base = self.settings.api_base
+
         prefixes = ["anyscale/", "azure/", "together/"]
         for prefix in prefixes:
             model = model.replace(prefix, "")
 
         messages = [{"role": "user", "content": prompt}]
 
         data = {"model": model, "messages": messages, "temperature": temperature}
         if seed is not None:
             data["seed"] = seed
         if response_format is not None:
             data["response_format"] = response_format
+        if custom_llm_provider is not None:
+            data["custom_llm_provider"] = custom_llm_provider
+        if api_base is not None:
+            data["api_base"] = api_base
         return Payload(
             endpoint="chat.completions",
             data=data,
             metadata={"index": index},
         )
 
     def fetch_responses(
```

### Comparing `uptrain-0.6.9/uptrain/operators/language/meteor.py` & `uptrain-0.7.0/uptrain/operators/language/meteor.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/language/model_grade.py` & `uptrain-0.7.0/uptrain/operators/language/model_grade.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/language/openai_eval_custom/completion_fns/dummy.py` & `uptrain-0.7.0/uptrain/operators/language/openai_eval_custom/completion_fns/dummy.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/language/openai_eval_custom/elsuite/model_run.py` & `uptrain-0.7.0/uptrain/operators/language/openai_eval_custom/elsuite/model_run.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/language/openai_evals.py` & `uptrain-0.7.0/uptrain/operators/language/openai_evals.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/language/prompts/classic.py` & `uptrain-0.7.0/uptrain/operators/language/prompts/classic.py`

 * *Files 14% similar despite different names*

```diff
@@ -317,15 +317,15 @@
 
 Task Data.
 [Persona]: {llm_persona}
 [Response]: {response}
 """
 
 
-# Critique Language Coherence
+# Coherence
 LANGUAGE_COHERENCE_PROMPT_TEMPLATE = """
 Please assess the language quality of the provided machine-generated response, and rate how coherent the response is, i.e. if the multiple parts of the response have conflicting information.
 
 {scenario_description}
 
 Example Data.
 {few_shot_examples}
@@ -340,34 +340,112 @@
 Return the output only in the corresponding JSON format. Do not output anything other than this JSON object:
 {output_format}
 
 Task Data.
 [Response]: {response}
 """
 
+
+# Critique Language Coherence
+LANGUAGE_CRITIQUE_COHERENCE_PROMPT_TEMPLATE = """
+You are a detail-oriented LLM which pays close attention to the details. You are given a text and your job is to evaluate the quality of the provided text, focusing on the coherence aspect.
+
+Coherence is the quality of the text that makes it logical and consistent. It is important that the text is well-organized and the ideas are connected in a clear and meaningful way. A coherent text is easy to follow and understand.
+
+Please provide a score on the scale of 1-5, with 1 meaning that the text is completely incoherent and the elements in the text do not stitch together to produce meaningful text, and 5 meaning that the text is completely coherent and the elements in the text stitch together to produce meaningful text.
+
+{scenario_description}
+
+Example Data.
+{few_shot_examples}
+
+First, analyze the text and determine how fluent and natural sounding it is. Consider the structure, connectivity of ideas, and overall readability of the text. Write down step-by-step reasoning to make sure that your conclusion is correct.
+
+{prompting_instructions}
+
+Return the output only in the corresponding JSON format. Do not output anything other than this JSON object:
+{output_format}
+
+Task data.
+[Resposne]: {response}
+"""
+
+
 # Critique Language Fluency
-LANGUAGE_FLUENCY_PROMPT_TEMPLATE = """
-Please assess the language quality of the provided machine-generated response, and rate how fluent the response is.
+LANGUAGE_CRITIQUE_FLUENCY_PROMPT_TEMPLATE = """
+You are a detail-oriented LLM which pays close attention to the details. You are given a text and your job is to evaluate the quality of the provided text, focusing on the fluency aspect.
+
+Fluency is the ability of the text to flow smoothly and naturally. It is important that the text is easy to read and understand. A fluent text is well-structured, coherent, and free of awkward phrasing.
+
+Please provide a score on the scale of 1-5, with 1 meaning that the text is not fluent at all and/or has awkward phrasing, and 5 meaning that the text is completely fluent and natural sounding.
+
+{scenario_description}
+
+Example Data.
+{few_shot_examples}
+
+First, analyze the text and determine how fluent and natural sounding it is. Consider the structure, connectivity of ideas, and overall readability of the text. Write down step-by-step reasoning to make sure that your conclusion is correct.
+
+{prompting_instructions}
+
+Return the output only in the corresponding JSON format. Do not output anything other than this JSON object:
+{output_format}
+
+Task data.
+[Resposne]: {response}
+"""
+
+
+# Critique Language Grammar
+LANGUAGE_CRITIQUE_GRAMMAR_PROMPT_TEMPLATE = """
+You are a detail-oriented LLM which pays close attention to the details. You are given a text and your job is to evaluate the quality of the provided text, focusing on the grammar aspect.
+
+Grammar is the correctness of the text in terms of spelling, punctuation, and sentence structure. It is important that the text is free of grammatical errors and follows the rules of the language.
+
+Please provide a score on the scale of 1-5, with 1 meaning that the text has many grammatical errors, and 5 meaning that the text has perfect grammar and word choice.
 
 {scenario_description}
 
 Example Data.
 {few_shot_examples}
 
-For the given task data, determine which case applies by selecting one of the following options:
-A. The response is highly fluent.
-B. The response is moderately fluent and can be improved.
-C. The response is not fluent at all.
+First, analyze the text and determine the grammar and word usage in the text.
+
 {prompting_instructions}
 
 Return the output only in the corresponding JSON format. Do not output anything other than this JSON object:
 {output_format}
 
-Task Data.
-[Response]: {response}
+Task data.
+[Resposne]: {response}
+"""
+
+
+# Critique Language Politeness
+LANGUAGE_CRITIQUE_POLITENESS_PROMPT_TEMPLATE = """
+You are a detail-oriented LLM which pays close attention to the details. You are given a text and your job is to evaluate the quality of the provided text, focusing on the politeness aspect.
+
+Politeness is the tone of the text and how polite or impolite it is. It is important that the text is written in a respectful and appropriate tone.
+
+Please provide a score on the scale of 1-5, with 1 meaning that the tone of the text is very rude or inappropriate, and 5 meaning that the tone of the text is extremely polite.
+
+{scenario_description}
+
+Example Data.
+{few_shot_examples}
+
+First, analyze the text and determine how polite or impolite the tone of the text is.
+
+{prompting_instructions}
+
+Return the output only in the corresponding JSON format. Do not output anything other than this JSON object:
+{output_format}
+
+Task data.
+[Resposne]: {response}
 """
 
 
 # Sub-query Completeness
 SUB_QUERY_COMPLETENESS_PROMPT_TEMPLATE = """
 You are given a question and a list of sub questions generated from an AI assistant. Please assess if the all sub-questions comprehensively cover the various aspects of the main question. 
 
@@ -467,7 +545,55 @@
 
 Return the output only in the corresponding JSON format. Do not output anything other than this JSON object:
 {output_format}
 
 Task data:
 [Response]: {response}
 """
+
+
+# Multi Query Accuracy
+MULTI_QUERY_ACCURACY_PROMPT_TEMPLATE = """
+You are given a question and list of variations of the same question. Your task is to determine if the given variations mean the same as the original question.
+
+It should consider the relevance and similarity of the given variations with respect to the original question. The goal is to generate a qualitative assessment of how well the variations collectively cover all relevant aspects of the main question.
+
+{scenario_description}
+
+Example Data.
+{few_shot_examples}
+
+Determine which case applies by selecting one of the following options:
+A. The given variations mean the same as the original question.
+B. The given variations partially mean the same as the original question.
+C. The given variations do not mean the same as the original question.
+
+{prompting_instructions}
+
+Return the output only in the corresponding JSON format. Do not output anything other than this JSON object:
+{output_format}
+
+Task data:
+[Question]: {question}
+[Variants]: {variants}
+"""
+
+# Query Rewrite Prompt
+QUERY_REWRITE_PROMPT_TEMPLATE = """
+
+You have been presented with a scenario where an AI assistant engages in a conversation with a user. 
+
+{scenario_description}
+
+The user poses a question within this dialogue. Your task is to rephrase the question provided in a manner that encapsulates the essence of the ongoing conversation. 
+Your rewritten question should be comprehensible independently of the preceding dialogue, yet it should seamlessly integrate the contextual nuances inferred from the conversation.
+
+
+{prompting_instructions}
+
+Return the output only in the corresponding JSON format. Do not output anything other than this JSON object:
+{output_format}
+
+Task data.
+[Question]: {question}
+[Conversation]: {conversation}
+"""
```

### Comparing `uptrain-0.6.9/uptrain/operators/language/prompts/few_shots.py` & `uptrain-0.7.0/uptrain/operators/language/prompts/few_shots.py`

 * *Files 10% similar despite different names*

```diff
@@ -366,61 +366,197 @@
     "Reasoning": "Although the machine doesn't help the user by directly providing the answers (which doesn't align with the helpful trait of the machine), it encourages the user to show their current progress and offers help by assisting in figuring the right answer. It is reasonable to expect a teacher to not just provide the answer but help the student in solving them, hence, the tone aligns moderately with the persona.",
     "Choice": "B"
 }
 """
 
 
 # Critique Language Fluency
-LANGUAGE_FLUENCY_FEW_SHOT__CLASSIFY = """
+LANGUAGE_CRITIQUE_FLUENCY_FEW_SHOT__CLASSIFY = """
 [Response]: Exercise is good  health. It makes body strong and helps the mind too. Many benefits gained.
 [Output]:
 {
-    "Choice": "B"
+    "Score": 3
 }
 
 [Response]: Exercises are very good for your health as they make the body physically strong as well as promote mental well-being.
 [Output]:
 {
-    "Choice": "A"
+    "Score": 5
 }
 
 
 [Response]: Exercise good  health your. It maken strong strong body, fit, mind and.
 [Output]:
 {
-    "Choice": "C"
+    "Score": 1
 }
 """
 
-LANGUAGE_FLUENCY_FEW_SHOT__COT = """
+LANGUAGE_CRITIQUE_FLUENCY_FEW_SHOT__COT = """
 [Response]: Exercise is good  health. It makes body strong and helps the mind too. Many benefits gained.
 [Output]:
 {
     "Reasoning": "The text is somewhat fluent but lacks variety in sentence structure and uses repetitive language.",
-    "Choice": "B"
+    "Score": 3
 }
 
 [Response]: Exercises are very good for your health as they make the body physically strong as well as promote mental well-being.
 [Output]:
 {
     "Reasoning": "The text is completely fluent and natural sounding.",
-    "Choice": "A"
+    "Score": 5
 }
 
 
 [Response]: Exercise good  health your. It maken strong strong body, fit, mind and.
 [Output]:
 {
     "Reasoning": "The text is not fluent at all and has awkward phrasing, making it difficult to understand.",
-    "Choice": "C"
+    "Score": 1
 }
 """
 
 
 # Critique Language Coherence
+LANGUAGE_CRITIQUE_COHERENCE_FEW_SHOT__CLASSIFY = """
+[Response]: Exercise is beneficial for both physical and mental health. It strengthens the body and uplifts the mind.
+[Output]:
+{
+    "Score": 5
+}
+
+[Response]: Regular exercise contributes to overall well-being by enhancing physical strength and mental clarity.
+[Output]:
+{
+    "Score": 4
+}
+
+[Response]: Exercise good. Health. Make body strong. Help mind. Benefits many.
+[Output]:
+{
+    "Score": 2
+}
+"""
+
+
+LANGUAGE_CRITIQUE_COHERENCE_FEW_SHOT__COT = """
+[Response]: Exercise is beneficial for both physical and mental health. It strengthens the body and uplifts the mind.
+[Output]:
+{
+    "Reasoning": "The text is coherent and effectively conveys the message with clear organization of ideas.",
+    "Score": 5
+}
+
+[Response]: Regular exercise contributes to overall well-being by enhancing physical strength and mental clarity.
+[Output]:
+{
+    "Reasoning": "The text maintains coherence by linking ideas logically, providing a clear flow of information.",
+    "Score": 4
+}
+
+[Response]: Exercise good. Health. Make body strong. Help mind. Benefits many.
+[Output]:
+{
+    "Reasoning": "The text lacks coherence, as it presents fragmented ideas without clear connections.",
+    "Score": 2
+}
+"""
+
+
+# Critique Language Grammar
+LANGUAGE_CRITIQUE_GRAMMAR_FEW_SHOT__CLASSIFY = """
+[Response]: Exercise is essential for maintaining good health. It strengthens the body and improves mental well-being.
+[Output]:
+{
+    "Score": 5
+}
+
+[Response]: Exercises is important for healthiness. It makes body strong and helps the mind too.
+[Output]:
+{
+    "Score": 3
+}
+
+[Response]: Exercise good for healthy. It make body strong and help mind.
+[Output]:
+{
+    "Score": 2
+}
+"""
+
+LANGUAGE_CRITIQUE_GRAMMAR_FEW_SHOT__COT = """
+[Response]: Exercise is essential for maintaining good health. It strengthens the body and improves mental well-being.
+[Output]:
+{
+    "Reasoning": "The text demonstrates proper grammar usage and sentence structure.",
+    "Score": 5
+}
+
+[Response]: Exercises is important for healthiness. It makes body strong and helps the mind too.
+[Output]:
+{
+    "Reasoning": "The text contains some grammatical errors, such as subject-verb agreement and pluralization.",
+    "Score": 3
+}
+
+[Response]: Exercise good for healthy. It make body strong and help mind.
+[Output]:
+{
+    "Reasoning": "The text has several grammatical errors, such as missing articles and incorrect verb forms.",
+    "Score": 2
+}
+"""
+
+
+# Critique Language Politness
+LANGUAGE_CRITIQUE_POLITENESS_FEW_SHOT__CLASSIFY = """
+[Response]: Thank you for considering my application. I appreciate the opportunity to interview for the position.
+[Output]:
+{
+    "Score": 5
+}
+
+[Response]: Thanks for considering my application. I appreciate the opportunity to interview for the position.
+[Output]:
+{
+    "Score": 4
+}
+
+[Response]: Consider my application. Interview for position.
+[Output]:
+{
+    "Score": 1
+}
+"""
+
+LANGUAGE_CRITIQUE_POLITENESS_FEW_SHOT__COT = """
+[Response]: Thank you for considering my application. I appreciate the opportunity to interview for the position.
+[Output]:
+{
+    "Reasoning": "The text is very polite and courteous, expressing gratitude and appreciation.",
+    "Score": 5
+}
+
+[Response]: Thanks for considering my application. I appreciate the opportunity to interview for the position.
+[Output]:
+{
+    "Reasoning": "The text is polite, but could be slightly improved with a more formal expression such as 'thank you'.",
+    "Score": 4
+}
+
+[Response]: Consider my application. Interview for position.
+[Output]:
+{
+    "Reasoning": "The text lacks politeness and appears rather abrupt, lacking in courtesy.",
+    "Score": 1
+}
+"""
+
+
+# Response Coherence
 LANGUAGE_COHERENCE_FEW_SHOT__CLASSIFY = """
 [Response]: Exercise is good  health. It makes body strong and helps the mind too. Many benefits gained.
 [Output]:
 {
     "Choice": "B"
 }
 
@@ -591,7 +727,34 @@
     "3. The provided content is SQL syntax, which is a programming language used for database queries.",
     "4. The text does not just mention a function or method but includes an actual code example in SQL."
   ],
   "Choice": "A",
   "Snippet": "SELECT * FROM hospitals WHERE name = \"St. Mary's Hospital\";"
 }
 """
+
+
+# Multi query accuracy
+MULTI_QUERY_ACCURACY_FEW_SHOT__CLASSIFY = """
+[Question]: What are the main causes of climate change?
+[Variants]: 
+    1. What factors contribute to climate change?
+    2. Please explain the primary reasons for global warming.
+    3. How do human activities impact climate change?
+[Output]:
+{
+    "Choice": "A"
+}
+"""
+
+MULTI_QUERY_ACCURACY_FEW_SHOT__COT = """
+[Question]: What are the main causes of climate change?
+[Variants]: 
+    1. What factors contribute to climate change?
+    2. Please explain the primary reasons for global warming.
+    3. How do human activities impact climate change?
+[Output]:
+{
+    "Reasoning": "The response provides accurate and relevant information about the main causes of climate change, addressing the various aspects of the question across different queries. It covers the factors contributing to climate change, the impact of human activities, and the primary reasons for global warming, demonstrating a comprehensive understanding of the topic.",
+    "Choice": "A"
+}
+"""
```

### Comparing `uptrain-0.6.9/uptrain/operators/language/prompts/output_format.py` & `uptrain-0.7.0/uptrain/operators/language/prompts/output_format.py`

 * *Files 20% similar despite different names*

```diff
@@ -210,29 +210,74 @@
     "Reasoning": [Reasoning],  # Reasoning to determine if the response tone matches the given persona,
     "Choice": [Selected Choice],  # Choice selected for the given task data, one of ("A", "B", "C")
 }
 """
 
 
 # Critique Language Fluency
-LANGUAGE_FLUENCY_OUTPUT_FORMAT__CLASSIFY = """
+LANGUAGE_CRITIQUE_FLUENCY_OUTPUT_FORMAT__CLASSIFY = """
 {
-    "Choice": [Selected Choice],  # Choice selected for the given task data, one of ("A", "B", "C")
+    "Score": [Score],  # Score between 1 to 5, to evaluate the fluency of the response,
 }
 """
 
-LANGUAGE_FLUENCY_OUTPUT_FORMAT__COT = """
+LANGUAGE_CRITIQUE_FLUENCY_OUTPUT_FORMAT__COT = """
 {
     "Reasoning": [Reasoning],  # Reasoning to critique the fluency of the response,
-    "Choice": [Selected Choice],  # Choice selected for the given task data, one of ("A", "B", "C")
+    "Score": [Score],  # Score between 1 to 5, to evaluate the fluency of the response,
 }
 """
 
 
 # Critique Language Coherence
+LANGUAGE_CRITIQUE_COHERENCE_OUTPUT_FORMAT__CLASSIFY = """
+{
+    "Score": [Score],  # Score between 1 to 5, to evaluate the coherence of the response,
+}
+"""
+
+LANGUAGE_CRITIQUE_COHERENCE_OUTPUT_FORMAT__COT = """
+{
+    "Reasoning": [Reasoning],  # Reasoning to critique the coherence of the response,
+    "Score": [Score],  # Score between 1 to 5, to evaluate the coherence of the response,
+}
+"""
+
+
+# Critique Language Grammar
+LANGUAGE_CRITIQUE_GRAMMAR_OUTPUT_FORMAT__CLASSIFY = """
+{
+    "Score": [Score],  # Score between 1 to 5, to evaluate the grammar of the response,
+}
+"""
+
+LANGUAGE_CRITIQUE_GRAMMAR_OUTPUT_FORMAT__COT = """
+{
+    "Reasoning": [Reasoning],  # Reasoning to critique the grammar of the response,
+    "Score": [Score],  # Score between 1 to 5, to evaluate the grammar of the response,
+}
+"""
+
+
+# Critique Language Politeness
+LANGUAGE_CRITIQUE_POLITENESS_OUTPUT_FORMAT__CLASSIFY = """
+{
+    "Score": [Score],  # Score between 1 to 5, to evaluate the politeness of the response,
+}
+"""
+
+LANGUAGE_CRITIQUE_POLITENESS_OUTPUT_FORMAT__COT = """
+{
+    "Reasoning": [Reasoning],  # Reasoning to critique the politeness of the response,
+    "Score": [Score],  # Score between 1 to 5, to evaluate the politeness of the response,
+}
+"""
+
+
+# Coherence
 LANGUAGE_COHERENCE_OUTPUT_FORMAT__CLASSIFY = """
 {
     "Choice": [Selected Choice],  # Choice selected for the given task data, one of ("A", "B", "C")
 }
 """
 
 LANGUAGE_COHERENCE_OUTPUT_FORMAT__COT = """
@@ -298,7 +343,55 @@
 CODE_HALLUCINATION_OUTPUT_FORMAT__COT = """
 {
     "Reasoning": [Reasoning],  # Reasoning to critique the hallucination of the code,
     "Choice": [Selected Choice],  # Choice selected for the given task data, one of ("A", "B"),
     "Snippet": [Code Snippet],  # Code snippet (if any) found in the response,
 }
 """
+
+
+COT_CLASSIFY_JSON_OUTPUT_FORMAT = """
+You are given {num_choices} choices:
+{choices}
+
+Respond with one of the given choices which you think is most suitable for the given case. And write down a step-by-step explanation for your selected choice. 
+I WILL TIP YOU IF YOU WRITE DOWN THE SELECTED CHOICE, WORD-TO-WORD MATCHING WITH ONE OF THE CHOICES SPECIFIED ABOVE.
+
+Return the output only in the corresponding JSON format. Do not output anything other than this JSON object:
+{output_format}
+
+"""
+
+
+CLASSIFY_JSON_OUTPUT_FORMAT = """
+You are given {num_choices} choices:
+{choices}
+
+Respond with one of the given choices which you think is most suitable for the given case.
+I WILL TIP YOU IF YOU WRITE DOWN THE SELECTED CHOICE, WORD-TO-WORD MATCHING WITH ONE OF THE CHOICES SPECIFIED ABOVE.
+
+Return the output only in the corresponding JSON format. Do not output anything other than this JSON object:
+{output_format}
+
+"""
+
+
+# Multi Query Accuracy
+MULTI_QUERY_ACCURACY_OUTPUT_FORMAT__CLASSIFY = """
+{
+    "Choice": [Selected Choice],  # Choice selected for the given task data, one of ("A", "B", "C")
+}
+"""
+
+MULTI_QUERY_ACCURACY_OUTPUT_FORMAT__COT = """
+{
+    "Reasoning": [Reasoning],  # Reasoning to determine the accuracy of the variations of the given query,
+    "Choice": [Selected Choice],  # Choice selected for the given task data, one of ("A", "B", "C")
+}
+"""
+
+# Query Rewrite
+QUERY_REWRITE_OUTPUT_FORMAT__CLASSIFY = """
+{
+    "Question": [Rewritten Question],
+}
+"""
```

### Comparing `uptrain-0.6.9/uptrain/operators/language/response_quality.py` & `uptrain-0.7.0/uptrain/operators/language/response_quality.py`

 * *Files 1% similar despite different names*

```diff
@@ -899,15 +899,15 @@
         output_recall = output[len(data) :]
 
         results = []
         for combined_row in zip(output_precision, output_recall):
             precision = combined_row[0]["score_factual_accuracy"]
             recall = combined_row[1]["score_factual_accuracy"]
             output = {
-                "score_response_matching": None,
+                "score_response_match": None,
                 "explanation_response_matching": None,
                 "score_response_match_recall": None,
                 "score_response_match_precision": None,
             }
             if precision is not None and recall is not None:
                 explanation = (
                     "Information Recall: "
@@ -917,16 +917,16 @@
                     + "Information Precision: "
                     + str(precision)
                     + str(combined_row[0]["explanation_factual_accuracy"])
                 )
                 output["explanation_response_matching"] = explanation
 
                 if precision != 0 and recall != 0:
-                    output["score_response_matching"] = 4 * (
+                    output["score_response_match"] = 4 * (
                         (precision * recall) / (precision * 3 + recall)
                     )
                 else:
-                    output["score_response_matching"] = 0.0
+                    output["score_response_match"] = 0.0
                 output["score_response_match_recall"] = recall
                 output["score_response_match_precision"] = precision
             results.append(output)
         return results
```

### Comparing `uptrain-0.6.9/uptrain/operators/language/rouge.py` & `uptrain-0.7.0/uptrain/operators/language/rouge.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/language/subquery.py` & `uptrain-0.7.0/uptrain/operators/language/subquery.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/language/text.py` & `uptrain-0.7.0/uptrain/operators/language/text.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/language/tone.py` & `uptrain-0.7.0/uptrain/operators/language/tone.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/language/topic.py` & `uptrain-0.7.0/uptrain/operators/language/topic.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/metrics.py` & `uptrain-0.7.0/uptrain/operators/metrics.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/rca/rag_with_citation.py` & `uptrain-0.7.0/uptrain/operators/rca/rag_with_citation.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/similarity.py` & `uptrain-0.7.0/uptrain/operators/similarity.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/operators/table.py` & `uptrain-0.7.0/uptrain/operators/table.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/st_classic/st_helpers.py` & `uptrain-0.7.0/uptrain/st_classic/st_helpers.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/st_classic/st_run.py` & `uptrain-0.7.0/uptrain/st_classic/st_run.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/st_classic/st_setup.py` & `uptrain-0.7.0/uptrain/st_classic/st_setup.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/utilities/__init__.py` & `uptrain-0.7.0/uptrain/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/utilities/prompt_utils.py` & `uptrain-0.7.0/uptrain/utilities/prompt_utils.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/utilities/sql_utils.py` & `uptrain-0.7.0/uptrain/utilities/sql_utils.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/utilities/sql_utils_test.py` & `uptrain-0.7.0/uptrain/utilities/sql_utils_test.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/utilities/sqlglot_test.py` & `uptrain-0.7.0/uptrain/utilities/sqlglot_test.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain/utilities/utils.py` & `uptrain-0.7.0/uptrain/utilities/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     "response_alignment_with_scenario": Evals.RESPONSE_ALIGNMENT_WITH_SCENARIO,
     "response_sincerity_with_scenario": Evals.RESPONSE_SINCERITY_WITH_SCENARIO,
     "prompt_injection": Evals.PROMPT_INJECTION,
     "code_hallucination": Evals.CODE_HALLUCINATION,
     "sub_query_completeness": Evals.SUB_QUERY_COMPLETENESS,
     "context_reranking": Evals.CONTEXT_RERANKING,
     "context_conciseness ": Evals.CONTEXT_CONCISENESS,
+    "multi_query_accuracy": Evals.MULTI_QUERY_ACCURACY,
 }
 
 parametric_evals_mapping = {
     "CritiqueTone": CritiqueTone,
     "GuidelineAdherence": GuidelineAdherence,
     "ConversationSatisfaction": ConversationSatisfaction,
     "ResponseMatching": ResponseMatching,
@@ -84,14 +85,15 @@
 
 
 def create_dirs(path: str):
     dirs_to_create = [
         os.path.join(path),
         os.path.join(path, "uptrain-datasets"),
         os.path.join(path, "uptrain-eval-results"),
+        os.path.join(path, 'temp-datasets')
     ]
     for _dir in dirs_to_create:
         os.makedirs(_dir, exist_ok=True)
     return
 
 
 def get_sqlite_utils_db(fpath: str):
```

### Comparing `uptrain-0.6.9/uptrain/validation_wrapper/validation_manager.py` & `uptrain-0.7.0/uptrain/validation_wrapper/validation_manager.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.9/uptrain.egg-info/PKG-INFO` & `uptrain-0.7.0/uptrain.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uptrain
-Version: 0.6.9
+Version: 0.7.0
 Summary: UpTrain - tool to evaluate LLM applications on aspects like factual accuracy, response quality, retrieval quality, tonality, etc.
 Maintainer-email: UpTrain AI Team <oss@uptrain.ai>
 License: Apache-2.0
 Project-URL: Homepage, https://uptrain.ai
 Project-URL: Repository, https://github.com/uptrain-ai/uptrain
 Keywords: uptrain,ai,LLM,evaluation,hallucinations,observability,response quality
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,14 +28,17 @@
 Requires-Dist: plotly>=5.0.0
 Requires-Dist: aiolimiter>=1.1
 Requires-Dist: openai>=1.6.1
 Requires-Dist: fsspec
 Requires-Dist: litellm
 Requires-Dist: pyyaml
 Requires-Dist: json5
+Requires-Dist: python-docx
+Requires-Dist: pymupdf
+Requires-Dist: faiss-cpu
 Provides-Extra: test
 Requires-Dist: pytest>=7.0; extra == "test"
 
 <h4 align="center">
   <a href="https://uptrain.ai">
    <img alt="Logo of UpTrain - an open-source platform to evaluate and improve LLM applications" src="https://github.com/uptrain-ai/uptrain/assets/108270398/b6a4905f-63fd-47ab-a894-1026a6669c86"/>
   </a>
@@ -49,15 +52,18 @@
         <img alt="Read Docs" src="https://img.shields.io/badge/Read%20Docs-uptrain?logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAAGQAAABkCAYAAABw4pVUAAAACXBIWXMAAAsTAAALEwEAmpwYAAAC%2FklEQVR4nO3dO2sUURiH8SPipVAhKngJWggKolZ%2BAEGQIFiaL2CICNoLBmJAsBAbKxEREcTAYq%2BFYKGx8orxFkmhEltNY6P4yIEjs5FlJ4k7s%2B975v%2BD6ZJhD0%2FenZnsMhOCiIiIiIhIQwFbgFHgCjAJtPq83QF2hqYBNgNXgZ%2FYMwvsCE0B7E2LtuwjMBga8hb1CR9mso8C3MWXGWB7yBFwAPiNP2%2FjZIfcABfw6z2wLeQEuIdv74CtIRfA85IFv%2BnDdceTJUZ5FU%2FZQw6A6ZLFTvThNQ2zdC%2BBTcG7jIJEL9xHySzI3ygbg1cZBiEdF31GyTRI9AwYCN5kHIR0trYheJJ5kGgKWB%2B8aECQ6HHfogBHgJvpX%2BlPF%2FHzTQgSnat7EYPAAxaaXsTvNSXIRJ0L2APMdXgRClJ3kHgWAXygMwXpQ5Bu%2Fz73GmQAOLjEbbbv6wBWA99zC7IcJtaRzqi6UZCag5ymOwWpOcg43SlIzUEm6E5BCgrSxIO6JiRRkIXfBz5b8TYSSihIAuyjej6OhRbeslAQBelEE5JoQtroLaugCUk0IW00IQVNSALsip%2FdV7y1QgkFMUZBjFEQYxTEGAVJdNrbRqe9BU1IoglpowkpaEISTUgbTUhBE5JoQtpoQgqakIXfvh%2BueBsKJRTEGAUxRkGMURBjFMQYBTFGQYzJKcjrkn20arjO6MX2uWQd416CPKQZTnkJco1mOOwlyDHy9w1Y5SXIykUcR7w7X3mMXgVJ%2Bzlk9IkIvboD9jpXQdK%2BRoBf5OULsLvaChUFSfsbcvSUhDL3a78Nea%2BDpH2uBU6mW5DPOZqaH%2Bn5IjdqOaOqK4j8BwUxRkGMURBjFMQYBTFGQYxREGPi3ZpLrkPmDTw2tbWM7UzwCDhBni4Fj4D95Ol48Co9RS0n864eL%2FGv%2BNdEXsaCd8B18jAFrAnexUWkB9F79iibh0NGwApgFPiKv2PGWLyPfchRmpajwEXgloFrilaH7TZwOX3BrZ7Pu0VERERERIJ9fwBA%2FZMtFhwT0AAAAABJRU5ErkJggg%3D%3D&labelColor=976DA5&color=6A6A6A">
     </a>
     </a>
     <a href="https://join.slack.com/t/uptraincommunity/shared_invite/zt-1yih3aojn-CEoR_gAh6PDSknhFmuaJeg">
         <img alt="Slack Community" src="https://img.shields.io/badge/Slack%20Community-uptrain?logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAAGQAAABkCAYAAABw4pVUAAAACXBIWXMAAAsTAAALEwEAmpwYAAADFklEQVR4nO2cPW4TURSFLaWBhg6xACs9YhEsISiLiIzoUkGNRIV3kDSxhJVVBArKrCBUSCnCTyTc8KGRphomjsfv3vGBdz7JpY%2Bu5iQz9v3kN5kYY4wxxhhjjDHG%2FAXwGDgGPgJfgRXwBfgAHAJ7u8yrCuAI%2BM56LoFnu8irCuA9m3MLPB8zryrav%2BSh3AD7Y%2BRVRXuP%2F8Z2nGfnVUf7wC1hmplXHcBF4QWcZeZVB3BdeAHnmXnVAfwqvIBnnbzfkXnVAVwVXsBFJ4%2FIvOoAli5EiHZ94f8QFZpdUru%2B8C1LBeAp8NPPECGaXVK7vhiKH%2BqJpew36wtciBbAFHjZbmwX97xedd5bSt0fe6PBhWiBC9GC2gvpcdbRrIY48OxCpB39hs46mst1DjyzEGlHP9BZR3N7lwPPKkTa0W%2FprKO56XPgGYVIO%2FpCZx3NeXYh8o4%2BwFlHM00uRNvRBzjraGbJhWg7%2BgBnHc08uRBtRx%2FgwKM56czXfC8o4TTY0Z%2BoO%2FBo3gbP180LnU%2FRgUdzEDxfNy90PkUHHskP4FHgfH15ofMpOvBIXgfP15cXOp%2BiA4%2FiM%2FAwcL7evIz51Bx4BJ%2BAJ4Hz3ZmXNZ%2BSAy%2B9J78BHgTNd29e5nwqDnzo6xR4B7zY9gHZmW9Q3hjzGWNMrWzh1Ed11og5f0WnPpqzRtD5Kzr1UZw1os5f0amnO2uEnb%2BiU0911og7%2F4xCjpWdNeLOP6OQC2VnjbjzzyjkWtlZI%2B78FZ16tLM%2BC54vGnmnHu2sF8HzRSPv1A%2BSC1mihbRTj3bWfYVIO%2F%2BMQpScdV8h0s4%2FqxQFZ73um7%2B0888qZZfOepPdmLTzT2EHznro9lja%2BadR6KzTf6SJuPOXYoxCzABciBgu5D8vhH%2FJgSuyg0K6%2BOx3sUIafPa7WCENPvtdrJAGn%2F1OOYvgW2D1Z7%2BrFTKb1IxgIfNJzST8rnwl7cDVSXD0V5F51ZHg6JeRedWR4OgPI%2FOqI8HR70XmVUmko8%2FIq5IoR5%2BVVyURjj4zr1oocPRj5BljjDHGGGOMMcYYY8xElT9jEHRBpJyhuQAAAABJRU5ErkJggg%3D%3D&labelColor=6565d8&color=6A6A6A">
     </a>
     <a href="https://github.com/uptrain-ai/uptrain/issues/new?assignees=&labels=enhancement&template=feature_request.md&title=">
-        <img alt="Request New Feature" src="https://img.shields.io/badge/Request%20New%20Feature-uptrain?logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAAGQAAABkCAYAAABw4pVUAAAACXBIWXMAAAsTAAALEwEAmpwYAAAG%2BElEQVR4nO2da6gWRRjHN1NLKy1Tu2B5CjEsMiO0wEiqoxhmZQUJ5YfyQ5FhdLEiIiItLQtRIswiMIvKNDOTCosyCzsVGWiXLykVdrESQz1aXn7xcObAsmdmdvc9715md37wftAzszuz%2F3eemX3mmecNAo%2FH4%2FF4PKUF6AmMBxYDG4E1wLii21VXEZYAf9KV%2F4BLim5n3UWIsqboNlcO0osQ5sui218J6J4IYRYX3RdnAY4ELgYWAr%2FRHFqL7pdTkI0IncjI6ll0H%2BsuQpjn8ujIWGAacA9wf0GfmcCwBuaEVnlI3ZwTOtkNvAq8YCkzPishzlQ3%2FoviaAdWADcAxxQswrVAH3UP%2BXc%2B5kp16EngX%2BotwmvAdZ0ihO7VR%2F1dx5Jmi3EC8AHFsAd4ADi%2BbCJE7isjJXtzBfQCPqIYfgHOSTif5S5CpA35mCu1%2BiiCfcDIHEXYk1aE3M0VMAI4GNORA8BmYFuCTsuy8mtgf4KyszXt6VGECMD54hgE%2Bhr%2BLvVzMVfSWBubwktOYAKw0yDaLaFyA4G1luseAk6KtGU48B05jgRgMPBpqK58CS5N8ZyaZ67UMNxr6dgB3fpfHrym7HxNuX7A74Zrf6MpL%2BLnZo7kCwF8a3jIfYswV5NiOrnZUE%2B%2B%2FVG0mzPA64Zrr46UG0K%2Bc4KIscVy7XFFmKs7Yzq8zVDvDE3ZSYayaw3XXh8pd6IyY0mR0TsbGNRAv%2BPEEM7L1VypGz2RoOMTNPXmasq9pSk3XL3s6djZwHymQxYPS4HRTRTjk4Tmqrm%2BK%2BCZBB3eqeaMgWpkzLWsypYBZwP9gasSrMouirTnWLVH3ainoE353Y6yTOBxYsjfB%2BdurlIIkiXvWL7F4lT8qcHr%2FgHMA4ZGxJClu43vgVMSzoGZ%2BK6KFkS4LcaDIH6tDTTGAeUbm5xwZESX4X1zM1clEuQgMD1BW0cBz1vmpO7QRYwE5qq1qoJ08n6SuCZgADAL2EqGYuS6uiqpIJ38oJbjVvd7yMUiAWqHaYwuc0ZCc5VNIENJBenkH%2BXPGpGgH8PUJK5z6aQWQ13zekvdy5suRowg69W3rwyfy0wOP01%2FjgNmJPSHTY65lslc7cgskMEiyPLAYYAjlJirLOZshaV%2BvqurqgsSRoliWt0NLY25qpEgrZaHO8dQJ7%2BXwboJIlje0GU%2BODooenVVQ0FmWEbJtFKYK9cFoSPyZApwl0QlJlh9yTJaR1vhqyvXBaHDrHweafOimDqLLN%2F8MYWuriogyEOGdo%2B11DnLsgRemtZ3JRExWXTMVUHeNrT77ph64i8zbXINSmOu5IU1i465KshCQ7uviaknbngTc9Qefay5Uhtp87PomKuCnK7xW22Mm3SVQ3KrZe8kqbmaKs8ui445KYgAnKZGymrgwRShP%2FeSDp25WlkbQejYar1dPeRRGVx%2FQEwsWhJz1V4LQejYFZT98LC%2F6dYM7mM7dJPEXFEXQT7UtGVvUvd7SuEbNVcr6iTILkN7Rmdwrw3dMFe1EaTNkK5icAb3kmiWtOYqXMddQYALgPtkPpAgOku5KzXLT62LvAltkhCj7Q2aK3cFoeOo2qHIiakWS%2FkLVbiPnFaa2qx2GO71cIPmyk1BZEcOfdjpsqAEACdbwlZt5spZQaYYrr8lKAkqlrhL%2B6LOw4i5claQkYbrd4mULwqJ%2F1LmsdOsfhU9pKSOSrQ7L4hhf7pdzvMFJUO9wZuC5h7RPCNnBemltlDfBJ6VMyOBQ6gV4r7KCOI6lj2S8gmiDnVKYpjHgKslQC2oGMByJwRRXtkfI%2FVerJooOCSI6XyiNQLENVwS5F1D3TuCCoFDgixIemrXZVwSZIjyS4WR%2FQw%2FhxS4yhJf0KPAS2KqgN5BxcCVEVIX8IKUCy9IyfCClIzSC6I2nU4NagJlFUQlnvkissRtevBB2SizIJ9pyq0MKg5lFEQ5Ek1h%2FJV793BBkH6GbG9y2qhHUGEooyCq7Bu5NKpklFmQ%2FipIeZdK0r8gbeJJFymtIKE6lXIelk2Qp9IKUjcw7%2FvMy%2BJmEubpBbEfgfvV8IxmBs0GuMIL0lDkpTAxaDZqotbFHNXeZAEtlt%2Br2h3NkdJMUXS%2FiVFbQYDewI2Ro3VRXsmyAedqItS1gqjELBI49rJpyKqFwjpHP22WnCjhA0TZRl8CT8cJYlgA3KwpV9Qv9eRF8xMGGIap5Fk0uU56G%2FLlbq%2BZIOty%2B%2BFIlcLoY3XjVZpD%2BjoOaxKA6bzCVeA923G8LHNQPS4nVDVJJXXn8TZprvEz1WK%2FyoPS%2FOw%2FaXKJaP5vYiQ5y9%2BaXzdo6UZS47KxQ%2BUN1ibKLFPSFzlJO92QK32MSmjs6mcWcJM6eFrciPB4PB6Px%2BPxeDwej8fj8XiCYvgfmdGLzXmrOA4AAAAASUVORK5CYII%3D&labelColor=3E93C4&color=6A6A6A">
+        <img alt="Request New Feature" src="https://img.shields.io/badge/Request%20New%20Feature-uptrain?logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAAGQAAABkCAYAAABw4pVUAAAACXBIWXMAAAsTAAALEwEAmpwYAAAG%2BElEQVR4nO2da6gWRRjHN1NLKy1Tu2B5CjEsMiO0wEiqoxhmZQUJ5YfyQ5FhdLEiIiItLQtRIswiMIvKNDOTCosyCzsVGWiXLykVdrESQz1aXn7xcObAsmdmdvc9715md37wftAzszuz%2F3eemX3mmecNAo%2FH4%2FF4PKUF6AmMBxYDG4E1wLii21VXEZYAf9KV%2F4BLim5n3UWIsqboNlcO0osQ5sui218J6J4IYRYX3RdnAY4ELgYWAr%2FRHFqL7pdTkI0IncjI6ll0H%2BsuQpjn8ujIWGAacA9wf0GfmcCwBuaEVnlI3ZwTOtkNvAq8YCkzPishzlQ3%2FoviaAdWADcAxxQswrVAH3UP%2BXc%2B5kp16EngX%2BotwmvAdZ0ihO7VR%2F1dx5Jmi3EC8AHFsAd4ADi%2BbCJE7isjJXtzBfQCPqIYfgHOSTif5S5CpA35mCu1%2BiiCfcDIHEXYk1aE3M0VMAI4GNORA8BmYFuCTsuy8mtgf4KyszXt6VGECMD54hgE%2Bhr%2BLvVzMVfSWBubwktOYAKw0yDaLaFyA4G1luseAk6KtGU48B05jgRgMPBpqK58CS5N8ZyaZ67UMNxr6dgB3fpfHrym7HxNuX7A74Zrf6MpL%2BLnZo7kCwF8a3jIfYswV5NiOrnZUE%2B%2B%2FVG0mzPA64Zrr46UG0K%2Bc4KIscVy7XFFmKs7Yzq8zVDvDE3ZSYayaw3XXh8pd6IyY0mR0TsbGNRAv%2BPEEM7L1VypGz2RoOMTNPXmasq9pSk3XL3s6djZwHymQxYPS4HRTRTjk4Tmqrm%2BK%2BCZBB3eqeaMgWpkzLWsypYBZwP9gasSrMouirTnWLVH3ainoE353Y6yTOBxYsjfB%2BdurlIIkiXvWL7F4lT8qcHr%2FgHMA4ZGxJClu43vgVMSzoGZ%2BK6KFkS4LcaDIH6tDTTGAeUbm5xwZESX4X1zM1clEuQgMD1BW0cBz1vmpO7QRYwE5qq1qoJ08n6SuCZgADAL2EqGYuS6uiqpIJ38oJbjVvd7yMUiAWqHaYwuc0ZCc5VNIENJBenkH%2BXPGpGgH8PUJK5z6aQWQ13zekvdy5suRowg69W3rwyfy0wOP01%2FjgNmJPSHTY65lslc7cgskMEiyPLAYYAjlJirLOZshaV%2BvqurqgsSRoliWt0NLY25qpEgrZaHO8dQJ7%2BXwboJIlje0GU%2BODooenVVQ0FmWEbJtFKYK9cFoSPyZApwl0QlJlh9yTJaR1vhqyvXBaHDrHweafOimDqLLN%2F8MYWuriogyEOGdo%2B11DnLsgRemtZ3JRExWXTMVUHeNrT77ph64i8zbXINSmOu5IU1i465KshCQ7uviaknbngTc9Qefay5Uhtp87PomKuCnK7xW22Mm3SVQ3KrZe8kqbmaKs8ui445KYgAnKZGymrgwRShP%2FeSDp25WlkbQejYar1dPeRRGVx%2FQEwsWhJz1V4LQejYFZT98LC%2F6dYM7mM7dJPEXFEXQT7UtGVvUvd7SuEbNVcr6iTILkN7Rmdwrw3dMFe1EaTNkK5icAb3kmiWtOYqXMddQYALgPtkPpAgOku5KzXLT62LvAltkhCj7Q2aK3cFoeOo2qHIiakWS%2FkLVbiPnFaa2qx2GO71cIPmyk1BZEcOfdjpsqAEACdbwlZt5spZQaYYrr8lKAkqlrhL%2B6LOw4i5claQkYbrd4mULwqJ%2F1LmsdOsfhU9pKSOSrQ7L4hhf7pdzvMFJUO9wZuC5h7RPCNnBemltlDfBJ6VMyOBQ6gV4r7KCOI6lj2S8gmiDnVKYpjHgKslQC2oGMByJwRRXtkfI%2FVerJooOCSI6XyiNQLENVwS5F1D3TuCCoFDgixIemrXZVwSZIjyS4WR%2FQw%2FhxS4yhJf0KPAS2KqgN5BxcCVEVIX8IKUCy9IyfCClIzSC6I2nU4NagJlFUQlnvkissRtevBB2SizIJ9pyq0MKg5lFEQ5Ek1h%2FJV793BBkH6GbG9y2qhHUGEooyCq7Bu5NKpklFmQ%2FipIeZdK0r8gbeJJFymtIKE6lXIelk2Qp9IKUjcw7%2FvMy%2BJmEubpBbEfgfvV8IxmBs0GuMIL0lDkpTAxaDZqotbFHNXeZAEtlt%2Br2h3NkdJMUXS%2FiVFbQYDewI2Ro3VRXsmyAedqItS1gqjELBI49rJpyKqFwjpHP22WnCjhA0TZRl8CT8cJYlgA3KwpV9Qv9eRF8xMGGIap5Fk0uU56G%2FLlbq%2BZIOty%2B%2BFIlcLoY3XjVZpD%2BjoOaxKA6bzCVeA923G8LHNQPS4nVDVJJXXn8TZprvEz1WK%2FyoPS%2FOw%2FaXKJaP5vYiQ5y9%2BaXzdo6UZS47KxQ%2BUN1ibKLFPSFzlJO92QK32MSmjs6mcWcJM6eFrciPB4PB6Px%2BPxeDwej8fj8XiCYvgfmdGLzXmrOA4AAAAASUVORK5CYII%3D&labelColor=5B92E9&color=6A6A6A">
+    </a>
+    <a href="https://demo.uptrain.ai/benchmark">
+      <img alt="Daily Monitoring" src="https://img.shields.io/badge/Daily%20Monitoring-uptrain?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAGQAAABkCAYAAABw4pVUAAAACXBIWXMAAAsTAAALEwEAmpwYAAAFUUlEQVR4nO2daahVVRTHt2WDls3RQDYXRUZBkRkRjdAraPjSAJUUKVSE0QuiQZ4FmRj2lMwwqGgitZTq5cvEIipKpGgymogwCrKs7IOkDf5i9ZYorzvsM+99zvrB/XjWXfv+z9ln7zXs65xhGIZhGIZhGIZRCsD2wOXAIuA94P2MH7HxLHBBOSOoEcBewJsUx/PATlWPMxqAQYpnXtXjjALgDMrhb+CwqscbPMAMymNy1eMNHuDxEgXpq3q8wQP0lSjIPVWPN3iAY4HNJkhAAHNMkIAAdgBml/Ck2JSVBOAo4HbgYWD+sM9KEyQQZP8ArDVBAgDYDfjUpqwAAEYCy+0dEgjAPHupBwJwq62yAgHo0WCgLXurBjgOWG/7kAAA9gfW2MYwAIDRwKoUYkiq9pdG7NQZSq3eD3wCrANWAwuBOyRXDRyU0/dsB7yQQoxvgf2AH2svCHCO50BFqBXALGAicCKwY8Lvmp5CjN+BcXp9fQXRu3VqxlXOn8DHwFNAL3AusG+b7xMRkyK+9Wxj42vP625zMQHsAyyjOH4AXtW07RXAZcCmFHZuHub3y57XxVMSBEwAviN85rbw/SKP62T1NtLFADBFp5nQWdbuRwWe6HDdRqlucZFEUqWILAZWi79d3n13tdhUfgSMd6EDnAB8RRys9a2pAnbRWq+Lt6zCgge4BthAHPwBnObqCLCzpkNjYTNwlasjwNG6N8jCr/opi2mujuh8+lvGH2cVcKjaO1A3e1N08/dZAeFyaUsY4eqEhDC0vCbrtDFLSnU8XqbjpX5Wq0be0fBGGt6V6dXVCWCsRkKzsB64NIMPI4DDxYZMP8AS4Jsu9VeDnZa3UQKcD/ycUYwPgSML3P+cDtykT5NMT/3Aea5O6B0phWb/ZBRD3gujqx5P1Ghg8LUc1vzXVz2W6AGO0GRNFr4AjneRA+ypwcZrgbOS5mby6l6VeE0WJAs4xsVfVDddA4nb8n2WhUkaRy7JIMSm4bmFWAGe6TBOWdVdGXpvxZoooqAeABd6jFciDHu4ogEeTSGGrPX3djWBoWWzDxNDK7mU8MbdkjtwNQL/GN2MMpw5RJer3ZDKjLNdDQG+9BRkdlkO3dLFkbckIOhqCqEJok5NalHBt0HTmnEk9+skiDq2q1YUTtaA3u6uARCqIE0FEyQsTJDAaIwgDFWWS/X7B5pYegO4ofSAXRcaIYiWlq5rM7CVIe30ay+I5lZ+6jK4V1wgNEEQ3yOTTnEB0ARB3vYc4J0uAJogyOcxDZAGCCLpXB/muAAwQbZigtTpCWGobUCqIhcAD0pRQko7NmVlEUSDoFLF2IqBpEFREyS7IC/SmUETpKQpCzjT03ZP9FOWtglcJ/sDzYmMDVCQfk/b86MVRBse723R8y2dtQ8kzRgWLMgiT9uDMQvSn9fdVoIgSzxtL49SEKnH9ax2PzWBTRMkLcB9ed/NJkgGgOc8BVmawKY9IWkBFnsKsiKBTRMkLSaIC+6lbk8IJsgWbNlrT8j/sSdkK/aEtLg7JJeQdyhCTiH1YWaB/g4U4G8p/SEzPZ15JIFN3zMMbyzwb/IeSmDzpWD+Nk9CIp7OeJ+SAFztYe8v4IAU/p7s6a/3kXzS0Olhb2O7k1FzR09e6MRAkpN1tNX69S42p2bw97EuthekiHZ3OzSh15UFMAp4uo0ji9P0oOup1kvb9ClOy9KnKH8ULFNom0No5DDLUSlsjtF++1ZPRnliDHPqJA02PqlF0hNymhL75HhWPRT54Hy8/c/2MXps+Vzt9BqXU/S7V3+HSaVNU4ZhGIZhGIZhGIZhGIbhquVfiiAaCf/Kq/8AAAAASUVORK5CYII=&labelColor=35B9D2&color=6A6A6A">
     </a>
 </p>
 
 <p align="center">
   <a href="https://github.com/uptrain-ai/uptrain/releases">
     <img alt="GitHub Release" src="https://img.shields.io/github/v/release/uptrain-ai/uptrain?labelColor=6A6A6A&color=CC766E">
   </a>
@@ -73,18 +79,14 @@
 </p>
 
 <h4 align="center">
   <video src="https://github.com/uptrain-ai/uptrain/assets/43818888/68a3b169-2217-446b-93b2-96b48ec7201d" alt="Demo of UpTrain's LLM evaluations with scores for hallucinations, retrieved-context quality, response tonality for a customer support chatbot" autoplay>
 </h4>
 
 
-
-
-
-
 **[UpTrain](https://uptrain.ai)** is an open-source unified platform to evaluate and improve Generative AI applications. We provide grades for [20+ preconfigured evaluations](https://github.com/uptrain-ai/uptrain?tab=readme-ov-file#pre-built-evaluations-we-offer-) (covering language, code, embedding use cases), perform [root cause analysis](https://github.com/uptrain-ai/uptrain/blob/main/examples/root_cause_analysis/rag_with_citation.ipynb) on failure cases and give insights on how to resolve them.    
 
 <br />
 
 # Key Features 🔑
 
 <img width="1088" alt="Interactive Dashboards" src="https://github.com/uptrain-ai/uptrain/assets/36454110/eb1c8239-dd99-4e66-ba8a-cbaee2beec10">
@@ -249,14 +251,16 @@
 |[Jailbreak Detection](https://docs.uptrain.ai/predefined-evaluations/safeguarding/jailbreak) | Grades whether the user's prompt is an attempt to jailbreak (i.e. generate illegal or harmful responses). |
 
 <img width="1088" alt="evaluate the clarity of user queries" src="https://github.com/uptrain-ai/uptrain/assets/36454110/50ed622f-0b92-468c-af48-2391ff6ab8e0">
 
 | Eval | Description |
 | ---- | ----------- |
 |[Sub-Query Completeness](https://docs.uptrain.ai/predefined-evaluations/query-quality/sub-query-completeness) | Evaluate whether all of the sub-questions generated from a user's query, taken together, cover all aspects of the user's query or not |
+| [Multi-Query Accuracy](https://docs.uptrain.ai/predefined-evaluations/query-quality/multi-query-accuracy) | Evaluate whether the variants generated accurately represent the original query |
+
 
 <br />
 
 # Integrations 🤝
 
 | Eval Frameworks  | LLM Providers | LLM Packages | Serving frameworks | LLM Observability | Vector DBs |
 | ------------- | ------------- | ------------- | ------------- | ------------- |  ------------- |
@@ -266,14 +270,23 @@
 | | [Mistral](https://docs.uptrain.ai/llms/mistral) | | Replicate  |
 | |  | |  HuggingFace  |
 
 More integrations are coming soon. If you have a specific integration in mind, please let us know by [creating an issue](https://github.com/uptrain-ai/uptrain/issues).
 
 <br />
 
+# Monitoring Prompt Drift in LLMs: Benchmark by UpTrain
+
+Most popular LLMs like GPT-4, GPT-3.5-turbo, Claude-2.1 etc., are closed-source, i.e. exposed via an API with very little visibility on what happens under the hood. There are many reported instances of prompt drift (or GPT-4 becoming lazy) and research work exploring the degradation in model quality. This benchmark is an attempt to track the change in model behaviour by evaluating its response on a fixed dataset.
+
+<img width="1316" alt="image" src="https://github.com/uptrain-ai/uptrain/assets/43818888/65b7e8c3-3f5e-48bb-98c1-88208520945b">
+
+You can find the benchmark [here](https://demo.uptrain.ai/benchmark).
+
+
 # Resources 💡
 
 1. [How to evaluate your LLM application](https://blog.uptrain.ai/how-to-evaluate-your-llm-applications)
 1. [How to detect jailbreaks](https://blog.uptrain.ai/llm-jailbreak/)
 1. [Dealing with hallucinations](https://blog.uptrain.ai/dealing-with-hallucinations-in-llms-a-deep-dive/)
 
 <br />
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: uptrain Version: 0.6.9 Summary: UpTrain - tool to
+Metadata-Version: 2.1 Name: uptrain Version: 0.7.0 Summary: UpTrain - tool to
 evaluate LLM applications on aspects like factual accuracy, response quality,
 retrieval quality, tonality, etc. Maintainer-email: UpTrain AI Team
 uptrain.ai> License: Apache-2.0 Project-URL: Homepage, https://uptrain.ai
 Project-URL: Repository, https://github.com/uptrain-ai/uptrain Keywords:
 uptrain,ai,LLM,evaluation,hallucinations,observability,response quality
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Topic :: Software Development :: Build Tools
@@ -11,19 +11,20 @@
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: pydantic
 Requires-Dist: pydantic-settings Requires-Dist: loguru Requires-Dist:
 lazy_loader Requires-Dist: networkx Requires-Dist: polars>=0.18 Requires-Dist:
 pandas Requires-Dist: numpy>=1.23.0 Requires-Dist: httpx>=0.24.1 Requires-Dist:
 plotly>=5.0.0 Requires-Dist: aiolimiter>=1.1 Requires-Dist: openai>=1.6.1
 Requires-Dist: fsspec Requires-Dist: litellm Requires-Dist: pyyaml Requires-
-Dist: json5 Provides-Extra: test Requires-Dist: pytest>=7.0; extra == "test"
+Dist: json5 Requires-Dist: python-docx Requires-Dist: pymupdf Requires-Dist:
+faiss-cpu Provides-Extra: test Requires-Dist: pytest>=7.0; extra == "test"
   ****** _[[_LL_oo_gg_oo_ _oo_ff_ _UU_pp_TT_rr_aa_ii_nn_ _--_ _aa_nn_ _oo_pp_ee_nn_--_ss_oo_uu_rr_cc_ee_ _pp_ll_aa_tt_ff_oo_rr_mm_ _tt_oo_ _ee_vv_aa_ll_uu_aa_tt_ee_ _aa_nn_dd_ _ii_mm_pp_rr_oo_vv_ee_ _LL_LL_MM
                                _aa_pp_pp_ll_ii_cc_aa_tt_ii_oo_nn_ss_]] ******
                         _[_T_r_y_ _o_u_t_ _E_v_a_l_u_a_t_i_o_n_]_[_R_e_a_d_ _D_o_c_s_]
-_[_S_l_a_c_k_ _C_o_m_m_u_n_i_t_y_]_[_R_e_q_u_e_s_t_ _N_e_w_ _F_e_a_t_u_r_e_]
+_[_S_l_a_c_k_ _C_o_m_m_u_n_i_t_y_]_[_R_e_q_u_e_s_t_ _N_e_w_ _F_e_a_t_u_r_e_]_[_D_a_i_l_y_ _M_o_n_i_t_o_r_i_n_g_]
   _[_G_i_t_H_u_b_ _R_e_l_e_a_s_e_]_[_G_i_t_H_u_b_ _c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]_[_G_i_t_H_u_b_ _L_i_c_e_n_s_e_]_[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]
 **[UpTrain](https://uptrain.ai)** is an open-source unified platform to
 evaluate and improve Generative AI applications. We provide grades for [20+
 preconfigured evaluations](https://github.com/uptrain-ai/uptrain?tab=readme-ov-
 file#pre-built-evaluations-we-offer-) (covering language, code, embedding use
 cases), perform [root cause analysis](https://github.com/uptrain-ai/uptrain/
 blob/main/examples/root_cause_analysis/rag_with_citation.ipynb) on failure
@@ -152,15 +153,18 @@
 LLM reveal its system prompts. | |[Jailbreak Detection](https://
 docs.uptrain.ai/predefined-evaluations/safeguarding/jailbreak) | Grades whether
 the user's prompt is an attempt to jailbreak (i.e. generate illegal or harmful
 responses). | [evaluate the clarity of user queries]| Eval | Description | | --
 -- | ----------- | |[Sub-Query Completeness](https://docs.uptrain.ai/
 predefined-evaluations/query-quality/sub-query-completeness) | Evaluate whether
 all of the sub-questions generated from a user's query, taken together, cover
-all aspects of the user's query or not |
+all aspects of the user's query or not | | [Multi-Query Accuracy](https://
+docs.uptrain.ai/predefined-evaluations/query-quality/multi-query-accuracy) |
+Evaluate whether the variants generated accurately represent the original query
+|
 # Integrations ð¤ | Eval Frameworks | LLM Providers | LLM Packages | Serving
 frameworks | LLM Observability | Vector DBs | | ------------- | ------------- |
 ------------- | ------------- | ------------- | ------------- | | [OpenAI
 Evals](https://docs.uptrain.ai/tutorials/openai-evals) | [OpenAI](https://
 docs.uptrain.ai/llms/openai) | [LlamaIndex](https://docs.uptrain.ai/
 integrations/framework/llamaindex-methods/overview) | [Ollama](https://
 docs.uptrain.ai/llms/ollama) | [Langfuse](https://docs.uptrain.ai/integrations/
@@ -172,15 +176,22 @@
 docs.uptrain.ai/llms/claude) | | [Anyscale](https://docs.uptrain.ai/llms/
 anyscale) | [Zeno](https://docs.uptrain.ai/integrations/observation-tools/zeno)
 | [Chroma](https://docs.uptrain.ai/integrations/vector_db/chroma) | | |
 [Mistral](https://docs.uptrain.ai/llms/mistral) | | Replicate | | | | |
 HuggingFace | More integrations are coming soon. If you have a specific
 integration in mind, please let us know by [creating an issue](https://
 github.com/uptrain-ai/uptrain/issues).
-# Resources ð¡ 1. [How to evaluate your LLM application](https://
+# Monitoring Prompt Drift in LLMs: Benchmark by UpTrain Most popular LLMs like
+GPT-4, GPT-3.5-turbo, Claude-2.1 etc., are closed-source, i.e. exposed via an
+API with very little visibility on what happens under the hood. There are many
+reported instances of prompt drift (or GPT-4 becoming lazy) and research work
+exploring the degradation in model quality. This benchmark is an attempt to
+track the change in model behaviour by evaluating its response on a fixed
+dataset. [image]You can find the benchmark [here](https://demo.uptrain.ai/
+benchmark). # Resources ð¡ 1. [How to evaluate your LLM application](https://
 blog.uptrain.ai/how-to-evaluate-your-llm-applications) 1. [How to detect
 jailbreaks](https://blog.uptrain.ai/llm-jailbreak/) 1. [Dealing with
 hallucinations](https://blog.uptrain.ai/dealing-with-hallucinations-in-llms-a-
 deep-dive/)
 # Why we are building UpTrain ð¤ Having worked with ML and NLP models for the
 last 8 years, we were continuosly frustated with numerous hidden failures in
 our models which led to us building UpTrain. UpTrain was initially started as
```

### Comparing `uptrain-0.6.9/uptrain.egg-info/SOURCES.txt` & `uptrain-0.7.0/uptrain.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 uptrain/framework/builtins.py
 uptrain/framework/checks.py
 uptrain/framework/evalllm.py
 uptrain/framework/evals.py
 uptrain/framework/rca_templates.py
 uptrain/framework/remote.py
 uptrain/framework/signal.py
+uptrain/framework/eval_assistant/__init__.py
+uptrain/framework/eval_assistant/assistant_evals_prompts.py
+uptrain/framework/eval_assistant/assistant_evals_utils.py
+uptrain/framework/eval_assistant/parse_files_utils.py
 uptrain/integrations/__init__.py
 uptrain/integrations/__init__.pyi
 uptrain/integrations/llama_index.py
 uptrain/integrations/promptfoo.py
 uptrain/integrations/promptfoo_utils.py
 uptrain/operators/__init__.py
 uptrain/operators/__init__.pyi
@@ -52,23 +56,25 @@
 uptrain/operators/io/duck.py
 uptrain/operators/io/excel.py
 uptrain/operators/io/mongodb.py
 uptrain/operators/language/__init__.py
 uptrain/operators/language/bleu.py
 uptrain/operators/language/context_quality.py
 uptrain/operators/language/conversation.py
+uptrain/operators/language/custom.py
 uptrain/operators/language/factual_accuracy.py
 uptrain/operators/language/generation.py
 uptrain/operators/language/grammar.py
 uptrain/operators/language/guideline.py
 uptrain/operators/language/jailbreak.py
 uptrain/operators/language/language_quality.py
 uptrain/operators/language/llm.py
 uptrain/operators/language/meteor.py
 uptrain/operators/language/model_grade.py
+uptrain/operators/language/multiquery.py
 uptrain/operators/language/openai_evals.py
 uptrain/operators/language/question_quality.py
 uptrain/operators/language/response_quality.py
 uptrain/operators/language/rouge.py
 uptrain/operators/language/subquery.py
 uptrain/operators/language/text.py
 uptrain/operators/language/tone.py
```


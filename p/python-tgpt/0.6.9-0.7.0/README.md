# Comparing `tmp/python_tgpt-0.6.9.tar.gz` & `tmp/python_tgpt-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_tgpt-0.6.9.tar", last modified: Tue Apr 30 21:48:52 2024, max compression
+gzip compressed data, was "python_tgpt-0.7.0.tar", last modified: Thu May  2 23:23:40 2024, max compression
```

## Comparing `python_tgpt-0.6.9.tar` & `python_tgpt-0.7.0.tar`

### file list

```diff
@@ -1,97 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.986392 python_tgpt-0.6.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21925 2024-04-30 21:48:52.986392 python_tgpt-0.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18985 2024-04-30 21:48:52.000000 python_tgpt-0.6.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 21:48:52.986392 python_tgpt-0.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.970392 python_tgpt-0.6.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.970392 python_tgpt-0.6.9/src/pytgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.974392 python_tgpt-0.6.9/src/pytgpt/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/api/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17394 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/api/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.974392 python_tgpt-0.6.9/src/pytgpt/auto/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/auto/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7999 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/auto/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.974392 python_tgpt-0.6.9/src/pytgpt/blackboxai/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/blackboxai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/blackboxai/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    85252 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.974392 python_tgpt-0.6.9/src/pytgpt/gemini/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/gemini/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.974392 python_tgpt-0.6.9/src/pytgpt/gpt4all/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/gpt4all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/gpt4all/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.974392 python_tgpt-0.6.9/src/pytgpt/gpt4free/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/gpt4free/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/gpt4free/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/gpt4free/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.974392 python_tgpt-0.6.9/src/pytgpt/groq/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/groq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/groq/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.974392 python_tgpt-0.6.9/src/pytgpt/imager/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/imager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/imager/imager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.974392 python_tgpt-0.6.9/src/pytgpt/koboldai/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/koboldai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/koboldai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.978392 python_tgpt-0.6.9/src/pytgpt/leo/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/leo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/leo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.978392 python_tgpt-0.6.9/src/pytgpt/llama2/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/llama2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/llama2/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.978392 python_tgpt-0.6.9/src/pytgpt/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/openai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.978392 python_tgpt-0.6.9/src/pytgpt/opengpt/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/opengpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/opengpt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.978392 python_tgpt-0.6.9/src/pytgpt/perplexity/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/perplexity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/perplexity/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.978392 python_tgpt-0.6.9/src/pytgpt/phind/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/phind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/phind/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.978392 python_tgpt-0.6.9/src/pytgpt/poe/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/poe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/poe/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    34123 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.978392 python_tgpt-0.6.9/src/pytgpt/webchatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/webchatgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/webchatgpt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.978392 python_tgpt-0.6.9/src/pytgpt/yepchat/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/yepchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/src/pytgpt/yepchat/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.982392 python_tgpt-0.6.9/src/python_tgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21925 2024-04-30 21:48:52.000000 python_tgpt-0.6.9/src/python_tgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-30 21:48:52.000000 python_tgpt-0.6.9/src/python_tgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 21:48:52.000000 python_tgpt-0.6.9/src/python_tgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-30 21:48:52.000000 python_tgpt-0.6.9/src/python_tgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-30 21:48:52.000000 python_tgpt-0.6.9/src/python_tgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 21:48:52.000000 python_tgpt-0.6.9/src/python_tgpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:48:52.982392 python_tgpt-0.6.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/tests/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/tests/test_blackboxai.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/tests/test_gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/tests/test_gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/tests/test_gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/tests/test_groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/tests/test_imager.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/tests/test_koboldai.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/tests/test_leo.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/tests/test_llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/tests/test_opengpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/tests/test_perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/tests/test_phind.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/tests/test_poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-30 21:48:23.000000 python_tgpt-0.6.9/tests/test_webchatgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.090761 python_tgpt-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23449 2024-05-02 23:23:40.090761 python_tgpt-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-05-02 23:23:39.000000 python_tgpt-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 23:23:40.090761 python_tgpt-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.074760 python_tgpt-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.078760 python_tgpt-0.7.0/src/pytgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.078760 python_tgpt-0.7.0/src/pytgpt/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/api/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17339 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/api/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/async_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.078760 python_tgpt-0.7.0/src/pytgpt/auto/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/auto/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16877 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/auto/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.078760 python_tgpt-0.7.0/src/pytgpt/blackboxai/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/blackboxai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16048 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/blackboxai/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85577 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.078760 python_tgpt-0.7.0/src/pytgpt/gemini/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/gemini/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.078760 python_tgpt-0.7.0/src/pytgpt/gpt4all/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/gpt4all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/gpt4all/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.078760 python_tgpt-0.7.0/src/pytgpt/gpt4free/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/gpt4free/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/gpt4free/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/gpt4free/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.078760 python_tgpt-0.7.0/src/pytgpt/groq/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/groq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20358 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/groq/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.078760 python_tgpt-0.7.0/src/pytgpt/imager/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/imager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/imager/imager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.078760 python_tgpt-0.7.0/src/pytgpt/koboldai/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/koboldai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/koboldai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.082760 python_tgpt-0.7.0/src/pytgpt/leo/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/leo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18641 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/leo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.082760 python_tgpt-0.7.0/src/pytgpt/llama2/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/llama2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16850 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/llama2/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.082760 python_tgpt-0.7.0/src/pytgpt/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19455 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/openai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.082760 python_tgpt-0.7.0/src/pytgpt/opengpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/opengpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/opengpt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.082760 python_tgpt-0.7.0/src/pytgpt/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/perplexity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/perplexity/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.082760 python_tgpt-0.7.0/src/pytgpt/phind/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/phind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19038 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/phind/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.082760 python_tgpt-0.7.0/src/pytgpt/poe/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/poe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/poe/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36065 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.082760 python_tgpt-0.7.0/src/pytgpt/webchatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/webchatgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/webchatgpt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.082760 python_tgpt-0.7.0/src/pytgpt/yepchat/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/yepchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19001 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/yepchat/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.086760 python_tgpt-0.7.0/src/python_tgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23449 2024-05-02 23:23:40.000000 python_tgpt-0.7.0/src/python_tgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-02 23:23:40.000000 python_tgpt-0.7.0/src/python_tgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 23:23:40.000000 python_tgpt-0.7.0/src/python_tgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 23:23:40.000000 python_tgpt-0.7.0/src/python_tgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-02 23:23:40.000000 python_tgpt-0.7.0/src/python_tgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 23:23:40.000000 python_tgpt-0.7.0/src/python_tgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.086760 python_tgpt-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_auto_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_blackboxai_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_gpt4free_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_imager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_koboldai_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_leo_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_llama2_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_opengpt_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_phind_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_webchatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_yepchat_tgpt.py
```

### Comparing `python_tgpt-0.6.9/LICENSE` & `python_tgpt-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.9/PKG-INFO` & `python_tgpt-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tgpt
-Version: 0.6.9
+Version: 0.7.0
 Summary: Interact with AI without API key
 Home-page: https://github.com/Simatwa/python-tgpt
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
@@ -34,37 +34,38 @@
 Requires-Dist: requests[socks]==2.31.0
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: webchatgpt==0.3.0
 Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: poe-api-wrapper==1.3.6
 Requires-Dist: brotli==1.1.0
-Requires-Dist: g4f>=0.2.6.1
+Requires-Dist: g4f>=0.3.0.8
 Requires-Dist: Helpingai_T2-fork==0.3.2
 Requires-Dist: python-vlc>=3.0.20
+Requires-Dist: httpx==0.27.0
 Provides-Extra: cli
 Requires-Dist: click==8.1.3; extra == "cli"
 Requires-Dist: rich==13.3.4; extra == "cli"
 Requires-Dist: clipman==3.1.0; extra == "cli"
 Requires-Dist: pyperclip==1.8.2; extra == "cli"
 Requires-Dist: colorama==0.4.6; extra == "cli"
-Requires-Dist: g4f>=0.2.6.1; extra == "cli"
+Requires-Dist: g4f>=0.3.0.8; extra == "cli"
 Requires-Dist: python-dotenv==1.0.0; extra == "cli"
 Provides-Extra: api
 Requires-Dist: fastapi[all]==0.110.1; extra == "api"
 Provides-Extra: all
 Requires-Dist: g4f[all]>=0.2.6.1; extra == "all"
 Requires-Dist: matplotlib; extra == "all"
 Requires-Dist: gpt4all==2.2.0; extra == "all"
 Requires-Dist: click==8.1.3; extra == "all"
 Requires-Dist: rich==13.3.4; extra == "all"
 Requires-Dist: clipman==3.1.0; extra == "all"
 Requires-Dist: pyperclip==1.8.2; extra == "all"
 Requires-Dist: colorama==0.4.6; extra == "all"
-Requires-Dist: g4f>=0.2.6.1; extra == "all"
+Requires-Dist: g4f>=0.3.0.8; extra == "all"
 Requires-Dist: python-dotenv==1.0.0; extra == "all"
 Requires-Dist: fastapi[all]==0.110.1; extra == "all"
 
 <p align="center">
 <img src="https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true" width='40%'>
 </p>
 
@@ -73,15 +74,15 @@
 <!--
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 -->
 <a href="https://github.com/Simatwa/python-tgpt/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/python-tgpt"/></a>
 <a href="https://pypi.org/project/python-tgpt"><img alt="PyPi" src="https://img.shields.io/pypi/v/python-tgpt?color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>
-<a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
+<a href="#"><img alt="Website status" src="https://img.shields.io/website?url=https://python-tgpt.onrender.com"/></a>
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml"><img alt="Python Package flow" src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml/badge.svg?branch=master"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="https://pepy.tech/project/tgpt2"><img src="https://static.pepy.tech/personalized-badge/tgpt2?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" alt="Downloads"></a>
 <a href="https://pepy.tech/project/python-tgpt"><img src="https://static.pepy.tech/personalized-badge/python-tgpt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" alt="Downloads"></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases/latest"><img src="https://img.shields.io/github/downloads/Simatwa/python-tgpt/total?label=Asset%20Downloads&color=success" alt="Downloads"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/v/release/Simatwa/python-tgpt?color=success&label=Release&logo=github" alt="Latest release"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/release-date/Simatwa/python-tgpt?label=Release date&logo=github" alt="release date"></img></a>
@@ -129,15 +130,17 @@
 - 🔌 Offline support for Large Language Models
 - 🎨 Image generation capabilities
 - 🎤 Text-to-audio conversion capabilities
 - ⛓️ Chained requests via proxy
 - 🗨️ Enhanced conversational chat experience
 - 💾 Capability to save prompts and responses (Conversation)
 - 🔄 Ability to load previous conversations
-- 🤖 Pass [awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
+- 🚀 Pass [awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
+- 🤖 [Telegram bot](https://t.me/pytgpt_bot) - interface
+- 🔄 Asynchronous support for all major operations.
 
 
 ## Providers
 
 These are simply the hosts of the LLMs, which include:
 
 1. [Leo](https://brave.com/leo/) - **Brave**
@@ -388,14 +391,62 @@
 import pytgpt.gpt4free as gpt4free
 bot = gpt4free.GPT4FREE(provider="Koala")
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
+### Asynchronous
+
+**Version 0.7.0** introduces asynchronous implementation to almost all providers except a few such as *perplexity & gemini*, which relies on other libraries which lacks such implementation.
+
+To make it easier, you just have to prefix `Async` to the common synchronous class name. For instance `OPENGPT` will be accessed as `AsyncOPENGPT`:
+
+#### Streaming Whole ai response.
+
+```python
+import asyncio
+from pytgpt.phind import AsyncPHIND
+
+async def main():
+    async_ask = await AsyncPHIND(False).ask(
+        "Critique that python is cool.",
+        stream=True
+    )
+    async for streaming_response in async_ask:
+        print(
+            streaming_response
+        )
+
+asyncio.run(
+    main()
+)
+```
+
+#### Streaming just the text
+
+```python
+import asyncio
+from pytgpt.phind import AsyncPHIND
+
+async def main():
+    async_ask = await AsyncPHIND(False).chat(
+        "Critique that python is cool.",
+        stream=True
+    )
+    async for streaming_text in async_ask:
+        print(
+            streaming_text
+        )
+
+asyncio.run(
+    main()
+)
+```
+
 </details>
 
 <details>
 
 <summary>
 
 To obtain more tailored responses, consider utilizing [optimizers](pytgpt/utils.py) using the `optimizer` parameter. Its values can be set to either `code` or `system_command`.
@@ -596,14 +647,24 @@
 
 Version **0.6.4** introduces another dynamic provider, `auto`, which denotes the working provider **overall**. This relieves you of the workload of manually checking a working provider each time you fire up pytgpt.
 
 ## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot)
 
 If you're not satisfied with the existing interfaces, [pytgpt-bot](https://github.com/Simatwa/pytgpt-bot) could be the solution you're seeking. This bot is designed to enhance your experience by offering a wide range of functionalities. Whether you're interested in engaging in AI-driven conversations, creating images and audio from text, or exploring other innovative features, [pytgpt-bot is equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot)
 
+The bot is maintained as a separate project so you just have to execute a command get it installed :
+
+```
+$ pip install pytgpt-bot
+```
+
+Usage : `pytgpt bot run <bot-api-token>`
+
+Or you can simply interact with the one running now as [@pytgpt-bot](https://t.me/pytgpt_bot)
+
 <details>
 
 <summary>
 
 For more usage info run `$ pytgpt --help`
 
 </summary>
@@ -614,14 +675,15 @@
 Options:
   -v, --version  Show the version and exit.
   -h, --help     Show this message and exit.
 
 Commands:
   api          FastAPI control endpoint
   awesome      Perform CRUD operations on awesome-prompts
+  bot          Telegram bot interface control
   generate     Generate a quick response with AI
   gpt4free     Discover gpt4free models, providers etc
   imager       Generate images with pollinations.ai
   interactive  Chat with AI interactively (Default)
   utils        Utility endpoint for pytgpt
   webchatgpt   Reverse Engineered ChatGPT Web-Version
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.9 Summary: Interact with
+Metadata-Version: 2.1 Name: python-tgpt Version: 0.7.0 Summary: Interact with
 AI without API key Home-page: https://github.com/Simatwa/python-tgpt Author:
 Smartwa Author-email: simatwacaleb@proton.me Maintainer: Smartwa License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/python-tgpt Project-URL:
 Source Code, https://github.com/Simatwa/python-tgpt Project-URL: Issue Tracker,
 https://github.com/Simatwa/python-tgpt/issues Project-URL: Download, https://
 github.com/Simatwa/python-tgpt/releases Project-URL: Documentation, https://
@@ -19,34 +19,34 @@
 Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: requests[socks]==2.31.0 Requires-Dist: appdirs==1.4.4
 Requires-Dist: pyyaml==6.0.1 Requires-Dist: webchatgpt==0.3.0 Requires-Dist:
 GoogleBard1>=2.1.4 Requires-Dist: poe-api-wrapper==1.3.6 Requires-Dist:
-brotli==1.1.0 Requires-Dist: g4f>=0.2.6.1 Requires-Dist: Helpingai_T2-
-fork==0.3.2 Requires-Dist: python-vlc>=3.0.20 Provides-Extra: cli Requires-
-Dist: click==8.1.3; extra == "cli" Requires-Dist: rich==13.3.4; extra == "cli"
-Requires-Dist: clipman==3.1.0; extra == "cli" Requires-Dist: pyperclip==1.8.2;
-extra == "cli" Requires-Dist: colorama==0.4.6; extra == "cli" Requires-Dist:
-g4f>=0.2.6.1; extra == "cli" Requires-Dist: python-dotenv==1.0.0; extra ==
-"cli" Provides-Extra: api Requires-Dist: fastapi[all]==0.110.1; extra == "api"
-Provides-Extra: all Requires-Dist: g4f[all]>=0.2.6.1; extra == "all" Requires-
-Dist: matplotlib; extra == "all" Requires-Dist: gpt4all==2.2.0; extra == "all"
-Requires-Dist: click==8.1.3; extra == "all" Requires-Dist: rich==13.3.4; extra
-== "all" Requires-Dist: clipman==3.1.0; extra == "all" Requires-Dist:
-pyperclip==1.8.2; extra == "all" Requires-Dist: colorama==0.4.6; extra == "all"
-Requires-Dist: g4f>=0.2.6.1; extra == "all" Requires-Dist: python-
-dotenv==1.0.0; extra == "all" Requires-Dist: fastapi[all]==0.110.1; extra ==
-"all"
+brotli==1.1.0 Requires-Dist: g4f>=0.3.0.8 Requires-Dist: Helpingai_T2-
+fork==0.3.2 Requires-Dist: python-vlc>=3.0.20 Requires-Dist: httpx==0.27.0
+Provides-Extra: cli Requires-Dist: click==8.1.3; extra == "cli" Requires-Dist:
+rich==13.3.4; extra == "cli" Requires-Dist: clipman==3.1.0; extra == "cli"
+Requires-Dist: pyperclip==1.8.2; extra == "cli" Requires-Dist: colorama==0.4.6;
+extra == "cli" Requires-Dist: g4f>=0.3.0.8; extra == "cli" Requires-Dist:
+python-dotenv==1.0.0; extra == "cli" Provides-Extra: api Requires-Dist: fastapi
+[all]==0.110.1; extra == "api" Provides-Extra: all Requires-Dist: g4f
+[all]>=0.2.6.1; extra == "all" Requires-Dist: matplotlib; extra == "all"
+Requires-Dist: gpt4all==2.2.0; extra == "all" Requires-Dist: click==8.1.3;
+extra == "all" Requires-Dist: rich==13.3.4; extra == "all" Requires-Dist:
+clipman==3.1.0; extra == "all" Requires-Dist: pyperclip==1.8.2; extra == "all"
+Requires-Dist: colorama==0.4.6; extra == "all" Requires-Dist: g4f>=0.3.0.8;
+extra == "all" Requires-Dist: python-dotenv==1.0.0; extra == "all" Requires-
+Dist: fastapi[all]==0.110.1; extra == "all"
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true]
-_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_P_a_s_s_i_n_g_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]_[_c_o_v_e_r_a_g_e_]
-   _[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]_[_h_t_t_p_s_:_/_/
-  _h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/_b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/
-                        _S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
+  _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_W_e_b_s_i_t_e_ _s_t_a_t_u_s_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]
+   _[_c_o_v_e_r_a_g_e_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]
+                 _[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
+     _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/_S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
                              ******** ppyytthhoonn--ttggpptt ********
  [https://github.com/Simatwa/python-tgpt/blob/main/assets/demo-1.gif?raw=True]
 ```python >>> import pytgpt.phind as phind >>> bot = phind.PHIND() >>> bot.chat
 ('hello there') 'Hello! How can I assist you today?' ``` ```python from
 pytgpt.imager import Imager img = Imager() generated_images = img.generate
 (prompt="Cyberpunk", amount=3, stream=True) img.save(generated_images) ``` This
 project enables seamless interaction with over **45 free LLM providers**
@@ -59,37 +59,39 @@
 tgpt.onrender.com) - â¨ï¸ Command-line interface - ð§  Multiple LLM
 providers - **45+** - ð Stream and non-stream response - ð Ready to use
 (No API key required) - ð¯ Customizable script generation and execution -
 ð Offline support for Large Language Models - ð¨ Image generation
 capabilities - ð¤ Text-to-audio conversion capabilities - âï¸ Chained
 requests via proxy - ð¨ï¸ Enhanced conversational chat experience - ð¾
 Capability to save prompts and responses (Conversation) - ð Ability to load
-previous conversations - ð¤ Pass [awesome-chatgpt prompts](https://
-github.com/f/awesome-chatgpt-prompts) easily ## Providers These are simply the
-hosts of the LLMs, which include: 1. [Leo](https://brave.com/leo/) - **Brave**
-2. [Koboldai](https://koboldai-koboldcpp-tiefighter.hf.space) 3. [OpenGPTs]
-(https://opengpts-example-vz4y4ooboq-uc.a.run.app/) 4. [OpenAI](https://
-chat.openai.com) *(API key required)* 5. [WebChatGPT](https://github.com/
-Simatwa/WebChatGPT) - **OpenAI** *(Session ID required)* 6. [Gemini](https://
-github.com/Simatwa/bard) - **Google** *(Session ID required)* 9. [Phind](https:
-//www.phind.com) 10. [Llama2](https://www.llama2.ai) 11. [Blackboxai](https://
-www.blackbox.ai) 12. [gpt4all](https://gpt4all.io) *(Offline)* 13. [Poe](https:
-//poe.com) - Poe|Quora *(Session ID required)* 14. [Groq](https://
-console.groq.com/playground) *(API Key required)* 15. [Perplexity](https://
-www.perplexity.ai) 16. [YepChat](https://yep.com) 41+ providers proudly offered
-by [gpt4free](https://github.com/xtekky/gpt4free). - To list working providers
-run: ```sh $ pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10]
-(https://python.org) *(Optional)* ## Installation and Usage ### Installation
-Download binaries for your system from [here.](https://github.com/Simatwa/
-python-tgpt/releases/latest/) Alternatively, you can install non-binaries. *
-(Recommended)* 1. Developers: ```sh pip install --upgrade python-tgpt ``` 2.
-Commandline: ```sh pip install --upgrade "python-tgpt[cli]" ``` 3. Full
-installation: ```sh pip install --upgrade "python-tgpt[all]" ``` > `pip install
--U "python-tgt[api]"` will install REST API dependencies. ## Usage This package
-offers a convenient command-line interface. > [!NOTE] > `phind` is the default
+previous conversations - ð Pass [awesome-chatgpt prompts](https://
+github.com/f/awesome-chatgpt-prompts) easily - ð¤ [Telegram bot](https://
+t.me/pytgpt_bot) - interface - ð Asynchronous support for all major
+operations. ## Providers These are simply the hosts of the LLMs, which include:
+1. [Leo](https://brave.com/leo/) - **Brave** 2. [Koboldai](https://koboldai-
+koboldcpp-tiefighter.hf.space) 3. [OpenGPTs](https://opengpts-example-
+vz4y4ooboq-uc.a.run.app/) 4. [OpenAI](https://chat.openai.com) *(API key
+required)* 5. [WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI**
+*(Session ID required)* 6. [Gemini](https://github.com/Simatwa/bard) -
+**Google** *(Session ID required)* 9. [Phind](https://www.phind.com) 10.
+[Llama2](https://www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12.
+[gpt4all](https://gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) -
+Poe|Quora *(Session ID required)* 14. [Groq](https://console.groq.com/
+playground) *(API Key required)* 15. [Perplexity](https://www.perplexity.ai)
+16. [YepChat](https://yep.com) 41+ providers proudly offered by [gpt4free]
+(https://github.com/xtekky/gpt4free). - To list working providers run: ```sh $
+pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10](https://
+python.org) *(Optional)* ## Installation and Usage ### Installation Download
+binaries for your system from [here.](https://github.com/Simatwa/python-tgpt/
+releases/latest/) Alternatively, you can install non-binaries. *(Recommended)*
+1. Developers: ```sh pip install --upgrade python-tgpt ``` 2. Commandline:
+```sh pip install --upgrade "python-tgpt[cli]" ``` 3. Full installation: ```sh
+pip install --upgrade "python-tgpt[all]" ``` > `pip install -U "python-tgt
+[api]"` will install REST API dependencies. ## Usage This package offers a
+convenient command-line interface. > [!NOTE] > `phind` is the default
 *provider*. - For a quick response: ```bash python -m pytgpt generate "" ``` -
 For interactive mode: ```bash python -m pytgpt interactive "" ``` Make use of
 flag `--provider` followed by the provider name of your choice. e.g `--provider
 koboldai` > To list all providers offered by gpt4free, use following commands:
 ```pytgpt gpt4free list providers``` You can also simply use `pytgpt` instead
 of `python -m pytgpt`. Starting from version 0.2.7, running `$ pytgpt` without
 any other command or option will automatically enter the `interactive` mode.
@@ -122,68 +124,80 @@
 import pytgpt.auto import auto bot = auto.AUTO() print(bot.chat("")) ``` Openai
 ```python import pytgpt.openai as openai bot = openai.OPENAI("") print(bot.chat
 ("")) ``` Koboldai ```python import pytgpt.koboldai as koboldai bot =
 koboldai.KOBOLDAI() print(bot.chat("")) ``` Opengpt ```python import
 pytgpt.opengpt as opengpt bot = opengpt.OPENGPT() print(bot.chat("")) ``` phind
 ```python import pytgpt.phind as phind bot = phind.PHIND() print(bot.chat(""))
 ``` Gpt4free providers ```python import pytgpt.gpt4free as gpt4free bot =
-gpt4free.GPT4FREE(provider="Koala") print(bot.chat("")) ``` To obtain more
-tailored responses, consider utilizing [optimizers](pytgpt/utils.py) using the
-`optimizer` parameter. Its values can be set to either `code` or
-`system_command`. ```python from pytgpt.leo import LEO bot = LEO() resp =
-bot.ask('', optimizer='code') print(resp) ``` > [!IMPORTANT] > Commencing from
-[v0.1.0](https://github.com/Simatwa/python-tgpt/releases/), the default mode of
-interaction is conversational. This mode enhances the interactive experience,
-offering better control over the chat history. By associating previous prompts
-and responses, it tailors conversations for a more engaging experience. You can
-still disable the mode: ```python bot = koboldai.KOBOLDAI
-(is_conversation=False) ``` Utilize the `--disable-conversation` flag in the
-console to achieve the same functionality. > [!CAUTION] > **Bard** autohandles
-context due to the obvious reason; the `is_conversation` parameter is not
-necessary at all hence not required when initializing the class. Also be
-informed that majority of providers offered by *gpt4free* requires *Google
-Chrome* inorder to function. ### Image Generation This has been made possible
-by [pollinations.ai](https://pollination.ai). ```sh $ pytgpt imager "" # e.g
-pytgpt imager "Coding bot" ``` Developers ```python from pytgpt.imager import
-Imager img = Imager() generated_img = img.generate('Coding bot') # [bytes]
-img.save(generated_img) ``` Download Multiple Images ```python from
-pytgpt.imager import Imager img = Imager() img_generator = img.generate('Coding
-bot', amount=3, stream=True) img.save(img_generator) # RAM friendly ``` ####
-Using **Prodia** provider ```python from pytgpt.imager import Prodia img =
-Prodia() img_generator = img.generate('Coding bot', amount=3, stream=True)
-img.save(img_generator) ``` ### Advanced Usage of Placeholders The `generate`
-functionality has been enhanced starting from *v0.3.0* to enable comprehensive
-utilization of the `--with-copied` option and support for accepting piped
-inputs. This improvement introduces placeholders, offering dynamic values for
-more versatile interactions. | Placeholder | Represents | | ------------ | ----
-------- | | `{{stream}}` | The piped input | | `{{copied}}` | The last copied
-text | This feature is particularly beneficial for intricate operations. For
-example: ```bash $ git diff | pytgpt generate "Here is a diff file: {{stream}}
-Make a concise commit message from it, aligning with my commit message history:
-{{copied}}" --shell --new ``` > In this illustration, `{{stream}}` denotes the
-result of the `$ git diff` operation, while `{{copied}}` signifies the content
-copied from the output of the `$ git log` command. ### Awesome Prompts [These
-prompts](https://github.com/Simatwa/gpt-cli/blob/main/assets/all-
-acts.pdf?raw=True) are designed to guide the AI's behavior or responses in a
-particular direction, encouraging it to exhibit certain characteristics or
-behaviors. The term "awesome-prompt" is not a formal term in AI or machine
-learning literature, but it encapsulates the idea of crafting prompts that are
-effective in achieving desired outcomes. Let's say you want it to behave like a
-*Linux Terminal*, *PHP Interpreter*, or just to [**JAIL BREAK.**](https://
-gist.github.com/coolaj86/6f4f7b30129b0251f61fa7baaa881516) Instances : ```sh $
-pytgpt interactve --awesome-prompt "Linux Terminal" # Act like a Linux Terminal
-$ pytgpt interactive -ap DAN # Jailbreak ``` > [!NOTE] > Awesome prompts are
-alternative to `--intro`. > Run `$ pytgpt awesome whole` to list available
-prompts (*200+*). > Run `$ pytgpt awesome --help` for more info. ###
-Introducing RawDog RawDog is a masterpiece feature that exploits the versatile
-capabilities of Python to command and control your system as per your needs.
-You can literally do anything with it, since it generates and executes python
-codes, driven by **your prompts**! To have a bite of *rawdog* simply append the
-flag `--rawdog` *shortform* `-rd` in *generate/interactive* mode. This
-introduces a never seen-before feature in the *tgpt ecosystem*. Thanks to
+gpt4free.GPT4FREE(provider="Koala") print(bot.chat("")) ``` ### Asynchronous
+**Version 0.7.0** introduces asynchronous implementation to almost all
+providers except a few such as *perplexity & gemini*, which relies on other
+libraries which lacks such implementation. To make it easier, you just have to
+prefix `Async` to the common synchronous class name. For instance `OPENGPT`
+will be accessed as `AsyncOPENGPT`: #### Streaming Whole ai response. ```python
+import asyncio from pytgpt.phind import AsyncPHIND async def main(): async_ask
+= await AsyncPHIND(False).ask( "Critique that python is cool.", stream=True )
+async for streaming_response in async_ask: print( streaming_response )
+asyncio.run( main() ) ``` #### Streaming just the text ```python import asyncio
+from pytgpt.phind import AsyncPHIND async def main(): async_ask = await
+AsyncPHIND(False).chat( "Critique that python is cool.", stream=True ) async
+for streaming_text in async_ask: print( streaming_text ) asyncio.run( main() )
+``` To obtain more tailored responses, consider utilizing [optimizers](pytgpt/
+utils.py) using the `optimizer` parameter. Its values can be set to either
+`code` or `system_command`. ```python from pytgpt.leo import LEO bot = LEO()
+resp = bot.ask('', optimizer='code') print(resp) ``` > [!IMPORTANT] >
+Commencing from [v0.1.0](https://github.com/Simatwa/python-tgpt/releases/), the
+default mode of interaction is conversational. This mode enhances the
+interactive experience, offering better control over the chat history. By
+associating previous prompts and responses, it tailors conversations for a more
+engaging experience. You can still disable the mode: ```python bot =
+koboldai.KOBOLDAI(is_conversation=False) ``` Utilize the `--disable-
+conversation` flag in the console to achieve the same functionality. >
+[!CAUTION] > **Bard** autohandles context due to the obvious reason; the
+`is_conversation` parameter is not necessary at all hence not required when
+initializing the class. Also be informed that majority of providers offered by
+*gpt4free* requires *Google Chrome* inorder to function. ### Image Generation
+This has been made possible by [pollinations.ai](https://pollination.ai). ```sh
+$ pytgpt imager "" # e.g pytgpt imager "Coding bot" ``` Developers ```python
+from pytgpt.imager import Imager img = Imager() generated_img = img.generate
+('Coding bot') # [bytes] img.save(generated_img) ``` Download Multiple Images
+```python from pytgpt.imager import Imager img = Imager() img_generator =
+img.generate('Coding bot', amount=3, stream=True) img.save(img_generator) # RAM
+friendly ``` #### Using **Prodia** provider ```python from pytgpt.imager import
+Prodia img = Prodia() img_generator = img.generate('Coding bot', amount=3,
+stream=True) img.save(img_generator) ``` ### Advanced Usage of Placeholders The
+`generate` functionality has been enhanced starting from *v0.3.0* to enable
+comprehensive utilization of the `--with-copied` option and support for
+accepting piped inputs. This improvement introduces placeholders, offering
+dynamic values for more versatile interactions. | Placeholder | Represents | |
+------------ | ----------- | | `{{stream}}` | The piped input | | `{{copied}}`
+| The last copied text | This feature is particularly beneficial for intricate
+operations. For example: ```bash $ git diff | pytgpt generate "Here is a diff
+file: {{stream}} Make a concise commit message from it, aligning with my commit
+message history: {{copied}}" --shell --new ``` > In this illustration, `{
+{stream}}` denotes the result of the `$ git diff` operation, while `{{copied}}`
+signifies the content copied from the output of the `$ git log` command. ###
+Awesome Prompts [These prompts](https://github.com/Simatwa/gpt-cli/blob/main/
+assets/all-acts.pdf?raw=True) are designed to guide the AI's behavior or
+responses in a particular direction, encouraging it to exhibit certain
+characteristics or behaviors. The term "awesome-prompt" is not a formal term in
+AI or machine learning literature, but it encapsulates the idea of crafting
+prompts that are effective in achieving desired outcomes. Let's say you want it
+to behave like a *Linux Terminal*, *PHP Interpreter*, or just to [**JAIL
+BREAK.**](https://gist.github.com/coolaj86/6f4f7b30129b0251f61fa7baaa881516)
+Instances : ```sh $ pytgpt interactve --awesome-prompt "Linux Terminal" # Act
+like a Linux Terminal $ pytgpt interactive -ap DAN # Jailbreak ``` > [!NOTE] >
+Awesome prompts are alternative to `--intro`. > Run `$ pytgpt awesome whole` to
+list available prompts (*200+*). > Run `$ pytgpt awesome --help` for more info.
+### Introducing RawDog RawDog is a masterpiece feature that exploits the
+versatile capabilities of Python to command and control your system as per your
+needs. You can literally do anything with it, since it generates and executes
+python codes, driven by **your prompts**! To have a bite of *rawdog* simply
+append the flag `--rawdog` *shortform* `-rd` in *generate/interactive* mode.
+This introduces a never seen-before feature in the *tgpt ecosystem*. Thanks to
 [AbanteAI/rawdog](https://github.com/AbanteAI/rawdog) for the idea. This can be
 useful in some ways. For instance : ```sh $ pytgpt generate -n -q "Visualize
 the disk usage using pie chart" --rawdog ``` This will pop up a window showing
 system disk usage as shown below.
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/Figure_1.png?raw=true]
 ## Passing Environment Variables Pytgpt **v0.4.6** introduces a convention way
 of taking variables from the environment. To achieve that, set the environment
@@ -225,21 +239,24 @@
 the workload of manually checking a working provider each time you fire up
 pytgpt. ## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot) If you're not
 satisfied with the existing interfaces, [pytgpt-bot](https://github.com/
 Simatwa/pytgpt-bot) could be the solution you're seeking. This bot is designed
 to enhance your experience by offering a wide range of functionalities. Whether
 you're interested in engaging in AI-driven conversations, creating images and
 audio from text, or exploring other innovative features, [pytgpt-bot is
-equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot) For more
-usage info run `$ pytgpt --help` ``` Usage: pytgpt [OPTIONS] COMMAND [ARGS]...
-Options: -v, --version Show the version and exit. -h, --help Show this message
-and exit. Commands: api FastAPI control endpoint awesome Perform CRUD
-operations on awesome-prompts generate Generate a quick response with AI
-gpt4free Discover gpt4free models, providers etc imager Generate images with
-pollinations.ai interactive Chat with AI interactively (Default) utils Utility
-endpoint for pytgpt webchatgpt Reverse Engineered ChatGPT Web-Version ``` ###
-API Health Status | No. | API | Status | |--------|-----|--------| | 1. | [On-
-render](https://python-tgpt.onrender.com) | [cron-job](https://
-pqfzhmvz.status.cron-job.org/) | ## [CHANGELOG](https://github.com/Simatwa/
-python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [x] [tgpt]
-(https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://github.com/
-xtekky/gpt4free)
+equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot) The bot is
+maintained as a separate project so you just have to execute a command get it
+installed : ``` $ pip install pytgpt-bot ``` Usage : `pytgpt bot run ` Or you
+can simply interact with the one running now as [@pytgpt-bot](https://t.me/
+pytgpt_bot) For more usage info run `$ pytgpt --help` ``` Usage: pytgpt
+[OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the version and exit. -
+h, --help Show this message and exit. Commands: api FastAPI control endpoint
+awesome Perform CRUD operations on awesome-prompts bot Telegram bot interface
+control generate Generate a quick response with AI gpt4free Discover gpt4free
+models, providers etc imager Generate images with pollinations.ai interactive
+Chat with AI interactively (Default) utils Utility endpoint for pytgpt
+webchatgpt Reverse Engineered ChatGPT Web-Version ``` ### API Health Status |
+No. | API | Status | |--------|-----|--------| | 1. | [On-render](https://
+python-tgpt.onrender.com) | [cron-job](https://pqfzhmvz.status.cron-job.org/) |
+## [CHANGELOG](https://github.com/Simatwa/python-tgpt/blob/main/docs/
+CHANGELOG.md) ## Acknowledgements 1. [x] [tgpt](https://github.com/aandrew-me/
+tgpt) 2. [x] [gpt4free](https://github.com/xtekky/gpt4free)
```

### Comparing `python_tgpt-0.6.9/README.md` & `python_tgpt-0.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 <!--
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 -->
 <a href="https://github.com/Simatwa/python-tgpt/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/python-tgpt"/></a>
 <a href="https://pypi.org/project/python-tgpt"><img alt="PyPi" src="https://img.shields.io/pypi/v/python-tgpt?color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>
-<a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
+<a href="#"><img alt="Website status" src="https://img.shields.io/website?url=https://python-tgpt.onrender.com"/></a>
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml"><img alt="Python Package flow" src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml/badge.svg?branch=master"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="https://pepy.tech/project/tgpt2"><img src="https://static.pepy.tech/personalized-badge/tgpt2?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" alt="Downloads"></a>
 <a href="https://pepy.tech/project/python-tgpt"><img src="https://static.pepy.tech/personalized-badge/python-tgpt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" alt="Downloads"></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases/latest"><img src="https://img.shields.io/github/downloads/Simatwa/python-tgpt/total?label=Asset%20Downloads&color=success" alt="Downloads"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/v/release/Simatwa/python-tgpt?color=success&label=Release&logo=github" alt="Latest release"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/release-date/Simatwa/python-tgpt?label=Release date&logo=github" alt="release date"></img></a>
@@ -63,15 +63,17 @@
 - 🔌 Offline support for Large Language Models
 - 🎨 Image generation capabilities
 - 🎤 Text-to-audio conversion capabilities
 - ⛓️ Chained requests via proxy
 - 🗨️ Enhanced conversational chat experience
 - 💾 Capability to save prompts and responses (Conversation)
 - 🔄 Ability to load previous conversations
-- 🤖 Pass [awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
+- 🚀 Pass [awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
+- 🤖 [Telegram bot](https://t.me/pytgpt_bot) - interface
+- 🔄 Asynchronous support for all major operations.
 
 
 ## Providers
 
 These are simply the hosts of the LLMs, which include:
 
 1. [Leo](https://brave.com/leo/) - **Brave**
@@ -322,14 +324,62 @@
 import pytgpt.gpt4free as gpt4free
 bot = gpt4free.GPT4FREE(provider="Koala")
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
+### Asynchronous
+
+**Version 0.7.0** introduces asynchronous implementation to almost all providers except a few such as *perplexity & gemini*, which relies on other libraries which lacks such implementation.
+
+To make it easier, you just have to prefix `Async` to the common synchronous class name. For instance `OPENGPT` will be accessed as `AsyncOPENGPT`:
+
+#### Streaming Whole ai response.
+
+```python
+import asyncio
+from pytgpt.phind import AsyncPHIND
+
+async def main():
+    async_ask = await AsyncPHIND(False).ask(
+        "Critique that python is cool.",
+        stream=True
+    )
+    async for streaming_response in async_ask:
+        print(
+            streaming_response
+        )
+
+asyncio.run(
+    main()
+)
+```
+
+#### Streaming just the text
+
+```python
+import asyncio
+from pytgpt.phind import AsyncPHIND
+
+async def main():
+    async_ask = await AsyncPHIND(False).chat(
+        "Critique that python is cool.",
+        stream=True
+    )
+    async for streaming_text in async_ask:
+        print(
+            streaming_text
+        )
+
+asyncio.run(
+    main()
+)
+```
+
 </details>
 
 <details>
 
 <summary>
 
 To obtain more tailored responses, consider utilizing [optimizers](pytgpt/utils.py) using the `optimizer` parameter. Its values can be set to either `code` or `system_command`.
@@ -530,14 +580,24 @@
 
 Version **0.6.4** introduces another dynamic provider, `auto`, which denotes the working provider **overall**. This relieves you of the workload of manually checking a working provider each time you fire up pytgpt.
 
 ## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot)
 
 If you're not satisfied with the existing interfaces, [pytgpt-bot](https://github.com/Simatwa/pytgpt-bot) could be the solution you're seeking. This bot is designed to enhance your experience by offering a wide range of functionalities. Whether you're interested in engaging in AI-driven conversations, creating images and audio from text, or exploring other innovative features, [pytgpt-bot is equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot)
 
+The bot is maintained as a separate project so you just have to execute a command get it installed :
+
+```
+$ pip install pytgpt-bot
+```
+
+Usage : `pytgpt bot run <bot-api-token>`
+
+Or you can simply interact with the one running now as [@pytgpt-bot](https://t.me/pytgpt_bot)
+
 <details>
 
 <summary>
 
 For more usage info run `$ pytgpt --help`
 
 </summary>
@@ -548,14 +608,15 @@
 Options:
   -v, --version  Show the version and exit.
   -h, --help     Show this message and exit.
 
 Commands:
   api          FastAPI control endpoint
   awesome      Perform CRUD operations on awesome-prompts
+  bot          Telegram bot interface control
   generate     Generate a quick response with AI
   gpt4free     Discover gpt4free models, providers etc
   imager       Generate images with pollinations.ai
   interactive  Chat with AI interactively (Default)
   utils        Utility endpoint for pytgpt
   webchatgpt   Reverse Engineered ChatGPT Web-Version
 ```
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true]
-_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_P_a_s_s_i_n_g_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]_[_c_o_v_e_r_a_g_e_]
-   _[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]_[_h_t_t_p_s_:_/_/
-  _h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/_b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/
-                        _S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
+  _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_W_e_b_s_i_t_e_ _s_t_a_t_u_s_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]
+   _[_c_o_v_e_r_a_g_e_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]
+                 _[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
+     _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/_S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
                              ******** ppyytthhoonn--ttggpptt ********
  [https://github.com/Simatwa/python-tgpt/blob/main/assets/demo-1.gif?raw=True]
 ```python >>> import pytgpt.phind as phind >>> bot = phind.PHIND() >>> bot.chat
 ('hello there') 'Hello! How can I assist you today?' ``` ```python from
 pytgpt.imager import Imager img = Imager() generated_images = img.generate
 (prompt="Cyberpunk", amount=3, stream=True) img.save(generated_images) ``` This
 project enables seamless interaction with over **45 free LLM providers**
@@ -19,37 +19,39 @@
 tgpt.onrender.com) - â¨ï¸ Command-line interface - ð§  Multiple LLM
 providers - **45+** - ð Stream and non-stream response - ð Ready to use
 (No API key required) - ð¯ Customizable script generation and execution -
 ð Offline support for Large Language Models - ð¨ Image generation
 capabilities - ð¤ Text-to-audio conversion capabilities - âï¸ Chained
 requests via proxy - ð¨ï¸ Enhanced conversational chat experience - ð¾
 Capability to save prompts and responses (Conversation) - ð Ability to load
-previous conversations - ð¤ Pass [awesome-chatgpt prompts](https://
-github.com/f/awesome-chatgpt-prompts) easily ## Providers These are simply the
-hosts of the LLMs, which include: 1. [Leo](https://brave.com/leo/) - **Brave**
-2. [Koboldai](https://koboldai-koboldcpp-tiefighter.hf.space) 3. [OpenGPTs]
-(https://opengpts-example-vz4y4ooboq-uc.a.run.app/) 4. [OpenAI](https://
-chat.openai.com) *(API key required)* 5. [WebChatGPT](https://github.com/
-Simatwa/WebChatGPT) - **OpenAI** *(Session ID required)* 6. [Gemini](https://
-github.com/Simatwa/bard) - **Google** *(Session ID required)* 9. [Phind](https:
-//www.phind.com) 10. [Llama2](https://www.llama2.ai) 11. [Blackboxai](https://
-www.blackbox.ai) 12. [gpt4all](https://gpt4all.io) *(Offline)* 13. [Poe](https:
-//poe.com) - Poe|Quora *(Session ID required)* 14. [Groq](https://
-console.groq.com/playground) *(API Key required)* 15. [Perplexity](https://
-www.perplexity.ai) 16. [YepChat](https://yep.com) 41+ providers proudly offered
-by [gpt4free](https://github.com/xtekky/gpt4free). - To list working providers
-run: ```sh $ pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10]
-(https://python.org) *(Optional)* ## Installation and Usage ### Installation
-Download binaries for your system from [here.](https://github.com/Simatwa/
-python-tgpt/releases/latest/) Alternatively, you can install non-binaries. *
-(Recommended)* 1. Developers: ```sh pip install --upgrade python-tgpt ``` 2.
-Commandline: ```sh pip install --upgrade "python-tgpt[cli]" ``` 3. Full
-installation: ```sh pip install --upgrade "python-tgpt[all]" ``` > `pip install
--U "python-tgt[api]"` will install REST API dependencies. ## Usage This package
-offers a convenient command-line interface. > [!NOTE] > `phind` is the default
+previous conversations - ð Pass [awesome-chatgpt prompts](https://
+github.com/f/awesome-chatgpt-prompts) easily - ð¤ [Telegram bot](https://
+t.me/pytgpt_bot) - interface - ð Asynchronous support for all major
+operations. ## Providers These are simply the hosts of the LLMs, which include:
+1. [Leo](https://brave.com/leo/) - **Brave** 2. [Koboldai](https://koboldai-
+koboldcpp-tiefighter.hf.space) 3. [OpenGPTs](https://opengpts-example-
+vz4y4ooboq-uc.a.run.app/) 4. [OpenAI](https://chat.openai.com) *(API key
+required)* 5. [WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI**
+*(Session ID required)* 6. [Gemini](https://github.com/Simatwa/bard) -
+**Google** *(Session ID required)* 9. [Phind](https://www.phind.com) 10.
+[Llama2](https://www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12.
+[gpt4all](https://gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) -
+Poe|Quora *(Session ID required)* 14. [Groq](https://console.groq.com/
+playground) *(API Key required)* 15. [Perplexity](https://www.perplexity.ai)
+16. [YepChat](https://yep.com) 41+ providers proudly offered by [gpt4free]
+(https://github.com/xtekky/gpt4free). - To list working providers run: ```sh $
+pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10](https://
+python.org) *(Optional)* ## Installation and Usage ### Installation Download
+binaries for your system from [here.](https://github.com/Simatwa/python-tgpt/
+releases/latest/) Alternatively, you can install non-binaries. *(Recommended)*
+1. Developers: ```sh pip install --upgrade python-tgpt ``` 2. Commandline:
+```sh pip install --upgrade "python-tgpt[cli]" ``` 3. Full installation: ```sh
+pip install --upgrade "python-tgpt[all]" ``` > `pip install -U "python-tgt
+[api]"` will install REST API dependencies. ## Usage This package offers a
+convenient command-line interface. > [!NOTE] > `phind` is the default
 *provider*. - For a quick response: ```bash python -m pytgpt generate "" ``` -
 For interactive mode: ```bash python -m pytgpt interactive "" ``` Make use of
 flag `--provider` followed by the provider name of your choice. e.g `--provider
 koboldai` > To list all providers offered by gpt4free, use following commands:
 ```pytgpt gpt4free list providers``` You can also simply use `pytgpt` instead
 of `python -m pytgpt`. Starting from version 0.2.7, running `$ pytgpt` without
 any other command or option will automatically enter the `interactive` mode.
@@ -82,68 +84,80 @@
 import pytgpt.auto import auto bot = auto.AUTO() print(bot.chat("")) ``` Openai
 ```python import pytgpt.openai as openai bot = openai.OPENAI("") print(bot.chat
 ("")) ``` Koboldai ```python import pytgpt.koboldai as koboldai bot =
 koboldai.KOBOLDAI() print(bot.chat("")) ``` Opengpt ```python import
 pytgpt.opengpt as opengpt bot = opengpt.OPENGPT() print(bot.chat("")) ``` phind
 ```python import pytgpt.phind as phind bot = phind.PHIND() print(bot.chat(""))
 ``` Gpt4free providers ```python import pytgpt.gpt4free as gpt4free bot =
-gpt4free.GPT4FREE(provider="Koala") print(bot.chat("")) ``` To obtain more
-tailored responses, consider utilizing [optimizers](pytgpt/utils.py) using the
-`optimizer` parameter. Its values can be set to either `code` or
-`system_command`. ```python from pytgpt.leo import LEO bot = LEO() resp =
-bot.ask('', optimizer='code') print(resp) ``` > [!IMPORTANT] > Commencing from
-[v0.1.0](https://github.com/Simatwa/python-tgpt/releases/), the default mode of
-interaction is conversational. This mode enhances the interactive experience,
-offering better control over the chat history. By associating previous prompts
-and responses, it tailors conversations for a more engaging experience. You can
-still disable the mode: ```python bot = koboldai.KOBOLDAI
-(is_conversation=False) ``` Utilize the `--disable-conversation` flag in the
-console to achieve the same functionality. > [!CAUTION] > **Bard** autohandles
-context due to the obvious reason; the `is_conversation` parameter is not
-necessary at all hence not required when initializing the class. Also be
-informed that majority of providers offered by *gpt4free* requires *Google
-Chrome* inorder to function. ### Image Generation This has been made possible
-by [pollinations.ai](https://pollination.ai). ```sh $ pytgpt imager "" # e.g
-pytgpt imager "Coding bot" ``` Developers ```python from pytgpt.imager import
-Imager img = Imager() generated_img = img.generate('Coding bot') # [bytes]
-img.save(generated_img) ``` Download Multiple Images ```python from
-pytgpt.imager import Imager img = Imager() img_generator = img.generate('Coding
-bot', amount=3, stream=True) img.save(img_generator) # RAM friendly ``` ####
-Using **Prodia** provider ```python from pytgpt.imager import Prodia img =
-Prodia() img_generator = img.generate('Coding bot', amount=3, stream=True)
-img.save(img_generator) ``` ### Advanced Usage of Placeholders The `generate`
-functionality has been enhanced starting from *v0.3.0* to enable comprehensive
-utilization of the `--with-copied` option and support for accepting piped
-inputs. This improvement introduces placeholders, offering dynamic values for
-more versatile interactions. | Placeholder | Represents | | ------------ | ----
-------- | | `{{stream}}` | The piped input | | `{{copied}}` | The last copied
-text | This feature is particularly beneficial for intricate operations. For
-example: ```bash $ git diff | pytgpt generate "Here is a diff file: {{stream}}
-Make a concise commit message from it, aligning with my commit message history:
-{{copied}}" --shell --new ``` > In this illustration, `{{stream}}` denotes the
-result of the `$ git diff` operation, while `{{copied}}` signifies the content
-copied from the output of the `$ git log` command. ### Awesome Prompts [These
-prompts](https://github.com/Simatwa/gpt-cli/blob/main/assets/all-
-acts.pdf?raw=True) are designed to guide the AI's behavior or responses in a
-particular direction, encouraging it to exhibit certain characteristics or
-behaviors. The term "awesome-prompt" is not a formal term in AI or machine
-learning literature, but it encapsulates the idea of crafting prompts that are
-effective in achieving desired outcomes. Let's say you want it to behave like a
-*Linux Terminal*, *PHP Interpreter*, or just to [**JAIL BREAK.**](https://
-gist.github.com/coolaj86/6f4f7b30129b0251f61fa7baaa881516) Instances : ```sh $
-pytgpt interactve --awesome-prompt "Linux Terminal" # Act like a Linux Terminal
-$ pytgpt interactive -ap DAN # Jailbreak ``` > [!NOTE] > Awesome prompts are
-alternative to `--intro`. > Run `$ pytgpt awesome whole` to list available
-prompts (*200+*). > Run `$ pytgpt awesome --help` for more info. ###
-Introducing RawDog RawDog is a masterpiece feature that exploits the versatile
-capabilities of Python to command and control your system as per your needs.
-You can literally do anything with it, since it generates and executes python
-codes, driven by **your prompts**! To have a bite of *rawdog* simply append the
-flag `--rawdog` *shortform* `-rd` in *generate/interactive* mode. This
-introduces a never seen-before feature in the *tgpt ecosystem*. Thanks to
+gpt4free.GPT4FREE(provider="Koala") print(bot.chat("")) ``` ### Asynchronous
+**Version 0.7.0** introduces asynchronous implementation to almost all
+providers except a few such as *perplexity & gemini*, which relies on other
+libraries which lacks such implementation. To make it easier, you just have to
+prefix `Async` to the common synchronous class name. For instance `OPENGPT`
+will be accessed as `AsyncOPENGPT`: #### Streaming Whole ai response. ```python
+import asyncio from pytgpt.phind import AsyncPHIND async def main(): async_ask
+= await AsyncPHIND(False).ask( "Critique that python is cool.", stream=True )
+async for streaming_response in async_ask: print( streaming_response )
+asyncio.run( main() ) ``` #### Streaming just the text ```python import asyncio
+from pytgpt.phind import AsyncPHIND async def main(): async_ask = await
+AsyncPHIND(False).chat( "Critique that python is cool.", stream=True ) async
+for streaming_text in async_ask: print( streaming_text ) asyncio.run( main() )
+``` To obtain more tailored responses, consider utilizing [optimizers](pytgpt/
+utils.py) using the `optimizer` parameter. Its values can be set to either
+`code` or `system_command`. ```python from pytgpt.leo import LEO bot = LEO()
+resp = bot.ask('', optimizer='code') print(resp) ``` > [!IMPORTANT] >
+Commencing from [v0.1.0](https://github.com/Simatwa/python-tgpt/releases/), the
+default mode of interaction is conversational. This mode enhances the
+interactive experience, offering better control over the chat history. By
+associating previous prompts and responses, it tailors conversations for a more
+engaging experience. You can still disable the mode: ```python bot =
+koboldai.KOBOLDAI(is_conversation=False) ``` Utilize the `--disable-
+conversation` flag in the console to achieve the same functionality. >
+[!CAUTION] > **Bard** autohandles context due to the obvious reason; the
+`is_conversation` parameter is not necessary at all hence not required when
+initializing the class. Also be informed that majority of providers offered by
+*gpt4free* requires *Google Chrome* inorder to function. ### Image Generation
+This has been made possible by [pollinations.ai](https://pollination.ai). ```sh
+$ pytgpt imager "" # e.g pytgpt imager "Coding bot" ``` Developers ```python
+from pytgpt.imager import Imager img = Imager() generated_img = img.generate
+('Coding bot') # [bytes] img.save(generated_img) ``` Download Multiple Images
+```python from pytgpt.imager import Imager img = Imager() img_generator =
+img.generate('Coding bot', amount=3, stream=True) img.save(img_generator) # RAM
+friendly ``` #### Using **Prodia** provider ```python from pytgpt.imager import
+Prodia img = Prodia() img_generator = img.generate('Coding bot', amount=3,
+stream=True) img.save(img_generator) ``` ### Advanced Usage of Placeholders The
+`generate` functionality has been enhanced starting from *v0.3.0* to enable
+comprehensive utilization of the `--with-copied` option and support for
+accepting piped inputs. This improvement introduces placeholders, offering
+dynamic values for more versatile interactions. | Placeholder | Represents | |
+------------ | ----------- | | `{{stream}}` | The piped input | | `{{copied}}`
+| The last copied text | This feature is particularly beneficial for intricate
+operations. For example: ```bash $ git diff | pytgpt generate "Here is a diff
+file: {{stream}} Make a concise commit message from it, aligning with my commit
+message history: {{copied}}" --shell --new ``` > In this illustration, `{
+{stream}}` denotes the result of the `$ git diff` operation, while `{{copied}}`
+signifies the content copied from the output of the `$ git log` command. ###
+Awesome Prompts [These prompts](https://github.com/Simatwa/gpt-cli/blob/main/
+assets/all-acts.pdf?raw=True) are designed to guide the AI's behavior or
+responses in a particular direction, encouraging it to exhibit certain
+characteristics or behaviors. The term "awesome-prompt" is not a formal term in
+AI or machine learning literature, but it encapsulates the idea of crafting
+prompts that are effective in achieving desired outcomes. Let's say you want it
+to behave like a *Linux Terminal*, *PHP Interpreter*, or just to [**JAIL
+BREAK.**](https://gist.github.com/coolaj86/6f4f7b30129b0251f61fa7baaa881516)
+Instances : ```sh $ pytgpt interactve --awesome-prompt "Linux Terminal" # Act
+like a Linux Terminal $ pytgpt interactive -ap DAN # Jailbreak ``` > [!NOTE] >
+Awesome prompts are alternative to `--intro`. > Run `$ pytgpt awesome whole` to
+list available prompts (*200+*). > Run `$ pytgpt awesome --help` for more info.
+### Introducing RawDog RawDog is a masterpiece feature that exploits the
+versatile capabilities of Python to command and control your system as per your
+needs. You can literally do anything with it, since it generates and executes
+python codes, driven by **your prompts**! To have a bite of *rawdog* simply
+append the flag `--rawdog` *shortform* `-rd` in *generate/interactive* mode.
+This introduces a never seen-before feature in the *tgpt ecosystem*. Thanks to
 [AbanteAI/rawdog](https://github.com/AbanteAI/rawdog) for the idea. This can be
 useful in some ways. For instance : ```sh $ pytgpt generate -n -q "Visualize
 the disk usage using pie chart" --rawdog ``` This will pop up a window showing
 system disk usage as shown below.
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/Figure_1.png?raw=true]
 ## Passing Environment Variables Pytgpt **v0.4.6** introduces a convention way
 of taking variables from the environment. To achieve that, set the environment
@@ -185,21 +199,24 @@
 the workload of manually checking a working provider each time you fire up
 pytgpt. ## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot) If you're not
 satisfied with the existing interfaces, [pytgpt-bot](https://github.com/
 Simatwa/pytgpt-bot) could be the solution you're seeking. This bot is designed
 to enhance your experience by offering a wide range of functionalities. Whether
 you're interested in engaging in AI-driven conversations, creating images and
 audio from text, or exploring other innovative features, [pytgpt-bot is
-equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot) For more
-usage info run `$ pytgpt --help` ``` Usage: pytgpt [OPTIONS] COMMAND [ARGS]...
-Options: -v, --version Show the version and exit. -h, --help Show this message
-and exit. Commands: api FastAPI control endpoint awesome Perform CRUD
-operations on awesome-prompts generate Generate a quick response with AI
-gpt4free Discover gpt4free models, providers etc imager Generate images with
-pollinations.ai interactive Chat with AI interactively (Default) utils Utility
-endpoint for pytgpt webchatgpt Reverse Engineered ChatGPT Web-Version ``` ###
-API Health Status | No. | API | Status | |--------|-----|--------| | 1. | [On-
-render](https://python-tgpt.onrender.com) | [cron-job](https://
-pqfzhmvz.status.cron-job.org/) | ## [CHANGELOG](https://github.com/Simatwa/
-python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [x] [tgpt]
-(https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://github.com/
-xtekky/gpt4free)
+equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot) The bot is
+maintained as a separate project so you just have to execute a command get it
+installed : ``` $ pip install pytgpt-bot ``` Usage : `pytgpt bot run ` Or you
+can simply interact with the one running now as [@pytgpt-bot](https://t.me/
+pytgpt_bot) For more usage info run `$ pytgpt --help` ``` Usage: pytgpt
+[OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the version and exit. -
+h, --help Show this message and exit. Commands: api FastAPI control endpoint
+awesome Perform CRUD operations on awesome-prompts bot Telegram bot interface
+control generate Generate a quick response with AI gpt4free Discover gpt4free
+models, providers etc imager Generate images with pollinations.ai interactive
+Chat with AI interactively (Default) utils Utility endpoint for pytgpt
+webchatgpt Reverse Engineered ChatGPT Web-Version ``` ### API Health Status |
+No. | API | Status | |--------|-----|--------| | 1. | [On-render](https://
+python-tgpt.onrender.com) | [cron-job](https://pqfzhmvz.status.cron-job.org/) |
+## [CHANGELOG](https://github.com/Simatwa/python-tgpt/blob/main/docs/
+CHANGELOG.md) ## Acknowledgements 1. [x] [tgpt](https://github.com/aandrew-me/
+tgpt) 2. [x] [gpt4free](https://github.com/xtekky/gpt4free)
```

### Comparing `python_tgpt-0.6.9/setup.py` & `python_tgpt-0.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,26 +9,27 @@
     "requests[socks]==2.31.0",
     "appdirs==1.4.4",
     "pyyaml==6.0.1",
     "webchatgpt==0.3.0",
     "GoogleBard1>=2.1.4",
     "poe-api-wrapper==1.3.6",
     "brotli==1.1.0",
-    "g4f>=0.2.6.1",
+    "g4f>=0.3.0.8",
     "Helpingai_T2-fork==0.3.2",
     "python-vlc>=3.0.20",
+    "httpx==0.27.0",
 ]
 
 cli_reqs = [
     "click==8.1.3",
     "rich==13.3.4",
     "clipman==3.1.0",
     "pyperclip==1.8.2",
     "colorama==0.4.6",
-    "g4f>=0.2.6.1",
+    "g4f>=0.3.0.8",
     "python-dotenv==1.0.0",
 ]
 
 api = [
     "fastapi[all]==0.110.1",
 ]
 
@@ -43,15 +44,15 @@
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="python-tgpt",
-    version="0.6.9",
+    version="0.7.0",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Interact with AI without API key",
     packages=find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `python_tgpt-0.6.9/src/pytgpt/api/__init__.py` & `python_tgpt-0.7.0/src/pytgpt/api/__init__.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.9/src/pytgpt/api/utils.py` & `python_tgpt-0.7.0/src/pytgpt/api/utils.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.9/src/pytgpt/api/v1.py` & `python_tgpt-0.7.0/src/pytgpt/api/v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,61 +5,48 @@
 from pydantic import BaseModel, validator, PositiveInt
 from typing import Union, Any, Generator
 from pytgpt import gpt4free_providers
 from uuid import uuid4
 from .utils import api_exception_handler
 
 # providers
-from pytgpt.leo import LEO
-from pytgpt.opengpt import OPENGPT
-from pytgpt.koboldai import KOBOLDAI
-from pytgpt.phind import PHIND
-from pytgpt.llama2 import LLAMA2
-from pytgpt.blackboxai import BLACKBOXAI
-from pytgpt.perplexity import PERPLEXITY
-from pytgpt.yepchat import YEPCHAT
-from pytgpt.gpt4free import GPT4FREE
-from pytgpt.auto import AUTO
-from pytgpt.imager import Imager
-from pytgpt.imager import Prodia
+from pytgpt.gpt4free import AsyncGPT4FREE
+from pytgpt.auto import AsyncAUTO
+from pytgpt.imager import AsyncImager
+from pytgpt.imager import AsyncProdia
 from pytgpt.utils import Audio
+from pytgpt.async_providers import tgpt_mapper as provider_map
 from pytgpt.utils import api_static_image_dir
 
-provider_map = {
-    "leo": LEO,
-    "opengpt": OPENGPT,
-    "koboldai": KOBOLDAI,
-    "phind": PHIND,
-    "llama2": LLAMA2,
-    "blackboxai": BLACKBOXAI,
-    "perplexity": PERPLEXITY,
-    "yepchat": YEPCHAT,
-    "auto": AUTO,
-}
+provider_map.update({"auto": AsyncAUTO})
 
-image_providers = {"default": Imager, "prodia": Prodia}
+image_providers = {"default": AsyncImager, "prodia": AsyncProdia}
 
 supported_providers = list(provider_map.keys()) + gpt4free_providers
 
 app = APIRouter()
 
 
 class ProvidersModel(BaseModel):
     tgpt: list[str] = list(provider_map.keys())
     g4f: list[str] = gpt4free_providers
 
     model_config = {
         "json_schema_extra": {
             "examples": [
                 {
-                    "tgpt": ["phind", "opengpt", "koboldai"],
+                    "tgpt": [
+                        "phind",
+                        "opengpt",
+                        "koboldai",
+                    ],
                     "g4f": [
                         "Koala",
-                        "FreeGPT",
-                        "You",
+                        "Blackbox",
+                        "FreeChatgpt",
                     ],
                 }
             ]
         }
     }
 
 
@@ -146,15 +133,15 @@
 
 
 class ImagePayload(BaseModel):
     prompt: str
     amount: PositiveInt = 1
     proxy: Union[dict[str, str], None] = None
     timeout: PositiveInt = 30
-    provider: Union[str, None] = None
+    provider: Union[str, None] = "default"
 
     model_config = {
         "json_schema_extra": {
             "examples": [
                 {
                     "prompt": "Sunset view from ISS",
                     "amount": 2,
@@ -184,29 +171,30 @@
                     message=f"Amount {amount} is out of range : 1-10",
                 ),
             )
         return amount
 
     @validator("provider")
     def validate_provider(provider: Union[str, None]) -> str:
-        if provider not in image_providers:
+
+        if provider is not None and not provider in image_providers:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
                 detail=dict(
                     message=f"Image provider '{provider}' is not one of [{', '.join(list(image_providers.keys()))}]",
                 ),
             )
         return "default" if provider is None else provider
 
 
 class ImageBytesPayload(BaseModel):
     prompt: str
     proxy: Union[dict[str, str], None] = None
     timeout: PositiveInt = 30
-    provider: Union[str, None] = None
+    provider: Union[str, None] = "default"
 
     model_config = {
         "json_schema_extra": {
             "examples": [
                 {
                     "prompt": "Alan Walker performing",
                     "proxy": {
@@ -219,15 +207,15 @@
                 {"prompt": "Developed Nairobi in 3050", "proxy": None, "timeout": 30},
             ]
         }
     }
 
     @validator("provider")
     def validate_provider(provider: Union[str, None]) -> str:
-        if provider not in image_providers:
+        if provider is not None and not provider in image_providers:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
                 detail=dict(
                     message=f"Image provider '{provider}' is not one of [{', '.join(list(image_providers.keys()))}]",
                 ),
             )
         return "default" if provider is None else provider
@@ -256,22 +244,22 @@
             ]
         }
     }
 
 
 class TextToAudioPayload(BaseModel):
     message: str
-    voice: Union[str, None] = "Brian"
+    voice: Union[str, None] = "en-US-Wavenet-C"
     proxy: Union[dict[str, str], None] = None
     timeout: int = 30
     model_config = {
         "json_schema_extra": {
             "example": {
                 "message": "There is a place for people like you.",
-                "voice": "Brian",
+                "voice": "en-US-Wavenet-C",
                 "proxy": {
                     "http": "socks4://199.229.254.129:4145",
                     "https": "socks4://199.229.254.129:4145",
                 },
                 "timeout": 30,
             }
         }
@@ -282,15 +270,15 @@
         if not voice in Audio.all_voices:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
                 detail=dict(
                     message=f"Voice '{voice}' is not one of '[{', '.join(Audio.all_voices)}]"
                 ),
             )
-        return "Brian" if not voice else voice
+        return "en-US-Wavenet-C" if not voice else voice
 
 
 class TextToAudioResponse(BaseModel):
     """
     - `url` : Link to generated audio file.
     """
 
@@ -302,15 +290,15 @@
                 "url": "http://localhost:8000/static/audios/f9d4233f-9b78-4d87-bc27-5d2ab928f673.mp3",
             }
         }
     }
 
 
 def init_provider(payload: TextGenerationPayload) -> object:
-    return provider_map.get(payload.provider, GPT4FREE)(
+    return provider_map.get(payload.provider, AsyncAUTO)(
         is_conversation=False,  # payload.is_conversation,
         max_tokens=payload.max_tokens,
         timeout=payload.timeout,
         proxies=payload.proxy,
     )
 
 
@@ -340,31 +328,31 @@
     - `timeout` : Http request timeout.
     - `proxy` : Http request proxy.
 
     *Ensure `proxy` value is correct otherwise make it `null`*
 
     **NOTE** : Example values are modified for illustration purposes.
     """
-    provider_obj: LEO = init_provider(payload)
-    ai_generated_text: str = provider_obj.chat(payload.prompt)
+    provider_obj: AsyncGPT4FREE = init_provider(payload)
+    ai_generated_text: str = await provider_obj.chat(payload.prompt)
     return ProviderResponse(
         provider=(
             provider_obj.provider_name
             if payload.provider == "auto"
             else payload.provider
         ),
         text=ai_generated_text,
         body=provider_obj.last_response if payload.whole else None,
     )
 
 
-def generate_streaming_response(payload: TextGenerationPayload) -> Generator:
-    provider_obj: LEO = init_provider(payload)
-
-    for text in provider_obj.chat(payload.prompt, stream=True):
+async def generate_streaming_response(payload: TextGenerationPayload) -> Generator:
+    provider_obj = init_provider(payload)
+    async_chat = await provider_obj.chat(payload.prompt, stream=True)
+    async for text in async_chat:
         response = ProviderResponse(
             provider=(
                 provider_obj.provider_name
                 if payload.provider == "auto"
                 else payload.provider
             ),
             text=text,
@@ -408,18 +396,18 @@
 
     **NOTE** : *Ensure `proxy` value is correct otherwise make it `null`*
     """
     host = f"{request.url.scheme}://{request.url.netloc}"
     image_gen_obj = image_providers.get(payload.provider)(
         timeout=payload.timeout, proxies=payload.proxy
     )
-    image_generator = image_gen_obj.generate(
+    image_generator = await image_gen_obj.generate(
         prompt=payload.prompt, amount=payload.amount, stream=True
     )
-    image_urls = image_gen_obj.save(
+    image_urls = await image_gen_obj.save(
         image_generator,
         name=uuid4().__str__(),
         dir=api_static_image_dir,
         filenames_prefix=f"{host}/static/images/",
     )
     return ImageResponse(urls=image_urls)
 
@@ -437,15 +425,15 @@
     **Only one image is generated.**
 
     **NOTE** : *Ensure `proxy` value is correct otherwise make it `null`*
     """
     image_gen_obj = image_providers.get(payload.provider)(
         timeout=payload.timeout, proxies=payload.proxy
     )
-    image_list = image_gen_obj.generate(prompt=payload.prompt)
+    image_list = await image_gen_obj.generate(prompt=payload.prompt)
     response = Response(
         image_list[0],
         media_type=f"image/{image_gen_obj.image_extension}",
     )
     response.headers["Content-Disposition"] = (
         f"attachment; filename={payload.prompt[:25]+'...' if len(payload.prompt)>25 else payload.prompt}.{image_gen_obj.image_extension}"
     )
@@ -470,15 +458,15 @@
     **Only one image is generated.**
 
     **NOTE** : *Ensure `proxy` value is correct otherwise make it `null`*
     """
     image_gen_obj = image_providers.get(provider, "default")(
         timeout=timeout, proxies={"https": proxy} if proxy else {}
     )
-    image_list = image_gen_obj.generate(prompt=prompt)
+    image_list = await image_gen_obj.generate(prompt=prompt)
     response = Response(
         image_list[0],
         media_type=f"image/{image_gen_obj.image_extension}",
     )
     response.headers["Content-Disposition"] = (
         f"attachment; filename={prompt[:25]+'...' if len(prompt)>25 else prompt}.{image_gen_obj.image_extension}"
     )
@@ -506,44 +494,44 @@
     - `timeout` : Http request timeout in seconds.
     - `proxy` : Http request proxy.
 
     **NOTE** : *Ensure `proxy` value is correct otherwise make it `null`*
     """
     host = f"{request.url.scheme}://{request.url.netloc}"
     filename = uuid4().__str__() + ".mp3"
-    Audio.text_to_audio(
+    await Audio.async_text_to_audio(
         message=payload.message,
         voice=payload.voice,
         proxies=payload.proxy,
         timeout=payload.timeout,
         save_to=Audio.cache_dir.joinpath(filename).as_posix(),
     )
     return TextToAudioResponse(url=f"{host}/static/audios/" + filename)
 
 
 @app.get("/audio", name="text-to-audio (bytes)")
 @api_exception_handler
 async def text_to_audio_bytes(
     message: str,
-    voice: str = "Brian",
+    voice: str = "en-US-Wavenet-C",
     timeout: int = 30,
     proxy: Union[str, None] = None,
 ):
     """Return raw audio
 
     - `message` : Text to be synthesised.
     - `voice` :  The voice to use for speech synthesis.
     - `timeout` : Http request timeout in seconds.
     - `proxy` : Http request proxy.
 
     **NOTE** : *Ensure `proxy` value is correct otherwise make it `null`*
     """
-    image_bytes = Audio.text_to_audio(
+    image_bytes = await Audio.async_text_to_audio(
         message=message,
-        voice=voice if voice in Audio.all_voices else "Brian",
+        voice=voice if voice in Audio.all_voices else "en-US-Wavenet-C",
         proxies={"https": proxy} if proxy else {},
         timeout=timeout,
     )
     return Response(
         content=image_bytes,
         media_type="audio/mpeg",
         headers={
```

### Comparing `python_tgpt-0.6.9/src/pytgpt/auto/main.py` & `python_tgpt-0.7.0/src/pytgpt/perplexity/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,225 +1,212 @@
-from pytgpt.opengpt import OPENGPT
-from pytgpt.koboldai import KOBOLDAI
-from pytgpt.phind import PHIND
-from pytgpt.llama2 import LLAMA2
-from pytgpt.blackboxai import BLACKBOXAI
-from pytgpt.perplexity import PERPLEXITY
-from pytgpt.gpt4free import GPT4FREE
-from pytgpt.gpt4free.utils import TestProviders
-from .errors import AllProvidersFailure
-
-from typing import Union
+import json
+import yaml
+import requests
+from pytgpt.utils import Optimizers
+from pytgpt.utils import Conversation
+from pytgpt.utils import AwesomePrompts
+from pytgpt.base import Provider
+from Helpingai_T2 import Perplexity
 from typing import Any
-import logging
-
 
-provider_map: dict[
-    str, Union[OPENGPT, KOBOLDAI, PHIND, LLAMA2, BLACKBOXAI, PERPLEXITY, GPT4FREE]
-] = {
-    "phind": PHIND,
-    "perplexity": PERPLEXITY,
-    "opengpt": OPENGPT,
-    "koboldai": KOBOLDAI,
-    "llama2": LLAMA2,
-    "blackboxai": BLACKBOXAI,
-    "gpt4free": GPT4FREE,
-}
+session = requests.Session()
 
 
-class AUTO:
+class PERPLEXITY(Provider):
     def __init__(
         self,
         is_conversation: bool = True,
         max_tokens: int = 600,
         timeout: int = 30,
         intro: str = None,
         filepath: str = None,
         update_file: bool = True,
         proxies: dict = {},
         history_offset: int = 10250,
         act: str = None,
+        quiet: bool = False,
     ):
-        """Instantiates AUTO
+        """Instantiates PERPLEXITY
 
         Args:
             is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True
             max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
             timeout (int, optional): Http request timeout. Defaults to 30.
             intro (str, optional): Conversation introductory prompt. Defaults to None.
             filepath (str, optional): Path to file containing conversation history. Defaults to None.
             update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
             proxies (dict, optional): Http request proxies. Defaults to {}.
             history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
             act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+            quiet (bool, optional): Ignore web search-results and yield final response only. Defaults to False.
         """
-        self.provider: Union[
-            OPENGPT, KOBOLDAI, PHIND, LLAMA2, BLACKBOXAI, PERPLEXITY, GPT4FREE
-        ] = None
-        self.provider_name: str = None
+        self.max_tokens_to_sample = max_tokens
         self.is_conversation = is_conversation
-        self.max_tokens = max_tokens
-        self.timeout = timeout
-        self.intro = intro
-        self.filepath = filepath
-        self.update_file = update_file
-        self.proxies = proxies
-        self.history_offset = history_offset
-        self.act = act
-
-    @property
-    def last_response(self) -> dict[str, Any]:
-        return self.provider.last_response
-
-    @property
-    def conversation(self) -> object:
-        return self.provider.conversation
+        self.last_response = {}
+        self.web_results: dict = {}
+        self.quiet = quiet
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
 
     def ask(
         self,
         prompt: str,
         stream: bool = False,
         raw: bool = False,
         optimizer: str = None,
         conversationally: bool = False,
-        run_new_test: bool = False,
     ) -> dict:
         """Chat with AI
 
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            raw (bool, optional): Stream back raw response as received. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-            run_new_test (bool, optional): Perform new test on g4f-based providers. Defaults to False.
-        Returns:
-           dict : {}
-        """
-        ask_kwargs: dict[str, Union[str, bool]] = {
-            "prompt": prompt,
-            "stream": stream,
-            "raw": raw,
-            "optimizer": optimizer,
-            "conversationally": conversationally,
+                Args:
+                    prompt (str): Prompt to be send.
+                    stream (bool, optional): Flag for streaming response. Defaults to False.
+                    raw (bool, optional): Stream back raw response as received. Defaults to False.
+                    optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+                    conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+                Returns:
+                   dict : {}
+                ```json
+        {
+            "status": "pending",
+            "uuid": "3604dfcc-611f-4b7d-989d-edca2a7233c7",
+            "read_write_token": null,
+            "frontend_context_uuid": "f6d43119-5231-481d-b692-f52e1f52d2c6",
+            "final": false,
+            "backend_uuid": "a6d6ec9e-da69-4841-af74-0de0409267a8",
+            "media_items": [],
+            "widget_data": [],
+            "knowledge_cards": [],
+            "expect_search_results": "false",
+            "mode": "concise",
+            "search_focus": "internet",
+            "gpt4": false,
+            "display_model": "turbo",
+            "attachments": null,
+            "answer": "",
+            "web_results": [],
+            "chunks": [],
+            "extra_web_results": []
         }
-
-        # tgpt-based providers
-        for provider_name, provider_obj in provider_map.items():
-            # continue
-            try:
-                self.provider_name = f"tgpt-{provider_name}"
-                self.provider = provider_obj(
-                    is_conversation=self.is_conversation,
-                    max_tokens=self.max_tokens,
-                    timeout=self.timeout,
-                    intro=self.intro,
-                    filepath=self.filepath,
-                    update_file=self.update_file,
-                    proxies=self.proxies,
-                    history_offset=self.history_offset,
-                    act=self.act,
+                ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
                 )
-
-                def for_stream():
-                    for chunk in self.provider.ask(**ask_kwargs):
-                        yield chunk
-
-                def for_non_stream():
-                    return self.provider.ask(**ask_kwargs)
-
-                return for_stream() if stream else for_non_stream()
-
-            except Exception as e:
-                logging.debug(
-                    f"Failed to generate response using provider {provider_name} - {e}"
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
                 )
 
-        # g4f-based providers
+        def for_stream():
+            for response in Perplexity().generate_answer(conversation_prompt):
+                yield json.dumps(response) if raw else response
+                self.last_response.update(response)
 
-        for provider_info in TestProviders(timeout=self.timeout).get_results(
-            run=run_new_test
-        ):
-            try:
-                self.provider_name = f"g4f-{provider_info['name']}"
-                self.provider = GPT4FREE(
-                    provider=provider_info["name"],
-                    is_conversation=self.is_conversation,
-                    max_tokens=self.max_tokens,
-                    intro=self.intro,
-                    filepath=self.filepath,
-                    update_file=self.update_file,
-                    proxies=self.proxies,
-                    history_offset=self.history_offset,
-                    act=self.act,
-                )
+            self.conversation.update_chat_history(
+                prompt,
+                self.get_message(self.last_response),
+            )
 
-                def for_stream():
-                    for chunk in self.provider.ask(**ask_kwargs):
-                        yield chunk
-
-                def for_non_stream():
-                    return self.provider.ask(**ask_kwargs)
-
-                return for_stream() if stream else for_non_stream()
-
-            except Exception as e:
-                logging.debug(
-                    f"Failed to generate response using GPT4FREE-base provider {provider_name} - {e}"
-                )
+        def for_non_stream():
+            for _ in for_stream():
+                pass
+            return self.last_response
 
-        raise AllProvidersFailure(
-            "None of the providers generated response successfully."
-        )
+        return for_stream() if stream else for_non_stream()
 
     def chat(
         self,
         prompt: str,
         stream: bool = False,
         optimizer: str = None,
         conversationally: bool = False,
-        run_new_test: bool = False,
     ) -> str:
         """Generate response `str`
         Args:
             prompt (str): Prompt to be send.
             stream (bool, optional): Flag for streaming response. Defaults to False.
             optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
             conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-            run_new_test (bool, optional): Perform new test on g4f-based providers. Defaults to False.
         Returns:
             str: Response generated
         """
 
         def for_stream():
             for response in self.ask(
-                prompt,
-                True,
-                optimizer=optimizer,
-                conversationally=conversationally,
-                run_new_test=run_new_test,
+                prompt, True, optimizer=optimizer, conversationally=conversationally
             ):
                 yield self.get_message(response)
 
         def for_non_stream():
-            ask_response = self.ask(
-                prompt,
-                False,
-                optimizer=optimizer,
-                conversationally=conversationally,
-                run_new_test=run_new_test,
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
             )
-            return self.get_message(ask_response)
 
         return for_stream() if stream else for_non_stream()
 
     def get_message(self, response: dict) -> str:
         """Retrieves message only from response
 
         Args:
             response (dict): Response generated by `self.ask`
 
         Returns:
             str: Message extracted
         """
-        assert self.provider is not None, "Chat with AI first"
-        return self.provider.get_message(response)
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        text_str: str = response.get("answer", "")
+
+        def update_web_results(web_results: list) -> None:
+            for index, results in enumerate(web_results, start=1):
+                self.web_results[str(index) + ". " + results["name"]] = dict(
+                    url=results.get("url"), snippet=results.get("snippet")
+                )
+
+        if response.get("text"):
+            # last chunk
+            target: dict[str, Any] = json.loads(response.get("text"))
+            text_str = target.get("answer")
+            web_results: list[dict] = target.get("web_results")
+            self.web_results.clear()
+            update_web_results(web_results)
+
+            return (
+                text_str
+                if self.quiet or not self.web_results
+                else text_str + "\n\n# WEB-RESULTS\n\n" + yaml.dump(self.web_results)
+            )
+
+        else:
+            if str(response.get("expect_search_results")).lower() == "true":
+                return (
+                    text_str
+                    if self.quiet
+                    else text_str
+                    + "\n\n# WEB-RESULTS\n\n"
+                    + yaml.dump(response.get("web_results"))
+                )
+            else:
+                return text_str
```

### Comparing `python_tgpt-0.6.9/src/pytgpt/base.py` & `python_tgpt-0.7.0/src/pytgpt/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC
 from abc import abstractmethod
 
 
 class Provider(ABC):
-    """Base class for models class"""
+    """Base class for providers"""
 
     @abstractmethod
     def ask(
         self,
         prompt: str,
         stream: bool = False,
         raw: bool = False,
@@ -63,8 +63,76 @@
 
         Args:
             response (dict): Response generated by `self.ask`
 
         Returns:
             str: Message extracted
         """
+        raise NotImplementedError("Method needs to be implemented in subclass")
+
+
+class AsyncProvider(ABC):
+    """Asynchronous base class for providers"""
+
+    @abstractmethod
+    async def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Asynchronously chat with AI
+
+        Args:
+            prompt (str): Prompt to be sent
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict : {}
+        ```json
+        {
+            "completion": "\nNext: domestic cat breeds with short hair >>",
+            "stop_reason": null,
+            "truncated": false,
+            "stop": null,
+            "model": "llama-2-13b-chat",
+            "log_id": "cmpl-3kYiYxSNDvgMShSzFooz6t",
+            "exception": null
+        }
+        ```
+        """
+        raise NotImplementedError("Method needs to be implemented in subclass")
+
+    @abstractmethod
+    async def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Asynchronously generate response `str`
+        Args:
+            prompt (str): Prompt to be sent
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+        raise NotImplementedError("Method needs to be implemented in subclass")
+
+    @abstractmethod
+    async def get_message(self, response: dict) -> str:
+        """Asynchronously retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
         raise NotImplementedError("Method needs to be implemented in subclass")
```

### Comparing `python_tgpt-0.6.9/src/pytgpt/blackboxai/main.py` & `python_tgpt-0.7.0/src/pytgpt/poe/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,170 +1,165 @@
-import re
-import json
-import requests
-from pytgpt.utils import Optimizers
+from poe_api_wrapper import PoeApi
+from poe_api_wrapper.api import BOTS_LIST
+from pytgpt.base import Provider
 from pytgpt.utils import Conversation
+from pytgpt.utils import Optimizers
 from pytgpt.utils import AwesomePrompts
+from pathlib import Path
+from json import loads
+from json import dumps
+from loguru import logger
+import logging
 
-session = requests.Session()
+logger.remove()
 
-default_model = None
+default_model = "Assistant"
 
 
-class BLACKBOXAI:
+class POE(Provider):
     def __init__(
         self,
-        is_conversation: bool = True,
-        max_tokens: int = 600,
+        cookie: str,
+        model: str = default_model,
+        proxy: bool = False,
         timeout: int = 30,
-        intro: str = None,
         filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
+        update_file: str = True,
+        intro: str = None,
         act: str = None,
-        model: str = default_model,
+        init: bool = True,
     ):
-        """Instantiates BLACKBOXAI
+        """Initializes POE
 
         Args:
-            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            cookie (str): Path to `poe.com.cookies.json` file or 'p-b' cookie-value.
+            model (str, optional): Model name. Default to Assistant.
+            proxy (bool, optional): Flag for Httpx request proxy. Defaults to False.
             timeout (int, optional): Http request timeout. Defaults to 30.
+            filepath (str, optional): Path to save the chat history. Defaults to None.
+            update_file (str, optional): Flag for controlling chat history updates. Defaults to True.
             intro (str, optional): Conversation introductory prompt. Defaults to None.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional): Http request proxies. Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
             act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-            model (str, optional): Model name. Defaults to "Phind Model".
+            init (bool, optional): Resend the intro prompt. Defaults to True.
         """
-        self.max_tokens_to_sample = max_tokens
-        self.is_conversation = is_conversation
-        self.chat_endpoint = "https://www.blackbox.ai/api/chat"
-        self.stream_chunk_size = 64
-        self.timeout = timeout
-        self.last_response = {}
-        self.model = model
-        self.previewToken: str = None
-        self.userId: str = ""
-        self.codeModelMode: bool = True
-        self.id: str = ""
-        self.agentMode: dict = {}
-        self.trendingAgentMode: dict = {}
-        self.isMicMode: bool = False
-
-        self.headers = {
-            "Content-Type": "application/json",
-            "User-Agent": "",
-            "Accept": "*/*",
-            "Accept-Encoding": "Identity",
-        }
+        assert isinstance(
+            cookie, str
+        ), f"Cookie must be of {str} datatype only not {type(cookie)}"
+        assert (
+            model in BOTS_LIST.keys()
+        ), f"model name '{model}' is not one of {', '.join(list(BOTS_LIST.keys()))}"
+        cookie_path = Path(cookie)
+
+        if cookie_path.exists() or any(["/" in cookie, ".json" in cookie]):
+            cookie = None
+            all_cookies = loads(cookie_path.read_text())
+            for entry in all_cookies:
+                if entry["name"] == "p-b":
+                    cookie = entry["value"]
+            assert (
+                cookie
+            ), f'Required cookie value cannot be retrieved from the path  "{cookie_path.as_posix()}"'
+
+        if proxy:
+            import poe_api_wrapper.proxies as proxies
+
+            proxies.PROXY = True
 
+        self.bot = BOTS_LIST[model]
+        self.session = PoeApi(cookie)
+        self.last_response = {}
         self.__available_optimizers = (
             method
             for method in dir(Optimizers)
             if callable(getattr(Optimizers, method)) and not method.startswith("__")
         )
-        session.headers.update(self.headers)
         Conversation.intro = (
             AwesomePrompts().get_act(
                 act, raise_not_found=True, default=None, case_insensitive=True
             )
             if act
             else intro or Conversation.intro
         )
         self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
+            status=False, filepath=filepath, update_file=update_file
         )
-        self.conversation.history_offset = history_offset
-        session.proxies = proxies
+        if init:
+            self.ask(self.conversation.intro)  # Init
 
     def ask(
         self,
         prompt: str,
         stream: bool = False,
         raw: bool = False,
         optimizer: str = None,
         conversationally: bool = False,
     ) -> dict:
         """Chat with AI
 
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            raw (bool, optional): Stream back raw response as received. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-           dict : {}
+            Args:
+                prompt (str): Prompt to be send.
+                stream (bool, optional): Flag for streaming response. Defaults to False.
+                raw (bool, optional): Stream back raw response as received. Defaults to False.
+                optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defeaults to None
+                conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+            Returns:
+               dict : {}
         ```json
         {
-           "text" : "print('How may I help you today?')"
+            "id": "TWVzc2FnZToxMTU0MzgyNDQ1ODU=",
+            "messageId": 115438244585,
+            "creationTime": 1707777376544407,
+            "clientNonce": null,
+            "state": "complete",
+            "text": "Hello! How can I assist you today?",
+            "author": "capybara",
+            "contentType": "text_markdown",
+            "sourceType": "chat_input",
+            "attachmentTruncationState": "not_truncated",
+            "attachments": [],
+            "vote": null,
+            "suggestedReplies": [],
+            "hasCitations": false,
+            "__isNode": "Message",
+            "textLengthOnCancellation": null,
+            "chatCode": "21a2jn0yrq9phxiy478",
+            "chatId": 328236777,
+            "title": null,
+            "response": ""
         }
         ```
         """
         conversation_prompt = self.conversation.gen_complete_prompt(prompt)
         if optimizer:
             if optimizer in self.__available_optimizers:
                 conversation_prompt = getattr(Optimizers, optimizer)(
                     conversation_prompt if conversationally else prompt
                 )
             else:
                 raise Exception(
                     f"Optimizer is not one of {self.__available_optimizers}"
                 )
 
-        session.headers.update(self.headers)
-        payload = {
-            "messages": [
-                # json.loads(prev_messages),
-                {"content": conversation_prompt, "role": "user"}
-            ],
-            "id": self.id,
-            "previewToken": self.previewToken,
-            "userId": self.userId,
-            "codeModelMode": self.codeModelMode,
-            "agentMode": self.agentMode,
-            "trendingAgentMode": self.trendingAgentMode,
-            "isMicMode": self.isMicMode,
-        }
-
         def for_stream():
-            response = session.post(
-                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
-            )
-            if (
-                not response.ok
-                or not response.headers.get("Content-Type")
-                == "text/plain; charset=utf-8"
-            ):
-                raise Exception(
-                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
-                )
-            streaming_text = ""
-            for value in response.iter_lines(
-                decode_unicode=True,
-                chunk_size=self.stream_chunk_size,
-                delimiter="\n",
-            ):
-                try:
-                    if bool(value):
-                        streaming_text += value + ("\n" if stream else "")
-
-                        resp = dict(text=streaming_text)
-                        self.last_response.update(resp)
-                        yield value if raw else resp
-                except json.decoder.JSONDecodeError:
-                    pass
+            for response in self.session.send_message(self.bot, conversation_prompt):
+                if raw:
+                    yield dumps(response)
+                else:
+                    yield response
+
+                self.last_response.update(response)
+
             self.conversation.update_chat_history(
-                prompt, self.get_message(self.last_response)
+                prompt,
+                self.get_message(self.last_response),
+                force=True,
             )
 
         def for_non_stream():
+            # let's make use of stream
             for _ in for_stream():
                 pass
             return self.last_response
 
         return for_stream() if stream else for_non_stream()
 
     def chat(
```

### Comparing `python_tgpt-0.6.9/src/pytgpt/console.py` & `python_tgpt-0.7.0/src/pytgpt/console.py`

 * *Files 0% similar despite different names*

```diff
@@ -1262,14 +1262,21 @@
     @staticmethod
     @tgpt2_.group()
     @click.help_option("-h", "--help")
     def api():
         """FastAPI control endpoint"""
         pass
 
+    @staticmethod
+    @tgpt2_.group()
+    @click.help_option("-h", "--help")
+    def bot():
+        """Telegram bot interface control"""
+        pass
+
 
 class ChatInteractive:
     """Interactive command"""
 
     @staticmethod
     @click.command(context_settings=this.context_settings)
     @click.option(
@@ -2597,14 +2604,21 @@
 
     # Image generator
     EntryGroup.tgpt2_.add_command(ImageGen.generate_image, "imager")
 
     # FastAPI
     EntryGroup.api.add_command(API.run)
     EntryGroup.api.add_command(API.clear)
+    try:
+        import pytgpt_bot.cli as bot
+
+        EntryGroup.bot.add_command(bot.run)
+        EntryGroup.bot.add_command(bot.clear)
+    except ImportError:
+        pass
 
 
 # @this.handle_exception
 def main(*args):
     """Fireup console programmically"""
     sys.argv += list(args)
     args = sys.argv
```

### Comparing `python_tgpt-0.6.9/src/pytgpt/gemini/main.py` & `python_tgpt-0.7.0/src/pytgpt/gemini/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 from pytgpt.utils import Optimizers
 from os import path
 from json import load
 from json import dumps
 import warnings
 import logging
 
-logging.getLogger("httpx").setLevel(logging.ERROR)
-
 warnings.simplefilter("ignore", category=UserWarning)
 
 
 class GEMINI(Provider):
     def __init__(
         self,
         cookie_file: str,
```

### Comparing `python_tgpt-0.6.9/src/pytgpt/gpt4all/main.py` & `python_tgpt-0.7.0/src/pytgpt/gpt4all/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.9/src/pytgpt/gpt4free/main.py` & `python_tgpt-0.7.0/src/pytgpt/webchatgpt/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,209 +1,149 @@
-from pytgpt.utils import Optimizers
+from WebChatGPT import ChatGPT
+from WebChatGPT.utils import get_message
+from pytgpt.base import Provider
 from pytgpt.utils import Conversation
+from pytgpt.utils import Optimizers
 from pytgpt.utils import AwesomePrompts
-from pytgpt.base import Provider
-from pytgpt import available_providers
-import g4f
-
-g4f.debug.version_check = False
-
-working_providers = available_providers
-
-completion_allowed_models = [
-    "code-davinci-002",
-    "text-ada-001",
-    "text-babbage-001",
-    "text-curie-001",
-    "text-davinci-002",
-    "text-davinci-003",
-]
-
-default_models = {
-    "completion": "text-davinci-003",
-    "chat_completion": "gpt-3.5-turbo",
-}
 
-default_provider = "Koala"
+default_model = "text-davinci-002-render-sha"
 
 
-class GPT4FREE(Provider):
+class WEBCHATGPT(Provider):
     def __init__(
         self,
-        provider: str = default_provider,
-        is_conversation: bool = True,
-        auth: str = None,
-        max_tokens: int = 600,
-        model: str = None,
-        chat_completion: bool = False,
-        ignore_working: bool = False,
+        cookie_file: str,
+        model: str = default_model,
+        proxy: dict = {},
         timeout: int = 30,
-        intro: str = None,
         filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
+        update_file: str = True,
+        intro: str = None,
         act: str = None,
     ):
-        """Initialies GPT4FREE
+        """Initializes WEBCHATGPT
 
         Args:
-            provider (str, optional): gpt4free based provider name. Defaults to Koala.
-            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
-            auth (str, optional): Authentication value for the provider incase it needs. Defaults to None.
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            model (str, optional): LLM model name. Defaults to text-davinci-003|gpt-3.5-turbo.
-            chat_completion(bool, optional): Provide native auto-contexting (conversationally). Defaults to False.
-            ignore_working (bool, optional): Ignore working status of the provider. Defaults to False.
+            cookie_file (str): Path to `chat.openai.com.cookies.json` file
+            model (str, optional): Modl name. Default to text-davinci-002-render-sha.
+            proxy (dict, optional): Http request proxy. Defaults to {}.
             timeout (int, optional): Http request timeout. Defaults to 30.
+            filepath (str, optional): Path to save the chat history. Defaults to None.
+            update_file (str, optional): Flag for controlling chat history updates. Defaults to True.
             intro (str, optional): Conversation introductory prompt. Defaults to None.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional): Http request proxies. Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
             act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
         """
-        assert provider in available_providers, (
-            f"Provider '{provider}' is not yet supported. "
-            f"Try others like {', '.join(available_providers)}"
-        )
-        if model is None:
-            model = (
-                default_models["chat_completion"]
-                if chat_completion
-                else default_models["completion"]
-            )
-
-        elif not chat_completion:
-            assert model in completion_allowed_models, (
-                f"Model '{model}' is not yet supported for completion. "
-                f"Try other models like {', '.join(completion_allowed_models)}"
-            )
-        self.is_conversation = is_conversation
-        self.max_tokens_to_sample = max_tokens
-        self.stream_chunk_size = 64
-        self.timeout = timeout
+        self.session = ChatGPT(cookie_path=cookie_file, model=model, timeout=timeout)
+        self.session.session.proxies = proxy
         self.last_response = {}
-
         self.__available_optimizers = (
             method
             for method in dir(Optimizers)
             if callable(getattr(Optimizers, method)) and not method.startswith("__")
         )
         Conversation.intro = (
             AwesomePrompts().get_act(
                 act, raise_not_found=True, default=None, case_insensitive=True
             )
             if act
             else intro or Conversation.intro
         )
         self.conversation = Conversation(
-            False if chat_completion else is_conversation,
-            self.max_tokens_to_sample,
-            filepath,
-            update_file,
+            status=False, filepath=filepath, update_file=update_file
         )
-        self.conversation.history_offset = history_offset
-        self.model = model
-        self.provider = provider
-        self.chat_completion = chat_completion
-        self.ignore_working = ignore_working
-        self.auth = auth
-        self.proxy = None if not proxies else list(proxies.values())[0]
-        self.__chat_class = g4f.ChatCompletion if chat_completion else g4f.Completion
-
-    def __str__(self):
-        return f"GPTFREE(provider={self.provider})"
 
     def ask(
         self,
         prompt: str,
         stream: bool = False,
         raw: bool = False,
         optimizer: str = None,
         conversationally: bool = False,
     ) -> dict:
         """Chat with AI
 
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            raw (bool, optional): Stream back raw response as received. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-           dict : {}
+            Args:
+                prompt (str): Prompt to be send.
+                stream (bool, optional): Flag for streaming response. Defaults to False.
+                raw (bool, optional): Stream back raw response as received. Defaults to False.
+                optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defeaults to None
+                conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+            Returns:
+               dict : {}
         ```json
         {
-          "text" : "How may I help you today?"
+            "message": {
+                "id": "2c98d9ff-495c-4f08-af9e-affbd17xxxxx",
+                "author": {
+                    "role": "assistant",
+                    "name": null,
+                    "metadata": {}
+                },
+                "create_time": 1702666802.823688,
+                "update_time": null,
+                "content": {
+                    "content_type": "text",
+                    "parts": [
+                        "Of course, your privacy matters! I don't store or remember our conversations once they're completed, so your information is kept confidential. If there's anything specific you'd like to discuss or if you have any concerns, feel free to let me know. I'm here to assist you!"
+                    ]
+                },
+                "status": "finished_successfully",
+                "end_turn": true,
+                "weight": 1.0,
+                "metadata": {
+                    "finish_details": {
+                        "type": "stop",
+                        "stop_tokens": [
+                            100260
+                        ]
+                    },
+                    "inline_gizmo_id": null,
+                    "is_complete": true,
+                    "message_type": "next",
+                    "model_slug": "text-davinci-002-render-sha",
+                    "parent_id": "7bf27013-a47a-438c-ae17-0ee846b4xxxx",
+                    "timestamp_": "absolute"
+                },
+                "recipient": "all"
+            },
+            "conversation_id": "affdda8c-588c-4342-9869-26c5bd7xxxxx",
+            "error": null
         }
         ```
         """
         conversation_prompt = self.conversation.gen_complete_prompt(prompt)
         if optimizer:
             if optimizer in self.__available_optimizers:
                 conversation_prompt = getattr(Optimizers, optimizer)(
                     conversation_prompt if conversationally else prompt
                 )
             else:
                 raise Exception(
                     f"Optimizer is not one of {self.__available_optimizers}"
                 )
 
-        def payload():
-            if self.chat_completion:
-                return dict(
-                    model=self.model,
-                    provider=self.provider,  # g4f.Provider.Aichat,
-                    messages=[{"role": "user", "content": conversation_prompt}],
-                    stream=stream,
-                    ignore_working=self.ignore_working,
-                    auth=self.auth,
-                    proxy=self.proxy,
-                    timeout=self.timeout,
-                )
-
-            else:
-                return dict(
-                    model=self.model,
-                    prompt=conversation_prompt,
-                    provider=self.provider,
-                    stream=stream,
-                    ignore_working=self.ignore_working,
-                    auth=self.auth,
-                    proxy=self.proxy,
-                    timeout=self.timeout,
-                )
-
-        def format_response(response):
-            return dict(text=response)
-
         def for_stream():
-            previous_chunks = ""
-            response = self.__chat_class.create(**payload())
-
-            for chunk in response:
-                previous_chunks += chunk
-                formatted_resp = format_response(previous_chunks)
-                self.last_response.update(formatted_resp)
-                yield previous_chunks if raw else formatted_resp
+            for response in self.session.ask(prompt, stream=True, raw_response=raw):
+                if raw:
+                    yield response
+                else:
+                    self.last_response.update(response)
+                    yield response
 
             self.conversation.update_chat_history(
                 prompt,
-                previous_chunks,
+                self.get_message(self.last_response),
+                force=True,
             )
 
         def for_non_stream():
-            response = self.__chat_class.create(**payload())
-            formatted_resp = format_response(response)
-
-            self.last_response.update(formatted_resp)
-            self.conversation.update_chat_history(prompt, response)
-
-            return response if raw else formatted_resp
+            # let's make use of stream
+            for _ in for_stream():
+                pass
+            return self.last_response
 
         return for_stream() if stream else for_non_stream()
 
     def chat(
         self,
         prompt: str,
         stream: bool = False,
@@ -244,8 +184,8 @@
         Args:
             response (dict): Response generated by `self.ask`
 
         Returns:
             str: Message extracted
         """
         assert isinstance(response, dict), "Response should be of dict data-type only"
-        return response["text"]
+        return get_message(response)
```

### Comparing `python_tgpt-0.6.9/src/pytgpt/gpt4free/utils.py` & `python_tgpt-0.7.0/src/pytgpt/gpt4free/utils.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.9/src/pytgpt/groq/main.py` & `python_tgpt-0.7.0/src/pytgpt/koboldai/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,64 @@
 import requests
 import json
+import httpx
+import pytgpt.exceptions as exceptions
 from pytgpt.utils import Optimizers
 from pytgpt.utils import Conversation
 from pytgpt.utils import AwesomePrompts
-from pytgpt.base import Provider
+from pytgpt.utils import sanitize_stream
+from pytgpt.base import Provider, AsyncProvider
+from typing import AsyncGenerator
 
 session = requests.Session()
 
-model = "mixtral-8x7b-32768"
 
-
-class GROQ(Provider):
+class KOBOLDAI(Provider):
     def __init__(
         self,
-        api_key: str,
         is_conversation: bool = True,
         max_tokens: int = 600,
         temperature: float = 1,
-        presence_penalty: int = 0,
-        frequency_penalty: int = 0,
         top_p: float = 1,
-        model: str = model,
         timeout: int = 30,
         intro: str = None,
         filepath: str = None,
         update_file: bool = True,
         proxies: dict = {},
         history_offset: int = 10250,
         act: str = None,
     ):
-        """Instantiates GROQ
+        """Instantiate TGPT
 
         Args:
-            api_key (key): GROQ's API key.
-            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
+            is_conversation (str, optional): Flag for chatting conversationally. Defaults to True.
             max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            temperature (float, optional): Charge of the generated text's randomness. Defaults to 1.
-            presence_penalty (int, optional): Chances of topic being repeated. Defaults to 0.
-            frequency_penalty (int, optional): Chances of word being repeated. Defaults to 0.
+            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.2.
             top_p (float, optional): Sampling threshold during inference time. Defaults to 0.999.
-            model (str, optional): LLM model name. Defaults to "gpt-3.5-turbo".
-            timeout (int, optional): Http request timeout. Defaults to 30.
-            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            timeout (int, optional): Http requesting timeout. Defaults to 30
+            intro (str, optional): Conversation introductory prompt. Defaults to `Conversation.intro`.
             filepath (str, optional): Path to file containing conversation history. Defaults to None.
             update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional): Http request proxies. Defaults to {}.
+            proxies (dict, optional) : Http reqiuest proxies (socks). Defaults to {}.
             history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
             act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
         """
         self.is_conversation = is_conversation
         self.max_tokens_to_sample = max_tokens
-        self.api_key = api_key
-        self.model = model
         self.temperature = temperature
-        self.presence_penalty = presence_penalty
-        self.frequency_penalty = frequency_penalty
         self.top_p = top_p
-        self.chat_endpoint = "https://api.groq.com/openai/v1/chat/completions"
+        self.chat_endpoint = (
+            "https://koboldai-koboldcpp-tiefighter.hf.space/api/extra/generate/stream"
+        )
         self.stream_chunk_size = 64
         self.timeout = timeout
         self.last_response = {}
         self.headers = {
             "Content-Type": "application/json",
-            "Authorization": f"Bearer {self.api_key}",
+            "Accept": "application/json",
         }
 
         self.__available_optimizers = (
             method
             for method in dir(Optimizers)
             if callable(getattr(Optimizers, method)) and not method.startswith("__")
         )
@@ -90,117 +82,78 @@
         stream: bool = False,
         raw: bool = False,
         optimizer: str = None,
         conversationally: bool = False,
     ) -> dict:
         """Chat with AI
 
-                Args:
-                    prompt (str): Prompt to be send.
-                    stream (bool, optional): Flag for streaming response. Defaults to False.
-                    raw (bool, optional): Stream back raw response as received. Defaults to False.
-                    optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-                    conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-                Returns:
-                   dict : {}
-                ```json
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict : {}
+        ```json
         {
-            "id": "c0c8d139-d2b9-9909-8aa1-14948bc28404",
-            "object": "chat.completion",
-            "created": 1710852779,
-            "model": "mixtral-8x7b-32768",
-            "choices": [
-                {
-                    "index": 0,
-                    "message": {
-                        "role": "assistant",
-                        "content": "Hello! How can I assist you today? I'm here to help answer your questions and engage in conversation on a wide variety of topics. Feel free to ask me anything!"
-                    },
-                    "logprobs": null,
-                    "finish_reason": "stop"
-                }
-            ],
-            "usage": {
-                "prompt_tokens": 47,
-                "prompt_time": 0.03,
-                "completion_tokens": 37,
-                "completion_time": 0.069,
-                "total_tokens": 84,
-                "total_time": 0.099
-            },
-            "system_fingerprint": null
+           "token" : "How may I assist you today?"
         }
-                ```
+        ```
         """
         conversation_prompt = self.conversation.gen_complete_prompt(prompt)
         if optimizer:
             if optimizer in self.__available_optimizers:
                 conversation_prompt = getattr(Optimizers, optimizer)(
                     conversation_prompt if conversationally else prompt
                 )
             else:
                 raise Exception(
                     f"Optimizer is not one of {self.__available_optimizers}"
                 )
+
         session.headers.update(self.headers)
         payload = {
-            "frequency_penalty": self.frequency_penalty,
-            "messages": [{"content": conversation_prompt, "role": "user"}],
-            "model": self.model,
-            "presence_penalty": self.presence_penalty,
-            "stream": stream,
+            "prompt": conversation_prompt,
             "temperature": self.temperature,
             "top_p": self.top_p,
         }
 
         def for_stream():
             response = session.post(
                 self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
             )
             if not response.ok:
-                raise Exception(
-                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                raise exceptions.FailedToGenerateResponseError(
+                    f"Failed to generate response - ({response.status_code}, {response.reason})"
                 )
 
             message_load = ""
             for value in response.iter_lines(
                 decode_unicode=True,
-                delimiter="" if raw else "data:",
+                delimiter="" if raw else "event: message\ndata:",
                 chunk_size=self.stream_chunk_size,
             ):
                 try:
                     resp = json.loads(value)
-                    incomplete_message = self.get_message(resp)
-                    if incomplete_message:
-                        message_load += incomplete_message
-                        resp["choices"][0]["delta"]["content"] = message_load
-                        self.last_response.update(resp)
-                        yield value if raw else resp
-                    elif raw:
-                        yield value
+                    message_load += self.get_message(resp)
+                    resp["token"] = message_load
+                    self.last_response.update(resp)
+                    yield value if raw else resp
                 except json.decoder.JSONDecodeError:
                     pass
             self.conversation.update_chat_history(
                 prompt, self.get_message(self.last_response)
             )
 
         def for_non_stream():
-            response = session.post(
-                self.chat_endpoint, json=payload, stream=False, timeout=self.timeout
-            )
-            if not response.ok:
-                raise Exception(
-                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
-                )
-            resp = response.json()
-            self.last_response.update(resp)
-            self.conversation.update_chat_history(
-                prompt, self.get_message(self.last_response)
-            )
-            return resp
+            # let's make use of stream
+            for _ in for_stream():
+                pass
+            return self.last_response
 
         return for_stream() if stream else for_non_stream()
 
     def chat(
         self,
         prompt: str,
         stream: bool = False,
@@ -241,22 +194,214 @@
         Args:
             response (dict): Response generated by `self.ask`
 
         Returns:
             str: Message extracted
         """
         assert isinstance(response, dict), "Response should be of dict data-type only"
-        try:
-            if response["choices"][0].get("delta"):
-                return response["choices"][0]["delta"]["content"]
-            return response["choices"][0]["message"]["content"]
-        except KeyError:
-            return ""
+        return response.get("token")
+
+
+class AsyncKOBOLDAI(AsyncProvider):
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        temperature: float = 1,
+        top_p: float = 1,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        """Instantiate TGPT
+
+        Args:
+            is_conversation (str, optional): Flag for chatting conversationally. Defaults to True.
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.2.
+            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.999.
+            timeout (int, optional): Http requesting timeout. Defaults to 30
+            intro (str, optional): Conversation introductory prompt. Defaults to `Conversation.intro`.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional) : Http reqiuest proxies (socks). Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.temperature = temperature
+        self.top_p = top_p
+        self.chat_endpoint = (
+            "https://koboldai-koboldcpp-tiefighter.hf.space/api/extra/generate/stream"
+        )
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.headers = {
+            "Content-Type": "application/json",
+            "Accept": "application/json",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session = httpx.AsyncClient(headers=self.headers, proxies=proxies)
+
+    async def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict | AsyncGenerator:
+        """Chat with AI asynchronously.
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict|AsyncGenerator : ai content
+        ```json
+        {
+           "token" : "How may I assist you today?"
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        payload = {
+            "prompt": conversation_prompt,
+            "temperature": self.temperature,
+            "top_p": self.top_p,
+        }
+
+        async def for_stream():
+            async with self.session.stream(
+                "POST", self.chat_endpoint, json=payload, timeout=self.timeout
+            ) as response:
+                if not response.is_success:
+                    raise exceptions.FailedToGenerateResponseError(
+                        f"Failed to generate response - ({response.status_code}, {response.reason_phrase})"
+                    )
+
+                message_load = ""
+                async for value in response.aiter_lines():
+                    try:
+                        resp = sanitize_stream(value)
+                        message_load += await self.get_message(resp)
+                        resp["token"] = message_load
+                        self.last_response.update(resp)
+                        yield value if raw else resp
+                    except json.decoder.JSONDecodeError:
+                        pass
+
+            self.conversation.update_chat_history(
+                prompt, await self.get_message(self.last_response)
+            )
+
+        async def for_non_stream():
+            # let's make use of stream
+            async for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str | AsyncGenerator:
+        """Generate response `str` asynchronously.
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        async def for_stream():
+            async_ask = await self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            )
+            async for response in async_ask:
+                yield await self.get_message(response)
+
+        async def for_non_stream():
+            return await self.get_message(
+                await self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response.get("token")
 
 
 if __name__ == "__main__":
-    bot = GROQ("grog api key")
+    bot = KOBOLDAI()
+
+    def main():
+        resp = bot.ask("hello")
+        for value in resp:
+            print(value)
+
+    async def asyncmain():
+        bot = AsyncKOBOLDAI()
+        resp = await bot.chat("hello", False)
+        print(resp)
+        # async for value in resp:
+        #    print(value)
 
-    resp = bot.ask("coding", stream=True)
+    main()
+    import asyncio
 
-    for val in resp:
-        print(json.dumps(val, indent=4))
+    asyncio.run(asyncmain())
```

### Comparing `python_tgpt-0.6.9/src/pytgpt/leo/main.py` & `python_tgpt-0.7.0/src/pytgpt/blackboxai/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,72 @@
-import requests
 import json
+import httpx
+import requests
+import pytgpt.exceptions as exceptions
 from pytgpt.utils import Optimizers
 from pytgpt.utils import Conversation
 from pytgpt.utils import AwesomePrompts
-from pytgpt.base import Provider
+from pytgpt.base import Provider, AsyncProvider
+from typing import AsyncGenerator
 
 session = requests.Session()
 
-model = "llama-2-13b-chat"
-
-key = "qztbjzBqJueQZLFkwTTJrieu8Vw3789u"
+default_model = None
 
 
-class LEO(Provider):
+class BLACKBOXAI(Provider):
     def __init__(
         self,
         is_conversation: bool = True,
         max_tokens: int = 600,
-        temperature: float = 0.2,
-        top_k: int = -1,
-        top_p: float = 0.999,
-        model: str = model,
-        brave_key: str = key,
         timeout: int = 30,
         intro: str = None,
         filepath: str = None,
         update_file: bool = True,
         proxies: dict = {},
         history_offset: int = 10250,
         act: str = None,
+        model: str = default_model,
     ):
-        """Instantiate TGPT
+        """Instantiates BLACKBOXAI
 
         Args:
-            is_conversation (str, optional): Flag for chatting conversationally. Defaults to True.
-            brave_key (str, optional): Brave API access key. Defaults to "qztbjzBqJueQZLFkwTTJrieu8Vw3789u".
-            model (str, optional): Text generation model name. Defaults to "llama-2-13b-chat".
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True
             max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.2.
-            top_k (int, optional): Chance of topic being repeated. Defaults to -1.
-            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.999.
-            timeput (int, optional): Http requesting timeout. Defaults to 30
-            intro (str, optional): Conversation introductory prompt. Defaults to `Conversation.intro`.
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
             filepath (str, optional): Path to file containing conversation history. Defaults to None.
             update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional) : Http reqiuest proxies (socks). Defaults to {}.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
             history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
             act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+            model (str, optional): Model name. Defaults to "Phind Model".
         """
-        self.is_conversation = is_conversation
         self.max_tokens_to_sample = max_tokens
-        self.model = model
-        self.stop_sequences = ["</response>", "</s>"]
-        self.temperature = temperature
-        self.top_k = top_k
-        self.top_p = top_p
-        self.chat_endpoint = "https://ai-chat.bsg.brave.com/v1/complete"
+        self.is_conversation = is_conversation
+        self.chat_endpoint = "https://www.blackbox.ai/api/chat"
         self.stream_chunk_size = 64
         self.timeout = timeout
         self.last_response = {}
+        self.model = model
+        self.previewToken: str = None
+        self.userId: str = ""
+        self.codeModelMode: bool = True
+        self.id: str = ""
+        self.agentMode: dict = {}
+        self.trendingAgentMode: dict = {}
+        self.isMicMode: bool = False
+
         self.headers = {
             "Content-Type": "application/json",
-            "accept": "text/event-stream",
-            "x-brave-key": brave_key,
-            "accept-language": "en-US,en;q=0.9",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:99.0) Gecko/20100101 Firefox/110.0",
+            "User-Agent": "",
+            "Accept": "*/*",
+            "Accept-Encoding": "Identity",
         }
+
         self.__available_optimizers = (
             method
             for method in dir(Optimizers)
             if callable(getattr(Optimizers, method)) and not method.startswith("__")
         )
         session.headers.update(self.headers)
         Conversation.intro = (
@@ -80,22 +77,14 @@
             else intro or Conversation.intro
         )
         self.conversation = Conversation(
             is_conversation, self.max_tokens_to_sample, filepath, update_file
         )
         self.conversation.history_offset = history_offset
         session.proxies = proxies
-        self.system_prompt = (
-            "\n\nYour name is Leo, a helpful"
-            "respectful and honest AI assistant created by the company Brave. You will be replying to a user of the Brave browser. "
-            "Always respond in a neutral tone. Be polite and courteous. Answer concisely in no more than 50-80 words."
-            "\n\nPlease ensure that your responses are socially unbiased and positive in nature."
-            "If a question does not make any sense, or is not factually coherent, explain why instead of answering something not correct. "
-            "If you don't know the answer to a question, please don't share false information.\n"
-        )
 
     def ask(
         self,
         prompt: str,
         stream: bool = False,
         raw: bool = False,
         optimizer: str = None,
@@ -109,21 +98,15 @@
             raw (bool, optional): Stream back raw response as received. Defaults to False.
             optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
             conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
         Returns:
            dict : {}
         ```json
         {
-            "completion": "\nNext: domestic cat breeds with short hair >>",
-            "stop_reason": null,
-            "truncated": false,
-            "stop": null,
-            "model": "llama-2-13b-chat",
-            "log_id": "cmpl-3kYiYxSNDvgMShSzFooz6t",
-            "exception": null
+           "text" : "print('How may I help you today?')"
         }
         ```
         """
         conversation_prompt = self.conversation.gen_complete_prompt(prompt)
         if optimizer:
             if optimizer in self.__available_optimizers:
                 conversation_prompt = getattr(Optimizers, optimizer)(
@@ -132,68 +115,62 @@
             else:
                 raise Exception(
                     f"Optimizer is not one of {self.__available_optimizers}"
                 )
 
         session.headers.update(self.headers)
         payload = {
-            "max_tokens_to_sample": self.max_tokens_to_sample,
-            "model": self.model,
-            "prompt": f"<s>[INST] <<SYS>>{self.system_prompt}<</SYS>>{conversation_prompt} [/INST]",
-            "self.stop_sequence": self.stop_sequences,
-            "stream": stream,
-            "top_k": self.top_k,
-            "top_p": self.top_p,
+            "messages": [
+                # json.loads(prev_messages),
+                {"content": conversation_prompt, "role": "user"}
+            ],
+            "id": self.id,
+            "previewToken": self.previewToken,
+            "userId": self.userId,
+            "codeModelMode": self.codeModelMode,
+            "agentMode": self.agentMode,
+            "trendingAgentMode": self.trendingAgentMode,
+            "isMicMode": self.isMicMode,
         }
 
         def for_stream():
             response = session.post(
                 self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
             )
             if (
                 not response.ok
                 or not response.headers.get("Content-Type")
-                == "text/event-stream; charset=utf-8"
+                == "text/plain; charset=utf-8"
             ):
-                raise Exception(
-                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                raise exceptions.FailedToGenerateResponseError(
+                    f"Failed to generate response - ({response.status_code}, {response.reason})"
                 )
-
+            streaming_text = ""
             for value in response.iter_lines(
                 decode_unicode=True,
-                delimiter="" if raw else "data:",
                 chunk_size=self.stream_chunk_size,
+                delimiter="\n",
             ):
                 try:
-                    resp = json.loads(value)
-                    self.last_response.update(resp)
-                    yield value if raw else resp
+                    if bool(value):
+                        streaming_text += value + ("\n" if stream else "")
+
+                        resp = dict(text=streaming_text)
+                        self.last_response.update(resp)
+                        yield value if raw else resp
                 except json.decoder.JSONDecodeError:
                     pass
             self.conversation.update_chat_history(
                 prompt, self.get_message(self.last_response)
             )
 
         def for_non_stream():
-            response = session.post(
-                self.chat_endpoint, json=payload, stream=False, timeout=self.timeout
-            )
-            if (
-                not response.ok
-                or not response.headers.get("Content-Type", "") == "application/json"
-            ):
-                raise Exception(
-                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
-                )
-            resp = response.json()
-            self.last_response.update(resp)
-            self.conversation.update_chat_history(
-                prompt, self.get_message(self.last_response)
-            )
-            return resp
+            for _ in for_stream():
+                pass
+            return self.last_response
 
         return for_stream() if stream else for_non_stream()
 
     def chat(
         self,
         prompt: str,
         stream: bool = False,
@@ -234,8 +211,228 @@
         Args:
             response (dict): Response generated by `self.ask`
 
         Returns:
             str: Message extracted
         """
         assert isinstance(response, dict), "Response should be of dict data-type only"
-        return response.get("completion")
+        return response["text"]
+
+
+class AsyncBLACKBOXAI(AsyncProvider):
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+        model: str = default_model,
+    ):
+        """Instantiates BLACKBOXAI
+
+        Args:
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+            model (str, optional): Model name. Defaults to "Phind Model".
+        """
+        self.max_tokens_to_sample = max_tokens
+        self.is_conversation = is_conversation
+        self.chat_endpoint = "https://www.blackbox.ai/api/chat"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.model = model
+        self.previewToken: str = None
+        self.userId: str = ""
+        self.codeModelMode: bool = True
+        self.id: str = ""
+        self.agentMode: dict = {}
+        self.trendingAgentMode: dict = {}
+        self.isMicMode: bool = False
+
+        self.headers = {
+            "Content-Type": "application/json",
+            "User-Agent": "",
+            "Accept": "*/*",
+            "Accept-Encoding": "Identity",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session = httpx.AsyncClient(headers=self.headers, proxies=proxies)
+
+    async def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict | AsyncGenerator:
+        """Chat with AI asynchronously.
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict|AsyncGenerator : ai content
+        ```json
+        {
+           "text" : "print('How may I help you today?')"
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        payload = {
+            "messages": [
+                # json.loads(prev_messages),
+                {"content": conversation_prompt, "role": "user"}
+            ],
+            "id": self.id,
+            "previewToken": self.previewToken,
+            "userId": self.userId,
+            "codeModelMode": self.codeModelMode,
+            "agentMode": self.agentMode,
+            "trendingAgentMode": self.trendingAgentMode,
+            "isMicMode": self.isMicMode,
+        }
+
+        async def for_stream():
+            async with self.session.stream(
+                "POST", self.chat_endpoint, json=payload, timeout=self.timeout
+            ) as response:
+                if (
+                    not response.is_success
+                    or not response.headers.get("Content-Type")
+                    == "text/plain; charset=utf-8"
+                ):
+                    raise exceptions.FailedToGenerateResponseError(
+                        f"Failed to generate response - ({response.status_code}, {response.reason_phrase})"
+                    )
+                streaming_text = ""
+                async for value in response.aiter_lines():
+                    try:
+                        if bool(value):
+                            streaming_text += value + ("\n" if stream else "")
+                            resp = dict(text=streaming_text)
+                            self.last_response.update(resp)
+                            yield value if raw else resp
+                    except json.decoder.JSONDecodeError:
+                        pass
+            self.conversation.update_chat_history(
+                prompt, await self.get_message(self.last_response)
+            )
+
+        async def for_non_stream():
+            async for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str | AsyncGenerator:
+        """Generate response `str` asynchronously.
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str|AsyncGenerator: Response generated
+        """
+
+        async def for_stream():
+            async_ask = await self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            )
+            async for response in async_ask:
+                yield await self.get_message(response)
+
+        async def for_non_stream():
+            return await self.get_message(
+                await self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response["text"]
+
+
+if __name__ == "__main__":
+    bot = BLACKBOXAI()
+
+    def main():
+        resp = bot.ask("hello")
+        for value in resp:
+            print(value)
+
+    async def asyncmain():
+        bot = AsyncBLACKBOXAI()
+        resp = await bot.chat("hello", True)
+        # print(resp)
+        async for value in resp:
+            print(value)
+
+    # main()
+    import asyncio
+
+    asyncio.run(asyncmain())
```

### Comparing `python_tgpt-0.6.9/src/pytgpt/phind/main.py` & `python_tgpt-0.7.0/src/pytgpt/phind/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import re
 import json
 import yaml
+import httpx
 import requests
 from pytgpt.utils import Optimizers
 from pytgpt.utils import Conversation
 from pytgpt.utils import AwesomePrompts
+from pytgpt.base import Provider, AsyncProvider
+import pytgpt.exceptions as exceptions
+from typing import AsyncGenerator
 
 session = requests.Session()
 
 default_model = "Phind Model"
 
 
-class PHIND:
+class PHIND(Provider):
     def __init__(
         self,
         is_conversation: bool = True,
         max_tokens: int = 600,
         timeout: int = 30,
         intro: str = None,
         filepath: str = None,
@@ -140,15 +144,15 @@
                 self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
             )
             if (
                 not response.ok
                 or not response.headers.get("Content-Type")
                 == "text/event-stream; charset=utf-8"
             ):
-                raise Exception(
+                raise exceptions.FailedToGenerateResponseError(
                     f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
                 )
             streaming_text = ""
             for value in response.iter_lines(
                 decode_unicode=True,
                 chunk_size=self.stream_chunk_size,
             ):
@@ -247,7 +251,274 @@
 
         else:
             return (
                 response["choices"][0]["delta"].get("content")
                 if response["choices"][0].get("finish_reason") is None
                 else ""
             )
+
+
+class AsyncPHIND(AsyncProvider):
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+        model: str = default_model,
+        quiet: bool = False,
+    ):
+        """Instantiates PHIND
+
+        Args:
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+            model (str, optional): Model name. Defaults to "Phind Model".
+            quiet (bool, optional): Ignore web search-results and yield final response only. Defaults to False.
+        """
+        self.max_tokens_to_sample = max_tokens
+        self.is_conversation = is_conversation
+        self.chat_endpoint = "https://https.extension.phind.com/agent/"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.model = model
+        self.quiet = quiet
+
+        self.headers = {
+            "Content-Type": "application/json",
+            "User-Agent": "",
+            "Accept": "*/*",
+            "Accept-Encoding": "Identity",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session = httpx.AsyncClient(headers=self.headers, proxies=proxies)
+
+    async def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+        synchronous_generator=False,
+    ) -> dict | AsyncGenerator:
+        """Asynchronously Chat with AI
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict|AsyncGenerator : ai content.
+        ```json
+        {
+            "id": "chatcmpl-r0wujizf2i2xb60mjiwt",
+            "object": "chat.completion.chunk",
+            "created": 1706775384,
+            "model": "trt-llm-phind-model-serving",
+            "choices": [
+                {
+                    "index": 0,
+                    "delta": {
+                        "content": "Hello! How can I assist you with your programming today?"
+                        },
+                    "finish_reason": null
+                }
+            ]
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        payload = {
+            "additional_extension_context": "",
+            "allow_magic_buttons": True,
+            "is_vscode_extension": True,
+            "message_history": [
+                {"content": conversation_prompt, "metadata": {}, "role": "user"}
+            ],
+            "requested_model": self.model,
+            "user_input": prompt,
+        }
+
+        async def for_stream():
+            async with self.session.stream(
+                "POST",
+                self.chat_endpoint,
+                json=payload,
+                timeout=self.timeout,
+            ) as response:
+                if (
+                    not response.is_success
+                    or not response.headers.get("Content-Type")
+                    == "text/event-stream; charset=utf-8"
+                ):
+                    raise exceptions.FailedToGenerateResponseError(
+                        f"Failed to generate response - ({response.status_code}, {response.reason_phrase})"
+                    )
+                streaming_text = ""
+                async for value in response.aiter_lines():
+                    try:
+                        modified_value = re.sub("data:", "", value)
+                        json_modified_value = json.loads(modified_value)
+                        retrieved_text = await self.get_message(json_modified_value)
+                        if not retrieved_text:
+                            continue
+                        streaming_text += retrieved_text
+                        json_modified_value["choices"][0]["delta"][
+                            "content"
+                        ] = streaming_text
+                        self.last_response.update(json_modified_value)
+                        yield value if raw else json_modified_value
+                    except json.decoder.JSONDecodeError:
+                        pass
+                self.conversation.update_chat_history(
+                    prompt, await self.get_message(self.last_response)
+                )
+
+        async def for_non_stream():
+            async for _ in for_stream():
+                pass
+            return self.last_response
+
+        return (
+            for_stream()
+            if stream and not synchronous_generator
+            else await for_non_stream()
+        )
+
+    async def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str | AsyncGenerator:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str|AsyncGenerator: Response generated
+        """
+
+        async def for_stream():
+            ask_resp = await self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            )
+            async for response in ask_resp:
+                yield await self.get_message(response)
+
+        async def for_non_stream():
+            return await self.get_message(
+                await self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        if response.get("type", "") == "metadata":
+            return
+
+        delta: dict = response["choices"][0]["delta"]
+
+        if not delta:
+            return ""
+
+        elif delta.get("function_call"):
+            if self.quiet:
+                return ""
+
+            function_call: dict = delta["function_call"]
+            if function_call.get("name"):
+                return function_call["name"]
+            elif function_call.get("arguments"):
+                return function_call.get("arguments")
+
+        elif delta.get("metadata"):
+            if self.quiet:
+                return ""
+            return yaml.dump(delta["metadata"])
+
+        else:
+            return (
+                response["choices"][0]["delta"].get("content")
+                if response["choices"][0].get("finish_reason") is None
+                else ""
+            )
+
+
+if __name__ == "__main__":
+    bot = PHIND()
+
+    def main():
+        resp = bot.ask("hello")
+        for value in resp:
+            print(value)
+
+    async def asyncmain():
+        bot = AsyncPHIND()
+        resp = await bot.chat("hello", False)
+        print(resp)
+        # async for value in resp:
+        #    print(value)
+
+    main()
+    import asyncio
+
+    asyncio.run(asyncmain())
```

### Comparing `python_tgpt-0.6.9/src/pytgpt/utils.py` & `python_tgpt-0.7.0/src/pytgpt/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from rich.markdown import Markdown
 from rich.console import Console
 from pathlib import Path
 from typing import Union
 from typing import NoReturn
 import requests
 import vlc
+import httpx
+import asyncio
 from time import sleep as wait
 
 appdir = appdirs.AppDirs("pytgpt", "Smartwa")
 
 default_path = appdir.user_cache_dir
 
 api_static_dir = Path(default_path) / "api"
@@ -29,14 +31,34 @@
 
 os.makedirs(default_path, exist_ok=True)
 os.makedirs(api_static_dir.as_posix(), exist_ok=True)
 os.makedirs(api_static_image_dir.as_posix(), exist_ok=True)
 os.makedirs(api_static_audio_dir.as_posix(), exist_ok=True)
 
 
+def sanitize_stream(
+    chunk: str, intro_value: str = "data:", to_json: bool = True
+) -> str | dict:
+    """Remove streaming flags
+
+    Args:
+        chunk (str): Streamig chunk.
+        intro_value (str, optional): streaming flag. Defaults to "data:".
+        to_json (bool, optional). Return chunk as dictionary. Defaults to True.
+
+    Returns:
+        str: Sanitized streaming value.
+    """
+
+    if chunk.startswith(intro_value):
+        chunk = chunk[len(intro_value) :]
+
+    return json.loads(chunk) if to_json else chunk
+
+
 def run_system_command(
     command: str,
     exit_on_error: bool = True,
     stdout_error: bool = True,
     help: str = None,
 ):
     """Run commands against system
@@ -889,50 +911,52 @@
         "Jakub",
         "Szabolcs",
         "Hoda",
         "Naayf",
     ]
 
     @classmethod
-    def text_to_audio(
+    async def async_text_to_audio(
         cls,
         message: str,
-        voice: str = "Brian",
+        voice: str = "en-US-Wavenet-C",
         proxies: dict[str, str] = {},
         timeout: int = 30,
         save_to: Union[Path, str] = None,
         auto: bool = False,
     ) -> Union[str, bytes]:
         """
+        Asynchronous implementation of text_to_audio.
         Text to speech using StreamElements API
 
         Parameters:
             message (str): The text to convert to speech
-            voice (str, optional): The voice to use for speech synthesis. Defaults to "Brian".
+            voice (str, optional): The voice to use for speech synthesis. Defaults to "en-US-Wavenet-C".
             proxies (dict, optional): Http request proxies. Default to {}.
             timeout (int, optional): Http request timeout. Defaults to 30.
             save_to (bool, optional): Path to save the audio file. Defaults to None.
             auto (bool, optional): Generate filename for the contents based on `message` and save to `cls.cache_dir`. Defaults to False.
 
         Returns:
             result (Union[str, bytes]): Path to saved contents or audio content.
         """
         assert (
             voice in cls.all_voices
         ), f"Voice '{voice}' not one of [{', '.join(cls.all_voices)}]"
         # Base URL for provider API
+        session = httpx.AsyncClient(
+            headers=cls.headers, proxies=proxies, timeout=timeout
+        )
         url: str = (
             f"https://api.streamelements.com/kappa/v2/speech?voice={voice}&text={{{message}}}"
         )
-        resp = requests.get(
-            url=url, headers=cls.headers, stream=True, proxies=proxies, timeout=timeout
-        )
-        if not resp.ok:
+        resp = await session.get(url)
+        if not resp.is_success:
             raise Exception(
-                f"Failed to perform the operation - ({resp.status_code}, {resp.reason}) - {resp.text}"
+                f"Failed to perform the operation - ({resp.status_code}, {resp.reason_phrase}) - {resp.text}"
             )
 
         def sanitize_filename(path):
             trash = [
                 "\\",
                 "/",
                 ":",
@@ -953,19 +977,53 @@
             save_to = save_to.as_posix()
 
         if save_to:
             if not save_to.endswith("mp3"):
                 save_to += ".mp3"
 
             with open(save_to, "wb") as fh:
-                for chunk in resp.iter_content(chunk_size=512):
-                    fh.write(chunk)
+                fh.write(resp.content)
+            return save_to
         else:
             return resp.content
-        return save_to
+
+    @classmethod
+    def text_to_audio(
+        cls,
+        message: str,
+        voice: str = "en-US-Wavenet-C",
+        proxies: dict[str, str] = {},
+        timeout: int = 30,
+        save_to: Union[Path, str] = None,
+        auto: bool = False,
+    ) -> Union[str, bytes]:
+        """
+        Text to speech using StreamElements API
+
+        Parameters:
+            message (str): The text to convert to speech
+            voice (str, optional): The voice to use for speech synthesis. Defaults to "en-US-Wavenet-C".
+            proxies (dict, optional): Http request proxies. Default to {}.
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            save_to (bool, optional): Path to save the audio file. Defaults to None.
+            auto (bool, optional): Generate filename for the contents based on `message` and save to `cls.cache_dir`. Defaults to False.
+
+        Returns:
+            result (Union[str, bytes]): Path to saved contents or audio content.
+        """
+        return asyncio.get_event_loop().run_until_complete(
+            cls.async_text_to_audio(
+                message=message,
+                voice=voice,
+                proxies=proxies,
+                timeout=timeout,
+                save_to=save_to,
+                auto=auto,
+            )
+        )
 
     @staticmethod
     def play(path_to_audio_file: Union[Path, str]) -> NoReturn:
         """Play audio (.mp3) using vlc media player or termux-media-player
 
         Args:
             path_to_audio_file (Union[Path, str]): Path to audio file.
```

### Comparing `python_tgpt-0.6.9/src/pytgpt/yepchat/main.py` & `python_tgpt-0.7.0/src/pytgpt/llama2/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 import requests
 import json
+import httpx
+import pytgpt.exceptions as exceptions
 from pytgpt.utils import Optimizers
 from pytgpt.utils import Conversation
 from pytgpt.utils import AwesomePrompts
-from pytgpt.base import Provider
+from pytgpt.base import Provider, AsyncProvider
+from typing import AsyncGenerator
 
 session = requests.Session()
 
-model = "Mixtral-8x7B-Instruct-v0.1"
+default_model = "meta/llama-2-70b-chat"
 
 
-class YEPCHAT(Provider):
+class LLAMA2(Provider):
     def __init__(
         self,
         is_conversation: bool = True,
-        max_tokens: int = 600,
-        temperature: float = 0.6,
+        max_tokens: int = 800,
+        temperature: float = 0.75,
         presence_penalty: int = 0,
         frequency_penalty: int = 0,
-        top_p: float = 0.7,
-        model: str = model,
+        top_p: float = 0.9,
+        model: str = default_model,
         timeout: int = 30,
         intro: str = None,
         filepath: str = None,
         update_file: bool = True,
         proxies: dict = {},
         history_offset: int = 10250,
         act: str = None,
     ):
-        """Instantiates YEPCHAT
+        """Instantiates LLAMA2
 
         Args:
             is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.6.
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 800.
+            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.75.
             presence_penalty (int, optional): Chances of topic being repeated. Defaults to 0.
             frequency_penalty (int, optional): Chances of word being repeated. Defaults to 0.
-            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.7.
-            model (str, optional): LLM model name. Defaults to "gpt-3.5-turbo".
+            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.9.
+            model (str, optional): LLM model name. Defaults to "meta/llama-2-70b-chat".
             timeout (int, optional): Http request timeout. Defaults to 30.
             intro (str, optional): Conversation introductory prompt. Defaults to None.
             filepath (str, optional): Path to file containing conversation history. Defaults to None.
             update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
             proxies (dict, optional): Http request proxies. Defaults to {}.
             history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
             act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
@@ -49,26 +52,23 @@
         self.is_conversation = is_conversation
         self.max_tokens_to_sample = max_tokens
         self.model = model
         self.temperature = temperature
         self.presence_penalty = presence_penalty
         self.frequency_penalty = frequency_penalty
         self.top_p = top_p
-        self.chat_endpoint = "https://api.yep.com/v1/chat/completions"
+        self.chat_endpoint = "https://www.llama2.ai/api"
         self.stream_chunk_size = 64
         self.timeout = timeout
         self.last_response = {}
         self.headers = {
-            "Accept": "*/*",
-            "Accept-Encoding": "gzip, deflate",
-            "Accept-Language": "en-US,en;q=0.9",
-            "Content-Type": "application/json; charset=utf-8",
-            "Origin": "https://yep.com",
-            "Referer": "https://yep.com/",
-            "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36",
+            "Content-Type": "application/json",
+            "Referer": "https://www.llama2.ai/",
+            "Content-Type": "text/plain;charset=UTF-8",
+            "Origin": "https://www.llama2.ai",
         }
 
         self.__available_optimizers = (
             method
             for method in dir(Optimizers)
             if callable(getattr(Optimizers, method)) and not method.startswith("__")
         )
@@ -102,76 +102,66 @@
             raw (bool, optional): Stream back raw response as received. Defaults to False.
             optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
             conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
         Returns:
            dict : {}
         ```json
         {
-            "id": "cmpl-c61c1c88de4e4ad3a79134775d17ea0c",
-            "object": "chat.completion.chunk",
-            "created": 1713876886,
-            "model": "Mixtral-8x7B-Instruct-v0.1",
-            "choices": [
-                {
-                    "index": 0,
-                    "delta": {
-                        "role": null,
-                        "content": " Sure, I can help with that. Are you looking for information on how to start coding, or do you need help with a specific coding problem? We can discuss various programming languages like Python, JavaScript, Java, C++, or others. Please provide more details so I can assist you better."
-                        },
-                    "finish_reason": null
-                }
-            ]
+           "text" : "How may I help you today?"
         }
         ```
         """
         conversation_prompt = self.conversation.gen_complete_prompt(prompt)
         if optimizer:
             if optimizer in self.__available_optimizers:
                 conversation_prompt = getattr(Optimizers, optimizer)(
                     conversation_prompt if conversationally else prompt
                 )
             else:
                 raise Exception(
                     f"Optimizer is not one of {self.__available_optimizers}"
                 )
         session.headers.update(self.headers)
+
         payload = {
-            "stream": True,
-            "max_tokens": 1280,
-            "top_p": self.top_p,
-            "temperature": self.temperature,
-            "messages": [{"content": conversation_prompt, "role": "user"}],
+            "prompt": f"{conversation_prompt}<s>[INST] {prompt} [/INST]",
             "model": self.model,
+            "systemPrompt": "You are a helpful assistant.",
+            "temperature": self.temperature,
+            "topP": self.top_p,
+            "maxTokens": self.max_tokens_to_sample,
+            "image": None,
+            "audio": None,
         }
 
         def for_stream():
             response = session.post(
                 self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
             )
-            if not response.ok:
-                raise Exception(
-                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+            if (
+                not response.ok
+                or not response.headers.get("Content-Type")
+                == "text/plain; charset=utf-8"
+            ):
+                raise exceptions.FailedToGenerateResponseError(
+                    f"Failed to generate response - ({response.status_code}, {response.reason})"
                 )
 
-            message_load = ""
+            message_load: str = ""
             for value in response.iter_lines(
                 decode_unicode=True,
-                delimiter="" if raw else "data:",
+                delimiter="\n",
                 chunk_size=self.stream_chunk_size,
             ):
                 try:
-                    resp = json.loads(value)
-                    incomplete_message = self.get_message(resp)
-                    if incomplete_message:
-                        message_load += incomplete_message
-                        resp["choices"][0]["delta"]["content"] = message_load
-                        self.last_response.update(resp)
+                    if bool(value.strip()):
+                        message_load += value + "\n"
+                        resp: dict = dict(text=message_load)
                         yield value if raw else resp
-                    elif raw:
-                        yield value
+                        self.last_response.update(resp)
                 except json.decoder.JSONDecodeError:
                     pass
             self.conversation.update_chat_history(
                 prompt, self.get_message(self.last_response)
             )
 
         def for_non_stream():
@@ -216,27 +206,238 @@
 
         return for_stream() if stream else for_non_stream()
 
     def get_message(self, response: dict) -> str:
         """Retrieves message only from response
 
         Args:
-            response (dict): Response generated by `self.ask`
+            response (str): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response["text"]
+
+
+class AsyncLLAMA2(AsyncProvider):
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 800,
+        temperature: float = 0.75,
+        presence_penalty: int = 0,
+        frequency_penalty: int = 0,
+        top_p: float = 0.9,
+        model: str = default_model,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        """Instantiates LLAMA2
+
+        Args:
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 800.
+            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.75.
+            presence_penalty (int, optional): Chances of topic being repeated. Defaults to 0.
+            frequency_penalty (int, optional): Chances of word being repeated. Defaults to 0.
+            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.9.
+            model (str, optional): LLM model name. Defaults to "meta/llama-2-70b-chat".
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.model = model
+        self.temperature = temperature
+        self.presence_penalty = presence_penalty
+        self.frequency_penalty = frequency_penalty
+        self.top_p = top_p
+        self.chat_endpoint = "https://www.llama2.ai/api"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.headers = {
+            "Content-Type": "application/json",
+            "Referer": "https://www.llama2.ai/",
+            "Content-Type": "text/plain;charset=UTF-8",
+            "Origin": "https://www.llama2.ai",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session = httpx.AsyncClient(
+            headers=self.headers,
+            proxies=proxies,
+        )
+
+    async def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict | AsyncGenerator:
+        """Chat with AI asynchronously.
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict|AsyncGeneraror[dict] : ai content
+        ```json
+        {
+           "text" : "How may I help you today?"
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        payload = {
+            "prompt": f"{conversation_prompt}<s>[INST] {prompt} [/INST]",
+            "model": self.model,
+            "systemPrompt": "You are a helpful assistant.",
+            "temperature": self.temperature,
+            "topP": self.top_p,
+            "maxTokens": self.max_tokens_to_sample,
+            "image": None,
+            "audio": None,
+        }
+
+        async def for_stream():
+            async with self.session.stream(
+                "POST", self.chat_endpoint, json=payload, timeout=self.timeout
+            ) as response:
+                if (
+                    not response.is_success
+                    or not response.headers.get("Content-Type")
+                    == "text/plain; charset=utf-8"
+                ):
+                    raise exceptions.FailedToGenerateResponseError(
+                        f"Failed to generate response - ({response.status_code}, {response.reason_phrase})"
+                    )
+                message_load: str = ""
+                async for value in response.aiter_lines():
+                    try:
+                        if bool(value.strip()):
+                            message_load += value + "\n"
+                            resp: dict = dict(text=message_load)
+                            yield value if raw else resp
+                            self.last_response.update(resp)
+                    except json.decoder.JSONDecodeError:
+                        pass
+            self.conversation.update_chat_history(
+                prompt, await self.get_message(self.last_response)
+            )
+
+        async def for_non_stream():
+            async for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str | AsyncGenerator:
+        """Generate response `str` asynchronously.
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str|AsyncGenerator: Response generated
+        """
+
+        async def for_stream():
+            async_ask = await self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            )
+            async for response in async_ask:
+                yield await self.get_message(response)
+
+        async def for_non_stream():
+            return await self.get_message(
+                await self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (str): Response generated by `self.ask`
 
         Returns:
             str: Message extracted
         """
         assert isinstance(response, dict), "Response should be of dict data-type only"
-        try:
-            if response["choices"][0].get("delta"):
-                return response["choices"][0]["delta"]["content"]
-            return response["choices"][0]["message"]["content"]
-        except KeyError:
-            return ""
+        return response["text"]
 
 
 if __name__ == "__main__":
-    bot = YEPCHAT()
+    bot = LLAMA2()
+
+    def main():
+        resp = bot.ask("hello")
+        for value in resp:
+            print(value)
+
+    async def asyncmain():
+        bot = AsyncLLAMA2()
+        resp = await bot.chat("hello", True)
+        # print(resp)
+        async for value in resp:
+            print(value)
+
+    # main()
+    import asyncio
 
-    resp = bot.ask("coding", stream=False)
-    # print(bot.get_message(resp))
-    print(json.dumps(resp, indent=4))
+    asyncio.run(asyncmain())
```

### Comparing `python_tgpt-0.6.9/src/python_tgpt.egg-info/PKG-INFO` & `python_tgpt-0.7.0/src/python_tgpt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tgpt
-Version: 0.6.9
+Version: 0.7.0
 Summary: Interact with AI without API key
 Home-page: https://github.com/Simatwa/python-tgpt
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
@@ -34,37 +34,38 @@
 Requires-Dist: requests[socks]==2.31.0
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: webchatgpt==0.3.0
 Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: poe-api-wrapper==1.3.6
 Requires-Dist: brotli==1.1.0
-Requires-Dist: g4f>=0.2.6.1
+Requires-Dist: g4f>=0.3.0.8
 Requires-Dist: Helpingai_T2-fork==0.3.2
 Requires-Dist: python-vlc>=3.0.20
+Requires-Dist: httpx==0.27.0
 Provides-Extra: cli
 Requires-Dist: click==8.1.3; extra == "cli"
 Requires-Dist: rich==13.3.4; extra == "cli"
 Requires-Dist: clipman==3.1.0; extra == "cli"
 Requires-Dist: pyperclip==1.8.2; extra == "cli"
 Requires-Dist: colorama==0.4.6; extra == "cli"
-Requires-Dist: g4f>=0.2.6.1; extra == "cli"
+Requires-Dist: g4f>=0.3.0.8; extra == "cli"
 Requires-Dist: python-dotenv==1.0.0; extra == "cli"
 Provides-Extra: api
 Requires-Dist: fastapi[all]==0.110.1; extra == "api"
 Provides-Extra: all
 Requires-Dist: g4f[all]>=0.2.6.1; extra == "all"
 Requires-Dist: matplotlib; extra == "all"
 Requires-Dist: gpt4all==2.2.0; extra == "all"
 Requires-Dist: click==8.1.3; extra == "all"
 Requires-Dist: rich==13.3.4; extra == "all"
 Requires-Dist: clipman==3.1.0; extra == "all"
 Requires-Dist: pyperclip==1.8.2; extra == "all"
 Requires-Dist: colorama==0.4.6; extra == "all"
-Requires-Dist: g4f>=0.2.6.1; extra == "all"
+Requires-Dist: g4f>=0.3.0.8; extra == "all"
 Requires-Dist: python-dotenv==1.0.0; extra == "all"
 Requires-Dist: fastapi[all]==0.110.1; extra == "all"
 
 <p align="center">
 <img src="https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true" width='40%'>
 </p>
 
@@ -73,15 +74,15 @@
 <!--
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 -->
 <a href="https://github.com/Simatwa/python-tgpt/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/python-tgpt"/></a>
 <a href="https://pypi.org/project/python-tgpt"><img alt="PyPi" src="https://img.shields.io/pypi/v/python-tgpt?color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>
-<a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
+<a href="#"><img alt="Website status" src="https://img.shields.io/website?url=https://python-tgpt.onrender.com"/></a>
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml"><img alt="Python Package flow" src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml/badge.svg?branch=master"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="https://pepy.tech/project/tgpt2"><img src="https://static.pepy.tech/personalized-badge/tgpt2?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" alt="Downloads"></a>
 <a href="https://pepy.tech/project/python-tgpt"><img src="https://static.pepy.tech/personalized-badge/python-tgpt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" alt="Downloads"></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases/latest"><img src="https://img.shields.io/github/downloads/Simatwa/python-tgpt/total?label=Asset%20Downloads&color=success" alt="Downloads"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/v/release/Simatwa/python-tgpt?color=success&label=Release&logo=github" alt="Latest release"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/release-date/Simatwa/python-tgpt?label=Release date&logo=github" alt="release date"></img></a>
@@ -129,15 +130,17 @@
 - 🔌 Offline support for Large Language Models
 - 🎨 Image generation capabilities
 - 🎤 Text-to-audio conversion capabilities
 - ⛓️ Chained requests via proxy
 - 🗨️ Enhanced conversational chat experience
 - 💾 Capability to save prompts and responses (Conversation)
 - 🔄 Ability to load previous conversations
-- 🤖 Pass [awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
+- 🚀 Pass [awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
+- 🤖 [Telegram bot](https://t.me/pytgpt_bot) - interface
+- 🔄 Asynchronous support for all major operations.
 
 
 ## Providers
 
 These are simply the hosts of the LLMs, which include:
 
 1. [Leo](https://brave.com/leo/) - **Brave**
@@ -388,14 +391,62 @@
 import pytgpt.gpt4free as gpt4free
 bot = gpt4free.GPT4FREE(provider="Koala")
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
+### Asynchronous
+
+**Version 0.7.0** introduces asynchronous implementation to almost all providers except a few such as *perplexity & gemini*, which relies on other libraries which lacks such implementation.
+
+To make it easier, you just have to prefix `Async` to the common synchronous class name. For instance `OPENGPT` will be accessed as `AsyncOPENGPT`:
+
+#### Streaming Whole ai response.
+
+```python
+import asyncio
+from pytgpt.phind import AsyncPHIND
+
+async def main():
+    async_ask = await AsyncPHIND(False).ask(
+        "Critique that python is cool.",
+        stream=True
+    )
+    async for streaming_response in async_ask:
+        print(
+            streaming_response
+        )
+
+asyncio.run(
+    main()
+)
+```
+
+#### Streaming just the text
+
+```python
+import asyncio
+from pytgpt.phind import AsyncPHIND
+
+async def main():
+    async_ask = await AsyncPHIND(False).chat(
+        "Critique that python is cool.",
+        stream=True
+    )
+    async for streaming_text in async_ask:
+        print(
+            streaming_text
+        )
+
+asyncio.run(
+    main()
+)
+```
+
 </details>
 
 <details>
 
 <summary>
 
 To obtain more tailored responses, consider utilizing [optimizers](pytgpt/utils.py) using the `optimizer` parameter. Its values can be set to either `code` or `system_command`.
@@ -596,14 +647,24 @@
 
 Version **0.6.4** introduces another dynamic provider, `auto`, which denotes the working provider **overall**. This relieves you of the workload of manually checking a working provider each time you fire up pytgpt.
 
 ## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot)
 
 If you're not satisfied with the existing interfaces, [pytgpt-bot](https://github.com/Simatwa/pytgpt-bot) could be the solution you're seeking. This bot is designed to enhance your experience by offering a wide range of functionalities. Whether you're interested in engaging in AI-driven conversations, creating images and audio from text, or exploring other innovative features, [pytgpt-bot is equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot)
 
+The bot is maintained as a separate project so you just have to execute a command get it installed :
+
+```
+$ pip install pytgpt-bot
+```
+
+Usage : `pytgpt bot run <bot-api-token>`
+
+Or you can simply interact with the one running now as [@pytgpt-bot](https://t.me/pytgpt_bot)
+
 <details>
 
 <summary>
 
 For more usage info run `$ pytgpt --help`
 
 </summary>
@@ -614,14 +675,15 @@
 Options:
   -v, --version  Show the version and exit.
   -h, --help     Show this message and exit.
 
 Commands:
   api          FastAPI control endpoint
   awesome      Perform CRUD operations on awesome-prompts
+  bot          Telegram bot interface control
   generate     Generate a quick response with AI
   gpt4free     Discover gpt4free models, providers etc
   imager       Generate images with pollinations.ai
   interactive  Chat with AI interactively (Default)
   utils        Utility endpoint for pytgpt
   webchatgpt   Reverse Engineered ChatGPT Web-Version
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.9 Summary: Interact with
+Metadata-Version: 2.1 Name: python-tgpt Version: 0.7.0 Summary: Interact with
 AI without API key Home-page: https://github.com/Simatwa/python-tgpt Author:
 Smartwa Author-email: simatwacaleb@proton.me Maintainer: Smartwa License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/python-tgpt Project-URL:
 Source Code, https://github.com/Simatwa/python-tgpt Project-URL: Issue Tracker,
 https://github.com/Simatwa/python-tgpt/issues Project-URL: Download, https://
 github.com/Simatwa/python-tgpt/releases Project-URL: Documentation, https://
@@ -19,34 +19,34 @@
 Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: requests[socks]==2.31.0 Requires-Dist: appdirs==1.4.4
 Requires-Dist: pyyaml==6.0.1 Requires-Dist: webchatgpt==0.3.0 Requires-Dist:
 GoogleBard1>=2.1.4 Requires-Dist: poe-api-wrapper==1.3.6 Requires-Dist:
-brotli==1.1.0 Requires-Dist: g4f>=0.2.6.1 Requires-Dist: Helpingai_T2-
-fork==0.3.2 Requires-Dist: python-vlc>=3.0.20 Provides-Extra: cli Requires-
-Dist: click==8.1.3; extra == "cli" Requires-Dist: rich==13.3.4; extra == "cli"
-Requires-Dist: clipman==3.1.0; extra == "cli" Requires-Dist: pyperclip==1.8.2;
-extra == "cli" Requires-Dist: colorama==0.4.6; extra == "cli" Requires-Dist:
-g4f>=0.2.6.1; extra == "cli" Requires-Dist: python-dotenv==1.0.0; extra ==
-"cli" Provides-Extra: api Requires-Dist: fastapi[all]==0.110.1; extra == "api"
-Provides-Extra: all Requires-Dist: g4f[all]>=0.2.6.1; extra == "all" Requires-
-Dist: matplotlib; extra == "all" Requires-Dist: gpt4all==2.2.0; extra == "all"
-Requires-Dist: click==8.1.3; extra == "all" Requires-Dist: rich==13.3.4; extra
-== "all" Requires-Dist: clipman==3.1.0; extra == "all" Requires-Dist:
-pyperclip==1.8.2; extra == "all" Requires-Dist: colorama==0.4.6; extra == "all"
-Requires-Dist: g4f>=0.2.6.1; extra == "all" Requires-Dist: python-
-dotenv==1.0.0; extra == "all" Requires-Dist: fastapi[all]==0.110.1; extra ==
-"all"
+brotli==1.1.0 Requires-Dist: g4f>=0.3.0.8 Requires-Dist: Helpingai_T2-
+fork==0.3.2 Requires-Dist: python-vlc>=3.0.20 Requires-Dist: httpx==0.27.0
+Provides-Extra: cli Requires-Dist: click==8.1.3; extra == "cli" Requires-Dist:
+rich==13.3.4; extra == "cli" Requires-Dist: clipman==3.1.0; extra == "cli"
+Requires-Dist: pyperclip==1.8.2; extra == "cli" Requires-Dist: colorama==0.4.6;
+extra == "cli" Requires-Dist: g4f>=0.3.0.8; extra == "cli" Requires-Dist:
+python-dotenv==1.0.0; extra == "cli" Provides-Extra: api Requires-Dist: fastapi
+[all]==0.110.1; extra == "api" Provides-Extra: all Requires-Dist: g4f
+[all]>=0.2.6.1; extra == "all" Requires-Dist: matplotlib; extra == "all"
+Requires-Dist: gpt4all==2.2.0; extra == "all" Requires-Dist: click==8.1.3;
+extra == "all" Requires-Dist: rich==13.3.4; extra == "all" Requires-Dist:
+clipman==3.1.0; extra == "all" Requires-Dist: pyperclip==1.8.2; extra == "all"
+Requires-Dist: colorama==0.4.6; extra == "all" Requires-Dist: g4f>=0.3.0.8;
+extra == "all" Requires-Dist: python-dotenv==1.0.0; extra == "all" Requires-
+Dist: fastapi[all]==0.110.1; extra == "all"
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true]
-_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_P_a_s_s_i_n_g_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]_[_c_o_v_e_r_a_g_e_]
-   _[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]_[_h_t_t_p_s_:_/_/
-  _h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/_b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/
-                        _S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
+  _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_W_e_b_s_i_t_e_ _s_t_a_t_u_s_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]
+   _[_c_o_v_e_r_a_g_e_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]
+                 _[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
+     _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/_S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
                              ******** ppyytthhoonn--ttggpptt ********
  [https://github.com/Simatwa/python-tgpt/blob/main/assets/demo-1.gif?raw=True]
 ```python >>> import pytgpt.phind as phind >>> bot = phind.PHIND() >>> bot.chat
 ('hello there') 'Hello! How can I assist you today?' ``` ```python from
 pytgpt.imager import Imager img = Imager() generated_images = img.generate
 (prompt="Cyberpunk", amount=3, stream=True) img.save(generated_images) ``` This
 project enables seamless interaction with over **45 free LLM providers**
@@ -59,37 +59,39 @@
 tgpt.onrender.com) - â¨ï¸ Command-line interface - ð§  Multiple LLM
 providers - **45+** - ð Stream and non-stream response - ð Ready to use
 (No API key required) - ð¯ Customizable script generation and execution -
 ð Offline support for Large Language Models - ð¨ Image generation
 capabilities - ð¤ Text-to-audio conversion capabilities - âï¸ Chained
 requests via proxy - ð¨ï¸ Enhanced conversational chat experience - ð¾
 Capability to save prompts and responses (Conversation) - ð Ability to load
-previous conversations - ð¤ Pass [awesome-chatgpt prompts](https://
-github.com/f/awesome-chatgpt-prompts) easily ## Providers These are simply the
-hosts of the LLMs, which include: 1. [Leo](https://brave.com/leo/) - **Brave**
-2. [Koboldai](https://koboldai-koboldcpp-tiefighter.hf.space) 3. [OpenGPTs]
-(https://opengpts-example-vz4y4ooboq-uc.a.run.app/) 4. [OpenAI](https://
-chat.openai.com) *(API key required)* 5. [WebChatGPT](https://github.com/
-Simatwa/WebChatGPT) - **OpenAI** *(Session ID required)* 6. [Gemini](https://
-github.com/Simatwa/bard) - **Google** *(Session ID required)* 9. [Phind](https:
-//www.phind.com) 10. [Llama2](https://www.llama2.ai) 11. [Blackboxai](https://
-www.blackbox.ai) 12. [gpt4all](https://gpt4all.io) *(Offline)* 13. [Poe](https:
-//poe.com) - Poe|Quora *(Session ID required)* 14. [Groq](https://
-console.groq.com/playground) *(API Key required)* 15. [Perplexity](https://
-www.perplexity.ai) 16. [YepChat](https://yep.com) 41+ providers proudly offered
-by [gpt4free](https://github.com/xtekky/gpt4free). - To list working providers
-run: ```sh $ pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10]
-(https://python.org) *(Optional)* ## Installation and Usage ### Installation
-Download binaries for your system from [here.](https://github.com/Simatwa/
-python-tgpt/releases/latest/) Alternatively, you can install non-binaries. *
-(Recommended)* 1. Developers: ```sh pip install --upgrade python-tgpt ``` 2.
-Commandline: ```sh pip install --upgrade "python-tgpt[cli]" ``` 3. Full
-installation: ```sh pip install --upgrade "python-tgpt[all]" ``` > `pip install
--U "python-tgt[api]"` will install REST API dependencies. ## Usage This package
-offers a convenient command-line interface. > [!NOTE] > `phind` is the default
+previous conversations - ð Pass [awesome-chatgpt prompts](https://
+github.com/f/awesome-chatgpt-prompts) easily - ð¤ [Telegram bot](https://
+t.me/pytgpt_bot) - interface - ð Asynchronous support for all major
+operations. ## Providers These are simply the hosts of the LLMs, which include:
+1. [Leo](https://brave.com/leo/) - **Brave** 2. [Koboldai](https://koboldai-
+koboldcpp-tiefighter.hf.space) 3. [OpenGPTs](https://opengpts-example-
+vz4y4ooboq-uc.a.run.app/) 4. [OpenAI](https://chat.openai.com) *(API key
+required)* 5. [WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI**
+*(Session ID required)* 6. [Gemini](https://github.com/Simatwa/bard) -
+**Google** *(Session ID required)* 9. [Phind](https://www.phind.com) 10.
+[Llama2](https://www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12.
+[gpt4all](https://gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) -
+Poe|Quora *(Session ID required)* 14. [Groq](https://console.groq.com/
+playground) *(API Key required)* 15. [Perplexity](https://www.perplexity.ai)
+16. [YepChat](https://yep.com) 41+ providers proudly offered by [gpt4free]
+(https://github.com/xtekky/gpt4free). - To list working providers run: ```sh $
+pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10](https://
+python.org) *(Optional)* ## Installation and Usage ### Installation Download
+binaries for your system from [here.](https://github.com/Simatwa/python-tgpt/
+releases/latest/) Alternatively, you can install non-binaries. *(Recommended)*
+1. Developers: ```sh pip install --upgrade python-tgpt ``` 2. Commandline:
+```sh pip install --upgrade "python-tgpt[cli]" ``` 3. Full installation: ```sh
+pip install --upgrade "python-tgpt[all]" ``` > `pip install -U "python-tgt
+[api]"` will install REST API dependencies. ## Usage This package offers a
+convenient command-line interface. > [!NOTE] > `phind` is the default
 *provider*. - For a quick response: ```bash python -m pytgpt generate "" ``` -
 For interactive mode: ```bash python -m pytgpt interactive "" ``` Make use of
 flag `--provider` followed by the provider name of your choice. e.g `--provider
 koboldai` > To list all providers offered by gpt4free, use following commands:
 ```pytgpt gpt4free list providers``` You can also simply use `pytgpt` instead
 of `python -m pytgpt`. Starting from version 0.2.7, running `$ pytgpt` without
 any other command or option will automatically enter the `interactive` mode.
@@ -122,68 +124,80 @@
 import pytgpt.auto import auto bot = auto.AUTO() print(bot.chat("")) ``` Openai
 ```python import pytgpt.openai as openai bot = openai.OPENAI("") print(bot.chat
 ("")) ``` Koboldai ```python import pytgpt.koboldai as koboldai bot =
 koboldai.KOBOLDAI() print(bot.chat("")) ``` Opengpt ```python import
 pytgpt.opengpt as opengpt bot = opengpt.OPENGPT() print(bot.chat("")) ``` phind
 ```python import pytgpt.phind as phind bot = phind.PHIND() print(bot.chat(""))
 ``` Gpt4free providers ```python import pytgpt.gpt4free as gpt4free bot =
-gpt4free.GPT4FREE(provider="Koala") print(bot.chat("")) ``` To obtain more
-tailored responses, consider utilizing [optimizers](pytgpt/utils.py) using the
-`optimizer` parameter. Its values can be set to either `code` or
-`system_command`. ```python from pytgpt.leo import LEO bot = LEO() resp =
-bot.ask('', optimizer='code') print(resp) ``` > [!IMPORTANT] > Commencing from
-[v0.1.0](https://github.com/Simatwa/python-tgpt/releases/), the default mode of
-interaction is conversational. This mode enhances the interactive experience,
-offering better control over the chat history. By associating previous prompts
-and responses, it tailors conversations for a more engaging experience. You can
-still disable the mode: ```python bot = koboldai.KOBOLDAI
-(is_conversation=False) ``` Utilize the `--disable-conversation` flag in the
-console to achieve the same functionality. > [!CAUTION] > **Bard** autohandles
-context due to the obvious reason; the `is_conversation` parameter is not
-necessary at all hence not required when initializing the class. Also be
-informed that majority of providers offered by *gpt4free* requires *Google
-Chrome* inorder to function. ### Image Generation This has been made possible
-by [pollinations.ai](https://pollination.ai). ```sh $ pytgpt imager "" # e.g
-pytgpt imager "Coding bot" ``` Developers ```python from pytgpt.imager import
-Imager img = Imager() generated_img = img.generate('Coding bot') # [bytes]
-img.save(generated_img) ``` Download Multiple Images ```python from
-pytgpt.imager import Imager img = Imager() img_generator = img.generate('Coding
-bot', amount=3, stream=True) img.save(img_generator) # RAM friendly ``` ####
-Using **Prodia** provider ```python from pytgpt.imager import Prodia img =
-Prodia() img_generator = img.generate('Coding bot', amount=3, stream=True)
-img.save(img_generator) ``` ### Advanced Usage of Placeholders The `generate`
-functionality has been enhanced starting from *v0.3.0* to enable comprehensive
-utilization of the `--with-copied` option and support for accepting piped
-inputs. This improvement introduces placeholders, offering dynamic values for
-more versatile interactions. | Placeholder | Represents | | ------------ | ----
-------- | | `{{stream}}` | The piped input | | `{{copied}}` | The last copied
-text | This feature is particularly beneficial for intricate operations. For
-example: ```bash $ git diff | pytgpt generate "Here is a diff file: {{stream}}
-Make a concise commit message from it, aligning with my commit message history:
-{{copied}}" --shell --new ``` > In this illustration, `{{stream}}` denotes the
-result of the `$ git diff` operation, while `{{copied}}` signifies the content
-copied from the output of the `$ git log` command. ### Awesome Prompts [These
-prompts](https://github.com/Simatwa/gpt-cli/blob/main/assets/all-
-acts.pdf?raw=True) are designed to guide the AI's behavior or responses in a
-particular direction, encouraging it to exhibit certain characteristics or
-behaviors. The term "awesome-prompt" is not a formal term in AI or machine
-learning literature, but it encapsulates the idea of crafting prompts that are
-effective in achieving desired outcomes. Let's say you want it to behave like a
-*Linux Terminal*, *PHP Interpreter*, or just to [**JAIL BREAK.**](https://
-gist.github.com/coolaj86/6f4f7b30129b0251f61fa7baaa881516) Instances : ```sh $
-pytgpt interactve --awesome-prompt "Linux Terminal" # Act like a Linux Terminal
-$ pytgpt interactive -ap DAN # Jailbreak ``` > [!NOTE] > Awesome prompts are
-alternative to `--intro`. > Run `$ pytgpt awesome whole` to list available
-prompts (*200+*). > Run `$ pytgpt awesome --help` for more info. ###
-Introducing RawDog RawDog is a masterpiece feature that exploits the versatile
-capabilities of Python to command and control your system as per your needs.
-You can literally do anything with it, since it generates and executes python
-codes, driven by **your prompts**! To have a bite of *rawdog* simply append the
-flag `--rawdog` *shortform* `-rd` in *generate/interactive* mode. This
-introduces a never seen-before feature in the *tgpt ecosystem*. Thanks to
+gpt4free.GPT4FREE(provider="Koala") print(bot.chat("")) ``` ### Asynchronous
+**Version 0.7.0** introduces asynchronous implementation to almost all
+providers except a few such as *perplexity & gemini*, which relies on other
+libraries which lacks such implementation. To make it easier, you just have to
+prefix `Async` to the common synchronous class name. For instance `OPENGPT`
+will be accessed as `AsyncOPENGPT`: #### Streaming Whole ai response. ```python
+import asyncio from pytgpt.phind import AsyncPHIND async def main(): async_ask
+= await AsyncPHIND(False).ask( "Critique that python is cool.", stream=True )
+async for streaming_response in async_ask: print( streaming_response )
+asyncio.run( main() ) ``` #### Streaming just the text ```python import asyncio
+from pytgpt.phind import AsyncPHIND async def main(): async_ask = await
+AsyncPHIND(False).chat( "Critique that python is cool.", stream=True ) async
+for streaming_text in async_ask: print( streaming_text ) asyncio.run( main() )
+``` To obtain more tailored responses, consider utilizing [optimizers](pytgpt/
+utils.py) using the `optimizer` parameter. Its values can be set to either
+`code` or `system_command`. ```python from pytgpt.leo import LEO bot = LEO()
+resp = bot.ask('', optimizer='code') print(resp) ``` > [!IMPORTANT] >
+Commencing from [v0.1.0](https://github.com/Simatwa/python-tgpt/releases/), the
+default mode of interaction is conversational. This mode enhances the
+interactive experience, offering better control over the chat history. By
+associating previous prompts and responses, it tailors conversations for a more
+engaging experience. You can still disable the mode: ```python bot =
+koboldai.KOBOLDAI(is_conversation=False) ``` Utilize the `--disable-
+conversation` flag in the console to achieve the same functionality. >
+[!CAUTION] > **Bard** autohandles context due to the obvious reason; the
+`is_conversation` parameter is not necessary at all hence not required when
+initializing the class. Also be informed that majority of providers offered by
+*gpt4free* requires *Google Chrome* inorder to function. ### Image Generation
+This has been made possible by [pollinations.ai](https://pollination.ai). ```sh
+$ pytgpt imager "" # e.g pytgpt imager "Coding bot" ``` Developers ```python
+from pytgpt.imager import Imager img = Imager() generated_img = img.generate
+('Coding bot') # [bytes] img.save(generated_img) ``` Download Multiple Images
+```python from pytgpt.imager import Imager img = Imager() img_generator =
+img.generate('Coding bot', amount=3, stream=True) img.save(img_generator) # RAM
+friendly ``` #### Using **Prodia** provider ```python from pytgpt.imager import
+Prodia img = Prodia() img_generator = img.generate('Coding bot', amount=3,
+stream=True) img.save(img_generator) ``` ### Advanced Usage of Placeholders The
+`generate` functionality has been enhanced starting from *v0.3.0* to enable
+comprehensive utilization of the `--with-copied` option and support for
+accepting piped inputs. This improvement introduces placeholders, offering
+dynamic values for more versatile interactions. | Placeholder | Represents | |
+------------ | ----------- | | `{{stream}}` | The piped input | | `{{copied}}`
+| The last copied text | This feature is particularly beneficial for intricate
+operations. For example: ```bash $ git diff | pytgpt generate "Here is a diff
+file: {{stream}} Make a concise commit message from it, aligning with my commit
+message history: {{copied}}" --shell --new ``` > In this illustration, `{
+{stream}}` denotes the result of the `$ git diff` operation, while `{{copied}}`
+signifies the content copied from the output of the `$ git log` command. ###
+Awesome Prompts [These prompts](https://github.com/Simatwa/gpt-cli/blob/main/
+assets/all-acts.pdf?raw=True) are designed to guide the AI's behavior or
+responses in a particular direction, encouraging it to exhibit certain
+characteristics or behaviors. The term "awesome-prompt" is not a formal term in
+AI or machine learning literature, but it encapsulates the idea of crafting
+prompts that are effective in achieving desired outcomes. Let's say you want it
+to behave like a *Linux Terminal*, *PHP Interpreter*, or just to [**JAIL
+BREAK.**](https://gist.github.com/coolaj86/6f4f7b30129b0251f61fa7baaa881516)
+Instances : ```sh $ pytgpt interactve --awesome-prompt "Linux Terminal" # Act
+like a Linux Terminal $ pytgpt interactive -ap DAN # Jailbreak ``` > [!NOTE] >
+Awesome prompts are alternative to `--intro`. > Run `$ pytgpt awesome whole` to
+list available prompts (*200+*). > Run `$ pytgpt awesome --help` for more info.
+### Introducing RawDog RawDog is a masterpiece feature that exploits the
+versatile capabilities of Python to command and control your system as per your
+needs. You can literally do anything with it, since it generates and executes
+python codes, driven by **your prompts**! To have a bite of *rawdog* simply
+append the flag `--rawdog` *shortform* `-rd` in *generate/interactive* mode.
+This introduces a never seen-before feature in the *tgpt ecosystem*. Thanks to
 [AbanteAI/rawdog](https://github.com/AbanteAI/rawdog) for the idea. This can be
 useful in some ways. For instance : ```sh $ pytgpt generate -n -q "Visualize
 the disk usage using pie chart" --rawdog ``` This will pop up a window showing
 system disk usage as shown below.
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/Figure_1.png?raw=true]
 ## Passing Environment Variables Pytgpt **v0.4.6** introduces a convention way
 of taking variables from the environment. To achieve that, set the environment
@@ -225,21 +239,24 @@
 the workload of manually checking a working provider each time you fire up
 pytgpt. ## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot) If you're not
 satisfied with the existing interfaces, [pytgpt-bot](https://github.com/
 Simatwa/pytgpt-bot) could be the solution you're seeking. This bot is designed
 to enhance your experience by offering a wide range of functionalities. Whether
 you're interested in engaging in AI-driven conversations, creating images and
 audio from text, or exploring other innovative features, [pytgpt-bot is
-equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot) For more
-usage info run `$ pytgpt --help` ``` Usage: pytgpt [OPTIONS] COMMAND [ARGS]...
-Options: -v, --version Show the version and exit. -h, --help Show this message
-and exit. Commands: api FastAPI control endpoint awesome Perform CRUD
-operations on awesome-prompts generate Generate a quick response with AI
-gpt4free Discover gpt4free models, providers etc imager Generate images with
-pollinations.ai interactive Chat with AI interactively (Default) utils Utility
-endpoint for pytgpt webchatgpt Reverse Engineered ChatGPT Web-Version ``` ###
-API Health Status | No. | API | Status | |--------|-----|--------| | 1. | [On-
-render](https://python-tgpt.onrender.com) | [cron-job](https://
-pqfzhmvz.status.cron-job.org/) | ## [CHANGELOG](https://github.com/Simatwa/
-python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [x] [tgpt]
-(https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://github.com/
-xtekky/gpt4free)
+equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot) The bot is
+maintained as a separate project so you just have to execute a command get it
+installed : ``` $ pip install pytgpt-bot ``` Usage : `pytgpt bot run ` Or you
+can simply interact with the one running now as [@pytgpt-bot](https://t.me/
+pytgpt_bot) For more usage info run `$ pytgpt --help` ``` Usage: pytgpt
+[OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the version and exit. -
+h, --help Show this message and exit. Commands: api FastAPI control endpoint
+awesome Perform CRUD operations on awesome-prompts bot Telegram bot interface
+control generate Generate a quick response with AI gpt4free Discover gpt4free
+models, providers etc imager Generate images with pollinations.ai interactive
+Chat with AI interactively (Default) utils Utility endpoint for pytgpt
+webchatgpt Reverse Engineered ChatGPT Web-Version ``` ### API Health Status |
+No. | API | Status | |--------|-----|--------| | 1. | [On-render](https://
+python-tgpt.onrender.com) | [cron-job](https://pqfzhmvz.status.cron-job.org/) |
+## [CHANGELOG](https://github.com/Simatwa/python-tgpt/blob/main/docs/
+CHANGELOG.md) ## Acknowledgements 1. [x] [tgpt](https://github.com/aandrew-me/
+tgpt) 2. [x] [gpt4free](https://github.com/xtekky/gpt4free)
```

### Comparing `python_tgpt-0.6.9/src/python_tgpt.egg-info/SOURCES.txt` & `python_tgpt-0.7.0/src/python_tgpt.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 LICENSE
 README.md
 setup.py
 src/pytgpt/__init__.py
 src/pytgpt/__main__.py
+src/pytgpt/async_providers.py
 src/pytgpt/base.py
 src/pytgpt/console.py
+src/pytgpt/exceptions.py
 src/pytgpt/utils.py
 src/pytgpt/api/__init__.py
 src/pytgpt/api/__main__.py
 src/pytgpt/api/utils.py
 src/pytgpt/api/v1.py
 src/pytgpt/auto/__init__.py
 src/pytgpt/auto/errors.py
@@ -49,24 +51,25 @@
 src/python_tgpt.egg-info/PKG-INFO
 src/python_tgpt.egg-info/SOURCES.txt
 src/python_tgpt.egg-info/dependency_links.txt
 src/python_tgpt.egg-info/entry_points.txt
 src/python_tgpt.egg-info/requires.txt
 src/python_tgpt.egg-info/top_level.txt
 tests/test_api.py
-tests/test_auto.py
-tests/test_blackboxai.py
+tests/test_auto_tgpt.py
+tests/test_blackboxai_tgpt.py
 tests/test_gemini.py
 tests/test_gpt4all.py
-tests/test_gpt4free.py
+tests/test_gpt4free_tgpt.py
 tests/test_groq.py
 tests/test_imager.py
-tests/test_koboldai.py
-tests/test_leo.py
-tests/test_llama2.py
+tests/test_koboldai_tgpt.py
+tests/test_leo_tgpt.py
+tests/test_llama2_tgpt.py
 tests/test_openai.py
-tests/test_opengpt.py
+tests/test_opengpt_tgpt.py
 tests/test_perplexity.py
-tests/test_phind.py
+tests/test_phind_tgpt.py
 tests/test_poe.py
 tests/test_utils.py
-tests/test_webchatgpt.py
+tests/test_webchatgpt.py
+tests/test_yepchat_tgpt.py
```

### Comparing `python_tgpt-0.6.9/tests/test_api.py` & `python_tgpt-0.7.0/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                 "whole": True,
                 "max_tokens": 600,
                 "timeout": 30,
                 "proxy": None,
             },
         )
         resp_dict = resp.json()
-        self.assertEqual(resp_dict["text"], None)
+        self.assertIsNotNone(resp_dict["text"])
         self.assertIsInstance(resp_dict["body"], dict)
 
     def test_text_stream(self):
         """Streaming response"""
         resp = self.client.post(
             "/v1/chat/stream",
             json={
```

### Comparing `python_tgpt-0.6.9/tests/test_imager.py` & `python_tgpt-0.7.0/tests/test_imager.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,9 +18,16 @@
 
     def test_stream(self):
         """Test multiple photo generation"""
         generator = self.imager.generate(self.prompt, amount=2, stream=True)
         self.assertIsInstance(generator, Generator)
 
 
+class TestProdia(TestImager):
+    def setUp(self):
+        self.imager = imager.Prodia()
+        self.prompt: str = "hello world"
+
+
+# Tests for AsyncImager and AsyncProdia to be implemented
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `python_tgpt-0.6.9/tests/test_utils.py` & `python_tgpt-0.7.0/tests/test_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
 import os
 from pytgpt.utils import Optimizers
 from pytgpt.utils import Conversation
 from pytgpt.utils import AwesomePrompts
+from pytgpt.utils import Audio
 
 
 class TestOptimizers(unittest.TestCase):
     def setUp(self):
         self.optimizer = Optimizers
         self.prompt = "This is a prompt example"
 
@@ -36,15 +37,17 @@
         if not os.path.exists(self.filepath):
             return ""
         with open(self.filepath) as fh:
             return fh.read()
 
     def test_intro_in_prompt(self):
         """Test intro presence in chat_history"""
-        self.assertEqual(self.intro, self.conversation.chat_history)
+        self.assertIn(
+            self.intro, self.conversation.gen_complete_prompt(self.user_prompt)
+        )
 
     def test_history_based_prompt_generation(self):
         """Test combination of chat_history and new user prompt"""
         new_prompt = self.conversation.gen_complete_prompt(self.user_prompt)
         self.assertIn(self.user_prompt, new_prompt)
 
     def test_update_chat_history(self):
@@ -56,21 +59,28 @@
         self.conversation = Conversation(filepath=self.filepath)
         self.assertTrue(os.path.exists(self.filepath))
         before_history_text = self.get_file_content()
         self.conversation.update_chat_history(self.user_prompt, self.llm_response)
         after_history_text = self.get_file_content()
         self.assertNotEqual(before_history_text, after_history_text)
 
-    def test_prompt_offset_after_long_chat(self):
+    def test_chat_history_offset(self):
         """Test truncating lengthy chats"""
-        self.conversation.history_offset = 30
-        for _ in range(5):
+        maximum_chat_length = 400
+        range_amount = (
+            int(maximum_chat_length / (len(self.user_prompt) + len(self.llm_response)))
+            + 10
+        )
+        self.conversation.history_offset = maximum_chat_length
+        for _ in range(range_amount):
             self.conversation.update_chat_history(self.user_prompt, self.llm_response)
-        generated_prompt = self.conversation.gen_complete_prompt(self.user_prompt)
-        self.assertEqual(self.conversation.chat_history, generated_prompt)
+        incomplete_conversation = self.conversation.gen_complete_prompt(
+            self.user_prompt
+        )
+        self.assertTrue(len(incomplete_conversation) < maximum_chat_length)
 
     def tearDown(self):
         if os.path.exists(self.filepath):
             os.remove(self.filepath)
 
 
 class TestAwesomePrompt(unittest.TestCase):
@@ -108,9 +118,31 @@
         """Test get_act raises KeyError"""
         with self.assertRaises(KeyError):
             self.awesome.get_act(
                 "Som ranDom sTrInG here", default=None, raise_not_found=True
             )
 
 
+class TestAudio(unittest.TestCase):
+    """Text to speech synthesis"""
+
+    def setUp(self):
+        self.audio_generator = Audio()
+        self.text = "This is a speech synthesis test"
+
+    def test_text_to_audio(self):
+        """Speech synthesis"""
+        voice_bytes = self.audio_generator.text_to_audio(
+            self.text,
+        )
+        self.assertIs(type(voice_bytes), bytes)
+
+    def test_text_to_audio_save_to(self):
+        """Save speech to a file"""
+        saved_to = self.audio_generator.text_to_audio(self.text, auto=True)
+        self.assertIsInstance(saved_to, str)
+        self.assertTrue(os.path.exists(saved_to))
+        os.remove(saved_to)
+
+
 if __name__ == "__main__":
     unittest.main()
```


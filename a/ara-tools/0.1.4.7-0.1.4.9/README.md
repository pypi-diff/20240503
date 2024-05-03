# Comparing `tmp/ara-tools-0.1.4.7.tar.gz` & `tmp/ara-tools-0.1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ara-tools-0.1.4.7.tar", last modified: Tue Oct 24 11:42:20 2023, max compression
+gzip compressed data, was "ara-tools-0.1.4.9.tar", last modified: Wed Nov  8 10:40:07 2023, max compression
```

## Comparing `ara-tools-0.1.4.7.tar` & `ara-tools-0.1.4.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2023-10-24 11:42:20.586434 ara-tools-0.1.4.7/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       39 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/MANIFEST.in
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       55 2023-10-24 11:42:20.586434 ara-tools-0.1.4.7/PKG-INFO
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3041 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/README.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2023-10-24 11:42:20.571434 ara-tools-0.1.4.7/ara_tools/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      361 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/__init__.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2224 2023-10-24 09:52:49.000000 ara-tools-0.1.4.7/ara_tools/__main__.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3409 2023-10-24 11:40:56.000000 ara-tools-0.1.4.7/ara_tools/ara_config.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2517 2023-10-24 11:37:58.000000 ara-tools-0.1.4.7/ara_tools/artefact.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      931 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/classifier.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      108 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/classifier_validator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2661 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/directory_navigator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4761 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/directory_searcher.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1247 2023-10-18 14:43:52.000000 ara-tools-0.1.4.7/ara_tools/file_classifier.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     7213 2023-10-24 10:47:20.000000 ara-tools-0.1.4.7/ara_tools/file_creator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      102 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/filename_validator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3445 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/glossary_generator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3986 2023-10-12 09:37:50.000000 ara-tools-0.1.4.7/ara_tools/template_manager.py
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2023-10-24 11:42:20.581434 ara-tools-0.1.4.7/ara_tools/templates/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     8233 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/agile.artefacts
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2023-10-24 11:42:20.585434 ara-tools-0.1.4.7/ara_tools/templates/specification_breakdown_files/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      893 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/specification_breakdown_files/template.concept.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2117 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/specification_breakdown_files/template.concept_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1471 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/specification_breakdown_files/template.customer.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2284 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/specification_breakdown_files/template.customer_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2340 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/specification_breakdown_files/template.persona.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4194 2023-10-21 11:27:19.000000 ara-tools-0.1.4.7/ara_tools/templates/specification_breakdown_files/template.persona_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      947 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/specification_breakdown_files/template.technology.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2274 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/specification_breakdown_files/template.technology_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      571 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.businessgoal
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      217 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.businessgoal_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      534 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.capability
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      208 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.capability_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      694 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.epic
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      190 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.epic_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      427 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.example
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      199 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.example_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1519 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.feature
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      199 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.feature_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      753 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.issue
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      815 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.keyfeature
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      211 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.keyfeature_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      193 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.steps_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      741 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.story
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      193 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.story_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      475 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.task
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      190 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.task_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      660 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.tasklist
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      202 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.tasklist_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      671 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.vision
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      226 2023-10-11 16:52:57.000000 ara-tools-0.1.4.7/ara_tools/templates/template.vision_exploration.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2023-10-24 11:42:20.573434 ara-tools-0.1.4.7/ara_tools.egg-info/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       55 2023-10-24 11:42:20.000000 ara-tools-0.1.4.7/ara_tools.egg-info/PKG-INFO
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2193 2023-10-24 11:42:20.000000 ara-tools-0.1.4.7/ara_tools.egg-info/SOURCES.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)        1 2023-10-24 11:42:20.000000 ara-tools-0.1.4.7/ara_tools.egg-info/dependency_links.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       47 2023-10-24 11:42:20.000000 ara-tools-0.1.4.7/ara_tools.egg-info/entry_points.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       10 2023-10-24 11:42:20.000000 ara-tools-0.1.4.7/ara_tools.egg-info/top_level.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       38 2023-10-24 11:42:20.586434 ara-tools-0.1.4.7/setup.cfg
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      403 2023-10-24 05:54:03.000000 ara-tools-0.1.4.7/setup.py
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2023-11-08 10:40:07.921014 ara-tools-0.1.4.9/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       39 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/MANIFEST.in
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       55 2023-11-08 10:40:07.921014 ara-tools-0.1.4.9/PKG-INFO
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3338 2023-11-08 10:38:23.000000 ara-tools-0.1.4.9/README.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2023-11-08 10:40:07.903014 ara-tools-0.1.4.9/ara_tools/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      361 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/__init__.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3040 2023-11-08 10:38:23.000000 ara-tools-0.1.4.9/ara_tools/__main__.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3409 2023-11-08 10:38:23.000000 ara-tools-0.1.4.9/ara_tools/ara_config.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2517 2023-11-08 10:38:23.000000 ara-tools-0.1.4.9/ara_tools/artefact.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1857 2023-11-08 10:38:23.000000 ara-tools-0.1.4.9/ara_tools/artefact_link_updater.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3729 2023-11-08 10:38:23.000000 ara-tools-0.1.4.9/ara_tools/artefact_renamer.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1489 2023-11-08 10:38:23.000000 ara-tools-0.1.4.9/ara_tools/classifier.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      108 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/classifier_validator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2660 2023-11-08 10:38:23.000000 ara-tools-0.1.4.9/ara_tools/directory_navigator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4761 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/directory_searcher.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1361 2023-11-08 10:38:23.000000 ara-tools-0.1.4.9/ara_tools/file_classifier.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     7041 2023-11-08 10:38:23.000000 ara-tools-0.1.4.9/ara_tools/file_creator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      102 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/filename_validator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3445 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/glossary_generator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3984 2023-11-08 10:38:23.000000 ara-tools-0.1.4.9/ara_tools/template_manager.py
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2023-11-08 10:40:07.916014 ara-tools-0.1.4.9/ara_tools/templates/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     8233 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/agile.artefacts
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2023-11-08 10:40:07.920014 ara-tools-0.1.4.9/ara_tools/templates/specification_breakdown_files/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      893 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/specification_breakdown_files/template.concept.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2117 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/specification_breakdown_files/template.concept_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1471 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/specification_breakdown_files/template.customer.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2284 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/specification_breakdown_files/template.customer_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2340 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/specification_breakdown_files/template.persona.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4194 2023-11-08 10:38:23.000000 ara-tools-0.1.4.9/ara_tools/templates/specification_breakdown_files/template.persona_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      947 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/specification_breakdown_files/template.technology.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2274 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/specification_breakdown_files/template.technology_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      571 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/template.businessgoal
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      217 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/template.businessgoal_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      534 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/template.capability
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      208 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/template.capability_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      694 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/template.epic
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      190 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/template.epic_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      427 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/template.example
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      199 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/template.example_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1090 2023-11-08 10:38:23.000000 ara-tools-0.1.4.9/ara_tools/templates/template.feature
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      199 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/template.feature_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      753 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/template.issue
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      815 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/template.keyfeature
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      211 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/template.keyfeature_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      193 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/template.steps_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      741 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/template.story
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      193 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/template.story_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      727 2023-11-08 10:38:23.000000 ara-tools-0.1.4.9/ara_tools/templates/template.task
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      190 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/template.task_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      671 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/template.vision
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      226 2023-11-08 10:20:33.000000 ara-tools-0.1.4.9/ara_tools/templates/template.vision_exploration.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2023-11-08 10:40:07.909014 ara-tools-0.1.4.9/ara_tools.egg-info/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       55 2023-11-08 10:40:07.000000 ara-tools-0.1.4.9/ara_tools.egg-info/PKG-INFO
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2167 2023-11-08 10:40:07.000000 ara-tools-0.1.4.9/ara_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)        1 2023-11-08 10:40:07.000000 ara-tools-0.1.4.9/ara_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       47 2023-11-08 10:40:07.000000 ara-tools-0.1.4.9/ara_tools.egg-info/entry_points.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       10 2023-11-08 10:40:07.000000 ara-tools-0.1.4.9/ara_tools.egg-info/top_level.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       38 2023-11-08 10:40:07.921014 ara-tools-0.1.4.9/setup.cfg
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      402 2023-11-08 10:38:23.000000 ara-tools-0.1.4.9/setup.py
```

### Comparing `ara-tools-0.1.4.7/README.md` & `ara-tools-0.1.4.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 - [ara-tool](#ara-tool)
   - [best practices commit and merge and recreate workspace](#best-practices-commit-and-merge-and-recreate-workspace)
   - [test and run during development](#test-and-run-during-development)
   - [build and install locally for testing](#build-and-install-locally-for-testing)
   - [upload to test pypi with test pypi API key](#upload-to-test-pypi-with-test-pypi-api-key)
-  - [upload to live pypi with talsen team production API key](#upload-to-live-pypi-with-talsen-team-production-api-key)
+  - [upload to live pypi with talsen team production API key (from main branch)](#upload-to-live-pypi-with-talsen-team-production-api-key-from-main-branch)
 
 
 # ara-tool
 ## best practices commit and merge and recreate workspace
 1. commit and publish everything in the branch
 2. go to git and merge
 3. destroy old workspace from merged branch from within the working directory
@@ -18,26 +18,28 @@
    > workspace new ara-cmd hans-ara-cmd
 6. switch to new workspace 
    
 ## test and run during development
 1. run `bash deploy.sh`
 2. run `bash login.sh`
 3. --> in container --> for behave BDD tests `bash test-feature.sh` 
+3.a. --> in container --> for only 1 test: behave ara/features/<name>.feature
 4. --> in container --> for unit tests in folder ara_tools `pytest --cov=. --cov-report term-missing tests/ `
 5. --> in container --> example for running a single unit test in ara_tools folder `pytest tests/test_template_manager.py::test_files_created_from_template`
 6. if change is successfull always commit before proceeding with next change
 7. if change was successfully reviewd merge in gitlab: https://git.talsen.team/talsen-products/ara-tool/-/merge_requests/new
 
 ## build and install locally for testing
 1. use `bash local_install.sh` to control local setup procedure
 
 ## upload to test pypi with test pypi API key
 1. run `bash deploy.sh`
 2. run `login.sh`
-3. in `setup.py` increment `version` otherwise upload will fail! 
+3. in `setup.py` and `local_install.sh` increment `version` otherwise upload will fail! 
+3.a merge to staging and continue from a new workspace
 4. from inside container run `python setup.py sdist bdist_wheel`
 5. run the following command: 
 
 ```bash
 twine upload --repository testpypi dist/* --verbose -u __token__ -p pypi-AgENdGVzdC5weXBpLm9yZwIkZGI5YzUyZTUtNDhjMy00NmI3LTgxNmMtY2QwMTRjYjZmZjlmAAIqWzMsImM3ZTM0MDRmLWU1MzUtNDliMi05ZDhiLWQ0NGUyNzlmYTU0MiJdAAAGID-dX7aQZZimTyUQeKPzbP0TlqMEpLQlzRW7VJr1JKab
 ```
 
@@ -45,17 +47,17 @@
 
 
 6. run `python3 -m pip install --index-url https://test.pypi.org/simple/ ara_tools==<VERSION>`
 7. run `ara -h`
 8. if everything has worked (upload, installation and usage) you can now continue to upload the package to pypi (live)
 
 
-## upload to live pypi with talsen team production API key
+## upload to live pypi with talsen team production API key (from main branch)
 1. run `bash deploy.sh`
 2. run `login.sh`
-3. `dist`should still be there from the testupload, do NOT upload to live without previously testing in test pypi!
+3. `dist` folder should still be there from the testupload (otherwise do `python setup.py sdist bdist_wheel` inside the container again), do NOT upload to live without previously testing in test pypi!
 4. Get the API-Key from [nextcloud](https://cloud.talsen.team/apps/keeweb/?open=%2Finfrastructure%2Fpublic-services%2Fapi-keys.kdbx)
 5. Get the Password from Hans or DevOps
 6. run the following command: 
 ```bash
 twine upload dist/* --verbose -u __token__ -p <API-Key>
 ```
```

### Comparing `ara-tools-0.1.4.7/ara_tools/__main__.py` & `ara-tools-0.1.4.9/ara_tools/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,73 @@
-import os
-import sys
-import argparse
-from .file_creator import FileCreator
-from .filename_validator import is_valid_filename
-from .classifier_validator import is_valid_classifier
-from .template_manager import SpecificationBreakdownAspects
-
-def cli():
-    parser = argparse.ArgumentParser(description="Ara tools for creating files and directories.")
-    parser.add_argument("action", help="Action to perform (e.g. 'create', 'delete', 'list')")
-    parser.add_argument("parameter", help="Filename for create/delete action, or tag for list action", nargs="?")
-    parser.add_argument("classifier", help="Classifier for the file to be created or deleted", nargs="?")
-    parser.add_argument("aspect", help="Specification breakdown aspect", nargs="?")
-
-    args = parser.parse_args()
-
-    file_creator = FileCreator()
-
-    if args.action.lower() == "create":
-        if args.parameter and args.classifier and args.aspect:
-            sba = SpecificationBreakdownAspects()
-            try:
-                sba.create(args.parameter, args.classifier, args.aspect)
-            except ValueError as ve:
-                print(f"Error: {ve}")
-                sys.exit(1)
-            return
-        if not is_valid_filename(args.parameter):
-            print("Invalid filename provided. Please provide a valid filename.")
-            sys.exit(1)
-
-        if not is_valid_classifier(args.classifier):
-            print("Invalid classifier provided. Please provide a valid classifier.")
-            sys.exit(1)
-
-        template_path = os.path.join(os.path.dirname(__file__), 'templates')
-        print(f"in __main__ file_creator.run called with {args.parameter}, {args.classifier} and {template_path}")
-        file_creator.run(args.parameter, args.classifier, template_path)
-    elif args.action.lower() == "delete":
-        file_creator.delete(args.parameter, args.classifier)
-    elif args.action.lower() == "list":
-        if args.parameter:
-            file_creator.list_files(tag=args.parameter)
-        else:
-            file_creator.list_files()
-    else:
-        print("Invalid action provided. Type ara -h for help")
-        sys.exit(1)
-
-if __name__ == "__main__":
-    cli()
+import os
+import sys
+import argparse
+from .file_creator import FileCreator
+from .artefact_renamer import ArtefactRenamer
+from .filename_validator import is_valid_filename
+from .classifier_validator import is_valid_classifier
+from .template_manager import SpecificationBreakdownAspects
+
+def cli():
+    parser = argparse.ArgumentParser(description="Ara tools for creating files and directories.")
+    parser.add_argument("action", help="Action to perform (e.g. 'create', 'delete', 'list','rename')")
+    parser.add_argument("parameter", help="Filename for create/delete/rename action, or tags for list action", nargs="?")
+    parser.add_argument("classifier", help="Classifier for the file to be created/deleted/renamed", nargs="?")
+    parser.add_argument("aspect", help="Specification breakdown aspect", nargs="?")
+    
+
+    args = parser.parse_args()
+
+    file_creator = FileCreator()
+    artefact_renamer = ArtefactRenamer()
+
+    if args.action.lower() == "create":
+        if args.parameter and args.classifier and args.aspect:
+            sba = SpecificationBreakdownAspects()
+            try:
+                sba.create(args.parameter, args.classifier, args.aspect)
+            except ValueError as ve:
+                print(f"Error: {ve}")
+                sys.exit(1)
+            return
+        if not is_valid_filename(args.parameter):  # Assuming first parameter as filename
+            print("Invalid filename provided. Please provide a valid filename.")
+            sys.exit(1)
+
+        if not is_valid_classifier(args.classifier):
+            print("Invalid classifier provided. Please provide a valid classifier.")
+            sys.exit(1)
+
+        template_path = os.path.join(os.path.dirname(__file__), 'templates')
+        print(f"in __main__ file_creator.run called with {args.parameter}, {args.classifier} and {template_path}")
+        file_creator.run(args.parameter, args.classifier, template_path)
+    elif args.action.lower() == "delete":
+        file_creator.delete(args.parameter, args.classifier)
+
+    elif args.action.lower() == "rename":
+        
+        if not is_valid_filename(args.parameter):  # Assuming first parameter as filename
+            print("Invalid filename provided. Please provide a valid filename.")
+            sys.exit(1)
+
+        if not is_valid_classifier(args.classifier):
+            print("Invalid classifier provided. Please provide a valid classifier.")
+            sys.exit(1)
+
+        if not is_valid_filename(args.aspect):  # Assuming aspect is the new name
+            print("Invalid new filename provided. Please provide a valid filename.")
+            sys.exit(1)
+
+        artefact_renamer.rename(args.parameter,args.aspect, args.classifier)
+        
+    elif args.action.lower() == "list":
+        if args.parameter:
+            tags = args.parameter
+            file_creator.list_files(tags=tags)
+        else:
+            file_creator.list_files()
+    else:
+        print("Invalid action provided. Type ara -h for help")
+        sys.exit(1)
+
+if __name__ == "__main__":
+    cli()
```

### Comparing `ara-tools-0.1.4.7/ara_tools/ara_config.py` & `ara-tools-0.1.4.9/ara_tools/ara_config.py`

 * *Files identical despite different names*

### Comparing `ara-tools-0.1.4.7/ara_tools/artefact.py` & `ara-tools-0.1.4.9/ara_tools/artefact.py`

 * *Files identical despite different names*

### Comparing `ara-tools-0.1.4.7/ara_tools/classifier.py` & `ara-tools-0.1.4.9/ara_tools/classifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,18 +23,37 @@
         "example",
         "feature",
         "task",
         "tasklist",
         "issue",
     ]
 
+    artefact_title = {
+        "vision": "Vision statement",
+        "businessgoal": "Business goal",
+        "capability": "Capability",
+        "keyfeature": "Key feature",
+        "epic": "Epic",
+        "story": "User story",
+        "example": "Example",
+        "feature": "Feature",
+        # Use a non-capturing group for "Task list" or "Task" to ensure the capturing group is consistent
+        "task": "(?:Task list|Task)"
+    }
+
+
+
     @staticmethod
     def get_sub_directory(classifier):
         return Classifier.valid_classifiers.get(classifier)
 
     @staticmethod
     def is_valid_classifier(classifier):
         return classifier in Classifier.valid_classifiers
 
     @staticmethod
     def ordered_classifiers():
         return Classifier.classifier_order
+
+    @staticmethod
+    def get_artefact_title(classifier):
+        return Classifier.artefact_title.get(classifier)
```

### Comparing `ara-tools-0.1.4.7/ara_tools/directory_navigator.py` & `ara-tools-0.1.4.9/ara_tools/directory_navigator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from os.path import join, exists, isdir, dirname, basename
-from .directory_searcher import DirectorySearcher
+from directory_searcher import DirectorySearcher
 
 class DirectoryNavigator:
     def __init__(self, target_directory='ara'):
         self.target_directory = target_directory
 
     def exists(self, dir_path):
         """Check if a directory exists."""
```

### Comparing `ara-tools-0.1.4.7/ara_tools/directory_searcher.py` & `ara-tools-0.1.4.9/ara_tools/directory_searcher.py`

 * *Files identical despite different names*

### Comparing `ara-tools-0.1.4.7/ara_tools/file_classifier.py` & `ara-tools-0.1.4.9/ara_tools/file_classifier.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-from .classifier import Classifier
+from classifier import Classifier
 
 class FileClassifier:
     def __init__(self, file_system):
         self.file_system = file_system
     
-    def classify_files(self, tag=None):
+    def classify_files(self, tags=None):
         files_by_classifier = {classifier: [] for classifier in Classifier.ordered_classifiers()}
 
         for root, _, files in self.file_system.walk("."):
             for file in files:
                 file_path = self.file_system.path.join(root, file)
-                if tag:
-                    # Check if file contains the tag
+                if tags:
                     with open(file_path, 'r') as f:
                         content = f.read()
-                        if tag not in content:
+                        # Ensure all tags are in content
+                        if not all(tag in content for tag in tags):
+                           # print(f"DEBUG: Skipping file {file_path} due to missing tags")
                             continue
                 
                 for classifier in Classifier.ordered_classifiers():
                     if file.endswith(f".{classifier}"):
                         files_by_classifier[classifier].append(file_path)
         return files_by_classifier
-    
+
     def print_classified_files(self, files_by_classifier):
         for classifier, files in files_by_classifier.items():
             if files:
                 print(f"{classifier.capitalize()} files:")
                 for file in files:
                     print(f"  - {file}")
                 print()
```

### Comparing `ara-tools-0.1.4.7/ara_tools/file_creator.py` & `ara-tools-0.1.4.9/ara_tools/file_creator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-import os
-from .classifier import Classifier
-from .file_classifier import FileClassifier
-from .template_manager import DirectoryNavigator
-from pathlib import Path
-import shutil
-from shutil import rmtree
-from shutil import copyfile
-
-class FileCreator:
-        
-    def __init__(self, file_system=None):
-        self.file_system = file_system or os
-
-    def create_artefact_exploration(self, dir_path, template_path, classifier):
-        # print(f"[DEBUG] dir_path: {dir_path}")
-        # print(f"[DEBUG] template_path: {template_path}")
-        # print(f"[DEBUG] classifier: {classifier}")
-
-        if not template_path:
-            raise ValueError("template_path must not be None or empty!")
-
-        if not classifier:
-            raise ValueError("classifier must not be None or empty!")
-
-        # Standard exploration artefact
-        self._copy_template_file(dir_path, template_path, f"template.{classifier}_exploration.md", f"{classifier}_exploration.md")
-
-        # Additional exploration artefact for 'feature' classifier
-        if classifier == 'feature':
-            self._copy_template_file(dir_path, template_path, "template.steps_exploration.md", "steps_exploration.md")
-
-    def _copy_template_file(self, dir_path, template_path, source_name, dest_name):
-        source = Path(template_path) / source_name
-        destination = Path(dir_path) / dest_name
-
-        # print(f"[DEBUG] Constructed destination path: {destination}")
-        # print(f"[DEBUG] Constructed source path: {source}")
-
-        if not source.exists():
-            print("[ERROR] Source file does not exist!")
-            raise FileNotFoundError(f"Source file {source} not found!")
-        
-        if not destination.parent.exists():
-            print("[ERROR] Destination directory does not exist!")
-            raise NotADirectoryError(f"Destination directory {destination.parent} does not exist!")
-
-        # print(f"[DEBUG] Copying file from {source} to {destination}...")
-        copyfile(source, destination)
-        print("[DEBUG] Copy completed.")
-
-
-    def create_file(self, file_path, template_path=None, classifier=None, filename=None):
-        if template_path and classifier:
-            template_file_path = self.file_system.path.join(template_path, f"template.{classifier}")
-            if self.file_system.path.exists(template_file_path):
-                with open(template_file_path, "r") as template_file:
-                    template_content = template_file.read()
-
-                template_content = template_content.replace("<descriptive title>", filename.replace("-", " "))
-
-                with open(file_path, "w") as file:
-                    file.write(template_content)
-            else:
-                with open(file_path, "w") as file:
-                    pass
-        else:
-            with open(file_path, "w") as file:
-                pass
-
-    def create_directory(self, dir_path):
-        self.file_system.makedirs(dir_path, exist_ok=True)
-
-    def template_exists(self, template_path, template_name):
-        if not template_path:
-            return False
-
-        full_path = self.file_system.path.join(template_path, template_name)
-
-        if not self.file_system.path.isfile(full_path):
-            print(f"Template file '{template_name}' not found at: {full_path}")
-            return False
-
-        return True
-
-
-    def run(self, filename, classifier, template_path=None):
-        # make sure this function is always called from the ara top level directory
-        navigator = DirectoryNavigator()
-        navigator.navigate_to_target()
-
-        if not Classifier.is_valid_classifier(classifier):
-            print("Invalid classifier provided. Please provide a valid classifier.")
-            return
-
-        sub_directory = Classifier.get_sub_directory(classifier)
-        self.file_system.makedirs(sub_directory, exist_ok=True)
-
-        file_path = self.file_system.path.join(sub_directory, f"{filename}.{classifier}")
-        dir_path = self.file_system.path.join(sub_directory, f"{filename}.data")
-
-        if self.file_system.path.exists(file_path) or self.file_system.path.exists(dir_path):
-            user_choice = input("File or directory already exists. Do you want to overwrite the existing file and directory? (Y/N): ")
-
-            if user_choice.lower() != "y":
-                print("No changes were made to the existing file and directory.")
-                return
-
-        template_name = f"template.{classifier}"
-        if template_path and not self.template_exists(template_path, template_name):
-            print(f"Template file '{template_name}' not found in the specified template path.")
-            return
-
-        
-
-        self.create_file(file_path, template_path, classifier, filename)
-        self.create_directory(dir_path)
-        self.create_artefact_exploration(dir_path, template_path, classifier)
-
-        print(f"Created file: {file_path}")
-        print(f"Created directory: {dir_path}")
-        print(f"Created artefact exploration: {dir_path}/{classifier}_exploration.md")
-
-    def delete(self, filename, classifier):
-        # print(f"DEBUG: Starting delete function...")  # DEBUG PRINT
-        
-        # make sure this function is always called from the ara top level directory
-        navigator = DirectoryNavigator()
-        navigator.navigate_to_target()
-
-        if not Classifier.is_valid_classifier(classifier):
-            print("Invalid classifier provided. Please provide a valid classifier.")
-            return
-
-        sub_directory = Classifier.get_sub_directory(classifier)
-        # print(f"DEBUG: Subdirectory determined: {sub_directory}")  # DEBUG PRINT
-
-        file_path = self.file_system.path.join(sub_directory, f"{filename}.{classifier}")
-        dir_path = self.file_system.path.join(sub_directory, f"{filename}.data")
-
-        # print(f"DEBUG: File path to delete: {file_path}")  # DEBUG PRINT
-        # print(f"DEBUG: Directory path to delete: {dir_path}")  # DEBUG PRINT
-
-        if not self.file_system.path.exists(file_path) or not self.file_system.path.exists(dir_path):
-            print("File or directory not found.")
-            return
-
-        user_choice = input("Are you sure you want to delete the file and directory? (Y/N): ")
-
-        if user_choice.lower() != "y":
-            print("No changes were made.")
-            return
-
-        # print(f"DEBUG: Proceeding to delete...")  # DEBUG PRINT
-
-        self.file_system.remove(file_path)
-        shutil.rmtree(dir_path)
-
-        print(f"Deleted file: {file_path}")
-        print(f"Deleted directory: {dir_path}")
-
-        # print(f"DEBUG: Deletion completed.")  # DEBUG PRINT
-
-    def list_files(self, tag=None):
-        # make sure this function is always called from the ara top level directory
-        navigator = DirectoryNavigator()
-        navigator.navigate_to_target()
-        
-        file_classifier = FileClassifier(self.file_system)
-        classified_files = file_classifier.classify_files(tag=tag)
-        file_classifier.print_classified_files(classified_files)
+import os
+from classifier import Classifier
+from file_classifier import FileClassifier
+from template_manager import DirectoryNavigator
+from pathlib import Path
+import shutil
+from shutil import rmtree
+from shutil import copyfile
+
+class FileCreator:
+        
+    def __init__(self, file_system=None):
+        self.file_system = file_system or os
+
+    def create_artefact_exploration(self, dir_path, template_path, classifier):
+        # print(f"[DEBUG] dir_path: {dir_path}")
+        # print(f"[DEBUG] template_path: {template_path}")
+        # print(f"[DEBUG] classifier: {classifier}")
+
+        if not template_path:
+            raise ValueError("template_path must not be None or empty!")
+
+        if not classifier:
+            raise ValueError("classifier must not be None or empty!")
+
+        # Standard exploration artefact
+        self._copy_template_file(dir_path, template_path, f"template.{classifier}_exploration.md", f"{classifier}_exploration.md")
+
+        # Additional exploration artefact for 'feature' classifier
+        if classifier == 'feature':
+            self._copy_template_file(dir_path, template_path, "template.steps_exploration.md", "steps_exploration.md")
+
+    def _copy_template_file(self, dir_path, template_path, source_name, dest_name):
+        source = Path(template_path) / source_name
+        destination = Path(dir_path) / dest_name
+
+        # print(f"[DEBUG] Constructed destination path: {destination}")
+        # print(f"[DEBUG] Constructed source path: {source}")
+
+        if not source.exists():
+            print("[ERROR] Source file does not exist!")
+            raise FileNotFoundError(f"Source file {source} not found!")
+        
+        if not destination.parent.exists():
+            print("[ERROR] Destination directory does not exist!")
+            raise NotADirectoryError(f"Destination directory {destination.parent} does not exist!")
+
+        # print(f"[DEBUG] Copying file from {source} to {destination}...")
+        copyfile(source, destination)
+        print("[DEBUG] Copy completed.")
+
+
+    def create_file(self, file_path, template_path=None, classifier=None, filename=None):
+        if template_path and classifier:
+            template_file_path = self.file_system.path.join(template_path, f"template.{classifier}")
+            if self.file_system.path.exists(template_file_path):
+                with open(template_file_path, "r") as template_file:
+                    template_content = template_file.read()
+
+                template_content = template_content.replace("<descriptive title>", filename.replace("-", " "))
+
+                with open(file_path, "w") as file:
+                    file.write(template_content)
+            else:
+                with open(file_path, "w") as file:
+                    pass
+        else:
+            with open(file_path, "w") as file:
+                pass
+
+    def create_directory(self, dir_path):
+        self.file_system.makedirs(dir_path, exist_ok=True)
+
+    def template_exists(self, template_path, template_name):
+        if not template_path:
+            return False
+
+        full_path = self.file_system.path.join(template_path, template_name)
+
+        if not self.file_system.path.isfile(full_path):
+            print(f"Template file '{template_name}' not found at: {full_path}")
+            return False
+
+        return True
+
+
+    def run(self, filename, classifier, template_path=None):
+        # make sure this function is always called from the ara top level directory
+        navigator = DirectoryNavigator()
+        navigator.navigate_to_target()
+
+        if not Classifier.is_valid_classifier(classifier):
+            print("Invalid classifier provided. Please provide a valid classifier.")
+            return
+
+        sub_directory = Classifier.get_sub_directory(classifier)
+        self.file_system.makedirs(sub_directory, exist_ok=True)
+
+        file_path = self.file_system.path.join(sub_directory, f"{filename}.{classifier}")
+        dir_path = self.file_system.path.join(sub_directory, f"{filename}.data")
+
+        if self.file_system.path.exists(file_path) or self.file_system.path.exists(dir_path):
+            user_choice = input("File or directory already exists. Do you want to overwrite the existing file and directory? (Y/N): ")
+
+            if user_choice.lower() != "y":
+                print("No changes were made to the existing file and directory.")
+                return
+
+        template_name = f"template.{classifier}"
+        if template_path and not self.template_exists(template_path, template_name):
+            print(f"Template file '{template_name}' not found in the specified template path.")
+            return
+
+        
+
+        self.create_file(file_path, template_path, classifier, filename)
+        self.create_directory(dir_path)
+        self.create_artefact_exploration(dir_path, template_path, classifier)
+
+        print(f"Created file: {file_path}")
+        print(f"Created directory: {dir_path}")
+        print(f"Created artefact exploration: {dir_path}/{classifier}_exploration.md")
+
+    def delete(self, filename, classifier):
+        # print(f"DEBUG: Starting delete function...")  # DEBUG PRINT
+        
+        # make sure this function is always called from the ara top level directory
+        navigator = DirectoryNavigator()
+        navigator.navigate_to_target()
+
+        if not Classifier.is_valid_classifier(classifier):
+            print("Invalid classifier provided. Please provide a valid classifier.")
+            return
+
+        sub_directory = Classifier.get_sub_directory(classifier)
+        # print(f"DEBUG: Subdirectory determined: {sub_directory}")  # DEBUG PRINT
+
+        file_path = self.file_system.path.join(sub_directory, f"{filename}.{classifier}")
+        dir_path = self.file_system.path.join(sub_directory, f"{filename}.data")
+
+        # print(f"DEBUG: File path to delete: {file_path}")  # DEBUG PRINT
+        # print(f"DEBUG: Directory path to delete: {dir_path}")  # DEBUG PRINT
+
+        if not self.file_system.path.exists(file_path) or not self.file_system.path.exists(dir_path):
+            print("File or directory not found.")
+            return
+
+        user_choice = input("Are you sure you want to delete the file and directory? (Y/N): ")
+
+        if user_choice.lower() != "y":
+            print("No changes were made.")
+            return
+
+        # print(f"DEBUG: Proceeding to delete...")  # DEBUG PRINT
+
+        self.file_system.remove(file_path)
+        shutil.rmtree(dir_path)
+
+        print(f"Deleted file: {file_path}")
+        print(f"Deleted directory: {dir_path}")
+
+        # print(f"DEBUG: Deletion completed.")  # DEBUG PRINT
+
+    def list_files(self, tags=None):
+        # make sure this function is always called from the ara top level directory
+        navigator = DirectoryNavigator()
+        navigator.navigate_to_target()
+        
+        file_classifier = FileClassifier(self.file_system)
+        classified_files = file_classifier.classify_files(tags=tags)
+        file_classifier.print_classified_files(classified_files)
```

### Comparing `ara-tools-0.1.4.7/ara_tools/glossary_generator.py` & `ara-tools-0.1.4.9/ara_tools/glossary_generator.py`

 * *Files identical despite different names*

### Comparing `ara-tools-0.1.4.7/ara_tools/template_manager.py` & `ara-tools-0.1.4.9/ara_tools/template_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from pathlib import Path
-from .classifier import Classifier
+from classifier import Classifier
 from shutil import copy
-from .directory_navigator import DirectoryNavigator
+from directory_navigator import DirectoryNavigator
 
 class TemplatePathManager:
     @staticmethod
     def get_template_base_path_aspects():
         """Returns the absolute path to the templates directory."""
         current_file_path = Path(__file__).absolute()  # Get current absolute path
         base_dir = current_file_path.parent  # Get directory of current file
```

### Comparing `ara-tools-0.1.4.7/ara_tools/templates/agile.artefacts` & `ara-tools-0.1.4.9/ara_tools/templates/agile.artefacts`

 * *Files identical despite different names*

### Comparing `ara-tools-0.1.4.7/ara_tools/templates/specification_breakdown_files/template.concept.md` & `ara-tools-0.1.4.9/ara_tools/templates/specification_breakdown_files/template.concept.md`

 * *Files identical despite different names*

### Comparing `ara-tools-0.1.4.7/ara_tools/templates/specification_breakdown_files/template.concept_exploration.md` & `ara-tools-0.1.4.9/ara_tools/templates/specification_breakdown_files/template.concept_exploration.md`

 * *Files identical despite different names*

### Comparing `ara-tools-0.1.4.7/ara_tools/templates/specification_breakdown_files/template.customer.md` & `ara-tools-0.1.4.9/ara_tools/templates/specification_breakdown_files/template.customer.md`

 * *Files identical despite different names*

### Comparing `ara-tools-0.1.4.7/ara_tools/templates/specification_breakdown_files/template.customer_exploration.md` & `ara-tools-0.1.4.9/ara_tools/templates/specification_breakdown_files/template.customer_exploration.md`

 * *Files identical despite different names*

### Comparing `ara-tools-0.1.4.7/ara_tools/templates/specification_breakdown_files/template.persona.md` & `ara-tools-0.1.4.9/ara_tools/templates/specification_breakdown_files/template.persona.md`

 * *Files identical despite different names*

### Comparing `ara-tools-0.1.4.7/ara_tools/templates/specification_breakdown_files/template.persona_exploration.md` & `ara-tools-0.1.4.9/ara_tools/templates/specification_breakdown_files/template.persona_exploration.md`

 * *Files identical despite different names*

### Comparing `ara-tools-0.1.4.7/ara_tools/templates/specification_breakdown_files/template.technology.md` & `ara-tools-0.1.4.9/ara_tools/templates/specification_breakdown_files/template.technology.md`

 * *Files identical despite different names*

### Comparing `ara-tools-0.1.4.7/ara_tools/templates/specification_breakdown_files/template.technology_exploration.md` & `ara-tools-0.1.4.9/ara_tools/templates/specification_breakdown_files/template.technology_exploration.md`

 * *Files identical despite different names*

### Comparing `ara-tools-0.1.4.7/ara_tools/templates/template.businessgoal` & `ara-tools-0.1.4.9/ara_tools/templates/template.businessgoal`

 * *Files identical despite different names*

### Comparing `ara-tools-0.1.4.7/ara_tools/templates/template.capability` & `ara-tools-0.1.4.9/ara_tools/templates/template.capability`

 * *Files identical despite different names*

### Comparing `ara-tools-0.1.4.7/ara_tools/templates/template.epic` & `ara-tools-0.1.4.9/ara_tools/templates/template.epic`

 * *Files identical despite different names*

### Comparing `ara-tools-0.1.4.7/ara_tools/templates/template.issue` & `ara-tools-0.1.4.9/ara_tools/templates/template.issue`

 * *Files identical despite different names*

### Comparing `ara-tools-0.1.4.7/ara_tools/templates/template.keyfeature` & `ara-tools-0.1.4.9/ara_tools/templates/template.keyfeature`

 * *Files identical despite different names*

### Comparing `ara-tools-0.1.4.7/ara_tools/templates/template.story` & `ara-tools-0.1.4.9/ara_tools/templates/template.story`

 * *Files identical despite different names*

### Comparing `ara-tools-0.1.4.7/ara_tools/templates/template.tasklist` & `ara-tools-0.1.4.9/ara_tools/templates/template.task`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
 @tag_name_1 @tag_name_n <optional>
-Task list: <descriptive title of the task list>  
+Task: <descriptive title>  
 
-Contributes to <agile requirement artefact category> <filename or title of the artefact> <(optional in case the contribution is to an artefact that is detailed with rules) using rule <rule as it is formulated>  | blank | filled with text that does not refer to an artefact or rule (then this is a **free task list**) 
+Contributes to <agile requirement artefact category> <filename or title of the artefact> <(optional in case the contribution is to an artefact that is detailed with rules) using rule <rule as it is formulated>  | blank | filled with text that does not refer to an artefact or rule (then this is a free task)
+
+Description (optional): <further optional description to understand the task, no format defined> 
 
 [@tag_name_1 @tag_name_n|<empty>] <list item 1>: <further optional description to understand the item, no format defined>  
-[@tag_name_1 @tag_name_n|<empty>] <list item 2>: <further optional description to understand the item, no format defined>  
+[@tag_name_1 @tag_name_n|<empty>] <list item 2>: <further optional description to understand the item, no format defined>
```

### Comparing `ara-tools-0.1.4.7/ara_tools/templates/template.vision` & `ara-tools-0.1.4.9/ara_tools/templates/template.vision`

 * *Files identical despite different names*

### Comparing `ara-tools-0.1.4.7/ara_tools.egg-info/SOURCES.txt` & `ara-tools-0.1.4.9/ara_tools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 MANIFEST.in
 README.md
 setup.py
 ara_tools/__init__.py
 ara_tools/__main__.py
 ara_tools/ara_config.py
 ara_tools/artefact.py
+ara_tools/artefact_link_updater.py
+ara_tools/artefact_renamer.py
 ara_tools/classifier.py
 ara_tools/classifier_validator.py
 ara_tools/directory_navigator.py
 ara_tools/directory_searcher.py
 ara_tools/file_classifier.py
 ara_tools/file_creator.py
 ara_tools/filename_validator.py
@@ -34,16 +36,14 @@
 ara_tools/templates/template.keyfeature
 ara_tools/templates/template.keyfeature_exploration.md
 ara_tools/templates/template.steps_exploration.md
 ara_tools/templates/template.story
 ara_tools/templates/template.story_exploration.md
 ara_tools/templates/template.task
 ara_tools/templates/template.task_exploration.md
-ara_tools/templates/template.tasklist
-ara_tools/templates/template.tasklist_exploration.md
 ara_tools/templates/template.vision
 ara_tools/templates/template.vision_exploration.md
 ara_tools/templates/specification_breakdown_files/template.concept.md
 ara_tools/templates/specification_breakdown_files/template.concept_exploration.md
 ara_tools/templates/specification_breakdown_files/template.customer.md
 ara_tools/templates/specification_breakdown_files/template.customer_exploration.md
 ara_tools/templates/specification_breakdown_files/template.persona.md
```


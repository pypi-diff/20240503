# Comparing `tmp/pih-answ_auto-0.18.2.tar.gz` & `tmp/pih-answ_auto-0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-answ_auto-0.18.2.tar", last modified: Thu May  2 01:34:41 2024, max compression
+gzip compressed data, was "pih-answ_auto-0.19.tar", last modified: Fri May  3 10:33:10 2024, max compression
```

## Comparing `pih-answ_auto-0.18.2.tar` & `pih-answ_auto-0.19.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 01:34:41.984393 pih-answ_auto-0.18.2/
-drwxrwxrwx   0        0        0        0 2024-05-02 01:34:41.146307 pih-answ_auto-0.18.2/AnswerAutomationService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-answ_auto-0.18.2/AnswerAutomationService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-04-16 00:17:31.000000 pih-answ_auto-0.18.2/AnswerAutomationService/__main__.py
--rw-rw-rw-   0        0        0      414 2024-05-02 01:30:04.000000 pih-answ_auto-0.18.2/AnswerAutomationService/const.py
--rw-rw-rw-   0        0        0     6961 2024-05-02 01:29:52.000000 pih-answ_auto-0.18.2/AnswerAutomationService/service.py
--rw-rw-rw-   0        0        0      285 2024-05-02 01:34:41.953139 pih-answ_auto-0.18.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 01:34:41.903836 pih-answ_auto-0.18.2/pih_answ_auto.egg-info/
--rw-rw-rw-   0        0        0      285 2024-05-02 01:34:39.000000 pih-answ_auto-0.18.2/pih_answ_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2024-05-02 01:34:40.000000 pih-answ_auto-0.18.2/pih_answ_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 01:34:39.000000 pih-answ_auto-0.18.2/pih_answ_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-05-02 01:34:39.000000 pih-answ_auto-0.18.2/pih_answ_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-05-02 01:34:39.000000 pih-answ_auto-0.18.2/pih_answ_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-02 01:34:39.000000 pih-answ_auto-0.18.2/pih_answ_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 01:34:42.000014 pih-answ_auto-0.18.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-03 10:33:10.669137 pih-answ_auto-0.19/
+drwxrwxrwx   0        0        0        0 2024-05-03 10:33:10.261817 pih-answ_auto-0.19/AnswerAutomationService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-answ_auto-0.19/AnswerAutomationService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-04-16 00:17:31.000000 pih-answ_auto-0.19/AnswerAutomationService/__main__.py
+-rw-rw-rw-   0        0        0      412 2024-05-03 10:27:50.000000 pih-answ_auto-0.19/AnswerAutomationService/const.py
+-rw-rw-rw-   0        0        0     6962 2024-05-03 10:16:21.000000 pih-answ_auto-0.19/AnswerAutomationService/service.py
+-rw-rw-rw-   0        0        0      283 2024-05-03 10:33:10.653514 pih-answ_auto-0.19/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 10:33:10.622266 pih-answ_auto-0.19/pih_answ_auto.egg-info/
+-rw-rw-rw-   0        0        0      283 2024-05-03 10:33:09.000000 pih-answ_auto-0.19/pih_answ_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2024-05-03 10:33:10.000000 pih-answ_auto-0.19/pih_answ_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 10:33:09.000000 pih-answ_auto-0.19/pih_answ_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-03 10:33:09.000000 pih-answ_auto-0.19/pih_answ_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-03 10:33:09.000000 pih-answ_auto-0.19/pih_answ_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-03 10:33:09.000000 pih-answ_auto-0.19/pih_answ_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 10:33:10.684762 pih-answ_auto-0.19/setup.cfg
```

### Comparing `pih-answ_auto-0.18.2/AnswerAutomationService/service.py` & `pih-answ_auto-0.19/AnswerAutomationService/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                                             ),
                                             A.S.get(
                                                 A.CT_S.POLIBASE_PERSON_ANSWER_VISIT_MODIFICATION_VARIANTS
                                             ),
                                         ],
                                     ):
                                         if A.D.has_one_of(message, variants):
-                                            answer_type |= 2 ^ (index + 1)
+                                            answer_type |= 2 ** (index + 1)
 
                                     if answer_type == 0:
                                         answer_type = ANSWER_TYPE.VISIT
 
                                     def send_message(value: str) -> None:
                                         A.ME_WH_W_Q.add_message(
                                             Message(
```


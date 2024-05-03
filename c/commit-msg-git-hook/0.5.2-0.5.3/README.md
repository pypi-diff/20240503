# Comparing `tmp/commit_msg_git_hook-0.5.2.tar.gz` & `tmp/commit_msg_git_hook-0.5.3.tar.gz`

## Comparing `commit_msg_git_hook-0.5.2.tar` & `commit_msg_git_hook-0.5.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/__builtins__.pyi
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/__init__.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/commit_msg.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/scan_git.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/setup.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/commit_msg.pot
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/setup.pot
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/commit_msg.mo
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/commit_msg.po
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/setup.mo
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/setup.po
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/templates/commit-msg.config.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/templates/darwin/commit-msg
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/templates/linux/commit-msg
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/templates/win32/commit-msg
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/LICENSE
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/README.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/__builtins__.pyi
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/__init__.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/commit_msg.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/scan_git.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/setup.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/commit_msg.pot
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/setup.pot
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/commit_msg.mo
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/commit_msg.po
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/setup.mo
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/setup.po
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/templates/commit-msg.config.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/templates/darwin/commit-msg
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/templates/linux/commit-msg
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/templates/win32/commit-msg
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/LICENSE
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/README.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/PKG-INFO
```

### Comparing `commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/commit_msg.py` & `commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/commit_msg.py`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/scan_git.py` & `commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/scan_git.py`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/setup.py` & `commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/setup.py`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/commit_msg.mo` & `commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/commit_msg.mo`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/commit_msg.po` & `commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/commit_msg.pot`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-# SOME DESCRIPTIVE TITLE.
-# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
-# This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+# commit-msg git-hook translation.
+# Copyright (C) 2024 Lucio Meira David
+# This file is distributed under the same license as the commit-msg git-hook package.
+# Lucio Meira David <lucio.meira@om30.com.br>, 2024.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
-"Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-05-02 17:11-0300\n"
+"Project-Id-Version: commit_msg_git_hook-0.5.3\n"
+"Report-Msgid-Bugs-To: lucio.meira@om30.com.br\n"
+"POT-Creation-Date: 2024-05-02 18:14-0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Last-Translator: Lucio Meira David <lucio.meira@om30.com.br>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"Language: en\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=CHARSET\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: src/commit_msg_git_hook/commit_msg.py:76
+#: commit_msg.py:80
 msgid "COMMIT MESSAGE TOO LONG"
-msgstr "MENSAGEM DE COMMIT MUITO LONGA"
+msgstr ""
 
-#: src/commit_msg_git_hook/commit_msg.py:78
+#: commit_msg.py:82
 msgid "Configured max length (first line)"
-msgstr "Comprimento máx. configurado (primeira linha)"
+msgstr ""
 
-#: src/commit_msg_git_hook/commit_msg.py:93
+#: commit_msg.py:97
 msgid "INVALID COMMIT MESSAGE"
-msgstr "MENSAGEM DE COMMIT INVÁLIDA"
+msgstr ""
 
-#: src/commit_msg_git_hook/commit_msg.py:95
+#: commit_msg.py:99
 msgid "Use the Conventional Commits specification."
-msgstr "Use a especificação Conventional Commits."
+msgstr ""
 
-#: src/commit_msg_git_hook/commit_msg.py:96
+#: commit_msg.py:100
 msgid "Valid types"
-msgstr "Tipos válidos"
+msgstr ""
 
-#: src/commit_msg_git_hook/commit_msg.py:97
+#: commit_msg.py:101
 msgid "Valid scopes"
-msgstr "Escopos válidos"
+msgstr ""
 
-#: src/commit_msg_git_hook/commit_msg.py:98
+#: commit_msg.py:102
 msgid "See the specification"
-msgstr "Veja a especificação"
+msgstr ""
 
-#: src/commit_msg_git_hook/commit_msg.py:99
+#: commit_msg.py:103
 msgid "https://www.conventionalcommits.org/en/v1.0.0/"
-msgstr "https://www.conventionalcommits.org/pt-br/v1.0.0/"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/setup.mo` & `commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/setup.mo`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/setup.po` & `commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/setup.pot`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# SOME DESCRIPTIVE TITLE.
-# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
-# This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+# commit-msg git-hook translation.
+# Copyright (C) 2024 Lucio Meira David
+# This file is distributed under the same license as the commit-msg git-hook package.
+# Lucio Meira David <lucio.meira@om30.com.br>, 2024.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
-"Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-05-02 17:38-0300\n"
+"Project-Id-Version: commit_msg_git_hook-0.5.3\n"
+"Report-Msgid-Bugs-To: lucio.meira@om30.com.br\n"
+"POT-Creation-Date: 2024-05-02 18:14-0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Last-Translator: Lucio Meira David <lucio.meira@om30.com.br>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"Language: en\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=CHARSET\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: src/commit_msg_git_hook/setup.py:39
+#: setup.py:39
 msgid "Your OS type is"
-msgstr "Seu tipo de OS é"
+msgstr ""
 
-#: src/commit_msg_git_hook/setup.py:79
+#: setup.py:79
 msgid "ERROR: Your OS type is currently unsupported."
-msgstr "ERRO: Seu tipo de OS não é compatível no momento."
+msgstr ""
 
-#: src/commit_msg_git_hook/setup.py:86
+#: setup.py:86
 msgid "Success: commit-msg git-hook configured for"
-msgstr "Sucesso: commit-msg git-hook configurado para"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `commit_msg_git_hook-0.5.2/LICENSE` & `commit_msg_git_hook-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.2/README.md` & `commit_msg_git_hook-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.2/pyproject.toml` & `commit_msg_git_hook-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "commit_msg_git_hook"
-version = "0.5.2"
+version = "0.5.3"
 authors = [
   { name="Lucio Meira David", email="lucio.meira@om30.com.br" },
 ]
 description = "A set of tools to validate git Conventional Commit messages."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `commit_msg_git_hook-0.5.2/PKG-INFO` & `commit_msg_git_hook-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: commit_msg_git_hook
-Version: 0.5.2
+Version: 0.5.3
 Summary: A set of tools to validate git Conventional Commit messages.
 Project-URL: Homepage, https://github.com/OM30/commit-msg-git-hook-package
 Project-URL: Bug Tracker, https://github.com/OM30/commit-msg-git-hook-package/issues
 Author-email: Lucio Meira David <lucio.meira@om30.com.br>
 License-File: LICENSE
 Keywords: ci,commit-msg,git,git hook,git-hook,scan
 Classifier: Development Status :: 4 - Beta
```


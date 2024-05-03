# Comparing `tmp/commit_msg_git_hook-0.5.1.tar.gz` & `tmp/commit_msg_git_hook-0.5.2.tar.gz`

## Comparing `commit_msg_git_hook-0.5.1.tar` & `commit_msg_git_hook-0.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/__builtins__.pyi
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/.vscode/settings.json
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/locales/commit_msg.pot
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/locales/setup.pot
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/locales/pt_BR/LC_MESSAGES/commit_msg.mo
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/locales/pt_BR/LC_MESSAGES/commit_msg.po
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/locales/pt_BR/LC_MESSAGES/setup.mo
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/locales/pt_BR/LC_MESSAGES/setup.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/__init__.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/commit_msg.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/scan_git.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/setup.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/templates/commit-msg.config.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/templates/darwin/commit-msg
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/templates/linux/commit-msg
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/templates/win32/commit-msg
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/LICENSE
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/README.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/__builtins__.pyi
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/__init__.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/commit_msg.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/scan_git.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/setup.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/commit_msg.pot
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/setup.pot
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/commit_msg.mo
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/commit_msg.po
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/setup.mo
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/setup.po
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/templates/commit-msg.config.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/templates/darwin/commit-msg
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/templates/linux/commit-msg
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/templates/win32/commit-msg
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/LICENSE
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/README.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.2/PKG-INFO
```

### Comparing `commit_msg_git_hook-0.5.1/locales/commit_msg.pot` & `commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/commit_msg.po`

 * *Files 12% similar despite different names*

```diff
@@ -4,47 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-05-02 17:37-0300\n"
+"POT-Creation-Date: 2024-05-02 17:11-0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=CHARSET\n"
+"Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: src/commit_msg_git_hook/commit_msg.py:80
+#: src/commit_msg_git_hook/commit_msg.py:76
 msgid "COMMIT MESSAGE TOO LONG"
-msgstr ""
+msgstr "MENSAGEM DE COMMIT MUITO LONGA"
 
-#: src/commit_msg_git_hook/commit_msg.py:82
+#: src/commit_msg_git_hook/commit_msg.py:78
 msgid "Configured max length (first line)"
-msgstr ""
+msgstr "Comprimento máx. configurado (primeira linha)"
 
-#: src/commit_msg_git_hook/commit_msg.py:97
+#: src/commit_msg_git_hook/commit_msg.py:93
 msgid "INVALID COMMIT MESSAGE"
-msgstr ""
+msgstr "MENSAGEM DE COMMIT INVÁLIDA"
 
-#: src/commit_msg_git_hook/commit_msg.py:99
+#: src/commit_msg_git_hook/commit_msg.py:95
 msgid "Use the Conventional Commits specification."
-msgstr ""
+msgstr "Use a especificação Conventional Commits."
 
-#: src/commit_msg_git_hook/commit_msg.py:100
+#: src/commit_msg_git_hook/commit_msg.py:96
 msgid "Valid types"
-msgstr ""
+msgstr "Tipos válidos"
 
-#: src/commit_msg_git_hook/commit_msg.py:101
+#: src/commit_msg_git_hook/commit_msg.py:97
 msgid "Valid scopes"
-msgstr ""
+msgstr "Escopos válidos"
 
-#: src/commit_msg_git_hook/commit_msg.py:102
+#: src/commit_msg_git_hook/commit_msg.py:98
 msgid "See the specification"
-msgstr ""
+msgstr "Veja a especificação"
 
-#: src/commit_msg_git_hook/commit_msg.py:103
+#: src/commit_msg_git_hook/commit_msg.py:99
 msgid "https://www.conventionalcommits.org/en/v1.0.0/"
-msgstr ""
+msgstr "https://www.conventionalcommits.org/pt-br/v1.0.0/"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `commit_msg_git_hook-0.5.1/locales/setup.pot` & `commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/setup.pot`

 * *Files 20% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-05-02 17:38-0300\n"
+"POT-Creation-Date: 2024-05-02 18:14-0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=CHARSET\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: src/commit_msg_git_hook/setup.py:39
+#: setup.py:39
 msgid "Your OS type is"
 msgstr ""
 
-#: src/commit_msg_git_hook/setup.py:79
+#: setup.py:79
 msgid "ERROR: Your OS type is currently unsupported."
 msgstr ""
 
-#: src/commit_msg_git_hook/setup.py:86
+#: setup.py:86
 msgid "Success: commit-msg git-hook configured for"
 msgstr ""
```

### Comparing `commit_msg_git_hook-0.5.1/locales/pt_BR/LC_MESSAGES/commit_msg.mo` & `commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/commit_msg.mo`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.1/locales/pt_BR/LC_MESSAGES/setup.mo` & `commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/setup.mo`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.1/locales/pt_BR/LC_MESSAGES/setup.po` & `commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/setup.po`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/commit_msg.py` & `commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/commit_msg.py`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/scan_git.py` & `commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/scan_git.py`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/setup.py` & `commit_msg_git_hook-0.5.2/src/commit_msg_git_hook/setup.py`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.1/LICENSE` & `commit_msg_git_hook-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.1/README.md` & `commit_msg_git_hook-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.1/pyproject.toml` & `commit_msg_git_hook-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "commit_msg_git_hook"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
   { name="Lucio Meira David", email="lucio.meira@om30.com.br" },
 ]
 description = "A set of tools to validate git Conventional Commit messages."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `commit_msg_git_hook-0.5.1/PKG-INFO` & `commit_msg_git_hook-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: commit_msg_git_hook
-Version: 0.5.1
+Version: 0.5.2
 Summary: A set of tools to validate git Conventional Commit messages.
 Project-URL: Homepage, https://github.com/OM30/commit-msg-git-hook-package
 Project-URL: Bug Tracker, https://github.com/OM30/commit-msg-git-hook-package/issues
 Author-email: Lucio Meira David <lucio.meira@om30.com.br>
 License-File: LICENSE
 Keywords: ci,commit-msg,git,git hook,git-hook,scan
 Classifier: Development Status :: 4 - Beta
```


# Comparing `tmp/commit_msg_git_hook-0.5.3.tar.gz` & `tmp/commit_msg_git_hook-0.5.3.1.tar.gz`

## Comparing `commit_msg_git_hook-0.5.3.tar` & `commit_msg_git_hook-0.5.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/__builtins__.pyi
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/__init__.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/commit_msg.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/scan_git.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/setup.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/commit_msg.pot
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/setup.pot
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/commit_msg.mo
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/commit_msg.po
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/setup.mo
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/setup.po
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/templates/commit-msg.config.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/templates/darwin/commit-msg
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/templates/linux/commit-msg
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/templates/win32/commit-msg
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/LICENSE
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/README.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/__builtins__.pyi
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/__init__.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/commit_msg.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/scan_git.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/setup.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/locales/commit_msg.pot
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/locales/setup.pot
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/commit_msg.mo
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/commit_msg.po
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/setup.mo
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/setup.po
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/templates/commit-msg.config.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/templates/darwin/commit-msg
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/templates/linux/commit-msg
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/templates/win32/commit-msg
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/LICENSE
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/README.md
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.3.1/PKG-INFO
```

### Comparing `commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/commit_msg.py` & `commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/commit_msg.py`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/scan_git.py` & `commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/scan_git.py`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/setup.py` & `commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/setup.py`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/commit_msg.pot` & `commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/locales/commit_msg.pot`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/setup.pot` & `commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/locales/setup.pot`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/commit_msg.mo` & `commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/commit_msg.mo`

 * *Files 19% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,15 +1,15 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
-"Report-Msgid-Bugs-To: \n"
+"Project-Id-Version: commit_msg_git_hook-0.5.3\n"
+"Report-Msgid-Bugs-To: lucio.meira@om30.com.br\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Last-Translator: Lucio Meira David <lucio.meira@om30.com.br>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 msgid "COMMIT MESSAGE TOO LONG"
 msgstr "MENSAGEM DE COMMIT MUITO LONGA"
```

### Comparing `commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/commit_msg.po` & `commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/commit_msg.po`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/setup.mo` & `commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/setup.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,15 +1,15 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
-"Report-Msgid-Bugs-To: \n"
+"Project-Id-Version: commit_msg_git_hook-0.5.3\n"
+"Report-Msgid-Bugs-To: lucio.meira@om30.com.br\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Last-Translator: Lucio Meira David <lucio.meira@om30.com.br>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 msgid "ERROR: Your OS type is currently unsupported."
 msgstr "ERRO: Seu tipo de OS não é compatível no momento."
```

### Comparing `commit_msg_git_hook-0.5.3/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/setup.po` & `commit_msg_git_hook-0.5.3.1/src/commit_msg_git_hook/locales/pt_BR/LC_MESSAGES/setup.po`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.3/LICENSE` & `commit_msg_git_hook-0.5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.3/README.md` & `commit_msg_git_hook-0.5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.3/pyproject.toml` & `commit_msg_git_hook-0.5.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "commit_msg_git_hook"
-version = "0.5.3"
+version = "0.5.3.1"
 authors = [
   { name="Lucio Meira David", email="lucio.meira@om30.com.br" },
 ]
 description = "A set of tools to validate git Conventional Commit messages."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `commit_msg_git_hook-0.5.3/PKG-INFO` & `commit_msg_git_hook-0.5.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: commit_msg_git_hook
-Version: 0.5.3
+Version: 0.5.3.1
 Summary: A set of tools to validate git Conventional Commit messages.
 Project-URL: Homepage, https://github.com/OM30/commit-msg-git-hook-package
 Project-URL: Bug Tracker, https://github.com/OM30/commit-msg-git-hook-package/issues
 Author-email: Lucio Meira David <lucio.meira@om30.com.br>
 License-File: LICENSE
 Keywords: ci,commit-msg,git,git hook,git-hook,scan
 Classifier: Development Status :: 4 - Beta
```


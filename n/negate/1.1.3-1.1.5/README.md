# Comparing `tmp/negate-1.1.3.tar.gz` & `tmp/negate-1.1.5.tar.gz`

## Comparing `negate-1.1.3.tar` & `negate-1.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 negate-1.1.3/.deepsource.toml
--rw-r--r--   0        0        0    13967 2020-02-02 00:00:00.000000 negate-1.1.3/.pylintrc
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 negate-1.1.3/test.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 negate-1.1.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 negate-1.1.3/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0    28134 2020-02-02 00:00:00.000000 negate-1.1.3/img/negate_logo.svg
--rw-r--r--   0        0        0    15816 2020-02-02 00:00:00.000000 negate-1.1.3/img/negate_logo_description.svg
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 negate-1.1.3/negate/__init__.py
--rw-r--r--   0        0        0    40053 2020-02-02 00:00:00.000000 negate-1.1.3/negate/negate.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 negate-1.1.3/negate/py.typed
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 negate-1.1.3/negate/tokens.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 negate-1.1.3/negate/version.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 negate-1.1.3/tests/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 negate-1.1.3/tests/__init__.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 negate-1.1.3/tests/conftest.py
--rw-r--r--   0        0        0    23320 2020-02-02 00:00:00.000000 negate-1.1.3/tests/data.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 negate-1.1.3/tests/requirements.txt
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 negate-1.1.3/tests/test_negate.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 negate-1.1.3/.gitignore
--rw-r--r--   0        0        0    11378 2020-02-02 00:00:00.000000 negate-1.1.3/LICENSE
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 negate-1.1.3/README.md
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 negate-1.1.3/pyproject.toml
--rw-r--r--   0        0        0    22382 2020-02-02 00:00:00.000000 negate-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 negate-1.1.5/.deepsource.toml
+-rw-r--r--   0        0        0    13967 2020-02-02 00:00:00.000000 negate-1.1.5/.pylintrc
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 negate-1.1.5/test.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 negate-1.1.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 negate-1.1.5/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0    28134 2020-02-02 00:00:00.000000 negate-1.1.5/img/negate_logo.svg
+-rw-r--r--   0        0        0    15816 2020-02-02 00:00:00.000000 negate-1.1.5/img/negate_logo_description.svg
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 negate-1.1.5/negate/__init__.py
+-rw-r--r--   0        0        0    41638 2020-02-02 00:00:00.000000 negate-1.1.5/negate/negate.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 negate-1.1.5/negate/py.typed
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 negate-1.1.5/negate/tokens.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 negate-1.1.5/negate/version.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 negate-1.1.5/tests/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 negate-1.1.5/tests/__init__.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 negate-1.1.5/tests/conftest.py
+-rw-r--r--   0        0        0    24064 2020-02-02 00:00:00.000000 negate-1.1.5/tests/data.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 negate-1.1.5/tests/requirements.txt
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 negate-1.1.5/tests/test_negate.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 negate-1.1.5/.gitignore
+-rw-r--r--   0        0        0    11378 2020-02-02 00:00:00.000000 negate-1.1.5/LICENSE
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 negate-1.1.5/README.md
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 negate-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0    22382 2020-02-02 00:00:00.000000 negate-1.1.5/PKG-INFO
```

### Comparing `negate-1.1.3/.pylintrc` & `negate-1.1.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `negate-1.1.3/.github/workflows/run-tests.yml` & `negate-1.1.5/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `negate-1.1.3/img/negate_logo.svg` & `negate-1.1.5/img/negate_logo.svg`

 * *Files identical despite different names*

### Comparing `negate-1.1.3/img/negate_logo_description.svg` & `negate-1.1.5/img/negate_logo_description.svg`

 * *Files identical despite different names*

### Comparing `negate-1.1.3/negate/negate.py` & `negate-1.1.5/negate/negate.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,20 +128,23 @@
         while (negation and first_aux_or_verb
                    and first_aux_or_verb.tag_ not in("VB", "VBG")
                    and negation.i < first_aux_or_verb.i):
             # Search for another negation, if any.
             negation = self._get_negated_child(root, min_index=negation.i+1)
         aux_child = self._get_aux_child(root)
         if negation:
-            remove, add = self._handle_ca_wo(root, aux_child, negation=negation)
+            remove, add = self._handle_ca_wo_sha(root, aux_child, negation=negation)
             # General verbs -> Remove negation and conjugate verb.
             # If there is an AUX child, we need to "unnegate" the AUX instead.
             if (not self._is_aux(root) and root.tag_ not in ("VBN", "VBG")
                     and not aux_child and not self._is_verb_to_do(root)
-                    and not self._is_verb_to_be(root)):
+                    and not self._is_verb_to_be(root)
+                    # The latest spaCy model sometimes misclassifies "shan't".
+                    # This is a temporal workaround.
+                    and not root.text.lower() == "sha"):
                 remove = [root.i, negation.i]
                 add = {root.i: Token(
                     text=self.conjugate_verb(root.text, root.tag_),
                     has_space_after=negation._.has_space_after
                 )}
             # Any other AUX or verb in past participle -> Remove negation.
             elif not remove and not add:
@@ -330,15 +333,15 @@
             prefer_contractions = True
         if fail_on_unsupported is None:
             fail_on_unsupported = self.fail_on_unsupported
 
         negation = self._get_negated_child(aux)
         # If AUX negated -> Remove negation.
         if negation:
-            remove, add = self._handle_ca_wo(aux, negation=negation)
+            remove, add = self._handle_ca_wo_sha(aux, negation=negation)
             if not remove and not add:
                 remove = [aux.i, negation.i]
                 add = Token(
                     text=aux.text,
                     has_space_after=negation._.has_space_after
                 )
             return self._compile_sentence(
@@ -392,28 +395,29 @@
                 )
         return self._compile_sentence(
             doc,
             remove_tokens=remove,
             add_tokens=add
         )
 
-    def _handle_ca_wo(
+    def _handle_ca_wo_sha(
         self,
         *aux_tokens: Optional[SpacyToken],
         negation: SpacyToken
     ) -> Tuple[Optional[List[int]], Optional[Dict[int, Token]]]:
-        """Handle special cases ``"won't"`` and ``"can't"``.
+        """Handle special cases ``"won't"``, ``"can't"`` and ``"shan't"``.
 
         These auxiliary verbs are split into ``"wo"`` (AUX) and ``"n't"`` (neg),
-        and ``"ca"`` (AUX) / ``"n't"`` (neg), respectively. If we simply removed
-        the negation as with other negated auxiliaries (e.g., ``"cannot"`` →
-        ``"can"`` (AUX) / ``"not"`` (neg), we remove ``"not"`` and keep
-        ``"can"``), we would end up with ``"wo"`` and ``"ca"``, which are not
-        correct words. Therefore, we need to take extra steps to replace these
-        words by ``"will"`` and ``"can"``, respectively.
+        ``"ca"`` (AUX) / ``"n't"`` (neg), and ``"sha"`` (AUX) / ``"n't"`` (neg),
+        respectively. If we simply removed the negation as with other negated
+        auxiliaries (e.g., ``"cannot"`` → ``"can"`` (AUX) / ``"not"`` (neg), we
+        remove ``"not"`` and keep ``"can"``), we would end up with ``"wo"``,
+        ``"ca"``, and ``"sha"``which are not correct words. Therefore, we need
+        to take extra steps to replace these words by ``"will"``, ``"can"``, and
+        ``"shall"``respectively.
 
         Args:
             *aux_tokens (:obj:`Optional[SpacyToken]`):
                 The tokens representing auxiliary verbs to consider. Of all the
                 tokens passed, only the first one that actually corresponds to
                 this special case will be processed.
 
@@ -436,30 +440,35 @@
             case, ``(None, None)`` is returned.
         """
         remove = []
         add = {}
         for aux in aux_tokens:
             if not aux:
                 continue
-            # Case AUX "won't" -> Remove negation and replace
-            # "wo" -> "will".
+            # Case AUX "won't" -> Remove negation and replace "wo" -> "will".
             if aux.text.lower() == "wo":
                 remove.append(aux.i)
                 add.update({aux.i: Token(
                     text=" will",
                     has_space_after=negation._.has_space_after
                 )})
-            # Case AUX "can't" -> Remove negation and replace
-            # "ca" -> "can".
+            # Case AUX "can't" -> Remove negation and replace "ca" -> "can".
             elif aux.text.lower() == "ca":
                 remove.append(aux.i)
                 add.update({aux.i: Token(
                     text=" can",
                     has_space_after=negation._.has_space_after
                 )})
+            # Case AUX "shan't" -> Remove negation and replace "sha" -> "shall".
+            elif aux.text.lower() == "sha":
+                remove.append(aux.i)
+                add.update({aux.i: Token(
+                    text=" shall",
+                    has_space_after=negation._.has_space_after
+                )})
             if remove and add:
                 remove.append(negation.i)
                 return remove, add
         return None, None
 
     def _parse(self, string_: str) -> SpacyDoc:
         """Parse a string.
@@ -503,15 +512,19 @@
 
         Returns:
             :obj:`Optional[SpacyToken]`: The chosen entry point (verb), or
             :obj:`None` if the sentence has no root, or contains no verbs.
         """
         if contains_inversion:
             entry_point = [tk for tk in doc
-                           if self._is_aux(tk) or self._is_verb(tk)]
+                           if self._is_aux(tk)
+                           or self._is_verb(tk)
+                           # The latest spaCy model sometimes misclassifies
+                           # "shan't". This is a temporal workaround.
+                           or tk.text.lower() == "sha"]
             if entry_point:
                 return entry_point[0]
         root = self._get_root(doc)
         if root is None:  # nothing we can do
             return None
         # If the root token is not an AUX or a VERB, look for an AUX or
         # VERB in its children.
@@ -789,15 +802,17 @@
         Returns:
             :obj:`bool`: :obj:`True` if the sentence contains an inversion,
             otherwise :obj:`False`.
         """
         aux = None
         pronoun = None
         for tk in doc:
-            if self._is_aux(tk):
+            # The latest spaCy model sometimes misclassifies "shan't". The
+            # additional check here is just a temporal workaround.
+            if self._is_aux(tk) or tk.text.lower() == "sha":
                 aux = tk
             # Only attend to pronouns that don't refer to a noun (i.e., those
             # which could act as subjects).
             if (self._is_pronoun(tk)
                 and not self._is_noun(self._get_parent(tk, doc))):
                 pronoun = tk
             if aux and pronoun:
@@ -934,19 +949,28 @@
             f"en_core_web_trf-{EN_CORE_WEB_TRF_VERSION}" if use_transformers
             else f"en_core_web_md-{EN_CORE_WEB_MD_VERSION}"
         )
         module_name = model_name.split("-")[0]
         try:  # Model installed?
             model_module = importlib.import_module(module_name)
         except ModuleNotFoundError:  # Download and install model.
-            self.logger.info("Downloading model. This only needs to happen "
+            self.logger.info("Downloading spaCy model. This only needs to happen "
                              "once. Please, be patient...")
             with suppress_stdout():
                 spacy.cli.download(model_name, True, False, "-q")
             model_module = importlib.import_module(module_name)
+        spacy_model = model_module.load(**kwargs)
+        installed_model_version: str = spacy_model.meta["version"]
+        expected_version: str = model_name.split("-")[1]
+        if installed_model_version != expected_version:
+            self.logger.info("Updating spaCy model to version %s."
+                             " Please, be patient...", expected_version)
+            with suppress_stdout():
+                spacy.cli.download(model_name, True, False, "-q")
+            model_module = importlib.import_module(module_name)
         return model_module.load(**kwargs)
 
     def _handle_unsupported(self, fail: Optional[bool] = None):
         """Handle behavior upon unsupported sentences.
 
         Args:
             fail (:obj:`Optional[bool]`):
@@ -993,14 +1017,15 @@
                 "'d": " hadn't",
                 "had": "hadn't",
                 "can": "can't",
                 "could": "couldn't",
                 "must": "mustn't",
                 "might": "mightn't",
                 "may": "may not",
+                "shall": "shan't",
                 "should": "shouldn't",
                 "ought": "oughtn't",
                 "'ll": " won't",
                 "will": "won't",
                 "would": "wouldn't"
             },
             False: {
@@ -1022,14 +1047,15 @@
                 "'d": " had not",
                 "had": "had not",
                 "can": "cannot",
                 "could": "could not",
                 "must": "must not",
                 "might": "might not",
                 "may": "may not",
+                "shall": "shall not",
                 "should": "should not",
                 "ought": "ought not",
                 "'ll": " will not",
                 "will": "will not",
                 "would": "would not"
             }
         }
```

### Comparing `negate-1.1.3/negate/tokens.py` & `negate-1.1.5/negate/tokens.py`

 * *Files identical despite different names*

### Comparing `negate-1.1.3/tests/README.md` & `negate-1.1.5/tests/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 ```console
 pytest --transformers
 ```
 
 Remember that to use Transformers, the additional dependencies have to be installed first with:
 ```shell
-pip install -U "negator[transformers]"
+pip install -U "negate[transformers]"
 ```
 
 <br>
 
 Currently, there are several non-passing sentences. These will be marked with
 `XFAIL`. If any of these sentences unexpectedly passed, it would be marked with
 `XPASS`. In this case, please move the sentence from `tests.data.failing` to
```

### Comparing `negate-1.1.3/tests/conftest.py` & `negate-1.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `negate-1.1.3/tests/data.py` & `negate-1.1.5/tests/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 aux_root_affirmative = [
     ("I should.", "I shouldn't.", True),
     ("I should.", "I should not.", False),
     ("I can.", "I can't.", True),
     ("I can.", "I cannot.", False),
     ("I will.", "I won't.", True),
     ("I will.", "I will not.", False),
+    ("I shall.", "I shan't.", True),
+    ("I shall.", "I shall not.", False),
     ("I'm excited.", "I'm not excited.", True),
     ("I'm excited.", "I am not excited.", False),
     ("I am excited.", "I am not excited.", True),
     ("I am excited.", "I am not excited.", False),
     ("I've been excited.", "I haven't been excited.", True),
     ("I've been excited.", "I have not been excited.", False),
     ("I have been excited.", "I haven't been excited.", True),
@@ -71,14 +73,18 @@
     ("I can't.", "I can.", False),
     ("I cannot.", "I can.", True),
     ("I cannot.", "I can.", False),
     ("I won't.", "I will.", True),
     ("I won't.", "I will.", False),
     ("I will not.", "I will.", True),
     ("I will not.", "I will.", False),
+    ("I shan't.", "I shall.", True),
+    ("I shan't.", "I shall.", False),
+    ("I shall not.", "I shall.", True),
+    ("I shall not.", "I shall.", False),
     ("I'm not excited.", "I'm excited.", True),
     ("I'm not excited.", "I'm excited.", False),
     ("I am not excited.", "I am excited.", True),
     ("I am not excited.", "I am excited.", False),
     ("I've not been excited.", "I've been excited.", True),
     ("I've not been excited.", "I've been excited.", False),
     ("I have not been excited.", "I have been excited.", True),
@@ -116,14 +122,16 @@
     ("I should do it.", "I shouldn't do it.", True),
     ("I should do it.", "I should not do it.", False),
     ("You ought to do it.", "You ought not to do it.", False),
     ("I can do it.", "I can't do it.", True),
     ("I can do it.", "I cannot do it.", False),
     ("I will do it.", "I won't do it.", True),
     ("I will do it.", "I will not do it.", False),
+    ("I shall do it.", "I shan't do it.", True),
+    ("I shall do it.", "I shall not do it.", False),
     ("I've done it.", "I haven't done it.", True),
     ("I've done it.", "I have not done it.", False),
     ("I've been doing it.", "I haven't been doing it.", True),
     ("I've been doing it.", "I have not been doing it.", False),
     ("I have done it.", "I haven't done it.", True),
     ("I have done it.", "I have not done it.", False),
     ("I have been doing it.", "I haven't been doing it.", True),
@@ -171,14 +179,18 @@
     ("I can't do it.", "I can do it.", False),
     ("I cannot do it.", "I can do it.", True),
     ("I cannot do it.", "I can do it.", False),
     ("I won't do it.", "I will do it.", True),
     ("I won't do it.", "I will do it.", False),
     ("I will not do it.", "I will do it.", True),
     ("I will no do it.", "I will do it.", False),
+    ("I shan't do it.", "I shall do it.", True),
+    ("I shan't do it.", "I shall do it.", False),
+    ("I shall not do it.", "I shall do it.", True),
+    ("I shall not do it.", "I shall do it.", False),
     ("I've not done it.", "I've done it.", True),
     ("I've not done it.", "I've done it.", False),
     ("I've not been doing it.", "I've been doing it.", True),
     ("I've not been doing it.", "I've been doing it.", False),
     ("I haven't done it.", "I have done it.", True),
     ("I haven't done it.", "I have done it.", False),
     ("I haven't been doing it.", "I have been doing it.", True),
@@ -274,20 +286,22 @@
     ("Has he heard the news?", "Has he not heard the news?", False),
     ("Would you do it?", "Wouldn't you do it?", True),
     ("Should they go?", "Should they not go?", False),
     ("Do you know about it?", "Don't you know about it?", True),
     ("Do you know about it?", "Do you not know about it?", False),
     ("Does she know about it?", "Doesn't she know about it?", True),
     ("Does she know about it?", "Does she not know about it?", False),
-    ("Will it work?", "Will it not work?", False),
     ("Will it work?", "Won't it work?", True),
-    ("Can it work?", "Can it not work?", False),
+    ("Will it work?", "Will it not work?", False),
     ("Can it work?", "Can't it work?", True),
-    ("Could it work?", "Could it not work?", False),
+    ("Can it work?", "Can it not work?", False),
+    ("Shall it work?", "Shan't it work?", True),
+    ("Shall it work?", "Shall it not work?", False),
     ("Could it work?", "Couldn't it work?", True),
+    ("Could it work?", "Could it not work?", False),
     ("Are there many ways it can be done?", "Aren't there many ways it can be done?", True),
     ("Are there many ways it can be done?", "Are there not many ways it can be done?", False),
     ("Little did I know their opinion was so biased.", "Little didn't I know their opinion was so biased.", True),
     ("Little did I know their opinion was so biased.", "Little did I not know their opinion was so biased.", False),
 ]
 
 # Inversions - Negative
@@ -306,18 +320,20 @@
     ("Has he not heard the news?", "Has he heard the news?", True),
     ("Wouldn't you do it?", "Would you do it?", True),
     ("Should they not go?", "Should they go?", False),
     ("Don't you know about it?", "Do you know about it?", True),
     ("Do you not know about it?", "Do you know about it?", False),
     ("Doesn't she know about it?", "Does she know about it?", False),
     ("Does she not know about it?", "Does she know about it?", False),
-    ("Will it not work?", "Will it work?", False),
     ("Won't it work?", "Will it work?", True),
-    ("Can it not work?", "Can it work?", False),
+    ("Will it not work?", "Will it work?", False),
     ("Can't it work?", "Can it work?", True),
+    ("Can it not work?", "Can it work?", False),
+    ("Shan't it work?", "Shall it work?", True),
+    ("Shall it not work?", "Shall it work?", False),
     ("Could it not work?", "Could it work?", False),
     ("Couldn't it work?", "Could it work?", True),
     ("Aren't there many ways it can be done?", "Are there many ways it can be done?", True),
     ("Are there not many ways it can be done?", "Are there many ways it can be done?", False),
     ("Little did I not know their opinion was so biased.", "Little did I know their opinion was so biased.", True),
     ("Little didn't I know their opinion was so biased.", "Little did I know their opinion was so biased.", False),
 ]
```

### Comparing `negate-1.1.3/tests/test_negate.py` & `negate-1.1.5/tests/test_negate.py`

 * *Files identical despite different names*

### Comparing `negate-1.1.3/.gitignore` & `negate-1.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `negate-1.1.3/LICENSE` & `negate-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `negate-1.1.3/README.md` & `negate-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `negate-1.1.3/pyproject.toml` & `negate-1.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `negate-1.1.3/PKG-INFO` & `negate-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: negate
-Version: 1.1.3
+Version: 1.1.5
 Summary: A Python module that negates sentences.
 Project-URL: Homepage, https://github.com/dmlls/negate
 Project-URL: GitHub Issues, https://github.com/dmlls/negate/issues
 Project-URL: GitHub Repo, https://github.com/dmlls/negate
 Author-email: Diego Miguel Lozano <hello@diegomiguel.me>
 Maintainer-email: Diego Miguel Lozano <hello@diegomiguel.me>
 License:
```


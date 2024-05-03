# Comparing `tmp/cim_11_certic-0.6.2.tar.gz` & `tmp/cim_11_certic-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cim_11_certic-0.6.2.tar", max compression
+gzip compressed data, was "cim_11_certic-0.6.3.tar", max compression
```

## Comparing `cim_11_certic-0.6.2.tar` & `cim_11_certic-0.6.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3448 2023-12-18 17:23:25.585872 cim_11_certic-0.6.2/LICENSE.txt
--rw-r--r--   0        0        0     1823 2024-03-12 12:11:37.118412 cim_11_certic-0.6.2/README.md
--rw-r--r--   0        0        0     9235 2024-05-02 09:41:20.185919 cim_11_certic-0.6.2/cim_11/__init__.py
--rw-r--r--   0        0        0 11919360 2024-03-12 10:47:06.046802 cim_11_certic-0.6.2/cim_11/cim-11.sqlite3
--rw-r--r--   0        0        0   403379 2024-05-01 09:48:10.188567 cim_11_certic-0.6.2/cim_11/stopwords.py
--rw-r--r--   0        0        0      534 2024-05-02 09:43:01.248592 cim_11_certic-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 cim_11_certic-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     3448 2023-12-18 17:23:25.585872 cim_11_certic-0.6.3/LICENSE.txt
+-rw-r--r--   0        0        0     1823 2024-03-12 12:11:37.118412 cim_11_certic-0.6.3/README.md
+-rw-r--r--   0        0        0     9204 2024-05-02 09:45:05.128697 cim_11_certic-0.6.3/cim_11/__init__.py
+-rw-r--r--   0        0        0 11919360 2024-03-12 10:47:06.046802 cim_11_certic-0.6.3/cim_11/cim-11.sqlite3
+-rw-r--r--   0        0        0   403379 2024-05-01 09:48:10.188567 cim_11_certic-0.6.3/cim_11/stopwords.py
+-rw-r--r--   0        0        0      534 2024-05-02 09:45:21.067227 cim_11_certic-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 cim_11_certic-0.6.3/PKG-INFO
```

### Comparing `cim_11_certic-0.6.2/LICENSE.txt` & `cim_11_certic-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cim_11_certic-0.6.2/README.md` & `cim_11_certic-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `cim_11_certic-0.6.2/cim_11/__init__.py` & `cim_11_certic-0.6.3/cim_11/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     return items
 
 
 def filter_stopwords(terms: str, lang="fr") -> List[str]:
     wrds = []
     for wrd in terms.replace("'", " ").replace("’", " ").split(" "):
         if wrd not in stopwords.get(lang, []):
-            wrds.append('"' + wrd.replace('"', '""') + '"')
+            wrds.append(wrd)
     return wrds
 
 
 def label_search(
     terms: str, lang="fr", search_type: str = "AND", filter_stopwords=False
 ) -> List[Concept]:
     """
```

### Comparing `cim_11_certic-0.6.2/cim_11/cim-11.sqlite3` & `cim_11_certic-0.6.3/cim_11/cim-11.sqlite3`

 * *Files identical despite different names*

### Comparing `cim_11_certic-0.6.2/cim_11/stopwords.py` & `cim_11_certic-0.6.3/cim_11/stopwords.py`

 * *Files identical despite different names*

### Comparing `cim_11_certic-0.6.2/pyproject.toml` & `cim_11_certic-0.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cim-11-CERTIC"
-version = "0.6.2"
+version = "0.6.3"
 description = "Classification Internationale des Maladies Onzième Révision en français. Données OMS."
 authors = ["Mickaël Desfrênes <mickael.desfrenes@unicaen.fr>", "Arnaud Daret <arnaud.daret@unicaen.fr>"]
 readme = "README.md"
 license = "LICENSE.txt"
 packages = [{include = "cim_11"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cim_11_certic-0.6.2/PKG-INFO` & `cim_11_certic-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cim-11-CERTIC
-Version: 0.6.2
+Version: 0.6.3
 Summary: Classification Internationale des Maladies Onzième Révision en français. Données OMS.
 License: LICENSE.txt
 Author: Mickaël Desfrênes
 Author-email: mickael.desfrenes@unicaen.fr
 Requires-Python: >=3.9
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```


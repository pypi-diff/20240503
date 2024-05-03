# Comparing `tmp/nnfasta-0.1.6.tar.gz` & `tmp/nnfasta-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnfasta-0.1.6.tar", max compression
+gzip compressed data, was "nnfasta-0.1.7.tar", max compression
```

## Comparing `nnfasta-0.1.6.tar` & `nnfasta-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-05-03 00:07:18.824495 nnfasta-0.1.6/LICENSE
--rw-r--r--   0        0        0      802 2024-05-03 05:42:04.544439 nnfasta-0.1.6/README.md
--rw-r--r--   0        0        0       70 2024-05-03 05:27:16.632116 nnfasta-0.1.6/nnfasta/__init__.py
--rw-r--r--   0        0        0     5094 2024-05-03 05:57:53.246317 nnfasta-0.1.6/nnfasta/fasta.py
--rw-r--r--   0        0        0        0 2024-05-03 00:33:29.864485 nnfasta-0.1.6/nnfasta/py.typed
--rw-r--r--   0        0        0      368 2024-05-03 05:58:38.962714 nnfasta-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 nnfasta-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-03 00:07:18.824495 nnfasta-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1118 2024-05-03 06:04:14.677648 nnfasta-0.1.7/README.md
+-rw-r--r--   0        0        0       70 2024-05-03 05:27:16.632116 nnfasta-0.1.7/nnfasta/__init__.py
+-rw-r--r--   0        0        0     5094 2024-05-03 05:57:53.246317 nnfasta-0.1.7/nnfasta/fasta.py
+-rw-r--r--   0        0        0        0 2024-05-03 00:33:29.864485 nnfasta-0.1.7/nnfasta/py.typed
+-rw-r--r--   0        0        0      368 2024-05-03 06:06:16.762719 nnfasta-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1693 1970-01-01 00:00:00.000000 nnfasta-0.1.7/PKG-INFO
```

### Comparing `nnfasta-0.1.6/LICENSE` & `nnfasta-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nnfasta-0.1.6/nnfasta/fasta.py` & `nnfasta-0.1.7/nnfasta/fasta.py`

 * *Files identical despite different names*

### Comparing `nnfasta-0.1.6/PKG-INFO` & `nnfasta-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnfasta
-Version: 0.1.6
+Version: 0.1.7
 Summary: Neural Net efficient Fasta
 License: MIT
 Author: arabidopsis
 Author-email: ian.castleden@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -51,7 +51,24 @@
 print('sequence', rec.id, rec.description, rec.seq)
 ```
 
 **Warning**: No checks are made for the existence of
 the fasta files. Also files of zero length will be rejected
 by `mmap`.
 
+A `Record` mimics biopython's `Record` and is simply:
+
+```python
+@dataclass
+class Record:
+    id: str
+    """Sequence ID"""
+    description: str
+    """Line prefixed by '>'"""
+    seq: str
+    """Sequence stripped of whitespace and uppercased"""
+
+    @property
+    def name(self) -> str:
+        return self.id
+```
+
```


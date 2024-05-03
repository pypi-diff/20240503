# Comparing `tmp/nnfasta-0.1.4.tar.gz` & `tmp/nnfasta-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnfasta-0.1.4.tar", max compression
+gzip compressed data, was "nnfasta-0.1.5.tar", max compression
```

## Comparing `nnfasta-0.1.4.tar` & `nnfasta-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-05-03 00:07:18.824495 nnfasta-0.1.4/LICENSE
--rw-r--r--   0        0        0      675 2024-05-03 00:43:36.614581 nnfasta-0.1.4/README.md
--rw-r--r--   0        0        0       69 2024-05-03 00:23:42.410553 nnfasta-0.1.4/nnfasta/__init__.py
--rw-r--r--   0        0        0     4493 2024-05-03 01:19:49.182374 nnfasta-0.1.4/nnfasta/fasta.py
--rw-r--r--   0        0        0        0 2024-05-03 00:33:29.864485 nnfasta-0.1.4/nnfasta/py.typed
--rw-r--r--   0        0        0      312 2024-05-03 01:24:16.744846 nnfasta-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1228 2024-05-03 01:24:23.163178 nnfasta-0.1.4/setup.py
--rw-r--r--   0        0        0     1148 2024-05-03 01:24:23.163442 nnfasta-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-03 00:07:18.824495 nnfasta-0.1.5/LICENSE
+-rw-r--r--   0        0        0      675 2024-05-03 00:43:36.614581 nnfasta-0.1.5/README.md
+-rw-r--r--   0        0        0       70 2024-05-03 05:27:16.632116 nnfasta-0.1.5/nnfasta/__init__.py
+-rw-r--r--   0        0        0     4549 2024-05-03 05:27:16.760117 nnfasta-0.1.5/nnfasta/fasta.py
+-rw-r--r--   0        0        0        0 2024-05-03 00:33:29.864485 nnfasta-0.1.5/nnfasta/py.typed
+-rw-r--r--   0        0        0      368 2024-05-03 05:29:20.609280 nnfasta-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1250 1970-01-01 00:00:00.000000 nnfasta-0.1.5/PKG-INFO
```

### Comparing `nnfasta-0.1.4/LICENSE` & `nnfasta-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nnfasta-0.1.4/README.md` & `nnfasta-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nnfasta-0.1.4/nnfasta/fasta.py` & `nnfasta-0.1.5/nnfasta/fasta.py`

 * *Files 7% similar despite different names*

```diff
@@ -89,15 +89,18 @@
     @overload
     def __getitem__(self, idx: list[int]) -> list[Record]: ...
     def __getitem__(self, idx: int | slice | list[int]) -> Record | list[Record]:
         if isinstance(idx, int):
             return self.get_idx(idx)
         if isinstance(idx, list):
             return [self.get_idx(i) for i in idx]
-        return [self.get_idx(i) for i in range(idx.start, idx.stop or len(self), idx.step or 1)]
+        return [
+            self.get_idx(i)
+            for i in range(idx.start, idx.stop or len(self), idx.step or 1)
+        ]
 
 
 class CollectionFasta(Sequence[Record]):
     """Multiple memory mapped fasta files"""
 
     def __init__(self, fasta_files: Sequence[os.PathLike], encoding: str | None = None):
         self.fastas = [RandomFasta(f, encoding=encoding) for f in fasta_files]
@@ -138,8 +141,10 @@
     @overload
     def __getitem__(self, idx: list[int]) -> list[Record]: ...
     def __getitem__(self, idx: int | slice | list[int]) -> Record | list[Record]:  # type: ignore
         if isinstance(idx, int):
             return self.get_idx(idx)
         if isinstance(idx, list):
             return [self.get_idx(i) for i in idx]
-        return list(self.get_idxs(range(idx.start, idx.stop or len(self), idx.step or 1)))
+        return list(
+            self.get_idxs(range(idx.start, idx.stop or len(self), idx.step or 1))
+        )
```

### Comparing `nnfasta-0.1.4/PKG-INFO` & `nnfasta-0.1.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: nnfasta
-Version: 0.1.4
+Version: 0.1.5
 Summary: Neural Net efficient Fasta
 License: MIT
 Author: arabidopsis
 Author-email: ian.castleden@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # nnfasta
 
 Neural Net efficient fasta Dataset for Training.
 
 Should be memory efficient across process boundaries.
```


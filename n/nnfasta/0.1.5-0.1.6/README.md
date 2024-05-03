# Comparing `tmp/nnfasta-0.1.5.tar.gz` & `tmp/nnfasta-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnfasta-0.1.5.tar", max compression
+gzip compressed data, was "nnfasta-0.1.6.tar", max compression
```

## Comparing `nnfasta-0.1.5.tar` & `nnfasta-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-05-03 00:07:18.824495 nnfasta-0.1.5/LICENSE
--rw-r--r--   0        0        0      675 2024-05-03 00:43:36.614581 nnfasta-0.1.5/README.md
--rw-r--r--   0        0        0       70 2024-05-03 05:27:16.632116 nnfasta-0.1.5/nnfasta/__init__.py
--rw-r--r--   0        0        0     4549 2024-05-03 05:27:16.760117 nnfasta-0.1.5/nnfasta/fasta.py
--rw-r--r--   0        0        0        0 2024-05-03 00:33:29.864485 nnfasta-0.1.5/nnfasta/py.typed
--rw-r--r--   0        0        0      368 2024-05-03 05:29:20.609280 nnfasta-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1250 1970-01-01 00:00:00.000000 nnfasta-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-03 00:07:18.824495 nnfasta-0.1.6/LICENSE
+-rw-r--r--   0        0        0      802 2024-05-03 05:42:04.544439 nnfasta-0.1.6/README.md
+-rw-r--r--   0        0        0       70 2024-05-03 05:27:16.632116 nnfasta-0.1.6/nnfasta/__init__.py
+-rw-r--r--   0        0        0     5094 2024-05-03 05:57:53.246317 nnfasta-0.1.6/nnfasta/fasta.py
+-rw-r--r--   0        0        0        0 2024-05-03 00:33:29.864485 nnfasta-0.1.6/nnfasta/py.typed
+-rw-r--r--   0        0        0      368 2024-05-03 05:58:38.962714 nnfasta-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 nnfasta-0.1.6/PKG-INFO
```

### Comparing `nnfasta-0.1.5/LICENSE` & `nnfasta-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nnfasta-0.1.5/README.md` & `nnfasta-0.1.6/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -18,20 +18,22 @@
 ```
 
 There are **no** dependencies.
 
 ## Usage
 
 ```python
-
 from nnfasta import nnfastas 
 
-
 dataset = nnfastas(['athaliana.fasta','triticum.fasta','zmays.fasta'])
 
-# display number of sequences
+# display the number of sequences
 print(len(dataset))
 
 # get a particular record
 rec = dataset[20]
 print('sequence', rec.id, rec.description, rec.seq)
 ```
+
+**Warning**: No checks are made for the existence of
+the fasta files. Also files of zero length will be rejected
+by `mmap`.
```

### Comparing `nnfasta-0.1.5/nnfasta/fasta.py` & `nnfasta-0.1.6/nnfasta/fasta.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+import bisect
 import mmap
 import re
 import os
-import bisect
-from dataclasses import dataclass
 from collections.abc import Sequence
+from dataclasses import dataclass
 from typing import Iterator, overload
 
 
 @dataclass
 class Record:
     id: str
+    """Sequence ID"""
     description: str
+    """Line prefixed by '>'"""
     seq: str
+    """Sequence stripped of whitespace and uppercased"""
 
     @property
     def name(self) -> str:
         return self.id
 
 
 PREFIX = re.compile(b"(\n>|\r>|^>)", re.M)
@@ -25,29 +28,44 @@
 
 
 def remove_white(s: bytes) -> bytes:
     return WHITE.sub(b"", s)
 
 
 def nnfastas(
-    fasta_files: Sequence[os.PathLike], encoding: str | None = None
+    fasta_files: Sequence[os.PathLike | str], encoding: str | None = None
 ) -> Sequence[Record]:
+    """Given a sequence of fasta files return an indexable (list like) Fasta object.
+
+    Parameters
+    ----------
+
+    fasta_files: Sequence[PathLike | str]
+        sequence of Fasta files to mmap.
+    encoding: str, optional
+        text encoding of these files [default: ascii]
+
+    Returns
+    -------
+
+    A ``Sequence[Record]`` object.
+    """
     if not fasta_files:
         raise ValueError("no fasta files!")
     if len(fasta_files) == 1:
         return RandomFasta(fasta_files[0], encoding=encoding)
     return CollectionFasta(fasta_files, encoding=encoding)
 
 
 class RandomFasta(Sequence[Record]):
     """Memory mapped fasta file."""
 
     ENCODING = "ascii"
 
-    def __init__(self, fasta_file: os.PathLike, encoding: str | None = None):
+    def __init__(self, fasta_file: os.PathLike | str, encoding: str | None = None):
 
         self.encoding = encoding or self.ENCODING
         self.fp = open(fasta_file, "rb")  # pylint: disable=consider-using-with
         self.fasta = mmap.mmap(self.fp.fileno(), 0, prot=mmap.PROT_READ)
         self.pos = self._find_pos()
 
     def __del__(self):
@@ -98,15 +116,17 @@
             for i in range(idx.start, idx.stop or len(self), idx.step or 1)
         ]
 
 
 class CollectionFasta(Sequence[Record]):
     """Multiple memory mapped fasta files"""
 
-    def __init__(self, fasta_files: Sequence[os.PathLike], encoding: str | None = None):
+    def __init__(
+        self, fasta_files: Sequence[os.PathLike | str], encoding: str | None = None
+    ):
         self.fastas = [RandomFasta(f, encoding=encoding) for f in fasta_files]
         _cumsum = []
         cumsum = 0
         for f in self.fastas:
             cumsum += len(f)
             _cumsum.append(cumsum)
         self._cumsum = _cumsum
@@ -123,14 +143,15 @@
         for idx in idxs:
             yield self._map_idx(idx)
 
     def __len__(self) -> int:
         return self._len
 
     def get_idx(self, idx: int) -> Record:
+        """Given an integer ID return the Record"""
         i, rf = self._map_idx(idx)
         return rf.get_idx(i)
 
     def get_idxs(self, idxs: Sequence[int]) -> Iterator[Record]:
         for i, rf in self._map_idxs(idxs):
             yield rf.get_idx(i)
```


# Comparing `tmp/nnfasta-0.1.0.tar.gz` & `tmp/nnfasta-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnfasta-0.1.0.tar", max compression
+gzip compressed data, was "nnfasta-0.1.1.tar", max compression
```

## Comparing `nnfasta-0.1.0.tar` & `nnfasta-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2024-05-03 00:07:18.824495 nnfasta-0.1.0/LICENSE
--rw-r--r--   0        0        0       58 2024-05-03 00:07:18.824495 nnfasta-0.1.0/README.md
--rw-r--r--   0        0        0       75 2024-05-03 00:14:30.328905 nnfasta-0.1.0/nnfasta/__init__.py
--rw-r--r--   0        0        0     4466 2024-05-03 00:11:32.491051 nnfasta-0.1.0/nnfasta/fasta.py
--rw-r--r--   0        0        0      312 2024-05-03 00:16:49.918347 nnfasta-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 nnfasta-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-03 00:07:18.824495 nnfasta-0.1.1/LICENSE
+-rw-r--r--   0        0        0      547 2024-05-03 00:29:05.753798 nnfasta-0.1.1/README.md
+-rw-r--r--   0        0        0       69 2024-05-03 00:23:42.410553 nnfasta-0.1.1/nnfasta/__init__.py
+-rw-r--r--   0        0        0     4463 2024-05-03 00:23:19.530322 nnfasta-0.1.1/nnfasta/fasta.py
+-rw-r--r--   0        0        0      312 2024-05-03 00:31:16.643106 nnfasta-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 nnfasta-0.1.1/PKG-INFO
```

### Comparing `nnfasta-0.1.0/LICENSE` & `nnfasta-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nnfasta-0.1.0/nnfasta/fasta.py` & `nnfasta-0.1.1/nnfasta/fasta.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 EOL = re.compile(rb"\n|\r", re.I | re.M)
 
 
 def remove_white(s: bytes) -> bytes:
     return WHITE.sub(b"", s)
 
 
-def mmap_fastas(
+def nnfastas(
     fasta_files: Sequence[os.PathLike], encoding: str | None = None
 ) -> Sequence[Record]:
     if not fasta_files:
         raise ValueError("no fasta files!")
     if len(fasta_files) == 1:
         return RandomFasta(fasta_files[0], encoding=encoding)
     return CollectionFasta(fasta_files, encoding=encoding)
```


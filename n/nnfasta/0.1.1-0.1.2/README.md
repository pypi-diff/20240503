# Comparing `tmp/nnfasta-0.1.1.tar.gz` & `tmp/nnfasta-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnfasta-0.1.1.tar", max compression
+gzip compressed data, was "nnfasta-0.1.2.tar", max compression
```

## Comparing `nnfasta-0.1.1.tar` & `nnfasta-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-05-03 00:07:18.824495 nnfasta-0.1.1/LICENSE
--rw-r--r--   0        0        0      547 2024-05-03 00:29:05.753798 nnfasta-0.1.1/README.md
--rw-r--r--   0        0        0       69 2024-05-03 00:23:42.410553 nnfasta-0.1.1/nnfasta/__init__.py
--rw-r--r--   0        0        0     4463 2024-05-03 00:23:19.530322 nnfasta-0.1.1/nnfasta/fasta.py
--rw-r--r--   0        0        0      312 2024-05-03 00:31:16.643106 nnfasta-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 nnfasta-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-03 00:07:18.824495 nnfasta-0.1.2/LICENSE
+-rw-r--r--   0        0        0      675 2024-05-03 00:43:36.614581 nnfasta-0.1.2/README.md
+-rw-r--r--   0        0        0       69 2024-05-03 00:23:42.410553 nnfasta-0.1.2/nnfasta/__init__.py
+-rw-r--r--   0        0        0     4463 2024-05-03 00:23:19.530322 nnfasta-0.1.2/nnfasta/fasta.py
+-rw-r--r--   0        0        0        0 2024-05-03 00:33:29.864485 nnfasta-0.1.2/nnfasta/py.typed
+-rw-r--r--   0        0        0      312 2024-05-03 00:51:24.418887 nnfasta-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1250 1970-01-01 00:00:00.000000 nnfasta-0.1.2/PKG-INFO
```

### Comparing `nnfasta-0.1.1/LICENSE` & `nnfasta-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nnfasta-0.1.1/README.md` & `nnfasta-0.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 # nnfasta
 
 Neural Net efficient fasta Dataset for Training.
 
-Should be efficient across process boundaries etc.
+Should be memory efficient across process boundaries.
 So useful as input to torch/tensorflow dataloaders etc.
 
 Presents a list of fasta files as a simple `abc.Sequence`
 so you can inquire about `len(dataset)` and retrieve
 `Record`s with `dataset[i]`
 
-## Usage
+## Install
 
 Install:
 
 ```bash
 pip install nnfasta
 ```
 
+There are **no** dependencies.
+
+## Usage
+
 ```python
 
 from nnfasta import nnfastas 
 
 
-dataset = nnfastas(['athaliana.fasta','triticum.fasta','zmays.fasta'])`
+dataset = nnfastas(['athaliana.fasta','triticum.fasta','zmays.fasta'])
 
-print(len(datset))
+# display number of sequences
+print(len(dataset))
 
+# get a particular record
 rec = dataset[20]
-print('sequence', rec.seq)
+print('sequence', rec.id, rec.description, rec.seq)
 ```
```

### Comparing `nnfasta-0.1.1/nnfasta/fasta.py` & `nnfasta-0.1.2/nnfasta/fasta.py`

 * *Files identical despite different names*

### Comparing `nnfasta-0.1.1/PKG-INFO` & `nnfasta-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnfasta
-Version: 0.1.1
+Version: 0.1.2
 Summary: Neural Net efficient Fasta
 License: MIT
 Author: arabidopsis
 Author-email: ian.castleden@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,35 +15,41 @@
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # nnfasta
 
 Neural Net efficient fasta Dataset for Training.
 
-Should be efficient across process boundaries etc.
+Should be memory efficient across process boundaries.
 So useful as input to torch/tensorflow dataloaders etc.
 
 Presents a list of fasta files as a simple `abc.Sequence`
 so you can inquire about `len(dataset)` and retrieve
 `Record`s with `dataset[i]`
 
-## Usage
+## Install
 
 Install:
 
 ```bash
 pip install nnfasta
 ```
 
+There are **no** dependencies.
+
+## Usage
+
 ```python
 
 from nnfasta import nnfastas 
 
 
-dataset = nnfastas(['athaliana.fasta','triticum.fasta','zmays.fasta'])`
+dataset = nnfastas(['athaliana.fasta','triticum.fasta','zmays.fasta'])
 
-print(len(datset))
+# display number of sequences
+print(len(dataset))
 
+# get a particular record
 rec = dataset[20]
-print('sequence', rec.seq)
+print('sequence', rec.id, rec.description, rec.seq)
 ```
```


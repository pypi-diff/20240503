# Comparing `tmp/wgse_ng-0.0.2a0.tar.gz` & `tmp/wgse_ng-0.0.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wgse_ng-0.0.2a0.tar", last modified: Thu May  2 13:19:56 2024, max compression
+gzip compressed data, was "wgse_ng-0.0.4a1.tar", last modified: Fri May  3 17:42:43 2024, max compression
```

## Comparing `wgse_ng-0.0.2a0.tar` & `wgse_ng-0.0.4a1.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:19:56.749802 wgse_ng-0.0.2a0/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-02 13:19:56.745802 wgse_ng-0.0.2a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-02 13:19:52.000000 wgse_ng-0.0.2a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:19:56.745802 wgse_ng-0.0.2a0/WGSE_NG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-02 13:19:56.000000 wgse_ng-0.0.2a0/WGSE_NG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-02 13:19:56.000000 wgse_ng-0.0.2a0/WGSE_NG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:19:56.000000 wgse_ng-0.0.2a0/WGSE_NG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 13:19:56.000000 wgse_ng-0.0.2a0/WGSE_NG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 13:19:56.000000 wgse_ng-0.0.2a0/WGSE_NG.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:19:56.749802 wgse_ng-0.0.2a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-02 13:19:52.000000 wgse_ng-0.0.2a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:19:56.745802 wgse_ng-0.0.2a0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-02 13:19:52.000000 wgse_ng-0.0.2a0/test/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-02 13:19:52.000000 wgse_ng-0.0.2a0/test/test_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-02 13:19:52.000000 wgse_ng-0.0.2a0/test/test_fasta_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-02 13:19:52.000000 wgse_ng-0.0.2a0/test/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-02 13:19:52.000000 wgse_ng-0.0.2a0/test/test_unknown_bases_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:19:56.745802 wgse_ng-0.0.2a0/wgse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:19:52.000000 wgse_ng-0.0.2a0/wgse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-05-02 13:19:52.000000 wgse_ng-0.0.2a0/wgse/external.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-02 13:19:52.000000 wgse_ng-0.0.2a0/wgse/genome_file_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-02 13:19:52.000000 wgse_ng-0.0.2a0/wgse/variant_caller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:42:43.882105 wgse_ng-0.0.4a1/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-03 17:42:43.882105 wgse_ng-0.0.4a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-03 17:42:39.000000 wgse_ng-0.0.4a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:42:43.882105 wgse_ng-0.0.4a1/WGSE_NG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-03 17:42:43.000000 wgse_ng-0.0.4a1/WGSE_NG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-03 17:42:43.000000 wgse_ng-0.0.4a1/WGSE_NG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:42:43.000000 wgse_ng-0.0.4a1/WGSE_NG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 17:42:43.000000 wgse_ng-0.0.4a1/WGSE_NG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 17:42:43.000000 wgse_ng-0.0.4a1/WGSE_NG.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:42:43.882105 wgse_ng-0.0.4a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-03 17:42:40.000000 wgse_ng-0.0.4a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:42:43.878105 wgse_ng-0.0.4a1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-03 17:42:40.000000 wgse_ng-0.0.4a1/test/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-03 17:42:40.000000 wgse_ng-0.0.4a1/test/test_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-03 17:42:40.000000 wgse_ng-0.0.4a1/test/test_fasta_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-03 17:42:40.000000 wgse_ng-0.0.4a1/test/test_microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-03 17:42:40.000000 wgse_ng-0.0.4a1/test/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-03 17:42:40.000000 wgse_ng-0.0.4a1/test/test_unknown_bases_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:42:43.882105 wgse_ng-0.0.4a1/wgse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 17:42:40.000000 wgse_ng-0.0.4a1/wgse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-03 17:42:40.000000 wgse_ng-0.0.4a1/wgse/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-05-03 17:42:40.000000 wgse_ng-0.0.4a1/wgse/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-03 17:42:40.000000 wgse_ng-0.0.4a1/wgse/genome_file_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-03 17:42:40.000000 wgse_ng-0.0.4a1/wgse/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 17:42:40.000000 wgse_ng-0.0.4a1/wgse/prerequisites.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-03 17:42:40.000000 wgse_ng-0.0.4a1/wgse/variant_caller.py
```

### Comparing `wgse_ng-0.0.2a0/PKG-INFO` & `wgse_ng-0.0.4a1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: WGSE-NG
-Version: 0.0.2a0
+Version: 0.0.4a1
 Summary: Whole Genome Sequencing data manipulation tool
 Home-page: https://github.com/chaplin89/WGSE-NG
 Author: Multiple
 Author-email: 
 Keywords: bioinformatics
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `wgse_ng-0.0.2a0/README.md` & `wgse_ng-0.0.4a1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 [![Documentation Status](https://readthedocs.org/projects/wgse-ng/badge/?version=latest)](https://wgse-ng.readthedocs.io/en/latest/?badge=latest)
 [![Python application](https://github.com/chaplin89/WGSE-NG/actions/workflows/python-app.yml/badge.svg)](https://github.com/chaplin89/WGSE-NG/actions/workflows/python-app.yml/badge.svg)
 [![Python Publish](https://github.com/chaplin89/WGSE-NG/actions/workflows/python-publish.yml/badge.svg)](https://github.com/chaplin89/WGSE-NG/actions/workflows/python-publish.yml/badge.svg)
 [![Python Publish](https://github.com/chaplin89/WGSE-NG/actions/workflows/python-pyinstaller.yml/badge.svg)](https://github.com/chaplin89/WGSE-NG/actions/workflows/python-pyinstaller.yml/badge.svg)
 
-- [Read the docs](https://wgse-ng.readthedocs.io/en/latest/)
+This is my attempt to improve [WGSE](https://github.com/WGSExtract/WGSExtract-Dev). Still under heavy development. Don't expect anything working.
 
-## Develop/Launch
+## Documentation
+- [Read the docs](https://wgse-ng.readthedocs.io/en/latest/) (pretty much empty at this point)
 
+## Develop/Launch
+_Note: The best experience is with [VS Code](https://code.visualstudio.com/) as this project already contains sensible settings for VS code._
 ```bash
 git clone https://github.com/chaplin89/WGSE-NG
 cd WGSE-NG
 python -m venv .venv
 ./.venv/Scripts/activate
 python -m pip install -r requirements.txt
+python -m pip install -e .
 python main.py
+# If this is run from the terminal of an IDE, 
+# at this point you should restart the IDE as
+# there are some executables that are installed
+# by pip that otherwise won't be found by the IDE.
 ```
 
 ## What's working
 
 - [x] Basic file info extraction
 - [x] Index stats
 - [x] Alignment stats
```

### Comparing `wgse_ng-0.0.2a0/WGSE_NG.egg-info/PKG-INFO` & `wgse_ng-0.0.4a1/WGSE_NG.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: WGSE-NG
-Version: 0.0.2a0
+Version: 0.0.4a1
 Summary: Whole Genome Sequencing data manipulation tool
 Home-page: https://github.com/chaplin89/WGSE-NG
 Author: Multiple
 Author-email: 
 Keywords: bioinformatics
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `wgse_ng-0.0.2a0/setup.py` & `wgse_ng-0.0.4a1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from setuptools import setup
 
-
 DEPENDENCIES = ['setuptools']
 
-# get the version without an import
-VERSION = "0.0.2-alpha"
+VERSION = "0.0.4-alpha1"
 DOC = ""
 
 setup(
     name='WGSE-NG',
     packages=['wgse'],
     author='Multiple',
     author_email='',
     description='Whole Genome Sequencing data manipulation tool',
     long_description='Whole Genome Sequencing data manipulation tool',
     install_requires=DEPENDENCIES,
     entry_points = {},
     url='https://github.com/chaplin89/WGSE-NG',
     version=VERSION,
     classifiers = [
-        'Development Status :: 4 - Beta',
+        'Development Status :: 1 - Planning',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3.12',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
```

### Comparing `wgse_ng-0.0.2a0/test/test_buckets.py` & `wgse_ng-0.0.4a1/test/test_buckets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import pytest
+
 from wgse.fasta.letter_run_buckets import LetterRunBuckets
 from wgse.fasta.letter_run_collection import LetterRunCollection
-import pytest
+
 
 def test_single_bucket():
     # Arrange
     sequence = LetterRunCollection("Foo", 1000)
     sequence.open_run(0)
     sequence.close_run(100)
     # Act
```

### Comparing `wgse_ng-0.0.2a0/test/test_fasta.py` & `wgse_ng-0.0.4a1/test/test_fasta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from wgse.fasta.fasta_letter_counter import FASTALetterCounter
 
 
 class MockFile:
     def __init__(self, lines) -> None:
         self.lines = lines
```

### Comparing `wgse_ng-0.0.2a0/test/test_fasta_dictionary.py` & `wgse_ng-0.0.4a1/test/test_fasta_dictionary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from wgse.data.sorting import Sorting
 from wgse.alignment_map.alignment_map_header import AlignmentMapHeader
+from wgse.data.sorting import Sorting
+
 
 def test_header_parsed_correctly():
     lines = [
         "@HD\tVN:1.0\tSO:coordinate",
     ]
     sut = AlignmentMapHeader(lines)
     assert len(sut.sequences) == 0
```

### Comparing `wgse_ng-0.0.2a0/test/test_sequence.py` & `wgse_ng-0.0.4a1/test/test_sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from wgse.fasta.letter_run_collection import LetterRunCollection
 
 
 def test_sequence_with_invalid_length():
     with pytest.raises(IndexError) as e:
         LetterRunCollection("Foo", 0)
     assert "greater than" in str(e.value)
```

### Comparing `wgse_ng-0.0.2a0/test/test_unknown_bases_stats.py` & `wgse_ng-0.0.4a1/test/test_unknown_bases_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from wgse.fasta.fasta_letter_counter import FASTALetterCounter
 
 
 class MockFile:
     def __init__(self, lines) -> None:
         self.lines = lines
```

### Comparing `wgse_ng-0.0.2a0/wgse/external.py` & `wgse_ng-0.0.4a1/wgse/external.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import enum
-import pathlib
-import subprocess
-import sys
 import os
 import shutil
+import subprocess
+import sys
+from pathlib import Path
+
+from wgse import configuration
 
 if "win" in sys.platform:
     """On windows we expect to find all the 
     executables under .\\3rd_party (if not specified 
     differently). On other OSs the executables need 
     to be under path.
     """
-    third_party = str(pathlib.Path(".", "3rd_party"))
+    third_party = str(Path(".", "3rd_party"))
     if third_party not in os.environ["PATH"]:
         os.environ["PATH"] += ";" + third_party
     if ".JAR" not in os.environ["PATHEXT"]:
         os.environ["PATHEXT"] += ";.JAR"
 
 
 class BgzipAction(enum.Enum):
     Compress = 0
     Decompress = 1
     Reindex = 2
 
 
-def run(f, interpreter=[]):
+def exe(f, interpreter=[]):
     """This decorator will return a function that will try to launch
     an executable from disk that has the same name of the function
     it's decorating, passing the arguments that were received when
     the function was invoked.
 
     Args:
         f (Callable): function to decorate.
@@ -65,87 +67,83 @@
 
     Returns:
         callable: Decorated function
     """
     full_path = shutil.which(f.__name__)
     if full_path is None:
         return f
-    full_path = pathlib.Path(".", full_path)
+    full_path = Path(".", full_path)
     full_path = full_path.with_suffix(".jar")
     f.__name__ = str(full_path)
-    return run(f, ["java", "-jar"])
+    return exe(f, ["java", "-jar"])
 
 
 class External:
     """Wrapper around 3rd party executables"""
 
-    def __init__(self, installation_directory: pathlib.Path = None, threads = None) -> None:
-        if installation_directory is not None:
-            if not installation_directory.exists():
-                raise FileNotFoundError(
-                    f"Unable to find root directory for External: {str(installation_directory)}"
-                )
-            if str(installation_directory) not in os.environ["PATH"]:
-                os.environ["PATH"] += ";" + str(installation_directory)
-        if threads is None:
-            threads = 32
-
-        self.threads = threads
+    def __init__(self, config: configuration.ExternalConfig = configuration.EXTERNAL_CFG) -> None:
+        self._config = config
+        if not self._config.root.exists():
+            raise FileNotFoundError(
+                f"Unable to find root directory for External: {str(self._config.root)}"
+            )
+        if str(self._config.root) not in os.environ["PATH"]:
+            os.environ["PATH"] += ";" + str(self._config.root)
+        
         self._htsfile = "htsfile"
         self._samtools = "samtools"
-        self._bgzip = "bgzip"
         self._gzip = "gzip"
 
-    def get_file_type(self, path: pathlib.Path):
+    def get_file_type(self, path: Path):
         process = subprocess.run([self._htsfile, path], capture_output=True, check=True)
         return process.stdout.decode("utf-8")
 
-    def fasta_index(self, path: pathlib.Path, output: pathlib.Path = None):
+    def fasta_index(self, path: Path, output: Path = None):
         if output is None:
-            output = pathlib.Path(str(path) + ".fai")
+            output = Path(str(path) + ".fai")
 
         arguments = [self._samtools, "faidx", path, "-o", output]
         process = subprocess.run(arguments, check=True, capture_output=True)
         return process.stdout.decode("utf-8")
 
-    def view(self, file: pathlib.Path, output: pathlib.Path, *args):
+    def view(self, file: Path, output: Path, *args):
         arguments = [self._samtools, "view", "-H", "--no-PG", *args, file]
         process = subprocess.run(arguments, check=True, capture_output=True)
         return process.stdout.decode("utf-8")
 
-    def make_dictionary(self, path: pathlib.Path, output: pathlib.Path = None):
+    def make_dictionary(self, path: Path, output: Path = None):
         if output is None:
-            output = pathlib.Path(path.parent, path.name + ".dict")
+            output = Path(path.parent, path.name + ".dict")
         arguments = [self._samtools, "dict", str(path), "-o", str(output)]
         process = subprocess.run(arguments, check=True, capture_output=True)
         return process.stdout.decode("utf-8")
     
-    def index(self, path: pathlib.Path):
-        return self.samtools(["index", "-@", self.threads, "-b", str(path)], wait=True)
+    def index(self, path: Path):
+        return self.samtools(["index", "-@", self._config.threads, "-b", str(path)], wait=True)
 
-    def _gzip_filename(self, input: pathlib.Path, action: BgzipAction):
+    def _gzip_filename(self, input: Path, action: BgzipAction):
         if action == BgzipAction.Compress:
-            return pathlib.Path(str(input) + ".gz")
+            return Path(str(input) + ".gz")
         elif action == BgzipAction.Decompress:
             if len(input.suffixes) == 0:
                 raise RuntimeError(
                     f"Unable to determine decompressed filename, invalid filename {str(input)} (no extensions)."
                 )
             return input.with_suffix("")
         elif action == BgzipAction.Reindex:
-            return pathlib.Path(str(input) + ".gzi")
+            return Path(str(input) + ".gzi")
         else:
             raise RuntimeError(f"Action {action.name} not supported.")
 
     def gzip(
         self,
-        input: pathlib.Path,
-        output: pathlib.Path,
+        input: Path,
+        output: Path,
         action: BgzipAction = BgzipAction.Decompress,
-    ) -> pathlib.Path:
+    ) -> Path:
         if output.exists():
             raise RuntimeError(
                 f"Trying to decompress {str(input)} but the destination file {str(output)} exists."
             )
         inferred_filename = self._gzip_filename(input, action)
 
         action_flags = {BgzipAction.Compress: "", BgzipAction.Decompress: "-d"}
@@ -166,36 +164,36 @@
                 )
 
         if inferred_filename != output:
             inferred_filename.rename(output)
 
     def bgzip_wrapper(
         self,
-        input: pathlib.Path,
-        output: pathlib.Path,
+        input: Path,
+        output: Path,
         action: BgzipAction = BgzipAction.Compress,
-    ) -> pathlib.Path:
+    ) -> Path:
         if output.exists():
             output.unlink()
 
         action_flags = {
             BgzipAction.Compress: "-if",
             BgzipAction.Decompress: "-d",
             BgzipAction.Reindex: "-r",
         }
         inferred_filename = self._gzip_filename(input, action)
 
         out = self.bgzip([action_flags[action], str(input), "-@", "32"], wait=True)
         if inferred_filename != output:
             inferred_filename.rename(output)
             if action == BgzipAction.Compress:
-                inferred_gzi_filename = pathlib.Path(str(inferred_filename) + ".gzi")
+                inferred_gzi_filename = Path(str(inferred_filename) + ".gzi")
                 inferred_gzi_filename.rename(str(output) + ".gzi")
 
-    def idxstats(self, input: pathlib.Path):
+    def idxstats(self, input: Path):
         """Generate BAM index statistics"""
         arguments = [self._samtools, "idxstat", input]
         process = subprocess.run(arguments)
         return process.stdout.decode("utf-8")
 
     def haplogrep_classify(self, vcf_file, output_file):
         output = self.haplogrep(
@@ -203,46 +201,46 @@
             wait=True,
         )
         output.decode("utf-8")
         return output
     
     # Starting from here all the functions are
     # just calling executables with the same name.
-    # See the implementation of run and jar decorator
+    # See the implementation of @exe and @jar decorator
     # for more details.
     
-    @run
+    @exe
     def bgzip(self, args=[], stdout=None, stdin=None, wait=False):
         pass
 
-    @run
+    @exe
     def samtools(self, args=[], stdout=None, stdin=None, wait=False):
         pass
 
-    @run
+    @exe
     def bwa(self, args=[], stdout=None, stdin=None, wait=False):
         pass
 
-    @run
+    @exe
     def bwamem2(self, args=[], stdout=None, stdin=None, wait=False):
         pass
 
-    @run
+    @exe
     def minimap2(self, args=[], stdout=None, stdin=None, wait=False):
         pass
 
-    @run
+    @exe
     def fastp(self, args=[], stdout=None, stdin=None, wait=False):
         pass
 
-    @run
+    @exe
     def bcftool(self, args=[], stdout=None, stdin=None, wait=False):
         pass
 
-    @run
+    @exe
     def tabix(self, args=[], stdout=None, stdin=None, wait=False):
         pass
 
     @jar
     def haplogrep(self, args=[], stdout=None, stdin=None, wait=False):
         pass
```

### Comparing `wgse_ng-0.0.2a0/wgse/genome_file_finder.py` & `wgse_ng-0.0.4a1/wgse/genome_file_finder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import pathlib
+from pathlib import Path
 
-from .utility.file_type_checker import FileTypeChecker
-from .reference_genome.metadata_loader import Genome
+from wgse.reference_genome.metadata_loader import Genome
+from wgse.utility.file_type_checker import FileTypeChecker
 
 
 class GenomeFileFinder:
-    def __init__(self, file_type_checker: FileTypeChecker = FileTypeChecker(), repository = pathlib.Path("repository")) -> None:
+    def __init__(self, file_type_checker: FileTypeChecker = FileTypeChecker(), repository = Path("metadata")) -> None:
         self.temporary_dir = repository.joinpath("temp")
         self.genomes_dir = repository.joinpath("genomes")
         self.file_type_checker = file_type_checker
         
     def find(self, genome: Genome):
         if genome.fasta.exists():
             if genome.bgzip_size == genome.fasta.stat().st_size:
```

### Comparing `wgse_ng-0.0.2a0/wgse/variant_caller.py` & `wgse_ng-0.0.4a1/wgse/variant_caller.py`

 * *Files identical despite different names*


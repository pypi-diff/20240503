# Comparing `tmp/opencf_core-0.2.0.tar.gz` & `tmp/opencf_core-0.2.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencf_core-0.2.0.tar", max compression
+gzip compressed data, was "opencf_core-0.2.1a0.tar", max compression
```

## Comparing `opencf_core-0.2.0.tar` & `opencf_core-0.2.1a0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7078 2024-04-22 20:51:03.106038 opencf_core-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-04-22 20:47:52.871940 opencf_core-0.2.0/opencf_core/__init__.py
--rw-r--r--   0        0        0    18012 2024-04-22 20:47:52.871940 opencf_core-0.2.0/opencf_core/base_converter.py
--rw-r--r--   0        0        0     4510 2024-04-22 20:47:52.871940 opencf_core-0.2.0/opencf_core/converter_app.py
--rw-r--r--   0        0        0    15473 2024-04-22 20:47:52.875939 opencf_core-0.2.0/opencf_core/filetypes.py
--rw-r--r--   0        0        0     5887 2024-04-22 20:47:52.875939 opencf_core-0.2.0/opencf_core/io_handler.py
--rw-r--r--   0        0        0      594 2024-04-22 20:47:52.875939 opencf_core-0.2.0/opencf_core/logger.py
--rw-r--r--   0        0        0     2014 2024-04-22 20:47:52.875939 opencf_core-0.2.0/opencf_core/mimes.py
--rw-r--r--   0        0        0     1137 2024-04-22 20:47:52.875939 opencf_core-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     8323 1970-01-01 00:00:00.000000 opencf_core-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     7078 2024-04-22 20:51:03.106038 opencf_core-0.2.1a0/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 20:47:52.871940 opencf_core-0.2.1a0/opencf_core/__init__.py
+-rw-r--r--   0        0        0    19187 2024-05-03 16:19:35.014300 opencf_core-0.2.1a0/opencf_core/base_converter.py
+-rw-r--r--   0        0        0     6124 2024-05-03 15:57:22.801633 opencf_core-0.2.1a0/opencf_core/converter_app.py
+-rw-r--r--   0        0        0    15473 2024-04-22 20:47:52.875939 opencf_core-0.2.1a0/opencf_core/filetypes.py
+-rw-r--r--   0        0        0     5891 2024-05-03 16:17:36.405376 opencf_core-0.2.1a0/opencf_core/io_handler.py
+-rw-r--r--   0        0        0     2660 2024-05-03 16:20:42.970858 opencf_core-0.2.1a0/opencf_core/logging_config.py
+-rw-r--r--   0        0        0     2014 2024-05-03 16:19:18.558168 opencf_core-0.2.1a0/opencf_core/mimes.py
+-rw-r--r--   0        0        0     1110 2024-05-03 16:28:39.043172 opencf_core-0.2.1a0/pyproject.toml
+-rw-r--r--   0        0        0     8275 1970-01-01 00:00:00.000000 opencf_core-0.2.1a0/PKG-INFO
```

### Comparing `opencf_core-0.2.0/README.md` & `opencf_core-0.2.1a0/README.md`

 * *Files identical despite different names*

### Comparing `opencf_core-0.2.0/opencf_core/base_converter.py` & `opencf_core-0.2.1a0/opencf_core/base_converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 Exceptions:
 - ValueError: Raised when file paths or types are incompatible or unsupported.
 - AssertionError: Ensured for internal consistency checks, confirming that file types match expected values.
 """
 
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import Any, Iterable, List, Optional, Tuple, Union
 
 from .filetypes import EmptySuffixError, FileType
 from .io_handler import FileReader, FileWriter, SamePathReader
-from .logger import logger
+from .logging_config import logger
 
 
 class ResolvedInputFile:
     """
     Handles resolving the file type of a given file or folder, managing path adjustments and optional content reading.
     """
 
@@ -127,15 +127,17 @@
         # Create directory if it doesn't exist
         self.path.mkdir(exist_ok=True)
         resolved_file_type = FileType.from_suffix(file_type, raise_err=True)
         assert resolved_file_type.is_true_filetype()
         suffix = resolved_file_type.get_suffix()
         return resolved_file_type, suffix
 
-    def _resolve_file_type(self, file_type: str, read_content: bool, add_suffix: bool):
+    def _resolve_file_type(
+        self, file_type: Optional[str], read_content: bool, add_suffix: bool
+    ):
         """
         Resolves the file type based on given parameters.
 
         Args:
             file_type (FileType or str, optional): An explicit file type or extension.
             read_content (bool): Indicates if file content should be used to help resolve the file type.
             add_suffix (bool): Whether to append the resolved file type's suffix to the file path.
@@ -151,15 +153,15 @@
         # Optionally add suffix to the file path
         if add_suffix:
             self.path = self.path.with_suffix(suffix)
 
         return resolved_file_type, suffix
 
     def __resolve_filetype__(
-        self, file_type: str, file_path: Path, read_content: bool
+        self, file_type: Optional[str], file_path: Path, read_content: bool
     ) -> FileType:
         """
         Determines the file type, utilizing the provided type, file path, or content as needed.
 
         Args:
             file_type (FileType or str, optional): An explicit file type or extension.
             file_path (str): The path to the file, used if file_type is not provided.
@@ -220,17 +222,17 @@
 
 
 class BaseConverter(ABC):
     """
     Abstract base class for file conversion, defining the template for input to output file conversion.
     """
 
-    file_reader: FileReader = None
-    file_writer: FileWriter = None
-    folder_as_output: bool = None
+    file_reader: Optional[FileReader] = None
+    file_writer: Optional[FileWriter] = None
+    folder_as_output: Optional[bool] = None
 
     def __init__(
         self,
         input_files: Union[ResolvedInputFile, List[ResolvedInputFile]],
         output_file: ResolvedInputFile,
     ):
         """
@@ -260,15 +262,15 @@
         """
         Orchestrates the file conversion process, including reading, converting, and writing the file.
         """
         logger.info("Starting conversion process...")
 
         # log
         logger.debug(
-            f"Converting {self.input_files[0].path.name} and {len(self.input_files)-1} more ({self.get_supported_input_type()}) to {self.output_file.path.name} ({self.get_supported_output_type()})..."
+            f"Converting {self.input_files[0].path.name} and {len(self.input_files)-1} more ({self.get_supported_input_types()}) to {self.output_file.path.name} ({self.get_supported_output_types()})..."
         )
         logger.debug(f"Input files ({len(self.input_files)}): {self.input_files}")
 
         # Read all input files
         logger.info("Reading input file...")
         self._input_contents = [
             self._read_content(input_file.path) for input_file in self.input_files
@@ -315,41 +317,44 @@
         kwargs = {}
         if self.folder_as_output:
             assert (
                 output_path.is_dir()
             ), f"output_path {output_path} is not a dir while a folder is required for this conversion"
             kwargs["output_folder"] = output_path
         else:
-            if output_path.is_dir():
-                suffix = self.get_supported_output_type().get_suffix()
-                output_path = (output_path / "opencf-output").with_suffix(suffix)
+            assert (
+                not output_path.is_dir()
+            ), f"output_path {output_path} exists as a dir while a file is required for this conversion"
+            # if output_path.is_dir():
+            #     suffix = self.get_supported_output_types().get_suffix()
+            #     output_path = (output_path / "opencf-output").with_suffix(suffix)
             kwargs["output_file"] = output_path
         return kwargs, output_path
 
     def _check_file_types(self):
         """
         Validates that the provided files have acceptable and supported file types for conversion.
         """
         for input_file in self.input_files:
             if not isinstance(input_file, ResolvedInputFile):
                 raise ValueError(
                     f"Invalid input file. Expected: {ResolvedInputFile}. Actual: {type(input_file)}"
                 )
-            if input_file.file_type != self.get_supported_input_type():
+            if input_file.file_type not in self.get_supported_input_types():
                 raise ValueError(
-                    f"Unsupported input file type. Expected: {self.get_supported_input_type()}, Actual: {input_file.file_type}"
+                    f"Unsupported input file type. Expected one of the followings: {self.get_supported_input_types()}, Actual: {input_file.file_type}"
                 )
 
         if not isinstance(self.output_file, ResolvedInputFile):
             raise ValueError(
                 f"Invalid output file. Expected: {ResolvedInputFile}. Actual: {type(self.output_file)}"
             )
-        if self.output_file.file_type != self.get_supported_output_type():
+        if self.output_file.file_type not in self.get_supported_output_types():
             raise ValueError(
-                f"Unsupported output file type. Expected: {self.get_supported_output_type()}, Actual: {self.output_file.file_type}"
+                f"Unsupported output file type. Expected one of the followings: {self.get_supported_output_types()}, Actual: {self.output_file.file_type}"
             )
 
     def check_io_handlers(self):
         """
         Ensures that valid I/O handlers (file reader and writer) are set for the conversion.
         """
         if self.file_reader is None:
@@ -367,91 +372,109 @@
 
         if not isinstance(self.file_writer, FileWriter):
             raise ValueError("Invalid file writer")
 
         self.folder_as_output = False
 
     @classmethod
-    def get_input_type(cls):
-        return cls.get_supported_input_type()
+    def get_input_types(cls):
+        return cls.get_supported_input_types()
 
     @classmethod
-    def get_output_type(cls):
-        return cls.get_supported_output_type()
+    def get_output_types(cls):
+        return cls.get_supported_output_types()
 
     @classmethod
-    def get_supported_input_type(cls) -> FileType:
+    def get_supported_input_types(cls) -> Tuple[FileType, ...]:
         """
-        Defines the supported input file type for this converter.
+        Defines the supported input file types for this converter.
 
         Returns:
-            FileType: The file type supported for input.
+            Tuple[FileType]: The file types supported for input.
         """
-        input_type = cls._get_supported_input_type()
-        if not isinstance(input_type, FileType):
+        input_types = cls._get_supported_input_types()
+
+        # Check if input_types is a single FileType instance
+        if isinstance(input_types, FileType):
+            return (input_types,)  # Convert single instance to tuple
+
+        # Check if input_types is an iterable of FileType instances
+        input_types = tuple(input_types)
+        if not all(isinstance(input_type, FileType) for input_type in input_types):
             raise ValueError("Invalid supported input file type")
-        return input_type
+
+        return input_types
 
     @classmethod
-    def get_supported_output_type(cls) -> FileType:
+    def get_supported_output_types(cls) -> Tuple[FileType, ...]:
         """
-        Defines the supported output file type for this converter.
+        Defines the supported output file types for this converter.
 
         Returns:
-            FileType: The file type supported for output.
+            Tuple[FileType]: The file types supported for output.
         """
-        output_type = cls._get_supported_output_type()
-        if not isinstance(output_type, FileType):
+        output_types = cls._get_supported_output_types()
+
+        # Check if output_types is a single FileType instance
+        if isinstance(output_types, FileType):
+            return (output_types,)  # Convert single instance to tuple
+
+        # Check if output_types is an iterable of FileType instances
+        output_types = tuple(output_types)
+        if not all(isinstance(output_type, FileType) for output_type in output_types):
             raise ValueError("Invalid supported output file type")
-        return output_type
+
+        return output_types
 
     @classmethod
     @abstractmethod
-    def _get_supported_input_type(cls) -> FileType:
+    def _get_supported_input_types(cls) -> Iterable[FileType]:
         """
-        Abstract method to define the supported input file type by the converter.
+        Abstract method to define the supported input file types by the converter.
 
         Returns:
-            FileType: The supported input file type.
+            Iterable[FileType]: The supported input file type.
         """
         pass
 
     @classmethod
     @abstractmethod
-    def _get_supported_output_type(cls) -> FileType:
+    def _get_supported_output_types(cls) -> Iterable[FileType]:
         """
-        Abstract method to define the supported output file type by the converter.
+        Abstract method to define the supported output file types by the converter.
 
         Returns:
-            FileType: The supported output file type.
+            Iterable[FileType]: The supported output file type.
         """
         pass
 
     @abstractmethod
     def _convert(
         self,
         input_contents: List,
         output_file: Optional[Path] = None,
         output_folder: Optional[Path] = None,
-    ):
+    ) -> Any:
         """
         Abstract method to be implemented by subclasses to perform the actual file conversion process.
         """
         logger.info("Conversion method not implemented")
 
     def __get_bad_output_content_solving_tips__(self) -> str:
         _solving_tips = (
             f"If you convertion method (`{self.__class__.__name__}._convert(self, input_content:List[])`) uses only one input, make sure you select the first element of input_contents list before procedding",
         )
         return "\n".join(f"{i+1}. {elt}" for i, elt in enumerate(_solving_tips))
 
     def _read_content(self, input_path: Path):
+        assert self.file_reader is not None
         return self.file_reader._read_content(input_path)
 
     def _check_input_format(self, input_content):
         return self.file_reader._check_input_format(input_content)
 
     def _check_output_format(self, output_content):
         return self.file_writer._check_output_format(output_content)
 
     def _write_content(self, output_path: Path, output_content):
+        assert self.file_writer is not None
         return self.file_writer._write_content(output_path, output_content)
```

### Comparing `opencf_core-0.2.0/opencf_core/filetypes.py` & `opencf_core-0.2.1a0/opencf_core/filetypes.py`

 * *Files identical despite different names*

### Comparing `opencf_core-0.2.0/opencf_core/io_handler.py` & `opencf_core-0.2.1a0/opencf_core/io_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class FileReader(ABC):
     """
     Abstract base class for file readers.
     """
 
-    input_format: type = None
+    # input_format: type = None
 
     @abstractmethod
     def _check_input_format(self, content: Any) -> bool:
         """
         Checks if the provided content matches the expected input format.
 
         Args:
@@ -49,15 +49,15 @@
 
 
 class FileWriter(ABC):
     """
     Abstract base class for file writers.
     """
 
-    output_format = None
+    # output_format = None
 
     @abstractmethod
     def _check_output_format(self, content: Any) -> bool:
         """
         Checks if the provided content matches the expected output format.
 
         Args:
```

### Comparing `opencf_core-0.2.0/opencf_core/mimes.py` & `opencf_core-0.2.1a0/opencf_core/mimes.py`

 * *Files identical despite different names*

### Comparing `opencf_core-0.2.0/pyproject.toml` & `opencf_core-0.2.1a0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [tool.poetry]
 name = "opencf-core"
 packages = [
     {include = "opencf_core"}
 ]
-version = "0.2.0"
+version = "0.2.1a0"
 description = "A robust framework for handling file conversion tasks in Python"
 authors = ["Hermann Agossou <agossouhermann7@gmail.com>"]
 readme = "README.md"
 maintainers = [
     "Hermann Agossou <agossouhermann7@gmail.com>"
 ]
 license = "MIT"
 homepage = "https://github.com/Hermann-web/opencf-core"
 repository = "https://github.com/Hermann-web/opencf-core"
-documentation = "https://opencf-core.readthedocs.io/en/latest/"
+documentation = "https://opencf-core.readthedocs.io"
 keywords = ["file conversion", "data processing", "file formats"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-loguru = "^0.7.2"
 python-magic = "^0.4.27"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.10.2"
 black = "^23.0.0"
 flake8 = "^5.0.0"
 mypy = "^1.4.0"
```

### Comparing `opencf_core-0.2.0/PKG-INFO` & `opencf_core-0.2.1a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencf-core
-Version: 0.2.0
+Version: 0.2.1a0
 Summary: A robust framework for handling file conversion tasks in Python
 Home-page: https://github.com/Hermann-web/opencf-core
 License: MIT
 Keywords: file conversion,data processing,file formats
 Author: Hermann Agossou
 Author-email: agossouhermann7@gmail.com
 Maintainer: Hermann Agossou
@@ -17,17 +17,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0)
-Project-URL: Documentation, https://opencf-core.readthedocs.io/en/latest/
+Project-URL: Documentation, https://opencf-core.readthedocs.io
 Project-URL: Repository, https://github.com/Hermann-web/opencf-core
 Description-Content-Type: text/markdown
 
 # OpenCF Core: The File Convertion Framework
 
 The `opencf-core` package provides a robust framework for handling file conversion tasks in Python. It offers a set of classes and utilities designed to simplify the process of reading from and writing to different file formats efficiently.
```


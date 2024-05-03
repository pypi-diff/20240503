# Comparing `tmp/snewpy-1.4b2.tar.gz` & `tmp/snewpy-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snewpy-1.4b2.tar", last modified: Wed Sep  6 20:06:41 2023, max compression
+gzip compressed data, was "snewpy-1.5.tar", last modified: Fri May  3 14:21:56 2024, max compression
```

## Comparing `snewpy-1.4b2.tar` & `snewpy-1.5.tar`

### file list

```diff
@@ -1,39 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 20:06:41.581560 snewpy-1.4b2/
--rw-r--r--   0 runner    (1001) docker     (999)     2892 2023-09-06 20:06:41.581560 snewpy-1.4b2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 20:06:41.577560 snewpy-1.4b2/python/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 20:06:41.577560 snewpy-1.4b2/python/snewpy/
--rw-r--r--   0 runner    (1001) docker     (999)     5102 2023-09-06 20:05:50.201288 snewpy-1.4b2/python/snewpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     5671 2023-09-06 20:05:50.201288 snewpy-1.4b2/python/snewpy/_git.py
--rw-r--r--   0 runner    (1001) docker     (999)     5872 2023-09-06 20:05:50.201288 snewpy-1.4b2/python/snewpy/_model_downloader.py
--rw-r--r--   0 runner    (1001) docker     (999)    89954 2023-09-06 20:06:02.309350 snewpy-1.4b2/python/snewpy/_model_urls.py
--rw-r--r--   0 runner    (1001) docker     (999)       22 2023-09-06 20:05:50.201288 snewpy-1.4b2/python/snewpy/_version.py
--rw-r--r--   0 runner    (1001) docker     (999)    45394 2023-09-06 20:05:50.201288 snewpy-1.4b2/python/snewpy/flavor_transformation.py
--rw-r--r--   0 runner    (1001) docker     (999)    14332 2023-09-06 20:05:50.201288 snewpy-1.4b2/python/snewpy/flux.py
--rw-r--r--   0 runner    (1001) docker     (999)      528 2023-09-06 20:05:50.201288 snewpy-1.4b2/python/snewpy/from_snowglobes.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 20:06:41.577560 snewpy-1.4b2/python/snewpy/models/
--rw-r--r--   0 runner    (1001) docker     (999)     2470 2023-09-06 20:05:50.201288 snewpy-1.4b2/python/snewpy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    18202 2023-09-06 20:05:50.201288 snewpy-1.4b2/python/snewpy/models/base.py
--rw-r--r--   0 runner    (1001) docker     (999)    33528 2023-09-06 20:05:50.201288 snewpy-1.4b2/python/snewpy/models/ccsn.py
--rw-r--r--   0 runner    (1001) docker     (999)    27793 2023-09-06 20:05:50.201288 snewpy-1.4b2/python/snewpy/models/loaders.py
--rw-r--r--   0 runner    (1001) docker     (999)      922 2023-09-06 20:05:50.201288 snewpy-1.4b2/python/snewpy/models/model_files.yml
--rw-r--r--   0 runner    (1001) docker     (999)     5136 2023-09-06 20:05:50.201288 snewpy-1.4b2/python/snewpy/models/presn.py
--rw-r--r--   0 runner    (1001) docker     (999)     8274 2023-09-06 20:05:50.201288 snewpy-1.4b2/python/snewpy/neutrino.py
--rw-r--r--   0 runner    (1001) docker     (999)     7470 2023-09-06 20:05:50.201288 snewpy-1.4b2/python/snewpy/rate_calculator.py
--rw-r--r--   0 runner    (1001) docker     (999)      443 2023-09-06 20:05:50.201288 snewpy-1.4b2/python/snewpy/run_snowglobes.py
--rw-r--r--   0 runner    (1001) docker     (999)    18818 2023-09-06 20:05:50.201288 snewpy-1.4b2/python/snewpy/snowglobes.py
--rw-r--r--   0 runner    (1001) docker     (999)    14149 2023-09-06 20:05:50.201288 snewpy-1.4b2/python/snewpy/snowglobes_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 20:06:41.581560 snewpy-1.4b2/python/snewpy/test/
--rw-r--r--   0 runner    (1001) docker     (999)       40 2023-09-06 20:05:50.201288 snewpy-1.4b2/python/snewpy/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2301 2023-09-06 20:05:50.205288 snewpy-1.4b2/python/snewpy/test/_rate_crosscheck_table.py
--rw-r--r--   0 runner    (1001) docker     (999)     3462 2023-09-06 20:05:50.205288 snewpy-1.4b2/python/snewpy/test/simplerate_integrationtest.py
--rw-r--r--   0 runner    (1001) docker     (999)      703 2023-09-06 20:05:50.205288 snewpy-1.4b2/python/snewpy/test/snewpy_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (999)      157 2023-09-06 20:05:50.205288 snewpy-1.4b2/python/snewpy/test/test_00_init.py
--rw-r--r--   0 runner    (1001) docker     (999)    13032 2023-09-06 20:05:50.205288 snewpy-1.4b2/python/snewpy/test/test_01_registry.py
--rw-r--r--   0 runner    (1001) docker     (999)    13675 2023-09-06 20:05:50.205288 snewpy-1.4b2/python/snewpy/test/test_02_models.py
--rw-r--r--   0 runner    (1001) docker     (999)     2022 2023-09-06 20:05:50.205288 snewpy-1.4b2/python/snewpy/test/test_03_neutrino.py
--rw-r--r--   0 runner    (1001) docker     (999)    25185 2023-09-06 20:05:50.205288 snewpy-1.4b2/python/snewpy/test/test_04_xforms.py
--rw-r--r--   0 runner    (1001) docker     (999)     1317 2023-09-06 20:05:50.205288 snewpy-1.4b2/python/snewpy/test/test_05_snowglobes.py
--rw-r--r--   0 runner    (1001) docker     (999)     4183 2023-09-06 20:05:50.205288 snewpy-1.4b2/python/snewpy/test/test_flux_container.py
--rw-r--r--   0 runner    (1001) docker     (999)     2517 2023-09-06 20:05:50.205288 snewpy-1.4b2/python/snewpy/test/test_rate_calculation.py
--rw-r--r--   0 runner    (1001) docker     (999)     1121 2023-09-06 20:05:50.205288 snewpy-1.4b2/python/snewpy/to_snowglobes.py
--rw-r--r--   0 runner    (1001) docker     (999)     2324 2023-09-06 20:05:50.205288 snewpy-1.4b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:21:56.966618 snewpy-1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-03 14:21:25.000000 snewpy-1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-03 14:21:56.966618 snewpy-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-03 14:21:25.000000 snewpy-1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:21:56.958618 snewpy-1.5/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:21:56.962618 snewpy-1.5/python/snewpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/_model_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54158 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/flavor_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15744 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/from_snowglobes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:21:56.966618 snewpy-1.5/python/snewpy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25596 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/models/ccsn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34393 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/models/ccsn_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/models/model_files.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/models/presn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/models/presn_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21931 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/models/registry_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/neutrino.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17477 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/rate_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/run_snowglobes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19106 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/snowglobes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/snowglobes_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:21:56.966618 snewpy-1.5/python/snewpy/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/_rate_crosscheck_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/simplerate_integrationtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/snewpy_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/test_00_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/test_01_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/test_02_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/test_03_neutrino.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33885 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/test_04_xforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/test_05_snowglobes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/test_flux_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/test_presn_rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/test_rate_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/to_snowglobes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:21:56.962618 snewpy-1.5/python/snewpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-03 14:21:56.000000 snewpy-1.5/python/snewpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-03 14:21:56.000000 snewpy-1.5/python/snewpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:21:56.000000 snewpy-1.5/python/snewpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:21:39.000000 snewpy-1.5/python/snewpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-03 14:21:56.000000 snewpy-1.5/python/snewpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 14:21:56.000000 snewpy-1.5/python/snewpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 14:21:56.966618 snewpy-1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-03 14:21:25.000000 snewpy-1.5/setup.py
```

### Comparing `snewpy-1.4b2/python/snewpy/_git.py` & `snewpy-1.5/python/snewpy/_git.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 #
 """Some code for interacting with git.
 """
 
 import re
 from os.path import abspath, isdir, isfile, join
 from setuptools import Command
-from distutils.log import INFO
 
 
 def get_version():
     """Get the value of ``__version__`` without having to import the module.
 
     Returns
     -------
@@ -173,8 +172,8 @@
 
     def finalize_options(self):
         pass
 
     def run(self):
         update_version(tag=self.tag)
         ver = get_version()
-        self.announce("Version is now {}.".format(ver), level=INFO)
+        self.announce("Version is now {}.".format(ver), level=2)
```

### Comparing `snewpy-1.4b2/python/snewpy/_model_downloader.py` & `snewpy-1.5/python/snewpy/_model_downloader.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,154 +17,218 @@
 from tqdm.auto import tqdm
 from typing import Optional
 
 from snewpy import model_path
 from snewpy import __version__ as snewpy_version
 
 import logging
-logger = logging.getLogger('FileHandle')
 
+logger = logging.getLogger("FileHandle")
 
-def _md5(fname:str) -> str:
+
+def _md5(fname: str) -> str:
     """calculate the md5sum hash of a file."""
     hash_md5 = hashlib.md5()
     with open(fname, "rb") as f:
         for chunk in iter(lambda: f.read(4096), b""):
             hash_md5.update(chunk)
     return hash_md5.hexdigest()
 
 
-def _download(src:str, dest:str, chunk_size=8192):
+def _download(src: str, dest: str, chunk_size=8192):
     """Download a file from 'src' to 'dest' and show the progress bar."""
-    #make sure parent dir exists
+    # make sure parent dir exists
     Path(dest).parent.mkdir(exist_ok=True, parents=True)
     with requests.get(src, stream=True) as r:
         r.raise_for_status()
-        fileSize = int(r.headers.get('content-length', 0))
-        with tqdm(desc=dest.name, total=fileSize, unit='iB', unit_scale=True, unit_divisor=1024) as bar:
-            with open(dest, 'wb') as f:
+        fileSize = int(r.headers.get("content-length", 0))
+        with tqdm(
+            desc=dest.name,
+            total=fileSize,
+            unit="iB",
+            unit_scale=True,
+            unit_divisor=1024,
+        ) as bar:
+            with open(dest, "wb") as f:
                 for chunk in r.iter_content(chunk_size=chunk_size):
                     size = f.write(chunk)
                     bar.update(size)
 
 
 class ChecksumError(FileNotFoundError):
-    """Raise an exception due to a mismatch in the MD5 checksum.
-    """
+    """Raise an exception due to a mismatch in the MD5 checksum."""
+
     def __init__(self, path, md5_exp, md5_actual):
-        super().__init__(f'Checksum error for file {path}: {md5_actual}!={md5_exp}')
+        super().__init__(f"Checksum error for file {path}: {md5_actual}!={md5_exp}")
+
     pass
 
 
 class MissingFileError(FileNotFoundError):
-    """Raise an exception due to a missing file.
-    """
+    """Raise an exception due to a missing file."""
+
     pass
 
 
 @dataclass
 class FileHandle:
     """Object storing local path, remote URL (optional), and MD5 sum
-(optional) for a SNEWPY model file. If the requested file is already present
-locally, open it. Otherwise, download it from the remote URL to the desired
-local path.
+    (optional) for a SNEWPY model file. If the requested file is already present
+    locally, open it. Otherwise, download it from the remote URL to the desired
+    local path.
     """
+
     path: Path
     remote: str = None
     md5: Optional[str] = None
-    
+
     def check(self) -> None:
         """Check if the given file exists locally and has a correct md5 sum.
         Raises
         ------
         :class:`MissingFileError`
             if the local copy of the file is missing
-        :class:`ChecksumError` 
+        :class:`ChecksumError`
             if the local file exists, but the checksum is wrong"""
         if not self.path.exists():
             raise MissingFileError(self.path)
         if self.md5:
-            logger.info(f'File {self.path}: checking md5')
+            logger.info(f"File {self.path}: checking md5")
             md5 = _md5(self.path)
-            logger.debug(f'{md5} vs expected {self.md5}')
-            if (md5 != self.md5):
+            logger.debug(f"{md5} vs expected {self.md5}")
+            if md5 != self.md5:
                 raise ChecksumError(self.path, self.md5, md5)
-    
+
     def load(self) -> Path:
         """Make sure that local file exists and has a correct checksum.
         Download the file if needed.
         """
         try:
             self.check()
         except FileNotFoundError as e:
-            logger.info(f'Downloading file {self.path}')
+            logger.info(f"Downloading file {self.path}")
             _download(self.remote, self.path)
             self.check()
         return self.path
 
 
-def from_zenodo(zenodo_id:str, model:str, filename:str):
+def _from_zenodo(zenodo_id: str, filename: str):
     """Access files on Zenodo.
 
     Parameters
     ----------
     zenodo_id : Zenodo record for model files.
-    model : Name of the model class for this model file.
     filename : Expected filename storing simulation data.
 
     Returns
     -------
     file_url, md5sum
     """
-    zenodo_url = f'https://zenodo.org/api/records/{zenodo_id}'
+    zenodo_url = f"https://zenodo.org/api/records/{zenodo_id}"
     record = requests.get(zenodo_url).json()
-    # Search for model file string in Zenodo request for this record.
-    file = next((_file for _file in record['files'] if _file['key'] == filename), None)
+    # Search for file string in Zenodo request for this record.
+    file = next((_file for _file in record["files"] if _file["key"] == filename), None)
 
     # If matched, return a tuple of URL and checksum.Otherwise raise an exception.
     if file is not None:
-        return file['links']['self'], file['checksum'].split(':')[1]
+        return file["links"]["self"], file["checksum"].split(":")[1]
     else:
         raise MissingFileError(filename)
 
-def get_model_data(model: str, filename: str, path: str = model_path) -> Path:
+
+class ModelRegistry:
     """Access model data. Configuration for each model is in a YAML file
     distributed with SNEWPY.
+    """
+
+    def __init__(self, config_file: Path = None, local_path: str = model_path):
+        """
+        Parameters
+        ----------
+        config_file: YAML configuration file. If None (default) use the 'model_files.yml' from SNEWPY resources
+        local_path: local installation path (defaults to astropy cache).
+        """
+        if config_file is None:
+            context = open_text("snewpy.models", "model_files.yml")
+        else:
+            context = open(config_file)
+        with context as f:
+            self.config = yaml.safe_load(f)
+        self.models = self.config["models"]
+        self.local_path = local_path
+
+    def get_file(self, config_path: str, filename: str) -> Path:
+        """Get the requested data file from the models file repository
+
+        Parameters
+        ----------
+        config_path : dot-separated path of the model in the YAML configuration (e.g. "ccsn.Bollig_2016")
+        filename : Name of simulation datafile, or a relative path from the model sub-directory
+
+        Returns
+        -------
+        Path of downloaded file.
+        """
+        tokens = config_path.split(".")
+        config = self.models
+        for t in tokens:
+            config = config[t]
+        # store the model name
+        model = tokens[-1]
+        # Get data from GitHub or Zenodo.
+        repo = config["repository"]
+        if repo == "zenodo":
+            url, md5 = _from_zenodo(zenodo_id=config["zenodo_id"], filename=filename)
+        else:
+            # format the url directly
+            params = {
+                "model": model,
+                "filename": filename,
+                "snewpy_version": snewpy_version,
+            }
+            params.update(
+                config
+            )  # default parameters can be overriden in the model config
+            url, md5 = repo.format(**params), None
+        localpath = Path(model_path) / str(model)
+        localpath.mkdir(exist_ok=True, parents=True)
+        fh = FileHandle(path=localpath / filename, remote=url, md5=md5)
+        return fh.load()
+
+
+registry = ModelRegistry()
+
+
+class LocalFileLoader:
+    @classmethod
+    def request_file(cls, filename:str)->Path:
+        "Require that the provided filename exists locally"
+        path = Path(filename).absolute()
+        if not path.exists():
+            raise FileNotFoundError(path)
+        return path
+
+class RegistryFileLoader(LocalFileLoader):
+    _registry = registry
+    
+    @classmethod
+    def request_file(cls, filename:str)->Path:
+        "Request file from the model registry"
+        return cls._registry.get_file(cls._config_path, filename)
+        
+        
+def get_model_data(model: str, filename: str) -> Path:
+    """Get the requested data file from the models file repository
 
     Parameters
     ----------
-    model : Name of the model class for this model file.
-    filename : Name of simulation datafile, or a relative path from the model sub-directory
-    path : Local installation path (defaults to astropy cache).
+    model : dot-separated path of the model in the YAML configuration (e.g. "ccsn.Bollig_2016")
+    filename : Absolute path to simulation datafile, or a relative path from the model sub-directory
 
     Returns
     -------
     Path of downloaded file.
     """
     if os.path.isabs(filename):
         return Path(filename)
-
-    params = { 'model':model, 'filename':filename, 'snewpy_version':snewpy_version}
-
-    # Parse YAML file with model repository configurations.
-    with open_text('snewpy.models', 'model_files.yml') as f:
-        config = yaml.safe_load(f)
-        models = config['models']
-        # Search for model in YAML configuration.
-        if model in models.keys():
-            # Get data from GitHub or Zenodo.
-            modconf = models[model]
-            repo = modconf.pop('repository')
-            if repo == 'zenodo':
-                params['zenodo_id'] = modconf['zenodo_id']
-                url, md5 = from_zenodo(**params)
-            else:
-                #format the url directly
-                params.update(modconf) #default parameters can be overriden in the model config
-                url, md5 = repo.format(**params), None
-            localpath = Path(path)/str(model)
-            localpath.mkdir(exist_ok=True, parents=True)
-            fh = FileHandle(path = localpath/filename,remote = url, md5=md5)
-            return fh.load()
-        else:
-            raise KeyError(f'No configuration for {model}')
-
+    else:
+        return registry.get_file(model, filename)
```

### Comparing `snewpy-1.4b2/python/snewpy/flavor_transformation.py` & `snewpy-1.5/python/snewpy/flavor_transformation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1670,7 +1670,310 @@
             Transition probability.
         """        
         if self.mass_order == MassHierarchy.NORMAL:
             return ( 1 - self.De1 - self.Ds1 ) / 2
         else:
             return ( 1 - self.De3 - self.Ds3 ) / 2        
     
+
+class QuantumDecoherence(FlavorTransformation):
+    """Quantum Decoherence, where propagation in vacuum leads to equipartition
+    of states. For a description and typical parameters, see M. V. dos Santos et al.,
+    2023, arXiv:2306.17591.
+    """
+    def __init__(self, mix_angles=None, Gamma3=1e-27*u.eV, Gamma8=1e-27*u.eV, dist=10*u.kpc, n=0, E0=10*u.MeV, mh=MassHierarchy.NORMAL):
+        """Initialize transformation matrix.
+
+        Parameters
+        ----------
+        mix_angles : tuple or None
+            If not None, override default mixing angles using tuple (theta12, theta13, theta23).
+        Gamma3 : astropy.units.quantity.Quantity
+            Quantum decoherence parameter; expect in eV.
+        Gamma8 : astropy.units.quantity.Quantity
+            Quantum decoherence parameter; expect in eV.
+        dist : astropy.units.quantity.Quantity
+            Distance to the supernova.
+        n : float
+            Exponent of power law for energy dependent quantum decoherence parameters,
+            i.e. Gamma = Gamma0*(E/E0)**n. If not specified, it is taken as zero.
+        E0 : astropy.units.quantity.Quantity
+            Reference energy in the power law Gamma = Gamma0*(E/E0)**n. If not specified, 
+            it is taken as 10 MeV. Note that if n = 0, quantum decoherence parameters are independent
+            of E0.
+        mh : MassHierarchy
+            MassHierarchy.NORMAL or MassHierarchy.INVERTED.
+        """
+        if type(mh) == MassHierarchy:
+            self.mass_order = mh
+        else:
+            raise TypeError('mh must be of type MassHierarchy')
+
+        if mix_angles is not None:
+            theta12, theta13, theta23 = mix_angles
+        else:
+            pars = MixingParameters(mh)
+            theta12, theta13, theta23 = pars.get_mixing_angles()
+
+        self.De1 = float((np.cos(theta12) * np.cos(theta13))**2)
+        self.De2 = float((np.sin(theta12) * np.cos(theta13))**2)
+        self.De3 = float(np.sin(theta13)**2)
+
+        self.Gamma3 = (Gamma3 / (c.hbar.to('eV s') * c.c)).to('1/kpc')
+        self.Gamma8 = (Gamma8 / (c.hbar.to('eV s') * c.c)).to('1/kpc')
+        self.d = dist
+        self.n = n
+        self.E0 = E0
+    
+    def P11(self, E):
+        """Survival probability of state nu1 in vacuum.
+
+        Parameters
+        ----------
+        E : float
+            Energy.
+
+        Returns
+        -------
+        P11 : float
+            Survival probability of state nu1 in vacuum.
+
+        :meta private:
+        """
+        return 1/3 + 1/2 * np.exp(-(self.Gamma3 * (E/self.E0)**self.n + self.Gamma8 * (E/self.E0)**self.n / 3) * self.d) + 1/6 * np.exp(-self.Gamma8 * (E/self.E0)**self.n * self.d)
+
+    def P21(self, E):
+        """Transition probability from the state nu2 to nu1 in vacuum.
+
+        Parameters
+        ----------
+        E : float
+            Energy.
+
+        Returns
+        -------
+        P21 : float
+            Transition probability from the state nu2 to nu1 in vacuum.
+            Note that P21 = P12.
+
+        :meta private:
+        """
+        return 1/3 - 1/2 * np.exp(-(self.Gamma3 * (E/self.E0)**self.n + self.Gamma8 * (E/self.E0)**self.n / 3) * self.d) + 1/6 * np.exp(-self.Gamma8 * (E/self.E0)**self.n * self.d)
+
+    def P22(self, E):
+        """Survival probability of state nu2 in vacuum.
+
+        Parameters
+        ----------
+        E : float
+            Energy.
+
+        Returns
+        -------
+        P21 : float
+            Survival probability of state nu2 in vacuum.
+
+        :meta private:
+        """
+        return self.P11(E)
+
+
+    def P31(self, E):
+        """Transition probability from the state nu3 to nu1 in vacuum.
+
+        Parameters
+        ----------
+        E : float
+            Energy.
+
+        Returns
+        -------
+        P31 : float
+            Transition probability from the state nu3 to nu1 in vacuum.
+            Note that P31 = P13.
+
+        :meta private:
+        """
+        return 1/3 - 1/3 * np.exp(-self.Gamma8 * (E/self.E0)**self.n * self.d)
+    
+    def P32(self, E):
+        """Transition probability from the state nu3 to nu2 in vacuum.
+
+        Parameters
+        ----------
+        E : float
+            Energy.
+
+        Returns
+        -------
+        P32 : float
+            Transition probability from the state nu3 to nu2 in vacuum.
+            Note that P32 = P23.
+
+        :meta private:
+        """
+        return self.P31(E)
+    
+    def P33(self, E):
+        """Survival probability of state nu3 in vacuum.
+
+        Parameters
+        ----------
+        E : float
+            Energy.
+
+        Returns
+        -------
+        P33 : float
+            Survival probability of state nu3 in vacuum.
+
+        :meta private:
+        """
+        return 1/3 + 2/3 * np.exp(-self.Gamma8 * (E/self.E0)**self.n * self.d)
+
+    def prob_ee(self, t, E):
+        """Electron neutrino survival probability.
+
+        Parameters
+        ----------
+        t : float or ndarray
+            List of times.
+        E : float or ndarray
+            List of energies.
+
+        Returns
+        -------
+        prob : float or ndarray
+            Transition probability.
+        """
+        # NMO case.
+        if self.mass_order == MassHierarchy.NORMAL:
+            pe_array = self.P31(E)*self.De1 + self.P32(E)*self.De2 + self.P33(E)*self.De3
+        # IMO case.
+        else:
+            pe_array = self.P22(E)*self.De2 + self.P21(E)*self.De1 + self.P32(E)*self.De3
+        return pe_array
+
+    def prob_ex(self, t, E):
+        """X -> e neutrino transition probability.
+
+        Parameters
+        ----------
+        t : float or ndarray
+            List of times.
+        E : float or ndarray
+            List of energies.
+
+        Returns
+        -------
+        prob : float or ndarray
+            Transition probability.
+        """
+        return 1. - self.prob_ee(t,E)
+
+    def prob_xx(self, t, E):
+        """Flavor X neutrino survival probability.
+
+        Parameters
+        ----------
+        t : float or ndarray
+            List of times.
+        E : float or ndarray
+            List of energies.
+
+        Returns
+        -------
+        prob : float or ndarray
+            Transition probability.
+        """
+        return 1. - self.prob_ex(t,E) / 2.
+
+    def prob_xe(self, t, E):
+        """e -> X neutrino transition probability.
+
+        Parameters
+        ----------
+        t : float or ndarray
+            List of times.
+        E : float or ndarray
+            List of energies.
+
+        Returns
+        -------
+        prob : float or ndarray
+            Transition probability.
+        """
+        return (1. - self.prob_ee(t,E)) / 2.
+
+    def prob_eebar(self, t, E):
+        """Electron antineutrino survival probability.
+
+        Parameters
+        ----------
+        t : float or ndarray
+            List of times.
+        E : float or ndarray
+            List of energies.
+
+        Returns
+        -------
+        prob : float or ndarray
+            Transition probability.
+        """
+        # NMO case.
+        if self.mass_order == MassHierarchy.NORMAL:
+            pe_array = self.P11(E)*self.De1 + self.P21(E)*self.De2 + self.P31(E)*self.De3
+        # IMO case.
+        else:
+            pe_array = self.P31(E)*self.De1 + self.P32(E)*self.De2 + self.P33(E)*self.De3
+        return pe_array
+
+    def prob_exbar(self, t, E):
+        """X -> e antineutrino transition probability.
+
+        Parameters
+        ----------
+        t : float or ndarray
+            List of times.
+        E : float or ndarray
+            List of energies.
+
+        Returns
+        -------
+        prob : float or ndarray
+            Transition probability.
+        """
+        return 1. - self.prob_eebar(t,E)
+
+    def prob_xxbar(self, t, E):
+        """X -> X antineutrino survival probability.
+
+        Parameters
+        ----------
+        t : float or ndarray
+            List of times.
+        E : float or ndarray
+            List of energies.
+
+        Returns
+        -------
+        prob : float or ndarray
+            Transition probability.
+        """
+        return 1. - self.prob_exbar(t,E) / 2.
+
+    def prob_xebar(self, t, E):  
+        """e -> X antineutrino transition probability.
+
+        Parameters
+        ----------
+        t : float or ndarray
+            List of times.
+        E : float or ndarray
+            List of energies.
+
+        Returns
+        -------
+        prob : float or ndarray
+            Transition probability.
+        """
+        return (1. - self.prob_eebar(t,E)) / 2.
```

### Comparing `snewpy-1.4b2/python/snewpy/flux.py` & `snewpy-1.5/python/snewpy/flux.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,18 +56,19 @@
 from astropy import units as u
 
 import numpy as np
 
 from scipy.integrate import cumulative_trapezoid
 from scipy.interpolate import interp1d
 from enum import IntEnum
-
-from copy import copy
 from functools import wraps
 
+#list of units which will be used as units for decomposition inside the Container
+snewpy_unit_bases = [u.MeV, u.m, u.s, u.kg]
+
 class Axes(IntEnum):
     """Enum to keep the number number of the array dimension for each axis""" 
     flavor=0, #Flavor dimension
     time=1,   #Time dimension
     energy=2, #Energy dimension
     
     @classmethod
@@ -94,36 +95,51 @@
         """A container class storing the physical quantity (flux, fluence, rate...), which depends on flavor, time and energy.
 
         Parameters
         ----------
         data: :class:`astropy.Quantity`
             3D array of the stored quantity, must have dimensions compatible with (flavor, time, energy)
         
-        flavor: list of :class:`snewpy.neutrino.Flavor`
+        flavor: list or a single value of :class:`snewpy.neutrino.Flavor`
             array of flavors (should be ``len(flavor)==data.shape[0]``
         
-        time: array of :class:`astropy.Quantity`
+        time: :class:`astropy.Quantity`
             sampling points in time (then ``len(time)==data.shape[1]``) 
             or time bin edges (then ``len(time)==data.shape[1]+1``) 
     
-        energy: array of :class:`astropy.Quantity`
+        energy: :class:`astropy.Quantity`
             sampling points in energy (then ``len(energy)=data.shape[2]``) 
             or energy bin edges (then ``len(energy)=data.shape[2]+1``) 
     
         integrable_axes: set of :class:`Axes` or None
             List of axes which can be integrated.
             If None (default) this set will be derived from the axes shapes 
         """
         if self.unit is not None:
             #try to convert to the unit
             data = data.to(self.unit)
-        self.array = data
-        self.flavor = np.sort(flavor)
-        self.time = time
-        self.energy = energy
+        #convert the input values to arrays if they are scalar
+        self.array = u.Quantity(data)
+        self.time = u.Quantity(time, ndmin=1)
+        self.energy = u.Quantity(energy, ndmin=1)
+        self.flavor = np.sort(np.array(flavor, ndmin=1))
+        
+        Nf,Nt,Ne = len(self.flavor), len(self.time), len(self.energy)
+        #list all valid shapes of the input array
+        expected_shapes=[(nf,nt,ne) for nf in (Nf,Nf-1) for nt in (Nt,Nt-1) for ne in (Ne,Ne-1)]
+        #treat special case if data is 1d array
+        if self.array.ndim==1:
+            #try to reshape the array to expected shape
+            for expected_shape in expected_shapes:
+                if np.prod(expected_shape)==self.array.size:
+                    self.array = self.array.reshape(expected_shape)
+                    break
+        #validate the data array shape
+        if self.array.shape not in expected_shapes:
+            raise ValueError(f"Data array of shape {data.shape} is inconsistent with any valid shapes {expected_shapes}")
         
         if integrable_axes is not None:
             #store which axes can be integrated
             self._integrable_axes = set(integrable_axes)
         else:
             #guess which axes can be integrated
             self._integrable_axes = {a for a in Axes if(self._axshape[a]==self.array.shape[a])}
@@ -258,45 +274,49 @@
             raise ValueError(f'Cannot integrate over {axis.name}! Valid axes are {self._integrable_axes}')
         #set the limits
         ax = self.axes[axis]
         xmin, xmax = ax.min(), ax.max()
         if limits is None:
             limits = u.Quantity([xmin, xmax])
         limits = limits.to(ax.unit)
-        limits = limits.clip(xmin, xmax)
+        #limits = limits.clip(xmin,xmax)
         #compute the integral
         yc = cumulative_trapezoid(self.array, x=ax, axis=axis, initial=0)
-        _integral = interp1d(x=ax, y=yc, fill_value=0, axis=axis, bounds_error=False)
+        #get first and last value to use as the fill values
+        yc_limits = (yc.take(0,axis=axis), yc.take(-1,axis=axis)) 
+        #this will make the _integral constant if it gets out of bounds,
+        # i.e. effectively the flux outside of bounds is zero
+        _integral = interp1d(x=ax, y=yc, fill_value=yc_limits, axis=axis, bounds_error=False)
         array = np.diff(_integral(limits),axis=axis) << (self.array.unit*ax.unit)
         axes = list(self.axes)
         axes[axis] = limits
         #choose the proper class
         return Container(array, *axes, integrable_axes=self._integrable_axes.difference({axis}))
-        return result
-        
+
     def integrate_or_sum(self, axis:Union[Axes,str])->'Container':
         if self.can_integrate(axis):
             return self.integrate(axis)
         else:
             return self.sum(axis)
             
     def can_integrate(self, axis):
         "return true if can be integrated along given axis"
         return Axes.get(axis) in self._integrable_axes
     def can_sum(self, axis):
         "return true if can be summed along given axis"
         return Axes.get(axis) not in self._integrable_axes
     
     def __rmul__(self, factor):
-        "multiply array by givem factor or matrix"
-        return self.__mul__(self, factor)
+        "multiply array by given factor or matrix"
+        return self.__mul__(factor)
 
     def __mul__(self, factor) -> 'Container':
-        "multiply array by givem factor or matrix"
-        #if not (np.isscalar(factor)):
+        "multiply array by given factor or matrix"
+        if not (np.isscalar(factor) or isinstance(factor, np.ndarray)):
+            return NotImplemented
         #    raise ValueError("Factor should be a scalar value")
         array = self.array*factor
         axes = list(self.axes)
         return Container(array, *axes)
 
     def save(self, fname:str)->None:
         """Save container data to a given file (using `numpy.savez`)"""
@@ -346,14 +366,15 @@
 
 class Container(_ContainerBase):
     #a dictionary holding classes for each unit
     _unit_classes = {}
 
     @wraps(_ContainerBase.__init__)
     def __new__(cls, data,*args, **kwargs):
+        data = data.decompose(snewpy_unit_bases) #simplify the units, reducing to the bases
         if not cls.unit:
             data = u.Quantity(data)
             cls = cls[data.unit]
         return super().__new__(cls)
 
     def __class_getitem__(cls, args):
         try:
@@ -366,15 +387,15 @@
             #create subclass of this type with given unit
             name = name or f'{cls.__name__}[{unit}]'
             cls._unit_classes[unit] = type(name,(cls,),{'unit':unit})
         return cls._unit_classes[unit]
         
 
 #some standard container classes that can be used for 
-Flux = Container['1/(MeV*s*cm**2)', "d2FdEdT"]
+Flux = Container['1/(MeV*s*m**2)', "d2FdEdT"]
 Fluence = Container[Flux.unit*u.s, "dFdE"]
 Spectrum= Container[Flux.unit*u.MeV, "dFdT"]
 IntegralFlux= Container[Flux.unit*u.s*u.MeV, "dF"]
 
 DifferentialEventRate = Container['1/(MeV*s)', "d2NdEdT"]
 EventRate = Container['1/s', "dNdT"]
 EventSpectrum = Container['1/MeV', "dNdE"]
```

### Comparing `snewpy-1.4b2/python/snewpy/from_snowglobes.py` & `snewpy-1.5/python/snewpy/from_snowglobes.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.4b2/python/snewpy/models/__init__.py` & `snewpy-1.5/python/snewpy/models/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,26 @@
-import logging
 from warnings import warn
 
-from snewpy import get_models, model_path
 from . import ccsn, presn
 
 
 def __getattr__(name):
     if name in dir(ccsn):
         warn(f"{__name__}.{name} is moved to {__name__}.ccsn.{name}", FutureWarning, stacklevel=2)
         return getattr(ccsn, name)
     raise AttributeError(f"module {__name__} has no attribute {name}")
 
 
-def _init_model(model_name, download=True, download_dir=model_path, **user_param):
+def _init_model(model_name, **user_param):
     """Attempts to retrieve instantiated SNEWPY model using model class name and model parameters.
-    If a model name is valid, but is not found and `download`=True, this function will attempt to download the model
 
     Parameters
     ----------
     model_name : str
         Name of SNEWPY model to import, must exactly match the name of the corresponding model class
-    download : bool
-        Switch for attempting to download model data if the first load attempt failed due to a missing file.
-    download_dir : str
-        Local directory to download model files to.
     user_param : varies
         User-requested model parameters used to initialize the model, if one is found.
         Error checking is performed during model initialization
 
     Raises
     ------
     ValueError
@@ -53,17 +46,8 @@
     if model_name in dir(ccsn):
         module = ccsn
     elif model_name in dir(presn):
         module = presn
     else:
         raise ValueError(f"Unable to find model with name '{model_name}' in snewpy.models.ccsn or snewpy.models.presn")
 
-    try:
-        return getattr(module, model_name)(**user_param)
-    except FileNotFoundError as e:
-        logger = logging.getLogger()
-        logger.warning(f"Unable to find model {model_name} in {download_dir}")
-        if not download:
-            raise e
-        logger.warning(f"Attempting to download model...")
-        get_models(model_name, download_dir)
-        return getattr(module, model_name)(**user_param)
+    return getattr(module, model_name)(**user_param)
```

### Comparing `snewpy-1.4b2/python/snewpy/models/base.py` & `snewpy-1.5/python/snewpy/snowglobes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,469 +1,378 @@
-import itertools as it
+# -*- coding: utf-8 -*-
+"""The ``snewpy.snowglobes`` module contains functions for interacting with SNOwGLoBES.
+
+`SNOwGLoBES <https://github.com/SNOwGLoBES/snowglobes>`_ can estimate detected
+event rates from a given input supernova neutrino flux. It supports many
+different neutrino detectors, detector materials and interaction channels.
+There are three basic steps to using SNOwGLoBES from SNEWPY:
+
+* **Generating input files for SNOwGLoBES:**
+    There are two ways to do this, either generate a time series or a fluence file. This is done taking as input the supernova simulation model.
+    The first will evaluate the neutrino flux at each time step, the latter will compute the integrated neutrino flux (fluence) in the time bin.
+    The result is a compressed .tar file containing all individual input files.
+* **Running SNOwGLoBES:**
+    This step convolves the fluence generated in the previous step with the cross-sections for the interaction channels happening in various detectors supported by SNOwGLoBES.
+    It takes into account the effective mass of the detector as well as a smearing matrix describing the energy-dependent detection efficiency.
+    The output gives the number of events detected as a function of energy for each interaction channel, integrated in a given time window (or time bin), or in a snapshot in time.
+* **Collating SNOwGLoBES outputs:**
+    This step puts together all the interaction channels and time bins evaluated by SNOwGLoBES in a single file (for each detector and for each time bin).
+    The output tables allow to build the detected neutrino energy spectrum and neutrino time distribution, for each reaction channel or the sum of them.
+"""
+
+import logging
 import os
-from abc import ABC, abstractmethod
-from warnings import warn
+import re
+import tarfile
+from pathlib import Path
+from tempfile import TemporaryDirectory
 
+import matplotlib.pyplot as plt
 import numpy as np
+import pandas as pd
 from astropy import units as u
-from astropy.table import Table, join
-from astropy.units import UnitTypeError, get_physical_type
-from astropy.units.quantity import Quantity
-from scipy.special import loggamma
-from snewpy import _model_downloader
-
-from snewpy.neutrino import Flavor
-from snewpy.flavor_transformation import NoTransformation
-from functools import wraps
-
-from snewpy.flux import Flux
-
-def _wrap_init(init, check):
-    @wraps(init)
-    def _wrapper(self, *arg, **kwargs):
-        init(self, *arg, **kwargs)
-        check(self)
-    return _wrapper
-
-
-class SupernovaModel(ABC):
-    """Base class defining an interface to a supernova model."""
-
-    def __init_subclass__(cls, **kwargs):
-        """Hook to modify the subclasses on creation"""
-        super().__init_subclass__(**kwargs)
-        cls.__init__ = _wrap_init(cls.__init__, cls.__post_init_check)
-
-    def __init__(self, time, metadata):
-        """Initialize supernova model base class
-        (call this method in the subclass constructor as ``super().__init__(time,metadata)``).
-
-        Parameters
-        ----------
-        time : ndarray of astropy.Quantity
-            Time points where the model flux is defined.
-            Must be array of :class:`Quantity`, with units convertable to "second".
-        metadata : dict
-            Dict of model parameters <name>:<value>,
-            to be used for printing table in :meth:`__repr__` and :meth:`_repr_markdown_`
-        """
-        self.time = time
-        self.metadata = metadata
-        
-    def __repr__(self):
-        """Default representation of the model.
-        """
+from warnings import warn
 
-        mod = f"{self.__class__.__name__} Model"
-        try:
-            mod += f': {self.filename}'
-        except AttributeError:
-            pass
-        s = [mod]
-        for name, v in self.metadata.items():
-            s += [f"{name:16} : {v}"]
-        return '\n'.join(s)
+import snewpy.models
+from snewpy.flavor_transformation import *
+from snewpy.neutrino import MassHierarchy
+from snewpy.rate_calculator import RateCalculator, center
+from snewpy.flux import Container
+logger = logging.getLogger(__name__)
 
-    def __post_init_check(self):
-        """A function to check model integrity after initialization"""
-        try:
-            t = self.time
-            m = self.metadata
-        except AttributeError as e:
-            clsname = self.__class__.__name__
-            raise TypeError(f"Model not initialized. Please call 'SupernovaModel.__init__' within the '{clsname}.__init__'") from e
-
-    def _repr_markdown_(self):
-        """Markdown representation of the model, for Jupyter notebooks.
-        """
-        mod = f'**{self.__class__.__name__} Model**'
-        try:
-            mod +=f': {self.filename}'
-        except:
-            pass
-        s = [mod,'']
-        if self.metadata:
-            s += ['|Parameter|Value|',
-                  '|:--------|:----:|']
-            for name, v in self.metadata.items():
-                try: 
-                    s += [f"|{name} | ${v.value:g}$ {v.unit:latex}|"]
-                except:
-                    s += [f"|{name} | {v} |"]
-        return '\n'.join(s)
-
-    def get_time(self):
-        """Returns
-        -------
-        ndarray of astropy.Quantity
-            Snapshot times from the simulation
-        """
-        return self.time
-
-    @abstractmethod
-    def get_initial_spectra(self, t, E, flavors=Flavor):
-        """Get neutrino spectra at the source.
-
-        Parameters
-        ----------
-        t : astropy.Quantity
-            Time to evaluate initial spectra.
-        E : astropy.Quantity or ndarray of astropy.Quantity
-            Energies to evaluate the initial spectra.
-        flavors: iterable of snewpy.neutrino.Flavor
-            Return spectra for these flavors only (default: all)
-
-        Returns
-        -------
-        initialspectra : dict
-            Dictionary of neutrino spectra, keyed by neutrino flavor.
-        """
-        pass
-
-    def get_initialspectra(self, *args):
-        """DO NOT USE! Only for backward compatibility!
-
-        :meta private:
-        """
-        warn("Please use `get_initial_spectra()` instead of `get_initialspectra()`!", FutureWarning)
-        return self.get_initial_spectra(*args)
-
-    def get_transformed_spectra(self, t, E, flavor_xform):
-        """Get neutrino spectra after applying oscillation.
-
-        Parameters
-        ----------
-        t : astropy.Quantity
-            Time to evaluate initial and oscillated spectra.
-        E : astropy.Quantity or ndarray of astropy.Quantity
-            Energies to evaluate the initial and oscillated spectra.
-        flavor_xform : FlavorTransformation
-            An instance from the flavor_transformation module.
-
-        Returns
-        -------
-        dict
-            Dictionary of transformed spectra, keyed by neutrino flavor.
-        """
-        initialspectra = self.get_initial_spectra(t, E)
-        transformed_spectra = {}
-
-        transformed_spectra[Flavor.NU_E] = \
-            flavor_xform.prob_ee(t, E) * initialspectra[Flavor.NU_E] + \
-            flavor_xform.prob_ex(t, E) * initialspectra[Flavor.NU_X]
-
-        transformed_spectra[Flavor.NU_X] = \
-            flavor_xform.prob_xe(t, E) * initialspectra[Flavor.NU_E] + \
-            flavor_xform.prob_xx(t, E) * initialspectra[Flavor.NU_X] 
-
-        transformed_spectra[Flavor.NU_E_BAR] = \
-            flavor_xform.prob_eebar(t, E) * initialspectra[Flavor.NU_E_BAR] + \
-            flavor_xform.prob_exbar(t, E) * initialspectra[Flavor.NU_X_BAR]
-
-        transformed_spectra[Flavor.NU_X_BAR] = \
-            flavor_xform.prob_xebar(t, E) * initialspectra[Flavor.NU_E_BAR] + \
-            flavor_xform.prob_xxbar(t, E) * initialspectra[Flavor.NU_X_BAR] 
-
-        return transformed_spectra   
-
-    def get_flux (self, t, E, distance, flavor_xform=NoTransformation()):
-        """Get neutrino flux through 1cm^2 surface at the given distance
-
-        Parameters
-        ----------
-        t : astropy.Quantity
-            Time to evaluate the neutrino spectra.
-        E : astropy.Quantity or ndarray of astropy.Quantity
-            Energies to evaluate the the neutrino spectra.
-        distance : astropy.Quantity or float (in kpc)
-            Distance from supernova.
-        flavor_xform : FlavorTransformation
-            An instance from the flavor_transformation module.
-
-        Returns
-        -------
-        dict
-            Dictionary of neutrino fluxes in [neutrinos/(cm^2*erg*s)], 
-            keyed by neutrino flavor.
-
-        """
-        distance = distance << u.kpc #assume that provided distance is in kpc, or convert
-        factor = 1/(4*np.pi*(distance.to('cm'))**2)
-        f = self.get_transformed_spectra(t, E, flavor_xform)
-
-        array = np.stack([f[flv] for flv in sorted(Flavor)])
-        return  Flux(data=array*factor, flavor=np.sort(Flavor), time=t, energy=E)
-
-
-
-    def get_oscillatedspectra(self, *args):
-        """DO NOT USE! Only for backward compatibility!
-
-        :meta private:
-        """
-        warn("Please use `get_transformed_spectra()` instead of `get_oscillatedspectra()`!", FutureWarning)
-        return self.get_transformed_spectra(*args)
-
-def get_value(x):
-    """If quantity x has is an astropy Quantity with units, return just the
-    value.
+def generate_time_series(model_path, model_type, transformation_type, d, output_filename=None, ntbins=30, deltat=None, snmodel_dict={}):
+    """Generate time series files in SNOwGLoBES format.
+
+    This version will subsample the times in a supernova model, produce energy
+    tables expected by SNOwGLoBES, and compress the output into a tarfile.
 
     Parameters
     ----------
-    x : Quantity, float, or ndarray
-        Input quantity.
+    model_path : str
+        Input file containing neutrino flux information from supernova model.
+    model_type : str
+        Format of input file. Matches the name of the corresponding class in :py:mod:`snewpy.models`.
+    transformation_type : str
+        Name of flavor transformation. See snewpy.flavor_transformation documentation for possible values.
+    d : int or float
+        Distance to supernova in kpc.
+    output_filename : str or None
+        Name of output file. If ``None``, will be based on input file name.
+    ntbins : int
+        Number of time slices. Will be ignored if ``deltat`` is also given.
+    deltat : astropy.Quantity or None
+        Length of time slices.
+    snmodel_dict : dict
+        Additional arguments for setting up the supernova model. See documentation of relevant ``SupernovaModel`` subclass for available options. (Optional)
 
     Returns
     -------
-    value : float or ndarray
-    
-    :meta private:
+    str
+        Path of NumPy archive file with neutrino fluence data.
     """
-    if type(x) == Quantity:
-        return x.value
-    return x
-
-class PinchedModel(SupernovaModel):
-    """Subclass that contains spectra/luminosity pinches"""
-    def __init__(self, simtab, metadata):
-        """ Initialize the PinchedModel using the data from the given table.
-
-        Parameters
-        ----------
-        simtab: astropy.Table 
-            Should contain columns TIME, {L,E,ALPHA}_NU_{E,E_BAR,X,X_BAR}
-            The values for X_BAR may be missing, then NU_X data will be used
-        metadata: dict
-            Model parameters dict
-        """
-        if not 'L_NU_X_BAR' in simtab.colnames:
-            # table only contains NU_E, NU_E_BAR, and NU_X, so double up
-            # the use of NU_X for NU_X_BAR.
-            for val in ['L','E','ALPHA']:
-                simtab[f'{val}_NU_X_BAR'] = simtab[f'{val}_NU_X']
-        # Get grid of model times.
-        time = simtab['TIME'] << u.s
-        # Set up dictionary of luminosity, mean energy and shape parameter
-        # alpha, keyed by neutrino flavor (NU_E, NU_X, NU_E_BAR, NU_X_BAR).
-        self.luminosity = {}
-        self.meanE = {}
-        self.pinch = {}
-        for f in Flavor:
-            self.luminosity[f] = simtab[f'L_{f.name}'] << u.erg/u.s
-            self.meanE[f] = simtab[f'E_{f.name}'] << u.MeV
-            self.pinch[f] = simtab[f'ALPHA_{f.name}']
-        super().__init__(time, metadata)
-
-
-    def get_initial_spectra(self, t, E, flavors=Flavor):
-        """Get neutrino spectra/luminosity curves before oscillation.
-
-        Parameters
-        ----------
-        t : astropy.Quantity
-            Time to evaluate initial spectra.
-        E : astropy.Quantity or ndarray of astropy.Quantity
-            Energies to evaluate the initial spectra.
-        flavors: iterable of snewpy.neutrino.Flavor
-            Return spectra for these flavors only (default: all)
-
-        Returns
-        -------
-        initialspectra : dict
-            Dictionary of model spectra, keyed by neutrino flavor.
-        """
-        #convert input arguments to 1D arrays
-        t = u.Quantity(t, ndmin=1)
-        E = u.Quantity(E, ndmin=1)
-        #Reshape the Energy array to shape [1,len(E)]
-        E = np.expand_dims(E, axis=0)
-
-        initialspectra = {}
-
-        # Avoid division by zero in energy PDF below.
-        E[E==0] = np.finfo(float).eps * E.unit
-
-        # Estimate L(t), <E_nu(t)> and alpha(t). Express all energies in erg.
-        E = E.to_value('erg')
-
-        # Make sure input time uses the same units as the model time grid, or
-        # the interpolation will not work correctly.
-        t = t.to(self.time.unit)
-
-        for flavor in flavors:
-            # Use np.interp rather than scipy.interpolate.interp1d because it
-            # can handle dimensional units (astropy.Quantity).
-            L  = get_value(np.interp(t, self.time, self.luminosity[flavor].to('erg/s')))
-            Ea = get_value(np.interp(t, self.time, self.meanE[flavor].to('erg')))
-            a  = np.interp(t, self.time, self.pinch[flavor])
-
-            #Reshape the time-related arrays to shape [len(t),1]
-            L  = np.expand_dims(L, axis=1)
-            Ea = np.expand_dims(Ea,axis=1)
-            a  = np.expand_dims(a, axis=1)
-            # For numerical stability, evaluate log PDF and then exponentiate.
-            result = \
-              np.exp(np.log(L) - (2+a)*np.log(Ea) + (1+a)*np.log(1+a)
-                    - loggamma(1+a) + a*np.log(E) - (1+a)*(E/Ea)) / (u.erg * u.s)
-            #remove bad values
-            result[np.isnan(result)] = 0
-            #remove unnecessary dimensions, if E or t was scalar:
-            result = np.squeeze(result)
-            initialspectra[flavor] = result
-        return initialspectra
-
-
-class _GarchingArchiveModel(PinchedModel):
-    """Subclass that reads models in the format used in the
-    `Garching Supernova Archive <https://wwwmpa.mpa-garching.mpg.de/ccsnarchive/>`_."""
-    def __init__(self, filename, eos='LS220', metadata={}):
-        """Model Initialization.
-
-        Parameters
-        ----------
-        filename : str
-            Absolute or relative path to file with model data, we add nue/nuebar/nux.  This argument will be deprecated.
-        eos: str
-            Equation of state. Valid value is 'LS220'. This argument will be deprecated.
-
-        Other Parameters
-        ----------------
-        progenitor_mass: astropy.units.Quantity
-            Mass of model progenitor in units Msun. Valid values are {progenitor_mass}.
-        Raises
-        ------
-        FileNotFoundError
-            If a file for the chosen model parameters cannot be found
-        ValueError
-            If a combination of parameters is invalid when loading from parameters
-        """
-        if not metadata:
-            metadata = {
-                'Progenitor mass': float(os.path.basename(filename).split('s')[1].split('c')[0]) * u.Msun,
-                'EOS': eos,
-            }
-
-        # Read through the several ASCII files for the chosen simulation and
-        # merge the data into one giant table.
-        mergtab = None
-        for flavor in Flavor:
-            _flav = Flavor.NU_X if flavor == Flavor.NU_X_BAR else flavor
-            _sfx = _flav.name.replace('_', '').lower()
-            _filename = '{}_{}_{}'.format(filename, eos, _sfx)
-            _lname = 'L_{}'.format(flavor.name)
-            _ename = 'E_{}'.format(flavor.name)
-            _e2name = 'E2_{}'.format(flavor.name)
-            _aname = 'ALPHA_{}'.format(flavor.name)
-
-            # Open the requested filename using the model downloader.
-            datafile = _model_downloader.get_model_data(self.__class__.__name__, _filename)
-
-            simtab = Table.read(datafile,
-                                names=['TIME', _lname, _ename, _e2name],
-                                format='ascii')
-            simtab['TIME'].unit = 's'
-            simtab[_lname].unit = '1e51 erg/s'
-            simtab[_aname] = (2*simtab[_ename]**2 - simtab[_e2name]) / (simtab[_e2name] - simtab[_ename]**2)
-            simtab[_ename].unit = 'MeV'
-            del simtab[_e2name]
+    model_class = getattr(snewpy.models.ccsn, model_type)
 
-            if mergtab is None:
-                mergtab = simtab
-            else:
-                mergtab = join(mergtab, simtab, keys='TIME', join_type='left')
-                mergtab[_lname].fill_value = 0.
-                mergtab[_ename].fill_value = 0.
-                mergtab[_aname].fill_value = 0.
-        simtab = mergtab.filled()
-        super().__init__(simtab, metadata)
-
-
-class _RegistryModel(ABC):
-    """Base class for supernova model classes that initialise from physics parameters."""
-
-    _param_validator = None
-
-    @classmethod
-    def get_param_combinations(cls):
-        """Returns all valid combinations of parameters for a given SNEWPY register model.
-
-        Subclasses can provide a Callable `cls._param_validator` that takes a combination of parameters
-        as an argument and returns True if a particular combinations of parameters is valid.
-        If None is provided, all combinations are considered valid.
-
-        Returns
-        -------
-        valid_combinations: tuple[dict]
-            A tuple of all valid parameter combinations stored as Dictionaries
-        """
-        for key, val in cls.param.items():
-            if not isinstance(val, (list, Quantity)):
-                cls.param[key] = [val]
-            elif isinstance(val, Quantity) and val.size == 1:
-                try:
-                    # check if val.value is iterable, e.g. a list or a NumPy array
-                    iter(val.value)
-                except:
-                    cls.param[key] = [val.value] * val.unit
-        combos = tuple(dict(zip(cls.param, combo)) for combo in it.product(*cls.param.values()))
-        return tuple(c for c in filter(cls._param_validator, combos))
-
-    def check_valid_params(cls, **user_params):
-        """Checks that the model-specific values, units, names and conbinations of requested parameters are valid.
-
-        Parameters
-        ----------
-        user_params : varies
-            User-requested model parameters to be tested for validity.
-            NOTE: This must be provided as kwargs that match the keys of cls.param
-
-        Raises
-        ------
-        ValueError
-            If invalid model parameters are provided based on units, allowed values, etc.
-        UnitTypeError
-            If invalid units are provided for a model parameter
-
-        See Also
-        --------
-        snewpy.models.ccsn
-        snewpy.models.presn
-        """
-        # Check that the appropriate number of params are provided
-        if not all(key in user_params for key in cls.param.keys()):
-            raise ValueError(f"Missing parameter! Expected {cls.param.keys()} but was given {user_params.keys()}")
-
-        # Check parameter units and values
-        for (key, allowed_params), user_param in zip(cls.param.items(), user_params.values()):
-
-            # If both have units, check that the user param value is valid. If valid, continue. Else, error
-            if type(user_param) == Quantity and type(allowed_params) == Quantity:
-                if get_physical_type(user_param.unit) != get_physical_type(allowed_params.unit):
-                    raise UnitTypeError(f"Incorrect units {user_param.unit} provided for parameter {key}, "
-                                        f"expected {allowed_params.unit}")
-
-                elif np.isin(user_param.to(allowed_params.unit).value, allowed_params.value):
-                    continue
-                else:
-                    raise ValueError(f"Invalid value '{user_param}' provided for parameter {key}, "
-                                     f"allowed value(s): {allowed_params}")
-
-            # If one only one has units, then error
-            elif (type(user_param) == Quantity) ^ (type(allowed_params) == Quantity):
-                # User param has units, model param is unitless
-                if type(user_param) == Quantity:
-                    raise ValueError(f"Invalid units {user_param.unit} for parameter {key} provided, expected None")
-                else:
-                    raise ValueError(f"Missing units for parameter {key}, expected {allowed_params.unit}")
-
-            # Check that unitless user param value is valid. If valid, continue. Else, Error
-            elif user_param in allowed_params:
-                continue
+    # Choose flavor transformation. Use dict to associate the transformation name with its class.
+    flavor_transformation_dict = {'NoTransformation': NoTransformation(), 'AdiabaticMSW_NMO': AdiabaticMSW(mh=MassHierarchy.NORMAL), 'AdiabaticMSW_IMO': AdiabaticMSW(mh=MassHierarchy.INVERTED), 'NonAdiabaticMSWH_NMO': NonAdiabaticMSWH(mh=MassHierarchy.NORMAL), 'NonAdiabaticMSWH_IMO': NonAdiabaticMSWH(mh=MassHierarchy.INVERTED), 'TwoFlavorDecoherence': TwoFlavorDecoherence(), 'ThreeFlavorDecoherence': ThreeFlavorDecoherence(), 'NeutrinoDecay_NMO': NeutrinoDecay(mh=MassHierarchy.NORMAL), 'NeutrinoDecay_IMO': NeutrinoDecay(mh=MassHierarchy.INVERTED), 'QuantumDecoherence_NMO': QuantumDecoherence(mh=MassHierarchy.NORMAL), 'QuantumDecoherence_IMO': QuantumDecoherence(mh=MassHierarchy.INVERTED)}
+    flavor_transformation = flavor_transformation_dict[transformation_type]
+
+    model_dir, model_file = os.path.split(os.path.abspath(model_path))
+    snmodel = model_class(model_path, **snmodel_dict)
+
+    # Subsample the model time. Default to 30 time slices.
+    tmin = snmodel.get_time()[0]
+    tmax = snmodel.get_time()[-1]
+    if deltat is not None:
+        dt = deltat
+        ntbins = int((tmax-tmin)/dt)
+    else:
+        dt = (tmax - tmin) / (ntbins+1)
+
+    times = np.arange(tmin/u.s, tmax/u.s, dt/u.s)*u.s
+    energy = np.linspace(0, 100, 501) * u.MeV
+    flux = snmodel.get_flux(t=times, E=energy,  distance=d, flavor_xform=flavor_transformation)
+    fluence = flux.integrate('time', limits = times).integrate('energy', limits = energy)
+    #save resulting fluence to file
+    if output_filename is not None:
+        tfname = output_filename + '.npz'
+    else:
+        model_file_root, _ = os.path.splitext(model_file)  # strip extension (if present)
+        tfname = f'{model_file_root}.{transformation_type}.{tmin:.3f},{tmax:.3f},{ntbins:d}-{d:.1f}.npz'
+    fluence.save(tfname)
+    return tfname
+
+def generate_fluence(model_path, model_type, transformation_type, d, output_filename=None, tstart=None, tend=None, snmodel_dict={}):
+    """Generate fluence files in SNOwGLoBES format.
+
+    This version will subsample the times in a supernova model, produce energy
+    tables expected by SNOwGLoBES, and compress the output into a tarfile.
+
+    Parameters
+    ----------
+    model_path : str
+        Input file containing neutrino flux information from supernova model.
+    model_type : str
+        Format of input file. Matches the name of the corresponding class in :py:mod:`snewpy.models`.
+    transformation_type : str
+        Name of flavor transformation. See snewpy.flavor_transformation documentation for possible values.
+    d : int or float
+        Distance to supernova in kpc.
+    output_filename : str or None
+        Name of output file. If ``None``, will be based on input file name.
+    tstart : astropy.Quantity or None
+        Start of time interval to integrate over, or list of start times of the time series bins.
+    tend : astropy.Quantity or None
+        End of time interval to integrate over, or list of end times of the time series bins.
+    snmodel_dict : dict
+        Additional arguments for setting up the supernova model. See documentation of relevant ``SupernovaModel`` subclass for available options. (Optional)
+
+    Returns
+    -------
+    str
+        Path of NumPy archive file with neutrino fluence data.
+    """
+    model_class = getattr(snewpy.models.ccsn, model_type)
+
+    # Choose flavor transformation. Use dict to associate the transformation name with its class.
+    flavor_transformation_dict = {'NoTransformation': NoTransformation(), 'AdiabaticMSW_NMO': AdiabaticMSW(mh=MassHierarchy.NORMAL), 'AdiabaticMSW_IMO': AdiabaticMSW(mh=MassHierarchy.INVERTED), 'NonAdiabaticMSWH_NMO': NonAdiabaticMSWH(mh=MassHierarchy.NORMAL), 'NonAdiabaticMSWH_IMO': NonAdiabaticMSWH(mh=MassHierarchy.INVERTED), 'TwoFlavorDecoherence': TwoFlavorDecoherence(), 'ThreeFlavorDecoherence': ThreeFlavorDecoherence(), 'NeutrinoDecay_NMO': NeutrinoDecay(mh=MassHierarchy.NORMAL), 'NeutrinoDecay_IMO': NeutrinoDecay(mh=MassHierarchy.INVERTED), 'QuantumDecoherence_NMO': QuantumDecoherence(mh=MassHierarchy.NORMAL), 'QuantumDecoherence_IMO': QuantumDecoherence(mh=MassHierarchy.INVERTED)}
+    flavor_transformation = flavor_transformation_dict[transformation_type]
+
+    model_dir, model_file = os.path.split(os.path.abspath(model_path))
+    snmodel = model_class(model_path, **snmodel_dict)
+
+    #set the timings up
+    #default if inputs are None: full time window of the model
+    times = None
+    if tstart is not None and tend is not None:
+        try:
+            #in case we have arrays: join them together
+            times = np.append(tstart, tend)
+            #and get rid of the duplicates with 1e-10 tolerance
+            times = np.unique(times.round(decimals=10))
+        except:
+            #in case we have single values
+            times = u.Quantity([tstart,tend])
+        times.sort()
+
+    #energy with 0.2 MeV binning
+    energy   = np.arange(0, 101, 0.2) << u.MeV
+    #energy bins similar to SNOwGLoBES
+    energy_t = (np.linspace(0, 100, 201)+0.25) << u.MeV 
+    flux = snmodel.get_flux(t=snmodel.get_time(), E=energy,  distance=d, flavor_xform=flavor_transformation)
+    fluence = flux.integrate('time', limits = times).integrate('energy', limits = energy_t)
+    times = fluence.time
+    #store the energy bin centers instead of the edges
+    if output_filename is not None:
+        tfname = output_filename+'.npz'
+    else:
+        model_file_root, _ = os.path.splitext(model_file)  # strip extension (if present)
+        tfname = f'{model_file_root}.{transformation_type}.{times[0]:.3f},{times[1]:.3f},{len(times)-1:d}-{d:.1f}.npz'
+
+    fluence.save(tfname)
+    return tfname
+
+def simulate(SNOwGLoBESdir, tarball_path, detector_input="all", verbose=False, *, detector_effects=True):
+    """Calculate expected event rates for the given neutrino flux files and the given (set of) SNOwGLoBES detector(s).
+    These event rates are given as a function of the neutrino energy and time, for each interaction channel.
+
+    Parameters
+    ----------
+    SNOwGLoBESdir : str or None
+        Path to SNOwGLoBES directory. Set to ``None`` to automatically use the latest supported SNOwGLoBES release.
+    tarball_path : str
+        Path of compressed .tar file produced e.g. by ``generate_time_series()`` or ``generate_fluence()``.
+    detector_input : str
+        Name of detector. If ``"all"``, will use all detectors supported by SNOwGLoBES.
+    verbose : bool
+        [DEPRECATED, DO NOT USE.]
+    detector_effects : bool
+         Whether to account for detector smearing and efficiency.
+    """
+    if verbose:  # Deprecated since SNEWPY v1.2
+        warn(f"The 'verbose' parameter to 'snewpy.snowglobes.simulate()' is deprecated and should not be used.", FutureWarning)
+
+    rc = RateCalculator(base_dir=SNOwGLoBESdir)
+    if detector_input == 'all':
+        detector_input = list(rc.detectors)
+    if(isinstance(detector_input,str)):
+        detector_input=[detector_input]
+    rates_dict = {}
+    #read the fluence
+    fluence = Container.load(tarball_path)
+    for det in detector_input:
+        rates_smeared=rc.run(fluence, det, detector_effects=True)
+        rates_unsmeared=rc.run(fluence, det, detector_effects=False)
+        #collect everything to pandas DataFrame, to make the output similar to previous
+        rates_dict[det]={'weighted':{'unsmeared':rates_unsmeared,
+                                 'smeared':rates_smeared,
+                                }}
+    # reorder results to produce the same format as before:
+    #    {detector: {time_bin:{'weighted':{smeared/unsmeared: [rate vs energy bins]}}}}
+    result = {}
+    fname_base = tarball_path[:tarball_path.rfind('.')]
+    for det in rates_dict:
+        #get the time bins
+        rates_smeared   = rates_dict[det]['weighted']['smeared']
+        rates_unsmeared = rates_dict[det]['weighted']['unsmeared']
+
+        #get the first rate from the dict to access the energy and time binning
+        some_rate = list(rates_smeared.values())[0]
+        tbins = center(some_rate.time)
+        ebins = center(some_rate.energy)
+        result[det] = {}
+        for n_bin, t_bin in enumerate(tbins):
+            data = {**{(chan,'unsmeared','weighted'): rate.array[0,n_bin,:]
+                      for chan,rate in rates_unsmeared.items()},
+                    **{(chan,'smeared','weighted'): rate.array[0,n_bin,:] 
+                      for chan,rate in rates_smeared.items()}}
+            
+            df = pd.DataFrame(data, index = ebins)
+            df.index.rename('E', inplace=True)
+            df.columns.rename(['channel','is_smeared','is_weighted'], inplace=True)
+            df = df.reorder_levels([2,1,0], axis='columns')
+            if len(tbins) > 1:
+                result[det][f'{fname_base}_{n_bin:01d}'] = df
             else:
-                raise ValueError(f"Invalid value '{user_param}' provided for parameter {key}, "
-                                 f"allowed value(s): {allowed_params}")
+                result[det][f'{fname_base}'] = df
+        
+    # save result to file for re-use in collate()
+    cache_file = f'{fname_base}.npy'
+    logging.info(f'Saving simulation results to {cache_file}')
+    np.save(cache_file, result)
+    return result
+
+
+re_chan_label = re.compile(r'nu(e|mu|tau)(bar|)_([A-Z][a-z]*)(\d*)_?(.*)')
+def get_channel_label(c):
+    mapp = {'nc':'NeutralCurrent',
+            'ibd':'Inverse Beta Decay',
+            'e':r'${\nu}_x+e^-$'}
+    def gen_label(m):
+        flv,bar,Nuc,num,res = m.groups()
+        if flv!='e':
+            flv='\\'+flv
+        if bar:
+            bar='\\'+bar
+        s = f'${bar}{{\\nu}}_{flv}$ '+f'${{}}^{{{num}}}{Nuc}$ '+res
+        return s
+
+    if c in mapp:
+        return mapp[c]
+    else: 
+        return re_chan_label.sub(gen_label, c) 
+
+def collate(SNOwGLoBESdir, tarball_path, detector_input="", skip_plots=False, verbose=False, remove_generated_files=True, *, smearing=True):
+    """Collates SNOwGLoBES output files and generates plots or returns a data table.
+
+    Parameters
+    ----------
+    SNOwGLoBESdir : str or None
+        [DEPRECATED, DO NOT USE.]
+    tarball_path : str
+        Path of compressed .tar file produced e.g. by ``generate_time_series()`` or ``generate_fluence()``.
+    detector_input : str
+        [DEPRECATED, DO NOT USE. SNEWPY will use all detectors included in the tarball.]
+    skip_plots: bool
+        If False, it gives as output the plot of the energy distribution for each time bin and for each interaction channel.
+    verbose : bool
+        [DEPRECATED, DO NOT USE.]
+    remove_generated_files: bool
+        [DEPRECATED, DO NOT USE.]
+    smearing: bool
+        Also consider results with smearing effects.
 
-        # Check Combinations (Logic lives inside model subclasses under model.isvalid_param_combo)
-        if user_params not in cls.get_param_combinations():
-            raise ValueError(
-                f"Invalid parameter combination. See {cls.__class__.__name__}.get_param_combinations() for a "
-                "list of allowed parameter combinations.")
+    Returns
+    -------
+    dict
+        Dictionary of data tables: One table per time bin; each table contains in the first column the energy bins, in the remaining columns the number of events for each interaction channel in the detector.
+    """
+    if verbose:  # Deprecated since SNEWPY v1.2
+        warn(f"The 'verbose' parameter to 'snewpy.snowglobes.collate()' is deprecated and should not be used.", FutureWarning)
+    if detector_input:  # Deprecated since SNEWPY v1.2
+        warn(f"The 'detector_input' parameter to 'snewpy.snowglobes.collate()' is deprecated and should not be used.", FutureWarning)
+    if not remove_generated_files:  # Deprecated since SNEWPY v1.2
+        warn(f"The 'remove_generated_files' parameter to 'snewpy.snowglobes.collate()' is deprecated and should not be used.", FutureWarning)
+
+    def aggregate_channels(table, **patterns):
+        #rearrange the table to have only channel column
+        levels = list(table.columns.names)
+        levels.remove('channel')
+        t = table.stack(levels)
+        for name,pattern in patterns.items():
+            #get channels which contain `like`
+            t_sel = t.filter(like=pattern)
+            #sum over them and save to a separate column
+            t_agg = t_sel.sum(axis='columns')
+            #drop processed channels
+            t.drop(t_sel.columns, axis='columns',inplace=True)
+            t[name]=t_agg #fill the column
+        #return table with the original levels order
+        t = t.unstack(levels)
+        t = t.reorder_levels(table.columns.names, axis=1)
+        return t
+        
+    def do_plot(table, params):
+        #plotting the events from given table
+        flux,det,weighted,smeared = params
+        for c in table.columns:
+            if table[c].max() > 0.1:
+                plt.plot(table[c],drawstyle='steps',label=get_channel_label(c), lw=1)
+        plt.xlim(right=0.10)
+        plt.ylim(bottom=0.10)
+        plt.yscale('log')
+        plt.legend(bbox_to_anchor=(0.5, 0.5, 0.5, 0.5), loc='best', borderaxespad=0)  # formats complete graph
+        smear_title = 'Interaction' if smeared=='unsmeared' else 'Detected'
+        plt.title(f'{flux} {det.capitalize()} {weighted.capitalize()} {smear_title} Events')
+        if smeared=='smeared':
+            plt.xlabel('Detected Energy (GeV)')
+            plt.ylabel('Events')  
+        else:
+            plt.xlabel('Neutrino Energy (GeV)')
+            plt.ylabel('Interaction Events')  
+
+    #read the results from storage
+    cache_file = tarball_path[:tarball_path.rfind('.')] + '.npy'
+    logging.info(f'Reading tables from {cache_file}')
+    tables = np.load(cache_file, allow_pickle=True).tolist()
+    #This output is similar to what produced by:
+    #tables = simulate(SNOwGLoBESdir, tarball_path,detector_input)
+
+    #dict for old-style results, for backward compatibiity
+    results = {}
+    smearing_options = ['smeared','unsmeared'] if smearing else ['unsmeared']
+    #save collated files:
+    with TemporaryDirectory(prefix='snowglobes') as tempdir:
+        tempdir = Path(tempdir)
+        for det in tables:
+            results[det] = {}
+            for flux,t in tables[det].items():
+                t = aggregate_channels(t,nc='nc_',e='_e')
+                for w in ['weighted']:
+                    for s in smearing_options:
+                        table = t[w][s]
+                        filename_base = f'{flux}_{det}_events_{s}_{w}'
+                        filename = tempdir/f'Collated_{filename_base}.dat'
+                        #save results to text files
+                        with open(filename,'w') as f:
+                            f.write(table.to_string(float_format='%23.15g'))
+                        #format the results for the output
+                        header = 'Energy '+' '.join(list(table.columns))
+                        data = table.to_numpy().T
+                        index = table.index.to_numpy()
+                        data = np.concatenate([[index],data])
+                        results[filename.name] = {'header':header,'data':data}
+                        #optionally plot the results
+                        if skip_plots is False:
+                            plt.figure(dpi=300)
+                            do_plot(table,(flux,det,w,s))
+                            filename = tempdir/f'{filename_base}_log_plot.png'
+                            plt.savefig(filename, dpi=300, bbox_inches='tight')
+                            plt.close()
+        #Make a tarfile with the condensed data files and plots
+        output_name = Path(tarball_path).stem
+        output_name = output_name[:output_name.rfind('.tar')]+'_SNOprocessed'
+        output_path = Path(tarball_path).parent/(output_name+'.tar.gz')
+        with tarfile.open(output_path, "w:gz") as tar:
+            for file in tempdir.iterdir():
+                tar.add(file,arcname=output_name+'/'+file.name)
+        logging.info(f'Created archive: {output_path}')
+    return results
```

### Comparing `snewpy-1.4b2/python/snewpy/models/loaders.py` & `snewpy-1.5/python/snewpy/models/ccsn_loaders.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,98 @@
 # -*- coding: utf-8 -*-
 """
-The submodule ``snewpy.models.loaders`` contains classes to load core-collapse
+The submodule ``snewpy.models.ccsn_loaders`` contains classes to load core-collapse
 supernova models from files stored on disk.
 """
 
 import logging
 import os
 import re
 import sys
 import tarfile
 
 from astropy import units as u
-from astropy.table import Table
+from astropy.table import Table, join
 from astropy.io import ascii, fits
 import h5py
 import numpy as np
 from scipy.special import gamma, lpmv
 
 try:
     import healpy as hp
 except ImportError:
     pass
 
-from snewpy.models.base import PinchedModel, _GarchingArchiveModel, SupernovaModel
+from snewpy.models.base import PinchedModel, SupernovaModel
 from snewpy.neutrino import Flavor
 from snewpy import _model_downloader
 
+class GarchingArchiveModel(PinchedModel):
+    """Subclass that reads models in the format used in the
+    `Garching Supernova Archive <https://wwwmpa.mpa-garching.mpg.de/ccsnarchive/>`_."""
+    def __init__(self, filename, eos='LS220', metadata={}):
+        """Model Initialization.
+
+        Parameters
+        ----------
+        filename : str
+            Absolute or relative path to file with model data, we add nue/nuebar/nux.  This argument will be deprecated.
+        eos: str
+            Equation of state. Valid value is 'LS220'. This argument will be deprecated.
+
+        Other Parameters
+        ----------------
+        progenitor_mass: astropy.units.Quantity
+            Mass of model progenitor in units Msun. Valid values are {progenitor_mass}.
+        Raises
+        ------
+        FileNotFoundError
+            If a file for the chosen model parameters cannot be found
+        ValueError
+            If a combination of parameters is invalid when loading from parameters
+        """
+        # Read through the several ASCII files for the chosen simulation and
+        # merge the data into one giant table.
+        mergtab = None
+        for flavor in Flavor:
+            _flav = Flavor.NU_X if flavor == Flavor.NU_X_BAR else flavor
+            _sfx = _flav.name.replace('_', '').lower()
+            _filename = '{}_{}_{}'.format(filename, eos, _sfx)
+            _lname = 'L_{}'.format(flavor.name)
+            _ename = 'E_{}'.format(flavor.name)
+            _e2name = 'E2_{}'.format(flavor.name)
+            _aname = 'ALPHA_{}'.format(flavor.name)
+
+            # Open the requested filename using the model downloader.
+            datafile = self.request_file(_filename)
+
+            simtab = Table.read(datafile,
+                                names=['TIME', _lname, _ename, _e2name],
+                                format='ascii')
+            simtab['TIME'].unit = 's'
+            simtab[_lname].unit = '1e51 erg/s'
+            simtab[_aname] = (2*simtab[_ename]**2 - simtab[_e2name]) / (simtab[_e2name] - simtab[_ename]**2)
+            simtab[_ename].unit = 'MeV'
+            del simtab[_e2name]
+
+            if mergtab is None:
+                mergtab = simtab
+            else:
+                mergtab = join(mergtab, simtab, keys='TIME', join_type='left')
+                mergtab[_lname].fill_value = 0.
+                mergtab[_ename].fill_value = 0.
+                mergtab[_aname].fill_value = 0.
+        simtab = mergtab.filled()
+        if not metadata:
+            metadata = {
+                'Progenitor mass': float(os.path.basename(filename).split('s')[1].split('c')[0]) * u.Msun,
+                'EOS': eos,
+            }
+        super().__init__(simtab, metadata)
+        
 class Nakazato_2013(PinchedModel):
     def __init__(self, filename, metadata={}):
         """Model initialization.
 
         Parameters
         ----------
         filename : str
@@ -37,54 +100,54 @@
 
         Raises
         ------
         FileNotFoundError
             If a file for the chosen model parameters cannot be found
         """
         # Open the requested filename using the model downloader.
-        datafile = _model_downloader.get_model_data(self.__class__.__name__, filename)
+        datafile = self.request_file(filename)
         # Read FITS table using the astropy reader.
         simtab = Table.read(datafile)
 
         self.filename = os.path.basename(filename)
         super().__init__(simtab, metadata)
 
 
 class Sukhbold_2015(Nakazato_2013):
     pass
 
 
-class Tamborra_2014(_GarchingArchiveModel):
+class Tamborra_2014(GarchingArchiveModel):
     pass
 
 
-class Bollig_2016(_GarchingArchiveModel):
+class Bollig_2016(GarchingArchiveModel):
     pass
 
 
-class Walk_2018(_GarchingArchiveModel):
+class Walk_2018(GarchingArchiveModel):
     pass
 
 
-class Walk_2019(_GarchingArchiveModel):
+class Walk_2019(GarchingArchiveModel):
     pass
 
 
 class OConnor_2013(PinchedModel):
     """Model based on the black hole formation simulation in `O'Connor & Ott (2013) <https://arxiv.org/abs/1207.1100>`_.
     """
 
     def __init__(self, filename, metadata={}):
         """
         Parameters
         ----------
         filename : str
             Absolute or relative path to FITS file with model data.
         """
-        datafile = _model_downloader.get_model_data(self.__class__.__name__, filename)
+        datafile = self.request_file(filename)
         # Open luminosity file.
         with tarfile.open(datafile) as tf:
             # Extract luminosity data.
             dataname = 's{:d}_{}_timeseries.dat'.format(int(metadata['Progenitor mass'].value), metadata['EOS'])
             # Read FITS table using the astropy reader.
             simtab = ascii.read(tf.extractfile(dataname), names=['TIME', 'L_NU_E', 'L_NU_E_BAR', 'L_NU_X',
                                                                     'E_NU_E', 'E_NU_E_BAR', 'E_NU_X',
@@ -109,15 +172,15 @@
         """
         Parameters
         ----------
         filename : str
             Absolute or relative path to FITS file with model data.
         """
 
-        datafile = _model_downloader.get_model_data(self.__class__.__name__, filename)
+        datafile = self.request_file(filename)
         simtab = Table.read(datafile,
                             names=['TIME', 'L_NU_E', 'L_NU_E_BAR', 'L_NU_X',
                                     'E_NU_E', 'E_NU_E_BAR', 'E_NU_X',
                                     'RMS_NU_E', 'RMS_NU_E_BAR', 'RMS_NU_X'],
                             format='ascii')
 
         header = ascii.read(simtab.meta['comments'], delimiter='=', format='no_header', names=['key', 'val'])
@@ -153,15 +216,15 @@
         """
         Parameters
         ----------
         filename : str
             Absolute or relative path to file prefix, we add nue/nuebar/nux
         """
         # Open the requested filename using the model downloader.
-        datafile = _model_downloader.get_model_data(self.__class__.__name__, filename)
+        datafile = self.request_file(filename)
 
         # Open luminosity file.
         # Read data from HDF5 files, then store.
         f = h5py.File(datafile, 'r')
 
         simtab = Table()
 
@@ -200,15 +263,15 @@
         Parameters
         ----------
         filename : str
             Absolute or relative path to file prefix, we add nue/nuebar/nux
         """
 
         # Open the requested filename using the model downloader.
-        datafile = _model_downloader.get_model_data(self.__class__.__name__, filename)
+        datafile = self.request_file(filename)
         # Read ASCII data.
         simtab = Table.read(datafile, format='ascii')
 
         # Get grid of model times.
         simtab['TIME'] = simtab['Tpb[ms]'] << u.ms
         for f in [Flavor.NU_E, Flavor.NU_E_BAR, Flavor.NU_X]:
             fkey = re.sub('(E|X)_BAR', r'A\g<1>', f.name).lower()
@@ -331,15 +394,15 @@
             # Conversion of flavor to key name in the model HDF5 file.
             self._flavorkeys = {Flavor.NU_E: 'nu0',
                                 Flavor.NU_E_BAR: 'nu1',
                                 Flavor.NU_X: 'nu2',
                                 Flavor.NU_X_BAR: 'nu2'}
 
             # Open the requested filename using the model downloader.
-            datafile = _model_downloader.get_model_data(self.__class__.__name__, filename)
+            datafile = self.request_file(filename)
             # Open HDF5 data file.
             self._h5file = h5py.File(datafile, 'r')
 
             # Get grid of model times in seconds.
             self.time = self._h5file['nu0']['g0'].attrs['time'] * u.s
 
     def _read_fits(self, filename):
@@ -555,15 +618,15 @@
         for flavor in flavors:
 
             # Linear interpolation in flux.
             if interpolation.lower() == 'linear':
                 # Pad log(E) array with values where flux is fixed to zero.
                 _logE = np.log10(_E[flavor].to_value('MeV'))
                 _dlogE = np.diff(_logE)
-                _logEbins = np.insert(_logE, 0, np.log10(np.finfo(float).eps))
+                _logEbins = np.insert(_logE, 0, np.log10(np.finfo(float).eps * E.unit/u.MeV))
                 _logEbins = np.append(_logEbins, _logE[-1] + _dlogE[-1])
 
                 # Pad with values where flux is fixed to zero.
                 _dLdE = _spec[flavor].to_value(self.fluxunit)
                 _dLdE = np.insert(_dLdE, 0, 0.)
                 _dLdE = np.append(_dLdE, 0.)
 
@@ -591,22 +654,22 @@
 
 class Fornax_2021(SupernovaModel):
     def __init__(self, filename, metadata={}):
         """
         Parameters
         ----------
         filename : str
-            Absolute or relative path to FITS file with model data.
+            Absolute or relative path to HDF5 file with model data.
         """
+
+        # Open the requested filename using the model downloader.
+        datafile = self.request_file(filename)
         # Set up model metadata.
         self.progenitor_mass = float(filename.split('/')[-1].split('_')[2][:-1]) * u.Msun
         self.metadata = metadata
-
-        # Open the requested filename using the model downloader.
-        datafile = _model_downloader.get_model_data(self.__class__.__name__, filename)
         # Open HDF5 data file.
         _h5file = h5py.File(datafile, 'r')
 
         self.time = _h5file['nu0'].attrs['time'] * u.s
 
         self.luminosity = {}
         self._E = {}
@@ -655,50 +718,149 @@
 
         # Avoid "division by zero" in retrieval of the spectrum.
         E[E == 0] = np.finfo(float).eps * E.unit
         logE = np.log10(E.to_value('MeV'))
 
         # Make sure the input time uses the same units as the model time grid.
         # Convert input time to a time index.
-        t = t.to(self.time.unit)
-        j = (np.abs(t - self.time)).argmin()
+        t = u.Quantity(t.to(self.time.unit), ndmin=1)
+        j = np.array(list(np.abs(_t - self.time).argmin() for _t in t))
 
         for flavor in flavors:
             # Energy bin centers (in MeV)
             _E = self._E[flavor][j]
             _logE = np.log10(_E)
             _dlogE = np.diff(_logE)
 
             # Model flavors (internally) are nu_e, nu_e_bar, and nu_x, which stands
             # for nu_mu(_bar) and nu_tau(_bar), making the flux 4x higher than nu_e and nu_e_bar.
             factor = 1. if flavor.is_electron else 0.25
 
             # Linear interpolation in flux.
             if interpolation.lower() == 'linear':
                 # Pad log(E) array with values where flux is fixed to zero.
-                _logEbins = np.insert(_logE, 0, np.log10(np.finfo(float).eps))
-                _logEbins = np.append(_logEbins, _logE[-1] + _dlogE[-1])
+                _logEbins = np.insert(_logE, 0, np.log10(np.finfo(float).eps * E.unit/u.MeV), axis=1)
+                _logEbins = np.append(_logEbins, np.expand_dims(_logE[:,-1] + _dlogE[:,-1], 1), axis=1)
 
                 # Luminosity spectrum _dLdE is in units of 1e50 erg/s/MeV.
                 # Pad with values where flux is fixed to zero, then divide by E to get number luminosity
-                _dNLdE = np.asarray([0.] + [self._dLdE[flavor]['g{}'.format(i)][j] for i in range(12)] + [0.])
-                initialspectra[flavor] = (np.interp(logE, _logEbins, _dNLdE) / E *
-                                          factor * 1e50 * u.erg/u.s/u.MeV).to('1 / (erg s)')
+                _dNLdE = np.asarray([np.zeros(j.shape)] + [self._dLdE[flavor]['g{}'.format(i)][j] for i in range(12)] + [np.zeros(j.shape)]).T
+                interp_values = np.array([np.interp(logE, __logEbins, __dNLdE)
+                                          for __logEbins, __dNLdE in zip(_logEbins, _dNLdE)])
+                initialspectra[flavor] = (interp_values / E * factor * 1e50 * u.erg/u.s/u.MeV).to('1 / (erg s)')
 
             elif interpolation.lower() == 'nearest':
                 # Find edges of energy bins and identify which energy bin (each entry of) E falls into
-                _logEbinEdges = _logE - _dlogE[0] / 2
-                _logEbinEdges = np.concatenate((_logEbinEdges, [_logE[-1] + _dlogE[-1] / 2]))
+                _logEbinEdges = _logE - _dlogE[0,0] / 2
+                _logEbinEdges = np.append(_logEbinEdges, np.expand_dims(_logE[:,-1] + _dlogE[:,-1]/2, 1), axis=1)
                 _EbinEdges = 10**_logEbinEdges
-                idx = np.searchsorted(_EbinEdges, E) - 1
-                select = (idx > 0) & (idx < len(_E))
+                idx = np.array([np.searchsorted(edges, E) - 1 for edges in _EbinEdges])
+                select = np.array([(_idx > 0) & (_idx < len(__E)) for _idx, __E in zip(idx, _E)])
 
                 # Divide luminosity spectrum by energy at bin center to get number luminosity spectrum
-                _dNLdE = np.zeros(len(E))
-                _dNLdE[np.where(select)] = np.asarray(
-                    [self._dLdE[flavor]['g{}'.format(i)][j] / _E[i] for i in idx[select]])
+                _dNLdE = np.zeros([len(j), len(np.atleast_1d(E))])
+                for i in range(len(j)):
+                    _dNLdE[i][np.where(select[i])] = np.asarray([self._dLdE[flavor]['g{}'.format(ebin_idx)][j[i]] / _E[i][ebin_idx]
+                                                                 for ebin_idx in idx[i][select[i]]])
                 initialspectra[flavor] = ((_dNLdE << 1/u.MeV) * factor * 1e50 * u.erg/u.s/u.MeV).to('1 / (erg s)')
 
             else:
                 raise ValueError('Unrecognized interpolation type "{}"'.format(interpolation))
 
         return initialspectra
+
+
+class Fornax_2022(Fornax_2021):
+    def __init__(self, filename, metadata={}):
+        """
+        Parameters
+        ----------
+        filename : str
+            Absolute or relative path to HDF5 file with model data.
+        """
+        # Open the requested filename using the model downloader.
+        datafile = self.request_file(filename)
+        # Set up model metadata.
+        self.progenitor = os.path.splitext(os.path.basename(filename))[0].split('_')[2]
+        self.progenitor_mass = float(self.progenitor[:-3])*u.Msun if self.progenitor.endswith('bh') else float(self.progenitor)*u.Msun
+
+        self.metadata = metadata
+
+        # Open HDF5 data file.
+        _h5file = h5py.File(datafile, 'r')
+
+        self.metadata['PNS mass'] = _h5file.attrs['Mpns'] * u.Msun
+        self.time = _h5file['nu0'].attrs['time'] * u.s
+
+        self.luminosity = {}
+        self._E = {}
+        self._dLdE = {}
+        for flavor in Flavor:
+            # Convert flavor to key name in the model HDF5 file
+            key = {Flavor.NU_E: 'nu0',
+                   Flavor.NU_E_BAR: 'nu1',
+                   Flavor.NU_X: 'nu2',
+                   Flavor.NU_X_BAR: 'nu2'}[flavor]
+
+            self._E[flavor] = np.asarray(_h5file[key]['egroup'])
+            self._dLdE[flavor] = {f"g{i}": np.asarray(_h5file[key][f'g{i}']) for i in range(12)}
+
+            # Compute luminosity by integrating over model energy bins.
+            dE = np.asarray(_h5file[key]['degroup'])
+            n = len(dE[0])
+            dLdE = np.zeros((len(self.time), n), dtype=float)
+            for i in range(n):
+                dLdE[:, i] = self._dLdE[flavor][f"g{i}"]
+
+            # Note factor of 0.25 in nu_x and nu_x_bar.
+            factor = 1. if flavor.is_electron else 0.25
+            self.luminosity[flavor] = np.sum(dLdE*dE, axis=1) * factor * 1e50 * u.erg/u.s
+
+
+class Mori_2023(PinchedModel):
+    def __init__(self, filename, metadata={}):
+        """
+        Parameters
+        ----------
+        filename : str
+            Absolute or relative path to file prefix.
+        """
+        # Open the requested filename using the model downloader.
+        datafile = self.request_file(filename)
+
+        self.metadata = metadata
+
+        # Read ASCII data.
+        simtab = Table.read(datafile, format='ascii')
+
+        # Remove the first table row, which appears to have zero input.
+        simtab = simtab[simtab['1:t_sim[s]'] > 0]
+
+        # Get grid of model times.
+        simtab['TIME'] = simtab['2:t_pb[s]'] << u.s
+        for j, (f, fkey) in enumerate(zip([Flavor.NU_E, Flavor.NU_E_BAR, Flavor.NU_X], 'ebx')):
+            simtab[f'L_{f.name}'] = simtab[f'{6+j}:Le{fkey}[e/s]'] << u.erg / u.s
+            # Compute the pinch parameter from E_rms and E_avg
+            # <E^2> / <E>^2 = (2+a)/(1+a), where
+            # E_rms^2 = <E^2> - <E>^2.
+            Eavg = simtab[f'{9+j}:Em{fkey}[MeV]']
+            Erms = simtab[f'{12+j}:Er{fkey}[MeV]']
+            E2 = Erms**2 + Eavg**2
+            x = E2 / Eavg**2
+            alpha = (2-x) / (x-1)
+
+            simtab[f'E_{f.name}'] = Eavg << u.MeV
+            simtab[f'E2_{f.name}'] = E2 << u.MeV**2
+            simtab[f'ALPHA_{f.name}'] = alpha
+
+#            simtab[f'E_{f.name}'] = simtab[f'{9+j}:Em{fkey}[MeV]'] << u.MeV
+#            Erms = simtab[f'{12+j}:Er{fkey}[MeV]'] * u.MeV
+#
+#            # Compute the pinch parameter from E_rms and E_avg
+#            simtab[f'E2_{f.name}'] = Erms**2 + simtab[f'E_{f.name}']**2
+#            x = simtab[f'E2_{f.name}'] / simtab[f'E_{f.name}']**2
+#            simtab[f'ALPHA_{f.name}'] = (2-x) / (x-1)
+
+        self.filename = os.path.basename(filename)
+
+        super().__init__(simtab, metadata)
+
```

### Comparing `snewpy-1.4b2/python/snewpy/models/presn.py` & `snewpy-1.5/python/snewpy/models/presn_loaders.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,18 @@
+# -*- coding: utf-8 -*-
+"""
+The submodule ``snewpy.models.presn_loaders`` contains classes to load pre-supernova
+models from files stored on disk.
+"""
+
 import numpy as np
 import pandas as pd
 from scipy.interpolate import interp1d
 from astropy import units as u
-from .base import SupernovaModel
+from snewpy.models.base import SupernovaModel
 from snewpy.neutrino import Flavor
 from pathlib import Path
 
 def _interp_T(t0, v0, dt=1e-3, dv=1e-10, axis=0):
     "dilog interpolation"
     lt0 = np.log(t0 + dt)
     lv0 = np.log(v0 + dv)
@@ -28,37 +34,34 @@
     return _f
 
 class Odrzywolek_2010(SupernovaModel):
     """Set up a presupernova model, based on 
     [A. Odrzywolek and A. Heger, Acta Phys. Polon. B 41 (2010) 1611.]
     """
 
-    def __init__(self, fname):
+    def __init__(self, filename:str):
         df = pd.read_csv(
-            fname,
-            delim_whitespace=True,
+            self.request_file(filename),
+            sep='\s+',
             skiprows=1,
             usecols=[1,6,7,8],
             names=["time","a","alpha","b"],
             index_col="time",
         )
         # interpolated in time
         self.df_t = _interp_T(df.index, df)
         self.factor = {}
         for f in Flavor:
             if f.is_electron:
                 self.factor[f] = 1.0
             else:
                 # nuX/nuE ratio from Odrzywolek paper: (arXiv:astro-ph/0311012)
-                self.factor[f] = 0.36
-        self.filename = Path(fname).stem
-        self.progenitor_mass = float(self.filename.split('_')[0][1:]) * u.Msun
+                self.factor[f] = 0.19
         time = -df.index.to_numpy() << u.s
-        metadata = {'Progenitor Mass': self.progenitor_mass}
-        super().__init__(time, metadata)
+        super().__init__(time, self.metadata)
 
     def get_initial_spectra(self, t, E, flavors=Flavor):
         # negative t for time before SN
         t = -t.to_value("s")
         E = E.to_value("MeV")
         df = self.df_t(t)
         a, alpha, b = df.T
@@ -72,71 +75,67 @@
 
 
 class Patton_2017(SupernovaModel):
     """Set up a presupernova model based on 
     [Kelly M. Patton et al 2017 ApJ 851 6, 
      https://doi.org/10.5281/zenodo.2598709]
     """
-    def __init__(self, fname):
+    def __init__(self, filename:str):
         df = pd.read_csv(
-            fname,
+            self.request_file(filename),
             comment="#",
-            delim_whitespace=True,
+            sep='\s+',
             names=["time","Enu",Flavor.NU_E,Flavor.NU_E_BAR,Flavor.NU_X,Flavor.NU_X_BAR],
             usecols=range(6),
         )
 
         df = df.set_index(["time", "Enu"])
         times = df.index.levels[0].to_numpy()
         energies = df.index.levels[1].to_numpy()
         df = df.unstack("Enu")
         # make a 3d array
         self.array = np.stack([df[f] for f in Flavor], axis=0)
         self.interpolated = _interp_TE(
             times, energies, self.array, ax_t=1, ax_e=2
         )
-        self.filename = Path(fname).stem
-        self.progenitor_mass = float(self.filename.split('_')[-1].rstrip('SolarMass')) * u.Msun
-        metadata = {'Progenitor Mass': self.progenitor_mass}
-        super().__init__(times << u.hour, metadata)
+        super().__init__(times << u.hour, self.metadata)
 
     def get_initial_spectra(self, t, E, flavors=Flavor):
         t = np.array(-t.to_value("hour"), ndmin=1)
         E = np.array(E.to_value("MeV"), ndmin=1)
         flux = self.interpolated(t, E) / (u.MeV * u.s)
         return {f: flux[f] for f in flavors}
 
 class Kato_2017(SupernovaModel):
     """Set up a presupernova model based on 
     [Chinami Kato et al 2017 ApJ 848 48]
     """
     def __init__(self, path):
         fluxes = {}
         #reading the time steps values:
-        times, step = np.loadtxt(f"{path}/total_nue/lightcurve_nue_all.dat", usecols=[0, 3]).T
+        times, step = np.loadtxt(self.request_file(f"{path}/total_nue/lightcurve_nue_all.dat"), usecols=[0, 3]).T
 
         file_base = {Flavor.NU_E: 'total_nue/spe_all',
                  Flavor.NU_E_BAR:'total_nueb/spe_all',
                  Flavor.NU_X:    'total_nux/spe_sum_mu_nu',
                  Flavor.NU_X_BAR:'total_nux/spe_sum_mu'
                  }
         for flv,file_base in file_base.items():
             d2NdEdT = []
             for s in step:
-                energies, dNdE = np.loadtxt(f"{path}/{file_base}{s:05.0f}.dat").T
+                energies, dNdE = np.loadtxt(
+                    self.request_file(f"{path}/{file_base}{s:05.0f}.dat")
+                ).T
                 d2NdEdT += [dNdE]
             fluxes[flv] = np.stack(d2NdEdT)
         self.array = np.stack([fluxes[f] for f in Flavor], axis=0)
         self.interpolated = _interp_TE(
             times, energies, self.array, ax_t=1, ax_e=2
         )
-        self.filename = Path(path).stem
-        self.progenitor_mass = float(self.filename.strip('m')) * u.Msun
-        metadata = {'Progenitor Mass': self.progenitor_mass}
-        super().__init__(times << u.s, metadata)
+        super().__init__(times << u.s, self.metadata)
 
     def get_initial_spectra(self, t, E, flavors=Flavor):
         t = np.array(-t.to_value("s"), ndmin=1)
         E = np.array(E.to_value("MeV"), ndmin=1)
         flux = self.interpolated(t, E) / (u.MeV * u.s)
         return {f: flux[f] for f in flavors}
```

### Comparing `snewpy-1.4b2/python/snewpy/neutrino.py` & `snewpy-1.5/python/snewpy/neutrino.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,9 +224,9 @@
             dm21_2 = 7.53e-5 << u.eV**2,
             dm32_2 = -2.536e-3 << u.eV**2
         )
     }
 }
    
 
-def MixingParameters(mass_order:MassHierarchy=MassHierarchy.NORMAL, version:str='NuFIT5.0'):
-    return parameter_presets[version][mass_order]
+def MixingParameters(mh:MassHierarchy=MassHierarchy.NORMAL, version:str='NuFIT5.0'):
+    return parameter_presets[version][mh]
```

### Comparing `snewpy-1.4b2/python/snewpy/snowglobes_interface.py` & `snewpy-1.5/python/snewpy/snowglobes_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self.efficiencies = None
         self.smearings = None
         if detector_effects:
             self._load_efficiency_vectors(self.base_dir/'effic')
             self._load_smearing_matrices(self.base_dir/'smear')
 
     def _load_detectors(self, path:Path, detectors:str):
-        df = pd.read_table(path,names=['name','mass','factor'], delim_whitespace=True, comment='#')
+        df = pd.read_table(path, names=['name', 'mass', 'factor'], sep='\s+', comment='#')
         df['tgt_mass']=df.mass*df.factor
 
         if detectors == 'all':
             detectors = list(df['name'])
             detectors.remove('d2O')
         elif isinstance(detectors, str):
             detectors = [detectors]
@@ -104,25 +104,25 @@
             # in SNOwGLoBES v1.3, there are three different formats of channel files
             # We identify these based on their first line and read them in separately:
             with open(f) as _f:
                 l = _f.readline().strip()
             if l.startswith('%'):
                 # Format 1: explicit binning, same for all channels
                 tokens = l.split()[1:]
-                df = pd.read_table(f, delim_whitespace=True, index_col=1, comment='%', names=['name','n','parity','flavor','weight'])
+                df = pd.read_table(f, sep='\s+', index_col=1, comment='%', names=['name','n','parity','flavor','weight'])
             elif l.startswith('SN_nu'):
                 # Format 2: explicit binning, differs per channel
                 tokens = l.split()[6:]
-                df = pd.read_table(f, delim_whitespace=True, index_col=1, comment='%', names=['name','n','parity','flavor','weight'], usecols=range(1,6))
+                df = pd.read_table(f, sep='\s+', index_col=1, comment='%', names=['name','n','parity','flavor','weight'], usecols=range(1,6))
                 # drop coherent scattering channels, which have different binning
                 df = df[df["name"].str.startswith('coh_') == False]
             else:
                 # Format 3: no binning specified, use SNOwGLoBES default values
                 tokens = '% 200 0.0005 0.100 200 0.0005 0.100'.split()[1:]
-                df = pd.read_table(f, delim_whitespace=True, index_col=1, comment='%', names=['name','n','parity','flavor','weight'])
+                df = pd.read_table(f, sep='\s+', index_col=1, comment='%', names=['name','n','parity','flavor','weight'])
 
             self.channels[material] = df
 
             nsamples, smin, smax, nbins, emin, emax = [float(t) for t in tokens]
             self.binning[material] = {'e_true': np.linspace(smin, smax, int(nsamples)),
                                       'e_smear': np.linspace(emin, emax, int(nbins))
                                       }
@@ -132,15 +132,15 @@
         logger.debug(f'channels: {self.channels}')
 
     def _load_efficiency_vectors(self, path):
         result = {}
         for detector in self.detectors:
             res_det = {}
             for file in (path/str(detector)).glob(f'effic_*_{detector}.dat'):
-                channel =  file.stem[len('effic_'):-len(detector)-1]
+                channel = file.stem[len('effic_'):-len(detector)-1]
                 logger.debug(f'Reading file ({detector},{channel}): {file}')
                 with open(file) as f:
                     effs = np.fromiter(f.readlines()[0].split("{")[-1].split("}")[0].split(","), float)
                     res_det[channel]= effs
             result[detector]=res_det
         self.efficiencies = result 
         logger.info(f'read efficiencies for detectors: {list(self.efficiencies.keys())}')
```

### Comparing `snewpy-1.4b2/python/snewpy/test/_rate_crosscheck_table.py` & `snewpy-1.5/python/snewpy/test/_rate_crosscheck_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #generated by "make_rate_table.py" on 2023-06-02 14:05:49.504799
 rate_table= \
-{('Bollig_2016', 's11.2c', 'AdiabaticMSW_IMO'): {'ar40kt': 2680.934960405018,
+{('Bollig_2016', 's11.2c', 'AdiabaticMSW_IMO'): {'ar40kt': 2509.8697955822163,
                                                  'halo1': 3.7370536263087892,
                                                  'halo2': 47.30447628238974,
                                                  'icecube': 332587.17107218195,
                                                  'novaFD': 1955.8019842893325,
                                                  'novaND': 41.91004252048569,
                                                  'wc100kt30prct': 12723.21134007678},
- ('Bollig_2016', 's11.2c', 'AdiabaticMSW_NMO'): {'ar40kt': 2860.015571948873,
+ ('Bollig_2016', 's11.2c', 'AdiabaticMSW_NMO'): {'ar40kt': 2696.396378383758,
                                                  'halo1': 4.261668358305819,
                                                  'halo2': 53.94516909247873,
                                                  'icecube': 320766.2999953658,
                                                  'novaFD': 1947.9479073661355,
                                                  'novaND': 41.741740872131466,
                                                  'wc100kt30prct': 12645.788228369147},
- ('Bollig_2016', 's27.0c', 'AdiabaticMSW_IMO'): {'ar40kt': 5465.621983231249,
+ ('Bollig_2016', 's27.0c', 'AdiabaticMSW_IMO'): {'ar40kt': 5192.001233928208,
                                                  'halo1': 8.180298088573792,
                                                  'halo2': 103.54807707055436,
                                                  'icecube': 659449.9649827218,
                                                  'novaFD': 3638.7825760092305,
                                                  'novaND': 77.97391234305493,
                                                  'wc100kt30prct': 23596.070817047243},
- ('Bollig_2016', 's27.0c', 'AdiabaticMSW_NMO'): {'ar40kt': 5785.497035954946,
+ ('Bollig_2016', 's27.0c', 'AdiabaticMSW_NMO'): {'ar40kt': 5520.903869068218,
                                                  'halo1': 9.105675711861647,
                                                  'halo2': 115.2617178716664,
                                                  'icecube': 661517.4858901916,
                                                  'novaFD': 3734.4927394154874,
                                                  'novaND': 80.02484441604615,
                                                  'wc100kt30prct': 24241.28672972421}}
```

### Comparing `snewpy-1.4b2/python/snewpy/test/simplerate_integrationtest.py` & `snewpy-1.5/python/snewpy/test/simplerate_integrationtest.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 # -*- coding: utf-8 -*-
 """Integration test based on SNEWS2.0_rate_table_singleexample.py
 """
 import unittest
 from snewpy import snowglobes
+from snewpy import model_path 
+
+from snewpy.models import ccsn
+import astropy.units as u
+
+def preload_model(name:str, **parameters):
+    #initialize the model with given name and parameters
+    model = ccsn.__dict__[name](**parameters)
+    return model
 
 
 class TestSimpleRate(unittest.TestCase):
 
     def test_simplerate(self):
         """Integration test based on SNEWS2.0_rate_table_singleexample.py
         """
         # Hardcoded paths on GitHub Action runner machines
         SNOwGLoBES_path = None
-        SNEWPY_model_dir = "models/"
 
         distance = 10  # Supernova distance in kpc
         detector = "wc100kt30prct" #SNOwGLoBES detector for water Cerenkov
         modeltype = 'Bollig_2016' # Model type from snewpy.models
         model = 's11.2c' # Name of model
         transformation = 'AdiabaticMSW_NMO' # Desired flavor transformation
 
         # Construct file system path of model file and name of output file
-        model_path = SNEWPY_model_dir + "/" + modeltype + "/" + model
-        outfile = modeltype + "_" + model + "_" + transformation
+        model_file_path = f'{model_path}/{modeltype}/{model}'
+        outfile = f'{modeltype}_{model}_{transformation}'
 
+        #make sure the model files are loaded
+        preload_model(modeltype, progenitor_mass=11.2*u.Msun)
+        
         # Now, do the main work:
         print("Generating fluence files ...")
-        tarredfile = snowglobes.generate_fluence(model_path, modeltype, transformation, distance, outfile)
+        tarredfile = snowglobes.generate_fluence(model_file_path, modeltype, transformation, distance, outfile)
 
         print("Simulating detector effects with SNOwGLoBES ...")
         snowglobes.simulate(SNOwGLoBES_path, tarredfile, detector_input=detector, detector_effects=True)
 
         print("Collating results ...")
         tables = snowglobes.collate(SNOwGLoBES_path, tarredfile, skip_plots=True, smearing=True)
```

### Comparing `snewpy-1.4b2/python/snewpy/test/snewpy_test_suite.py` & `snewpy-1.5/python/snewpy/test/snewpy_test_suite.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.4b2/python/snewpy/test/test_01_registry.py` & `snewpy-1.5/python/snewpy/test/test_01_registry.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import unittest
 
 from snewpy.neutrino import Flavor
 from snewpy.flavor_transformation import NoTransformation
 from snewpy.models.ccsn import Nakazato_2013, Tamborra_2014, OConnor_2013, OConnor_2015, \
                           Sukhbold_2015, Bollig_2016, Walk_2018, \
                           Walk_2019, Fornax_2019, Warren_2020, \
-                          Kuroda_2020, Fornax_2021, Zha_2021
+                          Kuroda_2020, Fornax_2021, Zha_2021, \
+                          Fornax_2022, Mori_2023
 
 from astropy import units as u
 
 import numpy as np
 
 
 class TestModels(unittest.TestCase):
@@ -26,15 +27,18 @@
                   Bollig_2016,
                   Walk_2018,
                   Walk_2019,
                   Fornax_2019,
                   Warren_2020,
                   Kuroda_2020,
                   Fornax_2021,
-                  Zha_2021]
+                  Zha_2021,
+                  Fornax_2022,
+                  Mori_2023,
+                  ]
 
         for model in models:
             for pc in model.get_param_combinations():
                 model(**pc)  # Initialize
 
     def test_Nakazato_2013(self):
         """
@@ -317,11 +321,92 @@
 
             # Check that times are in proper units.
             t = model.get_time()
             self.assertTrue(t.unit, u.s)
 
             # Check that we can compute flux dictionaries.
             f = model.get_initial_spectra(0*u.s, 10*u.MeV)
+            self.assertEqual(type(f), dict)
+            self.assertEqual(len(f), len(Flavor))
+            self.assertEqual(f[Flavor.NU_E].unit, 1./(u.erg * u.s))
+
+    def test_Fornax_2022(self):
+        """
+        Instantiate a set of 'Fornax 2022' models
+        """
+        progenitors = Fornax_2022.param['progenitor_mass']
+        bh_masses = [12.  , 12.03, 12.07, 12.1 , 12.18, 12.2 , 12.33, 12.4 , 12.45,
+                      12.5 , 12.54, 12.6 , 12.72, 12.8 , 12.85, 12.9 , 12.97, 13.  ,
+                      13.05, 13.25, 13.27, 13.32, 13.4 , 13.5 , 13.6 , 13.82, 13.9 ,
+                      14.13, 14.25, 14.4 , 14.41, 14.44, 14.7 , 14.87, 15.  , 15.04,
+                      15.38]<<u.Msun
+        # PNS masses for each simulation, D. Vartanyan, private comm.
+        pns_masses = [  1.35 , 1.38 , 1.4  , 1.45 , 1.5  ,
+                        1.52 , 1.54 , 1.57 , 1.55 , 1.54 ,
+                        1.55 , 1.57 , 1.69 , 1.73 , 1.72 ,
+                        1.87 , 1.67 , 1.67 , 1.73 , 1.69 ,
+                        1.68 , 1.73 , 1.75 , 1.75 , 1.73 ,
+                        1.75 , 1.78 , 1.83 , 1.81 , 1.75 ,
+                        1.84 , 1.74 , 1.8  , 1.74 , 1.86 ,
+                        1.77 , 1.83 , 1.84 , 1.78 , 1.85 ,
+                        1.79 , 1.87 , 1.87 , 1.84 , 1.75 ,
+                        1.85 , 1.9  , 1.85 , 1.77 , 1.84 ,
+                        1.87 , 1.79 , 1.77 , 1.87 , 1.82 ,
+                        1.76 , 1.86 , 1.89 , 1.95 , 1.94 ,
+                        1.69 , 1.94 , 1.74 , 1.99 , 1.97 ,
+                        2.05 , 2.08 , 2.07 , 2.02 , 2.03 ,
+                        1.72 , 1.68 , 2.12 , 1.81 , 1.83 ,
+                        2.16 , 1.84 , 1.68 , 2.12 , 2.23 ,
+                        1.85 , 2.39 , 2.34 , 2.31 , 1.99 ,
+                        2.37 , 2.25 , 2.25 , 2.36 , 2.23 ,
+                        2.1  , 2.16 , 1.98 , 2.01 , 2.1  ,
+                        1.98 , 2.11 , 2.18 , 2.14 , 2.2 ]<<u.Msun
+        
+        for progenitor, m_pns in zip(progenitors, pns_masses):
+            model = Fornax_2022(progenitor_mass=progenitor)
+
+            self.assertEqual(model.metadata['Progenitor mass'], progenitor)
+            self.assertEqual(model.metadata['PNS mass'], m_pns)
+            self.assertEqual(model.metadata['Black hole'], progenitor in bh_masses)
+            # Check that times are in proper units.
+            t = model.get_time()
+            self.assertTrue(t.unit, u.s)
+
+            # Check that we can compute flux dictionaries.
+            f = model.get_initial_spectra(0*u.s, 10*u.MeV)
+            self.assertEqual(type(f), dict)
+            self.assertEqual(len(f), len(Flavor))
+            self.assertEqual(f[Flavor.NU_E].unit, 1/(u.erg * u.s))
+
+    def test_Mori_2023(self):
+        """
+        Instantiate a set of 'Mori 2023' models
+        """
+        axion_mass_coupling = [ (0,0),
+            (100,2), (100,4), (100,10), (100,12), (100,14), (100,16), (100,20),
+            (200,2), (200,4), (200,6), (200,8), (200,10), (200,20)]
+
+        pns_mass = [1.78, 1.77, 1.76, 1.77, 1.77, 1.77, 1.77, 1.74, 1.77, 1.76, 1.75, 1.74, 1.73, 1.62] * u.Msun
+
+        for ((am, ac), mpns) in zip(axion_mass_coupling, pns_mass):
+            model = Mori_2023(axion_mass=am*u.MeV, axion_coupling=ac*1e-10/u.GeV)
+
+            axion_mass = float(am) * u.MeV
+            self.assertEqual(model.metadata['Axion mass'], axion_mass)
+    
+            axion_coupling = float(ac) * 1e-10/u.GeV
+            axion_coupling = np.round(axion_coupling.to('1e-10/GeV'))
+            self.assertEqual(model.metadata['Axion coupling'], axion_coupling)
+
+            self.assertEqual(model.metadata['Progenitor mass'], 20*u.Msun)
+            self.assertEqual(model.metadata['PNS mass'], mpns)
+
+            # Check that times are in proper units.
+            t = model.get_time()
+            self.assertTrue(t.unit, u.s)
+
+            # Check that we can compute flux dictionaries.
+            f = model.get_initial_spectra(0*u.s, 10*u.MeV)
             self.assertEqual(type(f), dict)
             self.assertEqual(len(f), len(Flavor))
             self.assertEqual(f[Flavor.NU_E].unit, 1./(u.erg * u.s))
```

### Comparing `snewpy-1.4b2/python/snewpy/test/test_02_models.py` & `snewpy-1.5/python/snewpy/test/test_02_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 # -*- coding: utf-8 -*-
-"""Unit tests for the neutrino submodule.
+"""Unit tests for the models initializations.
 """
 import unittest
 
 from snewpy.neutrino import Flavor
-from snewpy.models.loaders import Nakazato_2013, Tamborra_2014, OConnor_2013, OConnor_2015, \
+from snewpy.models.ccsn_loaders import Nakazato_2013, Tamborra_2014, OConnor_2013, OConnor_2015, \
                                   Sukhbold_2015, Bollig_2016, Walk_2018, \
                                   Walk_2019, Fornax_2019, Warren_2020, \
                                   Kuroda_2020, Fornax_2021, Zha_2021
-from snewpy._model_urls import model_urls
 from astropy import units as u
 from snewpy import model_path
 import os
 
 
 class TestModels(unittest.TestCase):
 
-    def test_model_urls(self):
-        """Test that snewpy._model_urls.model_urls is empty. This should be populated if snewpy is downloaded from PyPI.
-        This serves as a guard against accidentally committing/merging a populated model_urls to main.
-        """
-        self.assertFalse(model_urls)
-
     def test_Nakazato_2013(self):
         """
         Instantiate a set of 'Nakazato 2013' models
         """
         for z in [0.004, 0.02]:
             for trev in [100, 200, 300]:
                 for mass in [13., 20., 50.]:
@@ -72,15 +65,16 @@
         """
         for mass in list(range(12, 34)) + list(range(35, 61, 5)) + [70, 80, 100, 120]:
             for eos in ['LS220', 'HShen']:
                 metadata = {
                     'Progenitor mass': mass * u.Msun,
                     'EOS': eos,
                 }
-                model = OConnor_2013(filename=f'{eos}_timeseries.tar.gz', metadata=metadata)
+                mfile = f'OConnor_2013/{eos}_timeseries.tar.gz'
+                model = OConnor_2013(filename=os.path.join(model_path,mfile), metadata=metadata)
 
                 self.assertEqual(model.metadata['EOS'], eos)
                 self.assertEqual(model.metadata['Progenitor mass'].value, mass)
 
                 # Check that times are in proper units.
                 t = model.get_time()
                 self.assertTrue(t.unit, u.s)
@@ -91,16 +85,16 @@
                 self.assertEqual(len(f), len(Flavor))
                 self.assertEqual(f[Flavor.NU_E].unit, 1/(u.erg * u.s))
 
     def test_OConnor_2015(self):
         """
         Instantiate a set of "O'Connor 2015" models
         """
-        mfile = 'M1_neutrinos.dat'
-        model = OConnor_2015(mfile)
+        mfile = 'OConnor_2015/M1_neutrinos.dat'
+        model = OConnor_2015(filename=os.path.join(model_path,mfile))
 
         # Check that times are in proper units.
         t = model.get_time()
         self.assertTrue(t.unit, u.s)
 
         # Check that we can compute flux dictionaries.
         f = model.get_initial_spectra(0*u.s, 10*u.MeV)
@@ -233,21 +227,21 @@
             '27.8', '27.9', '28.0', '28.1', '28.2', '28.3', '28.4', '28.5', '28.6',
             '28.7', '28.8', '28.9', '29.0', '29.1', '29.2', '29.3', '29.4', '29.5',
             '29.6', '29.7', '29.8', '29.9', '30.0', '31', '32', '33', '35', '40', '45',
             '50', '55', '60', '70', '80', '9.0', '9.25', '9.5', '9.75']
 
         for mixing in [1.23, 1.25, 1.27]:
             for mass in masses:
-                mfile = f'stir_a{mixing}/stir_multimessenger_a{mixing}_m{mass}.h5'
+                mfile = f'Warren_2020/stir_a{mixing}/stir_multimessenger_a{mixing}_m{mass}.h5'
                 metadata = {
                     'Progenitor mass': float(mass) * u.Msun,
                     'Turb. mixing param.': mixing,
                     'EOS': 'SFHo',
                 }
-                model = Warren_2020(mfile, metadata)
+                model = Warren_2020(os.path.join(model_path, mfile), metadata)
 
                 # Check that times are in proper units.
                 t = model.get_time()
                 self.assertTrue(t.unit, u.s)
 
                 # Check that we can compute flux dictionaries.
                 f = model.get_initial_spectra(0 * u.s, 10 * u.MeV)
```

### Comparing `snewpy-1.4b2/python/snewpy/test/test_03_neutrino.py` & `snewpy-1.5/python/snewpy/test/test_03_neutrino.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.4b2/python/snewpy/test/test_04_xforms.py` & `snewpy-1.5/python/snewpy/test/test_04_xforms.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from snewpy.flavor_transformation import MassHierarchy, MixingParameters
 from snewpy.flavor_transformation import \
     NoTransformation, CompleteExchange, \
     AdiabaticMSW, NonAdiabaticMSWH, \
     AdiabaticMSWes, NonAdiabaticMSWes, \
     TwoFlavorDecoherence, ThreeFlavorDecoherence, \
-    NeutrinoDecay
+    NeutrinoDecay, QuantumDecoherence
 
 from astropy import units as u
 from astropy import constants as c
 import numpy as np
 from numpy import sin, cos, exp, abs
 
 class TestFlavorTransformations(unittest.TestCase):
@@ -28,14 +28,20 @@
         self.theta14 =  1 * u.deg
 
         # Dummy neutrino decay parameters; see arXiv:1910.01127.
         self.mass3 = 0.5 * u.eV/c.c**2
         self.lifetime = 1 * u.day
         self.distance = 10 * u.kpc
 
+        # Quantum decoherence parameters; see arXiv:2306.17591.
+        self.gamma3 = (1e-27 * u.eV / (c.hbar * c.c)).to('1/kpc')
+        self.gamma8 = (1e-27 * u.eV / (c.hbar * c.c)).to('1/kpc')
+        self.n = 0
+        self.energy_ref = 10 * u.MeV
+
     def test_noxform(self):
         """
         Survival probabilities for no oscillations
         """
         xform = NoTransformation()
 
         self.assertEqual(xform.prob_ee(self.t, self.E), 1)
@@ -482,7 +488,131 @@
         prob_exbar = np.asarray([De1 + De2*np.exp(-xform.gamma(_E)*self.distance) +
                                  De3*(1-np.exp(-xform.gamma(_E)*self.distance)) for _E in self.E])
 
         self.assertEqual(xform.prob_eebar(self.t, self.E), De3)
         self.assertTrue(np.array_equal(xform.prob_exbar(self.t, self.E), prob_exbar))
         self.assertTrue(np.array_equal(xform.prob_xxbar(self.t, self.E), 1. - 0.5*prob_exbar))
         self.assertEqual(xform.prob_xebar(self.t, self.E), 0.5*(1. - De3))
+
+    def test_quantumdecoherence_nmo(self):
+        """
+        Quantum Decoherence with NMO and new mixing angles 
+        """
+        # Override the default mixing angles.
+        xform = QuantumDecoherence(mix_angles=(self.theta12, self.theta13, self.theta23), Gamma3=self.gamma3 * c.hbar * c.c, Gamma8=self.gamma8 * c.hbar * c.c, dist=self.distance, n=self.n, E0=self.energy_ref, mh=MassHierarchy.NORMAL)
+
+        # Test computation survival and transition probabilities of mass states.
+        _E = 10*u.MeV
+        self.assertTrue(xform.P11(_E) == 1/3 + 1/2 * np.exp(-(self.gamma3 * (_E/self.energy_ref)**self.n + self.gamma8 * (_E/self.energy_ref)**self.n / 3) * self.distance) + 1/6 * np.exp(-self.gamma8 * (_E/self.energy_ref)**self.n * self.distance))
+        self.assertTrue(xform.P21(_E) == 1/3 - 1/2 * np.exp(-(self.gamma3 * (_E/self.energy_ref)**self.n + self.gamma8 * (_E/self.energy_ref)**self.n / 3) * self.distance) + 1/6 * np.exp(-self.gamma8 * (_E/self.energy_ref)**self.n * self.distance))
+        self.assertTrue(xform.P22(_E) == 1/3 + 1/2 * np.exp(-(self.gamma3 * (_E/self.energy_ref)**self.n + self.gamma8 * (_E/self.energy_ref)**self.n / 3) * self.distance) + 1/6 * np.exp(-self.gamma8 * (_E/self.energy_ref)**self.n * self.distance))
+        self.assertTrue(xform.P31(_E) == 1/3 - 1/3 * np.exp(-self.gamma8 * (_E/self.energy_ref)**self.n * self.distance))
+        self.assertTrue(xform.P32(_E) == 1/3 - 1/3 * np.exp(-self.gamma8 * (_E/self.energy_ref)**self.n * self.distance))
+        self.assertAlmostEqual(float(xform.P33(_E)), float(1/3 + 2/3 * np.exp(-self.gamma8 * (_E/self.energy_ref)**self.n * self.distance)), places=12)
+
+        De1 = (cos(self.theta12) * cos(self.theta13))**2
+        De2 = (sin(self.theta12) * cos(self.theta13))**2
+        De3 = sin(self.theta13)**2
+
+        # Check flavor transition probabilities.
+        prob_ee = np.asarray([xform.P31(_E)*De1 + xform.P32(_E)*De2 + xform.P33(_E)*De3 for _E in self.E])
+
+        self.assertTrue(np.array_equal(xform.prob_ee(self.t, self.E), prob_ee))
+        self.assertTrue(np.array_equal(xform.prob_ex(self.t, self.E), 1 - prob_ee))
+        self.assertTrue(np.array_equal(xform.prob_xx(self.t, self.E), 1 - 0.5*(1 - prob_ee)))
+        self.assertTrue(np.array_equal(xform.prob_xe(self.t, self.E), 0.5*(1 - prob_ee)))
+
+        prob_eebar = np.asarray([xform.P11(_E)*De1 + xform.P21(_E)*De2 + xform.P31(_E)*De3 for _E in self.E])
+
+        self.assertTrue(np.array_equal(xform.prob_exbar(self.t, self.E), 1 - prob_eebar))
+        self.assertTrue(np.array_equal(xform.prob_xxbar(self.t, self.E), 1. - 0.5*(1 - prob_eebar)))
+        self.assertTrue(np.array_equal(xform.prob_xebar(self.t, self.E), 0.5*(1. - prob_eebar)))
+
+    def test_quantumdecoherence_nmo_default_mixing(self):
+        """
+        Quantum decoherence with NMO and default mixing angles
+        """
+        # Use default mixing angles defined in the submodule.
+        xform = QuantumDecoherence(Gamma3=self.gamma3 * c.hbar * c.c, Gamma8=self.gamma8 * c.hbar * c.c, dist=self.distance, n=self.n, E0=self.energy_ref)
+
+        # Check transition probabilities (normal hierarchy is default).
+        mixpars = MixingParameters()
+        th12, th13, th23 = mixpars.get_mixing_angles()
+
+        De1 = (cos(th12) * cos(th13))**2
+        De2 = (sin(th12) * cos(th13))**2
+        De3 = sin(th13)**2
+
+        prob_ee = np.asarray([xform.P31(_E)*De1 + xform.P32(_E)*De2 + xform.P33(_E)*De3 for _E in self.E])
+
+        self.assertTrue(np.array_equal(xform.prob_ee(self.t, self.E), prob_ee))
+        self.assertTrue(np.array_equal(xform.prob_ex(self.t, self.E), 1 - prob_ee))
+        self.assertTrue(np.array_equal(xform.prob_xx(self.t, self.E), 1 - 0.5*(1 - prob_ee)))
+        self.assertTrue(np.array_equal(xform.prob_xe(self.t, self.E), 0.5*(1 - prob_ee)))
+
+        prob_eebar = np.asarray([xform.P11(_E)*De1 + xform.P21(_E)*De2 + xform.P31(_E)*De3 for _E in self.E])
+
+        self.assertTrue(np.array_equal(xform.prob_exbar(self.t, self.E), 1 - prob_eebar))
+        self.assertTrue(np.array_equal(xform.prob_xxbar(self.t, self.E), 1. - 0.5*(1 - prob_eebar)))
+        self.assertTrue(np.array_equal(xform.prob_xebar(self.t, self.E), 0.5*(1. - prob_eebar)))
+
+    def test_quantumdecoherence_imo(self):
+        """
+        Quantum Decoherence with IMO and new mixing angles 
+        """
+        # Override the default mixing angles.
+        xform = QuantumDecoherence(mix_angles=(self.theta12, self.theta13, self.theta23), Gamma3=self.gamma3 * c.hbar * c.c, Gamma8=self.gamma8 * c.hbar * c.c, dist=self.distance, n=self.n, E0=self.energy_ref, mh=MassHierarchy.INVERTED)
+
+        # Test computation survival and transition probabilities of mass states.
+        _E = 10*u.MeV
+        self.assertTrue(xform.P11(_E) == 1/3 + 1/2 * np.exp(-(self.gamma3 * (_E/self.energy_ref)**self.n + self.gamma8 * (_E/self.energy_ref)**self.n / 3) * self.distance) + 1/6 * np.exp(-self.gamma8 * (_E/self.energy_ref)**self.n * self.distance))
+        self.assertTrue(xform.P21(_E) == 1/3 - 1/2 * np.exp(-(self.gamma3 * (_E/self.energy_ref)**self.n + self.gamma8 * (_E/self.energy_ref)**self.n / 3) * self.distance) + 1/6 * np.exp(-self.gamma8 * (_E/self.energy_ref)**self.n * self.distance))
+        self.assertTrue(xform.P22(_E) == 1/3 + 1/2 * np.exp(-(self.gamma3 * (_E/self.energy_ref)**self.n + self.gamma8 * (_E/self.energy_ref)**self.n / 3) * self.distance) + 1/6 * np.exp(-self.gamma8 * (_E/self.energy_ref)**self.n * self.distance))
+        self.assertTrue(xform.P31(_E) == 1/3 - 1/3 * np.exp(-self.gamma8 * (_E/self.energy_ref)**self.n * self.distance))
+        self.assertTrue(xform.P32(_E) == 1/3 - 1/3 * np.exp(-self.gamma8 * (_E/self.energy_ref)**self.n * self.distance))
+        self.assertAlmostEqual(float(xform.P33(_E)), float(1/3 + 2/3 * np.exp(-self.gamma8 * (_E/self.energy_ref)**self.n * self.distance)), places=12)
+
+        De1 = (cos(self.theta12) * cos(self.theta13))**2
+        De2 = (sin(self.theta12) * cos(self.theta13))**2
+        De3 = sin(self.theta13)**2
+
+        # Check transition probabilities.
+        prob_ee = np.asarray([xform.P22(_E)*De2 + xform.P21(_E)*De1 + xform.P32(_E)*De3 for _E in self.E])
+
+        self.assertTrue(np.array_equal(xform.prob_ee(self.t, self.E), prob_ee))
+        self.assertTrue(np.array_equal(xform.prob_ex(self.t, self.E), 1 - prob_ee))
+        self.assertTrue(np.array_equal(xform.prob_xx(self.t, self.E), 1 - 0.5*(1 - prob_ee)))
+        self.assertTrue(np.array_equal(xform.prob_xe(self.t, self.E), 0.5*(1 - prob_ee)))
+
+        prob_eebar = np.asarray([xform.P31(_E)*De1 + xform.P32(_E)*De2 + xform.P33(_E)*De3 for _E in self.E])
+
+        self.assertTrue(np.array_equal(xform.prob_exbar(self.t, self.E), 1 - prob_eebar))
+        self.assertTrue(np.array_equal(xform.prob_xxbar(self.t, self.E), 1. - 0.5*(1 - prob_eebar)))
+        self.assertTrue(np.array_equal(xform.prob_xebar(self.t, self.E), 0.5*(1. - prob_eebar)))
+
+    def test_quantumdecoherence_imo_default_mixing(self):
+        """
+        Quantum decoherence with IMO and default mixing angles
+        """
+        # Use default mixing angles defined in the submodule.
+        xform = QuantumDecoherence(Gamma3=self.gamma3 * c.hbar * c.c, Gamma8=self.gamma8 * c.hbar * c.c, dist=self.distance, n=self.n, E0=self.energy_ref, mh=MassHierarchy.INVERTED)
+
+        # Check transition probabilities.
+        mixpars = MixingParameters(MassHierarchy.INVERTED)
+        th12, th13, th23 = mixpars.get_mixing_angles()
+
+        De1 = (cos(th12) * cos(th13))**2
+        De2 = (sin(th12) * cos(th13))**2
+        De3 = sin(th13)**2
+
+        prob_ee = np.asarray([xform.P22(_E)*De2 + xform.P21(_E)*De1 + xform.P32(_E)*De3 for _E in self.E])
+
+        self.assertTrue(np.array_equal(xform.prob_ee(self.t, self.E), prob_ee))
+        self.assertTrue(np.array_equal(xform.prob_ex(self.t, self.E), 1 - prob_ee))
+        self.assertTrue(np.array_equal(xform.prob_xx(self.t, self.E), 1 - 0.5*(1 - prob_ee)))
+        self.assertTrue(np.array_equal(xform.prob_xe(self.t, self.E), 0.5*(1 - prob_ee)))
+
+        prob_eebar = np.asarray([xform.P31(_E)*De1 + xform.P32(_E)*De2 + xform.P33(_E)*De3 for _E in self.E])
+
+        self.assertTrue(np.array_equal(xform.prob_exbar(self.t, self.E), 1 - prob_eebar))
+        self.assertTrue(np.array_equal(xform.prob_xxbar(self.t, self.E), 1. - 0.5*(1 - prob_eebar)))
+        self.assertTrue(np.array_equal(xform.prob_xebar(self.t, self.E), 0.5*(1. - prob_eebar)))
```

### Comparing `snewpy-1.4b2/python/snewpy/test/test_05_snowglobes.py` & `snewpy-1.5/python/snewpy/test/test_05_snowglobes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 import pytest
 from pathlib import Path
 from snewpy.test._rate_crosscheck_table import rate_table
-from snewpy import snowglobes
+from snewpy import snowglobes, model_path
+
+from snewpy.models import ccsn
+import astropy.units as u
 
 pytestmark=pytest.mark.snowglobes
 
 #get available model parameters from table
 param_values = list(rate_table.keys())
 #get available detectors from table
 detectors = list(list(rate_table.values())[0].keys())
 
+#make sure the model files are loaded
+model = ccsn.Bollig_2016
+for params in model.get_param_combinations():
+    model(**params)
+    
 def fluence_calculation(model_name,model_file,transform):
     #generating fluence file
-    model_path = f'models/{model_name}/{model_file}'
-    return snowglobes.generate_fluence(model_path,model_name,transform,d=10)
+    model_file_path = f'{model_path}/{model_name}/{model_file}'
+    print(model_file_path)
+    return snowglobes.generate_fluence(model_file_path, model_name, transform,d=10)
 
 def rates_calculation(fluence_file):
     tables = snowglobes.simulate(None,fluence_file,detector_input=detectors)
     result = {}
     for det,table in tables.items():
         table = list(table.values())[0] #take the first and the only time bin
         result[det] = table['weighted']['smeared'].values.sum()
```

### Comparing `snewpy-1.4b2/python/snewpy/test/test_flux_container.py` & `snewpy-1.5/python/snewpy/test/test_flux_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 @st.composite
 def quantities(draw, values, unit):
     return draw(values)<<unit
 
 #how to generate axes values
 flavors = st.lists(elements=st.sampled_from(Flavor),
                    unique=True,min_size=1,max_size=len(Flavor)).map(sorted)
-units = st.sampled_from(['1/MeV','1/(MeV*s)','1/(MeV*s*cm**2)']).map(u.Unit)
+units = st.sampled_from(['1/MeV','1/(MeV*s)','1/(MeV*s*m**2)']).map(u.Unit)
 energies = quantities(sorted_floats(shape=array_shapes(max_dims=1)),u.MeV)
 times    = quantities(sorted_floats(shape=array_shapes(max_dims=1)),u.s)
 integrable_axess = st.lists(st.sampled_from(list(Axes)[1:]))
 
 @st.composite
 def random_flux_containers(draw, times=times, energies=energies, units=units, axes=st.just(None)):
     "Strategy to generate a random flux container"
@@ -55,21 +55,27 @@
 #--------------------------------------------------------------
 @given(flavor=flavors, time=times, energy=energies, unit=units)
 def test_construction_succesfull(flavor, energy, time, unit):
     data = np.ones([len(flavor),len(time), len(energy)])<<unit
     assert Container[unit](data, flavor, time, energy)
 
 @given(flavor=flavors, time=times, energy=energies, unit=units)
-def test_construction_with_wrong_units_raises_ValueError(flavor, energy, time, unit):
+def test_construction_with_wrong_units_raises_ConversionError(flavor, energy, time, unit):
     data = np.ones([len(flavor),len(time), len(energy)])<<unit
     with pytest.raises(u.UnitConversionError):
         Container[unit*u.kg](data, flavor, time, energy)
     with pytest.raises(u.UnitConversionError):
         Container[unit](data*u.kg, flavor, time, energy)
 
+@given(flavor=flavors, time=times, energy=energies, unit=units)
+def test_construction_with_wrong_dimensions_raises_ValueError(flavor, energy, time, unit):
+    data = np.ones([len(flavor)+1,len(time), len(energy)])<<unit
+    with pytest.raises(ValueError):
+        Container[unit](data, flavor, time, energy)
+
 @given(f=random_flux_containers())
 def test_summation_over_flavor(f:Container):
     fS = f.sum('flavor')
     #check the result array shapes
     assert fS.shape[Axes.flavor] == 1
     assert fS.shape[Axes.energy] == f.shape[Axes.energy]
     assert fS.shape[Axes.time]   == f.shape[Axes.time]
```

### Comparing `snewpy-1.4b2/python/snewpy/test/test_rate_calculation.py` & `snewpy-1.5/python/snewpy/test/test_rate_calculation.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.4b2/python/snewpy/to_snowglobes.py` & `snewpy-1.5/python/snewpy/to_snowglobes.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.4b2/setup.py` & `snewpy-1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python
 #
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import os
-from distutils.command.sdist import sdist as DistutilsSdist
 from setuptools import setup, find_packages
 
 # Git-based version info. Remove?
 from python.snewpy._git import get_version, SetVersion
 
 #
 # Begin setup
@@ -37,15 +36,15 @@
 # setup_keywords['entry_points'] = {'console_scripts': ['to_snowglobes = snewpy.to_snowglobes:generate_time_series', ], },
 setup_keywords['provides'] = [setup_keywords['name']]
 setup_keywords['python_requires'] = '>=3.8'
 setup_keywords['zip_safe'] = False
 setup_keywords['packages'] = find_packages('python')
 setup_keywords['package_dir'] = {'': 'python'}
 setup_keywords['package_data'] = {'':['templates/*.glb', 'models/*.yml']}
-setup_keywords['cmdclass'] = {'version': SetVersion, 'sdist': DistutilsSdist}
+setup_keywords['cmdclass'] = {'version': SetVersion}
 setup_keywords['test_suite']='snewpy.test.snewpy_test_suite.snewpy_test_suite'
 
 requires = []
 with open('requirements.txt', 'r') as f:
     for line in f:
         if line.strip():
             requires.append(line.strip())
```


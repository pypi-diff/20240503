# Comparing `tmp/unico_device_setuper-0.1.0.tar.gz` & `tmp/unico_device_setuper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unico_device_setuper-0.1.0.tar", max compression
+gzip compressed data, was "unico_device_setuper-0.2.0.tar", max compression
```

## Comparing `unico_device_setuper-0.1.0.tar` & `unico_device_setuper-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0        0 2024-05-02 14:31:28.799663 unico_device_setuper-0.1.0/README.md
--rw-r--r--   0        0        0     4882 2024-05-03 12:27:45.001045 unico_device_setuper-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-03 09:31:25.439950 unico_device_setuper-0.1.0/unico_device_setuper/__init__.py
--rw-r--r--   0        0        0     1430 2024-05-03 12:24:29.940281 unico_device_setuper-0.1.0/unico_device_setuper/adb.py
--rw-r--r--   0        0        0     1039 2024-05-03 12:24:29.938691 unico_device_setuper-0.1.0/unico_device_setuper/cfg.py
--rw-r--r--   0        0        0      424 2024-05-03 10:30:41.798455 unico_device_setuper-0.1.0/unico_device_setuper/cfg.toml
--rw-r--r--   0        0        0      936 2024-05-03 12:27:26.036325 unico_device_setuper-0.1.0/unico_device_setuper/datadir.py
--rw-r--r--   0        0        0      656 2024-05-03 12:24:57.286523 unico_device_setuper-0.1.0/unico_device_setuper/entrypoint.py
--rw-r--r--   0        0        0     2684 2024-05-03 10:28:42.842664 unico_device_setuper-0.1.0/unico_device_setuper/helpers.py
--rw-r--r--   0        0        0      899 2024-05-03 12:24:29.917284 unico_device_setuper-0.1.0/unico_device_setuper/local_db.py
--rw-r--r--   0        0        0      421 2024-05-03 12:25:53.506416 unico_device_setuper-0.1.0/unico_device_setuper/main.py
--rw-r--r--   0        0        0      607 1970-01-01 00:00:00.000000 unico_device_setuper-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-03 13:54:31.062047 unico_device_setuper-0.2.0/README.md
+-rw-r--r--   0        0        0     4948 2024-05-03 13:54:31.010047 unico_device_setuper-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-03 13:54:31.010047 unico_device_setuper-0.2.0/unico_device_setuper/__init__.py
+-rw-r--r--   0        0        0     1429 2024-05-03 13:36:58.809570 unico_device_setuper-0.2.0/unico_device_setuper/adb.py
+-rw-r--r--   0        0        0     1039 2024-05-03 13:36:58.809570 unico_device_setuper-0.2.0/unico_device_setuper/cfg.py
+-rw-r--r--   0        0        0      424 2024-05-03 13:36:58.809570 unico_device_setuper-0.2.0/unico_device_setuper/cfg.toml
+-rw-r--r--   0        0        0      936 2024-05-03 13:36:58.809570 unico_device_setuper-0.2.0/unico_device_setuper/datadir.py
+-rw-r--r--   0        0        0     1069 2024-05-03 13:36:58.809570 unico_device_setuper-0.2.0/unico_device_setuper/dl.py
+-rw-r--r--   0        0        0      656 2024-05-03 13:36:58.809570 unico_device_setuper-0.2.0/unico_device_setuper/entrypoint.py
+-rw-r--r--   0        0        0     1613 2024-05-03 13:36:58.809570 unico_device_setuper-0.2.0/unico_device_setuper/helpers.py
+-rw-r--r--   0        0        0      899 2024-05-03 13:36:58.809570 unico_device_setuper-0.2.0/unico_device_setuper/local_db.py
+-rw-r--r--   0        0        0      421 2024-05-03 13:36:58.809570 unico_device_setuper-0.2.0/unico_device_setuper/main.py
+-rw-r--r--   0        0        0      607 1970-01-01 00:00:00.000000 unico_device_setuper-0.2.0/PKG-INFO
```

### Comparing `unico_device_setuper-0.1.0/pyproject.toml` & `unico_device_setuper-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [tool.poetry]
 name = "unico_device_setuper"
-version = "0.1.0"
+version = '0.2.0'
 description = ""
 authors = ["Florian Daude <floriandaude@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "3.12"
+python = ">=3.12,<3.13"
 httpx = "^0.27.0"
 typer = "^0.12.3"
 slcfg = "^0.2"
 pydantic = "^2.7.1"
 tqdm = "^4.66.4"
 platformdirs = "^4.2.1"
 
 
 [tool.poetry.group.dev.dependencies]
 poetry = "^1.8.2"
+ruff = "^0.4.2"
+pyright = "^1.1.361"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry.scripts]
@@ -127,7 +129,8 @@
     "TCH003",  # move import into type checking block (it is error prone and module must be imported by someone else)
 ]
 
 
 [tool.ruff.lint.per-file-ignores]
 "unico_device_setuper/main.py" = ["T201"]
 "unico_device_setuper/entrypoint.py" = ["T201"]
+"tools/*" = ["T201"]
```

### Comparing `unico_device_setuper-0.1.0/unico_device_setuper/adb.py` & `unico_device_setuper-0.2.0/unico_device_setuper/adb.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import dataclasses
 import pathlib
 import stat
 import zipfile
 
 import httpx
 
-from unico_device_setuper import cfg, datadir, helpers
+from unico_device_setuper import cfg, datadir, dl, helpers
 
 
 async def get_exe_path(config: cfg.Config):
     data_dir = datadir.get()
     archive_path = data_dir / 'adb.zip'
     if not archive_path.exists():
         async with httpx.AsyncClient() as http_client:
-            await helpers.download_url(config.adb.download_urls.mac_os, archive_path, http_client)
+            await dl.download_url(config.adb.download_urls.mac_os, archive_path, http_client)
     adb_dir = data_dir / 'adb'
     if not adb_dir.exists():
         with zipfile.ZipFile(archive_path, 'r') as zip_ref:
             zip_ref.extractall(adb_dir)
     adb_exe = adb_dir / 'platform-tools' / 'adb'
     adb_exe.chmod(adb_exe.stat().st_mode | stat.S_IXUSR)
     return adb_exe
```

### Comparing `unico_device_setuper-0.1.0/unico_device_setuper/cfg.py` & `unico_device_setuper-0.2.0/unico_device_setuper/cfg.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.1.0/unico_device_setuper/datadir.py` & `unico_device_setuper-0.2.0/unico_device_setuper/datadir.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.1.0/unico_device_setuper/entrypoint.py` & `unico_device_setuper-0.2.0/unico_device_setuper/entrypoint.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.1.0/unico_device_setuper/local_db.py` & `unico_device_setuper-0.2.0/unico_device_setuper/local_db.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.1.0/PKG-INFO` & `unico_device_setuper-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unico_device_setuper
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: Florian Daude
 Author-email: floriandaude@hotmail.fr
 Requires-Python: >=3.12,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


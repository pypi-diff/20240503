# Comparing `tmp/shellfish-0.5.0.tar.gz` & `tmp/shellfish-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellfish-0.5.0.tar", max compression
+gzip compressed data, was "shellfish-0.5.1.tar", max compression
```

## Comparing `shellfish-0.5.0.tar` & `shellfish-0.5.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1029 2024-02-22 14:17:28.891830 shellfish-0.5.0/README.md
--rw-r--r--   0        0        0     2322 2024-05-01 17:31:22.272070 shellfish-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      331 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/__about__.py
--rw-r--r--   0        0        0     7545 2024-05-01 17:20:40.492154 shellfish-0.5.0/shellfish/__init__.py
--rw-r--r--   0        0        0      520 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/__main__.py
--rw-r--r--   0        0        0      395 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/_meta.py
--rw-r--r--   0        0        0      866 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/_types.py
--rw-r--r--   0        0        0     3279 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/aios/__init__.py
--rw-r--r--   0        0        0      640 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/aios/_path.py
--rw-r--r--   0        0        0      539 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/aioshutil.py
--rw-r--r--   0        0        0     7252 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/batman.py
--rw-r--r--   0        0        0      296 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/const.py
--rw-r--r--   0        0        0       49 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/dev/__init__.py
--rw-r--r--   0        0        0     1467 2024-04-29 21:13:24.986924 shellfish-0.5.0/shellfish/dev/do.py
--rw-r--r--   0        0        0     3390 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/dev/popen_gen.py
--rw-r--r--   0        0        0     8131 2024-04-29 21:13:24.986924 shellfish-0.5.0/shellfish/dev/run_async.py
--rw-r--r--   0        0        0     4266 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/dotenv.py
--rw-r--r--   0        0        0      681 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/echo.py
--rw-r--r--   0        0        0     8126 2024-04-29 21:13:24.986924 shellfish-0.5.0/shellfish/exe.py
--rw-r--r--   0        0        0    54237 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/fs/__init__.py
--rw-r--r--   0        0        0    15170 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/fs/_async.py
--rw-r--r--   0        0        0     1535 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/fs/promises.py
--rw-r--r--   0        0        0     1963 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/libhash.py
--rw-r--r--   0        0        0       50 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/libsh/__init__.py
--rw-r--r--   0        0        0     3656 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/libsh/_dirtree.py
--rw-r--r--   0        0        0     1872 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/libsh/args.py
--rw-r--r--   0        0        0    10604 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/osfs.py
--rw-r--r--   0        0        0     7752 2024-05-01 17:19:37.612163 shellfish-0.5.0/shellfish/process.py
--rw-r--r--   0        0        0      344 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/psu.py
--rw-r--r--   0        0        0        0 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/py.typed
--rw-r--r--   0        0        0    63836 2024-05-01 17:19:37.612163 shellfish-0.5.0/shellfish/sh.py
--rw-r--r--   0        0        0     8275 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/sp.py
--rw-r--r--   0        0        0      229 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/stdio.py
--rw-r--r--   0        0        0     2617 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/testing.py
--rw-r--r--   0        0        0       27 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/tests/__init__.py
--rw-r--r--   0        0        0     3369 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/tests/test_fs.py
--rw-r--r--   0        0        0     2216 1970-01-01 00:00:00.000000 shellfish-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1029 2024-02-22 14:17:28.891830 shellfish-0.5.1/README.md
+-rw-r--r--   0        0        0     2308 2024-05-03 20:35:40.609698 shellfish-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      331 2024-05-03 20:35:40.609698 shellfish-0.5.1/shellfish/__about__.py
+-rw-r--r--   0        0        0     8166 2024-05-03 20:35:40.609698 shellfish-0.5.1/shellfish/__init__.py
+-rw-r--r--   0        0        0      520 2024-05-03 17:50:22.153908 shellfish-0.5.1/shellfish/__main__.py
+-rw-r--r--   0        0        0      395 2024-03-21 23:48:47.639525 shellfish-0.5.1/shellfish/_meta.py
+-rw-r--r--   0        0        0      866 2024-02-22 14:17:28.891830 shellfish-0.5.1/shellfish/_types.py
+-rw-r--r--   0        0        0     3315 2024-05-03 20:35:40.609698 shellfish-0.5.1/shellfish/aios/__init__.py
+-rw-r--r--   0        0        0      640 2024-02-22 14:17:28.891830 shellfish-0.5.1/shellfish/aios/_path.py
+-rw-r--r--   0        0        0      539 2024-03-21 23:48:47.639525 shellfish-0.5.1/shellfish/aioshutil.py
+-rw-r--r--   0        0        0     7252 2024-05-03 20:35:30.719702 shellfish-0.5.1/shellfish/batman.py
+-rw-r--r--   0        0        0      296 2024-05-03 20:35:30.719702 shellfish-0.5.1/shellfish/const.py
+-rw-r--r--   0        0        0       49 2024-02-22 14:17:28.891830 shellfish-0.5.1/shellfish/dev/__init__.py
+-rw-r--r--   0        0        0     1467 2024-05-03 20:35:30.719702 shellfish-0.5.1/shellfish/dev/do.py
+-rw-r--r--   0        0        0     3390 2024-05-03 20:35:30.719702 shellfish-0.5.1/shellfish/dev/popen_gen.py
+-rw-r--r--   0        0        0     8131 2024-05-03 20:35:30.719702 shellfish-0.5.1/shellfish/dev/run_async.py
+-rw-r--r--   0        0        0     4279 2024-05-03 20:35:40.609698 shellfish-0.5.1/shellfish/dotenv.py
+-rw-r--r--   0        0        0      681 2024-03-21 23:48:47.639525 shellfish-0.5.1/shellfish/echo.py
+-rw-r--r--   0        0        0     8126 2024-05-03 20:35:30.719702 shellfish-0.5.1/shellfish/exe.py
+-rw-r--r--   0        0        0    54277 2024-05-03 20:35:40.609698 shellfish-0.5.1/shellfish/fs/__init__.py
+-rw-r--r--   0        0        0    16147 2024-05-03 20:35:40.609698 shellfish-0.5.1/shellfish/fs/_async.py
+-rw-r--r--   0        0        0     1535 2024-03-21 23:48:47.639525 shellfish-0.5.1/shellfish/fs/promises.py
+-rw-r--r--   0        0        0     1963 2024-02-22 14:17:28.891830 shellfish-0.5.1/shellfish/libhash.py
+-rw-r--r--   0        0        0       50 2024-02-22 14:17:28.891830 shellfish-0.5.1/shellfish/libsh/__init__.py
+-rw-r--r--   0        0        0     3656 2024-05-03 17:50:22.183908 shellfish-0.5.1/shellfish/libsh/_dirtree.py
+-rw-r--r--   0        0        0     1872 2024-05-03 20:35:30.719702 shellfish-0.5.1/shellfish/libsh/args.py
+-rw-r--r--   0        0        0    10604 2024-05-03 20:35:30.719702 shellfish-0.5.1/shellfish/osfs.py
+-rw-r--r--   0        0        0     7824 2024-05-03 20:35:40.609698 shellfish-0.5.1/shellfish/process.py
+-rw-r--r--   0        0        0      344 2024-02-22 14:17:28.891830 shellfish-0.5.1/shellfish/psu.py
+-rw-r--r--   0        0        0        0 2024-02-22 14:17:28.891830 shellfish-0.5.1/shellfish/py.typed
+-rw-r--r--   0        0        0    64211 2024-05-03 20:35:40.609698 shellfish-0.5.1/shellfish/sh.py
+-rw-r--r--   0        0        0     8275 2024-05-03 20:35:30.719702 shellfish-0.5.1/shellfish/sp.py
+-rw-r--r--   0        0        0      229 2024-03-21 23:48:47.639525 shellfish-0.5.1/shellfish/stdio.py
+-rw-r--r--   0        0        0     2617 2024-05-03 20:35:30.719702 shellfish-0.5.1/shellfish/testing.py
+-rw-r--r--   0        0        0       27 2024-02-22 14:17:28.891830 shellfish-0.5.1/shellfish/tests/__init__.py
+-rw-r--r--   0        0        0     3369 2024-05-03 17:50:22.203908 shellfish-0.5.1/shellfish/tests/test_fs.py
+-rw-r--r--   0        0        0     2216 1970-01-01 00:00:00.000000 shellfish-0.5.1/PKG-INFO
```

### Comparing `shellfish-0.5.0/README.md` & `shellfish-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `shellfish-0.5.0/pyproject.toml` & `shellfish-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shellfish"
-version = "0.5.0"
+version = "0.5.1"
 description = "shellfish ~ shell & file-system utils"
 license = "MIT"
 authors = ["jesse <jesse@dgi.com>"]
 repository = "https://github.com/dynamic-graphics-inc/dgpy-libs"
 homepage = "https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/shellfish"
 readme = 'README.md'
 packages = [
@@ -73,15 +73,14 @@
   "timeout",
   "aio",
   "asyncio",
 ]
 
 [tool.coverage.run]
 source = ['shellfish']
-branch = true
 context = '${CONTEXT}'
 omit = ["**/__main__.py"]
 
 [tool.coverage.report]
 precision = 2
 show_missing = true
 exclude_lines = [
```

### Comparing `shellfish-0.5.0/shellfish/__init__.py` & `shellfish-0.5.1/shellfish/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -129,52 +129,74 @@
     wstr as wstr,
     wstr_async as wstr_async,
     wstring as wstring,
     wstring_async as wstring_async,
 )
 from shellfish.process import env as env
 from shellfish.sh import (
+    LIN as LIN,
+    WIN as WIN,
     Done as Done,
     DoneDict as DoneDict,
+    DoneError as DoneError,
+    DoneObj as DoneObj,
+    Flag as Flag,
+    FlagMeta as FlagMeta,
+    HrTime as HrTime,
+    TimeoutExpired as TimeoutExpired,
     basename as basename,
     cd as cd,
+    decode_stdio_bytes as decode_stdio_bytes,
     dirname as dirname,
     do as do,
+    do_ as do_,
     do_async as do_async,
+    doa as doa,
     export as export,
     flatten_args as flatten_args,
+    link_dir as link_dir,
+    link_dirs as link_dirs,
+    link_file as link_file,
+    link_files as link_files,
     ls as ls,
     ls_dirs as ls_dirs,
     ls_files as ls_files,
     ls_files_dirs as ls_files_dirs,
     mkenv as mkenv,
     mv as mv,
     pwd as pwd,
     q as q,
     quote as quote,
     rm as rm,
+    run as run,
     seconds2hrtime as seconds2hrtime,
     setenv as setenv,
     shell as shell,
     shplit as shplit,
+    shx as shx,
     source as source,
+    sync as sync,
     tree as tree,
+    unlink_dir as unlink_dir,
+    unlink_dirs as unlink_dirs,
+    unlink_file as unlink_file,
+    unlink_files as unlink_files,
     utf8_string as utf8_string,
     where as where,
     which as which,
     which_lru as which_lru,
+    x as x,
 )
 from shellfish.stdio import Stdio as Stdio
 
 _funkify(sh.do, key="shellfish.sh")
 _funkify(sh.do, key="shellfish")
 
 ps = process
 
-
 __all__ = (
     "LIN",
     "WIN",
     "Done",
     "DoneDict",
     "DoneError",
     "DoneObj",
@@ -261,14 +283,15 @@
     "lstat_async",
     "lstr",
     "lstr_async",
     "lstring",
     "lstring_async",
     "mkdir",
     "mkdirp",
+    "mkenv",
     "move",
     "mv",
     "path_gen",
     "process",
     "ps",
     "pwd",
     "q",
@@ -299,14 +322,15 @@
     "sbytes",
     "sbytes_async",
     "sbytes_gen",
     "sbytes_gen_async",
     "scandir",
     "scandir_gen",
     "scandir_list",
+    "seconds2hrtime",
     "sep_join",
     "sep_lstrip",
     "sep_rstrip",
     "sep_split",
     "sep_strip",
     "setenv",
     "sh",
@@ -327,14 +351,15 @@
     "sync",
     "touch",
     "tree",
     "unlink_dir",
     "unlink_dirs",
     "unlink_file",
     "unlink_files",
+    "utf8_string",
     "walk_gen",
     "wbin",
     "wbin_async",
     "wbin_gen",
     "wbin_gen_async",
     "wbytes",
     "wbytes_async",
```

### Comparing `shellfish-0.5.0/shellfish/__main__.py` & `shellfish-0.5.1/shellfish/__main__.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.5.0/shellfish/_types.py` & `shellfish-0.5.1/shellfish/_types.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.5.0/shellfish/aios/__init__.py` & `shellfish-0.5.1/shellfish/aios/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 
 from typing import AnyStr, AsyncIterator, Generic
 
 from asyncify import asyncify
 from shellfish.aios import _path
 
 __all__ = (
+    "DirEntryAsync",
     "chmod",
     "listdir",
     "lstat",
     "makedirs",
     "mkdir",
     "path",
     "readlink",
     "remove",
     "removedirs",
     "rename",
     "renames",
     "replace",
     "rmdir",
+    "scandir",
     "stat",
     "truncate",
 )
 
 path = _path
 
 chmod = asyncify(os.chmod)
```

### Comparing `shellfish-0.5.0/shellfish/aios/_path.py` & `shellfish-0.5.1/shellfish/aios/_path.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.5.0/shellfish/aioshutil.py` & `shellfish-0.5.1/shellfish/aioshutil.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.5.0/shellfish/batman.py` & `shellfish-0.5.1/shellfish/batman.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.5.0/shellfish/dev/do.py` & `shellfish-0.5.1/shellfish/dev/do.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.5.0/shellfish/dev/popen_gen.py` & `shellfish-0.5.1/shellfish/dev/popen_gen.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.5.0/shellfish/dev/run_async.py` & `shellfish-0.5.1/shellfish/dev/run_async.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.5.0/shellfish/dotenv.py` & `shellfish-0.5.1/shellfish/dotenv.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from __future__ import annotations
 
 import re
 
 from os import getcwd, path
 from shlex import split as shplit
 
-from shellfish.fs import rstring
+from shellfish.fs import rstring as _rstring
 from xtyping import Dict, FsPath, Optional
 
 __all__ = ("ldotenv", "parse_dotenv", "parse_env", "strip_comments")
 
 
 def strip_comments(string: str) -> str:
     """Remove comments from python/shell scripts given the script as a string
@@ -120,15 +120,15 @@
         Traceback (most recent call last):
         ...
         ValueError: Given fspath/dirpath does not exist: path/does/not/exist
 
     """
     if fspath:
         if path.isfile(str(fspath)):
-            dotenv_string = rstring(fspath)
+            dotenv_string = _rstring(fspath)
             return parse_dotenv(dotenv_string)
         if path.isdir(str(fspath)):
             dotenv_filepath = path.join(str(fspath), ".env")
             if path.exists(dotenv_filepath):
                 return ldotenv(dotenv_filepath)
         raise ValueError(f"Given fspath/dirpath does not exist: {str(fspath)}")
     return ldotenv(getcwd())
```

### Comparing `shellfish-0.5.0/shellfish/echo.py` & `shellfish-0.5.1/shellfish/echo.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.5.0/shellfish/exe.py` & `shellfish-0.5.1/shellfish/exe.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.5.0/shellfish/fs/__init__.py` & `shellfish-0.5.1/shellfish/fs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     wbin_gen_async as wbin_gen_async,
     wbytes_async as wbytes_async,
     wbytes_gen_async as wbytes_gen_async,
     wjson_async as wjson_async,
     wstr_async as wstr_async,
     wstring_async as wstring_async,
 )
-from shellfish.process import is_win as is_win
+from shellfish.process import is_win as _is_win
 from shellfish.stdio import Stdio as Stdio
 from xtyping import (
     Any,
     AnyStr,
     Callable,
     Generator,
     Iterable,
@@ -1593,15 +1593,15 @@
         os.stat_result: stat_result object
 
     """
     return _stat(_fspath(fspath))
 
 
 def symlink(link: FsPath, target: FsPath, *, _type: SymlinkType = "file") -> None:
-    if is_win():
+    if _is_win():
         raise NotImplementedError("TODO")
     _symlink(str(link), str(target))
 
 
 def copy_file(
     src: FsPath, dest: FsPath, *, dryrun: bool = False, mkdirp: bool = False
 ) -> Tuple[str, str]:
@@ -1701,14 +1701,15 @@
     "filepath_gen",
     "filepath_mtimedelta_sec",
     "files_dirs_gen",
     "files_gen",
     "filesize",
     "filesize_async",
     "fspath",
+    "glob",
     "is_dir",
     "is_dir_async",
     "is_file",
     "is_file_async",
     "is_link",
     "is_link_async",
     "isdir",
@@ -1760,14 +1761,15 @@
     "sbin_async",
     "sbytes",
     "sbytes_async",
     "sbytes_gen",
     "sbytes_gen_async",
     "scandir",
     "scandir_gen",
+    "scandir_gen_filter",
     "scandir_list",
     "sep_join",
     "sep_lstrip",
     "sep_rstrip",
     "sep_split",
     "sep_strip",
     "shebang",
```

### Comparing `shellfish-0.5.0/shellfish/fs/_async.py` & `shellfish-0.5.1/shellfish/fs/_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,28 +10,33 @@
 
 from aiopen import aiopen
 from jsonbourne import JSON
 from shellfish import aios
 from xtyping import AsyncIterator, FsPath, Iterable, Union
 
 __all__ = (
+    "dir_exists_async",
     "exists_async",
+    "file_exists_async",
+    "filesize_async",
     "is_dir_async",
     "is_file_async",
     "is_link_async",
     "isdir_async",
     "isfile_async",
     "islink_async",
     "lbytes_async",
     "lbytes_gen_async",
     "listdir_async",
     "ljson_async",
     "lstat_async",
     "lstr_async",
     "lstring_async",
+    "mkdir_async",
+    "mkdirp_async",
     "rbin_async",
     "rbin_gen_async",
     "rbytes_async",
     "rbytes_gen_async",
     "rjson_async",
     "rstr_async",
     "rstring_async",
@@ -126,14 +131,40 @@
 
 
 async def listdir_async(fspath: FsPath) -> List[str]:
     """Async version of `os.listdir`"""
     return await aios.listdir(_fspath(fspath))
 
 
+async def mkdir_async(
+    fspath: FsPath, *, parents: bool = False, p: bool = False, exist_ok: bool = False
+) -> None:
+    """Make directory at given fspath (async)
+
+    Args:
+        fspath (FsPath): Directory path to create
+        parents (bool): Make parent dirs if True; do not make parent dirs if False
+        p (bool): Make parent dirs if True; do not make parent dirs if False (alias of parents)
+        exist_ok (bool): Throw error if directory exists and exist_ok is False
+
+    Returns:
+         None
+
+    """
+    _parents = parents or p
+    if _parents or exist_ok:
+        return await aios.makedirs(_fspath(fspath), exist_ok=_parents or exist_ok)
+    return await aios.mkdir(_fspath(fspath))
+
+
+async def mkdirp_async(fspath: FsPath) -> None:
+    """Make directory and parents (async)"""
+    return await aios.makedirs(_fspath(fspath), exist_ok=True)
+
+
 # IO # IO # IO # IO # IO # IO # IO # IO # IO # IO # IO # IO # IO # IO # IO #
 async def wbytes_async(
     filepath: FsPath,
     bites: bytes,
     *,
     append: bool = False,
     chmod: Optional[int] = None,
```

### Comparing `shellfish-0.5.0/shellfish/fs/promises.py` & `shellfish-0.5.1/shellfish/fs/promises.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.5.0/shellfish/libhash.py` & `shellfish-0.5.1/shellfish/libhash.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.5.0/shellfish/libsh/_dirtree.py` & `shellfish-0.5.1/shellfish/libsh/_dirtree.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.5.0/shellfish/libsh/args.py` & `shellfish-0.5.1/shellfish/libsh/args.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.5.0/shellfish/osfs.py` & `shellfish-0.5.1/shellfish/osfs.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.5.0/shellfish/process.py` & `shellfish-0.5.1/shellfish/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,25 +31,29 @@
 __all__ = (
     "ENV",
     "PYTHON_IMPLEMENTATION",
     "SYS_PATH_SEP",
     "Env",
     "env",
     "env_dict",
+    "hostname",
     "is_cpython",
     "is_mac",
     "is_notebook",
     "is_pypy",
     "is_win",
     "is_wsl",
     "ismac",
     "iswin",
     "iswsl",
+    "linux_version",
     "opsys",
     "sys_path_sep",
+    "syspath_paths",
+    "tmpenv",
 )
 _OS_ENVIRON_ATTRS = set(dir(environ))
 
 
 @contextmanager
 def tmpenv(**kwargs: str) -> Generator[Type[Env], Any, None]:
     """Context manager for Env"""
```

### Comparing `shellfish-0.5.0/shellfish/sh.py` & `shellfish-0.5.1/shellfish/sh.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     filepath_gen as filepath_gen,
     filepath_mtimedelta_sec as filepath_mtimedelta_sec,
     files_dirs_gen as files_dirs_gen,
     files_gen as files_gen,
     filesize as filesize,
     filesize_async as filesize_async,
     fspath as fspath,
+    glob as glob,
     is_dir as is_dir,
     is_dir_async as is_dir_async,
     is_file as is_file,
     is_file_async as is_file_async,
     is_link as is_link,
     is_link_async as is_link_async,
     isdir as isdir,
@@ -117,14 +118,15 @@
     sbin_async as sbin_async,
     sbytes as sbytes,
     sbytes_async as sbytes_async,
     sbytes_gen as sbytes_gen,
     sbytes_gen_async as sbytes_gen_async,
     scandir as scandir,
     scandir_gen as scandir_gen,
+    scandir_gen_filter as scandir_gen_filter,
     scandir_list as scandir_list,
     sep_join as sep_join,
     sep_lstrip as sep_lstrip,
     sep_rstrip as sep_rstrip,
     sep_split as sep_split,
     sep_strip as sep_strip,
     shebang as shebang,
@@ -160,19 +162,22 @@
 from shellfish.stdio import Stdio as Stdio
 from xtyping import STDIN, AnyStr, IterableStr, TypedDict
 
 __all__ = (
     "LIN",
     "WIN",
     "Done",
+    "DoneDict",
     "DoneError",
     "DoneObj",
     "Flag",
     "FlagMeta",
     "HrTime",
+    "HrTimeDict",
+    "HrTimeObj",
     # fs exports
     "Stdio",
     "SymlinkType",
     "TimeoutExpired",
     "__version__",
     "basename",
     "cd",
@@ -184,14 +189,15 @@
     "dir_exists_async",
     "dirname",
     "dirpath_gen",
     "dirs_gen",
     "do",
     "do_",
     "do_async",
+    "do_asyncify",
     "doa",
     "echo",
     "exists",
     "exists_async",
     "export",
     "extension",
     "file_exists",
@@ -202,14 +208,15 @@
     "filepath_mtimedelta_sec",
     "files_dirs_gen",
     "files_gen",
     "filesize",
     "filesize_async",
     "flatten_args",
     "fspath",
+    "glob",
     "is_dir",
     "is_dir_async",
     "is_file",
     "is_file_async",
     "is_link",
     "is_link_async",
     "isdir",
@@ -228,27 +235,30 @@
     "link_file",
     "link_files",
     "listdir_async",
     "listdir_gen",
     "ljson",
     "ljson_async",
     "ls",
+    "ls_async",
     "ls_dirs",
     "ls_files",
     "ls_files_dirs",
     "lstat_async",
     "lstr",
     "lstr_async",
     "lstring",
     "lstring_async",
     "mkdir",
     "mkdirp",
+    "mkenv",
     "move",
     "mv",
     "path_gen",
+    "popen_has_pipe_character",
     "pstderr",
     "pstdout",
     "pstdout_pstderr",
     "pwd",
     "q",
     "quote",
     "rbin",
@@ -267,24 +277,27 @@
     "rmdir",
     "rmfile",
     "rstr",
     "rstr_async",
     "rstring",
     "rstring_async",
     "run",
+    "run_async",
     "safepath",
     "sbin",
     "sbin_async",
     "sbytes",
     "sbytes_async",
     "sbytes_gen",
     "sbytes_gen_async",
     "scandir",
     "scandir_gen",
+    "scandir_gen_filter",
     "scandir_list",
+    "seconds2hrtime",
     "sep_join",
     "sep_lstrip",
     "sep_rstrip",
     "sep_split",
     "sep_strip",
     "setenv",
     "shebang",
@@ -304,14 +317,18 @@
     "sync",
     "touch",
     "tree",
     "unlink_dir",
     "unlink_dirs",
     "unlink_file",
     "unlink_files",
+    "utf8_string",
+    "validate_popen_args",
+    "validate_popen_args_windows",
+    "validate_stdin",
     "walk_gen",
     "wbin",
     "wbin_async",
     "wbin_gen",
     "wbin_gen_async",
     "wbytes",
     "wbytes_async",
```

### Comparing `shellfish-0.5.0/shellfish/sp.py` & `shellfish-0.5.1/shellfish/sp.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.5.0/shellfish/testing.py` & `shellfish-0.5.1/shellfish/testing.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.5.0/shellfish/tests/test_fs.py` & `shellfish-0.5.1/shellfish/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.5.0/PKG-INFO` & `shellfish-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellfish
-Version: 0.5.0
+Version: 0.5.1
 Summary: shellfish ~ shell & file-system utils
 Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/shellfish
 License: MIT
 Keywords: dgpy,shell,fs,filesystem,typed
 Author: jesse
 Author-email: jesse@dgi.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shellfish Version: 0.5.0 Summary: shellfish ~ shell
+Metadata-Version: 2.1 Name: shellfish Version: 0.5.1 Summary: shellfish ~ shell
 & file-system utils Home-page: https://github.com/dynamic-graphics-inc/dgpy-
 libs/tree/main/libs/shellfish License: MIT Keywords:
 dgpy,shell,fs,filesystem,typed Author: jesse Author-email: jesse@dgi.com
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```


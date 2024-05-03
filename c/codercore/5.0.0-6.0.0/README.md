# Comparing `tmp/codercore-5.0.0.tar.gz` & `tmp/codercore-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codercore-5.0.0.tar", last modified: Fri Oct 27 12:33:20 2023, max compression
+gzip compressed data, was "codercore-6.0.0.tar", last modified: Fri May  3 09:25:21 2024, max compression
```

## Comparing `codercore-5.0.0.tar` & `codercore-6.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 12:33:20.320715 codercore-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      913 2023-10-27 12:33:20.320715 codercore-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-27 12:32:11.000000 codercore-5.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 12:33:20.308714 codercore-5.0.0/codercore/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-10-27 12:32:11.000000 codercore-5.0.0/codercore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 12:33:20.308714 codercore-5.0.0/codercore/db/
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2023-10-27 12:32:11.000000 codercore-5.0.0/codercore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2023-10-27 12:32:11.000000 codercore-5.0.0/codercore/db/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2023-10-27 12:32:11.000000 codercore-5.0.0/codercore/db/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 12:33:20.312714 codercore-5.0.0/codercore/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-10-27 12:32:11.000000 codercore-5.0.0/codercore/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-10-27 12:32:11.000000 codercore-5.0.0/codercore/lib/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-10-27 12:32:11.000000 codercore-5.0.0/codercore/lib/hash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 12:33:20.312714 codercore-5.0.0/codercore/lib/http/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2023-10-27 12:32:11.000000 codercore-5.0.0/codercore/lib/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2023-10-27 12:32:11.000000 codercore-5.0.0/codercore/lib/http/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2023-10-27 12:32:11.000000 codercore-5.0.0/codercore/lib/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 12:33:20.312714 codercore-5.0.0/codercore/lib/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 12:32:11.000000 codercore-5.0.0/codercore/lib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-10-27 12:32:11.000000 codercore-5.0.0/codercore/lib/schemas/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2023-10-27 12:32:11.000000 codercore-5.0.0/codercore/lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-10-27 12:32:11.000000 codercore-5.0.0/codercore/lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 12:33:20.316715 codercore-5.0.0/codercore/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 12:32:11.000000 codercore-5.0.0/codercore/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2023-10-27 12:32:11.000000 codercore-5.0.0/codercore/test/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2023-10-27 12:32:11.000000 codercore-5.0.0/codercore/test/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-10-27 12:32:11.000000 codercore-5.0.0/codercore/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 12:33:20.308714 codercore-5.0.0/codercore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      913 2023-10-27 12:33:20.000000 codercore-5.0.0/codercore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      687 2023-10-27 12:33:20.000000 codercore-5.0.0/codercore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-27 12:33:20.000000 codercore-5.0.0/codercore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-10-27 12:33:20.000000 codercore-5.0.0/codercore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-27 12:33:20.000000 codercore-5.0.0/codercore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-10-27 12:32:11.000000 codercore-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-27 12:33:20.320715 codercore-5.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 12:33:20.316715 codercore-5.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-10-27 12:32:11.000000 codercore-5.0.0/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:25:21.155644 codercore-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-03 09:25:21.155644 codercore-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 09:24:14.000000 codercore-6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:25:21.143644 codercore-6.0.0/codercore/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-03 09:24:14.000000 codercore-6.0.0/codercore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:25:21.147644 codercore-6.0.0/codercore/db/
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-03 09:24:14.000000 codercore-6.0.0/codercore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-03 09:24:14.000000 codercore-6.0.0/codercore/db/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-03 09:24:14.000000 codercore-6.0.0/codercore/db/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:25:21.147644 codercore-6.0.0/codercore/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-03 09:24:14.000000 codercore-6.0.0/codercore/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-03 09:24:14.000000 codercore-6.0.0/codercore/lib/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-03 09:24:14.000000 codercore-6.0.0/codercore/lib/hash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:25:21.147644 codercore-6.0.0/codercore/lib/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-03 09:24:14.000000 codercore-6.0.0/codercore/lib/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-03 09:24:14.000000 codercore-6.0.0/codercore/lib/http/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-03 09:24:14.000000 codercore-6.0.0/codercore/lib/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:25:21.147644 codercore-6.0.0/codercore/lib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:24:14.000000 codercore-6.0.0/codercore/lib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-03 09:24:14.000000 codercore-6.0.0/codercore/lib/schemas/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-03 09:24:14.000000 codercore-6.0.0/codercore/lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-03 09:24:14.000000 codercore-6.0.0/codercore/lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:25:21.151644 codercore-6.0.0/codercore/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:24:14.000000 codercore-6.0.0/codercore/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-03 09:24:14.000000 codercore-6.0.0/codercore/test/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-03 09:24:14.000000 codercore-6.0.0/codercore/test/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-03 09:24:14.000000 codercore-6.0.0/codercore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:25:21.151644 codercore-6.0.0/codercore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-03 09:25:21.000000 codercore-6.0.0/codercore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-03 09:25:21.000000 codercore-6.0.0/codercore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:25:21.000000 codercore-6.0.0/codercore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-03 09:25:21.000000 codercore-6.0.0/codercore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 09:25:21.000000 codercore-6.0.0/codercore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-03 09:24:14.000000 codercore-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 09:25:21.155644 codercore-6.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:25:21.151644 codercore-6.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 09:24:14.000000 codercore-6.0.0/tests/test_types.py
```

### Comparing `codercore-5.0.0/PKG-INFO` & `codercore-6.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: codercore
-Version: 5.0.0
+Version: 6.0.0
 Summary: codercore
 Author-email: Code R <hello@coderstudio.dev>
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp~=3.8
 Requires-Dist: asyncpg~=0.27
 Requires-Dist: asyncstdlib~=3.10
 Requires-Dist: bcrypt~=4.0
 Requires-Dist: cloud-sql-python-connector[asyncpg]~=1.1
 Requires-Dist: psycopg2~=2.9
 Requires-Dist: pydantic~=2.4
 Requires-Dist: pytest~=7.2
-Requires-Dist: redis~=4.3
-Requires-Dist: sqlalchemy[asyncio]~=2.0
-Requires-Dist: sqlalchemy-utils~=0.41
+Requires-Dist: redis~=5.0
+Requires-Dist: sqlalchemy[asyncio]~=1.4
+Requires-Dist: sqlalchemy-utils~=0.38
 Provides-Extra: test
 Requires-Dist: pytest-asyncio~=0.20; extra == "test"
 Requires-Dist: pytest-cov~=4.0; extra == "test"
 Requires-Dist: pytest-mock~=3.10; extra == "test"
 Requires-Dist: pytest-xdist[psutil]~=3.0; extra == "test"
 Provides-Extra: dev
 Requires-Dist: black~=22.10; extra == "dev"
```

### Comparing `codercore-5.0.0/codercore/db/__init__.py` & `codercore-6.0.0/codercore/db/__init__.py`

 * *Files identical despite different names*

### Comparing `codercore-5.0.0/codercore/db/pagination.py` & `codercore-6.0.0/codercore/db/pagination.py`

 * *Files identical despite different names*

### Comparing `codercore-5.0.0/codercore/lib/hash.py` & `codercore-6.0.0/codercore/lib/hash.py`

 * *Files identical despite different names*

### Comparing `codercore-5.0.0/codercore/lib/redis.py` & `codercore-6.0.0/codercore/lib/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,18 @@
         await super().set(*args, ex=ex, **kwargs)
 
 
 def cache(
     key: Callable[P, str] | str,
     ex: int | None = None,
     deserialize: Callable[[Any], RT] = lambda x: x,
-) -> Callable[Callable[P, CT], Callable[Concatenate[Redis, str, P], Awaitable[RT]],]:
+) -> Callable[
+    Callable[P, CT],
+    Callable[Concatenate[Redis, str, P], Awaitable[RT]],
+]:
     def decorate(
         func: Callable[P, CT]
     ) -> Callable[Concatenate[Redis, str, P], Awaitable[RT]]:
         @wraps(func)
         async def wrapper(
             *args: P.args,
             connection: Redis,
```

### Comparing `codercore-5.0.0/codercore/lib/settings.py` & `codercore-6.0.0/codercore/lib/settings.py`

 * *Files identical despite different names*

### Comparing `codercore-5.0.0/codercore/test/fixtures.py` & `codercore-6.0.0/codercore/test/fixtures.py`

 * *Files identical despite different names*

### Comparing `codercore-5.0.0/codercore/test/pydantic.py` & `codercore-6.0.0/codercore/test/pydantic.py`

 * *Files identical despite different names*

### Comparing `codercore-5.0.0/codercore.egg-info/PKG-INFO` & `codercore-6.0.0/codercore.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: codercore
-Version: 5.0.0
+Version: 6.0.0
 Summary: codercore
 Author-email: Code R <hello@coderstudio.dev>
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp~=3.8
 Requires-Dist: asyncpg~=0.27
 Requires-Dist: asyncstdlib~=3.10
 Requires-Dist: bcrypt~=4.0
 Requires-Dist: cloud-sql-python-connector[asyncpg]~=1.1
 Requires-Dist: psycopg2~=2.9
 Requires-Dist: pydantic~=2.4
 Requires-Dist: pytest~=7.2
-Requires-Dist: redis~=4.3
-Requires-Dist: sqlalchemy[asyncio]~=2.0
-Requires-Dist: sqlalchemy-utils~=0.41
+Requires-Dist: redis~=5.0
+Requires-Dist: sqlalchemy[asyncio]~=1.4
+Requires-Dist: sqlalchemy-utils~=0.38
 Provides-Extra: test
 Requires-Dist: pytest-asyncio~=0.20; extra == "test"
 Requires-Dist: pytest-cov~=4.0; extra == "test"
 Requires-Dist: pytest-mock~=3.10; extra == "test"
 Requires-Dist: pytest-xdist[psutil]~=3.0; extra == "test"
 Provides-Extra: dev
 Requires-Dist: black~=22.10; extra == "dev"
```

### Comparing `codercore-5.0.0/codercore.egg-info/SOURCES.txt` & `codercore-6.0.0/codercore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codercore-5.0.0/pyproject.toml` & `codercore-6.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "codercore"
-version = "5.0.0"
+version = "6.0.0"
 description = "codercore"
 readme = "README.md"
 authors = [{ name = "Code R", email = "hello@coderstudio.dev" }]
 dependencies = [
     'aiohttp ~= 3.8',
     'asyncpg ~= 0.27',
     'asyncstdlib ~= 3.10',
     'bcrypt ~= 4.0',
     'cloud-sql-python-connector[asyncpg] ~= 1.1',
     'psycopg2 ~= 2.9',
     'pydantic ~= 2.4',
     'pytest ~= 7.2',
-    'redis ~= 4.3',
-    'sqlalchemy[asyncio] ~= 2.0',
-    'sqlalchemy-utils ~= 0.41'
+    'redis ~= 5.0',
+    'sqlalchemy[asyncio] ~= 1.4',
+    'sqlalchemy-utils ~= 0.38'
 ]
 
 [project.optional-dependencies]
 test = [
     'pytest-asyncio ~= 0.20',
     'pytest-cov ~= 4.0',
     'pytest-mock ~= 3.10',
@@ -32,15 +32,15 @@
 dev = [
     'black ~= 22.10',
     'flake8 ~= 6.0',
     'isort ~= 5.11',
 ]
 
 [tool.bumpver]
-current_version = "5.0.0"
+current_version = "6.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```


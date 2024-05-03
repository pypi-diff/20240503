# Comparing `tmp/python_none_objects-1.1.7.tar.gz` & `tmp/python_none_objects-1.1.8.tar.gz`

## Comparing `python_none_objects-1.1.7.tar` & `python_none_objects-1.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/README_printable.md
--rwxr-xr-x   0        0        0     2345 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/build_and_checks.sh
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/wget_sha512.sh
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/src/python_none_objects/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/src/python_none_objects/py.typed
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/typing_test/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/COPYING.LESSER
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/README.md
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/pyproject.toml
--rw-r--r--   0        0        0    14879 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/README_printable.md
+-rwxr-xr-x   0        0        0     2468 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/build_and_checks.sh
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/wget_sha512.sh
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/src/python_none_objects/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/src/python_none_objects/py.typed
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/typing_test/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/COPYING.LESSER
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/README.md
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0    14879 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/PKG-INFO
```

### Comparing `python_none_objects-1.1.7/README_printable.md` & `python_none_objects-1.1.8/README_printable.md`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.7/build_and_checks.sh` & `python_none_objects-1.1.8/build_and_checks.sh`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 
 echo "Running isort"
 isort .
 
 echo "Running black"
 black .
 
+echo "Checking empty lines after Python function docstrings"
+pcregrep -M $'def [^"]*"""([^"]|"(?!""))*"""\n\n' -- **/*.py
+
 echo "Running pylint"
 pylint src/python_none_objects/
 pylint typing_test/
 
 echo "Running mypy"
 mypy .
```

### Comparing `python_none_objects-1.1.7/wget_sha512.sh` & `python_none_objects-1.1.8/wget_sha512.sh`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.7/src/python_none_objects/__init__.py` & `python_none_objects-1.1.8/src/python_none_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.7/typing_test/__init__.py` & `python_none_objects-1.1.8/typing_test/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,42 +36,38 @@
 )
 
 
 def foo_collection(x: Collection[str] = NoneCollection) -> bool:
     """
     Check typing for NoneCollection.
     """
-
     for y in x:
         print(f"foo {y}")
     return "toto" in x
 
 
 def foo_iterable(x: Iterable[str] = NoneIterable) -> None:
     """
     Check typing for NoneIterable.
     """
-
     for y in x:
         print(f"foo {y}")
 
 
 def foo_container(x: Container[str] = NoneContainer) -> bool:
     """
     Check typing for NoneContainer.
     """
-
     return "toto" in x
 
 
 def foo_mapping(x: Mapping[str, str] = NoneMapping) -> None:
     """
     Check typing for NoneMapping.
     """
-
     for y, z in x.items():
         print(f"foo {y} bar {z}")
 
 
 foo_collection()
 foo_iterable()
 foo_container()
```

### Comparing `python_none_objects-1.1.7/COPYING` & `python_none_objects-1.1.8/COPYING`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.7/COPYING.LESSER` & `python_none_objects-1.1.8/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.7/README.md` & `python_none_objects-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.7/pyproject.toml` & `python_none_objects-1.1.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python-none-objects"
-version = "1.1.7"
+version = "1.1.8"
 description = """\
 Add more constant \"None\" objects to Python \
 to avoid boilerplate code\
 """
 readme = "README.md"
 authors = [
     { name = "Laurent Lyaudet", email = "laurent.lyaudet@gmail.com" },
```

### Comparing `python_none_objects-1.1.7/PKG-INFO` & `python_none_objects-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python-none-objects
-Version: 1.1.7
+Version: 1.1.8
 Summary: Add more constant "None" objects to Python to avoid boilerplate code
 Project-URL: Homepage, https://github.com/LLyaudet/python-none-objects
 Project-URL: Bug Tracker, https://github.com/LLyaudet/python-none-objects/issues
 Author-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 Maintainer-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```


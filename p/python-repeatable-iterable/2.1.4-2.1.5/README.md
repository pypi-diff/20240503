# Comparing `tmp/python_repeatable_iterable-2.1.4.tar.gz` & `tmp/python_repeatable_iterable-2.1.5.tar.gz`

## Comparing `python_repeatable_iterable-2.1.4.tar` & `python_repeatable_iterable-2.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/CONTRIBUTORS.md
--rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/README_printable.md
--rwxr-xr-x   0        0        0     2380 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/build_and_checks.sh
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/wget_sha512.sh
--rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/src/python_repeatable_iterable/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/src/python_repeatable_iterable/py.typed
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/typing_test/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/COPYING.LESSER
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/README.md
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/pyproject.toml
--rw-r--r--   0        0        0    14586 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/CONTRIBUTORS.md
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/README_printable.md
+-rwxr-xr-x   0        0        0     2503 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/build_and_checks.sh
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/wget_sha512.sh
+-rw-r--r--   0        0        0     4904 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/src/python_repeatable_iterable/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/src/python_repeatable_iterable/py.typed
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/typing_test/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/COPYING.LESSER
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/README.md
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0    14586 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/PKG-INFO
```

### Comparing `python_repeatable_iterable-2.1.4/README_printable.md` & `python_repeatable_iterable-2.1.5/README_printable.md`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.4/build_and_checks.sh` & `python_repeatable_iterable-2.1.5/build_and_checks.sh`

 * *Files 4% similar despite different names*

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
 pylint src/python_repeatable_iterable/
 pylint typing_test/
 
 echo "Running mypy"
 mypy .
```

### Comparing `python_repeatable_iterable-2.1.4/wget_sha512.sh` & `python_repeatable_iterable-2.1.5/wget_sha512.sh`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.4/src/python_repeatable_iterable/__init__.py` & `python_repeatable_iterable-2.1.5/src/python_repeatable_iterable/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,14 @@
         cls,
         iterable: Iterable[T],
         safe_classes: Iterable[type[object]] = NoneIterable,
     ) -> "RepeatableIterable[T]":
         """
         Here is an implementation avoiding the previous problem.
         """
-
         iterable_type = type(iterable)
         for some_class in (
             list,
             tuple,
             range,
             str,
             bytes,
```

### Comparing `python_repeatable_iterable-2.1.4/typing_test/__init__.py` & `python_repeatable_iterable-2.1.5/typing_test/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     x: RepeatableIterable[List[T1]],
 ) -> List[T1]:
     """
     Check that mypy follows the types
     between the argument and the return of the function
     for the type of the content of the list.
     """
-
     result = []
     for y in x:
         result.extend(y)
     for y in x:
         result.extend(y)
     return result
 
@@ -56,15 +55,14 @@
 ) -> List[T1]:
     """
     Check that mypy follows the types
     between the argument and the return of the function
     for the type of the content of the list
     with indirections.
     """
-
     return test_arg_to_return_typing(RepeatableIterable(x))
 
 
 a: List[List[Never]] = [[], []]
 print(test_arg_to_return_via_call_typing(a))
 
 b = (x for x in a)
@@ -76,14 +74,13 @@
 ) -> RepeatableIterable[T1]:
     """
     Check that mypy follows the types
     between the argument and the return of the function
     for the type of the content of the list
     with a final cast.
     """
-
     result = []
     for y in x:
         result.extend(y)
     for y in x:
         result.extend(y)
     return RepeatableIterable(result)
```

### Comparing `python_repeatable_iterable-2.1.4/COPYING` & `python_repeatable_iterable-2.1.5/COPYING`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.4/COPYING.LESSER` & `python_repeatable_iterable-2.1.5/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.4/README.md` & `python_repeatable_iterable-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.4/pyproject.toml` & `python_repeatable_iterable-2.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python-repeatable-iterable"
-version = "2.1.4"
+version = "2.1.5"
 description = """\
 Add a RepeatableIterable type and a function to obtain it\
 """
 readme = "README.md"
 authors = [
     { name = "Laurent Lyaudet", email = "laurent.lyaudet@gmail.com" },
 ]
```

### Comparing `python_repeatable_iterable-2.1.4/PKG-INFO` & `python_repeatable_iterable-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python-repeatable-iterable
-Version: 2.1.4
+Version: 2.1.5
 Summary: Add a RepeatableIterable type and a function to obtain it
 Project-URL: Homepage, https://github.com/LLyaudet/python-repeatable-iterable
 Project-URL: Bug Tracker, https://github.com/LLyaudet/python-repeatable-iterable/issues
 Author-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 Maintainer-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```


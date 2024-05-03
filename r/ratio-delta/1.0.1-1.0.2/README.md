# Comparing `tmp/ratio_delta-1.0.1.tar.gz` & `tmp/ratio_delta-1.0.2.tar.gz`

## Comparing `ratio_delta-1.0.1.tar` & `ratio_delta-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    14448 2020-02-02 00:00:00.000000 ratio_delta-1.0.1/README_printable.md
--rw-r--r--   0        0        0     8501 2020-02-02 00:00:00.000000 ratio_delta-1.0.1/src/ratio_delta/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ratio_delta-1.0.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 ratio_delta-1.0.1/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 ratio_delta-1.0.1/COPYING.LESSER
--rw-r--r--   0        0        0    14394 2020-02-02 00:00:00.000000 ratio_delta-1.0.1/README.md
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 ratio_delta-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    24610 2020-02-02 00:00:00.000000 ratio_delta-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    14448 2020-02-02 00:00:00.000000 ratio_delta-1.0.2/README_printable.md
+-rw-r--r--   0        0        0     8481 2020-02-02 00:00:00.000000 ratio_delta-1.0.2/src/ratio_delta/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ratio_delta-1.0.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 ratio_delta-1.0.2/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 ratio_delta-1.0.2/COPYING.LESSER
+-rw-r--r--   0        0        0    14394 2020-02-02 00:00:00.000000 ratio_delta-1.0.2/README.md
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 ratio_delta-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    24610 2020-02-02 00:00:00.000000 ratio_delta-1.0.2/PKG-INFO
```

### Comparing `ratio_delta-1.0.1/README_printable.md` & `ratio_delta-1.0.2/README_printable.md`

 * *Files identical despite different names*

### Comparing `ratio_delta-1.0.1/src/ratio_delta/__init__.py` & `ratio_delta-1.0.2/src/ratio_delta/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,210 +31,194 @@
     b: float,
     c: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
-
     return a / b + c
 
 
 def fused_divide_subtract(
     a: float,
     b: float,
     c: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
-
     return a / b - c
 
 
 def fused_absolute_divide_add(
     a: float,
     b: float,
     c: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
-
     return abs(a / b + c)
 
 
 def fused_absolute_divide_subtract(
     a: float,
     b: float,
     c: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
-
     return abs(a / b - c)
 
 
 def scaled_fused_divide_add(
     a: float,
     b: float,
     c: float,
     scale: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
-
     return (a / b + c) * scale
 
 
 def scaled_fused_divide_subtract(
     a: float,
     b: float,
     c: float,
     scale: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
-
     return (a / b - c) * scale
 
 
 def scaled_fused_absolute_divide_add(
     a: float,
     b: float,
     c: float,
     scale: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
-
     return abs(a / b + c) * scale
 
 
 def scaled_fused_absolute_divide_subtract(
     a: float,
     b: float,
     c: float,
     scale: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
-
     return abs(a / b - c) * scale
 
 
 def fused_divide_increment(
     a: float,
     b: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
-
     return a / b + 1
 
 
 def fused_divide_decrement(
     a: float,
     b: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
-
     return a / b - 1
 
 
 def fused_absolute_divide_increment(
     a: float,
     b: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
-
     return abs(a / b + 1)
 
 
 def fused_absolute_divide_decrement(
     a: float,
     b: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
-
     return abs(a / b - 1)
 
 
 def scaled_fused_divide_increment(
     a: float,
     b: float,
     scale: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
-
     return (a / b + 1) * scale
 
 
 def scaled_fused_divide_decrement(
     a: float,
     b: float,
     scale: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
-
     return (a / b - 1) * scale
 
 
 def scaled_fused_absolute_divide_increment(
     a: float,
     b: float,
     scale: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
-
     return abs(a / b + 1) * scale
 
 
 def scaled_fused_absolute_divide_decrement(
     a: float,
     b: float,
     scale: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
-
     return abs(a / b - 1) * scale
 
 
 # pylint: disable-next=too-many-arguments,too-many-return-statements
 def ratio_iota(
     a: Optional[float],
     b: Optional[float],
@@ -245,15 +229,14 @@
     a_null: Optional[float] = None,
     b_null: Optional[float] = None,
     b_zero: Optional[float] = None,
 ) -> Optional[float]:
     """
     Divide and increment, and more if affinity.
     """
-
     if a is None:
         if b is None:
             return both_null
         return a_null
     if b is None:
         return b_null
     if b == 0:
@@ -278,15 +261,14 @@
     a_null: Optional[float] = None,
     b_null: Optional[float] = None,
     b_zero: Optional[float] = None,
 ) -> Optional[float]:
     """
     Divide and decrement, and more if affinity.
     """
-
     if a is None:
         if b is None:
             return both_null
         return a_null
     if b is None:
         return b_null
     if b == 0:
@@ -316,15 +298,14 @@
     b_null: Optional[float] = None,
     c_null: Optional[float] = None,
     b_zero: Optional[float] = None,
 ) -> Optional[float]:
     """
     Divide and add, and more if affinity.
     """
-
     if a is None:
         if b is None:
             if c is None:
                 return all_null
             return a_b_null
         if c is None:
             return a_c_null
@@ -362,15 +343,14 @@
     b_null: Optional[float] = None,
     c_null: Optional[float] = None,
     b_zero: Optional[float] = None,
 ) -> Optional[float]:
     """
     Divide and subtract, and more if affinity.
     """
-
     if a is None:
         if b is None:
             if c is None:
                 return all_null
             return a_b_null
         if c is None:
             return a_c_null
```

### Comparing `ratio_delta-1.0.1/COPYING` & `ratio_delta-1.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `ratio_delta-1.0.1/COPYING.LESSER` & `ratio_delta-1.0.2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `ratio_delta-1.0.1/README.md` & `ratio_delta-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ratio_delta-1.0.1/pyproject.toml` & `ratio_delta-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ratio-delta"
-version = "1.0.1"
+version = "1.0.2"
 description = """\
 Add functions for variants of a common arithmetic operation\
 """
 readme = "README.md"
 authors = [
     { name = "Laurent Lyaudet", email = "laurent.lyaudet@gmail.com" },
 ]
```

### Comparing `ratio_delta-1.0.1/PKG-INFO` & `ratio_delta-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ratio-delta
-Version: 1.0.1
+Version: 1.0.2
 Summary: Add functions for variants of a common arithmetic operation
 Project-URL: Homepage, https://github.com/LLyaudet/RatioDelta
 Project-URL: Bug Tracker, https://github.com/LLyaudet/RatioDelta/issues
 Author-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 Maintainer-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```


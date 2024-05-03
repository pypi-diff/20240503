# Comparing `tmp/django_monkey_patches-3.0.2.tar.gz` & `tmp/django_monkey_patches-3.0.3.tar.gz`

## Comparing `django_monkey_patches-3.0.2.tar` & `django_monkey_patches-3.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/README_printable.md
--rwxr-xr-x   0        0        0     2307 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/build_and_checks.sh
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/wget_sha512.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/src/django_monkey_patches/__init__.py
--rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/src/django_monkey_patches/django__base_cache__make_cache_key.py
--rw-r--r--   0        0        0    15568 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/src/django_monkey_patches/django__orm__prefetch.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/src/django_monkey_patches/django__query_set.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/src/django_monkey_patches/django__query_set__get.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/src/django_monkey_patches/django__query_set__get_or_create.py
--rw-r--r--   0        0        0    37274 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/src/django_monkey_patches/django__query_wrapper.py
--rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/src/django_monkey_patches/django__test_case__tear_down.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/src/django_monkey_patches/django_rest_framework__field__get_request.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py
--rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/src/django_monkey_patches.egg-info/PKG-INFO
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/src/django_monkey_patches.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/src/django_monkey_patches.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/src/django_monkey_patches.egg-info/requires.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/src/django_monkey_patches.egg-info/top_level.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/COPYING.LESSER
--rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/README.md
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/pyproject.toml
--rw-r--r--   0        0        0    13867 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/README_printable.md
+-rwxr-xr-x   0        0        0     2439 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/build_and_checks.sh
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/wget_sha512.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/__init__.py
+-rw-r--r--   0        0        0    39101 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/django__base_cache__make_cache_key.py
+-rw-r--r--   0        0        0    15669 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/django__orm__prefetch.py
+-rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/django__query_set.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/django__query_set__get.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/django__query_set__get_or_create.py
+-rw-r--r--   0        0        0    37322 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/django__query_wrapper.py
+-rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/django__test_case__tear_down.py
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/django_rest_framework__field__get_request.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py
+-rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches.egg-info/requires.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches.egg-info/top_level.txt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/COPYING.LESSER
+-rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/README.md
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0    13867 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/PKG-INFO
```

### Comparing `django_monkey_patches-3.0.2/README_printable.md` & `django_monkey_patches-3.0.3/README_printable.md`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.2/build_and_checks.sh` & `django_monkey_patches-3.0.3/build_and_checks.sh`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # You should have received a copy of
 # the GNU Lesser General Public License
 # along with django-monkey-patches.
 # If not, see <http://www.gnu.org/licenses/>.
 #
 # ©Copyright 2023-2024 Laurent Lyaudet
 
+shopt -s globstar
 source ./wget_sha512.sh
 
 personal_github="https://raw.githubusercontent.com/LLyaudet/"
 
 echo "Building README.md"
 script="$personal_github""DevOrSysAdminScripts/main/build_readme.sh"
 correct_sha512="a7705592c14c7709f8762967f5c5d1c98d27b8ab97fe2aaa73302"
@@ -37,19 +38,20 @@
 
 echo "Running isort"
 isort .
 
 echo "Running black"
 black .
 
+echo "Checking empty lines after Python function docstrings"
+pcregrep -M $'def [^"]*"""([^"]|"(?!""))*"""\n\n(?!\s*def)' -- **/*.py
+
 echo "Running pylint"
 pylint src/django_monkey_patches/
 
-shopt -s globstar
-
 echo "Analyzing too long lines"
 script="$personal_github"
 script+="DevOrSysAdminScripts/main/too_long_code_lines.sh"
 correct_sha512="eab26337506d6fabdea227c4b584391cc4a728e6b852be2232a7e"
 correct_sha512+="4d21261eb356df77257b0ea7152c9587ce89a963732fc644caf1"
 correct_sha512+="38c21ee51932e6fa6168bf9"
 wget_sha512 ./too_long_code_lines.sh "$script" "$correct_sha512"
```

### Comparing `django_monkey_patches-3.0.2/wget_sha512.sh` & `django_monkey_patches-3.0.3/wget_sha512.sh`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.2/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py` & `django_monkey_patches-3.0.3/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -775,15 +775,14 @@
     A function to obtain a c_field_list_list_nnl.
     """
 
     def c_field_list_list_nnl(x):
         """
         The customized c_field_list_list_nnl.
         """
-
         return [getattr(x, f)] if getattr(x, f) else []
 
     return c_field_list_list_nnl
 
 
 def cc_field_id_list_list_nnl(f):
     """
@@ -791,30 +790,28 @@
     """
     g = f + "_id"
 
     def c_field_id_list_list_nnl(x):
         """
         The customized c_field_id_list_list_nnl.
         """
-
         return [getattr(x, f)] if getattr(x, g) else []
 
     return c_field_id_list_list_nnl
 
 
 def cc_field_not_none_list_list_nnl(f):
     """
     A function to obtain a c_field_not_none_list_list_nnl.
     """
 
     def c_field_not_none_list_list_nnl(x):
         """
         The customized c_field_not_none_list_list_nnl.
         """
-
         return [getattr(x, f)] if getattr(x, f) is not None else []
 
     return c_field_not_none_list_list_nnl
 
 
 def cc_field_id_not_none_list_list_nnl(f):
     """
@@ -822,30 +819,28 @@
     """
     g = f + "_id"
 
     def c_field_id_not_none_list_list_nnl(x):
         """
         The customized c_field_id_not_none_list_list_nnl.
         """
-
         return [getattr(x, f)] if getattr(x, g) is not None else []
 
     return c_field_id_not_none_list_list_nnl
 
 
 def cc_field_none_list_list_nnl(f):
     """
     A function to obtain a c_field_none_list_list_nnl.
     """
 
     def c_field_none_list_list_nnl(x):
         """
         The customized c_field_none_list_list_nnl.
         """
-
         return [] if getattr(x, f) is None else [getattr(x, f)]
 
     return c_field_none_list_list_nnl
 
 
 def cc_field_id_none_list_list_nnl(f):
     """
@@ -853,30 +848,28 @@
     """
     g = f + "_id"
 
     def c_field_id_none_list_list_nnl(x):
         """
         The customized c_field_id_none_list_list_nnl.
         """
-
         return [] if getattr(x, g) is None else [getattr(x, f)]
 
     return c_field_id_none_list_list_nnl
 
 
 def cc_field_tuple_tuple_nnl(f):
     """
     A function to obtain a c_field_tuple_tuple_nnl.
     """
 
     def c_field_tuple_tuple_nnl(x):
         """
         The customized c_field_tuple_tuple_nnl.
         """
-
         return (getattr(x, f),) if getattr(x, f) else ()
 
     return c_field_tuple_tuple_nnl
 
 
 def cc_field_id_tuple_tuple_nnl(f):
     """
@@ -884,30 +877,28 @@
     """
     g = f + "_id"
 
     def c_field_id_tuple_tuple_nnl(x):
         """
         The customized c_field_id_tuple_tuple_nnl.
         """
-
         return (getattr(x, f),) if getattr(x, g) else ()
 
     return c_field_id_tuple_tuple_nnl
 
 
 def cc_field_not_none_tuple_tuple_nnl(f):
     """
     A function to obtain a c_field_not_none_tuple_tuple_nnl.
     """
 
     def c_field_not_none_tuple_tuple_nnl(x):
         """
         The customized c_field_not_none_tuple_tuple_nnl.
         """
-
         return (getattr(x, f),) if getattr(x, f) is not None else ()
 
     return c_field_not_none_tuple_tuple_nnl
 
 
 def cc_field_id_not_none_tuple_tuple_nnl(f):
     """
@@ -915,30 +906,28 @@
     """
     g = f + "_id"
 
     def c_field_id_not_none_tuple_tuple_nnl(x):
         """
         The customized c_field_id_not_none_tuple_tuple_nnl.
         """
-
         return (getattr(x, f),) if getattr(x, g) is not None else ()
 
     return c_field_id_not_none_tuple_tuple_nnl
 
 
 def cc_field_none_tuple_tuple_nnl(f):
     """
     A function to obtain a c_field_none_tuple_tuple_nnl.
     """
 
     def c_field_none_tuple_tuple_nnl(x):
         """
         The customized c_field_none_tuple_tuple_nnl.
         """
-
         return () if getattr(x, f) is None else (getattr(x, f),)
 
     return c_field_none_tuple_tuple_nnl
 
 
 def cc_field_id_none_tuple_tuple_nnl(f):
     """
@@ -946,30 +935,28 @@
     """
     g = f + "_id"
 
     def c_field_id_none_tuple_tuple_nnl(x):
         """
         The customized c_field_id_none_tuple_tuple_nnl.
         """
-
         return () if getattr(x, g) is None else (getattr(x, f),)
 
     return c_field_id_none_tuple_tuple_nnl
 
 
 def cc_field_list_tuple_nnl(f):
     """
     A function to obtain a c_field_list_tuple_nnl.
     """
 
     def c_field_list_tuple_nnl(x):
         """
         The customized c_field_list_tuple_nnl.
         """
-
         return [getattr(x, f)] if getattr(x, f) else ()
 
     return c_field_list_tuple_nnl
 
 
 def cc_field_id_list_tuple_nnl(f):
     """
@@ -977,30 +964,28 @@
     """
     g = f + "_id"
 
     def c_field_id_list_tuple_nnl(x):
         """
         The customized c_field_id_list_tuple_nnl.
         """
-
         return [getattr(x, f)] if getattr(x, g) else ()
 
     return c_field_id_list_tuple_nnl
 
 
 def cc_field_not_none_list_tuple_nnl(f):
     """
     A function to obtain a c_field_not_none_list_tuple_nnl.
     """
 
     def c_field_not_none_list_tuple_nnl(x):
         """
         The customized c_field_not_none_list_tuple_nnl.
         """
-
         return [getattr(x, f)] if getattr(x, f) is not None else ()
 
     return c_field_not_none_list_tuple_nnl
 
 
 def cc_field_id_not_none_list_tuple_nnl(f):
     """
@@ -1008,30 +993,28 @@
     """
     g = f + "_id"
 
     def c_field_id_not_none_list_tuple_nnl(x):
         """
         The customized c_field_id_not_none_list_tuple_nnl.
         """
-
         return [getattr(x, f)] if getattr(x, g) is not None else ()
 
     return c_field_id_not_none_list_tuple_nnl
 
 
 def cc_field_none_list_tuple_nnl(f):
     """
     A function to obtain a c_field_none_list_tuple_nnl.
     """
 
     def c_field_none_list_tuple_nnl(x):
         """
         The customized c_field_none_list_tuple_nnl.
         """
-
         return () if getattr(x, f) is None else [getattr(x, f)]
 
     return c_field_none_list_tuple_nnl
 
 
 def cc_field_id_none_list_tuple_nnl(f):
     """
@@ -1039,30 +1022,28 @@
     """
     g = f + "_id"
 
     def c_field_id_none_list_tuple_nnl(x):
         """
         The customized c_field_id_none_list_tuple_nnl.
         """
-
         return () if getattr(x, g) is None else [getattr(x, f)]
 
     return c_field_id_none_list_tuple_nnl
 
 
 def cc_field_tuple_list_nnl(f):
     """
     A function to obtain a c_field_tuple_list_nnl.
     """
 
     def c_field_tuple_list_nnl(x):
         """
         The customized c_field_tuple_list_nnl.
         """
-
         return (getattr(x, f),) if getattr(x, f) else []
 
     return c_field_tuple_list_nnl
 
 
 def cc_field_id_tuple_list_nnl(f):
     """
@@ -1070,30 +1051,28 @@
     """
     g = f + "_id"
 
     def c_field_id_tuple_list_nnl(x):
         """
         The customized c_field_id_tuple_list_nnl.
         """
-
         return (getattr(x, f),) if getattr(x, g) else []
 
     return c_field_id_tuple_list_nnl
 
 
 def cc_field_not_none_tuple_list_nnl(f):
     """
     A function to obtain a c_field_not_none_tuple_list_nnl.
     """
 
     def c_field_not_none_tuple_list_nnl(x):
         """
         The customized c_field_not_none_tuple_list_nnl.
         """
-
         return (getattr(x, f),) if getattr(x, f) is not None else []
 
     return c_field_not_none_tuple_list_nnl
 
 
 def cc_field_id_not_none_tuple_list_nnl(f):
     """
@@ -1101,30 +1080,28 @@
     """
     g = f + "_id"
 
     def c_field_id_not_none_tuple_list_nnl(x):
         """
         The customized c_field_id_not_none_tuple_list_nnl.
         """
-
         return (getattr(x, f),) if getattr(x, g) is not None else []
 
     return c_field_id_not_none_tuple_list_nnl
 
 
 def cc_field_none_tuple_list_nnl(f):
     """
     A function to obtain a c_field_none_tuple_list_nnl.
     """
 
     def c_field_none_tuple_list_nnl(x):
         """
         The customized c_field_none_tuple_list_nnl.
         """
-
         return [] if getattr(x, f) is None else (getattr(x, f),)
 
     return c_field_none_tuple_list_nnl
 
 
 def cc_field_id_none_tuple_list_nnl(f):
     """
@@ -1132,30 +1109,28 @@
     """
     g = f + "_id"
 
     def c_field_id_none_tuple_list_nnl(x):
         """
         The customized c_field_id_none_tuple_list_nnl.
         """
-
         return [] if getattr(x, g) is None else (getattr(x, f),)
 
     return c_field_id_none_tuple_list_nnl
 
 
 def cc_field_tuple_empty_nnl(f):
     """
     A function to obtain a c_field_tuple_empty_nnl.
     """
 
     def c_field_tuple_empty_nnl(x):
         """
         The customized c_field_tuple_empty_nnl.
         """
-
         return (getattr(x, f),) if getattr(x, f) else e
 
     return c_field_tuple_empty_nnl
 
 
 def cc_field_id_tuple_empty_nnl(f):
     """
@@ -1163,30 +1138,28 @@
     """
     g = f + "_id"
 
     def c_field_id_tuple_empty_nnl(x):
         """
         The customized c_field_id_tuple_empty_nnl.
         """
-
         return (getattr(x, f),) if getattr(x, g) else e
 
     return c_field_id_tuple_empty_nnl
 
 
 def cc_field_not_none_tuple_empty_nnl(f):
     """
     A function to obtain a c_field_not_none_tuple_empty_nnl.
     """
 
     def c_field_not_none_tuple_empty_nnl(x):
         """
         The customized c_field_not_none_tuple_empty_nnl.
         """
-
         return (getattr(x, f),) if getattr(x, f) is not None else e
 
     return c_field_not_none_tuple_empty_nnl
 
 
 def cc_field_id_not_none_tuple_empty_nnl(f):
     """
@@ -1194,30 +1167,28 @@
     """
     g = f + "_id"
 
     def c_field_id_not_none_tuple_empty_nnl(x):
         """
         The customized c_field_id_not_none_tuple_empty_nnl.
         """
-
         return (getattr(x, f),) if getattr(x, g) is not None else e
 
     return c_field_id_not_none_tuple_empty_nnl
 
 
 def cc_field_none_tuple_empty_nnl(f):
     """
     A function to obtain a c_field_none_tuple_empty_nnl.
     """
 
     def c_field_none_tuple_empty_nnl(x):
         """
         The customized c_field_none_tuple_empty_nnl.
         """
-
         return e if getattr(x, f) is None else (getattr(x, f),)
 
     return c_field_none_tuple_empty_nnl
 
 
 def cc_field_id_none_tuple_empty_nnl(f):
     """
@@ -1225,30 +1196,28 @@
     """
     g = f + "_id"
 
     def c_field_id_none_tuple_empty_nnl(x):
         """
         The customized c_field_id_none_tuple_empty_nnl.
         """
-
         return e if getattr(x, g) is None else (getattr(x, f),)
 
     return c_field_id_none_tuple_empty_nnl
 
 
 def cc_field_list_empty_nnl(f):
     """
     A function to obtain a c_field_list_empty_nnl.
     """
 
     def c_field_list_empty_nnl(x):
         """
         The customized c_field_list_empty_nnl.
         """
-
         return [getattr(x, f)] if getattr(x, f) else e
 
     return c_field_list_empty_nnl
 
 
 def cc_field_id_list_empty_nnl(f):
     """
@@ -1256,30 +1225,28 @@
     """
     g = f + "_id"
 
     def c_field_id_list_empty_nnl(x):
         """
         The customized c_field_id_list_empty_nnl.
         """
-
         return [getattr(x, f)] if getattr(x, g) else e
 
     return c_field_id_list_empty_nnl
 
 
 def cc_field_not_none_list_empty_nnl(f):
     """
     A function to obtain a c_field_not_none_list_empty_nnl.
     """
 
     def c_field_not_none_list_empty_nnl(x):
         """
         The customized c_field_not_none_list_empty_nnl.
         """
-
         return [getattr(x, f)] if getattr(x, f) is not None else e
 
     return c_field_not_none_list_empty_nnl
 
 
 def cc_field_id_not_none_list_empty_nnl(f):
     """
@@ -1287,30 +1254,28 @@
     """
     g = f + "_id"
 
     def c_field_id_not_none_list_empty_nnl(x):
         """
         The customized c_field_id_not_none_list_empty_nnl.
         """
-
         return [getattr(x, f)] if getattr(x, g) is not None else e
 
     return c_field_id_not_none_list_empty_nnl
 
 
 def cc_field_none_list_empty_nnl(f):
     """
     A function to obtain a c_field_none_list_empty_nnl.
     """
 
     def c_field_none_list_empty_nnl(x):
         """
         The customized c_field_none_list_empty_nnl.
         """
-
         return e if getattr(x, f) is None else [getattr(x, f)]
 
     return c_field_none_list_empty_nnl
 
 
 def cc_field_id_none_list_empty_nnl(f):
     """
@@ -1318,15 +1283,14 @@
     """
     g = f + "_id"
 
     def c_field_id_none_list_empty_nnl(x):
         """
         The customized c_field_id_none_list_empty_nnl.
         """
-
         return e if getattr(x, g) is None else [getattr(x, f)]
 
     return c_field_id_none_list_empty_nnl
 
 
 callbacks.update(
     {
@@ -1530,15 +1494,14 @@
 NUMBER_OF_ITERATIONS = 1000000
 
 
 def benchmark(callbacks_to_benchmark):
     """
     Benchmark all the callbacks in the argument dict.
     """
-
     result = []
     for name, callback in callbacks_to_benchmark.items():
         time_with_fk = timeit.timeit(
             functools.partial(callback, instance_with_fk),
             number=NUMBER_OF_ITERATIONS,
         )
         time_without_fk = timeit.timeit(
```

### Comparing `django_monkey_patches-3.0.2/src/django_monkey_patches/django__base_cache__make_cache_key.py` & `django_monkey_patches-3.0.3/src/django_monkey_patches/django__base_cache__make_cache_key.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,28 +25,31 @@
 A collection of functions to make the key used by the cache.
 As of now, it is only for tests.
 """
 
 import os
 
 
-def make_test_cache_key(key, key_prefix, version):
+def get_test_cache_key(key, key_prefix, version):
     """
     Add a simple "test_cache" prefix.
 
     For example, apply it in your settings file with:
     # if len(sys.argv) > 1 and sys.argv[1] == "test":
     if TESTING:
         for cache in CACHES.values():
             cache["KEY_FUNCTION"] = make_test_cache_key
     """
     return f"test_cache:{key_prefix}:{version}:{key}"
 
 
-def make_parallel_test_cache_key(key, key_prefix, version):
+make_test_cache_key = get_test_cache_key
+
+
+def get_parallel_test_cache_key(key, key_prefix, version):
     """
     Add a simple "test_cache" prefix plus the current pid.
     The local memory cache is isolated between processes.
     But it may not be the case of a Redis backend cache, for example.
     https://stackoverflow.com/questions/71583690/
     It may seem inefficient to call os.getpid() here,
     but Django loads settings only once even when multiple processes
@@ -56,9 +59,11 @@
 
     For example, apply it in your settings file with:
     # if len(sys.argv) > 1 and sys.argv[1] == "test":
     if TESTING:
         for cache in CACHES.values():
             cache["KEY_FUNCTION"] = make_parallel_test_cache_key
     """
-
     return f"test_cache{os.getpid()}:{key_prefix}:{version}:{key}"
+
+
+make_parallel_test_cache_key = get_parallel_test_cache_key
```

### Comparing `django_monkey_patches-3.0.2/src/django_monkey_patches/django__orm__prefetch.py` & `django_monkey_patches-3.0.3/src/django_monkey_patches/django__orm__prefetch.py`

 * *Files 5% similar despite different names*

```diff
@@ -268,22 +268,24 @@
     if len(instances) == 0:
         return [], ()
     return old_prefetch_one_level(
         instances, prefetcher, lookup, level
     )
 
 
-def apply_patch_prefetch_with_filter_callback_v1():
+def apply_patch_prefetch_v1():
     """
     Applying the patch for prefetches on subsets of instances.
     """
     Prefetch.__init__ = patched_prefetch__init__v1
     query.prefetch_one_level = patched_prefetch_one_level_v1
 
 
+apply_patch_prefetch_with_filter_callback_v1 = apply_patch_prefetch_v1
+
 # Now things are starting to be amusing.
 # We load the source code of the function prefetch_related_objects()
 # in the installed version of Django and we patch its source code
 # with string manipulations.
 # First time for me in Python (not in PHP). :)
 # It works with Django 2.2 and Django 5.0,
 # probably also with versions in-between and after.
@@ -334,27 +336,30 @@
 exec(
     source,
     globals(),
     locals(),
 )
 
 
-def apply_patch_prefetch_with_v2():
+def apply_patch_prefetch_v2():
     """
     Applying the patch for prefetches with:
     - filter_callback,
     - post_prefetch_callback.
     """
     Prefetch.__init__ = patched_prefetch__init__v2
     query.prefetch_one_level = patched_prefetch_one_level_v1
     query.prefetch_related_objects = (
         patched_prefetch_related_objects_v1
     )
 
 
+apply_patch_prefetch_with_v2 = apply_patch_prefetch_v2
+
+
 def get_previous_prefetch_to(prefetch_to):
     """
     Going one step before in the order of prefetches.
     """
     if prefetch_to == "":
         raise ValueError(
             "get_previous_prefetch_to()"
@@ -455,15 +460,14 @@
     g = f + "_id"
 
     def retrieve_forward_cache_callback_for_foreign_key(x):
         """
         The customized retrieve_forward_cache_callback function
         that will be returned.
         """
-
         return e if getattr(x, g) is None else (getattr(x, f),)
 
     return retrieve_forward_cache_callback_for_foreign_key
 
 
 def create_retrieve_forward_cache_callback_for_prefetched_objects(
     c,  # cache_name
@@ -475,15 +479,14 @@
     """
 
     def retrieve_forward_cache_callback_for_prefetched_objects(x):
         """
         The customized retrieve_forward_cache_callback function
         that will be returned.
         """
-
         if not hasattr(x, "_prefetched_objects_cache"):
             return e
 
         # pylint: disable-next=protected-access
         return x._prefetched_objects_cache.get(c, e)
 
     return retrieve_forward_cache_callback_for_prefetched_objects
```

### Comparing `django_monkey_patches-3.0.2/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py` & `django_monkey_patches-3.0.3/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.2/src/django_monkey_patches/django__query_set.py` & `django_monkey_patches-3.0.3/src/django_monkey_patches/django__query_set.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.2/src/django_monkey_patches/django__query_set__get.py` & `django_monkey_patches-3.0.3/src/django_monkey_patches/django__query_set__get.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.2/src/django_monkey_patches/django__query_set__get_or_create.py` & `django_monkey_patches-3.0.3/src/django_monkey_patches/django__query_set__get_or_create.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.2/src/django_monkey_patches/django__query_wrapper.py` & `django_monkey_patches-3.0.3/src/django_monkey_patches/django__query_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,26 +98,24 @@
 
 
 def get_reference_pid():
     """
     A central function needed because Django connections can be shared
     between multiple processes.
     """
-
     return connections.django_monkey_patches_reference_pids.get(
         os.getpid(), os.getpid()
     )
 
 
 def get_connection_dict(connection):
     """
     Always use this method
     if you don't want compatibility problems later.
     """
-
     return connection.django_monkey_patches_dict.get(
         get_reference_pid()
     )
 
 
 def custom_query_wrapper_v1(execute, sql, params, many, context):
     """
@@ -164,15 +162,14 @@
                 # See at end of file to wrap all connections.
                 output = self.handle(*args, **options)
         ...
     And then, make all your commands inherit from CustomBaseCommand.
     You can go way further
     in this line of customization and monitoring.
     """
-
     if THROTTLE_QUERIES:
         time.sleep(QUERY_PENALTY_MILLISECONDS / 1000)
 
     call_stack = None
     if COMPUTE_CALL_STACK:
         call_stack = traceback.format_stack()
 
@@ -224,15 +221,14 @@
 
 # pylint: disable-next=unused-argument
 def get_full_query_v1(extra_data_dict, data):
     """
     An helper function to see the request
     as it will be transmitted to the DBMS.
     """
-
     connection = data["context"]["connection"]
     return connection.cursor().mogrify(data["sql"], data["params"])
 
 
 get_full_query_v1.field_name = "full_query_v1"
 
 
@@ -252,29 +248,27 @@
     But since our in-house framework was rarely using
     prepared statements,
     the code to obtain an "SQL signature" was different.
     All the code in this file is more general and flexible than
     what we had at Teliae when I was working there.
     But the ideas here both stem from my work at Teliae and Deleev.
     """
-
     return params_placeholders_regexp.sub("", data["sql"])
 
 
 get_sql_signature_v1.field_name = "sql_signature_v1"
 
 
 # pylint: disable-next=unused-argument
 def get_light_call_stack_v1(extra_data_dict, data):
     """
     An helper function to remove framework code from the call stack.
     Usually, you want to know where you generate a DB request
     in your own code.
     """
-
     return [
         line
         for line in data["call_stack"]
         if "site-packages/" not in line
     ]
 
 
@@ -283,27 +277,25 @@
 
 def get_managed_list(manager):
     """
     Smaller with auto-completion:
     get_managed_list(manager)
     [] if manager is None else manager.list()
     """
-
     if manager is None:
         return []
     return manager.list()
 
 
 def get_managed_dict(manager):
     """
     Smaller with auto-completion:
     get_managed_dict(manager)
     {} if manager is None else manager.dict()
     """
-
     if manager is None:
         return {}
     return manager.dict()
 
 
 # Unfortunately, there is no "inline" function or macro in Python.
 # Another strange fact, C has inline functions,
@@ -388,15 +380,14 @@
     without my code
     or eventually wrapping mines may be subject to interpretation.
     Basically, I think that if you use your own additional "fields"
     and your own callbacks to fill/use the "fields" below,
     you have no obligation at all.
     But it would be nice to contribute anyway.
     """
-
     if query_fields is None:
         query_fields = get_managed_list(manager)
     if subsets_extra_data is None:
         subsets_extra_data = get_managed_dict(manager)
     if allocated_subsets_extra_data is None:
         allocated_subsets_extra_data = get_managed_dict(manager)
     if allocated_subsets_key_callback is None:
@@ -517,40 +508,37 @@
 
 
 def get_connection_stack(connection):
     """
     Always use this method
     if you don't want compatibility problems later.
     """
-
     return connection.django_monkey_patches_stash_stack.get(
         get_reference_pid()
     )
 
 
 def is_globally_init():
     """
     Since Django connections are shared between processes
     in many cases,
     tell if these connections already have the dicts linked
     to this patch.
     """
-
     return hasattr(connections, "django_monkey_patches_dict")
 
 
 def is_locally_init():
     """
     Since Django connections are shared between processes
     in many cases,
     tell if these connections already have the dicts linked
     to this patch.
     And test if these dicts have values for the current reference_pid.
     """
-
     return (
         is_globally_init()
         and connections.django_monkey_patches_dict.get(
             get_reference_pid()
         )
         is not None
     )
@@ -561,15 +549,14 @@
     manager=None,
     empty_stash_stack=False,
 ):
     """
     You should call this function or a custom one
     before using the custom query wrapper.
     """
-
     if not is_globally_init():
         connections.django_monkey_patches_reference_pids = {}
         connections.django_monkey_patches_dict = {}
         connections.django_monkey_patches_stash_stack = {}
         for connection_key in connections:
             connection = connections[connection_key]
             connection.django_monkey_patches_reference_pids = {}
@@ -664,15 +651,14 @@
     end_time,
     duration,
 ):
     """
     The entry-point function to insert query data in relevant dicts.
     It should be your default POST_EXECUTION_CALLBACK.
     """
-
     all_dicts = [
         connections.django_monkey_patches_dict[get_reference_pid()],
         context["connection"].django_monkey_patches_dict[
             get_reference_pid()
         ],
     ]
     data = {
@@ -694,15 +680,14 @@
 
 # pylint: disable-next=too-many-branches
 def insert_in_extra_data_dict_v1(extra_data_dict, data):
     """
     The recursive function used to insert the data of a query
     in all relevant dicts.
     """
-
     # Filtering part -------------------------------------------------
     if data["duration"] is not None:
         # /!\ check list: you did activate TIME_QUERIES?
         if (
             extra_data_dict["min_seconds_threshold"]
             > data["duration"]
         ):
@@ -783,15 +768,14 @@
 
 
 def synthetize_connections_extra_data_v1():
     """
     The entry-point function to call synthetize_extra_data_dict_v1()
     on all root extra data dicts.
     """
-
     extra_data_dicts = [
         connections.django_monkey_patches_dict[get_reference_pid()]
     ]
     extra_data_dicts.extend(
         connections[connection_key].django_monkey_patches_dict[
             get_reference_pid()
         ]
@@ -802,15 +786,14 @@
 
 
 def synthetize_extra_data_dict_v1(extra_data_dict):
     """
     The recursive function used to synthetize
     the results at the end.
     """
-
     if extra_data_dict["query_count"] > 0:
         extra_data_dict["average_duration"] = (
             extra_data_dict["total_duration"]
             / extra_data_dict["query_count"]
         )
 
     # Top-down
@@ -839,15 +822,14 @@
 
 def reorder_dict_by_total_duration_of_sub_dicts(some_dict):
     """
     A common tool to visualize the result of profiling DB queries
     is to see at the top
     similar queries where most of the time is spent.
     """
-
     couples_list = list(some_dict.items())
     couples_list.sort(
         key=lambda x: x[1]["total_duration"],
         reverse=True,
     )
     return dict(couples_list)
 
@@ -855,15 +837,14 @@
 def apply_reorder_dict_by_total_duration_of_sub_dicts_to(
     main_dict,
     some_sub_dict_key,
 ):
     """
     This function simplifies use of the previous one.
     """
-
     main_dict[some_sub_dict_key] = (
         reorder_dict_by_total_duration_of_sub_dicts(
             main_dict[some_sub_dict_key]
         )
     )
 
 
@@ -874,30 +855,28 @@
 ):
     """
     Apply the context-manager connection.execute_wrapper()
     with the given custom_query_wrapper
     on an ExitStack() instance,
     for given connections or all connections if none is given.
     """
-
     if connections_to_wrap is None:
         connections_to_wrap = connections
     for connection_key in connections_to_wrap:
         connection = connections[connection_key]
         exit_stack.enter_context(
             connection.execute_wrapper(custom_query_wrapper)
         )
 
 
 def stash_extra_data_dicts(reinit_after_stash=None):
     """
     Stash current django_monkey_patches_dicts
     in django_monkey_patches_stash_stacks.
     """
-
     connections.django_monkey_patches_stash_stack[
         get_reference_pid()
     ].append(
         connections.django_monkey_patches_dict[get_reference_pid()]
     )
 
     if reinit_after_stash is None:
@@ -972,56 +951,56 @@
 
 
 def pop_extra_data_dicts():
     """
     Pop last dicts in django_monkey_patches_stash_stacks
     to django_monkey_patches_dicts.
     """
-
     connections.django_monkey_patches_dict[get_reference_pid()] = (
         connections.django_monkey_patches_stash_stack[
             get_reference_pid()
         ].pop()
     )
     for connection_key in connections:
         connection = connections[connection_key]
         connection.django_monkey_patches_dict[get_reference_pid()] = (
             connection.django_monkey_patches_stash_stack[
                 get_reference_pid()
             ].pop()
         )
 
 
-def patch_rq_v1():
+def apply_patch_rq_v1():
     """
     A function to apply a patch to rq needed to follow pids between
     parent and child processes in Django-rq.
     """
-
     # pylint: disable-next=import-error,import-outside-toplevel
     from rq.worker import Worker
 
     original_fork_work_horse = Worker.fork_work_horse
     original_main_work_horse = Worker.main_work_horse
 
-    def fork_work_horse(self, job, queue):
+    def patched_fork_work_horse(self, job, queue):
         job.reference_pid = os.getpid()
         return original_fork_work_horse(self, job, queue)
 
-    def main_work_horse(self, job, queue):
+    def patched_main_work_horse(self, job, queue):
         connections.django_monkey_patches_reference_pids[
             os.getpid()
         ] = job.reference_pid
         return original_main_work_horse(self, job, queue)
 
-    Worker.fork_work_horse = fork_work_horse
-    Worker.main_work_horse = main_work_horse
+    Worker.fork_work_horse = patched_fork_work_horse
+    Worker.main_work_horse = patched_main_work_horse
     return (original_fork_work_horse, original_main_work_horse)
 
 
+patch_rq_v1 = apply_patch_rq_v1
+
 # You should extract the data to logs or files,
 # during execution or at the end,
 # using custom insertion_callback or post_processing_callback.
 # Here is an example of intermediate complexity
 # using all of the above.
 #
 # from contextlib import ExitStack
```

### Comparing `django_monkey_patches-3.0.2/src/django_monkey_patches/django__test_case__tear_down.py` & `django_monkey_patches-3.0.3/src/django_monkey_patches/django__test_case__tear_down.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.2/src/django_monkey_patches/django_rest_framework__field__get_request.py` & `django_monkey_patches-3.0.3/src/django_monkey_patches/django_rest_framework__field__get_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,18 +100,20 @@
     """
     Enables still shorter code to access one request POST datum
     from serializer.
     """
     return self.get_request_POST().get(key, default)
 
 
-def apply_get_request_patch_v1():
+def apply_patch_field_get_request_v1():
     """
     Add to Field (and Serializer) all the shortcuts.
     """
-
     Field.get_request_query_params = get_request_query_params
     Field.get_request_data = get_request_data
     Field.get_request_POST = get_request_POST
     Field.get_one_request_query_param = get_one_request_query_param
     Field.get_one_request_datum = get_one_request_datum
     Field.get_one_request_POST_datum = get_one_request_POST_datum
+
+
+apply_get_request_patch_v1 = apply_patch_field_get_request_v1
```

### Comparing `django_monkey_patches-3.0.2/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py` & `django_monkey_patches-3.0.3/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.2/src/django_monkey_patches.egg-info/PKG-INFO` & `django_monkey_patches-3.0.3/src/django_monkey_patches.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.2/src/django_monkey_patches.egg-info/SOURCES.txt` & `django_monkey_patches-3.0.3/src/django_monkey_patches.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.2/COPYING` & `django_monkey_patches-3.0.3/COPYING`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.2/COPYING.LESSER` & `django_monkey_patches-3.0.3/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.2/README.md` & `django_monkey_patches-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.2/pyproject.toml` & `django_monkey_patches-3.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-monkey-patches"
-version = "3.0.2"
+version = "3.0.3"
 description = """\
 Add monkey-patches to correct and enhance your favorite framework\
 """
 readme = "README.md"
 authors = [
     { name = "Laurent Lyaudet", email = "laurent.lyaudet@gmail.com" },
 ]
```

### Comparing `django_monkey_patches-3.0.2/PKG-INFO` & `django_monkey_patches-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-monkey-patches
-Version: 3.0.2
+Version: 3.0.3
 Summary: Add monkey-patches to correct and enhance your favorite framework
 Project-URL: Homepage, https://github.com/LLyaudet/django-monkey-patches
 Project-URL: Bug Tracker, https://github.com/LLyaudet/django-monkey-patches/issues
 Author-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 Maintainer-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```


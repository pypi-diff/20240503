# Comparing `tmp/wood_nano-0.1.0-cp39-cp39-win_amd64.whl.zip` & `tmp/wood_nano-0.1.1-cp39-cp39-macosx_12_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 1857254 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat     1009 b- defN 24-May-02 22:25 wood_nano/__init__.py
--rw-rw-rw-  2.0 fat     3560 b- defN 24-May-02 22:25 wood_nano/conversions_python.py
--rw-rw-rw-  2.0 fat   543027 b- defN 24-May-02 22:25 wood_nano/libgmp-10.dll
--rw-rw-rw-  2.0 fat   436011 b- defN 24-May-02 22:25 wood_nano/libmpfr-4.dll
--rw-rw-rw-  2.0 fat  3232768 b- defN 24-May-02 22:25 wood_nano/wood_nano_ext.cp39-win_amd64.pyd
--rw-rw-r--  2.0 fat     7301 b- defN 24-May-02 22:25 wood_nano-0.1.0.dist-info/METADATA
--rw-rw-r--  2.0 fat      103 b- defN 24-May-02 22:25 wood_nano-0.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 fat     1547 b- defN 24-May-02 22:25 wood_nano-0.1.0.dist-info/licenses/LICENSE
--rw-rw-r--  2.0 fat      744 b- defN 24-May-02 22:25 wood_nano-0.1.0.dist-info/RECORD
-9 files, 4226070 bytes uncompressed, 1855990 bytes compressed:  56.1%
+Zip file size: 2180225 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      985 b- defN 24-May-02 23:23 wood_nano/__init__.py
+-rw-r--r--  2.0 unx     3439 b- defN 24-May-02 23:23 wood_nano/conversions_python.py
+-rw-r--r--  2.0 unx   543027 b- defN 24-May-02 23:23 wood_nano/libgmp-10.dll
+-rw-r--r--  2.0 unx   436011 b- defN 24-May-02 23:23 wood_nano/libmpfr-4.dll
+-rwxr-xr-x  2.0 unx  4110080 b- defN 24-May-02 23:23 wood_nano/wood_nano_ext.cpython-39-darwin.so
+-rw-rw-r--  2.0 unx     7301 b- defN 24-May-02 23:23 wood_nano-0.1.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx      112 b- defN 24-May-02 23:23 wood_nano-0.1.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     1521 b- defN 24-May-02 23:23 wood_nano-0.1.1.dist-info/licenses/LICENSE
+-rw-rw-r--  2.0 unx      745 b- defN 24-May-02 23:23 wood_nano-0.1.1.dist-info/RECORD
+9 files, 5103221 bytes uncompressed, 2178957 bytes compressed:  57.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: wood_nano/libgmp-10.dll
 Comment: 
 
 Filename: wood_nano/libmpfr-4.dll
 Comment: 
 
-Filename: wood_nano/wood_nano_ext.cp39-win_amd64.pyd
+Filename: wood_nano/wood_nano_ext.cpython-39-darwin.so
 Comment: 
 
-Filename: wood_nano-0.1.0.dist-info/METADATA
+Filename: wood_nano-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: wood_nano-0.1.0.dist-info/WHEEL
+Filename: wood_nano-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: wood_nano-0.1.0.dist-info/licenses/LICENSE
+Filename: wood_nano-0.1.1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: wood_nano-0.1.0.dist-info/RECORD
+Filename: wood_nano-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wood_nano/__init__.py

 * *Ordering differences only*

```diff
@@ -1,24 +1,24 @@
-from .wood_nano_ext import add
-from .wood_nano_ext import version
-from .wood_nano_ext import inspect
-from .wood_nano_ext import int1, int2, int3, int4
-from .wood_nano_ext import double1, double2, double3, double4
-from .wood_nano_ext import bool1
-from .wood_nano_ext import point, point1, point2, point3, point4
-from .wood_nano_ext import vector, vector1, vector2, vector3, vector4
-from .wood_nano_ext import middle_point
-from .wood_nano_ext import rtree
-from .wood_nano_ext import get_connection_zones
-from .wood_nano_ext import cut_type, cut_type1, cut_type2
-from .wood_nano_ext import test
-from .wood_nano_ext import read_xml_polylines
-from .wood_nano_ext import read_xml_polylines_and_properties
-from .wood_nano_ext import closed_mesh_from_polylines
-from .wood_nano_ext import joints
-from .wood_nano_ext import joint_parameters_and_types
-from .wood_nano_ext import mesh_boolean_difference_from_polylines
-from .wood_nano_ext import GLOBALS
-from .wood_nano_ext import beam_volumes
-
-
-
+from .wood_nano_ext import add
+from .wood_nano_ext import version
+from .wood_nano_ext import inspect
+from .wood_nano_ext import int1, int2, int3, int4
+from .wood_nano_ext import double1, double2, double3, double4
+from .wood_nano_ext import bool1
+from .wood_nano_ext import point, point1, point2, point3, point4
+from .wood_nano_ext import vector, vector1, vector2, vector3, vector4
+from .wood_nano_ext import middle_point
+from .wood_nano_ext import rtree
+from .wood_nano_ext import get_connection_zones
+from .wood_nano_ext import cut_type, cut_type1, cut_type2
+from .wood_nano_ext import test
+from .wood_nano_ext import read_xml_polylines
+from .wood_nano_ext import read_xml_polylines_and_properties
+from .wood_nano_ext import closed_mesh_from_polylines
+from .wood_nano_ext import joints
+from .wood_nano_ext import joint_parameters_and_types
+from .wood_nano_ext import mesh_boolean_difference_from_polylines
+from .wood_nano_ext import GLOBALS
+from .wood_nano_ext import beam_volumes
+
+
+
```

## wood_nano/conversions_python.py

 * *Ordering differences only*

```diff
@@ -1,121 +1,121 @@
-import wood_nano as m
-
-
-
-######################################################################################################
-# Conversion of integers
-######################################################################################################
-
-def to_int(vectors, depth):
-    if depth == 1:
-        vector = m.int1(vectors)
-    else:
-        vector = getattr(m, f'int{depth}')()
-        for vec in vectors:
-            vector.append(to_int(vec, depth - 1))
-    return vector
-
-def to_int1(vectors):
-    return to_int(vectors, 1)
-
-def to_int2(vectors):
-    return to_int(vectors, 2)
-
-def to_int3(vectors):
-    return to_int(vectors, 3)
-
-def to_int4(vectors):
-    return to_int(vectors, 4)
-
-def from_int1(int1):
-    return list(int1)
-
-def from_int2(int2):
-    return [from_int1(i) for i in int2]
-
-def from_int3(int3):
-    return [from_int2(i) for i in int3]
-
-def from_int4(int4):
-    return [from_int3(i) for i in int4]
-
-######################################################################################################
-# Conversion of doubles
-######################################################################################################
-
-def to_double(vectors, depth):
-    if depth == 1:
-        vector = m.double1(vectors)
-    else:
-        vector = getattr(m, f'double{depth}')()
-        for vec in vectors:
-            vector.append(to_double(vec, depth - 1))
-    return vector
-
-def to_double1(vectors):
-    return to_double(vectors, 1)
-
-def to_double2(vectors):
-    return to_double(vectors, 2)
-
-def to_double3(vectors):
-    return to_double(vectors, 3)
-
-def to_double4(vectors):
-    return to_double(vectors, 4)
-
-def from_double1(double1):
-    return list(double1)
-
-def from_double2(double2):
-    return [from_double1(d) for d in double2]
-
-def from_double3(double3):
-    return [from_double2(d) for d in double3]
-
-def from_double4(double4):
-    return [from_double3(d) for d in double4]
-
-######################################################################################################
-# Conversion of booleans
-######################################################################################################
-
-def to_bool1(vectors):
-    return m.bool1(vectors)
-
-def from_bool1(bool1):
-    return list(bool1)
-
-######################################################################################################
-# Conversion of strings
-######################################################################################################
-def to_string1(vectors):
-    return m.string1(vectors)
-
-def from_string1(string1):
-    return list(string1)
-
-######################################################################################################
-# Conversion functions for Enums
-######################################################################################################
-
-def enum_to_dict(enum_type):
-    dict = {}
-    enum_attributes = dir(enum_type)
-    for attribute in enum_attributes:
-        if not attribute.startswith('__') and not attribute.startswith('@'): 
-            value = getattr(enum_type, attribute)
-            dict[int(value)] = str(attribute)
-    return dict
-
-
-def from_cut_type(cut_type, enum_types):
-    cut_types = []
-    for i in range(len(cut_type)):
-        cut_types.append(enum_types[cut_type[i]])
-    return cut_types
-
-def from_cut_type2(cut_type2):
-    enum_types = enum_to_dict(m.cut_type)
-    return [from_cut_type(c, enum_types) for c in cut_type2]
-
+import wood_nano as m
+
+
+
+######################################################################################################
+# Conversion of integers
+######################################################################################################
+
+def to_int(vectors, depth):
+    if depth == 1:
+        vector = m.int1(vectors)
+    else:
+        vector = getattr(m, f'int{depth}')()
+        for vec in vectors:
+            vector.append(to_int(vec, depth - 1))
+    return vector
+
+def to_int1(vectors):
+    return to_int(vectors, 1)
+
+def to_int2(vectors):
+    return to_int(vectors, 2)
+
+def to_int3(vectors):
+    return to_int(vectors, 3)
+
+def to_int4(vectors):
+    return to_int(vectors, 4)
+
+def from_int1(int1):
+    return list(int1)
+
+def from_int2(int2):
+    return [from_int1(i) for i in int2]
+
+def from_int3(int3):
+    return [from_int2(i) for i in int3]
+
+def from_int4(int4):
+    return [from_int3(i) for i in int4]
+
+######################################################################################################
+# Conversion of doubles
+######################################################################################################
+
+def to_double(vectors, depth):
+    if depth == 1:
+        vector = m.double1(vectors)
+    else:
+        vector = getattr(m, f'double{depth}')()
+        for vec in vectors:
+            vector.append(to_double(vec, depth - 1))
+    return vector
+
+def to_double1(vectors):
+    return to_double(vectors, 1)
+
+def to_double2(vectors):
+    return to_double(vectors, 2)
+
+def to_double3(vectors):
+    return to_double(vectors, 3)
+
+def to_double4(vectors):
+    return to_double(vectors, 4)
+
+def from_double1(double1):
+    return list(double1)
+
+def from_double2(double2):
+    return [from_double1(d) for d in double2]
+
+def from_double3(double3):
+    return [from_double2(d) for d in double3]
+
+def from_double4(double4):
+    return [from_double3(d) for d in double4]
+
+######################################################################################################
+# Conversion of booleans
+######################################################################################################
+
+def to_bool1(vectors):
+    return m.bool1(vectors)
+
+def from_bool1(bool1):
+    return list(bool1)
+
+######################################################################################################
+# Conversion of strings
+######################################################################################################
+def to_string1(vectors):
+    return m.string1(vectors)
+
+def from_string1(string1):
+    return list(string1)
+
+######################################################################################################
+# Conversion functions for Enums
+######################################################################################################
+
+def enum_to_dict(enum_type):
+    dict = {}
+    enum_attributes = dir(enum_type)
+    for attribute in enum_attributes:
+        if not attribute.startswith('__') and not attribute.startswith('@'): 
+            value = getattr(enum_type, attribute)
+            dict[int(value)] = str(attribute)
+    return dict
+
+
+def from_cut_type(cut_type, enum_types):
+    cut_types = []
+    for i in range(len(cut_type)):
+        cut_types.append(enum_types[cut_type[i]])
+    return cut_types
+
+def from_cut_type2(cut_type2):
+    enum_types = enum_to_dict(m.cut_type)
+    return [from_cut_type(c, enum_types) for c in cut_type2]
+
```

## Comparing `wood_nano-0.1.0.dist-info/METADATA` & `wood_nano-0.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wood-nano
-Version: 0.1.0
+Version: 0.1.1
 Summary: Binding for wood project that  is compiled into a binding using nanobind and scikit-build
 Author-Email: Petras Vestartas <petrasvestartas@gmail.com>
 Classifier: License :: OSI Approved :: BSD License
 Project-URL: Homepage, https://github.com/petrasvestartas/wood_nano
 Requires-Python: >=3.8.16
 Description-Content-Type: text/markdown
```


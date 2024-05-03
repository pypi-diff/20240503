# Comparing `tmp/custom_cytomine_client-0.1.0.tar.gz` & `tmp/custom_cytomine_client-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_cytomine_client-0.1.0.tar", max compression
+gzip compressed data, was "custom_cytomine_client-0.1.0a0.tar", max compression
```

## Comparing `custom_cytomine_client-0.1.0.tar` & `custom_cytomine_client-0.1.0a0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       71 2024-05-03 06:34:10.409973 custom_cytomine_client-0.1.0/README.md
--rw-r--r--   0        0        0       76 2024-05-03 00:53:11.175071 custom_cytomine_client-0.1.0/custom_cytomine_client/__init__.py
--rw-r--r--   0        0        0     9624 2024-05-03 06:34:10.458657 custom_cytomine_client-0.1.0/custom_cytomine_client/converter.py
--rw-r--r--   0        0        0        0 2024-05-03 00:53:11.175335 custom_cytomine_client-0.1.0/custom_cytomine_client/interface/__init__.py
--rw-r--r--   0        0        0      789 2024-05-03 06:34:10.407971 custom_cytomine_client-0.1.0/custom_cytomine_client/interface/converter.py
--rw-r--r--   0        0        0        0 2024-05-03 00:53:11.175524 custom_cytomine_client-0.1.0/custom_cytomine_client/object/__init__.py
--rw-r--r--   0        0        0      676 2024-05-03 00:53:11.175618 custom_cytomine_client-0.1.0/custom_cytomine_client/object/converter.py
--rw-r--r--   0        0        0        0 2024-05-03 00:53:11.175686 custom_cytomine_client-0.1.0/custom_cytomine_client/util/__init__.py
--rw-r--r--   0        0        0      225 2024-05-03 00:53:11.175766 custom_cytomine_client-0.1.0/custom_cytomine_client/util/custom_exception.py
--rw-r--r--   0        0        0     3137 2024-05-03 06:34:10.428392 custom_cytomine_client-0.1.0/custom_cytomine_client/util/fit_util.py
--rw-r--r--   0        0        0      485 2024-05-03 00:53:11.175942 custom_cytomine_client-0.1.0/custom_cytomine_client/util/normal_util.py
--rw-r--r--   0        0        0      726 2024-05-03 06:34:43.713807 custom_cytomine_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1203 1970-01-01 00:00:00.000000 custom_cytomine_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       71 2024-05-03 06:34:10.409973 custom_cytomine_client-0.1.0a0/README.md
+-rw-r--r--   0        0        0       76 2024-05-03 00:53:11.175071 custom_cytomine_client-0.1.0a0/custom_cytomine_client/__init__.py
+-rw-r--r--   0        0        0    10120 2024-05-03 07:22:34.611117 custom_cytomine_client-0.1.0a0/custom_cytomine_client/converter.py
+-rw-r--r--   0        0        0        0 2024-05-03 00:53:11.175335 custom_cytomine_client-0.1.0a0/custom_cytomine_client/interface/__init__.py
+-rw-r--r--   0        0        0      789 2024-05-03 06:34:10.407971 custom_cytomine_client-0.1.0a0/custom_cytomine_client/interface/converter.py
+-rw-r--r--   0        0        0        0 2024-05-03 00:53:11.175524 custom_cytomine_client-0.1.0a0/custom_cytomine_client/object/__init__.py
+-rw-r--r--   0        0        0      676 2024-05-03 00:53:11.175618 custom_cytomine_client-0.1.0a0/custom_cytomine_client/object/converter.py
+-rw-r--r--   0        0        0        0 2024-05-03 00:53:11.175686 custom_cytomine_client-0.1.0a0/custom_cytomine_client/util/__init__.py
+-rw-r--r--   0        0        0      225 2024-05-03 00:53:11.175766 custom_cytomine_client-0.1.0a0/custom_cytomine_client/util/custom_exception.py
+-rw-r--r--   0        0        0     3137 2024-05-03 06:34:10.428392 custom_cytomine_client-0.1.0a0/custom_cytomine_client/util/fit_util.py
+-rw-r--r--   0        0        0      485 2024-05-03 00:53:11.175942 custom_cytomine_client-0.1.0a0/custom_cytomine_client/util/normal_util.py
+-rw-r--r--   0        0        0      728 2024-05-03 07:23:08.678331 custom_cytomine_client-0.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0     1205 1970-01-01 00:00:00.000000 custom_cytomine_client-0.1.0a0/PKG-INFO
```

### Comparing `custom_cytomine_client-0.1.0/custom_cytomine_client/converter.py` & `custom_cytomine_client-0.1.0a0/custom_cytomine_client/converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -230,14 +230,21 @@
                     "class": class_name,
                     "type": "polygon",
                 }
                 annotation_elem = ET.SubElement(annotations_elem, "Annotation", annotation_attributes)
                 coordinates_elem = ET.SubElement(annotation_elem, "Coordinates")
 
                 # 좌표 요소들 추가
-                for x, y in wkt.loads(annotation.location).exterior.coords:
-                    ET.SubElement(coordinates_elem, "Coordinate", x=str(x), y=str(y))
+                try:
+                    for x, y in wkt.loads(annotation.location).exterior.coords:
+                        ET.SubElement(coordinates_elem, "Coordinate", x=str(x), y=str(y))
+                except Exception as e:
+                    for polygon in wkt.loads(annotation.location).geoms:
+                        annotation_elem = ET.SubElement(annotations_elem, "Annotation", annotation_attributes)
+                        coordinates_elem = ET.SubElement(annotation_elem, "Coordinates")
+                        for x, y in polygon.exterior.coords:
+                            ET.SubElement(coordinates_elem, "Coordinate", x=str(x), y=str(y))
 
             # XML 트리를 문자열로 변환
             ET.indent(root)
             tree = ET.ElementTree(root)
             tree.write(f"{save_path}/{image_name.replace('.jpg', '')}.xml")
```

### Comparing `custom_cytomine_client-0.1.0/custom_cytomine_client/interface/converter.py` & `custom_cytomine_client-0.1.0a0/custom_cytomine_client/interface/converter.py`

 * *Files identical despite different names*

### Comparing `custom_cytomine_client-0.1.0/custom_cytomine_client/object/converter.py` & `custom_cytomine_client-0.1.0a0/custom_cytomine_client/object/converter.py`

 * *Files identical despite different names*

### Comparing `custom_cytomine_client-0.1.0/custom_cytomine_client/util/fit_util.py` & `custom_cytomine_client-0.1.0a0/custom_cytomine_client/util/fit_util.py`

 * *Files identical despite different names*

### Comparing `custom_cytomine_client-0.1.0/pyproject.toml` & `custom_cytomine_client-0.1.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "custom-cytomine-client"
-version = "0.1.0"
+version = "0.1.00a"
 description = "Custom Cytomine client for Python"
 authors = ["punrabbit <tjdmsch2201@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 annotated-types = "0.6.0"
```

### Comparing `custom_cytomine_client-0.1.0/PKG-INFO` & `custom_cytomine_client-0.1.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-cytomine-client
-Version: 0.1.0
+Version: 0.1.0a0
 Summary: Custom Cytomine client for Python
 Author: punrabbit
 Author-email: tjdmsch2201@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


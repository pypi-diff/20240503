# Comparing `tmp/custom_cytomine_client-0.0.9.tar.gz` & `tmp/custom_cytomine_client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_cytomine_client-0.0.9.tar", max compression
+gzip compressed data, was "custom_cytomine_client-0.1.0.tar", max compression
```

## Comparing `custom_cytomine_client-0.0.9.tar` & `custom_cytomine_client-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       70 2024-04-03 09:00:43.689977 custom_cytomine_client-0.0.9/README.md
--rw-r--r--   0        0        0      124 2024-04-04 08:28:30.381656 custom_cytomine_client-0.0.9/custom_cytomine_client/__init__.py
--rw-r--r--   0        0        0     7084 2024-04-04 08:21:59.692699 custom_cytomine_client-0.0.9/custom_cytomine_client/converter.py
--rw-r--r--   0        0        0        0 2024-04-04 08:21:59.692773 custom_cytomine_client-0.0.9/custom_cytomine_client/interface/__init__.py
--rw-r--r--   0        0        0      667 2024-04-04 08:21:59.692900 custom_cytomine_client-0.0.9/custom_cytomine_client/interface/converter.py
--rw-r--r--   0        0        0        0 2024-04-04 08:21:59.693022 custom_cytomine_client-0.0.9/custom_cytomine_client/object/__init__.py
--rw-r--r--   0        0        0      594 2024-04-04 08:21:59.693147 custom_cytomine_client-0.0.9/custom_cytomine_client/object/converter.py
--rw-r--r--   0        0        0        0 2024-04-04 08:21:59.693627 custom_cytomine_client-0.0.9/custom_cytomine_client/util/__init__.py
--rw-r--r--   0        0        0      225 2024-04-02 08:34:59.565119 custom_cytomine_client-0.0.9/custom_cytomine_client/util/custom_exception.py
--rw-r--r--   0        0        0     2220 2024-04-04 08:21:59.693785 custom_cytomine_client-0.0.9/custom_cytomine_client/util/fit_util.py
--rw-r--r--   0        0        0      485 2024-04-02 07:41:42.188210 custom_cytomine_client-0.0.9/custom_cytomine_client/util/normal_util.py
--rw-r--r--   0        0        0      726 2024-04-04 08:28:34.704166 custom_cytomine_client-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 custom_cytomine_client-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0       71 2024-05-03 06:34:10.409973 custom_cytomine_client-0.1.0/README.md
+-rw-r--r--   0        0        0       76 2024-05-03 00:53:11.175071 custom_cytomine_client-0.1.0/custom_cytomine_client/__init__.py
+-rw-r--r--   0        0        0     9624 2024-05-03 06:34:10.458657 custom_cytomine_client-0.1.0/custom_cytomine_client/converter.py
+-rw-r--r--   0        0        0        0 2024-05-03 00:53:11.175335 custom_cytomine_client-0.1.0/custom_cytomine_client/interface/__init__.py
+-rw-r--r--   0        0        0      789 2024-05-03 06:34:10.407971 custom_cytomine_client-0.1.0/custom_cytomine_client/interface/converter.py
+-rw-r--r--   0        0        0        0 2024-05-03 00:53:11.175524 custom_cytomine_client-0.1.0/custom_cytomine_client/object/__init__.py
+-rw-r--r--   0        0        0      676 2024-05-03 00:53:11.175618 custom_cytomine_client-0.1.0/custom_cytomine_client/object/converter.py
+-rw-r--r--   0        0        0        0 2024-05-03 00:53:11.175686 custom_cytomine_client-0.1.0/custom_cytomine_client/util/__init__.py
+-rw-r--r--   0        0        0      225 2024-05-03 00:53:11.175766 custom_cytomine_client-0.1.0/custom_cytomine_client/util/custom_exception.py
+-rw-r--r--   0        0        0     3137 2024-05-03 06:34:10.428392 custom_cytomine_client-0.1.0/custom_cytomine_client/util/fit_util.py
+-rw-r--r--   0        0        0      485 2024-05-03 00:53:11.175942 custom_cytomine_client-0.1.0/custom_cytomine_client/util/normal_util.py
+-rw-r--r--   0        0        0      726 2024-05-03 06:34:43.713807 custom_cytomine_client-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1203 1970-01-01 00:00:00.000000 custom_cytomine_client-0.1.0/PKG-INFO
```

### Comparing `custom_cytomine_client-0.0.9/custom_cytomine_client/converter.py` & `custom_cytomine_client-0.1.0/custom_cytomine_client/converter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,33 @@
+import xml.etree.ElementTree as ET
 from cytomine import Cytomine
 from cytomine.models import (
     ImageInstanceCollection,
     Term,
     OntologyCollection,
     ProjectCollection,
     TermCollection,
     Annotation,
     AnnotationTerm,
+    AnnotationCollection,
 )
 from typing import List, Union, Optional
+from shapely import wkt
 from overrides import override
 
-from interface.converter import CustomCytomineClientInterface
-from util.normal_util import NormalUtil
-from util.fit_util import FitUtil
-from util.custom_exception import XMLImageNameNotFoundError
-from object.converter import (
+from .interface.converter import CustomCytomineClientInterface
+from .util.normal_util import NormalUtil
+from .util.fit_util import FitUtil
+from .util.custom_exception import XMLImageNameNotFoundError
+from .object.converter import (
     CytomineAnnotationInfo,
     CytomineTermInfo,
     CytomineImageInfo,
     CytomineProjectInfo,
+    PolygonClassMatchingInfo,
 )
 
 
 class CustomCytomineClient(CustomCytomineClientInterface):
     def __init__(
         self,
         host: str,
@@ -80,15 +84,20 @@
                 image_info: CytomineImageInfo = self._find_image_info_by_name(
                     project_name, cytomine_metric.image_name
                 )
             except XMLImageNameNotFoundError:
                 image_info: CytomineImageInfo = self._find_image_info_by_name(project_name, file_name)
 
             for annotation_info in cytomine_metric.annotation_infos:
-                self._save_annotation(image_info.image_id, annotation_info, project_name, image_info.height)
+                self._save_annotation(
+                    image_info.image_id,
+                    annotation_info,
+                    project_name,
+                    image_info.height,
+                )
         return True
 
     @override
     def find_project_info_with_name(self, name: str) -> CytomineProjectInfo:
         with self._connect_cytomine():
             ontologies: list = OntologyCollection().fetch()
             projects: list = ProjectCollection().fetch()
@@ -100,14 +109,34 @@
             )
 
             if ontology_id is None or project_id is None:
                 raise Exception("해당 이름을 가진 프로젝트가 없습니다.")
 
             return CytomineProjectInfo(project_id=project_id, ontology_id=ontology_id)
 
+    @override
+    def save_xml_files_from_project(self, save_path: str, project_name: str) -> None:
+        with self._connect_cytomine():
+            projects = ProjectCollection().fetch()
+            project = next((proj for proj in projects if proj.name == project_name), None)
+
+            images = ImageInstanceCollection().fetch_with_filter("project", project.id)
+
+            for img in images:
+                annotations = AnnotationCollection(
+                    image=img.id,
+                    showWKT=True,
+                    showMeta=True,
+                    showGIS=True,
+                    showTerm=True,
+                ).fetch()
+
+                self._create_annotation_xml(annotations, img.instanceFilename, save_path=save_path)
+        return None
+
     def _find_image_names_in_project(self, project_name: str) -> List[CytomineImageInfo]:
         with self._connect_cytomine():
             project_info: CytomineProjectInfo = self.find_project_info_with_name(name=project_name)
             images: list = ImageInstanceCollection().fetch_with_filter("project", project_info.project_id)
             return [
                 CytomineImageInfo(
                     image_id=image.id,
@@ -170,7 +199,45 @@
                 if info.image_name.rsplit(".", 1)[0] == image_name.rsplit(".", 1)[0]
             ),
             None,
         )
         if not image_info:
             raise XMLImageNameNotFoundError(msg=f"{image_name} / {image_infos}")
         return image_info
+
+    @classmethod
+    def _create_annotation_xml(cls, annotations, image_name, save_path: str) -> None:
+        root = ET.Element("object-stream")
+        annotations_elem = ET.SubElement(root, "Annotations", image=image_name)
+
+        for annotation in annotations:
+
+            class_names: list = []
+            decimal_colors: list = []
+
+            if not annotation.term:
+                class_names.append("")
+                decimal_colors.append("15886723")
+            else:
+                for term in annotation.term:
+                    term_info = Term().fetch(id=term)
+                    class_names.append(term_info.name)
+                    decimal_colors.append(str(int(term_info.color[1:], 16)))
+
+            for class_name, color in zip(class_names, decimal_colors):
+
+                annotation_attributes = {
+                    "color": color,
+                    "class": class_name,
+                    "type": "polygon",
+                }
+                annotation_elem = ET.SubElement(annotations_elem, "Annotation", annotation_attributes)
+                coordinates_elem = ET.SubElement(annotation_elem, "Coordinates")
+
+                # 좌표 요소들 추가
+                for x, y in wkt.loads(annotation.location).exterior.coords:
+                    ET.SubElement(coordinates_elem, "Coordinate", x=str(x), y=str(y))
+
+            # XML 트리를 문자열로 변환
+            ET.indent(root)
+            tree = ET.ElementTree(root)
+            tree.write(f"{save_path}/{image_name.replace('.jpg', '')}.xml")
```

### Comparing `custom_cytomine_client-0.0.9/custom_cytomine_client/interface/converter.py` & `custom_cytomine_client-0.1.0/custom_cytomine_client/interface/converter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABCMeta, abstractmethod
 from typing import List
 
-from object.converter import CytomineProjectInfo, CytomineTermInfo
+from ..object.converter import CytomineProjectInfo, CytomineTermInfo
 
 
 class CustomCytomineClientInterface(metaclass=ABCMeta):
     @abstractmethod
     def save_annotation_from_xml(self, xml_path: str, project_name: str) -> bool:
         pass
 
@@ -16,7 +16,11 @@
     @abstractmethod
     def find_project_info_with_name(self, name: str) -> CytomineProjectInfo:
         pass
 
     @abstractmethod
     def find_terms_info_with_project_name(self, project_name: str) -> List[CytomineTermInfo]:
         pass
+
+    @abstractmethod
+    def save_xml_files_from_project(self, save_path: str, project_name: str) -> None:
+        pass
```

### Comparing `custom_cytomine_client-0.0.9/custom_cytomine_client/object/converter.py` & `custom_cytomine_client-0.1.0/custom_cytomine_client/object/converter.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,7 +27,12 @@
     image_id: int
     height: int
 
 
 class CytomineProjectInfo(BaseModel):
     project_id: int
     ontology_id: int
+
+
+class PolygonClassMatchingInfo(BaseModel):
+    class_name: str
+    polygon: str
```

### Comparing `custom_cytomine_client-0.0.9/custom_cytomine_client/util/fit_util.py` & `custom_cytomine_client-0.1.0/custom_cytomine_client/util/fit_util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, Any, List
 
-from object.converter import CytomineAnnotationInfo
+from ..object.converter import CytomineAnnotationInfo, PolygonClassMatchingInfo
 
 
 class FitUtil:
     @classmethod
     def parse_xml_to_cytomine_annotation_info(cls, xml_dict_data: Dict[str, Any]) -> CytomineAnnotationInfo:
         annotations_data = xml_dict_data["object-stream"]["Annotations"]
         image_name = annotations_data["@image"]
@@ -45,7 +45,29 @@
     @classmethod
     def make_polygon_info_to_cytomine_polygon_metric(
         cls,
         polygon_info: List[CytomineAnnotationInfo.AnnotationInfo.PolygonInfo],
         image_height: int,
     ) -> str:
         return "POLYGON((" + ", ".join(f"{point.x} {image_height - point.y}" for point in polygon_info) + "))"
+
+    @classmethod
+    def parse_cytomine_annotation_string_to_data_model(
+        cls, polygon_info: List[PolygonClassMatchingInfo], image_name: str
+    ) -> CytomineAnnotationInfo:
+        cytomine_annotation_info: CytomineAnnotationInfo = CytomineAnnotationInfo(
+            image_name=image_name,
+            annotation_infos=[
+                CytomineAnnotationInfo.AnnotationInfo(
+                    class_name="ExampleClass",
+                    polygon_points=[
+                        CytomineAnnotationInfo.AnnotationInfo.PolygonInfo(
+                            x=float(pair.split()[0]), y=float(pair.split()[1])
+                        )
+                        for pair in info.polygon.split("((")[1].split("))")[0].split(", ")
+                    ],
+                )
+                for info in polygon_info
+            ],
+        )
+
+        return cytomine_annotation_info
```

### Comparing `custom_cytomine_client-0.0.9/pyproject.toml` & `custom_cytomine_client-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "custom-cytomine-client"
-version = "0.0.9"
+version = "0.1.0"
 description = "Custom Cytomine client for Python"
 authors = ["punrabbit <tjdmsch2201@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 annotated-types = "0.6.0"
```

### Comparing `custom_cytomine_client-0.0.9/PKG-INFO` & `custom_cytomine_client-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-cytomine-client
-Version: 0.0.9
+Version: 0.1.0
 Summary: Custom Cytomine client for Python
 Author: punrabbit
 Author-email: tjdmsch2201@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -29,7 +29,8 @@
 Requires-Dist: typing-extensions (==4.10.0)
 Requires-Dist: xmltodict (==0.13.0)
 Description-Content-Type: text/markdown
 
 # Custom Cytomine Client
 
 ## It works only with fit custom xml format.
+
```


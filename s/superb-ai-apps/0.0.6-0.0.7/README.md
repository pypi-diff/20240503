# Comparing `tmp/superb-ai-apps-0.0.6.tar.gz` & `tmp/superb-ai-apps-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superb-ai-apps-0.0.6.tar", last modified: Tue Apr 30 08:01:43 2024, max compression
+gzip compressed data, was "superb-ai-apps-0.0.7.tar", last modified: Fri May  3 06:52:04 2024, max compression
```

## Comparing `superb-ai-apps-0.0.6.tar` & `superb-ai-apps-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:43.627031 superb-ai-apps-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-30 08:01:43.627031 superb-ai-apps-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 08:01:43.627031 superb-ai-apps-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:43.623031 superb-ai-apps-0.0.6/spb_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/spb_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/spb_apps/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:43.623031 superb-ai-apps-0.0.6/spb_apps/curate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/spb_apps/curate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/spb_apps/curate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:43.623031 superb-ai-apps-0.0.6/spb_apps/label/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/spb_apps/label/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11965 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/spb_apps/superb_curate.py
--rw-r--r--   0 runner    (1001) docker     (127)    13570 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/spb_apps/superb_label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:43.623031 superb-ai-apps-0.0.6/spb_apps/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/spb_apps/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/spb_apps/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/spb_apps/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:43.623031 superb-ai-apps-0.0.6/superb_ai_apps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-30 08:01:43.000000 superb-ai-apps-0.0.6/superb_ai_apps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-30 08:01:43.000000 superb-ai-apps-0.0.6/superb_ai_apps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:01:43.000000 superb-ai-apps-0.0.6/superb_ai_apps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-30 08:01:43.000000 superb-ai-apps-0.0.6/superb_ai_apps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 08:01:43.000000 superb-ai-apps-0.0.6/superb_ai_apps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:52:04.458516 superb-ai-apps-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-03 06:52:04.458516 superb-ai-apps-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 06:51:27.000000 superb-ai-apps-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 06:52:04.458516 superb-ai-apps-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-03 06:51:27.000000 superb-ai-apps-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:52:04.454516 superb-ai-apps-0.0.7/spb_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 06:51:27.000000 superb-ai-apps-0.0.7/spb_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-03 06:51:27.000000 superb-ai-apps-0.0.7/spb_apps/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:52:04.454516 superb-ai-apps-0.0.7/spb_apps/curate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 06:51:27.000000 superb-ai-apps-0.0.7/spb_apps/curate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 06:51:27.000000 superb-ai-apps-0.0.7/spb_apps/curate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:52:04.454516 superb-ai-apps-0.0.7/spb_apps/label/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 06:51:27.000000 superb-ai-apps-0.0.7/spb_apps/label/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11965 2024-05-03 06:51:27.000000 superb-ai-apps-0.0.7/spb_apps/superb_curate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17673 2024-05-03 06:51:27.000000 superb-ai-apps-0.0.7/spb_apps/superb_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:52:04.458516 superb-ai-apps-0.0.7/spb_apps/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 06:51:27.000000 superb-ai-apps-0.0.7/spb_apps/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-03 06:51:27.000000 superb-ai-apps-0.0.7/spb_apps/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-05-03 06:51:27.000000 superb-ai-apps-0.0.7/spb_apps/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:52:04.458516 superb-ai-apps-0.0.7/superb_ai_apps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-03 06:52:04.000000 superb-ai-apps-0.0.7/superb_ai_apps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-03 06:52:04.000000 superb-ai-apps-0.0.7/superb_ai_apps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 06:52:04.000000 superb-ai-apps-0.0.7/superb_ai_apps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-03 06:52:04.000000 superb-ai-apps-0.0.7/superb_ai_apps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 06:52:04.000000 superb-ai-apps-0.0.7/superb_ai_apps.egg-info/top_level.txt
```

### Comparing `superb-ai-apps-0.0.6/setup.py` & `superb-ai-apps-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="superb-ai-apps",
-    version="0.0.6",
+    version="0.0.7",
     description="Python Package for Superb-AI Apps",
     install_requires=[
         "asttokens==2.4.1",
         "attrs==23.2.0",
         "backcall==0.2.0",
         "beautifulsoup4==4.12.3",
         "bleach==6.1.0",
@@ -59,15 +59,15 @@
         "referencing==0.34.0",
         "requests==2.31.0",
         "rpds-py==0.18.0",
         "semver==3.0.2",
         "six==1.16.0",
         "soupsieve==2.5",
         "stack-data==0.6.3",
-        "superb-ai-curate==1.2.1",
+        "superb-ai-curate==1.2.2",
         "superb-ai-label==0.21.2",
         "tinycss2==1.2.1",
         "tornado==6.4",
         "traitlets==5.14.2",
         "typing_extensions==4.10.0",
         "urllib3==2.2.1",
         "wcwidth==0.2.13",
```

### Comparing `superb-ai-apps-0.0.6/spb_apps/apps.py` & `superb-ai-apps-0.0.7/spb_apps/apps.py`

 * *Files identical despite different names*

### Comparing `superb-ai-apps-0.0.6/spb_apps/superb_curate.py` & `superb-ai-apps-0.0.7/spb_apps/superb_curate.py`

 * *Files identical despite different names*

### Comparing `superb-ai-apps-0.0.6/spb_apps/superb_label.py` & `superb-ai-apps-0.0.7/spb_apps/superb_label.py`

 * *Files 18% similar despite different names*

```diff
@@ -48,20 +48,36 @@
         - access_key (str): The access key for authentication.
         - project_id (str, optional): The ID of the project to be set for the client. Defaults to an empty string.
         - project_name (str, optional): The name of the project. Defaults to an empty string.
         """
         self.team_name: str = team_name
         self.access_key: str = access_key
         super().__init__(team_name, access_key)
-        self.client = spb_label.Client(
-            team_name=team_name,
-            access_key=access_key,
-            project_id=project_id if project_id else None,
-            project_name=project_name if project_name else None,
-        )
+        try:
+            self.client = spb_label.Client(
+                team_name=team_name,
+                access_key=access_key,
+                project_id=project_id if project_id else None,
+                project_name=project_name if project_name else None,
+            )
+        except spb_label.exceptions.NotFoundException as e:
+            print(f"[INFO]: Project not found, creating a new Image project")
+            self.client = spb_label.Client(
+                team_name=team_name,
+                access_key=access_key,
+            )
+            image_label_interface = (
+                phy_credit.imageV2.LabelInterface.get_default()
+            )
+            self.client.create_project(
+                name=project_name,
+                label_interface=image_label_interface.to_dict(),
+                description="Created from Superb Apps",
+            )
+            self.client.set_project(name=project_name)
 
     def change_project(self, project_name: str):
         """
         Changes the project context for the label client.
 
         Parameters:
             project_name (str): The name of the project to switch to.
@@ -244,25 +260,85 @@
                     "height": annotation[3],
                 }
             },
         }
 
         return bbox
 
-    def upload_images(self, image_paths: list, dataset_name: str):
+    def upload_image(
+        self,
+        image_path: str,
+        dataset_name: str,
+        data_key: str = None,
+        ignore: bool = False,
+    ):
         """
-        Upload images to a specified dataset.
+        Upload an image to a specified dataset. If the 'ignore' flag is set to True, the image will be uploaded without checking for existing entries.
+        If 'ignore' is False, it checks if the image already exists using the provided 'data_key' or derives a key from the image path.
+
+        Parameters:
+        - image_path (str): The path to the image to be uploaded.
+        - dataset_name (str): The name of the dataset to upload the image to.
+        - data_key (str, optional): The unique identifier for the image. If not provided, it is derived from the image path.
+        - ignore (bool, optional): If set to True, the image will be uploaded without checking for existing entries. Defaults to False.
+
+        Raises:
+        - ParameterException: If the upload fails due to incorrect parameters.
+        """
+        if ignore:
+            try:
+                self.client.upload_image(
+                    path=image_path,
+                    dataset_name=dataset_name,
+                )
+            except ParameterException as e:
+                print(f"[ERROR]: Uploading went wrong: {e}")
+        else:
+            if data_key is None:
+                key = image_path.split("/")[-1]
+                count, labels = self.get_labels(data_key=key)
+            else:
+                count, labels = self.get_labels(data_key=data_key)
+                key = data_key
+
+            if count == 0:
+                # try:
+                call_with_retry(
+                    fn=self.client.upload_image,
+                    path=image_path,
+                    dataset_name=dataset_name,
+                    key=data_key,
+                )
+                # except ParameterException as e:
+                #     print(f"[ERROR]: Uploading went wrong: {e}")
+
+            else:
+                print(
+                    f"[INFO]: Image already exists, skipping upload for data key {key}"
+                )
+
+    def upload_images(
+        self, image_paths: list, dataset_name: str, ignore: bool = False
+    ):
+        """
+        Upload multiple images to a specified dataset. This function iterates over a list of image paths and uploads each using the 'upload_image' method.
 
         Parameters:
         - image_paths (list): A list of paths to the images to be uploaded.
         - dataset_name (str): The name of the dataset to upload the images to.
+        - ignore (bool, optional): If set to True, the images will be uploaded without checking for existing entries. Defaults to False.
+
+        Raises:
+        - ParameterException: If the upload fails due to incorrect parameters.
         """
         for path in image_paths:
             try:
-                self.client.upload_image(path, dataset_name)
+                self.upload_image(
+                    image_path=path, dataset_name=dataset_name, ignore=ignore
+                )
             except ParameterException as e:
                 print(f"[ERROR]: Uploading went wrong: {e}")
 
     def upload_annotation(
         self,
         label: spb_label.DataHandle,
         annotations: list,
@@ -308,61 +384,79 @@
                 call_with_retry(
                     fn=label.add_object_label,
                     class_name=bbox["class_name"],
                     annotation=bbox["annotation"],
                 )
         call_with_retry(fn=label.update_info)
 
-    def build_label_interface(
-        self,
-        format: str,
-        class_list: list,
-        bbox: bool,
-    ):
+    def add_object_classes_to_project(self, class_name: str, class_type: str):
         """
-        Build and update the label interface for the project based on the provided class list and bounding box flag.
+        Adds various types of object classes to the label interface of the project based on the specified class type.
 
         Parameters:
-        - class_list (list): A list of class names to be included in the label interface.
-        - bbox (bool): A flag indicating whether bounding boxes should be used.
+        - class_names (list): A list of class names to be added to the label interface.
+        - class_type (str): The type of class to be added. Supported types include 'bbox' (bounding box), 'polygon', 'polyline', 'rbox' (rotated bounding box), and '2dcuboid'.
 
         Returns:
-        A tuple containing the updated label interface and a category map.
+        A tuple containing the updated label interface.
         """
+        existing_label_interface = self.client.project.label_interface
+        if existing_label_interface:
+            label_interface = phy_credit.imageV2.LabelInterface.from_dict(
+                existing_label_interface
+            )
+            object_detection = phy_credit.imageV2.ObjectDetectionDef.from_dict(
+                existing_label_interface.get("object_detection")
+            )
+        else:
+            label_interface = phy_credit.imageV2.LabelInterface.get_default()
+            object_detection = (
+                phy_credit.imageV2.ObjectDetectionDef.get_default()
+            )
 
-        if format.lower() == "yolo":
-            existing_label_interface = self.client.project.label_interface
-            if existing_label_interface:
-                label_interface = phy_credit.imageV2.LabelInterface.from_dict(
-                    existing_label_interface
-                )
-                object_detection = (
-                    phy_credit.imageV2.ObjectDetectionDef.from_dict(
-                        existing_label_interface.get("object_detection")
-                    )
-                )
-            else:
-                label_interface = (
-                    phy_credit.imageV2.LabelInterface.get_default()
-                )
-                object_detection = (
-                    phy_credit.imageV2.ObjectDetectionDef.get_default()
-                )
-
-            category_map = dict()
-            for class_name in class_list:
+            if class_type == "bbox":
                 bbox_suite_class_id = str(uuid4())
                 bbox_suite_class_name = class_name
 
                 object_detection.add_box(
                     name=bbox_suite_class_name, id=bbox_suite_class_id
                 )
 
-            label_interface.set_object_detection(
-                object_detection=object_detection
-            )
+            if class_type == "polygon":
+                seg_suite_class_id = str(uuid4())
+                seg_suite_class_name = class_name
 
-            self.client.update_project(
-                id=self.client.project.id,
-                label_interface=label_interface.to_dict(),
-            )
-        return label_interface, category_map
+                object_detection.add_polygon(
+                    name=seg_suite_class_name, id=seg_suite_class_id
+                )
+
+            if class_type == "polyline":
+                seg_suite_class_id = str(uuid4())
+                seg_suite_class_name = class_name
+
+                object_detection.add_polyline(
+                    name=seg_suite_class_name, id=seg_suite_class_id
+                )
+
+            if class_type == "rbox":
+                seg_suite_class_id = str(uuid4())
+                seg_suite_class_name = class_name
+
+                object_detection.add_rbox(
+                    name=seg_suite_class_name, id=seg_suite_class_id
+                )
+            if class_type == "2dcuboid":
+                seg_suite_class_id = str(uuid4())
+                seg_suite_class_name = class_name
+
+                object_detection.add_2dcuboid(
+                    name=seg_suite_class_name, id=seg_suite_class_id
+                )
+
+        label_interface.set_object_detection(object_detection=object_detection)
+
+        call_with_retry(
+            fn=self.client.update_project,
+            id=self.client.project.id,
+            label_interface=label_interface.to_dict(),
+        )
+        return label_interface
```

### Comparing `superb-ai-apps-0.0.6/spb_apps/utils/converter.py` & `superb-ai-apps-0.0.7/spb_apps/utils/converter.py`

 * *Files identical despite different names*

### Comparing `superb-ai-apps-0.0.6/spb_apps/utils/utils.py` & `superb-ai-apps-0.0.7/spb_apps/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,17 @@
 from pathlib import Path
 from typing import Callable, TypeVar, Union
 from uuid import uuid4
 from zipfile import BadZipFile, ZipFile
 
 import requests
 from directory_tree import display_tree
-from spb_label.exceptions import (
-    APIException,
-    BadRequestException,
-    ConflictException,
-    # InvaildObjectException,
-)
 from phy_credit.exceptions import InvalidObjectException
+from spb_label.exceptions import APIException  # InvaildObjectException,
+from spb_label.exceptions import BadRequestException, ConflictException
 
 logger = logging.getLogger("superb_label")
 
 
 def separate_batches(image_batch_size: int, to_batch_list: list):
     """
     Separates a list of items into batches of a specified size.
```

### Comparing `superb-ai-apps-0.0.6/superb_ai_apps.egg-info/requires.txt` & `superb-ai-apps-0.0.7/superb_ai_apps.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 referencing==0.34.0
 requests==2.31.0
 rpds-py==0.18.0
 semver==3.0.2
 six==1.16.0
 soupsieve==2.5
 stack-data==0.6.3
-superb-ai-curate==1.2.1
+superb-ai-curate==1.2.2
 superb-ai-label==0.21.2
 tinycss2==1.2.1
 tornado==6.4
 traitlets==5.14.2
 typing_extensions==4.10.0
 urllib3==2.2.1
 wcwidth==0.2.13
```


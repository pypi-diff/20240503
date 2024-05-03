# Comparing `tmp/deepview_datasets-0.3.2.tar.gz` & `tmp/deepview_datasets-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepview_datasets-0.3.2.tar", last modified: Thu Apr 25 21:22:39 2024, max compression
+gzip compressed data, was "deepview_datasets-0.3.3.tar", last modified: Fri May  3 20:08:40 2024, max compression
```

## Comparing `deepview_datasets-0.3.2.tar` & `deepview_datasets-0.3.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:22:39.170867 deepview_datasets-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    34675 2024-04-25 21:22:35.000000 deepview_datasets-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    41536 2024-04-25 21:22:39.170867 deepview_datasets-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-25 21:22:35.000000 deepview_datasets-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:22:39.166867 deepview_datasets-0.3.2/deepview/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:22:39.166867 deepview_datasets-0.3.2/deepview/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:22:39.166867 deepview_datasets-0.3.2/deepview/datasets/generators/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-25 21:22:35.000000 deepview_datasets-0.3.2/deepview/datasets/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-25 21:22:35.000000 deepview_datasets-0.3.2/deepview/datasets/generators/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-04-25 21:22:35.000000 deepview_datasets-0.3.2/deepview/datasets/generators/detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:22:39.166867 deepview_datasets-0.3.2/deepview/datasets/readers/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-25 21:22:35.000000 deepview_datasets-0.3.2/deepview/datasets/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-25 21:22:35.000000 deepview_datasets-0.3.2/deepview/datasets/readers/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-25 21:22:35.000000 deepview_datasets-0.3.2/deepview/datasets/readers/coco.py
--rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-04-25 21:22:35.000000 deepview_datasets-0.3.2/deepview/datasets/readers/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-25 21:22:35.000000 deepview_datasets-0.3.2/deepview/datasets/readers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)    13404 2024-04-25 21:22:35.000000 deepview_datasets-0.3.2/deepview/datasets/readers/darknet.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-25 21:22:35.000000 deepview_datasets-0.3.2/deepview/datasets/readers/pascal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:22:39.166867 deepview_datasets-0.3.2/deepview/datasets/writers/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-25 21:22:35.000000 deepview_datasets-0.3.2/deepview/datasets/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-25 21:22:35.000000 deepview_datasets-0.3.2/deepview/datasets/writers/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-04-25 21:22:35.000000 deepview_datasets-0.3.2/deepview/datasets/writers/polars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:22:39.170867 deepview_datasets-0.3.2/deepview_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41536 2024-04-25 21:22:39.000000 deepview_datasets-0.3.2/deepview_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-25 21:22:39.000000 deepview_datasets-0.3.2/deepview_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:22:39.000000 deepview_datasets-0.3.2/deepview_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 21:22:39.000000 deepview_datasets-0.3.2/deepview_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 21:22:39.000000 deepview_datasets-0.3.2/deepview_datasets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-25 21:22:35.000000 deepview_datasets-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 21:22:39.170867 deepview_datasets-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:08:40.589801 deepview_datasets-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    34675 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    41536 2024-05-03 20:08:40.589801 deepview_datasets-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:08:40.585801 deepview_datasets-0.3.3/deepview/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:08:40.585801 deepview_datasets-0.3.3/deepview/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:08:40.585801 deepview_datasets-0.3.3/deepview/datasets/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/generators/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/generators/detection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:08:40.585801 deepview_datasets-0.3.3/deepview/datasets/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/readers/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/readers/coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/readers/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/readers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14474 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/readers/darknet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/readers/pascal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:08:40.585801 deepview_datasets-0.3.3/deepview/datasets/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/writers/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/writers/polars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:08:40.589801 deepview_datasets-0.3.3/deepview_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41536 2024-05-03 20:08:40.000000 deepview_datasets-0.3.3/deepview_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-03 20:08:40.000000 deepview_datasets-0.3.3/deepview_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:08:40.000000 deepview_datasets-0.3.3/deepview_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 20:08:40.000000 deepview_datasets-0.3.3/deepview_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 20:08:40.000000 deepview_datasets-0.3.3/deepview_datasets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:08:40.589801 deepview_datasets-0.3.3/setup.cfg
```

### Comparing `deepview_datasets-0.3.2/LICENSE` & `deepview_datasets-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deepview_datasets-0.3.2/PKG-INFO` & `deepview_datasets-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepview-datasets
-Version: 0.3.2
+Version: 0.3.3
 Summary: DeepView Datasets
 Author-email: Au-Zone Technologies <info@au-zone.com>
 License:    DUAL-LICENSED UNDER AGPL-3.0 OR DEEPVIEW AI MIDDLEWARE COMMERCIAL LICENSE
              CONTACT AU-ZONE TECHNOLOGIES <INFO@AU-ZONE.COM> FOR LICENSING DETAILS
         
                             GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
```

### Comparing `deepview_datasets-0.3.2/README.md` & `deepview_datasets-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `deepview_datasets-0.3.2/deepview/datasets/generators/core.py` & `deepview_datasets-0.3.3/deepview/datasets/generators/core.py`

 * *Files identical despite different names*

### Comparing `deepview_datasets-0.3.2/deepview/datasets/generators/detection.py` & `deepview_datasets-0.3.3/deepview/datasets/generators/detection.py`

 * *Files 10% similar despite different names*

```diff
@@ -290,7 +290,31 @@
         else:
             reader = self.val_reader
 
         if reader is None:
             reader = self.__get_generator__(is_train=train)
 
         return reader.get_boxes_dimensions()
+
+    def get_class_distribution(self, train: bool = True) -> dict:
+        """
+        This function computes the number of instances per class and return them into a dictionary
+
+        Parameters
+        ----------
+        trian : bool, optional
+            _description_, by default True
+
+        Returns
+        -------
+        dict
+            _description_
+        """
+        if train:
+            reader = self.training_reader
+        else:
+            reader = self.val_reader
+
+        if reader is None:
+            reader = self.__get_generator__(is_train=train)
+
+        return reader.get_class_distribution()
```

### Comparing `deepview_datasets-0.3.2/deepview/datasets/readers/arrow.py` & `deepview_datasets-0.3.3/deepview/datasets/readers/arrow.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,12 +127,12 @@
 
         bboxes = np.asarray(bboxes.to_list(), dtype=np.float32)
         classes = np.asarray(classes.cast(
             self.__class_order__).to_physical(), dtype=np.int32)
         classes = classes[:, None]
 
         if len(bboxes) == 0:
-            return image, np.zeros(shape=(1, 5), dtype=np.float32)
+            return image, np.asarray([], dtype=np.float32)
 
         boxes = np.concatenate([bboxes, classes], axis=1)
 
         return image, boxes
```

### Comparing `deepview_datasets-0.3.2/deepview/datasets/readers/core.py` & `deepview_datasets-0.3.3/deepview/datasets/readers/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -183,14 +183,16 @@
         tuple
             Contains the inputs and labels for a given random element in the dataset
 
         """
         item = np.random.randint(0, self.__size__ - 1)
         return self[item]
 
+    def get_class_distribution(self) -> dict:
+        raise NotImplementedError("Abstract method should be implemented bu child classes")
 
 class ObjectDetectionBaseReader(BaseReader):
     """This class wraps the Object Detection Dataset Reader
 
     Parameters
     ----------
     BaseReader : Base class
@@ -207,7 +209,10 @@
 
         Raises
         ------
         NotImplementedError
             Abstract method
         """
         raise NotImplementedError("Abstract method")
+
+    def get_class_distribution(self) -> dict:
+        raise NotImplementedError("Abstract method should be implemented bu child classes")
```

### Comparing `deepview_datasets-0.3.2/deepview/datasets/readers/darknet.py` & `deepview_datasets-0.3.3/deepview/datasets/readers/darknet.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         self.images = []
         self.annotations = []
         self.__size__ = 0
         self.__current__ = -1
 
         if isinstance(images, str):
-            if not exists(images):
+            if "*" not in annotations and not exists(images):
                 raise FileNotFoundError(
                     f"\n\t - [ERROR] Images folder does not exist at: {images}"
                 )
 
             image_files = []
             for ext in ['*.[pP][nN][gG]',
                         '*.[jJ][pP][gG]',
@@ -112,28 +112,36 @@
                 self.images,
                 desc="\t [INFO] Reading",
                 colour="green",
                 bar_format='{l_bar}{bar:15}{r_bar}{bar:-15b}'
             )
 
         if isinstance(annotations, str):
-            if not exists(annotations):
+            if "*" not in annotations and not exists(annotations):
                 raise FileNotFoundError(
-                    f"\n\t - [ERROR] Images folder does not exist at: {annotations}"
+                    f"\n\t - [ERROR] Annotations folder does not exist at: {annotations}"
                 )
 
             for image in loop:
                 image_name = splitext(basename(image))[0]
-                ann_file = join(annotations, image_name + '.txt')
-
-                if not exists(ann_file):
-                    ann_file = None
+                
+                if "*" in annotations:
+                    ann_path = splitext(image)[0] + ".txt"
+                    if exists(ann_path):
+                        self.annotations.append(ann_path)
+                        ann_file = ann_path
+                    else:
+                        ann_file = None
                 else:
-                    self.annotations.append(ann_file)
-
+                    ann_file = join(annotations, image_name + '.txt')
+                    if exists(ann_file):
+                        self.annotations.append(ann_path)
+                    else:
+                        ann_file = None
+                
                 self.__storage__.append([image, ann_file])
                 self.__size__ += 1
         else:
             loop = tqdm(
                 zip(self.images, annotations),
                 desc="\t [INFO] Reading",
                 colour="green",
@@ -191,14 +199,35 @@
 
         instance = super().__getitem__(item)
         self.__instance_id__ = splitext(basename(instance[0]))[0]
 
         image = np.fromfile(instance[0], dtype=np.uint8)
         return image, instance[1]
 
+    def get_class_distribution(self) -> dict:
+
+        loop = tqdm(
+            self.annotations,
+            desc="Loading class distribution",
+            colour="green",
+            bar_format='{l_bar}{bar:15}{r_bar}{bar:-15b}'
+        )
+        classes = []
+        for ann in loop:
+            data = np.genfromtxt(ann)
+            if len(data) == 0:
+                continue
+            if len(data.shape) == 1:
+                data = np.expand_dims(data, 0)
+
+            classes.append(data[:, 0])
+        classes = np.concatenate(classes, axis=0).astype(np.int32)
+        classes = np.bincount(classes)        
+        return dict(enumerate(classes))
+    
 
 class DarknetDetectionReader(DarknetReader):
 
     def __init__(
         self,
         images: Union[str, Iterable],
         annotations: Union[str, Iterable],
@@ -305,24 +334,24 @@
             A tuple containing the real values of a single instance for object
             detection. The image and bounding boxes.
         """
         data, ann_file = super().__getitem__(item)
         image = np.asarray(data, dtype=np.uint8)
 
         if ann_file is None:
-            return image, np.zeros(shape=(1, 5), dtype=np.float32)
+            return image, np.array([], dtype=np.float32)
 
         try:
             boxes = pl.read_csv(ann_file, has_header=False,
                                 separator=" ").to_numpy()
         except pl.exceptions.NoDataError:
-            return image, np.zeros(shape=(1, 5), dtype=np.float32)
+            return image, np.array([], dtype=np.float32)
 
         if len(boxes) == 0:
-            return image, np.zeros(shape=(1, 5), dtype=np.float32)
+            return image, np.array([], dtype=np.float32)
 
         if len(boxes.shape) == 1:
             boxes = boxes[None, :]
 
         boxes = boxes[:, [1, 2, 3, 4, 0]].astype(np.float32)
 
         if self.box_format == 'xywh':
```

### Comparing `deepview_datasets-0.3.2/deepview/datasets/writers/core.py` & `deepview_datasets-0.3.3/deepview/datasets/writers/core.py`

 * *Files identical despite different names*

### Comparing `deepview_datasets-0.3.2/deepview/datasets/writers/polars.py` & `deepview_datasets-0.3.3/deepview/datasets/writers/polars.py`

 * *Files identical despite different names*

### Comparing `deepview_datasets-0.3.2/deepview_datasets.egg-info/PKG-INFO` & `deepview_datasets-0.3.3/deepview_datasets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepview-datasets
-Version: 0.3.2
+Version: 0.3.3
 Summary: DeepView Datasets
 Author-email: Au-Zone Technologies <info@au-zone.com>
 License:    DUAL-LICENSED UNDER AGPL-3.0 OR DEEPVIEW AI MIDDLEWARE COMMERCIAL LICENSE
              CONTACT AU-ZONE TECHNOLOGIES <INFO@AU-ZONE.COM> FOR LICENSING DETAILS
         
                             GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
```

### Comparing `deepview_datasets-0.3.2/deepview_datasets.egg-info/SOURCES.txt` & `deepview_datasets-0.3.3/deepview_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepview_datasets-0.3.2/pyproject.toml` & `deepview_datasets-0.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "deepview-datasets"
-version = "0.3.2"
+version = "0.3.3"
 description = "DeepView Datasets"
 readme = "README.md"
 authors = [{ name = "Au-Zone Technologies", email = "info@au-zone.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```


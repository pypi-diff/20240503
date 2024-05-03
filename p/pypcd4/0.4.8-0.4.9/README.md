# Comparing `tmp/pypcd4-0.4.8.tar.gz` & `tmp/pypcd4-0.4.9.tar.gz`

## Comparing `pypcd4-0.4.8.tar` & `pypcd4-0.4.9.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 pypcd4-0.4.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pypcd4-0.4.8/.python-version
--rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 pypcd4-0.4.8/COPYRIGHT.txt
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 pypcd4-0.4.8/requirements-dev.lock
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 pypcd4-0.4.8/requirements.lock
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pypcd4-0.4.8/.vscode/settings.json
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypcd4-0.4.8/src/pypcd4/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pypcd4-0.4.8/src/pypcd4/_version.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 pypcd4-0.4.8/src/pypcd4/pointcloud2.py
--rw-r--r--   0        0        0    25082 2020-02-02 00:00:00.000000 pypcd4-0.4.8/src/pypcd4/pypcd4.py
--rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 pypcd4-0.4.8/tests/conftest.py
--rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 pypcd4-0.4.8/tests/pcd/ascii.pcd
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 pypcd4-0.4.8/tests/pcd/ascii_with_empty_points.pcd
--rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 pypcd4-0.4.8/tests/pcd/ascii_with_underscore.pcd
--rw-r--r--   0        0        0     7504 2020-02-02 00:00:00.000000 pypcd4-0.4.8/tests/pcd/binary.pcd
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pypcd4-0.4.8/tests/pcd/binary_compressed.pcd
--rw-r--r--   0        0        0    23950 2020-02-02 00:00:00.000000 pypcd4-0.4.8/tests/test/test_pypcd4.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pypcd4-0.4.8/.gitignore
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pypcd4-0.4.8/LICENSE.txt
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pypcd4-0.4.8/README.md
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 pypcd4-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 pypcd4-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 pypcd4-0.4.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pypcd4-0.4.9/.python-version
+-rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 pypcd4-0.4.9/COPYRIGHT.txt
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 pypcd4-0.4.9/requirements-dev.lock
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 pypcd4-0.4.9/requirements.lock
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypcd4-0.4.9/src/pypcd4/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pypcd4-0.4.9/src/pypcd4/_version.py
+-rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 pypcd4-0.4.9/src/pypcd4/pointcloud2.py
+-rw-r--r--   0        0        0    26040 2020-02-02 00:00:00.000000 pypcd4-0.4.9/src/pypcd4/pypcd4.py
+-rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 pypcd4-0.4.9/tests/conftest.py
+-rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 pypcd4-0.4.9/tests/pcd/ascii.pcd
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 pypcd4-0.4.9/tests/pcd/ascii_with_empty_points.pcd
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 pypcd4-0.4.9/tests/pcd/ascii_with_underscore.pcd
+-rw-r--r--   0        0        0     7504 2020-02-02 00:00:00.000000 pypcd4-0.4.9/tests/pcd/binary.pcd
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pypcd4-0.4.9/tests/pcd/binary_compressed.pcd
+-rw-r--r--   0        0        0    25133 2020-02-02 00:00:00.000000 pypcd4-0.4.9/tests/test/test_pypcd4.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 pypcd4-0.4.9/.gitignore
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pypcd4-0.4.9/LICENSE.txt
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 pypcd4-0.4.9/README.md
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 pypcd4-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     6959 2020-02-02 00:00:00.000000 pypcd4-0.4.9/PKG-INFO
```

### Comparing `pypcd4-0.4.8/COPYRIGHT.txt` & `pypcd4-0.4.9/COPYRIGHT.txt`

 * *Files identical despite different names*

### Comparing `pypcd4-0.4.8/src/pypcd4/pointcloud2.py` & `pypcd4-0.4.9/src/pypcd4/pointcloud2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Any, ClassVar
 
 import numpy as np
+import numpy.typing as npt
 
 
 @dataclass
 class builtin_interfaces__msg__Time:
     sec: int
     nanosec: int
 
@@ -64,15 +65,15 @@
 
     __msgtype__: ClassVar[str] = "sensor_msgs/msg/PointCloud2"
 
 
 PointCloud2 = sensor_msgs__msg__PointCloud2
 
 
-TYPE_MAPPINGS = [
+TYPE_MAPPINGS: list[tuple[int, npt.DTypeLike]] = [
     (PointField.INT8, np.dtype("int8")),
     (PointField.UINT8, np.dtype("uint8")),
     (PointField.INT16, np.dtype("int16")),
     (PointField.UINT16, np.dtype("uint16")),
     (PointField.INT32, np.dtype("int32")),
     (PointField.UINT32, np.dtype("uint32")),
     (PointField.FLOAT32, np.dtype("float32")),
@@ -112,10 +113,12 @@
     return dtypes
 
 
 def pointcloud2_to_array(msg: PointCloud2) -> np.ndarray:
     dtype = build_dtype(msg)
 
     array = np.frombuffer(msg.data, dtype)
-    array = np.hstack([array[n][:, None] for n in array.dtype.names if not n.startswith("__")])
+    array = np.hstack(
+        [array[n][:, None] for n in array.dtype.names if not n.startswith("__")]  # type: ignore
+    )
 
     return array
```

### Comparing `pypcd4-0.4.8/src/pypcd4/pypcd4.py` & `pypcd4-0.4.9/src/pypcd4/pypcd4.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 import random
 import re
 import string
 import struct
 from enum import Enum
 from pathlib import Path
-from typing import BinaryIO, List, Literal, Optional, Sequence, Tuple, Type, Union
+from typing import BinaryIO, List, Literal, Optional, Sequence, Tuple, Union
 
 import lzf
 import numpy as np
+import numpy.typing as npt
 from pydantic import BaseModel, NonNegativeInt, PositiveInt
 
 from .pointcloud2 import PFTYPE_TO_NPTYPE, PointCloud2, pointcloud2_to_array
 
-NpNumberType = Type[Union[np.integer, np.floating]]
 PathLike = Union[str, Path]
 
 MetaDataVersion = Literal[".7", "0.7"]
 MetaDataViewPoint = Tuple[float, float, float, float, float, float, float]
 
 NUMPY_TYPE_TO_PCD_TYPE: dict[
-    np.dtype,
+    npt.DTypeLike,
     Tuple[str, int],
 ] = {
     np.dtype("uint8"): ("U", 1),
     np.dtype("uint16"): ("U", 2),
     np.dtype("uint32"): ("U", 4),
     np.dtype("uint64"): ("U", 8),
     np.dtype("int8"): ("I", 1),
@@ -34,15 +34,15 @@
     np.dtype("int64"): ("I", 8),
     np.dtype("float32"): ("F", 4),
     np.dtype("float64"): ("F", 8),
 }
 
 PCD_TYPE_TO_NUMPY_TYPE: dict[
     Tuple[str, int],
-    NpNumberType,
+    npt.DTypeLike,
 ] = {
     ("F", 4): np.float32,
     ("F", 8): np.float64,
     ("U", 1): np.uint8,
     ("U", 2): np.uint16,
     ("U", 4): np.uint32,
     ("U", 8): np.uint64,
@@ -88,15 +88,15 @@
 
         Returns:
             MetaData: Parsed MetaData object
         """
 
         _header = {}
         for line in lines:
-            if line.startswith("#") or len(line) < 2:
+            if line.startswith("#") or len(line) < 2:  # noqa: PLR2004
                 continue
 
             if (match := re.match(HEADER_PATTERN, line)) is None:
                 continue
 
             value = match.group(2).split()
             if (key := match.group(1).lower()) in ["version", "data"]:
@@ -144,71 +144,71 @@
         header.append(f"POINTS {self.points}")
         header.append(f"DATA {self.data.value}")
 
         return "\n".join(header) + "\n"
 
     def build_dtype(self) -> np.dtype[np.void]:
         field_names: List[str] = []
-        type_names: List[np.dtype] = []
+        np_types: List[npt.DTypeLike] = []
 
         for i, field in enumerate(self.fields):
-            np_type: np.dtype = np.dtype(PCD_TYPE_TO_NUMPY_TYPE[(self.type[i], self.size[i])])
+            np_type: npt.DTypeLike = np.dtype(PCD_TYPE_TO_NUMPY_TYPE[(self.type[i], self.size[i])])
 
             if (count := self.count[i]) == 1:
                 field_names.append(field)
-                type_names.append(np_type)
+                np_types.append(np_type)
             else:
                 field_names.extend([f"{field}_{i:04d}" for i in range(count)])
-                type_names.extend([np_type] * count)
+                np_types.extend([np_type] * count)
 
-        return np.dtype([x for x in zip(field_names, type_names)])
+        return np.dtype([x for x in zip(field_names, np_types)])
 
 
-def _parse_pc_data(fp: BinaryIO, metadata: MetaData) -> np.ndarray:
+def _parse_pc_data(fp: BinaryIO, metadata: MetaData) -> npt.NDArray:
     dtype = metadata.build_dtype()
 
     if metadata.points > 0:
         if metadata.data == Encoding.ASCII:
             pc_data = np.loadtxt(fp, dtype, delimiter=" ")
         elif metadata.data == Encoding.BINARY:
             buffer = fp.read(metadata.points * dtype.itemsize)
-            pc_data = np.frombuffer(buffer, dtype)  # type: ignore
+            pc_data = np.frombuffer(buffer, dtype)
         else:
             compressed_size, uncompressed_size = struct.unpack("II", fp.read(8))  # type: ignore
 
             buffer = lzf.decompress(fp.read(compressed_size), uncompressed_size)
             if (actual_size := len(buffer)) != uncompressed_size:
                 raise RuntimeError(
                     f"Failed to decompress data. "
                     f"Expected decompressed file size is {uncompressed_size}, but got {actual_size}"
                 )
 
             offset = 0
             pc_data = np.zeros(metadata.width, dtype=dtype)
-            for name in dtype.names:
+            for name in dtype.names:  # type: ignore
                 dt: np.dtype = dtype[name]
                 bytes = dt.itemsize * metadata.width
                 pc_data[name] = np.frombuffer(buffer[offset : (offset + bytes)], dtype=dt)
                 offset += bytes
     else:
         pc_data = np.empty((0, len(metadata.fields)), dtype)
 
     return pc_data
 
 
 def _compose_pc_data(
-    points: Union[np.ndarray, Sequence[np.ndarray]], metadata: MetaData
-) -> np.ndarray:
-    arrays: Sequence[np.ndarray] = tuple(points.T) if isinstance(points, np.ndarray) else points
+    points: Union[npt.NDArray, Sequence[npt.NDArray]], metadata: MetaData
+) -> npt.NDArray:
+    arrays: Sequence[npt.NDArray] = tuple(points.T) if isinstance(points, np.ndarray) else points
 
     return np.rec.fromarrays(arrays, dtype=metadata.build_dtype())
 
 
 class PointCloud:
-    def __init__(self, metadata: MetaData, pc_data: np.ndarray) -> None:
+    def __init__(self, metadata: MetaData, pc_data: npt.NDArray) -> None:
         self.metadata = metadata
         self.pc_data = pc_data
 
     @staticmethod
     def from_fileobj(fp: BinaryIO) -> PointCloud:
         lines: List[str] = []
         while True:
@@ -243,31 +243,31 @@
         """
 
         with open(path, mode="rb") as fp:
             return PointCloud.from_fileobj(fp)
 
     @staticmethod
     def from_points(
-        points: Union[np.ndarray, List[np.ndarray], Tuple[np.ndarray, ...]],
+        points: Union[npt.NDArray, List[npt.NDArray], Tuple[npt.NDArray, ...]],
         fields: Sequence[str],
-        types: Sequence[Union[NpNumberType, np.dtype]],
+        types: Sequence[npt.DTypeLike],
         count: Optional[Sequence[int]] = None,
     ) -> PointCloud:
         """Create PointCloud from 2D numpy array or sequence of 1D numpy arrays of each field
 
         Args:
-            points (Union[np.ndarray, List[np.ndarray], Tuple[np.ndarray, ...]]): Numpy array
+            points (Union[npt.NDArray, List[npt.NDArray], Tuple[npt.NDArray, ...]]): Numpy array
             fields (Sequence[str]): Field names for each numpy array or sequence of numpy arrays
-            types (Sequence[Union[NpNumberType, np.dtype]]): Numpy type for each numpy array or
+            types (Sequence[npt.DTypeLike]): Numpy type for each numpy array or
                 sequence of numpy arrays
             count (Optional[Sequence[int]], optional): Number of values for each numpy array or
                 sequence of numpy arrays. If None, set to 1 for all fields. Defaults to None.
 
         Raises:
-            TypeError: Raise if `points` type is neither `np.ndarray` nor `Sequence[np.ndarray]`.
+            TypeError: Raise if `points` type is neither `npt.NDArray` nor `Sequence[npt.NDArray]`.
 
         Returns:
             PointCloud: PointCloud object
 
         >>> PointCloud.from_points(
                 np.array([[1, 2, 3], [4, 5, 6]]),
                 ("x", "y", "z"),
@@ -341,153 +341,155 @@
                     "data": Encoding.BINARY_COMPRESSED,
                 }
             )
 
         return PointCloud(metadata, _compose_pc_data(points, metadata))
 
     @staticmethod
-    def from_xyz_points(points: np.ndarray) -> PointCloud:
+    def from_xyz_points(points: npt.NDArray) -> PointCloud:
         fields = ("x", "y", "z")
         types = (np.float32, np.float32, np.float32)
 
         return PointCloud.from_points(points, fields, types)
 
     @staticmethod
-    def from_xyzi_points(points: np.ndarray) -> PointCloud:
+    def from_xyzi_points(points: npt.NDArray) -> PointCloud:
         fields = ("x", "y", "z", "intensity")
         types = (np.float32, np.float32, np.float32, np.float32)
 
         return PointCloud.from_points(points, fields, types)
 
     @staticmethod
-    def from_xyzl_points(points: np.ndarray, label_type: NpNumberType = np.float32) -> PointCloud:
+    def from_xyzl_points(points: npt.NDArray, label_type: npt.DTypeLike = np.float32) -> PointCloud:
         fields = ("x", "y", "z", "label")
         types = (np.float32, np.float32, np.float32, label_type)
 
         return PointCloud.from_points(points, fields, types)
 
     @staticmethod
-    def from_xyzrgb_points(points: np.ndarray) -> PointCloud:
+    def from_xyzrgb_points(points: npt.NDArray) -> PointCloud:
         fields = ("x", "y", "z", "rgb")
         types = (np.float32, np.float32, np.float32, np.float32)
 
         return PointCloud.from_points(points, fields, types)
 
     @staticmethod
     def from_xyzrgbl_points(
-        points: np.ndarray, label_type: NpNumberType = np.float32
+        points: npt.NDArray, label_type: npt.DTypeLike = np.float32
     ) -> PointCloud:
         fields = ("x", "y", "z", "rgb", "label")
         types = (np.float32, np.float32, np.float32, np.float32, label_type)
 
         return PointCloud.from_points(points, fields, types)
 
     @staticmethod
-    def from_xyzil_points(points: np.ndarray, label_type: NpNumberType = np.float32) -> PointCloud:
+    def from_xyzil_points(
+        points: npt.NDArray, label_type: npt.DTypeLike = np.float32
+    ) -> PointCloud:
         fields = ("x", "y", "z", "intensity", "label")
         types = (np.float32, np.float32, np.float32, np.float32, label_type)
 
         return PointCloud.from_points(points, fields, types)
 
     @staticmethod
-    def from_xyzirgb_points(points: np.ndarray) -> PointCloud:
+    def from_xyzirgb_points(points: npt.NDArray) -> PointCloud:
         fields = ("x", "y", "z", "intensity", "rgb")
         types = (np.float32, np.float32, np.float32, np.float32, np.float32)
 
         return PointCloud.from_points(points, fields, types)
 
     @staticmethod
     def from_xyzirgbl_points(
-        points: np.ndarray, label_type: NpNumberType = np.float32
+        points: npt.NDArray, label_type: npt.DTypeLike = np.float32
     ) -> PointCloud:
         fields = ("x", "y", "z", "intensity", "rgb", "label")
         types = (np.float32, np.float32, np.float32, np.float32, np.float32, label_type)
 
         return PointCloud.from_points(points, fields, types)
 
     @staticmethod
-    def from_xyzt_points(points: np.ndarray) -> PointCloud:
+    def from_xyzt_points(points: npt.NDArray) -> PointCloud:
         fields = ("x", "y", "z", "sec", "nsec")
         types = (np.float32, np.float32, np.float32, np.uint32, np.uint32)
 
         return PointCloud.from_points(points, fields, types)
 
     @staticmethod
-    def from_xyzir_points(points: np.ndarray) -> PointCloud:
+    def from_xyzir_points(points: npt.NDArray) -> PointCloud:
         fields = ("x", "y", "z", "intensity", "ring")
         types = (np.float32, np.float32, np.float32, np.float32, np.uint16)
 
         return PointCloud.from_points(points, fields, types)
 
     @staticmethod
-    def from_xyzirt_points(points: np.ndarray) -> PointCloud:
+    def from_xyzirt_points(points: npt.NDArray) -> PointCloud:
         fields = ("x", "y", "z", "intensity", "ring", "time")
         types = (np.float32, np.float32, np.float32, np.float32, np.uint16, np.float32)
 
         return PointCloud.from_points(points, fields, types)
 
     @staticmethod
-    def from_xyzit_points(points: np.ndarray) -> PointCloud:
+    def from_xyzit_points(points: npt.NDArray) -> PointCloud:
         fields = ("x", "y", "z", "intensity", "timestamp")
         types = (np.float32, np.float32, np.float32, np.float32, np.float64)
 
         return PointCloud.from_points(points, fields, types)
 
     @staticmethod
-    def from_xyzis_points(points: np.ndarray) -> PointCloud:
+    def from_xyzis_points(points: npt.NDArray) -> PointCloud:
         fields = ("x", "y", "z", "intensity", "stamp")
         types = (np.float32, np.float32, np.float32, np.float32, np.float64)
 
         return PointCloud.from_points(points, fields, types)
 
     @staticmethod
-    def from_xyzisc_points(points: np.ndarray) -> PointCloud:
+    def from_xyzisc_points(points: npt.NDArray) -> PointCloud:
         fields = ("x", "y", "z", "intensity", "stamp", "classification")
         types = (np.float32, np.float32, np.float32, np.float32, np.float64, np.uint8)
 
         return PointCloud.from_points(points, fields, types)
 
     @staticmethod
-    def from_xyzrgbs_points(points: np.ndarray) -> PointCloud:
+    def from_xyzrgbs_points(points: npt.NDArray) -> PointCloud:
         fields = ("x", "y", "z", "rgb", "stamp")
         types = (np.float32, np.float32, np.float32, np.float32, np.float64)
 
         return PointCloud.from_points(points, fields, types)
 
     @staticmethod
-    def from_xyzirgbs_points(points: np.ndarray) -> PointCloud:
+    def from_xyzirgbs_points(points: npt.NDArray) -> PointCloud:
         fields = ("x", "y", "z", "intensity", "rgb", "stamp")
         types = (
             np.float32,
             np.float32,
             np.float32,
             np.float32,
             np.float32,
             np.float64,
         )
 
         return PointCloud.from_points(points, fields, types)
 
     @staticmethod
-    def from_xyzirgbsc_points(points: np.ndarray) -> PointCloud:
+    def from_xyzirgbsc_points(points: npt.NDArray) -> PointCloud:
         fields = ("x", "y", "z", "intensity", "rgb", "stamp", "classification")
         types = (
             np.float32,
             np.float32,
             np.float32,
             np.float32,
             np.float32,
             np.float64,
             np.uint8,
         )
 
         return PointCloud.from_points(points, fields, types)
 
     @staticmethod
-    def from_xyziradt_points(points: np.ndarray) -> PointCloud:
+    def from_xyziradt_points(points: npt.NDArray) -> PointCloud:
         fields = (
             "x",
             "y",
             "z",
             "intensity",
             "ring",
             "azimuth",
@@ -506,15 +508,15 @@
             np.uint8,
             np.float64,
         )
 
         return PointCloud.from_points(points, fields, types)
 
     @staticmethod
-    def from_ouster_points(points: np.ndarray) -> PointCloud:
+    def from_ouster_points(points: npt.NDArray) -> PointCloud:
         fields = (
             "x",
             "y",
             "z",
             "intensity",
             "t",
             "reflectivity",
@@ -536,20 +538,20 @@
 
         return PointCloud.from_points(points, fields, types)
 
     @staticmethod
     def from_msg(msg: PointCloud2) -> PointCloud:
         points = pointcloud2_to_array(msg)
         fields = [f.name for f in msg.fields]
-        types = [PFTYPE_TO_NPTYPE[f.datatype] for f in msg.fields]
+        types: list[npt.DTypeLike] = [PFTYPE_TO_NPTYPE[f.datatype] for f in msg.fields]
 
-        return PointCloud.from_points(points, fields, types)  # type: ignore
+        return PointCloud.from_points(points, fields, types)
 
     @staticmethod
-    def encode_rgb(rgb: np.ndarray | list[np.ndarray]) -> np.ndarray:
+    def encode_rgb(rgb: npt.NDArray | list[npt.NDArray]) -> npt.NDArray:
         """
         Encode Nx3 uint8 array with RGB values to
         Nx1 float32 array with bit-packed RGB
         """
 
         if isinstance(rgb, np.ndarray):
             if rgb.ndim == 1:
@@ -563,15 +565,15 @@
             dtype=np.uint32,
         )
         rgb_u32.dtype = np.float32  # type: ignore
 
         return rgb_u32
 
     @staticmethod
-    def decode_rgb(rgb: np.ndarray) -> np.ndarray:
+    def decode_rgb(rgb: npt.NDArray) -> npt.NDArray:
         """
         Decode Nx1 float32 array with bit-packed RGB to
         Nx3 uint8 array with RGB values
         """
 
         rgb = rgb.copy()
         rgb.dtype = np.uint32  # type: ignore
@@ -593,19 +595,19 @@
         >>> pc.fields
         ("x", "y", "z")
         """
 
         return self.metadata.fields
 
     @property
-    def types(self) -> Tuple[NpNumberType, ...]:
+    def types(self) -> Tuple[npt.DTypeLike, ...]:
         """Returns types of the point cloud
 
         Returns:
-            Tuple[NpNumberType, ...]: Tuple of numpy types for each field
+            Tuple[npt.DTypeLike, ...]: Tuple of numpy types for each field
 
         >>> pc.types
         (np.float32, np.float32, np.float32)
         """
 
         return tuple(
             PCD_TYPE_TO_NUMPY_TYPE[ts] for ts in zip(self.metadata.type, self.metadata.size)
@@ -633,23 +635,23 @@
 
         >>> pc.points
         1000
         """
 
         return self.metadata.points
 
-    def numpy(self, fields: Optional[Sequence[str]] = None) -> np.ndarray:
+    def numpy(self, fields: Optional[Sequence[str]] = None) -> npt.NDArray:
         """Returns numpy array of the point cloud
 
         Args:
             fields (Optional[Sequence[str]], optional): Fields to return.
                 If None, all fields are returned. Defaults to None.
 
         Returns:
-            np.ndarray: Numpy array of the point cloud
+            npt.NDArray: Numpy array of the point cloud
 
         >>> pc.fields
         ("x", "y", "z")
 
         >>> pc.numpy()
         array([[0.0, 0.1, 0.2],
                [0.3, 0.4, 0.5],
@@ -697,24 +699,52 @@
         if self.fields != other.fields:
             raise ValueError(
                 "Can't concatenate point clouds with different fields. "
                 f"({self.fields} vs. {other.fields})"
             )
         if self.types != other.types:
             raise ValueError(
-                "Can't concatenate point clouds with different metadata. "
+                "Can't concatenate point clouds with different types. "
                 f"({self.types} vs. {other.types})"
             )
 
         concatenated_pc = PointCloud.from_points(
             np.vstack((self.numpy(), other.numpy())), self.fields, self.types
         )
 
         return concatenated_pc
 
+    def __getitem__(self, mask: npt.NDArray[np.bool_]) -> PointCloud:
+        """Returns a point cloud with only the points that match the mask
+
+        >>> np.random.seed(42)
+        >>> pc = PointCloud.from_xyz_points(np.random.rand(100, 3))
+        >>> pc.points
+        10
+        >>> mask = (pc.pc_data["x"] > 0.5) & (pc.pc_data["y"] < 0.5)
+        >>> pc[mask].points
+        3
+        >>> pc[mask].numpy()
+        [[0.5986585  0.15601864 0.15599452]
+        [0.7080726  0.02058449 0.96990985]
+        [0.83244264 0.21233912 0.18182497]]
+        """
+
+        mask = mask.squeeze()
+
+        if mask.ndim != 1:
+            raise ValueError(f"mask array must be 1-dimensional but got {mask.ndim}")
+
+        points_list = [
+            self.pc_data[field][mask]
+            for field in self.pc_data.dtype.names  # type: ignore
+        ]
+
+        return PointCloud.from_points(points_list, self.fields, self.types)
+
     def _save_as_ascii(self, fp: BinaryIO) -> None:
         """Saves point cloud to a file as a ascii
 
         Args:
             fp (BinaryIO): io buffer.
         """
 
@@ -743,15 +773,15 @@
 
         Args:
             fp (BinaryIO): io buffer.
         """
 
         uncompressed = b"".join(
             np.ascontiguousarray(self.pc_data[field]).tobytes()
-            for field in self.pc_data.dtype.names
+            for field in self.pc_data.dtype.names  # type: ignore
         )
 
         if (compressed := lzf.compress(uncompressed)) is None:
             compressed = uncompressed
 
         fp.write(struct.pack("II", len(compressed), len(uncompressed)))
         fp.write(compressed)
```

### Comparing `pypcd4-0.4.8/tests/conftest.py` & `pypcd4-0.4.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pypcd4-0.4.8/tests/pcd/ascii.pcd` & `pypcd4-0.4.9/tests/pcd/ascii.pcd`

 * *Files identical despite different names*

### Comparing `pypcd4-0.4.8/tests/pcd/ascii_with_underscore.pcd` & `pypcd4-0.4.9/tests/pcd/ascii_with_underscore.pcd`

 * *Files identical despite different names*

### Comparing `pypcd4-0.4.8/tests/pcd/binary.pcd` & `pypcd4-0.4.9/tests/pcd/binary.pcd`

 * *Files identical despite different names*

### Comparing `pypcd4-0.4.8/tests/pcd/binary_compressed.pcd` & `pypcd4-0.4.9/tests/pcd/binary_compressed.pcd`

 * *Files identical despite different names*

### Comparing `pypcd4-0.4.8/tests/test/test_pypcd4.py` & `pypcd4-0.4.9/tests/test/test_pypcd4.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from io import BytesIO
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 import numpy as np
 import pytest
 from pydantic import ValidationError
-
 from pypcd4 import Encoding, MetaData, PointCloud
 
 
 def test_parse_pcd_header(pcd_header):
     metadata = MetaData.parse_header(pcd_header)
 
     assert metadata.version == ".7"
@@ -125,15 +124,17 @@
     assert metadata.width == 213
     assert metadata.height == 1
     assert metadata.viewpoint == (1.0, -2.0, 3.0, 1.0, -1.0, 2.0, -3.0)
     assert metadata.points == 213
     assert metadata.data == "ascii"
 
 
-def test_parse_pcd_header_with_underscore_in_fields(pcd_header_with_underscore_in_fields):
+def test_parse_pcd_header_with_underscore_in_fields(
+    pcd_header_with_underscore_in_fields,
+):
     metadata = MetaData.parse_header(pcd_header_with_underscore_in_fields)
 
     assert metadata.version == ".7"
     assert metadata.fields != ("_", "y", "_")
     assert metadata.size == (4, 4, 4)
     assert metadata.type == ("F", "F", "F")
     assert metadata.count == (1, 1, 1)
@@ -403,27 +404,48 @@
 def test_from_xyzirgbl_points():
     points = np.random.random((100, 6))
 
     label_type = np.int32
     pc = PointCloud.from_xyzirgbl_points(points, label_type)
 
     assert pc.fields == ("x", "y", "z", "intensity", "rgb", "label")
-    assert pc.types == (np.float32, np.float32, np.float32, np.float32, np.float32, label_type)
+    assert pc.types == (
+        np.float32,
+        np.float32,
+        np.float32,
+        np.float32,
+        np.float32,
+        label_type,
+    )
 
     label_type = np.float32
     pc = PointCloud.from_xyzirgbl_points(points, label_type)
 
     assert pc.fields == ("x", "y", "z", "intensity", "rgb", "label")
-    assert pc.types == (np.float32, np.float32, np.float32, np.float32, np.float32, label_type)
+    assert pc.types == (
+        np.float32,
+        np.float32,
+        np.float32,
+        np.float32,
+        np.float32,
+        label_type,
+    )
 
     label_type = np.uint8
     pc = PointCloud.from_xyzirgbl_points(points, label_type)
 
     assert pc.fields == ("x", "y", "z", "intensity", "rgb", "label")
-    assert pc.types == (np.float32, np.float32, np.float32, np.float32, np.float32, label_type)
+    assert pc.types == (
+        np.float32,
+        np.float32,
+        np.float32,
+        np.float32,
+        np.float32,
+        label_type,
+    )
 
 
 def test_from_xyzt_points():
     points = np.random.random((100, 5))
 
     pc = PointCloud.from_xyzt_points(points)
 
@@ -442,15 +464,22 @@
 
 def test_from_xyzirt_points():
     points = np.random.random((100, 6))
 
     pc = PointCloud.from_xyzirt_points(points)
 
     assert pc.fields == ("x", "y", "z", "intensity", "ring", "time")
-    assert pc.types == (np.float32, np.float32, np.float32, np.float32, np.uint16, np.float32)
+    assert pc.types == (
+        np.float32,
+        np.float32,
+        np.float32,
+        np.float32,
+        np.uint16,
+        np.float32,
+    )
 
 
 def test_from_xyzit_points():
     points = np.random.random((100, 5))
 
     pc = PointCloud.from_xyzit_points(points)
 
@@ -469,15 +498,22 @@
 
 def test_from_xyzisc_points():
     points = np.random.random((100, 6))
 
     pc = PointCloud.from_xyzisc_points(points)
 
     assert pc.fields == ("x", "y", "z", "intensity", "stamp", "classification")
-    assert pc.types == (np.float32, np.float32, np.float32, np.float32, np.float64, np.uint8)
+    assert pc.types == (
+        np.float32,
+        np.float32,
+        np.float32,
+        np.float32,
+        np.float64,
+        np.uint8,
+    )
 
 
 def test_from_xyzrgbs_points():
     points = np.random.random((100, 5))
 
     pc = PointCloud.from_xyzrgbs_points(points)
 
@@ -487,15 +523,22 @@
 
 def test_from_xyzirgbs_points():
     points = np.random.random((100, 6))
 
     pc = PointCloud.from_xyzirgbs_points(points)
 
     assert pc.fields == ("x", "y", "z", "intensity", "rgb", "stamp")
-    assert pc.types == (np.float32, np.float32, np.float32, np.float32, np.float32, np.float64)
+    assert pc.types == (
+        np.float32,
+        np.float32,
+        np.float32,
+        np.float32,
+        np.float32,
+        np.float64,
+    )
 
 
 def test_from_xyzirgbsc_points():
     points = np.random.random((100, 7))
 
     pc = PointCloud.from_xyzirgbsc_points(points)
 
@@ -760,7 +803,34 @@
     with pytest.raises(ValueError):
         pc + pc4
 
     # Cannot concatenate because types are different
     pc5 = PointCloud.from_points(in_points, fields, (np.float32, np.int8, np.float32))
     with pytest.raises(ValueError):
         pc + pc5
+
+
+def test_pointcloud_getitem():
+    in_points = np.random.randint(0, 1000, (100, 3))
+    fields = ("x", "y", "z")
+    types = (np.float32, np.int8, np.uint64)
+    pc = PointCloud.from_points(in_points, fields, types)
+
+    # Can filter PointCloud
+    mask1 = (pc.pc_data["x"] > 0.5) & (pc.pc_data["y"] < 0.5)
+    pc2 = pc[mask1]
+    assert pc2.points == np.count_nonzero(mask1)
+    assert pc2.fields == pc.fields
+    assert pc2.types == pc.types
+
+    # Can filter PointCloud with mask can be squeezed
+    mask2 = pc.numpy("x") > 0.5
+    mask2 = mask2[:, None, None, None]
+    pc3 = pc[mask2]
+    assert pc3.points == np.count_nonzero(mask2)
+    assert pc3.fields == pc.fields
+    assert pc3.types == pc.types
+
+    # Cannot filter mask dimension is not 1
+    mask3 = pc.numpy(("x", "y")) > 0.5
+    with pytest.raises(ValueError):
+        pc[mask3]
```

### Comparing `pypcd4-0.4.8/.gitignore` & `pypcd4-0.4.9/.gitignore`

 * *Files 19% similar despite different names*

```diff
@@ -57,7 +57,10 @@
 env.bak/
 venv.bak/
 
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
+
+# Editor
+.vscode/
```

### Comparing `pypcd4-0.4.8/LICENSE.txt` & `pypcd4-0.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypcd4-0.4.8/pyproject.toml` & `pypcd4-0.4.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -19,56 +19,53 @@
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries",
     "Topic :: Utilities",
 ]
 urls."Release Notes" = "https://github.com/MapIV/pypcd4/releases"
 urls.Source = "https://github.com/MapIV/pypcd4"
 urls.Tracker = "https://github.com/MapIV/pypcd4/issues"
 
 [project.optional-dependencies]
-dev = ["black", "mypy", "setuptools-scm", "isort"]
+dev = ["ruff", "mypy", "setuptools-scm"]
 
 [build-system]
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
 dev-dependencies = [
-    "black>=23.7.0",
     "mypy>=1.5.1",
     "setuptools-scm>=7.1.0",
-    "isort>=5.12.0",
-    "pyproject-flake8>=6.0.0.post1",
     "pre-commit>=3.4.0",
     "pytest>=7.4.1",
     "tox>=4.11.1",
     "pytest-cov>=4.1.0",
+    "ruff>=0.3.4",
 ]
 
 [tool.rye.scripts]
 lint = { chain = [
-    "lint:isort",
-    "lint:black",
-    "lint:flake8",
+    "lint:ruff-lint",
+    "lint:ruff-format",
     "lint:mypy",
     "lint:tox",
 ] }
-"lint:isort" = "isort src"
-"lint:black" = "black src"
-"lint:flake8" = "pflake8 src"
-"lint:mypy" = "mypy src"
+"lint:ruff-lint" = "ruff check --verbose --fix src"
+"lint:ruff-format" = "ruff format --verbose src"
+"lint:mypy" = "mypy --verbose src"
 "lint:tox" = "tox"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch]
 version.source = "vcs"
@@ -78,40 +75,43 @@
 local_scheme = "no-local-version"
 
 [tool.setuptools_scm]
 write_to = "src/pypcd4/_version.py"
 version_scheme = "guess-next-dev"
 local_scheme = "node-and-date"
 
-[tool.isort]
-line_length = 100
-profile = "black"
-
-[tool.flake8]
-max-line-length = 100
-max-complexity = 18
-ignore = "E203,E266,W503,"
-
-[tool.black]
-target-version = ["py38", "py39", "py310", "py311"]
+[tool.ruff]
 line-length = 100
+indent-width = 4
+
+[tool.ruff.lint]
+select = ["E", "F", "I", "PLR", "B", "ANN"]
+ignore = ["ANN101", "ANN102"]
+fixable = ["ALL"]
+unfixable = []
+
+[tool.ruff.format]
+quote-style = "double"
+indent-style = "space"
+docstring-code-format = true
+docstring-code-line-length = 60
 
 [tool.mypy]
-no_strict_optional = true
 ignore_missing_imports = true
 check_untyped_defs = true
 
 [tool.tox]
 legacy_tox_ini = """
     [tox]
     min_version = 4.0
     isolated_build = true
     env_list =
         py38
         py39
         py310
         py311
+        py312
 
     [testenv]
     deps = pytest
     commands = pytest tests -vv
 """
```

### Comparing `pypcd4-0.4.8/PKG-INFO` & `pypcd4-0.4.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pypcd4
-Version: 0.4.8
+Version: 0.4.9
 Summary: Read and write PCL .pcd files in python
 Project-URL: Release Notes, https://github.com/MapIV/pypcd4/releases
 Project-URL: Source, https://github.com/MapIV/pypcd4
 Project-URL: Tracker, https://github.com/MapIV/pypcd4/issues
 Author-email: urasakikeisuke <keisuke.urasaki@map4.jp>
 License: BSD 3-Clause License
         
@@ -45,116 +45,168 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8.2
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: pydantic<=2.5.2,>=1.10.8
 Requires-Dist: python-lzf>=0.2.4
 Provides-Extra: dev
-Requires-Dist: black; extra == 'dev'
-Requires-Dist: isort; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: setuptools-scm; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # pypcd4
 
 ## Description
 
 pypcd4 is a modern reimagining of the original [pypcd](https://github.com/dimatura/pypcd) library,
 offering enhanced capabilities and performance for working with Point Cloud Data (PCD) files.
 
 This library builds upon the foundation laid by the original pypcd while incorporating modern
 Python3 syntax and methodologies to provide a more efficient and user-friendly experience.
 
-## Install
+## Installation
 
-You can install pypcd4 via pip,
+To get started with `pypcd4`, install it using pip:
 
 ```shell
 pip install pypcd4
 ```
 
-## How to use
+## Usage
 
-### Import pypcd4
+Let’s walk through some examples of how you can use pypcd4:
+
+### Getting Started
+
+First, import the PointCloud class from pypcd4:
 
 ```python
 from pypcd4 import PointCloud
 ```
 
-### Read from .pcd file
+### Working with .pcd Files
+
+If you have a .pcd file, you can read it into a PointCloud object:
 
 ```python
-pc: PointCloud = PointCloud.from_path("xyzi.pcd")
+pc: PointCloud = PointCloud.from_path("point_cloud.pcd")
+
+pc.fields
+# ('x', 'y', 'z', 'intensity')
 ```
 
-### PointCloud -> NumPy array
+### Converting Between PointCloud and NumPy Array
+
+You can convert a PointCloud to a NumPy array:
 
 ```python
 array: np.ndarray = pc.numpy()
 
 array.shape
 # (1000, 4)
 ```
 
-### NumPy array -> PointCloud
+You can also specify the fields you want to include in the conversion:
 
 ```python
-# Depends on number of features of your array
+array: np.ndarray = pc.numpy(("x", "y", "z"))
+
+array.shape
+# (1000, 3)
+```
+
+And you can convert a NumPy array back to a PointCloud.
+The method you use depends on the fields in your array:
 
-# If PointXYZI,
+```python
+# If the array has x, y, z, and intensity fields,
 pc = PointCloud.from_xyzi_points(array)
 
-# If PointXYZL,
+# Or if the array has x, y, z, and label fields,
 pc = PointCloud.from_xyzl_points(array, label_type=np.uint32)
 ```
 
-### ROS PointCloud2 Message -> PointCloud
+#### Creating Custom Conversion Methods
+
+If you can’t find your preferred point type in the pre-defined conversion methods,
+you can create your own:
+
+```python
+fields = ("x", "y", "z", "intensity", "new_field")
+types = (np.float32, np.float32, np.float32, np.float32, np.float64)
+
+pc = PointCloud.from_points(array, fields, types)
+```
+
+### Working with ROS PointCloud2 Messages
 
-Added in v0.4.0
+As of v0.4.0, you can convert a ROS PointCloud2 Message to a PointCloud:
 
 ```python
 def callback(msg):
     pc = PointCloud.from_msg(msg)
 
     pc.fields
     # ("x", "y", "z", "intensity", "ring", "time")
 ```
 
-### Create custom conversion method
+### Concatenating Two PointClouds
+
+The `pypcd4` supports concatenating two `PointCloud` objects together using the `+` operator.
+This can be very useful when you want to merge two point clouds into one.
 
-If you cannot find preferred point type in pre-defined conversion methods,
-you can create it easily like,
+Here's how you can use it:
 
 ```python
-fields = ("x", "y", "z", "intensity", "new_field")
-types = (np.float32, np.float32, np.float32, np.float32, np.float64)
+pc1: PointCloud = PointCloud.from_path("xyzi1.pcd")
+pc2: PointCloud = PointCloud.from_path("xyzi2.pcd")
 
-pc = PointCloud.from_points(array, fields, types)
+# Concatenate two PointClouds
+pc3: PointCloud = pc1 + pc2
+```
+
+Please note that the two PointCloud objects must have the same fields and types. If they don’t, a `ValueError` will be raised.
+
+### Filtering a PointCloud
+
+The `pypcd4` library provides a convenient way to filter a `PointCloud` using a mask.
+Here's an example of how you can use it:
+
+```python
+# Create a random PointCloud
+pc = PointCloud.from_xyz_points(np.random.rand(100, 3))
+
+# Create a mask
+mask = (pc.pc_data["x"] > 0.5) & (pc.pc_data["y"] < 0.5)
+
+# Apply the mask to the PointCloud
+filtered_pc = pc[mask]
+
+# The filtered PointCloud only includes the points that match the mask
+print(filtered_pc.numpy())
 ```
 
-### Save as .pcd file
+Please note that the mask must be a 1-dimensional array. If it’s not, a `ValueError` will be raised.
+
+### Saving Your Work
+
+Finally, you can save your PointCloud as a .pcd file:
 
 ```python
 pc.save("nice_point_cloud.pcd")
 ```
 
 ## License
 
 The library was rewritten and does not borrow any code from the original [pypcd](https://github.com/dimatura/pypcd) library.
 Since it was heavily inspired by the original author's work, we extend his original BSD 3-Clause License and include his Copyright notice.
-
-## TODO
-
-- [ ] Support ROS message conversion
-  - [x] ROS message -> PointCloud
-  - [ ] PointCloud  -> ROS message
-- [ ] Visualization
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


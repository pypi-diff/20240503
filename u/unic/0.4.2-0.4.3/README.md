# Comparing `tmp/unic-0.4.2.tar.gz` & `tmp/unic-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unic-0.4.2.tar", max compression
+gzip compressed data, was "unic-0.4.3.tar", max compression
```

## Comparing `unic-0.4.2.tar` & `unic-0.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1064 2023-08-02 13:34:57.957684 unic-0.4.2/LICENSE
--rw-r--r--   0        0        0      841 2024-01-29 11:49:12.939532 unic-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2398 2024-01-29 11:47:57.829122 unic-0.4.2/README.md
--rw-r--r--   0        0        0      897 2023-12-11 12:31:51.919297 unic-0.4.2/unic/__init__.py
--rw-r--r--   0        0        0      912 2023-12-11 13:01:08.512829 unic-0.4.2/unic/configs/metirc_system/settings.toml
--rw-r--r--   0        0        0      244 2023-08-02 13:34:57.987478 unic-0.4.2/unic/configs/timeunit/settings.toml
--rw-r--r--   0        0        0     2232 2023-08-02 13:34:57.987478 unic-0.4.2/unic/configs/timezone/settings.toml
--rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.4.2/unic/length_unit/metric_system/__init__.py
--rw-r--r--   0        0        0     1128 2024-01-23 12:43:39.352115 unic-0.4.2/unic/length_unit/metric_system/metric_system_model.py
--rw-r--r--   0        0        0        0 2023-08-08 15:37:47.030079 unic-0.4.2/unic/time_unit/datetime/__init__.py
--rw-r--r--   0        0        0     1853 2024-01-29 11:46:46.867410 unic-0.4.2/unic/time_unit/datetime/datetime_model.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.4.2/unic/time_unit/time/__init__.py
--rw-r--r--   0        0        0     1152 2023-10-22 14:50:30.117384 unic-0.4.2/unic/time_unit/time/time_model.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:58.002017 unic-0.4.2/unic/time_unit/unixtime/__init__.py
--rw-r--r--   0        0        0     1346 2023-11-12 06:03:34.687599 unic-0.4.2/unic/time_unit/unixtime/unixtime_model.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.2/unic/utils/__init__.py
--rw-r--r--   0        0        0      391 2023-10-29 05:14:04.780174 unic-0.4.2/unic/utils/config_parser.py
--rw-r--r--   0        0        0     3739 2024-01-29 11:47:01.284876 unic-0.4.2/unic/utils/validators.py
--rw-r--r--   0        0        0     3046 1970-01-01 00:00:00.000000 unic-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-02 13:34:57.957684 unic-0.4.3/LICENSE
+-rw-r--r--   0        0        0      888 2024-02-09 13:34:52.408369 unic-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2398 2024-01-29 11:47:57.829122 unic-0.4.3/README.md
+-rw-r--r--   0        0        0      897 2023-12-11 12:31:51.919297 unic-0.4.3/unic/__init__.py
+-rw-r--r--   0        0        0      912 2023-12-11 13:01:08.512829 unic-0.4.3/unic/configs/metirc_system/settings.toml
+-rw-r--r--   0        0        0      244 2023-08-02 13:34:57.987478 unic-0.4.3/unic/configs/timeunit/settings.toml
+-rw-r--r--   0        0        0     2232 2023-08-02 13:34:57.987478 unic-0.4.3/unic/configs/timezone/settings.toml
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.4.3/unic/length_unit/metric_system/__init__.py
+-rw-r--r--   0        0        0     1128 2024-01-23 12:43:39.352115 unic-0.4.3/unic/length_unit/metric_system/metric_system_model.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:37:47.030079 unic-0.4.3/unic/time_unit/datetime/__init__.py
+-rw-r--r--   0        0        0     1853 2024-01-29 11:46:46.867410 unic-0.4.3/unic/time_unit/datetime/datetime_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.4.3/unic/time_unit/time/__init__.py
+-rw-r--r--   0        0        0     1107 2024-01-29 12:03:05.141190 unic-0.4.3/unic/time_unit/time/time_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.002017 unic-0.4.3/unic/time_unit/unixtime/__init__.py
+-rw-r--r--   0        0        0     1310 2024-02-09 13:22:45.717612 unic-0.4.3/unic/time_unit/unixtime/unixtime_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.3/unic/utils/__init__.py
+-rw-r--r--   0        0        0      391 2023-10-29 05:14:04.780174 unic-0.4.3/unic/utils/config_parser.py
+-rw-r--r--   0        0        0     3040 2024-02-08 14:06:23.439103 unic-0.4.3/unic/utils/validators.py
+-rw-r--r--   0        0        0     3097 1970-01-01 00:00:00.000000 unic-0.4.3/PKG-INFO
```

### Comparing `unic-0.4.2/LICENSE` & `unic-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unic-0.4.2/pyproject.toml` & `unic-0.4.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unic"
-version = "0.4.2"
+version = "0.4.3"
 description = "Python package for converting various units."
 authors = ["Subretu"]
 maintainers = ["Subretu"]
 license = "MIT"
 readme = 'README.md'
 repository = 'https://github.com/subretu/unic'
 keywords = ['unit', 'convert', 'time', 'timestamp', 'length']
@@ -12,14 +12,15 @@
 classifiers=[
     'License :: OSI Approved :: MIT License',
 
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 toml = "^0.10.2"
 pydantic = "^2.1"
```

### Comparing `unic-0.4.2/README.md` & `unic-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `unic-0.4.2/unic/__init__.py` & `unic-0.4.3/unic/__init__.py`

 * *Files identical despite different names*

### Comparing `unic-0.4.2/unic/configs/metirc_system/settings.toml` & `unic-0.4.3/unic/configs/metirc_system/settings.toml`

 * *Files identical despite different names*

### Comparing `unic-0.4.2/unic/configs/timezone/settings.toml` & `unic-0.4.3/unic/configs/timezone/settings.toml`

 * *Files identical despite different names*

### Comparing `unic-0.4.2/unic/length_unit/metric_system/metric_system_model.py` & `unic-0.4.3/unic/length_unit/metric_system/metric_system_model.py`

 * *Files identical despite different names*

### Comparing `unic-0.4.2/unic/time_unit/datetime/datetime_model.py` & `unic-0.4.3/unic/time_unit/datetime/datetime_model.py`

 * *Files identical despite different names*

### Comparing `unic-0.4.2/unic/time_unit/time/time_model.py` & `unic-0.4.3/unic/time_unit/time/time_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,16 +14,14 @@
             raise ValueError(e.errors()[0]["msg"])
 
         parameter = config_parser.parse_toml("timeunit")
         data = float(input_data.data * Fraction(parameter[from_unit][to_unit]))
 
         return data
 
-    def check_parameter_count(self, from_unit: str, to_unit: str) -> bool:
+    def check_parameter_count(self, from_unit: str, to_unit: str) -> None:
         if from_unit is None and to_unit is None:
             raise ValueError("Both 'from_unit' and 'to_unit' arguments are required.")
-        elif from_unit is None:
-            raise ValueError("The 'from_unit' argument is required.")
-        elif to_unit is None:
-            raise ValueError("The 'to_unit' argument is required.")
-        else:
-            return
+        if from_unit is None or to_unit is None:
+            raise ValueError(
+                f"The '{'from_unit' if from_unit is None else 'to_unit'}' argument is required."
+            )
```

### Comparing `unic-0.4.2/unic/time_unit/unixtime/unixtime_model.py` & `unic-0.4.3/unic/time_unit/unixtime/unixtime_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,13 +29,11 @@
         dt_unixtime = (
             str(int(dt_timestamp.replace(tzinfo=timezone.utc).timestamp()))
         ) + milisecond
 
         return int(dt_unixtime)
 
     def check_parameter_count(self, parameter: dict) -> None:
-        if len(parameter) <= 1:
-            return
-        else:
+        if len(parameter) > 1:
             raise ValueError(
                 "Too many parameter.If specify parameters to the function,the number should be one."
             )
```

### Comparing `unic-0.4.2/unic/utils/validators.py` & `unic-0.4.3/unic/utils/validators.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,67 @@
-from pydantic import (
-    BaseModel,
-    StrictFloat,
-    field_validator,
-    StrictInt,
-    StrictStr,
-)
+from pydantic import BaseModel, StrictFloat, field_validator, StrictInt, StrictStr
 from typing import Union
 from datetime import datetime
 from unic.utils import config_parser
 
 
-class TimeModelValidator(BaseModel):
-    # Prevent automatic conversion
+class ValidatorMixin:
+    @classmethod
+    def validate_units(cls, v, valid_units, parameter):
+        if v not in valid_units:
+            raise ValueError(
+                f"{v} is invalid value for parameter: {parameter}. Allowed values are {valid_units}."
+            )
+        return v
+
+    @classmethod
+    def validate_timezone(cls, v):
+        valid_timezones = config_parser.parse_toml("timezone")
+        if v not in valid_timezones.keys() and v is not None:
+            raise ValueError(f"{v} is invalid value for parameter: tz.")
+        return v
+
+
+class TimeModelValidator(BaseModel, ValidatorMixin):
     data: Union[StrictInt, StrictFloat]
     from_unit: StrictStr
     to_unit: StrictStr
 
     @field_validator("from_unit")
     def from_unit_check(cls, v):
-        valid_units = ["msec", "sec", "min", "hour"]
-        if v not in valid_units:
-            raise ValueError(
-                f"{v} is invalid value for parameter: from_unit. Allowed values are {valid_units}."
-            )
-        return v
+        return cls.validate_units(v, ["msec", "sec", "min", "hour"], "from_unit")
 
     @field_validator("to_unit")
     def to_unit_check(cls, v):
-        valid_units = ["msec", "sec", "min", "hour"]
-        if v not in valid_units:
-            raise ValueError(
-                f"{v} is invalid value for parameter: to_unit. Allowed values are {valid_units}."
-            )
-        return v
+        return cls.validate_units(v, ["msec", "sec", "min", "hour"], "to_unit")
 
 
-class DatetimeModelValidator(BaseModel):
-    # Prevent automatic conversion
+class DatetimeModelValidator(BaseModel, ValidatorMixin):
     data: StrictInt
     format: StrictStr
     tz: Union[StrictStr, None]
 
     @field_validator("data")
     def data_check(cls, v):
         digits = len(str(abs(v)))
-
         if digits == 10 or digits == 13:
             return v
         else:
             raise ValueError("Unixtime digits is 10 or 13.")
 
     @field_validator("format")
     def format_check(cls, v):
-        valid_formats = ["datetime", "date"]
-        if v not in valid_formats:
-            raise ValueError(
-                f"{v} is invalid value for parameter: format. Allowed values are {valid_formats}."
-            )
-        return v
+        return cls.validate_units(v, ["datetime", "date"], "format")
 
     @field_validator("tz")
     def timezone_check(cls, v):
-        valid_timezones = config_parser.parse_toml("timezone")
-        if v not in valid_timezones.keys() and v is not None:
-            raise ValueError(f"{v} is invalid value for parameter: tz.")
-        return v
+        return cls.validate_timezone(v)
 
 
-class UnixtimeModelValidator(BaseModel):
-    # Prevent automatic conversion
+class UnixtimeModelValidator(BaseModel, ValidatorMixin):
     data: StrictStr
     tz: Union[StrictStr, None]
 
     @field_validator("data")
     def data_check(cls, v):
         date_formats = ["%Y-%m-%d %H:%M:%S", "%Y-%m-%d %H:%M:%S.%f"]
         for date_format in date_formats:
@@ -83,36 +72,26 @@
                 continue
         raise ValueError(
             f"'{v}' is invalid date format. Allowed formats are {date_formats}."
         )
 
     @field_validator("tz")
     def timezone_check(cls, v):
-        valid_timezones = config_parser.parse_toml("timezone")
-        if v not in valid_timezones.keys() and v is not None:
-            raise ValueError(f"{v} is invalid value for parameter: tz.")
-        return v
+        return cls.validate_timezone(v)
 
 
-class MetricSystemModelValidator(BaseModel):
-    # Prevent automatic conversion
+class MetricSystemModelValidator(BaseModel, ValidatorMixin):
     data: Union[StrictInt, StrictFloat]
     from_unit: StrictStr
     to_unit: StrictStr
 
     @field_validator("from_unit")
     def from_unit_check(cls, v):
-        valid_units = ["nm", "um", "mm", "cm", "m", "km", "Mm", "Gm", "Tm"]
-        if v not in valid_units:
-            raise ValueError(
-                f"{v} is invalid value for parameter: from_unit. Allowed values are {valid_units}."
-            )
-        return v
+        return cls.validate_units(
+            v, ["nm", "um", "mm", "cm", "m", "km", "Mm", "Gm", "Tm"], "from_unit"
+        )
 
     @field_validator("to_unit")
     def to_unit_check(cls, v):
-        valid_units = ["nm", "um", "mm", "cm", "m", "km", "Mm", "Gm", "Tm"]
-        if v not in valid_units:
-            raise ValueError(
-                f"{v} is invalid value for parameter: to_unit. Allowed values are {valid_units}."
-            )
-        return v
+        return cls.validate_units(
+            v, ["nm", "um", "mm", "cm", "m", "km", "Mm", "Gm", "Tm"], "to_unit"
+        )
```

### Comparing `unic-0.4.2/PKG-INFO` & `unic-0.4.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: unic
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python package for converting various units.
 Home-page: https://github.com/subretu/unic
 License: MIT
 Keywords: unit,convert,time,timestamp,length
 Author: Subretu
 Maintainer: Subretu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=2.1,<3.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Repository, https://github.com/subretu/unic
 Description-Content-Type: text/markdown
 
 ![Python minimum version](https://img.shields.io/badge/Python-3.8%2B-brightgreen)
 [![pytest](https://github.com/subretu/unic/actions/workflows/pytest.yml/badge.svg)](https://github.com/subretu/unic/actions/workflows/pytest.yml)
```


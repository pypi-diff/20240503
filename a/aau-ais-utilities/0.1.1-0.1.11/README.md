# Comparing `tmp/aau_ais_utilities-0.1.1.tar.gz` & `tmp/aau_ais_utilities-0.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aau_ais_utilities-0.1.1.tar", last modified: Mon Apr 29 09:56:48 2024, max compression
+gzip compressed data, was "aau_ais_utilities-0.1.11.tar", last modified: Fri May  3 12:25:43 2024, max compression
```

## Comparing `aau_ais_utilities-0.1.1.tar` & `aau_ais_utilities-0.1.11.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      145 2024-04-19 08:48:38.959957 aau_ais_utilities-0.1.1/README.md
--rw-r--r--   0        0        0      628 2024-04-29 09:56:48.375833 aau_ais_utilities-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 12:04:56.661628 aau_ais_utilities-0.1.1/src/aau_ais_utilities/__init__.py
--rw-r--r--   0        0        0      158 2024-04-25 09:08:00.197116 aau_ais_utilities-0.1.1/src/aau_ais_utilities/connections/__init__.py
--rw-r--r--   0        0        0      504 2024-04-29 09:43:50.319740 aau_ais_utilities-0.1.1/src/aau_ais_utilities/connections/engine_settings.py
--rw-r--r--   0        0        0     1762 2024-04-17 12:06:39.000000 aau_ais_utilities-0.1.1/src/aau_ais_utilities/connections/postgresql_connection.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:29.563946 aau_ais_utilities-0.1.1/src/aau_ais_utilities/lookup/__init__.py
--rw-r--r--   0        0        0    18270 2024-04-24 11:56:27.025069 aau_ais_utilities-0.1.1/src/aau_ais_utilities/lookup/mmsi.py
--rw-r--r--   0        0        0      111 2024-04-17 06:44:56.872198 aau_ais_utilities-0.1.1/src/aau_ais_utilities/validate/__init__.py
--rw-r--r--   0        0        0     2792 2024-04-17 06:44:56.873437 aau_ais_utilities-0.1.1/src/aau_ais_utilities/validate/imo.py
--rw-r--r--   0        0        0     1136 2024-04-17 06:44:56.873437 aau_ais_utilities-0.1.1/src/aau_ais_utilities/validate/mmsi.py
--rw-r--r--   0        0        0     1253 2024-04-17 06:44:56.874519 aau_ais_utilities-0.1.1/src/aau_ais_utilities/validate/validator.py
--rw-r--r--   0        0        0     1534 2024-04-24 11:56:27.052662 aau_ais_utilities-0.1.1/tests/validate/test_imo.py
--rw-r--r--   0        0        0        0 2024-04-10 14:19:47.264802 aau_ais_utilities-0.1.1/tests/validate/test_mmsi.py
--rw-r--r--   0        0        0        0 2024-04-17 06:44:56.878541 aau_ais_utilities-0.1.1/tests/validate/test_validator.py
--rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 aau_ais_utilities-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      135 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.11/README.md
+-rw-r--r--   0        0        0      629 2024-05-03 12:25:43.098286 aau_ais_utilities-0.1.11/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.11/src/aau_ais_utilities/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.11/src/aau_ais_utilities/connections/__init__.py
+-rw-r--r--   0        0        0      482 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.11/src/aau_ais_utilities/connections/engine_settings.py
+-rw-r--r--   0        0        0     1812 2024-05-03 12:25:02.811676 aau_ais_utilities-0.1.11/src/aau_ais_utilities/connections/postgresql_connection.py
+-rw-r--r--   0        0        0        0 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.11/src/aau_ais_utilities/lookup/__init__.py
+-rw-r--r--   0        0        0    17629 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.11/src/aau_ais_utilities/lookup/mmsi.py
+-rw-r--r--   0        0        0      107 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.11/src/aau_ais_utilities/validate/__init__.py
+-rw-r--r--   0        0        0     2695 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.11/src/aau_ais_utilities/validate/imo.py
+-rw-r--r--   0        0        0     1091 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.11/src/aau_ais_utilities/validate/mmsi.py
+-rw-r--r--   0        0        0     1208 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.11/src/aau_ais_utilities/validate/validator.py
+-rw-r--r--   0        0        0     1478 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.11/tests/validate/test_imo.py
+-rw-r--r--   0        0        0        0 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.11/tests/validate/test_mmsi.py
+-rw-r--r--   0        0        0        0 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.11/tests/validate/test_validator.py
+-rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 aau_ais_utilities-0.1.11/PKG-INFO
```

### Comparing `aau_ais_utilities-0.1.1/pyproject.toml` & `aau_ais_utilities-0.1.11/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aau-ais-utilities"
-version = "0.1.1"
+version = "0.1.11"
 description = "Utilities for working with the AAU AIS database."
 authors = [
     { name = "Mikael Vind Mikkelsen", email = "mvmi@cs.aau.dk" },
 ]
 dependencies = [
     "sqlalchemy==2.0.*",
     "pydantic-settings==2.2.*",
```

### Comparing `aau_ais_utilities-0.1.1/src/aau_ais_utilities/validate/mmsi.py` & `aau_ais_utilities-0.1.11/src/aau_ais_utilities/validate/mmsi.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-"""Module for MMSI number validation."""
-from .validator import Validator
-
-
-class MMSIValidator(Validator):
-
-    @property
-    def error_messages(self) -> dict:
-        return {
-            "incorrect_format": "Incorrect Format - MMSI number must be 9 digits long. May include the prefix 'MMSI'."
-        }
-
-    def __init__(self) -> None:
-        """Initialize the MMSIValidator class."""
-        super().__init__()
-
-    def validate(self, mmsi: str) -> bool:
-        """Validate MMSI number.
-
-        Args:
-            mmsi (str): MMSI number to validate.
-        """
-
-        mmsi = self._parse_mmsi(mmsi)
-
-        if not mmsi.isdigit() or len(mmsi) != 9:
-            self._add_error_to_log("incorrect_format", mmsi)
-            return False
-
-        return True
-
-    @staticmethod
-    def _parse_mmsi(mmsi: str) -> str:
-        """Parse MMSI number, removing any whitespace or MMSI prefix.
-
-        Args:
-            mmsi (str): MMSI number to parse.
-        """
-
-        mmsi = mmsi.replace(" ", "")
-
-        if mmsi.startswith("MMSI"):
-            mmsi = mmsi[4:]
-
-        return mmsi
+"""Module for MMSI number validation."""
+from .validator import Validator
+
+
+class MMSIValidator(Validator):
+
+    @property
+    def error_messages(self) -> dict:
+        return {
+            "incorrect_format": "Incorrect Format - MMSI number must be 9 digits long. May include the prefix 'MMSI'."
+        }
+
+    def __init__(self) -> None:
+        """Initialize the MMSIValidator class."""
+        super().__init__()
+
+    def validate(self, mmsi: str) -> bool:
+        """Validate MMSI number.
+
+        Args:
+            mmsi (str): MMSI number to validate.
+        """
+
+        mmsi = self._parse_mmsi(mmsi)
+
+        if not mmsi.isdigit() or len(mmsi) != 9:
+            self._add_error_to_log("incorrect_format", mmsi)
+            return False
+
+        return True
+
+    @staticmethod
+    def _parse_mmsi(mmsi: str) -> str:
+        """Parse MMSI number, removing any whitespace or MMSI prefix.
+
+        Args:
+            mmsi (str): MMSI number to parse.
+        """
+
+        mmsi = mmsi.replace(" ", "")
+
+        if mmsi.startswith("MMSI"):
+            mmsi = mmsi[4:]
+
+        return mmsi
```

### Comparing `aau_ais_utilities-0.1.1/src/aau_ais_utilities/validate/validator.py` & `aau_ais_utilities-0.1.11/src/aau_ais_utilities/validate/validator.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from abc import ABC, abstractmethod
-from datetime import datetime
-
-
-class Validator(ABC):
-    """Abstract class for data validation.
-
-    Contains methods for validating data and logging errors to a log if validation fails.
-    Log messages are stored in the format [datetime, data, error_message].
-    """
-
-    @property
-    @abstractmethod
-    def error_messages(self) -> dict:
-        pass
-
-    def __init__(self):
-        self.log = []
-
-    @abstractmethod
-    def validate(self, data) -> bool:
-        pass
-
-    def _add_error_to_log(self, error_key: str, data: str) -> None:
-        """Add a message to the log.
-
-        Args:
-            error_key (str): The message to add to the log.
-        """
-        log_message = self.error_messages.get(error_key)
-
-        if log_message is None:
-            raise ValueError(f"Error message '{error_key}' not found.")
-
-        self.log.append([datetime.now().strftime("%Y-%m-%d %H:%M:%S"), data, log_message])
-
-    def get_log(self) -> list[list[datetime, str, str]]:
-        """Return the log."""
-
-        return self.log
-
-    def get_last_error(self) -> list[datetime, str, str]:
-        """Return the last error in the log."""
-
-        return self.log[-1]
+from abc import ABC, abstractmethod
+from datetime import datetime
+
+
+class Validator(ABC):
+    """Abstract class for data validation.
+
+    Contains methods for validating data and logging errors to a log if validation fails.
+    Log messages are stored in the format [datetime, data, error_message].
+    """
+
+    @property
+    @abstractmethod
+    def error_messages(self) -> dict:
+        pass
+
+    def __init__(self):
+        self.log = []
+
+    @abstractmethod
+    def validate(self, data) -> bool:
+        pass
+
+    def _add_error_to_log(self, error_key: str, data: str) -> None:
+        """Add a message to the log.
+
+        Args:
+            error_key (str): The message to add to the log.
+        """
+        log_message = self.error_messages.get(error_key)
+
+        if log_message is None:
+            raise ValueError(f"Error message '{error_key}' not found.")
+
+        self.log.append([datetime.now().strftime("%Y-%m-%d %H:%M:%S"), data, log_message])
+
+    def get_log(self) -> list[list[datetime, str, str]]:
+        """Return the log."""
+
+        return self.log
+
+    def get_last_error(self) -> list[datetime, str, str]:
+        """Return the last error in the log."""
+
+        return self.log[-1]
```


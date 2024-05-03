# Comparing `tmp/aau_ais_dipaal-0.1.21.tar.gz` & `tmp/aau_ais_dipaal-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aau_ais_dipaal-0.1.21.tar", last modified: Mon Apr 29 09:59:59 2024, max compression
+gzip compressed data, was "aau_ais_dipaal-0.1.22.tar", last modified: Fri May  3 12:26:08 2024, max compression
```

## Comparing `aau_ais_dipaal-0.1.21.tar` & `aau_ais_dipaal-0.1.22.tar`

### file list

```diff
@@ -1,15 +1,13 @@
--rw-r--r--   0        0        0      139 2024-04-18 10:19:07.540695 aau_ais_dipaal-0.1.21/README.md
--rw-r--r--   0        0        0      671 2024-04-29 09:59:59.509815 aau_ais_dipaal-0.1.21/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 11:59:12.781590 aau_ais_dipaal-0.1.21/src/dipaal/__init__.py
--rw-r--r--   0        0        0      244 2024-04-17 14:41:48.579028 aau_ais_dipaal-0.1.21/src/dipaal/convert/__init__.py
--rw-r--r--   0        0        0     1207 2024-04-25 09:28:54.746754 aau_ais_dipaal-0.1.21/src/dipaal/convert/callsign.py
--rw-r--r--   0        0        0     1544 2024-04-29 09:09:13.050378 aau_ais_dipaal-0.1.21/src/dipaal/convert/converter.py
--rw-r--r--   0        0        0     1177 2024-04-25 09:28:54.789569 aau_ais_dipaal-0.1.21/src/dipaal/convert/imo.py
--rw-r--r--   0        0        0     1187 2024-04-25 09:28:54.736736 aau_ais_dipaal-0.1.21/src/dipaal/convert/mmsi.py
--rw-r--r--   0        0        0      152 2024-04-23 11:19:37.881658 aau_ais_dipaal-0.1.21/src/dipaal/export/__init__.py
--rw-r--r--   0        0        0     5913 2024-04-24 11:38:06.792730 aau_ais_dipaal-0.1.21/src/dipaal/export/exporter.py
--rw-r--r--   0        0        0     4077 2024-04-24 12:04:56.635681 aau_ais_dipaal-0.1.21/src/dipaal/export/map_exporter.py
--rw-r--r--   0        0        0        0 2024-04-23 14:21:24.000145 aau_ais_dipaal-0.1.21/src/dipaal/export/sql/map_exporter/exists/enc.sql
--rw-r--r--   0        0        0        0 2024-04-23 14:21:52.095786 aau_ais_dipaal-0.1.21/src/dipaal/export/sql/map_exporter/exists/ship_type.sql
--rw-r--r--   0        0        0      401 2024-04-29 09:31:48.467158 aau_ais_dipaal-0.1.21/src/dipaal/settings.py
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 aau_ais_dipaal-0.1.21/PKG-INFO
+-rw-r--r--   0        0        0      130 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.22/README.md
+-rw-r--r--   0        0        0      692 2024-05-03 12:26:08.257387 aau_ais_dipaal-0.1.22/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.22/src/dipaal/__init__.py
+-rw-r--r--   0        0        0      237 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.22/src/dipaal/convert/__init__.py
+-rw-r--r--   0        0        0     1161 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.22/src/dipaal/convert/callsign.py
+-rw-r--r--   0        0        0     1540 2024-05-03 12:25:02.814192 aau_ais_dipaal-0.1.22/src/dipaal/convert/converter.py
+-rw-r--r--   0        0        0     1132 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.22/src/dipaal/convert/imo.py
+-rw-r--r--   0        0        0     1142 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.22/src/dipaal/convert/mmsi.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:25:02.814192 aau_ais_dipaal-0.1.22/src/dipaal/export/__init__.py
+-rw-r--r--   0        0        0     7939 2024-05-03 12:25:02.815185 aau_ais_dipaal-0.1.22/src/dipaal/export/map_exporter.py
+-rw-r--r--   0        0        0     5863 2024-05-03 12:25:02.815185 aau_ais_dipaal-0.1.22/src/dipaal/export/sql_map.py
+-rw-r--r--   0        0        0      389 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.22/src/dipaal/settings.py
+-rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 aau_ais_dipaal-0.1.22/PKG-INFO
```

### Comparing `aau_ais_dipaal-0.1.21/pyproject.toml` & `aau_ais_dipaal-0.1.22/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [project]
 name = "aau-ais-dipaal"
-version = "0.1.21"
+version = "0.1.22"
 description = "TODO: Add a description of your project."
 authors = [
     { name = "Mikael Vind Mikkelsen", email = "mvmi@cs.aau.dk" },
 ]
 dependencies = [
     "aau-ais-utilities==0.1.*",
     "pydantic==2.7.*",
     "pydantic-settings==2.2.*",
     "jinjasql==0.1.*",
+    "jinja2==3.0.*",
 ]
 requires-python = "==3.12.*"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `aau_ais_dipaal-0.1.21/src/dipaal/convert/callsign.py` & `aau_ais_dipaal-0.1.22/src/dipaal/convert/callsign.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from .converter import Converter
-from sqlalchemy import Engine
-from dipaal.settings import get_dipaal_engine
-
-
-class CallsignConverter(Converter):
-    """Convert callsigns to other formats.
-
-    This class requires a connection to a database containing the relevant data.
-    """
-
-    def __init__(self, engine: Engine = get_dipaal_engine()) -> None:
-        super().__init__(engine)
-
-    def to_mmsi(self, callsign: str) -> str:
-        """Convert a callsign to an MMSI number.
-
-        Args:
-            callsign: The callsign to convert.
-
-        Returns:
-            The MMSI number.
-        """
-
-        return self.convert_within_table(
-            from_format="callsign",
-            to_format="mmsi",
-            table="public.dim_ship",
-            value=callsign)
-
-
-    def to_imo(self, callsign: str) -> str:
-        """Convert a callsign to an IMO number.
-
-        Args:
-            callsign: The callsign to convert.
-
-        Returns:
-            The IMO number.
-        """
-
-        return self.convert_within_table(
-            from_format="callsign",
-            to_format="imo",
-            table="public.dim_ship",
-            value=callsign)
+from .converter import Converter
+from sqlalchemy import Engine
+from dipaal.settings import get_dipaal_engine
+
+
+class CallsignConverter(Converter):
+    """Convert callsigns to other formats.
+
+    This class requires a connection to a database containing the relevant data.
+    """
+
+    def __init__(self, engine: Engine = get_dipaal_engine()) -> None:
+        super().__init__(engine)
+
+    def to_mmsi(self, callsign: str) -> str:
+        """Convert a callsign to an MMSI number.
+
+        Args:
+            callsign: The callsign to convert.
+
+        Returns:
+            The MMSI number.
+        """
+
+        return self.convert_within_table(
+            from_format="callsign",
+            to_format="mmsi",
+            table="public.dim_ship",
+            value=callsign)
+
+
+    def to_imo(self, callsign: str) -> str:
+        """Convert a callsign to an IMO number.
+
+        Args:
+            callsign: The callsign to convert.
+
+        Returns:
+            The IMO number.
+        """
+
+        return self.convert_within_table(
+            from_format="callsign",
+            to_format="imo",
+            table="public.dim_ship",
+            value=callsign)
```

### Comparing `aau_ais_dipaal-0.1.21/src/dipaal/convert/converter.py` & `aau_ais_dipaal-0.1.22/src/dipaal/convert/converter.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         """
 
         # TODO: Change the SQL query so that it ignores non-vessels (e.g. ports, etc.).
         #  Currently, the query will return the most recent value for the given input, regardless of the type of vessel.
         #  Meaning that IMO to MMSI might have a MID in the 800 range, which are handheld radios.
         sql_statement = f"SELECT {to_format} FROM {table} WHERE {from_format} = :VALUE ORDER BY ship_id DESC LIMIT 1;"
 
-        result = self.connection.execute_sql(
+        result = self.connection.execute(
             sql=sql_statement,
             params={'VALUE': value}
         ).fetchone()
 
         if result is None:
             return "No value found in the database for the given input."
```

### Comparing `aau_ais_dipaal-0.1.21/src/dipaal/convert/imo.py` & `aau_ais_dipaal-0.1.22/src/dipaal/convert/imo.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from .converter import Converter
-from dipaal.settings import get_dipaal_engine
-from sqlalchemy import Engine
-
-
-class IMOConverter(Converter):
-    """Convert IMO numbers to other formats.
-
-    This class requires a connection to a database containing the relevant data.
-    """
-
-    def __init__(self, engine: Engine = get_dipaal_engine()) -> None:
-        super().__init__(engine)
-
-    def to_mmsi(self, imo: str) -> str:
-        """Convert an IMO number to an MMSI number.
-
-        Args:
-            imo: The IMO number to convert.
-
-        Returns:
-            The MMSI number.
-        """
-
-        return self.convert_within_table(
-            from_format="imo",
-            to_format="mmsi",
-            table="public.dim_ship",
-            value=imo)
-
-    def to_callsign(self, imo: str) -> str:
-        """Convert an IMO number to a callsign.
-
-        Args:
-            imo: The IMO number to convert.
-
-        Returns:
-            The callsign.
-        """
-
-        return self.convert_within_table(
-            from_format="imo",
-            to_format="callsign",
-            table="public.dim_ship",
-            value=imo)
+from .converter import Converter
+from dipaal.settings import get_dipaal_engine
+from sqlalchemy import Engine
+
+
+class IMOConverter(Converter):
+    """Convert IMO numbers to other formats.
+
+    This class requires a connection to a database containing the relevant data.
+    """
+
+    def __init__(self, engine: Engine = get_dipaal_engine()) -> None:
+        super().__init__(engine)
+
+    def to_mmsi(self, imo: str) -> str:
+        """Convert an IMO number to an MMSI number.
+
+        Args:
+            imo: The IMO number to convert.
+
+        Returns:
+            The MMSI number.
+        """
+
+        return self.convert_within_table(
+            from_format="imo",
+            to_format="mmsi",
+            table="public.dim_ship",
+            value=imo)
+
+    def to_callsign(self, imo: str) -> str:
+        """Convert an IMO number to a callsign.
+
+        Args:
+            imo: The IMO number to convert.
+
+        Returns:
+            The callsign.
+        """
+
+        return self.convert_within_table(
+            from_format="imo",
+            to_format="callsign",
+            table="public.dim_ship",
+            value=imo)
```

### Comparing `aau_ais_dipaal-0.1.21/PKG-INFO` & `aau_ais_dipaal-0.1.22/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: aau-ais-dipaal
-Version: 0.1.21
+Version: 0.1.22
 Summary: TODO: Add a description of your project.
 Author-Email: Mikael Vind Mikkelsen <mvmi@cs.aau.dk>
 License: MIT
 Requires-Python: ==3.12.*
 Requires-Dist: aau-ais-utilities==0.1.*
 Requires-Dist: pydantic==2.7.*
 Requires-Dist: pydantic-settings==2.2.*
 Requires-Dist: jinjasql==0.1.*
+Requires-Dist: jinja2==3.0.*
 Description-Content-Type: text/markdown
 
 # Convert Package
 
 ## Overview
 
 ## Usage
```


# Comparing `tmp/ophyd-registry-1.1.0.tar.gz` & `tmp/ophyd_registry-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ophyd-registry-1.1.0.tar", last modified: Mon Mar 25 15:03:44 2024, max compression
+gzip compressed data, was "ophyd_registry-1.2.0.tar", last modified: Thu May  2 22:56:28 2024, max compression
```

## Comparing `ophyd-registry-1.1.0.tar` & `ophyd_registry-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-03-25 15:03:44.214060 ophyd-registry-1.1.0/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     7688 2024-03-25 15:03:44.214060 ophyd-registry-1.1.0/PKG-INFO
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     6751 2024-03-25 15:03:33.000000 ophyd-registry-1.1.0/README.md
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      895 2024-03-25 02:46:41.000000 ophyd-registry-1.1.0/pyproject.toml
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)       38 2024-03-25 15:03:44.214060 ophyd-registry-1.1.0/setup.cfg
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-03-25 15:03:44.212060 ophyd-registry-1.1.0/src/
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-03-25 15:03:44.214060 ophyd-registry-1.1.0/src/ophyd_registry.egg-info/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     7688 2024-03-25 15:03:44.000000 ophyd-registry-1.1.0/src/ophyd_registry.egg-info/PKG-INFO
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      377 2024-03-25 15:03:44.000000 ophyd-registry-1.1.0/src/ophyd_registry.egg-info/SOURCES.txt
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)        1 2024-03-25 15:03:44.000000 ophyd-registry-1.1.0/src/ophyd_registry.egg-info/dependency_links.txt
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)       56 2024-03-25 15:03:44.000000 ophyd-registry-1.1.0/src/ophyd_registry.egg-info/requires.txt
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)       14 2024-03-25 15:03:44.000000 ophyd-registry-1.1.0/src/ophyd_registry.egg-info/top_level.txt
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-03-25 15:03:44.213060 ophyd-registry-1.1.0/src/ophydregistry/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      126 2024-03-24 15:55:03.000000 ophyd-registry-1.1.0/src/ophydregistry/__init__.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      371 2023-12-22 00:11:16.000000 ophyd-registry-1.1.0/src/ophydregistry/exceptions.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)    17428 2024-03-25 15:03:33.000000 ophyd-registry-1.1.0/src/ophydregistry/registry.py
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-03-25 15:03:44.213060 ophyd-registry-1.1.0/src/ophydregistry/tests/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)    11652 2024-03-25 15:03:33.000000 ophyd-registry-1.1.0/src/ophydregistry/tests/test_instrument_registry.py
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-02 22:56:28.841963 ophyd_registry-1.2.0/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     9085 2024-05-02 22:56:28.840963 ophyd_registry-1.2.0/PKG-INFO
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     8066 2024-05-02 20:05:45.000000 ophyd_registry-1.2.0/README.md
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      921 2024-05-02 22:53:46.000000 ophyd_registry-1.2.0/pyproject.toml
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)       38 2024-05-02 22:56:28.841963 ophyd_registry-1.2.0/setup.cfg
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-02 22:56:28.838963 ophyd_registry-1.2.0/src/
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-02 22:56:28.840963 ophyd_registry-1.2.0/src/ophyd_registry.egg-info/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     9085 2024-05-02 22:56:28.000000 ophyd_registry-1.2.0/src/ophyd_registry.egg-info/PKG-INFO
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      377 2024-05-02 22:56:28.000000 ophyd_registry-1.2.0/src/ophyd_registry.egg-info/SOURCES.txt
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)        1 2024-05-02 22:56:28.000000 ophyd_registry-1.2.0/src/ophyd_registry.egg-info/dependency_links.txt
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)       76 2024-05-02 22:56:28.000000 ophyd_registry-1.2.0/src/ophyd_registry.egg-info/requires.txt
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)       14 2024-05-02 22:56:28.000000 ophyd_registry-1.2.0/src/ophyd_registry.egg-info/top_level.txt
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-02 22:56:28.839963 ophyd_registry-1.2.0/src/ophydregistry/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      126 2024-03-24 15:55:03.000000 ophyd_registry-1.2.0/src/ophydregistry/__init__.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      371 2023-12-22 00:11:16.000000 ophyd_registry-1.2.0/src/ophydregistry/exceptions.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)    19461 2024-05-02 21:23:07.000000 ophyd_registry-1.2.0/src/ophydregistry/registry.py
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-02 22:56:28.839963 ophyd_registry-1.2.0/src/ophydregistry/tests/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)    14037 2024-05-02 22:54:12.000000 ophyd_registry-1.2.0/src/ophydregistry/tests/test_instrument_registry.py
```

### Comparing `ophyd-registry-1.1.0/PKG-INFO` & `ophyd_registry-1.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: ophyd-registry
-Version: 1.1.0
-Summary: A registry to keep track of, and retrieve, Ophyd objects.
-Author-email: Mark Wolfman <wolfman@anl.gov>
-Project-URL: Homepage, https://github.com/spc-group/ophyd-registry
-Project-URL: Bug Tracker, https://github.com/spc-group/ophyd-registry/issues
-Keywords: synchrotron,xray,bluesky
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: System :: Hardware
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: ophyd
-Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
-
 # Ophyd Registry
 
 [![Python Tests](https://github.com/spc-group/ophyd-registry/actions/workflows/ci.yml/badge.svg)](https://github.com/spc-group/ophyd-registry/actions/workflows/ci.yml)
 
 A registry to keep track of, and retrieve, Ophyd objects.
 
 The **Ophyd registry** provides a way to keep track of the devices
@@ -224,14 +199,23 @@
 method:
 
 ```python
 
 registry.clear()
 ```
 
+To **remove disconnected devices** from the registry, use the ``pop_disconnected()`` method with an optional timeout:
+
+```python
+
+# Wait 5 seconds to give devices a chance to connect
+disconnected_devices = registry.pop_disconnected(timeout=5)
+
+```
+
 To **remove individual objects**, use either the *del* keyword, or the
 ``pop()`` method. These approaches work with either the
 ``OphydObject`` instance itself, or the instance's name:
 
 ```python
 
 # Just delete the item and move on
@@ -244,14 +228,47 @@
 # Remove the item and use it
 # (return a simulated motor if "motor1" is not in the registry)
 motor = registry.pop("motor1", ophyd.sim.motor)
 motor.set(5).wait()
 
 ```
 
+Keeping References
+------------------
+
+It may be useful to not actually keep a strong reference to the
+``OphydObject``s. This means that if all other references to the
+object are removed, the device may be dropped from the registry.
+
+By default, the registry keeps direct references to the objects that
+get registered, but if initalized with ``keep_references=False`` the
+Registry will not keep these references. Instead, **it is up to you to
+keep references to the registered objects**.
+
+```python
+
+# Create two registers with both referencing behaviors
+ref_registry = Registry(keep_references=True)
+noref_registry = Registry(keep_references=False)
+motor = EpicsMotor(...)
+
+# Check if we can get the motor (should be no problem)
+ref_registry[motor.name]  # <- succeeds
+noref_registry[motor.name]  # <- succeeds
+
+# Delete the object and try again
+del motor
+gc.collect()  # <- make sure it's *really* gone
+
+# Check again if we can get the motor (now it gets fun)
+ref_registry[motor.name]  # <- succeeds
+noref_registry[motor.name]  # <- raises ComponentNotFound
+
+```
+
 Integrating with Typhos
 -----------------------
 
 Typhos includes a PyDM plugin that can directly interact with ophyd
 devices. It requires ophyd objects to be registered in order to find
 them. **ophyd_registry** can automatically register devices with
 Typhos by simply passing the *use_typhos* argument when creating the
```

### Comparing `ophyd-registry-1.1.0/pyproject.toml` & `ophyd_registry-1.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ophyd-registry"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Mark Wolfman", email="wolfman@anl.gov" },
 ]
 description = "A registry to keep track of, and retrieve, Ophyd objects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -15,15 +15,15 @@
     "Topic :: System :: Hardware",
 ]
 keywords = ["synchrotron", "xray", "bluesky"]
 dependencies = ["ophyd"]
 
 [project.optional-dependencies]
 
-dev = ["black", "isort", "pytest", "build", "twine", "flake8", "ruff"]
+dev = ["black", "isort", "pytest", "build", "twine", "flake8", "ruff", "pytest-mock", "caproto"]
 
 [project.urls]
 "Homepage" = "https://github.com/spc-group/ophyd-registry"
 "Bug Tracker" = "https://github.com/spc-group/ophyd-registry/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
```

### Comparing `ophyd-registry-1.1.0/src/ophyd_registry.egg-info/PKG-INFO` & `ophyd_registry-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ophyd-registry
-Version: 1.1.0
+Version: 1.2.0
 Summary: A registry to keep track of, and retrieve, Ophyd objects.
 Author-email: Mark Wolfman <wolfman@anl.gov>
 Project-URL: Homepage, https://github.com/spc-group/ophyd-registry
 Project-URL: Bug Tracker, https://github.com/spc-group/ophyd-registry/issues
 Keywords: synchrotron,xray,bluesky
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,16 @@
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
+Requires-Dist: pytest-mock; extra == "dev"
+Requires-Dist: caproto; extra == "dev"
 
 # Ophyd Registry
 
 [![Python Tests](https://github.com/spc-group/ophyd-registry/actions/workflows/ci.yml/badge.svg)](https://github.com/spc-group/ophyd-registry/actions/workflows/ci.yml)
 
 A registry to keep track of, and retrieve, Ophyd objects.
 
@@ -224,14 +226,23 @@
 method:
 
 ```python
 
 registry.clear()
 ```
 
+To **remove disconnected devices** from the registry, use the ``pop_disconnected()`` method with an optional timeout:
+
+```python
+
+# Wait 5 seconds to give devices a chance to connect
+disconnected_devices = registry.pop_disconnected(timeout=5)
+
+```
+
 To **remove individual objects**, use either the *del* keyword, or the
 ``pop()`` method. These approaches work with either the
 ``OphydObject`` instance itself, or the instance's name:
 
 ```python
 
 # Just delete the item and move on
@@ -244,14 +255,47 @@
 # Remove the item and use it
 # (return a simulated motor if "motor1" is not in the registry)
 motor = registry.pop("motor1", ophyd.sim.motor)
 motor.set(5).wait()
 
 ```
 
+Keeping References
+------------------
+
+It may be useful to not actually keep a strong reference to the
+``OphydObject``s. This means that if all other references to the
+object are removed, the device may be dropped from the registry.
+
+By default, the registry keeps direct references to the objects that
+get registered, but if initalized with ``keep_references=False`` the
+Registry will not keep these references. Instead, **it is up to you to
+keep references to the registered objects**.
+
+```python
+
+# Create two registers with both referencing behaviors
+ref_registry = Registry(keep_references=True)
+noref_registry = Registry(keep_references=False)
+motor = EpicsMotor(...)
+
+# Check if we can get the motor (should be no problem)
+ref_registry[motor.name]  # <- succeeds
+noref_registry[motor.name]  # <- succeeds
+
+# Delete the object and try again
+del motor
+gc.collect()  # <- make sure it's *really* gone
+
+# Check again if we can get the motor (now it gets fun)
+ref_registry[motor.name]  # <- succeeds
+noref_registry[motor.name]  # <- raises ComponentNotFound
+
+```
+
 Integrating with Typhos
 -----------------------
 
 Typhos includes a PyDM plugin that can directly interact with ophyd
 devices. It requires ophyd objects to be registered in order to find
 them. **ophyd_registry** can automatically register devices with
 Typhos by simply passing the *use_typhos* argument when creating the
```

### Comparing `ophyd-registry-1.1.0/src/ophydregistry/registry.py` & `ophyd_registry-1.2.0/src/ophydregistry/registry.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
+import time
 import warnings
 from collections import OrderedDict
 from itertools import chain
-from typing import List, Mapping, Optional
+from typing import List, Mapping, Optional, Set
+from weakref import WeakSet, WeakValueDictionary
 
 from ophyd import ophydobj
 
 # Sentinal value for default parameters
 UNSET = object()
 
 
@@ -99,31 +101,43 @@
     ==========
     auto_register
       If true, new ophyd objects will be registered without needing to
       call ``register()``.
     use_typhos
       If true, items added to this registry will also be added to the
       Typhos registry for inclusion in PyDM windows.
+    keep_references
+      If false, items will be dropped from this registry if the only
+      reference comes from this registry. Relies on the garbage
+      collector, so to force cleanup use ``gc.collect()``.
 
     """
 
-    use_typhos: bool = False
+    use_typhos: bool
+    keep_references: bool
     _auto_register: bool
+    _valid_classes: Set[type] = {ophydobj.OphydObject}
 
     # components: Sequence
     _objects_by_name: Mapping
     _objects_by_label: Mapping
 
-    def __init__(self, auto_register: bool = True, use_typhos: bool = False):
+    def __init__(
+        self,
+        auto_register: bool = True,
+        use_typhos: bool = False,
+        keep_references: bool = True,
+    ):
         # Check that Typhos is installed if needed
         if use_typhos and not typhos_available:
             raise ModuleNotFoundError("No module named 'typhos'")
         # Set up empty lists and things for registering components
-        self.clear()
+        self.keep_references = keep_references
         self.use_typhos = use_typhos
+        self.clear()
         self.auto_register = auto_register
 
     @property
     def auto_register(self):
         return self._auto_register
 
     @auto_register.setter
@@ -198,19 +212,51 @@
         Parameters
         ==========
         clear_typhos
           If true, also empty the Typhos registry. Has no effect is
           *self.use_typhos* is false.
 
         """
-        self._objects_by_name = OrderedDict()
         self._objects_by_label = OrderedDict()
+        if self.keep_references:
+            self._objects_by_name = OrderedDict()
+        else:
+            self._objects_by_name = WeakValueDictionary()
         if clear_typhos and self.use_typhos:
             typhos.plugins.core.signal_registry.clear()
 
+    def pop_disconnected(self, timeout: float = 0.0) -> List:
+        """Remove any registered objects that are disconnected.
+
+        Parameters
+        ==========
+        timeout
+          How long to wait for devices to connect, in seconds.
+
+        Returns
+        =======
+        disconnected
+          The root level devices that were removed.
+
+        """
+        remaining = [dev for dev in self.root_devices]
+        t0 = time.monotonic()
+        timeout_reached = False
+        while not timeout_reached:
+            # Remove any connected devices for the running list
+            remaining = [dev for dev in remaining if not dev.connected]
+            if len(remaining) == 0:
+                # All devices are connected, so just end early.
+                break
+            time.sleep(min((0.05, timeout / 10.0)))
+            timeout_reached = (time.monotonic() - t0) > timeout
+        # Remove unconnected devices from the registry
+        popped = [self.pop(dev) for dev in remaining]
+        return popped
+
     @property
     def component_names(self):
         return set(self._objects_by_name.keys())
 
     @property
     def root_devices(self):
         """Only return root devices, those without parents."""
@@ -288,17 +334,30 @@
                 "Consider using ``findall()``. "
                 f"{results}"
             )
         else:
             result = None
         return result
 
+    def _is_resolved(self, obj):
+        """Is the object already resolved into an ophyd device, etc.
+
+        This method checks the type of the object. To extend this to
+        other types of objects, override this objects
+        ``_valid_classes`` attribute with a new set.
+
+        """
+        for cls in self._valid_classes:
+            if isinstance(obj, cls):
+                return True
+        return False
+
     def _findall_by_label(self, label, allow_none):
         # Check for already created ophyd objects (return as is)
-        if isinstance(label, ophydobj.OphydObject):
+        if self._is_resolved(label):
             yield label
             return
         # Recursively get lists of components
         if is_iterable(label):
             for lbl in label:
                 yield from self.findall(label=lbl, allow_none=allow_none)
         else:
@@ -317,15 +376,15 @@
                 # No components found so just move on
                 pass
             except TypeError:
                 raise InvalidComponentLabel(label)
 
     def _findall_by_name(self, name):
         # Check for already created ophyd objects (return as is)
-        if isinstance(name, ophydobj.OphydObject):
+        if self._is_resolved(name):
             yield name
             return
         # Check for an edge case with EpicsMotor objects (user_readback name is same as parent)
         try:
             is_user_readback = name[-13:] == "user_readback"
         except TypeError:
             is_user_readback = False
@@ -468,16 +527,14 @@
             # Register this object with Typhos
             if self.use_typhos:
                 register_typhos_signal(component)
             # Ignore any instances with the same name as a previous component
             # (Needed for some sub-components that are just readback
             # values of the parent)
             # Check that we're not adding a duplicate component name
-            if name == "I0_center":
-                print(self._objects_by_name.keys(), self)
             if name in self._objects_by_name.keys():
                 old_obj = self._objects_by_name[name]
                 is_readback = component in [
                     getattr(old_obj, "readback", None),
                     getattr(old_obj, "user_readback", None),
                     getattr(old_obj, "val", None),
                 ]
@@ -492,15 +549,18 @@
             # Register this component
             log.debug(f"Registering {name}")
             # Create a set for this device name if it doesn't exist
             self._objects_by_name[component.name] = component
             # Create a set for this device's labels if it doesn't exist
             for label in getattr(component, "_ophyd_labels_", []):
                 if label not in self._objects_by_label.keys():
-                    self._objects_by_label[label] = set()
+                    if self.keep_references:
+                        self._objects_by_label[label] = set()
+                    else:
+                        self._objects_by_label[label] = WeakSet()
                 self._objects_by_label[label].add(component)
             # Register this object with Typhos
             if self.use_typhos:
                 import typhos
 
                 typhos.plugins.register_signal(component)
             # Recusively register sub-components
```

### Comparing `ophyd-registry-1.1.0/src/ophydregistry/tests/test_instrument_registry.py` & `ophyd_registry-1.2.0/src/ophydregistry/tests/test_instrument_registry.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import gc
 import logging
+import time
+from concurrent.futures import ThreadPoolExecutor
+from unittest import mock
 
 import pytest
 from ophyd import Device, EpicsMotor, sim
 
 from ophydregistry import ComponentNotFound, MultipleComponentsFound, Registry
 
 
 @pytest.fixture()
 def registry():
     reg = Registry(auto_register=False, use_typhos=False)
+    reg._valid_classes = {mock.MagicMock, *reg._valid_classes}
     try:
         yield reg
     finally:
         del reg
 
 
 def test_register_component(registry):
@@ -274,15 +278,14 @@
 def test_auto_register():
     """Ensure the registry gets devices that aren't explicitly registered.
 
     Uses ophyds instantiation callback mechanism.
 
     """
     registry = Registry(auto_register=True)
-    print(f"auto_register: {registry}")
     sim.SynGauss(
         "I0",
         sim.motor,
         "motor",
         center=-0.5,
         Imax=1,
         sigma=1,
@@ -310,15 +313,14 @@
     registry.clear()
     with pytest.raises(ComponentNotFound):
         registry.find("I0")
 
 
 def test_component_properties(registry):
     """Check that we can get lists of component and devices."""
-    print(f"component_properties: {registry}")
     I0 = sim.SynGauss(
         "I0",
         sim.motor,
         "motor",
         center=-0.5,
         Imax=1,
         sigma=1,
@@ -425,7 +427,75 @@
     popped = registry.pop("gibberish", motor)
     assert popped is motor
     # Check that the test fails
     with pytest.raises(ComponentNotFound):
         registry[motor.name]
     with pytest.raises(ComponentNotFound):
         registry["motors"]
+
+
+def test_weak_references():
+    """Check that we can make a registry that automatically drops
+    objects that are only referenced by this registry.
+
+    """
+    motor = sim.SynAxis(name="weak_motor", labels={"motors"})
+    registry = Registry(keep_references=False)
+    registry.register(motor)
+    # Can we still find the object if the test has a reference?
+    assert registry.find("weak_motor") is motor
+    # Delete the original object
+    del motor
+    gc.collect()
+    # Check that it's not in the registry anymore
+    with pytest.raises(ComponentNotFound):
+        registry.find("weak_motor")
+
+
+@pytest.fixture()
+def motors(mocker):
+    mocker.patch("ophyd.epics_motor.EpicsMotor.connected", new=True)
+    good_motor = EpicsMotor("255idVME:m1", name="good_motor")
+    good_motor.connected = True
+    bad_motor = EpicsMotor("255idVME:m2", name="bad_motor")
+    bad_motor.connected = False
+    return (good_motor, bad_motor)
+
+
+def test_pop_disconnected(registry, motors):
+    """Check that we can remove disconnected devices."""
+    good_motor, bad_motor = motors
+    registry.register(good_motor)
+    registry.register(bad_motor)
+    # Check that the disconnected device gets removed
+    popped = registry.pop_disconnected()
+    with pytest.raises(ComponentNotFound):
+        registry["bad_motor"]
+    # Check that the popped device was returned
+    assert len(popped) == 1
+    assert popped[0] is bad_motor
+    # Check that the connected device is still in the registry
+    assert registry["good_motor"] is good_motor
+
+
+def test_pop_disconnected_with_timeout(registry, motors):
+    """Check that we can apply a timeout when waiting for disconnected
+    devices.
+
+    """
+    good_motor, bad_motor = motors
+    good_motor.connected = False  # It starts disconnected
+    # Register the devices
+    registry.register(good_motor)
+    registry.register(bad_motor)
+
+    # Remove the devices with a timeout
+    def make_connected(dev, wait):
+        time.sleep(wait)
+        dev.connected = True
+
+    with ThreadPoolExecutor(max_workers=1) as executor:
+        # Make the connection happen after 50 ms
+        executor.submit(make_connected, good_motor, 0.15)
+        registry.pop_disconnected(timeout=0.3)
+    # Check that the connected device is still in the registry
+    assert registry["good_motor"] is good_motor
```


# Comparing `tmp/pyson_data-0.1.0.tar.gz` & `tmp/pyson_data-0.1.1.1.tar.gz`

## Comparing `pyson_data-0.1.0.tar` & `pyson_data-0.1.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pyson_data-0.1.0/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pyson_data-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pyson_data-0.1.0/src/pyson_data/__init__.py
--rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 pyson_data-0.1.0/src/pyson_data/pyson.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pyson_data-0.1.0/tests/example.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pyson_data-0.1.0/tests/example.pyson
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyson_data-0.1.0/.gitignore
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pyson_data-0.1.0/LICENSE
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 pyson_data-0.1.0/README.md
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 pyson_data-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3826 2020-02-02 00:00:00.000000 pyson_data-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/src/pyson_data/__init__.py
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/src/pyson_data/pyson.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/tests/example.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/tests/example.pyson
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/.gitignore
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/LICENSE
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/README.md
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/PKG-INFO
```

### Comparing `pyson_data-0.1.0/setup.py` & `pyson_data-0.1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
      name='pyson_data',
-     version='0.0.3',
+     version='0.1.2',
      scripts=['pyson_data'],
      author="ComputingSquid",
      description="Provides support for storing data in .pyson format",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/ProbablyComputingSquid/PYSON",
      packages=setuptools.find_packages(),
```

### Comparing `pyson_data-0.1.0/.github/workflows/python-publish.yml` & `pyson_data-0.1.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyson_data-0.1.0/src/pyson_data/pyson.py` & `pyson_data-0.1.1.1/src/pyson_data/pyson.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,25 +133,41 @@
         case _:
             raise Exception(f"Data type {type} not supported")
     toWrite = name + ":" + type + ":" + value
     if mode == "a":
         toWrite = "\n" + toWrite
     open(filePath, mode).write(toWrite)
 
+def writeMultiple(filePath: str, data: dict[str, PysonValue], mode: str = "a") -> None:
+    for tup in data.items():
+        name, value = tup
+        type = ""
+        if isinstance(value, list):
+            type = "list"
+        if isinstance(value, int):
+            type = "int"
+        if isinstance(value, float):
+            type = "float"
+        if isinstance(value, str):
+            type = "str"
+        if type == "":
+            raise Exception("Invalid pyson typein writeMultiple()")
+        write(filePath, name, type, value, mode)
+        mode = "a"
 
 def updateData(filePath: str, name: str, data: str) -> None:
     """
     Note: the type of data currently cannot be updated
     Parameters:
         filePath: str - File path where the value is
         name: str - Name of the data to update
         data: str - The value to update as a string
     Return value: None
     """
-    
+    data=str(data)
     # Read in the data
     file = open(filePath, "r")
     fileData: list[str] = file.read().split("\n")
     file.close()
     # Look through the data to find the value to update
     index: int = 0
     foundItem: bool = False
```

### Comparing `pyson_data-0.1.0/tests/example.py` & `pyson_data-0.1.1.1/tests/example.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import pyson # to use this in your project, simply change the name from "pyson" to the name of the file you're importing it from
 import os
+import pyson_data as pyson
+# this is an example of how to use the pyson module
 
 # Read test
 print("-----READ TEST-------")
 print(pyson.getData("example.pyson","str_example"))
 print(pyson.getData("example.pyson","int_example"))
 print(pyson.getData("example.pyson","list_example"))
 print(pyson.getData("example.pyson","float_example"))
@@ -17,14 +18,15 @@
 pyson.write("newfile.pyson", "string", "str", "value", "w")
 
 # Append test
 print("---APPEND TEST-------")
 pyson.write("newfile.pyson", "integer", "int", 123, "a")
 pyson.write("newfile.pyson", "floating-point", "float", 3.14, "a")
 pyson.write("newfile.pyson", "string list", "list", ["this is a list", "of strings"])
+pyson.writeMultiple("example.pyson", {"test": "value", "integer": 69, "list1": ["1","2"], "pypi": 3.1415962})
 print(pyson.getWhole("newfile.pyson"))
 
 # Compatability test
 print("---COMPATABILITY TEST------")
 print(pyson.checkCompatible("example.pyson"))
 print(pyson.checkCompatible("newfile.pyson"))
 os.remove("newfile.pyson")
```

### Comparing `pyson_data-0.1.0/LICENSE` & `pyson_data-0.1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyson_data-0.1.0/README.md` & `pyson_data-0.1.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,67 @@
+Metadata-Version: 2.3
+Name: pyson_data
+Version: 0.1.1.1
+Summary: Pyson package for .pyson data format support
+Project-URL: Homepage, https://github.com/ProbablyComputingSquid/PYSON/
+Project-URL: Issues, https://github.com/ProbablyComputingSquid/PYSON/issues
+Author-email: josh-co <omegaraspberrypi@gmail.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 # PYSON #
-##### Maintained by: [OmegaGodzilla66](https://github.com/OmegaGodzilla66), [ComputingSquid](https://github.com/ProbablyComputingSquid), and [coolSchnoodle](https://github.com/coolSchnoodle) #####
+##### Maintained by: [OmegaGodzilla66](https://github.com/OmegaGodzilla66), [ComputingSquid](https://github.com/ProbablyComputingSquid), and [CoolSchnoodle](https://github.com/coolSchnoodle) #####
 
 
 ## Overview ##
 The purpose of this project is to provide a python-based alternative to JSON. This is a (almost) fully functional JSON-inspired data management system!
 
 ## How to Use ##
 **THIS PROJECT IS NOT YET FINISHED! DOCUMENTATION IS ONLY SHOWN FOR COMPLETED FEATURES. SOME FEATURES MAY BREAK DUE TO CONTINUED DEVELOPMENT. IF YOU SEE A PROBLEM, PLEASE LET ME KNOW!**
-<br>Belive it or not, this project is surprisingly easy to use. The only thing you have to do is copy/paste the contents of pyson.py into your own Python project! From then, you can just `import pyson`, and use functions as normal! Support for other languages may come soon. Support for this as a library (no copypaste needed) may be coming soon as well.<br>
-**The PYSON format does NOT include a newline at the end of the file, files with a newline at the end will be considered invalid**
-### List of Functions ###
-
-#### getData() ####
-Required inputs: `filePath`, `datacall`<br>
-Output: The item in the stored type at index `datacall` in file `filePath`<br>
-
-#### getWhole() ####
-Required inputs: `filePath`<br>
-Output: A list of all datas in their respective types<br>
-
-#### updateData() ####
-Required inputs: `filePath`, `name`, `data`<br>
-Updates entry `name` to contain value `data`<br>
-Output: Whether or not function call worked<br>
-
-#### isCompatible() ####
-Required inputs: `filePath`<br>
-Outputs: Bool<br>
-Checks if a file is compatible with .cnf file format. Returns True if so, returns False if not. <br>
+<br>Believe it or not, this project is surprisingly easy to use.<br>
+<br> The only thing you have to do is `pip install pyson-data` ! From then, you can just `import pyson_data as pyson`, and use functions as normal!
+Support for other languages may come soon.<br>
+
+## quickstart ## 
+TODO: write later
+
+## documentation ##
+Documentation has been moved to the project wiki [here](https://github.com/OmegaGodzilla66/PYSON/wiki) to decrease clutter in the README.
 
 ## Supported Types ##
 There are 4 supported types: int, float, str, and list
 <br><br>
 - An int is a whole number that can be any value<br>
 - A str is a list of text (quotes not required)<br>
-- A list is a list of values, which currently have to all be strings. List items are seperated by the (*) seperator. Currently there is no escaping support. I don't really know why you would use that value normally in a list. <br> 
+- A list is a list of values, which currently have to all be strings. List items are seperated by the (*) seperator.
+Currently there is no escaping support. I don't really know why you would use that value normally in a list. <br> 
 - A float is a decimal number, that can be any value<br>
 
 More supported types may be added. 
 
 ## Changelog ##
+- v0.1.1: Added writeMultiple function, various bug fixes
+- v0.1.0-alpha: package & release deployed to pypi, merged code to main, and resolved all merge conflicts! truly a cause for celebration 🎉
+- v0.0.9: coolSchnoodle and nmd102 made code fixes and README fixes
 - v0.0.8: Added updateData function
 - v0.0.7: Fixed errors, refactored bad code
 - v0.0.6: Added floats
 - v0.0.5: Updated naming system, ported to github!
 - v0.0.4: Added a function that checks if a file is compatible with .pyson file format. Fixed a bug in the write. Other general bug fixes. 
-- v0.0.3: Added a write function! This is now (technicaally) a fully functioning data service!
+- v0.0.3: Added a write function! This is now (technically) a fully functioning data service!
 - v0.0.2: Added a read function for the whole file. Returns a list of all contents. This is actually getting pretty cool!
-- v0.0.1: Initial launch! Basic reading features for a .cnf file. Current compatible types are string, int, and list.
+- v0.0.1: Initial launch! Basic reading features for a .cnf (renamed almost immediately to pyson) file. Current compatible types are string, int, and list.
 
 ### Dev comments ###
 0.0.8:<br>
-> I (computingSquid) have had to resort to drastic measures to get my pull request approved. coolSchnoodle was forced to say "uwu"
+> I (computingSquid) have had to resort to drastic measures to get my pull request approved. CoolSchnoodle was forced to say "uwu"
 
 0.0.5: <br>
 > Wahoo! Porting to github!...oh shoot now I have to rename everything.
 
 - OmegoGodzilla66
 
 0.0.4: <br>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyson_data-0.1.0/pyproject.toml` & `pyson_data-0.1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyson_data"
-version = "0.1.0"
+version = "0.1.1.1"
 authors = [
   { name="josh-co", email="omegaraspberrypi@gmail.com" },
 ]
 description = "Pyson package for .pyson data format support"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```


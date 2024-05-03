# Comparing `tmp/connpy-4.0.0b3.tar.gz` & `tmp/connpy-4.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connpy-4.0.0b3.tar", last modified: Wed Apr 17 20:35:46 2024, max compression
+gzip compressed data, was "connpy-4.0.0b5.tar", last modified: Mon Apr 22 21:19:23 2024, max compression
```

## Comparing `connpy-4.0.0b3.tar` & `connpy-4.0.0b5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:35:46.026694 connpy-4.0.0b3/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-17 20:35:40.000000 connpy-4.0.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12164 2024-04-17 20:35:46.026694 connpy-4.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-04-17 20:35:40.000000 connpy-4.0.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:35:46.026694 connpy-4.0.0b3/connpy/
--rw-r--r--   0 runner    (1001) docker     (127)    10798 2024-04-17 20:35:40.000000 connpy-4.0.0b3/connpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-17 20:35:40.000000 connpy-4.0.0b3/connpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 20:35:40.000000 connpy-4.0.0b3/connpy/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24698 2024-04-17 20:35:40.000000 connpy-4.0.0b3/connpy/ai.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5102 2024-04-17 20:35:40.000000 connpy-4.0.0b3/connpy/api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7896 2024-04-17 20:35:40.000000 connpy-4.0.0b3/connpy/completion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16208 2024-04-17 20:35:40.000000 connpy-4.0.0b3/connpy/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    74522 2024-04-17 20:35:40.000000 connpy-4.0.0b3/connpy/connapp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    32826 2024-04-17 20:35:40.000000 connpy-4.0.0b3/connpy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:35:46.026694 connpy-4.0.0b3/connpy/core_plugins/
--rwxr-xr-x   0 runner    (1001) docker     (127)    16380 2024-04-17 20:35:40.000000 connpy-4.0.0b3/connpy/core_plugins/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-17 20:35:40.000000 connpy-4.0.0b3/connpy/core_plugins/sync_client
--rwxr-xr-x   0 runner    (1001) docker     (127)     1572 2024-04-17 20:35:40.000000 connpy-4.0.0b3/connpy/hooks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7133 2024-04-17 20:35:40.000000 connpy-4.0.0b3/connpy/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:35:46.026694 connpy-4.0.0b3/connpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12164 2024-04-17 20:35:46.000000 connpy-4.0.0b3/connpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-17 20:35:46.000000 connpy-4.0.0b3/connpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:35:46.000000 connpy-4.0.0b3/connpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-17 20:35:46.000000 connpy-4.0.0b3/connpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-17 20:35:46.000000 connpy-4.0.0b3/connpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 20:35:46.000000 connpy-4.0.0b3/connpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-17 20:35:46.026694 connpy-4.0.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-17 20:35:40.000000 connpy-4.0.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:19:23.135183 connpy-4.0.0b5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-22 21:19:17.000000 connpy-4.0.0b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17495 2024-04-22 21:19:23.135183 connpy-4.0.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16385 2024-04-22 21:19:17.000000 connpy-4.0.0b5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:19:23.131183 connpy-4.0.0b5/connpy/
+-rw-r--r--   0 runner    (1001) docker     (127)    16127 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24877 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/ai.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5181 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7896 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/completion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16438 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    74729 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/connapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33096 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:19:23.135183 connpy-4.0.0b5/connpy/core_plugins/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13827 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/core_plugins/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/core_plugins/sync_client
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3231 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/hooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7133 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:19:23.135183 connpy-4.0.0b5/connpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17495 2024-04-22 21:19:23.000000 connpy-4.0.0b5/connpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-22 21:19:23.000000 connpy-4.0.0b5/connpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 21:19:23.000000 connpy-4.0.0b5/connpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-22 21:19:23.000000 connpy-4.0.0b5/connpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-22 21:19:23.000000 connpy-4.0.0b5/connpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-22 21:19:23.000000 connpy-4.0.0b5/connpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-22 21:19:23.135183 connpy-4.0.0b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-22 21:19:17.000000 connpy-4.0.0b5/setup.py
```

### Comparing `connpy-4.0.0b3/LICENSE` & `connpy-4.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `connpy-4.0.0b3/PKG-INFO` & `connpy-4.0.0b5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 4.0.0b3
+Version: 4.0.0b5
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
@@ -140,35 +140,122 @@
   - Class definitions
   - Function definitions
   - Import statements
   - The `if __name__ == "__main__":` block for standalone execution
   - Pass statements
 
 ### Specific Class Requirements
-- The plugin script must define at least two specific classes:
+- The plugin script must define specific classes with particular attributes and methods. Each class serves a distinct role within the plugin's architecture:
   1. **Class `Parser`**:
-     - Must contain only one method: `__init__`.
-     - The `__init__` method must initialize at least two attributes:
-       - `self.parser`: An instance of `argparse.ArgumentParser`.
-       - `self.description`: A string containing the description of the parser.
+     - **Purpose**: Handles parsing of command-line arguments.
+     - **Requirements**:
+       - Must contain only one method: `__init__`.
+       - The `__init__` method must initialize at least two attributes:
+         - `self.parser`: An instance of `argparse.ArgumentParser`.
+         - `self.description`: A string containing the description of the parser.
   2. **Class `Entrypoint`**:
-     - Must have an `__init__` method that accepts exactly three parameters besides `self`:
-       - `args`: Arguments passed to the plugin.
-       - The parser instance (typically `self.parser` from the `Parser` class).
-       - The Connapp instance to interact with the Connpy app.
+     - **Purpose**: Acts as the entry point for plugin execution, utilizing parsed arguments and integrating with the main application.
+     - **Requirements**:
+       - Must have an `__init__` method that accepts exactly three parameters besides `self`:
+         - `args`: Arguments passed to the plugin.
+         - The parser instance (typically `self.parser` from the `Parser` class).
+         - The Connapp instance to interact with the Connpy app.
+  3. **Class `Preload`**:
+     - **Purpose**: Performs any necessary preliminary setup or configuration independent of the main parsing and entry logic.
+   - **Requirements**:
+     - Contains at least an `__init__` method that accepts parameter connapp besides `self`.
+
+### Class Dependencies and Combinations
+- **Dependencies**:
+  - `Parser` and `Entrypoint` are interdependent and must both be present if one is included.
+  - `Preload` is independent and may exist alone or alongside the other classes.
+- **Valid Combinations**:
+  - `Parser` and `Entrypoint` together.
+  - `Preload` alone.
+  - All three classes (`Parser`, `Entrypoint`, `Preload`).
+
+### Preload Modifications and Hooks
+
+In the `Preload` class of the plugin system, you have the ability to customize the behavior of existing classes and methods within the application through a robust hooking system. This documentation explains how to use the `modify`, `register_pre_hook`, and `register_post_hook` methods to tailor plugin functionality to your needs.
+
+#### Modifying Classes with `modify`
+The `modify` method allows you to alter instances of a class at the time they are created or after their creation. This is particularly useful for setting or modifying configuration settings, altering default behaviors, or adding new functionalities to existing classes without changing the original class definitions.
+
+- **Usage**: Modify a class to include additional configurations or changes
+- **Modify Method Signature**:
+  - `modify(modification_method)`: A function that is invoked with an instance of the class as its argument. This function should perform any modifications directly on this instance.
+- **Modification Method Signature**:
+  - **Arguments**:
+    - `cls`:  This function accepts a single argument, the class instance, which it then modifies.
+  - **Modifiable Classes**:
+    - `connapp.config`
+    - `connapp.node`
+    - `connapp.nodes`
+    - `connapp.ai`
+  - ```python
+    def modify_config(cls):
+        # Example modification: adding a new attribute or modifying an existing one
+        cls.new_attribute = 'New Value'
+
+    class Preload:
+        def __init__(self, connapp):
+            # Applying modification to the config class instance
+            connapp.config.modify(modify_config)
+    ```
+
+#### Implementing Hooks with `register_pre_hook` and `register_post_hook`
+These methods allow you to define custom logic to be executed before (`register_pre_hook`) or after (`register_post_hook`) the main logic of a method. This is particularly useful for logging, auditing, preprocessing inputs, postprocessing outputs or adding functionalities.
+
+  - **Usage**: Register hooks to methods to execute additional logic before or after the main method execution.
+- **Registration Methods Signature**:
+  - `register_pre_hook(pre_hook_method)`: A function that is invoked before the main method is executed. This function should do preprocessing of the arguments.
+  - `register_post_hook(post_hook_method)`: A function that is invoked after the main method is executed. This function should do postprocessing of the outputs.
+- **Method Signatures for Pre-Hooks**
+  - `pre_hook_method(*args, **kwargs)`
+  - **Arguments**:
+    - `*args`, `**kwargs`: The arguments and keyword arguments that will be passed to the method being hooked. The pre-hook function has the opportunity to inspect and modify these arguments before they are passed to the main method.
+  - **Return**:
+    - Must return a tuple `(args, kwargs)`, which will be used as the new arguments for the main method. If the original arguments are not modified, the function should return them as received.
+- **Method Signatures for Post-Hooks**:
+  - `post_hook_method(*args, **kwargs)`
+  - **Arguments**:
+    - `*args`, `**kwargs`: The arguments and keyword arguments that were passed to the main method.
+      - `kwargs["result"]`: The value returned by the main method. This allows the post-hook to inspect and even alter the result before it is returned to the original caller.
+  - **Return**:
+    - Can return a modified result, which will replace the original result of the main method, or simply return `kwargs["result"]` to return the original method result.    
+  - ```python
+    def pre_processing_hook(*args, **kwargs):
+        print("Pre-processing logic here")
+        # Modify arguments or perform any checks
+        return args, kwargs  # Return modified or unmodified args and kwargs
+
+    def post_processing_hook(*args, **kwargs):
+        print("Post-processing logic here")
+        # Modify the result or perform any final logging or cleanup
+        return kwargs["result"]  # Return the modified or unmodified result
+
+    class Preload:
+        def __init__(self, connapp):
+            # Registering a pre-hook
+            connapp.ai.some_method.register_pre_hook(pre_processing_hook)
+
+            # Registering a post-hook
+            connapp.node.another_method.register_post_hook(post_processing_hook)
+    ```
+  
 
 ### Executable Block
 - The plugin script can include an executable block:
   - `if __name__ == "__main__":`
   - This block allows the plugin to be run as a standalone script for testing or independent use.
 
 ### Script Verification
 - The `verify_script` method in `plugins.py` is used to check the plugin script's compliance with these standards.
 - Non-compliant scripts will be rejected to ensure consistency and proper functionality within the plugin system.
-- 
+ 
 ### Example Script
 
 For a practical example of how to write a compatible plugin script, please refer to the following example:
 
 [Example Plugin Script](https://github.com/fluzzi/awspy)
 
 This script demonstrates the required structure and implementation details according to the plugin system's standards.
```

### Comparing `connpy-4.0.0b3/README.md` & `connpy-4.0.0b5/connpy/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,47 @@
-# Conn
-[![](https://img.shields.io/pypi/v/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
-[![](https://img.shields.io/pypi/pyversions/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
-[![](https://img.shields.io/pypi/l/connpy.svg?style=flat-square)](https://github.com/fluzzi/connpy/blob/main/LICENSE)
-[![](https://img.shields.io/pypi/dm/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
+#!/usr/bin/env python3
+'''
+## Connection manager
 
-Connpy is a ssh and telnet connection manager and automation module for Linux, Mac and Docker
+Connpy is a connection manager that allows you to store nodes to connect them fast and password free.
 
-## Installation
-
-pip install connpy
-
-### Run it in Windows using docker
-```
-git clone https://github.com/fluzzi/connpy
-docker compose -f path/to/folder/docker-compose.yml build
-docker compose -f path/to/folder/docker-compose.yml run -it connpy-app
-```
-
-## Connection manager 
 ### Features
     - You can generate profiles and reference them from nodes using @profilename so you dont
       need to edit multiple nodes when changing password or other information.
     - Nodes can be stored on @folder or @subfolder@folder to organize your devices. Then can 
       be referenced using node@subfolder@folder or node@folder
     - If you have too many nodes. Get completion script using: conn config --completion.
       Or use fzf installing pyfzf and running conn config --fzf true
     - Create in bulk, copy, move, export and import nodes for easy management.
     - Run automation scripts in network devices.
     - use GPT AI to help you manage your devices.
     - Add plugins with your own scripts.
     - Much more!
 
-### Usage:
+### Usage
 ```
 usage: conn [-h] [--add | --del | --mod | --show | --debug] [node|folder] [--sftp]
        conn {profile,move,mv,copy,cp,list,ls,bulk,export,import,ai,run,api,plugin,config} ...
 
 positional arguments:
   node|folder    node[@subfolder][@folder]
                  Connect to specific node or show all matching nodes
                  [@subfolder][@folder]
                  Show all available connections globaly or in specified path
-```
-
-### Options:
-```
+Options:
   -h, --help         show this help message and exit
   -v, --version      Show version
   -a, --add          Add new node[@subfolder][@folder] or [@subfolder]@folder
   -r, --del, --rm    Delete node[@subfolder][@folder] or [@subfolder]@folder
   -e, --mod, --edit  Modify node[@subfolder][@folder]
   -s, --show         Show node[@subfolder][@folder]
   -d, --debug        Display all conections steps
   -t, --sftp         Connects using sftp instead of ssh
-```
 
-### Commands:
-```
+Commands:
   profile         Manage profiles
   move(mv)        Move node
   copy(cp)        Copy node
   list(ls)        List profiles, nodes or folders
   bulk            Add nodes in bulk
   export          Export connection folder to Yaml file
   import          Import connection folder to config from Yaml file
@@ -68,15 +49,15 @@
   run             Run scripts or commands on nodes
   api             Start and stop connpy api
   plugin          Manage plugins
   config          Manage app config
   sync            Sync config with Google
 ```
 
-### Manage profiles:
+###   Manage profiles
 ```
 usage: conn profile [-h] (--add | --del | --mod | --show) profile
 
 positional arguments:
   profile        Name of profile to manage
 
 options:
@@ -84,48 +65,133 @@
   -a, --add          Add new profile
   -r, --del, --rm    Delete profile
   -e, --mod, --edit  Modify profile
   -s, --show         Show profile
 
 ```
 
-### Examples:
+###   Examples
 ```
    conn profile --add office-user
    conn --add @office
    conn --add @datacenter@office
    conn --add server@datacenter@office
    conn --add pc@office
    conn --show server@datacenter@office
    conn pc@office
    conn server
 ``` 
 ## Plugin Requirements for Connpy
-
 ### General Structure
 - The plugin script must be a Python file.
 - Only the following top-level elements are allowed in the plugin script:
   - Class definitions
   - Function definitions
   - Import statements
   - The `if __name__ == "__main__":` block for standalone execution
   - Pass statements
 
 ### Specific Class Requirements
-- The plugin script must define at least two specific classes:
+- The plugin script must define specific classes with particular attributes and methods. Each class serves a distinct role within the plugin's architecture:
   1. **Class `Parser`**:
-     - Must contain only one method: `__init__`.
-     - The `__init__` method must initialize at least two attributes:
-       - `self.parser`: An instance of `argparse.ArgumentParser`.
-       - `self.description`: A string containing the description of the parser.
+     - **Purpose**: Handles parsing of command-line arguments.
+     - **Requirements**:
+       - Must contain only one method: `__init__`.
+       - The `__init__` method must initialize at least two attributes:
+         - `self.parser`: An instance of `argparse.ArgumentParser`.
+         - `self.description`: A string containing the description of the parser.
   2. **Class `Entrypoint`**:
-     - Must have an `__init__` method that accepts exactly three parameters besides `self`:
-       - `args`: Arguments passed to the plugin.
-       - The parser instance (typically `self.parser` from the `Parser` class).
-       - The Connapp instance to interact with the Connpy app.
+     - **Purpose**: Acts as the entry point for plugin execution, utilizing parsed arguments and integrating with the main application.
+     - **Requirements**:
+       - Must have an `__init__` method that accepts exactly three parameters besides `self`:
+         - `args`: Arguments passed to the plugin.
+         - The parser instance (typically `self.parser` from the `Parser` class).
+         - The Connapp instance to interact with the Connpy app.
+  3. **Class `Preload`**:
+     - **Purpose**: Performs any necessary preliminary setup or configuration independent of the main parsing and entry logic.
+   - **Requirements**:
+     - Contains at least an `__init__` method that accepts parameter connapp besides `self`.
+
+### Class Dependencies and Combinations
+- **Dependencies**:
+  - `Parser` and `Entrypoint` are interdependent and must both be present if one is included.
+  - `Preload` is independent and may exist alone or alongside the other classes.
+- **Valid Combinations**:
+  - `Parser` and `Entrypoint` together.
+  - `Preload` alone.
+  - All three classes (`Parser`, `Entrypoint`, `Preload`).
+
+### Preload Modifications and Hooks
+
+In the `Preload` class of the plugin system, you have the ability to customize the behavior of existing classes and methods within the application through a robust hooking system. This documentation explains how to use the `modify`, `register_pre_hook`, and `register_post_hook` methods to tailor plugin functionality to your needs.
+
+#### Modifying Classes with `modify`
+The `modify` method allows you to alter instances of a class at the time they are created or after their creation. This is particularly useful for setting or modifying configuration settings, altering default behaviors, or adding new functionalities to existing classes without changing the original class definitions.
+
+- **Usage**: Modify a class to include additional configurations or changes
+- **Modify Method Signature**:
+  - `modify(modification_method)`: A function that is invoked with an instance of the class as its argument. This function should perform any modifications directly on this instance.
+- **Modification Method Signature**:
+  - **Arguments**:
+    - `cls`:  This function accepts a single argument, the class instance, which it then modifies.
+  - **Modifiable Classes**:
+    - `connapp.config`
+    - `connapp.node`
+    - `connapp.nodes`
+    - `connapp.ai`
+  - ```python
+    def modify_config(cls):
+        # Example modification: adding a new attribute or modifying an existing one
+        cls.new_attribute = 'New Value'
+
+    class Preload:
+        def __init__(self, connapp):
+            # Applying modification to the config class instance
+            connapp.config.modify(modify_config)
+    ```
+
+#### Implementing Hooks with `register_pre_hook` and `register_post_hook`
+These methods allow you to define custom logic to be executed before (`register_pre_hook`) or after (`register_post_hook`) the main logic of a method. This is particularly useful for logging, auditing, preprocessing inputs, postprocessing outputs or adding functionalities.
+
+  - **Usage**: Register hooks to methods to execute additional logic before or after the main method execution.
+- **Registration Methods Signature**:
+  - `register_pre_hook(pre_hook_method)`: A function that is invoked before the main method is executed. This function should do preprocessing of the arguments.
+  - `register_post_hook(post_hook_method)`: A function that is invoked after the main method is executed. This function should do postprocessing of the outputs.
+- **Method Signatures for Pre-Hooks**
+  - `pre_hook_method(*args, **kwargs)`
+  - **Arguments**:
+    - `*args`, `**kwargs`: The arguments and keyword arguments that will be passed to the method being hooked. The pre-hook function has the opportunity to inspect and modify these arguments before they are passed to the main method.
+  - **Return**:
+    - Must return a tuple `(args, kwargs)`, which will be used as the new arguments for the main method. If the original arguments are not modified, the function should return them as received.
+- **Method Signatures for Post-Hooks**:
+  - `post_hook_method(*args, **kwargs)`
+  - **Arguments**:
+    - `*args`, `**kwargs`: The arguments and keyword arguments that were passed to the main method.
+      - `kwargs["result"]`: The value returned by the main method. This allows the post-hook to inspect and even alter the result before it is returned to the original caller.
+  - **Return**:
+    - Can return a modified result, which will replace the original result of the main method, or simply return `kwargs["result"]` to return the original method result.    
+  - ```python
+    def pre_processing_hook(*args, **kwargs):
+        print("Pre-processing logic here")
+        # Modify arguments or perform any checks
+        return args, kwargs  # Return modified or unmodified args and kwargs
+
+    def post_processing_hook(*args, **kwargs):
+        print("Post-processing logic here")
+        # Modify the result or perform any final logging or cleanup
+        return kwargs["result"]  # Return the modified or unmodified result
+
+    class Preload:
+        def __init__(self, connapp):
+            # Registering a pre-hook
+            connapp.ai.some_method.register_pre_hook(pre_processing_hook)
+
+            # Registering a post-hook
+            connapp.node.another_method.register_post_hook(post_processing_hook)
+    ```
 
 ### Executable Block
 - The plugin script can include an executable block:
   - `if __name__ == "__main__":`
   - This block allows the plugin to be run as a standalone script for testing or independent use.
 
 ### Script Verification
@@ -136,97 +202,14 @@
 
 For a practical example of how to write a compatible plugin script, please refer to the following example:
 
 [Example Plugin Script](https://github.com/fluzzi/awspy)
 
 This script demonstrates the required structure and implementation details according to the plugin system's standards.
 
-## Automation module usage
-### Standalone module
-```
-import connpy
-router = connpy.node("uniqueName","ip/host", user="username", password="password")
-router.run(["term len 0","show run"])
-print(router.output)
-hasip = router.test("show ip int brief","1.1.1.1")
-if hasip:
-    print("Router has ip 1.1.1.1")
-else:
-    print("router does not have ip 1.1.1.1")
-```
-
-### Using manager configuration
-```
-import connpy
-conf = connpy.configfile()
-device = conf.getitem("router@office")
-router = connpy.node("unique name", **device, config=conf)
-result = router.run("show ip int brief")
-print(result)
-```
-### Running parallel tasks on multiple devices 
-```
-import connpy
-conf = connpy.configfile()
-#You can get the nodes from the config from a folder and fitlering in it
-nodes = conf.getitem("@office", ["router1", "router2", "router3"])
-#You can also get each node individually:
-nodes = {}
-nodes["router1"] = conf.getitem("router1@office")
-nodes["router2"] = conf.getitem("router2@office")
-nodes["router10"] = conf.getitem("router10@datacenter")
-#Also, you can create the nodes manually:
-nodes = {}
-nodes["router1"] = {"host": "1.1.1.1", "user": "user", "password": "password1"}
-nodes["router2"] = {"host": "1.1.1.2", "user": "user", "password": "password2"}
-nodes["router3"] = {"host": "1.1.1.2", "user": "user", "password": "password3"}
-#Finally you run some tasks on the nodes
-mynodes = connpy.nodes(nodes, config = conf)
-result = mynodes.test(["show ip int br"], "1.1.1.2")
-for i in result:
-    print("---" + i + "---")
-    print(result[i])
-    print()
-# Or for one specific node
-mynodes.router1.run(["term len 0". "show run"], folder = "/home/user/logs")
-```
-### Using variables
-```
-import connpy
-config = connpy.configfile()
-nodes = config.getitem("@office", ["router1", "router2", "router3"])
-commands = []
-commands.append("config t")
-commands.append("interface lo {id}")
-commands.append("ip add {ip} {mask}")
-commands.append("end")
-variables = {}
-variables["router1@office"] = {"ip": "10.57.57.1"}
-variables["router2@office"] = {"ip": "10.57.57.2"}
-variables["router3@office"] = {"ip": "10.57.57.3"}
-variables["__global__"] = {"id": "57"}
-variables["__global__"]["mask"] =  "255.255.255.255"
-expected = "!"
-routers = connpy.nodes(nodes, config = config)
-routers.run(commands, variables)
-routers.test("ping {ip}", expected, variables)
-for key in routers.result:
-    print(key, ' ---> ', ("pass" if routers.result[key] else "fail"))
-```
-### Using AI
-```
-import connpy
-conf = connpy.configfile()
-organization = 'openai-org'
-api_key = "openai-key"
-myia = ai(conf, organization, api_key)
-input = "go to router 1 and get me the full configuration"
-result = myia.ask(input, dryrun = False)
-print(result)
-```
 ## http API
 With the Connpy API you can run commands on devices using http requests
 
 ### 1. List Nodes
 
 **Endpoint**: `/list_nodes`
 
@@ -326,8 +309,109 @@
 * `input` (required): The user input requesting the AI to perform an action on some devices or get the devices list.
 * `dryrun` (optional): If set to true, it will return the parameters to run the request but it won't run it. default is false.
 
 #### Response:
 
 - A JSON array containing the action to run and the parameters and the result of the action.
 
+## Automation module
+The automation module
+### Standalone module
+```
+import connpy
+router = connpy.node("uniqueName","ip/host", user="user", password="pass")
+router.run(["term len 0","show run"])
+print(router.output)
+hasip = router.test("show ip int brief","1.1.1.1")
+if hasip:
+    print("Router has ip 1.1.1.1")
+else:
+    print("router does not have ip 1.1.1.1")
+```
 
+### Using manager configuration
+```
+import connpy
+conf = connpy.configfile()
+device = conf.getitem("server@office")
+server = connpy.node("unique name", **device, config=conf)
+result = server.run(["cd /", "ls -la"])
+print(result)
+```
+### Running parallel tasks 
+```
+import connpy
+conf = connpy.configfile()
+#You can get the nodes from the config from a folder and fitlering in it
+nodes = conf.getitem("@office", ["router1", "router2", "router3"])
+#You can also get each node individually:
+nodes = {}
+nodes["router1"] = conf.getitem("router1@office")
+nodes["router2"] = conf.getitem("router2@office")
+nodes["router10"] = conf.getitem("router10@datacenter")
+#Also, you can create the nodes manually:
+nodes = {}
+nodes["router1"] = {"host": "1.1.1.1", "user": "user", "password": "pass1"}
+nodes["router2"] = {"host": "1.1.1.2", "user": "user", "password": "pass2"}
+nodes["router3"] = {"host": "1.1.1.2", "user": "user", "password": "pass3"}
+#Finally you run some tasks on the nodes
+mynodes = connpy.nodes(nodes, config = conf)
+result = mynodes.test(["show ip int br"], "1.1.1.2")
+for i in result:
+    print("---" + i + "---")
+    print(result[i])
+    print()
+# Or for one specific node
+mynodes.router1.run(["term len 0". "show run"], folder = "/home/user/logs")
+```
+### Using variables
+```
+import connpy
+config = connpy.configfile()
+nodes = config.getitem("@office", ["router1", "router2", "router3"])
+commands = []
+commands.append("config t")
+commands.append("interface lo {id}")
+commands.append("ip add {ip} {mask}")
+commands.append("end")
+variables = {}
+variables["router1@office"] = {"ip": "10.57.57.1"}
+variables["router2@office"] = {"ip": "10.57.57.2"}
+variables["router3@office"] = {"ip": "10.57.57.3"}
+variables["__global__"] = {"id": "57"}
+variables["__global__"]["mask"] =  "255.255.255.255"
+expected = "!"
+routers = connpy.nodes(nodes, config = config)
+routers.run(commands, variables)
+routers.test("ping {ip}", expected, variables)
+for key in routers.result:
+    print(key, ' ---> ', ("pass" if routers.result[key] else "fail"))
+```
+### Using AI
+```
+import connpy
+conf = connpy.configfile()
+organization = 'openai-org'
+api_key = "openai-key"
+myia = ai(conf, organization, api_key)
+input = "go to router 1 and get me the full configuration"
+result = myia.ask(input, dryrun = False)
+print(result)
+```
+'''
+from .core import node,nodes
+from .configfile import configfile
+from .connapp import connapp
+from .api import *
+from .ai import ai
+from .plugins import Plugins
+from ._version import __version__
+from pkg_resources import get_distribution
+
+__all__ = ["node", "nodes", "configfile", "connapp", "ai", "Plugins"]
+__author__ = "Federico Luzzi"
+__pdoc__ = {
+    'core': False,
+    'completion': False,
+    'api': False,
+    'plugins': False
+}
```

### Comparing `connpy-4.0.0b3/connpy/ai.py` & `connpy-4.0.0b5/connpy/ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 import time
 import json
 import re
 import ast
 from textwrap import dedent
 from .core import nodes
 from copy import deepcopy
+from .hooks import ClassHook,MethodHook
 
+@ClassHook
 class ai:
     ''' This class generates a ai object. Containts all the information and methods to make requests to openAI chatGPT to run actions on the application.
 
     ### Attributes:  
 
         - model        (str): Model of GPT api to use. Default is gpt-3.5-turbo.
 
@@ -171,24 +173,26 @@
         self.__prompt["confirmation_function"]["parameters"]["properties"]["result"]["type"] = "string"
         self.__prompt["confirmation_function"]["parameters"]["properties"]["result"]["enum"] = ["true", "false", "none"]
         self.__prompt["confirmation_function"]["parameters"]["properties"]["response"] = {}
         self.__prompt["confirmation_function"]["parameters"]["properties"]["response"]["description"] = "If the user don't message is not an affiramtion or negation, kindly ask the user to rephrase."
         self.__prompt["confirmation_function"]["parameters"]["properties"]["response"]["type"] = "string"
         self.__prompt["confirmation_function"]["parameters"]["required"] = ["result"]
 
+    @MethodHook
     def process_string(self, s):
         if s.startswith('[') and s.endswith(']') and not (s.startswith("['") and s.endswith("']")) and not (s.startswith('["') and s.endswith('"]')):
             # Extract the content inside square brackets and split by comma
             content = s[1:-1].split(',')
             # Add single quotes around each item and join them back together with commas
             new_content = ', '.join(f"'{item.strip()}'" for item in content)
             # Replace the old content with the new content
             s = '[' + new_content + ']'
         return s
 
+    @MethodHook
     def _retry_function(self, function, max_retries, backoff_num, *args):
         #Retry openai requests
         retries = 0
         while retries < max_retries:
             try:
                 myfunction = function(*args)
                 break
@@ -197,14 +201,15 @@
                 time.sleep(wait_time)
                 retries += 1
                 continue
         if retries == max_retries:
             myfunction = False
         return myfunction
 
+    @MethodHook
     def _clean_command_response(self, raw_response, node_list):
         #Parse response for command request to openAI GPT.
         info_dict = {}
         info_dict["commands"] = []
         info_dict["variables"] = {}
         info_dict["variables"]["__global__"] = {}
         for key, value in node_list.items():
@@ -214,14 +219,15 @@
                 newvalue[f"command{i}"] = e
                 if f"{{command{i}}}" not in info_dict["commands"]:
                     info_dict["commands"].append(f"{{command{i}}}")
                     info_dict["variables"]["__global__"][f"command{i}"] = ""
                 info_dict["variables"][key] = newvalue
         return info_dict
 
+    @MethodHook
     def _get_commands(self, user_input, nodes):
         #Send the request for commands for each device to openAI GPT.
         output_list = []
         command_function = deepcopy(self.__prompt["command_function"])
         node_list = {}
         for key, value in nodes.items():
             tags = value.get('tags', {})
@@ -253,14 +259,15 @@
             )
         output = {}
         result = response["choices"][0]["message"].to_dict()
         json_result = json.loads(result["function_call"]["arguments"])
         output["response"] = self._clean_command_response(json_result, node_list)
         return output
 
+    @MethodHook
     def _get_filter(self, user_input, chat_history = None):
         #Send the request to identify the filter and other attributes from the user input to GPT.
         message = []
         message.append({"role": "system", "content": dedent(self.__prompt["original_system"]).strip()})
         message.append({"role": "user", "content": dedent(self.__prompt["original_user"]).strip()})
         message.append({"role": "assistant", "content": None, "function_call": self.__prompt["original_assistant"]})
         functions = [self.__prompt["original_function"]]
@@ -294,14 +301,15 @@
             output["filter"] = json_result["filter"]
             output["type"] = json_result["type"]
             chat_history.append({"role": "assistant", "content": result["content"], "function_call": {"name": result["function_call"]["name"], "arguments": json.dumps(json_result)}})
         output["expected"] = expected
         output["chat_history"] = chat_history
         return output
         
+    @MethodHook
     def _get_confirmation(self, user_input):
         #Send the request to identify if user is confirming or denying the task
         message = []
         message.append({"role": "user", "content": user_input})
         functions = [self.__prompt["confirmation_function"]]
         response = openai.ChatCompletion.create(
             model=self.model,
@@ -318,14 +326,15 @@
             output["result"] = True
         elif json_result["result"] == "false":
             output["result"] = False
         elif json_result["result"] == "none":
             output["result"] = json_result["response"]
         return output
 
+    @MethodHook
     def confirm(self, user_input, max_retries=3, backoff_num=1):
         '''
         Send the user input to openAI GPT and verify if response is afirmative or negative.
 
         ### Parameters:  
 
             - user_input (str): User response confirming or denying.
@@ -343,14 +352,15 @@
         result = self._retry_function(self._get_confirmation, max_retries, backoff_num, user_input)
         if result:
             output = result["result"]
         else:
             output = f"{self.model} api is not responding right now, please try again later."
         return output
 
+    @MethodHook
     def ask(self, user_input, dryrun = False, chat_history = None,  max_retries=3, backoff_num=1):
         '''
         Send the user input to openAI GPT and parse the response to run an action in the application.
 
         ### Parameters:  
 
             - user_input (str): Request to send to openAI that will be parsed
```

### Comparing `connpy-4.0.0b3/connpy/api.py` & `connpy-4.0.0b5/connpy/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from flask import Flask, request, jsonify
-from connpy import configfile, node, nodes
+from connpy import configfile, node, nodes, hooks
 from connpy.ai import ai as myai
 from waitress import serve
 import os
 import signal
 
 app = Flask(__name__)
 conf = configfile()
@@ -122,14 +122,15 @@
         output["result"] = mynodes.test(**args)
         output["output"] = mynodes.output
     else:
         error = "Wrong action '{}'".format(action)
         return({"DataError": error})
     return output
 
+@hooks.MethodHook
 def stop_api():
     # Read the process ID (pid) from the file
     try:
         with open(PID_FILE1, "r") as f:
             pid = int(f.readline().strip())
             port = int(f.readline().strip())
         PID_FILE=PID_FILE1
@@ -148,22 +149,25 @@
     except:
         pass
     # Delete the PID file
     os.remove(PID_FILE)
     print(f"Server with process ID {pid} stopped.")
     return port
 
+@hooks.MethodHook
 def debug_api(port=8048):
     app.custom_config = configfile()
     app.run(debug=True, port=port)
 
+@hooks.MethodHook
 def start_server(port=8048):
     app.custom_config = configfile()
     serve(app, host='0.0.0.0', port=port)
 
+@hooks.MethodHook
 def start_api(port=8048):
     if os.path.exists(PID_FILE1) or os.path.exists(PID_FILE2):
         print("Connpy server is already running.")
         return
     pid = os.fork()
     if pid == 0:
         start_server(port)
```

### Comparing `connpy-4.0.0b3/connpy/completion.py` & `connpy-4.0.0b5/connpy/completion.py`

 * *Files identical despite different names*

### Comparing `connpy-4.0.0b3/connpy/configfile.py` & `connpy-4.0.0b5/connpy/configfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 #Imports
 import json
 import os
 import re
 from Crypto.PublicKey import RSA
 from pathlib import Path
 from copy import deepcopy
-from .hooks import ConfigHook
+from .hooks import MethodHook, ClassHook
 
 
 
 #functions and classes
 
+@ClassHook
 class configfile:
     ''' This class generates a configfile object. Containts a dictionary storing, config, nodes and profiles, normaly used by connection manager.
 
     ### Attributes:  
 
         - file         (str): Path/file to config file.
 
@@ -103,15 +104,15 @@
                 f.close()
                 os.chmod(conf, 0o600)
         jsonconf = open(conf)
         jsondata = json.load(jsonconf)
         jsonconf.close()
         return jsondata
 
-    @ConfigHook
+    @MethodHook
     def _saveconfig(self, conf):
         #Save config file
         newconfig = {"config":{}, "connections": {}, "profiles": {}}
         newconfig["config"] = self.config
         newconfig["connections"] = self.connections
         newconfig["profiles"] = self.profiles
         try:
@@ -127,14 +128,15 @@
         key = RSA.generate(2048)
         with open(keyfile,'wb') as f:
             f.write(key.export_key('PEM'))
             f.close()
             os.chmod(keyfile, 0o600)
         return key
 
+    @MethodHook
     def _explode_unique(self, unique):
         #Divide unique name into folder, subfolder and id
         uniques = unique.split("@")
         if not unique.startswith("@"):
             result = {"id": uniques[0]}
         else:
             result = {}
@@ -147,14 +149,15 @@
             result["subfolder"] = uniques[1]
             if result["folder"] == "" or result["subfolder"] == "":
                 return False
         elif len(uniques) > 3:
             return False
         return result
 
+    @MethodHook
     def getitem(self, unique, keys = None):
         '''
         Get an node or a group of nodes from configfile which can be passed to node/nodes class
 
         ### Parameters:  
 
             - unique (str): Unique name of the node or folder in config using
@@ -202,14 +205,15 @@
                 node = self.connections[uniques["folder"]][uniques["id"]]
             else:
                 node = self.connections[uniques["id"]]
             newnode = deepcopy(node)
             newnode.pop("type")
             return newnode
 
+    @MethodHook
     def getitems(self, uniques):
         '''
         Get a group of nodes from configfile which can be passed to node/nodes class
 
         ### Parameters:  
 
             - uniques (str/list): String name that will match hostnames 
@@ -243,59 +247,66 @@
                 if not self.config["case"]:
                     i = i.lower()
                 this = self.getitem(i)
                 nodes[i] = this
         return nodes
 
 
+    @MethodHook
     def _connections_add(self,*, id, host, folder='', subfolder='', options='', logs='', password='', port='', protocol='', user='', tags='', jumphost='', type = "connection" ):
         #Add connection from config
         if folder == '':
             self.connections[id] = {"host": host, "options": options, "logs": logs, "password": password, "port": port, "protocol": protocol, "user": user, "tags": tags,"jumphost": jumphost,"type": type}
         elif folder != '' and subfolder == '':
             self.connections[folder][id] = {"host": host, "options": options, "logs": logs, "password": password, "port": port, "protocol": protocol, "user": user, "tags": tags, "jumphost": jumphost, "type": type}
         elif folder != '' and subfolder != '':
             self.connections[folder][subfolder][id] = {"host": host, "options": options, "logs": logs, "password": password, "port": port, "protocol": protocol, "user": user, "tags": tags,  "jumphost": jumphost, "type": type}
             
 
+    @MethodHook
     def _connections_del(self,*, id, folder='', subfolder=''):
         #Delete connection from config
         if folder == '':
             del self.connections[id]
         elif folder != '' and subfolder == '':
             del self.connections[folder][id]
         elif folder != '' and subfolder != '':
             del self.connections[folder][subfolder][id]
 
+    @MethodHook
     def _folder_add(self,*, folder, subfolder = ''):
         #Add Folder from config
         if subfolder == '':
             if folder not in self.connections:
                 self.connections[folder] = {"type": "folder"}
         else:
             if subfolder not in self.connections[folder]:
                 self.connections[folder][subfolder] = {"type": "subfolder"}
 
+    @MethodHook
     def _folder_del(self,*, folder, subfolder=''):
         #Delete folder from config
         if subfolder == '':
             del self.connections[folder]
         else:
             del self.connections[folder][subfolder]
 
 
+    @MethodHook
     def _profiles_add(self,*, id, host = '', options='', logs='', password='', port='', protocol='', user='', tags='', jumphost='' ):
         #Add profile from config
         self.profiles[id] = {"host": host, "options": options, "logs": logs, "password": password, "port": port, "protocol": protocol, "user": user, "tags": tags, "jumphost": jumphost}
             
 
+    @MethodHook
     def _profiles_del(self,*, id ):
         #Delete profile from config
         del self.profiles[id]
         
+    @MethodHook
     def _getallnodes(self, filter = None):
         #get all nodes on configfile
         nodes = []
         layer1 = [k for k,v in self.connections.items() if isinstance(v, dict) and v["type"] == "connection"]
         folders = [k for k,v in self.connections.items() if isinstance(v, dict) and v["type"] == "folder"]
         nodes.extend(layer1)
         for f in folders:
@@ -310,14 +321,15 @@
                 nodes = [item for item in nodes if re.search(filter, item)]
             elif isinstance(filter, list):
                 nodes = [item for item in nodes if any(re.search(pattern, item) for pattern in filter)]
             else:
                 raise ValueError("filter must be a string or a list of strings")
         return nodes
 
+    @MethodHook
     def _getallnodesfull(self, filter = None, extract = True):
         #get all nodes on configfile with all their attributes.
         nodes = {}
         layer1 = {k:v for k,v in self.connections.items() if isinstance(v, dict) and v["type"] == "connection"}
         folders = [k for k,v in self.connections.items() if isinstance(v, dict) and v["type"] == "folder"]
         nodes.update(layer1)
         for f in folders:
@@ -349,24 +361,26 @@
                         try:
                             nodes[node][key] = config.profiles["default"][key]
                         except:
                             nodes[node][key] = "ssh"
         return nodes
 
 
+    @MethodHook
     def _getallfolders(self):
         #get all folders on configfile
         folders = ["@" + k for k,v in self.connections.items() if isinstance(v, dict) and v["type"] == "folder"]
         subfolders = []
         for f in folders:
             s = ["@" + k + f for k,v in self.connections[f[1:]].items() if isinstance(v, dict) and v["type"] == "subfolder"]
             subfolders.extend(s)
         folders.extend(subfolders)
         return folders
 
+    @MethodHook
     def _profileused(self, profile):
         #Check if profile is used before deleting it
         nodes = []
         layer1 = [k for k,v in self.connections.items() if isinstance(v, dict) and v["type"] == "connection" and ("@" + profile in v.values() or ( isinstance(v["password"],list) and "@" + profile in v["password"]))]
         folders = [k for k,v in self.connections.items() if isinstance(v, dict) and v["type"] == "folder"]
         nodes.extend(layer1)
         for f in folders:
```

### Comparing `connpy-4.0.0b3/connpy/connapp.py` & `connpy-4.0.0b5/connpy/connapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,21 @@
 
             - config (obj): Object generated with configfile class, it contains
                             the nodes configuration and the methods to manage
                             the config file.
 
         '''
         self.node = node
-        self.connnodes = nodes
+        self.nodes = nodes
+        self.start_api = start_api
+        self.stop_api = stop_api
+        self.debug_api = debug_api
+        self.ai = ai
         self.config = config
-        self.nodes = self.config._getallnodes()
+        self.nodes_list = self.config._getallnodes()
         self.folders = self.config._getallfolders()
         self.profiles = list(self.config.profiles.keys())
         self.case = self.config.config["case"]
         try:
             self.fzf = self.config.config["fzf"]
         except:
             self.fzf = False
@@ -207,24 +211,24 @@
         return actions.get(args.action)(args)
 
     def _version(self, args):
         print(__version__)
 
     def _connect(self, args):
         if args.data == None:
-            matches = self.nodes
+            matches = self.nodes_list
             if len(matches) == 0:
                 print("There are no nodes created")
                 print("try: conn --help")
                 exit(9)
         else:
             if args.data.startswith("@"):
-                matches = list(filter(lambda k: args.data in k, self.nodes))
+                matches = list(filter(lambda k: args.data in k, self.nodes_list))
             else:
-                matches = list(filter(lambda k: k.startswith(args.data), self.nodes))
+                matches = list(filter(lambda k: k.startswith(args.data), self.nodes_list))
         if len(matches) == 0:
             print("{} not found".format(args.data))
             exit(2)
         elif len(matches) > 1:
             matches[0] = self._choose(matches,"node", "connect")
         if matches[0] == None:
             exit(7)
@@ -271,18 +275,18 @@
         args.data = self._type_node(args.data)
         if args.data == None:
             print("Missing argument node")
             exit(3)
         elif args.data.startswith("@"):
             type = "folder"
             matches = list(filter(lambda k: k == args.data, self.folders))
-            reversematches = list(filter(lambda k: "@" + k == args.data, self.nodes))
+            reversematches = list(filter(lambda k: "@" + k == args.data, self.nodes_list))
         else:
             type = "node"
-            matches = list(filter(lambda k: k == args.data, self.nodes))
+            matches = list(filter(lambda k: k == args.data, self.nodes_list))
             reversematches = list(filter(lambda k: k == "@" + args.data, self.folders))
         if len(matches) > 0:
             print("{} already exist".format(matches[0]))
             exit(4)
         if len(reversematches) > 0:
             print("{} already exist".format(reversematches[0]))
             exit(4)
@@ -322,15 +326,15 @@
                 self.config._saveconfig(self.config.file)
                 print("{} added succesfully".format(args.data))
 
     def _show(self, args):
         if args.data == None:
             print("Missing argument node")
             exit(3)
-        matches = list(filter(lambda k: k == args.data, self.nodes))
+        matches = list(filter(lambda k: k == args.data, self.nodes_list))
         if len(matches) == 0:
             print("{} not found".format(args.data))
             exit(2)
         node = self.config.getitem(matches[0])
         for k, v in node.items():
             if isinstance(v, str):
                 print(k + ": " + v)
@@ -507,16 +511,16 @@
             items = newitems
         print(*items, sep="\n")
 
     def _mvcp(self, args):
         if not self.case:
             args.data[0] = args.data[0].lower()
             args.data[1] = args.data[1].lower()
-        source = list(filter(lambda k: k == args.data[0], self.nodes))
-        dest = list(filter(lambda k: k == args.data[1], self.nodes))
+        source = list(filter(lambda k: k == args.data[0], self.nodes_list))
+        dest = list(filter(lambda k: k == args.data[1], self.nodes_list))
         if len(source) != 1:
             print("{} not found".format(args.data[0]))
             exit(2)
         if len(dest) > 0:
             print("Node {} Already exist".format(args.data[1]))
             exit(4)
         nodefolder = args.data[1].partition("@")
@@ -546,15 +550,15 @@
             newnodes["location"] = newnodes["location"].lower()
             newnodes["ids"] = newnodes["ids"].lower()
         ids = newnodes["ids"].split(",")
         hosts = newnodes["host"].split(",")
         count = 0
         for n in ids:
             unique = n + newnodes["location"]
-            matches = list(filter(lambda k: k == unique, self.nodes))
+            matches = list(filter(lambda k: k == unique, self.nodes_list))
             reversematches = list(filter(lambda k: k == "@" + unique, self.folders))
             if len(matches) > 0:
                 print("Node {} already exist, ignoring it".format(unique))
                 continue
             if len(reversematches) > 0:
                 print("Folder with name {} already exist, ignoring it".format(unique))
                 continue
@@ -573,15 +577,15 @@
             newnode["logs"] = newnodes["logs"]
             newnode["tags"] = newnodes["tags"]
             newnode["jumphost"] = newnodes["jumphost"]
             newnode["user"] = newnodes["user"]
             newnode["password"] = newnodes["password"]
             count +=1
             self.config._connections_add(**newnode)
-            self.nodes = self.config._getallnodes()
+            self.nodes_list = self.config._getallnodes()
         if count > 0:
             self.config._saveconfig(self.config.file)
             print("Succesfully added {} nodes".format(count))
         else:
             print("0 nodes added")
 
     def _completion(self, args):
@@ -825,15 +829,15 @@
         arguments = {}
         if args.model:
             arguments["model"] = args.model[0]
         if args.org:
             arguments["org"] = args.org[0]
         if args.api_key:
             arguments["api_key"] = args.api_key[0]
-        self.myai = ai(self.config, **arguments)
+        self.myai = self.ai(self.config, **arguments)
         if args.ask:
             input = " ".join(args.ask)
             request = self.myai.ask(input, dryrun = True)
             if not request["app_related"]:
                 mdprint(Markdown(request["response"]))
                 print("\r")
             else:
@@ -916,15 +920,15 @@
                     if answers == None:
                         exit(7)
                     confirmation = self.myai.confirm(answers["message"])
                     if isinstance(confirmation, bool):
                         if not confirmation:
                             response = "Request cancelled"
                         else:
-                            nodes = self.connnodes(self.config.getitems(response["nodes"]), config = self.config)
+                            nodes = self.nodes(self.config.getitems(response["nodes"]), config = self.config)
                             if response["action"] == "run":
                                 output = nodes.run(**response["args"])
                                 response = ""
                             elif response["action"] == "test":
                                 result = nodes.test(**response["args"])
                                 yaml_result = yaml.dump(result,default_flow_style=False, indent=4)
                                 output = nodes.output
@@ -932,25 +936,25 @@
                             for k,v in output.items():
                                 response += f"\n***{k}***:\n```\n{v}\n```\n"
                         break
             return response, history
 
     def _func_api(self, args):
         if args.command == "stop" or args.command == "restart":
-            args.data = stop_api()
+            args.data = self.stop_api()
         if args.command == "start" or args.command == "restart":
             if args.data:
-                start_api(args.data)
+                self.start_api(args.data)
             else:
-                start_api()
+                self.start_api()
         if args.command == "debug":
             if args.data:
-                debug_api(args.data)
+                self.debug_api(args.data)
             else:
-                debug_api()
+                self.debug_api()
         return
 
     def _node_run(self, args):
         command = " ".join(args.data[1:])
         script = {}
         script["name"] = "Output"
         script["action"] = "run"
@@ -993,15 +997,15 @@
         except KeyError as e:
             print("'{}' is mandatory".format(e.args[0]))
             exit(11)
         nodes = self.config._getallnodes(nodelist)
         if len(nodes) == 0:
             print("{} don't match any node".format(nodelist))
             exit(2)
-        nodes = self.connnodes(self.config.getitems(nodes), config = self.config)
+        nodes = self.nodes(self.config.getitems(nodes), config = self.config)
         stdout = False
         if output is None:
             pass
         elif output == "stdout":
             stdout = True
         elif isinstance(output, str) and action == "run":
             args["folder"] = output
@@ -1154,22 +1158,22 @@
 
     def _jumphost_validation(self, answers, current):
         #Validation for Jumphost in inquirer when managing nodes
         if current.startswith("@"):
             if current[1:] not in self.profiles:
                 raise inquirer.errors.ValidationError("", reason="Profile {} don't exist".format(current))
         elif current != "":
-            if current not in self.nodes :
+            if current not in self.nodes_list :
                 raise inquirer.errors.ValidationError("", reason="Node {} don't exist.".format(current))
         return True
 
     def _profile_jumphost_validation(self, answers, current):
         #Validation for Jumphost in inquirer when managing profiles
         if current != "":
-            if current not in self.nodes :
+            if current not in self.nodes_list :
                 raise inquirer.errors.ValidationError("", reason="Node {} don't exist.".format(current))
         return True
 
     def _default_validation(self, answers, current):
         #Default validation type used in multiples questions in inquirer
         if current.startswith("@"):
             if current[1:] not in self.profiles:
```

### Comparing `connpy-4.0.0b3/connpy/core.py` & `connpy-4.0.0b5/connpy/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 import ast
 from time import sleep,time
 import datetime
 import sys
 import threading
 from pathlib import Path
 from copy import deepcopy
+from .hooks import ClassHook, MethodHook
 import io
 
 #functions and classes
-
+@ClassHook
 class node:
     ''' This class generates a node object. Containts all the information and methods to connect and interact with a device using ssh or telnet.
 
     ### Attributes:  
 
         - output (str): Output of the commands you ran with run or test 
                         method.  
@@ -135,14 +136,15 @@
                     jumphost_cmd = jumphost_cmd + " {}".format(self.jumphost["host"])
                 else:
                     jumphost_cmd = jumphost_cmd + " {}".format("@".join([self.jumphost["user"],self.jumphost["host"]]))
                 self.jumphost = f"-o ProxyCommand=\"{jumphost_cmd}\""
             else:
                 self.jumphost = ""
 
+    @MethodHook
     def _passtx(self, passwords, *, keyfile=None):
         # decrypts passwords, used by other methdos.
         dpass = []
         if keyfile is None:
             keyfile = self.key
         if keyfile is not None:
             with open(keyfile) as f:
@@ -157,14 +159,15 @@
                     dpass.append(decrypted)
                 except:
                     raise ValueError("Missing or corrupted key")
         return dpass
 
     
 
+    @MethodHook
     def _logfile(self, logfile = None):
         # translate logs variables and generate logs path.
         if logfile == None:
             logfile = self.logs
         logfile = logfile.replace("${unique}", self.unique)
         logfile = logfile.replace("${host}", self.host)
         logfile = logfile.replace("${port}", self.port)
@@ -172,14 +175,15 @@
         logfile = logfile.replace("${protocol}", self.protocol)
         now = datetime.datetime.now()
         dateconf = re.search(r'\$\{date \'(.*)\'}', logfile)
         if dateconf:
             logfile = re.sub(r'\$\{date (.*)}',now.strftime(dateconf.group(1)), logfile)
         return logfile
 
+    @MethodHook
     def _logclean(self, logfile, var = False):
         #Remove special ascii characters and other stuff from logfile.
         if var == False:
             t = open(logfile, "r").read()
         else:
             t = logfile
         while t.find("\b") != -1:
@@ -198,14 +202,15 @@
             d = open(logfile, "w")
             d.write(t)
             d.close()
             return
         else:
             return t
 
+    @MethodHook
     def _savelog(self):
         '''Save the log buffer to the file at regular intervals if there are changes.'''
         t = threading.current_thread()
         prev_size = 0  # Store the previous size of the buffer
 
         while getattr(t, "do_run", True):  # Check if thread is signaled to stop
             current_size = self.mylog.tell()  # Current size of the buffer
@@ -213,30 +218,33 @@
             # Only save if the buffer size has changed
             if current_size != prev_size:
                 with open(self.logfile, "w") as f:  # Use "w" to overwrite the file
                     f.write(self._logclean(self.mylog.getvalue().decode(), True))
                 prev_size = current_size  # Update the previous size
             sleep(5)
 
+    @MethodHook
     def _filter(self, a):
         #Set time for last input when using interact
         self.lastinput = time()
         return a
 
+    @MethodHook
     def _keepalive(self):
         #Send keepalive ctrl+e when idletime passed without new inputs on interact
         self.lastinput = time()
         t = threading.current_thread()
         while True:
             if time() - self.lastinput >= self.idletime:
                 self.child.sendcontrol("e")
                 self.lastinput = time()
             sleep(1)
 
 
+    @MethodHook
     def interact(self, debug = False):
         '''
         Allow user to interact with the node directly, mostly used by connection manager.
 
         ### Optional Parameters:  
 
             - debug (bool): If True, display all the connecting information 
@@ -270,14 +278,15 @@
                 with open(self.logfile, "w") as f:
                     f.write(self._logclean(self.mylog.getvalue().decode(), True))
 
         else:
             print(connect)
             exit(1)
 
+    @MethodHook
     def run(self, commands, vars = None,*, folder = '', prompt = r'>$|#$|\$$|>.$|#.$|\$.$', stdout = False, timeout = 10):
         '''
         Run a command or list of commands on the node and return the output.
 
         ### Parameters:  
 
             - commands (str/list): Commands to run on the node. Should be 
@@ -358,14 +367,15 @@
                 print(connect)
             if folder != '':
                 with open(folder + "/" + self.unique + "_" + now + ".txt", "w") as f:
                     f.write(connect)
                     f.close()
             return connect
 
+    @MethodHook
     def test(self, commands, expected, vars = None,*, prompt = r'>$|#$|\$$|>.$|#.$|\$.$', timeout = 10):
         '''
         Run a command or list of commands on the node, then check if expected value appears on the output after the last command.
 
         ### Parameters:  
 
             - commands (str/list): Commands to run on the node. Should be
@@ -453,14 +463,15 @@
                 return output
         else:
             self.result = None
             self.output = connect
             self.status = 1
             return connect
 
+    @MethodHook
     def _connect(self, debug = False, timeout = 10, max_attempts = 3):
         # Method to connect to the node, it parse all the information, create the ssh/telnet command and login to the node.
         if self.protocol in ["ssh", "sftp"]:
             cmd = self.protocol
             if self.idletime > 0:
                 cmd = cmd + " -o ServerAliveInterval=" + str(self.idletime)
             if self.port != '':
@@ -553,14 +564,15 @@
                 continue
             else:
                 break
         child.readline(0)
         self.child = child
         return True
 
+@ClassHook
 class nodes:
     ''' This class generates a nodes object. Contains a list of node class objects and methods to run multiple tasks on nodes simultaneously.
 
     ### Attributes:  
 
         - nodelist (list): List of node class objects passed to the init 
                            function.  
@@ -604,20 +616,22 @@
         self.config = config
         for n in nodes:
             this = node(n, **nodes[n], config = config)
             self.nodelist.append(this)
             setattr(self,n,this)
 
     
+    @MethodHook
     def _splitlist(self, lst, n):
         #split a list in lists of n members.
         for i in range(0, len(lst), n):
             yield lst[i:i + n]
 
 
+    @MethodHook
     def run(self, commands, vars = None,*, folder = None, prompt = None, stdout = None, parallel = 10, timeout = None):
         '''
         Run a command or list of commands on all the nodes in nodelist.
 
         ### Parameters:  
 
             - commands (str/list): Commands to run on the nodes. Should be str or 
@@ -694,14 +708,15 @@
         for i in self.nodelist:
             output[i.unique] = i.output
             status[i.unique] = i.status
         self.output = output
         self.status = status
         return output
 
+    @MethodHook
     def test(self, commands, expected, vars = None,*, prompt = None, parallel = 10, timeout = None):
         '''
         Run a command or list of commands on all the nodes in nodelist, then check if expected value appears on the output after the last command.
 
         ### Parameters:  
 
             - commands (str/list): Commands to run on the node. Should be str or
```

### Comparing `connpy-4.0.0b3/connpy/core_plugins/sync.py` & `connpy-4.0.0b5/connpy/core_plugins/sync.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import argparse
 import os
 import time
 import zipfile
 import tempfile
 import io
 import yaml
+import threading
 from google.oauth2.credentials import Credentials
 from google.auth.transport.requests import Request
 from googleapiclient.discovery import build
 from google.auth.exceptions import RefreshError
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.http import MediaFileUpload,MediaIoBaseDownload
 from googleapiclient.errors import HttpError
@@ -19,16 +20,17 @@
 
     def __init__(self, connapp):
         self.scopes = ['https://www.googleapis.com/auth/drive.appdata']
         self.token_file = f"{connapp.config.defaultdir}/gtoken.json"
         self.file = connapp.config.file
         self.key = connapp.config.key
         self.google_client = f"{os.path.dirname(os.path.abspath(__file__))}/sync_client"
+        self.connapp = connapp
         try:
-            self.sync = connapp.config.config["sync"]
+            self.sync = self.connapp.config.config["sync"]
         except:
             self.sync = False
 
     def login(self):
         creds = None
         # The file token.json stores the user's access and refresh tokens.
         if os.path.exists(self.token_file):
@@ -289,26 +291,37 @@
         if self.decompress_zip(temp_download_path):
             print("Failed to decompress the file.")
             return 1
 
         print(f"Backup from Google Drive restored successfully: {selected_file['name']}")
         return 0
 
-    # @staticmethod
-    def config_listener_post(self, file, result):
+    def config_listener_post(self, args, kwargs):
         if self.sync:
             if self.check_login_status() == True:
-                if not result:
+                if not kwargs["result"]:
                     self.compress_and_upload()
-        return result
+        return kwargs["result"]
+
+    def config_listener_pre(self, *args, **kwargs):
+        try:
+            self.sync = self.connapp.config.config["sync"]
+        except:
+            self.sync = False
+        return args, kwargs
+
+    def start_post_thread(self, *args, **kwargs):
+        post_thread = threading.Thread(target=self.config_listener_post, args=(args,kwargs))
+        post_thread.start()
 
 class Preload:
     def __init__(self, connapp):
         syncapp = sync(connapp)
-        connapp.config._saveconfig.register_post_hook(syncapp.config_listener_post)
+        connapp.config._saveconfig.register_post_hook(syncapp.start_post_thread)
+        connapp.config._saveconfig.register_pre_hook(syncapp.config_listener_pre)
 
 class Parser:
     def __init__(self):
         self.parser = argparse.ArgumentParser(description="Sync config with Google")
         self.description = "Sync config with Google"
         subparsers = self.parser.add_subparsers(title="Commands", dest='command',metavar="")
         login_parser = subparsers.add_parser("login", help="Login to Google to enable synchronization")
@@ -320,16 +333,14 @@
         restore_parser.add_argument("--id", type=str, help="Optional file ID to restore a specific backup", required=False)
         status_parser = subparsers.add_parser("status", help="Check the current status of synchronization")
         list_parser = subparsers.add_parser("list", help="List all backups stored on Google")
 
 class Entrypoint:
     def __init__(self, args, parser, connapp):
         syncapp = sync(connapp)
-        # print(args)
-        # print(syncapp.__dict__)
         if args.command == 'login':
             syncapp.login()
         elif args.command == "status":
             syncapp.status()
         elif args.command == "start":
             connapp._change_settings("sync", True)
         elif args.command == "stop":
@@ -338,85 +349,15 @@
             syncapp.dump_appdata_files_yaml()
         elif args.command == "once":
             syncapp.compress_and_upload()
         elif args.command == "restore":
             syncapp.restore_last_config(args.id)
         elif args.command == "logout":
             syncapp.logout()
-        # if args.command == 'netmask':
-            # if args.file:
-                # for line in args.file:
-                    # line = line.strip()
-                    # if line:
-                        # print(NetmaskTools.process_input(args.conversion, line.strip()))
-            # else:
-                # input_str = ' '.join(args.input)
-                # print(NetmaskTools.process_input(args.conversion, input_str))
-        # elif args.command == 'summarize':
-            # with args.file as file:
-                # subnets = [line.strip() for line in file if line.strip()]
-            # summarized = Sumarize.summarize_subnets(subnets, args.mode)
-            # if isinstance(summarized, list):
-                # for subnet in summarized:
-                    # print(subnet)
-            # else:
-                # print(summarized)
-        # elif args.command == 'password':
-            # if connapp:
-                # for passwd in Password.get_passwords(args, connapp):
-                    # print(passwd)
-        # elif args.command == 'connect':
-            # Connect.connect_command(args)
-        # else:
-            # parser.print_help()
-
 
 def _connpy_completion(wordsnumber, words, info = None):
     if wordsnumber == 3:
-        result = ["--help", "netmask", "summarize", "password", "connect"]
+        result = ["--help", "login", "status", "start", "stop", "list", "once", "restore", "logout"]
     #NETMASK_completion
-    if wordsnumber == 4 and words[1] == "netmask":
-        result = ['cidr_to_netmask', 'cidr_to_wildcard', 
-        'netmask_to_cidr', 'wildcard_to_cidr', 
-        'netmask_to_wildcard', 'wildcard_to_netmask', 'cidr_to_range', "--file", "--help"] 
-    elif wordsnumber == 6 and words[1] == "netmask" and words[2] in ["-f", "--file"]:
-        result = ['cidr_to_netmask', 'cidr_to_wildcard', 
-        'netmask_to_cidr', 'wildcard_to_cidr', 
-        'netmask_to_wildcard', 'wildcard_to_netmask'] 
-    elif wordsnumber == 5 and words[1] == "netmask" and words[2] in ["-f", "--file"]:
-        result = _getcwd(words, words[2])
-    elif wordsnumber == 6 and words[1] == "netmask" and words[3] in ["-f", "--file"]:
-        result = _getcwd(words, words[2])
-    #SUMMARIZE_completion
-    elif wordsnumber == 4 and words[1] == "summarize":
-        result = _getcwd(words, words[1])
-        result.extend(["--mode", "--help"])
-    elif wordsnumber == 5 and words[1] == "summarize":
-        if words[2] == "--mode":
-            result = ["strict", "inclusive"]
-        else:
-            result = ["--mode"]
-    elif wordsnumber == 6 and words[1] == "summarize":
-        if words[3] == "--mode":
-            result = ["strict", "inclusive"]
-        elif words[3] in ["strict", "inclusive"]:
-            result = _getcwd(words, words[3])
-    #PASSWORD_completion
-    elif wordsnumber == 4 and words[1] == "password":
-        result = info["nodes"]
-        result.extend(info["profiles"])
-        result.extend(["--help", "--profile"])
-    elif wordsnumber == 5 and words[1] == "password":
-        if words[2] == "--profile":
-            result = info["profiles"]
-        else:
-            result = ["--profile"]
-    #CONNECT_completion
-    elif wordsnumber == 4 and words[1] == "connect":
-        result = ["start", "stop", "restart", "--help"]
-
+    if wordsnumber == 4 and words[1] == "restore":
+            result = ["--help", "--id"]
     return result
-
-if __name__ == "__main__":
-    parser = Parser()
-    args = parser.parser.parse_args()
-    Entrypoint(args, parser.parser, None)
```

### Comparing `connpy-4.0.0b3/connpy/hooks.py` & `connpy-4.0.0b5/connpy/hooks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,89 @@
 #!/usr/bin/env python3
 #Imports
-from functools import wraps
+from functools import wraps, partial
 
 #functions and classes
 
-class ConfigHook:
-    """Decorator class to enable Config save hooking"""
+class MethodHook:
+    """Decorator class to enable Methods hooking"""
 
     def __init__(self, func):
         self.func = func
         self.pre_hooks = []   # List to store registered pre-hooks
         self.post_hooks = []  # List to store registered post-hooks
         wraps(func)(self)
 
     def __call__(self, *args, **kwargs):
         # Execute pre-hooks before the original function
         for hook in self.pre_hooks:
             try:
                 args, kwargs = hook(*args, **kwargs)
             except Exception as e:
-                print(f"ConfigHook Pre-hook raised an exception: {e}")
+                print(f"{self.func.__name__} Pre-hook {hook.__name__} raised an exception: {e}")
 
         try:
-            # Execute original function
-            result = self.func(self.instance, *args, **kwargs)
+            result = self.func(*args, **kwargs)
 
         finally:
             # Execute post-hooks after the original function
             for hook in self.post_hooks:
                 try:
                     result = hook(*args, **kwargs, result=result)  # Pass result to hooks
                 except Exception as e:
-                    print(f"ConfigHook Post-hook raised an exception: {e}")
+                    print(f"{self.func.__name__} Post-hook {hook.__name__} raised an exception: {e}")
 
         return result
 
     def __get__(self, instance, owner):
-        self.instance = instance
-        return self
+        if not instance:
+            return self
+        else:
+            return self.make_callable(instance)
+
+    def make_callable(self, instance):
+        # Returns a callable that also allows access to hook registration methods
+        callable_instance = partial(self.__call__, instance)
+        callable_instance.register_pre_hook = self.register_pre_hook
+        callable_instance.register_post_hook = self.register_post_hook
+        return callable_instance
 
     def register_pre_hook(self, hook):
         """Register a function to be called before the original function"""
         self.pre_hooks.append(hook)
 
     def register_post_hook(self, hook):
         """Register a function to be called after the original function"""
         self.post_hooks.append(hook)
+
+class ClassHook:
+    """Decorator class to enable Class Modifying"""
+    def __init__(self, cls):
+        self.cls = cls
+        # Initialize deferred class hooks if they don't already exist
+        if not hasattr(cls, 'deferred_class_hooks'):
+            cls.deferred_class_hooks = []
+
+    def __call__(self, *args, **kwargs):
+        instance = self.cls(*args, **kwargs)
+        # Attach instance-specific modify method
+        instance.modify = self.make_instance_modify(instance)
+        # Apply any deferred modifications
+        for hook in self.cls.deferred_class_hooks:
+            hook(instance)
+        return instance
+
+    def __getattr__(self, name):
+        """Delegate attribute access to the class."""
+        return getattr(self.cls, name)
+
+    def modify(self, modification_func):
+        """Queue a modification to be applied to all future instances of the class."""
+        self.cls.deferred_class_hooks.append(modification_func)
+
+    def make_instance_modify(self, instance):
+        """Create a modify function that is bound to a specific instance."""
+        def modify_instance(modification_func):
+            """Modify this specific instance."""
+            modification_func(instance)
+        return modify_instance
+
```

### Comparing `connpy-4.0.0b3/connpy/plugins.py` & `connpy-4.0.0b5/connpy/plugins.py`

 * *Files identical despite different names*

### Comparing `connpy-4.0.0b3/connpy.egg-info/PKG-INFO` & `connpy-4.0.0b5/connpy.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 4.0.0b3
+Version: 4.0.0b5
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
@@ -140,35 +140,122 @@
   - Class definitions
   - Function definitions
   - Import statements
   - The `if __name__ == "__main__":` block for standalone execution
   - Pass statements
 
 ### Specific Class Requirements
-- The plugin script must define at least two specific classes:
+- The plugin script must define specific classes with particular attributes and methods. Each class serves a distinct role within the plugin's architecture:
   1. **Class `Parser`**:
-     - Must contain only one method: `__init__`.
-     - The `__init__` method must initialize at least two attributes:
-       - `self.parser`: An instance of `argparse.ArgumentParser`.
-       - `self.description`: A string containing the description of the parser.
+     - **Purpose**: Handles parsing of command-line arguments.
+     - **Requirements**:
+       - Must contain only one method: `__init__`.
+       - The `__init__` method must initialize at least two attributes:
+         - `self.parser`: An instance of `argparse.ArgumentParser`.
+         - `self.description`: A string containing the description of the parser.
   2. **Class `Entrypoint`**:
-     - Must have an `__init__` method that accepts exactly three parameters besides `self`:
-       - `args`: Arguments passed to the plugin.
-       - The parser instance (typically `self.parser` from the `Parser` class).
-       - The Connapp instance to interact with the Connpy app.
+     - **Purpose**: Acts as the entry point for plugin execution, utilizing parsed arguments and integrating with the main application.
+     - **Requirements**:
+       - Must have an `__init__` method that accepts exactly three parameters besides `self`:
+         - `args`: Arguments passed to the plugin.
+         - The parser instance (typically `self.parser` from the `Parser` class).
+         - The Connapp instance to interact with the Connpy app.
+  3. **Class `Preload`**:
+     - **Purpose**: Performs any necessary preliminary setup or configuration independent of the main parsing and entry logic.
+   - **Requirements**:
+     - Contains at least an `__init__` method that accepts parameter connapp besides `self`.
+
+### Class Dependencies and Combinations
+- **Dependencies**:
+  - `Parser` and `Entrypoint` are interdependent and must both be present if one is included.
+  - `Preload` is independent and may exist alone or alongside the other classes.
+- **Valid Combinations**:
+  - `Parser` and `Entrypoint` together.
+  - `Preload` alone.
+  - All three classes (`Parser`, `Entrypoint`, `Preload`).
+
+### Preload Modifications and Hooks
+
+In the `Preload` class of the plugin system, you have the ability to customize the behavior of existing classes and methods within the application through a robust hooking system. This documentation explains how to use the `modify`, `register_pre_hook`, and `register_post_hook` methods to tailor plugin functionality to your needs.
+
+#### Modifying Classes with `modify`
+The `modify` method allows you to alter instances of a class at the time they are created or after their creation. This is particularly useful for setting or modifying configuration settings, altering default behaviors, or adding new functionalities to existing classes without changing the original class definitions.
+
+- **Usage**: Modify a class to include additional configurations or changes
+- **Modify Method Signature**:
+  - `modify(modification_method)`: A function that is invoked with an instance of the class as its argument. This function should perform any modifications directly on this instance.
+- **Modification Method Signature**:
+  - **Arguments**:
+    - `cls`:  This function accepts a single argument, the class instance, which it then modifies.
+  - **Modifiable Classes**:
+    - `connapp.config`
+    - `connapp.node`
+    - `connapp.nodes`
+    - `connapp.ai`
+  - ```python
+    def modify_config(cls):
+        # Example modification: adding a new attribute or modifying an existing one
+        cls.new_attribute = 'New Value'
+
+    class Preload:
+        def __init__(self, connapp):
+            # Applying modification to the config class instance
+            connapp.config.modify(modify_config)
+    ```
+
+#### Implementing Hooks with `register_pre_hook` and `register_post_hook`
+These methods allow you to define custom logic to be executed before (`register_pre_hook`) or after (`register_post_hook`) the main logic of a method. This is particularly useful for logging, auditing, preprocessing inputs, postprocessing outputs or adding functionalities.
+
+  - **Usage**: Register hooks to methods to execute additional logic before or after the main method execution.
+- **Registration Methods Signature**:
+  - `register_pre_hook(pre_hook_method)`: A function that is invoked before the main method is executed. This function should do preprocessing of the arguments.
+  - `register_post_hook(post_hook_method)`: A function that is invoked after the main method is executed. This function should do postprocessing of the outputs.
+- **Method Signatures for Pre-Hooks**
+  - `pre_hook_method(*args, **kwargs)`
+  - **Arguments**:
+    - `*args`, `**kwargs`: The arguments and keyword arguments that will be passed to the method being hooked. The pre-hook function has the opportunity to inspect and modify these arguments before they are passed to the main method.
+  - **Return**:
+    - Must return a tuple `(args, kwargs)`, which will be used as the new arguments for the main method. If the original arguments are not modified, the function should return them as received.
+- **Method Signatures for Post-Hooks**:
+  - `post_hook_method(*args, **kwargs)`
+  - **Arguments**:
+    - `*args`, `**kwargs`: The arguments and keyword arguments that were passed to the main method.
+      - `kwargs["result"]`: The value returned by the main method. This allows the post-hook to inspect and even alter the result before it is returned to the original caller.
+  - **Return**:
+    - Can return a modified result, which will replace the original result of the main method, or simply return `kwargs["result"]` to return the original method result.    
+  - ```python
+    def pre_processing_hook(*args, **kwargs):
+        print("Pre-processing logic here")
+        # Modify arguments or perform any checks
+        return args, kwargs  # Return modified or unmodified args and kwargs
+
+    def post_processing_hook(*args, **kwargs):
+        print("Post-processing logic here")
+        # Modify the result or perform any final logging or cleanup
+        return kwargs["result"]  # Return the modified or unmodified result
+
+    class Preload:
+        def __init__(self, connapp):
+            # Registering a pre-hook
+            connapp.ai.some_method.register_pre_hook(pre_processing_hook)
+
+            # Registering a post-hook
+            connapp.node.another_method.register_post_hook(post_processing_hook)
+    ```
+  
 
 ### Executable Block
 - The plugin script can include an executable block:
   - `if __name__ == "__main__":`
   - This block allows the plugin to be run as a standalone script for testing or independent use.
 
 ### Script Verification
 - The `verify_script` method in `plugins.py` is used to check the plugin script's compliance with these standards.
 - Non-compliant scripts will be rejected to ensure consistency and proper functionality within the plugin system.
-- 
+ 
 ### Example Script
 
 For a practical example of how to write a compatible plugin script, please refer to the following example:
 
 [Example Plugin Script](https://github.com/fluzzi/awspy)
 
 This script demonstrates the required structure and implementation details according to the plugin system's standards.
```

### Comparing `connpy-4.0.0b3/setup.cfg` & `connpy-4.0.0b5/setup.cfg`

 * *Files identical despite different names*


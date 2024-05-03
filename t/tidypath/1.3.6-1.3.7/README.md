# Comparing `tmp/tidypath-1.3.6.tar.gz` & `tmp/tidypath-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidypath-1.3.6.tar", last modified: Fri Apr 26 08:36:56 2024, max compression
+gzip compressed data, was "tidypath-1.3.7.tar", last modified: Fri May  3 15:36:09 2024, max compression
```

## Comparing `tidypath-1.3.6.tar` & `tidypath-1.3.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-26 08:36:56.813414 tidypath-1.3.6/
--rwxr-xr-x   0 userx     (1000) wheel      (998)    35149 2023-06-08 21:46:44.000000 tidypath-1.3.6/LICENSE.md
--rw-r--r--   0 userx     (1000) wheel      (998)     3682 2024-04-26 08:36:56.813414 tidypath-1.3.6/PKG-INFO
--rwxr-xr-x   0 userx     (1000) wheel      (998)     2804 2023-06-08 21:46:44.000000 tidypath-1.3.6/README.md
--rwxr-xr-x   0 userx     (1000) wheel      (998)      106 2024-04-26 08:36:56.816748 tidypath-1.3.6/setup.cfg
--rwxr-xr-x   0 userx     (1000) wheel      (998)     1161 2024-04-26 08:36:45.000000 tidypath-1.3.6/setup.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-26 08:36:56.813414 tidypath-1.3.6/tidypath/
--rwxr-xr-x   0 userx     (1000) wheel      (998)      371 2023-09-01 13:40:54.000000 tidypath-1.3.6/tidypath/__init__.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     1629 2023-06-08 21:46:44.000000 tidypath-1.3.6/tidypath/_helper.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     4998 2024-02-21 23:01:12.000000 tidypath-1.3.6/tidypath/config.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)    14364 2024-04-26 08:36:36.000000 tidypath-1.3.6/tidypath/decorators.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     6165 2023-07-01 08:06:57.000000 tidypath-1.3.6/tidypath/fmt.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     5197 2023-06-08 21:46:44.000000 tidypath-1.3.6/tidypath/inspection.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)    14158 2024-02-14 00:36:13.000000 tidypath-1.3.6/tidypath/paths.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     9844 2023-06-08 21:46:44.000000 tidypath-1.3.6/tidypath/storage.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-26 08:36:56.813414 tidypath-1.3.6/tidypath.egg-info/
--rwxr-xr-x   0 userx     (1000) wheel      (998)     3682 2024-04-26 08:36:56.000000 tidypath-1.3.6/tidypath.egg-info/PKG-INFO
--rwxr-xr-x   0 userx     (1000) wheel      (998)      358 2024-04-26 08:36:56.000000 tidypath-1.3.6/tidypath.egg-info/SOURCES.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)        1 2024-04-26 08:36:56.000000 tidypath-1.3.6/tidypath.egg-info/dependency_links.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)       63 2024-04-26 08:36:56.000000 tidypath-1.3.6/tidypath.egg-info/requires.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)        9 2024-04-26 08:36:56.000000 tidypath-1.3.6/tidypath.egg-info/top_level.txt
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-05-03 15:36:09.752033 tidypath-1.3.7/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)    35149 2023-06-08 21:46:44.000000 tidypath-1.3.7/LICENSE.md
+-rw-r--r--   0 userx     (1000) wheel      (998)     3682 2024-05-03 15:36:09.752033 tidypath-1.3.7/PKG-INFO
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     2804 2023-06-08 21:46:44.000000 tidypath-1.3.7/README.md
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      106 2024-05-03 15:36:09.752033 tidypath-1.3.7/setup.cfg
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     1161 2024-05-03 15:35:25.000000 tidypath-1.3.7/setup.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-05-03 15:36:09.752033 tidypath-1.3.7/tidypath/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      371 2023-09-01 13:40:54.000000 tidypath-1.3.7/tidypath/__init__.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     1629 2023-06-08 21:46:44.000000 tidypath-1.3.7/tidypath/_helper.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     4998 2024-02-21 23:01:12.000000 tidypath-1.3.7/tidypath/config.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)    14666 2024-05-03 15:35:15.000000 tidypath-1.3.7/tidypath/decorators.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     6165 2023-07-01 08:06:57.000000 tidypath-1.3.7/tidypath/fmt.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     5197 2023-06-08 21:46:44.000000 tidypath-1.3.7/tidypath/inspection.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)    14158 2024-02-14 00:36:13.000000 tidypath-1.3.7/tidypath/paths.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     9844 2023-06-08 21:46:44.000000 tidypath-1.3.7/tidypath/storage.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-05-03 15:36:09.752033 tidypath-1.3.7/tidypath.egg-info/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     3682 2024-05-03 15:36:09.000000 tidypath-1.3.7/tidypath.egg-info/PKG-INFO
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      358 2024-05-03 15:36:09.000000 tidypath-1.3.7/tidypath.egg-info/SOURCES.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)        1 2024-05-03 15:36:09.000000 tidypath-1.3.7/tidypath.egg-info/dependency_links.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)       63 2024-05-03 15:36:09.000000 tidypath-1.3.7/tidypath.egg-info/requires.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)        9 2024-05-03 15:36:09.000000 tidypath-1.3.7/tidypath.egg-info/top_level.txt
```

### Comparing `tidypath-1.3.6/LICENSE.md` & `tidypath-1.3.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.6/PKG-INFO` & `tidypath-1.3.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.3.6
+Version: 1.3.7
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tidypath-1.3.6/README.md` & `tidypath-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.6/setup.py` & `tidypath-1.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tidypath',
-    version='1.3.6',
+    version='1.3.7',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=['tidypath'],
     url='https://github.com/medinajorge/tidypath',
     download_url='https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz',
     description="Automatically store/load data in a tidy, efficient way.",
     long_description=open('README.md').read(),
```

### Comparing `tidypath-1.3.6/tidypath/_helper.py` & `tidypath-1.3.7/tidypath/_helper.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.6/tidypath/config.py` & `tidypath-1.3.7/tidypath/config.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.6/tidypath/decorators.py` & `tidypath-1.3.7/tidypath/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,16 +26,31 @@
 from .paths import datapath, figpath, hash_path
 from .inspection import classify_call_attrs, merge_wrapper_signatures
 from ._helper import merge_nested_dict
 
 class SavedataSkippedComputation:
     pass
 
+def _preprocess_keys_or_function(keys_or_function, keys, extra_keys):
+    if isinstance(keys_or_function, Iterable):
+        func = None
+        if isinstance(keys_or_function, dict):
+            extra_keys = keys_or_function
+        else:
+            keys = keys_or_function
+    elif callable(keys_or_function):
+        func = keys_or_function
+    else:
+        func = None
+    return func, keys, extra_keys
+
+
 def savedata(keys_or_function=None, include_classes="file",
-             ext=config.EXT_DEFAULT_DATA, keys=config.KEYS_DEFAULT_DATA, funcname_in_filename=config.FUNCNAME_IN_FILENAME_DEFAULT_DATA,
+             ext=config.EXT_DEFAULT_DATA, keys=config.KEYS_DEFAULT_DATA, extra_keys={},
+             funcname_in_filename=config.FUNCNAME_IN_FILENAME_DEFAULT_DATA,
              overwrite=False, save=True, load_opts_default_save=True,  #defaults for extra arguments
              max_str_length=255,
              skip_computation=False,
              iterable_maxsize=math.inf,
              load_opts={}, **save_opts):
     """
     Decorator for automatically saving output and then loading cached data.
@@ -46,26 +61,25 @@
     If filename is too long, it is shortened by hashing it.
 
 
     NOTE (!) decorated funcs will have extra arguments:
         - save (bool).                 whether to save the output of the function.
         - overwrite (bool).            whether to overwrite the saved version.
         - funcname_in_filename(bool)   whether to include funcname in the filename.
-        - keys (dict/str/iterable)   · dict:     specifies filename of the form k1-v1_k2-v2_...kn_vn.
-                                                 k_i do not have to be arguments of the function.
-                                     · str:       key of a keyword argument. Example: keys = 'x'.
+        - keys (dict/str/iterable)    · str:       key of a keyword argument. Example: keys = 'x'.
                                                  "kwargs_defaults"  =>  default kwargs that were not modified.
                                                  "kwargs"           =>  kwargs passed during function call.
                                                  "kwargs_full"      =>  kws_defaults + kws.
                                                  "pos_only"         =>  length of *args
                                                  "args"             =>  attrs != **kwargs, *args.
                                                  "all"              if config.KEYS_ADD_POSONLY_TO_ALL  =>  all attrs
                                                                     else                               =>  all attrs except pos_only: kwargs_full + args
                                                  can combine options using "+" or "-". Example: "args+z", "x+y+kwargs", "all-y".
                                      · iterable: containing a combination of the available string keys (above). ["k1", "k2"] == "k1+k2".
+        - extra_keys (dict):         additional keys to be included in the filename. They do not have to be arguments of the function.
         - skip_computation (bool).     whether to skip computation if the data is not stored.
         - ext (str/list/tuple):    storing extension. Selects 'storage' functions save_ext, load_ext.
                                    Supported: 'lzma' (default), 'bz2', 'json', 'csv', 'npz'.
 
 
     Attrs:
         - function:                function to which the decorator is applied
@@ -75,30 +89,26 @@
         - load_opts_default_save:  use save_opts as default for load_opts.
         - max_str_length:          max length of filename. If exceeded, filename is shortened by hashing it.
         - iterable_maxsize:        max size of iterable keys. If exceeded, keys are shortened by counting val numbers.
         - rest:                    default behavior for decorated funcs extra arguments (above).
 
     Returns: Function decorator
     """
-    if isinstance(keys_or_function, Iterable):
-        keys = keys_or_function
-        func = None
-    elif callable(keys_or_function):
-        func = keys_or_function
-    else:
-        func = None
+    func, keys, extra_keys = _preprocess_keys_or_function(keys_or_function, keys, extra_keys)
 
     if load_opts_default_save:
         load_opts = {**save_opts, **load_opts}
 
     def _savedata(func):
         @wraps(func)
-        def wrapper(*args, overwrite=overwrite, keys=keys, save=save, funcname_in_filename=funcname_in_filename, skip_computation=skip_computation, ext=ext, **kwargs):
+        def wrapper(*args, overwrite=overwrite, keys=keys, extra_keys=extra_keys, save=save, funcname_in_filename=funcname_in_filename, skip_computation=skip_computation, ext=ext, **kwargs):
             key_opts = classify_call_attrs(func, args, kwargs, add_pos_only_to_all=config.KEYS_ADD_POSONLY_TO_ALL)
             save_keys = merge_nested_dict(key_opts, keys, key_default="all")
+            if extra_keys:
+                save_keys.update(extra_keys)
 
             def get_saving_path(ext):
                 saving_path = datapath(keys=save_keys, func=func, ext=ext, include_classes=include_classes, funcname_in_filename=funcname_in_filename, iterable_maxsize=iterable_maxsize)
                 filename = os.path.basename(saving_path)
                 if len(filename) > max_str_length:
                     saving_path = hash_path(saving_path)
                     warnings.warn("Filename too long. Hashing it ...", RuntimeWarning)
@@ -149,15 +159,16 @@
     if func is None:
         return _savedata
     else:
         return _savedata(func)
 
 
 def savefig(keys_or_function=None, include_classes="file",
-            ext=config.EXT_DEFAULT_FIG, keys=config.KEYS_DEFAULT_FIG, funcname_in_filename=config.FUNCNAME_IN_FILENAME_DEFAULT_FIG, return_fig=config.RETURN_FIG_DEFAULT,
+            ext=config.EXT_DEFAULT_FIG, keys=config.KEYS_DEFAULT_FIG, extra_keys={},
+            funcname_in_filename=config.FUNCNAME_IN_FILENAME_DEFAULT_FIG, return_fig=config.RETURN_FIG_DEFAULT,
             max_str_length=255,
             iterable_maxsize=3,
             overwrite=True, save=True,  #defaults for extra arguments
             **save_opts):
     """
     Generates figsaver decorator.
     Figure returned by function is automatically saved. Compatible with matplotlib and plotly.
@@ -166,58 +177,53 @@
     If filename is too long, it is shortened by hashing it.
 
     NOTE (!) decorated funcs will have extra arguments:
         - return_fig (bool)            whether to return the figure (output of function).
         - save (bool).                 whether to save the figure.
         - overwrite (bool).            whether to overwrite the saved version.
         - funcname_in_filename(bool)   whether to include funcname in the filename.
-        - keys (dict/str/iterable)   · dict:     specifies filename of the form k1-v1_k2-v2_...kn_vn.
-                                                 k_i do not have to be arguments of the function.
-                                     · str:       key of a keyword argument. Example: keys = 'x'.
+        - keys (dict/str/iterable)   · str:       key of a keyword argument. Example: keys = 'x'.
                                                  "kwargs_defaults"  =>  default kwargs that were not modified.
                                                  "kwargs"           =>  kwargs passed during function call.
                                                  "kwargs_full"      =>  kws_defaults + kws.
                                                  "pos_only"         =>  length of *args. Also self and cls are counted as pos_only arguments.
                                                  "args"             =>  attrs != **kwargs, *args.
                                                  "all"              if config.KEYS_ADD_POSONLY_TO_ALL  =>  all attrs
                                                                     else                               =>  all attrs except pos_only: kwargs_full + args
                                                  can combine options using "+" or "-". Example: "args+z", "x+y+kwargs", "all-y".
                                      · iterable: containing a combination of the available string keys (above). ["k1", "k2"] == "k1+k2".
+        - extra_keys (dict):         additional keys to be included in the filename. They do not have to be arguments of the function.
         - ext (str/list/tuple):    Storing extension. 'pdf' recommended for articles.
                                    Supported: any extension supported by matplotlib/plotly. Example: 'png', 'eps', 'html' (plotly), etc.
 
 
     Attrs:
         - function:                function to which the decorator is applied
         - include_classes:         include class tree in saving_path.
         - save_opts:               kws for saving function.
         - max_str_length:          max length of filename. If exceeded, filename is shortened by hashing it.
         - iterable_maxsize:        max size of iterable keys. If exceeded, keys are shortened by counting val numbers.
         - rest:                    default behavior for decorated funcs extra arguments (above).
 
     Returns: Function decorator
     """
-    if isinstance(keys_or_function, Iterable):
-        keys = keys_or_function
-        func = None
-    elif callable(keys_or_function):
-        func = keys_or_function
-    else:
-        func = None
+    func, keys, extra_keys = _preprocess_keys_or_function(keys_or_function, keys, extra_keys)
 
     mpl_save_defaults = dict(bbox_inches="tight")
 
     def _savefig(func):
         @wraps(func)
         def wrapper(*args, overwrite=overwrite, keys=keys, save=save, return_fig=return_fig, funcname_in_filename=funcname_in_filename, ext=ext, **kwargs):
             fig = func(*args, **kwargs)
             is_mpl_axes = type(fig).__name__ == 'AxesSubplot'
             if isinstance(fig, (mpl_figure, plotly_figure)) or is_mpl_axes:
                 key_opts = classify_call_attrs(func, args, kwargs, add_pos_only_to_all=config.KEYS_ADD_POSONLY_TO_ALL)
                 save_keys = merge_nested_dict(key_opts, keys, key_default="all")
+                if extra_keys:
+                    save_keys.update(extra_keys)
                 def get_saving_path(ext):
                     saving_path = figpath(keys=save_keys, func=func, ext=ext, include_classes=include_classes, funcname_in_filename=funcname_in_filename, iterable_maxsize=iterable_maxsize)
                     filename = os.path.basename(saving_path)
                     if len(filename) > max_str_length:
                         saving_path = hash_path(saving_path)
                         warnings.warn("Filename too long. Hashing it ...", RuntimeWarning)
                     return saving_path
```

### Comparing `tidypath-1.3.6/tidypath/fmt.py` & `tidypath-1.3.7/tidypath/fmt.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.6/tidypath/inspection.py` & `tidypath-1.3.7/tidypath/inspection.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.6/tidypath/paths.py` & `tidypath-1.3.7/tidypath/paths.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.6/tidypath/storage.py` & `tidypath-1.3.7/tidypath/storage.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.6/tidypath.egg-info/PKG-INFO` & `tidypath-1.3.7/tidypath.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.3.6
+Version: 1.3.7
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```


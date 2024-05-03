# Comparing `tmp/nbtof-0.0.4.tar.gz` & `tmp/nbtof-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbtof-0.0.4.tar", last modified: Tue Jan  2 02:57:38 2024, max compression
+gzip compressed data, was "nbtof-0.0.6.tar", last modified: Fri May  3 07:18:23 2024, max compression
```

## Comparing `nbtof-0.0.4.tar` & `nbtof-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-01-02 02:57:38.619354 nbtof-0.0.4/
--rw-rw-rw-   0        0        0     1084 2023-11-20 14:37:06.000000 nbtof-0.0.4/LICENSE
--rw-rw-rw-   0        0        0        0 2023-12-12 14:56:20.000000 nbtof-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2779 2024-01-02 02:57:38.618355 nbtof-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2105 2023-12-21 14:48:35.000000 nbtof-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-01-02 02:57:38.609353 nbtof-0.0.4/nbtof/
--rw-rw-rw-   0        0        0       54 2024-01-02 02:55:07.000000 nbtof-0.0.4/nbtof/__init__.py
--rw-rw-rw-   0        0        0    11608 2024-01-02 02:41:45.000000 nbtof-0.0.4/nbtof/nbtof_base.py
--rw-rw-rw-   0        0        0     7485 2023-12-16 13:49:32.000000 nbtof-0.0.4/nbtof/nbtof_concat.py
--rw-rw-rw-   0        0        0     1852 2024-01-02 02:52:39.000000 nbtof-0.0.4/nbtof/nbtof_generate.py
-drwxrwxrwx   0        0        0        0 2024-01-02 02:57:38.616354 nbtof-0.0.4/nbtof.egg-info/
--rw-rw-rw-   0        0        0     2779 2024-01-02 02:57:38.000000 nbtof-0.0.4/nbtof.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-01-02 02:57:38.000000 nbtof-0.0.4/nbtof.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-02 02:57:38.000000 nbtof-0.0.4/nbtof.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-01-02 02:57:38.000000 nbtof-0.0.4/nbtof.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-01-02 02:57:38.000000 nbtof-0.0.4/nbtof.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-02 02:57:38.620356 nbtof-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1358 2023-12-16 13:57:28.000000 nbtof-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 07:18:23.133345 nbtof-0.0.6/
+-rw-rw-rw-   0        0        0     1084 2023-11-20 14:37:06.000000 nbtof-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-12-12 14:56:20.000000 nbtof-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3107 2024-05-03 07:18:23.132386 nbtof-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2433 2024-01-02 04:04:03.000000 nbtof-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 07:18:23.122348 nbtof-0.0.6/nbtof/
+-rw-rw-rw-   0        0        0       54 2024-05-03 07:16:39.000000 nbtof-0.0.6/nbtof/__init__.py
+-rw-rw-rw-   0        0        0    11564 2024-05-03 06:03:50.000000 nbtof-0.0.6/nbtof/nbtof_base.py
+-rw-rw-rw-   0        0        0     9289 2024-05-02 07:02:04.000000 nbtof-0.0.6/nbtof/nbtof_concat.py
+-rw-rw-rw-   0        0        0     2777 2024-05-03 06:05:36.000000 nbtof-0.0.6/nbtof/nbtof_generate.py
+drwxrwxrwx   0        0        0        0 2024-05-03 07:18:23.130416 nbtof-0.0.6/nbtof.egg-info/
+-rw-rw-rw-   0        0        0     3107 2024-05-03 07:18:23.000000 nbtof-0.0.6/nbtof.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-03 07:18:23.000000 nbtof-0.0.6/nbtof.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 07:18:23.000000 nbtof-0.0.6/nbtof.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-03 07:18:23.000000 nbtof-0.0.6/nbtof.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 07:18:23.133345 nbtof-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1337 2024-05-03 07:17:44.000000 nbtof-0.0.6/setup.py
```

### Comparing `nbtof-0.0.4/LICENSE` & `nbtof-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nbtof-0.0.4/nbtof/nbtof_base.py` & `nbtof-0.0.6/nbtof/nbtof_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 import tempfile
 import os
 import subprocess
 import sys
 import copy
+import warnings
 
 def nbtof_base(
-    nb_path,
+    notebook_name,
     func_name=None,
     func_file_name=None,
     ):
     """
     This function converts noetbook into a function that performs the same processing as the notebook according to nbtof tags.
     
     Parameters
     ----------
-    nb_path : str
+    notebook_name : str
         notebook file path
     func_name : str
         function's name. If nothing is assigned, func_name gets notebook file name.
-    funcfile_name : str
+    func_file_name : str
         the .py file name that has the converted function.
     
     Returns
     -------
     tuple
         str
             output function file path.
         str
             output function file name.
     """
     
     if func_name is None:
-        func_name = os.path.split(os.path.splitext(nb_path)[0])[1]
+        func_name = os.path.split(os.path.splitext(notebook_name)[0])[1]
         func_name = func_name.replace("-","_")
         
     if func_file_name is None:
-        func_file_path = os.path.splitext(nb_path)[0] + '.py'
+        func_file_path = os.path.splitext(notebook_name)[0] + '.py'
     elif '.py' in func_file_name:
         func_file_path = func_file_name
-    else:
+    elif ".py" not in func_file_name:
         func_file_path = func_file_name + '.py'
     
     code_dict = {
         '#@header': -3,
         '# In[': -2,
         '#@ignore': -1,
         '#@advance': 0,
@@ -55,17 +56,17 @@
         '#@plane': 7,
         '#@return': 8,
         '#@r_advance': 9,
     }
     
     table_hist_list = []
     with tempfile.TemporaryDirectory() as td:
-        jupyter_path = sys.base_prefix + '\\Scripts\\jupyter.exe'
-        instant_py_file_path = td + '\\' + os.path.splitext(os.path.split(nb_path)[1])[0] + '.py'
-        nbconvert_cmd = jupyter_path + ' nbconvert ' + nb_path + ' --to python --output ' + instant_py_file_path
+        jupyter_path = "\"" + sys.base_prefix + '\\Scripts\\jupyter.exe' + "\""
+        instant_py_file_path = td + '\\' + os.path.splitext(os.path.split(notebook_name)[1])[0] + '.py'
+        nbconvert_cmd = jupyter_path + ' nbconvert ' + "\"" + notebook_name + "\"" + ' --to python --output '  + "\"" + instant_py_file_path + "\""
         
         returncode = subprocess.Popen(nbconvert_cmd, shell=True)
         _ = returncode.wait()
     
         with open(instant_py_file_path) as f:
             instant_table = []
             code_num = code_dict['#@header']
@@ -127,33 +128,18 @@
     # remove ignore
     instant_table = []
     for instant_list in table_hist_list[-1]:
         if (instant_list[0] != code_dict['#@ignore']):
             instant_table.append(instant_list)
     table_hist_list.append(instant_table)
     
-    ## decreace indention
-    #instant_table = []
-    #for instant_list in table_hist_list[-1]:
-    #    if ('#@' == instant_list[1][:len('#@')])*(len(instant_table)!=0):
-    #        if instant_table[-1][1] == '\n':
-    #            instant_table = instant_table[:-1]    
-    #    instant_table.append(instant_list)
-    #table_hist_list.append(instant_table)
-    #
-    ##@ignore
-    #table_hist_list[-1]
-    
     # arrange for advance and parameter
     instant_table = []
     for instant_list in table_hist_list[-1]:
-        if (instant_list[0]==code_dict['#@advance']):
-            instant_table.append(instant_list)
-    for instant_list in table_hist_list[-1]:
-        if (instant_list[0]==code_dict['#@r_advance']):
+        if (instant_list[0]==code_dict['#@advance'])+(instant_list[0]==code_dict['#@r_advance']):
             instant_table.append(instant_list)
     for instant_list in table_hist_list[-1]:
         if (instant_list[0]==code_dict['#@param']):
             instant_table.append(instant_list)
     for instant_list in table_hist_list[-1]:
         if (instant_list[0]==code_dict['#@args']):
             instant_table.append(instant_list)
@@ -243,19 +229,26 @@
     table_hist_list.append(instant_table)
     
     # setting parameter
     instant_table = []
     old_instant_table = copy.deepcopy(table_hist_list[-1])
     check_num = 0
     for instant_list in old_instant_table:
-        if (instant_list[0]==code_dict['#@param'])*(check_num==0):
+        if (
+            (instant_list[0]==code_dict['#@param']) + 
+            (instant_list[0]==code_dict['#@args']) + 
+            (instant_list[0]==code_dict['#@default']) + 
+            (instant_list[0]==code_dict['#@kwargs']) + 
+            (instant_list[0]==code_dict['#@help']) +
+            (instant_list[0]==code_dict['#@plane']) +
+            (instant_list[0]==code_dict['#@return'])
+            )*(check_num==0):
             instant_table.append([0, '\n',-1])
             instant_table.append([0, 'def ' + func_name +'(\n',-1])
-            check_num=1
-        
+            check_num=1    
         if (instant_list[0]!=code_dict['#@param'])*\
             (instant_list[0]!=code_dict['#@args'])*\
             (instant_list[0]!=code_dict['#@default'])*\
             (instant_list[0]!=code_dict['#@kwargs'])*\
             (check_num==1):
     
             instant_table.append([0, '    ):\n',-1])
```

### Comparing `nbtof-0.0.4/nbtof/nbtof_concat.py` & `nbtof-0.0.6/nbtof/nbtof_concat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,138 +1,166 @@
 import ast, copy
 import numpy as np
 import pandas as pd
 import os
+import warnings
+
+
 def body_dig(node, i = -1):
     return_name_table = []
     for j, node_u in enumerate(node.body):
         if type(node_u) == ast.Import:
             for name in node_u.names:
                 if name.asname is not None:
-                    return_name_table.append([name.asname, j * (i<0) + i * (i>=0), type(node_u), None, name.name, name.asname])
+                    return_name_table.append([name.asname, j * (i<0) + i * (i>=0), type(node_u), None, name.name, name.asname, None])
                 else:
-                    return_name_table.append([name.name, j * (i<0) + i * (i>=0), type(node_u), None, name.name, name.asname])
+                    return_name_table.append([name.name, j * (i<0) + i * (i>=0), type(node_u), None, name.name, name.asname, None])
         elif type(node_u) == ast.ImportFrom:
+            level = node_u.level
             for name in node_u.names:
                 if name.asname is not None:
-                    return_name_table.append([name.asname, j * (i<0) + i * (i>=0), type(node_u), node_u.module, name.name, name.asname])
+                    return_name_table.append([name.asname, j * (i<0) + i * (i>=0), type(node_u), node_u.module, name.name, name.asname, level])
                 else:
-                    return_name_table.append([name.name, j * (i<0) + i * (i>=0), type(node_u), node_u.module, name.name, name.asname])
+                    return_name_table.append([name.name, j * (i<0) + i * (i>=0), type(node_u), node_u.module, name.name, name.asname, level])
         elif type(node_u) == ast.Assign:
             if type(node_u.targets[0]) == ast.Tuple:
                 for elt in node_u.targets[0].elts:
                     #return_name_table.append(elt.id)
-                    return_name_table.append([elt.id, j * (i<0) + i * (i>=0), type(node_u), None, None, None])
+                    return_name_table.append([elt.id, j * (i<0) + i * (i>=0), type(node_u), None, None, None, None])
             elif type(node_u.targets[0]) == ast.Name:
-                return_name_table.append([node_u.targets[0].id, j * (i<0) + i * (i>=0), type(node_u), None, None, None])
+                return_name_table.append([node_u.targets[0].id, j * (i<0) + i * (i>=0), type(node_u), None, None, None, None])
         elif type(node_u) == ast.For:
             if type(node_u.target) == ast.Tuple:
                 for elt in node_u.target.elts:
                     #return_name_table.append(elt.id)
-                    return_name_table.append([elt.id, j * (i<0) + i * (i>=0), type(node_u), None, None, None])
+                    return_name_table.append([elt.id, j * (i<0) + i * (i>=0), type(node_u), None, None, None, None])
             elif type(node_u.target) == ast.Name:
                 #return_name_table.append(node_u.target.id)
-                return_name_table.append([node_u.target.id, j * (i<0) + i * (i>=0), type(node_u), None, None, None])
+                return_name_table.append([node_u.target.id, j * (i<0) + i * (i>=0), type(node_u), None, None, None, None])
 
             return_name_table = return_name_table + body_dig(node_u, j * (i<0) + i * (i>=0))
         
         elif type(node_u) == ast.FunctionDef:
-            return_name_table.append([node_u.name, j * (i<0) + i * (i>=0), type(node_u), None, None, None])
+            return_name_table.append([node_u.name, j * (i<0) + i * (i>=0), type(node_u), None, None, None, None])
         elif type(node_u) == ast.While:
             return_name_table = return_name_table + body_dig(node_u, j * (i<0) + i * (i>=0))
+        elif type(node_u) == ast.Try:
+            return_name_table = return_name_table + body_dig(node_u, j * (i<0) + i * (i>=0))
+            for handler in node_u.handlers:
+                return_name_table = return_name_table + body_dig(handler, j * (i<0) + i * (i>=0))               
         elif type(node_u) == ast.If:
             return_name_table = return_name_table + body_dig(node_u, j * (i<0) + i * (i>=0))
     return return_name_table
 def name_info_df(func_p):
     func_name_table = body_dig(func_p)
     if func_name_table == []:
         return_name_df = pd.DataFrame(
-            columns=['name', 'idx', 'type', 'module', 'import', 'as']
+            columns=['name', 'idx', 'type', 'module', 'import', 'as', "level"]
         )
     else:
         return_name_df = pd.DataFrame(
             data=np.array(func_name_table),
-            columns=['name', 'idx', 'type', 'module', 'import', 'as']
+            columns=['name', 'idx', 'type', 'module', 'import', 'as', "level"]
         )
     return return_name_df
 def import_str(name_ds):
     if name_ds['module'] is not None:
         return name_ds['module'] + '.' + name_ds['import']
     else:
         return name_ds['import']
 def new_import_check(add_name_ds, base_name_df):
     #add_import_info_alist = add_name_df.iloc[4][['module', 'import', 'as']].values
     #base_import_info_array = base_name_df[['module', 'import', 'as']].values
     concat_status = 'new'
     for _, base_name_ds in base_name_df.iterrows():
-        if (add_name_ds['name'] == base_name_ds['name'])*(import_str(add_name_ds) == import_str(base_name_ds)):
-            concat_status = 'exist'
-        elif (add_name_ds['name'] == base_name_ds['name'])*(import_str(add_name_ds) != import_str(base_name_ds)):
+        if (add_name_ds['name'] == base_name_ds['name'])*(import_str(add_name_ds) == import_str(base_name_ds))*(add_name_ds["level"] == base_name_ds["level"]):
+            concat_status = 'same_import'
+        elif (add_name_ds['name'] == base_name_ds['name'])*((import_str(add_name_ds) != import_str(base_name_ds))+(add_name_ds["level"] == base_name_ds["level"])):
             concat_status = 'error'
     return concat_status
 
-def nbtof_update_base(
-    base_py_file_name,
-    add_py_file_name,
-    auto_sort=True,
+def nbtof_concat(
+    base_py_path:str,
+    add_py_path:str,
+    concatenated_py_path:str=None,
+    auto_sort:bool=True,
+    func_update:bool=False,
     ):
     
-    if base_py_file_name[-3:] != '.py':
-        base_py_file_name = base_py_file_name +'.py'
+    if base_py_path[-3:] != '.py':
+        base_py_path = base_py_path +'.py'
+    if add_py_path[-3:] != '.py':
+        add_py_path = add_py_path +'.py'
+    
+    if concatenated_py_path is None:
+        concatenated_py_path = base_py_path
+    elif concatenated_py_path is not None:
+        if concatenated_py_path[-3:] != '.py':
+            concatenated_py_path = concatenated_py_path +'.py'
+    
+    #if not os.path.isfile(base_py_path):
+    #    with open(base_py_path, 'w') as f:
+    #        pass
     
-    if not os.path.isfile(base_py_file_name):
-        with open(base_py_file_name, 'w') as f:
-            pass
-    
-    with open(base_py_file_name) as f:
+    with open(base_py_path) as f:
         base_p = copy.deepcopy(ast.parse(f.read()))
-    with open(add_py_file_name) as f:
+    with open(add_py_path) as f:
         add_p = copy.deepcopy(ast.parse(f.read()))
     
-    add_name_df = name_info_df(add_p)
     base_name_df = name_info_df(base_p)
+    add_name_df = name_info_df(add_p)
     
     return_p = copy.deepcopy(base_p)
     return_body_list = []
     for idx, node in enumerate(add_p.body):
         instant_name_df = add_name_df[add_name_df['idx'] == idx]
-        if (type(node) == ast.Import) + (type(node) == ast.ImportFrom):
+        if (type(node) == ast.Import):
             for _, instant_name_ds in instant_name_df.iterrows():
                 concat_status = new_import_check(instant_name_ds, base_name_df)
-                #print(instant_name_ds['name'], concat_status)
-                if (concat_status == 'new')&(instant_name_ds['type'] == ast.Import):
+                if (concat_status == 'new'):
                     instant_module = ast.Import(
                         names=[
                             ast.alias(
                                 name = instant_name_ds['import'], 
                                 asname=instant_name_ds['as']
                                 )
                             ]
                         )
                     return_body_list.append(copy.deepcopy(instant_module))
-                elif (concat_status == 'new')&(instant_name_ds['type'] == ast.ImportFrom):
+        elif (type(node) == ast.ImportFrom):
+            for _, instant_name_ds in instant_name_df.iterrows():
+                concat_status = new_import_check(instant_name_ds, base_name_df)
+                if (concat_status == 'new'):
                     instant_module = ast.ImportFrom(
                         module=instant_name_ds['module'],
                         names=[
                             ast.alias(
                                 name = instant_name_ds['import'], 
-                                asname=instant_name_ds['as']
+                                asname=instant_name_ds['as'],
                                 )
                             ],
-                        level=0
+                        level=instant_name_ds['level']
                         )
                     return_body_list.append(copy.deepcopy(instant_module))
         elif (type(node) == ast.FunctionDef):
             add_func_name = add_name_df[(add_name_df['idx'] == idx)&(add_name_df['type'] == ast.FunctionDef)]['name'].values[0]
             return_body_list.append(copy.deepcopy(node))
             for _, instant_name_ds in base_name_df.iterrows():
-                if (instant_name_ds['name'] == add_func_name)&(instant_name_ds['type'] == ast.FunctionDef):
-                    return_p.body[instant_name_ds['idx']] = copy.deepcopy(node)
-                    return_body_list = return_body_list[:-1]        
+                if (instant_name_ds['name'] == add_func_name)*(instant_name_ds['type'] == ast.FunctionDef):
+                    if func_update == False:
+                        warnings.warn(f"There is the same function name \"{add_func_name}\" in several files. If you want to replace function, plase set \"func_update\" True.")
+                        return_body_list = return_body_list[:-1]
+                    elif func_update == True:
+                        return_p.body[instant_name_ds['idx']] = copy.deepcopy(node)
+                        return_body_list = return_body_list[:-1]        
                     break
+                elif (instant_name_ds['name'] == add_func_name)*(instant_name_ds['type'] == ast.Assign):
+                    warnings.warn(f"function name \"{add_func_name}\" in \"{add_py_path}\" is already used as variable name in other file.")
+                elif (instant_name_ds['name'] == add_func_name)*((instant_name_ds['type'] == ast.Import) + (instant_name_ds['type'] == ast.ImportFrom)):
+                    warnings.warn(f"function name \"{add_func_name}\" in \"{add_py_path}\" is already used as imported module name in other file.")
         else:
             return_body_list.append(copy.deepcopy(node))
             
     return_p.body = return_p.body + return_body_list
     
     if auto_sort:
         auto_sort_table = [
@@ -145,11 +173,11 @@
         sort_body_list = []
         for auto_sort_list in auto_sort_table:
             for node in return_p.body:
                 if type(node) in auto_sort_list:
                     sort_body_list.append(copy.deepcopy(node))
         return_p.body = sort_body_list
     
-    with open(base_py_file_name, mode='w') as f:
+    with open(base_py_path, mode='w') as f:
         f.write(ast.unparse(return_p))
 
     return True
```

### Comparing `nbtof-0.0.4/setup.py` & `nbtof-0.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from setuptools import setup
-import nbtof
 
 DESCRIPTION = "nbtof: transfering notebook to function"
 NAME = 'nbtof'
 AUTHOR = 'Haruka Nodaka'
 AUTHOR_EMAIL = 'haruka.nodaka@gmail.com'
 URL = 'https://github.com/Nodaka/nbtof'
 LICENSE = 'MIT'
 DOWNLOAD_URL = 'https://github.com/Nodaka/nbtof'
-VERSION = nbtof.__version__
+VERSION = "0.0.6"
 PYTHON_REQUIRES = ">=3.9"
 
 INSTALL_REQUIRES = [
-    'pandas',
-    'nbconvert',
-    'jupyter',
+#    'pandas',
+#    'nbconvert',
+#    'jupyter',
 ]
 
 PACKAGES = [
     'nbtof',
 ]
 
 CLASSIFIERS = [
```


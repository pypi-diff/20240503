# Comparing `tmp/corebridge-0.1.3.tar.gz` & `tmp/corebridge-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corebridge-0.1.3.tar", last modified: Wed Apr 24 16:39:15 2024, max compression
+gzip compressed data, was "corebridge-0.1.4.tar", last modified: Fri May  3 10:28:21 2024, max compression
```

## Comparing `corebridge-0.1.3.tar` & `corebridge-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-24 16:39:15.098434 corebridge-0.1.3/
--rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.1.3/LICENSE
--rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.1.3/MANIFEST.in
--rw-r--r--   0 fenke     (1000) users      (100)     1203 2024-04-24 16:39:15.098434 corebridge-0.1.3/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)      435 2024-04-17 14:51:56.000000 corebridge-0.1.3/README.md
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-24 16:39:15.098434 corebridge-0.1.3/corebridge/
--rw-r--r--   0 fenke     (1000) users      (100)       22 2024-04-24 16:39:11.000000 corebridge-0.1.3/corebridge/__init__.py
--rw-r--r--   0 fenke     (1000) users      (100)     3300 2024-04-24 16:39:11.000000 corebridge-0.1.3/corebridge/_modidx.py
--rw-r--r--   0 fenke     (1000) users      (100)     8484 2024-04-24 16:39:11.000000 corebridge-0.1.3/corebridge/aicorebridge.py
--rw-r--r--   0 fenke     (1000) users      (100)     3766 2024-04-24 16:39:11.000000 corebridge-0.1.3/corebridge/core.py
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-24 16:39:15.098434 corebridge-0.1.3/corebridge.egg-info/
--rw-r--r--   0 fenke     (1000) users      (100)     1203 2024-04-24 16:39:15.000000 corebridge-0.1.3/corebridge.egg-info/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)      381 2024-04-24 16:39:15.000000 corebridge-0.1.3/corebridge.egg-info/SOURCES.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-04-24 16:39:15.000000 corebridge-0.1.3/corebridge.egg-info/dependency_links.txt
--rw-r--r--   0 fenke     (1000) users      (100)       42 2024-04-24 16:39:15.000000 corebridge-0.1.3/corebridge.egg-info/entry_points.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.1.3/corebridge.egg-info/not-zip-safe
--rw-r--r--   0 fenke     (1000) users      (100)      225 2024-04-24 16:39:15.000000 corebridge-0.1.3/corebridge.egg-info/requires.txt
--rw-r--r--   0 fenke     (1000) users      (100)       11 2024-04-24 16:39:15.000000 corebridge-0.1.3/corebridge.egg-info/top_level.txt
--rw-r--r--   0 fenke     (1000) users      (100)     1146 2024-04-24 15:28:30.000000 corebridge-0.1.3/settings.ini
--rw-r--r--   0 fenke     (1000) users      (100)       38 2024-04-24 16:39:15.098434 corebridge-0.1.3/setup.cfg
--rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.1.3/setup.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-03 10:28:21.469702 corebridge-0.1.4/
+-rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.1.4/LICENSE
+-rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.1.4/MANIFEST.in
+-rw-r--r--   0 fenke     (1000) users      (100)     2655 2024-05-03 10:28:21.469702 corebridge-0.1.4/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)     1887 2024-05-03 10:28:01.000000 corebridge-0.1.4/README.md
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-03 10:28:21.469702 corebridge-0.1.4/corebridge/
+-rw-r--r--   0 fenke     (1000) users      (100)       22 2024-05-03 10:28:12.000000 corebridge-0.1.4/corebridge/__init__.py
+-rw-r--r--   0 fenke     (1000) users      (100)     3300 2024-05-03 10:28:12.000000 corebridge-0.1.4/corebridge/_modidx.py
+-rw-r--r--   0 fenke     (1000) users      (100)     8545 2024-05-03 10:28:12.000000 corebridge-0.1.4/corebridge/aicorebridge.py
+-rw-r--r--   0 fenke     (1000) users      (100)     3766 2024-05-03 10:28:12.000000 corebridge-0.1.4/corebridge/core.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-03 10:28:21.469702 corebridge-0.1.4/corebridge.egg-info/
+-rw-r--r--   0 fenke     (1000) users      (100)     2655 2024-05-03 10:28:21.000000 corebridge-0.1.4/corebridge.egg-info/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)      381 2024-05-03 10:28:21.000000 corebridge-0.1.4/corebridge.egg-info/SOURCES.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-05-03 10:28:21.000000 corebridge-0.1.4/corebridge.egg-info/dependency_links.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       42 2024-05-03 10:28:21.000000 corebridge-0.1.4/corebridge.egg-info/entry_points.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.1.4/corebridge.egg-info/not-zip-safe
+-rw-r--r--   0 fenke     (1000) users      (100)      225 2024-05-03 10:28:21.000000 corebridge-0.1.4/corebridge.egg-info/requires.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       11 2024-05-03 10:28:21.000000 corebridge-0.1.4/corebridge.egg-info/top_level.txt
+-rw-r--r--   0 fenke     (1000) users      (100)     1146 2024-04-29 12:11:53.000000 corebridge-0.1.4/settings.ini
+-rw-r--r--   0 fenke     (1000) users      (100)       38 2024-05-03 10:28:21.469702 corebridge-0.1.4/setup.cfg
+-rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.1.4/setup.py
```

### Comparing `corebridge-0.1.3/LICENSE` & `corebridge-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `corebridge-0.1.3/corebridge/_modidx.py` & `corebridge-0.1.4/corebridge/_modidx.py`

 * *Files identical despite different names*

### Comparing `corebridge-0.1.3/corebridge/aicorebridge.py` & `corebridge-0.1.4/corebridge/aicorebridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,52 +20,55 @@
 
 # %% ../nbs/01_aicorebridge.ipynb 5
 print(f"loading {__name__}")
 
 # %% ../nbs/01_aicorebridge.ipynb 6
 class AICoreModule(): pass
 
-# %% ../nbs/01_aicorebridge.ipynb 7
+# %% ../nbs/01_aicorebridge.ipynb 8
 @patch
 def __init__(self:AICoreModule, 
              processor:typing.Callable, # data processing function
              save_dir:str, # path where the module can keep files 
              assets_dir:str,
              *args, **kwargs):
     
-    self.save_dir  = save_dir
-    self.assets_dir  = assets_dir
+    self.directory_args = dict(
+        save_dir=save_dir,
+        assets_dir=assets_dir
+    )
+    
     self._init_processor(processor)
 
     self.init_args = args
     self.init_kwargs = {k:v for k,v in kwargs.items() if v is not None}
 
 
 
-# %% ../nbs/01_aicorebridge.ipynb 8
+# %% ../nbs/01_aicorebridge.ipynb 10
 @patch
 def _init_processor(
         self:AICoreModule, 
         processor:typing.Callable):
     """Initializes processor related variables on self"""
     
     self.processor = processor
     self.processor_signature = inspect.signature(self.processor)
     self.processor_params = dict(self.processor_signature.parameters)
     self.return_param = self.processor_params.pop('return', None)
     self.data_param, *self.call_params = list(self.processor_params.keys())
 
 
-# %% ../nbs/01_aicorebridge.ipynb 9
+# %% ../nbs/01_aicorebridge.ipynb 11
 @patch
 def call_processor(self:AICoreModule, calldata, **callargs):
     return self.processor(calldata, **callargs)
 
 
-# %% ../nbs/01_aicorebridge.ipynb 10
+# %% ../nbs/01_aicorebridge.ipynb 12
 @patch
 def infer(self:AICoreModule, data:dict, *_, **kwargs):
     msg=[]
     try:
 
         msg=[
             f"{self.processor.__name__}({self.processor_signature})",
@@ -82,15 +85,15 @@
             data, 
             recordformat=recordformat,
             timezone=timezone,
             reversed=reversed)
         
         msg.append(f"calldata shape: {calldata.shape}")
 
-        callargs = self.get_callargs(**kwargs)
+        callargs = self.get_callargs(**kwargs, **self.directory_args)
 
         for arg, val in callargs.items():
             msg.append(f"{arg}: {val}")
             
         result = self.call_processor(calldata, **callargs)
         msg.append(f"result shape: {result.shape}")
 
@@ -108,15 +111,15 @@
         syslog.exception(f"Exception {str(err)} in infer()")
         return {
             'msg': msg,
             'data': []
         }
 
 
-# %% ../nbs/01_aicorebridge.ipynb 11
+# %% ../nbs/01_aicorebridge.ipynb 13
 @patch
 def get_callargs(self:AICoreModule, **kwargs):
     "Get arguments for the processor call"
 
     # Remove null / None values
     kwargs = {k:v for k,v in kwargs.items() if v is not None}
     
@@ -124,15 +127,15 @@
 
     return {
         K:self.processor_signature.parameters[K].annotation(kwargs.get(K,metadata.get(K, self.init_kwargs.get(K, self.processor_signature.parameters[K].default))))
         for K in self.call_params
     }
 
 
-# %% ../nbs/01_aicorebridge.ipynb 12
+# %% ../nbs/01_aicorebridge.ipynb 14
 @patch
 def get_call_data(
         self:AICoreModule, 
         data:dict, 
         recordformat='records', 
         timezone='UTC', 
         reversed=False):
@@ -174,15 +177,15 @@
         df.index = (df.index - datetime.datetime(1970,1,1, tzinfo=datetime.timezone.utc)) / datetime.timedelta(seconds=1)
         return df.to_records(index=True)
     else:
         df.index = (df.index - datetime.datetime(1970,1,1, tzinfo=datetime.timezone.utc)) / datetime.timedelta(seconds=1)
         return df.reset_index().to_numpy()
         
 
-# %% ../nbs/01_aicorebridge.ipynb 13
+# %% ../nbs/01_aicorebridge.ipynb 15
 @patch
 def rewrite_data(
         self:AICoreModule, 
         data:typing.Union[pd.DataFrame, pd.Series, dict], 
         recordformat:str='split', 
         timezone:str='UTC', 
         reversed:bool=False):
@@ -210,15 +213,15 @@
     if normalized_data.isna().any(axis=None):
         return [ {k:v for k,v in m.items() if pd.notnull(v)} for m in records]
     else:
         return records
 
     
 
-# %% ../nbs/01_aicorebridge.ipynb 14
+# %% ../nbs/01_aicorebridge.ipynb 16
 @patch
 def convert_to_dataframe(
         self:AICoreModule, 
         adata:typing.Union[pd.DataFrame, pd.Series, dict, np.ndarray, np.recarray], 
         timezone='UTC', 
         columnnames=None):
     """Convert various data formats to standardized timeseries DataFrame"""
```

### Comparing `corebridge-0.1.3/corebridge/core.py` & `corebridge-0.1.4/corebridge/core.py`

 * *Files identical despite different names*

### Comparing `corebridge-0.1.3/settings.ini` & `corebridge-0.1.4/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = corebridge
 lib_name = %(repo)s
-version = 0.1.3
+version = 0.1.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = corebridge
```

### Comparing `corebridge-0.1.3/setup.py` & `corebridge-0.1.4/setup.py`

 * *Files identical despite different names*


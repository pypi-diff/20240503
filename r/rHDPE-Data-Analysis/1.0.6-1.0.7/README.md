# Comparing `tmp/rHDPE_Data_Analysis-1.0.6.tar.gz` & `tmp/rHDPE_Data_Analysis-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rHDPE_Data_Analysis-1.0.6.tar", last modified: Thu May  2 14:08:56 2024, max compression
+gzip compressed data, was "rHDPE_Data_Analysis-1.0.7.tar", last modified: Fri May  3 14:24:13 2024, max compression
```

## Comparing `rHDPE_Data_Analysis-1.0.6.tar` & `rHDPE_Data_Analysis-1.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-02 14:08:56.874483 rHDPE_Data_Analysis-1.0.6/
--rw-r--r--   0 philsmith   (501) staff       (20)      353 2024-05-02 14:08:56.873762 rHDPE_Data_Analysis-1.0.6/PKG-INFO
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-02 14:08:56.811484 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-02 14:08:56.829150 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/FTIR_Analysis/
--rw-r--r--   0 philsmith   (501) staff       (20)     2750 2024-05-02 13:57:15.000000 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py
--rw-r--r--   0 philsmith   (501) staff       (20)    16419 2023-08-07 12:36:28.000000 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/FTIR_Analysis/Deprecated.py
--rw-r--r--   0 philsmith   (501) staff       (20)     8459 2024-05-02 13:58:33.000000 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py
--rw-r--r--   0 philsmith   (501) staff       (20)     2284 2024-05-02 13:57:15.000000 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py
--rw-r--r--   0 philsmith   (501) staff       (20)     9607 2024-04-29 13:43:44.000000 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py
--rw-r--r--   0 philsmith   (501) staff       (20)    43760 2024-05-01 16:22:46.000000 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py
--rw-r--r--   0 philsmith   (501) staff       (20)      148 2023-12-22 10:54:51.000000 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/FTIR_Analysis/__init__.py
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-02 14:08:56.872489 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/Global_Analysis/
--rw-r--r--   0 philsmith   (501) staff       (20)     2077 2024-04-25 11:31:49.000000 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/Global_Analysis/Analysis.py
--rw-r--r--   0 philsmith   (501) staff       (20)     1446 2024-01-09 12:15:24.000000 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/Global_Analysis/Input_Parameters_Class.py
--rw-r--r--   0 philsmith   (501) staff       (20)     3503 2024-04-25 11:31:49.000000 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/Global_Analysis/Preprocessing.py
--rw-r--r--   0 philsmith   (501) staff       (20)    37968 2024-04-25 11:31:49.000000 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/Global_Analysis/Utilities.py
--rw-r--r--   0 philsmith   (501) staff       (20)      120 2024-01-03 12:56:03.000000 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/Global_Analysis/__init__.py
--rw-r--r--   0 philsmith   (501) staff       (20)    35883 2024-04-19 16:24:08.000000 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/Global_Utilities.py
--rw-r--r--   0 philsmith   (501) staff       (20)        1 2024-04-25 11:22:18.000000 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/__init__.py
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-02 14:08:56.819732 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis.egg-info/
--rw-r--r--   0 philsmith   (501) staff       (20)      353 2024-05-02 14:08:56.000000 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis.egg-info/PKG-INFO
--rw-r--r--   0 philsmith   (501) staff       (20)      861 2024-05-02 14:08:56.000000 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis.egg-info/SOURCES.txt
--rw-r--r--   0 philsmith   (501) staff       (20)        1 2024-05-02 14:08:56.000000 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis.egg-info/dependency_links.txt
--rw-r--r--   0 philsmith   (501) staff       (20)       20 2024-05-02 14:08:56.000000 rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis.egg-info/top_level.txt
--rw-r--r--   0 philsmith   (501) staff       (20)       38 2024-05-02 14:08:56.874640 rHDPE_Data_Analysis-1.0.6/setup.cfg
--rw-r--r--   0 philsmith   (501) staff       (20)      416 2024-05-02 14:08:33.000000 rHDPE_Data_Analysis-1.0.6/setup.py
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-03 14:24:13.213927 rHDPE_Data_Analysis-1.0.7/
+-rw-r--r--   0 philsmith   (501) staff       (20)      353 2024-05-03 14:24:13.213212 rHDPE_Data_Analysis-1.0.7/PKG-INFO
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-03 14:24:13.188158 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-03 14:24:13.206122 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/FTIR_Analysis/
+-rw-r--r--   0 philsmith   (501) staff       (20)     2750 2024-05-02 13:57:15.000000 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py
+-rw-r--r--   0 philsmith   (501) staff       (20)    16419 2023-08-07 12:36:28.000000 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/FTIR_Analysis/Deprecated.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     8459 2024-05-02 13:58:33.000000 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     2284 2024-05-02 13:57:15.000000 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     9607 2024-04-29 13:43:44.000000 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py
+-rw-r--r--   0 philsmith   (501) staff       (20)    43760 2024-05-01 16:22:46.000000 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py
+-rw-r--r--   0 philsmith   (501) staff       (20)      148 2023-12-22 10:54:51.000000 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/FTIR_Analysis/__init__.py
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-03 14:24:13.212075 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/Global_Analysis/
+-rw-r--r--   0 philsmith   (501) staff       (20)     2061 2024-05-03 12:04:44.000000 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/Global_Analysis/Analysis.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     1690 2024-05-03 09:44:18.000000 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/Global_Analysis/Input_Parameters_Class.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     4957 2024-05-03 11:51:35.000000 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/Global_Analysis/Preprocessing.py
+-rw-r--r--   0 philsmith   (501) staff       (20)    38479 2024-05-03 12:18:54.000000 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/Global_Analysis/Utilities.py
+-rw-r--r--   0 philsmith   (501) staff       (20)      120 2024-01-03 12:56:03.000000 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/Global_Analysis/__init__.py
+-rw-r--r--   0 philsmith   (501) staff       (20)    35883 2024-04-19 16:24:08.000000 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/Global_Utilities.py
+-rw-r--r--   0 philsmith   (501) staff       (20)        1 2024-04-25 11:22:18.000000 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/__init__.py
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-03 14:24:13.196840 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis.egg-info/
+-rw-r--r--   0 philsmith   (501) staff       (20)      353 2024-05-03 14:24:13.000000 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis.egg-info/PKG-INFO
+-rw-r--r--   0 philsmith   (501) staff       (20)      861 2024-05-03 14:24:13.000000 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 philsmith   (501) staff       (20)        1 2024-05-03 14:24:13.000000 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 philsmith   (501) staff       (20)       20 2024-05-03 14:24:13.000000 rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis.egg-info/top_level.txt
+-rw-r--r--   0 philsmith   (501) staff       (20)       38 2024-05-03 14:24:13.214099 rHDPE_Data_Analysis-1.0.7/setup.cfg
+-rw-r--r--   0 philsmith   (501) staff       (20)      416 2024-05-03 14:24:03.000000 rHDPE_Data_Analysis-1.0.7/setup.py
```

### Comparing `rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py` & `rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/FTIR_Analysis/Deprecated.py` & `rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/FTIR_Analysis/Deprecated.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py` & `rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py` & `rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py` & `rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py` & `rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/Global_Analysis/Analysis.py` & `rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/Global_Analysis/Analysis.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,66 @@
 # Imports.
 
-import sys
-from pathlib import Path
-
-sys.path.append( Path( __file__ ).absolute().parents[1].as_posix() )
-
 from . import Preprocessing
 from . import Utilities as util
 
-sys.path.append( Path( __file__ ).absolute().parents[3].as_posix() )
-
 from .. import Global_Utilities as gu
 
 # Main function definition.
 
-def Global_Analysis_Main( directory, ip ):
+def Global_Analysis_Main( ip ):
+
+    if type( ip.datasets_to_read ) == int:
+
+        ip.datasets_to_read = [ip.datasets_to_read]
 
     if ip.datasets_to_read == False:
 
         print( "Please select a dataset(s)" )
 
         return 0
 
-    output_directory = directory + "Global/Output/"
-
-    resin_data = gu.get_list_of_resins_data( directory ) # Obtain the spreadsheet of data for the resins.
+    resin_data = gu.get_list_of_resins_data( ip.directory ) # Obtain the spreadsheet of data for the resins.
 
     if ip.read_files:
 
-        features_df, std_of_features_df, rank_features_df = Preprocessing.read_files_and_preprocess( directory, ip.datasets_to_read, ip.sample_mask )
+        features_df, std_of_features_df, rank_features_df = Preprocessing.read_files_and_preprocess( ip.directory, ip.output_directory, ip.shiny, ip.datasets_to_read, ip.sample_mask.copy() )
 
     if ip.plot_global_features:
 
-        gu.plot_global_features( output_directory, features_df.to_numpy(), features_df.columns, [resin_data.loc[i]["Label"] for i in features_df.index] )
+        gu.plot_global_features( ip.output_directory + "Global/", features_df.to_numpy(), features_df.columns, [resin_data.loc[i]["Label"] for i in features_df.index] )
 
     if ip.scatterplot:
 
-        util.scatterplots( directory, features_df, std_of_features_df )
+        util.scatterplots( ip.directory, features_df, std_of_features_df )
 
     if ip.correlation_heatmaps:
 
         spearman_rank_df = util.correlation_heatmap( rank_features_df, spearman = True )
         pearson_df = util.correlation_heatmap( features_df )
 
-        gu.plot_df_heatmap( spearman_rank_df, savefig = True, filename = output_directory + "Correlations/Spearman.pdf" )
-        gu.plot_df_heatmap( pearson_df, savefig = True, filename = output_directory + "Correlations/Pearson.pdf" )
+        gu.plot_df_heatmap( spearman_rank_df, savefig = True, filename = ip.output_directory + "Global/Correlations/Spearman.pdf" )
+        gu.plot_df_heatmap( pearson_df, savefig = True, filename = ip.output_directory + "Global/Correlations/Pearson.pdf" )
 
     if ip.pca:
 
-        util.pca( directory, features_df, std_of_features_df )
+        util.pca( ip.directory, ip.output_directory, features_df, std_of_features_df )
 
     if ip.distance_to_virgin_analysis_based_on_pcas:
 
-        util.distance_to_virgin_analysis_based_on_pcas( directory, features_df )
+        util.distance_to_virgin_analysis_based_on_pcas( ip.output_directory, features_df )
 
     if ip.rank_resins_by_pp_content:
 
-        util.rank_resins_by_pp_content( directory, features_df, rank_features_df )
+        util.rank_resins_by_pp_content( ip.directory, features_df, rank_features_df )
 
     if ip.manual_ml:
 
-        util.manual_ml( directory, ip, features_df )
+        util.manual_ml( ip.directory, ip, features_df )
 
     if ip.pca_ml:
 
-        util.pca_ml( directory, ip, features_df )
+        util.pca_ml( ip.directory, ip, features_df )
 
     if ip.sandbox:
 
-        util.sandbox( directory, features_df, std_of_features_df )
+        util.sandbox( ip.directory, features_df, std_of_features_df )
```

### Comparing `rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/Global_Analysis/Input_Parameters_Class.py` & `rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/Global_Analysis/Input_Parameters_Class.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 
 # Class definitions.
 
 class Input_Parameters():
 
     def __init__( self ):
 
+        self.shiny = False
+
+        self.directory = ""
+
+        self.output_directory = ""
+
         self.datasets_to_read = []
 
         self.sample_mask = []
 
         self.read_files = False
 
         self.plot_global_features = False
@@ -38,30 +44,36 @@
 
     doc = Document( filename )
 
     sheets = doc.sheets
     tables = sheets[0].tables
     rows = tables[0].rows()
 
-    ip.datasets_to_read = [int( i.value ) for i in rows[0][1:] if i.value != None]
+    ip.shiny = bool( rows[0][1].value )
+
+    ip.directory = str( rows[1][1].value or "" )
+
+    ip.output_directory = str( rows[2][1].value or "" )
+
+    ip.datasets_to_read = [int( i.value ) for i in rows[3][1:] if i.value != None]
 
-    ip.sample_mask = [int( i.value ) for i in rows[1][1:] if i.value != None]
+    ip.sample_mask = [int( i.value ) for i in rows[4][1:] if i.value != None]
 
-    ip.read_files = bool( rows[2][1].value )
+    ip.read_files = bool( rows[5][1].value )
 
-    ip.plot_global_features = bool( rows[3][1].value )
+    ip.plot_global_features = bool( rows[6][1].value )
 
-    ip.scatterplot = bool( rows[4][1].value )
+    ip.scatterplot = bool( rows[7][1].value )
 
-    ip.correlation_heatmaps = bool( rows[5][1].value )
+    ip.correlation_heatmaps = bool( rows[8][1].value )
 
-    ip.pca = bool( rows[6][1].value )
+    ip.pca = bool( rows[9][1].value )
 
-    ip.distance_to_virgin_analysis_based_on_pcas = bool( rows[7][1].value )
+    ip.distance_to_virgin_analysis_based_on_pcas = bool( rows[10][1].value )
 
-    ip.rank_resins_by_pp_content = bool( rows[8][1].value )
+    ip.rank_resins_by_pp_content = bool( rows[11][1].value )
 
-    ip.manual_ml = bool( rows[9][1].value )
+    ip.manual_ml = bool( rows[12][1].value )
 
-    ip.pca_ml = bool( rows[10][1].value )
+    ip.pca_ml = bool( rows[13][1].value )
 
-    ip.sandbox = bool( rows[11][1].value )
+    ip.sandbox = bool( rows[14][1].value )
```

### Comparing `rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/Global_Analysis/Utilities.py` & `rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/Global_Analysis/Utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,14 @@
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import mean_squared_error
 from math import sqrt
 from sklearn.metrics import r2_score
 import math
 from sklearn import datasets, linear_model
 
-import sys
-from pathlib import Path
-
-sys.path.append( Path( __file__ ).absolute().parents[3].as_posix() )
-
 from .. import Global_Utilities as gu
 
 def compile_full_dataset_of_features( dataset ):
 
     samples_present = []
 
     for i in dataset:
@@ -310,34 +305,32 @@
 
         sum_ranks += ranks[i]
 
     temp = sum_ranks.argsort()
 
     print( "Mean:", [resin_data.loc[i]["Label"] for i in sample_mask_array[temp]] )
 
-def pca( directory, features_df, std_of_features_df ):
+def pca( directory, output_directory, features_df, std_of_features_df ):
 
     resin_data = gu.get_list_of_resins_data( directory ) # Obtain the spreadsheet of data for the resins.
 
-    output_directory = directory + "Global/Output/"
-
     pca_of_whole_dataset = False
     pca_of_pca_of_individual_datasets = True
 
     if pca_of_whole_dataset:
 
-        gu.perform_pca( directory, features_df, [int( i ) for i in features_df.index], std_error = True, std_of_features_df = std_of_features_df, num_components = 2, filename = output_directory + "PCA/Overall.pdf" )
+        gu.perform_pca( directory, features_df, [int( i ) for i in features_df.index], std_error = True, std_of_features_df = std_of_features_df, num_components = 2, filename = output_directory + "Global/PCA/Overall.pdf" )
 
     if pca_of_pca_of_individual_datasets:
 
         compute_distance_to_virgin = False
 
         perform_k_means = False
 
-        dataset_names = ["FTIR", "DSC", "TGA", "Rhe", "TT", "Colour"]
+        dataset_names = ["FTIR", "DSC", "TGA", "Rhe", "TT", "Colour", "SHM", "TLS", "ESCR"]
 
         sample_mask = features_df.index.to_list()
 
         features_split_by_dataset_df, std_split_by_dataset_df = [], []
 
         for i, n in enumerate( dataset_names ):
 
@@ -349,15 +342,15 @@
 
             std_split_by_dataset_df.append( df )
 
         pcas, stds = [], []
 
         for i in range( len( features_split_by_dataset_df ) ):
 
-            if not features_split_by_dataset_df[i].empty:
+            if not (features_split_by_dataset_df[i].empty or len( features_split_by_dataset_df[i].columns ) == 1):
 
                 num_components = 2
 
                 pca = PCA( n_components = num_components )
                 pca_ft = pca.fit_transform( features_split_by_dataset_df[i] )
 
                 gu.pca_analysis( pca, features_split_by_dataset_df[i] )
@@ -377,22 +370,27 @@
                         std[k].append( s )
 
                 std_array = np.array( std ).transpose()
 
                 pcas.append( gu.array_with_column_titles_and_label_titles_to_df( pca_ft, [dataset_names[i] + "_PC1", dataset_names[i] + "_PC2"], sample_mask ) )
                 stds.append( gu.array_with_column_titles_and_label_titles_to_df( std_array, [dataset_names[i] + "_PC1", dataset_names[i] + "_PC2"], sample_mask ) )
 
+            elif len( features_split_by_dataset_df[i].columns ) == 1:
+
+                pcas.append( features_split_by_dataset_df[i] )
+                stds.append( std_split_by_dataset_df[i] )
+
             else:
 
                 pcas.append( pd.DataFrame() )
                 stds.append( pd.DataFrame() )
 
         pcas_to_include, stds_to_include = [], []
 
-        for i in range( 6 ):
+        for i in range( len( dataset_names ) ):
 
             if not pcas[i].empty:
 
                 pcas_to_include.append( pcas[i] )
                 stds_to_include.append( stds[i] )
 
         overall_pca = np.zeros( len( sample_mask ) )[:, np.newaxis]
@@ -410,23 +408,31 @@
                 feature_names.append( pcas_to_include[i].columns[j] )
 
         overall_pca = overall_pca[:, 1:]
         overall_stds = overall_stds[:, 1:]
 
         num_components = len( overall_pca[0] )
 
-        for i in range( num_components ):
+        if len( pcas_to_include ) != 1:
 
-            overall_pca[:, i] =  (overall_pca[:, i] - overall_pca[:, i].min()) / (overall_pca[:, i].max() - overall_pca[:, i].min())
-            overall_stds[:, i] =  overall_stds[:, i] / (overall_pca[:, i].max() - overall_pca[:, i].min())
+            for i in range( num_components ):
+
+                overall_pca[:, i] =  (overall_pca[:, i] - overall_pca[:, i].min()) / (overall_pca[:, i].max() - overall_pca[:, i].min())
+                overall_stds[:, i] =  overall_stds[:, i] / (overall_pca[:, i].max() - overall_pca[:, i].min())
 
         overall_pca_df = gu.array_with_column_titles_and_label_titles_to_df( overall_pca, feature_names, sample_mask )
         overall_stds_df = gu.array_with_column_titles_and_label_titles_to_df( overall_stds, feature_names, sample_mask )
 
-        pca_ft_df = gu.perform_pca( directory, overall_pca_df, [int( i ) for i in overall_pca_df.index], std_error = True, std_of_features_df = overall_stds_df, num_components = 2, filename = output_directory + "PCA/Overall.pdf" )
+        if shiny:
+
+            pca_ft_df = gu.perform_pca( directory, overall_pca_df, [int( i ) for i in overall_pca_df.index], std_error = True, std_of_features_df = overall_stds_df, num_components = 2, filename = output_directory + "Global/PCA/Overall.png" )
+
+        else:
+
+            pca_ft_df = gu.perform_pca( directory, overall_pca_df, [int( i ) for i in overall_pca_df.index], std_error = True, std_of_features_df = overall_stds_df, num_components = 2, filename = output_directory + "Global/PCA/Overall.pdf" )
 
         pca_ft = pca_ft_df.to_numpy()
 
         if compute_distance_to_virgin:
 
             virgin_samples = [16, 17, 19]
 
@@ -441,21 +447,21 @@
             # Virgin V8: ['V8', 'V6', 'V7', 'PCR 15', 'PCR 1', 'PCR 12', 'PCR 3', 'PCR 5', 'PCR 6', 'PCR 2', 'PCR 7', 'PCR 9', 'PCR 14', 'PCR 11', 'PCR 13', 'PCR 8', 'PCR 10', 'PCR 4', 'PCR 21', 'PCR 20', 'PCR 18', 'PCR 22', 'PCR 23']
             # Mean: ['V8', 'V6', 'PCR 15', 'V7', 'PCR 1', 'PCR 12', 'PCR 5', 'PCR 6', 'PCR 3', 'PCR 2', 'PCR 7', 'PCR 9', 'PCR 14', 'PCR 11', 'PCR 13', 'PCR 8', 'PCR 10', 'PCR 4', 'PCR 21', 'PCR 20', 'PCR 18', 'PCR 22', 'PCR 23']
 
         if perform_k_means:
 
             kmeans = KMeans( n_clusters = 3, random_state = 0 ).fit( pca_ft[:, [0, 1]] )
 
-            gu.plot_kmeans_plus_pca( pca_ft, kmeans, sample_mask, [resin_data.loc[i]["Label"] for i in sample_mask], savefig = True, xlabel = "First Principal Component", ylabel = "Second Principal Component", filename = output_directory + "Kmeans/Kmeans.png" )
+            gu.plot_kmeans_plus_pca( pca_ft, kmeans, sample_mask, [resin_data.loc[i]["Label"] for i in sample_mask], savefig = True, xlabel = "First Principal Component", ylabel = "Second Principal Component", filename = output_directory + "Global/Kmeans/Kmeans.png" )
 
             label_and_cluster_label = zip( [resin_data.loc[i]["Label"] for i in sample_mask], kmeans.labels_ )
 
             print( "KMeans cluster labels:", list( label_and_cluster_label ) )
 
-def distance_to_virgin_analysis_based_on_pcas( directory, features_df ):
+def distance_to_virgin_analysis_based_on_pcas( output_directory, features_df ):
 
     dataset_names = ["FTIR", "DSC", "TGA", "Rhe", "TT", "Colour"]
     dataset_labels = ["FTIR", "DSC", "TGA", "Rheo", "Mech", "Colour"]
 
     iter = gu.subset_combinations_for_all_sizes_of_subsets( len( dataset_names ) )
 
     virgin_samples = [16, 17, 19]
@@ -637,15 +643,15 @@
 
         cbar_ax = fig.add_axes( [0.8, 0.4, 0.04, 0.2] )
         cbar = fig.colorbar( im, cax = cbar_ax, shrink = 0.2 )
         cbar.ax.tick_params( labelsize = 25 )
 
         plt.subplots_adjust( left = 0.1, bottom = 0.4, right = 0.9, top = 0.6, wspace = 0.4, hspace = 0.4 )
 
-        plt.savefig( directory + "Global/Output/Distance_to_Virgin_Analysis/" + "Horizontal.pdf" )
+        plt.savefig( output_directory + "Global/Distance_to_Virgin_Analysis/" + "Horizontal.pdf" )
 
         plt.close()
 
     if True:
 
         # Triplets, vertical.
 
@@ -693,15 +699,15 @@
 
         cbar_ax = fig.add_axes( [0.66, 0.22, 0.06, 0.56] )
         cbar = fig.colorbar( im, cax = cbar_ax, shrink = 1 )
         cbar.ax.tick_params( labelsize = 25 )
 
         plt.subplots_adjust( left = 0.4, bottom = 0.1, right = 0.6, top = 0.9, wspace = 0.4, hspace = 0.4 )
 
-        plt.savefig( directory + "Global/Output/Distance_to_Virgin_Analysis/" + "Vertical.pdf" )
+        plt.savefig( output_directory + "Global/Distance_to_Virgin_Analysis/" + "Vertical.pdf" )
 
         plt.close()
 
     if False:
 
         searches = ["FTIR", "DSC", "TGA", "Rheo", "Mech", "Colour"]
 
@@ -735,15 +741,15 @@
             #
             #     ax[i].text( 0, j, pattern.search( dfs[i].index[j] ).groups()[0] + "\n" + pattern.search( dfs[i].index[j] ).groups()[1] + "\n" + pattern.search( dfs[i].index[j] ).groups()[2], ha = "center", va = "center", color = "w" )
 
             ax[i].invert_yaxis()
 
         plt.tight_layout()
 
-        plt.savefig( directory + "Global/Output/Distance_to_Virgin_Analysis/" + "Plot.pdf" )
+        plt.savefig( output_directory + "Global/Distance_to_Virgin_Analysis/" + "Plot.pdf" )
 
         plt.close()
 
 def rank_resins_by_pp_content( directory, features_df, rank_features_df ):
 
     resin_data = gu.get_list_of_resins_data( directory ) # Obtain the spreadsheet of data for the resins.
```

### Comparing `rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis/Global_Utilities.py` & `rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis/Global_Utilities.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.6/rHDPE_Data_Analysis.egg-info/SOURCES.txt` & `rHDPE_Data_Analysis-1.0.7/rHDPE_Data_Analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*


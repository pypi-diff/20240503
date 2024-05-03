# Comparing `tmp/dsplus-0.4.2.tar.gz` & `tmp/dsplus-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsplus-0.4.2.tar", last modified: Wed Apr 17 03:57:11 2024, max compression
+gzip compressed data, was "dsplus-0.4.3.tar", last modified: Fri May  3 00:22:43 2024, max compression
```

## Comparing `dsplus-0.4.2.tar` & `dsplus-0.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 03:57:11.741144 dsplus-0.4.2/
--rw-rw-rw-   0        0        0     1083 2024-03-15 02:57:42.000000 dsplus-0.4.2/LICENSE
--rw-rw-rw-   0        0        0      690 2024-04-17 03:57:11.735693 dsplus-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0       99 2024-02-24 21:14:11.000000 dsplus-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 03:57:11.707527 dsplus-0.4.2/dsplus/
--rw-rw-rw-   0        0        0      171 2024-04-17 03:56:55.000000 dsplus-0.4.2/dsplus/__init__.py
--rw-rw-rw-   0        0        0    24320 2024-04-02 22:58:04.000000 dsplus-0.4.2/dsplus/pb_functions_general.py
--rw-rw-rw-   0        0        0    42751 2024-04-17 00:36:26.000000 dsplus-0.4.2/dsplus/pb_functions_pandas.py
--rw-rw-rw-   0        0        0    56894 2024-04-02 22:58:04.000000 dsplus-0.4.2/dsplus/pb_functions_plotly.py
--rw-rw-rw-   0        0        0    44406 2024-04-12 03:03:10.000000 dsplus-0.4.2/dsplus/pb_functions_spatial.py
-drwxrwxrwx   0        0        0        0 2024-04-17 03:57:11.726224 dsplus-0.4.2/dsplus.egg-info/
--rw-rw-rw-   0        0        0      690 2024-04-17 03:57:11.000000 dsplus-0.4.2/dsplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-04-17 03:57:11.000000 dsplus-0.4.2/dsplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 03:57:11.000000 dsplus-0.4.2/dsplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-17 03:57:11.000000 dsplus-0.4.2/dsplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 03:57:11.741144 dsplus-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1650 2024-03-29 02:13:48.000000 dsplus-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 03:57:11.730037 dsplus-0.4.2/tests/
--rw-rw-rw-   0        0        0    12530 2024-04-17 03:55:44.000000 dsplus-0.4.2/tests/Test_pandas.py
+drwxrwxrwx   0        0        0        0 2024-05-03 00:22:43.069855 dsplus-0.4.3/
+-rw-rw-rw-   0        0        0     1083 2024-03-15 02:57:42.000000 dsplus-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0      690 2024-05-03 00:22:43.066053 dsplus-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0       99 2024-02-24 21:14:11.000000 dsplus-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 00:22:43.035422 dsplus-0.4.3/dsplus/
+-rw-rw-rw-   0        0        0      171 2024-05-03 00:09:20.000000 dsplus-0.4.3/dsplus/__init__.py
+-rw-rw-rw-   0        0        0    24324 2024-05-02 23:18:42.000000 dsplus-0.4.3/dsplus/pb_functions_general.py
+-rw-rw-rw-   0        0        0    42785 2024-05-02 23:18:42.000000 dsplus-0.4.3/dsplus/pb_functions_pandas.py
+-rw-rw-rw-   0        0        0    56894 2024-04-02 22:58:04.000000 dsplus-0.4.3/dsplus/pb_functions_plotly.py
+-rw-rw-rw-   0        0        0    48825 2024-05-02 23:18:42.000000 dsplus-0.4.3/dsplus/pb_functions_spatial.py
+drwxrwxrwx   0        0        0        0 2024-05-03 00:22:43.053322 dsplus-0.4.3/dsplus.egg-info/
+-rw-rw-rw-   0        0        0      690 2024-05-03 00:22:42.000000 dsplus-0.4.3/dsplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-03 00:22:42.000000 dsplus-0.4.3/dsplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 00:22:42.000000 dsplus-0.4.3/dsplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-03 00:22:42.000000 dsplus-0.4.3/dsplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 00:22:43.069855 dsplus-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1650 2024-03-29 02:13:48.000000 dsplus-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 00:22:43.057687 dsplus-0.4.3/tests/
+-rw-rw-rw-   0        0        0    12530 2024-04-17 03:55:44.000000 dsplus-0.4.3/tests/Test_pandas.py
```

### Comparing `dsplus-0.4.2/LICENSE` & `dsplus-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.2/PKG-INFO` & `dsplus-0.4.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsplus
-Version: 0.4.2
+Version: 0.4.3
 Summary: Helper functions for data science applications.
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: data science,pandas
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dsplus-0.4.2/dsplus/pb_functions_general.py` & `dsplus-0.4.3/dsplus/pb_functions_general.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,15 +423,15 @@
             temp_str_current = temp_str_current.reset_index(drop = True)
 
             str_c = str_c.str.cat(temp_str_current.astype(str))
 
         return (str_c)
 
 #%%
-def str_join(v_str: list|np.ndarray|pd.Series, join_sep: str=',') -> str:
+def str_join(v_str: list|np.ndarray|pd.Series, join_sep: str = ',') -> str:
     '''Join multiple strings into a single string with a join separator. Wrapper around 'join()'.
 
     Args:
         v_str (list | np.ndarray | pd.Series): Vector of strings.
         join_sep (str, optional): Join separator. Defaults to ', '.
 
     Returns:
@@ -489,15 +489,15 @@
     else:
         return (pd.Series())
 
     y_smooth = pd.Series(y_smooth)
     return (y_smooth)
 
 #%%
-def interp_1d(x: list|np.ndarray|pd.Series, y: list|np.ndarray|pd.Series, x_out: float|list|np.ndarray|pd.Series = None, fill_value: str='extrapolate') -> pd.Series:
+def interp_1d(x: list|np.ndarray|pd.Series, y: list|np.ndarray|pd.Series, x_out: float|list|np.ndarray|pd.Series = None, fill_value: str = 'extrapolate') -> pd.Series:
     '''Estimate values through linear interpolation. Can be used to fill NA values. Can fill or extrapolate values outside bounds.
 
     Args:
         x (list | np.ndarray | pd.Series): Vector of x values.
         y (list | np.ndarray | pd.Series): Vector of y values.
         x_out (float | list | array | Series, optional): Vector of x values for which y values are to be estimated. Defaults to None.
         fill_value (str, optional): Fill value for 'x_out' values outside the bounds of 'x'. Acceptable values are 'extrapolate' to extrapolate values, 'na' to set as NA values, 'ffill' to do a forward fill, 'bfill' to do a back fill, and 'fill' to do a forward and backward fill. Defaults to 'extrapolate'.
```

### Comparing `dsplus-0.4.2/dsplus/pb_functions_pandas.py` & `dsplus-0.4.3/dsplus/pb_functions_pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
     return vector
 
 #endregion -----------------------------------------------------------------------------------------
 #region Functions: Pandas: Slice
 
 #%%
-def pd_cols(df: pd.DataFrame, cols: str, to_list=True) -> list|pd.Series:
+def pd_cols(df: pd.DataFrame, cols: str, to_list = True) -> list|pd.Series:
     '''Get a vector of desired column names in desired order. Works well together with 'pd_select_simple()'.
 
     Args:
         df (pd.DataFrame): Dataframe whose column names are to be extracted.
         cols (str): String representing column name extraction rules. See notes.
         to_list (bool, optional): Whether to return a list or series of column names. Defaults to True (return list).
 
@@ -265,18 +265,18 @@
         >>> df.pipe(pd_select, 'select_dtypes("number"), *')
         >>> df.pipe(pd_select, '-v2:')
     '''
     return df[lambda _: pd_cols(_, cols)]
 
 #%%
 def pd_select_simple(df: pd.DataFrame,
-                     cols_before: str|list|np.ndarray|pd.Series=None,
-                     cols_after: str|list|np.ndarray|pd.Series=None,
-                     cols_drop: str|list|np.ndarray|pd.Series=None,
-                     remaining=True) -> pd.DataFrame:
+                     cols_before: str|list|np.ndarray|pd.Series = None,
+                     cols_after: str|list|np.ndarray|pd.Series = None,
+                     cols_drop: str|list|np.ndarray|pd.Series = None,
+                     remaining = True) -> pd.DataFrame:
     '''Select columns to keep or drop from dataframe. Can be used to change order of columns.
 
     Args:
         df (pd.DataFrame): Dataframe.
         cols_before (str | list | np.ndarray | pd.Series, optional): Columns to keep at the start. Defaults to None.
         cols_after (str | list | np.ndarray | pd.Series, optional): Columns to keep at the end. Defaults to None.
         cols_drop (str | list | np.ndarray | pd.Series, optional): Columns to drop. Defaults to None.
@@ -316,17 +316,17 @@
 
     cols_keep = [x for x in cols_keep if x not in cols_drop]
 
     return df[cols_keep]
 
 #%%
 def pd_drop(df: pd.DataFrame,
-            cols: str|list|np.ndarray|pd.Series=None,
-            col_from: str=None,
-            col_to: str=None) -> pd.DataFrame:
+            cols: str|list|np.ndarray|pd.Series = None,
+            col_from: str = None,
+            col_to: str = None) -> pd.DataFrame:
     '''Drop selected columns from dataframe.
 
     Args:
         df (pd.DataFrame): Dataframe.
         cols (str | list | np.ndarray | pd.Series, optional): Vector of columns to drop. Defaults to None (first column).
         col_from (str, optional): First column in series of columns to drop. Defaults to None (last column).
         col_to (str, optional): Last column in series of column to drop. Defaults to None.
@@ -383,15 +383,15 @@
         >>> v_values.pipe(pd_concat_series, 3)
         >>> v_values.pipe(pd_concat_series, [3, 4])
     '''
     v_values_concat = pd.concat([v_values, pd.Series(values)])
     return v_values_concat
 
 #%%
-def pd_concat_rows(df1: pd.DataFrame, df2: pd.DataFrame, ignore_index=True) -> pd.DataFrame:
+def pd_concat_rows(df1: pd.DataFrame, df2: pd.DataFrame, ignore_index = True) -> pd.DataFrame:
     '''Concatenate dataframes by rows. Mainly useful for piping with 'pd.pipe()'. Wrapper around 'pd.concat()'. If one of the dataframes is blank, the other is returned, ensuring no change in datatype like with 'pd.concat()'.
 
     Args:
         df1 (pd.DataFrame): Dataframe.
         df2 (pd.DataFrame): Dataframe.
         ignore_index (bool):  If True, do not use the index values along the concatenation axis. The resulting axis will be labeled 0, ..., n - 1. Defaults to True.
 
@@ -477,17 +477,17 @@
 
 #endregion -----------------------------------------------------------------------------------------
 #region Functions: Pandas: Merge
 
 #%%
 def pd_merge_asof(df1: pd.DataFrame,
                   df2: pd.DataFrame,
-                  on: str= None,
-                  left_on: str= None,
-                  right_on: str= None,
+                  on: str = None,
+                  left_on: str = None,
+                  right_on: str = None,
                   direction: Literal['backward', 'forward', 'nearest'] = 'forward',
                   one_to_many = False):
     '''Perform a merge by key direction. Wrapper around 'pandas.merge_asof()'. Unlike 'pandas.merge_asof()', default direction is 'forward'. Additionally, 'one_to_many' is an additional option. Finally, if one of the two dataframes are blank, 'df1' is still returned along with columns from 'df2' added and set to np.nan, and no error is raised
 
     Args:
         df1 (pd.DataFrame): Dataframe.
         df2 (pd.DataFrame): Dataframe.
@@ -572,17 +572,17 @@
 
 #endregion -----------------------------------------------------------------------------------------
 #region Functions: Pandas: Reshape
 
 #%%
 def pd_pivot_longer(df_wide: pd.DataFrame,
                     id_vars: str|list|np.ndarray|pd.Series,
-                    value_vars: str|list|np.ndarray|pd.Series=None,
-                    var_name: str=None,
-                    value_name: str=None) -> pd.DataFrame:
+                    value_vars: str|list|np.ndarray|pd.Series = None,
+                    var_name: str = None,
+                    value_name: str = None) -> pd.DataFrame:
     '''Reshape table from wide to long. Wrapper around 'pd.melt()' but provides easier documentation.
 
     Args:
         df_wide (pd.DataFrame): Dataframe in wide format.
         id_vars (str | list | np.ndarray | pd.Series): Columns that uniquely identify each observation.
         value_vars (str | list | np.ndarray | pd.Series, optional): Columns to unpivot. Defaults to None. If set to None, all of the other columns are used.
         var_name (str, optional): Name to use for the 'variable' column. Defaults to None. If set to None, new column is named 'variable'.
@@ -612,15 +612,15 @@
 
     return df_long
 
 #%%
 def pd_pivot_wider(df_long: pd.DataFrame,
                    index: str|list|np.ndarray|pd.Series,
                    columns: str,
-                   values: str|list|np.ndarray|pd.Series=None,
+                   values: str|list|np.ndarray|pd.Series = None,
                    keep_val:bool = False,
                    join_sep: str = '_',
                    col_first:bool = True) -> pd.DataFrame:
     '''Reshape table from long to wide. Wrapper around 'pd.pivot()' but prevents multiindex and provides easier documentation.
 
     Args:
         df_long (pd.DataFrame): Dataframe in long format.
@@ -780,15 +780,15 @@
 #region Functions: Pandas: View
 
 #%%
 def pd_style(df: pd.DataFrame,
              negative = True,
              highlight_max = True,
              highlight_min = True,
-             precision: int=None):
+             precision: int = None):
     '''Return tabular visualization.
 
     Args:
         df (pd.DataFrame): Dataframe.
         negative (bool, optional): Show negative numbers in red font. Defaults to True.
         max (bool, optional): Highlight max column values in purple. Defaults to True.
         min (bool, optional): Highlight min column vlaues in blue. Defaults to True.
@@ -822,15 +822,15 @@
                                   props='color:white;background-color:purple;',
                                   axis=0,
                                   subset=v_col_num)
 
     return df_style
 
 #%%
-def pd_print(df: pd.DataFrame, title: str=None) -> pd.DataFrame:
+def pd_print(df: pd.DataFrame, title: str = None) -> pd.DataFrame:
     '''Print and return dataframe. This is mainly to be used to print and assign or print and pipe at the same time.
 
     Args:
         df (pd.DataFrame): Dataframe to print and return.
         title (str, optional): Text to print before printing dataframe. Defaults to None.
 
     Returns:
@@ -850,15 +850,15 @@
 #region Functions: Pandas: Index
 
 #%%
 def pd_reset_column(df: pd.DataFrame,
                     rev: bool = False,
                     join_sep: str = '_',
                     keep_name: bool = False,
-                    join_sep_name:str = '_') -> pd.DataFrame:
+                    join_sep_name: str = '_') -> pd.DataFrame:
     '''Flatten multi-level column and remove column index name.
 
     Args:
         df (pd.DataFrame): Dataframe.
         rev (bool, optional): Whether to join in reverse order (down to up). Defaults to False.
         join_sep (str, optional): Separator string between column levels when joining. Defaults to '_'.
         keep_name (str, optional): Whether to join column index names to column names. Defaults to False.
```

### Comparing `dsplus-0.4.2/dsplus/pb_functions_plotly.py` & `dsplus-0.4.3/dsplus/pb_functions_plotly.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.2/dsplus/pb_functions_spatial.py` & `dsplus-0.4.3/dsplus/pb_functions_spatial.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 
     if crs is not None:
         sp_polygons.crs = crs
 
     return (sp_polygons)
 
 #%%
-def sp_to_df_xy(sp: gpd.GeoDataFrame, explode:bool = True, cols_to_keep:str|list|np.ndarray|pd.Series = None, cols_keep_all:bool = False):
+def sp_to_df_xy(sp: gpd.GeoDataFrame, explode:bool = True, cols_to_keep:str|list|np.ndarray|pd.Series = None, cols_keep_all:bool = False) -> pd.DataFrame:
     '''Convert geodataframe to dataframe of x and y values.
 
     Args:
         sp (GeoDataFrame): Geodataframe.
         explode (bool, optional): Whether to explode geometry. Defaults to True
         cols_to_keep (str | list | np.ndarray | pd.Series, optional): Vector of columns to keep from 'sp'. Defaults to None.
         cols_keep_all (bool, optional): Whether to keep all columns from 'sp'. Defaults to False.
@@ -220,44 +220,146 @@
         df_xy = df_xy.merge(sp[cols_to_keep].reset_index(), on='index')
 
     if cols_to_keep_extra is not None:
         df_xy = df_xy.pipe(pd_select_simple, ['index', *cols_to_keep_extra])
     return df_xy
 
 #endregion -----------------------------------------------------------------------------------------
+#region Functions: Vector Combination
+
+#%%
+def sp_intersection(sp_1: gpd.GeoDataFrame, sp_2: gpd.GeoDataFrame, multipart = False) -> gpd.GeoDataFrame:
+    '''Get intersection of two geometries.
+
+    Args:
+        sp_1 (gpd.GeoDataFrame): First geometry.
+        sp_2 (gpd.GeoDataFrame): Second geometry.
+        multipart (bool, optional): Whether to include multippart geometries. If set to False, the intersected geometry is exploded usign 'sp_explode()'. Defaults to False.
+
+    Returns:
+        gpd.GeoDataFrame: Intersected geometry. Attributes from both geometries are included.
+    '''
+    sp_intersect = pd.DataFrame()
+    for i, row_i in sp_1.iterrows():
+        for j, row_j in sp_2.iterrows():
+            if row_i.geometry.intersects(row_j.geometry):
+                temp_sp_intersect = row_i.geometry.intersection(row_j.geometry)
+
+                temp_sp_intersect = \
+                (pd_concat_cols_multiple(
+                    sp_1.iloc[[i]].drop(columns='geometry'),
+                    sp_2.iloc[[j]].drop(columns='geometry'),
+                    )
+                    .assign(geometry = [temp_sp_intersect])
+                )
+
+                sp_intersect = sp_intersect.pipe(pd_concat_rows, temp_sp_intersect)
+
+    sp_intersect = gpd.GeoDataFrame(sp_intersect, geometry='geometry')
+    sp_intersect.crs = sp_1.crs
+
+    if not multipart:
+        sp_intersect = sp_explode(sp_intersect)
+
+    return sp_intersect
+
+#%%
+def sp_intersects(sp_1: gpd.GeoDataFrame, sp_2: gpd.GeoDataFrame) -> pd.DataFrame:
+    '''Check if geometries intersect.
+
+    Args:
+        sp_1 (gpd.GeoDataFrame): First geometry.
+        sp_2 (gpd.GeoDataFrame): Second geometry.
+
+    Returns:
+        pd.DataFrame: Dataframe with a column, 'intersects' which is True if two geometries intersect and False if they don't. Attributes from both geometries are included.
+
+    Notes:
+        - Each individual feature pairs are tested. So if 'sp_1' has m features and 'sp_2' has n features, the resulting dataframe will have m*n rows.
+    '''
+    df_intersects = pd.DataFrame()
+    for i, row_i in sp_1.iterrows():
+        for j, row_j in sp_2.iterrows():
+            check = row_i.geometry.intersects(row_j.geometry)
+
+            temp_df_intersects = \
+            (pd_concat_cols_multiple(
+                sp_1.iloc[[i]].drop(columns='geometry'),
+                sp_2.iloc[[j]].drop(columns='geometry'),
+                )
+                .assign(intersects = [check])
+            )
+
+            df_intersects = df_intersects.pipe(pd_concat_rows, temp_df_intersects)
+
+    return df_intersects
+
+#%%
+def sp_intersects_summary(sp_1: gpd.GeoDataFrame, sp_2: gpd.GeoDataFrame, count = False, return_series = False) -> np.ndarray | pd.Series:
+    '''Check if geometries in 'sp_1' intersect any of the geometries in 'sp_2'. Uses 'sp_intersects()' as a backend.
+
+    Args:
+        sp_1 (gpd.GeoDataFrame): First geometry.
+        sp_2 (gpd.GeoDataFrame): Second geometry.
+        count (bool, False): Whether to return True/False or count (number of intersersections). Defaults to False (returns True/False).
+        return_series (bool, False): Whether to return numpy array or pandas series. Defaults to False (return numpy array).
+
+    Returns:
+        np.ndarray | pd.Series: An array or series of True/False values (or intersection counts) indicating if (or how many times) each feature in 'sp_1' intersects any feature in 'sp_2'. The length of this array is the same as the number of features (rows) in 'sp_1'.
+    '''
+    sp_1 = sp_1.assign(_sn = lambda _: np.arange(_.shape[0]))
+
+    df_intersects = sp_intersects(sp_1, sp_2)
+
+    v_intersects = \
+    (df_intersects
+        .groupby('_sn')
+        ['intersects']
+        .sum()
+    )
+
+    if not return_series:
+        v_intersects = v_intersects.to_numpy()
+
+    if not count:
+        v_intersects = (v_intersects > 0)
+
+    return v_intersects
+
+#endregion -----------------------------------------------------------------------------------------
 #region Functions: Chainage
 
 #%%
-def sp_get_chainage(sp_line: gpd.GeoDataFrame, sp_points: gpd.GeoDataFrame, return_series=True):
+def sp_get_chainage(sp_line: gpd.GeoDataFrame, sp_points: gpd.GeoDataFrame, return_series=True) -> np.ndarray | pd.Series:
     '''Get chainage of points on a polyline.
 
     Args:
         sp_line (GeoDataFrame): Polyline geodataframe.
         sp_points (GeoDataFrame): Points geodataframe.
         return_series (bool, optional): Return series (if True) or list (if False). Defaults to True.
 
     Returns:
-        pd.Series | List of float: Series or list of chainages. Same unit as geodataframe.
+        np.ndarray | pd.Series of float: Array or series of chainages. Same unit as geodataframe.
     '''
     chainage = [sp_line.geometry.iloc[0].project(sp_point) for sp_point in sp_points.geometry]
     # chainage = [sp_line.geometry.project(sp_point).iloc[0] for sp_point in sp_points.geometry]
     if return_series:
         return (pd.Series(chainage))
     else:
-        return (chainage)
+        return (np.array(chainage))
 
 #%%
-def sp_get_chainage_from_df_xy(df_xy: pd.DataFrame):
+def sp_get_chainage_from_df_xy(df_xy: pd.DataFrame) -> pd.DataFrame:
     '''Get chainage from dataframe.
 
     Args:
         df_xy (DataFrame): Dataframe with 'x' and 'y' columns.
 
     Returns:
-        pd.DataFrame: dataframe with two appended columns: 'dist' (distance from previous point) and 'chainage' (chainage from first point).
+        pd.DataFrame: Dataframe with two appended columns: 'dist' (distance from previous point) and 'chainage' (chainage from first point).
     '''
     df_chainage = \
         (df_xy
             .assign(diff_x = lambda _: _['x'].diff().fillna(0))
             .assign(diff_y = lambda _: _['y'].diff().fillna(0))
             .assign(dist = lambda _: np.sqrt(_['diff_x']**2 + _['diff_y']**2))
             .assign(chainage = lambda _: _['dist'].cumsum())
@@ -291,23 +393,23 @@
         >>> sp_zonal_stats_points(sp_points, files_rasters, id_cols='name', col_names=os_basename(files_raster, keep_extension=False))
     '''
     df_xy = sp_points.geometry.get_coordinates()
     coords = [(x,y) for x, y in zip(df_xy.x, df_xy.y)]
 
     if isinstance(files_raster, str):
         with rasterio.open(files_raster) as f:
-            temp_values = [val[0] for val in f.sample(coords)]
+            temp_values = [val[0] for val in f.sample(coords)] # https://rasterio.readthedocs.io/en/latest/api/rasterio._io.html#rasterio._io.DatasetReaderBase.sample
         temp_values = pd.Series(temp_values)
 
         return (temp_values)
     else:
         df_values = []
         for file_raster in files_raster:
             with rasterio.open(file_raster) as f:
-                df_values.append([val[0] for val in f.sample(coords)])
+                df_values.append([val[0] for val in f.sample(coords)]) # https://rasterio.readthedocs.io/en/latest/api/rasterio._io.html#rasterio._io.DatasetReaderBase.sample
         df_values = pd.DataFrame(df_values).T
 
         if col_names is not None:
             df_values = df_values.pipe(pd_set_colnames, col_names)
 
         if id_cols is not None:
             id_cols = pd_to_series(id_cols)
@@ -378,15 +480,14 @@
     if files_raster_is_str:
         df_profile = df_profile.pipe(pd_select_simple, id_cols)
     else:
         df_profile = df_profile.pipe(pd_select_simple, filename_colname).pipe(pd_select_simple, id_cols)
 
     return (df_profile)
 
-
 #%%
 def sp_zonal_stats_poly(sp_poly: gpd.GeoDataFrame, files_raster: str|list|np.ndarray|pd.Series, stats: str|list=['min', 'max', 'mean', 'sum', 'median', 'majority'], id_cols: str|list|np.ndarray|pd.Series = None, files_raster_mapped: str|list|np.ndarray|pd.Series = None, filename_colname = 'file') -> pd.Series|pd.DataFrame|dict:
     '''Get raster value summaries at polygons.
 
     Args:
         sp_poly (GeoDataFrame): Geodataframe of polygons.
         files_raster (str | list | np.ndarray | pd.Series): Vector of raster file(s)
@@ -722,22 +823,22 @@
                            hovertemplate=None)
     return fig
 
 #endregion -----------------------------------------------------------------------------------------
 #region Functions: Others
 
 #%%
-def sp_explode(sp: gpd.GeoDataFrame):
+def sp_explode(sp: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
     '''Explodes geodataframe.
 
     Args:
-        sp (GeoDataFrame): Geodataframe.
+        sp (gpd.GeoDataFrame): Geodataframe.
 
     Returns:
-        pd.DataFrame: Exploded geodataframe with additional columns: 'id_geom' indicating individual geometry parts, 'id_sp' indicating index of 'sp', and 'id_part' indicating individual geometry parts for each index of 'sp'.
+        gpd.GeoDataFrame: Exploded geodataframe with additional columns: 'id_geom' indicating individual geometry parts, 'id_sp' indicating index of 'sp', and 'id_part' indicating individual geometry parts for each index of 'sp'.
 
     Notes:
         - 'id_geom' is f'{id_sp}__{id_part}' and is unique.
         - If all geometry are singlepart, each entry in 'id' will be unique, and 'id_part' will all be 0.
         - For a multipart geometry, 'id_sp' will be the same, and 'id_part' will be unique.
 
     Examples:
@@ -756,15 +857,15 @@
     return sp_exploded
 
 #%%
 def sp_get_points_along_line(sp_line: gpd.GeoDataFrame, v_distances_normalized: list|np.ndarray|pd.Series=None, count: int=None, spacing: float=None, spacing_normalized: float=None, include_ends=True) -> gpd.GeoDataFrame:
     '''Generate points along polyline.
 
     Args:
-        sp_line (GeoDataFrame): Geodataframe with single polyline feature.
+        sp_line (gpd.GeoDataFrame): Geodataframe with single polyline feature.
         v_distances (list | np.ndarray | pd.Series of float, optional): Vector of normalized distances ([0, 1]). Defaults to None. 0 means start of line and 1 means end.
         count (int, optional): Number of points to generate. Defaults to None.
         spacing (float, optional): Spacing between each point in absolute units. Defaults to None.
         spacing_normalized (float, optional): Spacing between each point in relative units ([0, 1]). Defaults to None.
         include_ends (bool, optional): Indicates where points at the ends (start and end) need to be included. Defaults to True. Overridden when 'v_distances_normalized' is used.
 
     Returns:
@@ -801,19 +902,19 @@
     v_distances_normalized = np.array(v_distances_normalized)
     sp_points = gpd.GeoDataFrame.from_features(gpd.GeoSeries([sp_line.geometry.iloc[0].interpolate(distance, normalized=True) for distance in v_distances_normalized]))
     sp_points = sp_points.eval('chainage_normalized = @v_distances_normalized').assign(chainage = lambda _: _['chainage_normalized']*temp_length.iloc[0])
 
     return (sp_points)
 
 #%%
-def sp_offset_line_poly(sp: gpd.GeoDataFrame, distance: float, join_style='mitre'):
+def sp_offset_line_poly(sp: gpd.GeoDataFrame, distance: float, join_style='mitre') -> gpd.GeoDataFrame:
     '''Offset polyline or polygon.
 
     Args:
-        sp (GeoDataFrame): Polyline or polygon geodataframe with single feature.
+        sp (gpd.GeoDataFrame): Polyline or polygon geodataframe with single feature.
         distance (numeric): Distance to offset by. Same unit as gdf. Positive means offset left. Direction is determined by following the direction of the given geometric points.
         join_style (str, optional): Join style for corners between line segments. Acceptable values are 'round' (rounded corner), 'mitre' (sharp corner), and 'bevel' (bevelled corner). Defaults to 'mitre'.
 
     Returns:
         gpd.GeoDataFrame: Polyline or polygon geodataframe with offsetted feature.
     '''
     return (gpd.GeoDataFrame.from_features(gpd.GeoSeries([sp.geometry.iloc[0].offset_curve(distance, join_style=join_style)])))
```

### Comparing `dsplus-0.4.2/dsplus.egg-info/PKG-INFO` & `dsplus-0.4.3/dsplus.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsplus
-Version: 0.4.2
+Version: 0.4.3
 Summary: Helper functions for data science applications.
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: data science,pandas
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dsplus-0.4.2/setup.py` & `dsplus-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.2/tests/Test_pandas.py` & `dsplus-0.4.3/tests/Test_pandas.py`

 * *Files identical despite different names*


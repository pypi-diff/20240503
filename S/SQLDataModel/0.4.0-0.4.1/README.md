# Comparing `tmp/sqldatamodel-0.4.0.tar.gz` & `tmp/sqldatamodel-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqldatamodel-0.4.0.tar", last modified: Tue Apr 23 22:06:52 2024, max compression
+gzip compressed data, was "sqldatamodel-0.4.1.tar", last modified: Thu May  2 23:00:27 2024, max compression
```

## Comparing `sqldatamodel-0.4.0.tar` & `sqldatamodel-0.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 22:06:52.990235 sqldatamodel-0.4.0/
--rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 sqldatamodel-0.4.0/LICENSE
--rw-rw-rw-   0        0        0    27204 2024-04-23 22:06:52.977437 sqldatamodel-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    25304 2024-04-18 17:59:54.000000 sqldatamodel-0.4.0/README.md
--rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 sqldatamodel-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-23 22:06:52.991235 sqldatamodel-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     2432 2024-04-23 20:12:46.000000 sqldatamodel-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 22:06:51.583553 sqldatamodel-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-23 22:06:52.758817 sqldatamodel-0.4.0/src/SQLDataModel/
--rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 sqldatamodel-0.4.0/src/SQLDataModel/ANSIColor.py
--rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 sqldatamodel-0.4.0/src/SQLDataModel/HTMLParser.py
--rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 sqldatamodel-0.4.0/src/SQLDataModel/JSONEncoder.py
--rw-rw-rw-   0        0        0   600424 2024-04-23 22:06:16.000000 sqldatamodel-0.4.0/src/SQLDataModel/SQLDataModel.py
--rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 sqldatamodel-0.4.0/src/SQLDataModel/StandardDeviation.py
--rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 sqldatamodel-0.4.0/src/SQLDataModel/__init__.py
--rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 sqldatamodel-0.4.0/src/SQLDataModel/converters.py
--rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 sqldatamodel-0.4.0/src/SQLDataModel/demo.py
--rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 sqldatamodel-0.4.0/src/SQLDataModel/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-23 22:06:52.905454 sqldatamodel-0.4.0/src/SQLDataModel/extensions/
--rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 sqldatamodel-0.4.0/src/SQLDataModel/extensions/__init__.py
--rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 sqldatamodel-0.4.0/src/SQLDataModel/extensions/str_utils.c
-drwxrwxrwx   0        0        0        0 2024-04-23 22:06:52.976028 sqldatamodel-0.4.0/src/SQLDataModel.egg-info/
--rw-rw-rw-   0        0        0    27204 2024-04-23 22:06:50.000000 sqldatamodel-0.4.0/src/SQLDataModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2024-04-23 22:06:51.000000 sqldatamodel-0.4.0/src/SQLDataModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 22:06:51.000000 sqldatamodel-0.4.0/src/SQLDataModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-23 22:06:51.000000 sqldatamodel-0.4.0/src/SQLDataModel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-23 22:06:52.920156 sqldatamodel-0.4.0/tests/
--rw-rw-rw-   0        0        0    59564 2024-04-23 20:10:21.000000 sqldatamodel-0.4.0/tests/test_Future.py
--rw-rw-rw-   0        0        0    59567 2024-04-23 20:10:35.000000 sqldatamodel-0.4.0/tests/test_SQLDataModel.py
+drwxrwxrwx   0        0        0        0 2024-05-02 23:00:27.950807 sqldatamodel-0.4.1/
+-rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 sqldatamodel-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0    27196 2024-05-02 23:00:27.940472 sqldatamodel-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0    25304 2024-04-18 17:59:54.000000 sqldatamodel-0.4.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 sqldatamodel-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-02 23:00:27.952810 sqldatamodel-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     2424 2024-05-02 22:54:03.000000 sqldatamodel-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 23:00:26.349831 sqldatamodel-0.4.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-02 23:00:27.554252 sqldatamodel-0.4.1/src/SQLDataModel/
+-rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 sqldatamodel-0.4.1/src/SQLDataModel/ANSIColor.py
+-rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 sqldatamodel-0.4.1/src/SQLDataModel/HTMLParser.py
+-rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 sqldatamodel-0.4.1/src/SQLDataModel/JSONEncoder.py
+-rw-rw-rw-   0        0        0   599974 2024-05-02 22:54:01.000000 sqldatamodel-0.4.1/src/SQLDataModel/SQLDataModel.py
+-rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 sqldatamodel-0.4.1/src/SQLDataModel/StandardDeviation.py
+-rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 sqldatamodel-0.4.1/src/SQLDataModel/__init__.py
+-rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 sqldatamodel-0.4.1/src/SQLDataModel/converters.py
+-rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 sqldatamodel-0.4.1/src/SQLDataModel/demo.py
+-rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 sqldatamodel-0.4.1/src/SQLDataModel/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-02 23:00:27.825180 sqldatamodel-0.4.1/src/SQLDataModel/extensions/
+-rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 sqldatamodel-0.4.1/src/SQLDataModel/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 sqldatamodel-0.4.1/src/SQLDataModel/extensions/str_utils.c
+drwxrwxrwx   0        0        0        0 2024-05-02 23:00:27.932476 sqldatamodel-0.4.1/src/SQLDataModel.egg-info/
+-rw-rw-rw-   0        0        0    27196 2024-05-02 23:00:26.000000 sqldatamodel-0.4.1/src/SQLDataModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2024-05-02 23:00:26.000000 sqldatamodel-0.4.1/src/SQLDataModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 23:00:26.000000 sqldatamodel-0.4.1/src/SQLDataModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-02 23:00:26.000000 sqldatamodel-0.4.1/src/SQLDataModel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 23:00:27.851276 sqldatamodel-0.4.1/tests/
+-rw-rw-rw-   0        0        0    59564 2024-04-23 20:10:21.000000 sqldatamodel-0.4.1/tests/test_Future.py
+-rw-rw-rw-   0        0        0    59567 2024-05-02 19:24:28.000000 sqldatamodel-0.4.1/tests/test_SQLDataModel.py
```

### Comparing `sqldatamodel-0.4.0/LICENSE` & `sqldatamodel-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.0/PKG-INFO` & `sqldatamodel-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.4.0
+Version: 0.4.1
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
-Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package,polars2pandas,pandas2polars
+Keywords: SQL,ETL,dataframe,terminal-tables,pretty-print-tables,sql2sql,data-analysis,data-science,datamodel,extract,transform,load,web-scraping-tables,data-mining,html,html-table-parsing,apache-arrow,pyarrow,pyarrow-conversion,pyarrow-to-table,pyarrow-to-sql,pyarrow-to-csv,parquet-file-parsing,csv,csv-parsing,markdown,markdown-table-parsing,latex,latex-table-parsing,delimited,delimited-data-parsing,file-conversion,format-conversion,terminal-styling,table-styling,from-sqlite,to-sqlite,from-postgresql,to-postgresql,sql-to-sql,excel,xlsx-file,excel-to-sql,DataFrames,polars2pandas,pandas2polars
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `sqldatamodel-0.4.0/README.md` & `sqldatamodel-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.0/setup.py` & `sqldatamodel-0.4.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='SQLDataModel',  
-     version='0.4.0',
+     version='0.4.1',
      scripts=['src/SQLDataModel/SQLDataModel.py'] ,
      author='Ante Tonkovic-Capin',
      author_email='antetc@icloud.com',
      description='SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.',
-     keywords=['SQL','ETL','dataframe','terminal tables','pretty print tables','sql2sql','data analysis','data science','data model','extract','transform','load','web scraping tables','data mining','html','html table parsing','apache arrow','pyarrow','pyarrow conversion','pyarrow to table','pyarrow to sql','pyarrow to csv','parquet file parsing','csv','csv parsing','markdown','markdown table parsing','latex','latex table parsing','delimited','delimited data parsing','file conversion','format conversion','terminal styling','table styling','from sqlite','to sqlite','from postgresql','to postgresql','sql to sql','excel','xlsx file','excel to sql','DataFrame package','polars2pandas','pandas2polars'],
+     keywords=['SQL','ETL','dataframe','terminal-tables','pretty-print-tables','sql2sql','data-analysis','data-science','datamodel','extract','transform','load','web-scraping-tables','data-mining','html','html-table-parsing','apache-arrow','pyarrow','pyarrow-conversion','pyarrow-to-table','pyarrow-to-sql','pyarrow-to-csv','parquet-file-parsing','csv','csv-parsing','markdown','markdown-table-parsing','latex','latex-table-parsing','delimited','delimited-data-parsing','file-conversion','format-conversion','terminal-styling','table-styling','from-sqlite','to-sqlite','from-postgresql','to-postgresql','sql-to-sql','excel','xlsx-file','excel-to-sql','DataFrames','polars2pandas','pandas2polars'],
      license_file='LICENSE',
      long_description=long_description,
      long_description_content_type='text/markdown',
      url='https://github.com/AnteT/SQLDataModel',
      project_urls = {
         'Documentation':'https://sqldatamodel.readthedocs.io/en/latest/',
         'Source': 'https://github.com/AnteT/SQLDataModel.git'
```

### Comparing `sqldatamodel-0.4.0/src/SQLDataModel/ANSIColor.py` & `sqldatamodel-0.4.1/src/SQLDataModel/ANSIColor.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.0/src/SQLDataModel/HTMLParser.py` & `sqldatamodel-0.4.1/src/SQLDataModel/HTMLParser.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.0/src/SQLDataModel/JSONEncoder.py` & `sqldatamodel-0.4.1/src/SQLDataModel/JSONEncoder.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.0/src/SQLDataModel/SQLDataModel.py` & `sqldatamodel-0.4.1/src/SQLDataModel/SQLDataModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -2322,18 +2322,18 @@
     @classmethod
     def from_csv(cls, csv_source:str, infer_types:bool=True, encoding:str = 'Latin1', delimiter:str = ',', quotechar:str = '"', headers:list[str] = None, **kwargs) -> SQLDataModel:
         """
         Returns a new ``SQLDataModel`` generated from the provided CSV source, which can be either a file path or a raw delimited string.
 
         Parameters:
             ``csv_source`` (str): The path to the CSV file or a raw delimited string.
-            ``infer_types`` (bool, optional): Infer column types based on random subset of data. Default is ``True``, when False, all columns are str type.
-            ``encoding`` (str, optional): The encoding used to decode the CSV source if it is a file. Default is ``'Latin1'``.
-            ``delimiter`` (str, optional): The delimiter to use when parsing CSV source. Default is ``','``.
-            ``quotechar`` (str, optional): The character used for quoting fields. Default is ``'"'``.
+            ``infer_types`` (bool, optional): Infer column types based on random subset of data. Default is True, when False, all columns are str type.
+            ``encoding`` (str, optional): The encoding used to decode the CSV source if it is a file. Default is 'Latin1'.
+            ``delimiter`` (str, optional): The delimiter to use when parsing CSV source. Default is ``,``.
+            ``quotechar`` (str, optional): The character used for quoting fields. Default is ``"``.
             ``headers`` (List[str], optional): List of column headers. If None, the first row of the CSV source is assumed to contain headers.
             ``**kwargs``: Additional keyword arguments to be passed to the SQLDataModel constructor.
 
         Returns:
             ``SQLDataModel``: The SQLDataModel object created from the provided CSV source.
 
         Raises:
@@ -2394,15 +2394,14 @@
                 - Modifed to only parse CSV files and removed all delimiter sniffing with introduction of new method :meth:`SQLDataModel.from_delimited()` to handle other delimiters.
                 - Renamed ``delimiters`` parameter to ``delimiter`` with ``,`` set as new default to reflect revised focus on CSV files only.
 
         Note:
             - If ``csv_source`` is delimited by characters other than those specified, use :meth:`SQLDataModel.from_delimited()` and provide delimiter to ``delimiters``.
             - If ``headers`` are provided, the first row parsed from source will be the first row in the table and not discarded.
             - The ``infer_types`` argument can be used to infer the appropriate data type for each column:
-            
                 - If ``infer_types = True``, a random subset of the data will be used to infer the correct type and cast values accordingly
                 - If ``infer_types = False``, values from the first row only will be used to assign types, almost always 'str' when reading from CSV.
         """
         if os.path.exists(csv_source):
             try:
                 with open(csv_source, encoding=encoding) as csvfile:
                     tmp_all_rows = list(csv.reader(csvfile, delimiter=delimiter, quotechar=quotechar))
@@ -2603,15 +2602,15 @@
         Returns a new ``SQLDataModel`` generated from the provided delimited source, which can be either a file path or a raw delimited string.
 
         Parameters:
             ``source`` (str): The path to the delimited file or a raw delimited string.
             ``infer_types`` (bool, optional): Infer column types based on random subset of data. Default is True, when False, all columns are str type.
             ``encoding`` (str, optional): The encoding used to decode the source if it is a file. Default is ``'Latin1'``.
             ``delimiters`` (str, optional): Possible delimiters. Default is ``\\s``, ``\\t``, ``;``, ``|``, ``:`` or ``,`` (space, tab, semicolon, pipe, colon or comma).
-            ``quotechar`` (str, optional): The character used for quoting fields. Default is ``'"'``.
+            ``quotechar`` (str, optional): The character used for quoting fields. Default is ``"``.
             ``headers`` (list[str], optional): List of column headers. If None, the first row of the delimited source is assumed to be the header row.
             ``**kwargs``: Additional keyword arguments to be passed to the SQLDataModel constructor.
 
         Returns:
             ``SQLDataModel``: The SQLDataModel object created from the provided CSV source.
 
         Raises:
@@ -4246,17 +4245,16 @@
             text_source = "/path/to/tabular_data.txt"
 
             # Create the model using the text source
             sdm = SQLDataModel.from_text(text_source, table_identifier=2)
 
         Note:
             - This method is made for parsing ``SQLDataModel`` formatted text, such as the kind generated with ``print(sdm)`` or the output created by the inverse method :meth:`SQLDataModel.to_text()`
-            - For parsing delimited tabular data, this method calls :meth:`SQLDataModel.from_delimited()` method, which parses tabular data constructed with common delimiters.
-            - For parsing delimited tabular data when the delimiter is known, use :meth:`SQLDataModel.from_csv()` and provide the delimiter to use for parsing output.
-            - See :meth:`SQLDataModel.to_text()` for converting ``SQLDataModel`` to textual representation or for styling output.
+            - For parsing other delimited tabular data, this method calls the related :meth:`SQLDataModel.from_csv()` method, which parses tabular data constructed with common delimiters.
+
         """
         if not isinstance(text_source, str):
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(text_source).__name__}', expected `text_source` to be of type 'str', representing a tabular data filepath or tabular string literal")
             )
         if not isinstance(table_identifier, int):
             raise TypeError(
@@ -4434,20 +4432,20 @@
         return [tuple(x[0] for x in res.description),*data] if include_headers else data
 
     def to_csv(self, filename:str=None, delimiter:str=',', quotechar:str='"', lineterminator:str='\r\n', na_rep:str='None', index:bool=False, **kwargs) -> str|None:
         """
         Writes ``SQLDataModel`` to the specified file if ``filename`` argument if provided, otherwise returns the model directly as a CSV formatted string literal.
 
         Parameters:
-            ``filename`` (str): The name of the CSV file to which the data will be written. Default is ``None``, returning as raw literal.
-            ``delimiter`` (str, optional): The delimiter to use for separating values. Default is ``','``.
-            ``quotechar`` (str, optional): The character used to quote fields. Default is ``'"'``.
-            ``lineterminator`` (str, optional): The character used to terminate the row and move to a new line. Default is ``'\\r\\n'``.
-            ``na_rep`` (str, optional): String representation to use for null or missing values. Default is ``'None'``.
-            ``index`` (bool, optional): If True, includes the index in the CSV file; if False, excludes the index. Default is ``False``.
+            ``filename`` (str): The name of the CSV file to which the data will be written. Default is None, returning as raw literal.
+            ``delimiter`` (str, optional): The delimiter to use for separating values. Default is ','.
+            ``quotechar`` (str, optional): The character used to quote fields. Default is '"'.
+            ``lineterminator`` (str, optional): The character used to terminate the row and move to a new line. Default is '\\r\\n'.
+            ``na_rep`` (str, optional): String representation to use for null or missing values. Default is 'None'.
+            ``index`` (bool, optional): If True, includes the index in the CSV file; if False, excludes the index. Default is False.
             ``**kwargs``: Additional arguments to be passed to the ``csv.writer`` constructor.
 
         Returns:
             ``str`` | ``None``: If ``filename`` is None, returns the model as a delimited string literal, ``None`` if ``filename`` is provided, writing the model to the specified file as a CSV file.
 
         Example:
 
@@ -8016,27 +8014,27 @@
             display_headers = display_headers[:max_cols] # +1 to include accounted for column
             table_dynamic_newline = f""" {table_truncated_ellipses}\n"""
         else:
             table_dynamic_newline = """\n"""
         row_sep_concat = f"""|| '{row_sep}' ||"""
         fetch_idx = SQLDataModel.sqlite_printf_format(self.sql_idx,"index",header_length_dict[self.sql_idx]) + row_sep_concat if display_index else ""
         header_fmt_str = row_sep_concat.join([f"""{SQLDataModel.sqlite_printf_format(col,header_py_dtype_dict[col],header_length_dict[col],self.display_float_precision,alignment=column_alignment)}""" for col in display_headers if col != self.sql_idx])
-        vertical_sep_chars = '⠒⠂' # '⠐⠒⠂'
-        vertical_sep_fmt_str = row_sep_concat.join([f"""printf("%!{header_length_dict[col]}.{header_length_dict[col]}s", printf("%*s%s%*s", ({header_length_dict[col]}-2)/2, "", '{vertical_sep_chars}', ({header_length_dict[col]}-2)/2, ""))""" for col in display_headers])
         if vertical_truncation_required:
+            vertical_sep_chars = '⠒⠂'
+            vertical_sep_fmt_str = f'''{row_lh}{row_sep.join([f"""{vertical_sep_chars:^{max(0,header_length_dict[col]+1)}}"""[:header_length_dict[col]] for col in display_headers])}{row_rh}{table_dynamic_newline}'''
             fetch_fmt_stmt = f"""
             with "_repr" as (
                 select "{self.sql_idx}" as "_row" from "{self.sql_model}" where "{self.sql_idx}" in 
                     (select "{self.sql_idx}" from "{self.sql_model}" order by "{self.sql_idx}" asc limit {split_row}+1)
                         or "{self.sql_idx}" in
                     (select "{self.sql_idx}" from "{self.sql_model}" order by "{self.sql_idx}" desc limit {split_row})
                 order by "{self.sql_idx}" asc limit {max_display_rows}+1)
                 ,"_trigger" as (select "{self.sql_idx}" as "_sep" from "{self.sql_model}" order by "{self.sql_idx}" asc limit 1 offset {split_row})
             select CASE WHEN "{self.sql_idx}" <> (select "_sep" from "_trigger") THEN "_full_row" 
-            ELSE '{row_lh}' || {vertical_sep_fmt_str} ||'{row_rh}{table_dynamic_newline}' 
+            ELSE '{vertical_sep_fmt_str}' 
             END from (select "{self.sql_idx}",'{row_lh}' || {fetch_idx}{header_fmt_str}||'{row_rh}{table_dynamic_newline}' as "_full_row" from "{self.sql_model}" where "{self.sql_idx}" in (select "_row" from "_repr") order by "{self.sql_idx}" asc)"""
         else:
             fetch_fmt_stmt = f"""select '{row_lh}' || {fetch_idx}{header_fmt_str}||'{row_rh}{table_dynamic_newline}' as "_full_row" from "{self.sql_model}" order by "{self.sql_idx}" asc limit {max_display_rows}"""
         formatted_response = self.sql_db_conn.execute(fetch_fmt_stmt)
         if column_alignment is None: # dynamic alignment
             formatted_headers = [f"""{(col if len(col) <= header_length_dict[col] else f"{col[:(header_length_dict[col]-2)]}⠤⠄"):{'>' if header_py_dtype_dict[col] in ('int','float') else '<'}{header_length_dict[col]}}""" if col != self.sql_idx else f"""{' ':>{header_length_dict[col]}}"""for col in display_headers]
         else: # left, center, right alignment
```

### Comparing `sqldatamodel-0.4.0/src/SQLDataModel/StandardDeviation.py` & `sqldatamodel-0.4.1/src/SQLDataModel/StandardDeviation.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.0/src/SQLDataModel/converters.py` & `sqldatamodel-0.4.1/src/SQLDataModel/converters.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.0/src/SQLDataModel/demo.py` & `sqldatamodel-0.4.1/src/SQLDataModel/demo.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.0/src/SQLDataModel/exceptions.py` & `sqldatamodel-0.4.1/src/SQLDataModel/exceptions.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.0/src/SQLDataModel/extensions/str_utils.c` & `sqldatamodel-0.4.1/src/SQLDataModel/extensions/str_utils.c`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.0/src/SQLDataModel.egg-info/PKG-INFO` & `sqldatamodel-0.4.1/src/SQLDataModel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.4.0
+Version: 0.4.1
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
-Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package,polars2pandas,pandas2polars
+Keywords: SQL,ETL,dataframe,terminal-tables,pretty-print-tables,sql2sql,data-analysis,data-science,datamodel,extract,transform,load,web-scraping-tables,data-mining,html,html-table-parsing,apache-arrow,pyarrow,pyarrow-conversion,pyarrow-to-table,pyarrow-to-sql,pyarrow-to-csv,parquet-file-parsing,csv,csv-parsing,markdown,markdown-table-parsing,latex,latex-table-parsing,delimited,delimited-data-parsing,file-conversion,format-conversion,terminal-styling,table-styling,from-sqlite,to-sqlite,from-postgresql,to-postgresql,sql-to-sql,excel,xlsx-file,excel-to-sql,DataFrames,polars2pandas,pandas2polars
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `sqldatamodel-0.4.0/src/SQLDataModel.egg-info/SOURCES.txt` & `sqldatamodel-0.4.1/src/SQLDataModel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.0/tests/test_Future.py` & `sqldatamodel-0.4.1/tests/test_Future.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.0/tests/test_SQLDataModel.py` & `sqldatamodel-0.4.1/tests/test_SQLDataModel.py`

 * *Files identical despite different names*


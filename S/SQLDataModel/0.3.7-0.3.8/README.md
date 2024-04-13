# Comparing `tmp/SQLDataModel-0.3.7.tar.gz` & `tmp/SQLDataModel-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLDataModel-0.3.7.tar", last modified: Thu Apr 11 00:31:03 2024, max compression
+gzip compressed data, was "SQLDataModel-0.3.8.tar", last modified: Sat Apr 13 00:44:59 2024, max compression
```

## Comparing `SQLDataModel-0.3.7.tar` & `SQLDataModel-0.3.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 00:31:03.315938 SQLDataModel-0.3.7/
--rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 SQLDataModel-0.3.7/LICENSE
--rw-rw-rw-   0        0        0    27185 2024-04-11 00:31:03.309870 SQLDataModel-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0    25313 2024-04-01 18:33:13.000000 SQLDataModel-0.3.7/README.md
--rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 SQLDataModel-0.3.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-11 00:31:03.316454 SQLDataModel-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0     2400 2024-04-11 00:20:07.000000 SQLDataModel-0.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 00:31:01.955320 SQLDataModel-0.3.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-11 00:31:03.110437 SQLDataModel-0.3.7/src/SQLDataModel/
--rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 SQLDataModel-0.3.7/src/SQLDataModel/ANSIColor.py
--rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 SQLDataModel-0.3.7/src/SQLDataModel/HTMLParser.py
--rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 SQLDataModel-0.3.7/src/SQLDataModel/JSONEncoder.py
--rw-rw-rw-   0        0        0   563580 2024-04-11 00:29:49.000000 SQLDataModel-0.3.7/src/SQLDataModel/SQLDataModel.py
--rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 SQLDataModel-0.3.7/src/SQLDataModel/StandardDeviation.py
--rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 SQLDataModel-0.3.7/src/SQLDataModel/__init__.py
--rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 SQLDataModel-0.3.7/src/SQLDataModel/converters.py
--rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 SQLDataModel-0.3.7/src/SQLDataModel/demo.py
--rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 SQLDataModel-0.3.7/src/SQLDataModel/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-11 00:31:03.250402 SQLDataModel-0.3.7/src/SQLDataModel/extensions/
--rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 SQLDataModel-0.3.7/src/SQLDataModel/extensions/__init__.py
--rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 SQLDataModel-0.3.7/src/SQLDataModel/extensions/str_utils.c
-drwxrwxrwx   0        0        0        0 2024-04-11 00:31:03.304171 SQLDataModel-0.3.7/src/SQLDataModel.egg-info/
--rw-rw-rw-   0        0        0    27185 2024-04-11 00:31:01.000000 SQLDataModel-0.3.7/src/SQLDataModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2024-04-11 00:31:01.000000 SQLDataModel-0.3.7/src/SQLDataModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 00:31:01.000000 SQLDataModel-0.3.7/src/SQLDataModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-11 00:31:01.000000 SQLDataModel-0.3.7/src/SQLDataModel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-11 00:31:03.262889 SQLDataModel-0.3.7/tests/
--rw-rw-rw-   0        0        0    50768 2024-04-11 00:17:44.000000 SQLDataModel-0.3.7/tests/test_Future.py
--rw-rw-rw-   0        0        0    50763 2024-04-11 00:17:45.000000 SQLDataModel-0.3.7/tests/test_SQLDataModel.py
+drwxrwxrwx   0        0        0        0 2024-04-13 00:44:59.879810 SQLDataModel-0.3.8/
+-rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 SQLDataModel-0.3.8/LICENSE
+-rw-rw-rw-   0        0        0    27267 2024-04-13 00:44:59.875540 SQLDataModel-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0    25395 2024-04-12 01:46:49.000000 SQLDataModel-0.3.8/README.md
+-rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 SQLDataModel-0.3.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-13 00:44:59.880344 SQLDataModel-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     2400 2024-04-13 00:43:24.000000 SQLDataModel-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 00:44:58.584088 SQLDataModel-0.3.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-13 00:44:59.719915 SQLDataModel-0.3.8/src/SQLDataModel/
+-rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 SQLDataModel-0.3.8/src/SQLDataModel/ANSIColor.py
+-rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 SQLDataModel-0.3.8/src/SQLDataModel/HTMLParser.py
+-rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 SQLDataModel-0.3.8/src/SQLDataModel/JSONEncoder.py
+-rw-rw-rw-   0        0        0   586081 2024-04-13 00:44:13.000000 SQLDataModel-0.3.8/src/SQLDataModel/SQLDataModel.py
+-rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 SQLDataModel-0.3.8/src/SQLDataModel/StandardDeviation.py
+-rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 SQLDataModel-0.3.8/src/SQLDataModel/__init__.py
+-rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 SQLDataModel-0.3.8/src/SQLDataModel/converters.py
+-rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 SQLDataModel-0.3.8/src/SQLDataModel/demo.py
+-rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 SQLDataModel-0.3.8/src/SQLDataModel/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-13 00:44:59.831965 SQLDataModel-0.3.8/src/SQLDataModel/extensions/
+-rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 SQLDataModel-0.3.8/src/SQLDataModel/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 SQLDataModel-0.3.8/src/SQLDataModel/extensions/str_utils.c
+drwxrwxrwx   0        0        0        0 2024-04-13 00:44:59.871228 SQLDataModel-0.3.8/src/SQLDataModel.egg-info/
+-rw-rw-rw-   0        0        0    27267 2024-04-13 00:44:58.000000 SQLDataModel-0.3.8/src/SQLDataModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2024-04-13 00:44:58.000000 SQLDataModel-0.3.8/src/SQLDataModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 00:44:58.000000 SQLDataModel-0.3.8/src/SQLDataModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-13 00:44:58.000000 SQLDataModel-0.3.8/src/SQLDataModel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 00:44:59.841962 SQLDataModel-0.3.8/tests/
+-rw-rw-rw-   0        0        0    58321 2024-04-13 00:42:51.000000 SQLDataModel-0.3.8/tests/test_Future.py
+-rw-rw-rw-   0        0        0    58324 2024-04-13 00:42:52.000000 SQLDataModel-0.3.8/tests/test_SQLDataModel.py
```

### Comparing `SQLDataModel-0.3.7/LICENSE` & `SQLDataModel-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.7/PKG-INFO` & `SQLDataModel-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.3.7
+Version: 0.3.8
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package
@@ -497,14 +497,15 @@
 - **JSON**: Extract from and write to `.json` files, JSON-like objects, or JSON formatted sring literals.
 - **LaTeX**: Extract from and write to `.tex` files, LaTeX formatted string literals.
 - **Markdown**: Extract from and write to `.MD` files, Markdown formatted string literals.
 - **Numpy**: Convert to and from `numpy.ndarray` objects, `numpy` required.
 - **Pandas**: Convert to and from `pandas.DataFrame` objects, `pandas` required.
 - **Parquet**: Extract from and write to `.parquet` files, `pyarrow` required.
 - **Pickle**: Extract from and write to `.pkl` files, package uses `.sdm` extension when pickling for `SQLDataModel` metadata.
+- **Polars**: Convert to and from `polars.DataFrame` objects, `polars` required.
 - **SQL**: Extract from and write to the following popular SQL databases:
     - **SQLite**: Using the built-in `sqlite3` module.
     - **PostgreSQL**: Using the `psycopg2` package.
     - **SQL Server**: Using the `pyodbc` package.
     - **Oracle**: Using the `cx_Oracle` package.
     - **Teradata**: Using the `teradatasql` package.
 - **Text**: Write to and from `.txt` files including other `SQLDataModel` string representations.
```

### Comparing `SQLDataModel-0.3.7/README.md` & `SQLDataModel-0.3.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -472,14 +472,15 @@
 - **JSON**: Extract from and write to `.json` files, JSON-like objects, or JSON formatted sring literals.
 - **LaTeX**: Extract from and write to `.tex` files, LaTeX formatted string literals.
 - **Markdown**: Extract from and write to `.MD` files, Markdown formatted string literals.
 - **Numpy**: Convert to and from `numpy.ndarray` objects, `numpy` required.
 - **Pandas**: Convert to and from `pandas.DataFrame` objects, `pandas` required.
 - **Parquet**: Extract from and write to `.parquet` files, `pyarrow` required.
 - **Pickle**: Extract from and write to `.pkl` files, package uses `.sdm` extension when pickling for `SQLDataModel` metadata.
+- **Polars**: Convert to and from `polars.DataFrame` objects, `polars` required.
 - **SQL**: Extract from and write to the following popular SQL databases:
     - **SQLite**: Using the built-in `sqlite3` module.
     - **PostgreSQL**: Using the `psycopg2` package.
     - **SQL Server**: Using the `pyodbc` package.
     - **Oracle**: Using the `cx_Oracle` package.
     - **Teradata**: Using the `teradatasql` package.
 - **Text**: Write to and from `.txt` files including other `SQLDataModel` string representations.
```

### Comparing `SQLDataModel-0.3.7/setup.py` & `SQLDataModel-0.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='SQLDataModel',  
-     version='0.3.7',
+     version='0.3.8',
      scripts=['src/SQLDataModel/SQLDataModel.py'] ,
      author='Ante Tonkovic-Capin',
      author_email='antetc@icloud.com',
      description='SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.',
      keywords=['SQL','ETL','dataframe','terminal tables','pretty print tables','sql2sql','data analysis','data science','data model','extract','transform','load','web scraping tables','data mining','html','html table parsing','apache arrow','pyarrow','pyarrow conversion','pyarrow to table','pyarrow to sql','pyarrow to csv','parquet file parsing','csv','csv parsing','markdown','markdown table parsing','latex','latex table parsing','delimited','delimited data parsing','file conversion','format conversion','terminal styling','table styling','from sqlite','to sqlite','from postgresql','to postgresql','sql to sql','excel','xlsx file','excel to sql','DataFrame package'],
      license_file='LICENSE',
      long_description=long_description,
```

### Comparing `SQLDataModel-0.3.7/src/SQLDataModel/ANSIColor.py` & `SQLDataModel-0.3.8/src/SQLDataModel/ANSIColor.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.7/src/SQLDataModel/HTMLParser.py` & `SQLDataModel-0.3.8/src/SQLDataModel/HTMLParser.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.7/src/SQLDataModel/JSONEncoder.py` & `SQLDataModel-0.3.8/src/SQLDataModel/JSONEncoder.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.7/src/SQLDataModel/SQLDataModel.py` & `SQLDataModel-0.3.8/src/SQLDataModel/SQLDataModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,20 @@
 try:
     import pandas as _pd
     _has_pd = True
 except ModuleNotFoundError:
     _has_pd = False
 
 try:
+    import polars as _pl
+    _has_pl = True
+except ModuleNotFoundError:
+    _has_pl = False
+
+try:
     import pyarrow as _pa, pyarrow.parquet as _pq
     _has_pa = True
 except ModuleNotFoundError:
     _has_pa = False
 
 try:
     import openpyxl as _xl
@@ -180,14 +186,15 @@
         sdm = SQLDataModel.from_dict(py_dict)
         sdm = SQLDataModel.from_html("output.html")
         sdm = SQLDataModel.from_json("output.json")
         sdm = SQLDataModel.from_latex("output.tex")
         sdm = SQLDataModel.from_markdown("output.md")
         sdm = SQLDataModel.from_numpy(np_arr)
         sdm = SQLDataModel.from_pandas(pd_df)
+        sdm = SQLDataModel.from_polars(pl_df)
         sdm = SQLDataModel.from_parquet("output.parquet")
         sdm = SQLDataModel.from_pickle("output.sdm")
         sdm = SQLDataModel.from_sql("output", sqlite3.connect('output.db'))
     ```
     
     Data Formats
     ------------
@@ -201,14 +208,15 @@
         - ``JSON``: Extract from and write to ``.json`` files, JSON-like objects, or JSON formatted sring literals.
         - ``LaTeX``: Extract from and write to ``.tex`` files, LaTeX formatted string literals.
         - ``Markdown``: Extract from and write to ``.MD`` files, Markdown formatted string literals.
         - ``Numpy``: Convert to and from ``numpy.ndarray`` objects, ``numpy`` required.
         - ``Pandas``: Convert to and from ``pandas.DataFrame`` objects, ``pandas`` required.
         - ``Parquet``: Extract from and write to ``.parquet`` files, ``pyarrow`` required.
         - ``Pickle``: Extract from and write to ``.pkl`` files, package uses ``.sdm`` extension when pickling for ``SQLDataModel`` metadata.
+        - ``Polars``: Convert to and from ``polars.DataFrame`` objects, ``polars`` required.
         - ``SQL``: Extract from and write to the following popular SQL databases:
 
           - ``SQLite``: Using the built-in ``sqlite3`` module.
           - ``PostgreSQL``: Using the ``psycopg2`` package.
           - ``SQL Server``: Using the ``pyodbc`` package.
           - ``Oracle``: Using the ``cx_Oracle`` package.
           - ``Teradata``: Using the ``teradatasql`` package.
@@ -253,17 +261,17 @@
     ```
     Note:
         - No additional dependencies are installed with this package, however you will obviously need to have pandas or numpy to create pandas or numpy objects.
         - Use :meth:`SQLDataModel.set_display_color()` to modify the terminal color of the table, by default no color styling is applied.
         - Use :meth:`SQLDataModel.get_supported_sql_connections()` to view supported SQL connection packages, please reach out with any issues or questions, thanks!
 
     """
-    __slots__ = ('sql_idx','sql_model','display_max_rows','min_column_width','max_column_width','column_alignment','display_color','display_index','row_count','headers','column_count','static_py_to_sql_map_dict','static_sql_to_py_map_dict','sql_db_conn','display_float_precision','header_master','indicies','dtypes','shape')
+    __slots__ = ('sql_idx','sql_model','display_max_rows','min_column_width','max_column_width','column_alignment','display_color','display_index','row_count','headers','column_count','static_py_to_sql_map_dict','static_sql_to_py_map_dict','sql_db_conn','display_float_precision','header_master','indicies','dtypes','shape','table_style')
     
-    def __init__(self, data:list[list]=None, headers:list[str]=None, dtypes:dict[str,str]=None, display_max_rows:int=None, min_column_width:int=3, max_column_width:int=38, column_alignment:Literal['dynamic','left','center','right']='dynamic', display_color:str=None, display_index:bool=True, display_float_precision:int=2, infer_types:bool=False):
+    def __init__(self, data:list[list]=None, headers:list[str]=None, dtypes:dict[str,str]=None, display_max_rows:int=None, min_column_width:int=3, max_column_width:int=38, column_alignment:Literal['dynamic','left','center','right']='dynamic', display_color:str=None, display_index:bool=True, display_float_precision:int=2, infer_types:bool=False, table_style:Literal['ascii','bare','dash','default','double','markdown','outline','pandas','polars','postgresql','round','thick']='default'):
         """
         Initializes a new instance of ``SQLDataModel``.
 
         Parameters:
             ``data`` (list[list]): The data to populate the model. Should be a list of lists or a list of tuples.
             ``headers`` (list[str]): The column headers for the model. If not provided, default headers will be used.
             ``dtypes`` (dict): A dictionary specifying the data types for each column. Format: {'column': 'dtype'}.
@@ -411,14 +419,16 @@
         """``tuple[int, int]``: The current dimensions of the model as a tuple of ``(rows, columns)``."""
         self.display_color = ANSIColor(display_color) if isinstance(display_color, (str,tuple)) else display_color if isinstance(display_color,ANSIColor) else None
         """``ANSIColor``: The display color to use for string representations of the model. Default is ``None``, using the standard terminal color."""
         self.static_py_to_sql_map_dict = {'None': 'TEXT','int': 'INTEGER','float': 'REAL','str': 'TEXT','bytes': 'BLOB', 'date': 'DATE', 'datetime': 'TIMESTAMP', 'NoneType':'TEXT', 'bool':'INTEGER'}
         """``dict``: The data type mapping to use when converting python types to SQL column types."""
         self.static_sql_to_py_map_dict = {'NULL': 'None','INTEGER': 'int','REAL': 'float','TEXT': 'str','BLOB': 'bytes', 'DATE': 'date', 'TIMESTAMP': 'datetime','':'str'}
         """``dict``: The data type mapping to use when converting SQL column types to python types."""
+        self.table_style = table_style
+        """``str``: The table style used for string representations of the model. Available styles are ``'ascii'``, ``'bare'``, ``'dash'``, ``'default'``, ``'double'``, ``'markdown'``, ``'outline'``, ``'pandas'``, ``'polars'``, ``'postgresql'``, ``'round'`` or ``'thick'``. Defaults to ``'default'`` table style."""
         if infer_types and self.row_count > 0:
             inferred_dtypes = SQLDataModel.infer_types_from_data(input_data=random.sample(data, min(self.row_count, 16)))
             headers_to_py_dtypes_dict = {self.headers[i]:inferred_dtypes[i+dyn_idx_offset] for i in range(self.column_count)}
         else:
             headers_to_py_dtypes_dict = {self.headers[i]:type(data[0][i+dyn_idx_offset]).__name__ for i in range(self.column_count)}        
         if dtypes is not None:
             [(headers_to_py_dtypes_dict.__setitem__(col,dtype)) for col,dtype in dtypes.items() if col in self.headers and dtype in self.static_py_to_sql_map_dict]
@@ -2408,14 +2418,15 @@
             
         Constructor methods are called according to the input type:
             - ``dict``: If all values are python datatypes, passed as ``dtypes`` to constructor, otherwise as ``data`` to :meth:`SQLDataModel.from_dict()`.
             - ``list``: If single dimension, passed as ``headers`` to constructor, otherwise as ``data`` containing list of lists.
             - ``tuple``: Same as with list, if single dimension passed as ``headers``, otherwise as ``data`` containing tuple of lists.
             - ``numpy.ndarray``: passed to :meth:`SQLDataModel.from_numpy()` as array data.
             - ``pandas.DataFrame``: passed to :meth:`SQLDataModel.from_pandas()` as dataframe data.
+            - ``polars.DataFrame``: passed to :meth:`SQLDataModel.from_polars()` as dataframe data.
             - ``str``: If starts with 'http', passed to :meth:`SQLDataModel.from_html()` as url, otherwise:
         
               - ``'.csv'``: passed to :meth:`SQLDataModel.from_csv()` as csv source data.
               - ``'.html'``: passed to :meth:`SQLDataModel.from_html()` as html source data.
               - ``'.json'``: passed to :meth:`SQLDataModel.from_json()` as json source data.
               - ``'.md'``: passed to :meth:`SQLDataModel.from_markdown()` as markdown source data.
               - ``'.parquet'``: passed to :meth:`SQLDataModel.from_parquet()` as parquet source data.
@@ -2548,15 +2559,18 @@
                     return ext_operation['.json'](data, **kwargs)
             return cls.from_text(data, **kwargs)
         else:
             arg_type = type(data).__name__
             if arg_type == 'ndarray':
                 return cls.from_numpy(data, **kwargs)
             elif arg_type == 'DataFrame':
-                return cls.from_pandas(data, **kwargs)
+                if 'pandas' in type(data).__module__:
+                    return cls.from_pandas(data, **kwargs)
+                else:
+                    return cls.from_polars(data, **kwargs)
             elif arg_type == 'Table':
                 return cls.from_pyarrow(data, **kwargs)
             else:
                 raise TypeError(
                     SQLDataModel.ErrorFormat(f"TypeError: unsupported type '{arg_type}', current supported external types are 'numpy.ndarray' or 'pandas.DataFrame' objects")
                 )
     
@@ -3574,27 +3588,27 @@
                 SQLDataModel.ErrorFormat(f"DimensionError: invalid dimension '{obj_ndim}', argument for `array` must have 2 dimensions representing `(rows, columns)`")
             )
         return cls(data=array.tolist(),headers=headers, **kwargs)
 
     @classmethod
     def from_pandas(cls, df, headers:list[str]=None, **kwargs) -> SQLDataModel:
         """
-        Returns a ``SQLDataModel`` object created from the provided ``df`` representing a pandas ``DataFrame`` object. Note that ``pandas`` must be installed in order to use this class method.
+        Returns a ``SQLDataModel`` object created from the provided ``df`` representing a Pandas ``DataFrame`` object. Note that ``pandas`` must be installed in order to use this method.
 
         Parameters:
             ``df`` (pandas.DataFrame): The pandas DataFrame to convert to a SQLDataModel.
-            ``headers`` (list of str, optional): The list of headers to use for the SQLDataModel. If None, the columns of the DataFrame will be used. Default is None.
+            ``headers`` (list[str], optional): The list of headers to use for the SQLDataModel. Default is None, using the columns from the ``df`` object.
             ``**kwargs``: Additional arguments to be passed to the SQLDataModel constructor.
 
         Returns:
             ``SQLDataModel``: The SQLDataModel object created from the pandas DataFrame.
 
         Raises:
             ``ModuleNotFoundError``: If the required package ``pandas`` is not found.
-            ``TypeError``: If ``df`` argument is not of type 'pandas.DataFrame'.
+            ``TypeError``: If ``df`` argument is not of type ``pandas.DataFrame``.
 
         Example::
 
             import pandas as pd
             from SQLDataModel import SQLDataModel
 
             # Create a pandas DataFrame
@@ -3605,15 +3619,15 @@
 
         Note:
             - If ``headers`` are not provided, the existing pandas columns will be used as the new ``SQLDataModel`` headers.
 
         """
         if not _has_pd:
             raise ModuleNotFoundError(
-                SQLDataModel.ErrorFormat(f"""ModuleNotFoundError: required package not found, pandas must be installed in order to use the `from_pandas()` method""")
+                SQLDataModel.ErrorFormat(f"""ModuleNotFoundError: required package not found, Pandas must be installed in order to use the `from_pandas()` method""")
                 )
         if (obj_type := type(df).__name__) != 'DataFrame':
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: invalid type '{obj_type}', argument for `df` must be of type 'DataFrame'")
             )        
         data = [x[1:] for x in df.itertuples()]
         headers = df.columns.tolist() if headers is None else headers
@@ -3752,14 +3766,82 @@
                 SQLDataModel.ErrorFormat(f"FileNotFoundError: no such file or directory '{filename}', please ensure the filename exists and is a valid path")
                 ) from None            
         if kwargs:
             sdm_deserialized.update(**kwargs)
         return cls(**sdm_deserialized)
  
     @classmethod
+    def from_polars(cls, df, headers:list[str]=None, **kwargs) -> SQLDataModel:
+        """
+        Returns a ``SQLDataModel`` object created from the provided ``df`` representing a Polars ``DataFrame`` object. Note that ``polars`` must be installed in order to use this method.
+
+        Parameters:
+            ``df`` (polars.DataFrame): The Polars DataFrame to convert to a SQLDataModel.
+            ``headers`` (list[str], optional): The list of headers to use for the SQLDataModel. Default is None, using the columns from the ``df`` object.
+            ``**kwargs``: Additional arguments to be passed to the SQLDataModel constructor.
+
+        Returns:
+            ``SQLDataModel``: The SQLDataModel object created from the Polars DataFrame.
+
+        Raises:
+            ``ModuleNotFoundError``: If the required package ``polars`` is not found.
+            ``TypeError``: If ``df`` argument is not of type ``polars.DataFrame``.
+
+        Example::
+
+            import polars as pl
+            from SQLDataModel import SQLDataModel
+
+            # Sample data
+            data = {
+                'Name': ['Beth', 'John', 'Alice', 'Travis'], 
+                'Age': [27, 30, 28, 35], 
+                'Height': [172.4, 175.3, 162.0, 185.8]
+            }
+
+            # Create the polars DataFrame
+            df = pl.DataFrame(data)
+            
+            # Create a SQLDataModel object
+            sdm = SQLDataModel.from_polars(df)
+        
+            # View result
+            print(sdm)
+
+        This will output a ``SQLDataModel`` constructed from the Polars ``df``:
+
+        ```shell
+            ┌────────┬─────┬─────────┐
+            │ Name   │ Age │  Height │
+            ├────────┼─────┼─────────┤
+            │ Beth   │  27 │  172.40 │
+            │ John   │  30 │  175.30 │
+            │ Alice  │  28 │  162.00 │
+            │ Travis │  35 │  185.80 │
+            └────────┴─────┴─────────┘
+            [4 rows x 3 columns]
+        ```
+
+        Note:
+            - If ``headers`` are not provided, the columns from the provided DataFrame's columns will be used as the new ``SQLDataModel`` headers.
+            - Polars uses different data types than those used by ``SQLDataModel``, see :meth:`SQLDataModel.set_column_dtypes()` for specific casting rules.
+            - See related :meth:`SQLDataModel.to_polars()` for the inverse method of converting a ``SQLDataModel`` into a Polars ``DataFrame`` object.
+        """
+        if not _has_pl:
+            raise ModuleNotFoundError(
+                SQLDataModel.ErrorFormat(f"""ModuleNotFoundError: required package not found, Polars must be installed in order to use the `from_polars()` method""")
+                )
+        if (obj_type := type(df).__name__) != 'DataFrame':
+            raise TypeError(
+                SQLDataModel.ErrorFormat(f"TypeError: invalid type '{obj_type}', argument for `df` must be of type 'DataFrame'")
+            )        
+        return cls(data=df.rows(), headers=df.columns if headers is None else headers, **kwargs)
+
+
+    @classmethod
     def from_pyarrow(cls, table, **kwargs) -> SQLDataModel:
         """
         Returns a new ``SQLDataModel`` instance from the provided Apache Arrow object.
 
         Parameters:
             ``table`` (pyarrow.lib.Table): Apache Arrow object from which to construct a new ``SQLDataModel`` object.
             ``**kwargs``: Additional keyword arguments to pass to the SQLDataModel constructor.
@@ -5255,15 +5337,14 @@
         
         Change Log:
             - Version 0.3.0 (2024-03-31):
                 - Renamed ``include_index`` parameter to ``index`` for package consistency.
 
         Note:
             - SQLDataModel uses different data types than those used in ``pandas``, see :meth:`SQLDataModel.set_column_dtypes()` for more information about casting rules.
-
         """
         if not _has_pd:
             raise ModuleNotFoundError(
                 SQLDataModel.ErrorFormat(f"""ModuleNotFoundError: required package not found, pandas must be installed in order to use `.to_pandas()` method""")
                 )
         res = self.sql_db_conn.execute(self._generate_sql_stmt(index=index))
         raw_data = res.fetchall()
@@ -5394,14 +5475,80 @@
             if not isinstance(filename, str):
                 raise TypeError(
                     SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(filename).__name__}', argument for `filename` must be of type 'str' representing a valid pickle filepath")
                 )
         with open(filename, 'wb') as handle:
             pickle.dump(serialized_sdm, handle, protocol=pickle.HIGHEST_PROTOCOL)
 
+    def to_polars(self, index:bool=False, include_headers:bool=True) -> _pl.DataFrame:
+        """
+        Converts ``SQLDataModel`` to a Polars ``DataFrame`` object.
+        Note that the ``polars`` package must be installed to use this method.
+
+        Parameters:
+            ``index`` (bool, optional): If True, includes the model index in the result. Default is False.
+            ``include_headers`` (bool, optional): If True, includes column headers in the result. Default is True.
+
+        Raises:
+            ``ModuleNotFoundError``: If Polars is not installed.
+
+        Returns:
+            ``polars.DataFrame``: The model's data converted to a Polars DataFrame.
+        
+        Example::
+
+            import polars
+            from SQLDataModel import SQLDataModel
+
+            # Sample data
+            headers = ['Name', 'Age', 'Height']
+            data = [
+                ('Beth', 27, 172.4),
+                ('John', 30, 175.3), 
+                ('Alice', 28, 162.0), 
+                ('Travis', 35, 185.8)
+            ]
+
+            # Create the model
+            sdm = SQLDataModel(data, headers)
+
+            # Convert the model to a polars df with the index
+            df = sdm.to_polars(index=True)
+
+            # View result
+            print(df)
+
+        This will output:
+
+        ```shell
+            shape: (4, 4)
+            ┌─────┬────────┬─────┬────────┐
+            │ idx ┆ Name   ┆ Age ┆ Height │
+            │ --- ┆ ---    ┆ --- ┆ ---    │
+            │ i64 ┆ str    ┆ i64 ┆ f64    │
+            ╞═════╪════════╪═════╪════════╡
+            │ 0   ┆ Beth   ┆ 27  ┆ 172.4  │
+            │ 1   ┆ John   ┆ 30  ┆ 175.3  │
+            │ 2   ┆ Alice  ┆ 28  ┆ 162.0  │
+            │ 3   ┆ Travis ┆ 35  ┆ 185.8  │
+            └─────┴────────┴─────┴────────┘
+        ```
+
+        Note:
+            - See related :meth:`SQLDataModel.from_polars()` for the inverse method of converting a Polars ``DataFrame`` object into to a ``SQLDataModel``.
+            - SQLDataModel uses different data types than those used in ``polars``, see :meth:`SQLDataModel.set_column_dtypes()` for more information about casting rules.
+            - Polars does not really have a concept of an index column, therefore when using ``index=True``, the SQLDataModel index is just an additional column in the returned DataFrame object.
+        """
+        if not _has_pl:
+            raise ModuleNotFoundError(
+                SQLDataModel.ErrorFormat(f"""ModuleNotFoundError: required package not found, polars must be installed in order to use `.to_polars()` method""")
+                )
+        data = self.data(index=index, include_headers=include_headers)
+        return _pl.DataFrame(data=data[1:] if include_headers else data,schema=data[0] if include_headers else None)
+
     def to_pyarrow(self, index:bool=False) -> _pa.Table:
         """
         Returns the current ``SQLDataModel`` in Apache Arrow columnar format as a ``pyarrow.Table``.
 
         Parameters:
             ``index`` (bool, optional): Specifies whether to include the index of the SQLDataModel in the resulting Table. Default is to False.
 
@@ -7290,14 +7437,207 @@
 
         ```shell        
             1000
         ```
         """        
         return self.row_count
 
+    def set_table_style(self, style:Literal['ascii','bare','dash','default','double','markdown','outline','pandas','polars','postgresql','round','thick']='default') -> None:
+        """
+        Sets the table style used for string representations of ``SQLDataModel``.
+        
+        Parameters:
+            ``style`` (Literal['ascii','bare','dash','default','double','markdown','outline','pandas','polars','postgresql','round','thick']): The table styling to set, use ``'default'`` for original style.
+
+        Raises:
+            ``ValueError``: If ``style`` provided is not one of the currently supported options 'ascii','bare','dash','default','double','markdown','outline','pandas','polars','postgresql','round' or 'thick'.
+        
+        Returns:
+            ``None``
+
+        Examples::
+
+            from SQLDataModel import SQLDataModel
+
+            # Sample data
+            headers = ['Name', 'Age', 'Height', 'Birthday']
+            data = [
+                ('Alice', 28, 162.08, '1996-11-20'), 
+                ('Bobby', 30, 175.36, '1994-06-15'), 
+                ('Craig', 37, 185.82, '1987-01-07'),
+                ('David', 32, 179.75, '1992-12-28')
+            ]
+
+            # Create the model
+            sdm = SQLDataModel(data, headers)
+
+            # Lets try the round style
+            sdm.set_table_style('round')
+
+            # View it
+            print(sdm)
+
+        This outputs the ``'round'`` table style:
+
+        ```shell
+            ╭───────┬─────┬─────────┬────────────╮
+            │ Name  │ Age │  Height │ Birthday   │
+            ├───────┼─────┼─────────┼────────────┤
+            │ Alice │  28 │  162.08 │ 1996-11-20 │
+            │ Bobby │  30 │  175.36 │ 1994-06-15 │
+            │ Craig │  37 │  185.82 │ 1987-01-07 │
+            │ David │  32 │  179.75 │ 1992-12-28 │
+            ╰───────┴─────┴─────────┴────────────╯
+        ```
+
+        Alternatively, set ``style = 'ascii'`` to format ``SQLDataModel`` in the ASCII style, the OG of terminal tables:        
+
+        ```shell
+            +-------+-----+---------+------------+
+            | Name  | Age |  Height | Birthday   |
+            +-------+-----+---------+------------+
+            | Alice |  28 |  162.08 | 1996-11-20 |
+            | Bobby |  30 |  175.36 | 1994-06-15 |
+            | Craig |  37 |  185.82 | 1987-01-07 |
+            | David |  32 |  179.75 | 1992-12-28 |
+            +-------+-----+---------+------------+
+        ```
+
+        Set ``style = 'bare'`` to format ``SQLDataModel`` in the following style:
+
+        ```shell
+            Name   Age   Height  Birthday
+            -------------------------------
+            Alice   28   162.08  1996-11-20
+            Bobby   30   175.36  1994-06-15
+            Craig   37   185.82  1987-01-07
+            David   32   179.75  1992-12-28
+        ```
+
+        Set ``style = 'dash'`` to format ``SQLDataModel`` with dashes for internal borders:
+
+        ```shell
+            ┌───────┬─────┬─────────┬────────────┐
+            │ Name  ╎ Age ╎  Height ╎ Birthday   │
+            ├╴╴╴╴╴╴╴┼╴╴╴╴╴┼╴╴╴╴╴╴╴╴╴┼╴╴╴╴╴╴╴╴╴╴╴╴┤
+            │ Alice ╎  28 ╎  162.08 ╎ 1996-11-20 │
+            │ Bobby ╎  30 ╎  175.36 ╎ 1994-06-15 │
+            │ Craig ╎  37 ╎  185.82 ╎ 1987-01-07 │
+            │ David ╎  32 ╎  179.75 ╎ 1992-12-28 │
+            └───────┴─────┴─────────┴────────────┘
+        ```        
+
+        Set ``style = 'default'`` to format ``SQLDataModel`` in the following style, which also happens to be the default styling applied:
+
+        ```shell
+            ┌───────┬─────┬─────────┬────────────┐
+            │ Name  │ Age │  Height │ Birthday   │
+            ├───────┼─────┼─────────┼────────────┤
+            │ Alice │  28 │  162.08 │ 1996-11-20 │
+            │ Bobby │  30 │  175.36 │ 1994-06-15 │
+            │ Craig │  37 │  185.82 │ 1987-01-07 │
+            │ David │  32 │  179.75 │ 1992-12-28 │
+            └───────┴─────┴─────────┴────────────┘
+            [4 rows x 4 columns]
+        ```        
+
+        Set ``style = 'double'`` to format ``SQLDataModel`` using double line borders:
+
+        ```shell
+            ╔═══════╦═════╦═════════╦════════════╗
+            ║ Name  ║ Age ║  Height ║ Birthday   ║
+            ╠═══════╬═════╬═════════╬════════════╣
+            ║ Alice ║  28 ║  162.08 ║ 1996-11-20 ║
+            ║ Bobby ║  30 ║  175.36 ║ 1994-06-15 ║
+            ║ Craig ║  37 ║  185.82 ║ 1987-01-07 ║
+            ║ David ║  32 ║  179.75 ║ 1992-12-28 ║
+            ╚═══════╩═════╩═════════╩════════════╝
+        ```
+
+        Set ``style = 'markdown'`` to format ``SQLDataModel`` in the Markdown style:
+
+        ```shell
+            | Name  | Age |  Height | Birthday   |
+            |-------|-----|---------|------------|
+            | Alice |  28 |  162.08 | 1996-11-20 |
+            | Bobby |  30 |  175.36 | 1994-06-15 |
+            | Craig |  37 |  185.82 | 1987-01-07 |
+            | David |  32 |  179.75 | 1992-12-28 |
+        ```
+
+        Set ``style = 'outline'`` to format ``SQLDataModel`` in the following style:
+
+        ```shell
+            ┌─────────────────────────────────┐
+            │ Name   Age   Height  Birthday   │
+            ├─────────────────────────────────┤
+            │ Alice   28   162.08  1996-11-20 │
+            │ Bobby   30   175.36  1994-06-15 │
+            │ Craig   37   185.82  1987-01-07 │
+            │ David   32   179.75  1992-12-28 │
+            └─────────────────────────────────┘
+        ```
+
+        Set ``style = 'pandas'`` to format ``SQLDataModel`` in the style used by Pandas DataFrames:
+
+        ```shell
+            Name   Age   Height  Birthday
+            Alice   28   162.08  1996-11-20
+            Bobby   30   175.36  1994-06-15
+            Craig   37   185.82  1987-01-07
+            David   32   179.75  1992-12-28
+        ```
+
+        Set ``style = 'polars'`` to format ``SQLDataModel`` in the style used by Polars DataFrames:
+
+        ```shell
+            ┌───────┬─────┬─────────┬────────────┐
+            │ Name  ┆ Age ┆  Height ┆ Birthday   │
+            ╞═══════╪═════╪═════════╪════════════╡
+            │ Alice ┆  28 ┆  162.08 ┆ 1996-11-20 │
+            │ Bobby ┆  30 ┆  175.36 ┆ 1994-06-15 │
+            │ Craig ┆  37 ┆  185.82 ┆ 1987-01-07 │
+            │ David ┆  32 ┆  179.75 ┆ 1992-12-28 │
+            └───────┴─────┴─────────┴────────────┘
+        ```
+
+        Set ``style = 'postgresql'`` to format ``SQLDataModel`` in the style used by PostgreSQL:
+
+        ```shell
+            Name  | Age |  Height | Birthday
+            ------+-----+---------+-----------
+            Alice |  28 |  162.08 | 1996-11-20
+            Bobby |  30 |  175.36 | 1994-06-15
+            Craig |  37 |  185.82 | 1987-01-07
+            David |  32 |  179.75 | 1992-12-28
+        ```
+
+        Set ``style = 'thick'`` to format ``SQLDataModel`` using thick borders:
+
+        ```shell
+            ┏━━━━━━━┳━━━━━┳━━━━━━━━━┳━━━━━━━━━━━━┓
+            ┃ Name  ┃ Age ┃  Height ┃ Birthday   ┃
+            ┣━━━━━━━╋━━━━━╋━━━━━━━━━╋━━━━━━━━━━━━┫
+            ┃ Alice ┃  28 ┃  162.08 ┃ 1996-11-20 ┃
+            ┃ Bobby ┃  30 ┃  175.36 ┃ 1994-06-15 ┃
+            ┃ Craig ┃  37 ┃  185.82 ┃ 1987-01-07 ┃
+            ┃ David ┃  32 ┃  179.75 ┃ 1992-12-28 ┃
+            ┗━━━━━━━┻━━━━━┻━━━━━━━━━┻━━━━━━━━━━━━┛
+        ```
+
+        Note:
+            - The labels given to certain styles are entirely subjective and do not in any way express original design or ownership of the styling used.
+            - Legacy character sets on older terminals may not support all the character encodings required for some styles.
+        """
+        if style not in ('ascii','bare','dash','default','double','markdown','outline','pandas','polars','postgresql','round','thick'):
+            raise ValueError(
+                SQLDataModel.ErrorFormat(f"ValueError: invalid value '{style}', argument for `style` must be one of 'ascii', 'bare', 'dash', 'default', 'double', 'markdown', 'outline', 'pandas', 'polars', 'postgresql', 'round' or 'thick'")
+            )
+        self.table_style = style
+
     def __repr__(self) -> str:
         """
         Returns a formatted string representation of the SQLDataModel instance.
 
         Returns:
             ``str``: The string representation of the SQLDataModel instance with tabular formatting.
 
@@ -7405,14 +7745,26 @@
 
         Note:
             - The representation includes a truncated table view of the SQLDataModel.
             - The output adjusts column widths dynamically and provides ellipses if the table is truncated.
             - The number of displayed rows is limited to either the row count or the specified maximum rows.
             - The output includes column headers, row data, and information about the total number of rows and columns.
         """         
+        table_format = self._generate_table_style()
+        top_lh, top_hbar, top_sep, top_rh = table_format[0]
+        mid_lh, mid_hbar, mid_sep, mid_rh = table_format[1]
+        row_lh, row_sep, row_rh = table_format[2]
+        low_lh, low_hbar, low_sep, low_rh = table_format[3]
+        table_repr = """""" # big things...
+        row_lh_width = len(row_lh)
+        row_rh_width = len(row_rh)
+        row_sep_width = len(row_sep)
+        table_truncated_ellipses = """⠤⠄"""
+        table_truncated_ellipses_width = len(table_truncated_ellipses) + 1 # added extra space after truncation mark before ellipses, looks better
+        table_bare_newline = """\n"""
         total_available_width, total_available_height = shutil.get_terminal_size()
         display_max_rows = self.display_max_rows if self.display_max_rows is not None else (total_available_height - 6) if (total_available_height - 6 > 0) else 1
         vertical_truncation_required = display_max_rows < self.row_count
         max_display_rows = display_max_rows if vertical_truncation_required else self.row_count # max rows to display in repr
         split_row = max_display_rows // 2
         check_width_top = 6 # resolves to 13 rows to ceck from, 7 off top 6 off bottom
         check_width_bottom = (self.row_count-1) - check_width_top
@@ -7423,72 +7775,72 @@
         # header_printf_modifiers_dict = {col:(f"'% .{self.display_float_precision}f'" if dtype == 'float' else "'% d'" if dtype == 'int' else "'%!s'" if dtype != 'bytes' else "'b''%!s'''") for col,dtype in header_py_dtype_dict.items()}
         header_printf_modifiers_dict = {col:(f"'% .{self.display_float_precision}f'" if dtype == 'float' else "'%!s'" if dtype != 'bytes' else "'b''%!s'''") for col,dtype in header_py_dtype_dict.items()}
         headers_sub_select = " ".join(("select",f"""max(length("{self.sql_idx}")) as "{self.sql_idx}",""" if display_index else "",",".join([f"""max(max(length(printf({header_printf_modifiers_dict[col]},"{col}"))),length('{col}')) as "{col}" """ for col in display_headers if col != self.sql_idx]),f'from "{self.sql_model}" where "{self.sql_idx}" in (select "{self.sql_idx}" from "{self.sql_model}" where ("{self.sql_idx}" <= {check_width_top} or "{self.sql_idx}" > {check_width_bottom}) order by "{self.sql_idx}" asc limit 13)'))
         headers_parse_lengths_select = " ".join(("select",",".join([f"""min(max(ifnull("{col}",length('{col}')),{self.min_column_width}),{self.max_column_width})""" if col != self.sql_idx else f"""ifnull("{col}",1)""" for col in display_headers]),"from"))
         headers_full_select = f"""{headers_parse_lengths_select}({headers_sub_select})"""
         length_meta = self.sql_db_conn.execute(headers_full_select).fetchone()
         header_length_dict = {display_headers[i]:width for i, width in enumerate(length_meta)}
-        table_repr = """""" # big things...
-        table_left_edge = """│ """
-        table_left_edge_width = 2
-        table_right_edge = """ │"""
-        table_right_edge_width = 2
-        table_column_interval_width = 3
-        table_truncated_ellipses = """⠤⠄"""
-        table_truncated_ellipses_width = 3 # added extra space after truncation mark before ellipses, looks better
-        table_bare_newline = """\n"""
-        total_required_width = table_left_edge_width + sum((table_column_interval_width + length) for length in header_length_dict.values()) + table_right_edge_width - table_column_interval_width
+        total_required_width = row_lh_width + sum((row_sep_width + length) for length in header_length_dict.values()) + row_rh_width - row_sep_width
         table_truncation_required = False if total_available_width > total_required_width else True
         # print(f'truncation info: {total_required_width} of {total_available_width}, truncation: {table_truncation_required}')
         if table_truncation_required:
             total_available_width -= table_truncated_ellipses_width
-            max_cols, max_width = 0, (table_left_edge_width + table_right_edge_width + table_truncated_ellipses_width) # max width starts with the tax of index and border already included, around 5-7 depending on index width
+            max_cols, max_width = 0, (row_lh_width + row_rh_width + table_truncated_ellipses_width) # max width starts with the tax of index and border already included, around 5-7 depending on index width
             for v in header_length_dict.values():
                 if max_width < total_available_width:
                     max_width += (v+3)
                     max_cols += 1
                     continue
                 break
             if max_width > total_available_width:
                 max_cols -= 1
                 max_width -= (header_length_dict[display_headers[max_cols]] +3)
             display_headers = display_headers[:max_cols] # +1 to include accounted for column
             table_dynamic_newline = f""" {table_truncated_ellipses}\n"""
         else:
             table_dynamic_newline = """\n"""
-        vconcat_column_separator = """|| ' │ ' ||"""
-        fetch_idx = SQLDataModel.sqlite_printf_format(self.sql_idx,"index",header_length_dict[self.sql_idx]) + vconcat_column_separator if display_index else ""
-        header_fmt_str = vconcat_column_separator.join([f"""{SQLDataModel.sqlite_printf_format(col,header_py_dtype_dict[col],header_length_dict[col],self.display_float_precision,alignment=column_alignment)}""" for col in display_headers if col != self.sql_idx])
+        row_sep_concat = f"""|| '{row_sep}' ||"""
+        fetch_idx = SQLDataModel.sqlite_printf_format(self.sql_idx,"index",header_length_dict[self.sql_idx]) + row_sep_concat if display_index else ""
+        header_fmt_str = row_sep_concat.join([f"""{SQLDataModel.sqlite_printf_format(col,header_py_dtype_dict[col],header_length_dict[col],self.display_float_precision,alignment=column_alignment)}""" for col in display_headers if col != self.sql_idx])
         vertical_sep_chars = '⠒⠂' # '⠐⠒⠂'
-        vertical_sep_fmt_str = vconcat_column_separator.join([f"""printf("%!{header_length_dict[col]}.{header_length_dict[col]}s", printf("%*s%s%*s", ({header_length_dict[col]}-2)/2, "", '{vertical_sep_chars}', ({header_length_dict[col]}-2)/2, ""))""" for col in display_headers])
+        vertical_sep_fmt_str = row_sep_concat.join([f"""printf("%!{header_length_dict[col]}.{header_length_dict[col]}s", printf("%*s%s%*s", ({header_length_dict[col]}-2)/2, "", '{vertical_sep_chars}', ({header_length_dict[col]}-2)/2, ""))""" for col in display_headers])
         if vertical_truncation_required:
             fetch_fmt_stmt = f"""
             with "_repr" as (
                 select "{self.sql_idx}" as "_row" from "{self.sql_model}" where "{self.sql_idx}" in 
                     (select "{self.sql_idx}" from "{self.sql_model}" order by "{self.sql_idx}" asc limit {split_row}+1)
                         or "{self.sql_idx}" in
                     (select "{self.sql_idx}" from "{self.sql_model}" order by "{self.sql_idx}" desc limit {split_row})
                 order by "{self.sql_idx}" asc limit {max_display_rows}+1)
                 ,"_trigger" as (select "{self.sql_idx}" as "_sep" from "{self.sql_model}" order by "{self.sql_idx}" asc limit 1 offset {split_row})
             select CASE WHEN "{self.sql_idx}" <> (select "_sep" from "_trigger") THEN "_full_row" 
-            ELSE '{table_left_edge}' || {vertical_sep_fmt_str} ||' │{table_dynamic_newline}' 
-            END from (select "{self.sql_idx}",'{table_left_edge}' || {fetch_idx}{header_fmt_str}||' │{table_dynamic_newline}' as "_full_row" from "{self.sql_model}" where "{self.sql_idx}" in (select "_row" from "_repr") order by "{self.sql_idx}" asc)"""
+            ELSE '{row_lh}' || {vertical_sep_fmt_str} ||'{row_rh}{table_dynamic_newline}' 
+            END from (select "{self.sql_idx}",'{row_lh}' || {fetch_idx}{header_fmt_str}||'{row_rh}{table_dynamic_newline}' as "_full_row" from "{self.sql_model}" where "{self.sql_idx}" in (select "_row" from "_repr") order by "{self.sql_idx}" asc)"""
         else:
-            fetch_fmt_stmt = f"""select '{table_left_edge}' || {fetch_idx}{header_fmt_str}||' │{table_dynamic_newline}' as "_full_row" from "{self.sql_model}" order by "{self.sql_idx}" asc limit {max_display_rows}"""
+            fetch_fmt_stmt = f"""select '{row_lh}' || {fetch_idx}{header_fmt_str}||'{row_rh}{table_dynamic_newline}' as "_full_row" from "{self.sql_model}" order by "{self.sql_idx}" asc limit {max_display_rows}"""
         formatted_response = self.sql_db_conn.execute(fetch_fmt_stmt)
         if column_alignment is None: # dynamic alignment
             formatted_headers = [f"""{(col if len(col) <= header_length_dict[col] else f"{col[:(header_length_dict[col]-2)]}⠤⠄"):{'>' if header_py_dtype_dict[col] in ('int','float') else '<'}{header_length_dict[col]}}""" if col != self.sql_idx else f"""{' ':>{header_length_dict[col]}}"""for col in display_headers]
         else: # left, center, right alignment
             formatted_headers = [(f"""{col:{column_alignment}{header_length_dict[col]}}""" if len(col) <= header_length_dict[col] else f"""{col[:(header_length_dict[col]-2)]}⠤⠄""") if col != self.sql_idx else f"""{' ':>{header_length_dict[col]}}"""for col in display_headers]
-        table_cross_bar = """┌─""" + """─┬─""".join(["""─""" * header_length_dict[col] for col in display_headers]) + """─┐""" + table_bare_newline
-        table_repr = "".join([table_repr, table_cross_bar])
-        table_repr = "".join([table_repr, table_left_edge + """ │ """.join(formatted_headers) + table_right_edge + table_dynamic_newline])
-        table_repr = "".join([table_repr, table_cross_bar.replace("┌","├").replace("┬","┼").replace("┐","┤")])
+        # table_top_bar = "".join([top_lh, top_sep.join([top_hbar * header_length_dict[col] for col in display_headers]), top_rh, table_bare_newline])
+        col_lengths = [val for val in header_length_dict.values()]
+        table_top_bar = "".join([top_lh, top_sep.join([top_hbar * length for length in col_lengths]), top_rh, table_bare_newline])
+        table_top_bar = table_top_bar if len(table_top_bar.strip()) >=1 else """"""
+        table_repr = "".join([table_repr, table_top_bar])
+        table_repr = "".join([table_repr, row_lh, row_sep.join(formatted_headers), row_rh, table_dynamic_newline])
+        # table_mid_bar = "".join([mid_lh, mid_sep.join([mid_hbar * header_length_dict[col] for col in display_headers]), mid_rh, table_bare_newline])
+        table_mid_bar = "".join([mid_lh, mid_sep.join([mid_hbar * length for length in col_lengths]), mid_rh, table_bare_newline])
+        table_mid_bar = table_mid_bar if len(table_mid_bar.strip()) >=1 else """"""
+        table_repr = "".join([table_repr, table_mid_bar])
         table_repr = "".join([table_repr,*[row[0] for row in formatted_response]])
-        table_repr = "".join([table_repr, table_cross_bar.replace("┌","└").replace("┬","┴").replace("┐","┘")])
+        # table_low_bar = "".join([low_lh, low_sep.join([low_hbar * header_length_dict[col] for col in display_headers]), low_rh, table_bare_newline])
+        table_low_bar = "".join([low_lh, low_sep.join([low_hbar * length for length in col_lengths]), low_rh, table_bare_newline])
+        table_low_bar = table_low_bar if len(table_low_bar.strip()) >=1 else """"""
+        table_repr = "".join([table_repr, table_low_bar])
         table_caption = f"""[{self.row_count} rows x {self.column_count} columns]"""
         table_repr = "".join([table_repr, table_caption])
         return table_repr if self.display_color is None else self.display_color.wrap(table_repr)
     
 ##################################################################################################################
 ############################################## sqldatamodel methods ##############################################
 ##################################################################################################################
@@ -10131,14 +10483,90 @@
         if isinstance(columns,str):
             columns = [columns]
         columns_str = ",".join([f'"{col}"' for col in columns])
         ordering_str = f"""order by "{self.sql_idx}" {ordering}""" if ordering in ("asc","desc") else "order by random()"
         fetch_stmt = " ".join(("select",f'"{self.sql_idx}",' if index else '',columns_str,f'from "{self.sql_model}"', ordering_str, f"limit {n_rows}"))
         return fetch_stmt
 
+    def _generate_table_style(self) -> tuple[tuple[str]]:
+        """
+        Generates the character sets required for formatting ``SQLDataModel`` according to the value currently set at :py:attr:`SQLDataModel.table_style`.
+        
+        Returns:
+            ``tuple[tuple[str]]``: A 4-tuple containing the characters required for top, middle, row and lower table sections.
+        
+        Note:
+            - This method is called by :meth:`SQLDataModel.__repr__()` to parse the characters necessary for constructing the tabular representation of the ``SQLDataModel``, any modifications or changes to this method may result in unexpected behavior.
+        """
+        if self.table_style == 'ascii':    
+            return  (('+-','-','-+-','-+') 
+                    ,('+-','-','-+-','-+') 
+                    ,('| ',    ' | ',' |') 
+                    ,('+-','-','-+-','-+'))
+        if self.table_style == 'bare':     
+            return  (('','','','')
+                    ,('','-','--','')      
+                    ,('',    '  ','')      
+                    ,('','','',''))        
+        if self.table_style == 'dash': 
+            return  (('┌─','─','─┬─','─┐')
+                    ,('├╴','╴','╴┼╴','╴┤')
+                    ,('│ ',    ' ╎ ',' │')
+                    ,('└─','─','─┴─','─┘'))            
+        if self.table_style == 'default':  
+            return  (('┌─','─','─┬─','─┐') 
+                    ,('├─','─','─┼─','─┤') 
+                    ,('│ ',    ' │ ',' │') 
+                    ,('└─','─','─┴─','─┘'))
+        if self.table_style == 'double':   
+            return  (('╔═','═','═╦═','═╗') 
+                    ,('╠═','═','═╬═','═╣') 
+                    ,('║ ',    ' ║ ',' ║') 
+                    ,('╚═','═','═╩═','═╝'))
+        if self.table_style == 'markdown': 
+            return  (('','','','')
+                    ,('|-','-','-|-','-|')
+                    ,('| ',    ' | ',' |')
+                    ,('','','',''))
+        if self.table_style == 'outline':
+            return  (('┌─','─','──','─┐')
+                    ,('├─','─','──','─┤')
+                    ,('│ ',    '  ',' │')
+                    ,('└─','─','──','─┘'))
+        if self.table_style == 'pandas':
+            return  (('','','','')
+                    ,('','','','')
+                    ,('',    '  ','')
+                    ,('','','',''))
+        if self.table_style == 'polars':
+            return  (('┌─','─','─┬─','─┐')
+                    ,('╞═','═','═╪═','═╡')
+                    ,('│ ',    ' ┆ ',' │')
+                    ,('└─','─','─┴─','─┘'))
+        if self.table_style == 'postgresql':
+            return  (('','','','')
+                    ,('','-','-+-','')
+                    ,('',    ' | ','')
+                    ,('','','',''))
+        if self.table_style == 'round':
+            return  (('╭─','─','─┬─','─╮')
+                    ,('├─','─','─┼─','─┤')
+                    ,('│ ',    ' │ ',' │')
+                    ,('╰─','─','─┴─','─╯'))
+        if self.table_style == 'thick':
+            return  (('┏━','━','━┳━','━┓')
+                    ,('┣━','━','━╋━','━┫')
+                    ,('┃ ',    ' ┃ ',' ┃')
+                    ,('┗━','━','━┻━','━┛'))
+        else: # default styling
+            return  (('┌─','─','─┬─','─┐') 
+                    ,('├─','─','─┼─','─┤') 
+                    ,('│ ',    ' │ ',' │') 
+                    ,('└─','─','─┴─','─┘'))   
+
     def _update_indicies(self) -> None:
         """
         Updates the :py:attr:`SQLDataModel.indicies` and :py:attr:`SQLDataModel.row_count` properties of the ``SQLDataModel`` instance representing the current valid row indicies and count.
 
         Returns:
             ``None``
 
@@ -10324,16 +10752,17 @@
             - :py:attr:`SQLDataModel.display_max_rows`: The maximum number of rows to display.
             - :py:attr:`SQLDataModel.min_column_width`: The minimum width of columns when displaying the model.
             - :py:attr:`SQLDataModel.max_column_width`: The maximum width of columns when displaying the model.
             - :py:attr:`SQLDataModel.column_alignment`: The alignment of columns ('left', 'center', or 'right').
             - :py:attr:`SQLDataModel.display_color`: True if color formatting is enabled, False otherwise.
             - :py:attr:`SQLDataModel.display_index`: True if displaying index column, False otherwise.
             - :py:attr:`SQLDataModel.display_float_precision`: The precision for displaying floating-point numbers.
+            - :py:attr:`SQLDataModel.table_style`: The table styling format to use for strng representations of the model.
         """        
-        return {"display_max_rows":self.display_max_rows, "min_column_width":self.min_column_width, "max_column_width":self.max_column_width, "column_alignment":self.column_alignment, "display_color":self.display_color, "display_index":self.display_index, "display_float_precision":self.display_float_precision}
+        return {"display_max_rows":self.display_max_rows, "min_column_width":self.min_column_width, "max_column_width":self.max_column_width, "column_alignment":self.column_alignment, "display_color":self.display_color, "display_index":self.display_index, "display_float_precision":self.display_float_precision, "table_style":self.table_style}
 
     def validate_indicies(self, indicies) -> tuple[int|slice, list[str]]:
         """
         Validates and returns a predictable notation form of indices for accessing rows and columns in the ``SQLDataModel`` from varying indexing input types.
 
         Row indexing:
               - int: Single row index.
@@ -10607,8 +11036,8 @@
         if dtype not in ('bool','bytes','date','datetime','float','int','None','str'):
             raise ValueError(
                 SQLDataModel.ErrorFormat(f"ValueError: invalid value '{type(dtype).__name__}', argument for `dtype` must be one of 'bool','bytes','date','datetime','float','int','None' or 'str'")
             )        
         str_col_cast = ",".join([SQLDataModel.sqlite_cast_type_format(param=col, dtype=dtype, as_binding=False, as_alias=True) for col in self.headers])        
         sql_stmt = " ".join(("select",str_col_cast,f'from "{self.sql_model}"'))
         dtype_dict = {col:dtype for col in self.headers}
-        return self.execute_fetch(sql_stmt, dtypes=dtype_dict)    
+        return self.execute_fetch(sql_stmt, dtypes=dtype_dict)
```

### Comparing `SQLDataModel-0.3.7/src/SQLDataModel/StandardDeviation.py` & `SQLDataModel-0.3.8/src/SQLDataModel/StandardDeviation.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.7/src/SQLDataModel/converters.py` & `SQLDataModel-0.3.8/src/SQLDataModel/converters.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.7/src/SQLDataModel/demo.py` & `SQLDataModel-0.3.8/src/SQLDataModel/demo.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.7/src/SQLDataModel/exceptions.py` & `SQLDataModel-0.3.8/src/SQLDataModel/exceptions.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.7/src/SQLDataModel/extensions/str_utils.c` & `SQLDataModel-0.3.8/src/SQLDataModel/extensions/str_utils.c`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.7/src/SQLDataModel.egg-info/PKG-INFO` & `SQLDataModel-0.3.8/src/SQLDataModel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.3.7
+Version: 0.3.8
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package
@@ -497,14 +497,15 @@
 - **JSON**: Extract from and write to `.json` files, JSON-like objects, or JSON formatted sring literals.
 - **LaTeX**: Extract from and write to `.tex` files, LaTeX formatted string literals.
 - **Markdown**: Extract from and write to `.MD` files, Markdown formatted string literals.
 - **Numpy**: Convert to and from `numpy.ndarray` objects, `numpy` required.
 - **Pandas**: Convert to and from `pandas.DataFrame` objects, `pandas` required.
 - **Parquet**: Extract from and write to `.parquet` files, `pyarrow` required.
 - **Pickle**: Extract from and write to `.pkl` files, package uses `.sdm` extension when pickling for `SQLDataModel` metadata.
+- **Polars**: Convert to and from `polars.DataFrame` objects, `polars` required.
 - **SQL**: Extract from and write to the following popular SQL databases:
     - **SQLite**: Using the built-in `sqlite3` module.
     - **PostgreSQL**: Using the `psycopg2` package.
     - **SQL Server**: Using the `pyodbc` package.
     - **Oracle**: Using the `cx_Oracle` package.
     - **Teradata**: Using the `teradatasql` package.
 - **Text**: Write to and from `.txt` files including other `SQLDataModel` string representations.
```

### Comparing `SQLDataModel-0.3.7/src/SQLDataModel.egg-info/SOURCES.txt` & `SQLDataModel-0.3.8/src/SQLDataModel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.7/tests/test_Future.py` & `SQLDataModel-0.3.8/tests/test_Future.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime, os, tempfile, csv, sqlite3, random
 import pytest
 import pandas as pd
+import polars as pl
 import numpy as np
 from .random_data_generator import data_generator
 from future.SQLDataModel_future import SQLDataModel
 
 @pytest.fixture
 def sample_data() -> tuple[list[list], list[str]]:
     """Returns sample data in format `(data, headers)` to use for testing."""
@@ -463,14 +464,23 @@
     input_headers, input_data = ['A','B','C','D'], [(1, 'foo', 4.5, datetime.date(1999, 11, 9)),(2, 'bar', 6.7, datetime.date(2024, 8, 24)),(3, 'baz', 8.9, datetime.date(1985, 1, 13))]
     df_in = pd.DataFrame(data=input_data,columns=input_headers)
     df_out = SQLDataModel.from_pandas(df_in).to_pandas()
     for i in range(len(df_in.index)):
         assert df_out.iloc[i].tolist() == df_in.iloc[i].tolist()     
 
 @pytest.mark.ext
+def test_to_from_polars():
+    input_headers, input_data = ['A','B','C','D'], [(1, 'foo', 4.5, datetime.date(1999, 11, 9)),(2, 'bar', 6.7, datetime.date(2024, 8, 24)),(3, 'baz', 8.9, datetime.date(1985, 1, 13))]
+    df_in = pl.DataFrame(data=input_data,schema=input_headers)
+    df_out = SQLDataModel.from_polars(df_in).to_polars()
+    output_data, output_headers = df_out.rows(), df_out.columns
+    assert output_headers == input_headers
+    assert output_data == input_data
+
+@pytest.mark.ext
 def test_to_from_numpy():
     input_data = [('1', 'foo', '4.5', '1999-11-09'),('2', 'bar', '6.7', '2024-08-24'),('3', 'baz', '8.9', '1985-01-13')]
     sdm = SQLDataModel(input_data)
     output_data = SQLDataModel.from_numpy(sdm.to_numpy()).data()
     for i in range(len(input_data)):
         assert output_data[i] == input_data[i]
         
@@ -797,8 +807,149 @@
 
 @pytest.mark.core
 def test_mean():
     data = [('QNkrwWcsJnL', -633, 996.8432, 1, datetime.date(1962, 6, 7), b'3S7Z8ZcCeSc', datetime.datetime(1948, 10, 13, 9, 42, 47), 'waRB660S'), ('C5', -380, -585.4195, 1, datetime.date(1944, 9, 6), b'VceF78VXuWI', datetime.datetime(2020, 4, 23, 20, 14, 56), 'rABpuXdI'), ('FfeWNVq', -378, 575.8778, 0, datetime.date(1998, 3, 3), b'YyPoUKrPK', datetime.datetime(1958, 4, 18, 3, 11, 46), 'j2lb'), ('Xx', -744, 972.1331, 1, datetime.date(1994, 1, 19), b'PJyDr', datetime.datetime(2022, 12, 17, 14, 49, 10), 'KpWirYfv'), ('SuzgO', -627, 332.6614, 1, datetime.date(2011, 9, 14), b'b9', datetime.datetime(1922, 2, 25, 23, 23, 58), 'WM1VHoJ25zf'), ('69UEuh0', -954, -906.1676, 1, datetime.date(1980, 7, 26), b'PYesip__', datetime.datetime(1954, 8, 5, 4, 38, 33), 'jUWRBAyJXV')]    
     expected_data = ('NaN', -619.3333333333334, 230.98806666666667, 0.8333333333333334, datetime.date(1981, 12, 7), 'NaN', datetime.datetime(1971, 3, 8, 16, 40, 11), 'NaN')
     output_data = SQLDataModel(data).mean().data()
     assert output_data == expected_data
-    
+
+@pytest.mark.core
+def test_table_styles():
+    style_output_dict = {
+'ascii':"""
++---+--------+-----+-------+------------+
+|   | string | int | float | date       |
++---+--------+-----+-------+------------+
+| 0 | text 1 |   1 |  1.10 | 2001-01-11 |
+| 1 | text 2 |   2 |  2.20 | 2002-02-12 |
+| 2 | text 3 |   3 |  3.30 | 2003-03-13 |
+| 3 | text 4 |   4 |  4.40 | 2004-04-14 |
++---+--------+-----+-------+------------+
+[4 rows x 4 columns]
+""",
+'bare':"""
+   string  int  float  date      
+---------------------------------
+0  text 1    1   1.10  2001-01-11
+1  text 2    2   2.20  2002-02-12
+2  text 3    3   3.30  2003-03-13
+3  text 4    4   4.40  2004-04-14
+[4 rows x 4 columns]
+""",
+'dash':"""
+┌───┬────────┬─────┬───────┬────────────┐
+│   ╎ string ╎ int ╎ float ╎ date       │
+├╴╴╴┼╴╴╴╴╴╴╴╴┼╴╴╴╴╴┼╴╴╴╴╴╴╴┼╴╴╴╴╴╴╴╴╴╴╴╴┤
+│ 0 ╎ text 1 ╎   1 ╎  1.10 ╎ 2001-01-11 │
+│ 1 ╎ text 2 ╎   2 ╎  2.20 ╎ 2002-02-12 │
+│ 2 ╎ text 3 ╎   3 ╎  3.30 ╎ 2003-03-13 │
+│ 3 ╎ text 4 ╎   4 ╎  4.40 ╎ 2004-04-14 │
+└───┴────────┴─────┴───────┴────────────┘
+[4 rows x 4 columns]
+""",
+'default':"""
+┌───┬────────┬─────┬───────┬────────────┐
+│   │ string │ int │ float │ date       │
+├───┼────────┼─────┼───────┼────────────┤
+│ 0 │ text 1 │   1 │  1.10 │ 2001-01-11 │
+│ 1 │ text 2 │   2 │  2.20 │ 2002-02-12 │
+│ 2 │ text 3 │   3 │  3.30 │ 2003-03-13 │
+│ 3 │ text 4 │   4 │  4.40 │ 2004-04-14 │
+└───┴────────┴─────┴───────┴────────────┘
+[4 rows x 4 columns]
+""",
+'double':"""
+╔═══╦════════╦═════╦═══════╦════════════╗
+║   ║ string ║ int ║ float ║ date       ║
+╠═══╬════════╬═════╬═══════╬════════════╣
+║ 0 ║ text 1 ║   1 ║  1.10 ║ 2001-01-11 ║
+║ 1 ║ text 2 ║   2 ║  2.20 ║ 2002-02-12 ║
+║ 2 ║ text 3 ║   3 ║  3.30 ║ 2003-03-13 ║
+║ 3 ║ text 4 ║   4 ║  4.40 ║ 2004-04-14 ║
+╚═══╩════════╩═════╩═══════╩════════════╝
+[4 rows x 4 columns]
+""",
+'markdown':"""
+|   | string | int | float | date       |
+|---|--------|-----|-------|------------|
+| 0 | text 1 |   1 |  1.10 | 2001-01-11 |
+| 1 | text 2 |   2 |  2.20 | 2002-02-12 |
+| 2 | text 3 |   3 |  3.30 | 2003-03-13 |
+| 3 | text 4 |   4 |  4.40 | 2004-04-14 |
+[4 rows x 4 columns]
+""",
+'outline':"""
+┌───────────────────────────────────┐
+│    string  int  float  date       │
+├───────────────────────────────────┤
+│ 0  text 1    1   1.10  2001-01-11 │
+│ 1  text 2    2   2.20  2002-02-12 │
+│ 2  text 3    3   3.30  2003-03-13 │
+│ 3  text 4    4   4.40  2004-04-14 │
+└───────────────────────────────────┘
+[4 rows x 4 columns]
+""",
+'pandas':"""
+   string  int  float  date      
+0  text 1    1   1.10  2001-01-11
+1  text 2    2   2.20  2002-02-12
+2  text 3    3   3.30  2003-03-13
+3  text 4    4   4.40  2004-04-14
+[4 rows x 4 columns]
+""",
+
+'polars':"""
+┌───┬────────┬─────┬───────┬────────────┐
+│   ┆ string ┆ int ┆ float ┆ date       │
+╞═══╪════════╪═════╪═══════╪════════════╡
+│ 0 ┆ text 1 ┆   1 ┆  1.10 ┆ 2001-01-11 │
+│ 1 ┆ text 2 ┆   2 ┆  2.20 ┆ 2002-02-12 │
+│ 2 ┆ text 3 ┆   3 ┆  3.30 ┆ 2003-03-13 │
+│ 3 ┆ text 4 ┆   4 ┆  4.40 ┆ 2004-04-14 │
+└───┴────────┴─────┴───────┴────────────┘
+[4 rows x 4 columns]
+""",
+'postgresql':"""
+  | string | int | float | date      
+--+--------+-----+-------+-----------
+0 | text 1 |   1 |  1.10 | 2001-01-11
+1 | text 2 |   2 |  2.20 | 2002-02-12
+2 | text 3 |   3 |  3.30 | 2003-03-13
+3 | text 4 |   4 |  4.40 | 2004-04-14
+[4 rows x 4 columns]
+""",
+'round':"""
+╭───┬────────┬─────┬───────┬────────────╮
+│   │ string │ int │ float │ date       │
+├───┼────────┼─────┼───────┼────────────┤
+│ 0 │ text 1 │   1 │  1.10 │ 2001-01-11 │
+│ 1 │ text 2 │   2 │  2.20 │ 2002-02-12 │
+│ 2 │ text 3 │   3 │  3.30 │ 2003-03-13 │
+│ 3 │ text 4 │   4 │  4.40 │ 2004-04-14 │
+╰───┴────────┴─────┴───────┴────────────╯
+[4 rows x 4 columns]
+""",
+'thick':"""
+┏━━━┳━━━━━━━━┳━━━━━┳━━━━━━━┳━━━━━━━━━━━━┓
+┃   ┃ string ┃ int ┃ float ┃ date       ┃
+┣━━━╋━━━━━━━━╋━━━━━╋━━━━━━━╋━━━━━━━━━━━━┫
+┃ 0 ┃ text 1 ┃   1 ┃  1.10 ┃ 2001-01-11 ┃
+┃ 1 ┃ text 2 ┃   2 ┃  2.20 ┃ 2002-02-12 ┃
+┃ 2 ┃ text 3 ┃   3 ┃  3.30 ┃ 2003-03-13 ┃
+┃ 3 ┃ text 4 ┃   4 ┃  4.40 ┃ 2004-04-14 ┃
+┗━━━┻━━━━━━━━┻━━━━━┻━━━━━━━┻━━━━━━━━━━━━┛
+[4 rows x 4 columns]
+"""}
+    headers = ['string', 'int', 'float', 'date']
+    data = [
+         ('text 1',  1, 1.1, datetime.date(2001, 1, 11))
+        ,('text 2', 2, 2.2, datetime.date(2002, 2, 12))
+        ,('text 3', 3, 3.3, datetime.date(2003, 3, 13))
+        ,('text 4', 4, 4.4, datetime.date(2004, 4, 14))
+    ]
+    sdm = SQLDataModel(data,headers, min_column_width=3, max_column_width=38, display_index=True, display_float_precision=2)
+    repr_styles = ['ascii','bare','dash','default','double','markdown','outline','pandas','polars','postgresql','round','thick']   
+    for style in repr_styles:
+        sdm.set_table_style(style=style)
+        expected_repr = style_output_dict[style].strip('\n')
+        output_repr = sdm.__repr__()
+        assert output_repr == expected_repr
```

### Comparing `SQLDataModel-0.3.7/tests/test_SQLDataModel.py` & `SQLDataModel-0.3.8/tests/test_SQLDataModel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime, os, tempfile, csv, sqlite3, random
 import pytest
 import pandas as pd
+import polars as pl
 import numpy as np
 from .random_data_generator import data_generator
 from src.SQLDataModel.SQLDataModel import SQLDataModel
 
 @pytest.fixture
 def sample_data() -> tuple[list[list], list[str]]:
     """Returns sample data in format `(data, headers)` to use for testing."""
@@ -463,14 +464,23 @@
     input_headers, input_data = ['A','B','C','D'], [(1, 'foo', 4.5, datetime.date(1999, 11, 9)),(2, 'bar', 6.7, datetime.date(2024, 8, 24)),(3, 'baz', 8.9, datetime.date(1985, 1, 13))]
     df_in = pd.DataFrame(data=input_data,columns=input_headers)
     df_out = SQLDataModel.from_pandas(df_in).to_pandas()
     for i in range(len(df_in.index)):
         assert df_out.iloc[i].tolist() == df_in.iloc[i].tolist()     
 
 @pytest.mark.ext
+def test_to_from_polars():
+    input_headers, input_data = ['A','B','C','D'], [(1, 'foo', 4.5, datetime.date(1999, 11, 9)),(2, 'bar', 6.7, datetime.date(2024, 8, 24)),(3, 'baz', 8.9, datetime.date(1985, 1, 13))]
+    df_in = pl.DataFrame(data=input_data,schema=input_headers)
+    df_out = SQLDataModel.from_polars(df_in).to_polars()
+    output_data, output_headers = df_out.rows(), df_out.columns
+    assert output_headers == input_headers
+    assert output_data == input_data
+
+@pytest.mark.ext
 def test_to_from_numpy():
     input_data = [('1', 'foo', '4.5', '1999-11-09'),('2', 'bar', '6.7', '2024-08-24'),('3', 'baz', '8.9', '1985-01-13')]
     sdm = SQLDataModel(input_data)
     output_data = SQLDataModel.from_numpy(sdm.to_numpy()).data()
     for i in range(len(input_data)):
         assert output_data[i] == input_data[i]
         
@@ -796,8 +806,150 @@
     assert output_data == expected_data    
 
 @pytest.mark.core
 def test_mean():
     data = [('QNkrwWcsJnL', -633, 996.8432, 1, datetime.date(1962, 6, 7), b'3S7Z8ZcCeSc', datetime.datetime(1948, 10, 13, 9, 42, 47), 'waRB660S'), ('C5', -380, -585.4195, 1, datetime.date(1944, 9, 6), b'VceF78VXuWI', datetime.datetime(2020, 4, 23, 20, 14, 56), 'rABpuXdI'), ('FfeWNVq', -378, 575.8778, 0, datetime.date(1998, 3, 3), b'YyPoUKrPK', datetime.datetime(1958, 4, 18, 3, 11, 46), 'j2lb'), ('Xx', -744, 972.1331, 1, datetime.date(1994, 1, 19), b'PJyDr', datetime.datetime(2022, 12, 17, 14, 49, 10), 'KpWirYfv'), ('SuzgO', -627, 332.6614, 1, datetime.date(2011, 9, 14), b'b9', datetime.datetime(1922, 2, 25, 23, 23, 58), 'WM1VHoJ25zf'), ('69UEuh0', -954, -906.1676, 1, datetime.date(1980, 7, 26), b'PYesip__', datetime.datetime(1954, 8, 5, 4, 38, 33), 'jUWRBAyJXV')]    
     expected_data = ('NaN', -619.3333333333334, 230.98806666666667, 0.8333333333333334, datetime.date(1981, 12, 7), 'NaN', datetime.datetime(1971, 3, 8, 16, 40, 11), 'NaN')
     output_data = SQLDataModel(data).mean().data()
-    assert output_data == expected_data
+    assert output_data == expected_data
+
+@pytest.mark.core
+def test_table_styles():
+    style_output_dict = {
+'ascii':"""
++---+--------+-----+-------+------------+
+|   | string | int | float | date       |
++---+--------+-----+-------+------------+
+| 0 | text 1 |   1 |  1.10 | 2001-01-11 |
+| 1 | text 2 |   2 |  2.20 | 2002-02-12 |
+| 2 | text 3 |   3 |  3.30 | 2003-03-13 |
+| 3 | text 4 |   4 |  4.40 | 2004-04-14 |
++---+--------+-----+-------+------------+
+[4 rows x 4 columns]
+""",
+'bare':"""
+   string  int  float  date      
+---------------------------------
+0  text 1    1   1.10  2001-01-11
+1  text 2    2   2.20  2002-02-12
+2  text 3    3   3.30  2003-03-13
+3  text 4    4   4.40  2004-04-14
+[4 rows x 4 columns]
+""",
+'dash':"""
+┌───┬────────┬─────┬───────┬────────────┐
+│   ╎ string ╎ int ╎ float ╎ date       │
+├╴╴╴┼╴╴╴╴╴╴╴╴┼╴╴╴╴╴┼╴╴╴╴╴╴╴┼╴╴╴╴╴╴╴╴╴╴╴╴┤
+│ 0 ╎ text 1 ╎   1 ╎  1.10 ╎ 2001-01-11 │
+│ 1 ╎ text 2 ╎   2 ╎  2.20 ╎ 2002-02-12 │
+│ 2 ╎ text 3 ╎   3 ╎  3.30 ╎ 2003-03-13 │
+│ 3 ╎ text 4 ╎   4 ╎  4.40 ╎ 2004-04-14 │
+└───┴────────┴─────┴───────┴────────────┘
+[4 rows x 4 columns]
+""",
+'default':"""
+┌───┬────────┬─────┬───────┬────────────┐
+│   │ string │ int │ float │ date       │
+├───┼────────┼─────┼───────┼────────────┤
+│ 0 │ text 1 │   1 │  1.10 │ 2001-01-11 │
+│ 1 │ text 2 │   2 │  2.20 │ 2002-02-12 │
+│ 2 │ text 3 │   3 │  3.30 │ 2003-03-13 │
+│ 3 │ text 4 │   4 │  4.40 │ 2004-04-14 │
+└───┴────────┴─────┴───────┴────────────┘
+[4 rows x 4 columns]
+""",
+'double':"""
+╔═══╦════════╦═════╦═══════╦════════════╗
+║   ║ string ║ int ║ float ║ date       ║
+╠═══╬════════╬═════╬═══════╬════════════╣
+║ 0 ║ text 1 ║   1 ║  1.10 ║ 2001-01-11 ║
+║ 1 ║ text 2 ║   2 ║  2.20 ║ 2002-02-12 ║
+║ 2 ║ text 3 ║   3 ║  3.30 ║ 2003-03-13 ║
+║ 3 ║ text 4 ║   4 ║  4.40 ║ 2004-04-14 ║
+╚═══╩════════╩═════╩═══════╩════════════╝
+[4 rows x 4 columns]
+""",
+'markdown':"""
+|   | string | int | float | date       |
+|---|--------|-----|-------|------------|
+| 0 | text 1 |   1 |  1.10 | 2001-01-11 |
+| 1 | text 2 |   2 |  2.20 | 2002-02-12 |
+| 2 | text 3 |   3 |  3.30 | 2003-03-13 |
+| 3 | text 4 |   4 |  4.40 | 2004-04-14 |
+[4 rows x 4 columns]
+""",
+'outline':"""
+┌───────────────────────────────────┐
+│    string  int  float  date       │
+├───────────────────────────────────┤
+│ 0  text 1    1   1.10  2001-01-11 │
+│ 1  text 2    2   2.20  2002-02-12 │
+│ 2  text 3    3   3.30  2003-03-13 │
+│ 3  text 4    4   4.40  2004-04-14 │
+└───────────────────────────────────┘
+[4 rows x 4 columns]
+""",
+'pandas':"""
+   string  int  float  date      
+0  text 1    1   1.10  2001-01-11
+1  text 2    2   2.20  2002-02-12
+2  text 3    3   3.30  2003-03-13
+3  text 4    4   4.40  2004-04-14
+[4 rows x 4 columns]
+""",
+
+'polars':"""
+┌───┬────────┬─────┬───────┬────────────┐
+│   ┆ string ┆ int ┆ float ┆ date       │
+╞═══╪════════╪═════╪═══════╪════════════╡
+│ 0 ┆ text 1 ┆   1 ┆  1.10 ┆ 2001-01-11 │
+│ 1 ┆ text 2 ┆   2 ┆  2.20 ┆ 2002-02-12 │
+│ 2 ┆ text 3 ┆   3 ┆  3.30 ┆ 2003-03-13 │
+│ 3 ┆ text 4 ┆   4 ┆  4.40 ┆ 2004-04-14 │
+└───┴────────┴─────┴───────┴────────────┘
+[4 rows x 4 columns]
+""",
+'postgresql':"""
+  | string | int | float | date      
+--+--------+-----+-------+-----------
+0 | text 1 |   1 |  1.10 | 2001-01-11
+1 | text 2 |   2 |  2.20 | 2002-02-12
+2 | text 3 |   3 |  3.30 | 2003-03-13
+3 | text 4 |   4 |  4.40 | 2004-04-14
+[4 rows x 4 columns]
+""",
+'round':"""
+╭───┬────────┬─────┬───────┬────────────╮
+│   │ string │ int │ float │ date       │
+├───┼────────┼─────┼───────┼────────────┤
+│ 0 │ text 1 │   1 │  1.10 │ 2001-01-11 │
+│ 1 │ text 2 │   2 │  2.20 │ 2002-02-12 │
+│ 2 │ text 3 │   3 │  3.30 │ 2003-03-13 │
+│ 3 │ text 4 │   4 │  4.40 │ 2004-04-14 │
+╰───┴────────┴─────┴───────┴────────────╯
+[4 rows x 4 columns]
+""",
+'thick':"""
+┏━━━┳━━━━━━━━┳━━━━━┳━━━━━━━┳━━━━━━━━━━━━┓
+┃   ┃ string ┃ int ┃ float ┃ date       ┃
+┣━━━╋━━━━━━━━╋━━━━━╋━━━━━━━╋━━━━━━━━━━━━┫
+┃ 0 ┃ text 1 ┃   1 ┃  1.10 ┃ 2001-01-11 ┃
+┃ 1 ┃ text 2 ┃   2 ┃  2.20 ┃ 2002-02-12 ┃
+┃ 2 ┃ text 3 ┃   3 ┃  3.30 ┃ 2003-03-13 ┃
+┃ 3 ┃ text 4 ┃   4 ┃  4.40 ┃ 2004-04-14 ┃
+┗━━━┻━━━━━━━━┻━━━━━┻━━━━━━━┻━━━━━━━━━━━━┛
+[4 rows x 4 columns]
+"""}
+    headers = ['string', 'int', 'float', 'date']
+    data = [
+         ('text 1',  1, 1.1, datetime.date(2001, 1, 11))
+        ,('text 2', 2, 2.2, datetime.date(2002, 2, 12))
+        ,('text 3', 3, 3.3, datetime.date(2003, 3, 13))
+        ,('text 4', 4, 4.4, datetime.date(2004, 4, 14))
+    ]
+    sdm = SQLDataModel(data,headers, min_column_width=3, max_column_width=38, display_index=True, display_float_precision=2)
+    repr_styles = ['ascii','bare','dash','default','double','markdown','outline','pandas','polars','postgresql','round','thick']   
+    for style in repr_styles:
+        sdm.set_table_style(style=style)
+        expected_repr = style_output_dict[style].strip('\n')
+        output_repr = sdm.__repr__()
+        assert output_repr == expected_repr
```


# Comparing `tmp/daffodil-0.2.2.tar.gz` & `tmp/daffodil-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daffodil-0.2.2.tar", last modified: Fri Mar  1 20:34:54 2024, max compression
+gzip compressed data, was "daffodil-0.3.0.tar", last modified: Sun Apr 14 21:33:25 2024, max compression
```

## Comparing `daffodil-0.2.2.tar` & `daffodil-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-03-01 20:34:54.792537 daffodil-0.2.2/
-drwxrwxrwx   0        0        0        0 2024-03-01 20:34:54.788538 daffodil-0.2.2/Daffodil.egg-info/
--rw-rw-rw-   0        0        0      276 2024-03-01 20:34:54.000000 daffodil-0.2.2/Daffodil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      479 2024-03-01 20:34:54.000000 daffodil-0.2.2/Daffodil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-01 20:34:54.000000 daffodil-0.2.2/Daffodil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-03-01 20:34:54.000000 daffodil-0.2.2/Daffodil.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-03-01 20:34:54.000000 daffodil-0.2.2/Daffodil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2024-02-28 17:20:31.000000 daffodil-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      276 2024-03-01 20:34:54.790537 daffodil-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    47480 2024-03-01 20:33:11.000000 daffodil-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-01 20:34:54.782536 daffodil-0.2.2/lib/
--rw-rw-rw-   0        0        0        4 2024-03-01 03:13:49.000000 daffodil-0.2.2/lib/__init__.py
--rw-rw-rw-   0        0        0    43076 2024-03-01 04:46:40.000000 daffodil-0.2.2/lib/daf_indexing.py
--rw-rw-rw-   0        0        0    31476 2024-03-01 04:07:20.000000 daffodil-0.2.2/lib/daf_md.py
--rw-rw-rw-   0        0        0     7589 2024-03-01 04:09:41.000000 daffodil-0.2.2/lib/daf_pandas.py
--rw-rw-rw-   0        0        0     5258 2024-03-01 01:03:09.000000 daffodil-0.2.2/lib/daf_types.py
--rw-rw-rw-   0        0        0    42755 2024-03-01 04:25:01.000000 daffodil-0.2.2/lib/daf_utils.py
--rw-rw-rw-   0        0        0     5796 2024-03-01 01:03:09.000000 daffodil-0.2.2/lib/md_demo.py
--rw-rw-rw-   0        0        0       42 2024-03-01 20:34:54.792537 daffodil-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      380 2024-03-01 03:42:31.000000 daffodil-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-01 20:34:54.785537 daffodil-0.2.2/tests/
--rw-rw-rw-   0        0        0   160239 2024-03-01 04:21:44.000000 daffodil-0.2.2/tests/test_daf.py
+drwxrwxrwx   0        0        0        0 2024-04-14 21:33:25.799924 daffodil-0.3.0/
+drwxrwxrwx   0        0        0        0 2024-04-14 21:33:25.791931 daffodil-0.3.0/Daffodil.egg-info/
+-rw-rw-rw-   0        0        0    50162 2024-04-14 21:33:25.000000 daffodil-0.3.0/Daffodil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      494 2024-04-14 21:33:25.000000 daffodil-0.3.0/Daffodil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 21:33:25.000000 daffodil-0.3.0/Daffodil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-04-14 21:33:25.000000 daffodil-0.3.0/Daffodil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-14 21:33:25.000000 daffodil-0.3.0/Daffodil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2024-02-28 17:20:31.000000 daffodil-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0    50162 2024-04-14 21:33:25.796925 daffodil-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    49512 2024-04-12 21:24:34.000000 daffodil-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 21:33:25.785425 daffodil-0.3.0/lib/
+-rw-rw-rw-   0        0        0        4 2024-03-01 21:59:22.000000 daffodil-0.3.0/lib/__init__.py
+-rw-rw-rw-   0        0        0    43076 2024-03-01 21:59:22.000000 daffodil-0.3.0/lib/daf_indexing.py
+-rw-rw-rw-   0        0        0    31511 2024-03-13 19:29:45.000000 daffodil-0.3.0/lib/daf_md.py
+-rw-rw-rw-   0        0        0     7580 2024-03-13 19:01:32.000000 daffodil-0.3.0/lib/daf_pandas.py
+-rw-rw-rw-   0        0        0     5327 2024-03-23 00:09:19.000000 daffodil-0.3.0/lib/daf_types.py
+-rw-rw-rw-   0        0        0    46595 2024-03-23 00:31:44.000000 daffodil-0.3.0/lib/daf_utils.py
+-rw-rw-rw-   0        0        0     5796 2024-03-01 21:59:22.000000 daffodil-0.3.0/lib/md_demo.py
+-rw-rw-rw-   0        0        0       86 2024-04-14 21:25:39.000000 daffodil-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 21:33:25.799924 daffodil-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      895 2024-04-14 21:25:39.000000 daffodil-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 21:33:25.788394 daffodil-0.3.0/tests/
+-rw-rw-rw-   0        0        0   164370 2024-04-14 19:08:24.000000 daffodil-0.3.0/tests/test_daf.py
```

### Comparing `daffodil-0.2.2/LICENSE` & `daffodil-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `daffodil-0.2.2/README.md` & `daffodil-0.3.0/Daffodil.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,48 @@
+Metadata-Version: 2.1
+Name: daffodil
+Version: 0.3.0
+Summary: Daffodil provides lightweight and fast 2-D dataframes
+Home-page: https://github.com/raylutz/daffodil
+Author: Ray Lutz
+Author-email: raylutz@cognisys.com
+License: MIT
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: xlsx2csv==0.8.2
+Requires-Dist: Markdown==3.4.1
+Provides-Extra: numpy
+Requires-Dist: numpy; extra == "numpy"
+
 ![daffodil_logo](https://github.com/raylutz/daffodil/assets/14955977/5e141583-0216-429d-9ba8-be938aa13017)
 
 # Python Daffodil
 
 The Python Daffodil (DAtaFrames For Optimized Data Inspection and Logical processing) package provides
 lightweight, simple and flexible 2-d dataframes built on 
 python data types, including a list-of-list array as the core datatype. Daffodil is similar to other data frame
 packages, such as Pandas, Numpy, Polars, Swift, Vaex, Dask, PyArrow, SQLite, PySpark, etc. but is simpler and may be faster 
 because it does not have conversion overhead.
 
-## Visualization of the data model
+STATUS: Daffodil is largely operating quite well, but there are still design tradeoffs that are being investigated.
+Some of the methods of the class and assumptions that can be made about the state of the data may change slightly
+as these design tradeoffs are being evaluated and the final initial design resolved. Please see GitHub issues to
+weigh in on the design.
+
+## Data Model
+The Daffodil data model is really very simple. The core array is a list-of-lists (lol), optionally with one or two associated
+dictionaries, one for the column names and one for row keys.
 
 ![pydf_table](https://github.com/raylutz/daffodil/assets/14955977/05c54a27-8d8e-47b6-ae73-957709a5d398)
 
-Daffodil provides basic dataframe functionality which is not available in core python, but should be. 
 Daffodil uses standard python data types, and can mix data types in rows and columns, and can store any type 
 within a cell, even another Daffodil instance. 
 
 It works well in traditional Pythonic processing paradigms, such as in loops, allowing fast row appends, 
 insertions and other operations that column-oriented packages like Pandas handle poorly or don't offer at all.
 Selecting, inserting, appending rows does not make a copy of the data but uses references and works the way 
 Python normally does, leveraging the inherent power of Python without replacing it.
@@ -65,19 +91,19 @@
 work on it in Python. 
 
 When is it worth porting to Pandas? That will depend on the size of the array and what the calculations are.
 But a convenient rule of thumb from our testing is that Pandas can be more performant than Daffodil if 
 column-oriented manipulations (similar to summing) are repeated on the same data at least ~30 times.
 
 In other words, if you have an array and you need to do just a few column-based operations (fewer than 30), 
-then it will be probably be faster to just do them using Daffodil `apply` or `reduce` operations, rather than
+then it will be probably be faster to just do them using Daffodil `.apply()` or `.reduce()` operations, rather than
 exporting the array to Pandas, performing the calcs and the transferring it back in. (You can see our benchmarks
 and other tests linked below.)
 
-In additiona, Daffodil is a good partner with Pandas and NumPy when only some number crunching and array-based operations are needed.
+In addition, Daffodil is a good partner with Pandas and NumPy when only some number crunching and array-based operations are needed.
 Use Daffodil to build the array incrementally using row-based operations, then export the data to NumPy or
 Pandas. NumPy is recommended if the data is uniform enough because it is faster and has a smaller
 memory footprint than Pandas.
 
 Daffodil is pure python and can be run with no (or few) other packages installed. It is relatively tiny. 
 If Pandas is not used, start up time is improved dramatically. This can be very important in cloud-based parallel processing where every millsecond
 is billed or in embedded systems that want to utilize tables but can't suffer the overhead.
@@ -106,28 +132,31 @@
 Daffodil arrays in one cell. We believe the UI is simpler than what is offered by Pandas.
         
 ## Supports incremental appends
 
 Daffodil can append or insert one or more rows or concatenate with another Daffodil object extremely quickly, because it leverages Python's
 data referencing approach. When the data can be used without copying, then this will 
 minimize overhead. Concatenating, dropping and inserting columns is functionality that is provided, but is not
-recommennded. Normally, columns need not be manipulated. Avoid explicitly dropping columns and simply provide a list of columns included in calculations.
+recommennded. Avoid explicitly dropping columns and simply provide a list of columns included in calculations.
 
 ## Column names
 
 Similar to Pandas and other dataframe concepts, Daffodil has a separate set of column names that can be optionally
 used to name the columns. This is organized internally as a Python dictionary (hd -- header dict) for fast column lookups by name.
 Column names must be hashable and unique, and other than that, there are no firm restrictions.  
 (However, to use the interface with SQLite, avoid using the double underscore "__" in the names, which is used to 
 allow arbitrary names in SQLite.)
     
 When reading CSV files, the header is normally taken from the first (non-comment) line. If "user_format" is 
 specified on reading csv files, the csv data will be pre-processed and "comment" lines starting with # are removed.
 
-Daffodil supports CSVJ, which is a mix of CSV with JSON metadata in comment fields in the first few lines of the file, to provide data type, formatting, and other information. Using CSVJ speeds importing CSV data into a Daffodil instance because the data can be converted to the appropriate type as it is read, and therefore avoids a second pass to convert data from str type, which is the default. This also may unflatten objects. (CSVJ not supported yet).
+Daffodil supports CSVJ, which is a mix of CSV with JSON metadata in comment fields in the first few lines of the file, 
+to provide data type, formatting, and other information. Using CSVJ speeds importing CSV data into a Daffodil instance 
+because the data can be converted to the appropriate type as it is read, and therefore avoids a second pass to convert 
+data from str type, which is the default. This also may unflatten objects. (CSVJ not supported yet).
 
 In some cases, you may be working with CSV files without a header line providing of column names. This is common
 in xlsx spreadsheets which have column names set by position. Setting noheader=True avoids 
 capturing the column names from the header line from csv input, and then column names will not be defined.
 
 If columns repeated or are missing, this will be detected when first read, and the header row will be adjusted
 so it can be used. If any column name is blank, then these are named "colN" (or any other prefix you may prefer) 
@@ -151,58 +180,68 @@
 ## Row keyfield   
     
 In many cases, one of the columns can be used as a unique key for locating records. If such a column exists, it 
 can be adopted as the primary index of the table by specifying that column name as the `keyfield`. When this is done,
 then the `kd` (key dictionary) is built and maintained from that column. 
 Creating a key index does not remove that field from the data array. `kd` is an additional structure created internally.
 
-If keyfield is set, then that column must be a hashable type and must have unique values. Searches of row entries use dictionary lookups, which are highly optimized for speed by Python.
+If keyfield is set, then that column must be a hashable type and must have unique values. Searches of row entries use 
+dictionary lookups, which are highly optimized for speed by Python.
+
+The kd can also be set without the existence of a column to adopt from the array. This is useful particularly when 
+transposing the dataframe so that the column names can be adopted as the row keys, and vice versa.
 
 Unlike the keyfield oriented lookup functionality, row indices do not stick to the rows and are always with respect to the frame. 
 This is similar behavior to the Polars package and differs from Pandas, which has an index that sticks with each row, and is more
-like the keyfield approach.
+like the kd approach used by Daffodil.
 
 When adopting a file that may have a column that is tainted, it will be best to follow the following steps:
 1. Set `keyfield=''` to turn off the key indexing functionality.
 2. Read in the data, and it will not be limited by the keyfield definition.
 3. Use method `my_daf.set_keyfield(keyfield_name)` to set the keyfield to the column `keyfield_name` and build the lookup dictionary.
 4. Check that they are all unique by comparing the number of keys vs. the number of records.
 5. if the lengths are different, remove, delete, or otherwise deal with records with duplicate keys so the keys are unique.
 6. And then use `.set_keyfield(keyfield)` again.
 
 The convenience method `my_daf.add_idx()` can be used to add a column with indices that can be used as a keyfield.
 
 Only one keyfield is supported, but additional keying can be built by the users by creating dicts of any column or set of columns.
     
 ## Column vs. Row Operations
-Daffodil is a row-oriented package. Other popular packages, like Pandas, Polars, etc, are column oriented because it can be very beneficial.
-Thus, it is easy to manipulate rows (appending, inserting, deleting, etc) while it is relatively much more difficult to manipulate
+Daffodil is a row-oriented package. Other popular packages, like Pandas, Polars, etc, are column oriented because it can be very 
+beneficial for calculations that can be performed on a column basis.
+
+Thus, in Daffodil, it is easy to manipulate rows (appending, inserting, deleting, etc) while it is relatively much more difficult to manipulate
 columns.  Rows are very easy to handle because the list-of-list underlying structure
 re-uses any lists selected in any selection operation. A new Daffodil instance which might include be a subset of the rows in the original 
 does not consume much additional space because the contents of those rows is not copied. Instead, Python
 copies only the _references_ to the rows. If only a few rows are used from the original, the the remaining rows will 
 be garbage collected by the normal Python mechanisms.  The rows that are still active are the same rows that existed in the original array without copying.
 
 This use-without-copying pattern means that Daffodil can perform quite well when compared with other packages when doing this type of manipulation, both in terms of space and also time.
 
 In contrast, operations that add, drop, or insert columns are relatively slow, 
 but it turns out that actually these operations are not normally that 
 necessary. Reducing the number of columns only is important in a few cases:
 
 1. When converting from/to other forms. Extraneous columns may exist or may be of the wrong type.
-2. When performing .apply() or .reduce() operations to avoid processing extraneous columns.
+2. When performing `.apply()` or `.reduce()` operations to avoid processing extraneous columns.
 4. When creating a report and only including some columns in the report
 
 In these cases, the columns to be included can be expressed explicitly, rather then modifying the array by dropping them. 
 
 Nevertheless, these operations are provided. When selecting/dropping columns, a transposition can be performed for free, if `flip=True` is indicated.
 
 Other column operations such as statistics are not as performant as column-based packages but in those cases when
 many operations are required, the appropriate portion of the array can be ported to NumPy, Pandas, or any other dataframe package.
 
+Also, rows can be conceptually treated as if they are columns, because the structure of a Daffodil array is transposition symmetrical. Simply
+place column data in each row and name the row with the column name. To sum values in a column, then the values in each row, which is a 
+list, can be summed with the sum() operator.
+
 ## Common Usage Pattern
        
 One common usage pattern allows iteration over the rows and appending to another instance. For example:
     
         # read csv file into 2-D array, handling column headers and unflattening
         my_daf = Daf.from_csv(file_path, unflatten=True)  
     
@@ -238,14 +277,19 @@
         result_manifest_daf = chunk_manifest_daf.manifest_apply(transform_row)
 
 Similarly, a set of csv_files can be reduced to a single record using a reduction method. For example, 
 for determining valuecounts of columns in a set of files:
 
         chunk_manifest_daf = Daf.from_csv(file_path, unflatten=True)
         result_record = chunk_manifest_daf.manifest_reduce(count_values)
+        
+Daffodil actually extends to chunks very elegantly because the apply() or reduce() operators can be applied to the
+rows and to chunks just as well. In contrast, column-based schemes require many passes through the data or delayed
+"lazy" operations that are difficult to comprehend.        
+        
     
 ## Methods and functionality
        
 ### print and markdown reports
 
 Daffodil can produce convenient form for interactive inspection similar to Pandas,
 but unlike Pandas, Markdown is the primary format for all reports. Markdown provided
@@ -678,15 +722,27 @@
 ## Comparison with Pandas, Numpy SQLite
 
 One of the primary reasons for developing Daffodil is that 
 conversion to Pandas directly from arbitrary Python list-of-dicts, for example, is surprisingly slow.
 
 We timed the various conversions using Pandas 1.5.3 and 2.4.1.
 
-See: https://github.com/raylutz/daffodil/blob/main/docs/daf_benchmarks
+See: https://github.com/raylutz/daffodil/blob/main/docs/daf_benchmarks.md
+
+Daffodil is faster than Pandas for array manipulation (inserting rows (300x faster) and cols (1.4x faster)), 
+performing actions on individual cells (5x faster), appending rows (which Pandas essentially outlaws), 
+and performing keyed lookups (8.4x faster). Daffodil arrays are smaller whenever any strings are included 
+in the array by about 3x over Pandas. While Pandas and Numpy are faster for columnar calculations, 
+Numpy is always faster if columns are all numeric data. Daffodil is larger than purely numeric arrays than
+Numpy and Pandas but if string columns are included, Pandas will likely be 3x larger. Numpy does not handle
+string columns mixed with numeric data.
+
+Therefore it is a good strategy to use Daffodil for all operations except for pure data manipulation, 
+and then port the appropriate columns to NumPy.
+
 
 ## Demo
 
 See this demo of Daffodil functionality.
 
 https://github.com/raylutz/daffodil/blob/main/docs/daf_demo.md
 
@@ -717,35 +773,34 @@
 |df.agg()                                          |daf.reduce()                              |reduce array to a record using arbitrary function  |
 |df.transform()                                    |daf.apply(by='table')                     |transform a table using a function producing a table   |
 |df.groupby()                                      |daf.groupby(); groupby_cols(); groupby_cols_reduce; groupby_reduce()  |group rows by values in a column and poss. apply a reduction  |
 |df.value_counts()                                 |daf.value_counts()                        |reduce a column by counting values.  |
 |df.tail(n)                                        |daf[-n:]                                  |return last n rows  |
 |df.sort_values()                                  |daf.sort_by_colname()                     |Daf only sorts rows   |
 |df.transpose()                                    |daf.select_kcols(flip=True)               |Not recommended in Daffodil but free if columns are dropped   |
-|df.drop()                                         |daf.select_kcols(kcols=[colnames], inverse=True)   |Drop columns by name. Transpose if free in Daf if done during a drop  |
+|df.drop()                                         |daf.select_kcols(kcols=[colnames], inverse=True)   |Drop columns by name. Transpose is free in Daf if done during a drop  |
 |df[~df[keyfield].isin(list of keys)]              |daf.select_krows(krows=[list of keys], inverse=True)  |Drop rows by keys in the keyfield.   |
 |df.to_records()                                   |daf.to_lod(); .to_dod()                   |convert from array to records in list-of-dict (or dict-of-dict) format.  |
 |df.to_markdown()                                  |daf.to_md()                               |convert to markdown representation. default presentation in Daf  |
 |df.assign()                                       |daf[:, n] = new_col                       |assign new values to a column  |
 | -- (not available?)                              |daf[rowname or idx] = dict                |assign new values to a row and respect column names as dict keys  |
 |df[df[colname] > 5]                               |daf.select_where(lambda row: row[colname] > 5)  |select rows where the value in colname > 5   |
-|df.rename(renaming dict)                          |daf.rename_cols(); daf.set_cols()         |Daf does not support renaming rows as this is a column in the table.  |
-|df.reset_index                                    |daf.set_keyfield('')                      |similar in operation but not exact.   |
-|df.set_index                                      |daf.set_keyfield(keyfieldname)            |Daf uses an existing column for the keyfield and does not have a separate index  |
-|df.truncate()                                     |daf[:n]; daf[n:]; daf[:n]; daf[n:]        |Truncate before or after some index   |
-|df.replace()                                      |daf.find_replace(find_pat, replace_val)   |Daf replaces values found in-place.   |
+|df.rename(renaming dict)                          |daf.rename_cols(); daf.set_cols(); daf.set_rowkeys()   |Daf allows renaming rows when keyfield=''  |
+|df.reset_index                                    |daf.set_keyfield(''); daf.set_rowkeys()   |similar in operation.   |
+|df.set_index                                      |daf.set_keyfield(keyfieldname)            |Daf can use an existing column for the keyfield or can set the rowkeys independently  |
+|df.truncate()                                     |daf[:n]; daf[n:]                          |Truncate before or after some index n.  |
+|df.replace()                                      |daf.find_replace(find_pat, replace_val)   |Replace values found in-place.   |
 
 
 
 ## Conclusion and Summary
 
 The general conclusion is that it generally beneficial to use Daffodil instead of lod or pandas df for
 general-purpose table manipulation, but when number crunching is needed, prepare the data with Daffodil 
-and convert directly to Numpy. The fact that we can convert quickly to Numpy and from Numpy to Pandas
-is instant makes the delay to load directly to Pandas dataframe seem nonsensical. 
+and convert directly to Numpy or Pandas. 
 
 We find that in practice, we had many cases where Pandas data frames were being used only for 
 reading data to the array, and then converting to lod data type and processing by rows to
 build a lod structure, only to convert to df at the end, with no data crunching where
 Pandas excels. We found also that when we performed column-based calculations, that they were 
 sometimes wasteful because they would routinely process all data in the column rather than terminating 
 early. Complex conditionals and using '.apply' is not recommended for Pandas but work well with Daffodil.
```

### Comparing `daffodil-0.2.2/lib/daf_indexing.py` & `daffodil-0.3.0/lib/daf_indexing.py`

 * *Files identical despite different names*

### Comparing `daffodil-0.2.2/lib/daf_md.py` & `daffodil-0.3.0/lib/daf_md.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pydf_md.py -- markdown generation
 
 # copyright (c) 2024 Ray Lutz
 
 import re
-import copy
+#import copy
 import markdown
 #import functools
 
 #import pprint
 from string import Template
 
 from lib.daf_types import T_ls, T_lola, T_da, T_li #, T_doda, T_df, T_lf, T_loda, T_loloda, T_lodolodi, T_ts, T_ds, T_dola 
@@ -256,30 +256,31 @@
     """
 
     if not cols_lol:
         return ''
     if max_text_len is None:
         max_text_len = 80
         
-    mutated_cols_lol = copy.deepcopy(cols_lol)
+    #mutated_cols_lol = copy.deepcopy(cols_lol)
+    mutated_cols_lol = cols_lol
 
     # either get the header or pull it off the columns
     if omit_header:
         pass
     elif header:
         # add header to the columns
         header = [f"{col}".replace('\n', '<br>').replace('\r', '') for col in header]
         for idx, col in enumerate(mutated_cols_lol):
             s = utils.safe_get_idx(header, idx, default='')
             col.insert(0, s)
     else:
         raise RuntimeError ("md header is required if 'omit_header' not specified.")
     
     num_cols = len(mutated_cols_lol)
-    max_row = utils.safe_max([len(col) for col in mutated_cols_lol])
+    max_row = max([len(col) for col in mutated_cols_lol], default=0)
     
     # fill new_cols with blanks to start with.
     new_cols_lol = []
     for _ in range(num_cols):
         new_cols_lol.append([''] * max_row)
 
     # sanitize cols
```

### Comparing `daffodil-0.2.2/lib/daf_pandas.py` & `daffodil-0.3.0/lib/daf_pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 def _from_pandas_df(
         cls,
         df: T_df, 
         keyfield: str='', 
         name: str='', 
         use_csv: bool=False, 
         dtypes: Optional[T_dtype_dict]=None
-        ) -> 'Daf':
+        ):
     """
     Convert a Pandas dataframe to pydf object
         @@TODO: This does not enforce dtypes are correct.
     """
     import pandas as pd     # type: ignore
     
     python_dtypes = pandas_dtype_to_python(df)
```

### Comparing `daffodil-0.2.2/lib/daf_types.py` & `daffodil-0.3.0/lib/daf_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,21 @@
 T_idi = Dict[int, int]
 T_di  = Dict[str, int]
 T_db  = Dict[str, bool]
 T_dsi = Dict[str, T_si]
 T_dn  = Dict[str, None]
 T_ls  = List[str]
 T_li  = List[int]
+T_lr  = List[range]
+T_rli = Union[range, T_li]
 T_lsi = List[T_si]
 T_la  = List[Any]
 T_lf  = List[float]
 T_lb  = List[bool]
+T_lt  = List[Type]
 T_ss  = Set[str]
 T_sa  = Set[Any]
 T_dsn = Dict[str, Optional[str]]
 T_ta  = Tuple[Any, ...]
 T_ts  = Tuple[str, ...]
 T_ti  = Tuple[int, ...]
```

### Comparing `daffodil-0.2.2/lib/daf_utils.py` & `daffodil-0.3.0/lib/daf_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,43 +20,75 @@
 
 from typing import List, Dict, Any, Tuple, Optional, Union, cast, Type #, Callable
 
 def fake_function(a: Optional[List[Dict[str, Tuple[int,Union[Any, str]]]]] = None) -> Optional[int]:
     return None or cast(int, 0)       # pragma: no cover
 
 
-from lib.daf_types import T_lola, T_loda, T_dtype_dict, T_da, T_ds, T_hdlola, T_la, T_loti, T_ls, T_doda, T_buff, T_li
+from lib.daf_types import T_lola, T_loda, T_dtype_dict, T_da, T_ds, T_hdlola, T_la, T_loti, T_ls, T_doda, T_buff, T_li, T_lr
                     
 
 def is_linux() -> bool: 
     return platform.system() == 'Linux'
+    
 
-def apply_dtypes_to_hdlol(hdlol: T_hdlola, dtypes: T_dtype_dict) -> T_hdlola:
+def apply_dtypes_to_hdlol(hdlol: T_hdlola, dtypes: T_dtype_dict, initially_all_str: bool=True) -> T_hdlola:
 
     hd, lol = hdlol
     
     if not lol or not lol[0] or not hd:
         return (hd, lol)
 
-    for idx, la in enumerate(lol):
-        da = dict(zip(hd.keys(), la))
-        type_set_da = set_dict_dtypes(da, dtypes)
-        lol[idx] = [type_set_da[col] for col in hd.keys()]
+    # make a worklist of those fields that need to be checked.
+    dtypes_worklist: List[Tuple[int, Type]] = []
+    # create a list of types
+    for idx, col in enumerate(hd.keys()):
+        desired_type = dtypes.get(col, str)
+        if desired_type == str and initially_all_str:
+            continue
+        dtypes_worklist.append( (idx, desired_type ) )
+
+    for la in lol:
+        set_type_la(la, dtypes_worklist)
         
     return (hd, lol)
     
 
+def set_type_la(la: T_la, dtypes_worklist: List[Tuple[int, Type]]) -> T_la:
+    """ set the types of each item in place based on a list of types without making a copy,
+        and only working on those fields that may need work.
+    """
+    
+    for idx, desired_type in dtypes_worklist:
+        value = la[idx]
+        if isinstance(value, desired_type):
+            continue
+        if desired_type in (int, bool):
+            try:
+                la[idx] = int(value)
+            except ValueError:
+                la[idx] = int(float(value))
+                
+        elif desired_type == float:
+            la[idx] = float(value)
+            
+        elif desired_type == str:    
+            la[idx] = str(value)
+    
+    return la
+    
+
 def set_cols_da(da: T_da, cols: T_ls, default: Any='') -> T_da:
     """ Set keys in dictionary da to be exactly cols
         Use default if key not already in da.
     """
     
     new_da = {k:da.get(k, default) for k in cols}
     return new_da
-    
+
 
 def select_col_of_lol_by_col_idx(lol: T_lola, col_idx: int) -> T_la:
     """
     select a row and col from lol
     
     Note: this creates a new object.
         
@@ -441,22 +473,22 @@
     info_d['non_missing']       = non_missing    = [v for v in alist if not(v is None or v == '' or v != v)]
     
     info_d['all_ints'] = is_list_allints(non_missing)
         
     if info_d['all_ints']:
         local_ilist = [int(float(clean_numeric_str(str(i)))) for i in non_missing if is_numeric(i)]
         info_d['all_numeric'] = True
-        info_d['max'] = safe_max(local_ilist)
-        info_d['min'] = safe_min(local_ilist)
+        info_d['max'] = max(local_ilist, default=0)
+        info_d['min'] = min(local_ilist, default=0)
 
     else:
         info_d['all_numeric'] = is_list_allnumeric(non_missing)
         local_flist = [float(clean_numeric_str(str(i))) for i in non_missing if is_numeric(i)]
-        info_d['max'] = safe_max(local_flist)
-        info_d['min'] = safe_min(local_flist)
+        info_d['max'] = max(local_flist, default=0)
+        info_d['min'] = min(local_flist, default=0)
         
     return info_d
     
 
 def list_stats_attrib(alist:T_la) -> T_da:         
     """ 
         evaluate a list as an attribute and provide stats info_d considering values only within this single list.
@@ -515,23 +547,23 @@
         
     if not info_d['all_ints']:    
         info_d['all_numeric'] = is_list_allnumeric(nonmissing)
     
     if info_d['all_ints']:
         info_d['all_numeric'] = True
         local_ilist     = [int(float(i)) for i in nonmissing]
-        info_d['max']   = safe_max(local_ilist)
-        info_d['min']   = safe_min(local_ilist)
+        info_d['max']   = max(local_ilist, default=0)
+        info_d['min']   = min(local_ilist, default=0)
         info_d['mean']  = safe_mean(local_ilist)
         info_d['stdev'] = safe_stdev(local_ilist)
 
     elif info_d['all_numeric']:
         local_flist     = [float(i) for i in nonmissing]
-        info_d['max']   = safe_max(local_flist)
-        info_d['min']   = safe_min(local_flist)
+        info_d['max']   = max(local_flist, default=0)
+        info_d['min']   = min(local_flist, default=0)
         info_d['mean']  = safe_mean(local_flist)
         info_d['stdev'] = safe_stdev(local_flist)
   
     return info_d
     
 
 def list_stats_localidx(alist: T_la) -> T_da:
@@ -542,16 +574,16 @@
     for val in alist:
         if not bool(re.search(r'^\d+$', f"{val}")):
             info_d['all_ints'] = False
             return info_d
             
     info_d['all_ints'] = True
     local_alist = [int(float(i)) for i in alist]
-    info_d['max'] = safe_max(local_alist)
-    info_d['min'] = safe_min(local_alist)
+    info_d['max'] = max(local_alist, default=0)
+    info_d['min'] = min(local_alist, default=0)
     
     info_d['sequential'] = bool(info_d['max'] - info_d['min'] == len(alist) - 1)
     
     return info_d
     
 
 def is_list_allints(alist: T_la) -> bool:
@@ -590,27 +622,35 @@
             if str2bool(val):
                 num_true += 1
         return True, num_true
     except Exception:
     
         return False, 0
     
-def profile_ls_to_loti(input_ls: T_ls, repeat_startswith='Unnamed', ignore_cols: Optional[T_ls]=None) -> T_loti:
+def profile_ls_to_loti(
+        input_ls: T_ls, 
+        repeat_startswith='Unnamed', 
+        include_cols: Optional[T_ls]=None,
+        ignore_cols: Optional[T_ls]=None,
+        ) -> T_loti:
     """ 
         Given a list strings, which are typically the header of a column,
         return a list of tuples of integers loti, that describes the
         column offset of a given starting string, and the length of
         any repeats of that string, or strings marked with the repeat_marker.
         
         for example:
         input_ls = ['Alice', 'Bob', 'Unnamed2', 'Charlie', 'David', 'Unnamed5', 'Unnamed6']
         
         will return:
         output_loti = [(0, 1), (1, 2), (3, 1), (4, 3)]
         
+        if either ignore cols or include cols are provided, then  do not profile 
+        any columns not included but include the offsets in the profile.
+        
     """    
     repeat_count = 0
     result_loti: T_loti = []
     unique_idx  = 0
     
     if ignore_cols is None:
         ignore_cols = []
@@ -635,14 +675,67 @@
     
     if repeat_count:
         result_loti.append( (unique_idx, repeat_count) )
         
     return result_loti            
             
 
+def profile_ls_to_lr(
+        input_ls: T_ls, 
+        repeat_startswith='Unnamed', 
+        include_cols: Optional[T_ls]=None,
+        ignore_cols: Optional[T_ls]=None,
+        ) -> T_lr:
+    """ 
+        Given a list strings, which each are typically the header of a column,
+        return a list of ranges T_lr, that describes the
+        column offset of a given starting string, and the ending offest of
+        any repeats of that string, or strings marked with the repeat_marker.
+        
+        for example:
+        input_ls = ['Alice', 'Bob', 'Unnamed2', 'Charlie', 'David', 'Unnamed5', 'Unnamed6']
+        
+        will return:
+        output_loti = [range(0, 1), range(1, 3), range(3, 4), range(4, 7)]
+        
+        if either ignore cols or include cols are provided, then  do not profile 
+        any columns not included but include the offsets in the profile.
+        
+    """    
+    repeat_count = 0
+    result_lr: T_lr = []
+    unique_idx  = 0
+    
+    if ignore_cols is None:
+        ignore_cols = []
+    
+    unique_idx = -1
+    for idx, colstr in enumerate(input_ls):
+    
+        if colstr in ignore_cols:
+            continue
+    
+        if unique_idx == -1:
+            repeat_count = 1
+            unique_idx = idx
+                
+        elif colstr.startswith(repeat_startswith):
+            repeat_count += 1
+            
+        else:
+            result_lr.append( range(unique_idx, unique_idx + repeat_count) )
+            unique_idx = idx
+            repeat_count = 1
+    
+    if repeat_count:
+        result_lr.append( range(unique_idx, unique_idx + repeat_count) )
+        
+    return result_lr
+            
+
 def reduce_lol_cols(lol: T_lola, max_cols:int=10, divider_str: str='...') -> T_lola:
     """ if input lol is over max_cols, display only max_cols//2 first_cols, a divider col, then same number of last_cols 
     
         does not alter lol
     
     """
     
@@ -750,17 +843,15 @@
         return default
     
 
 def safe_max(listlike):
     # note! Using try/except in to guard for the length of list is not specific enough. 
     #   We still need failure under other conditions.
 
-    if len(listlike) < 1:
-        return 0
-    return max(listlike)
+    return max(listlike, default=0)
      
 
 def shorten_str_keeping_ends(string: str, limit: int) -> str:
     """ combine multiple lines into a single line, then 
         shorten the line if needed to no more than limit chars
         by removing chars from the middle.
     """
@@ -1237,15 +1328,15 @@
 def _generate_spreadsheet_column_names_list(num_cols: int) -> T_ls:
     """ generate a full list of column names for the num_columns specified 
     """
 
     return [_calculate_single_column_name(i) for i in range(num_cols)]
 
 
-def _sanitize_cols(cols: T_ls, unnamed_prefix='col') -> list:
+def _sanitize_cols(cols: T_ls, unnamed_prefix='Unnamed') -> list:
     """ make sure there are no blanks and columns are unique.
         if missing, substitute with {unnamed_prefix}{col_idx}
         if duplicated, substitute with prior_name_{col_idx}
     """
     
     if cols:
         # first make sure all columns have names.
@@ -1256,10 +1347,37 @@
         for idx, col in enumerate(cols):
             if col not in col_hd:
                 col_hd[col] = idx
             else:
                 # if not unique, add _NNN after the name.
                 col_hd[f"{col}_{idx}"] = idx
         return list(col_hd.keys())
+
+
+def dict_with_index(iterable) -> Dict[Any, int]:
+
+    return dict(with_index(iterable))
+    
             
+def with_index(iterable):
+    """Like enumerate, but (val, i) tuples instead of (i, val)."""
+    for i, item in enumerate(iterable):
+        yield (item, i)
+
             
+def invert_dol_to_dict(input_dol:dict) -> dict:
+    """ given a dict of lists where no element in any is seen twice,
+        create a dict, where the list elements are the key and the
+        value is the prior key. This allows reverse lookup of key
+        based on values in the list. If some dict lists have duplicates,
+        the last item will dominate.
+    """
+    result_dict: Dict[Any, Any] = {}
+
+    for key, lst in input_dol.items():
+        for val in lst:
+            result_dict[val] = key
+
+    return result_dict
+
+
```

### Comparing `daffodil-0.2.2/lib/md_demo.py` & `daffodil-0.3.0/lib/md_demo.py`

 * *Files identical despite different names*

### Comparing `daffodil-0.2.2/tests/test_daf.py` & `daffodil-0.3.0/tests/test_daf.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,35 +386,35 @@
     
     def test_set_keyfield_nonexistent_column(self):
         # Test trying to set keyfield to a nonexistent column
         daf = Daf(lol=[[1, 'a'], [2, 'b']], cols=['ID', 'Value'])
         with self.assertRaises(KeyError):
             daf.set_keyfield('nonexistent_column')
 
-    # row_idx_of
-    def test_row_idx_of_existing_key(self):
-        # Test getting row index of an existing key
-        daf = Daf(lol=[['1', 'a'], ['2', 'b']], cols=['ID', 'Value'], keyfield='ID')
-        self.assertEqual(daf.row_idx_of('1'), 0)
+    # # row_idx_of (DEPRECATED)
+    # def test_row_idx_of_existing_key(self):
+        # # Test getting row index of an existing key
+        # daf = Daf(lol=[['1', 'a'], ['2', 'b']], cols=['ID', 'Value'], keyfield='ID')
+        # self.assertEqual(daf.row_idx_of('1'), 0)
     
-    def test_row_idx_of_nonexistent_key(self):
-        # Test getting row index of a nonexistent key
-        daf = Daf(lol=[['1', 'a'], ['2', 'b']], cols=['ID', 'Value'], keyfield='ID')
-        self.assertEqual(daf.row_idx_of('3'), -1)
+    # def test_row_idx_of_nonexistent_key(self):
+        # # Test getting row index of a nonexistent key
+        # daf = Daf(lol=[['1', 'a'], ['2', 'b']], cols=['ID', 'Value'], keyfield='ID')
+        # self.assertEqual(daf.row_idx_of('3'), -1)
     
-    def test_row_idx_of_no_keyfield(self):
-        # Test getting row index when no keyfield is defined
-        daf = Daf(lol=[['1', 'a'], ['2', 'b']], cols=['ID', 'Value'])
-        self.assertEqual(daf.row_idx_of('1'), -1)
+    # def test_row_idx_of_no_keyfield(self):
+        # # Test getting row index when no keyfield is defined
+        # daf = Daf(lol=[['1', 'a'], ['2', 'b']], cols=['ID', 'Value'])
+        # self.assertEqual(daf.row_idx_of('1'), -1)
     
-    def test_row_idx_of_no_kd(self):
-        # Test getting row index when kd is not available
-        daf = Daf(lol=[['1', 'a'], ['2', 'b']], cols=['ID', 'Value'], keyfield='ID')
-        daf.kd = None
-        self.assertEqual(daf.row_idx_of('1'), -1)
+    # def test_row_idx_of_no_kd(self):
+        # # Test getting row index when kd is not available
+        # daf = Daf(lol=[['1', 'a'], ['2', 'b']], cols=['ID', 'Value'], keyfield='ID')
+        # daf.kd = None
+        # self.assertEqual(daf.row_idx_of('1'), -1)
 
 
     # get_existing_keys
     def test_get_existing_keys_with_existing_keys(self):
         # Test case where all keys in keylist exist in kd
         daf = Daf(lol=[[1, 'a'], [2, 'b'], [3, 'c']], cols=['ID', 'Name'], keyfield='Name')
         existing_keys = daf.get_existing_keys(['a', 'b', 'd'])
@@ -1218,14 +1218,16 @@
         daf1 = Daf()
         daf2 = Daf()
 
         cols = ['col1', 'col2']
         hd = {'col1': 0, 'col2': 1}
         lol1 = [[1, 'a'], [2, 'b']]
         lol2 = [['x', 'y'], ['z', 'w']]
+        
+        # import pdb; pdb.set_trace() #temp
         daf1 = Daf(cols=cols, lol=lol1, keyfield='', dtypes={'col1': str, 'col2': str})
         daf2 = Daf(cols=cols, lol=lol2, keyfield='', dtypes={'col1': str, 'col2': str})
 
         daf1.append(daf2)
 
         self.assertEqual(daf1.name, '')
         self.assertEqual(daf1.keyfield, '')
@@ -2584,26 +2586,26 @@
 
     def test_daf_sum_selected_columns(self):
         cols = ['col1', 'col2', 'col3']
         lol = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes={'col1': int, 'col2': int, 'col3': int})
 
         result_sum = daf.daf_sum(cols=['col1', 'col3'])
-        expected_sum = {'col1': 12, 'col3': 18}
+        expected_sum = {'col1': 12, 'col2': '', 'col3': 18}
         self.assertEqual(result_sum, expected_sum)
 
     def test_daf_sum_include_types_int(self):
         cols = ['col1', 'col2', 'col3']
         dtypes_dict = {'col1': str, 'col2': int, 'col3': int}
         lol = [['a', 2, 3], ['b', 5, 6], ['c', 8, 9]]
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes=dtypes_dict)
 
         reduce_cols = daf.calc_cols(include_types=int)
         result_sum = daf.daf_sum(cols=reduce_cols)
-        expected_sum = {'col2': 15, 'col3': 18}
+        expected_sum = {'col1': '', 'col2': 15, 'col3': 18}
         self.assertEqual(result_sum, expected_sum)
 
     def test_daf_sum_include_types_int_and_float(self):
         cols = ['col1', 'col2', 'col3']
         dtypes_dict = {'col1': str, 'col2': int, 'col3': float}
         lol = [['a', 2, 3.2], ['b', 5, 6.1], ['c', 8, 9.4]]
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes=dtypes_dict)
@@ -2619,15 +2621,15 @@
         cols = ['col1', 'col2', 'col3']
         dtypes_dict = {'col1': str, 'col2': int, 'col3': int}
         lol = [['a', 2, 3], ['b', 5, 6], ['c', 8, 9]]
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes=dtypes_dict)
 
         reduce_cols = daf.calc_cols(exclude_types=[str, bool, list])
         result_sum = daf.daf_sum(cols=reduce_cols)
-        expected_sum = {'col2': 15, 'col3': 18}
+        expected_sum = {'col1': '', 'col2': 15, 'col3': 18}
         self.assertEqual(result_sum, expected_sum)
 
     def test_daf_sum_empty_daf(self):
         daf = Daf()
 
         result_sum = daf.daf_sum()
         expected_sum = {}
@@ -3841,9 +3843,95 @@
         # Call the set_lol method with the new lol
         self.daf.set_lol(new_lol)
 
         # Check if kd is recalculated
         self.assertIsNotNone(self.daf.kd)
         
 
+    # wide to narrow
+    def test_wide_to_narrow_conversion_basic(self):
+        # Initialize a wide Daffodil dataframe for testing
+        wide_daf = Daf(cols=['ID', 'A', 'B'], lol=[[1, 10, 100], [2, 20, 200], [3, 30, 300]])
+        
+        # Test if the method converts a wide DataFrame to a narrow format
+        narrow_daf = wide_daf.wide_to_narrow(id_cols=['ID'])
+        
+        # Check the exact content of the narrow DataFrame
+        expected_content = [
+            {'ID': 1, 'varname': 'A', 'value': 10},
+            {'ID': 1, 'varname': 'B', 'value': 100},
+            {'ID': 2, 'varname': 'A', 'value': 20},
+            {'ID': 2, 'varname': 'B', 'value': 200},
+            {'ID': 3, 'varname': 'A', 'value': 30},
+            {'ID': 3, 'varname': 'B', 'value': 300}
+        ]
+        self.assertEqual(len(narrow_daf), 6)  # Ensure correct number of rows
+        
+        # Check each row in the narrow DataFrame
+        for i, row in enumerate(narrow_daf):
+            self.assertDictEqual(row, expected_content[i])
+        
+        # Add more assertions based on the expected structure of the narrow DataFrame
+        
+        
+    # def test_wide_to_narrow_id_cols_handling_additional_columns(self):
+        # # Initialize a wide Daffodil dataframe for testing
+        # wide_daf = Daf(cols=['ID', 'A', 'B'], lol=[[1, 10, 100], [2, 20, 200], [3, 30, 300]])
+        
+        # # Test the handling of identifier columns
+        # narrow_daf = wide_daf.wide_to_narrow(id_cols=['ID', 'SomeOtherColumn'])
+        # self.assertEqual(len(narrow_daf.columns()), 4)  # ID, SomeOtherColumn, varname, value
+        
+        # # Add more assertions based on the expected handling of identifier columns
+        
+    def test_wide_to_narrow_input_data_types_invalid_id_cols(self):
+        # Initialize a wide Daffodil dataframe for testing
+        wide_daf = Daf(cols=['ID', 'A', 'B'], lol=[[1, 10, 100], [2, 20, 200], [3, 30, 300]])
+        
+        # Test the handling of different input data types
+        with self.assertRaises(TypeError):
+            wide_daf.wide_to_narrow(id_cols='ID')  # id_cols should be a list
+        
+        # Add more assertions based on the expected behavior with different data types
+
+    # narrow_to_wide
+    def test_narrow_to_wide_conversion_basic(self):
+        # Initialize a narrow Daffodil dataframe for testing
+        narrow_daf = Daf(
+                cols=['ID', 'varname', 'value'], 
+                lol=[[1, 'A', 10], 
+                    [1, 'B', 100], 
+                    [2, 'A', 20], 
+                    [2, 'B', 200], 
+                    [3, 'A', 30], 
+                    [3, 'B', 300]])
+        
+        # Test if the method converts a narrow DataFrame to a wide format
+        wide_daf = narrow_daf.narrow_to_wide(id_cols=['ID'], varname_col='varname', value_col='value')
+        
+        # Check the exact content of the wide DataFrame
+        expected_content = Daf(cols=['ID', 'A', 'B'], lol=[[1, 10, 100], [2, 20, 200], [3, 30, 300]])
+        self.assertEqual(wide_daf, expected_content)
+        
+        # Add more assertions based on the expected structure of the wide DataFrame
+        
+    def test_narrow_to_wide_id_cols_handling_additional_columns(self):
+        # Initialize a narrow Daffodil dataframe for testing
+        narrow_daf = Daf(
+                cols=['ID', 'varname', 'value'], 
+                lol=[[1, 'A', 10], 
+                    [1, 'B', 100], 
+                    [2, 'A', 20], 
+                    [2, 'B', 200], 
+                    [3, 'A', 30], 
+                    [3, 'B', 300]])
+        
+        # Test the handling of identifier columns
+        wide_daf = narrow_daf.narrow_to_wide(id_cols=['ID'], varname_col='varname', value_col='value')
+        self.assertEqual(len(wide_daf.columns()), 3)  # ID, A, B
+        
+        # Add more assertions based on the expected handling of identifier columns
+        
+
+
 if __name__ == '__main__':
     unittest.main()
```


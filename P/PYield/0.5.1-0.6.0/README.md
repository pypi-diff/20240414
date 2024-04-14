# Comparing `tmp/pyield-0.5.1.tar.gz` & `tmp/pyield-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyield-0.5.1.tar", last modified: Sun Apr  7 11:10:49 2024, max compression
+gzip compressed data, was "pyield-0.6.0.tar", last modified: Sat Apr 13 12:44:17 2024, max compression
```

## Comparing `pyield-0.5.1.tar` & `pyield-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.5.1/LICENSE
--rw-r--r--   0        0        0     3310 2024-04-07 11:09:13.991446 pyield-0.5.1/README.md
--rw-r--r--   0        0        0       22 2024-04-07 06:33:56.169777 pyield-0.5.1/pyield/__about__.py
--rw-r--r--   0        0        0      412 2024-04-07 06:33:13.009967 pyield-0.5.1/pyield/__init__.py
--rw-r--r--   0        0        0     8469 2024-04-07 11:02:46.452475 pyield-0.5.1/pyield/anbima.py
--rw-r--r--   0        0        0    12882 2024-04-07 10:34:38.993396 pyield-0.5.1/pyield/calendar.py
--rw-r--r--   0        0        0       78 2024-04-06 05:43:41.433643 pyield-0.5.1/pyield/di/__init__.py
--rw-r--r--   0        0        0     6977 2024-04-07 10:54:47.510769 pyield-0.5.1/pyield/di/core.py
--rw-r--r--   0        0        0     9701 2024-04-07 10:42:51.990316 pyield-0.5.1/pyield/di/web.py
--rw-r--r--   0        0        0     9557 2024-04-06 12:23:57.131890 pyield-0.5.1/pyield/di/xml.py
--rw-r--r--   0        0        0       55 2024-04-06 05:23:30.068485 pyield-0.5.1/pyield/holidays/__init__.py
--rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.5.1/pyield/holidays/br_holidays_new.txt
--rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.5.1/pyield/holidays/br_holidays_old.txt
--rw-r--r--   0        0        0     2192 2024-04-07 10:57:52.523509 pyield-0.5.1/pyield/holidays/core.py
--rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.5.1/pyield/py.typed
--rw-r--r--   0        0        0     1077 2024-04-07 11:10:49.438415 pyield-0.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0     1128 2024-04-06 05:41:13.954275 pyield-0.5.1/tests/test_br_calendar.py
--rw-r--r--   0        0        0     2491 2024-04-07 10:40:11.042085 pyield-0.5.1/tests/test_di.py
--rw-r--r--   0        0        0     5327 1970-01-01 00:00:00.000000 pyield-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4661 2024-04-13 12:39:44.026704 pyield-0.6.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-13 12:39:44.026704 pyield-0.6.0/pyield/__about__.py
+-rw-r--r--   0        0        0      334 2024-04-13 12:39:44.026704 pyield-0.6.0/pyield/__init__.py
+-rw-r--r--   0        0        0    13136 2024-04-13 12:39:44.026704 pyield-0.6.0/pyield/bday.py
+-rw-r--r--   0        0        0     1983 2024-04-13 12:39:44.026704 pyield-0.6.0/pyield/data_access.py
+-rw-r--r--   0        0        0     1250 2024-04-13 12:39:44.026704 pyield-0.6.0/pyield/data_analysis.py
+-rw-r--r--   0        0        0       90 2024-04-13 12:39:44.026704 pyield-0.6.0/pyield/di/__init__.py
+-rw-r--r--   0        0        0     6990 2024-04-13 12:39:44.026704 pyield-0.6.0/pyield/di/core.py
+-rw-r--r--   0        0        0     9638 2024-04-13 12:39:44.027704 pyield-0.6.0/pyield/di/web.py
+-rw-r--r--   0        0        0     9551 2024-04-13 12:39:44.027704 pyield-0.6.0/pyield/di/xml.py
+-rw-r--r--   0        0        0       55 2024-04-06 05:23:30.068485 pyield-0.6.0/pyield/holidays/__init__.py
+-rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.6.0/pyield/holidays/br_holidays_new.txt
+-rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.6.0/pyield/holidays/br_holidays_old.txt
+-rw-r--r--   0        0        0     2192 2024-04-07 10:57:52.523509 pyield-0.6.0/pyield/holidays/core.py
+-rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.6.0/pyield/py.typed
+-rw-r--r--   0        0        0     7294 2024-04-13 12:39:44.027704 pyield-0.6.0/pyield/treasuries.py
+-rw-r--r--   0        0        0      969 2024-04-13 12:39:44.027704 pyield-0.6.0/pyield/utils.py
+-rw-r--r--   0        0        0     1165 2024-04-13 12:44:17.075633 pyield-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     1114 2024-04-13 12:39:44.028704 pyield-0.6.0/tests/test_br_calendar.py
+-rw-r--r--   0        0        0     2503 2024-04-13 12:39:44.028704 pyield-0.6.0/tests/test_di.py
+-rw-r--r--   0        0        0     6678 1970-01-01 00:00:00.000000 pyield-0.6.0/PKG-INFO
```

### Comparing `pyield-0.5.1/LICENSE` & `pyield-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyield-0.5.1/pyield/anbima.py` & `pyield-0.6.0/pyield/treasuries.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,22 @@
 import io
 
 import pandas as pd
 import requests
 
 from . import di
-from . import calendar as cl
 
 # URL Constants
 ANBIMA_NON_MEMBER_URL = "https://www.anbima.com.br/informacoes/merc-sec/arqs/"
 ANBIMA_MEMBER_URL = "http://www.anbima.associados.rtm/merc_sec/arqs/"
 
 # Constant for conversion to basis points
 BPS_CONVERSION_FACTOR = 10_000
 
 
-def _normalize_date(reference_date: str | pd.Timestamp | None = None) -> pd.Timestamp:
-    if isinstance(reference_date, str):
-        normalized_date = pd.Timestamp(reference_date).normalize()
-    elif isinstance(reference_date, pd.Timestamp):
-        normalized_date = reference_date.normalize()
-    elif reference_date is None:
-        today = pd.Timestamp.today().normalize()
-        # Get last business day before today
-        normalized_date = cl.offset_bdays(today, -1)
-    else:
-        raise ValueError("Invalid date format.")
-
-    # Raise an error if the reference date is in the future
-    if normalized_date > pd.Timestamp.today().normalize():
-        raise ValueError("Reference date cannot be in the future.")
-
-    # Raise error if the reference date is not a business day
-    if not cl.is_bday(normalized_date):
-        raise ValueError("Reference date must be a business day.")
-
-    return normalized_date
-
-
 def _get_anbima_content(reference_date: pd.Timestamp) -> str:
     url_date = reference_date.strftime("%y%m%d")
     member_url = f"{ANBIMA_MEMBER_URL}ms{url_date}.txt"
     non_member_url = f"{ANBIMA_NON_MEMBER_URL}ms{url_date}.txt"
 
     # Tries to access the member URL first
     try:
@@ -58,15 +34,15 @@
         response.raise_for_status()  # Checks if the second attempt was successful
         return response.text
     except requests.exceptions.RequestException:
         # Both URLs failed
         return ""
 
 
-def _get_raw_data(reference_date: pd.Timestamp) -> pd.DataFrame:
+def _get_raw_df(reference_date: pd.Timestamp) -> pd.DataFrame:
     url_content = _get_anbima_content(reference_date)
     if url_content == "":
         date_str = reference_date.strftime("%d-%m-%Y")
         raise ValueError(f"Could not fetch ANBIMA data for {date_str}.")
 
     df = pd.read_csv(
         io.StringIO(url_content),
@@ -77,17 +53,18 @@
         thousands=".",
         na_values=["--"],
         dtype_backend="numpy_nullable",
     )
     return df
 
 
-def _process_raw_data(df_raw: pd.DataFrame) -> pd.DataFrame:
+def _process_raw_df(df_raw: pd.DataFrame) -> pd.DataFrame:
     """
-    Process raw data from ANBIMA by filtering selected columns, renaming them, and adjusting data formats.
+    Process raw data from ANBIMA by filtering selected columns, renaming them and
+    adjusting data formats.
 
     Parameters:
     - df (pd.DataFrame): Raw data DataFrame to process.
 
     Returns:
     - pd.DataFrame: Processed DataFrame.
     """
@@ -119,98 +96,96 @@
 
     df["ReferenceDate"] = pd.to_datetime(df["ReferenceDate"], format="%Y%m%d")
     df["MaturityDate"] = pd.to_datetime(df["MaturityDate"], format="%Y%m%d")
 
     return df.sort_values(["BondType", "MaturityDate"], ignore_index=True)
 
 
-def get_treasury_rates(
-    reference_date: str | pd.Timestamp | None = None,
-    return_raw=False,
-) -> pd.DataFrame:
-    """
-    Fetches and processes indicative treasury rates from ANBIMA for a specified reference date.
-
-    This function retrieves the indicative rates for Brazilian treasury securities from ANBIMA,
-    processing them into a structured pandas DataFrame. If no reference date is provided, it defaults
-    to the previous business day according to the Brazilian calendar. There is an option to return
-    raw data directly from the source without processing.
+def fetch_data(reference_date: pd.Timestamp, return_raw=False) -> pd.DataFrame:
+    """
+    Fetches indicative treasury rates from ANBIMA for a specified reference date.
+
+    This function retrieves the indicative rates for Brazilian treasury securities
+    from ANBIMA, processing them into a structured pandas DataFrame. If no reference
+    date is provided, it defaults to the previous business day according to the
+    Brazilian calendar. There is an option to return raw data directly from the source
+    without processing.
 
     Parameters:
-        reference_date (str | pd.Timestamp, optional): The date for which to fetch the indicative rates.
-            If None or not provided, the function defaults to the previous business day.
-        return_raw (bool, optional): Flag to return raw data without processing. Defaults to False.
+        reference_date (str | pd.Timestamp, optional): The date for which to fetch the
+            indicative rates. If None or not provided, the function defaults to the
+            previous business day.
+        return_raw (bool, optional): Flag to return raw data without processing.
+            Defaults to False.
 
     Returns:
-        pd.DataFrame: A DataFrame containing the processed indicative rates for the given reference date,
-        or raw data if `return_raw` is True. The processed data includes bond type, reference date, maturity date,
-        and various rates (bid, ask, indicative) among others, depending on the `return_raw` flag.
+        pd.DataFrame: A DataFrame containing the processed indicative rates for the
+            given reference date, or raw data if `return_raw` is True. The processed
+            data includes bond type, reference date, maturity date and various rates
+            (bid, ask, indicative) among others, depending on the `return_raw` flag.
 
     Examples:
         # Fetch processed indicative rates for the previous business day
         >>> get_treasury_rates()
 
         # Fetch raw indicative rates for a specific date
         >>> get_treasury_rates("2023-12-28")
     """
-
-    normalized_date = _normalize_date(reference_date)
-    df = _get_raw_data(normalized_date)
+    df = _get_raw_df(reference_date)
 
     if not return_raw:
-        df = _process_raw_data(df)
+        df = _process_raw_df(df)
 
     return df
 
 
-def calculate_treasury_di_spreads(
-    reference_date: str | pd.Timestamp | None = None,
-) -> pd.DataFrame:
-    """
-    Calculates the DI spread for Brazilian treasury bonds (LTN and NTN-F) based on ANBIMA's indicative rates.
-
-    This function fetches the indicative rates for Brazilian treasury securities (LTN and NTN-F bonds)
-    and the DI futures rates for a specified reference date, calculating the spread between these rates
-    in basis points. If no reference date is provided, the function uses the previous business day.
+def calculate_di_spreads(reference_date: pd.Timestamp) -> pd.DataFrame:
+    """
+    Calculates the DI spread for Brazilian treasury bonds (LTN and NTN-F) based on
+    ANBIMA's indicative rates.
+
+    This function fetches the indicative rates for Brazilian treasury securities (LTN
+    and NTN-F bonds) and the DI futures rates for a specified reference date,
+    calculating the spread between these rates in basis points. If no reference date is
+    provided, the function uses the previous business day.
 
     Parameters:
-        reference_date (str | pd.Timestamp, optional): The reference date for the DI spread calculation.
-            If None or not provided, defaults to the previous business day according to the Brazilian calendar.
+        reference_date (str | pd.Timestamp, optional): The reference date for the DI
+            spread calculation. If None or not provided, defaults to the previous
+            business day according to the Brazilian calendar.
 
     Returns:
-        pd.DataFrame: A DataFrame containing the bond type, reference date, maturity date, and the calculated
-        DI spread in basis points. The data is sorted by bond type and maturity date.
+        pd.DataFrame: A DataFrame containing the bond type, reference date, maturity
+            date, and the calculated DI spread in basis points. The data is sorted by
+            bond type and maturity date.
 
     Examples:
         # Calculate DI spreads for the previous business day
         >>> calculate_treasury_di_spreads()
 
         # Calculate DI spreads for a specific reference date
         >>> calculate_treasury_di_spreads("2023-12-15")
     """
-    # Validate the reference date, defaulting to the previous business day if not provided
-    normalized_date = _normalize_date(reference_date)
-
     # Fetch DI rates and adjust the maturity date format for compatibility
-    df_di = di.get_di(normalized_date)[["ExpirationDate", "SettlementRate"]]
+    df_di = di.fetch_data(reference_date)[["ExpirationDate", "SettlementRate"]]
 
     # Renaming the columns to match the ANBIMA structure
     df_di.rename(columns={"ExpirationDate": "MaturityDate"}, inplace=True)
 
     # Adjusting maturity date to match bond data format
     df_di["MaturityDate"] = df_di["MaturityDate"].dt.to_period("M").dt.to_timestamp()
 
     # Fetch bond rates, filtering for LTN and NTN-F types
-    df_anbima = get_treasury_rates(normalized_date, False)
+    df_anbima = fetch_data(reference_date, False)
     df_anbima.query("BondType in ['LTN', 'NTN-F']", inplace=True)
 
     # Merge bond and DI rates by maturity date to calculate spreads
     df_final = pd.merge(df_anbima, df_di, how="left", on="MaturityDate")
 
-    # Calculating the DI spread as the difference between indicative and settlement rates
+    # Calculate the DI spread as the difference between indicative and settlement rates
     df_final["DISpread"] = df_final["IndicativeRate"] - df_final["SettlementRate"]
 
     # Convert spread to basis points for clarity
     df_final["DISpread"] = (BPS_CONVERSION_FACTOR * df_final["DISpread"]).round(2)
 
     # Prepare and return the final sorted DataFrame
     select_columns = ["BondType", "ReferenceDate", "MaturityDate", "DISpread"]
```

### Comparing `pyield-0.5.1/pyield/calendar.py` & `pyield-0.6.0/pyield/bday.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-from typing import Literal, overload, Union
 from datetime import datetime
+from typing import Literal, overload
 
 import numpy as np
 import pandas as pd
 
-
 from .holidays import BrHolidays
 
-
-SingleDateTypes = Union[str, np.datetime64, pd.Timestamp, datetime]
-
-SeriesDateTypes = Union[list, tuple, np.ndarray, pd.Series, pd.Index, pd.DatetimeIndex]
+SingleDateTypes = str | np.datetime64 | pd.Timestamp | datetime
+SeriesDateTypes = list | tuple | np.ndarray | pd.Series | pd.Index | pd.DatetimeIndex
 
 TO_TIMESTAMP_TYPES = (str, np.datetime64, datetime)
 TO_SERIES_TYPES = (list, tuple, np.ndarray, pd.Series, pd.Index, pd.DatetimeIndex)
 
 # Initialize the BrHolidays class
 br_holidays = BrHolidays()
 
@@ -109,33 +106,41 @@
 def offset_bdays(
     dates: SingleDateTypes | SeriesDateTypes | None = None,
     offset: int = 0,
     roll: Literal["forward", "backward"] = "forward",
     holiday_list: Literal["old", "new", "infer"] = "infer",
 ) -> pd.Timestamp | pd.Series:
     """
-    Offsets the dates to the next or previous business day, considering brazilian holidays.
-    This function supports both single dates and collections of dates, handling them
-    intelligently to return either a single offset date or a series of offset dates.
-    It is a wrapper for `numpy.busday_offset` adapted for Pandas data types and holiday adjustments.
+    Offsets the dates to the next or previous business day, considering brazilian
+    holidays. This function supports both single dates and collections of dates,
+    handling them intelligently to return either a single offset date or a series of
+    offset dates. It is a wrapper for `numpy.busday_offset` adapted for Pandas data
+    types and holiday adjustments.
 
     Args:
-        dates (str | np.datetime64 | pd.Timestamp | datetime | list | tuple | np.ndarray | pd.Series | pd.Index | pd.DatetimeIndex, optional):
-            The date(s) to offset. Can be a single date in various formats (string, `datetime`, `Timestamp`, etc.)
-            or a collection of dates (list, tuple, `Series`, etc.). If None, the current date is used.
-        offset (int): The number of business days to offset the dates. Positive for future dates, negative for past dates.
-            Zero will return the same date if it's a business day, or the next business day otherwise.
-        roll (Literal["forward", "backward"], optional): Direction to roll the date if it falls on a holiday or weekend.
-            'forward' to the next business day, 'backward' to the previous. Defaults to 'forward'.
-        holiday_list (Literal["old", "new", "infer"], optional): The list of holidays to consider. 'old' or 'new' use predefined lists,
-            while 'infer' determines the most appropriate list based on the input dates. Defaults to "infer".
+        dates (str | np.datetime64 | pd.Timestamp | datetime | list | tuple | np.ndarray
+        | pd.Series | pd.Index | pd.DatetimeIndex, optional):
+            The date(s) to offset. Can be a single date in various formats (string,
+            `datetime`, `Timestamp`, etc.) or a collection of dates (list, tuple,
+            `Series`, etc.). If None, the current date is used.
+        offset (int): The number of business days to offset the dates. Positive for
+            future dates, negative for past dates. Zero will return the same date if
+            it's a business day, or the next business day otherwise.
+        roll (Literal["forward", "backward"], optional): Direction to roll the date if
+            it falls on a holiday or weekend. 'forward' to the next business day,
+            'backward' to the previous. Defaults to 'forward'.
+        holiday_list (Literal["old", "new", "infer"], optional):
+            The list of holidays to consider. 'old' or 'new' use predefined lists, while
+            'infer' determines the most appropriate list based on the input dates.
+            Defaults to "infer".
 
     Returns:
-         pd.Timestamp | pd.Series: If a single date is provided, returns a single `Timestamp` of the offset date.
-            If a series of dates is provided, returns a `Series` of offset dates.
+         pd.Timestamp | pd.Series: If a single date is provided, returns a single
+            `Timestamp` of the offset date. If a series of dates is provided, returns a
+            `Series` of offset dates.
 
     Examples:
         >>> date = '2023-12-23' # Saturday before Christmas
         >>> yd.offset_bdays(date, 0)
         Timestamp('2023-12-26')
 
         >>> date = '2023-12-22' # Friday before Christmas
@@ -145,16 +150,17 @@
         >>> yd.offset_bdays(date, 1)
         Timestamp('2023-12-26') # Offset to the next business day
 
         >>> yd.offset_bdays(date, -1)
         Timestamp('2023-12-21') # Offset to the previous business day
 
     Note:
-        This function uses `numpy.busday_offset` under the hood, which means it follows the same conventions and limitations
-        for business day calculations. For detailed information on error handling and behavior, refer to the `numpy.busday_offset`
+        This function uses `numpy.busday_offset` under the hood, which means it follows
+        the same conventions and limitations for business day calculations. For detailed
+        information on error handling and behavior, refer to the `numpy.busday_offset`
         documentation: https://numpy.org/doc/stable/reference/generated/numpy.busday_offset.html
     """
     normalized_dates = _normalize_input_dates(dates)
 
     selected_holidays = br_holidays.get_applicable_holidays(
         normalized_dates, holiday_list
     )
@@ -205,38 +211,48 @@
 
 def count_bdays(
     start: SingleDateTypes | SeriesDateTypes | None = None,
     end: SingleDateTypes | SeriesDateTypes | None = None,
     holiday_list: Literal["old", "new", "infer"] = "infer",
 ) -> int | pd.Series:
     """
-    Counts the number of business days between a `start` and `end` date(s), inclusively for
-    the start date and exclusively for the end date. The function can handle single dates,
-    arrays of dates, and mixed inputs, returning either a single integer or a Series
-    depending on the inputs. It accounts for specified holidays, effectively excluding
-    them from the business day count.
+    Counts the number of business days between a `start` and `end` date(s), inclusively
+    for the start date and exclusively for the end date. The function can handle single
+    dates, arrays of dates, and mixed inputs, returning either a single integer or a
+    Series depending on the inputs. It accounts for specified holidays, effectively
+    excluding them from the business day count.
 
     Args:
-        start (str | np.datetime64 | pd.Timestamp | datetime | list | tuple | np.ndarray | pd.Series | pd.Index | pd.DatetimeIndex, optional):
+        start (str | np.datetime64 | pd.Timestamp | datetime | list | tuple |
+            np.ndarray | pd.Series | pd.Index | pd.DatetimeIndex, optional):
             The start date(s) for counting. Defaults to the current date if None.
-        end (str | np.datetime64 | pd.Timestamp | datetime | list | tuple | np.ndarray | pd.Series | pd.Index | pd.DatetimeIndex, optional):
-            The end date(s) for counting, which are excluded from the count themselves. Defaults to the current date if None.
+        end (str | np.datetime64 | pd.Timestamp | datetime | list | tuple |
+            np.ndarray | pd.Series | pd.Index | pd.DatetimeIndex, optional):
+            The end date(s) for counting, which are excluded from the count themselves.
+            Defaults to the current date if None.
         holiday_list (Literal["old", "new", "infer"], optional):
-            Specifies which set of holidays to consider in the count. 'old' or 'new' refer to predefined holiday lists,
-            while 'infer' automatically selects the list based on the most recent date in the input. Defaults to "infer".
+            Specifies which set of holidays to consider in the count. 'old' or 'new'
+            refer to predefined holiday lists, while 'infer' automatically selects the
+            list based on the most recent date in the input. Defaults to "infer".
 
     Returns:
         int | pd.Series: Returns an integer if `start` and `end` are single dates,
-            or a Series if either or both are arrays of dates. The value(s) represent the count of business days between `start` and `end`.
+            or a Series if either or both are arrays of dates. The value(s) represent
+            the count of business days between `start` and `end`.
 
     Notes:
-        - This function is a wrapper around `numpy.busday_count`, adapted to work directly with various Pandas and Numpy date formats.
-        - It supports flexible date inputs, including single dates, lists, Series, and more, for both `start` and `end` parameters.
-        - The return type depends on the input types: single dates return an int, while arrays of dates return a pd.Series with the count for each date range.
-        - See `numpy.busday_count` documentation for more details on how holidays are handled and how business day counts are calculated: https://numpy.org/doc/stable/reference/generated/numpy.busday_count.html.
+        - This function is a wrapper around `numpy.busday_count`, adapted to work
+          directly with various Pandas and Numpy date formats.
+        - It supports flexible date inputs, including single dates, lists, Series, and
+          more, for both `start` and `end` parameters.
+        - The return type depends on the input types: single dates return an int, while
+          arrays of dates return a pd.Series with the count for each date range.
+        - See `numpy.busday_count` documentation for more details on how holidays are
+          handled and how business day counts are calculated:
+          https://numpy.org/doc/stable/reference/generated/numpy.busday_count.html.
 
     Examples:
         >>> yd.count_bdays('2023-12-15', '2024-01-01')
         10
 
         >>> start = '2023-01-01'
         >>> end = pd.to_datetime(['2023-01-31', '2023-03-01'])
@@ -273,36 +289,42 @@
     """
     Generates a Series of business days between a `start` and `end` date, considering
     the list of Brazilian holidays. It supports customization of holiday lists and
     inclusion options for start and end dates. It wraps `pandas.bdate_range`.
 
     Args:
         start (str | np.datetime64 | pd.Timestamp | datetime, optional):
-            The start date for generating business days. Defaults to None, using the current date.
+            The start date for generating business days. Defaults to None, using the
+            current date.
         end (str | np.datetime64 | pd.Timestamp | datetime, optional):
-            The end date for generating business days. Defaults to None, using the current date.
+            The end date for generating business days. Defaults to None, using the
+            current date.
         inclusive (Literal["both", "neither", "left", "right"], optional):
             Determines which of the start and end dates are included in the result.
             Valid options are 'both', 'neither', 'left', 'right'. Defaults to 'both'.
         holiday_list (Literal["old", "new", "infer"], optional):
-            Specifies the list of holidays to consider. 'old' or 'new' refer to predefined lists,
-            'infer' selects the list based on the most recent date in the range. Defaults to "infer".
+            Specifies the list of holidays to consider. 'old' or 'new' refer to
+            predefined lists, 'infer' selects the list based on the most recent date in
+            the range. Defaults to "infer".
         **kwargs:
-            Additional keyword arguments passed to `pandas.bdate_range` for customization.
+            Additional keyword arguments passed to `pandas.bdate_range` for
+            customization.
 
     Returns:
-        pd.Series: A Series representing a range of business days between the specified start and end dates,
-            considering the specified holidays.
+        pd.Series: A Series representing a range of business days between the specified
+            start and end dates, considering the specified holidays.
 
     Examples:
         >>> yd.generate_bdays(start='2023-12-22', end='2024-01-02')
-        pd.Series(['2023-12-22', '2023-12-26', '2023-12-27', '2023-12-28', '2023-12-29', '2024-01-02'], dtype='datetime64[ns]')
+        pd.Series(['2023-12-22', '2023-12-26', '2023-12-27', '2023-12-28', '2023-12-29',
+            '2024-01-02'], dtype='datetime64[ns]')
 
     Note:
-        For detailed information on parameters and error handling, refer to `pandas.bdate_range` documentation:
+        For detailed information on parameters and error handling, refer to
+        `pandas.bdate_range` documentation:
         https://pandas.pydata.org/docs/reference/api/pandas.bdate_range.html.
     """
     normalized_start = _normalize_input_dates(start)
     normalized_end = _normalize_input_dates(end)
 
     selected_holidays = br_holidays.get_applicable_holidays(
         normalized_start, holiday_list
```

### Comparing `pyield-0.5.1/pyield/di/core.py` & `pyield-0.6.0/pyield/di/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-from typing import Literal
 from pathlib import Path
+from typing import Literal
 
 import pandas as pd
 
-from . import web
-from . import xml
-from .. import calendar as cl
+from .. import bday
+from . import web, xml
 
 
 def _normalize_date(trade_date: str | pd.Timestamp | None = None) -> pd.Timestamp:
     if isinstance(trade_date, str):
         normalized_date = pd.Timestamp(trade_date).normalize()
     elif isinstance(trade_date, pd.Timestamp):
         normalized_date = trade_date.normalize()
     elif trade_date is None:
         today = pd.Timestamp.today().normalize()
         # Get last business day before today
-        normalized_date = cl.offset_bdays(today, -1)
+        normalized_date = bday.offset_bdays(today, -1)
     else:
         raise ValueError("Invalid date format.")
 
     # Raise an error if the trade date is in the future
     if normalized_date > pd.Timestamp.today().normalize():
         raise ValueError("Trade date cannot be in the future.")
 
     # Raise error if the reference date is not a business day
-    if not cl.is_bday(normalized_date):
+    if not bday.is_bday(normalized_date):
         raise ValueError("Trade date must be a business day.")
 
     return normalized_date
 
 
 def get_expiration_date(expiration_code: str) -> pd.Timestamp:
     """
@@ -83,48 +82,50 @@
         month_code = expiration_code[0]
         month = month_codes[month_code]
         year = int("20" + expiration_code[-2:])
         # The expiration date is always the first business day of the month
         expiration = pd.Timestamp(year, month, 1)
 
         # Adjust to the next business day when expiration date is a weekend or a holiday
-        adj_expiration = cl.offset_bdays(expiration, offset=0)
+        adj_expiration = bday.offset_bdays(expiration, offset=0)
 
         return adj_expiration
 
     except (KeyError, ValueError):
-        raise ValueError("Invalid expiration code.")
+        return pd.NaT  # type: ignore
 
 
-def get_di(
+def fetch_data(
     trade_date: str | pd.Timestamp | None = None,
     source_type: Literal["bmf", "b3", "b3s"] = "bmf",
     return_raw: bool = False,
 ) -> pd.DataFrame:
     """
     Fetches DI futures data for a specified trade date from B3.
 
-     Retrieves and processes DI futures data from B3 for a given trade date. This function
-     serves as the primary method for accessing DI data, with options to specify the source
-     of the data and whether to return raw data.
+     Retrieves and processes DI futures data from B3 for a given trade date. This
+     function serves as the primary method for accessing DI data, with options to
+     specify the source of the data and whether to return raw data.
 
      Args:
-         trade_date (str | pd.Timestamp | None, optional): The trade date for which to
-             fetch DI data. If None or not provided, uses the previous business day.
-         source_type (Literal["bmf", "b3", "b3s"], optional): Indicates the source of the
-             data. Options include:
-             - "bmf": Fetches data from the old BM&FBOVESPA website. Fastest option.
-             - "b3": Fetches data from the complete Price Report (XML file) provided by B3.
-             - "b3s": Fetches data from the simplified Price Report (XML file) provided by B3.
-               Faster than "b3" but less detailed.
-             Defaults to "bmf".
-         return_raw (bool, optional): If True, returns the raw DI data without processing.
+        trade_date (str | pd.Timestamp | None, optional): The trade date for which to
+            fetch DI data. If None or not provided, uses the previous business day.
+        source_type (Literal["bmf", "b3", "b3s"], optional): Indicates the source of
+            the data. Defaults to "bmf". Options include:
+                - "bmf": Fetches data from the old BM&FBOVESPA website. Fastest option.
+                - "b3": Fetches data from the complete Price Report (XML file) provided
+                    by B3.
+                - "b3s": Fetches data from the simplified Price Report (XML file)
+                    provided by B3. Faster than "b3" but less detailed.
+        return_raw (bool, optional): If True, returns the raw DI data without
+            processing.
 
      Returns:
-         pd.DataFrame: A DataFrame containing the DI futures data for the specified trade
+         pd.DataFrame: A DataFrame containing the DI futures data for the specified
+         trade
              date. Format and content depend on the source_type and return_raw flag.
 
      Examples:
          # Fetch DI data for the previous business day using default settings
          >>> get_di()
 
          # Fetch DI data for a specific trade date from the simplified B3 Price Report
@@ -137,20 +138,20 @@
     """
     # Force trade_date to be a pandas pd.Timestamp
     normalized_trade_date = _normalize_date(trade_date)
 
     if source_type == "bmf":
         return web.get_di(normalized_trade_date, return_raw)
     elif source_type in ["b3", "b3s"]:
-        return xml.get_di(normalized_trade_date, source_type, return_raw)
+        return xml.read_xml(normalized_trade_date, source_type, return_raw)
     else:
         raise ValueError("source_type must be either 'bmf', 'b3' or 'b3s'.")
 
 
-def read_di(file_path: Path, return_raw: bool = False) -> pd.DataFrame:
+def read_data(file_path: Path, return_raw: bool = False) -> pd.DataFrame:
     """
     Reads DI futures data from a file and returns it as a pandas DataFrame.
 
     This function opens and reads a DI futures data file, returning the contents as a
     pandas DataFrame. It supports reading from both XML files provided by B3, wich
     are the simplified and complete Price Reports.
```

### Comparing `pyield-0.5.1/pyield/di/web.py` & `pyield-0.6.0/pyield/di/web.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 import io
 import warnings
-from typing import Optional
 
 import pandas as pd
 import requests
 
-from .. import calendar as cl
+from .. import bday
 from . import core as cr
 
 
 def get_old_expiration_date(
-    ExpirationCode: str, trade_date: pd.Timestamp
-) -> Optional[pd.Timestamp]:
+    expiration_code: str, trade_date: pd.Timestamp
+) -> pd.Timestamp:
     """
-    Internal function to convert an old DI contract code into its ExpirationDate date. Valid for
-    contract codes up to 21-05-2006.
+    Internal function to convert an old DI contract code into its ExpirationDate date.
+    Valid for contract codes up to 21-05-2006.
 
     Args:
-        ExpirationCode (str):
-            An old DI ExpirationCode from B3, where the first three letters represent
-            the month and the last digit represents the year. Example: "JAN3".
-        trade_date (pd.Timestamp):
-            The trade date for which the contract code is valid.
+        expiration_code (str): An old DI Expiration Code from B3, where the first three
+            letters represent the month and the last digit represents the year.
+            Example: "JAN3".
+        trade_date (pd.Timestamp): The trade date for which the contract code is valid.
 
     Returns:
         pd.Timestamp
-            The contract's ExpirationDate date.
-            Returns pd.NaT if the input is invalid.
+            The contract's ExpirationDate date. Returns pd.NaT if the input is invalid.
 
     Examples:
         >>> get_old_expiration_date("JAN3", pd.Timestamp("2001-05-21"))
         pd.Timestamp('2003-01-01')
+
     Notes:
-        - In 22-05-2006, B3 changed the format of the DI contract codes. Before that date,
-          the first three letters represented the month and the last digit represented the
-          year.
+        - In 22-05-2006, B3 changed the format of the DI contract codes. Before that
+        date, the first three letters represented the month and the last digit
+        represented the year.
     """
 
     month_codes = {
         "JAN": 1,
         "FEV": 2,
         "MAR": 3,
         "ABR": 4,
@@ -48,34 +46,34 @@
         "AGO": 8,
         "SET": 9,
         "OUT": 10,
         "NOV": 11,
         "DEZ": 12,
     }
     try:
-        month_code = ExpirationCode[:3]
+        month_code = expiration_code[:3]
         month = month_codes[month_code]
 
-        # Year codes must generated dynamically, since it depends on the trade date
+        # Year codes must generated dynamically, since it depends on the trade date.
         reference_year = trade_date.year
         year_codes = {}
         for year in range(reference_year, reference_year + 10):
             year_codes[str(year)[-1:]] = year
-        year = year_codes[ExpirationCode[-1:]]
+        year = year_codes[expiration_code[-1:]]
 
-        ExpirationDate = pd.Timestamp(year, month, 1)
-        # Adjust to the next business day when ExpirationDate date is a weekend or a holiday
-        # Must use the old holiday calendar, since this type of contract code was used until 2006
-        return cl.offset_bdays(ExpirationDate, offset=0, holiday_list="old")
+        expiration_date = pd.Timestamp(year, month, 1)
+        # Adjust to the next business day when the date is a weekend or a holiday.
+        # Must use old holiday list, since this contract code was used until 2006.
+        return bday.offset_bdays(expiration_date, offset=0, holiday_list="old")
 
     except (KeyError, ValueError):
         return pd.NaT  # type: ignore
 
 
-def _get_raw_di(trade_date: pd.Timestamp) -> pd.DataFrame:
+def _get_raw_df(trade_date: pd.Timestamp) -> pd.DataFrame:
     """
     Internal function to fetch raw DI futures data from B3 for a specific trade date.
 
     Args:
         trade_date: a datetime-like object representing the trade date.
 
     Returns:
@@ -100,36 +98,37 @@
 
         # Remove rows with all NaN values
         df = df.dropna(how="all")
 
         # Remove columns with all NaN values
         df = df.dropna(axis=1, how="all")
 
-        # Force "VAR. PTOS." column to be string, since it can vary between str and float
+        # Force "VAR. PTOS." to be string, since it can also be read as float
         df["VAR. PTOS."] = df["VAR. PTOS."].astype(pd.StringDtype())
 
-        # Force "AJUSTE CORRIG. (4)" column to be float, since it can vary between int and float
+        # Force "AJUSTE CORRIG. (4)" to be float, since it can be also read as int
         df["AJUSTE CORRIG. (4)"] = df["AJUSTE CORRIG. (4)"].astype(pd.Float64Dtype())
 
         return df
 
     except Exception as e:
-        warnings.warn(
-            f"A {type(e).__name__} occurred while reading the DI futures data for {trade_date.strftime('%d/%m/%Y')}. Returning an empty pd.DataFrame."
-        )
+        trade_date_str = trade_date.strftime("%d/%m/%Y")
+        message = f"""A {type(e).__name__} occurred while reading the DI futures data
+        for {trade_date_str}. Returning an empty pd.DataFrame."""
+        warnings.warn(message, stacklevel=2)
         return pd.DataFrame()
 
 
 def _convert_prices_to_rates(prices: pd.Series, bd: pd.Series) -> pd.Series:
     """
     Internal function to convert DI futures prices to rates.
 
     Args:
         prices (pd.Series): A pd.Series containing DI futures prices.
-        bd (pd.Series): A pd.Series containing the number of business days to ExpirationDate.
+        bd (pd.Series): A serie containing the number of business days to expiration.
 
     Returns:
         pd.Series: A pd.Series containing DI futures rates.
     """
     rates = (100_000 / prices) ** (252 / bd) - 1
 
     # Return rates as percentage
@@ -152,15 +151,15 @@
 
     # Invert low and high prices
     df["MinRate"], df["MaxRate"] = df["MaxRate"], df["MinRate"]
 
     return df
 
 
-def _process_di(df: pd.DataFrame, trade_date: pd.Timestamp) -> pd.DataFrame:
+def _process_raw_df(df: pd.DataFrame, trade_date: pd.Timestamp) -> pd.DataFrame:
     """
     Internal function to process and transform raw DI futures data.
 
     Args:
         df (pd.DataFrame): the raw DI DataFrame.
         trade_date: a datetime-like object representing the trade date.
 
@@ -202,15 +201,15 @@
     if trade_date < pd.Timestamp("2006-05-22"):
         df["ExpirationDate"] = df["ExpirationCode"].apply(
             get_old_expiration_date, args=(trade_date,)
         )
     else:
         df["ExpirationDate"] = df["ExpirationCode"].apply(cr.get_expiration_date)
 
-    df["BDToExpiration"] = cl.count_bdays(trade_date, df["ExpirationDate"])
+    df["BDToExpiration"] = bday.count_bdays(trade_date, df["ExpirationDate"])
     # Convert to nullable integer, since other columns use this data type
     df["BDToExpiration"] = df["BDToExpiration"].astype(pd.Int64Dtype())
     # Remove expired contracts
     df.query("BDToExpiration > 0", inplace=True)
 
     # Columns where 0 means NaN
     cols_with_nan = [
@@ -220,26 +219,26 @@
         "MaxRate",
         "AvgRate",
         "LastRate",
         "LastBidRate",
         "LastAskRate",
     ]
     for col in cols_with_nan:
-        df[cols_with_nan] = df[cols_with_nan].replace(0, pd.NA)
+        df[col] = df[col].replace(0, pd.NA)
 
     # Prior to 17/01/2002 (incluive), prices were not converted to rates
     if trade_date <= pd.Timestamp("2002-01-17"):
         df = _convert_prices_in_older_contracts(df)
 
     df["SettlementRate"] = _convert_prices_to_rates(
         df["SettlementPrice"], df["BDToExpiration"]
     )
 
-    # Remove percentage in all rate columns and round to 5 decimal places since it's the precision used by B3
-    # Obs: 5 decimal places = 3 decimal places in percentage
+    # Remove percentage in all rate columns and round to 5 decimal places since it's the
+    # precision used by B3. Obs: 5 decimal places = 3 decimal places in percentage
     rate_cols = [col for col in df.columns if "Rate" in col]
     for col in rate_cols:
         df[col] = (df[col] / 100).round(5)
 
     # Filter and order columns
     ordered_cols = [
         "TradeDate",
@@ -284,11 +283,11 @@
         >>> get_di("2023-12-28")
 
     Notes:
         - BDToExpiration: number of business days to ExpirationDate.
         - OpenContracts: number of open contracts at the start of the trading day.
         - closed_contracts: number of closed contracts at the end of the trading day.
     """
-    df_raw = _get_raw_di(trade_date)
+    df_raw = _get_raw_df(trade_date)
     if return_raw:
         return df_raw
-    return _process_di(df_raw, trade_date)
+    return _process_raw_df(df_raw, trade_date)
```

### Comparing `pyield-0.5.1/pyield/di/xml.py` & `pyield-0.6.0/pyield/di/xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import io
 import zipfile
 from pathlib import Path
 
-import requests
 import pandas as pd
-from pandas import Timestamp, DataFrame
+import requests
 from lxml import etree
+from pandas import DataFrame, Timestamp
 
+from .. import bday
 from . import core as cr
-from .. import calendar as cd
 
 
 def _get_file_from_url(trade_date: Timestamp, source_type: str) -> io.BytesIO:
     """
     Types of XML files available:
     Full Price Report (all assets)
         - aprox. 5 MB zipped file;
@@ -228,27 +228,27 @@
     df = df_raw.copy()
     # Convert to datetime64[ns] since it is pandas default type for timestamps
     df["TradDt"] = df["TradDt"].astype("datetime64[ns]")
 
     expiration = df["TckrSymb"].str[3:].apply(cr.get_expiration_date)
     df.insert(2, "ExpirationDate", expiration)
 
-    business_days = cd.count_bdays(df["TradDt"], df["ExpirationDate"])
+    business_days = bday.count_bdays(df["TradDt"], df["ExpirationDate"])
     df.insert(3, "BDToExpiration", business_days)
 
     # Convert to nullable integer, since other columns use this data type
     df["BDToExpiration"] = df["BDToExpiration"].astype(pd.Int64Dtype())
 
     # Remove expired contracts
     df.query("BDToExpiration > 0", inplace=True)
 
     return df.sort_values(by=["ExpirationDate"], ignore_index=True)
 
 
-def get_di(trade_date: Timestamp, source_type: str, return_raw: bool) -> DataFrame:
+def read_xml(trade_date: Timestamp, source_type: str, return_raw: bool) -> DataFrame:
     zip_file = _get_file_from_url(trade_date, source_type)
 
     xml_file = _extract_xml_from_zip(zip_file)
 
     di_data = _extract_di_data_from_xml(xml_file)
 
     df_raw = _create_df_from_di_data(di_data)
```

### Comparing `pyield-0.5.1/pyield/holidays/br_holidays_new.txt` & `pyield-0.6.0/pyield/holidays/br_holidays_new.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.5.1/pyield/holidays/br_holidays_old.txt` & `pyield-0.6.0/pyield/holidays/br_holidays_old.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.5.1/pyield/holidays/core.py` & `pyield-0.6.0/pyield/holidays/core.py`

 * *Files identical despite different names*

### Comparing `pyield-0.5.1/pyproject.toml` & `pyield-0.6.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "pandas>=2.0.0",
     "numpy",
     "beautifulsoup4",
     "html5lib",
     "lxml",
 ]
 dynamic = []
-version = "0.5.1"
+version = "0.6.0"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Source = "https://github.com/crdcj/PYield"
 
@@ -48,7 +48,17 @@
 
 [tool.pdm.dev-dependencies]
 dev = [
     "ipykernel",
     "pytest",
     "mypy",
 ]
+
+[tool.ruff.lint]
+select = [
+    "E",
+    "F",
+    "UP",
+    "B",
+    "SIM",
+    "I",
+]
```

### Comparing `pyield-0.5.1/tests/test_br_calendar.py` & `pyield-0.6.0/tests/test_br_calendar.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import pandas as pd
 import numpy as np
 
-from pyield import calendar as cl
+import pyield as yd
 
 
 def test_count_bdays_1():
     start = "2023-01-01"
     end = "2023-01-08"
     # 01/01/2023 is a Sunday and a holiday
-    assert cl.count_bdays(start, end) == 5
+    assert yd.count_bdays(start, end) == 5
 
 
 def test_count_bdays_2():
     start = "2023-12-15"
     end = "2024-01-02"
     # 25/12/2023 is a holiday
     # 01/01/2024 is a holiday
-    assert cl.count_bdays(start, end) == 10
+    assert yd.count_bdays(start, end) == 10
 
 
 def test_count_bdays_with_series():
     start = "2023-01-01"
     end = pd.Series(["2023-01-08", "2023-01-22"])
     # Assuming no holidays in these periods
-    assert np.array_equal(cl.count_bdays(start, end), np.array([5, 15]))
+    assert np.array_equal(yd.count_bdays(start, end), np.array([5, 15]))
 
 
 def test_count_bdays_negative_count():
     start = "2023-01-08"
     end = "2023-01-01"
     # Negative count expected
-    assert cl.count_bdays(start, end) == -5
+    assert yd.count_bdays(start, end) == -5
 
 
 def test_count_bdays_new_holiday_list():
     start = "2024-11-20"  # Zumbi Nacional Day
     end = "2024-11-21"
-    assert cl.count_bdays(start, end) == 0
+    assert yd.count_bdays(start, end) == 0
 
 
 def test_count_bdays_old_holiday_list():
     start = "2020-11-20"  # Was not a holiday in 2020
     end = "2020-11-21"
-    assert cl.count_bdays(start, end) == 1
+    assert yd.count_bdays(start, end) == 1
```

### Comparing `pyield-0.5.1/tests/test_di.py` & `pyield-0.6.0/tests/test_di.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 def test_settlement_rate_with_old_holiday_list():
     settlement_rates = {
         "N27": 0.09809,
         "F33": 0.10368,
     }
 
     # 22-12-2023 is before the new holiday calendar
-    df = cr.get_di(trade_date="2023-12-22")
+    df = cr.fetch_data(trade_date="2023-12-22")
     expiration_codes = list(settlement_rates.keys())  # noqa: F841
     result = df.query("ExpirationCode in @expiration_codes")["SettlementRate"].to_list()
     assert result == list(settlement_rates.values())
 
 
 def test_settlement_rates_with_current_holiday_list():
     settlement_rates = {
@@ -64,19 +64,19 @@
         "F27": 0.09683,
         "N27": 0.09794,
         "F29": 0.10042,
         "F31": 0.10240,
         "F33": 0.10331,
     }
 
-    df = cr.get_di(trade_date="2023-12-26")
+    df = cr.fetch_data(trade_date="2023-12-26")
     expiration_codes = list(settlement_rates.keys())  # noqa: F841
     results = df.query("ExpirationCode in @expiration_codes")[
         "SettlementRate"
     ].to_list()
     assert results == list(settlement_rates.values())
 
 
 def test_non_business_day():
     non_business_day = "2023-12-24"
     with pytest.raises(ValueError):
-        cr.get_di(trade_date=non_business_day)
+        cr.fetch_data(trade_date=non_business_day)
```

### Comparing `pyield-0.5.1/PKG-INFO` & `pyield-0.6.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PYield
-Version: 0.5.1
+Version: 0.6.0
 Summary: A Python library for analysis of fixed income instruments in Brazil
 Keywords: fixed-income, brazil, finance, analysis, bonds
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Carlos Carvalho
         
@@ -40,72 +40,105 @@
 Requires-Dist: lxml
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://img.shields.io/pypi/v/pyield.svg)](https://pypi.python.org/pypi/pyield)
 [![Made with Python](https://img.shields.io/badge/Python->=3.11-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![License](https://img.shields.io/badge/License-MIT-blue)](#license)
 
-# PYield: Brazilian Fixed Income Analysis Library
+# PYield: Fixed Income Toolbox for Brazilian Markets
 
 ## Introduction
 
 Welcome to PYield, a Python library designed for the analysis of fixed income instruments in Brazil. This library is tailored for financial analysts, researchers, and enthusiasts interested in the Brazilian fixed income market. Leveraging the power of popular Python libraries like Pandas and Requests, PYield simplifies the process of obtaining and processing data from key sources such as ANBIMA and B3.
 
 ## Features
 
 - **Data Collection**: Automated fetching of data from ANBIMA and B3.
 - **Data Processing**: Efficient processing and normalization of fixed income data.
 - **Analysis Tools**: Built-in functions for common analysis tasks in fixed income markets.
-- **Easy Integration**: Seamless integration with Python data analysis workflows.
+- **Easy Integration**: Seamless integration with pandas data analysis workflows.
 - **Type Hints**: Full support for static type checking, enhancing development experience and code quality.
 
 ## Installation
 
 You can install PYield using pip:
 ```sh
 pip install pyield
 ```
 
 ## How to use PYield
 
-### DI Futures Data
+### Futures Data
 ```python
 import pyield as yd
 
-# Get a pandas dataframe with the DI processed data from B3 (default)
->>> yd.get_di(trade_date='2024-03-08')
- TradeDate ExpirationCode ExpirationDate  BDToExpiration  ...  LastRate  LastAskRate  LastBidRate  SettlementRate
-2024-03-08            J24     2024-04-01              15  ...    10.952       10.952       10.956          10.956
-2024-03-08            K24     2024-05-02              37  ...    10.776       10.774       10.780          10.777
-2024-03-08            M24     2024-06-03              58  ...    10.604       10.602       10.604          10.608
-       ...            ...            ...             ...  ...       ...          ...          ...             ...
-2024-03-08            F37     2037-01-02            3213  ...      <NA>         <NA>         <NA>          10.859
-2024-03-08            F38     2038-01-04            3462  ...      <NA>         <NA>         <NA>          10.859
-2024-03-08            F39     2039-01-03            3713  ...      <NA>         <NA>         <NA>          10.85
+# Get a DataFrame with the DI Futures data from B3
+>>> yd.get_data(asset_code="DI1", reference_date='2024-03-08')
+
+TradeDate  ExpirationCode ExpirationDate BDToExpiration  ... LastRate LastAskRate LastBidRate SettlementRate
+2024-03-08 J24            2024-04-01     15              ... 10.952   10.952      10.956      10.956
+2024-03-08 K24            2024-05-02     37              ... 10.776   10.774      10.780      10.777
+2024-03-08 M24            2024-06-03     58              ... 10.604   10.602      10.604      10.608
+...        ...            ...            ...             ... ...      ...         ...         ...
+2024-03-08 F37            2037-01-02     3213            ... <NA>     <NA>        <NA>        10.859
+2024-03-08 F38            2038-01-04     3462            ... <NA>     <NA>        <NA>        10.859
+2024-03-08 F39            2039-01-03     3713            ... <NA>     <NA>        <NA>        10.85
+```
+
+### Treasury Bonds Data
+```python
+# Get a DataFrame with the NTN-B data from ANBIMA
+# Anbima data is available for the last 5 working days
+# Obs: Anbima members have access to the full history
+>>> yd.get_data(asset_code="NTN-B", reference_date='2024-04-12')
+
+BondType ReferenceDate MaturityDate BidRate AskRate IndicativeRate Price
+NTN-B    2024-04-12    2024-08-15   0.07540 0.07504 0.07523        4,271.43565
+NTN-B    2024-04-12    2025-05-15   0.05945 0.05913 0.05930        4,361.34391
+NTN-B    2024-04-12    2026-08-15   0.05927 0.05897 0.05910        4,301.40082
+...      ...           ...          ...     ...     ...            ...
+NTN-B    2024-04-12    2050-08-15   0.06039 0.06006 0.06023        4,299.28233
+NTN-B    2024-04-12    2055-05-15   0.06035 0.05998 0.06017        4,367.13360
+NTN-B    2024-04-12    2060-08-15   0.06057 0.06016 0.06036        4,292.26323
+```
+
+### Spreads Calculation
+```python
+# Calculate the spread between two DI Futures contracts and the pre-fix bonds
+>>> yd.calculate_spreads(spread_type="di_vs_pre", reference_date="2024-4-11")
+
+BondType ReferenceDate MaturityDate  DISpread
+LTN      2024-04-11    2024-07-01    -20.28000
+LTN      2024-04-11    2024-10-01    -10.19000
+LTN      2024-04-11    2025-01-01    -15.05000
+...      ...           ...           ...
+NTN-F    2024-04-11    2031-01-01    -0.66000
+NTN-F    2024-04-11    2033-01-01    -5.69000
+NTN-F    2024-04-11    2035-01-01    -1.27000
 ```
 
 ### Business Days Tools (Brazilian holidays are automatically considered)
 ```python
-# Generate a pandas series with the business days between two dates
->>> yd.generate_bdays(start='2023-12-29', end='2024-01-03')
-0   2023-12-29
-1   2024-01-02
-2   2024-01-03
-dtype: datetime64[ns]
+# Count the number of business days between two dates
+# Start date is included, end date is excluded
+>>> yd.count_bdays(start='2023-12-29', end='2024-01-02')
+1
 
 # Get the next business day after a given date (offset=1)
 >>> yd.offset_bdays(dates="2023-12-29", offset=1)
 Timestamp('2024-01-02 00:00:00')
 
 # Get the next business day if it is not a business day (offset=0)
 >>> yd.offset_bdays(dates="2023-12-30", offset=0)
 Timestamp('2024-01-02 00:00:00')
 
 # Since 2023-12-29 is a business day, it returns the same date (offset=0)
 >>> yd.offset_bdays(dates="2023-12-29", offset=0)
 Timestamp('2023-12-29 00:00:00')
 
-# Count the number of business days between two dates
-# Start date is included, end date is excluded
->>> yd.count_bdays(start='2023-12-29', end='2024-01-02')
-1
+# Generate a pandas series with the business days between two dates
+>>> yd.generate_bdays(start='2023-12-29', end='2024-01-03')
+0   2023-12-29
+1   2024-01-02
+2   2024-01-03
+dtype: datetime64[ns]
 ```
```


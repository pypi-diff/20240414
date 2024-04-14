# Comparing `tmp/lottokit-0.6.tar.gz` & `tmp/lottokit-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lottokit-0.6.tar", last modified: Sat Mar 30 05:19:04 2024, max compression
+gzip compressed data, was "lottokit-0.7.tar", last modified: Sun Apr 14 09:06:22 2024, max compression
```

## Comparing `lottokit-0.6.tar` & `lottokit-0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-03-30 05:19:04.074996 lottokit-0.6/
--rw-r--r--   0 zhengdongqi   (501) staff       (20)    11357 2024-01-29 15:26:41.000000 lottokit-0.6/LICENSE
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      857 2024-03-30 05:19:04.074893 lottokit-0.6/PKG-INFO
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      465 2024-02-10 12:37:26.000000 lottokit-0.6/README.md
-drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-03-30 05:19:04.074008 lottokit-0.6/lottokit/
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      380 2024-01-29 15:26:41.000000 lottokit-0.6/lottokit/__init__.py
--rw-r--r--   0 zhengdongqi   (501) staff       (20)    47175 2024-03-30 05:11:27.000000 lottokit-0.6/lottokit/daletou.py
--rw-r--r--   0 zhengdongqi   (501) staff       (20)    51733 2024-02-12 12:15:11.000000 lottokit-0.6/lottokit/util.py
-drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-03-30 05:19:04.074615 lottokit-0.6/lottokit.egg-info/
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      857 2024-03-30 05:19:04.000000 lottokit-0.6/lottokit.egg-info/PKG-INFO
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      272 2024-03-30 05:19:04.000000 lottokit-0.6/lottokit.egg-info/SOURCES.txt
--rw-r--r--   0 zhengdongqi   (501) staff       (20)        1 2024-03-30 05:19:04.000000 lottokit-0.6/lottokit.egg-info/dependency_links.txt
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      155 2024-03-30 05:19:04.000000 lottokit-0.6/lottokit.egg-info/requires.txt
--rw-r--r--   0 zhengdongqi   (501) staff       (20)        9 2024-03-30 05:19:04.000000 lottokit-0.6/lottokit.egg-info/top_level.txt
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      218 2024-02-01 15:03:38.000000 lottokit-0.6/pyproject.toml
--rw-r--r--   0 zhengdongqi   (501) staff       (20)       38 2024-03-30 05:19:04.075045 lottokit-0.6/setup.cfg
--rw-r--r--   0 zhengdongqi   (501) staff       (20)     1182 2024-03-30 05:11:33.000000 lottokit-0.6/setup.py
-drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-03-30 05:19:04.074730 lottokit-0.6/tests/
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      216 2024-02-12 12:13:32.000000 lottokit-0.6/tests/test.py
+drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-04-14 09:06:22.346593 lottokit-0.7/
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)    11357 2024-01-29 15:26:41.000000 lottokit-0.7/LICENSE
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      857 2024-04-14 09:06:22.346489 lottokit-0.7/PKG-INFO
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      465 2024-02-10 12:37:26.000000 lottokit-0.7/README.md
+drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-04-14 09:06:22.345499 lottokit-0.7/lottokit/
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      380 2024-01-29 15:26:41.000000 lottokit-0.7/lottokit/__init__.py
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)    51544 2024-04-14 09:04:56.000000 lottokit-0.7/lottokit/daletou.py
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)    51733 2024-02-12 12:15:11.000000 lottokit-0.7/lottokit/util.py
+drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-04-14 09:06:22.346079 lottokit-0.7/lottokit.egg-info/
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      857 2024-04-14 09:06:22.000000 lottokit-0.7/lottokit.egg-info/PKG-INFO
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      272 2024-04-14 09:06:22.000000 lottokit-0.7/lottokit.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)        1 2024-04-14 09:06:22.000000 lottokit-0.7/lottokit.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      155 2024-04-14 09:06:22.000000 lottokit-0.7/lottokit.egg-info/requires.txt
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)        9 2024-04-14 09:06:22.000000 lottokit-0.7/lottokit.egg-info/top_level.txt
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      218 2024-02-01 15:03:38.000000 lottokit-0.7/pyproject.toml
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)       38 2024-04-14 09:06:22.346643 lottokit-0.7/setup.cfg
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)     1182 2024-04-14 09:04:56.000000 lottokit-0.7/setup.py
+drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-04-14 09:06:22.346216 lottokit-0.7/tests/
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      216 2024-02-12 12:13:32.000000 lottokit-0.7/tests/test.py
```

### Comparing `lottokit-0.6/LICENSE` & `lottokit-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lottokit-0.6/PKG-INFO` & `lottokit-0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lottokit
-Version: 0.6
+Version: 0.7
 Summary: Lotto Kit Package
 Author: nickdecodes
 Author-email: nickdecodes <nickdecodes@163.com>
 Project-URL: Documentation, http://python-lottokit.readthedocs.io
 Project-URL: Source, https://github.com/nickdecodes/python-lottokit
 Keywords: lottokit,lottery
 Requires-Python: >=3.6
```

### Comparing `lottokit-0.6/lottokit/daletou.py` & `lottokit-0.7/lottokit/daletou.py`

 * *Files 7% similar despite different names*

```diff
@@ -201,14 +201,15 @@
             # wait next page load
             try:
                 # try to find element of position == 13
                 next_button = WebDriverWait(driver, 10).until(
                     EC.element_to_be_clickable((By.XPATH, "/html/body/div/div/div[3]/ul/li[position()=13]"))
                 )
             except Exception as ex:
+                self.app_log.info(ex)
                 # try to find element of position == 8
                 next_button = WebDriverWait(driver, 10).until(
                     EC.element_to_be_clickable((By.XPATH, "/html/body/div/div/div[3]/ul/li[position()=8]"))
                 )
 
             # click to next page
             next_button.click()
@@ -666,14 +667,15 @@
                 period=data[0],
                 date=data[1],
                 weekday=self.calculate_weekday(data[1]),
                 front=self.calculate_front(data),
                 back=self.calculate_back(data)
             )
         except Exception as ex:
+            self.app_log.info(ex)
             # If there is an error, create a Lottery with the raw data
             # Ensure that 'data' can be unpacked into the Lottery named tuple
             return self.Lottery(*data)
 
     def calculate_front(self, data: Iterable[int]) -> List[int]:
         """
         Calculate the 'front' portion of the data based on predefined size settings.
@@ -848,16 +850,16 @@
                  {feature_key: {'front': set(), 'back': set()}}.
         """
         predictions = {}
 
         for feature, item in feature_results.items():
             for region, matrix in item.items():
                 # Transpose the matrix to iterate over columns (sequences)
-                # matrix_flip = [[matrix[j][i] for j in range(len(matrix))] for i in range(len(matrix[0]))]
-                matrix_flip = list(map(list, zip(*matrix)))
+                # matrix_flip = list(map(list, zip(*matrix)))
+                matrix_flip = [[matrix[j][i] for j in range(len(matrix))] for i in range(len(matrix[0]))]
 
                 for predictor in [
                     self.moving_average,
                     self.linear_regression,
                     self.random_forest_regressor
                 ]:
                     # Initialize the nested sets for each feature and region if not already present
@@ -914,15 +916,15 @@
         # Convert to Lottery data objects
         last_window_data = [self.convert_lottery_data(d) for d in data[-window:]]
 
         # Create a matrix of front and back area numbers
         matrix = [d.front + d.back for d in last_window_data]
 
         # Transpose the matrix
-        matrix_flip = list(map(list, zip(*matrix)))
+        matrix_flip = [[matrix[j][i] for j in range(len(matrix))] for i in range(len(matrix[0]))]
 
         # Apply the transposed matrix to each predictor and generate predictions
         predictions = [
             tuple(predictor(seq) for seq in matrix_flip) for predictor in [
                 self.moving_average,
                 self.linear_regression,
                 self.random_forest_regressor,
@@ -931,56 +933,128 @@
 
         # Create a list of Lottery objects based on the predictions
         return [
             self.Lottery('', '', '', self.calculate_front(d), self.calculate_back(d))
             for d in predictions
         ]
 
-    def predict_by_last_period(self):
+    def predict_by_last_period(self, next_period: int = None, show_details: bool = False) -> List[List[int]]:
         """
         Predicts features by the last period window of historical data and prints the results.
         Skips predictions where the sum of 'ratio' features does not match the expected size.
+        :param next_period: int eg: 24001
+        :param show_details: boolean flag to output details about the prediction
         """
         history_data = self.read_csv_data_from_file(self.history_record_path, app_log=self.app_log)
-        history_data = history_data[:]
+        if next_period is None:
+            history_data = history_data[:]
+        else:
+            index = next((i for i, sublist in enumerate(history_data) if sublist[0] == str(next_period)), -1)
+            history_data = history_data[:index] if index != -1 else history_data[:]
 
         maybe_combinations = self.predict_by_last_window_data(history_data, window=15)
-        self.app_log.info([mc.front + mc.back for mc in maybe_combinations])
+        predict_data = [mc.front + mc.back for mc in maybe_combinations]
+        self.app_log.info(predict_data) if show_details is True else None
 
         handle_result = self.handle_last_window_data(data=history_data, window=15)
-        self.app_log.info(handle_result)
+        self.app_log.info(handle_result) if show_details is True else None
+
+        return predict_data
 
-    def predict_by_same_period(self):
+    def predict_by_same_period(self, next_period: int = None, show_details: bool = False) -> List[List[int]]:
         """
         Predicts features by the last period window of historical data and prints the results.
         Skips predictions where the sum of 'ratio' features does not match the expected size.
+        :param next_period: int eg: 24001
+        :param show_details: boolean flag to output details about the prediction
         """
         period_data = self.read_json_data_from_file(self.period_record_path, app_log=self.app_log)
-        period_data = period_data.get(str(self.get_next_period()).zfill(3))
+        if next_period is None:
+            period_data = period_data.get(str(self.get_next_period()).zfill(3))
+        else:
+            period_data = period_data.get(str(next_period % 100).zfill(3))
+            index = next((i for i, sublist in enumerate(period_data) if sublist[0] == str(next_period)), -1)
+            period_data = period_data[:index] if index != -1 else period_data[:]
 
         maybe_combinations = self.predict_by_last_window_data(period_data, window=15)
-        self.app_log.info([mc.front + mc.back for mc in maybe_combinations])
+        predict_data = [mc.front + mc.back for mc in maybe_combinations]
+        self.app_log.info(predict_data) if show_details is True else None
 
         handle_result = self.handle_last_window_data(data=period_data, window=15)
-        self.app_log.info(handle_result)
+        self.app_log.info(handle_result) if show_details is True else None
+
+        return predict_data
 
-    def predict_by_last_weekday(self):
+    def predict_by_last_weekday(self,
+                                next_weekday: int = None,
+                                next_period: int = None,
+                                show_details: bool = False) -> List[List[int]]:
         """
         Predicts features by the last weekday window of historical data and prints the results.
         Skips predictions where the sum of 'ratio' features does not match the expected size.
+        :param next_weekday: int eg: [1 | 3 | 6]
+        :param next_period: int eg: 24001
+        :param show_details: boolean flag to output details about the prediction
         """
         weekday_data = self.read_json_data_from_file(self.weekday_record_path, app_log=self.app_log)
-        weekday_data = weekday_data.get(str(self.get_next_weekday()))
+        if next_weekday is None:
+            weekday_data = weekday_data.get(str(self.get_next_weekday()))
+        else:
+            weekday_data = weekday_data.get(str(next_weekday))
+            if next_period is not None:
+                index = next((i for i, sublist in enumerate(weekday_data) if sublist[0] == str(next_period)), -1)
+                weekday_data = weekday_data[:index] if index != -1 else weekday_data[:]
 
         maybe_combinations = self.predict_by_last_window_data(weekday_data, window=15)
-        self.app_log.info([mc.front + mc.back for mc in maybe_combinations])
+        predict_data = [mc.front + mc.back for mc in maybe_combinations]
+        self.app_log.info(predict_data) if show_details is True else None
 
         handle_result = self.handle_last_window_data(data=weekday_data, window=15)
-        self.app_log.info(handle_result)
+        self.app_log.info(handle_result) if show_details is True else None
+
+        return predict_data
 
-    def predict(self):
-        self.predict_by_last_period()
-        self.predict_by_same_period()
-        self.predict_by_last_weekday()
+    def predict(self, next_period: int = None, next_weekday: int = None, show_details: bool = False) -> List[List[int]]:
+        """
+        :param next_period: int eg: 24001
+        :param next_weekday: int eg: [1 | 3 | 6]
+        :param show_details: boolean flag to output details about the prediction
+        """
+        predict_data = []
+        predict_data.extend(self.predict_by_last_period(next_period=next_period,
+                                                        show_details=show_details))
+        predict_data.extend(self.predict_by_same_period(next_period=next_period,
+                                                        show_details=show_details))
+        predict_data.extend(self.predict_by_last_weekday(next_weekday=next_weekday,
+                                                         next_period=next_period,
+                                                         show_details=show_details))
+
+        if show_details is True:
+            self.app_log.info("The following is a preliminary forecast of the data analysis : ")
+            # Splitting the data into first 5 and last 2 numbers
+            front_zone = [num for row in predict_data for num in row[:5]]
+            back_zone = [num for row in predict_data for num in row[5:]]
+
+            # Counting occurrences
+            front_zone_frequency = Counter(front_zone)
+            back_zone_frequency = Counter(back_zone)
+
+            # Sorting the counts
+            sorted_front_zone_frequency = sorted(front_zone_frequency.items(), key=lambda x: x[1], reverse=True)
+            sorted_back_zone_frequency = sorted(back_zone_frequency.items(), key=lambda x: x[1], reverse=True)
+
+            # Printing the results
+            print("Counts of the front zone numbers in each row sorted by frequency:")
+            for number, count in sorted_front_zone_frequency:
+                print(f"Number {number}: {count} times")
+
+            print("\nCounts of the back zone numbers in each row sorted by frequency:")
+            for number, count in sorted_back_zone_frequency:
+                print(f"Number {number}: {count} times")
+
+            self.app_log.info("\nHere are the preliminary predictions: ")
+            for data in predict_data:
+                self.app_log.info(','.join(map(str, data)))
+        return predict_data
 
     def test(self):
         pass
```

### Comparing `lottokit-0.6/lottokit/util.py` & `lottokit-0.7/lottokit/util.py`

 * *Files identical despite different names*

### Comparing `lottokit-0.6/lottokit.egg-info/PKG-INFO` & `lottokit-0.7/lottokit.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lottokit
-Version: 0.6
+Version: 0.7
 Summary: Lotto Kit Package
 Author: nickdecodes
 Author-email: nickdecodes <nickdecodes@163.com>
 Project-URL: Documentation, http://python-lottokit.readthedocs.io
 Project-URL: Source, https://github.com/nickdecodes/python-lottokit
 Keywords: lottokit,lottery
 Requires-Python: >=3.6
```

### Comparing `lottokit-0.6/setup.py` & `lottokit-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='lottokit',
-    version='0.6',
+    version='0.7',
     keywords=['lottokit', 'lottery'],
     packages=find_packages(),
     package_data={"": ["LICENSE", "NOTICE"]},
     include_package_data=True,
     author="nickdecodes",
     author_email="nickdecodes@163.com",
     description="Lotto Kit Package",
```


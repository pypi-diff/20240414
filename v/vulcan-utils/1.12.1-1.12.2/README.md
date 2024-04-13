# Comparing `tmp/vulcan-utils-1.12.1.tar.gz` & `tmp/vulcan-utils-1.12.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-utils-1.12.1.tar", last modified: Fri Apr 12 23:36:11 2024, max compression
+gzip compressed data, was "vulcan-utils-1.12.2.tar", last modified: Sat Apr 13 22:36:27 2024, max compression
```

## Comparing `vulcan-utils-1.12.1.tar` & `vulcan-utils-1.12.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:36:11.489630 vulcan-utils-1.12.1/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-12 23:36:11.489630 vulcan-utils-1.12.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 23:36:11.489630 vulcan-utils-1.12.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:36:11.485630 vulcan-utils-1.12.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/tests/test_formatter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8171 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/tests/test_printable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:36:11.489630 vulcan-utils-1.12.1/vulcan_utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)       99 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/vulcan_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/vulcan_utils/cache.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9539 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/vulcan_utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/vulcan_utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/vulcan_utils/formatter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9285 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/vulcan_utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/vulcan_utils/printable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:36:11.489630 vulcan-utils-1.12.1/vulcan_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-12 23:36:11.000000 vulcan-utils-1.12.1/vulcan_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-12 23:36:11.000000 vulcan-utils-1.12.1/vulcan_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 23:36:11.000000 vulcan-utils-1.12.1/vulcan_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 23:36:11.000000 vulcan-utils-1.12.1/vulcan_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 23:36:11.000000 vulcan-utils-1.12.1/vulcan_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:36:27.952386 vulcan-utils-1.12.2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-13 22:36:19.000000 vulcan-utils-1.12.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-04-13 22:36:27.952386 vulcan-utils-1.12.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 22:36:27.952386 vulcan-utils-1.12.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      627 2024-04-13 22:36:19.000000 vulcan-utils-1.12.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:36:27.952386 vulcan-utils-1.12.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-13 22:36:19.000000 vulcan-utils-1.12.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-13 22:36:19.000000 vulcan-utils-1.12.2/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-04-13 22:36:19.000000 vulcan-utils-1.12.2/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-13 22:36:19.000000 vulcan-utils-1.12.2/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-13 22:36:19.000000 vulcan-utils-1.12.2/tests/test_formatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8171 2024-04-13 22:36:19.000000 vulcan-utils-1.12.2/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-13 22:36:19.000000 vulcan-utils-1.12.2/tests/test_printable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:36:27.952386 vulcan-utils-1.12.2/vulcan_utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       70 2024-04-13 22:36:19.000000 vulcan-utils-1.12.2/vulcan_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-13 22:36:19.000000 vulcan-utils-1.12.2/vulcan_utils/cache.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10571 2024-04-13 22:36:19.000000 vulcan-utils-1.12.2/vulcan_utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-13 22:36:19.000000 vulcan-utils-1.12.2/vulcan_utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-13 22:36:19.000000 vulcan-utils-1.12.2/vulcan_utils/formatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9785 2024-04-13 22:36:19.000000 vulcan-utils-1.12.2/vulcan_utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-13 22:36:19.000000 vulcan-utils-1.12.2/vulcan_utils/printable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:36:27.952386 vulcan-utils-1.12.2/vulcan_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-04-13 22:36:27.000000 vulcan-utils-1.12.2/vulcan_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-13 22:36:27.000000 vulcan-utils-1.12.2/vulcan_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 22:36:27.000000 vulcan-utils-1.12.2/vulcan_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 22:36:27.000000 vulcan-utils-1.12.2/vulcan_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-13 22:36:27.000000 vulcan-utils-1.12.2/vulcan_utils.egg-info/top_level.txt
```

### Comparing `vulcan-utils-1.12.1/LICENSE` & `vulcan-utils-1.12.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-utils-1.12.1/PKG-INFO` & `vulcan-utils-1.12.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: vulcan-utils
-Version: 1.12.1
+Version: 1.12.2
 Summary: A utility package for Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: coloredlogs
 
 <!-- docs/README.md -->
 # Vulcan Utils
 
-Vulcan Utils is a Python package designed to enhance the logging capabilities of Python applications. It simplifies the logging process by automatically including critical details like the caller's filename and line number, making it easier to trace the source of log entries. The package supports a range of features including customizable log levels, colored logs, and conditional logging, tailored to improve both the development and debugging processes.
+Vulcan Utils is a Python package designed to enhance the functionality of Python applications through advanced logging and function decorators. It simplifies the integration of complex behaviors like logging, retry mechanisms, and rate limiting into applications with minimal code changes. Its robust features make it an ideal choice for developers looking to add sophisticated capabilities to their applications efficiently.
 
 **Requires Python 3.9 or higher**
 
 [View the full technical documentation here](https://vulcan-utils.readthedocs.io/en/latest/)
 
 [View the PyPi project here](https://pypi.org/project/vulcan-utils/)
 
@@ -25,21 +24,22 @@
 - **Colored Logs**: To enhance readability and facilitate quicker log analysis, Vulcan Utils supports colored logging, distinguishing log levels with different colors.
 - **Conditional Logging**: This feature offers advanced control over logging operations, enabling logs to be generated based on dynamic runtime conditions, thereby keeping log files concise and focused.
 - **Function Decorators**: Vulcan Utils introduces function decorators for logging, retrying, JSON serialization, and rate limiting, each adding a layer of functionality that enhances method executions with minimal code intrusion.
 - **Advanced Retry Mechanisms**: The retry decorators provide robust error handling by allowing repeated execution of functions upon failure, customizable by attempts and delays, which is invaluable for dealing with transient system or network issues.
 - **Automatic JSON Serialization**: Simplify data interchange in API services and other integrations with automatic JSON serialization of function outputs, streamlining responses and reducing boilerplate code.
 - **Rate Limiting Controls**: Enforce execution limits on functions with the rate limit decorator to manage resource utilization effectively and prevent system overload, which is essential for maintaining service availability and performance under high load.
 - **Caching**: Easy to use interface to connect with a Redis database, store, and retrieve data.
+- **Environment Variable Checks**: Function execution can be controlled based on the presence or specific values of environment variables, improving security and configuration flexibility.
 
 
 ## Installation
 You can install Vulcan Utils via PIP:
 
 ```bash
-pip install vulcan-logger
+pip install vulcan-utils
 ```
 
 ## Usage
 [View example usage here](https://github.com/nodadyoushutup/vulcan-utils/blob/main/example.py)
 
 Below are examples of how to use the Vulcan Utils logging and decoration features.
 
@@ -176,14 +176,26 @@
 #### Clearing the Cache
 Clear all keys and values in the currently selected Redis database.
 
 ```python
 cache.clear()
 ```
 
+### Environment variable checks
+Vulcan Utils now includes a decorator that enables function execution based on the presence or value of environment variables. This feature enhances security and configuration flexibility by allowing functions to run only when certain environmental conditions are met.
+
+```python
+from vulcan_utils.decorator import Decorator
+
+@Decorator.env(variable="CONFIG_MODE", value="production")
+def sensitive_operation():
+    """ Perform operations that are only safe in production environment """
+    pass
+```
+
 ### Advanced Configuration
 Vulcan Utils offers several environment variables to fine-tune logging behavior for your application. You can set these variables before initializing your logger to customize logging output, destination, and file naming.
 
 #### Setting Global Log Level
 Control the log level globally across your application by setting the `VULCAN_LOG_LEVEL` environment variable. This determines the minimum level of messages that will be logged. Available levels are `DEBUG`, `INFO`, `WARNING`, `ERROR`, and `CRITICAL`.
 
 _bash_
```

### Comparing `vulcan-utils-1.12.1/tests/test_cache.py` & `vulcan-utils-1.12.2/tests/test_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # test/test_cache.py
-import pytest
+import json
 from unittest.mock import MagicMock, patch
+
+import pytest
 from redis.exceptions import RedisError
+
 from vulcan_utils.cache import Cache
-import json
 
 
 @pytest.fixture
 def mock_redis():
     with patch('redis.Redis') as mock:
         yield mock
```

### Comparing `vulcan-utils-1.12.1/tests/test_decorator.py` & `vulcan-utils-1.12.2/tests/test_decorator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,42 @@
+"""
+Utility Functions and Decorators
+
+This module contains a collection of utility functions and decorators for various purposes such as 
+    logging, retrying operations, rate-limiting function calls, and working with environment 
+    variables.
+
+Functions:
+- _sample_function: A simple function that adds two integers.
+- _slow_function: A function that simulates a delay before returning a value.
+- _failing_function: A function that simulates failure a specified number of times before 
+    succeeding.
+- sample_function: A function used for testing the to_json decorator.
+- complex_data_function: A function used for testing the to_json decorator with complex data types.
+- test_function: A function used for testing the rate_limit decorator.
+- test_rate_limit_reset: A function used for testing the rate_limit decorator's reset functionality.
+- sample_function: A function used for testing the env decorator.
+
+Decorators:
+- log: A decorator for logging function calls, returns, and execution times.
+- retry: A decorator for retrying operations upon failure.
+- to_json: A decorator for serializing function return values to JSON.
+- rate_limit: A decorator for rate-limiting function calls.
+- env: A decorator for controlling function execution based on environment variables.
+"""
+
 import json
 import time
 from datetime import datetime
 from typing import List
 from unittest.mock import patch
 
 import pytest
 
-from vulcan_utils.decorator import Decorator as decorator
+from vulcan_utils.decorator import env, log, rate_limit, retry, to_json
 from vulcan_utils.encoder import Encoder
 
 
 def _sample_function(x: int, y: int = 2) -> int:
     """
     Simple function that adds two integers.
 
@@ -23,35 +49,36 @@
     """
 
     return x + y
 
 
 def _slow_function(delay: float) -> float:
     """
-    Function that simulates a delay before returning the delay value. Used to test timing and performance.
+    Function that simulates a delay before returning the delay value. Used to test timing and 
+        performance.
 
     Args:
         delay (float): The duration in seconds for which the function should pause.
 
     Returns:
         float: The actual delay value used.
     """
 
     time.sleep(delay)
     return delay
 
 
 def _failing_function(attempts: List[int], max_attempts: int = 2) -> str:
     """
-    Simulates a function that fails a specified number of times before succeeding.
-    This function is used primarily to test retry logic in decorators or other error-handling mechanisms.
+    Simulates a function that fails a specified number of times before succeeding. This function 
+        is used primarily to test retry logic in decorators or other error-handling mechanisms.
 
     Args:
-        attempts (List[int]): A list containing a single integer that tracks the number of attempts made so far. 
-            This list is modified in-place to increment the count of attempts.
+        attempts (List[int]): A list containing a single integer that tracks the number of attempts 
+            made so far. This list is modified in-place to increment the count of attempts.
         max_attempts (int): The number of times the function should fail before finally succeeding.
 
     Returns:
         str: Returns "Success" once the function exceeds the number of allowed failures.
 
     Raises:
         ValueError: Raises a deliberate exception until the number of failures reaches max_attempts.
@@ -70,92 +97,95 @@
     This verifies that the decorator appends execution time information to the log.
 
     Args:
         delay (float): Simulated function execution delay to test timing accuracy.
     """
 
     with patch('vulcan_utils.decorator.Logger') as mock_logger:
-        decorated = decorator.log(_slow_function)
+        decorated = log(_slow_function)
         decorated(delay)
         last_call_args = mock_logger.return_value.debug.call_args_list[-1][0][0]
         assert "milliseconds" in last_call_args
 
 
 def test_log_decorator_basic() -> None:
     """
     Tests the basic functionality of the log decorator to ensure it logs function calls,
     returns, and execution times correctly and returns the expected function results.
     """
 
     with patch('vulcan_utils.decorator.Logger') as mock_logger:
-        decorated = decorator.log(_sample_function)
+        decorated = log(_sample_function)
         result = decorated(1, y=3)
         assert result == 4
         assert mock_logger.return_value.debug.call_count == 3
 
 
 def test_log_decorator_condition_false() -> None:
     """
     Tests the log decorator when the logging condition is set to False.
     Ensures that no logging occurs when the condition evaluates to False but the function
     still executes and returns correctly.
     """
 
     with patch('vulcan_utils.decorator.Logger') as mock_logger:
-        decorated = decorator.log(_sample_function, condition=False)
+        decorated = log(_sample_function, condition=False)
         result = decorated(1, y=3)
         assert result == 4
         mock_logger.return_value.debug.assert_not_called()
 
 
 def test_log_decorator_log_level() -> None:
     """
     Tests the log decorator's ability to log at a specified level.
-    This test ensures that the decorator respects the 'level' parameter and logs at the correct severity.
+    This test ensures that the decorator respects the 'level' parameter and logs at the correct 
+        severity.
     """
 
     with patch('vulcan_utils.decorator.Logger') as mock_logger:
-        decorated = decorator.log(_sample_function, level="INFO")
+        decorated = log(_sample_function, level="INFO")
         decorated(1, 2)
         assert mock_logger.return_value.info.call_count == 3
 
 
 def test_retry_success() -> None:
     """
-    Verifies that the retry decorator retries the correct number of times and then successfully returns
+    Verifies that the retry decorator retries the correct number of times and then successfully 
+        returns
     the result of the function when it finally succeeds.
     """
 
     attempts = [0]
-    decorated = decorator.retry(_failing_function, retries=2, delay=0.1)
+    decorated = retry(_failing_function, retries=2, delay=0.1)
     result = decorated(attempts=attempts, max_attempts=2)
     assert result == "Success"
     assert attempts[0] == 2
 
 
 def test_retry_fail() -> None:
     """
-    Ensures that the retry decorator properly raises the last encountered exception after all retries are exhausted.
+    Ensures that the retry decorator properly raises the last encountered exception after all 
+        retries are exhausted.
     """
 
     attempts = [0]
-    decorated = decorator.retry(_failing_function, retries=1, delay=0.1)
+    decorated = retry(_failing_function, retries=1, delay=0.1)
     with pytest.raises(ValueError):
         decorated(attempts=attempts, max_attempts=3)
     assert attempts[0] == 2
 
 
 @pytest.mark.parametrize("attempts_list, max_attempts", [([0], 2), ([0], 3)])
 def test_retry_logging(attempts_list, max_attempts) -> None:
     """
     Tests that logging occurs as expected during retries and at failure.
     """
 
     with patch('vulcan_utils.decorator.Logger') as mock_logger:
-        decorated = decorator.retry(
+        decorated = retry(
             _failing_function,
             retries=max_attempts - 1, delay=0.1
         )
         try:
             decorated(attempts=attempts_list, max_attempts=max_attempts)
         except ValueError:
             pass
@@ -163,73 +193,135 @@
         assert mock_logger.return_value.warning.call_count == expected_warning_calls
         assert mock_logger.return_value.error.called == (
             attempts_list[0] == max_attempts)
 
 
 def test_to_json():
     """
-    Test the to_json decorator to ensure it correctly serializes the return value of a function to a JSON string using
-    a custom encoder. The function will return a dictionary which should be serialized into a JSON string.
+    Test the to_json decorator to ensure it correctly serializes the return value of a function to 
+        a JSON string using
+    a custom encoder. The function will return a dictionary which should be serialized into a JSON 
+        string.
     """
 
-    @decorator.to_json
+    @to_json
     def sample_function():
         return {"name": "Alice", "age": 30, "time": datetime(2020, 5, 17)}
     result = sample_function()
     expected_json = json.dumps(
         {"name": "Alice", "age": 30, "time": "2020-05-17T00:00:00"}, cls=Encoder)
-    assert result == expected_json, "The JSON output from the decorated function did not match the expected JSON string."
+    assert result == expected_json, \
+        "The JSON output from the decorated function did not match the expected JSON string."
 
-    @decorator.to_json
+    @to_json
     def complex_data_function():
         return {"date": datetime.now(), "data": [1, 2, 3]}
     try:
         json_result = complex_data_function()
         # this will confirm json_result is a valid JSON string
         json.loads(json_result)
         assert True, "Serialization of complex data types was successful."
-    except Exception as e:
+    except Exception as e:  # pylint: disable=broad-except
         assert False, f"Serialization failed with error: {e}"
 
 
 @pytest.mark.parametrize("num_calls, sleep_time, expected_errors", [
     (10, 0.1, 0),  # All calls succeed without hitting the rate limit
     (60, 0.1, 10),  # 10 calls fail because they exceed the limit within the interval
     (50, 0.1, 0)    # Exactly at the limit, all should pass
 ])
 def test_rate_limit(num_calls, sleep_time, expected_errors):
     """
-    Test the rate_limit decorator to ensure it allows a specified number of function calls within a time interval
+    Test the rate_limit decorator to ensure it allows a specified number of function calls within 
+        a time interval
     and blocks additional calls until the interval has elapsed.
 
     Args:
         num_calls (int): Number of times to call the decorated function.
         sleep_time (float): Time to sleep between each call, in seconds.
         expected_errors (int): Number of times the rate limit should trigger and log an error.
     """
 
-    @decorator.rate_limit(limit=50, interval=10)
+    @rate_limit(limit=50, interval=10)
     def test_function():
         return
 
     with patch('vulcan_utils.decorator.Logger') as mock_logger:
         for _ in range(num_calls):
             test_function()
             time.sleep(sleep_time)
         assert mock_logger.return_value.error.call_count == expected_errors
 
 
 def test_rate_limit_reset():
     """
     Test that the rate limit properly resets after the cooldown interval.
     """
-    @decorator.rate_limit(limit=5, interval=1)  # Very short interval for test speed
+    @rate_limit(limit=5, interval=1)  # Very short interval for test speed
     def test_function():
         return
 
     with patch('vulcan_utils.decorator.Logger') as mock_logger:
         for _ in range(5):
             test_function()  # These should all pass
         time.sleep(1.1)      # Wait for the interval to pass
         for _ in range(5):
             test_function()  # These should also pass after the reset
         assert mock_logger.return_value.error.call_count == 0
+
+
+def test_env_decorator_variable_exists():
+    """
+    Test that the env decorator allows function execution when the environment variable exists.
+    """
+    with patch.dict('os.environ', {'TEST_VAR': 'test_value'}):
+        @env(variable='TEST_VAR')
+        def sample_function():
+            return True
+
+        assert sample_function() is True, "Function should execute and return True."
+
+
+def test_env_decorator_variable_equals_value():
+    """
+    Test that the env decorator allows function execution when the environment variable equals the 
+        specified value.
+    """
+    with patch.dict('os.environ', {'TEST_VAR': 'specific_value'}):
+        @env(variable='TEST_VAR', value='specific_value')
+        def sample_function():
+            return True
+
+        assert sample_function() is True, "Function should execute and return True."
+
+
+def test_env_decorator_variable_not_equal_value():
+    """
+    Test that the env decorator blocks function execution when the environment variable does not 
+        equal the specified value.
+    """
+    with patch.dict(
+        "os.environ",
+        {"TEST_VAR": "other_value"}
+    ), patch('vulcan_utils.decorator.Logger') as mock_logger:
+        @env(variable='TEST_VAR', value='specific_value')
+        def sample_function():
+            return True
+
+        result = sample_function()
+        assert result is None, "Function should not execute."
+        mock_logger.return_value.warning.assert_called_once()
+
+
+def test_env_decorator_variable_not_present():
+    """
+    Test that the env decorator blocks function execution when the environment variable is not 
+        present.
+    """
+    with patch('vulcan_utils.decorator.Logger') as mock_logger:
+        @env(variable='MISSING_VAR')
+        def sample_function():
+            return True
+
+        result = sample_function()
+        assert result is None, "Function should not execute."
+        mock_logger.return_value.warning.assert_called_once()
```

### Comparing `vulcan-utils-1.12.1/tests/test_encoder.py` & `vulcan-utils-1.12.2/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-utils-1.12.1/tests/test_formatter.py` & `vulcan-utils-1.12.2/tests/test_formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # tests/test_formatter.py
 import pytest
+
 from vulcan_utils.formatter import Formatter
 
 
 @pytest.mark.parametrize("milliseconds, expected", [
     (3901023, "1h 5m 1s 23ms"),
     (90061023, "1d 1h 1m 1s 23ms"),
     (31556952000, "1y 5h 49m 12s"),  # Corrected expected value
```

### Comparing `vulcan-utils-1.12.1/tests/test_logger.py` & `vulcan-utils-1.12.2/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `vulcan-utils-1.12.1/tests/test_printable.py` & `vulcan-utils-1.12.2/tests/test_printable.py`

 * *Files identical despite different names*

### Comparing `vulcan-utils-1.12.1/vulcan_utils/cache.py` & `vulcan-utils-1.12.2/vulcan_utils/cache.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,78 @@
+"""
+vulcan_utils/cache.py
+
+This module provides a high-level interface for caching data using Redis. It encapsulates
+the connection and basic operations such as setting, retrieving, deleting, and clearing data
+in Redis databases. This is useful for applications that require fast data retrieval and 
+effective data management using key-value storage.
+"""
+
+import json
 from typing import Any, Optional
+
 import redis
-import json
+from redis.exceptions import RedisError
+
 from vulcan_utils.encoder import Encoder
-from redis.exceptions import RedisError, ConnectionError
 
 
 class Cache:
+    """
+    Manages caching operations via Redis. Provides methods to set, get, delete, and clear cache 
+        data. The connection to the Redis server is established during class instantiation and 
+        will raise a ConnectionError if unable to connect. All methods that interact with the 
+        Redis server can raise a RedisError in case of operation failure.
+
+    Attributes:
+        redis (redis.Redis): Redis client instance connected to the specified server and database.
+
+    Raises:
+        ConnectionError: If the Redis server cannot be reached during initialization.
+        RedisError: For any failures in cache operations.
+    """
+
     def __init__(self, host="localhost", port=6379, db=0):
         """
         Initializes the Cache object with a Redis connection.
         Raises a ConnectionError if the Redis server cannot be reached.
 
         Args:
             host (str): The hostname of the Redis server.
             port (int): The port number on which the Redis server is running.
             db (int): The database number to connect to.
         """
         try:
             self.redis = redis.Redis(host=host, port=port, db=db)
             self.redis.ping()  # Try to ping the server to check connection
         except ConnectionError as e:
-            raise ConnectionError(f"Failed to connect to Redis: {str(e)}")
+            raise ConnectionError(
+                f"Failed to connect to Redis: {str(e)}"
+            ) from e
 
     def set(self, key: str, value: Any, expire: Optional[int] = None) -> None:
         """
         Stores a value in the cache, optionally setting an expiration time.
 
         Args:
             key (str): The key under which the value is stored.
             value (Any): The value to be stored.
-            expire (Optional[int]): The expiration time in seconds. If not specified, the value does not expire.
+            expire (Optional[int]): The expiration time in seconds. If not specified, the value 
+                does not expire.
 
         Raises:
             RedisError: If the operation cannot be completed.
         """
         try:
             serialized_value = json.dumps(value, cls=Encoder)
             self.redis.set(key, serialized_value, ex=expire)
         except RedisError as e:
-            raise RedisError(f"Failed to set key {key}: {str(e)}")
+            raise RedisError(
+                f"Failed to set key {key}: {str(e)}"
+            ) from e
 
     def get(self, key: str) -> Optional[Any]:
         """
         Retrieves a value from the cache.
 
         Args:
             key (str): The key for which the value is retrieved.
@@ -54,15 +84,17 @@
             RedisError: If the operation cannot be completed.
         """
         try:
             serialized_value = self.redis.get(key)
             if serialized_value is not None:
                 return json.loads(serialized_value)
         except RedisError as e:
-            raise RedisError(f"Failed to get key {key}: {str(e)}")
+            raise RedisError(
+                f"Failed to get key {key}: {str(e)}"
+            ) from e
         return None
 
     def delete(self, key: str) -> None:
         """
         Deletes a specific key from the cache.
 
         Args:
@@ -70,20 +102,24 @@
 
         Raises:
             RedisError: If the operation cannot be completed.
         """
         try:
             self.redis.delete(key)
         except RedisError as e:
-            raise RedisError(f"Failed to delete key {key}: {str(e)}")
+            raise RedisError(
+                f"Failed to delete key {key}: {str(e)}"
+            ) from e
 
     def clear(self) -> None:
         """
         Clears all keys and values from the current database.
 
         Raises:
             RedisError: If the operation cannot be completed.
         """
         try:
             self.redis.flushdb()
         except RedisError as e:
-            raise RedisError("Failed to clear database: {str(e)}")
+            raise RedisError(
+                f"Failed to clear database: {str(e)}"
+            ) from e
```

### Comparing `vulcan-utils-1.12.1/vulcan_utils/decorator.py` & `vulcan-utils-1.12.2/vulcan_utils/decorator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,230 +1,299 @@
-# vulcan_utils/decorator.py
+"""
+vulcan_utils/decorator.py
+
+This module provides decorators for logging, retrying, JSON serialization, rate limiting, 
+and environment variable restriction for function execution.
+"""
+
+
 import json
+import os
 import time
 from functools import wraps
 from typing import Any, Callable, Optional, TypeVar, Union
 
 from .encoder import Encoder
 from .logger import Logger
 
 # TypeVar for decorator type preservation
 F = TypeVar('F', bound=Callable[..., Any])
 
 
-class Decorator:
+def _call_message(func: Callable[..., Any], *args: Any, **kwargs: Any) -> str:
     """
-    A collection of decorators designed to enhance function capabilities with additional behaviors such as logging,
-    retrying on exceptions, converting return values to JSON, and rate-limiting function calls.his class primarily 
-    serves as a namespace for decorator methods.
-
-    This class implements static and class methods to provide utility functions that can be applied to other functions
-    to log details about their calls and results, retry execution on failures, serialize outputs to JSON, and limit
-    the rate of function execution.
-     """
-
-    @staticmethod
-    def _call_message(func: Callable[..., Any], *args: Any, **kwargs: Any) -> str:
-        """
-        Constructs a log message string for function calls, including function name,
-        positional arguments, and keyword arguments.
-
-        Args:
-            func (Callable[..., Any]): The function being called.
-            *args (Any): Positional arguments passed to the function.
-            **kwargs (Any): Keyword arguments passed to the function.
-
-        Returns:
-            A formatted log message string.
-        """
-
-        log_message_parts = [f"{func.__name__} call:"]
-        if args:
-            log_message_parts.append(f"args:{args}")
-        if kwargs:
-            log_message_parts.append(f"kwargs:{kwargs}")
-        return ' '.join(log_message_parts)
-
-    @staticmethod
-    def _return_message(func: Callable[..., Any], result: Any) -> str:
-        """
-        Constructs a log message string for function returns, including function name and the serialized return value.
-
-        Args:
-            func (Callable[..., Any]): The function that returned a value.
-            result (Any): The return value of the function.
-
-        Returns:
-            A formatted log message string with the serialized return value.
-        """
-
-        json_result = json.dumps(result, cls=Encoder, ensure_ascii=False)
-        return f"{func.__name__} return: {json_result} {type(result)}"
-
-    @staticmethod
-    def _log_func(logger: Logger, level: str) -> Callable[[str], None]:
-        """
-        Retrieves the appropriate logging function based on the specified log level.
-
-        Args:
-            logger (logger.Logger): An instance of Logger configured for logging messages.
-            level (str): A string representing the logging level.
-
-        Returns:
-            A logging function from the Logger instance corresponding to the specified level.
-        """
-
-        levels = {
-            "DEBUG": logger.debug,
-            "INFO": logger.info,
-            "WARNING": logger.warning,
-            "CRITICAL": logger.critical,
-            "ERROR": logger.error,
-        }
-        return levels.get(level.upper(), logger.debug)
-
-    @classmethod
-    def log(cls, _func: Optional[F] = None, *, condition: bool = True, level: str = "DEBUG") -> Union[Callable[[F], F], F]:
-        """
-        A decorator that logs the call and return of functions, including execution time.
-        Logging can be conditioned on a boolean expression.
-
-        Args:
-            _func (Callable[..., Any]): The function to be decorated. If None, other parameters are allowed to be specified first.
-            condition (bool): A boolean flag to determine if logging should occur, defaults to True.
-            level (str): A string indicating the logging level, defaults to "DEBUG".
-
-        Returns:
-            The decorated function with logging capabilities added.
-        """
-
-        def decorator_log(func: F):
-            @wraps(func)
-            def wrapper(*args, **kwargs):
-                result = None
-                if condition:
-                    start_time = time.time()
-                    logger = Logger(func.__module__)
-                    log_func = cls._log_func(logger, level)
-                    log_func(cls._call_message(func, *args, **kwargs))
-                    result = func(*args, **kwargs)
-                    log_func(cls._return_message(func, result))
-                    end_time = time.time()
-                    execution_time_ms = round(
-                        (end_time - start_time) * 1000,
-                        ndigits=4
-                    )
-                    log_func(
-                        f"{func.__name__} executed: {execution_time_ms} milliseconds")
-                else:
-                    result = func(*args, **kwargs)
-                return result
-            return wrapper
-        if _func is None:
-            return decorator_log
-        else:
-            return decorator_log(_func)
-
-    @classmethod
-    def retry(cls, _func: Optional[F] = None, *, retries: int = 3, delay: Union[int, float] = 1, infinite: bool = False) -> Union[Callable[[F], F], F]:
-        """
-        Decorator to retry a function if it raises an exception. Optionally retries the function indefinitely if
-        'infinite' is True. If not, it retries a specified number of times with a given delay between each attempt.
-
-        Args:
-            _func (Callable[..., Any]): The function to be decorated. If None, other parameters can be specified first.
-            retries (int): The maximum number of retries before giving up and raising the exception if not infinite.
-            delay (Union[int, float]): The delay between retries in seconds, can be an integer or a float for partial seconds.
-            infinite (bool): If True, the function will retry indefinitely, defaults to False.
-
-        Returns:
-            The decorated function that will retry on exceptions, or raises the last encountered exception if all retries fail and not infinite.
-
-        Raises:
-            Exception: The last exception encountered if the retry attempts exceed the specified limit and not infinite.
-        """
-
-        def decorator_retry(func: F):
-            @wraps(func)
-            def wrapper(*args, **kwargs):
-                attempt = 0
-                while True:
-                    try:
-                        return func(*args, **kwargs)
-                    except Exception as e:
-                        logger = Logger(__name__)
-                        if infinite:
+    Constructs a log message string for function calls, including function name,
+    positional arguments, and keyword arguments.
+
+    Args:
+        func (Callable[..., Any]): The function being called.
+        *args (Any): Positional arguments passed to the function.
+        **kwargs (Any): Keyword arguments passed to the function.
+
+    Returns:
+        A formatted log message string.
+    """
+
+    log_message_parts = [f"{func.__name__} call:"]
+    if args:
+        log_message_parts.append(f"args:{args}")
+    if kwargs:
+        log_message_parts.append(f"kwargs:{kwargs}")
+    return ' '.join(log_message_parts)
+
+
+def _return_message(func: Callable[..., Any], result: Any) -> str:
+    """
+    Constructs a log message string for function returns, including function name and the 
+    serialized return value.
+
+    Args:
+        func (Callable[..., Any]): The function that returned a value.
+        result (Any): The return value of the function.
+
+    Returns:
+        A formatted log message string with the serialized return value.
+    """
+
+    json_result = json.dumps(result, cls=Encoder, ensure_ascii=False)
+    return f"{func.__name__} return: {json_result} {type(result)}"
+
+
+def _log_func(logger: Logger, level: str) -> Callable[[str], None]:
+    """
+    Retrieves the appropriate logging function based on the specified log level.
+
+    Args:
+        logger (logger.Logger): An instance of Logger configured for logging messages.
+        level (str): A string representing the logging level.
+
+    Returns:
+        A logging function from the Logger instance corresponding to the specified level.
+    """
+
+    levels = {
+        "DEBUG": logger.debug,
+        "INFO": logger.info,
+        "WARNING": logger.warning,
+        "CRITICAL": logger.critical,
+        "ERROR": logger.error,
+    }
+    return levels.get(level.upper(), logger.debug)
+
+
+def log(
+    _func: Optional[F] = None,
+        *,
+        condition: bool = True,
+        level: str = "DEBUG"
+) -> Union[Callable[[F], F], F]:
+    """
+    A decorator that logs the call and return of functions, including execution time.
+    Logging can be conditioned on a boolean expression.
+
+    Args:
+        _func (Callable[..., Any]): The function to be decorated. If None, other parameters are 
+            allowed to be specified first.
+        condition (bool): A boolean flag to determine if logging should occur, defaults to True.
+        level (str): A string indicating the logging level, defaults to "DEBUG".
+
+    Returns:
+        The decorated function with logging capabilities added.
+    """
+
+    def decorator_log(func: F):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            result = None
+            if condition:
+                start_time = time.time()
+                logger = Logger(func.__module__)
+                log_func = _log_func(logger, level)
+                log_func(_call_message(func, *args, **kwargs))
+                result = func(*args, **kwargs)
+                log_func(_return_message(func, result))
+                end_time = time.time()
+                execution_time_ms = round(
+                    (end_time - start_time) * 1000,
+                    ndigits=4
+                )
+                log_func(
+                    f"{func.__name__} executed: {execution_time_ms} milliseconds")
+            else:
+                result = func(*args, **kwargs)
+            return result
+        return wrapper
+    if _func is None:
+        return decorator_log
+    else:
+        return decorator_log(_func)
+
+
+def retry(
+        _func: Optional[F] = None,
+        *,
+        retries: int = 3,
+        delay: Union[int, float] = 1,
+        infinite: bool = False
+) -> Union[Callable[[F], F], F]:
+    """
+    Decorator to retry a function if it raises an exception. Optionally retries the function 
+        indefinitely if `infinite` is True. If not, it retries a specified number of times with a 
+        given delay between each attempt.
+
+    Args:
+        _func (Callable[..., Any]): The function to be decorated. If None, other parameters can be 
+            specified first.
+        retries (int): The maximum number of retries before giving up and raising the exception if 
+            not infinite.
+        delay (Union[int, float]): The delay between retries in seconds, can be an integer or a 
+            float for partial seconds.
+        infinite (bool): If True, the function will retry indefinitely, defaults to False.
+
+    Returns:
+        The decorated function that will retry on exceptions, or raises the last encountered 
+            exception if all retries fail and not infinite.
+
+    Raises:
+        Exception: The last exception encountered if the retry attempts exceed the specified limit 
+            and not infinite.
+    """
+
+    def decorator_retry(func: F):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            attempt = 0
+            while True:
+                try:
+                    return func(*args, **kwargs)
+                except Exception as e:  # pylint: disable=broad-except
+                    logger = Logger(__name__)
+                    if infinite:
+                        logger.warning(
+                            f"{func.__name__} failed, retrying indefinitely: {e}"
+                        )
+                        time.sleep(delay)
+                    else:
+                        if attempt < retries:
                             logger.warning(
-                                f"{func.__name__} failed, retrying indefinitely: {e}"
+                                f"{func.__name__} failed, retrying: {e}, " +
+                                f"attempts left: {retries - attempt - 1}"
                             )
                             time.sleep(delay)
+                            attempt += 1
                         else:
-                            if attempt < retries:
-                                logger.warning(
-                                    f"{func.__name__} failed, retrying: {e}, attempts left: {retries - attempt - 1}")
-                                time.sleep(delay)
-                                attempt += 1
-                            else:
-                                logger.error(
-                                    f"{func.__name__} retry attempts failed: {e}")
-                                raise e
-            return wrapper
-        if _func is not None:
-            return decorator_retry(_func)
-        return decorator_retry
-
-    @classmethod
-    def to_json(cls, _func: Union[Callable[[F], F], F] = None) -> Union[Callable[[F], F], F]:
-        """
-        A decorator that serializes the return value of the decorated function to JSON using a custom encoder.
-
-        Args:
-            _func (Optional[Callable[[F], F]]): The function to decorate. If None, allows other parameters to be 
-                specified first as keyword arguments.
-
-        Returns:
-            Callable[[F], F]: The decorated function with its return value serialized as a JSON string.
-        """
-
-        def decorator_to_json(func: F) -> F:
-            @wraps(func)
-            def wrapper(*args, **kwargs) -> str:
-                result = func(*args, **kwargs)
-                return json.dumps(result, cls=Encoder, ensure_ascii=False)
-            return wrapper
-        if _func is not None:
-            return decorator_to_json(_func)
-        return decorator_to_json
-
-    @classmethod
-    def rate_limit(cls, limit: int, interval: float):
-        """
-        Decorator to rate limit the execution of a function. Allows a burst of 'limit' calls,
-        and then enforces a cooldown period of 'interval' seconds before allowing another burst.
-
-        Args:
-            limit (int): Maximum number of calls allowed within the burst.
-            interval (float): Cooldown interval (in seconds) after a burst before resetting the limit.
-        """
-
-        def decorator(func):
-            call_times = []
-            first_call_time = None
-
-            @wraps(func)
-            def wrapper(*args, **kwargs):
-                nonlocal first_call_time
-                now = time.time()
-                if first_call_time and now - first_call_time > interval:
-                    call_times.clear()
-                    first_call_time = None
-                if not first_call_time:
-                    first_call_time = now
-                if len(call_times) < limit:
-                    call_times.append(now)
+                            logger.error(
+                                f"{func.__name__} retry attempts failed: {e}")
+                            raise e
+        return wrapper
+    if _func is not None:
+        return decorator_retry(_func)
+    return decorator_retry
+
+
+def to_json(_func: Union[Callable[[F], F], F] = None) -> Union[Callable[[F], F], F]:
+    """
+    A decorator that serializes the return value of the decorated function to JSON using a custom 
+        encoder.
+
+    Args:
+        _func (Optional[Callable[[F], F]]): The function to decorate. If None, allows other 
+            parameters to be specified first as keyword arguments.
+
+    Returns:
+        Callable[[F], F]: The decorated function with its return value serialized as a JSON string.
+    """
+
+    def decorator_to_json(func: F) -> F:
+        @wraps(func)
+        def wrapper(*args, **kwargs) -> str:
+            logger = Logger(func.__module__)
+            result = func(*args, **kwargs)
+            json_result = json.dumps(result, cls=Encoder, ensure_ascii=False)
+            logger.debug(f"{func.__name__} JSON return: {json_result}")
+            return json_result
+        return wrapper
+    if _func is not None:
+        return decorator_to_json(_func)
+    return decorator_to_json
+
+
+def rate_limit(limit: int, interval: float):
+    """
+    Decorator to rate limit the execution of a function. Allows a burst of 'limit' calls,
+    and then enforces a cooldown period of 'interval' seconds before allowing another burst.
+
+    Args:
+        limit (int): Maximum number of calls allowed within the burst.
+        interval (float): Cooldown interval (in seconds) after a burst before resetting the limit.
+    """
+
+    def decorator(func):
+        call_times = []
+        first_call_time = None
+
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            nonlocal first_call_time
+            now = time.time()
+            if first_call_time and now - first_call_time > interval:
+                call_times.clear()
+                first_call_time = None
+            if not first_call_time:
+                first_call_time = now
+            if len(call_times) < limit:
+                call_times.append(now)
+                return func(*args, **kwargs)
+            else:
+                logger = Logger(func.__module__)
+                logger.error(f"Rate limit exceeded for {func.__name__}")
+                return
+        return wrapper
+    return decorator
+
+
+def env(
+        _func: Optional[F] = None,
+        *,
+        variable: str,
+        value: Optional[str] = None
+) -> Union[Callable[[F], F], F]:
+    """
+    A decorator that restricts function execution based on the presence or value of an environment 
+        variable.
+
+    Args:
+        _func (Callable[..., Any], optional): The function to be decorated. If None, allows 
+            decorator to be used with arguments.
+        variable (str): The environment variable name to check.
+        value (str, optional): The specific value the environment variable must have for the 
+            function to execute. If not specified, the existence of the variable is enough to 
+            allow execution.
+
+    Returns:
+        Callable[[F], F]: The decorated function, which will only execute if the conditions are 
+            met. Returns None if conditions are not met.
+    """
+
+    def decorator_env(func: F) -> F:
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            logger = Logger(func.__module__)
+            env_value = os.getenv(variable)
+            if env_value is not None:
+                if value is None or env_value == value:
+                    logger.debug(
+                        f"{func.__name__} execution allowed: '{variable}' set to '{env_value}'.")
                     return func(*args, **kwargs)
                 else:
-                    logger = Logger(func.__module__)
-                    logger.error(f"Rate limit exceeded for {func.__name__}")
-                    return
-            return wrapper
-        return decorator
+                    logger.warning(
+                        f"{func.__name__} blocked: '{variable}' value '{env_value}' " +
+                        f"does not match required '{value}'."
+                    )
+            else:
+                logger.warning(
+                    f"{func.__name__} blocked: Environment variable '{variable}' not set.")
+            return None
+        return wrapper
+    if _func is None:
+        return decorator_env
+    return decorator_env(_func)
```

### Comparing `vulcan-utils-1.12.1/vulcan_utils/encoder.py` & `vulcan-utils-1.12.2/vulcan_utils/encoder.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,51 @@
-# vulcan_utils/encoder.py
+"""
+vulcan_utils/encoder.py
+
+This module provides decorators for logging, retrying, JSON serialization, rate limiting, 
+and environment variable restriction for function execution.
+
+Classes:
+    - Encoder: A custom JSON encoder.
+"""
+
 import json
 import uuid
-from datetime import date, datetime
-from datetime import time as dt_time  # Alias for clarity
+from datetime import date, datetime, time
 from decimal import Decimal
 from enum import Enum
 from typing import Any
 
-try:
-    # Import numpy and pandas only if available
-    import numpy as np
-    import pandas as pd
-    HAS_NUMPY_PANDAS = True
-except ImportError:
-    HAS_NUMPY_PANDAS = False
-
 
 class Encoder(json.JSONEncoder):
-    def default(self, obj: Any) -> Any:
+    """
+    JSON encoder with custom serialization for specific types.
+    """
+
+    def default(self, o: Any) -> Any:
         """
         Override the default() method to serialize additional types.
 
         Args:
-            obj: The object to be serialized.
+            o: The object to be serialized.
 
         Returns:
             The serialized object, or calls the superclass's default method if the object
             does not match any known type.
         """
 
-        if isinstance(obj, datetime):
-            return obj.isoformat()
-        elif isinstance(obj, date):
-            return obj.isoformat()
-        elif isinstance(obj, dt_time):
-            return obj.isoformat()
-        elif isinstance(obj, Decimal):
-            return float(obj)
-        elif isinstance(obj, Enum):
-            return obj.value
-        elif isinstance(obj, uuid.UUID):
-            return str(obj)
-        elif HAS_NUMPY_PANDAS:
-            if isinstance(obj, np.ndarray):
-                return obj.tolist()
-            elif "pandas" in str(type(obj)):
-                return obj.to_dict(orient="records")
-        elif hasattr(obj, "__dict__"):
-            # Serialize objects by their dictionary representation, filtering out non-serializable attributes
-            return {key: self.default(value) for key, value in obj.__dict__.items()}
+        if isinstance(o, datetime):
+            return o.isoformat()
+        elif isinstance(o, date):
+            return o.isoformat()
+        elif isinstance(o, time):
+            return o.isoformat()
+        elif isinstance(o, Decimal):
+            return float(o)
+        elif isinstance(o, Enum):
+            return o.value
+        elif isinstance(o, uuid.UUID):
+            return str(o)
+        elif hasattr(o, "__dict__"):
+            return {key: self.default(value) for key, value in o.__dict__.items()}
         else:
-            # Skip serialization for other non-handled types
-            return str(obj)  # Fallback to a simple string representation
+            return str(o)
```

### Comparing `vulcan-utils-1.12.1/vulcan_utils/formatter.py` & `vulcan-utils-1.12.2/vulcan_utils/formatter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,23 @@
-# vulcan_utils/formatter.py
+"""
+vulcan_utils/formatter.py
+
+This module provides the Formatter class, which handles conversion of milliseconds to human-readable 
+formats. Supports list, string w/custom delimiters, or dictionary format expressing years, months, 
+weeks, days, hours, minutes, seconds, and milliseconds.
+
+Classes:
+    Formatter: Formats durations from milliseconds into lists, strings, or dictionaries.
+
+Constants:
+    MS_IN_SECOND, MS_IN_MINUTE, MS_IN_HOUR, MS_IN_DAY, MS_IN_WEEK, MS_IN_MONTH, MS_IN_YEAR: 
+        Constants representing milliseconds in each respective time unit.
+"""
+
+
 MS_IN_SECOND = 1000
 MS_IN_MINUTE = 60 * MS_IN_SECOND
 MS_IN_HOUR = 60 * MS_IN_MINUTE
 MS_IN_DAY = 24 * MS_IN_HOUR
 MS_IN_WEEK = 7 * MS_IN_DAY
 MS_IN_MONTH = 30 * MS_IN_DAY  # Approximation
 MS_IN_YEAR = 365 * MS_IN_DAY  # Simplified, does not account for leap years
@@ -45,15 +60,16 @@
         """
         Calculate the duration breakdown from milliseconds to years.
 
         Args:
             milliseconds (int): Duration in milliseconds.
 
         Returns:
-            tuple: A tuple containing years, months, weeks, days, hours, minutes, seconds, milliseconds.
+            tuple: A tuple containing years, months, weeks, days, hours, minutes, seconds, 
+                milliseconds.
         """
 
         years = milliseconds // MS_IN_YEAR
         milliseconds %= MS_IN_YEAR
         months = milliseconds // MS_IN_MONTH
         milliseconds %= MS_IN_MONTH
         weeks = milliseconds // MS_IN_WEEK
```

### Comparing `vulcan-utils-1.12.1/vulcan_utils/logger.py` & `vulcan-utils-1.12.2/vulcan_utils/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,17 @@
-# vulcan_utils/logger.py
+"""
+vulcan_utils/logger.py
+
+This module provides a customizable logging utility designed to enhance standard logging with
+additional features like automatic inclusion of caller context (filename and line number),
+colored console output, and optional file logging. It is tailored to simplify debugging and log
+analysis by providing more detailed contextual information.
+"""
+
+
 import inspect
 import logging
 import os
 import sys
 from types import TracebackType
 from typing import Callable, Optional
 
@@ -11,30 +20,35 @@
 EXCLUDE = (
     'decorator.py',
     'logger.py',
     'logging/__init__.py',
     '<frozen importlib._bootstrap>'
 )
 
-LOG_FORMAT = "%(asctime)s - %(name)s - %(levelname)s - %(message)s - (%(caller_filename)s:%(caller_lineno)d)"
+LOG_FORMAT = (
+    "%(asctime)s - %(name)s - %(levelname)s - %(message)s - "
+    "(%(caller_filename)s:%(caller_lineno)d)"
+)
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class Logger:
     """
     A customizable logger class designed to enhance logging functionality by automatically
     including the caller's filename and line number in log messages. This feature provides
     detailed contextual information, facilitating easier debugging and log analysis. The logger
     supports configuring different log levels, colored console output, and optional file logging.
 
     Attributes:
-        level (str): The log level as a string, determining the severity of messages to be processed.
-        file_name (str): The name of the file where logs will be written, if file logging is enabled.
-        path (Optional[str]): The directory path for the log file. If not specified, file logging may 
-            be disabled or use a default path.
+        level (str): The log level as a string, determining the severity of messages to be 
+            processed.
+        file_name (str): The name of the file where logs will be written, if file logging is 
+            enabled.
+        path (Optional[str]): The directory path for the log file. If not specified, file logging 
+            may be disabled or use a default path.
     """
 
     def __init__(
         self,
         name: str = __name__,
         level: Optional[str] = None,
         file_name: Optional[str] = None,
@@ -74,34 +88,33 @@
         Args:
             path (Optional[str]): An explicit path for the log output.
 
         Returns:
             Optional[str]: The determined path as a string, or None if no path is determined.
         """
 
-        # TODO: Validate path before returning it.
         env_log_path = os.environ.get("VULCAN_LOG_PATH")
         if path:
             return path
         elif env_log_path:
             return env_log_path
         return None
 
     def _level(self, level: Optional[str]) -> str:
         """
-        Determines the effective log level for the logger instance, based on direct input or environment variables.
+        Determines the effective log level for the logger instance, based on direct input or 
+            environment variables.
 
         Args:
             level (Optional[str]): A specified log level as a string.
 
         Returns:
             str: The determined log level as a string.
         """
 
-        # TODO: Validate level before returning it.
         env_log_level = os.environ.get("VULCAN_LOG_LEVEL")
         if level:
             return level.upper()
         elif env_log_level:
             return env_log_level
         return "DEBUG"
 
@@ -130,15 +143,15 @@
         try:
             coloredlogs.install(
                 level=os.environ.get("VULCAN_LOG_LEVEL", self.level).upper(),
                 logger=self._logger,
                 fmt=LOG_FORMAT,
                 datefmt=DATE_FORMAT
             )
-        except Exception as e:
+        except Exception as e:  # pylint: disable=broad-except
             self.error(f"Error installing coloredlogs: {e}")
 
     def _file_handler(self) -> None:
         """
         Configures a file handler for logging, setting the log file path, level, and format.
         """
 
@@ -149,36 +162,39 @@
                 file_handler.setLevel(self.level.upper())
                 formatter = logging.Formatter(
                     fmt=LOG_FORMAT,
                     datefmt=DATE_FORMAT
                 )
                 file_handler.setFormatter(formatter)
                 self._logger.addHandler(file_handler)
-        except Exception as e:
+        except Exception as e:  # pylint: disable=broad-except
             self.error(f"Error creating log file handler: {e}")
 
     def _setup(self) -> None:
         """
-        Sets up the logging format, date format, installs colored logs, and configures file logging if VULCAN_LOG_PATH is set.
+        Sets up the logging format, date format, installs colored logs, and configures file logging 
+            if VULCAN_LOG_PATH is set.
         """
 
         self._install_coloredlogs()
         if self.path:
             try:
                 self._file_handler()
-            except Exception as e:
+            except Exception as e:  # pylint: disable=broad-except
                 self.error(
                     f"Error setting up file handler for logger: {e}")
 
     def _stack_trace(self) -> dict:
         """
-        Generates a stack trace to identify the caller's filename and line number, excluding specified files and modules.
+        Generates a stack trace to identify the caller's filename and line number, excluding 
+            specified files and modules.
 
         Returns:
-            dict: A dictionary with keys 'caller_filename' and 'caller_lineno', representing the file and line number of the log call origin.
+            dict: A dictionary with keys 'caller_filename' and 'caller_lineno', representing the 
+                file and line number of the log call origin.
         """
 
         stack = inspect.stack()
         caller_info = {"caller_filename": "Unknown", "caller_lineno": 0}
         for frame_info in stack[1:]:
             if not frame_info.filename.endswith(EXCLUDE):
                 caller_info['caller_filename'] = os.path.basename(
@@ -186,30 +202,34 @@
                 )
                 caller_info['caller_lineno'] = frame_info.lineno
                 break
         return caller_info
 
     def _exc_info(self) -> tuple[Optional[type], Optional[BaseException], Optional[TracebackType]]:
         """
-        Checks if there is an exception being handled in the current context and returns a tuple of exception information.
+        Checks if there is an exception being handled in the current context and returns a tuple of 
+            exception information.
 
         Returns:
-            tuple[Optional[type], Optional[BaseException], Optional[TracebackType]]: A tuple containing exception type, exception instance, and traceback information.
+            tuple[Optional[type], Optional[BaseException], Optional[TracebackType]]: A tuple 
+                containing exception type, exception instance, and traceback information.
         """
         exc_info = sys.exc_info()
         if exc_info:
             return exc_info[0] is not None
         return False
 
     def _base(self, func: Callable[[str, dict, bool], None], message: str) -> None:
         """
-        A base logging function that enriches log messages with caller details and conditional exception information.
+        A base logging function that enriches log messages with caller details and conditional 
+            exception information.
 
         Args:
-            func (Callable[[str, dict, bool], None]): A logging function (e.g., self._logger.debug) to be invoked with enriched logging information.
+            func (Callable[[str, dict, bool], None]): A logging function (e.g., self._logger.debug) 
+                to be invoked with enriched logging information.
             message (str): The log message.
         """
 
         caller_info = self._stack_trace()
         exc_info = self._exc_info()
         func(message, extra=caller_info, exc_info=exc_info)
```

### Comparing `vulcan-utils-1.12.1/vulcan_utils/printable.py` & `vulcan-utils-1.12.2/vulcan_utils/printable.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,19 @@
-# vulcan_utils/printable.py
+"""
+vulcan_utils/printable.py
+
+This module defines the Printable class, a mixin that enhances any class with
+automatic, detailed string representations of its instances. By inheriting from
+Printable, other classes can provide meaningful __str__ and __repr__ methods
+without additional coding. These methods generate string outputs that include
+all instance variables, making it easier to visualize object states during
+debugging and logging.
+"""
+
+
 class Printable:
     """
     A mixin class that provides a default implementation for printable representations
     of objects. This class overrides the __repr__ and __str__ methods to return
     a string representation of all attributes of an instance.
 
     The mixin can be inherited by other classes to automatically equip them with
```

### Comparing `vulcan-utils-1.12.1/vulcan_utils.egg-info/PKG-INFO` & `vulcan-utils-1.12.2/vulcan_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: vulcan-utils
-Version: 1.12.1
+Version: 1.12.2
 Summary: A utility package for Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: coloredlogs
 
 <!-- docs/README.md -->
 # Vulcan Utils
 
-Vulcan Utils is a Python package designed to enhance the logging capabilities of Python applications. It simplifies the logging process by automatically including critical details like the caller's filename and line number, making it easier to trace the source of log entries. The package supports a range of features including customizable log levels, colored logs, and conditional logging, tailored to improve both the development and debugging processes.
+Vulcan Utils is a Python package designed to enhance the functionality of Python applications through advanced logging and function decorators. It simplifies the integration of complex behaviors like logging, retry mechanisms, and rate limiting into applications with minimal code changes. Its robust features make it an ideal choice for developers looking to add sophisticated capabilities to their applications efficiently.
 
 **Requires Python 3.9 or higher**
 
 [View the full technical documentation here](https://vulcan-utils.readthedocs.io/en/latest/)
 
 [View the PyPi project here](https://pypi.org/project/vulcan-utils/)
 
@@ -25,21 +24,22 @@
 - **Colored Logs**: To enhance readability and facilitate quicker log analysis, Vulcan Utils supports colored logging, distinguishing log levels with different colors.
 - **Conditional Logging**: This feature offers advanced control over logging operations, enabling logs to be generated based on dynamic runtime conditions, thereby keeping log files concise and focused.
 - **Function Decorators**: Vulcan Utils introduces function decorators for logging, retrying, JSON serialization, and rate limiting, each adding a layer of functionality that enhances method executions with minimal code intrusion.
 - **Advanced Retry Mechanisms**: The retry decorators provide robust error handling by allowing repeated execution of functions upon failure, customizable by attempts and delays, which is invaluable for dealing with transient system or network issues.
 - **Automatic JSON Serialization**: Simplify data interchange in API services and other integrations with automatic JSON serialization of function outputs, streamlining responses and reducing boilerplate code.
 - **Rate Limiting Controls**: Enforce execution limits on functions with the rate limit decorator to manage resource utilization effectively and prevent system overload, which is essential for maintaining service availability and performance under high load.
 - **Caching**: Easy to use interface to connect with a Redis database, store, and retrieve data.
+- **Environment Variable Checks**: Function execution can be controlled based on the presence or specific values of environment variables, improving security and configuration flexibility.
 
 
 ## Installation
 You can install Vulcan Utils via PIP:
 
 ```bash
-pip install vulcan-logger
+pip install vulcan-utils
 ```
 
 ## Usage
 [View example usage here](https://github.com/nodadyoushutup/vulcan-utils/blob/main/example.py)
 
 Below are examples of how to use the Vulcan Utils logging and decoration features.
 
@@ -176,14 +176,26 @@
 #### Clearing the Cache
 Clear all keys and values in the currently selected Redis database.
 
 ```python
 cache.clear()
 ```
 
+### Environment variable checks
+Vulcan Utils now includes a decorator that enables function execution based on the presence or value of environment variables. This feature enhances security and configuration flexibility by allowing functions to run only when certain environmental conditions are met.
+
+```python
+from vulcan_utils.decorator import Decorator
+
+@Decorator.env(variable="CONFIG_MODE", value="production")
+def sensitive_operation():
+    """ Perform operations that are only safe in production environment """
+    pass
+```
+
 ### Advanced Configuration
 Vulcan Utils offers several environment variables to fine-tune logging behavior for your application. You can set these variables before initializing your logger to customize logging output, destination, and file naming.
 
 #### Setting Global Log Level
 Control the log level globally across your application by setting the `VULCAN_LOG_LEVEL` environment variable. This determines the minimum level of messages that will be logged. Available levels are `DEBUG`, `INFO`, `WARNING`, `ERROR`, and `CRITICAL`.
 
 _bash_
```

### Comparing `vulcan-utils-1.12.1/vulcan_utils.egg-info/SOURCES.txt` & `vulcan-utils-1.12.2/vulcan_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*


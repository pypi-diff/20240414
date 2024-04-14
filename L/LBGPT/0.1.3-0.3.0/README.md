# Comparing `tmp/lbgpt-0.1.3.tar.gz` & `tmp/lbgpt-0.3.0.tar.gz`

## Comparing `lbgpt-0.1.3.tar` & `lbgpt-0.3.0.tar`

### file list

```diff
@@ -1,41 +1,44 @@
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 lbgpt-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 lbgpt-0.1.3/Taskfile.yml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 lbgpt-0.1.3/compose.yaml
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 lbgpt-0.1.3/pytest.ini
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 lbgpt-0.1.3/requirements-testing.in
--rw-r--r--   0        0        0     6213 2020-02-02 00:00:00.000000 lbgpt-0.1.3/requirements-testing.txt
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 lbgpt-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 lbgpt-0.1.3/examples/chatgpt.ipynb
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 lbgpt-0.1.3/lbgpt/__init__.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 lbgpt-0.1.3/lbgpt/allocation.py
--rw-r--r--   0        0        0     9867 2020-02-02 00:00:00.000000 lbgpt-0.1.3/lbgpt/base.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 lbgpt-0.1.3/lbgpt/cache.py
--rw-r--r--   0        0        0     9965 2020-02-02 00:00:00.000000 lbgpt-0.1.3/lbgpt/lbgpt.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 lbgpt-0.1.3/lbgpt/types.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 lbgpt-0.1.3/lbgpt/usage.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 lbgpt-0.1.3/lbgpt/semantic_cache/__init__.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 lbgpt-0.1.3/lbgpt/semantic_cache/base.py
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 lbgpt-0.1.3/lbgpt/semantic_cache/faiss_cache.py
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 lbgpt-0.1.3/lbgpt/semantic_cache/qdrant_cache.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 lbgpt-0.1.3/tests/conftest.py
--rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 lbgpt-0.1.3/tests/test_lb.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 lbgpt-0.1.3/tests/cache/test_immutability.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 lbgpt-0.1.3/tests/cache/test_lb_cache.py
--rw-r--r--   0        0        0     6569 2020-02-02 00:00:00.000000 lbgpt-0.1.3/tests/cache/cassette/test_lb_cache/test_chatgpt_cache[cache0].yaml
--rw-r--r--   0        0        0    11320 2020-02-02 00:00:00.000000 lbgpt-0.1.3/tests/cassette/test_lb/test_azure_async.yaml
--rw-r--r--   0        0        0    16385 2020-02-02 00:00:00.000000 lbgpt-0.1.3/tests/cassette/test_lb/test_chatgpt_async.yaml
--rw-r--r--   0        0        0    13346 2020-02-02 00:00:00.000000 lbgpt-0.1.3/tests/cassette/test_lb/test_lb_async_random.yaml
--rw-r--r--   0        0        0    16387 2020-02-02 00:00:00.000000 lbgpt-0.1.3/tests/cassette/test_lb/test_lbgpt_max_headroom.yaml
--rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 lbgpt-0.1.3/tests/semantic_cache/test_lb_semantic_cache.py
--rw-r--r--   0        0        0    14190 2020-02-02 00:00:00.000000 lbgpt-0.1.3/tests/semantic_cache/test_qdrant.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 lbgpt-0.1.3/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_exact[-lambda-0].yaml
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 lbgpt-0.1.3/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_exact[-lambda-1].yaml
--rw-r--r--   0        0        0     6569 2020-02-02 00:00:00.000000 lbgpt-0.1.3/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_failed[-lambda-0].yaml
--rw-r--r--   0        0        0     6569 2020-02-02 00:00:00.000000 lbgpt-0.1.3/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_failed[-lambda-1].yaml
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 lbgpt-0.1.3/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_inexact[-lambda-0].yaml
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 lbgpt-0.1.3/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_inexact[-lambda-1].yaml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 lbgpt-0.1.3/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 lbgpt-0.1.3/LICENSE
--rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 lbgpt-0.1.3/README.md
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 lbgpt-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     8321 2020-02-02 00:00:00.000000 lbgpt-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 lbgpt-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 lbgpt-0.3.0/Taskfile.yml
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 lbgpt-0.3.0/compose.yaml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 lbgpt-0.3.0/pytest.ini
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 lbgpt-0.3.0/requirements-testing.in
+-rw-r--r--   0        0        0     6213 2020-02-02 00:00:00.000000 lbgpt-0.3.0/requirements-testing.txt
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 lbgpt-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 lbgpt-0.3.0/examples/chatgpt.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lbgpt-0.3.0/src/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 lbgpt-0.3.0/src/lbgpt/__init__.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 lbgpt-0.3.0/src/lbgpt/allocation.py
+-rw-r--r--   0        0        0    13829 2020-02-02 00:00:00.000000 lbgpt-0.3.0/src/lbgpt/base.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 lbgpt-0.3.0/src/lbgpt/cache.py
+-rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 lbgpt-0.3.0/src/lbgpt/lbgpt.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 lbgpt-0.3.0/src/lbgpt/types.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 lbgpt-0.3.0/src/lbgpt/usage.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 lbgpt-0.3.0/src/lbgpt/semantic_cache/__init__.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 lbgpt-0.3.0/src/lbgpt/semantic_cache/base.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 lbgpt-0.3.0/src/lbgpt/semantic_cache/faiss_cache.py
+-rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 lbgpt-0.3.0/src/lbgpt/semantic_cache/qdrant_cache.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 lbgpt-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 lbgpt-0.3.0/tests/test_lb.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 lbgpt-0.3.0/tests/cache/test_immutability.py
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 lbgpt-0.3.0/tests/cache/test_lb_cache.py
+-rw-r--r--   0        0        0     6569 2020-02-02 00:00:00.000000 lbgpt-0.3.0/tests/cache/cassette/test_lb_cache/test_chatgpt_cache[cache0].yaml
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 lbgpt-0.3.0/tests/cache/cassette/test_lb_cache/test_chatgpt_cache[cache1].yaml
+-rw-r--r--   0        0        0    11320 2020-02-02 00:00:00.000000 lbgpt-0.3.0/tests/cassette/test_lb/test_azure_async.yaml
+-rw-r--r--   0        0        0    16385 2020-02-02 00:00:00.000000 lbgpt-0.3.0/tests/cassette/test_lb/test_chatgpt_async.yaml
+-rw-r--r--   0        0        0    13110 2020-02-02 00:00:00.000000 lbgpt-0.3.0/tests/cassette/test_lb/test_chatgpt_async_multiple_starts.yaml
+-rw-r--r--   0        0        0    13346 2020-02-02 00:00:00.000000 lbgpt-0.3.0/tests/cassette/test_lb/test_lb_async_random.yaml
+-rw-r--r--   0        0        0    16387 2020-02-02 00:00:00.000000 lbgpt-0.3.0/tests/cassette/test_lb/test_lbgpt_max_headroom.yaml
+-rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 lbgpt-0.3.0/tests/semantic_cache/test_lb_semantic_cache.py
+-rw-r--r--   0        0        0    14283 2020-02-02 00:00:00.000000 lbgpt-0.3.0/tests/semantic_cache/test_qdrant.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 lbgpt-0.3.0/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_exact[-lambda-0].yaml
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 lbgpt-0.3.0/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_exact[-lambda-1].yaml
+-rw-r--r--   0        0        0     6569 2020-02-02 00:00:00.000000 lbgpt-0.3.0/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_failed[-lambda-0].yaml
+-rw-r--r--   0        0        0     6569 2020-02-02 00:00:00.000000 lbgpt-0.3.0/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_failed[-lambda-1].yaml
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 lbgpt-0.3.0/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_inexact[-lambda-0].yaml
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 lbgpt-0.3.0/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_inexact[-lambda-1].yaml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 lbgpt-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 lbgpt-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 lbgpt-0.3.0/README.md
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 lbgpt-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8372 2020-02-02 00:00:00.000000 lbgpt-0.3.0/PKG-INFO
```

### Comparing `lbgpt-0.1.3/Taskfile.yml` & `lbgpt-0.3.0/Taskfile.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # https://taskfile.dev
 
 version: '3'
 
 env:
-  PYTHONPATH: .
+  PYTHONPATH: ./src
 
 dotenv: ['.env']
 
 tasks:
   update-pip-build-tools:
     internal: true
     cmds:
@@ -38,22 +38,24 @@
     cmds:
       - task: docker:start
       - pytest
 
   lint:
     desc: Linting
     cmds:
-      - black lbgpt/
+      - black src/
       - black tests/
 
-      - isort lbgpt/ --profile black --filter-files
+      - isort src/ --profile black --filter-files
       - isort tests/ --profile black --filter-files
 
   docker:start:
     desc: Starts docker containers
     cmds:
-      - docker-compose up -d
+      - cmd: docker-compose up -d
+        ignore_error: true
+
 
   docker:stop:
     desc: Stops docker containers
     cmds:
       - docker-compose down
```

### Comparing `lbgpt-0.1.3/requirements-testing.txt` & `lbgpt-0.3.0/requirements-testing.txt`

 * *Files identical despite different names*

### Comparing `lbgpt-0.1.3/.github/workflows/python-publish.yml` & `lbgpt-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lbgpt-0.1.3/examples/chatgpt.ipynb` & `lbgpt-0.3.0/examples/chatgpt.ipynb`

 * *Files identical despite different names*

### Comparing `lbgpt-0.1.3/lbgpt/allocation.py` & `lbgpt-0.3.0/src/lbgpt/allocation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import asyncio
 import random
 from logging import getLogger
 from typing import Optional, Sequence
 
+import tenacity
+
 from lbgpt.base import _BaseGPT
 
 logger = getLogger(__name__)
 
 
 async def random_allocation_function(
     gpts: list[_BaseGPT], weights=Optional[Sequence[float]], **kwargs
@@ -17,23 +19,22 @@
 async def max_headroom_allocation_function(
     gpts: list[_BaseGPT], overallocate: bool = False, **kwargs
 ) -> _BaseGPT:
     """
     Returns the model with the most headroom. If overallocate is set to true return the model with the most headroom
     even if there is no allocation left available. Otherwise, we are waiting here until the overallocation is resolved
     """
-
-    # choosing a random one in case of a tie
-    best_alternative = max(gpts, key=lambda gpt: (gpt.headroom(), random.random()))
+    gpts_with_headroom = [(await gpt.headroom(), gpt) for gpt in gpts]
+    best_headroom, best_alternative = max(gpts_with_headroom, key=lambda gpt: (gpt[0], random.random()))
 
     if overallocate:
         return best_alternative
 
     else:
-        if best_alternative.headroom() > 0:
+        if best_headroom > 0:
             return best_alternative
         else:
             await asyncio.sleep(1)
             logger.info(
                 "waiting for overallocation to resolve, best alternative: %s",
                 best_alternative,
             )
```

### Comparing `lbgpt-0.1.3/lbgpt/base.py` & `lbgpt-0.3.0/src/lbgpt/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 # -*- coding: utf-8 -*-
 import abc
 import asyncio
 import datetime
+import json
 import logging
 import sys
 import warnings
 from logging import getLogger
 from statistics import median
 from typing import Any, Callable, Optional, Sequence
 
 import openai
-from openai.types.chat import ChatCompletion
+from openai._compat import model_dump, model_parse
 from tenacity import (
     AsyncRetrying,
     RetryCallState,
     retry_if_exception_type,
     stop_after_attempt,
     wait_random_exponential,
 )
-from tqdm.asyncio import tqdm
 from tqdm.contrib.logging import logging_redirect_tqdm
 
 from lbgpt.cache import make_hash_chatgpt_request
 from lbgpt.semantic_cache.base import _SemanticCacheBase
 from lbgpt.types import ChatCompletionAddition
 from lbgpt.usage import Usage, UsageStats
 
 logger = getLogger(__name__)
 
 
 def after_logging(
     logger_level: int = logging.WARNING,
+    logger_exception: bool = True,
 ) -> Callable[[RetryCallState], None]:
     def logging_function(retry_state: RetryCallState) -> None:
         with logging_redirect_tqdm():
+            exception = retry_state.outcome.exception()
             logger.log(
                 level=logger_level,
-                msg=f"Retrying request after {'%0.2f' % retry_state.seconds_since_start}s as attempt {retry_state.attempt_number} ended with `{retry_state.outcome.exception()}`",
+                msg=f"Retrying request after {'%0.2f' % retry_state.seconds_since_start}s as attempt {retry_state.attempt_number} ended with `{repr(exception)}`",
             )
 
+            if logger_exception:
+                logger.exception(exception)
+                if hasattr(exception, "request"):
+                    logger.error(exception.request)
+
     return logging_function
 
 
 class _BaseGPT(abc.ABC):
     def __init__(
         self,
         max_parallel_calls: int,
@@ -50,91 +57,108 @@
         semantic_cache: Optional[Any] = None,
         stop_after_attempts: Optional[int] = 10,
         stop_on_exception: bool = False,
         max_usage_cache_size: Optional[int] = 1_000,
         limit_tpm: Optional[int] = None,
         limit_rpm: Optional[int] = None,
         propagate_standard_cache_to_semantic_cache: bool = False,
+        propagate_semantic_cache_to_standard_cache: bool = False,
     ):
         # this is standard cache, i.e. it only checks for equal items
         self.cache = cache
         self.semantic_cache: _SemanticCacheBase = semantic_cache
 
         self.max_parallel_calls = max_parallel_calls
-        self.semaphore = asyncio.Semaphore(value=self.max_parallel_calls)
         self.stop_after_attempts = stop_after_attempts
         self.stop_on_exception = stop_on_exception
 
         self._usage_cache_list = []
         self.max_usage_cache_size = max_usage_cache_size
 
         self.limit_tpm = limit_tpm
         self.limit_rpm = limit_rpm
 
         self.propagate_standard_cache_to_semantic_cache = (
             propagate_standard_cache_to_semantic_cache
         )
+        self.propagate_semantic_cache_to_standard_cache = (
+            propagate_semantic_cache_to_standard_cache
+        )
 
         # this is a silly configuration (propagating to semantic cache without having a semantic cache)
         if (
             self.propagate_standard_cache_to_semantic_cache
             and self.semantic_cache is None
         ):
             self.propagate_standard_cache_to_semantic_cache = False
             warnings.warn(
                 "propagate_standard_cache_to_semantic_cache is True, but no semantic cache is provided. There will be no propagation."
             )
 
+        # this is a silly configuration (propagating to standard cache without having a standard cache)
+        if self.propagate_semantic_cache_to_standard_cache and self.cache is None:
+            self.propagate_semantic_cache_to_standard_cache = False
+            warnings.warn(
+                "propagate_semantic_cache_to_standard_cache is True, but no standard cache is provided. There will be no propagation."
+            )
+
+        self.semaphore_chatgpt = asyncio.Semaphore(self.max_parallel_calls)
+        self.semaphore_standard_cache = asyncio.Semaphore(self.max_parallel_calls)
+        self.semaphore_semantic_cache = asyncio.Semaphore(self.max_parallel_calls)
+
+    def request_setup(self):
+        pass
+
     @property
-    def usage_cache_list(self) -> list[Usage]:
+    async def usage_cache_list(self) -> list[Usage]:
         return self._usage_cache_list
 
-    def add_usage_to_usage_cache(self, usage: Usage):
+    async def add_usage_to_usage_cache(self, usage: Usage):
         # evict if the list is too long. Do this to protect memory usage if required
         if (
             self.max_usage_cache_size
             and len(self._usage_cache_list) > self.max_usage_cache_size
         ):
             self._usage_cache_list.pop(0)
 
         self._usage_cache_list.append(usage)
 
-    def usage_cache_list_after_start_datetime(
+    async def usage_cache_list_after_start_datetime(
         self, start_datetime: datetime.datetime
     ) -> list[Usage]:
         return [k for k in self._usage_cache_list if k.start_datetime > start_datetime]
 
-    def get_usage_stats(self, include_usage_reservation: bool = False) -> UsageStats:
+    async def get_usage_stats(self, include_usage_reservation: bool = False) -> UsageStats:
         current_usage_tokens = 0
         current_usage_requests = 0
 
         if include_usage_reservation:
             # Estimating current usage as the expected number of tokens times the number of
             # currently outstanding requests (which are tracked in the semaphore)
             current_usage_tokens = (
-                self.semaphore._value * self.expected_tokens_per_request()
+                self.semaphore_chatgpt._value * await self.expected_tokens_per_request()
             )
-            current_usage_requests = self.semaphore._value
+            current_usage_requests = self.semaphore_chatgpt._value
 
-        cache_list_after_start_datetime = self.usage_cache_list_after_start_datetime(
+        cache_list_after_start_datetime = await self.usage_cache_list_after_start_datetime(
             datetime.datetime.now() - datetime.timedelta(seconds=60)
         )
 
         return UsageStats(
             tokens=sum(
                 [
                     k.input_tokens + k.output_tokens
                     for k in cache_list_after_start_datetime
                 ]
             )
             + current_usage_tokens,
             requests=len(cache_list_after_start_datetime) + current_usage_requests,
         )
 
-    def expected_tokens_per_request(self) -> int:
+    async def expected_tokens_per_request(self) -> int:
         """Returns the expected number of tokens per usage
         We are returning the following (in subsequent order of preference):
         (1) the median number of tokens per usage in the cache
         (2) 10% of the limit_tpm
         (3) zero otherwise
         """
         if len(self._usage_cache_list) > 0:
@@ -145,123 +169,192 @@
             )
 
         if self.limit_tpm:
             return int(self.limit_tpm * 0.1)
         else:
             return 0
 
-    def headroom(self) -> int:
+    async def headroom(self) -> int:
         """Returns the number of tokens remaining in the current minute"""
-        cur_usage = self.get_usage_stats()
+        cur_usage = await self.get_usage_stats()
 
         if self.limit_tpm:
             headroom_tpm = (
-                self.limit_tpm - cur_usage.tokens - self.expected_tokens_per_request()
+                self.limit_tpm - cur_usage.tokens - await self.expected_tokens_per_request()
             )
         else:
             headroom_tpm = sys.maxsize
 
         if self.limit_rpm:
-            headroom_rpm = self.expected_tokens_per_request() * (
+            headroom_rpm = await self.expected_tokens_per_request() * (
                 self.limit_rpm - cur_usage.requests - 1
             )
         else:
             headroom_rpm = sys.maxsize
 
         return min([headroom_tpm, headroom_rpm])
 
-    def refresh(self) -> None:
-        semaphore = asyncio.Semaphore(value=self.max_parallel_calls)
-        self.semaphore = semaphore
-
     @abc.abstractmethod
-    async def chat_completion(self, **kwargs) -> ChatCompletionAddition:
+    async def chat_completion(self, semaphore: Optional[asyncio.Semaphore] = None, **kwargs) -> ChatCompletionAddition:
         raise NotImplementedError
 
     async def chat_completion_list(
         self,
         chatgpt_chat_completion_request_body_list: list[dict],
         show_progress=True,
         logging_level: int = logging.WARNING,
+        logging_exception: bool = False,
     ) -> Sequence[ChatCompletionAddition]:
-        self.refresh()
 
-        return await tqdm.gather(
-            *[
-                self.cached_chat_completion(logging_level=logging_level, **content)
-                for content in chatgpt_chat_completion_request_body_list
-            ],
-            disable=not show_progress,
-        )
+        # we are setting up the semaphore here, so that we can refresh it if required
+        # we are rate limiting the three things we care about: gpt requests, standard cache requests,
+        # and semantic cache requests.
+
+        async with asyncio.TaskGroup() as tg:
+            tasks = [tg.create_task(
+                self.cached_chat_completion(
+                    logging_level=logging_level,
+                    logging_exception=logging_exception,
+                    content=content,
+                )
+            ) for content in chatgpt_chat_completion_request_body_list]
+
+        return [t.result() for t in tasks]
 
-    def _request_from_cache(self, hashed: str) -> Optional[ChatCompletionAddition]:
+    def _get_from_cache(self, hashed: str) -> Optional[ChatCompletionAddition]:
         if self.cache is not None:
+            logger.debug(f'trying to get {hashed} from standard cache')
             out = self.cache.get(hashed)
+
             if out is not None:
-                logger.debug("standard cache hit")
-                return out
+                logger.debug(f'found request {hashed} in standard cache')
+                out_dict = json.loads(out)
+                out_dict['is_cached'] = True
 
-    async def cached_chat_completion(
-        self, logging_level: int = logging.WARNING, **kwargs
-    ) -> Optional[ChatCompletionAddition]:
-        # we want to stagger even the cache access a bit, otherwise all requests immediately hit cache
-        # but do not see if a later request is putting anything into the cache.
-        # Thus, we are limiting the number of parallel executions here
+                return model_parse(ChatCompletionAddition, out_dict)
 
-        async with self.semaphore:
-            # this is standard cache. We are always trying standard cache first
-            if self.cache is not None:
-                hashed = make_hash_chatgpt_request(kwargs)
-                out = self._request_from_cache(hashed)
-                if out is not None and self.propagate_standard_cache_to_semantic_cache:
+    def _set_to_cache(self, hashed: str, value: ChatCompletionAddition):
+        if self.cache is not None:
+            self.cache.set(hashed, json.dumps(model_dump(value)))
+
+    async def get_chat_completion_from_cache(
+        self, hashed: str, **kwargs
+    ) -> Optional[ChatCompletionAddition]:
+        if self.cache is not None:
+            async with self.semaphore_standard_cache:
+                out = self._get_from_cache(hashed)
+            if out is not None:
+                # propagate to semantic cache if required
+                if self.propagate_standard_cache_to_semantic_cache:
+                    logger.debug("checking if the element exists in semantic cache")
                     try:
                         existing_item = await self.semantic_cache.query_cache(kwargs)
                     except Exception:
                         existing_item = None
 
                     if existing_item is None:
                         logger.debug("propagating standard cache to semantic cache")
                         await self.semantic_cache.add_cache(kwargs, out)
 
+                # but return in any case
+                return out
+
+        # if the item is not in the standard cache, we are trying the semantic cache (if available)
+        # we are currently only supporting semantic cache for FAISS models
+        if self.semantic_cache is not None:
+            logger.debug(f'trying to get {hashed} from semantic cache')
+            async with self.semaphore_semantic_cache:
+                out: Optional[
+                    ChatCompletionAddition
+                ] = await self.semantic_cache.query_cache(kwargs)
+
+            if out is not None:
+                # propagate to standard cache (we know it is not in standard cache),
+                # otherwise we would not end up here
+                logger.debug(f'found request {hashed} in semantic cache')
+
+                if self.propagate_semantic_cache_to_standard_cache and out.is_exact:
+                    logger.debug("propagating semantic cache to standard cache")
+                    self._set_to_cache(hashed, out)
+
+                return out
+
+    async def set_chat_completion_to_cache(
+        self, hashed: str, out: ChatCompletionAddition, request_params: dict[str, Any]
+    ) -> None:
+        if self.semantic_cache is not None:
+            logger.debug(f"adding request {hashed} to semantic cache")
+            await self.semantic_cache.add_cache(request_params, out)
+
+        if self.cache is not None:
+            logger.debug(f"adding request {hashed} to standard cache")
+            self._set_to_cache(hashed, out)
+
+    async def retrying_chat_completion(
+        self,
+        logging_level: int = logging.WARNING,
+        logging_exception: bool = False,
+        semaphore: Optional[asyncio.Semaphore] = None,
+        **kwargs,
+    ) -> Optional[ChatCompletionAddition]:
+
+        logger.debug('requesting chat completion for GPT model')
+        try:
+            async for attempt in AsyncRetrying(
+                retry=(
+                    retry_if_exception_type(openai.APIConnectionError)
+                    | retry_if_exception_type(openai.RateLimitError)
+                    | retry_if_exception_type(openai.InternalServerError)
+                    # shall also retry for bad gateway error (502)
+                    # profile the error when it comes up again
+                ),
+                wait=wait_random_exponential(min=5, max=60),
+                stop=stop_after_attempt(self.stop_after_attempts)
+                if self.stop_after_attempts is not None
+                else None,
+                after=after_logging(
+                    logger_level=logging_level, logger_exception=logging_exception
+                ),
+            ):
+                with attempt:
+                    out: ChatCompletionAddition = await self.chat_completion(**kwargs)
+                    logger.debug('got chat completion for GPT model')
                     return out
 
-            # if the item is not in the standard cache, we are trying the semantic cache (if available)
-            # we are currently only supporting semantic cache for FAISS models
-            if self.semantic_cache is not None:
-                sc: Optional[ChatCompletionAddition] = await self.semantic_cache.query_cache(
-                    kwargs
-                )
-                if sc is not None:
-                    logger.debug("semantic cache hit")
-                    return sc
-
-            try:
-                async for attempt in AsyncRetrying(
-                    retry=(
-                        retry_if_exception_type(openai.APIConnectionError)
-                        | retry_if_exception_type(openai.RateLimitError)
-                        # shall also retry for bad gateway error (502)
-                        # profile the error when it comes up again
-                    ),
-                    wait=wait_random_exponential(min=5, max=60),
-                    stop=stop_after_attempt(self.stop_after_attempts)
-                    if self.stop_after_attempts is not None
-                    else None,
-                    after=after_logging(logger_level=logging_level),
-                ):
-                    with attempt:
-                        out: ChatCompletionAddition = await self.chat_completion(**kwargs)
-
-            except Exception as e:
-                if self.stop_on_exception:
-                    raise e
-                else:
-                    logger.exception(e)
-                    return None
+        except Exception as e:
+            if self.stop_on_exception:
+                raise e
+            else:
+                logger.exception(e)
+                return None
+
+
+    async def cached_chat_completion(
+        self,
+        content: dict[str, Any],
+        logging_level: int = logging.WARNING,
+        logging_exception: bool = False,
+
+    ) -> Optional[ChatCompletionAddition]:
+        # we want to stagger even the cache access a bit, otherwise all requests immediately hit cache
+        # but do not see if a later request is putting anything into the cache.
+        # Thus, we are limiting the number of parallel executions here
+
+        hashed = make_hash_chatgpt_request(content)
+
+        # accessing cache, returning if available, otherwise proceeding.
+        cached_result = await self.get_chat_completion_from_cache(hashed, **content)
+        if cached_result is not None:
+            return cached_result
+
+        out = await self.retrying_chat_completion(
+            logging_level=logging_level, logging_exception=logging_exception, **content
+        )
+
+        if out is not None:
+            await self.set_chat_completion_to_cache(
+                hashed=hashed, out=out, request_params=content
+            )
 
-            if self.semantic_cache is not None:
-                await self.semantic_cache.add_cache(kwargs, out)
+        return out
 
-            if self.cache is not None:
-                self.cache[hashed] = out
 
-            return out
```

### Comparing `lbgpt-0.1.3/lbgpt/cache.py` & `lbgpt-0.3.0/src/lbgpt/cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,16 @@
         tool_choice=chat_completion_create.get("tool_choice"),
         function_call=chat_completion_create.get("function_call"),
         functions=chat_completion_create.get("functions"),
     )
 
 
 def make_hash_chatgpt_request(
-    chat_completion_create: CompletionCreateParams | dict[str, Any]
+    chat_completion_create: CompletionCreateParams | dict[str, Any],
+    include_messages: bool = True,
 ) -> str:
     """Converting a chatgpt request to a hash for caching and deduplication purposes"""
 
     non_message_parameters = non_message_parameters_from_create(
         chat_completion_create=chat_completion_create
     )
 
@@ -43,16 +44,17 @@
             "role": message["role"],
         }
         for message in chat_completion_create["messages"]
     ]
 
     hasher = hashlib.sha256()
     hasher.update(repr(make_hashable(non_message_parameters)).encode())
-    hasher.update(repr(make_hashable(messages)).encode())
-    return base64.b64encode(hasher.digest()).decode()
+    if include_messages:
+        hasher.update(repr(make_hashable(messages)).encode())
+    return f"lbgpt_{base64.b64encode(hasher.digest()).decode()}"
 
 
 def make_hashable(o):
     if isinstance(o, (tuple, list)):
         return tuple((make_hashable(e) for e in o))
 
     if isinstance(o, dict):
```

### Comparing `lbgpt-0.1.3/lbgpt/lbgpt.py` & `lbgpt-0.3.0/src/lbgpt/lbgpt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 import datetime
 from asyncio import Timeout
 from logging import getLogger
 from typing import Any, Optional, Sequence
 
-import httpx
 import openai
 from openai._types import NOT_GIVEN, NotGiven
 
 from lbgpt.allocation import (
     max_headroom_allocation_function,
     random_allocation_function,
 )
@@ -24,138 +23,150 @@
         self,
         api_key: str,
         max_parallel_calls: int = 5,
         request_timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         cache: Optional[Any] = None,
         semantic_cache: Optional[Any] = None,
         propagate_standard_cache_to_semantic_cache: bool = False,
+        propagate_semantic_cache_to_standard_cache: bool = False,
         stop_after_attempts: Optional[int] = 10,
         stop_on_exception: bool = False,
         max_usage_cache_size: Optional[int] = 1_000,
         limit_tpm: Optional[int] = None,
         limit_rpm: Optional[int] = None,
     ):
         super().__init__(
             cache=cache,
             semantic_cache=semantic_cache,
             propagate_standard_cache_to_semantic_cache=propagate_standard_cache_to_semantic_cache,
+            propagate_semantic_cache_to_standard_cache=propagate_semantic_cache_to_standard_cache,
             max_parallel_calls=max_parallel_calls,
             stop_after_attempts=stop_after_attempts,
             stop_on_exception=stop_on_exception,
             max_usage_cache_size=max_usage_cache_size,
             limit_tpm=limit_tpm,
             limit_rpm=limit_rpm,
         )
 
-        self.client = openai.AsyncOpenAI(
-            api_key=api_key,
-            timeout=request_timeout,
+        self.api_key = api_key
+        self.request_timeout = request_timeout
+
+    def get_client(self) -> openai.AsyncOpenAI:
+        return openai.AsyncOpenAI(
+            api_key=self.api_key,
+            timeout=self.request_timeout,
             max_retries=0,
         )
 
-    def refresh(self) -> None:
-        self.client = self.client.copy(http_client=httpx.AsyncClient())
-        super().refresh()
-
     async def chat_completion(self, **kwargs) -> ChatCompletionAddition:
         # one request to the OpenAI API respecting their ratelimit
+        async with self.semaphore_chatgpt:
+            timeout = kwargs.pop("request_timeout", self.request_timeout)
 
-        timeout = kwargs.pop("request_timeout", self.client.timeout)
-
-        async with self.semaphore:
             start = datetime.datetime.now()
-            out = await self.client.with_options(
-                timeout=timeout
-            ).chat.completions.create(
-                **kwargs,
-            )
-            self.add_usage_to_usage_cache(
-                Usage(
-                    input_tokens=out.usage.prompt_tokens,
-                    output_tokens=out.usage.total_tokens,
-                    start_datetime=start,
-                    end_datetime=datetime.datetime.now(),
+            out = (
+                await self.get_client()
+                .with_options(timeout=timeout)
+                .chat.completions.create(
+                    **kwargs,
                 )
             )
 
-            return ChatCompletionAddition.from_chat_completion(out)
+        await self.add_usage_to_usage_cache(
+            Usage(
+                input_tokens=out.usage.prompt_tokens,
+                output_tokens=out.usage.total_tokens,
+                start_datetime=start,
+                end_datetime=datetime.datetime.now(),
+            )
+        )
+
+        return ChatCompletionAddition.from_chat_completion(out, model_class=self.__class__.__name__)
 
 
 class AzureGPT(_BaseGPT):
     def __init__(
         self,
         api_key: str,
         azure_api_base: str,
         azure_model_map: dict[str, str],
         cache: Optional[Any] = None,
         semantic_cache: Optional[Any] = None,
         propagate_standard_cache_to_semantic_cache: bool = False,
-        azure_openai_version: str = "2023-05-15",
+        propagate_semantic_cache_to_standard_cache: bool = False,
+        azure_openai_version: str = "2024-02-01",
         azure_openai_type: str = "azure",
         max_parallel_calls: int = 5,
         request_timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         stop_after_attempts: Optional[int] = 10,
         stop_on_exception: bool = False,
         max_usage_cache_size: Optional[int] = 1_000,
         limit_tpm: Optional[int] = None,
         limit_rpm: Optional[int] = None,
     ):
         super().__init__(
             cache=cache,
             semantic_cache=semantic_cache,
             propagate_standard_cache_to_semantic_cache=propagate_standard_cache_to_semantic_cache,
+            propagate_semantic_cache_to_standard_cache=propagate_semantic_cache_to_standard_cache,
             max_parallel_calls=max_parallel_calls,
             stop_after_attempts=stop_after_attempts,
             stop_on_exception=stop_on_exception,
             max_usage_cache_size=max_usage_cache_size,
             limit_tpm=limit_tpm,
             limit_rpm=limit_rpm,
         )
 
-        self.client = openai.AsyncAzureOpenAI(
-            api_key=api_key,
-            azure_endpoint=azure_api_base,
-            api_version=azure_openai_version,
-            timeout=request_timeout,
-            max_retries=0,
-        )
+        self.api_key = api_key
+        self.azure_api_base = azure_api_base
+        self.azure_openai_version = azure_openai_version
+        self.request_timeout = request_timeout
 
         self.azure_model_map = azure_model_map
 
-    def refresh(self) -> None:
-        self.client = self.client.copy(http_client=httpx.AsyncClient())
-        super().refresh()
+    def get_client(self) -> openai.AsyncAzureOpenAI:
+        return openai.AsyncAzureOpenAI(
+            api_key=self.api_key,
+            azure_endpoint=self.azure_api_base,
+            api_version=self.azure_openai_version,
+            timeout=self.request_timeout,
+            max_retries=0,
+        )
 
     async def chat_completion(self, **kwargs) -> ChatCompletionAddition:
         """One request to the Azure OpenAI API respecting their ratelimit
         # needs to change the model parameter to deployment id
         """
 
         deployment_id = self.azure_model_map[kwargs["model"]]
         kwargs["model"] = deployment_id
 
-        timeout = kwargs.pop("request_timeout", self.client.timeout)
+        timeout = kwargs.pop("request_timeout", self.request_timeout)
 
-        async with self.semaphore:
-            start = datetime.datetime.now()
-            out = await self.client.with_options(
-                timeout=timeout
-            ).chat.completions.create(
-                **kwargs,
-            )
-            self.add_usage_to_usage_cache(
-                Usage(
-                    input_tokens=out.usage.prompt_tokens,
-                    output_tokens=out.usage.total_tokens,
-                    start_datetime=start,
-                    end_datetime=datetime.datetime.now(),
+        start = datetime.datetime.now()
+
+        async with self.semaphore_chatgpt:
+            out = (
+                await self.get_client()
+                .with_options(timeout=timeout)
+                .chat.completions.create(
+                    **kwargs,
                 )
             )
 
-            return ChatCompletionAddition.from_chat_completion(out)
+        await self.add_usage_to_usage_cache(
+            Usage(
+                input_tokens=out.usage.prompt_tokens,
+                output_tokens=out.usage.total_tokens,
+                start_datetime=start,
+                end_datetime=datetime.datetime.now(),
+            )
+        )
+
+        return ChatCompletionAddition.from_chat_completion(out, model_class=self.__class__.__name__)
 
 
 ALLOCATION_FUNCTIONS = {
     "random": random_allocation_function,
     "max_headroom": max_headroom_allocation_function,
 }
 
@@ -166,14 +177,15 @@
         gpts: list[_BaseGPT],
         allocation_function: str = "random",
         allocation_function_kwargs: Optional[dict] = None,
         allocation_function_weights: Optional[Sequence] = None,
         cache: Optional[Any] = None,
         semantic_cache: Optional[Any] = None,
         propagate_standard_cache_to_semantic_cache: bool = False,
+        propagate_semantic_cache_to_standard_cache: bool = False,
         stop_after_attempts: Optional[int] = 10,
         stop_on_exception: bool = False,
         max_parallel_requests: Optional[int] = None,
     ):
         self.gpts = gpts
 
         if isinstance(allocation_function, str):
@@ -195,22 +207,28 @@
         if max_parallel_requests is None:
             max_parallel_requests = sum([gpt.max_parallel_calls for gpt in gpts])
 
         super().__init__(
             cache=cache,
             semantic_cache=semantic_cache,
             propagate_standard_cache_to_semantic_cache=propagate_standard_cache_to_semantic_cache,
+            propagate_semantic_cache_to_standard_cache=propagate_semantic_cache_to_standard_cache,
             max_parallel_calls=max_parallel_requests,
             stop_after_attempts=stop_after_attempts,
             stop_on_exception=stop_on_exception,
         )
 
+    def request_setup(self):
+        for gpt in self.gpts:
+            gpt.request_setup()
+        super().request_setup()
+
     @property
-    def usage_cache_list(self) -> list[Usage]:
-        out = sum([gpt.usage_cache_list for gpt in self.gpts], [])
+    async def usage_cache_list(self) -> list[Usage]:
+        out = sum([await gpt.usage_cache_list for gpt in self.gpts], [])
         return out
 
     async def chat_completion(self, **kwargs) -> ChatCompletionAddition:
         gpt = await self.allocation_function(
             self.gpts,
             weights=self.allocation_function_weights,
             **self.allocation_function_kwargs,
@@ -229,41 +247,44 @@
         openai_api_key: str,
         azure_api_key: str,
         azure_api_base: str,
         azure_model_map: dict[str, str],
         cache: Optional[Any] = None,
         semantic_cache: Optional[Any] = None,
         propagate_standard_cache_to_semantic_cache: bool = False,
-        azure_openai_version: str = "2023-05-15",
+        propagate_semantic_cache_to_standard_cache: bool = False,
+        azure_openai_version: str = "2024-02-01",
         azure_openai_type: str = "azure",
         max_parallel_calls_openai: int = 5,
         max_parallel_calls_azure: int = 5,
         ratio_openai_to_azure: float = 0.25,
         stop_after_attempts: Optional[int] = 10,
         stop_on_exception: bool = False,
     ):
         self.openai = ChatGPT(
             api_key=openai_api_key,
             cache=cache,
             semantic_cache=semantic_cache,
             propagate_standard_cache_to_semantic_cache=propagate_standard_cache_to_semantic_cache,
+            propagate_semantic_cache_to_standard_cache=propagate_semantic_cache_to_standard_cache,
             max_parallel_calls=max_parallel_calls_openai,
             stop_after_attempts=stop_after_attempts,
             stop_on_exception=stop_on_exception,
         )
 
         self.azure = AzureGPT(
             api_key=azure_api_key,
             azure_api_base=azure_api_base,
             azure_model_map=azure_model_map,
             azure_openai_version=azure_openai_version,
             azure_openai_type=azure_openai_type,
             cache=cache,
             semantic_cache=semantic_cache,
             propagate_standard_cache_to_semantic_cache=propagate_standard_cache_to_semantic_cache,
+            propagate_semantic_cache_to_standard_cache=propagate_semantic_cache_to_standard_cache,
             max_parallel_calls=max_parallel_calls_azure,
             stop_after_attempts=stop_after_attempts,
             stop_on_exception=stop_on_exception,
         )
 
         super().__init__(
             gpts=[self.openai, self.azure],
```

### Comparing `lbgpt-0.1.3/lbgpt/semantic_cache/base.py` & `lbgpt-0.3.0/src/lbgpt/semantic_cache/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import abc
-import copy
 import logging
 from typing import Any, Iterable, Optional
 
 from langchain_core.embeddings import Embeddings
 from openai.types.chat import ChatCompletion, CompletionCreateParams
 from openai.types.completion_create_params import (
     CompletionCreateParamsNonStreaming,
@@ -45,14 +44,19 @@
 
         return txt
 
     def embed_messages(self, messages: list[dict[str, Any]]) -> list[float]:
         txt = self.messages_to_text(messages)
         return self.embeddings_model.embed_documents([txt])[0]
 
+    async def aembed_messages(self, messages: list[dict[str, Any]]) -> list[float]:
+        txt = self.messages_to_text(messages)
+        return await self.embeddings_model.aembed_query(txt)
+
+
     def non_message_dict(
         self,
         chat_completion_create: CompletionCreateParams | dict[str, Any],
         allowed_types: Optional[Iterable] = None,
         convert_not_allowed_to_empty: bool = True,
     ) -> dict[str, Any]:
         res = non_message_parameters_from_create(
```

### Comparing `lbgpt-0.1.3/lbgpt/semantic_cache/faiss_cache.py` & `lbgpt-0.3.0/src/lbgpt/semantic_cache/faiss_cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,16 +54,19 @@
             filter=self.non_message_dict(query),
             k=1,
         )
 
         res = [r for r in res if r[1] <= 1 - self.cosine_similarity_threshold]
 
         if len(res) > 0:
+            r = res[0][0].metadata["result"]
+            r = {k: v for k, v in r.items() if k not in ['is_exact', 'is_semantic_cached', 'is_cached']}
+
             return ChatCompletionAddition(
-                **res[0][0].metadata["result"], is_exact=res[0][1] <= 0.00001
+                **r, is_exact=res[0][1] <= 0.00001, is_semantic_cached=True
             )
         else:
             return
 
     async def add_cache(
         self, query: CompletionCreateParams | dict[str, Any], response: ChatCompletion
     ) -> None:
```

### Comparing `lbgpt-0.1.3/lbgpt/semantic_cache/qdrant_cache.py` & `lbgpt-0.3.0/src/lbgpt/semantic_cache/qdrant_cache.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,153 +1,228 @@
 import uuid
 from types import NoneType
 from typing import Any, Optional
-
-import tenacity
 from langchain_core.embeddings import Embeddings
 from openai.types.chat import ChatCompletion, CompletionCreateParams
+from pydantic import BaseModel
 from qdrant_client import AsyncQdrantClient, QdrantClient
 from qdrant_client.http.exceptions import ResponseHandlingException
 from qdrant_client.http.models import FieldCondition, Filter, MatchValue, PointStruct
 from qdrant_client.models import Distance, VectorParams
-from tenacity import retry_if_exception_type, wait_random_exponential
 
+from lbgpt.cache import make_hash_chatgpt_request
 from lbgpt.semantic_cache.base import _SemanticCacheBase, get_completion_create_params
 from lbgpt.types import ChatCompletionAddition
 
 
+from logging import getLogger
+
+
+logger = getLogger(__name__)
+
+
+class QdrantClientConfig(BaseModel):
+    host: Optional[str] = None
+    port: Optional[int] = 6333
+    url: Optional[str] = None
+    api_key: Optional[str] = None
+
+    class Config:
+        extra = "allow"
+
+    def get_async_client(self) -> AsyncQdrantClient:
+        if self.api_key == "":
+            api_key = None
+        else:
+            api_key = self.api_key
+
+        return AsyncQdrantClient(
+            host=self.host,
+            port=self.port,
+            url=self.url,
+            api_key=api_key,
+            **self.extra_fields,
+        )
+
+    def get_sync_client(self) -> QdrantClient:
+        if self.api_key == "":
+            api_key = None
+        else:
+            api_key = self.api_key
+        return QdrantClient(
+            host=self.host,
+            port=self.port,
+            url=self.url,
+            api_key=api_key,
+            **self.extra_fields,
+        )
+
+    @property
+    def extra_fields(self) -> dict[str, Any]:
+        field_names = set(self.__dict__) - set(self.__fields__)
+        return {fn: getattr(self, fn) for fn in field_names}
+
+
 class QdrantSemanticCache(_SemanticCacheBase):
     ALLOWED_TYPES_FOR_PAYLOAD = (int, str, bool)
 
     def __init__(
         self,
         embedding_model: Embeddings,
         collection_name: str,
         host: Optional[str] = None,
         port: Optional[int] = 6333,
         url: Optional[str] = None,
         api_key: Optional[str] = None,
         qdrant_properties: Optional[dict[str, Any]] = None,
         cosine_similarity_threshold: float = 0.99,
+        max_concurrent_requests=10,
     ):
         super().__init__(
             embedding_model=embedding_model,
             cosine_similarity_threshold=cosine_similarity_threshold,
         )
 
         # setting up the Qdrant client properly
         # we are setting up a synchroneous and an asynchroneous client
         # the synchroneous client is used for special operations like counting, listing, where we actually
         # care about precision
 
-        self.qdrant_client = AsyncQdrantClient(
-            host=host, port=port, url=url, api_key=api_key, **(qdrant_properties or {})
-        )
-        self._sync_qdrant_client = QdrantClient(
+        self.collection_name = collection_name
+        self._QdrantClientConfig = QdrantClientConfig(
             host=host, port=port, url=url, api_key=api_key, **(qdrant_properties or {})
         )
 
-        self.collection_name = collection_name
-
-        collection_result = self._sync_qdrant_client.get_collections()
+        client = self._QdrantClientConfig.get_sync_client()
+        collection_result = client.get_collections()
 
         existing_collection_names = [k.name for k in collection_result.collections]
         if collection_name not in existing_collection_names:
             # it is surprisingly difficult to figure out how long an embedding model is. Thus, we are actually
             # embedding a string here and then checking the length of the embedding
             _test_embedding = embedding_model.embed_query("test")
 
-            self._sync_qdrant_client.create_collection(
+            client.create_collection(
                 collection_name=self.collection_name,
                 vectors_config=VectorParams(
                     size=len(_test_embedding), distance=Distance.COSINE
                 ),
             )
+        client.close()
 
     def _create_filter_value(
         self, value: int | str | bool | NoneType
     ) -> int | str | bool:
         if isinstance(value, self.ALLOWED_TYPES_FOR_PAYLOAD):
             return value
         elif value is None:
             return ""
         else:
             raise NotImplementedError(f"cannot process type {type(value)}")
 
-    @tenacity.retry(
-        retry=(retry_if_exception_type(ResponseHandlingException)),
-        wait=wait_random_exponential(min=5, max=60),
-    )
     async def query_cache(
         self, query: CompletionCreateParams | dict[str, Any]
     ) -> Optional[ChatCompletionAddition]:
+        try:
+            return await self._query_cache(query=query)
+        except ResponseHandlingException as e:
+            logger.debug(f"Error querying cache, proceed anyways: {e}")
+            # we don't really care about errors here
+            return
+
+    async def add_cache(
+        self, query: CompletionCreateParams | dict[str, Any], response: ChatCompletion
+    ) -> None:
+        try:
+            return await self._add_cache(query=query, response=response)
+        except ResponseHandlingException as e:
+            logger.debug(f"Error querying cache, proceed anyways: {e}")
+            # we don't really care about errors here
+            return
+
+    def hashed_query_payload(
+        self, query: CompletionCreateParams | dict[str, Any]
+    ) -> str:
+        return make_hash_chatgpt_request(query, include_messages=False)
+
+    async def _query_cache(
+        self, query: CompletionCreateParams | dict[str, Any]
+    ) -> Optional[ChatCompletionAddition]:
         query = get_completion_create_params(**query)
+        filter_params_hash = make_hash_chatgpt_request(query, include_messages=False)
 
-        filter_params = self.non_message_dict(query)
         query_filter = Filter(
             must=[
                 FieldCondition(
-                    key=k, match=MatchValue(value=self._create_filter_value(v))
+                    key='hashed_model', match=MatchValue(value=filter_params_hash)
                 )
-                for k, v in filter_params.items()
-                if isinstance(v, self.ALLOWED_TYPES_FOR_PAYLOAD) or v is None
             ]
         )
 
-        res = await self.qdrant_client.search(
+        embedding = await self.aembed_messages(query["messages"])
+
+        res = await self._QdrantClientConfig.get_async_client().search(
             collection_name=self.collection_name,
-            query_vector=self.embed_messages(query["messages"]),
+            query_vector=embedding,
             query_filter=query_filter,
             with_payload=True,
             with_vectors=False,
             limit=1,
             score_threshold=self.cosine_similarity_threshold,
+            timeout=10,
         )
 
         res = [r for r in res if r.score >= self.cosine_similarity_threshold]
 
+
         if len(res) > 0:
+            r = res[0].payload["result"]
+            r = {k: v for k, v in r.items() if k not in ['is_exact', 'is_semantic_cached', 'is_cached']}
+
             return ChatCompletionAddition(
-                **res[0].payload["result"],
+                **r,
                 is_exact=res[0].score >= 1 - 0.00001,
+                is_semantic_cached=True,
             )
         else:
             return
 
-
-    @tenacity.retry(
-        retry=(retry_if_exception_type(ResponseHandlingException)),
-        wait=wait_random_exponential(min=5, max=60),
-    )
-    async def add_cache(
+    async def _add_cache(
         self, query: CompletionCreateParams | dict[str, Any], response: ChatCompletion
     ) -> None:
         query = get_completion_create_params(**query)
+        filter_params_hash = make_hash_chatgpt_request(query, include_messages=False)
+
+        embedding = await self.aembed_messages(query["messages"])
 
-        await self.qdrant_client.upsert(
+        await self._QdrantClientConfig.get_async_client().upsert(
             collection_name=self.collection_name,
             wait=False,
             points=[
                 PointStruct(
                     id=str(uuid.uuid4()),
-                    vector=self.embed_messages(query["messages"]),
+                    vector=embedding,
                     payload={
                         "result": response.model_dump(
                             exclude={
                                 "is_exact",
                             }
                         ),
+                        'hashed_model': filter_params_hash,
                         **self.non_message_dict(
                             query,
                             allowed_types=self.ALLOWED_TYPES_FOR_PAYLOAD,
                             convert_not_allowed_to_empty=True,
                         ),
+
                     },
                 )
             ],
         )
 
     @property
     def count(self) -> int:
-        return self._sync_qdrant_client.count(
-            collection_name=self.collection_name
-        ).count
+        return (
+            self._QdrantClientConfig.get_sync_client()
+            .count(collection_name=self.collection_name)
+            .count
+        )
```

### Comparing `lbgpt-0.1.3/tests/conftest.py` & `lbgpt-0.3.0/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, Dict
 
 import pytest
 import vcr  # type: ignore[import]
 import vcr.request  # type: ignore[import]
 import vcr.util  # type: ignore[import]
 
-vcr_match_on = ("method", "scheme", "host", "port", "path", "query")
+vcr_match_on = ("method", "scheme", "host", "port", "path", "query", "body")
 
 
 @pytest.fixture()
 def vcr_cassette_dir(request):  # type: ignore[no-untyped-def]
     return os.path.join(
         os.path.dirname(request.module.__file__), "cassette", request.module.__name__
     )
```

### Comparing `lbgpt-0.1.3/tests/test_lb.py` & `lbgpt-0.3.0/tests/test_lb.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 import asyncio
 import os
 import random
 
 import pytest
 from pytest_mock import MockerFixture
 
-from lbgpt import AzureGPT, ChatGPT, LoadBalancedGPT
-from lbgpt.lbgpt import MultiLoadBalancedGPT
+from lbgpt import AzureGPT, ChatGPT, LoadBalancedGPT, MultiLoadBalancedGPT
 from lbgpt.types import ChatCompletionAddition
 
 
 @pytest.mark.vcr
-def test_lb_async_random(mocker: MockerFixture):
+async def test_lb_async_random(mocker: MockerFixture):
     random.seed(42)
 
     messages = [
         {"role": "user", "content": "please respond with pong"},
     ]
     single_request_content = dict(
         messages=messages,
@@ -37,30 +36,28 @@
             "gpt-3.5-turbo-0613": os.environ["OPENAI_AZURE_DEPLOYMENT_ID"]
         },
     )
 
     azure = mocker.spy(lb.azure, "chat_completion")
     openai = mocker.spy(lb.openai, "chat_completion")
 
-    res = asyncio.run(
-        lb.chat_completion_list([single_request_content] * 5, show_progress=False)
-    )
+    res = await lb.chat_completion_list([single_request_content] * 5, show_progress=False)
 
     assert len(res) == 5
     for k in res:
         assert "pong" in k.choices[0].message.content.lower()
         assert isinstance(k, ChatCompletionAddition)
 
     assert azure.call_count >= 1
     assert openai.call_count >= 1
     assert azure.call_count + openai.call_count == 5
 
 
 @pytest.mark.vcr
-def test_lbgpt_max_headroom():
+async def test_lbgpt_max_headroom():
     random.seed(42)
 
     messages = [
         {"role": "user", "content": "please respond with pong"},
     ]
     single_request_content = dict(
         messages=messages,
@@ -90,30 +87,28 @@
     )
 
     lb = MultiLoadBalancedGPT(
         gpts=[model_openai, model_azure],
         allocation_function="max_headroom",
     )
 
-    res = asyncio.run(
-        lb.chat_completion_list([single_request_content] * 5, show_progress=False)
-    )
-    assert len(lb.usage_cache_list) == 5
+    res = await lb.chat_completion_list([single_request_content] * 5, show_progress=False)
 
-    assert len(lb.gpts[0].usage_cache_list) == 5
-    assert len(lb.gpts[1].usage_cache_list) == 0
+    assert len(await lb.usage_cache_list) == 5
+    assert len(await lb.gpts[0].usage_cache_list) == 5
+    assert len(await lb.gpts[1].usage_cache_list) == 0
 
     assert len(res) == 5
     for k in res:
         assert "pong" in k.choices[0].message.content.lower()
         assert isinstance(k, ChatCompletionAddition)
 
 
 @pytest.mark.vcr
-def test_chatgpt_async(mocker: MockerFixture):
+async def test_chatgpt_async(mocker: MockerFixture):
     messages = [
         {"role": "user", "content": "please respond with pong"},
     ]
     single_request_content = dict(
         messages=messages,
         model="gpt-3.5-turbo-0613",
         temperature=0,
@@ -128,30 +123,28 @@
         api_key=os.environ["OPEN_AI_API_KEY"],
         stop_after_attempts=1,
         stop_on_exception=True,
     )
 
     openai = mocker.spy(lb, "chat_completion")
 
-    res = asyncio.run(
-        lb.chat_completion_list([single_request_content] * 5, show_progress=False)
-    )
+    res = await lb.chat_completion_list([single_request_content] * 5, show_progress=False)
 
-    assert len(lb.usage_cache_list) == 5
+    assert len(await lb.usage_cache_list) == 5
 
     assert len(res) == 5
     for k in res:
         assert "pong" in k.choices[0].message.content.lower()
         assert isinstance(k, ChatCompletionAddition)
 
     assert openai.call_count >= 5
 
 
 @pytest.mark.vcr
-def test_azure_async(mocker: MockerFixture):
+async def test_azure_async(mocker: MockerFixture):
     messages = [
         {"role": "user", "content": "please respond with pong"},
     ]
     single_request_content = dict(
         messages=messages,
         model="gpt-3.5-turbo-0613",
         temperature=0,
@@ -170,19 +163,52 @@
         azure_model_map={
             "gpt-3.5-turbo-0613": os.environ["OPENAI_AZURE_DEPLOYMENT_ID"]
         },
     )
 
     azure = mocker.spy(lb, "chat_completion")
 
-    res = asyncio.run(
-        lb.chat_completion_list([single_request_content] * 5, show_progress=False)
-    )
+    res = await lb.chat_completion_list([single_request_content] * 5, show_progress=False)
 
-    assert len(lb.usage_cache_list) == 5
+    assert len(await lb.usage_cache_list) == 5
 
     assert len(res) == 5
     for k in res:
         assert "pong" in k.choices[0].message.content.lower()
         assert isinstance(k, ChatCompletionAddition)
 
     assert azure.call_count >= 5
+
+
+@pytest.mark.vcr
+def test_chatgpt_async_multiple_starts(mocker: MockerFixture):
+    messages = [
+        {"role": "user", "content": "please respond with pong"},
+    ]
+    single_request_content = dict(
+        messages=messages,
+        model="gpt-3.5-turbo-0613",
+        temperature=0,
+        max_tokens=50,
+        top_p=1,
+        frequency_penalty=0,
+        presence_penalty=0,
+        request_timeout=10,
+    )
+
+    lb = ChatGPT(
+        api_key=os.environ["OPEN_AI_API_KEY"],
+        stop_after_attempts=1,
+        stop_on_exception=True,
+    )
+
+    openai = mocker.spy(lb, "chat_completion")
+
+    res = asyncio.run(
+        lb.chat_completion_list([single_request_content] * 2, show_progress=False)
+    )
+
+    res2 = asyncio.run(
+        lb.chat_completion_list([single_request_content] * 2, show_progress=False)
+    )
+
+    assert len(res) + len(res2) == 4
```

### Comparing `lbgpt-0.1.3/tests/cache/test_immutability.py` & `lbgpt-0.3.0/tests/cache/test_immutability.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         max_tokens=50,
         top_p=1,
         frequency_penalty=0,
         presence_penalty=0,
         request_timeout=10,
     )
 
-    res_base = "PSez9z+xC/CxkHTYJ/4mMKic9Fdg6oRyRVeXu8AAtRI="
+    res_base = "lbgpt_PSez9z+xC/CxkHTYJ/4mMKic9Fdg6oRyRVeXu8AAtRI="
 
     for _ in range(20):
         res_next_pass = make_hash_chatgpt_request(single_request_content)
         assert res_base == res_next_pass
 
 
 def test_cache_immutability_with_slack():
```

### Comparing `lbgpt-0.1.3/tests/cache/test_lb_cache.py` & `lbgpt-0.3.0/tests/cache/test_lb_cache.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,42 @@
 # -*- coding: utf-8 -*-
 import asyncio
 import os
 import tempfile
 
 import diskcache
 import pytest
+import redis
 from pytest_mock import MockerFixture
 
 from lbgpt import ChatGPT
 from lbgpt.types import ChatCompletionAddition
 
-CACHES = [diskcache.Cache(tempfile.TemporaryDirectory().name)]
+redis_cache = redis.StrictRedis(
+    host="localhost",
+    port=6378,  # this is the port configured in the compose.yml file
+)
+
+redis_cache.flushdb()
+
+
+CACHES = [diskcache.Cache(tempfile.TemporaryDirectory().name), redis_cache]
+
+
+def _num_keys_in_cache(cache) -> int:
+    if isinstance(cache, redis.StrictRedis):
+        return cache.dbsize()
+    elif hasattr(cache, "count"):
+        return cache.count
+    else:
+        raise NotImplementedError
 
 
 @pytest.mark.parametrize("cache", CACHES)
-@pytest.mark.vcr
+@pytest.mark.vcr(ignore_localhost=True)
 def test_chatgpt_cache(mocker: MockerFixture, cache):
     messages = [
         {"role": "user", "content": "please respond with pong"},
     ]
     single_request_content = dict(
         messages=messages,
         model="gpt-3.5-turbo-0613",
@@ -33,34 +51,34 @@
     lb = ChatGPT(
         api_key=os.environ["OPEN_AI_API_KEY"],
         stop_after_attempts=1,
         stop_on_exception=True,
         cache=cache,
     )
 
-    # Setting the cache
-    cache_interaction = mocker.spy(lb, "_request_from_cache")
+    # Setting the mocks
+    cache_interaction = mocker.spy(lb, "_get_from_cache")
+    request_interaction = mocker.spy(lb, "chat_completion")
 
     # run with an empty cache
     asyncio.run(lb.chat_completion_list([single_request_content], show_progress=False))
 
     # asserting that the cache was not called
     assert cache_interaction.call_count == 1
     assert cache_interaction.spy_return is None
 
     # some cache stats and hash
-    cache_stats = {"hash": hash(cache)}
-
-    if hasattr(cache, "count"):
-        cache_stats["count"] = cache.count
+    cache_stats = {"hash": hash(cache), "count": _num_keys_in_cache(cache)}
 
     # Getting from cache
     asyncio.run(lb.chat_completion_list([single_request_content], show_progress=False))
 
     # asserting that the cache was called and returned the values
     assert cache_interaction.call_count == 2
     assert isinstance(cache_interaction.spy_return, ChatCompletionAddition)
 
     # asserting that no items were added to the cache
-    if hasattr(cache, "count"):
-        assert cache.count == cache_stats["count"]
     assert hash(cache) == cache_stats["hash"]
+    assert _num_keys_in_cache(cache) == cache_stats["count"]
+
+    # assert that chatgpt was requested only once
+    assert request_interaction.call_count == 1
```

### Comparing `lbgpt-0.1.3/tests/cache/cassette/test_lb_cache/test_chatgpt_cache[cache0].yaml` & `lbgpt-0.3.0/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_failed[-lambda-0].yaml`

 * *Files 8% similar despite different names*

```diff
@@ -31,84 +31,84 @@
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
       - 3.11.4
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
-    content: "{\n  \"id\": \"chatcmpl-8YBX5JCBw84tLSAY1Q9DXtRJ48cDC\",\n  \"object\":
-      \"chat.completion\",\n  \"created\": 1703158175,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+    content: "{\n  \"id\": \"chatcmpl-8Xw23g2xw8Dtnttk2qm0IP6qIRTOb\",\n  \"object\":
+      \"chat.completion\",\n  \"created\": 1703098591,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
       \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
       \"assistant\",\n        \"content\": \"Pong\"\n      },\n      \"logprobs\":
       null,\n      \"finish_reason\": \"stop\"\n    }\n  ],\n  \"usage\": {\n    \"prompt_tokens\":
       11,\n    \"completion_tokens\": 2,\n    \"total_tokens\": 13\n  },\n  \"system_fingerprint\":
       null\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 838fc9c27be8b476-DXB
+      - 838a1b134f95125a-DXB
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Thu, 21 Dec 2023 11:29:36 GMT
+      - Wed, 20 Dec 2023 18:56:31 GMT
       Server:
       - cloudflare
       Set-Cookie:
-      - __cf_bm=VQ544wdJlRlqIDFTgD6d2GJEvihb5CIq4SnerZMSEFU-1703158176-1-AaFWqaKsUpRvVlCWvnCqE+et2tif+ZBCKLKqvzbigIvYE6dqBhVAU+Ozc4/Q+i/wHKUumysM9yclzhqsNjHT8h0=;
-        path=/; expires=Thu, 21-Dec-23 11:59:36 GMT; domain=.api.openai.com; HttpOnly;
+      - __cf_bm=t5.oZigY9JptRi_I0r1lJ7IV3DZ46O.B6Q7eHs2l5hs-1703098591-1-ATntkxWqNh5ZyOKCkf8mz+KXSsykk0lwtbikn4fwqoThMVYsXGKkj6NVNegsBHfdPkt6S9Ymf6TNrx7XY+6kJQw=;
+        path=/; expires=Wed, 20-Dec-23 19:26:31 GMT; domain=.api.openai.com; HttpOnly;
         Secure; SameSite=None
-      - _cfuvid=wPkJSOfVJ45uMPSZ5oDRlhlRDSx5r3Bh3wtAQshuMA4-1703158176134-0-604800000;
+      - _cfuvid=kv3TrdMlUyWG3JQWQ6FdskydxESvW9wGMt8mp.lKtCY-1703098591884-0-604800000;
         path=/; domain=.api.openai.com; HttpOnly; Secure; SameSite=None
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
       - gpt-3.5-turbo-0613
       openai-organization:
       - marvin-labs
       openai-processing-ms:
-      - '471'
+      - '107'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '10000'
       x-ratelimit-limit-tokens:
       - '1000000'
       x-ratelimit-limit-tokens_usage_based:
       - '1000000'
       x-ratelimit-remaining-requests:
       - '9999'
       x-ratelimit-remaining-tokens:
-      - '999942'
+      - '999943'
       x-ratelimit-remaining-tokens_usage_based:
-      - '999942'
+      - '999943'
       x-ratelimit-reset-requests:
       - 6ms
       x-ratelimit-reset-tokens:
       - 3ms
       x-ratelimit-reset-tokens_usage_based:
       - 3ms
       x-request-id:
-      - 17abdf5f9332392a303c8b678b9d0e7e
+      - f2716e64184770e389e3076f4bc70ced
     http_version: HTTP/1.1
     status_code: 200
 - request:
-    body: '{"messages": [{"role": "user", "content": "please respond with pong"}],
+    body: '{"messages": [{"role": "user", "content": "please respond with test"}],
       "model": "gpt-3.5-turbo-0613", "frequency_penalty": 0, "max_tokens": 50, "presence_penalty":
       0, "temperature": 0, "top_p": 1}'
     headers:
       accept:
       - application/json
       accept-encoding:
       - gzip, deflate
@@ -135,56 +135,56 @@
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
       - 3.11.4
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
-    content: "{\n  \"id\": \"chatcmpl-8YBX6uew9uFyMNZc6U0aSAZremNZa\",\n  \"object\":
-      \"chat.completion\",\n  \"created\": 1703158176,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+    content: "{\n  \"id\": \"chatcmpl-8Xw24koIKj4g9T3cNdcWexbEmNgrT\",\n  \"object\":
+      \"chat.completion\",\n  \"created\": 1703098592,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
       \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
-      \"assistant\",\n        \"content\": \"Pong\"\n      },\n      \"logprobs\":
+      \"assistant\",\n        \"content\": \"test\"\n      },\n      \"logprobs\":
       null,\n      \"finish_reason\": \"stop\"\n    }\n  ],\n  \"usage\": {\n    \"prompt_tokens\":
-      11,\n    \"completion_tokens\": 2,\n    \"total_tokens\": 13\n  },\n  \"system_fingerprint\":
+      11,\n    \"completion_tokens\": 1,\n    \"total_tokens\": 12\n  },\n  \"system_fingerprint\":
       null\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 838fc9c92bbc125a-DXB
+      - 838a1b17bb8f125a-DXB
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Thu, 21 Dec 2023 11:29:37 GMT
+      - Wed, 20 Dec 2023 18:56:32 GMT
       Server:
       - cloudflare
       Set-Cookie:
-      - __cf_bm=Bn6gsAxLtXvR0iPeb4T2MX0fWjitZpKaZQhGREVgxXU-1703158177-1-AelrU6gLXp+Z05mV4MSs17KnxLUbMtDW6+j7t95ho8IjGTxMRauHqo3MaiLqlG5zpeuwGHjpnWLhMFvNh4ya5Q0=;
-        path=/; expires=Thu, 21-Dec-23 11:59:37 GMT; domain=.api.openai.com; HttpOnly;
+      - __cf_bm=z0SMSD.k8AopcQvSiwo7PvqMkhicSFDtQS9t_p3egKY-1703098592-1-AYDbMO4Z28gDCAm2CLEpNBLChj3rdtc4wIGSkFvVI0Y0PnSXacAHCJgLYMOhAgASzHpEqP1GxPhUGmixgJqZBFQ=;
+        path=/; expires=Wed, 20-Dec-23 19:26:32 GMT; domain=.api.openai.com; HttpOnly;
         Secure; SameSite=None
-      - _cfuvid=hIGhhR8c3gmgXJPS.rQYx.P.KsTXCU5Nz6dUT4tFhBs-1703158177220-0-604800000;
+      - _cfuvid=6zCLshzMSQo.xrUCodzzt3b9nCUtto13FxWv63DhToM-1703098592538-0-604800000;
         path=/; domain=.api.openai.com; HttpOnly; Secure; SameSite=None
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
       - gpt-3.5-turbo-0613
       openai-organization:
       - marvin-labs
       openai-processing-ms:
-      - '511'
+      - '308'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '10000'
       x-ratelimit-limit-tokens:
@@ -200,11 +200,11 @@
       x-ratelimit-reset-requests:
       - 6ms
       x-ratelimit-reset-tokens:
       - 3ms
       x-ratelimit-reset-tokens_usage_based:
       - 3ms
       x-request-id:
-      - e73e9cf290674efc33470d46095bab57
+      - 11426ffcf7b1c3b89d73eec40961fa16
     http_version: HTTP/1.1
     status_code: 200
 version: 1
```

### Comparing `lbgpt-0.1.3/tests/cassette/test_lb/test_azure_async.yaml` & `lbgpt-0.3.0/tests/cassette/test_lb/test_azure_async.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
       x-stainless-package-version:
       - 1.5.0
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
       - 3.11.4
     method: POST
-    uri: https://openai-mlexperiment.openai.azure.com//openai/deployments/gpt-35-turbo-0613/chat/completions?api-version=2023-05-15
+    uri: https://openai-mlexperiment.openai.azure.com//openai/deployments/gpt-35-turbo-0613/chat/completions?api-version=2024-02-01
   response:
     content: '{"id":"chatcmpl-8XtIeImxtDd1rGnTCXfjYb40QqKxP","object":"chat.completion","created":1703088088,"model":"gpt-35-turbo","choices":[{"finish_reason":"stop","index":0,"message":{"role":"assistant","content":"Pong"}}],"usage":{"prompt_tokens":11,"completion_tokens":2,"total_tokens":13}}
 
       '
     headers:
       Cache-Control:
       - no-cache, must-revalidate
@@ -105,15 +105,15 @@
       x-stainless-package-version:
       - 1.5.0
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
       - 3.11.4
     method: POST
-    uri: https://openai-mlexperiment.openai.azure.com//openai/deployments/gpt-35-turbo-0613/chat/completions?api-version=2023-05-15
+    uri: https://openai-mlexperiment.openai.azure.com//openai/deployments/gpt-35-turbo-0613/chat/completions?api-version=2024-02-01
   response:
     content: '{"id":"chatcmpl-8XtIem0F3mrLpcY8bLbKnM8IbRCMT","object":"chat.completion","created":1703088088,"model":"gpt-35-turbo","choices":[{"finish_reason":"stop","index":0,"message":{"role":"assistant","content":"Pong"}}],"usage":{"prompt_tokens":11,"completion_tokens":2,"total_tokens":13}}
 
       '
     headers:
       Cache-Control:
       - no-cache, must-revalidate
@@ -179,15 +179,15 @@
       x-stainless-package-version:
       - 1.5.0
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
       - 3.11.4
     method: POST
-    uri: https://openai-mlexperiment.openai.azure.com//openai/deployments/gpt-35-turbo-0613/chat/completions?api-version=2023-05-15
+    uri: https://openai-mlexperiment.openai.azure.com//openai/deployments/gpt-35-turbo-0613/chat/completions?api-version=2024-02-01
   response:
     content: '{"id":"chatcmpl-8XtIeCOf37wHKOf93mVkXtSDosgzk","object":"chat.completion","created":1703088088,"model":"gpt-35-turbo","choices":[{"finish_reason":"stop","index":0,"message":{"role":"assistant","content":"Pong"}}],"usage":{"prompt_tokens":11,"completion_tokens":2,"total_tokens":13}}
 
       '
     headers:
       Cache-Control:
       - no-cache, must-revalidate
@@ -253,15 +253,15 @@
       x-stainless-package-version:
       - 1.5.0
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
       - 3.11.4
     method: POST
-    uri: https://openai-mlexperiment.openai.azure.com//openai/deployments/gpt-35-turbo-0613/chat/completions?api-version=2023-05-15
+    uri: https://openai-mlexperiment.openai.azure.com//openai/deployments/gpt-35-turbo-0613/chat/completions?api-version=2024-02-01
   response:
     content: '{"id":"chatcmpl-8XtIeytwIryORERypaFtwiPVnNPbU","object":"chat.completion","created":1703088088,"model":"gpt-35-turbo","choices":[{"finish_reason":"stop","index":0,"message":{"role":"assistant","content":"Pong"}}],"usage":{"prompt_tokens":11,"completion_tokens":2,"total_tokens":13}}
 
       '
     headers:
       Cache-Control:
       - no-cache, must-revalidate
@@ -327,15 +327,15 @@
       x-stainless-package-version:
       - 1.5.0
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
       - 3.11.4
     method: POST
-    uri: https://openai-mlexperiment.openai.azure.com//openai/deployments/gpt-35-turbo-0613/chat/completions?api-version=2023-05-15
+    uri: https://openai-mlexperiment.openai.azure.com//openai/deployments/gpt-35-turbo-0613/chat/completions?api-version=2024-02-01
   response:
     content: '{"id":"chatcmpl-8XtIeMkb0KCWO7kA7x12wmQMIA5Dk","object":"chat.completion","created":1703088088,"model":"gpt-35-turbo","choices":[{"finish_reason":"stop","index":0,"message":{"role":"assistant","content":"Pong"}}],"usage":{"prompt_tokens":11,"completion_tokens":2,"total_tokens":13}}
 
       '
     headers:
       Cache-Control:
       - no-cache, must-revalidate
```

### Comparing `lbgpt-0.1.3/tests/cassette/test_lb/test_chatgpt_async.yaml` & `lbgpt-0.3.0/tests/cassette/test_lb/test_chatgpt_async.yaml`

 * *Files identical despite different names*

### Comparing `lbgpt-0.1.3/tests/cassette/test_lb/test_lb_async_random.yaml` & `lbgpt-0.3.0/tests/cassette/test_lb/test_lb_async_random.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
       x-stainless-package-version:
       - 1.5.0
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
       - 3.11.4
     method: POST
-    uri: https://openai-mlexperiment.openai.azure.com//openai/deployments/gpt-35-turbo-0613/chat/completions?api-version=2023-05-15
+    uri: https://openai-mlexperiment.openai.azure.com//openai/deployments/gpt-35-turbo-0613/chat/completions?api-version=2024-02-01
   response:
     content: '{"id":"chatcmpl-8XtJqfrq3KttTe1cc01Awu8Re1cQw","object":"chat.completion","created":1703088162,"model":"gpt-35-turbo","choices":[{"finish_reason":"stop","index":0,"message":{"role":"assistant","content":"Pong"}}],"usage":{"prompt_tokens":11,"completion_tokens":2,"total_tokens":13}}
 
       '
     headers:
       Cache-Control:
       - no-cache, must-revalidate
@@ -209,15 +209,15 @@
       x-stainless-package-version:
       - 1.5.0
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
       - 3.11.4
     method: POST
-    uri: https://openai-mlexperiment.openai.azure.com//openai/deployments/gpt-35-turbo-0613/chat/completions?api-version=2023-05-15
+    uri: https://openai-mlexperiment.openai.azure.com//openai/deployments/gpt-35-turbo-0613/chat/completions?api-version=2024-02-01
   response:
     content: '{"id":"chatcmpl-8XtJqI1r460hjzhNkZWyanX6gVwRM","object":"chat.completion","created":1703088162,"model":"gpt-35-turbo","choices":[{"finish_reason":"stop","index":0,"message":{"role":"assistant","content":"Pong"}}],"usage":{"prompt_tokens":11,"completion_tokens":2,"total_tokens":13}}
 
       '
     headers:
       Cache-Control:
       - no-cache, must-revalidate
@@ -283,15 +283,15 @@
       x-stainless-package-version:
       - 1.5.0
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
       - 3.11.4
     method: POST
-    uri: https://openai-mlexperiment.openai.azure.com//openai/deployments/gpt-35-turbo-0613/chat/completions?api-version=2023-05-15
+    uri: https://openai-mlexperiment.openai.azure.com//openai/deployments/gpt-35-turbo-0613/chat/completions?api-version=2024-02-01
   response:
     content: '{"id":"chatcmpl-8XtJq11XAyMn9hlKo8owbKrc4Thqt","object":"chat.completion","created":1703088162,"model":"gpt-35-turbo","choices":[{"finish_reason":"stop","index":0,"message":{"role":"assistant","content":"Pong"}}],"usage":{"prompt_tokens":11,"completion_tokens":2,"total_tokens":13}}
 
       '
     headers:
       Cache-Control:
       - no-cache, must-revalidate
```

### Comparing `lbgpt-0.1.3/tests/cassette/test_lb/test_lbgpt_max_headroom.yaml` & `lbgpt-0.3.0/tests/cassette/test_lb/test_lbgpt_max_headroom.yaml`

 * *Files identical despite different names*

### Comparing `lbgpt-0.1.3/tests/semantic_cache/test_lb_semantic_cache.py` & `lbgpt-0.3.0/tests/semantic_cache/test_lb_semantic_cache.py`

 * *Files identical despite different names*

### Comparing `lbgpt-0.1.3/tests/semantic_cache/test_qdrant.py` & `lbgpt-0.3.0/tests/semantic_cache/test_qdrant.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         embedding_model=TEST_EMBEDDING_MODEL,
         cosine_similarity_threshold=0.95,
         host="localhost",
         port=6333,
         collection_name="".join(rng.choice(string.ascii_letters) for _ in range(20)),
     )
 
-    cache._sync_qdrant_client.upsert(
+    cache._QdrantClientConfig.get_sync_client().upsert(
         collection_name=cache.collection_name,
         wait=False,
         points=[
             PointStruct(
                 id=str(uuid.uuid4()),
                 vector=cache.embed_messages([message]),
                 payload={"message": message},
@@ -90,15 +90,15 @@
 
     return cache
 
 
 @pytest.mark.asyncio
 async def test_exact(qdrant_cache, messages):
     message = messages[0]
-    res = await qdrant_cache.qdrant_client.search(
+    res = await qdrant_cache._QdrantClientConfig.get_async_client().search(
         collection_name=qdrant_cache.collection_name,
         query_vector=qdrant_cache.embed_messages([message]),
         with_payload=True,
         with_vectors=True,
         limit=1,
     )
 
@@ -111,15 +111,15 @@
     message = {
         "role": "user",
         "content": "Apple’s board of directors has declared a cash dividend of $0.53 per share of the Company’s common stock. The dividend is payable on March 12, 2019 to shareholders of record as of the close of business on March 10, 2019.",
     }
 
     embedded = qdrant_cache.embed_messages([message])
 
-    res = await qdrant_cache.qdrant_client.search(
+    res = await qdrant_cache._QdrantClientConfig.get_async_client().search(
         collection_name=qdrant_cache.collection_name,
         query_vector=embedded,
         with_payload=True,
         with_vectors=True,
         limit=1,
     )
 
@@ -138,15 +138,15 @@
     message = {
         "role": "user",
         "content": "The tolerance values are positive, typically very small numbers. The relative difference (rtol * abs(b)) and the absolute difference atol are added together to compare against the absolute difference between a and b.",
     }
 
     embedded = qdrant_cache.embed_messages([message])
 
-    res = await qdrant_cache.qdrant_client.search(
+    res = await qdrant_cache._QdrantClientConfig.get_async_client().search(
         collection_name=qdrant_cache.collection_name,
         query_vector=embedded,
         with_payload=True,
         with_vectors=True,
         limit=1,
     )
```

### Comparing `lbgpt-0.1.3/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_exact[-lambda-0].yaml` & `lbgpt-0.3.0/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_exact[-lambda-0].yaml`

 * *Files identical despite different names*

### Comparing `lbgpt-0.1.3/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_exact[-lambda-1].yaml` & `lbgpt-0.3.0/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_exact[-lambda-1].yaml`

 * *Files identical despite different names*

### Comparing `lbgpt-0.1.3/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_failed[-lambda-0].yaml` & `lbgpt-0.3.0/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_failed[-lambda-1].yaml`

 * *Files 7% similar despite different names*

```diff
@@ -31,56 +31,56 @@
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
       - 3.11.4
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
-    content: "{\n  \"id\": \"chatcmpl-8Xw23g2xw8Dtnttk2qm0IP6qIRTOb\",\n  \"object\":
-      \"chat.completion\",\n  \"created\": 1703098591,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+    content: "{\n  \"id\": \"chatcmpl-8Xw250r1upY6rAcwFVuboHsdoUjgu\",\n  \"object\":
+      \"chat.completion\",\n  \"created\": 1703098593,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
       \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
       \"assistant\",\n        \"content\": \"Pong\"\n      },\n      \"logprobs\":
       null,\n      \"finish_reason\": \"stop\"\n    }\n  ],\n  \"usage\": {\n    \"prompt_tokens\":
       11,\n    \"completion_tokens\": 2,\n    \"total_tokens\": 13\n  },\n  \"system_fingerprint\":
       null\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 838a1b134f95125a-DXB
+      - 838a1b1c6aeeb47f-DXB
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Wed, 20 Dec 2023 18:56:31 GMT
+      - Wed, 20 Dec 2023 18:56:33 GMT
       Server:
       - cloudflare
       Set-Cookie:
-      - __cf_bm=t5.oZigY9JptRi_I0r1lJ7IV3DZ46O.B6Q7eHs2l5hs-1703098591-1-ATntkxWqNh5ZyOKCkf8mz+KXSsykk0lwtbikn4fwqoThMVYsXGKkj6NVNegsBHfdPkt6S9Ymf6TNrx7XY+6kJQw=;
-        path=/; expires=Wed, 20-Dec-23 19:26:31 GMT; domain=.api.openai.com; HttpOnly;
+      - __cf_bm=ZCGKsuolKo.NtPvNpm021WK4jHby4YmVspsvIB77BWg-1703098593-1-AcxMGSZ0vB/tOErslMOTFi5+rXwT51ceGbCwrrBKUllhKWqm8S8rRjq61K+Pycag8NWFJE3RRoO+/j1p2vPRtTg=;
+        path=/; expires=Wed, 20-Dec-23 19:26:33 GMT; domain=.api.openai.com; HttpOnly;
         Secure; SameSite=None
-      - _cfuvid=kv3TrdMlUyWG3JQWQ6FdskydxESvW9wGMt8mp.lKtCY-1703098591884-0-604800000;
+      - _cfuvid=CCy_5LtjuTS6fb.6_7RwXO4JIQcn.v47uaPXqUdmNME-1703098593240-0-604800000;
         path=/; domain=.api.openai.com; HttpOnly; Secure; SameSite=None
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
       - gpt-3.5-turbo-0613
       openai-organization:
       - marvin-labs
       openai-processing-ms:
-      - '107'
+      - '262'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '10000'
       x-ratelimit-limit-tokens:
@@ -96,15 +96,15 @@
       x-ratelimit-reset-requests:
       - 6ms
       x-ratelimit-reset-tokens:
       - 3ms
       x-ratelimit-reset-tokens_usage_based:
       - 3ms
       x-request-id:
-      - f2716e64184770e389e3076f4bc70ced
+      - 95b98365d042efb29205b9d8030cd106
     http_version: HTTP/1.1
     status_code: 200
 - request:
     body: '{"messages": [{"role": "user", "content": "please respond with test"}],
       "model": "gpt-3.5-turbo-0613", "frequency_penalty": 0, "max_tokens": 50, "presence_penalty":
       0, "temperature": 0, "top_p": 1}'
     headers:
@@ -135,56 +135,56 @@
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
       - 3.11.4
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
-    content: "{\n  \"id\": \"chatcmpl-8Xw24koIKj4g9T3cNdcWexbEmNgrT\",\n  \"object\":
-      \"chat.completion\",\n  \"created\": 1703098592,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+    content: "{\n  \"id\": \"chatcmpl-8Xw25sEiAZhte8NJmu5CDLi7Ky1fR\",\n  \"object\":
+      \"chat.completion\",\n  \"created\": 1703098593,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
       \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
       \"assistant\",\n        \"content\": \"test\"\n      },\n      \"logprobs\":
       null,\n      \"finish_reason\": \"stop\"\n    }\n  ],\n  \"usage\": {\n    \"prompt_tokens\":
       11,\n    \"completion_tokens\": 1,\n    \"total_tokens\": 12\n  },\n  \"system_fingerprint\":
       null\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 838a1b17bb8f125a-DXB
+      - 838a1b202e74126e-DXB
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Wed, 20 Dec 2023 18:56:32 GMT
+      - Wed, 20 Dec 2023 18:56:34 GMT
       Server:
       - cloudflare
       Set-Cookie:
-      - __cf_bm=z0SMSD.k8AopcQvSiwo7PvqMkhicSFDtQS9t_p3egKY-1703098592-1-AYDbMO4Z28gDCAm2CLEpNBLChj3rdtc4wIGSkFvVI0Y0PnSXacAHCJgLYMOhAgASzHpEqP1GxPhUGmixgJqZBFQ=;
-        path=/; expires=Wed, 20-Dec-23 19:26:32 GMT; domain=.api.openai.com; HttpOnly;
+      - __cf_bm=lfACNFSXdNXOHtP.NgE3vY.QgOFfTdn2YXOYvYdc18E-1703098594-1-AdkbX0Jf14LBT5SMrGVhGZsdeNJwZbG1UBtqmzBpno2M3/bLtJ0RAyPhKHUF9Ldkx7lXRb7qoeKzNo76WIOtUm8=;
+        path=/; expires=Wed, 20-Dec-23 19:26:34 GMT; domain=.api.openai.com; HttpOnly;
         Secure; SameSite=None
-      - _cfuvid=6zCLshzMSQo.xrUCodzzt3b9nCUtto13FxWv63DhToM-1703098592538-0-604800000;
+      - _cfuvid=hsMtYVk6kOu9vTabx_PHCCEbI7yQ9XQuwVnGXOUq0fw-1703098594289-0-604800000;
         path=/; domain=.api.openai.com; HttpOnly; Secure; SameSite=None
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
       - gpt-3.5-turbo-0613
       openai-organization:
       - marvin-labs
       openai-processing-ms:
-      - '308'
+      - '439'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '10000'
       x-ratelimit-limit-tokens:
@@ -200,11 +200,11 @@
       x-ratelimit-reset-requests:
       - 6ms
       x-ratelimit-reset-tokens:
       - 3ms
       x-ratelimit-reset-tokens_usage_based:
       - 3ms
       x-request-id:
-      - 11426ffcf7b1c3b89d73eec40961fa16
+      - 54bbac59f0706c9d5309538cf0a432c8
     http_version: HTTP/1.1
     status_code: 200
 version: 1
```

### Comparing `lbgpt-0.1.3/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_failed[-lambda-1].yaml` & `lbgpt-0.3.0/tests/cache/cassette/test_lb_cache/test_chatgpt_cache[cache0].yaml`

 * *Files 21% similar despite different names*

```diff
@@ -27,60 +27,60 @@
       x-stainless-os:
       - Linux
       x-stainless-package-version:
       - 1.5.0
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
-      - 3.11.4
+      - 3.11.7
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
-    content: "{\n  \"id\": \"chatcmpl-8Xw250r1upY6rAcwFVuboHsdoUjgu\",\n  \"object\":
-      \"chat.completion\",\n  \"created\": 1703098593,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+    content: "{\n  \"id\": \"chatcmpl-8e2hfyzt1XIR29KnDS48olczhwHaf\",\n  \"object\":
+      \"chat.completion\",\n  \"created\": 1704554203,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
       \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
       \"assistant\",\n        \"content\": \"Pong\"\n      },\n      \"logprobs\":
       null,\n      \"finish_reason\": \"stop\"\n    }\n  ],\n  \"usage\": {\n    \"prompt_tokens\":
       11,\n    \"completion_tokens\": 2,\n    \"total_tokens\": 13\n  },\n  \"system_fingerprint\":
       null\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 838a1b1c6aeeb47f-DXB
+      - 8414ec76df71b479-DXB
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Wed, 20 Dec 2023 18:56:33 GMT
+      - Sat, 06 Jan 2024 15:16:43 GMT
       Server:
       - cloudflare
       Set-Cookie:
-      - __cf_bm=ZCGKsuolKo.NtPvNpm021WK4jHby4YmVspsvIB77BWg-1703098593-1-AcxMGSZ0vB/tOErslMOTFi5+rXwT51ceGbCwrrBKUllhKWqm8S8rRjq61K+Pycag8NWFJE3RRoO+/j1p2vPRtTg=;
-        path=/; expires=Wed, 20-Dec-23 19:26:33 GMT; domain=.api.openai.com; HttpOnly;
+      - __cf_bm=gnKAbE8D_YyvYMRwRCof.s4oUgdielOzbt7Rn159zEQ-1704554203-1-AQbTkxlrgXcHHfd4MCmeZCKT9fTQHmD0SyOOVe0xxu+bV9SKvr9yCdJBxpttyvYgfSauj6QwaYAPpmZRwsKHWQE=;
+        path=/; expires=Sat, 06-Jan-24 15:46:43 GMT; domain=.api.openai.com; HttpOnly;
         Secure; SameSite=None
-      - _cfuvid=CCy_5LtjuTS6fb.6_7RwXO4JIQcn.v47uaPXqUdmNME-1703098593240-0-604800000;
+      - _cfuvid=.MLIs.zr75QfliaVKc5uGhxcLhK46Cau9wB.FFJu0Q4-1704554203649-0-604800000;
         path=/; domain=.api.openai.com; HttpOnly; Secure; SameSite=None
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
       - gpt-3.5-turbo-0613
       openai-organization:
       - marvin-labs
       openai-processing-ms:
-      - '262'
+      - '444'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '10000'
       x-ratelimit-limit-tokens:
@@ -96,19 +96,19 @@
       x-ratelimit-reset-requests:
       - 6ms
       x-ratelimit-reset-tokens:
       - 3ms
       x-ratelimit-reset-tokens_usage_based:
       - 3ms
       x-request-id:
-      - 95b98365d042efb29205b9d8030cd106
+      - ad478dd26af6bc0364b2edb3e5cf35e9
     http_version: HTTP/1.1
     status_code: 200
 - request:
-    body: '{"messages": [{"role": "user", "content": "please respond with test"}],
+    body: '{"messages": [{"role": "user", "content": "please respond with pong"}],
       "model": "gpt-3.5-turbo-0613", "frequency_penalty": 0, "max_tokens": 50, "presence_penalty":
       0, "temperature": 0, "top_p": 1}'
     headers:
       accept:
       - application/json
       accept-encoding:
       - gzip, deflate
@@ -131,60 +131,60 @@
       x-stainless-os:
       - Linux
       x-stainless-package-version:
       - 1.5.0
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
-      - 3.11.4
+      - 3.11.7
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
-    content: "{\n  \"id\": \"chatcmpl-8Xw25sEiAZhte8NJmu5CDLi7Ky1fR\",\n  \"object\":
-      \"chat.completion\",\n  \"created\": 1703098593,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+    content: "{\n  \"id\": \"chatcmpl-8e2hgteIUtspQ4lRDRz7OAhD12XrR\",\n  \"object\":
+      \"chat.completion\",\n  \"created\": 1704554204,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
       \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
-      \"assistant\",\n        \"content\": \"test\"\n      },\n      \"logprobs\":
+      \"assistant\",\n        \"content\": \"Pong\"\n      },\n      \"logprobs\":
       null,\n      \"finish_reason\": \"stop\"\n    }\n  ],\n  \"usage\": {\n    \"prompt_tokens\":
-      11,\n    \"completion_tokens\": 1,\n    \"total_tokens\": 12\n  },\n  \"system_fingerprint\":
+      11,\n    \"completion_tokens\": 2,\n    \"total_tokens\": 13\n  },\n  \"system_fingerprint\":
       null\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 838a1b202e74126e-DXB
+      - 8414ec7d1f76b476-DXB
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Wed, 20 Dec 2023 18:56:34 GMT
+      - Sat, 06 Jan 2024 15:16:44 GMT
       Server:
       - cloudflare
       Set-Cookie:
-      - __cf_bm=lfACNFSXdNXOHtP.NgE3vY.QgOFfTdn2YXOYvYdc18E-1703098594-1-AdkbX0Jf14LBT5SMrGVhGZsdeNJwZbG1UBtqmzBpno2M3/bLtJ0RAyPhKHUF9Ldkx7lXRb7qoeKzNo76WIOtUm8=;
-        path=/; expires=Wed, 20-Dec-23 19:26:34 GMT; domain=.api.openai.com; HttpOnly;
+      - __cf_bm=DfBWR2OLIKJi1VtpFWDNaYJJxvXfJJxVobY6UH7V6yQ-1704554204-1-AULIlusPGsfS+ie0QB9OUSwHzswi3iHE/ndNsYSUQKdxqVVVOmGDUYRXe+pAqEeGdc6vqZhAnDIXFK98VKWQk3c=;
+        path=/; expires=Sat, 06-Jan-24 15:46:44 GMT; domain=.api.openai.com; HttpOnly;
         Secure; SameSite=None
-      - _cfuvid=hsMtYVk6kOu9vTabx_PHCCEbI7yQ9XQuwVnGXOUq0fw-1703098594289-0-604800000;
+      - _cfuvid=XsAKd6RuYsoEubud3jmwwu.G.c_X_XBXBD9EJ9_Jt7o-1704554204731-0-604800000;
         path=/; domain=.api.openai.com; HttpOnly; Secure; SameSite=None
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
       - gpt-3.5-turbo-0613
       openai-organization:
       - marvin-labs
       openai-processing-ms:
-      - '439'
+      - '508'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '10000'
       x-ratelimit-limit-tokens:
@@ -200,11 +200,11 @@
       x-ratelimit-reset-requests:
       - 6ms
       x-ratelimit-reset-tokens:
       - 3ms
       x-ratelimit-reset-tokens_usage_based:
       - 3ms
       x-request-id:
-      - 54bbac59f0706c9d5309538cf0a432c8
+      - d9402ddb7477926d3689ecb306eccdf2
     http_version: HTTP/1.1
     status_code: 200
 version: 1
```

### Comparing `lbgpt-0.1.3/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_inexact[-lambda-0].yaml` & `lbgpt-0.3.0/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_inexact[-lambda-0].yaml`

 * *Files identical despite different names*

### Comparing `lbgpt-0.1.3/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_inexact[-lambda-1].yaml` & `lbgpt-0.3.0/tests/semantic_cache/cassette/test_lb_semantic_cache/test_chatgpt_cache_inexact[-lambda-1].yaml`

 * *Files identical despite different names*

### Comparing `lbgpt-0.1.3/LICENSE` & `lbgpt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lbgpt-0.1.3/README.md` & `lbgpt-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,98 +14,103 @@
 
 ## Usage
 
 ### Basic
 Initiate asynchronous calls to the ChatGPT API using the following basic example:
 
 ```python
+
 import lbgpt
 import asyncio
 
 chatgpt = lbgpt.ChatGPT(api_key="YOUR_API_KEY")
-res = asyncio.run(chatgpt.chat_completion_list([ "your list of prompts" ]))
+res = asyncio.run(chatgpt.chat_completion_list(["your list of prompts"]))
 ```
 
 The `chat_completion_list` function expects a list of dictionaries with fully-formed OpenAI ChatCompletion API requests. Refer to the [OpenAI API definition](https://platform.openai.com/docs/api-reference/chat/create) for more details. You can also use the `chat_completion` function for single requests.
 
 By default, LBGPT processes five requests in parallel, but you can adjust this by setting the `max_concurrent_requests` parameter in the constructor.
 
 
 ### Azure
 For users with an Azure account and proper OpenAI services setup, lbgpt offers an interface for Azure, similar to the OpenAI API. Here's how you can use it:
 
 ```python
+
 import lbgpt
 import asyncio
 
-chatgpt = lbgpt.AzureGPT(api_key="YOUR_API_KEY", azure_api_base="YOUR AZURE API BASE", azure_model_map={"OPENAI_MODEL_NAME": "MODEL NAME IN AZURE"})
-res = asyncio.run(chatgpt.chat_completion_list([ "your list of prompts" ]))
+chatgpt = lbgpt.AzureGPT(api_key="YOUR_API_KEY", azure_api_base="YOUR AZURE API BASE",
+                         azure_model_map={"OPENAI_MODEL_NAME": "MODEL NAME IN AZURE"})
+res = asyncio.run(chatgpt.chat_completion_list(["your list of prompts"]))
 ```
 
 
 You can use the same request definition for both OpenAI and Azure. To ensure interchangeability, map OpenAI model names to Azure model names using the `azure_model_map` parameter in the constructor (see https://learn.microsoft.com/en-us/azure/ai-services/openai/how-to/switching-endpoints for details).
 
 
 ### Load Balacing OpenAI and Azure
 For optimal performance and reliability, it's recommended to set up the `LoadBalancedGPT` or `MultiLoadBalancedGPT`. These classes automatically balance requests between OpenAI and Azure, and they also offer caching and automatic retries.
 
 `LoadBalancedGPT` offers load-balancing just between OpenAI and Azure models, but is slightly easier to set up. By default, 75% of requests are routed to the Azure API, while 25% go to the OpenAI API. You can customize this ratio by setting the `ratio_openai_to_azure` parameter in the constructor, taking into account that the Azure API is considerably faster.
-  
 
 ```python
+
 import lbgpt
 import asyncio
 
 chatgpt = lbgpt.LoadBalancedGPT(
     openai_api_key="YOUR_OPENAI_API_KEY",
     azure_api_key="YOUR_AZURE_API_KEY",
     azure_api_base="YOUR AZURE API BASE",
     azure_model_map={"OPENAI_MODEL_NAME": "MODEL NAME IN AZURE"})
-res = asyncio.run(chatgpt.chat_completion_list([ "your list of prompts" ]))
+res = asyncio.run(chatgpt.chat_completion_list(["your list of prompts"]))
 ```
 
 `MultiLoadBalancedGPT` offers load-balancing between multiple OpenAI and Azure models, and offers more flexibility in terms of the load balancing inputs. In order to achieve the same load balancing as the `LoadBalancedGPT`, you can use the following code:
 
 ```python
+
 import lbgpt
 import asyncio
 
 openai_chatgpt = lbgpt.ChatGPT(api_key="YOUR_API_KEY")
-azure_chatgpt = lbgpt.AzureGPT(api_key="YOUR_API_KEY", azure_api_base="YOUR AZURE API BASE", azure_model_map={"OPENAI_MODEL_NAME": "MODEL NAME IN AZURE"})
-
+azure_chatgpt = lbgpt.AzureGPT(api_key="YOUR_API_KEY", azure_api_base="YOUR AZURE API BASE",
+                               azure_model_map={"OPENAI_MODEL_NAME": "MODEL NAME IN AZURE"})
 
 chatgpt = lbgpt.MultiLoadBalancedGPT(
     gpts=[openai_chatgpt, azure_chatgpt],
     allocation_function_weights=[0.25, 0.75],
     allocation_function='random',
 )
-    
-res = asyncio.run(chatgpt.chat_completion_list([ "your list of prompts" ]))
+
+res = asyncio.run(chatgpt.chat_completion_list(["your list of prompts"]))
 ```
 
 However, the MultiLoadBalancedGPT offers more flexibility in terms of the load balancing inputs, e.g. supporting multiple Azure instances or OpenAI keys. 
 
 You can also select the allocation function `max_headroom` to automatically pick the API with the most available capacity. This requires you to tell the model constructors your RPM (requests per minute) and/or TPM (tokens per minute) limits. 
 
 For example, if you have an OpenAI API key with a 5,000 TPM limit and an Azure API key with a 10,000 TPM limit, you can use the following code:
 
 ```python
+
 import lbgpt
 import asyncio
 
 openai_chatgpt = lbgpt.ChatGPT(api_key="YOUR_API_KEY", limit_tpm=5_000)
-azure_chatgpt = lbgpt.AzureGPT(api_key="YOUR_API_KEY", azure_api_base="YOUR AZURE API BASE", azure_model_map={"OPENAI_MODEL_NAME": "MODEL NAME IN AZURE"}, limit_tpm=10_000)
-
+azure_chatgpt = lbgpt.AzureGPT(api_key="YOUR_API_KEY", azure_api_base="YOUR AZURE API BASE",
+                               azure_model_map={"OPENAI_MODEL_NAME": "MODEL NAME IN AZURE"}, limit_tpm=10_000)
 
 chatgpt = lbgpt.MultiLoadBalancedGPT(
     gpts=[openai_chatgpt, azure_chatgpt],
     allocation_function='max_headroom',
 )
-    
-res = asyncio.run(chatgpt.chat_completion_list([ "your list of prompts" ]))
+
+res = asyncio.run(chatgpt.chat_completion_list(["your list of prompts"]))
 ```
 
 ## Caching
 
 LBGPT implements two means of caching: basic caching and semantic cachin:
 
 * Basic caching: Caches the exact request and response.
@@ -114,44 +119,46 @@
 Both caching methods can be combined. If both caches are used, requests are first requested from the basic cache. Only if the request is not found in the basic cache, the semantic cache is checked. If the request is not found in the semantic cache, the request is sent to the API and the response is cached in both caches.
 
 
 ### Basic Caching
 Take advantage of request caching to avoid redundant calls:
 
 ```python
+
 import lbgpt
 import asyncio
 import diskcache
 
 cache = diskcache.Cache("cache_dir")
 chatgpt = lbgpt.ChatGPT(api_key="YOUR_API_KEY", cache=cache)
-res = asyncio.run(chatgpt.chat_completion_list([ "your list of prompts" ]))
+res = asyncio.run(chatgpt.chat_completion_list(["your list of prompts"]))
 ```
 
 While LBGPT is tested only with [diskcache](https://pypi.org/project/diskcache/), it should work seamlessly with any cache that implements the `__getitem__` and `__setitem__` methods.
 
 
 ### Semantic Caching
 Semantic caching looks for semantic variations of the request in the cache. For example, if the request message is "Hello, how are you?", the semantic cache will also return a cached response for "Hello, how are you doing?". The semantic cache uses embedding models supported by HuggingFace to determine semantic similarity.
 
 ```python
+
 import lbgpt
 from lbgpt.semantic_cache import FaissSemanticCache
 from langchain.embeddings import HuggingFaceEmbeddings
 
 import asyncio
 
 semantic_cache = FaissSemanticCache(
-        embedding_model=HuggingFaceEmbeddings(model_name="bert-base-uncased"),
-        cosine_similarity_threshold=0.95,
-        path='cache_dir'
-    )
+    embedding_model=HuggingFaceEmbeddings(model_name="bert-base-uncased"),
+    cosine_similarity_threshold=0.95,
+    path='cache_dir'
+)
 
 chatgpt = lbgpt.ChatGPT(api_key="YOUR_API_KEY", semantic_cache=semantic_cache)
-res = asyncio.run(chatgpt.chat_completion_list([ "your list of prompts" ]))
+res = asyncio.run(chatgpt.chat_completion_list(["your list of prompts"]))
 ```
 
 Currently, the only supported semantic caches are [FAISS](https://faiss.ai/) (via the [langchain](https://www.langchain.com/) interface) and [Qdrant](https://qdrant.tech/). Please let us know if you would like to see support for other semantic caches. 
 
 In this example, all requests messages are embedded using the `bert-base-uncased` model from HuggingFace. The cosine similarity threshold determines how similar two messages must be to be considered semantically equivalent. The path parameter determines where the semantic cache is stored.
```

### Comparing `lbgpt-0.1.3/PKG-INFO` & `lbgpt-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: LBGPT
-Version: 0.1.3
+Version: 0.3.0
 Summary: Load balancer for asynchroneous requests to the APIs of OpenAI and Azure (if configured) for ChatGPT
 Project-URL: Homepage, https://github.com/Marvin-Labs/lbgpt
 Project-URL: Bug Tracker, https://github.com/Marvin-Labs/lbgpt/issues
 Author-email: Marvin Labs <marvin@marvin-labs.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Load Balancing ChatGPT (LBGPT)
 
 Enhance your ChatGPT API experience with the LoadBalancing ChatGPT (LBGPT), a wrapper around OpenAI's API designed to boost performance, enable caching, and provide seamless integration with Azure's OpenAI API.
 
 This tool significantly optimizes single request response times by asynchronously interacting with the OpenAI API and efficiently caching results. It also offers automatic retries in the event of API errors and the option to balance requests between OpenAI and Azure for an even more robust AI experience.
@@ -28,98 +28,103 @@
 
 ## Usage
 
 ### Basic
 Initiate asynchronous calls to the ChatGPT API using the following basic example:
 
 ```python
+
 import lbgpt
 import asyncio
 
 chatgpt = lbgpt.ChatGPT(api_key="YOUR_API_KEY")
-res = asyncio.run(chatgpt.chat_completion_list([ "your list of prompts" ]))
+res = asyncio.run(chatgpt.chat_completion_list(["your list of prompts"]))
 ```
 
 The `chat_completion_list` function expects a list of dictionaries with fully-formed OpenAI ChatCompletion API requests. Refer to the [OpenAI API definition](https://platform.openai.com/docs/api-reference/chat/create) for more details. You can also use the `chat_completion` function for single requests.
 
 By default, LBGPT processes five requests in parallel, but you can adjust this by setting the `max_concurrent_requests` parameter in the constructor.
 
 
 ### Azure
 For users with an Azure account and proper OpenAI services setup, lbgpt offers an interface for Azure, similar to the OpenAI API. Here's how you can use it:
 
 ```python
+
 import lbgpt
 import asyncio
 
-chatgpt = lbgpt.AzureGPT(api_key="YOUR_API_KEY", azure_api_base="YOUR AZURE API BASE", azure_model_map={"OPENAI_MODEL_NAME": "MODEL NAME IN AZURE"})
-res = asyncio.run(chatgpt.chat_completion_list([ "your list of prompts" ]))
+chatgpt = lbgpt.AzureGPT(api_key="YOUR_API_KEY", azure_api_base="YOUR AZURE API BASE",
+                         azure_model_map={"OPENAI_MODEL_NAME": "MODEL NAME IN AZURE"})
+res = asyncio.run(chatgpt.chat_completion_list(["your list of prompts"]))
 ```
 
 
 You can use the same request definition for both OpenAI and Azure. To ensure interchangeability, map OpenAI model names to Azure model names using the `azure_model_map` parameter in the constructor (see https://learn.microsoft.com/en-us/azure/ai-services/openai/how-to/switching-endpoints for details).
 
 
 ### Load Balacing OpenAI and Azure
 For optimal performance and reliability, it's recommended to set up the `LoadBalancedGPT` or `MultiLoadBalancedGPT`. These classes automatically balance requests between OpenAI and Azure, and they also offer caching and automatic retries.
 
 `LoadBalancedGPT` offers load-balancing just between OpenAI and Azure models, but is slightly easier to set up. By default, 75% of requests are routed to the Azure API, while 25% go to the OpenAI API. You can customize this ratio by setting the `ratio_openai_to_azure` parameter in the constructor, taking into account that the Azure API is considerably faster.
-  
 
 ```python
+
 import lbgpt
 import asyncio
 
 chatgpt = lbgpt.LoadBalancedGPT(
     openai_api_key="YOUR_OPENAI_API_KEY",
     azure_api_key="YOUR_AZURE_API_KEY",
     azure_api_base="YOUR AZURE API BASE",
     azure_model_map={"OPENAI_MODEL_NAME": "MODEL NAME IN AZURE"})
-res = asyncio.run(chatgpt.chat_completion_list([ "your list of prompts" ]))
+res = asyncio.run(chatgpt.chat_completion_list(["your list of prompts"]))
 ```
 
 `MultiLoadBalancedGPT` offers load-balancing between multiple OpenAI and Azure models, and offers more flexibility in terms of the load balancing inputs. In order to achieve the same load balancing as the `LoadBalancedGPT`, you can use the following code:
 
 ```python
+
 import lbgpt
 import asyncio
 
 openai_chatgpt = lbgpt.ChatGPT(api_key="YOUR_API_KEY")
-azure_chatgpt = lbgpt.AzureGPT(api_key="YOUR_API_KEY", azure_api_base="YOUR AZURE API BASE", azure_model_map={"OPENAI_MODEL_NAME": "MODEL NAME IN AZURE"})
-
+azure_chatgpt = lbgpt.AzureGPT(api_key="YOUR_API_KEY", azure_api_base="YOUR AZURE API BASE",
+                               azure_model_map={"OPENAI_MODEL_NAME": "MODEL NAME IN AZURE"})
 
 chatgpt = lbgpt.MultiLoadBalancedGPT(
     gpts=[openai_chatgpt, azure_chatgpt],
     allocation_function_weights=[0.25, 0.75],
     allocation_function='random',
 )
-    
-res = asyncio.run(chatgpt.chat_completion_list([ "your list of prompts" ]))
+
+res = asyncio.run(chatgpt.chat_completion_list(["your list of prompts"]))
 ```
 
 However, the MultiLoadBalancedGPT offers more flexibility in terms of the load balancing inputs, e.g. supporting multiple Azure instances or OpenAI keys. 
 
 You can also select the allocation function `max_headroom` to automatically pick the API with the most available capacity. This requires you to tell the model constructors your RPM (requests per minute) and/or TPM (tokens per minute) limits. 
 
 For example, if you have an OpenAI API key with a 5,000 TPM limit and an Azure API key with a 10,000 TPM limit, you can use the following code:
 
 ```python
+
 import lbgpt
 import asyncio
 
 openai_chatgpt = lbgpt.ChatGPT(api_key="YOUR_API_KEY", limit_tpm=5_000)
-azure_chatgpt = lbgpt.AzureGPT(api_key="YOUR_API_KEY", azure_api_base="YOUR AZURE API BASE", azure_model_map={"OPENAI_MODEL_NAME": "MODEL NAME IN AZURE"}, limit_tpm=10_000)
-
+azure_chatgpt = lbgpt.AzureGPT(api_key="YOUR_API_KEY", azure_api_base="YOUR AZURE API BASE",
+                               azure_model_map={"OPENAI_MODEL_NAME": "MODEL NAME IN AZURE"}, limit_tpm=10_000)
 
 chatgpt = lbgpt.MultiLoadBalancedGPT(
     gpts=[openai_chatgpt, azure_chatgpt],
     allocation_function='max_headroom',
 )
-    
-res = asyncio.run(chatgpt.chat_completion_list([ "your list of prompts" ]))
+
+res = asyncio.run(chatgpt.chat_completion_list(["your list of prompts"]))
 ```
 
 ## Caching
 
 LBGPT implements two means of caching: basic caching and semantic cachin:
 
 * Basic caching: Caches the exact request and response.
@@ -128,44 +133,46 @@
 Both caching methods can be combined. If both caches are used, requests are first requested from the basic cache. Only if the request is not found in the basic cache, the semantic cache is checked. If the request is not found in the semantic cache, the request is sent to the API and the response is cached in both caches.
 
 
 ### Basic Caching
 Take advantage of request caching to avoid redundant calls:
 
 ```python
+
 import lbgpt
 import asyncio
 import diskcache
 
 cache = diskcache.Cache("cache_dir")
 chatgpt = lbgpt.ChatGPT(api_key="YOUR_API_KEY", cache=cache)
-res = asyncio.run(chatgpt.chat_completion_list([ "your list of prompts" ]))
+res = asyncio.run(chatgpt.chat_completion_list(["your list of prompts"]))
 ```
 
 While LBGPT is tested only with [diskcache](https://pypi.org/project/diskcache/), it should work seamlessly with any cache that implements the `__getitem__` and `__setitem__` methods.
 
 
 ### Semantic Caching
 Semantic caching looks for semantic variations of the request in the cache. For example, if the request message is "Hello, how are you?", the semantic cache will also return a cached response for "Hello, how are you doing?". The semantic cache uses embedding models supported by HuggingFace to determine semantic similarity.
 
 ```python
+
 import lbgpt
 from lbgpt.semantic_cache import FaissSemanticCache
 from langchain.embeddings import HuggingFaceEmbeddings
 
 import asyncio
 
 semantic_cache = FaissSemanticCache(
-        embedding_model=HuggingFaceEmbeddings(model_name="bert-base-uncased"),
-        cosine_similarity_threshold=0.95,
-        path='cache_dir'
-    )
+    embedding_model=HuggingFaceEmbeddings(model_name="bert-base-uncased"),
+    cosine_similarity_threshold=0.95,
+    path='cache_dir'
+)
 
 chatgpt = lbgpt.ChatGPT(api_key="YOUR_API_KEY", semantic_cache=semantic_cache)
-res = asyncio.run(chatgpt.chat_completion_list([ "your list of prompts" ]))
+res = asyncio.run(chatgpt.chat_completion_list(["your list of prompts"]))
 ```
 
 Currently, the only supported semantic caches are [FAISS](https://faiss.ai/) (via the [langchain](https://www.langchain.com/) interface) and [Qdrant](https://qdrant.tech/). Please let us know if you would like to see support for other semantic caches. 
 
 In this example, all requests messages are embedded using the `bert-base-uncased` model from HuggingFace. The cosine similarity threshold determines how similar two messages must be to be considered semantically equivalent. The path parameter determines where the semantic cache is stored.
```


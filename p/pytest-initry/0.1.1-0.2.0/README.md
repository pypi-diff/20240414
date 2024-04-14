# Comparing `tmp/pytest_initry-0.1.1.tar.gz` & `tmp/pytest_initry-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_initry-0.1.1.tar", max compression
+gzip compressed data, was "pytest_initry-0.2.0.tar", max compression
```

## Comparing `pytest_initry-0.1.1.tar` & `pytest_initry-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,19 @@
--rw-r--r--   0        0        0     1072 2024-04-09 17:28:57.000000 pytest_initry-0.1.1/LICENSE
--rw-r--r--   0        0        0      645 2024-04-09 17:28:34.000000 pytest_initry-0.1.1/README.md
--rw-r--r--   0        0        0      923 2024-04-09 16:52:25.000000 pytest_initry-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-08 19:27:30.000000 pytest_initry-0.1.1/pytest_initry/__init__.py
--rw-r--r--   0        0        0    10789 2024-04-09 16:18:19.000000 pytest_initry-0.1.1/pytest_initry/plugin.py
--rw-r--r--   0        0        0       85 2024-04-09 17:28:07.000000 pytest_initry-0.1.1/pytest_initry/protobufs/__init__.py
--rw-r--r--   0        0        0      438 2024-04-04 21:49:30.907525 pytest_initry-0.1.1/pytest_initry/protobufs/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1260 2024-04-06 18:55:38.434205 pytest_initry-0.1.1/pytest_initry/protobufs/__pycache__/responses_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     2660 2024-04-06 18:55:38.454205 pytest_initry-0.1.1/pytest_initry/protobufs/__pycache__/test_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     7245 2024-04-06 18:55:38.454205 pytest_initry-0.1.1/pytest_initry/protobufs/__pycache__/test_pb2_grpc.cpython-311.pyc
--rw-r--r--   0        0        0     1999 2024-04-06 18:55:38.450205 pytest_initry-0.1.1/pytest_initry/protobufs/__pycache__/test_run_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     4743 2024-04-06 18:55:38.430205 pytest_initry-0.1.1/pytest_initry/protobufs/__pycache__/test_run_pb2_grpc.cpython-311.pyc
--rw-r--r--   0        0        0     1708 2024-04-06 18:55:38.454205 pytest_initry-0.1.1/pytest_initry/protobufs/__pycache__/tests_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     3527 2024-04-06 18:55:38.454205 pytest_initry-0.1.1/pytest_initry/protobufs/__pycache__/tests_pb2_grpc.cpython-311.pyc
--rw-r--r--   0        0        0     1028 2024-04-04 21:49:29.000000 pytest_initry-0.1.1/pytest_initry/protobufs/responses_pb2.py
--rw-r--r--   0        0        0      410 2024-04-04 21:49:30.000000 pytest_initry-0.1.1/pytest_initry/protobufs/responses_pb2.pyi
--rw-r--r--   0        0        0      158 2024-04-04 21:49:29.000000 pytest_initry-0.1.1/pytest_initry/protobufs/responses_pb2_grpc.py
--rw-r--r--   0        0        0     2883 2024-04-04 21:49:30.000000 pytest_initry-0.1.1/pytest_initry/protobufs/test_pb2.py
--rw-r--r--   0        0        0     2763 2024-04-04 21:49:30.000000 pytest_initry-0.1.1/pytest_initry/protobufs/test_pb2.pyi
--rw-r--r--   0        0        0     6308 2024-04-04 21:49:30.000000 pytest_initry-0.1.1/pytest_initry/protobufs/test_pb2_grpc.py
--rw-r--r--   0        0        0     1921 2024-04-04 21:49:30.000000 pytest_initry-0.1.1/pytest_initry/protobufs/test_run_pb2.py
--rw-r--r--   0        0        0     1426 2024-04-04 21:49:30.000000 pytest_initry-0.1.1/pytest_initry/protobufs/test_run_pb2.pyi
--rw-r--r--   0        0        0     4089 2024-04-04 21:49:30.000000 pytest_initry-0.1.1/pytest_initry/protobufs/test_run_pb2_grpc.py
--rw-r--r--   0        0        0     1615 2024-04-04 21:49:30.000000 pytest_initry-0.1.1/pytest_initry/protobufs/tests_pb2.py
--rw-r--r--   0        0        0     1390 2024-04-04 21:49:30.000000 pytest_initry-0.1.1/pytest_initry/protobufs/tests_pb2.pyi
--rw-r--r--   0        0        0     2489 2024-04-04 21:49:30.000000 pytest_initry-0.1.1/pytest_initry/protobufs/tests_pb2_grpc.py
--rw-r--r--   0        0        0     1413 1970-01-01 00:00:00.000000 pytest_initry-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-09 17:28:57.000000 pytest_initry-0.2.0/LICENSE
+-rw-r--r--   0        0        0      645 2024-04-09 17:28:34.000000 pytest_initry-0.2.0/README.md
+-rw-r--r--   0        0        0      924 2024-04-14 12:17:05.000000 pytest_initry-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-08 19:27:30.000000 pytest_initry-0.2.0/pytest_initry/__init__.py
+-rw-r--r--   0        0        0    11084 2024-04-14 15:05:50.000000 pytest_initry-0.2.0/pytest_initry/plugin.py
+-rw-r--r--   0        0        0       85 2024-04-09 17:28:07.000000 pytest_initry-0.2.0/pytest_initry/protobufs/__init__.py
+-rw-r--r--   0        0        0     1014 2024-04-14 14:30:38.374723 pytest_initry-0.2.0/pytest_initry/protobufs/responses_pb2.py
+-rw-r--r--   0        0        0      391 2024-04-14 14:30:38.374723 pytest_initry-0.2.0/pytest_initry/protobufs/responses_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-14 14:30:38.374723 pytest_initry-0.2.0/pytest_initry/protobufs/responses_pb2_grpc.py
+-rw-r--r--   0        0        0     2936 2024-04-14 14:30:38.454723 pytest_initry-0.2.0/pytest_initry/protobufs/test_pb2.py
+-rw-r--r--   0        0        0     2858 2024-04-14 14:30:38.454723 pytest_initry-0.2.0/pytest_initry/protobufs/test_pb2.pyi
+-rw-r--r--   0        0        0     6171 2024-04-14 14:30:38.454723 pytest_initry-0.2.0/pytest_initry/protobufs/test_pb2_grpc.py
+-rw-r--r--   0        0        0     1885 2024-04-14 14:30:38.410723 pytest_initry-0.2.0/pytest_initry/protobufs/test_run_pb2.py
+-rw-r--r--   0        0        0     1293 2024-04-14 14:30:38.410723 pytest_initry-0.2.0/pytest_initry/protobufs/test_run_pb2.pyi
+-rw-r--r--   0        0        0     3998 2024-04-14 14:30:38.414723 pytest_initry-0.2.0/pytest_initry/protobufs/test_run_pb2_grpc.py
+-rw-r--r--   0        0        0     1585 2024-04-14 14:30:38.490723 pytest_initry-0.2.0/pytest_initry/protobufs/tests_pb2.py
+-rw-r--r--   0        0        0     1248 2024-04-14 14:30:38.490723 pytest_initry-0.2.0/pytest_initry/protobufs/tests_pb2.pyi
+-rw-r--r--   0        0        0     2444 2024-04-14 14:30:38.490723 pytest_initry-0.2.0/pytest_initry/protobufs/tests_pb2_grpc.py
+-rw-r--r--   0        0        0     1413 1970-01-01 00:00:00.000000 pytest_initry-0.2.0/PKG-INFO
```

### Comparing `pytest_initry-0.1.1/LICENSE` & `pytest_initry-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_initry-0.1.1/README.md` & `pytest_initry-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_initry-0.1.1/pyproject.toml` & `pytest_initry-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-initry"
-version = "0.1.1"
+version = "0.2.0"
 description = "Plugin for sending automation test data from Pytest to the initry"
 authors = ["Andrejs Smirnovs <and.inbx@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Framework :: Pytest",
 ]
@@ -37,8 +37,8 @@
 exclude = [
     'pytest_initry/protobufs/*'
     ]
 
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `pytest_initry-0.1.1/pytest_initry/plugin.py` & `pytest_initry-0.2.0/pytest_initry/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,32 +159,39 @@
 
             self.cs_test_grpc_client.call_rpc_method(
                 "ModifyTest", self.started_finished_pairs()
             )
             self.pairs = []
 
     def pytest_runtest_logreport(self, report):
+
         if self.test_uuid is not None:
             if report.when == "call" and report.outcome == "failed":
                 if report.failed and not hasattr(report, "wasxfail"):
                     request = test_pb2.StopTestRequest(
                         uuid=self.test_uuid,
                         stopped_at=Timestamp(seconds=int(time.time())),
                         status=test_pb2.TestStatus.FAILED,
+                        log=report.longreprtext,
+                        stdout=report.capstdout,
+                        stderr=report.capstderr,
                     )
                     if not self.initry_batching:
                         self.test_grpc_client.call_rpc_method("StopTest", request)
                     else:
                         self.create_pairs_for_batching(request)
             elif report.when == "setup" and report.outcome == "failed":
                 if report.failed and not hasattr(report, "wasxfail"):
                     request = test_pb2.StopTestRequest(
                         uuid=self.test_uuid,
                         stopped_at=Timestamp(seconds=int(time.time())),
                         status=test_pb2.TestStatus.FAILED,
+                        log=report.longreprtext,
+                        stdout=report.capstdout,
+                        stderr=report.capstderr,
                     )
                     if not self.initry_batching:
                         self.test_grpc_client.call_rpc_method("StopTest", request)
                     else:
                         self.create_pairs_for_batching(request)
             elif report.when == "call" and report.outcome == "passed":
                 request = test_pb2.StopTestRequest(
```

### Comparing `pytest_initry-0.1.1/pytest_initry/protobufs/responses_pb2.py` & `pytest_initry-0.2.0/pytest_initry/protobufs/responses_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 # source: responses.proto
 # Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x0fresponses.proto"\x1a\n\x08StatusOk\x12\x0e\n\x06status\x18\x01 \x01(\tb\x06proto3'
-)
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fresponses.proto\"\x1a\n\x08StatusOk\x12\x0e\n\x06status\x18\x01 \x01(\tb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "responses_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'responses_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-    DESCRIPTOR._options = None
-    _globals["_STATUSOK"]._serialized_start = 19
-    _globals["_STATUSOK"]._serialized_end = 45
+  DESCRIPTOR._options = None
+  _globals['_STATUSOK']._serialized_start=19
+  _globals['_STATUSOK']._serialized_end=45
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pytest_initry-0.1.1/pytest_initry/protobufs/test_pb2.py` & `pytest_initry-0.2.0/pytest_initry/protobufs/test_run_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: test.proto
+# source: test_run.proto
 # Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 import responses_pb2 as responses__pb2
-from google.protobuf import \
-    timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\ntest.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x0fresponses.proto"m\n\x10StartTestRequest\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x06status\x18\x03 \x01(\x0e\x32\x0b.TestStatus"l\n\x0fStopTestRequest\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12.\n\nstopped_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x06status\x18\x03 \x01(\x0e\x32\x0b.TestStatus"\x9e\x01\n\x11ModifyTestRequest\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nstopped_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x06status\x18\x04 \x01(\x0e\x32\x0b.TestStatus*\x80\x01\n\nTestStatus\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07RUNNING\x10\x01\x12\n\n\x06PASSED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x0b\n\x07SKIPPED\x10\x04\x12\x13\n\x0f\x45XPECTED_PASSED\x10\x05\x12\x13\n\x0f\x45XPECTED_FAILED\x10\x06\x12\t\n\x05\x45RROR\x10\x07\x32\x61\n\x0bTestService\x12)\n\tStartTest\x12\x11.StartTestRequest\x1a\t.StatusOk\x12\'\n\x08StopTest\x12\x10.StopTestRequest\x1a\t.StatusOk2H\n\x17\x43lientStreamTestService\x12-\n\nModifyTest\x12\x12.ModifyTestRequest\x1a\t.StatusOk(\x01\x62\x06proto3'
-)
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0etest_run.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x0fresponses.proto\"~\n\x14\x43reateTestRunRequest\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0btests_count\x18\x03 \x01(\x05\x12\x13\n\x0bplugin_type\x18\x04 \x01(\t\"R\n\x12StopTestRunRequest\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12.\n\nstopped_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp2r\n\x0eTestRunService\x12\x31\n\rCreateTestRun\x12\x15.CreateTestRunRequest\x1a\t.StatusOk\x12-\n\x0bStopTestRun\x12\x13.StopTestRunRequest\x1a\t.StatusOkb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "test_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'test_run_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-    DESCRIPTOR._options = None
-    _globals["_TESTSTATUS"]._serialized_start = 447
-    _globals["_TESTSTATUS"]._serialized_end = 575
-    _globals["_STARTTESTREQUEST"]._serialized_start = 64
-    _globals["_STARTTESTREQUEST"]._serialized_end = 173
-    _globals["_STOPTESTREQUEST"]._serialized_start = 175
-    _globals["_STOPTESTREQUEST"]._serialized_end = 283
-    _globals["_MODIFYTESTREQUEST"]._serialized_start = 286
-    _globals["_MODIFYTESTREQUEST"]._serialized_end = 444
-    _globals["_TESTSERVICE"]._serialized_start = 577
-    _globals["_TESTSERVICE"]._serialized_end = 674
-    _globals["_CLIENTSTREAMTESTSERVICE"]._serialized_start = 676
-    _globals["_CLIENTSTREAMTESTSERVICE"]._serialized_end = 748
+  DESCRIPTOR._options = None
+  _globals['_CREATETESTRUNREQUEST']._serialized_start=68
+  _globals['_CREATETESTRUNREQUEST']._serialized_end=194
+  _globals['_STOPTESTRUNREQUEST']._serialized_start=196
+  _globals['_STOPTESTRUNREQUEST']._serialized_end=278
+  _globals['_TESTRUNSERVICE']._serialized_start=280
+  _globals['_TESTRUNSERVICE']._serialized_end=394
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pytest_initry-0.1.1/pytest_initry/protobufs/test_pb2.pyi` & `pytest_initry-0.2.0/pytest_initry/protobufs/test_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-from typing import ClassVar as _ClassVar
-from typing import Mapping as _Mapping
-from typing import Optional as _Optional
-from typing import Union as _Union
-
+from google.protobuf import timestamp_pb2 as _timestamp_pb2
 import responses_pb2 as _responses_pb2
+from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from google.protobuf import timestamp_pb2 as _timestamp_pb2
-from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
+from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class TestStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     UNKNOWN: _ClassVar[TestStatus]
     RUNNING: _ClassVar[TestStatus]
     PASSED: _ClassVar[TestStatus]
     FAILED: _ClassVar[TestStatus]
     SKIPPED: _ClassVar[TestStatus]
     EXPECTED_PASSED: _ClassVar[TestStatus]
     EXPECTED_FAILED: _ClassVar[TestStatus]
     ERROR: _ClassVar[TestStatus]
-
 UNKNOWN: TestStatus
 RUNNING: TestStatus
 PASSED: TestStatus
 FAILED: TestStatus
 SKIPPED: TestStatus
 EXPECTED_PASSED: TestStatus
 EXPECTED_FAILED: TestStatus
@@ -35,46 +30,36 @@
     __slots__ = ("uuid", "started_at", "status")
     UUID_FIELD_NUMBER: _ClassVar[int]
     STARTED_AT_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     uuid: str
     started_at: _timestamp_pb2.Timestamp
     status: TestStatus
-    def __init__(
-        self,
-        uuid: _Optional[str] = ...,
-        started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
-        status: _Optional[_Union[TestStatus, str]] = ...,
-    ) -> None: ...
+    def __init__(self, uuid: _Optional[str] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., status: _Optional[_Union[TestStatus, str]] = ...) -> None: ...
 
 class StopTestRequest(_message.Message):
-    __slots__ = ("uuid", "stopped_at", "status")
+    __slots__ = ("uuid", "stopped_at", "status", "log", "stdout", "stderr")
     UUID_FIELD_NUMBER: _ClassVar[int]
     STOPPED_AT_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
+    LOG_FIELD_NUMBER: _ClassVar[int]
+    STDOUT_FIELD_NUMBER: _ClassVar[int]
+    STDERR_FIELD_NUMBER: _ClassVar[int]
     uuid: str
     stopped_at: _timestamp_pb2.Timestamp
     status: TestStatus
-    def __init__(
-        self,
-        uuid: _Optional[str] = ...,
-        stopped_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
-        status: _Optional[_Union[TestStatus, str]] = ...,
-    ) -> None: ...
+    log: str
+    stdout: str
+    stderr: str
+    def __init__(self, uuid: _Optional[str] = ..., stopped_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., status: _Optional[_Union[TestStatus, str]] = ..., log: _Optional[str] = ..., stdout: _Optional[str] = ..., stderr: _Optional[str] = ...) -> None: ...
 
 class ModifyTestRequest(_message.Message):
     __slots__ = ("uuid", "started_at", "stopped_at", "status")
     UUID_FIELD_NUMBER: _ClassVar[int]
     STARTED_AT_FIELD_NUMBER: _ClassVar[int]
     STOPPED_AT_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     uuid: str
     started_at: _timestamp_pb2.Timestamp
     stopped_at: _timestamp_pb2.Timestamp
     status: TestStatus
-    def __init__(
-        self,
-        uuid: _Optional[str] = ...,
-        started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
-        stopped_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
-        status: _Optional[_Union[TestStatus, str]] = ...,
-    ) -> None: ...
+    def __init__(self, uuid: _Optional[str] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., stopped_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., status: _Optional[_Union[TestStatus, str]] = ...) -> None: ...
```

### Comparing `pytest_initry-0.1.1/pytest_initry/protobufs/test_pb2_grpc.py` & `pytest_initry-0.2.0/pytest_initry/protobufs/test_pb2_grpc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,198 +1,161 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
+
 import responses_pb2 as responses__pb2
 import test_pb2 as test__pb2
 
 
 class TestServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.StartTest = channel.unary_unary(
-            "/TestService/StartTest",
-            request_serializer=test__pb2.StartTestRequest.SerializeToString,
-            response_deserializer=responses__pb2.StatusOk.FromString,
-        )
+                '/TestService/StartTest',
+                request_serializer=test__pb2.StartTestRequest.SerializeToString,
+                response_deserializer=responses__pb2.StatusOk.FromString,
+                )
         self.StopTest = channel.unary_unary(
-            "/TestService/StopTest",
-            request_serializer=test__pb2.StopTestRequest.SerializeToString,
-            response_deserializer=responses__pb2.StatusOk.FromString,
-        )
+                '/TestService/StopTest',
+                request_serializer=test__pb2.StopTestRequest.SerializeToString,
+                response_deserializer=responses__pb2.StatusOk.FromString,
+                )
 
 
 class TestServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def StartTest(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def StopTest(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
 
 def add_TestServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "StartTest": grpc.unary_unary_rpc_method_handler(
-            servicer.StartTest,
-            request_deserializer=test__pb2.StartTestRequest.FromString,
-            response_serializer=responses__pb2.StatusOk.SerializeToString,
-        ),
-        "StopTest": grpc.unary_unary_rpc_method_handler(
-            servicer.StopTest,
-            request_deserializer=test__pb2.StopTestRequest.FromString,
-            response_serializer=responses__pb2.StatusOk.SerializeToString,
-        ),
+            'StartTest': grpc.unary_unary_rpc_method_handler(
+                    servicer.StartTest,
+                    request_deserializer=test__pb2.StartTestRequest.FromString,
+                    response_serializer=responses__pb2.StatusOk.SerializeToString,
+            ),
+            'StopTest': grpc.unary_unary_rpc_method_handler(
+                    servicer.StopTest,
+                    request_deserializer=test__pb2.StopTestRequest.FromString,
+                    response_serializer=responses__pb2.StatusOk.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "TestService", rpc_method_handlers
-    )
+            'TestService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
-# This class is part of an EXPERIMENTAL API.
+ # This class is part of an EXPERIMENTAL API.
 class TestService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def StartTest(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def StartTest(request,
             target,
-            "/TestService/StartTest",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/TestService/StartTest',
             test__pb2.StartTestRequest.SerializeToString,
             responses__pb2.StatusOk.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def StopTest(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def StopTest(request,
             target,
-            "/TestService/StopTest",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/TestService/StopTest',
             test__pb2.StopTestRequest.SerializeToString,
             responses__pb2.StatusOk.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
 
 class ClientStreamTestServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.ModifyTest = channel.stream_unary(
-            "/ClientStreamTestService/ModifyTest",
-            request_serializer=test__pb2.ModifyTestRequest.SerializeToString,
-            response_deserializer=responses__pb2.StatusOk.FromString,
-        )
+                '/ClientStreamTestService/ModifyTest',
+                request_serializer=test__pb2.ModifyTestRequest.SerializeToString,
+                response_deserializer=responses__pb2.StatusOk.FromString,
+                )
 
 
 class ClientStreamTestServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def ModifyTest(self, request_iterator, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
 
 def add_ClientStreamTestServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "ModifyTest": grpc.stream_unary_rpc_method_handler(
-            servicer.ModifyTest,
-            request_deserializer=test__pb2.ModifyTestRequest.FromString,
-            response_serializer=responses__pb2.StatusOk.SerializeToString,
-        ),
+            'ModifyTest': grpc.stream_unary_rpc_method_handler(
+                    servicer.ModifyTest,
+                    request_deserializer=test__pb2.ModifyTestRequest.FromString,
+                    response_serializer=responses__pb2.StatusOk.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "ClientStreamTestService", rpc_method_handlers
-    )
+            'ClientStreamTestService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
-# This class is part of an EXPERIMENTAL API.
+ # This class is part of an EXPERIMENTAL API.
 class ClientStreamTestService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def ModifyTest(
-        request_iterator,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.stream_unary(
-            request_iterator,
+    def ModifyTest(request_iterator,
             target,
-            "/ClientStreamTestService/ModifyTest",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.stream_unary(request_iterator, target, '/ClientStreamTestService/ModifyTest',
             test__pb2.ModifyTestRequest.SerializeToString,
             responses__pb2.StatusOk.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `pytest_initry-0.1.1/pytest_initry/protobufs/test_run_pb2.pyi` & `pytest_initry-0.2.0/pytest_initry/protobufs/test_run_pb2.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,27 @@
-from typing import ClassVar as _ClassVar
-from typing import Mapping as _Mapping
-from typing import Optional as _Optional
-from typing import Union as _Union
-
+from google.protobuf import timestamp_pb2 as _timestamp_pb2
 import responses_pb2 as _responses_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from google.protobuf import timestamp_pb2 as _timestamp_pb2
+from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class CreateTestRunRequest(_message.Message):
     __slots__ = ("uuid", "started_at", "tests_count", "plugin_type")
     UUID_FIELD_NUMBER: _ClassVar[int]
     STARTED_AT_FIELD_NUMBER: _ClassVar[int]
     TESTS_COUNT_FIELD_NUMBER: _ClassVar[int]
     PLUGIN_TYPE_FIELD_NUMBER: _ClassVar[int]
     uuid: str
     started_at: _timestamp_pb2.Timestamp
     tests_count: int
     plugin_type: str
-    def __init__(
-        self,
-        uuid: _Optional[str] = ...,
-        started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
-        tests_count: _Optional[int] = ...,
-        plugin_type: _Optional[str] = ...,
-    ) -> None: ...
+    def __init__(self, uuid: _Optional[str] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., tests_count: _Optional[int] = ..., plugin_type: _Optional[str] = ...) -> None: ...
 
 class StopTestRunRequest(_message.Message):
     __slots__ = ("uuid", "stopped_at")
     UUID_FIELD_NUMBER: _ClassVar[int]
     STOPPED_AT_FIELD_NUMBER: _ClassVar[int]
     uuid: str
     stopped_at: _timestamp_pb2.Timestamp
-    def __init__(
-        self,
-        uuid: _Optional[str] = ...,
-        stopped_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
-    ) -> None: ...
+    def __init__(self, uuid: _Optional[str] = ..., stopped_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
```

### Comparing `pytest_initry-0.1.1/pytest_initry/protobufs/test_run_pb2_grpc.py` & `pytest_initry-0.2.0/pytest_initry/protobufs/test_run_pb2_grpc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,124 +1,100 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
+
 import responses_pb2 as responses__pb2
 import test_run_pb2 as test__run__pb2
 
 
 class TestRunServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.CreateTestRun = channel.unary_unary(
-            "/TestRunService/CreateTestRun",
-            request_serializer=test__run__pb2.CreateTestRunRequest.SerializeToString,
-            response_deserializer=responses__pb2.StatusOk.FromString,
-        )
+                '/TestRunService/CreateTestRun',
+                request_serializer=test__run__pb2.CreateTestRunRequest.SerializeToString,
+                response_deserializer=responses__pb2.StatusOk.FromString,
+                )
         self.StopTestRun = channel.unary_unary(
-            "/TestRunService/StopTestRun",
-            request_serializer=test__run__pb2.StopTestRunRequest.SerializeToString,
-            response_deserializer=responses__pb2.StatusOk.FromString,
-        )
+                '/TestRunService/StopTestRun',
+                request_serializer=test__run__pb2.StopTestRunRequest.SerializeToString,
+                response_deserializer=responses__pb2.StatusOk.FromString,
+                )
 
 
 class TestRunServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def CreateTestRun(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def StopTestRun(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
 
 def add_TestRunServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "CreateTestRun": grpc.unary_unary_rpc_method_handler(
-            servicer.CreateTestRun,
-            request_deserializer=test__run__pb2.CreateTestRunRequest.FromString,
-            response_serializer=responses__pb2.StatusOk.SerializeToString,
-        ),
-        "StopTestRun": grpc.unary_unary_rpc_method_handler(
-            servicer.StopTestRun,
-            request_deserializer=test__run__pb2.StopTestRunRequest.FromString,
-            response_serializer=responses__pb2.StatusOk.SerializeToString,
-        ),
+            'CreateTestRun': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateTestRun,
+                    request_deserializer=test__run__pb2.CreateTestRunRequest.FromString,
+                    response_serializer=responses__pb2.StatusOk.SerializeToString,
+            ),
+            'StopTestRun': grpc.unary_unary_rpc_method_handler(
+                    servicer.StopTestRun,
+                    request_deserializer=test__run__pb2.StopTestRunRequest.FromString,
+                    response_serializer=responses__pb2.StatusOk.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "TestRunService", rpc_method_handlers
-    )
+            'TestRunService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
-# This class is part of an EXPERIMENTAL API.
+ # This class is part of an EXPERIMENTAL API.
 class TestRunService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def CreateTestRun(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def CreateTestRun(request,
             target,
-            "/TestRunService/CreateTestRun",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/TestRunService/CreateTestRun',
             test__run__pb2.CreateTestRunRequest.SerializeToString,
             responses__pb2.StatusOk.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def StopTestRun(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def StopTestRun(request,
             target,
-            "/TestRunService/StopTestRun",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/TestRunService/StopTestRun',
             test__run__pb2.StopTestRunRequest.SerializeToString,
             responses__pb2.StatusOk.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `pytest_initry-0.1.1/pytest_initry/protobufs/tests_pb2.py` & `pytest_initry-0.2.0/pytest_initry/protobufs/tests_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,31 +3,29 @@
 # source: tests.proto
 # Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 import responses_pb2 as responses__pb2
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x0btests.proto\x1a\x0fresponses.proto"b\n\x04Test\x12\x0e\n\x06nodeid\x18\x01 \x01(\t\x12\x10\n\x08location\x18\x02 \x01(\t\x12\x0c\n\x04uuid\x18\x03 \x01(\t\x12\x15\n\rtest_run_uuid\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t"*\n\x12\x43reateTestsRequest\x12\x14\n\x05tests\x18\x01 \x03(\x0b\x32\x05.Test2=\n\x0cTestsService\x12-\n\x0b\x43reateTests\x12\x13.CreateTestsRequest\x1a\t.StatusOkb\x06proto3'
-)
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0btests.proto\x1a\x0fresponses.proto\"b\n\x04Test\x12\x0e\n\x06nodeid\x18\x01 \x01(\t\x12\x10\n\x08location\x18\x02 \x01(\t\x12\x0c\n\x04uuid\x18\x03 \x01(\t\x12\x15\n\rtest_run_uuid\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\"*\n\x12\x43reateTestsRequest\x12\x14\n\x05tests\x18\x01 \x03(\x0b\x32\x05.Test2=\n\x0cTestsService\x12-\n\x0b\x43reateTests\x12\x13.CreateTestsRequest\x1a\t.StatusOkb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "tests_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tests_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-    DESCRIPTOR._options = None
-    _globals["_TEST"]._serialized_start = 32
-    _globals["_TEST"]._serialized_end = 130
-    _globals["_CREATETESTSREQUEST"]._serialized_start = 132
-    _globals["_CREATETESTSREQUEST"]._serialized_end = 174
-    _globals["_TESTSSERVICE"]._serialized_start = 176
-    _globals["_TESTSSERVICE"]._serialized_end = 237
+  DESCRIPTOR._options = None
+  _globals['_TEST']._serialized_start=32
+  _globals['_TEST']._serialized_end=130
+  _globals['_CREATETESTSREQUEST']._serialized_start=132
+  _globals['_CREATETESTSREQUEST']._serialized_end=174
+  _globals['_TESTSSERVICE']._serialized_start=176
+  _globals['_TESTSSERVICE']._serialized_end=237
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pytest_initry-0.1.1/pytest_initry/protobufs/tests_pb2.pyi` & `pytest_initry-0.2.0/pytest_initry/protobufs/tests_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-from typing import ClassVar as _ClassVar
-from typing import Iterable as _Iterable
-from typing import Mapping as _Mapping
-from typing import Optional as _Optional
-from typing import Union as _Union
-
 import responses_pb2 as _responses_pb2
+from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from google.protobuf.internal import containers as _containers
+from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Test(_message.Message):
     __slots__ = ("nodeid", "location", "uuid", "test_run_uuid", "description")
     NODEID_FIELD_NUMBER: _ClassVar[int]
     LOCATION_FIELD_NUMBER: _ClassVar[int]
@@ -19,23 +14,14 @@
     TEST_RUN_UUID_FIELD_NUMBER: _ClassVar[int]
     DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
     nodeid: str
     location: str
     uuid: str
     test_run_uuid: str
     description: str
-    def __init__(
-        self,
-        nodeid: _Optional[str] = ...,
-        location: _Optional[str] = ...,
-        uuid: _Optional[str] = ...,
-        test_run_uuid: _Optional[str] = ...,
-        description: _Optional[str] = ...,
-    ) -> None: ...
+    def __init__(self, nodeid: _Optional[str] = ..., location: _Optional[str] = ..., uuid: _Optional[str] = ..., test_run_uuid: _Optional[str] = ..., description: _Optional[str] = ...) -> None: ...
 
 class CreateTestsRequest(_message.Message):
     __slots__ = ("tests",)
     TESTS_FIELD_NUMBER: _ClassVar[int]
     tests: _containers.RepeatedCompositeFieldContainer[Test]
-    def __init__(
-        self, tests: _Optional[_Iterable[_Union[Test, _Mapping]]] = ...
-    ) -> None: ...
+    def __init__(self, tests: _Optional[_Iterable[_Union[Test, _Mapping]]] = ...) -> None: ...
```

### Comparing `pytest_initry-0.1.1/pytest_initry/protobufs/tests_pb2_grpc.py` & `pytest_initry-0.2.0/pytest_initry/protobufs/tests_pb2_grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,79 +1,67 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
+
 import responses_pb2 as responses__pb2
 import tests_pb2 as tests__pb2
 
 
 class TestsServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.CreateTests = channel.unary_unary(
-            "/TestsService/CreateTests",
-            request_serializer=tests__pb2.CreateTestsRequest.SerializeToString,
-            response_deserializer=responses__pb2.StatusOk.FromString,
-        )
+                '/TestsService/CreateTests',
+                request_serializer=tests__pb2.CreateTestsRequest.SerializeToString,
+                response_deserializer=responses__pb2.StatusOk.FromString,
+                )
 
 
 class TestsServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def CreateTests(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
 
 def add_TestsServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "CreateTests": grpc.unary_unary_rpc_method_handler(
-            servicer.CreateTests,
-            request_deserializer=tests__pb2.CreateTestsRequest.FromString,
-            response_serializer=responses__pb2.StatusOk.SerializeToString,
-        ),
+            'CreateTests': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateTests,
+                    request_deserializer=tests__pb2.CreateTestsRequest.FromString,
+                    response_serializer=responses__pb2.StatusOk.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "TestsService", rpc_method_handlers
-    )
+            'TestsService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
-# This class is part of an EXPERIMENTAL API.
+ # This class is part of an EXPERIMENTAL API.
 class TestsService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def CreateTests(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def CreateTests(request,
             target,
-            "/TestsService/CreateTests",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/TestsService/CreateTests',
             tests__pb2.CreateTestsRequest.SerializeToString,
             responses__pb2.StatusOk.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `pytest_initry-0.1.1/PKG-INFO` & `pytest_initry-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-initry
-Version: 0.1.1
+Version: 0.2.0
 Summary: Plugin for sending automation test data from Pytest to the initry
 Home-page: https://github.com/initry/pytest-initry
 License: MIT
 Keywords: pytest,initry
 Author: Andrejs Smirnovs
 Author-email: and.inbx@gmail.com
 Requires-Python: >=3.11,<4.0
```


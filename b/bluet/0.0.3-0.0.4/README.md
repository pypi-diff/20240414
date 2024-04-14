# Comparing `tmp/bluet-0.0.3.tar.gz` & `tmp/bluet-0.0.4.tar.gz`

## Comparing `bluet-0.0.3.tar` & `bluet-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 bluet-0.0.3/src/bluet/__about__.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 bluet-0.0.3/src/bluet/__init__.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 bluet-0.0.3/src/bluet/central.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 bluet-0.0.3/src/bluet/peripheral.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 bluet-0.0.3/src/bluet/process.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bluet-0.0.3/src/bluet/process_zephyr.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bluet-0.0.3/src/bluet/py.typed
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 bluet-0.0.3/src/bluet/tester_device.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bluet-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 bluet-0.0.3/tests/test_bumbled_process.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 bluet-0.0.3/tests/test_bumbled_process_for_zephyr.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 bluet-0.0.3/tests/test_bumbled_process_stdout.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 bluet-0.0.3/tests/test_central.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 bluet-0.0.3/tests/test_imports.py
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 bluet-0.0.3/tests/test_peripheral.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bluet-0.0.3/tests/test_tester_device.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 bluet-0.0.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 bluet-0.0.3/LICENSE
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 bluet-0.0.3/README.md
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 bluet-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 bluet-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 bluet-0.0.4/src/bluet/__about__.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 bluet-0.0.4/src/bluet/__init__.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 bluet-0.0.4/src/bluet/central.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 bluet-0.0.4/src/bluet/peripheral.py
+-rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 bluet-0.0.4/src/bluet/process.py
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 bluet-0.0.4/src/bluet/process_zephyr.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bluet-0.0.4/src/bluet/py.typed
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 bluet-0.0.4/src/bluet/tester_device.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bluet-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 bluet-0.0.4/tests/test_bumbled_process.py
+-rw-r--r--   0        0        0     5112 2020-02-02 00:00:00.000000 bluet-0.0.4/tests/test_bumbled_process_for_zephyr.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 bluet-0.0.4/tests/test_bumbled_process_stdout.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 bluet-0.0.4/tests/test_central.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 bluet-0.0.4/tests/test_imports.py
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 bluet-0.0.4/tests/test_peripheral.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bluet-0.0.4/tests/test_tester_device.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 bluet-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 bluet-0.0.4/LICENSE
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 bluet-0.0.4/README.md
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 bluet-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 bluet-0.0.4/PKG-INFO
```

### Comparing `bluet-0.0.3/src/bluet/__about__.py` & `bluet-0.0.4/src/bluet/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
```

### Comparing `bluet-0.0.3/src/bluet/__init__.py` & `bluet-0.0.4/src/bluet/__init__.py`

 * *Files identical despite different names*

### Comparing `bluet-0.0.3/src/bluet/central.py` & `bluet-0.0.4/src/bluet/central.py`

 * *Files identical despite different names*

### Comparing `bluet-0.0.3/src/bluet/peripheral.py` & `bluet-0.0.4/src/bluet/peripheral.py`

 * *Files identical despite different names*

### Comparing `bluet-0.0.3/src/bluet/process.py` & `bluet-0.0.4/src/bluet/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import logging
 from typing import TYPE_CHECKING, Callable
 
 from bumble.controller import Controller
 
 if TYPE_CHECKING:
     from asyncio.subprocess import Process
-    from typing import Awaitable
+    from collections.abc import Awaitable
 
     from bumble.link import LocalLink
     from bumble.transport import Transport
 
 
 class BumbledProcess:
     """A virtual device that contains the application/program under test.
```

### Comparing `bluet-0.0.3/src/bluet/process_zephyr.py` & `bluet-0.0.4/src/bluet/process_zephyr.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,57 +13,71 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import asyncio.subprocess
 import errno
 import os.path
+import socket
 import sys
 from typing import TYPE_CHECKING
 
 from bumble.transport.tcp_server import open_tcp_server_transport
 
 from bluet.process import BumbledProcess
 
 if TYPE_CHECKING:
-    from typing import Awaitable
+    from collections.abc import Awaitable
 
     from bumble.link import LocalLink
     from bumble.transport.common import Transport
 
 
 def _open_transport(*arg) -> Awaitable[Transport]:
     return open_tcp_server_transport(*arg)
 
 
+def _open_transport_with_sock(*arg) -> Awaitable[Transport]:
+    return open_tcp_server_transport(*arg)
+
+
+def _open_sock_with_unused_port() -> socket.socket:
+    sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+    sock.bind(("localhost", 0))  # Pick an unused port.
+    return sock
+
+
 def create_bumbled_process_for_zephyr(
     controller_name: str,
     link: LocalLink,
-    port: int,
+    port: int | None = None,
     zephyr_program: str | None = None,
     extra_program_args: list[str] | None = None,
 ) -> BumbledProcess:
     """Creates a BumbledProcess with a zephyr executable.
 
     This `zephyr` executable is assumed to be built with `native_sim`, which
     compiles in the whole bluetooth software stack EXCLUDING the controller.
     It has a flag '--bt-dev=...' to designate either a TCP server or a USB
     device. This function will make a bumble controller on the TCP server end,
-    and let the zephyr binary act as the TCP client.
+    and let the zephyr binary act as the TCP client. It is more recommended to
+    leave the argument `port` empty so an unused port can be picked, to ease
+    parallelizing tests.
 
     If argument `zephyr_program` is not explicitly given, one will be searched
     for, assuming the pytest command is initiated by `west twister`.
-
-    TODO: remove explicit `port` and use the `socket` library to open a socket
-    with an arbitrary unused port. Pending on
-        https://github.com/google/bumble/pull/435
     """
     if zephyr_program is None:
         zephyr_program = find_zephyr_binary_from_env()
-    transport = _open_transport(f"_:{port}")
+    if port is None:
+        sock = _open_sock_with_unused_port()
+        port = sock.getsockname()[1]
+        transport = _open_transport_with_sock(sock)
+    else:
+        transport = _open_transport(f"_:{port}")
     process = asyncio.create_subprocess_exec(
         zephyr_program,
         f"--bt-dev=127.0.0.1:{port}",
         *(extra_program_args or []),
         stdin=asyncio.subprocess.PIPE,
         stdout=asyncio.subprocess.PIPE,
     )
```

### Comparing `bluet-0.0.3/src/bluet/tester_device.py` & `bluet-0.0.4/src/bluet/tester_device.py`

 * *Files identical despite different names*

### Comparing `bluet-0.0.3/tests/test_bumbled_process.py` & `bluet-0.0.4/tests/test_bumbled_process.py`

 * *Files identical despite different names*

### Comparing `bluet-0.0.3/tests/test_bumbled_process_for_zephyr.py` & `bluet-0.0.4/tests/test_bumbled_process_for_zephyr.py`

 * *Files 20% similar despite different names*

```diff
@@ -79,14 +79,34 @@
     mock_open.assert_called_once_with("_:12345")
     async with process:
         pass
     assert ["fake-command", "--bt-dev=127.0.0.1:12345"] in fake_process.calls, f"Actually: {fake_process.calls!s}"
 
 
 @pytest.mark.asyncio
+async def test_create_bumbled_process_for_zephyr_normal_no_port(fake_process):
+    fake_process.register([fake_process.any()])
+    socks_used = []
+
+    def mock_open_side_effect(sock):
+        socks_used.append(sock)
+        return open_pty_transport("")
+
+    with patch("bluet.process_zephyr._open_transport_with_sock", side_effect=mock_open_side_effect) as mock_open:
+        # Important: no `port` argument is given.
+        process = create_bumbled_process_for_zephyr("test-name", link=LocalLink(), zephyr_program="fake-command")
+    mock_open.assert_called_once()
+    assert len(socks_used) == 1
+    port = socks_used[0].getsockname()[1]
+    async with process:
+        pass
+    assert ["fake-command", f"--bt-dev=127.0.0.1:{port}"] in fake_process.calls, f"Actually: {fake_process.calls!s}"
+
+
+@pytest.mark.asyncio
 async def test_create_bumbled_process_for_zephyr_extra_args(fake_process):
     fake_process.register([fake_process.any()])
     with _patch_open_transport():
         process = create_bumbled_process_for_zephyr(
             "test-name",
             link=LocalLink(),
             port=12345,
```

### Comparing `bluet-0.0.3/tests/test_bumbled_process_stdout.py` & `bluet-0.0.4/tests/test_bumbled_process_stdout.py`

 * *Files identical despite different names*

### Comparing `bluet-0.0.3/tests/test_central.py` & `bluet-0.0.4/tests/test_central.py`

 * *Files identical despite different names*

### Comparing `bluet-0.0.3/tests/test_imports.py` & `bluet-0.0.4/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `bluet-0.0.3/tests/test_peripheral.py` & `bluet-0.0.4/tests/test_peripheral.py`

 * *Files identical despite different names*

### Comparing `bluet-0.0.3/tests/test_tester_device.py` & `bluet-0.0.4/tests/test_tester_device.py`

 * *Files identical despite different names*

### Comparing `bluet-0.0.3/.gitignore` & `bluet-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `bluet-0.0.3/LICENSE` & `bluet-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bluet-0.0.3/README.md` & `bluet-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bluet-0.0.3/pyproject.toml` & `bluet-0.0.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -3,33 +3,32 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "bluet"
 dynamic = ["version"]
 description = "A unit-test library and setup for embedded bluetooth testing."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = "Apache-2.0"
 keywords = ["bluetooth", "ble", "test", "unit-test", "mock"]
 authors = [
   { name = "Cheng Sheng", email = "jeru.sheng@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "bumble",
+  "bumble>=0.0.190",
 ]
 
 [project.urls]
 Issues = "https://github.com/jeru/bluet/issues"
 Source = "https://github.com/jeru/bluet"
 
 [tool.hatch.version]
@@ -51,15 +50,15 @@
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
+python = ["3.9", "3.10", "3.11", "3.12"]
 
 [tool.hatch.envs.types]
 dependencies = [
   "mypy>=1.0.0",
 ]
 [tool.hatch.envs.types.scripts]
 check = "mypy --install-types --non-interactive {args:src/bluet tests}"
```

### Comparing `bluet-0.0.3/PKG-INFO` & `bluet-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.3
 Name: bluet
-Version: 0.0.3
+Version: 0.0.4
 Summary: A unit-test library and setup for embedded bluetooth testing.
 Project-URL: Issues, https://github.com/jeru/bluet/issues
 Project-URL: Source, https://github.com/jeru/bluet
 Author-email: Cheng Sheng <jeru.sheng@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: ble,bluetooth,mock,test,unit-test
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
-Requires-Dist: bumble
+Requires-Python: >=3.9
+Requires-Dist: bumble>=0.0.190
 Description-Content-Type: text/markdown
 
 # bluet
 
 A *unit-test* library and setup for embedded bluetooth testing.
 
 It expects a bluetooth application to be cross-compiled into an executable in a PC to run, and it should only include the bluetooth host but not the controller.
```


# Comparing `tmp/lxns-0.0a2.tar.gz` & `tmp/lxns-0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lxns-0.0a2.tar", last modified: Sun Mar 31 19:21:02 2024, max compression
+gzip compressed data, was "lxns-0.0a3.tar", last modified: Sun Apr 14 15:28:21 2024, max compression
```

## Comparing `lxns-0.0a2.tar` & `lxns-0.0a3.tar`

### file list

```diff
@@ -1,29 +1,37 @@
--rw-r--r--   0        0        0      156 2024-03-31 19:20:20.000000 lxns-0.0a2/.clang-format
--rw-r--r--   0        0        0      717 2024-03-31 19:20:20.000000 lxns-0.0a2/.github/workflows/ci.yaml
--rw-r--r--   0        0        0      178 2024-03-31 19:20:20.000000 lxns-0.0a2/.gitignore
--rw-r--r--   0        0        0      250 2024-03-31 19:20:20.000000 lxns-0.0a2/.readthedocs.yaml
--rw-r--r--   0        0        0     1078 2024-03-31 19:20:20.000000 lxns-0.0a2/LICENSES/MIT.txt
--rw-r--r--   0        0        0    16727 2024-03-31 19:20:20.000000 lxns-0.0a2/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0     1077 2024-03-31 19:20:20.000000 lxns-0.0a2/README.md
--rw-r--r--   0        0        0      333 2024-03-31 19:20:20.000000 lxns-0.0a2/docs/conf.py
--rw-r--r--   0        0        0      374 2024-03-31 19:20:20.000000 lxns-0.0a2/docs/index.rst
--rw-r--r--   0        0        0     2477 2024-03-31 19:20:20.000000 lxns-0.0a2/docs/namespace.rst
--rw-r--r--   0        0        0       92 2024-03-31 19:20:20.000000 lxns-0.0a2/docs/requirements.txt
--rw-r--r--   0        0        0     2191 2024-03-31 19:20:20.000000 lxns-0.0a2/docs/tips_and_tricks.rst
--rw-r--r--   0        0        0      572 2024-03-31 19:20:20.000000 lxns-0.0a2/examples/process_executor.py
--rw-r--r--   0        0        0      757 2024-03-31 19:20:20.000000 lxns-0.0a2/examples/process_executor_asyncio.py
--rw-r--r--   0        0        0      239 2024-03-31 19:20:20.000000 lxns-0.0a2/meson.build
--rw-r--r--   0        0        0      243 2024-03-31 19:20:20.000000 lxns-0.0a2/meson.options
--rw-r--r--   0        0        0      404 2024-03-31 19:20:20.000000 lxns-0.0a2/pyproject.toml
--rw-r--r--   0        0        0      110 2024-03-31 19:20:20.000000 lxns-0.0a2/setup.cfg
--rw-r--r--   0        0        0      110 2024-03-31 19:20:20.000000 lxns-0.0a2/src/lxns/__init__.py
--rw-r--r--   0        0        0      644 2024-03-31 19:20:20.000000 lxns-0.0a2/src/lxns/meson.build
--rw-r--r--   0        0        0     5827 2024-03-31 19:20:20.000000 lxns-0.0a2/src/lxns/namespaces.py
--rw-r--r--   0        0        0     5514 2024-03-31 19:20:20.000000 lxns-0.0a2/src/lxns/os.c
--rw-r--r--   0        0        0      938 2024-03-31 19:20:20.000000 lxns-0.0a2/src/lxns/os.py
--rw-r--r--   0        0        0       90 2024-03-31 19:20:20.000000 lxns-0.0a2/src/meson.build
--rw-r--r--   0        0        0       75 2024-03-31 19:20:20.000000 lxns-0.0a2/test/__init__.py
--rw-r--r--   0        0        0     1492 2024-03-31 19:20:20.000000 lxns-0.0a2/test/test_namespaces.py
--rw-r--r--   0        0        0     5023 2024-03-31 19:20:20.000000 lxns-0.0a2/test/test_os.py
--rw-r--r--   0        0        0     2513 2024-03-31 19:20:20.000000 lxns-0.0a2/tools/run_linters.py
--rw-r--r--   0        0        0    20961 2024-03-31 19:21:02.976203 lxns-0.0a2/PKG-INFO
+-rw-r--r--   0        0        0      156 2024-04-14 15:10:09.000000 lxns-0.0a3/.clang-format
+-rw-r--r--   0        0        0      717 2024-04-14 15:10:09.000000 lxns-0.0a3/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0      140 2024-04-14 15:10:09.000000 lxns-0.0a3/.gitignore
+-rw-r--r--   0        0        0      250 2024-04-14 15:10:09.000000 lxns-0.0a3/.readthedocs.yaml
+-rw-r--r--   0        0        0      614 2024-04-14 15:10:09.000000 lxns-0.0a3/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2024-04-14 15:10:09.000000 lxns-0.0a3/LICENSES/MIT.txt
+-rw-r--r--   0        0        0    16727 2024-04-14 15:10:09.000000 lxns-0.0a3/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     1214 2024-04-14 15:10:09.000000 lxns-0.0a3/README.md
+-rw-r--r--   0        0        0      333 2024-04-14 15:10:09.000000 lxns-0.0a3/docs/conf.py
+-rw-r--r--   0        0        0      384 2024-04-14 15:10:09.000000 lxns-0.0a3/docs/index.rst
+-rw-r--r--   0        0        0      595 2024-04-14 15:10:09.000000 lxns-0.0a3/docs/mount.rst
+-rw-r--r--   0        0        0     2712 2024-04-14 15:10:09.000000 lxns-0.0a3/docs/namespace.rst
+-rw-r--r--   0        0        0       92 2024-04-14 15:10:09.000000 lxns-0.0a3/docs/requirements.txt
+-rw-r--r--   0        0        0     2191 2024-04-14 15:10:09.000000 lxns-0.0a3/docs/tips_and_tricks.rst
+-rw-r--r--   0        0        0     1900 2024-04-14 15:10:09.000000 lxns-0.0a3/examples/add_bind_mount.py
+-rw-r--r--   0        0        0     1033 2024-04-14 15:10:09.000000 lxns-0.0a3/examples/join_all_pid_namespaces.py
+-rw-r--r--   0        0        0      572 2024-04-14 15:10:09.000000 lxns-0.0a3/examples/process_executor.py
+-rw-r--r--   0        0        0      757 2024-04-14 15:10:09.000000 lxns-0.0a3/examples/process_executor_asyncio.py
+-rw-r--r--   0        0        0      239 2024-04-14 15:10:09.000000 lxns-0.0a3/meson.build
+-rw-r--r--   0        0        0      611 2024-04-14 15:10:09.000000 lxns-0.0a3/meson.options
+-rw-r--r--   0        0        0     1215 2024-04-14 15:10:09.000000 lxns-0.0a3/pyproject.toml
+-rw-r--r--   0        0        0      110 2024-04-14 15:10:09.000000 lxns-0.0a3/setup.cfg
+-rw-r--r--   0        0        0      110 2024-04-14 15:10:09.000000 lxns-0.0a3/src/lxns/__init__.py
+-rw-r--r--   0        0        0     1516 2024-04-14 15:10:09.000000 lxns-0.0a3/src/lxns/meson.build
+-rw-r--r--   0        0        0     1958 2024-04-14 15:10:09.000000 lxns-0.0a3/src/lxns/mount.py
+-rw-r--r--   0        0        0     7789 2024-04-14 15:10:09.000000 lxns-0.0a3/src/lxns/namespaces.py
+-rw-r--r--   0        0        0     8753 2024-04-14 15:10:09.000000 lxns-0.0a3/src/lxns/os.c
+-rw-r--r--   0        0        0     1556 2024-04-14 15:10:09.000000 lxns-0.0a3/src/lxns/os.py
+-rw-r--r--   0        0        0       90 2024-04-14 15:10:09.000000 lxns-0.0a3/src/meson.build
+-rw-r--r--   0        0        0       75 2024-04-14 15:10:09.000000 lxns-0.0a3/test/__init__.py
+-rw-r--r--   0        0        0      493 2024-04-14 15:10:09.000000 lxns-0.0a3/test/check_typing.py
+-rw-r--r--   0        0        0     1101 2024-04-14 15:10:09.000000 lxns-0.0a3/test/test_mount.py
+-rw-r--r--   0        0        0     1921 2024-04-14 15:10:09.000000 lxns-0.0a3/test/test_namespaces.py
+-rw-r--r--   0        0        0     5958 2024-04-14 15:10:09.000000 lxns-0.0a3/test/test_os.py
+-rw-r--r--   0        0        0     4214 2024-04-14 15:10:09.000000 lxns-0.0a3/tools/build_in_container.py
+-rw-r--r--   0        0        0     2513 2024-04-14 15:10:09.000000 lxns-0.0a3/tools/run_linters.py
+-rw-r--r--   0        0        0     2259 2024-04-14 15:28:21.913429 lxns-0.0a3/PKG-INFO
```

### Comparing `lxns-0.0a2/.github/workflows/ci.yaml` & `lxns-0.0a3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `lxns-0.0a2/LICENSES/MIT.txt` & `lxns-0.0a3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `lxns-0.0a2/LICENSES/MPL-2.0.txt` & `lxns-0.0a3/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `lxns-0.0a2/README.md` & `lxns-0.0a3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 
 * Linux namespaces class abstractions with automatic resource control.
     * Opening existing namespaces using PIDs.
     * Opening parent user namespaces. (usually unaccessible from `/proc`)
     * Switching to a namespace.
     * Unsharing namespaces either from class method or function with boolean flags.
     * Automatic file descriptor resource control using `with`.
+    * Getting and setting the max number of namespaces.
+* Mount utilities using new file descriptor based API.
+    * Create bind mounts.
 
 ## [Documentation](https://python-lxns.readthedocs.io/en/latest/)
 
 ## Requirements
 
 ### Compiling source package
```

### Comparing `lxns-0.0a2/docs/namespace.rst` & `lxns-0.0a3/docs/namespace.rst`

 * *Files 17% similar despite different names*

```diff
@@ -9,67 +9,74 @@
 Namespace is an isolation mechanism. In total there are 7 different
 namespace types each representing a certain operating system domain.
 
 For example, :py:class:`MountNamespace` allows to creating new mount
 points without affecting other processes.
 
 Namespace classes should not be initialized directly. Instead either
-:py:meth:`UserNamespace.from_pid` or :py:meth:`UserNamespace.from_self`
+:py:meth:`BaseNamespace.from_pid` or :py:meth:`BaseNamespace.from_self`
 class methods should be used to create a namespace object which represents
 a reference to an existing namespace.
 
-An existing namespace can be entered using :py:meth:`UserNamespace.setns`.
-A new namespace can be created using :py:meth:`UserNamespace.unshare`
+An existing namespace can be entered using :py:meth:`BaseNamespace.setns`.
+A new namespace can be created using :py:meth:`BaseNamespace.unshare`
 class method or :py:meth:`unshare_namespaces` function.
 
 File descriptors are a limited resource and every namespace reference
 requires one. Because of this a warning will be emitted if a namespace
 object was deallocated without closing the file descriptor. To avoid this
-use :py:meth:`UserNamespace.close` or a ``with`` block. For example::
+use :py:meth:`BaseNamespace.close` or a ``with`` block. For example::
 
     from lxns.namespaces import UserNamespace
 
     with UserNamespace.from_pid(123456) as user_ns:
         user_ns.setns()
 
     # Inside the user namespace
 
 Namespace object cannot be used after it was closed and all methods will
 raise ``ValueError``.
 
 All namespace classes implement similar API and only differ in the type
-of namespace they reference. For brevity only :py:class:`UserNamespace`
+of namespace they reference. For brevity only :py:class:`BaseNamespace`
 has the methods documented.
 
+.. autoclass:: lxns.namespaces.BaseNamespace
+    :members: __init__, fileno, setns, get_user_namespace, close, from_pid, from_self,
+              get_current_ns_id, unshare, ns_id, get_current_limit, set_current_limit
+
 .. autoclass:: lxns.namespaces.UserNamespace
-    :members: setns, get_userns, close, from_pid, from_self, get_current_ns_id,
-              unshare, ns_id
+
+    Implements same API as :py:class:`BaseNamespace`.
 
 .. autoclass:: lxns.namespaces.MountNamespace
 
-    Implements same API as :py:class:`UserNamespace`.
+    Implements same API as :py:class:`BaseNamespace`.
 
 .. autoclass:: lxns.namespaces.NetworkNamespace
 
-    Implements same API as :py:class:`UserNamespace`.
+    Implements same API as :py:class:`BaseNamespace`.
 
 .. autoclass:: lxns.namespaces.IpcNamespace
 
-    Implements same API as :py:class:`UserNamespace`.
+    Implements same API as :py:class:`BaseNamespace`.
 
 .. autoclass:: lxns.namespaces.CgroupNamespace
 
-    Implements same API as :py:class:`UserNamespace`.
+    Implements same API as :py:class:`BaseNamespace`.
 
 .. autoclass:: lxns.namespaces.PidNamespace
 
-    Implements same API as :py:class:`UserNamespace`.
+    Implements same API as :py:class:`BaseNamespace`.
 
 .. autoclass:: lxns.namespaces.TimeNamespace
 
-    Implements same API as :py:class:`UserNamespace`.
+    Implements same API as :py:class:`BaseNamespace`.
 
 .. autoclass:: lxns.namespaces.UtsNamespace
 
-    Implements same API as :py:class:`UserNamespace`.
+    Implements same API as :py:class:`BaseNamespace`.
+
+.. autodata:: lxns.namespaces.ALL_NAMESPACE_CLASSES
+    :annotation:
 
 .. autofunction:: lxns.namespaces.unshare_namespaces
```

### Comparing `lxns-0.0a2/docs/tips_and_tricks.rst` & `lxns-0.0a3/docs/tips_and_tricks.rst`

 * *Files identical despite different names*

### Comparing `lxns-0.0a2/examples/process_executor.py` & `lxns-0.0a3/examples/process_executor.py`

 * *Files identical despite different names*

### Comparing `lxns-0.0a2/examples/process_executor_asyncio.py` & `lxns-0.0a3/examples/process_executor_asyncio.py`

 * *Files identical despite different names*

### Comparing `lxns-0.0a2/src/lxns/namespaces.py` & `lxns-0.0a3/src/lxns/namespaces.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     CLONE_NEWIPC,
     CLONE_NEWNET,
     CLONE_NEWNS,
     CLONE_NEWPID,
     CLONE_NEWTIME,
     CLONE_NEWUSER,
     CLONE_NEWUTS,
+    ns_get_nstype,
     ns_get_userns,
     setns,
 )
 from .os import unshare as _unshare
 
 if TYPE_CHECKING:
     from typing import Any, ClassVar, Literal, TypeVar
@@ -34,39 +35,64 @@
 class BaseNamespace:
     """Base namespace class for all namespaces.
 
     Should not be used directly.
     """
 
     NAMESPACE_CONSTANT: ClassVar[int] = -1
-    NAMESPACE_PROC_NAME: ClassVar[str] = ""
-    _fd: int | None
+    NAMESPACE_PROC_NAME: ClassVar[str] = "\0"
 
-    def __init__(self, *args: Any, **kwargs: Any):
-        self._fd = None
-        raise NotImplementedError(
-            "Please use one of the 'from' methods to initialize namespace."
-        )
+    def __init__(self, fd: int, closefd: bool = True):
+        """Wrap existing file descriptor in a Namespace object.
+
+        It is recommended to use the :py:meth:`BaseNamespace.from_pid` or
+        :py:meth:`BaseNamespace.from_pid` methods over manually opening the
+        namespace files.
+
+        :param int fd: File descriptor that references the namespace.
+        :param bool closefd: Close underlying file descriptor or not.
+        """
+        self._fd: int | None = None
+        self._closefd = closefd
+        if ns_get_nstype(fd) != self.NAMESPACE_CONSTANT:
+            raise ValueError(
+                f"File descriptor {fd!r} does not reference "
+                f"the {self.__class__.__name__} namespace."
+            )
+
+        # Only reference the file descriptor after it passed the check
+        self._fd = fd
 
     def __del__(self) -> None:
-        if self._fd is not None:
+        if self._fd is not None and self._closefd:
             warn(f"unclosed namespace {self}", ResourceWarning)
             self.close()
 
+    def fileno(self) -> int:
+        """Return namespace underlying file descriptor.
+
+        :raises ValueError: Namespace was already closed.
+        """
+        fd = self._fd
+        if fd is not None:
+            return fd
+        else:
+            raise ValueError("Namespace file descriptor is already closed.")
+
     def setns(self: Self) -> None:
         """Enter namespace.
 
         :raises OSError: Errors returned by the syscall.
         """
         if self._fd is None:
             raise ValueError("Trying switch to closed namespace.")
 
         setns(self._fd, self.NAMESPACE_CONSTANT)
 
-    def get_userns(self: Self) -> UserNamespace:
+    def get_user_namespace(self: Self) -> UserNamespace:
         """Open user namespace that owns this namespace.
 
         :return: User namespace.
         :rtype: :py:class:`UserNamespace`
         """
         if self._fd is None:
             raise ValueError("Namespace closed. Cannot get user namespace.")
@@ -76,32 +102,31 @@
     def close(self: Self) -> None:
         """Close namespace file descriptor.
 
         Can be called multiple times in which case only first call
         will close the namespace and subsequent calls will be ignored.
         """
         if self._fd is not None:
-            close_fd(self._fd)
+            if self._closefd:
+                close_fd(self._fd)
             self._fd = None
 
     def __enter__(self: Self) -> Self:
         return self
 
     def __exit__(self: Self, *args: Any, **kwargs: Any) -> None:
         self.close()
 
     @classmethod
     def from_pid(cls: type[Self], pid: int | Literal["self"]) -> Self:
         """Open namespace from a process id."""
         ns_fd = open_fd(
             f"/proc/{pid}/ns/{cls.NAMESPACE_PROC_NAME}", O_RDONLY | O_CLOEXEC
         )
-        new_instance = cls.__new__(cls)
-        new_instance._fd = ns_fd
-        return new_instance
+        return cls(ns_fd)
 
     @classmethod
     def from_self(cls: type[Self]) -> Self:
         """Open caller current namespace."""
         return cls.from_pid("self")
 
     @classmethod
@@ -129,14 +154,36 @@
         try:
             ns_id = str(self.ns_id)
         except ValueError:
             ns_id = "closed"
 
         return f"<{self.__class__.__name__} id={ns_id}>"
 
+    @classmethod
+    def get_current_limit(cls) -> int:
+        """Get the current limit for this type of namespace.
+
+        The limits are unique per user namespace and are propagated to the child
+        namespaces.
+        """
+        with open(f"/proc/sys/user/max_{cls.NAMESPACE_PROC_NAME}_namespaces") as f:
+            return int(f.read())
+
+    @classmethod
+    def set_current_limit(cls, new_limit: int) -> None:
+        """Set the current limit for this type of namespace.
+
+        The limits are unique per user namespace and are propagated to the child
+        namespaces.
+        """
+        with open(
+            f"/proc/sys/user/max_{cls.NAMESPACE_PROC_NAME}_namespaces", mode="w"
+        ) as f:
+            f.write(str(new_limit))
+
 
 class CgroupNamespace(BaseNamespace):
     """Cgroups namespace."""
 
     NAMESPACE_CONSTANT = CLONE_NEWCGROUP
     NAMESPACE_PROC_NAME = "cgroup"
 
@@ -229,14 +276,28 @@
 
     if uts:
         flags |= CLONE_NEWUTS
 
     _unshare(flags)
 
 
+ALL_NAMESPACE_CLASSES = (
+    UserNamespace,
+    CgroupNamespace,
+    IpcNamespace,
+    NetworkNamespace,
+    MountNamespace,
+    PidNamespace,
+    TimeNamespace,
+    UserNamespace,
+    UtsNamespace,
+)
+"""All Namespace classes arranged in order suited for joining."""
+
+
 __all__ = (
     "CgroupNamespace",
     "IpcNamespace",
     "NetworkNamespace",
     "MountNamespace",
     "PidNamespace",
     "TimeNamespace",
```

### Comparing `lxns-0.0a2/test/test_namespaces.py` & `lxns-0.0a3/test/test_namespaces.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,7 +39,19 @@
         with ProcessPoolExecutor() as executor:
             uid_before, uid_after = executor.submit(
                 self.unshare_from_class_test
             ).result(3)
 
         self.assertEqual(uid_now, uid_before)
         self.assertNotEqual(uid_now, uid_after)
+
+    @staticmethod
+    def namespaces_limits_test() -> int:
+        UserNamespace.unshare()
+        UserNamespace.set_current_limit(0)
+        return UserNamespace.get_current_limit()
+
+    def test_namespace_limits(self) -> None:
+        self.assertLess(0, UserNamespace.get_current_limit())
+
+        with ProcessPoolExecutor() as executor:
+            self.assertEqual(executor.submit(self.namespaces_limits_test).result(3), 0)
```

### Comparing `lxns-0.0a2/test/test_os.py` & `lxns-0.0a3/test/test_os.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 # SPDX-License-Identifier: MPL-2.0
 # SPDX-FileCopyrightText: 2024 igo95862
 from __future__ import annotations
 
 from concurrent.futures import ProcessPoolExecutor
 from os import fstat, getpid, getuid, stat
-from tempfile import TemporaryFile
+from pathlib import Path
+from tempfile import TemporaryDirectory, TemporaryFile
 from unittest import TestCase
 
 from lxns.os import (
+    CLONE_NEWNS,
     CLONE_NEWUSER,
+    MOVE_MOUNT_F_EMPTY_PATH,
+    OPEN_TREE_CLONE,
+    move_mount,
     ns_get_nstype,
     ns_get_owner_uid,
     ns_get_parent,
     ns_get_userns,
+    open_tree,
     setns,
     unshare,
 )
 
 NAMESPACES_FILE = "/proc/{pid}/ns/{namespace}"
 NAMESPACES_NAMES = (
     "cgroup",
@@ -158,7 +164,27 @@
                     current_ns_id,
                 )
 
                 self.assertEqual(
                     fstat(child_userns_owner_userns_file.fileno()).st_ino,
                     current_ns_id,
                 )
+
+    @staticmethod
+    def _open_tree_test(foo_file: Path, bar_file: Path) -> str:
+        unshare(CLONE_NEWUSER | CLONE_NEWNS)
+        tree_fd = open_tree(path=str(foo_file), flags=OPEN_TREE_CLONE)
+        move_mount(tree_fd, to_path=str(bar_file), flags=MOVE_MOUNT_F_EMPTY_PATH)
+        return bar_file.read_text()
+
+    def test_open_tree(self) -> None:
+        with ProcessPoolExecutor() as executor, TemporaryDirectory() as tmpdir:
+            tmpdir_path = Path(tmpdir)
+            foo_file = tmpdir_path / "foo"
+            foo_file.write_text("foo")
+            bar_file = tmpdir_path / "bar"
+            bar_file.write_text("bar")
+
+            self.assertEqual(
+                executor.submit(self._open_tree_test, foo_file, bar_file).result(3),
+                "foo",
+            )
```

### Comparing `lxns-0.0a2/tools/run_linters.py` & `lxns-0.0a3/tools/run_linters.py`

 * *Files identical despite different names*


# Comparing `tmp/accesskit-0.1.8.tar.gz` & `tmp/accesskit-0.2.0.tar.gz`

## Comparing `accesskit-0.1.8.tar` & `accesskit-0.2.0.tar`

### file list

```diff
@@ -1,96 +1,95 @@
--rw-r--r--   0     1001      127      407 2024-03-18 01:10:28.000000 accesskit-0.1.8/consumer/Cargo.toml
--rw-r--r--   0     1001      127    15592 2024-03-18 01:10:28.000000 accesskit-0.1.8/consumer/CHANGELOG.md
--rw-r--r--   0     1001      127      207 2024-03-18 01:10:28.000000 accesskit-0.1.8/consumer/README.md
--rw-r--r--   0     1001      127     1262 2024-03-18 01:10:28.000000 accesskit-0.1.8/consumer/src/filters.rs
--rw-r--r--   0     1001      127    24021 2024-03-18 01:10:28.000000 accesskit-0.1.8/consumer/src/iterators.rs
--rw-r--r--   0     1001      127     6371 2024-03-18 01:10:28.000000 accesskit-0.1.8/consumer/src/lib.rs
--rw-r--r--   0     1001      127    33855 2024-03-18 01:10:28.000000 accesskit-0.1.8/consumer/src/node.rs
--rw-r--r--   0     1001      127    64603 2024-03-18 01:10:28.000000 accesskit-0.1.8/consumer/src/text.rs
--rw-r--r--   0     1001      127    27230 2024-03-18 01:10:28.000000 accesskit-0.1.8/consumer/src/tree.rs
--rw-r--r--   0     1001      127      669 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/atspi-common/Cargo.toml
--rw-r--r--   0     1001      127     1126 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/atspi-common/CHANGELOG.md
--rw-r--r--   0     1001      127      317 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/atspi-common/README.md
--rw-r--r--   0     1001      127      432 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/atspi-common/src/action.rs
--rw-r--r--   0     1001      127    11296 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/atspi-common/src/adapter.rs
--rw-r--r--   0     1001      127      583 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/atspi-common/src/callback.rs
--rw-r--r--   0     1001      127     2713 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/atspi-common/src/context.rs
--rw-r--r--   0     1001      127      541 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/atspi-common/src/error.rs
--rw-r--r--   0     1001      127     1036 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/atspi-common/src/events.rs
--rw-r--r--   0     1001      127      334 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/atspi-common/src/filters.rs
--rw-r--r--   0     1001      127      708 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/atspi-common/src/lib.rs
--rw-r--r--   0     1001      127    39237 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/atspi-common/src/node.rs
--rw-r--r--   0     1001      127      898 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/atspi-common/src/rect.rs
--rw-r--r--   0     1001      127    13107 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/atspi-common/src/simplified.rs
--rw-r--r--   0     1001      127     1157 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/atspi-common/src/util.rs
--rw-r--r--   0     1001      127     1315 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/unix/Cargo.toml
--rw-r--r--   0     1001      127     9883 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/unix/CHANGELOG.md
--rw-r--r--   0     1001      127      487 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/unix/README.md
--rw-r--r--   0     1001      127     5292 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/unix/src/adapter.rs
--rw-r--r--   0     1001      127    13572 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/unix/src/atspi/bus.rs
--rw-r--r--   0     1001      127     6053 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/unix/src/atspi/interfaces/accessible.rs
--rw-r--r--   0     1001      127     1473 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/unix/src/atspi/interfaces/action.rs
--rw-r--r--   0     1001      127     1096 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/unix/src/atspi/interfaces/application.rs
--rw-r--r--   0     1001      127     2195 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/unix/src/atspi/interfaces/component.rs
--rw-r--r--   0     1001      127      945 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/unix/src/atspi/interfaces/mod.rs
--rw-r--r--   0     1001      127     1459 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/unix/src/atspi/interfaces/value.rs
--rw-r--r--   0     1001      127      404 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/unix/src/atspi/mod.rs
--rw-r--r--   0     1001      127     1224 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/unix/src/atspi/object_address.rs
--rw-r--r--   0     1001      127     2185 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/unix/src/atspi/object_id.rs
--rw-r--r--   0     1001      127     5439 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/unix/src/context.rs
--rw-r--r--   0     1001      127     4885 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/unix/src/executor.rs
--rw-r--r--   0     1001      127     1005 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/unix/src/lib.rs
--rw-r--r--   0     1001      127     1389 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/unix/src/util.rs
--rw-r--r--   0     1001      127      956 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/windows/Cargo.toml
--rw-r--r--   0     1001      127    22489 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/windows/CHANGELOG.md
--rw-r--r--   0     1001      127      172 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/windows/README.md
--rw-r--r--   0     1001      127    12704 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/windows/examples/hello_world.rs
--rw-r--r--   0     1001      127    10999 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/windows/src/adapter.rs
--rw-r--r--   0     1001      127     1220 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/windows/src/context.rs
--rw-r--r--   0     1001      127      403 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/windows/src/filters.rs
--rw-r--r--   0     1001      127     1474 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/windows/src/init.rs
--rw-r--r--   0     1001      127      522 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/windows/src/lib.rs
--rw-r--r--   0     1001      127    37364 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/windows/src/node.rs
--rw-r--r--   0     1001      127     6343 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/windows/src/subclass.rs
--rw-r--r--   0     1001      127    11734 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/windows/src/tests/mod.rs
--rw-r--r--   0     1001      127     6861 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/windows/src/tests/simple.rs
--rw-r--r--   0     1001      127     2968 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/windows/src/tests/subclassed.rs
--rw-r--r--   0     1001      127    19705 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/windows/src/text.rs
--rw-r--r--   0     1001      127     6500 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/windows/src/util.rs
--rw-r--r--   0     1001      127      885 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/macos/Cargo.toml
--rw-r--r--   0     1001      127    12625 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/macos/CHANGELOG.md
--rw-r--r--   0     1001      127      183 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/macos/README.md
--rw-r--r--   0     1001      127     4173 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/macos/src/adapter.rs
--rw-r--r--   0     1001      127     2281 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/macos/src/context.rs
--rw-r--r--   0     1001      127     8878 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/macos/src/event.rs
--rw-r--r--   0     1001      127      334 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/macos/src/filters.rs
--rw-r--r--   0     1001      127      559 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/macos/src/lib.rs
--rw-r--r--   0     1001      127    33032 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/macos/src/node.rs
--rw-r--r--   0     1001      127     3147 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/macos/src/patch.rs
--rw-r--r--   0     1001      127     9591 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/macos/src/subclass.rs
--rw-r--r--   0     1001      127     2878 2024-03-18 01:10:28.000000 accesskit-0.1.8/platforms/macos/src/util.rs
--rw-r--r--   0     1001      127      704 2024-03-18 01:10:28.000000 accesskit-0.1.8/common/Cargo.toml
--rw-r--r--   0     1001      127    12626 2024-03-18 01:10:28.000000 accesskit-0.1.8/common/CHANGELOG.md
--rw-r--r--   0     1001      127      740 2024-03-18 01:10:28.000000 accesskit-0.1.8/common/README.md
--rw-r--r--   0     1001      127    22792 2024-03-18 01:10:28.000000 accesskit-0.1.8/common/src/geometry.rs
--rw-r--r--   0     1001      127    79188 2024-03-18 01:10:28.000000 accesskit-0.1.8/common/src/lib.rs
--rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 accesskit-0.1.8/bindings/python/Cargo.toml
--rw-r--r--   0     1001      127      224 2024-03-18 01:10:28.000000 accesskit-0.1.8/bindings/python/.cargo/config.toml
--rw-r--r--   0     1001      127     1918 2024-03-18 01:10:28.000000 accesskit-0.1.8/bindings/python/CHANGELOG.md
--rw-r--r--   0     1001      127      981 2024-03-18 01:10:28.000000 accesskit-0.1.8/bindings/python/README.md
--rw-r--r--   0     1001      127     3078 2024-03-18 01:10:28.000000 accesskit-0.1.8/bindings/python/examples/pygame/.gitignore
--rw-r--r--   0     1001      127      367 2024-03-18 01:10:28.000000 accesskit-0.1.8/bindings/python/examples/pygame/README.md
--rw-r--r--   0     1001      127     6830 2024-03-18 01:10:28.000000 accesskit-0.1.8/bindings/python/examples/pygame/hello_world.py
--rw-r--r--   0     1001      127       24 2024-03-18 01:10:28.000000 accesskit-0.1.8/bindings/python/examples/pygame/requirements.txt
--rw-r--r--   0     1001      127    23523 2024-03-18 01:10:28.000000 accesskit-0.1.8/bindings/python/src/common.rs
--rw-r--r--   0     1001      127     4784 2024-03-18 01:10:28.000000 accesskit-0.1.8/bindings/python/src/geometry.rs
--rw-r--r--   0     1001      127     2917 2024-03-18 01:10:28.000000 accesskit-0.1.8/bindings/python/src/lib.rs
--rw-r--r--   0     1001      127     6901 2024-03-18 01:10:28.000000 accesskit-0.1.8/bindings/python/src/macos.rs
--rw-r--r--   0     1001      127     1450 2024-03-18 01:10:28.000000 accesskit-0.1.8/bindings/python/src/unix.rs
--rw-r--r--   0     1001      127     4450 2024-03-18 01:10:28.000000 accesskit-0.1.8/bindings/python/src/windows.rs
--rw-r--r--   0     1001      127    72633 2024-03-18 01:10:28.000000 accesskit-0.1.8/Cargo.lock
--rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 accesskit-0.1.8/Cargo.toml
--rw-r--r--   0     1001      127     1043 2024-03-18 01:10:28.000000 accesskit-0.1.8/pyproject.toml
--rw-r--r--   0     1001      127     9723 2024-03-18 01:10:28.000000 accesskit-0.1.8/LICENSE-APACHE
--rw-r--r--   0     1001      127     1023 2024-03-18 01:10:28.000000 accesskit-0.1.8/LICENSE-MIT
--rw-r--r--   0     1001      127     1559 2024-03-18 01:10:28.000000 accesskit-0.1.8/LICENSE.chromium
--rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 accesskit-0.1.8/PKG-INFO
+-rw-r--r--   0     1001      127      885 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/Cargo.toml
+-rw-r--r--   0     1001      127    13501 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/CHANGELOG.md
+-rw-r--r--   0     1001      127      183 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/README.md
+-rw-r--r--   0     1001      127     9664 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/src/adapter.rs
+-rw-r--r--   0     1001      127     2724 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/src/context.rs
+-rw-r--r--   0     1001      127     9005 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/src/event.rs
+-rw-r--r--   0     1001      127      334 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/src/filters.rs
+-rw-r--r--   0     1001      127      559 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/src/lib.rs
+-rw-r--r--   0     1001      127    33032 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/src/node.rs
+-rw-r--r--   0     1001      127     3147 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/src/patch.rs
+-rw-r--r--   0     1001      127     9525 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/src/subclass.rs
+-rw-r--r--   0     1001      127     2878 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/src/util.rs
+-rw-r--r--   0     1001      127      669 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/Cargo.toml
+-rw-r--r--   0     1001      127     1796 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/CHANGELOG.md
+-rw-r--r--   0     1001      127      317 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/README.md
+-rw-r--r--   0     1001      127      432 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/action.rs
+-rw-r--r--   0     1001      127    12747 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/adapter.rs
+-rw-r--r--   0     1001      127      583 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/callback.rs
+-rw-r--r--   0     1001      127     3414 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/context.rs
+-rw-r--r--   0     1001      127      541 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/error.rs
+-rw-r--r--   0     1001      127     1036 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/events.rs
+-rw-r--r--   0     1001      127      334 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/filters.rs
+-rw-r--r--   0     1001      127      753 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/lib.rs
+-rw-r--r--   0     1001      127    39237 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/node.rs
+-rw-r--r--   0     1001      127      898 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/rect.rs
+-rw-r--r--   0     1001      127    13107 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/simplified.rs
+-rw-r--r--   0     1001      127     1157 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/util.rs
+-rw-r--r--   0     1001      127      407 2024-04-14 17:20:57.000000 accesskit-0.2.0/consumer/Cargo.toml
+-rw-r--r--   0     1001      127    16203 2024-04-14 17:20:57.000000 accesskit-0.2.0/consumer/CHANGELOG.md
+-rw-r--r--   0     1001      127      207 2024-04-14 17:20:57.000000 accesskit-0.2.0/consumer/README.md
+-rw-r--r--   0     1001      127     1262 2024-04-14 17:20:57.000000 accesskit-0.2.0/consumer/src/filters.rs
+-rw-r--r--   0     1001      127    24021 2024-04-14 17:20:57.000000 accesskit-0.2.0/consumer/src/iterators.rs
+-rw-r--r--   0     1001      127     6371 2024-04-14 17:20:57.000000 accesskit-0.2.0/consumer/src/lib.rs
+-rw-r--r--   0     1001      127    33855 2024-04-14 17:20:57.000000 accesskit-0.2.0/consumer/src/node.rs
+-rw-r--r--   0     1001      127    64603 2024-04-14 17:20:57.000000 accesskit-0.2.0/consumer/src/text.rs
+-rw-r--r--   0     1001      127    27310 2024-04-14 17:20:57.000000 accesskit-0.2.0/consumer/src/tree.rs
+-rw-r--r--   0     1001      127      704 2024-04-14 17:20:57.000000 accesskit-0.2.0/common/Cargo.toml
+-rw-r--r--   0     1001      127    13085 2024-04-14 17:20:57.000000 accesskit-0.2.0/common/CHANGELOG.md
+-rw-r--r--   0     1001      127      740 2024-04-14 17:20:57.000000 accesskit-0.2.0/common/README.md
+-rw-r--r--   0     1001      127    22792 2024-04-14 17:20:57.000000 accesskit-0.2.0/common/src/geometry.rs
+-rw-r--r--   0     1001      127    81176 2024-04-14 17:20:57.000000 accesskit-0.2.0/common/src/lib.rs
+-rw-r--r--   0     1001      127     1315 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/Cargo.toml
+-rw-r--r--   0     1001      127    10539 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/CHANGELOG.md
+-rw-r--r--   0     1001      127      487 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/README.md
+-rw-r--r--   0     1001      127     6935 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/adapter.rs
+-rw-r--r--   0     1001      127    13572 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/atspi/bus.rs
+-rw-r--r--   0     1001      127     6053 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/atspi/interfaces/accessible.rs
+-rw-r--r--   0     1001      127     1473 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/atspi/interfaces/action.rs
+-rw-r--r--   0     1001      127     1096 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/atspi/interfaces/application.rs
+-rw-r--r--   0     1001      127     2195 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/atspi/interfaces/component.rs
+-rw-r--r--   0     1001      127      945 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/atspi/interfaces/mod.rs
+-rw-r--r--   0     1001      127     1459 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/atspi/interfaces/value.rs
+-rw-r--r--   0     1001      127      404 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/atspi/mod.rs
+-rw-r--r--   0     1001      127     1224 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/atspi/object_address.rs
+-rw-r--r--   0     1001      127     2185 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/atspi/object_id.rs
+-rw-r--r--   0     1001      127     8069 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/context.rs
+-rw-r--r--   0     1001      127     4885 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/executor.rs
+-rw-r--r--   0     1001      127     1005 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/lib.rs
+-rw-r--r--   0     1001      127     1389 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/util.rs
+-rw-r--r--   0     1001      127      955 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/Cargo.toml
+-rw-r--r--   0     1001      127    23152 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/CHANGELOG.md
+-rw-r--r--   0     1001      127      172 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/README.md
+-rw-r--r--   0     1001      127    11956 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/examples/hello_world.rs
+-rw-r--r--   0     1001      127    16625 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/adapter.rs
+-rw-r--r--   0     1001      127     1696 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/context.rs
+-rw-r--r--   0     1001      127      403 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/filters.rs
+-rw-r--r--   0     1001      127      482 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/lib.rs
+-rw-r--r--   0     1001      127    37364 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/node.rs
+-rw-r--r--   0     1001      127     6179 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/subclass.rs
+-rw-r--r--   0     1001      127    11438 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/tests/mod.rs
+-rw-r--r--   0     1001      127     7069 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/tests/simple.rs
+-rw-r--r--   0     1001      127     3178 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/tests/subclassed.rs
+-rw-r--r--   0     1001      127    19705 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/text.rs
+-rw-r--r--   0     1001      127     6500 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/util.rs
+-rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 accesskit-0.2.0/bindings/python/Cargo.toml
+-rw-r--r--   0     1001      127      224 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/.cargo/config.toml
+-rw-r--r--   0     1001      127     2674 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/CHANGELOG.md
+-rw-r--r--   0     1001      127      981 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/README.md
+-rw-r--r--   0     1001      127     3078 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/examples/pygame/.gitignore
+-rw-r--r--   0     1001      127      367 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/examples/pygame/README.md
+-rw-r--r--   0     1001      127     7179 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/examples/pygame/hello_world.py
+-rw-r--r--   0     1001      127       24 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/examples/pygame/requirements.txt
+-rw-r--r--   0     1001      127    24683 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/src/common.rs
+-rw-r--r--   0     1001      127     4784 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/src/geometry.rs
+-rw-r--r--   0     1001      127     2854 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/src/lib.rs
+-rw-r--r--   0     1001      127     7316 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/src/macos.rs
+-rw-r--r--   0     1001      127     1506 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/src/unix.rs
+-rw-r--r--   0     1001      127     4126 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/src/windows.rs
+-rw-r--r--   0     1001      127    72633 2024-04-14 17:20:57.000000 accesskit-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 accesskit-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      127     1043 2024-04-14 17:20:57.000000 accesskit-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      127     9723 2024-04-14 17:20:57.000000 accesskit-0.2.0/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1023 2024-04-14 17:20:57.000000 accesskit-0.2.0/LICENSE-MIT
+-rw-r--r--   0     1001      127     1559 2024-04-14 17:20:57.000000 accesskit-0.2.0/LICENSE.chromium
+-rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 accesskit-0.2.0/PKG-INFO
```

### Comparing `accesskit-0.1.8/consumer/CHANGELOG.md` & `accesskit-0.2.0/consumer/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,32 @@
   * dependencies
     * accesskit bumped from 0.11.1 to 0.11.2
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit bumped from 0.12.2 to 0.12.3
 
+## [0.18.0](https://github.com/AccessKit/accesskit/compare/accesskit_consumer-v0.17.1...accesskit_consumer-v0.18.0) (2024-04-14)
+
+
+### ⚠ BREAKING CHANGES
+
+* New approach to lazy initialization ([#375](https://github.com/AccessKit/accesskit/issues/375))
+
+### Code Refactoring
+
+* New approach to lazy initialization ([#375](https://github.com/AccessKit/accesskit/issues/375)) ([9baebdc](https://github.com/AccessKit/accesskit/commit/9baebdceed7300389b6768815d7ae48f1ce401e4))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit bumped from 0.12.3 to 0.13.0
+
 ## [0.17.0](https://github.com/AccessKit/accesskit/compare/accesskit_consumer-v0.16.1...accesskit_consumer-v0.17.0) (2024-01-03)
 
 
 ### Features
 
 * Support custom role descriptions ([#316](https://github.com/AccessKit/accesskit/issues/316)) ([c8d1a56](https://github.com/AccessKit/accesskit/commit/c8d1a5638fa6c33adfa059815c04f7e043c56026))
```

### Comparing `accesskit-0.1.8/consumer/src/filters.rs` & `accesskit-0.2.0/consumer/src/filters.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/consumer/src/iterators.rs` & `accesskit-0.2.0/consumer/src/iterators.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/consumer/src/lib.rs` & `accesskit-0.2.0/consumer/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/consumer/src/node.rs` & `accesskit-0.2.0/consumer/src/node.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/consumer/src/text.rs` & `accesskit-0.2.0/consumer/src/text.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/consumer/src/tree.rs` & `accesskit-0.2.0/consumer/src/tree.rs`

 * *Files 1% similar despite different names*

```diff
@@ -247,14 +247,18 @@
         self.data.root
     }
 
     pub fn root(&self) -> Node<'_> {
         self.node_by_id(self.root_id()).unwrap()
     }
 
+    pub fn is_host_focused(&self) -> bool {
+        self.is_host_focused
+    }
+
     pub fn focus_id(&self) -> Option<NodeId> {
         self.is_host_focused.then_some(self.focus)
     }
 
     pub fn focus(&self) -> Option<Node<'_>> {
         self.focus_id().map(|id| self.node_by_id(id).unwrap())
     }
```

### Comparing `accesskit-0.1.8/platforms/atspi-common/Cargo.toml` & `accesskit-0.2.0/platforms/atspi-common/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [package]
 name = "accesskit_atspi_common"
-version = "0.2.0"
+version = "0.3.0"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: core AT-SPI translation layer"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
 edition.workspace = true
 rust-version.workspace = true
 
 [dependencies]
-accesskit = { version = "0.12.3", path = "../../common" }
-accesskit_consumer = { version = "0.17.1", path = "../../consumer" }
+accesskit = { version = "0.13.0", path = "../../common" }
+accesskit_consumer = { version = "0.18.0", path = "../../consumer" }
 atspi-common = { version = "0.3.0", default-features = false }
 serde = "1.0"
 thiserror = "1.0.39"
 zvariant = { version = "3", default-features = false }
```

### Comparing `accesskit-0.1.8/platforms/atspi-common/CHANGELOG.md` & `accesskit-0.2.0/platforms/atspi-common/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,33 @@
 # Changelog
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_consumer bumped from 0.17.0 to 0.17.1
 
+## [0.3.0](https://github.com/AccessKit/accesskit/compare/accesskit_atspi_common-v0.2.0...accesskit_atspi_common-v0.3.0) (2024-04-14)
+
+
+### ⚠ BREAKING CHANGES
+
+* New approach to lazy initialization ([#375](https://github.com/AccessKit/accesskit/issues/375))
+
+### Code Refactoring
+
+* New approach to lazy initialization ([#375](https://github.com/AccessKit/accesskit/issues/375)) ([9baebdc](https://github.com/AccessKit/accesskit/commit/9baebdceed7300389b6768815d7ae48f1ce401e4))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit bumped from 0.12.3 to 0.13.0
+    * accesskit_consumer bumped from 0.17.1 to 0.18.0
+
 ## [0.2.0](https://github.com/AccessKit/accesskit/compare/accesskit_atspi_common-v0.1.2...accesskit_atspi_common-v0.2.0) (2024-03-11)
 
 
 ### Features
 
 * Expose root node ID in `accesskit_atspi_common::Adapter` ([#370](https://github.com/AccessKit/accesskit/issues/370)) ([a43b497](https://github.com/AccessKit/accesskit/commit/a43b497afbbbcf90e9d15259635a329164d6a791))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `accesskit-0.1.8/platforms/atspi-common/src/adapter.rs` & `accesskit-0.2.0/platforms/atspi-common/src/adapter.rs`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 use atspi_common::{InterfaceSet, Live, State};
 use std::sync::{
     atomic::{AtomicUsize, Ordering},
     Arc, RwLock,
 };
 
 use crate::{
-    context::{AppContext, Context},
+    context::{ActionHandlerNoMut, ActionHandlerWrapper, AppContext, Context},
     filters::{filter, filter_detached},
     node::{NodeIdOrRoot, NodeWrapper, PlatformNode, PlatformRoot},
     util::WindowBounds,
     AdapterCallback, Event, ObjectEvent, WindowEvent,
 };
 
 struct AdapterChangeHandler<'a> {
@@ -116,73 +116,91 @@
             self.remove_node(node);
         }
     }
 }
 
 static NEXT_ADAPTER_ID: AtomicUsize = AtomicUsize::new(0);
 
-pub struct AdapterIdToken(usize);
-
-impl AdapterIdToken {
-    pub fn next() -> Self {
-        let id = NEXT_ADAPTER_ID.fetch_add(1, Ordering::Relaxed);
-        Self(id)
-    }
-
-    pub fn id(&self) -> usize {
-        self.0
-    }
+/// If you use this function, you must ensure that only one adapter at a time
+/// has a given ID.
+pub fn next_adapter_id() -> usize {
+    NEXT_ADAPTER_ID.fetch_add(1, Ordering::Relaxed)
 }
 
 pub struct Adapter {
     id: usize,
     callback: Box<dyn AdapterCallback + Send + Sync>,
     context: Arc<Context>,
 }
 
 impl Adapter {
     pub fn new(
         app_context: &Arc<RwLock<AppContext>>,
-        callback: Box<dyn AdapterCallback + Send + Sync>,
+        callback: impl 'static + AdapterCallback + Send + Sync,
         initial_state: TreeUpdate,
         is_window_focused: bool,
         root_window_bounds: WindowBounds,
-        action_handler: Box<dyn ActionHandler + Send>,
+        action_handler: impl 'static + ActionHandler + Send,
     ) -> Self {
-        let id_token = AdapterIdToken::next();
+        let id = next_adapter_id();
         Self::with_id(
-            id_token,
+            id,
             app_context,
             callback,
             initial_state,
             is_window_focused,
             root_window_bounds,
             action_handler,
         )
     }
 
     pub fn with_id(
-        id_token: AdapterIdToken,
+        id: usize,
+        app_context: &Arc<RwLock<AppContext>>,
+        callback: impl 'static + AdapterCallback + Send + Sync,
+        initial_state: TreeUpdate,
+        is_window_focused: bool,
+        root_window_bounds: WindowBounds,
+        action_handler: impl 'static + ActionHandler + Send,
+    ) -> Self {
+        Self::with_wrapped_action_handler(
+            id,
+            app_context,
+            callback,
+            initial_state,
+            is_window_focused,
+            root_window_bounds,
+            Arc::new(ActionHandlerWrapper::new(action_handler)),
+        )
+    }
+
+    /// This is an implementation detail of `accesskit_unix`, required for
+    /// robust state transitions with minimal overhead.
+    pub fn with_wrapped_action_handler(
+        id: usize,
         app_context: &Arc<RwLock<AppContext>>,
-        callback: Box<dyn AdapterCallback + Send + Sync>,
+        callback: impl 'static + AdapterCallback + Send + Sync,
         initial_state: TreeUpdate,
         is_window_focused: bool,
         root_window_bounds: WindowBounds,
-        action_handler: Box<dyn ActionHandler + Send>,
+        action_handler: Arc<dyn ActionHandlerNoMut + Send + Sync>,
     ) -> Self {
-        let id = id_token.0;
         let tree = Tree::new(initial_state, is_window_focused);
+        let focus_id = tree.state().focus_id();
         let context = Context::new(app_context, tree, action_handler, root_window_bounds);
         context.write_app_context().push_adapter(id, &context);
         let adapter = Self {
             id,
-            callback,
+            callback: Box::new(callback),
             context,
         };
         adapter.register_tree();
+        if let Some(id) = focus_id {
+            adapter.emit_object_event(id, ObjectEvent::StateChanged(State::Focused, true));
+        }
         adapter
     }
 
     fn register_tree(&self) {
         fn add_children(node: Node<'_>, to_add: &mut Vec<(NodeId, InterfaceSet)>) {
             for child in node.filtered_children(&filter) {
                 let child_id = child.id();
@@ -248,26 +266,26 @@
 
     fn emit_root_object_event(&self, event: ObjectEvent) {
         let target = NodeIdOrRoot::Root;
         self.callback
             .emit_event(self, Event::Object { target, event });
     }
 
-    pub fn set_root_window_bounds(&self, new_bounds: WindowBounds) {
+    pub fn set_root_window_bounds(&mut self, new_bounds: WindowBounds) {
         let mut bounds = self.context.root_window_bounds.write().unwrap();
         *bounds = new_bounds;
     }
 
-    pub fn update(&self, update: TreeUpdate) {
+    pub fn update(&mut self, update: TreeUpdate) {
         let mut handler = AdapterChangeHandler { adapter: self };
         let mut tree = self.context.tree.write().unwrap();
         tree.update_and_process_changes(update, &mut handler);
     }
 
-    pub fn update_window_focus_state(&self, is_focused: bool) {
+    pub fn update_window_focus_state(&mut self, is_focused: bool) {
         let mut handler = AdapterChangeHandler { adapter: self };
         let mut tree = self.context.tree.write().unwrap();
         tree.update_host_focus_state_and_process_changes(is_focused, &mut handler);
     }
 
     fn window_created(&self, adapter_index: usize, window: NodeId) {
         self.emit_root_object_event(ObjectEvent::ChildAdded(adapter_index, window));
@@ -301,14 +319,28 @@
     fn window_destroyed(&self, window: NodeId) {
         self.emit_root_object_event(ObjectEvent::ChildRemoved(window));
     }
 
     pub fn id(&self) -> usize {
         self.id
     }
+
+    pub fn is_window_focused(&self) -> bool {
+        self.context.read_tree().state().is_host_focused()
+    }
+
+    pub fn root_window_bounds(&self) -> WindowBounds {
+        *self.context.read_root_window_bounds()
+    }
+
+    /// This is an implementation detail of `accesskit_unix`, required for
+    /// robust state transitions with minimal overhead.
+    pub fn wrapped_action_handler(&self) -> Arc<dyn ActionHandlerNoMut + Send + Sync> {
+        Arc::clone(&self.context.action_handler)
+    }
 }
 
 fn root_window(current_state: &TreeState) -> Option<Node> {
     const WINDOW_ROLES: &[Role] = &[Role::AlertDialog, Role::Dialog, Role::Window];
     let root = current_state.root();
     if WINDOW_ROLES.contains(&root.role()) {
         Some(root)
```

### Comparing `accesskit-0.1.8/platforms/atspi-common/src/callback.rs` & `accesskit-0.2.0/platforms/atspi-common/src/callback.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/atspi-common/src/context.rs` & `accesskit-0.2.0/platforms/atspi-common/src/context.rs`

 * *Files 10% similar despite different names*

```diff
@@ -5,46 +5,68 @@
 
 use accesskit::{ActionHandler, ActionRequest};
 use accesskit_consumer::Tree;
 use std::sync::{Arc, Mutex, RwLock, RwLockReadGuard, RwLockWriteGuard};
 
 use crate::WindowBounds;
 
+/// This is an implementation detail of `accesskit_unix`, required for robust
+/// state transitions with minimal overhead.
+pub trait ActionHandlerNoMut {
+    fn do_action(&self, request: ActionRequest);
+}
+
+/// This is an implementation detail of `accesskit_unix`, required for robust
+/// state transitions with minimal overhead.
+pub struct ActionHandlerWrapper<H: ActionHandler + Send>(Mutex<H>);
+
+impl<H: 'static + ActionHandler + Send> ActionHandlerWrapper<H> {
+    pub fn new(inner: H) -> Self {
+        Self(Mutex::new(inner))
+    }
+}
+
+impl<H: ActionHandler + Send> ActionHandlerNoMut for ActionHandlerWrapper<H> {
+    fn do_action(&self, request: ActionRequest) {
+        self.0.lock().unwrap().do_action(request)
+    }
+}
+
 pub(crate) struct Context {
     pub(crate) app_context: Arc<RwLock<AppContext>>,
     pub(crate) tree: RwLock<Tree>,
-    pub(crate) action_handler: Mutex<Box<dyn ActionHandler + Send>>,
+    pub(crate) action_handler: Arc<dyn ActionHandlerNoMut + Send + Sync>,
     pub(crate) root_window_bounds: RwLock<WindowBounds>,
 }
 
 impl Context {
     pub(crate) fn new(
         app_context: &Arc<RwLock<AppContext>>,
         tree: Tree,
-        action_handler: Box<dyn ActionHandler + Send>,
+        action_handler: Arc<dyn ActionHandlerNoMut + Send + Sync>,
         root_window_bounds: WindowBounds,
     ) -> Arc<Self> {
         Arc::new(Self {
             app_context: Arc::clone(app_context),
             tree: RwLock::new(tree),
-            action_handler: Mutex::new(action_handler),
+            action_handler,
             root_window_bounds: RwLock::new(root_window_bounds),
         })
     }
 
     pub(crate) fn read_tree(&self) -> RwLockReadGuard<'_, Tree> {
         self.tree.read().unwrap()
     }
 
     pub(crate) fn read_root_window_bounds(&self) -> RwLockReadGuard<'_, WindowBounds> {
         self.root_window_bounds.read().unwrap()
     }
 
     pub fn do_action(&self, request: ActionRequest) {
-        self.action_handler.lock().unwrap().do_action(request);
+        self.action_handler.do_action(request);
     }
 
     pub(crate) fn read_app_context(&self) -> RwLockReadGuard<'_, AppContext> {
         self.app_context.read().unwrap()
     }
 
     pub(crate) fn write_app_context(&self) -> RwLockWriteGuard<'_, AppContext> {
```

### Comparing `accesskit-0.1.8/platforms/atspi-common/src/error.rs` & `accesskit-0.2.0/platforms/atspi-common/src/error.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/atspi-common/src/events.rs` & `accesskit-0.2.0/platforms/atspi-common/src/events.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/atspi-common/src/lib.rs` & `accesskit-0.2.0/platforms/atspi-common/src/lib.rs`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 mod rect;
 pub mod simplified;
 mod util;
 
 pub use atspi_common::{CoordType, InterfaceSet, Layer, Role, State, StateSet};
 
 pub use action::*;
-pub use adapter::{Adapter, AdapterIdToken};
+pub use adapter::{next_adapter_id, Adapter};
 pub use callback::AdapterCallback;
-pub use context::AppContext;
+pub use context::{ActionHandlerNoMut, ActionHandlerWrapper, AppContext};
 pub use error::*;
 pub use events::*;
 pub use node::{NodeIdOrRoot, PlatformNode, PlatformRoot};
 pub use rect::*;
 pub use util::WindowBounds;
```

### Comparing `accesskit-0.1.8/platforms/atspi-common/src/node.rs` & `accesskit-0.2.0/platforms/atspi-common/src/node.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/atspi-common/src/rect.rs` & `accesskit-0.2.0/platforms/atspi-common/src/rect.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/atspi-common/src/simplified.rs` & `accesskit-0.2.0/platforms/atspi-common/src/simplified.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/atspi-common/src/util.rs` & `accesskit-0.2.0/platforms/atspi-common/src/util.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/unix/Cargo.toml` & `accesskit-0.2.0/platforms/unix/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "accesskit_unix"
-version = "0.7.5"
+version = "0.8.0"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: Linux adapter"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
@@ -13,16 +13,16 @@
 
 [features]
 default = ["async-io"]
 async-io = ["dep:async-channel", "dep:async-executor", "dep:async-task", "dep:futures-util", "atspi/async-std", "zbus/async-io"]
 tokio = ["dep:tokio", "dep:tokio-stream", "atspi/tokio", "zbus/tokio"]
 
 [dependencies]
-accesskit = { version = "0.12.3", path = "../../common" }
-accesskit_atspi_common = { version = "0.2.0", path = "../atspi-common" }
+accesskit = { version = "0.13.0", path = "../../common" }
+accesskit_atspi_common = { version = "0.3.0", path = "../atspi-common" }
 atspi = { version = "0.19", default-features = false }
 futures-lite = "1.13"
 once_cell = "1.17.1"
 serde = "1.0"
 zbus = { version = "3.14", default-features = false }
 
 # async-io support
```

### Comparing `accesskit-0.1.8/platforms/unix/CHANGELOG.md` & `accesskit-0.2.0/platforms/unix/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,33 @@
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_atspi_common bumped from 0.1.1 to 0.1.2
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit_atspi_common bumped from 0.1.2 to 0.2.0
 
+## [0.8.0](https://github.com/AccessKit/accesskit/compare/accesskit_unix-v0.7.5...accesskit_unix-v0.8.0) (2024-04-14)
+
+
+### ⚠ BREAKING CHANGES
+
+* New approach to lazy initialization ([#375](https://github.com/AccessKit/accesskit/issues/375))
+
+### Code Refactoring
+
+* New approach to lazy initialization ([#375](https://github.com/AccessKit/accesskit/issues/375)) ([9baebdc](https://github.com/AccessKit/accesskit/commit/9baebdceed7300389b6768815d7ae48f1ce401e4))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit bumped from 0.12.3 to 0.13.0
+    * accesskit_atspi_common bumped from 0.2.0 to 0.3.0
+
 ## [0.7.2](https://github.com/AccessKit/accesskit/compare/accesskit_unix-v0.7.1...accesskit_unix-v0.7.2) (2024-02-24)
 
 
 ### Bug Fixes
 
 * Don't emit focus event twice on Unix ([#354](https://github.com/AccessKit/accesskit/issues/354)) ([b39216c](https://github.com/AccessKit/accesskit/commit/b39216cb31df692fef377f9b3c3c718fd225cc3c))
 * Use the new accesskit_atspi_common crate in the Unix adapter ([#356](https://github.com/AccessKit/accesskit/issues/356)) ([b2a468c](https://github.com/AccessKit/accesskit/commit/b2a468ccb91ee4e6d3435e73eb00c65cbe75060a))
```

### Comparing `accesskit-0.1.8/platforms/unix/src/atspi/bus.rs` & `accesskit-0.2.0/platforms/unix/src/atspi/bus.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/unix/src/atspi/interfaces/accessible.rs` & `accesskit-0.2.0/platforms/unix/src/atspi/interfaces/accessible.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/unix/src/atspi/interfaces/action.rs` & `accesskit-0.2.0/platforms/unix/src/atspi/interfaces/action.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/unix/src/atspi/interfaces/application.rs` & `accesskit-0.2.0/platforms/unix/src/atspi/interfaces/application.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/unix/src/atspi/interfaces/component.rs` & `accesskit-0.2.0/platforms/unix/src/atspi/interfaces/component.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/unix/src/atspi/interfaces/mod.rs` & `accesskit-0.2.0/platforms/unix/src/atspi/interfaces/mod.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/unix/src/atspi/interfaces/value.rs` & `accesskit-0.2.0/platforms/unix/src/atspi/interfaces/value.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/unix/src/atspi/object_address.rs` & `accesskit-0.2.0/platforms/unix/src/atspi/object_address.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/unix/src/atspi/object_id.rs` & `accesskit-0.2.0/platforms/unix/src/atspi/object_id.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/unix/src/executor.rs` & `accesskit-0.2.0/platforms/unix/src/executor.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/unix/src/lib.rs` & `accesskit-0.2.0/platforms/unix/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/unix/src/util.rs` & `accesskit-0.2.0/platforms/unix/src/util.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/windows/Cargo.toml` & `accesskit-0.2.0/platforms/windows/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [package]
 name = "accesskit_windows"
-version = "0.16.4"
+version = "0.17.0"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: Windows adapter"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
 edition.workspace = true
 rust-version.workspace = true
 
 [dependencies]
-accesskit = { version = "0.12.3", path = "../../common" }
-accesskit_consumer = { version = "0.17.1", path = "../../consumer" }
-once_cell = "1.13.0"
+accesskit = { version = "0.13.0", path = "../../common" }
+accesskit_consumer = { version = "0.18.0", path = "../../consumer" }
 paste = "1.0"
 static_assertions = "1.1.0"
 
 [dependencies.windows]
 version = "0.54"
 features = [
     "implement",
@@ -30,10 +29,10 @@
     "Win32_System_Variant",
     "Win32_UI_Accessibility",
     "Win32_UI_Input_KeyboardAndMouse",
     "Win32_UI_WindowsAndMessaging",
 ]
 
 [dev-dependencies]
+once_cell = "1.13.0"
 scopeguard = "1.1.0"
 winit = "0.29"
-
```

### Comparing `accesskit-0.1.8/platforms/windows/CHANGELOG.md` & `accesskit-0.2.0/platforms/windows/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,33 @@
     * accesskit_consumer bumped from 0.15.1 to 0.15.2
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_consumer bumped from 0.17.0 to 0.17.1
 
+## [0.17.0](https://github.com/AccessKit/accesskit/compare/accesskit_windows-v0.16.4...accesskit_windows-v0.17.0) (2024-04-14)
+
+
+### ⚠ BREAKING CHANGES
+
+* New approach to lazy initialization ([#375](https://github.com/AccessKit/accesskit/issues/375))
+
+### Code Refactoring
+
+* New approach to lazy initialization ([#375](https://github.com/AccessKit/accesskit/issues/375)) ([9baebdc](https://github.com/AccessKit/accesskit/commit/9baebdceed7300389b6768815d7ae48f1ce401e4))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit bumped from 0.12.3 to 0.13.0
+    * accesskit_consumer bumped from 0.17.1 to 0.18.0
+
 ## [0.16.4](https://github.com/AccessKit/accesskit/compare/accesskit_windows-v0.16.3...accesskit_windows-v0.16.4) (2024-03-18)
 
 
 ### Bug Fixes
 
 * Update `windows` to `0.54` ([#373](https://github.com/AccessKit/accesskit/issues/373)) ([50f112f](https://github.com/AccessKit/accesskit/commit/50f112f0085a03f0180f86915d2ac4e5845f6b63))
```

### Comparing `accesskit-0.1.8/platforms/windows/examples/hello_world.rs` & `accesskit-0.2.0/platforms/windows/examples/hello_world.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 // Based on the create_window sample in windows-samples-rs.
 
 use accesskit::{
-    Action, ActionHandler, ActionRequest, DefaultActionVerb, Live, Node, NodeBuilder, NodeClassSet,
-    NodeId, Rect, Role, Tree, TreeUpdate,
+    Action, ActionHandler, ActionRequest, ActivationHandler, DefaultActionVerb, Live, Node,
+    NodeBuilder, NodeClassSet, NodeId, Rect, Role, Tree, TreeUpdate,
 };
-use accesskit_windows::UiaInitMarker;
-use once_cell::{sync::Lazy, unsync::OnceCell};
+use accesskit_windows::Adapter;
+use once_cell::sync::Lazy;
 use std::cell::RefCell;
 use windows::{
     core::*,
     Win32::{
         Foundation::*,
         Graphics::Gdi::ValidateRect,
         System::LibraryLoader::GetModuleHandleW,
@@ -81,30 +81,32 @@
     builder.set_name(text);
     builder.set_live(Live::Polite);
     builder.build(classes)
 }
 
 struct InnerWindowState {
     focus: NodeId,
-    is_window_focused: bool,
     announcement: Option<String>,
     node_classes: NodeClassSet,
 }
 
 impl InnerWindowState {
     fn build_root(&mut self) -> Node {
         let mut builder = NodeBuilder::new(Role::Window);
         builder.set_children(vec![BUTTON_1_ID, BUTTON_2_ID]);
         if self.announcement.is_some() {
             builder.push_child(ANNOUNCEMENT_ID);
         }
         builder.build(&mut self.node_classes)
     }
+}
 
-    fn build_initial_tree(&mut self) -> TreeUpdate {
+impl ActivationHandler for InnerWindowState {
+    fn request_initial_tree(&mut self) -> Option<TreeUpdate> {
+        println!("Initial tree requested");
         let root = self.build_root();
         let button_1 = build_button(BUTTON_1_ID, "Button 1", &mut self.node_classes);
         let button_2 = build_button(BUTTON_2_ID, "Button 2", &mut self.node_classes);
         let mut tree = Tree::new(WINDOW_ID);
         tree.app_name = Some("hello_world".to_string());
 
         let mut result = TreeUpdate {
@@ -118,89 +120,71 @@
         };
         if let Some(announcement) = &self.announcement {
             result.nodes.push((
                 ANNOUNCEMENT_ID,
                 build_announcement(announcement, &mut self.node_classes),
             ));
         }
-        result
+        Some(result)
     }
 }
 
 struct WindowState {
-    uia_init_marker: UiaInitMarker,
-    adapter: OnceCell<accesskit_windows::Adapter>,
+    adapter: RefCell<Adapter>,
     inner_state: RefCell<InnerWindowState>,
 }
 
 impl WindowState {
-    fn get_or_init_accesskit_adapter(&self, window: HWND) -> &accesskit_windows::Adapter {
-        self.adapter.get_or_init(|| {
-            let mut inner_state = self.inner_state.borrow_mut();
-            let initial_tree = inner_state.build_initial_tree();
-            let is_window_focused = inner_state.is_window_focused;
-            drop(inner_state);
-            let action_handler = Box::new(SimpleActionHandler { window });
-            accesskit_windows::Adapter::new(
-                window,
-                initial_tree,
-                is_window_focused,
-                action_handler,
-                self.uia_init_marker,
-            )
-        })
-    }
-
     fn set_focus(&self, focus: NodeId) {
-        let mut inner_state = self.inner_state.borrow_mut();
-        inner_state.focus = focus;
-        if let Some(adapter) = self.adapter.get() {
-            let update = TreeUpdate {
-                nodes: vec![],
-                tree: None,
-                focus,
-            };
-            let events = adapter.update(update);
+        self.inner_state.borrow_mut().focus = focus;
+        let mut adapter = self.adapter.borrow_mut();
+        if let Some(events) = adapter.update_if_active(|| TreeUpdate {
+            nodes: vec![],
+            tree: None,
+            focus,
+        }) {
+            drop(adapter);
             events.raise();
         }
     }
 
     fn press_button(&self, id: NodeId) {
         let mut inner_state = self.inner_state.borrow_mut();
         let text = if id == BUTTON_1_ID {
             "You pressed button 1"
         } else {
             "You pressed button 2"
         };
         inner_state.announcement = Some(text.into());
-        if let Some(adapter) = self.adapter.get() {
+        let mut adapter = self.adapter.borrow_mut();
+        if let Some(events) = adapter.update_if_active(|| {
             let announcement = build_announcement(text, &mut inner_state.node_classes);
             let root = inner_state.build_root();
-            let update = TreeUpdate {
+            TreeUpdate {
                 nodes: vec![(ANNOUNCEMENT_ID, announcement), (WINDOW_ID, root)],
                 tree: None,
                 focus: inner_state.focus,
-            };
-            let events = adapter.update(update);
+            }
+        }) {
+            drop(adapter);
+            drop(inner_state);
             events.raise();
         }
     }
 }
 
 unsafe fn get_window_state(window: HWND) -> *const WindowState {
     GetWindowLongPtrW(window, GWLP_USERDATA) as _
 }
 
-fn update_window_focus_state(window: HWND, is_window_focused: bool) {
-    let window_state = unsafe { &*get_window_state(window) };
-    let mut inner_state = window_state.inner_state.borrow_mut();
-    inner_state.is_window_focused = is_window_focused;
-    drop(inner_state);
-    if let Some(adapter) = window_state.adapter.get() {
-        let events = adapter.update_window_focus_state(is_window_focused);
+fn update_window_focus_state(window: HWND, is_focused: bool) {
+    let state = unsafe { &*get_window_state(window) };
+    let mut adapter = state.adapter.borrow_mut();
+    if let Some(events) = adapter.update_window_focus_state(is_focused) {
+        drop(adapter);
         events.raise();
     }
 }
 
 struct WindowCreateParams(NodeId);
 
 struct SimpleActionHandler {
@@ -242,49 +226,51 @@
         WM_NCCREATE => {
             let create_struct: &CREATESTRUCTW = unsafe { &mut *(lparam.0 as *mut _) };
             let create_params: Box<WindowCreateParams> =
                 unsafe { Box::from_raw(create_struct.lpCreateParams as _) };
             let WindowCreateParams(initial_focus) = *create_params;
             let inner_state = RefCell::new(InnerWindowState {
                 focus: initial_focus,
-                is_window_focused: false,
                 announcement: None,
                 node_classes: NodeClassSet::new(),
             });
+            let adapter = Adapter::new(window, false, SimpleActionHandler { window });
             let state = Box::new(WindowState {
-                uia_init_marker: UiaInitMarker::new(),
-                adapter: OnceCell::new(),
+                adapter: RefCell::new(adapter),
                 inner_state,
             });
             unsafe { SetWindowLongPtrW(window, GWLP_USERDATA, Box::into_raw(state) as _) };
             unsafe { DefWindowProcW(window, message, wparam, lparam) }
         }
         WM_PAINT => {
             unsafe { ValidateRect(window, None) }.unwrap();
             LRESULT(0)
         }
         WM_DESTROY => {
             let ptr = unsafe { SetWindowLongPtrW(window, GWLP_USERDATA, 0) };
             if ptr != 0 {
-                let _dropped: Box<WindowState> = unsafe { Box::from_raw(ptr as _) };
+                drop(unsafe { Box::<WindowState>::from_raw(ptr as _) });
             }
             unsafe { PostQuitMessage(0) };
             LRESULT(0)
         }
         WM_GETOBJECT => {
-            let window_state = unsafe { get_window_state(window) };
-            if window_state.is_null() {
+            let state_ptr = unsafe { get_window_state(window) };
+            if state_ptr.is_null() {
                 // We need to be prepared to gracefully handle WM_GETOBJECT
                 // while the window is being destroyed; this can happen if
                 // the thread is using a COM STA.
                 return unsafe { DefWindowProcW(window, message, wparam, lparam) };
             }
-            let window_state = unsafe { &*window_state };
-            let adapter = window_state.get_or_init_accesskit_adapter(window);
-            let result = adapter.handle_wm_getobject(wparam, lparam);
+            let state = unsafe { &*state_ptr };
+            let mut adapter = state.adapter.borrow_mut();
+            let mut inner_state = state.inner_state.borrow_mut();
+            let result = adapter.handle_wm_getobject(wparam, lparam, &mut *inner_state);
+            drop(inner_state);
+            drop(adapter);
             result.map_or_else(
                 || unsafe { DefWindowProcW(window, message, wparam, lparam) },
                 |result| result.into(),
             )
         }
         WM_SETFOCUS | WM_EXITMENULOOP | WM_EXITSIZEMOVE => {
             update_window_focus_state(window, true);
@@ -292,45 +278,45 @@
         }
         WM_KILLFOCUS | WM_ENTERMENULOOP | WM_ENTERSIZEMOVE => {
             update_window_focus_state(window, false);
             LRESULT(0)
         }
         WM_KEYDOWN => match VIRTUAL_KEY(wparam.0 as u16) {
             VK_TAB => {
-                let window_state = unsafe { &*get_window_state(window) };
-                let old_focus = window_state.inner_state.borrow().focus;
+                let state = unsafe { &*get_window_state(window) };
+                let old_focus = state.inner_state.borrow().focus;
                 let new_focus = if old_focus == BUTTON_1_ID {
                     BUTTON_2_ID
                 } else {
                     BUTTON_1_ID
                 };
-                window_state.set_focus(new_focus);
+                state.set_focus(new_focus);
                 LRESULT(0)
             }
             VK_SPACE => {
-                let window_state = unsafe { &*get_window_state(window) };
-                let id = window_state.inner_state.borrow().focus;
-                window_state.press_button(id);
+                let state = unsafe { &*get_window_state(window) };
+                let id = state.inner_state.borrow().focus;
+                state.press_button(id);
                 LRESULT(0)
             }
             _ => unsafe { DefWindowProcW(window, message, wparam, lparam) },
         },
         SET_FOCUS_MSG => {
             let id = NodeId(lparam.0 as _);
             if id == BUTTON_1_ID || id == BUTTON_2_ID {
-                let window_state = unsafe { &*get_window_state(window) };
-                window_state.set_focus(id);
+                let state = unsafe { &*get_window_state(window) };
+                state.set_focus(id);
             }
             LRESULT(0)
         }
         DO_DEFAULT_ACTION_MSG => {
             let id = NodeId(lparam.0 as _);
             if id == BUTTON_1_ID || id == BUTTON_2_ID {
-                let window_state = unsafe { &*get_window_state(window) };
-                window_state.press_button(id);
+                let state = unsafe { &*get_window_state(window) };
+                state.press_button(id);
             }
             LRESULT(0)
         }
         _ => unsafe { DefWindowProcW(window, message, wparam, lparam) },
     }
 }
```

### Comparing `accesskit-0.1.8/platforms/windows/src/adapter.rs` & `accesskit-0.2.0/platforms/windows/src/adapter.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,55 @@
 // Copyright 2022 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
-use accesskit::{ActionHandler, Live, NodeId, Role, TreeUpdate};
+use accesskit::{
+    ActionHandler, ActionRequest, ActivationHandler, Live, NodeBuilder, NodeId, Role,
+    Tree as TreeData, TreeUpdate,
+};
 use accesskit_consumer::{DetachedNode, FilterResult, Node, Tree, TreeChangeHandler, TreeState};
 use std::{collections::HashSet, sync::Arc};
 use windows::Win32::{
     Foundation::*,
     UI::{Accessibility::*, WindowsAndMessaging::*},
 };
 
 use crate::{
-    context::Context,
+    context::{ActionHandlerNoMut, ActionHandlerWrapper, Context},
     filters::{filter, filter_detached},
-    init::UiaInitMarker,
     node::{NodeWrapper, PlatformNode},
     util::QueuedEvent,
 };
 
+fn focus_event(context: &Arc<Context>, node_id: NodeId) -> QueuedEvent {
+    let platform_node = PlatformNode::new(context, node_id);
+    let element: IRawElementProviderSimple = platform_node.into();
+    QueuedEvent::Simple {
+        element,
+        event_id: UIA_AutomationFocusChangedEventId,
+    }
+}
+
 struct AdapterChangeHandler<'a> {
     context: &'a Arc<Context>,
     queue: Vec<QueuedEvent>,
     text_changed: HashSet<NodeId>,
 }
 
+impl<'a> AdapterChangeHandler<'a> {
+    fn new(context: &'a Arc<Context>) -> Self {
+        Self {
+            context,
+            queue: Vec::new(),
+            text_changed: HashSet::new(),
+        }
+    }
+}
+
 impl AdapterChangeHandler<'_> {
     fn insert_text_change_if_needed_parent(&mut self, node: Node) {
         if !node.supports_text_ranges() {
             return;
         }
         let id = node.id();
         if self.text_changed.contains(&id) {
@@ -118,135 +139,265 @@
     fn focus_moved(
         &mut self,
         _old_node: Option<&DetachedNode>,
         new_node: Option<&Node>,
         _current_state: &TreeState,
     ) {
         if let Some(new_node) = new_node {
-            let platform_node = PlatformNode::new(self.context, new_node.id());
-            let element: IRawElementProviderSimple = platform_node.into();
-            self.queue.push(QueuedEvent::Simple {
-                element,
-                event_id: UIA_AutomationFocusChangedEventId,
-            });
+            self.queue.push(focus_event(self.context, new_node.id()));
         }
     }
 
     fn node_removed(&mut self, node: &DetachedNode, current_state: &TreeState) {
         self.insert_text_change_if_needed_for_removed_node(node, current_state);
     }
 
     // TODO: handle other events (#20)
 }
 
+const PLACEHOLDER_ROOT_ID: NodeId = NodeId(0);
+
+enum State {
+    Inactive {
+        hwnd: HWND,
+        is_window_focused: bool,
+        action_handler: Arc<dyn ActionHandlerNoMut + Send + Sync>,
+    },
+    Placeholder {
+        placeholder_context: Arc<Context>,
+        is_window_focused: bool,
+        action_handler: Arc<dyn ActionHandlerNoMut + Send + Sync>,
+    },
+    Active(Arc<Context>),
+}
+
+struct PlaceholderActionHandler;
+
+impl ActionHandler for PlaceholderActionHandler {
+    fn do_action(&mut self, _request: ActionRequest) {}
+}
+
 pub struct Adapter {
-    context: Arc<Context>,
+    state: State,
 }
 
 impl Adapter {
     /// Creates a new Windows platform adapter.
     ///
     /// The action handler may or may not be called on the thread that owns
     /// the window.
+    ///
+    /// This must not be called while handling the `WM_GETOBJECT` message,
+    /// because this function must initialize UI Automation before
+    /// that message is handled. This is necessary to prevent a race condition
+    /// that leads to nested `WM_GETOBJECT` messages and, in some cases,
+    /// assistive technologies not realizing that the window natively implements.
+    /// UIA. See [AccessKit issue #37](https://github.com/AccessKit/accesskit/issues/37)
+    /// for more details.
     pub fn new(
         hwnd: HWND,
-        initial_state: TreeUpdate,
         is_window_focused: bool,
-        action_handler: Box<dyn ActionHandler + Send>,
-        _uia_init_marker: UiaInitMarker,
+        action_handler: impl 'static + ActionHandler + Send,
     ) -> Self {
-        let context = Context::new(
+        Self::with_wrapped_action_handler(
             hwnd,
-            Tree::new(initial_state, is_window_focused),
-            action_handler,
-        );
-        Self { context }
+            is_window_focused,
+            Arc::new(ActionHandlerWrapper::new(action_handler)),
+        )
     }
 
-    fn change_handler(&self) -> AdapterChangeHandler {
-        AdapterChangeHandler {
-            context: &self.context,
-            queue: Vec::new(),
-            text_changed: HashSet::new(),
-        }
+    // Currently required by the test infrastructure
+    pub(crate) fn with_wrapped_action_handler(
+        hwnd: HWND,
+        is_window_focused: bool,
+        action_handler: Arc<dyn ActionHandlerNoMut + Send + Sync>,
+    ) -> Self {
+        init_uia();
+
+        let state = State::Inactive {
+            hwnd,
+            is_window_focused,
+            action_handler,
+        };
+        Self { state }
     }
 
-    /// Apply the provided update to the tree.
+    /// If and only if the tree has been initialized, call the provided function
+    /// and apply the resulting update. Note: If the caller's implementation of
+    /// [`ActivationHandler::request_initial_tree`] initially returned `None`,
+    /// the [`TreeUpdate`] returned by the provided function must contain
+    /// a full tree.
     ///
-    /// The caller must call [`QueuedEvents::raise`] on the return value.
+    /// If a [`QueuedEvents`] instance is returned, the caller must call
+    /// [`QueuedEvents::raise`] on it.
     ///
     /// This method may be safely called on any thread, but refer to
     /// [`QueuedEvents::raise`] for restrictions on the context in which
     /// it should be called.
-    pub fn update(&self, update: TreeUpdate) -> QueuedEvents {
-        let mut handler = self.change_handler();
-        let mut tree = self.context.tree.write().unwrap();
-        tree.update_and_process_changes(update, &mut handler);
-        QueuedEvents(handler.queue)
+    pub fn update_if_active(
+        &mut self,
+        update_factory: impl FnOnce() -> TreeUpdate,
+    ) -> Option<QueuedEvents> {
+        match &self.state {
+            State::Inactive { .. } => None,
+            State::Placeholder {
+                placeholder_context,
+                is_window_focused,
+                action_handler,
+            } => {
+                let tree = Tree::new(update_factory(), *is_window_focused);
+                let context =
+                    Context::new(placeholder_context.hwnd, tree, Arc::clone(action_handler));
+                let result = context
+                    .read_tree()
+                    .state()
+                    .focus_id()
+                    .map(|id| QueuedEvents(vec![focus_event(&context, id)]));
+                self.state = State::Active(context);
+                result
+            }
+            State::Active(context) => {
+                let mut handler = AdapterChangeHandler::new(context);
+                let mut tree = context.tree.write().unwrap();
+                tree.update_and_process_changes(update_factory(), &mut handler);
+                Some(QueuedEvents(handler.queue))
+            }
+        }
     }
 
     /// Update the tree state based on whether the window is focused.
     ///
-    /// The caller must call [`QueuedEvents::raise`] on the return value.
+    /// If a [`QueuedEvents`] instance is returned, the caller must call
+    /// [`QueuedEvents::raise`] on it.
     ///
     /// This method may be safely called on any thread, but refer to
     /// [`QueuedEvents::raise`] for restrictions on the context in which
     /// it should be called.
-    pub fn update_window_focus_state(&self, is_focused: bool) -> QueuedEvents {
-        let mut handler = self.change_handler();
-        let mut tree = self.context.tree.write().unwrap();
-        tree.update_host_focus_state_and_process_changes(is_focused, &mut handler);
-        QueuedEvents(handler.queue)
-    }
-
-    fn root_platform_node(&self) -> PlatformNode {
-        let tree = self.context.read_tree();
-        let node_id = tree.state().root_id();
-        PlatformNode::new(&self.context, node_id)
+    pub fn update_window_focus_state(&mut self, is_focused: bool) -> Option<QueuedEvents> {
+        match &mut self.state {
+            State::Inactive {
+                is_window_focused, ..
+            } => {
+                *is_window_focused = is_focused;
+                None
+            }
+            State::Placeholder {
+                is_window_focused, ..
+            } => {
+                *is_window_focused = is_focused;
+                None
+            }
+            State::Active(context) => {
+                let mut handler = AdapterChangeHandler::new(context);
+                let mut tree = context.tree.write().unwrap();
+                tree.update_host_focus_state_and_process_changes(is_focused, &mut handler);
+                Some(QueuedEvents(handler.queue))
+            }
+        }
     }
 
-    /// Handle the `WM_GETOBJECT` window message.
+    /// Handle the `WM_GETOBJECT` window message. The accessibility tree
+    /// is lazily initialized if necessary using the provided
+    /// [`ActivationHandler`] implementation.
     ///
     /// This returns an `Option` so the caller can pass the message
     /// to `DefWindowProc` if AccessKit decides not to handle it.
     /// The optional value is an `Into<LRESULT>` rather than simply an `LRESULT`
     /// so the necessary call to UIA, which may lead to a nested `WM_GETOBJECT`
     /// message, can be done outside of any lock that the caller might hold
     /// on the `Adapter` or window state, while still abstracting away
     /// the details of that call to UIA.
-    ///
-    /// Callers must avoid a second deadlock scenario. The tree is lazily
-    /// initialized on the first call to this method. So if the caller
-    /// holds a lock while calling this method, it must be careful to ensure
-    /// that running its tree initialization function while holding that lock
-    /// doesn't lead to deadlock.
-    pub fn handle_wm_getobject(
-        &self,
+    pub fn handle_wm_getobject<H: ActivationHandler + ?Sized>(
+        &mut self,
         wparam: WPARAM,
         lparam: LPARAM,
+        activation_handler: &mut H,
     ) -> Option<impl Into<LRESULT>> {
         // Don't bother with MSAA object IDs that are asking for something other
         // than the client area of the window. DefWindowProc can handle those.
         // First, cast the lparam to i32, to handle inconsistent conversion
         // behavior in senders.
         let objid = normalize_objid(lparam);
         if objid < 0 && objid != UiaRootObjectId && objid != OBJID_CLIENT.0 {
             return None;
         }
 
-        let el: IRawElementProviderSimple = self.root_platform_node().into();
+        let (hwnd, platform_node) = match &self.state {
+            State::Inactive {
+                hwnd,
+                is_window_focused,
+                action_handler,
+            } => match activation_handler.request_initial_tree() {
+                Some(initial_state) => {
+                    let hwnd = *hwnd;
+                    let tree = Tree::new(initial_state, *is_window_focused);
+                    let context = Context::new(hwnd, tree, Arc::clone(action_handler));
+                    let node_id = context.read_tree().state().root_id();
+                    let platform_node = PlatformNode::new(&context, node_id);
+                    self.state = State::Active(context);
+                    (hwnd, platform_node)
+                }
+                None => {
+                    let hwnd = *hwnd;
+                    let placeholder_update = TreeUpdate {
+                        nodes: vec![(
+                            PLACEHOLDER_ROOT_ID,
+                            NodeBuilder::new(Role::Window).build(&mut Default::default()),
+                        )],
+                        tree: Some(TreeData::new(PLACEHOLDER_ROOT_ID)),
+                        focus: PLACEHOLDER_ROOT_ID,
+                    };
+                    let placeholder_tree = Tree::new(placeholder_update, false);
+                    let placeholder_context = Context::new(
+                        hwnd,
+                        placeholder_tree,
+                        Arc::new(ActionHandlerWrapper::new(PlaceholderActionHandler {})),
+                    );
+                    let platform_node =
+                        PlatformNode::new(&placeholder_context, PLACEHOLDER_ROOT_ID);
+                    self.state = State::Placeholder {
+                        placeholder_context,
+                        is_window_focused: *is_window_focused,
+                        action_handler: Arc::clone(action_handler),
+                    };
+                    (hwnd, platform_node)
+                }
+            },
+            State::Placeholder {
+                placeholder_context,
+                ..
+            } => (
+                placeholder_context.hwnd,
+                PlatformNode::new(placeholder_context, PLACEHOLDER_ROOT_ID),
+            ),
+            State::Active(context) => {
+                let node_id = context.read_tree().state().root_id();
+                (context.hwnd, PlatformNode::new(context, node_id))
+            }
+        };
+        let el: IRawElementProviderSimple = platform_node.into();
         Some(WmGetObjectResult {
-            hwnd: self.context.hwnd,
+            hwnd,
             wparam,
             lparam,
             el,
         })
     }
 }
 
+fn init_uia() {
+    // `UiaLookupId` is a cheap way of forcing UIA to initialize itself.
+    unsafe {
+        UiaLookupId(
+            AutomationIdentifierType_Property,
+            &ControlType_Property_GUID,
+        )
+    };
+}
+
 #[cfg(any(target_arch = "x86_64", target_arch = "aarch64"))]
 fn normalize_objid(lparam: LPARAM) -> i32 {
     (lparam.0 & 0xFFFFFFFF) as _
 }
 #[cfg(not(any(target_arch = "x86_64", target_arch = "aarch64")))]
 fn normalize_objid(lparam: LPARAM) -> i32 {
     lparam.0 as _
```

### Comparing `accesskit-0.1.8/platforms/windows/src/context.rs` & `accesskit-0.2.0/platforms/windows/src/context.rs`

 * *Files 18% similar despite different names*

```diff
@@ -6,38 +6,56 @@
 use accesskit::{ActionHandler, ActionRequest, Point};
 use accesskit_consumer::Tree;
 use std::sync::{Arc, Mutex, RwLock, RwLockReadGuard};
 use windows::Win32::Foundation::*;
 
 use crate::util::*;
 
+pub(crate) trait ActionHandlerNoMut {
+    fn do_action(&self, request: ActionRequest);
+}
+
+pub(crate) struct ActionHandlerWrapper<H: ActionHandler + Send>(Mutex<H>);
+
+impl<H: 'static + ActionHandler + Send> ActionHandlerWrapper<H> {
+    pub(crate) fn new(inner: H) -> Self {
+        Self(Mutex::new(inner))
+    }
+}
+
+impl<H: ActionHandler + Send> ActionHandlerNoMut for ActionHandlerWrapper<H> {
+    fn do_action(&self, request: ActionRequest) {
+        self.0.lock().unwrap().do_action(request)
+    }
+}
+
 pub(crate) struct Context {
     pub(crate) hwnd: HWND,
     pub(crate) tree: RwLock<Tree>,
-    pub(crate) action_handler: Mutex<Box<dyn ActionHandler + Send>>,
+    pub(crate) action_handler: Arc<dyn ActionHandlerNoMut + Send + Sync>,
 }
 
 impl Context {
     pub(crate) fn new(
         hwnd: HWND,
         tree: Tree,
-        action_handler: Box<dyn ActionHandler + Send>,
+        action_handler: Arc<dyn ActionHandlerNoMut + Send + Sync>,
     ) -> Arc<Self> {
         Arc::new(Self {
             hwnd,
             tree: RwLock::new(tree),
-            action_handler: Mutex::new(action_handler),
+            action_handler,
         })
     }
 
     pub(crate) fn read_tree(&self) -> RwLockReadGuard<'_, Tree> {
         self.tree.read().unwrap()
     }
 
     pub(crate) fn client_top_left(&self) -> Point {
         client_top_left(self.hwnd)
     }
 
     pub(crate) fn do_action(&self, request: ActionRequest) {
-        self.action_handler.lock().unwrap().do_action(request);
+        self.action_handler.do_action(request);
     }
 }
```

### Comparing `accesskit-0.1.8/platforms/windows/src/lib.rs` & `accesskit-0.2.0/platforms/macos/src/lib.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-// Copyright 2021 The AccessKit Authors. All rights reserved.
+// Copyright 2022 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
+#![deny(unsafe_op_in_unsafe_fn)]
+
 mod context;
 mod filters;
 mod node;
-mod text;
 mod util;
 
 mod adapter;
-pub use adapter::{Adapter, QueuedEvents};
+pub use adapter::Adapter;
+
+mod event;
+pub use event::QueuedEvents;
 
-mod init;
-pub use init::UiaInitMarker;
+mod patch;
+pub use patch::add_focus_forwarder_to_window_class;
 
 mod subclass;
 pub use subclass::SubclassingAdapter;
 
-pub use windows::Win32::Foundation::{HWND, LPARAM, LRESULT, WPARAM};
-
-#[cfg(test)]
-mod tests;
+pub use icrate::Foundation::{NSArray, NSObject, NSPoint};
```

### Comparing `accesskit-0.1.8/platforms/windows/src/node.rs` & `accesskit-0.2.0/platforms/windows/src/node.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/windows/src/subclass.rs` & `accesskit-0.2.0/platforms/windows/src/subclass.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,65 @@
 // Copyright 2022 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
-use accesskit::{ActionHandler, TreeUpdate};
-use once_cell::unsync::Lazy;
-use std::{cell::Cell, ffi::c_void, mem::transmute, rc::Rc};
+use accesskit::{ActionHandler, ActivationHandler, TreeUpdate};
+use std::{
+    cell::{Cell, RefCell},
+    ffi::c_void,
+    mem::transmute,
+};
 use windows::{
     core::*,
     Win32::{Foundation::*, UI::WindowsAndMessaging::*},
 };
 
-use crate::{Adapter, QueuedEvents, UiaInitMarker};
+use crate::{Adapter, QueuedEvents};
 
 fn win32_error() -> ! {
     panic!("{}", Error::from_win32())
 }
 
 // Work around a difference between the SetWindowLongPtrW API definition
 // in windows-rs on 32-bit and 64-bit Windows.
 #[cfg(any(target_arch = "x86_64", target_arch = "aarch64"))]
 type LongPtr = isize;
 #[cfg(not(any(target_arch = "x86_64", target_arch = "aarch64")))]
 type LongPtr = i32;
 
 const PROP_NAME: PCWSTR = w!("AccessKitAdapter");
 
-type LazyAdapter = Lazy<Adapter, Box<dyn FnOnce() -> Adapter>>;
+struct SubclassState {
+    adapter: Adapter,
+    activation_handler: Box<dyn ActivationHandler>,
+}
 
 struct SubclassImpl {
     hwnd: HWND,
-    is_window_focused: Rc<Cell<bool>>,
-    adapter: LazyAdapter,
+    state: RefCell<SubclassState>,
     prev_wnd_proc: WNDPROC,
     window_destroyed: Cell<bool>,
 }
 
 extern "system" fn wnd_proc(window: HWND, message: u32, wparam: WPARAM, lparam: LPARAM) -> LRESULT {
     let handle = unsafe { GetPropW(window, PROP_NAME) };
     let impl_ptr = handle.0 as *const SubclassImpl;
     assert!(!impl_ptr.is_null());
     let r#impl = unsafe { &*impl_ptr };
     match message {
         WM_GETOBJECT => {
-            let adapter = Lazy::force(&r#impl.adapter);
-            if let Some(result) = adapter.handle_wm_getobject(wparam, lparam) {
+            let mut state = r#impl.state.borrow_mut();
+            let state_mut = &mut *state;
+            if let Some(result) = state_mut.adapter.handle_wm_getobject(
+                wparam,
+                lparam,
+                &mut *state_mut.activation_handler,
+            ) {
+                drop(state);
                 return result.into();
             }
         }
         WM_SETFOCUS | WM_EXITMENULOOP | WM_EXITSIZEMOVE => {
             r#impl.update_window_focus_state(true);
         }
         WM_KILLFOCUS | WM_ENTERMENULOOP | WM_ENTERSIZEMOVE => {
@@ -61,35 +72,25 @@
     }
     unsafe { CallWindowProcW(r#impl.prev_wnd_proc, window, message, wparam, lparam) }
 }
 
 impl SubclassImpl {
     fn new(
         hwnd: HWND,
-        source: impl 'static + FnOnce() -> TreeUpdate,
-        action_handler: Box<dyn ActionHandler + Send>,
+        activation_handler: impl 'static + ActivationHandler,
+        action_handler: impl 'static + ActionHandler + Send,
     ) -> Box<Self> {
-        let is_window_focused = Rc::new(Cell::new(false));
-        let uia_init_marker = UiaInitMarker::new();
-        let adapter: LazyAdapter = Lazy::new(Box::new({
-            let is_window_focused = Rc::clone(&is_window_focused);
-            move || {
-                Adapter::new(
-                    hwnd,
-                    source(),
-                    is_window_focused.get(),
-                    action_handler,
-                    uia_init_marker,
-                )
-            }
-        }));
+        let adapter = Adapter::new(hwnd, false, action_handler);
+        let state = RefCell::new(SubclassState {
+            adapter,
+            activation_handler: Box::new(activation_handler),
+        });
         Box::new(Self {
             hwnd,
-            is_window_focused,
-            adapter,
+            state,
             prev_wnd_proc: None,
             window_destroyed: Cell::new(false),
         })
     }
 
     fn install(&mut self) {
         unsafe {
@@ -105,17 +106,17 @@
         if result == 0 {
             win32_error();
         }
         self.prev_wnd_proc = unsafe { transmute::<LongPtr, WNDPROC>(result) };
     }
 
     fn update_window_focus_state(&self, is_focused: bool) {
-        self.is_window_focused.set(is_focused);
-        if let Some(adapter) = Lazy::get(&self.adapter) {
-            let events = adapter.update_window_focus_state(is_focused);
+        let mut state = self.state.borrow_mut();
+        if let Some(events) = state.adapter.update_window_focus_state(is_focused) {
+            drop(state);
             events.raise();
         }
     }
 
     fn uninstall(&self) {
         if self.window_destroyed.get() {
             return;
@@ -141,53 +142,46 @@
 pub struct SubclassingAdapter(Box<SubclassImpl>);
 
 impl SubclassingAdapter {
     /// Creates a new Windows platform adapter using window subclassing.
     /// This must be done before the window is shown or focused
     /// for the first time.
     ///
-    /// The action handler may or may not be called on the thread that owns
-    /// the window.
+    /// This must be called on the thread that owns the window. The activation
+    /// handler will always be called on that thread. The action handler
+    /// may or may not be called on that thread.
     pub fn new(
         hwnd: HWND,
-        source: impl 'static + FnOnce() -> TreeUpdate,
-        action_handler: Box<dyn ActionHandler + Send>,
+        activation_handler: impl 'static + ActivationHandler,
+        action_handler: impl 'static + ActionHandler + Send,
     ) -> Self {
-        let mut r#impl = SubclassImpl::new(hwnd, source, action_handler);
+        let mut r#impl = SubclassImpl::new(hwnd, activation_handler, action_handler);
         r#impl.install();
         Self(r#impl)
     }
 
-    /// Initialize the tree if it hasn't been initialized already, then apply
-    /// the provided update.
-    ///
-    /// The caller must call [`QueuedEvents::raise`] on the return value.
-    ///
-    /// This method may be safely called on any thread, but refer to
-    /// [`QueuedEvents::raise`] for restrictions on the context in which
-    /// it should be called.
-    pub fn update(&self, update: TreeUpdate) -> QueuedEvents {
-        let adapter = Lazy::force(&self.0.adapter);
-        adapter.update(update)
-    }
-
     /// If and only if the tree has been initialized, call the provided function
-    /// and apply the resulting update.
+    /// and apply the resulting update. Note: If the caller's implementation of
+    /// [`ActivationHandler::request_initial_tree`] initially returned `None`,
+    /// the [`TreeUpdate`] returned by the provided function must contain
+    /// a full tree.
     ///
     /// If a [`QueuedEvents`] instance is returned, the caller must call
     /// [`QueuedEvents::raise`] on it.
-    ///
-    /// This method may be safely called on any thread, but refer to
-    /// [`QueuedEvents::raise`] for restrictions on the context in which
-    /// it should be called.
     pub fn update_if_active(
-        &self,
+        &mut self,
         update_factory: impl FnOnce() -> TreeUpdate,
     ) -> Option<QueuedEvents> {
-        Lazy::get(&self.0.adapter).map(|adapter| adapter.update(update_factory()))
+        // SAFETY: We use `RefCell::borrow_mut` here, even though
+        // `RefCell::get_mut` is allowed (because this method takes
+        // a mutable self reference), just in case there's some way
+        // this method can be called from within the subclassed window
+        // procedure, e.g. via `ActivationHandler`.
+        let mut state = self.0.state.borrow_mut();
+        state.adapter.update_if_active(update_factory)
     }
 }
 
 impl Drop for SubclassingAdapter {
     fn drop(&mut self) {
         self.0.uninstall();
     }
```

### Comparing `accesskit-0.1.8/platforms/windows/src/tests/mod.rs` & `accesskit-0.2.0/platforms/windows/src/tests/mod.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 // Copyright 2022 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
-use accesskit::{ActionHandler, TreeUpdate};
-use once_cell::{sync::Lazy as SyncLazy, unsync::Lazy};
+use accesskit::{ActionHandler, ActivationHandler};
+use once_cell::sync::Lazy;
 use std::{
     cell::RefCell,
-    rc::Rc,
     sync::{Arc, Condvar, Mutex},
     thread,
     time::Duration,
 };
 use windows as Windows;
 use windows::{
     core::*,
@@ -19,19 +18,22 @@
         Foundation::*,
         Graphics::Gdi::ValidateRect,
         System::{Com::*, LibraryLoader::GetModuleHandleW},
         UI::{Accessibility::*, WindowsAndMessaging::*},
     },
 };
 
-use super::{Adapter, UiaInitMarker};
+use super::{
+    context::{ActionHandlerNoMut, ActionHandlerWrapper},
+    Adapter,
+};
 
 const DEFAULT_TIMEOUT: Duration = Duration::from_secs(5);
 
-static WINDOW_CLASS_ATOM: SyncLazy<u16> = SyncLazy::new(|| {
+static WINDOW_CLASS_ATOM: Lazy<u16> = Lazy::new(|| {
     let class_name = w!("AccessKitTest");
 
     let wc = WNDCLASSW {
         hCursor: unsafe { LoadCursorW(None, IDC_ARROW) }.unwrap(),
         hInstance: unsafe { GetModuleHandleW(None) }.unwrap().into(),
         lpszClassName: class_name,
         style: CS_HREDRAW | CS_VREDRAW,
@@ -42,93 +44,80 @@
     let atom = unsafe { RegisterClassW(&wc) };
     if atom == 0 {
         panic!("{}", Error::from_win32());
     }
     atom
 });
 
-struct InnerWindowState {
-    is_window_focused: bool,
-}
-
-type LazyAdapter = Lazy<Adapter, Box<dyn FnOnce() -> Adapter>>;
-
 struct WindowState {
-    adapter: LazyAdapter,
-    inner_state: Rc<RefCell<InnerWindowState>>,
+    activation_handler: RefCell<Box<dyn ActivationHandler>>,
+    adapter: RefCell<Adapter>,
 }
 
 unsafe fn get_window_state(window: HWND) -> *const WindowState {
     GetWindowLongPtrW(window, GWLP_USERDATA) as _
 }
 
-fn update_window_focus_state(window: HWND, is_window_focused: bool) {
-    let window_state = unsafe { &*get_window_state(window) };
-    let mut inner_state = window_state.inner_state.borrow_mut();
-    inner_state.is_window_focused = is_window_focused;
-    drop(inner_state);
-    if let Some(adapter) = Lazy::get(&window_state.adapter) {
-        let events = adapter.update_window_focus_state(is_window_focused);
+fn update_window_focus_state(window: HWND, is_focused: bool) {
+    let state = unsafe { &*get_window_state(window) };
+    let mut adapter = state.adapter.borrow_mut();
+    if let Some(events) = adapter.update_window_focus_state(is_focused) {
         events.raise();
     }
 }
 
-struct WindowCreateParams(TreeUpdate, Box<dyn ActionHandler + Send + Sync>);
+struct WindowCreateParams {
+    activation_handler: Box<dyn ActivationHandler>,
+    action_handler: Arc<dyn ActionHandlerNoMut + Send + Sync>,
+}
 
 extern "system" fn wndproc(window: HWND, message: u32, wparam: WPARAM, lparam: LPARAM) -> LRESULT {
     match message {
         WM_NCCREATE => {
             let create_struct: &CREATESTRUCTW = unsafe { &mut *(lparam.0 as *mut _) };
             let create_params: Box<WindowCreateParams> =
                 unsafe { Box::from_raw(create_struct.lpCreateParams as _) };
-            let WindowCreateParams(initial_state, action_handler) = *create_params;
-            let inner_state = Rc::new(RefCell::new(InnerWindowState {
-                is_window_focused: false,
-            }));
-            let inner_state_for_tree_init = inner_state.clone();
-            let uia_init_marker = UiaInitMarker::new();
+            let WindowCreateParams {
+                activation_handler,
+                action_handler,
+            } = *create_params;
+            let adapter = Adapter::with_wrapped_action_handler(window, false, action_handler);
             let state = Box::new(WindowState {
-                adapter: Lazy::new(Box::new(move || {
-                    let state = inner_state_for_tree_init.borrow();
-                    Adapter::new(
-                        window,
-                        initial_state,
-                        state.is_window_focused,
-                        action_handler,
-                        uia_init_marker,
-                    )
-                })),
-                inner_state,
+                activation_handler: RefCell::new(activation_handler),
+                adapter: RefCell::new(adapter),
             });
             unsafe { SetWindowLongPtrW(window, GWLP_USERDATA, Box::into_raw(state) as _) };
             unsafe { DefWindowProcW(window, message, wparam, lparam) }
         }
         WM_PAINT => {
             unsafe { ValidateRect(window, None) }.unwrap();
             LRESULT(0)
         }
         WM_DESTROY => {
             let ptr = unsafe { SetWindowLongPtrW(window, GWLP_USERDATA, 0) };
             if ptr != 0 {
-                let _dropped: Box<WindowState> = unsafe { Box::from_raw(ptr as _) };
+                drop(unsafe { Box::<WindowState>::from_raw(ptr as _) });
             }
             unsafe { PostQuitMessage(0) };
             LRESULT(0)
         }
         WM_GETOBJECT => {
-            let window_state = unsafe { get_window_state(window) };
-            if window_state.is_null() {
+            let state_ptr = unsafe { get_window_state(window) };
+            if state_ptr.is_null() {
                 // We need to be prepared to gracefully handle WM_GETOBJECT
                 // while the window is being destroyed; this can happen if
                 // the thread is using a COM STA.
                 return unsafe { DefWindowProcW(window, message, wparam, lparam) };
             }
-            let window_state = unsafe { &*window_state };
-            let adapter = Lazy::force(&window_state.adapter);
-            let result = adapter.handle_wm_getobject(wparam, lparam);
+            let state = unsafe { &*state_ptr };
+            let mut adapter = state.adapter.borrow_mut();
+            let mut activation_handler = state.activation_handler.borrow_mut();
+            let result = adapter.handle_wm_getobject(wparam, lparam, &mut **activation_handler);
+            drop(activation_handler);
+            drop(adapter);
             result.map_or_else(
                 || unsafe { DefWindowProcW(window, message, wparam, lparam) },
                 |result| result.into(),
             )
         }
         WM_SETFOCUS | WM_EXITMENULOOP | WM_EXITSIZEMOVE => {
             update_window_focus_state(window, true);
@@ -140,18 +129,21 @@
         }
         _ => unsafe { DefWindowProcW(window, message, wparam, lparam) },
     }
 }
 
 fn create_window(
     title: &str,
-    initial_state: TreeUpdate,
-    action_handler: Box<dyn ActionHandler + Send + Sync>,
+    activation_handler: impl 'static + ActivationHandler,
+    action_handler: impl 'static + ActionHandler + Send,
 ) -> Result<HWND> {
-    let create_params = Box::new(WindowCreateParams(initial_state, action_handler));
+    let create_params = Box::new(WindowCreateParams {
+        activation_handler: Box::new(activation_handler),
+        action_handler: Arc::new(ActionHandlerWrapper::new(action_handler)),
+    });
 
     let window = unsafe {
         CreateWindowExW(
             Default::default(),
             PCWSTR(*WINDOW_CLASS_ATOM as usize as _),
             &HSTRING::from(title),
             WS_OVERLAPPEDWINDOW,
@@ -185,16 +177,16 @@
 }
 
 // It's not safe to run these UI-related tests concurrently.
 pub(crate) static MUTEX: Mutex<()> = Mutex::new(());
 
 pub(crate) fn scope<F>(
     window_title: &str,
-    initial_state: TreeUpdate,
-    action_handler: Box<dyn ActionHandler + Send + Sync>,
+    activation_handler: impl 'static + ActivationHandler + Send,
+    action_handler: impl 'static + ActionHandler + Send,
     f: F,
 ) -> Result<()>
 where
     F: FnOnce(&Scope) -> Result<()>,
 {
     let _lock_guard = MUTEX.lock().unwrap();
 
@@ -206,15 +198,15 @@
             // We explicitly don't want to initialize COM on the provider thread,
             // because we want to make sure that the provider side of UIA works
             // even if COM is never initialized on the provider thread
             // (as is the case if the window is never shown), or if COM is
             // initialized after the window is shown (as is the case,
             // at least on some Windows 10 machines, due to IME support).
 
-            let window = create_window(window_title, initial_state, action_handler).unwrap();
+            let window = create_window(window_title, activation_handler, action_handler).unwrap();
 
             {
                 let mut state = window_mutex.lock().unwrap();
                 *state = Some(window);
                 window_cv.notify_one();
             }
```

### Comparing `accesskit-0.1.8/platforms/windows/src/tests/simple.rs` & `accesskit-0.2.0/platforms/windows/src/tests/simple.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 // Copyright 2022 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
 use accesskit::{
-    Action, ActionHandler, ActionRequest, Node, NodeBuilder, NodeClassSet, NodeId, Role, Tree,
-    TreeUpdate,
+    Action, ActionHandler, ActionRequest, ActivationHandler, Node, NodeBuilder, NodeClassSet,
+    NodeId, Role, Tree, TreeUpdate,
 };
 use windows::{core::*, Win32::UI::Accessibility::*};
 
 use super::*;
 
 const WINDOW_TITLE: &str = "Simple test";
 
@@ -46,22 +46,30 @@
 
 pub struct NullActionHandler;
 
 impl ActionHandler for NullActionHandler {
     fn do_action(&mut self, _request: ActionRequest) {}
 }
 
+struct SimpleActivationHandler;
+
+impl ActivationHandler for SimpleActivationHandler {
+    fn request_initial_tree(&mut self) -> Option<TreeUpdate> {
+        Some(get_initial_state())
+    }
+}
+
 fn scope<F>(f: F) -> Result<()>
 where
     F: FnOnce(&Scope) -> Result<()>,
 {
     super::scope(
         WINDOW_TITLE,
-        get_initial_state(),
-        Box::new(NullActionHandler {}),
+        SimpleActivationHandler {},
+        NullActionHandler {},
         f,
     )
 }
 
 #[test]
 fn has_native_uia() -> Result<()> {
     scope(|s| {
```

### Comparing `accesskit-0.1.8/platforms/windows/src/tests/subclassed.rs` & `accesskit-0.2.0/platforms/windows/src/tests/subclassed.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 // Copyright 2022 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
 use accesskit::{
-    Action, ActionHandler, ActionRequest, Node, NodeBuilder, NodeClassSet, NodeId, Role, Tree,
-    TreeUpdate,
+    Action, ActionHandler, ActionRequest, ActivationHandler, Node, NodeBuilder, NodeClassSet,
+    NodeId, Role, Tree, TreeUpdate,
 };
 use windows::Win32::{Foundation::*, UI::Accessibility::*};
 use winit::{
     event_loop::EventLoopBuilder,
     platform::windows::EventLoopBuilderExtWindows,
     raw_window_handle::{HasWindowHandle, RawWindowHandle},
     window::WindowBuilder,
@@ -54,14 +54,22 @@
 
 pub struct NullActionHandler;
 
 impl ActionHandler for NullActionHandler {
     fn do_action(&mut self, _request: ActionRequest) {}
 }
 
+struct SimpleActivationHandler;
+
+impl ActivationHandler for SimpleActivationHandler {
+    fn request_initial_tree(&mut self) -> Option<TreeUpdate> {
+        Some(get_initial_state())
+    }
+}
+
 // This module uses winit for the purpose of testing with a real third-party
 // window implementation that we don't control.
 
 #[test]
 fn has_native_uia() {
     // This test is simple enough that we know it's fine to run entirely
     // on one thread, so we don't need a full multithreaded test harness.
@@ -78,12 +86,12 @@
         .build(&event_loop)
         .unwrap();
     let hwnd = match window.window_handle().unwrap().as_raw() {
         RawWindowHandle::Win32(handle) => HWND(handle.hwnd.get()),
         RawWindowHandle::WinRt(_) => unimplemented!(),
         _ => unreachable!(),
     };
-    let adapter = SubclassingAdapter::new(hwnd, get_initial_state, Box::new(NullActionHandler {}));
+    let adapter = SubclassingAdapter::new(hwnd, SimpleActivationHandler {}, NullActionHandler {});
     assert!(unsafe { UiaHasServerSideProvider(hwnd) }.as_bool());
     drop(window);
     drop(adapter);
 }
```

### Comparing `accesskit-0.1.8/platforms/windows/src/text.rs` & `accesskit-0.2.0/platforms/windows/src/text.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/windows/src/util.rs` & `accesskit-0.2.0/platforms/windows/src/util.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/macos/Cargo.toml` & `accesskit-0.2.0/platforms/macos/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [package]
 name = "accesskit_macos"
-version = "0.11.1"
+version = "0.12.0"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: macOS adapter"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
 edition.workspace = true
 rust-version.workspace = true
 
 [package.metadata.docs.rs]
 default-target = "x86_64-apple-darwin"
 
 [dependencies]
-accesskit = { version = "0.12.3", path = "../../common" }
-accesskit_consumer = { version = "0.17.1", path = "../../consumer" }
+accesskit = { version = "0.13.0", path = "../../common" }
+accesskit_consumer = { version = "0.18.0", path = "../../consumer" }
 objc2 = "0.5.0"
 once_cell = "1.13.0"
 
 [dependencies.icrate]
 version = "0.1.0"
 features = [
     "AppKit",
```

### Comparing `accesskit-0.1.8/platforms/macos/CHANGELOG.md` & `accesskit-0.2.0/platforms/macos/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,38 @@
     * accesskit_consumer bumped from 0.16.0 to 0.16.1
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_consumer bumped from 0.17.0 to 0.17.1
 
+## [0.12.0](https://github.com/AccessKit/accesskit/compare/accesskit_macos-v0.11.1...accesskit_macos-v0.12.0) (2024-04-14)
+
+
+### ⚠ BREAKING CHANGES
+
+* New approach to lazy initialization ([#375](https://github.com/AccessKit/accesskit/issues/375))
+
+### Bug Fixes
+
+* Fix new compiler warning in Rust 1.77 ([#376](https://github.com/AccessKit/accesskit/issues/376)) ([1de7c63](https://github.com/AccessKit/accesskit/commit/1de7c63e7db12bc7eda57a191e913fef0e572f43))
+
+
+### Code Refactoring
+
+* New approach to lazy initialization ([#375](https://github.com/AccessKit/accesskit/issues/375)) ([9baebdc](https://github.com/AccessKit/accesskit/commit/9baebdceed7300389b6768815d7ae48f1ce401e4))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit bumped from 0.12.3 to 0.13.0
+    * accesskit_consumer bumped from 0.17.1 to 0.18.0
+
 ## [0.11.0](https://github.com/AccessKit/accesskit/compare/accesskit_macos-v0.10.1...accesskit_macos-v0.11.0) (2024-01-03)
 
 
 ### Features
 
 * Support custom role descriptions ([#316](https://github.com/AccessKit/accesskit/issues/316)) ([c8d1a56](https://github.com/AccessKit/accesskit/commit/c8d1a5638fa6c33adfa059815c04f7e043c56026))
```

### Comparing `accesskit-0.1.8/platforms/macos/src/context.rs` & `accesskit-0.2.0/platforms/macos/src/context.rs`

 * *Files 12% similar despite different names*

```diff
@@ -7,35 +7,53 @@
 use accesskit_consumer::Tree;
 use icrate::{AppKit::*, Foundation::MainThreadMarker};
 use objc2::rc::{Id, WeakId};
 use std::{cell::RefCell, collections::HashMap, rc::Rc};
 
 use crate::node::PlatformNode;
 
+pub(crate) trait ActionHandlerNoMut {
+    fn do_action(&self, request: ActionRequest);
+}
+
+pub(crate) struct ActionHandlerWrapper<H: ActionHandler>(RefCell<H>);
+
+impl<H: 'static + ActionHandler> ActionHandlerWrapper<H> {
+    pub(crate) fn new(inner: H) -> Self {
+        Self(RefCell::new(inner))
+    }
+}
+
+impl<H: ActionHandler> ActionHandlerNoMut for ActionHandlerWrapper<H> {
+    fn do_action(&self, request: ActionRequest) {
+        self.0.borrow_mut().do_action(request)
+    }
+}
+
 pub(crate) struct Context {
     pub(crate) view: WeakId<NSView>,
     pub(crate) tree: RefCell<Tree>,
-    pub(crate) action_handler: RefCell<Box<dyn ActionHandler>>,
+    pub(crate) action_handler: Rc<dyn ActionHandlerNoMut>,
     platform_nodes: RefCell<HashMap<NodeId, Id<PlatformNode>>>,
-    _mtm: MainThreadMarker,
+    pub(crate) mtm: MainThreadMarker,
 }
 
 impl Context {
     pub(crate) fn new(
         view: WeakId<NSView>,
         tree: Tree,
-        action_handler: Box<dyn ActionHandler>,
+        action_handler: Rc<dyn ActionHandlerNoMut>,
         mtm: MainThreadMarker,
     ) -> Rc<Self> {
         Rc::new(Self {
             view,
             tree: RefCell::new(tree),
-            action_handler: RefCell::new(action_handler),
+            action_handler,
             platform_nodes: RefCell::new(HashMap::new()),
-            _mtm: mtm,
+            mtm,
         })
     }
 
     pub(crate) fn get_or_create_platform_node(self: &Rc<Self>, id: NodeId) -> Id<PlatformNode> {
         let mut platform_nodes = self.platform_nodes.borrow_mut();
         if let Some(result) = platform_nodes.get(&id) {
             return result.clone();
@@ -48,15 +66,15 @@
 
     pub(crate) fn remove_platform_node(&self, id: NodeId) -> Option<Id<PlatformNode>> {
         let mut platform_nodes = self.platform_nodes.borrow_mut();
         platform_nodes.remove(&id)
     }
 
     pub(crate) fn do_action(&self, request: ActionRequest) {
-        self.action_handler.borrow_mut().do_action(request);
+        self.action_handler.do_action(request);
     }
 }
 
 impl Drop for Context {
     fn drop(&mut self) {
         let platform_nodes = self.platform_nodes.borrow();
         for platform_node in platform_nodes.values() {
```

### Comparing `accesskit-0.1.8/platforms/macos/src/event.rs` & `accesskit-0.2.0/platforms/macos/src/event.rs`

 * *Files 3% similar despite different names*

```diff
@@ -110,27 +110,38 @@
 #[must_use = "events must be explicitly raised"]
 pub struct QueuedEvents {
     context: Rc<Context>,
     events: Vec<QueuedEvent>,
 }
 
 impl QueuedEvents {
+    pub(crate) fn new(context: Rc<Context>, events: Vec<QueuedEvent>) -> Self {
+        Self { context, events }
+    }
+
     /// Raise all queued events synchronously.
     ///
     /// It is unknown whether accessibility methods on the view may be
     /// called while events are being raised. This means that any locks
     /// or runtime borrows required to access the adapter must not
     /// be held while this method is called.
     pub fn raise(self) {
         for event in self.events {
             event.raise(&self.context);
         }
     }
 }
 
+pub(crate) fn focus_event(node_id: NodeId) -> QueuedEvent {
+    QueuedEvent::Generic {
+        node_id,
+        notification: unsafe { NSAccessibilityFocusedUIElementChangedNotification },
+    }
+}
+
 pub(crate) struct EventGenerator {
     context: Rc<Context>,
     events: Vec<QueuedEvent>,
     text_changed: HashSet<NodeId>,
 }
 
 impl EventGenerator {
@@ -139,18 +150,15 @@
             context,
             events: Vec::new(),
             text_changed: HashSet::new(),
         }
     }
 
     pub(crate) fn into_result(self) -> QueuedEvents {
-        QueuedEvents {
-            context: self.context,
-            events: self.events,
-        }
+        QueuedEvents::new(self.context, self.events)
     }
 
     fn insert_text_change_if_needed_parent(&mut self, node: Node) {
         if !node.supports_text_ranges() {
             return;
         }
         let id = node.id();
@@ -255,18 +263,15 @@
         new_node: Option<&Node>,
         _current_state: &TreeState,
     ) {
         if let Some(new_node) = new_node {
             if filter(new_node) != FilterResult::Include {
                 return;
             }
-            self.events.push(QueuedEvent::Generic {
-                node_id: new_node.id(),
-                notification: unsafe { NSAccessibilityFocusedUIElementChangedNotification },
-            });
+            self.events.push(focus_event(new_node.id()));
         }
     }
 
     fn node_removed(&mut self, node: &DetachedNode, current_state: &TreeState) {
         self.insert_text_change_if_needed_for_removed_node(node, current_state);
         self.events.push(QueuedEvent::NodeDestroyed(node.id()));
     }
```

### Comparing `accesskit-0.1.8/platforms/macos/src/node.rs` & `accesskit-0.2.0/platforms/macos/src/node.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/macos/src/patch.rs` & `accesskit-0.2.0/platforms/macos/src/patch.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/platforms/macos/src/subclass.rs` & `accesskit-0.2.0/platforms/macos/src/subclass.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 // Copyright 2022 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
-use accesskit::{ActionHandler, TreeUpdate};
+use accesskit::{ActionHandler, ActivationHandler, TreeUpdate};
 use icrate::{
     AppKit::{NSView, NSWindow},
     Foundation::{NSArray, NSObject, NSPoint},
 };
 use objc2::{
     declare::ClassBuilder,
     declare_class,
@@ -17,33 +17,35 @@
     },
     msg_send_id,
     mutability::InteriorMutable,
     rc::Id,
     runtime::{AnyClass, Sel},
     sel, ClassType, DeclaredClass,
 };
-use once_cell::{sync::Lazy as SyncLazy, unsync::Lazy};
-use std::{cell::Cell, collections::HashMap, ffi::c_void, rc::Rc, sync::Mutex};
+use once_cell::sync::Lazy;
+use std::{cell::RefCell, collections::HashMap, ffi::c_void, sync::Mutex};
 
 use crate::{event::QueuedEvents, Adapter};
 
-static SUBCLASSES: SyncLazy<Mutex<HashMap<&'static AnyClass, &'static AnyClass>>> =
-    SyncLazy::new(|| Mutex::new(HashMap::new()));
+static SUBCLASSES: Lazy<Mutex<HashMap<&'static AnyClass, &'static AnyClass>>> =
+    Lazy::new(|| Mutex::new(HashMap::new()));
 
-// Declare as mutable to ensure the address is unique.
-static mut ASSOCIATED_OBJECT_KEY: u8 = 0;
+static ASSOCIATED_OBJECT_KEY: u8 = 0;
 
 fn associated_object_key() -> *const c_void {
-    unsafe { &ASSOCIATED_OBJECT_KEY as *const u8 as *const _ }
+    (&ASSOCIATED_OBJECT_KEY as *const u8).cast()
 }
 
-type LazyAdapter = Lazy<Adapter, Box<dyn FnOnce() -> Adapter>>;
+struct AssociatedObjectState {
+    adapter: Adapter,
+    activation_handler: Box<dyn ActivationHandler>,
+}
 
 struct AssociatedObjectIvars {
-    adapter: LazyAdapter,
+    state: RefCell<AssociatedObjectState>,
     prev_class: &'static AnyClass,
 }
 
 declare_class!(
     struct AssociatedObject;
 
     unsafe impl ClassType for AssociatedObject {
@@ -54,19 +56,24 @@
 
     impl DeclaredClass for AssociatedObject {
         type Ivars = AssociatedObjectIvars;
     }
 );
 
 impl AssociatedObject {
-    fn new(adapter: LazyAdapter, prev_class: &'static AnyClass) -> Id<Self> {
-        let this = Self::alloc().set_ivars(AssociatedObjectIvars {
+    fn new(
+        adapter: Adapter,
+        activation_handler: impl 'static + ActivationHandler,
+        prev_class: &'static AnyClass,
+    ) -> Id<Self> {
+        let state = RefCell::new(AssociatedObjectState {
             adapter,
-            prev_class,
+            activation_handler: Box::new(activation_handler),
         });
+        let this = Self::alloc().set_ivars(AssociatedObjectIvars { state, prev_class });
 
         unsafe { msg_send_id![super(this), init] }
     }
 }
 
 fn associated_object(view: &NSView) -> &AssociatedObject {
     unsafe {
@@ -83,35 +90,41 @@
 unsafe extern "C" fn superclass(this: &NSView, _cmd: Sel) -> Option<&AnyClass> {
     let associated = associated_object(this);
     associated.ivars().prev_class.superclass()
 }
 
 unsafe extern "C" fn children(this: &NSView, _cmd: Sel) -> *mut NSArray<NSObject> {
     let associated = associated_object(this);
-    let adapter = Lazy::force(&associated.ivars().adapter);
-    adapter.view_children()
+    let mut state = associated.ivars().state.borrow_mut();
+    let state_mut = &mut *state;
+    state_mut
+        .adapter
+        .view_children(&mut *state_mut.activation_handler)
 }
 
 unsafe extern "C" fn focus(this: &NSView, _cmd: Sel) -> *mut NSObject {
     let associated = associated_object(this);
-    let adapter = Lazy::force(&associated.ivars().adapter);
-    adapter.focus()
+    let mut state = associated.ivars().state.borrow_mut();
+    let state_mut = &mut *state;
+    state_mut.adapter.focus(&mut *state_mut.activation_handler)
 }
 
 unsafe extern "C" fn hit_test(this: &NSView, _cmd: Sel, point: NSPoint) -> *mut NSObject {
     let associated = associated_object(this);
-    let adapter = Lazy::force(&associated.ivars().adapter);
-    adapter.hit_test(point)
+    let mut state = associated.ivars().state.borrow_mut();
+    let state_mut = &mut *state;
+    state_mut
+        .adapter
+        .hit_test(point, &mut *state_mut.activation_handler)
 }
 
 /// Uses dynamic Objective-C subclassing to implement the NSView
 /// accessibility methods when normal subclassing isn't an option.
 pub struct SubclassingAdapter {
     view: Id<NSView>,
-    is_view_focused: Rc<Cell<bool>>,
     associated: Id<AssociatedObject>,
 }
 
 impl SubclassingAdapter {
     /// Create an adapter that dynamically subclasses the specified view.
     /// This must be done before the view is shown or focused for
     /// the first time.
@@ -119,42 +132,34 @@
     /// The action handler will always be called on the main thread.
     ///
     /// # Safety
     ///
     /// `view` must be a valid, unreleased pointer to an `NSView`.
     pub unsafe fn new(
         view: *mut c_void,
-        source: impl 'static + FnOnce() -> TreeUpdate,
-        action_handler: Box<dyn ActionHandler>,
+        activation_handler: impl 'static + ActivationHandler,
+        action_handler: impl 'static + ActionHandler,
     ) -> Self {
         let view = view as *mut NSView;
         let retained_view = unsafe { Id::retain(view) }.unwrap();
-        Self::new_internal(retained_view, source, action_handler)
+        Self::new_internal(retained_view, activation_handler, action_handler)
     }
 
     fn new_internal(
         retained_view: Id<NSView>,
-        source: impl 'static + FnOnce() -> TreeUpdate,
-        action_handler: Box<dyn ActionHandler>,
+        activation_handler: impl 'static + ActivationHandler,
+        action_handler: impl 'static + ActionHandler,
     ) -> Self {
-        let is_view_focused = Rc::new(Cell::new(false));
-        let adapter: LazyAdapter = {
-            let retained_view = retained_view.clone();
-            let is_view_focused = Rc::clone(&is_view_focused);
-            Lazy::new(Box::new(move || {
-                let view = Id::as_ptr(&retained_view) as *mut c_void;
-                unsafe { Adapter::new(view, source(), is_view_focused.get(), action_handler) }
-            }))
-        };
         let view = Id::as_ptr(&retained_view) as *mut NSView;
+        let adapter = unsafe { Adapter::new(view as *mut c_void, false, action_handler) };
         // Cast to a pointer and back to force the lifetime to 'static
         // SAFETY: We know the class will live as long as the instance,
         // and we only use this reference while the instance is alive.
         let prev_class = unsafe { &*((*view).class() as *const AnyClass) };
-        let associated = AssociatedObject::new(adapter, prev_class);
+        let associated = AssociatedObject::new(adapter, activation_handler, prev_class);
         unsafe {
             objc_setAssociatedObject(
                 view as *mut _,
                 associated_object_key(),
                 Id::as_ptr(&associated) as *mut _,
                 OBJC_ASSOCIATION_RETAIN_NONATOMIC,
             )
@@ -186,15 +191,14 @@
         });
         // SAFETY: Changing the view's class is only safe because
         // the subclass doesn't add any instance variables;
         // it uses an associated object instead.
         unsafe { object_setClass(view as *mut _, (*subclass as *const AnyClass).cast()) };
         Self {
             view: retained_view,
-            is_view_focused,
             associated,
         }
     }
 
     /// Create an adapter that dynamically subclasses the content view
     /// of the specified window.
     ///
@@ -206,51 +210,45 @@
     ///
     /// # Panics
     ///
     /// This function panics if the specified window doesn't currently have
     /// a content view.
     pub unsafe fn for_window(
         window: *mut c_void,
-        source: impl 'static + FnOnce() -> TreeUpdate,
-        action_handler: Box<dyn ActionHandler>,
+        activation_handler: impl 'static + ActivationHandler,
+        action_handler: impl 'static + ActionHandler,
     ) -> Self {
         let window = unsafe { &*(window as *const NSWindow) };
         let retained_view = window.contentView().unwrap();
-        Self::new_internal(retained_view, source, action_handler)
-    }
-
-    /// Initialize the tree if it hasn't been initialized already, then apply
-    /// the provided update.
-    ///
-    /// The caller must call [`QueuedEvents::raise`] on the return value.
-    pub fn update(&self, update: TreeUpdate) -> QueuedEvents {
-        let adapter = Lazy::force(&self.associated.ivars().adapter);
-        adapter.update(update)
+        Self::new_internal(retained_view, activation_handler, action_handler)
     }
 
     /// If and only if the tree has been initialized, call the provided function
-    /// and apply the resulting update.
+    /// and apply the resulting update. Note: If the caller's implementation of
+    /// [`ActivationHandler::request_initial_tree`] initially returned `None`,
+    /// the [`TreeUpdate`] returned by the provided function must contain
+    /// a full tree.
     ///
     /// If a [`QueuedEvents`] instance is returned, the caller must call
     /// [`QueuedEvents::raise`] on it.
     pub fn update_if_active(
-        &self,
+        &mut self,
         update_factory: impl FnOnce() -> TreeUpdate,
     ) -> Option<QueuedEvents> {
-        Lazy::get(&self.associated.ivars().adapter).map(|adapter| adapter.update(update_factory()))
+        let mut state = self.associated.ivars().state.borrow_mut();
+        state.adapter.update_if_active(update_factory)
     }
 
     /// Update the tree state based on whether the window is focused.
     ///
     /// If a [`QueuedEvents`] instance is returned, the caller must call
     /// [`QueuedEvents::raise`] on it.
-    pub fn update_view_focus_state(&self, is_focused: bool) -> Option<QueuedEvents> {
-        self.is_view_focused.set(is_focused);
-        Lazy::get(&self.associated.ivars().adapter)
-            .map(|adapter| adapter.update_view_focus_state(is_focused))
+    pub fn update_view_focus_state(&mut self, is_focused: bool) -> Option<QueuedEvents> {
+        let mut state = self.associated.ivars().state.borrow_mut();
+        state.adapter.update_view_focus_state(is_focused)
     }
 }
 
 impl Drop for SubclassingAdapter {
     fn drop(&mut self) {
         let prev_class = self.associated.ivars().prev_class;
         let view = Id::as_ptr(&self.view) as *mut NSView;
```

### Comparing `accesskit-0.1.8/platforms/macos/src/util.rs` & `accesskit-0.2.0/platforms/macos/src/util.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/common/Cargo.toml` & `accesskit-0.2.0/common/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "accesskit"
-version = "0.12.3"
+version = "0.13.0"
 authors.workspace = true
 license.workspace = true
 description = "UI accessibility infrastructure across platforms"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
```

### Comparing `accesskit-0.1.8/common/CHANGELOG.md` & `accesskit-0.2.0/common/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # Changelog
 
+## [0.13.0](https://github.com/AccessKit/accesskit/compare/accesskit-v0.12.3...accesskit-v0.13.0) (2024-04-14)
+
+
+### ⚠ BREAKING CHANGES
+
+* New approach to lazy initialization ([#375](https://github.com/AccessKit/accesskit/issues/375))
+
+### Code Refactoring
+
+* New approach to lazy initialization ([#375](https://github.com/AccessKit/accesskit/issues/375)) ([9baebdc](https://github.com/AccessKit/accesskit/commit/9baebdceed7300389b6768815d7ae48f1ce401e4))
+
 ## [0.12.3](https://github.com/AccessKit/accesskit/compare/accesskit-v0.12.2...accesskit-v0.12.3) (2024-03-07)
 
 
 ### Bug Fixes
 
 * Derive `PartialOrd` and `Ord` on `NodeId` ([#363](https://github.com/AccessKit/accesskit/issues/363)) ([ce3bba1](https://github.com/AccessKit/accesskit/commit/ce3bba1e043d650c406d8814b4f33e9104199c8b))
 * Make `NodeClassSet::new` const ([#368](https://github.com/AccessKit/accesskit/issues/368)) ([11d2968](https://github.com/AccessKit/accesskit/commit/11d2968464d50c3e3f55e9a872d0d454c19e7e51))
```

### Comparing `accesskit-0.1.8/common/README.md` & `accesskit-0.2.0/common/README.md`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/common/src/geometry.rs` & `accesskit-0.2.0/common/src/geometry.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/common/src/lib.rs` & `accesskit-0.2.0/common/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2325,20 +2325,14 @@
     /// host (e.g. window) has focus. If no specific node within the tree
     /// has keyboard focus, this must be set to the root. The latest focus state
     /// must be provided with every tree update, even if the focus state
     /// didn't change in a given update.
     pub focus: NodeId,
 }
 
-impl<T: FnOnce() -> TreeUpdate> From<T> for TreeUpdate {
-    fn from(factory: T) -> Self {
-        factory()
-    }
-}
-
 #[derive(Clone, Debug, PartialEq)]
 #[cfg_attr(feature = "serde", derive(Serialize, Deserialize))]
 #[cfg_attr(feature = "schemars", derive(JsonSchema))]
 #[cfg_attr(feature = "serde", serde(rename_all = "camelCase"))]
 #[repr(C)]
 pub enum ActionData {
     CustomAction(i32),
@@ -2363,20 +2357,58 @@
 #[cfg_attr(feature = "serde", serde(rename_all = "camelCase"))]
 pub struct ActionRequest {
     pub action: Action,
     pub target: NodeId,
     pub data: Option<ActionData>,
 }
 
+/// Handles activation of the application's accessibility implementation.
+pub trait ActivationHandler {
+    /// Requests a [`TreeUpdate`] with a full tree. If the application
+    /// can generate the tree synchronously within this method call,
+    /// it should do so and return the [`TreeUpdate`]. Otherwise,
+    /// it must send the update to the platform adapter asynchronously,
+    /// no later than the next display refresh, even if a frame would not
+    /// normally be rendered due to user input or other activity.
+    /// The application should not return or send a placeholder [`TreeUpdate`];
+    /// the platform adapter will provide one if necessary until the real
+    /// tree is sent.
+    ///
+    /// The primary purpose of this method is to allow the application
+    /// to lazily initialize its accessibility implementation. However,
+    /// this method may be called consecutively without any call to
+    /// [`DeactivationHandler::deactivate_accessibility`]; this typically happens
+    /// if the platform adapter merely forwards tree updates to assistive
+    /// technologies without maintaining any state. A call to this method
+    /// must always generate a [`TreeUpdate`] with a full tree, even if
+    /// the application normally sends incremental updates.
+    ///
+    /// The thread on which this method is called is platform-dependent.
+    /// Refer to the platform adapter documentation for more details.
+    fn request_initial_tree(&mut self) -> Option<TreeUpdate>;
+}
+
 /// Handles requests from assistive technologies or other clients.
 pub trait ActionHandler {
     /// Perform the requested action. If the requested action is not supported,
     /// this method must do nothing.
     ///
     /// The thread on which this method is called is platform-dependent.
     /// Refer to the platform adapter documentation for more details.
     ///
     /// This method may queue the request and handle it asynchronously.
     /// This behavior is preferred over blocking, e.g. when dispatching
     /// the request to another thread.
     fn do_action(&mut self, request: ActionRequest);
 }
+
+/// Handles deactivation of the application's accessibility implementation.
+pub trait DeactivationHandler {
+    /// Deactivate the application's accessibility implementation and drop any
+    /// associated data that can be reconstructed later. After this method
+    /// is called, if an accessibility tree is needed again, the platform
+    /// adapter will call [`ActivationHandler::request_initial_tree`] again.
+    ///
+    /// The thread on which this method is called is platform-dependent.
+    /// Refer to the platform adapter documentation for more details.
+    fn deactivate_accessibility(&mut self);
+}
```

### Comparing `accesskit-0.1.8/bindings/python/Cargo.toml` & `accesskit-0.2.0/bindings/python/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "accesskit_python"
-version = "0.1.8"
+version = "0.2.0"
 authors.workspace = true
 license.workspace = true
 description = "Python bindings to the AccessKit library"
 readme = "README.md"
 publish = false
 edition.workspace = true
 
@@ -13,19 +13,19 @@
 crate-type = ["cdylib"]
 doc = false
 
 [features]
 extension-module = ["pyo3/extension-module"]
 
 [dependencies]
-accesskit = { version = "0.12.3", path = "../../common", features = ["pyo3"] }
+accesskit = { version = "0.13.0", path = "../../common", features = ["pyo3"] }
 pyo3 = { version = "0.20", features = ["abi3-py38", "multiple-pymethods"] }
 
 [target.'cfg(target_os = "windows")'.dependencies]
-accesskit_windows = { version = "0.16.4", path = "../../platforms/windows" }
+accesskit_windows = { version = "0.17.0", path = "../../platforms/windows" }
 
 [target.'cfg(target_os = "macos")'.dependencies]
-accesskit_macos = { version = "0.11.1", path = "../../platforms/macos" }
+accesskit_macos = { version = "0.12.0", path = "../../platforms/macos" }
 
 [target.'cfg(any(target_os = "linux", target_os = "dragonfly", target_os = "freebsd", target_os = "openbsd", target_os = "netbsd"))'.dependencies]
-accesskit_unix = { version = "0.7.5", path = "../../platforms/unix" }
+accesskit_unix = { version = "0.8.0", path = "../../platforms/unix" }
```

### Comparing `accesskit-0.1.8/bindings/python/README.md` & `accesskit-0.2.0/bindings/python/README.md`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/bindings/python/examples/pygame/.gitignore` & `accesskit-0.2.0/bindings/python/examples/pygame/.gitignore`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/bindings/python/examples/pygame/hello_world.py` & `accesskit-0.2.0/bindings/python/examples/pygame/hello_world.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,27 +37,29 @@
     builder = accesskit.NodeBuilder(accesskit.Role.STATIC_TEXT)
     builder.set_name(text)
     builder.set_live(accesskit.Live.POLITE)
     return builder.build(classes)
 
 
 class PygameAdapter:
-    def __init__(self, source, action_handler):
+    def __init__(self, activation_handler, action_handler, deactivation_handler):
         if PLATFORM_SYSTEM == "Darwin":
             accesskit.macos.add_focus_forwarder_to_window_class("SDLWindow")
             window = pygame.display.get_wm_info()["window"]
             self.adapter = accesskit.macos.SubclassingAdapter.for_window(
-                window, source, action_handler
+                window, activation_handler, action_handler
             )
         elif os.name == "posix":
-            self.adapter = accesskit.unix.Adapter(source, action_handler)
+            self.adapter = accesskit.unix.Adapter(
+                activation_handler, action_handler, deactivation_handler
+            )
         elif PLATFORM_SYSTEM == "Windows":
             hwnd = pygame.display.get_wm_info()["window"]
             self.adapter = accesskit.windows.SubclassingAdapter(
-                hwnd, source, action_handler
+                hwnd, activation_handler, action_handler
             )
 
     def update_if_active(self, update_factory):
         events = self.adapter.update_if_active(update_factory)
         if events is not None:
             events.raise_events()
 
@@ -121,14 +123,19 @@
     def set_focus(self, adapter, focus):
         self.focus = focus
         adapter.update_if_active(self.build_tree_update_for_focus_update)
 
     def build_tree_update_for_focus_update(self):
         return accesskit.TreeUpdate(self.focus)
 
+    def deactivate_accessibility(self):
+        # There's nothing in the state that depends on whether the adapter
+        # is active, so there's nothing to do here.
+        pass
+
 
 def do_action(request):
     if request.action in [accesskit.Action.DEFAULT, accesskit.Action.FOCUS]:
         args = {
             "event": SET_FOCUS_MSG
             if request.action == accesskit.Action.FOCUS
             else DO_DEFAULT_ACTION_MSG,
@@ -150,15 +157,17 @@
         )
     elif os.name == "posix" and PLATFORM_SYSTEM != "Darwin":
         print("Enable Orca with [Super]+[Alt]+[S].")
 
     state = WindowState()
     pygame.display.set_mode((WINDOW_WIDTH, WINDOW_HEIGHT), pygame.HIDDEN)
     pygame.display.set_caption(WINDOW_TITLE)
-    adapter = PygameAdapter(state.build_initial_tree, do_action)
+    adapter = PygameAdapter(
+        state.build_initial_tree, do_action, state.deactivate_accessibility
+    )
     pygame.display.set_mode((WINDOW_WIDTH, WINDOW_HEIGHT), pygame.SHOWN)
     is_running = True
     while is_running:
         for event in pygame.event.get():
             if event.type == pygame.QUIT:
                 is_running = False
             elif event.type == pygame.WINDOWFOCUSGAINED:
```

### Comparing `accesskit-0.1.8/bindings/python/src/common.rs` & `accesskit-0.2.0/bindings/python/src/common.rs`

 * *Files 2% similar despite different names*

```diff
@@ -724,17 +724,56 @@
                     TextSelection::from(&selection).into_py(py),
                 ),
             }),
         })
     }
 }
 
+pub(crate) struct LocalPythonActivationHandler<'a> {
+    pub(crate) py: Python<'a>,
+    pub(crate) handler: Py<PyAny>,
+}
+
+impl accesskit::ActivationHandler for LocalPythonActivationHandler<'_> {
+    fn request_initial_tree(&mut self) -> Option<accesskit::TreeUpdate> {
+        let result = self.handler.call0(self.py).unwrap();
+        result
+            .extract::<Option<TreeUpdate>>(self.py)
+            .unwrap()
+            .map(Into::into)
+    }
+}
+
+pub struct PythonActivationHandler(pub(crate) Py<PyAny>);
+
+impl accesskit::ActivationHandler for PythonActivationHandler {
+    fn request_initial_tree(&mut self) -> Option<accesskit::TreeUpdate> {
+        Python::with_gil(|py| {
+            let result = self.0.call0(py).unwrap();
+            result
+                .extract::<Option<TreeUpdate>>(py)
+                .unwrap()
+                .map(Into::into)
+        })
+    }
+}
+
 pub struct PythonActionHandler(pub(crate) Py<PyAny>);
 
 impl accesskit::ActionHandler for PythonActionHandler {
     fn do_action(&mut self, request: accesskit::ActionRequest) {
         let request = ActionRequest::from(request);
         Python::with_gil(|py| {
             self.0.call(py, (request,), None).unwrap();
         });
     }
 }
+
+pub struct PythonDeactivationHandler(pub(crate) Py<PyAny>);
+
+impl accesskit::DeactivationHandler for PythonDeactivationHandler {
+    fn deactivate_accessibility(&mut self) {
+        Python::with_gil(|py| {
+            self.0.call(py, (), None).unwrap();
+        });
+    }
+}
```

### Comparing `accesskit-0.1.8/bindings/python/src/geometry.rs` & `accesskit-0.2.0/bindings/python/src/geometry.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/bindings/python/src/lib.rs` & `accesskit-0.2.0/bindings/python/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,14 @@
         let unix_module = PyModule::new(py, "unix")?;
         unix_module.add_class::<unix::Adapter>()?;
         m.add_submodule(unix_module)?;
     }
     #[cfg(target_os = "windows")]
     {
         let windows_module = PyModule::new(py, "windows")?;
-        windows_module.add_class::<windows::UiaInitMarker>()?;
         windows_module.add_class::<windows::QueuedEvents>()?;
         windows_module.add_class::<windows::Adapter>()?;
         windows_module.add_class::<windows::SubclassingAdapter>()?;
         m.add_submodule(windows_module)?;
     }
 
     Ok(())
```

### Comparing `accesskit-0.1.8/bindings/python/src/macos.rs` & `accesskit-0.2.0/bindings/python/src/macos.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 // Copyright 2023 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
-use crate::{PythonActionHandler, TreeUpdate};
+use crate::{
+    LocalPythonActivationHandler, PythonActionHandler, PythonActivationHandler, TreeUpdate,
+};
 use accesskit_macos::NSPoint;
 use pyo3::{prelude::*, types::PyCapsule};
 use std::ffi::c_void;
 
 /// This class must only be used from the main thread.
 #[pyclass(module = "accesskit.macos", unsendable)]
 pub struct QueuedEvents(Option<accesskit_macos::QueuedEvents>);
@@ -36,50 +38,79 @@
     ///
     /// The action handler will always be called on the main thread.
     ///
     /// # Safety
     ///
     /// `view` must be a valid, unreleased pointer to an `NSView`.
     #[new]
-    pub unsafe fn new(
-        view: &PyAny,
-        initial_state: TreeUpdate,
-        is_view_focused: bool,
-        handler: Py<PyAny>,
-    ) -> Self {
+    pub unsafe fn new(view: &PyAny, is_view_focused: bool, action_handler: Py<PyAny>) -> Self {
         Self(accesskit_macos::Adapter::new(
             to_void_ptr(view),
-            initial_state.into(),
             is_view_focused,
-            Box::new(PythonActionHandler(handler)),
+            PythonActionHandler(action_handler),
         ))
     }
 
-    /// You must call `accesskit.macos.QueuedEvents.raise_events` on the returned value.
-    pub fn update(&self, update: TreeUpdate) -> QueuedEvents {
-        self.0.update(update.into()).into()
+    /// You must call `accesskit.macos.QueuedEvents.raise_events` on the returned value. It can be `None` if the window is not active.
+    pub fn update_if_active(
+        &mut self,
+        py: Python<'_>,
+        update_factory: Py<PyAny>,
+    ) -> Option<QueuedEvents> {
+        self.0
+            .update_if_active(|| {
+                let update = update_factory.call0(py).unwrap();
+                update.extract::<TreeUpdate>(py).unwrap().into()
+            })
+            .map(Into::into)
     }
 
-    /// You must call `accesskit.macos.QueuedEvents.raise_events` on the returned value.
-    pub fn update_view_focus_state(&self, is_focused: bool) -> QueuedEvents {
-        self.0.update_view_focus_state(is_focused).into()
+    /// You must call `accesskit.macos.QueuedEvents.raise_events` on the returned value. It can be `None` if the window is not active.
+    pub fn update_view_focus_state(&mut self, is_focused: bool) -> Option<QueuedEvents> {
+        self.0.update_view_focus_state(is_focused).map(Into::into)
     }
 
-    pub fn view_children(&self, py: Python<'_>) -> PyResult<Py<PyCapsule>> {
-        let ptr: isize = self.0.view_children() as _;
+    pub fn view_children(
+        &mut self,
+        py: Python<'_>,
+        activation_handler: Py<PyAny>,
+    ) -> PyResult<Py<PyCapsule>> {
+        let mut activation_handler = LocalPythonActivationHandler {
+            py,
+            handler: activation_handler,
+        };
+        let ptr: isize = self.0.view_children(&mut activation_handler) as _;
         Ok(PyCapsule::new(py, ptr, None)?.into())
     }
 
-    pub fn focus(&self, py: Python<'_>) -> PyResult<Py<PyCapsule>> {
-        let ptr: isize = self.0.focus() as _;
+    pub fn focus(
+        &mut self,
+        py: Python<'_>,
+        activation_handler: Py<PyAny>,
+    ) -> PyResult<Py<PyCapsule>> {
+        let mut activation_handler = LocalPythonActivationHandler {
+            py,
+            handler: activation_handler,
+        };
+        let ptr: isize = self.0.focus(&mut activation_handler) as _;
         Ok(PyCapsule::new(py, ptr, None)?.into())
     }
 
-    pub fn hit_test(&self, py: Python<'_>, x: f64, y: f64) -> PyResult<Py<PyCapsule>> {
-        let ptr: isize = self.0.hit_test(NSPoint::new(x, y)) as _;
+    pub fn hit_test(
+        &mut self,
+        py: Python<'_>,
+        x: f64,
+        y: f64,
+        activation_handler: Py<PyAny>,
+    ) -> PyResult<Py<PyCapsule>> {
+        let mut activation_handler = LocalPythonActivationHandler {
+            py,
+            handler: activation_handler,
+        };
+        let ptr: isize = self.0.hit_test(NSPoint::new(x, y), &mut activation_handler) as _;
         Ok(PyCapsule::new(py, ptr, None)?.into())
     }
 }
 
 /// This class must only be used from the main thread.
 #[pyclass(module = "accesskit.macos", unsendable)]
 pub struct SubclassingAdapter(accesskit_macos::SubclassingAdapter);
@@ -92,28 +123,23 @@
     ///
     /// The action handler will always be called on the main thread.
     ///
     /// # Safety
     ///
     /// `view` must be a valid, unreleased pointer to an `NSView`.
     #[new]
-    pub unsafe fn new(view: &PyAny, source: Py<PyAny>, handler: Py<PyAny>) -> Self {
+    pub unsafe fn new(
+        view: &PyAny,
+        activation_handler: Py<PyAny>,
+        action_handler: Py<PyAny>,
+    ) -> Self {
         Self(accesskit_macos::SubclassingAdapter::new(
             to_void_ptr(view),
-            move || {
-                Python::with_gil(|py| {
-                    source
-                        .call0(py)
-                        .unwrap()
-                        .extract::<TreeUpdate>(py)
-                        .unwrap()
-                        .into()
-                })
-            },
-            Box::new(PythonActionHandler(handler)),
+            PythonActivationHandler(activation_handler),
+            PythonActionHandler(action_handler),
         ))
     }
 
     /// Create an adapter that dynamically subclasses the content view
     /// of the specified window.
     ///
     /// The action handler will always be called on the main thread.
@@ -123,52 +149,42 @@
     /// `window` must be a valid, unreleased pointer to an `NSWindow`.
     ///
     /// # Panics
     ///
     /// This function panics if the specified window doesn't currently have
     /// a content view.
     #[staticmethod]
-    pub unsafe fn for_window(window: &PyAny, source: Py<PyAny>, handler: Py<PyAny>) -> Self {
+    pub unsafe fn for_window(
+        window: &PyAny,
+        activation_handler: Py<PyAny>,
+        action_handler: Py<PyAny>,
+    ) -> Self {
         Self(accesskit_macos::SubclassingAdapter::for_window(
             to_void_ptr(window),
-            move || {
-                Python::with_gil(|py| {
-                    source
-                        .call0(py)
-                        .unwrap()
-                        .extract::<crate::TreeUpdate>(py)
-                        .unwrap()
-                        .into()
-                })
-            },
-            Box::new(PythonActionHandler(handler)),
+            PythonActivationHandler(activation_handler),
+            PythonActionHandler(action_handler),
         ))
     }
 
-    /// You must call `accesskit.macos.QueuedEvents.raise_events` on the returned value.
-    pub fn update(&self, update: TreeUpdate) -> QueuedEvents {
-        self.0.update(update.into()).into()
-    }
-
     /// You must call `accesskit.macos.QueuedEvents.raise_events` on the returned value. It can be `None` if the window is not active.
     pub fn update_if_active(
-        &self,
+        &mut self,
         py: Python<'_>,
         update_factory: Py<PyAny>,
     ) -> Option<QueuedEvents> {
         self.0
             .update_if_active(|| {
                 let update = update_factory.call0(py).unwrap();
                 update.extract::<TreeUpdate>(py).unwrap().into()
             })
             .map(Into::into)
     }
 
     /// You must call `accesskit.macos.QueuedEvents.raise_events` on the returned value. It can be `None` if the window is not active.
-    pub fn update_view_focus_state(&self, is_focused: bool) -> Option<QueuedEvents> {
+    pub fn update_view_focus_state(&mut self, is_focused: bool) -> Option<QueuedEvents> {
         self.0.update_view_focus_state(is_focused).map(Into::into)
     }
 }
 
 /// Modifies the specified class, which must be a subclass of `NSWindow`,
 /// to include an `accessibilityFocusedUIElement` method that calls
 /// the corresponding method on the window's content view. This is needed
```

### Comparing `accesskit-0.1.8/bindings/python/src/unix.rs` & `accesskit-0.2.0/bindings/python/src/unix.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 // Copyright 2023 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
-use crate::{PythonActionHandler, Rect, TreeUpdate};
+use crate::{
+    PythonActionHandler, PythonActivationHandler, PythonDeactivationHandler, Rect, TreeUpdate,
+};
 use pyo3::prelude::*;
 
 #[pyclass(module = "accesskit.unix")]
 pub struct Adapter(accesskit_unix::Adapter);
 
 #[pymethods]
 impl Adapter {
+    /// Create a new Unix adapter.
+    ///
+    /// All of the handlers will always be called from another thread.
     #[new]
-    pub fn new(source: Py<PyAny>, action_handler: Py<PyAny>) -> Self {
+    pub fn new(
+        activation_handler: Py<PyAny>,
+        action_handler: Py<PyAny>,
+        deactivation_handler: Py<PyAny>,
+    ) -> Self {
         Self(accesskit_unix::Adapter::new(
-            move || {
-                Python::with_gil(|py| {
-                    source
-                        .call0(py)
-                        .unwrap()
-                        .extract::<TreeUpdate>(py)
-                        .unwrap()
-                        .into()
-                })
-            },
-            Box::new(PythonActionHandler(action_handler)),
+            PythonActivationHandler(activation_handler),
+            PythonActionHandler(action_handler),
+            PythonDeactivationHandler(deactivation_handler),
         ))
     }
 
     pub fn set_root_window_bounds(&mut self, outer: Rect, inner: Rect) {
         self.0.set_root_window_bounds(outer.into(), inner.into());
     }
 
-    pub fn update_if_active(&self, py: Python<'_>, update_factory: Py<PyAny>) {
+    pub fn update_if_active(&mut self, py: Python<'_>, update_factory: Py<PyAny>) {
         self.0.update_if_active(|| {
             let update = update_factory.call0(py).unwrap();
             update.extract::<TreeUpdate>(py).unwrap().into()
         });
     }
 
-    pub fn update_window_focus_state(&self, is_focused: bool) {
+    pub fn update_window_focus_state(&mut self, is_focused: bool) {
         self.0.update_window_focus_state(is_focused);
     }
 }
```

### Comparing `accesskit-0.1.8/bindings/python/src/windows.rs` & `accesskit-0.2.0/bindings/python/src/windows.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,18 @@
 // Copyright 2023 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
-use crate::{PythonActionHandler, TreeUpdate};
+use crate::{
+    LocalPythonActivationHandler, PythonActionHandler, PythonActivationHandler, TreeUpdate,
+};
 use accesskit_windows::{HWND, LPARAM, WPARAM};
 use pyo3::prelude::*;
 
-#[derive(Clone)]
-#[pyclass(module = "accesskit.windows")]
-pub struct UiaInitMarker(accesskit_windows::UiaInitMarker);
-
-#[pymethods]
-impl UiaInitMarker {
-    #[new]
-    pub fn __new__() -> Self {
-        Self(accesskit_windows::UiaInitMarker::new())
-    }
-}
-
-impl From<UiaInitMarker> for accesskit_windows::UiaInitMarker {
-    fn from(marker: UiaInitMarker) -> Self {
-        marker.0
-    }
-}
-
 #[pyclass(module = "accesskit.windows")]
 pub struct QueuedEvents(Option<accesskit_windows::QueuedEvents>);
 
 #[pymethods]
 impl QueuedEvents {
     pub fn raise_events(&mut self) {
         let events = self.0.take().unwrap();
@@ -48,43 +32,58 @@
 #[pymethods]
 impl Adapter {
     /// Creates a new Windows platform adapter.
     ///
     /// The action handler may or may not be called on the thread that owns
     /// the window.
     #[new]
-    pub fn new(
-        hwnd: &PyAny,
-        initial_state: TreeUpdate,
-        is_window_focused: bool,
-        action_handler: Py<PyAny>,
-        uia_init_marker: UiaInitMarker,
-    ) -> Self {
+    pub fn new(hwnd: &PyAny, is_window_focused: bool, action_handler: Py<PyAny>) -> Self {
         Self(accesskit_windows::Adapter::new(
             HWND(cast::<isize>(hwnd)),
-            initial_state.into(),
             is_window_focused,
-            Box::new(PythonActionHandler(action_handler)),
-            uia_init_marker.into(),
+            PythonActionHandler(action_handler),
         ))
     }
 
-    /// You must call `accesskit.windows.QueuedEvents.raise_events` on the returned value.
-    pub fn update(&self, update: TreeUpdate) -> QueuedEvents {
-        self.0.update(update.into()).into()
+    /// You must call `accesskit.windows.QueuedEvents.raise_events` on the returned value. It can be `None` if the window is not active.
+    pub fn update_if_active(
+        &mut self,
+        py: Python<'_>,
+        update_factory: Py<PyAny>,
+    ) -> Option<QueuedEvents> {
+        self.0
+            .update_if_active(|| {
+                let update = update_factory.call0(py).unwrap();
+                update.extract::<TreeUpdate>(py).unwrap().into()
+            })
+            .map(Into::into)
     }
 
     /// You must call `accesskit.windows.QueuedEvents.raise_events` on the returned value.
-    pub fn update_window_focus_state(&self, is_focused: bool) -> QueuedEvents {
-        self.0.update_window_focus_state(is_focused).into()
+    pub fn update_window_focus_state(&mut self, is_focused: bool) -> Option<QueuedEvents> {
+        self.0.update_window_focus_state(is_focused).map(Into::into)
     }
 
-    pub fn handle_wm_getobject(&self, wparam: &PyAny, lparam: &PyAny) -> Option<isize> {
+    pub fn handle_wm_getobject(
+        &mut self,
+        py: Python<'_>,
+        wparam: &PyAny,
+        lparam: &PyAny,
+        activation_handler: Py<PyAny>,
+    ) -> Option<isize> {
+        let mut activation_handler = LocalPythonActivationHandler {
+            py,
+            handler: activation_handler,
+        };
         self.0
-            .handle_wm_getobject(WPARAM(cast::<usize>(wparam)), LPARAM(cast::<isize>(lparam)))
+            .handle_wm_getobject(
+                WPARAM(cast::<usize>(wparam)),
+                LPARAM(cast::<isize>(lparam)),
+                &mut activation_handler,
+            )
             .map(|lresult| lresult.into().0)
     }
 }
 
 #[pyclass(module = "accesskit.windows", unsendable)]
 pub struct SubclassingAdapter(accesskit_windows::SubclassingAdapter);
 
@@ -93,39 +92,25 @@
     /// Creates a new Windows platform adapter using window subclassing.
     /// This must be done before the window is shown or focused
     /// for the first time.
     ///
     /// The action handler may or may not be called on the thread that owns
     /// the window.
     #[new]
-    pub fn new(hwnd: &PyAny, source: Py<PyAny>, action_handler: Py<PyAny>) -> Self {
+    pub fn new(hwnd: &PyAny, activation_handler: Py<PyAny>, action_handler: Py<PyAny>) -> Self {
         Self(accesskit_windows::SubclassingAdapter::new(
             HWND(cast::<isize>(hwnd)),
-            move || {
-                Python::with_gil(|py| {
-                    source
-                        .call0(py)
-                        .unwrap()
-                        .extract::<TreeUpdate>(py)
-                        .unwrap()
-                        .into()
-                })
-            },
-            Box::new(PythonActionHandler(action_handler)),
+            PythonActivationHandler(activation_handler),
+            PythonActionHandler(action_handler),
         ))
     }
 
-    /// You must call `accesskit.windows.QueuedEvents.raise_events` on the returned value.
-    pub fn update(&self, update: TreeUpdate) -> QueuedEvents {
-        self.0.update(update.into()).into()
-    }
-
     /// You must call `accesskit.windows.QueuedEvents.raise_events` on the returned value. It can be `None` if the window is not active.
     pub fn update_if_active(
-        &self,
+        &mut self,
         py: Python<'_>,
         update_factory: Py<PyAny>,
     ) -> Option<QueuedEvents> {
         self.0
             .update_if_active(|| {
                 let update = update_factory.call0(py).unwrap();
                 update.extract::<TreeUpdate>(py).unwrap().into()
```

### Comparing `accesskit-0.1.8/Cargo.lock` & `accesskit-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -16,77 +16,77 @@
 name = "ab_glyph_rasterizer"
 version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c71b1793ee61086797f5c80b6efa2b8ffa6d5dd703f118545808a7f2e27f7046"
 
 [[package]]
 name = "accesskit"
-version = "0.12.3"
+version = "0.13.0"
 dependencies = [
  "enumn",
  "pyo3",
  "schemars",
  "serde",
 ]
 
 [[package]]
 name = "accesskit_atspi_common"
-version = "0.2.0"
+version = "0.3.0"
 dependencies = [
  "accesskit",
  "accesskit_consumer",
  "atspi-common",
  "serde",
  "thiserror",
  "zvariant",
 ]
 
 [[package]]
 name = "accesskit_c"
-version = "0.7.7"
+version = "0.8.0"
 dependencies = [
  "accesskit",
  "accesskit_macos",
  "accesskit_unix",
  "accesskit_windows",
  "paste",
 ]
 
 [[package]]
 name = "accesskit_consumer"
-version = "0.17.1"
+version = "0.18.0"
 dependencies = [
  "accesskit",
 ]
 
 [[package]]
 name = "accesskit_macos"
-version = "0.11.1"
+version = "0.12.0"
 dependencies = [
  "accesskit",
  "accesskit_consumer",
  "icrate 0.1.0",
  "objc2 0.5.0",
  "once_cell",
 ]
 
 [[package]]
 name = "accesskit_python"
-version = "0.1.8"
+version = "0.2.0"
 dependencies = [
  "accesskit",
  "accesskit_macos",
  "accesskit_unix",
  "accesskit_windows",
  "pyo3",
 ]
 
 [[package]]
 name = "accesskit_unix"
-version = "0.7.5"
+version = "0.8.0"
 dependencies = [
  "accesskit",
  "accesskit_atspi_common",
  "async-channel 2.1.1",
  "async-executor",
  "async-task",
  "atspi",
@@ -97,29 +97,29 @@
  "tokio",
  "tokio-stream",
  "zbus",
 ]
 
 [[package]]
 name = "accesskit_windows"
-version = "0.16.4"
+version = "0.17.0"
 dependencies = [
  "accesskit",
  "accesskit_consumer",
  "once_cell",
  "paste",
  "scopeguard",
  "static_assertions",
  "windows",
  "winit",
 ]
 
 [[package]]
 name = "accesskit_winit"
-version = "0.18.7"
+version = "0.19.0"
 dependencies = [
  "accesskit",
  "accesskit_macos",
  "accesskit_unix",
  "accesskit_windows",
  "raw-window-handle 0.5.2",
  "raw-window-handle 0.6.0",
```

### Comparing `accesskit-0.1.8/pyproject.toml` & `accesskit-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/LICENSE-APACHE` & `accesskit-0.2.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/LICENSE-MIT` & `accesskit-0.2.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/LICENSE.chromium` & `accesskit-0.2.0/LICENSE.chromium`

 * *Files identical despite different names*

### Comparing `accesskit-0.1.8/PKG-INFO` & `accesskit-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: accesskit
-Version: 0.1.8
+Version: 0.2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


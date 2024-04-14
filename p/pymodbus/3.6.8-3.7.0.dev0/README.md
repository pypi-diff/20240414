# Comparing `tmp/pymodbus-3.6.8.tar.gz` & `tmp/pymodbus-3.7.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodbus-3.6.8.tar", last modified: Sun Apr 14 08:22:36 2024, max compression
+gzip compressed data, was "pymodbus-3.7.0.dev0.tar", last modified: Tue Mar  5 06:19:53 2024, max compression
```

## Comparing `pymodbus-3.6.8.tar` & `pymodbus-3.7.0.dev0.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2024-04-14 08:22:36.683027 pymodbus-3.6.8/
--rw-r--r--   0 jan        (501) staff       (20)     2604 2024-04-09 15:39:40.000000 pymodbus-3.6.8/AUTHORS.rst
--rw-r--r--   0 jan        (501) staff       (20)    35759 2024-04-14 08:22:03.000000 pymodbus-3.6.8/CHANGELOG.rst
--rw-r--r--   0 jan        (501) staff       (20)     1367 2024-04-07 15:47:51.000000 pymodbus-3.6.8/LICENSE
--rw-r--r--   0 jan        (501) staff       (20)       80 2024-02-04 13:28:30.000000 pymodbus-3.6.8/MANIFEST.in
--rw-r--r--   0 jan        (501) staff       (20)    14494 2024-04-14 08:22:36.682787 pymodbus-3.6.8/PKG-INFO
--rw-r--r--   0 jan        (501) staff       (20)    11446 2024-04-14 08:22:03.000000 pymodbus-3.6.8/README.rst
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2024-04-14 08:22:36.669888 pymodbus-3.6.8/pymodbus/
--rw-r--r--   0 jan        (501) staff       (20)      504 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     9422 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/bit_read_message.py
--rw-r--r--   0 jan        (501) staff       (20)     9536 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/bit_write_message.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2024-04-14 08:22:36.671708 pymodbus-3.6.8/pymodbus/client/
--rw-r--r--   0 jan        (501) staff       (20)      603 2024-04-07 15:47:51.000000 pymodbus-3.6.8/pymodbus/client/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)    17220 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/client/base.py
--rw-r--r--   0 jan        (501) staff       (20)    20443 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/client/mixin.py
--rw-r--r--   0 jan        (501) staff       (20)     9775 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/client/serial.py
--rw-r--r--   0 jan        (501) staff       (20)     9855 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/client/tcp.py
--rw-r--r--   0 jan        (501) staff       (20)     6621 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/client/tls.py
--rw-r--r--   0 jan        (501) staff       (20)     6517 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/client/udp.py
--rw-r--r--   0 jan        (501) staff       (20)     3499 2024-04-07 15:47:51.000000 pymodbus-3.6.8/pymodbus/constants.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2024-04-14 08:22:36.672432 pymodbus-3.6.8/pymodbus/datastore/
--rw-r--r--   0 jan        (501) staff       (20)      491 2023-12-08 17:46:25.000000 pymodbus-3.6.8/pymodbus/datastore/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     7098 2023-12-08 17:46:25.000000 pymodbus-3.6.8/pymodbus/datastore/context.py
--rw-r--r--   0 jan        (501) staff       (20)     4435 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/datastore/remote.py
--rw-r--r--   0 jan        (501) staff       (20)    30640 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/datastore/simulator.py
--rw-r--r--   0 jan        (501) staff       (20)    11159 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/datastore/store.py
--rw-r--r--   0 jan        (501) staff       (20)    22601 2024-04-07 15:47:51.000000 pymodbus-3.6.8/pymodbus/device.py
--rw-r--r--   0 jan        (501) staff       (20)    30484 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/diag_message.py
--rw-r--r--   0 jan        (501) staff       (20)     6482 2024-02-04 13:28:30.000000 pymodbus-3.6.8/pymodbus/events.py
--rw-r--r--   0 jan        (501) staff       (20)     3189 2024-02-04 13:28:30.000000 pymodbus-3.6.8/pymodbus/exceptions.py
--rw-r--r--   0 jan        (501) staff       (20)    12276 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/factory.py
--rw-r--r--   0 jan        (501) staff       (20)    14762 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/file_message.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2024-04-14 08:22:36.673371 pymodbus-3.6.8/pymodbus/framer/
--rw-r--r--   0 jan        (501) staff       (20)      953 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/framer/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     3838 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/framer/ascii_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     4674 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/framer/base.py
--rw-r--r--   0 jan        (501) staff       (20)     4893 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/framer/binary_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     9715 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/framer/rtu_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     5066 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/framer/socket_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     2955 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/framer/tls_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     3926 2024-02-04 13:28:30.000000 pymodbus-3.6.8/pymodbus/logging.py
--rw-r--r--   0 jan        (501) staff       (20)     7816 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/mei_message.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2024-04-14 08:22:36.674278 pymodbus-3.6.8/pymodbus/message/
--rw-r--r--   0 jan        (501) staff       (20)      122 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/message/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     2793 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/message/ascii.py
--rw-r--r--   0 jan        (501) staff       (20)     1305 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/message/base.py
--rw-r--r--   0 jan        (501) staff       (20)     3884 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/message/message.py
--rw-r--r--   0 jan        (501) staff       (20)     1081 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/message/raw.py
--rw-r--r--   0 jan        (501) staff       (20)     3627 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/message/rtu.py
--rw-r--r--   0 jan        (501) staff       (20)     1499 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/message/socket.py
--rw-r--r--   0 jan        (501) staff       (20)      658 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/message/tls.py
--rw-r--r--   0 jan        (501) staff       (20)    15363 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/other_message.py
--rw-r--r--   0 jan        (501) staff       (20)    15678 2024-04-07 15:47:51.000000 pymodbus-3.6.8/pymodbus/payload.py
--rw-r--r--   0 jan        (501) staff       (20)     7748 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/pdu.py
--rw-r--r--   0 jan        (501) staff       (20)        0 2023-12-08 17:46:25.000000 pymodbus-3.6.8/pymodbus/py.typed
--rw-r--r--   0 jan        (501) staff       (20)    14208 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/register_read_message.py
--rw-r--r--   0 jan        (501) staff       (20)    12510 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/register_write_message.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2024-04-14 08:22:36.674514 pymodbus-3.6.8/pymodbus/server/
--rw-r--r--   0 jan        (501) staff       (20)      996 2023-12-08 17:46:25.000000 pymodbus-3.6.8/pymodbus/server/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)    26198 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/server/async_io.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2024-04-14 08:22:36.675247 pymodbus-3.6.8/pymodbus/server/simulator/
--rw-r--r--   0 jan        (501) staff       (20)       18 2023-12-08 17:46:25.000000 pymodbus-3.6.8/pymodbus/server/simulator/__init__.py
--rwxr-xr-x   0 jan        (501) staff       (20)      187 2024-02-04 13:28:30.000000 pymodbus-3.6.8/pymodbus/server/simulator/custom_actions.py
--rw-r--r--   0 jan        (501) staff       (20)    25934 2024-04-07 15:47:51.000000 pymodbus-3.6.8/pymodbus/server/simulator/http_server.py
--rwxr-xr-x   0 jan        (501) staff       (20)     4200 2024-02-04 13:28:30.000000 pymodbus-3.6.8/pymodbus/server/simulator/main.py
--rw-r--r--   0 jan        (501) staff       (20)     7619 2023-12-08 17:46:25.000000 pymodbus-3.6.8/pymodbus/server/simulator/setup.json
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2024-04-14 08:22:36.677705 pymodbus-3.6.8/pymodbus/server/simulator/web/
--rw-r--r--   0 jan        (501) staff       (20)    11369 2023-12-08 17:46:25.000000 pymodbus-3.6.8/pymodbus/server/simulator/web/apple120.png
--rw-r--r--   0 jan        (501) staff       (20)    15391 2023-12-08 17:46:25.000000 pymodbus-3.6.8/pymodbus/server/simulator/web/apple152.png
--rw-r--r--   0 jan        (501) staff       (20)     4817 2023-12-08 17:46:25.000000 pymodbus-3.6.8/pymodbus/server/simulator/web/apple60.png
--rw-r--r--   0 jan        (501) staff       (20)     6344 2023-12-08 17:46:25.000000 pymodbus-3.6.8/pymodbus/server/simulator/web/apple76.png
--rw-r--r--   0 jan        (501) staff       (20)    12014 2023-12-08 17:46:25.000000 pymodbus-3.6.8/pymodbus/server/simulator/web/favicon.ico
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2024-04-14 08:22:36.678714 pymodbus-3.6.8/pymodbus/server/simulator/web/generator/
--rw-r--r--   0 jan        (501) staff       (20)     4314 2023-12-08 17:46:25.000000 pymodbus-3.6.8/pymodbus/server/simulator/web/generator/calls
--rw-r--r--   0 jan        (501) staff       (20)     1132 2023-12-08 17:46:25.000000 pymodbus-3.6.8/pymodbus/server/simulator/web/generator/log
--rw-r--r--   0 jan        (501) staff       (20)     5850 2023-12-08 17:46:25.000000 pymodbus-3.6.8/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png
--rw-r--r--   0 jan        (501) staff       (20)     2710 2023-12-08 17:46:25.000000 pymodbus-3.6.8/pymodbus/server/simulator/web/generator/registers
--rw-r--r--   0 jan        (501) staff       (20)      893 2023-12-08 17:46:25.000000 pymodbus-3.6.8/pymodbus/server/simulator/web/generator/server
--rw-r--r--   0 jan        (501) staff       (20)     1944 2023-12-08 17:46:25.000000 pymodbus-3.6.8/pymodbus/server/simulator/web/index.html
--rw-r--r--   0 jan        (501) staff       (20)      919 2023-12-08 17:46:25.000000 pymodbus-3.6.8/pymodbus/server/simulator/web/pymodbus.css
--rw-r--r--   0 jan        (501) staff       (20)      710 2023-12-08 17:46:25.000000 pymodbus-3.6.8/pymodbus/server/simulator/web/welcome.html
--rw-r--r--   0 jan        (501) staff       (20)    20947 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/transaction.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2024-04-14 08:22:36.679158 pymodbus-3.6.8/pymodbus/transport/
--rw-r--r--   0 jan        (501) staff       (20)      225 2024-04-07 15:47:51.000000 pymodbus-3.6.8/pymodbus/transport/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     5581 2024-04-07 15:47:51.000000 pymodbus-3.6.8/pymodbus/transport/serialtransport.py
--rw-r--r--   0 jan        (501) staff       (20)    22919 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pymodbus/transport/transport.py
--rw-r--r--   0 jan        (501) staff       (20)     5495 2024-04-07 15:47:51.000000 pymodbus-3.6.8/pymodbus/utilities.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2024-04-14 08:22:36.681309 pymodbus-3.6.8/pymodbus.egg-info/
--rw-r--r--   0 jan        (501) staff       (20)    14494 2024-04-14 08:22:36.000000 pymodbus-3.6.8/pymodbus.egg-info/PKG-INFO
--rw-r--r--   0 jan        (501) staff       (20)     2767 2024-04-14 08:22:36.000000 pymodbus-3.6.8/pymodbus.egg-info/SOURCES.txt
--rw-r--r--   0 jan        (501) staff       (20)        1 2024-04-14 08:22:36.000000 pymodbus-3.6.8/pymodbus.egg-info/dependency_links.txt
--rw-r--r--   0 jan        (501) staff       (20)       75 2024-04-14 08:22:36.000000 pymodbus-3.6.8/pymodbus.egg-info/entry_points.txt
--rw-r--r--   0 jan        (501) staff       (20)      582 2024-04-14 08:22:36.000000 pymodbus-3.6.8/pymodbus.egg-info/requires.txt
--rw-r--r--   0 jan        (501) staff       (20)        9 2024-04-14 08:22:36.000000 pymodbus-3.6.8/pymodbus.egg-info/top_level.txt
--rw-r--r--   0 jan        (501) staff       (20)        1 2022-11-08 12:27:57.000000 pymodbus-3.6.8/pymodbus.egg-info/zip-safe
--rw-r--r--   0 jan        (501) staff       (20)     7541 2024-04-14 08:22:03.000000 pymodbus-3.6.8/pyproject.toml
--rw-r--r--   0 jan        (501) staff       (20)       38 2024-04-14 08:22:36.683069 pymodbus-3.6.8/setup.cfg
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2024-04-14 08:22:36.681107 pymodbus-3.6.8/test/
--rw-r--r--   0 jan        (501) staff       (20)    13220 2024-02-04 13:28:30.000000 pymodbus-3.6.8/test/test_device.py
--rw-r--r--   0 jan        (501) staff       (20)     2359 2023-12-08 17:46:25.000000 pymodbus-3.6.8/test/test_events.py
--rw-r--r--   0 jan        (501) staff       (20)      772 2024-02-04 13:28:30.000000 pymodbus-3.6.8/test/test_exceptions.py
--rw-r--r--   0 jan        (501) staff       (20)     8508 2024-02-04 13:28:30.000000 pymodbus-3.6.8/test/test_factory.py
--rw-r--r--   0 jan        (501) staff       (20)    10219 2024-04-14 08:22:03.000000 pymodbus-3.6.8/test/test_file_message.py
--rw-r--r--   0 jan        (501) staff       (20)    18220 2024-04-14 08:22:03.000000 pymodbus-3.6.8/test/test_framers.py
--rw-r--r--   0 jan        (501) staff       (20)     1241 2024-02-04 13:28:30.000000 pymodbus-3.6.8/test/test_logging.py
--rw-r--r--   0 jan        (501) staff       (20)     4640 2024-04-14 08:22:03.000000 pymodbus-3.6.8/test/test_network.py
--rw-r--r--   0 jan        (501) staff       (20)     8780 2024-02-04 13:28:30.000000 pymodbus-3.6.8/test/test_payload.py
--rw-r--r--   0 jan        (501) staff       (20)     2818 2024-02-04 13:28:30.000000 pymodbus-3.6.8/test/test_pdu.py
--rw-r--r--   0 jan        (501) staff       (20)     2665 2024-04-14 08:22:03.000000 pymodbus-3.6.8/test/test_remote_datastore.py
--rw-r--r--   0 jan        (501) staff       (20)      649 2023-12-08 17:46:25.000000 pymodbus-3.6.8/test/test_sparse_datastore.py
--rwxr-xr-x   0 jan        (501) staff       (20)    28722 2024-04-14 08:22:03.000000 pymodbus-3.6.8/test/test_transaction.py
--rw-r--r--   0 jan        (501) staff       (20)     2703 2024-04-07 15:47:51.000000 pymodbus-3.6.8/test/test_utilities.py
+drwxr-xr-x   0 sanjay     (501) staff       (20)        0 2024-03-05 06:19:53.626595 pymodbus-3.7.0.dev0/
+-rw-r--r--   0 sanjay     (501) staff       (20)     2521 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/AUTHORS.rst
+-rw-r--r--   0 sanjay     (501) staff       (20)    34065 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/CHANGELOG.rst
+-rw-r--r--   0 sanjay     (501) staff       (20)     1367 2024-02-13 10:20:22.000000 pymodbus-3.7.0.dev0/LICENSE
+-rw-r--r--   0 sanjay     (501) staff       (20)       80 2023-11-03 07:44:37.000000 pymodbus-3.7.0.dev0/MANIFEST.in
+-rw-r--r--   0 sanjay     (501) staff       (20)    14519 2024-03-05 06:19:53.625734 pymodbus-3.7.0.dev0/PKG-INFO
+-rw-r--r--   0 sanjay     (501) staff       (20)    11467 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/README.rst
+drwxr-xr-x   0 sanjay     (501) staff       (20)        0 2024-03-05 06:19:53.586198 pymodbus-3.7.0.dev0/pymodbus/
+-rw-r--r--   0 sanjay     (501) staff       (20)      507 2024-02-13 10:20:23.000000 pymodbus-3.7.0.dev0/pymodbus/__init__.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     9422 2023-08-26 16:29:51.000000 pymodbus-3.7.0.dev0/pymodbus/bit_read_message.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     9536 2023-11-03 07:44:37.000000 pymodbus-3.7.0.dev0/pymodbus/bit_write_message.py
+drwxr-xr-x   0 sanjay     (501) staff       (20)        0 2024-03-05 06:19:53.591797 pymodbus-3.7.0.dev0/pymodbus/client/
+-rw-r--r--   0 sanjay     (501) staff       (20)      603 2024-02-13 10:20:23.000000 pymodbus-3.7.0.dev0/pymodbus/client/__init__.py
+-rw-r--r--   0 sanjay     (501) staff       (20)    17122 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/client/base.py
+-rw-r--r--   0 sanjay     (501) staff       (20)    20443 2024-02-13 10:20:23.000000 pymodbus-3.7.0.dev0/pymodbus/client/mixin.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     9661 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/client/serial.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     9881 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/client/tcp.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     6621 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/client/tls.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     6517 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/client/udp.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     3499 2024-02-13 10:20:23.000000 pymodbus-3.7.0.dev0/pymodbus/constants.py
+drwxr-xr-x   0 sanjay     (501) staff       (20)        0 2024-03-05 06:19:53.594970 pymodbus-3.7.0.dev0/pymodbus/datastore/
+-rw-r--r--   0 sanjay     (501) staff       (20)      491 2023-03-29 05:39:40.000000 pymodbus-3.7.0.dev0/pymodbus/datastore/__init__.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     7098 2023-11-03 07:44:37.000000 pymodbus-3.7.0.dev0/pymodbus/datastore/context.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     4305 2024-02-14 14:12:15.000000 pymodbus-3.7.0.dev0/pymodbus/datastore/remote.py
+-rw-r--r--   0 sanjay     (501) staff       (20)    30584 2024-02-14 14:12:15.000000 pymodbus-3.7.0.dev0/pymodbus/datastore/simulator.py
+-rw-r--r--   0 sanjay     (501) staff       (20)    11159 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/datastore/store.py
+-rw-r--r--   0 sanjay     (501) staff       (20)    22601 2024-02-13 10:20:23.000000 pymodbus-3.7.0.dev0/pymodbus/device.py
+-rw-r--r--   0 sanjay     (501) staff       (20)    30458 2023-11-03 07:44:37.000000 pymodbus-3.7.0.dev0/pymodbus/diag_message.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     6482 2023-11-03 07:44:37.000000 pymodbus-3.7.0.dev0/pymodbus/events.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     3189 2023-11-03 07:44:37.000000 pymodbus-3.7.0.dev0/pymodbus/exceptions.py
+-rw-r--r--   0 sanjay     (501) staff       (20)    14052 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/factory.py
+-rw-r--r--   0 sanjay     (501) staff       (20)    14762 2024-03-05 06:16:26.000000 pymodbus-3.7.0.dev0/pymodbus/file_message.py
+drwxr-xr-x   0 sanjay     (501) staff       (20)        0 2024-03-05 06:19:53.597689 pymodbus-3.7.0.dev0/pymodbus/framer/
+-rw-r--r--   0 sanjay     (501) staff       (20)      953 2023-11-03 07:44:37.000000 pymodbus-3.7.0.dev0/pymodbus/framer/__init__.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     4197 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/framer/ascii_framer.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     4666 2024-02-13 10:20:23.000000 pymodbus-3.7.0.dev0/pymodbus/framer/base.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     4889 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/framer/binary_framer.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     9678 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/framer/rtu_framer.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     4655 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/framer/socket_framer.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     2828 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/framer/tls_framer.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     3926 2023-11-03 07:44:37.000000 pymodbus-3.7.0.dev0/pymodbus/logging.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     7816 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/mei_message.py
+drwxr-xr-x   0 sanjay     (501) staff       (20)        0 2024-03-05 06:19:53.600139 pymodbus-3.7.0.dev0/pymodbus/message/
+-rw-r--r--   0 sanjay     (501) staff       (20)      122 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/message/__init__.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     2793 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/message/ascii.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     1305 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/message/base.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     3884 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/message/message.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     1081 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/message/raw.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     1909 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/message/rtu.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     1499 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/message/socket.py
+-rw-r--r--   0 sanjay     (501) staff       (20)      658 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/message/tls.py
+-rw-r--r--   0 sanjay     (501) staff       (20)    15363 2023-11-03 07:44:37.000000 pymodbus-3.7.0.dev0/pymodbus/other_message.py
+-rw-r--r--   0 sanjay     (501) staff       (20)    15678 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/payload.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     7748 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/pdu.py
+-rw-r--r--   0 sanjay     (501) staff       (20)        0 2023-03-29 05:39:40.000000 pymodbus-3.7.0.dev0/pymodbus/py.typed
+-rw-r--r--   0 sanjay     (501) staff       (20)    14208 2023-08-26 16:29:51.000000 pymodbus-3.7.0.dev0/pymodbus/register_read_message.py
+-rw-r--r--   0 sanjay     (501) staff       (20)    12510 2023-08-26 16:29:51.000000 pymodbus-3.7.0.dev0/pymodbus/register_write_message.py
+drwxr-xr-x   0 sanjay     (501) staff       (20)        0 2024-03-05 06:19:53.601146 pymodbus-3.7.0.dev0/pymodbus/server/
+-rw-r--r--   0 sanjay     (501) staff       (20)      996 2023-08-26 16:29:51.000000 pymodbus-3.7.0.dev0/pymodbus/server/__init__.py
+-rw-r--r--   0 sanjay     (501) staff       (20)    26507 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/server/async_io.py
+drwxr-xr-x   0 sanjay     (501) staff       (20)        0 2024-03-05 06:19:53.603930 pymodbus-3.7.0.dev0/pymodbus/server/simulator/
+-rw-r--r--   0 sanjay     (501) staff       (20)       18 2023-03-29 05:39:40.000000 pymodbus-3.7.0.dev0/pymodbus/server/simulator/__init__.py
+-rwxr-xr-x   0 sanjay     (501) staff       (20)      187 2023-11-03 07:44:37.000000 pymodbus-3.7.0.dev0/pymodbus/server/simulator/custom_actions.py
+-rw-r--r--   0 sanjay     (501) staff       (20)    25815 2024-03-05 06:16:26.000000 pymodbus-3.7.0.dev0/pymodbus/server/simulator/http_server.py
+-rwxr-xr-x   0 sanjay     (501) staff       (20)     4200 2023-11-03 07:44:37.000000 pymodbus-3.7.0.dev0/pymodbus/server/simulator/main.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     7619 2023-08-26 16:29:51.000000 pymodbus-3.7.0.dev0/pymodbus/server/simulator/setup.json
+drwxr-xr-x   0 sanjay     (501) staff       (20)        0 2024-03-05 06:19:53.608662 pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/
+-rw-r--r--   0 sanjay     (501) staff       (20)    11369 2023-03-29 05:39:40.000000 pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/apple120.png
+-rw-r--r--   0 sanjay     (501) staff       (20)    15391 2023-03-29 05:39:40.000000 pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/apple152.png
+-rw-r--r--   0 sanjay     (501) staff       (20)     4817 2023-03-29 05:39:40.000000 pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/apple60.png
+-rw-r--r--   0 sanjay     (501) staff       (20)     6344 2023-03-29 05:39:40.000000 pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/apple76.png
+-rw-r--r--   0 sanjay     (501) staff       (20)    12014 2023-03-29 05:39:40.000000 pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/favicon.ico
+drwxr-xr-x   0 sanjay     (501) staff       (20)        0 2024-03-05 06:19:53.610882 pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/generator/
+-rw-r--r--   0 sanjay     (501) staff       (20)     4314 2023-03-29 05:39:40.000000 pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/generator/calls
+-rw-r--r--   0 sanjay     (501) staff       (20)     1132 2023-03-29 05:39:40.000000 pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/generator/log
+-rw-r--r--   0 sanjay     (501) staff       (20)     5850 2023-03-29 05:39:40.000000 pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png
+-rw-r--r--   0 sanjay     (501) staff       (20)     2710 2023-03-29 05:39:40.000000 pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/generator/registers
+-rw-r--r--   0 sanjay     (501) staff       (20)      893 2023-03-29 05:39:40.000000 pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/generator/server
+-rw-r--r--   0 sanjay     (501) staff       (20)     1944 2023-03-29 05:39:40.000000 pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/index.html
+-rw-r--r--   0 sanjay     (501) staff       (20)      919 2023-03-29 05:39:40.000000 pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/pymodbus.css
+-rw-r--r--   0 sanjay     (501) staff       (20)      710 2023-03-29 05:39:40.000000 pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/welcome.html
+-rw-r--r--   0 sanjay     (501) staff       (20)    20471 2024-02-23 05:11:07.000000 pymodbus-3.7.0.dev0/pymodbus/transaction.py
+drwxr-xr-x   0 sanjay     (501) staff       (20)        0 2024-03-05 06:19:53.612595 pymodbus-3.7.0.dev0/pymodbus/transport/
+-rw-r--r--   0 sanjay     (501) staff       (20)      225 2024-02-13 10:20:23.000000 pymodbus-3.7.0.dev0/pymodbus/transport/__init__.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     5742 2024-02-13 10:20:23.000000 pymodbus-3.7.0.dev0/pymodbus/transport/serialtransport.py
+-rw-r--r--   0 sanjay     (501) staff       (20)    22918 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/transport/transport.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     6895 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/pymodbus/utilities.py
+drwxr-xr-x   0 sanjay     (501) staff       (20)        0 2024-03-05 06:19:53.620462 pymodbus-3.7.0.dev0/pymodbus.egg-info/
+-rw-r--r--   0 sanjay     (501) staff       (20)    14519 2024-03-05 06:19:53.000000 pymodbus-3.7.0.dev0/pymodbus.egg-info/PKG-INFO
+-rw-r--r--   0 sanjay     (501) staff       (20)     2767 2024-03-05 06:19:53.000000 pymodbus-3.7.0.dev0/pymodbus.egg-info/SOURCES.txt
+-rw-r--r--   0 sanjay     (501) staff       (20)        1 2024-03-05 06:19:53.000000 pymodbus-3.7.0.dev0/pymodbus.egg-info/dependency_links.txt
+-rw-r--r--   0 sanjay     (501) staff       (20)       75 2024-03-05 06:19:53.000000 pymodbus-3.7.0.dev0/pymodbus.egg-info/entry_points.txt
+-rw-r--r--   0 sanjay     (501) staff       (20)      581 2024-03-05 06:19:53.000000 pymodbus-3.7.0.dev0/pymodbus.egg-info/requires.txt
+-rw-r--r--   0 sanjay     (501) staff       (20)        9 2024-03-05 06:19:53.000000 pymodbus-3.7.0.dev0/pymodbus.egg-info/top_level.txt
+-rw-r--r--   0 sanjay     (501) staff       (20)        1 2022-05-22 09:43:08.000000 pymodbus-3.7.0.dev0/pymodbus.egg-info/zip-safe
+-rw-r--r--   0 sanjay     (501) staff       (20)     7443 2024-03-05 06:18:42.000000 pymodbus-3.7.0.dev0/pyproject.toml
+-rw-r--r--   0 sanjay     (501) staff       (20)       38 2024-03-05 06:19:53.626749 pymodbus-3.7.0.dev0/setup.cfg
+drwxr-xr-x   0 sanjay     (501) staff       (20)        0 2024-03-05 06:19:53.620099 pymodbus-3.7.0.dev0/test/
+-rw-r--r--   0 sanjay     (501) staff       (20)    13220 2023-11-03 07:44:37.000000 pymodbus-3.7.0.dev0/test/test_device.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     2359 2023-03-29 05:39:40.000000 pymodbus-3.7.0.dev0/test/test_events.py
+-rw-r--r--   0 sanjay     (501) staff       (20)      772 2023-11-03 07:44:37.000000 pymodbus-3.7.0.dev0/test/test_exceptions.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     8508 2023-11-03 07:44:37.000000 pymodbus-3.7.0.dev0/test/test_factory.py
+-rw-r--r--   0 sanjay     (501) staff       (20)    10203 2024-03-05 06:16:26.000000 pymodbus-3.7.0.dev0/test/test_file_message.py
+-rw-r--r--   0 sanjay     (501) staff       (20)    17679 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/test/test_framers.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     1241 2023-11-03 07:44:37.000000 pymodbus-3.7.0.dev0/test/test_logging.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     4503 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/test/test_network.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     8780 2023-11-03 07:44:37.000000 pymodbus-3.7.0.dev0/test/test_payload.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     2818 2023-11-03 07:44:37.000000 pymodbus-3.7.0.dev0/test/test_pdu.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     2665 2023-11-03 07:44:37.000000 pymodbus-3.7.0.dev0/test/test_remote_datastore.py
+-rw-r--r--   0 sanjay     (501) staff       (20)      649 2023-08-26 16:29:51.000000 pymodbus-3.7.0.dev0/test/test_sparse_datastore.py
+-rwxr-xr-x   0 sanjay     (501) staff       (20)    28722 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/test/test_transaction.py
+-rw-r--r--   0 sanjay     (501) staff       (20)     2903 2024-03-05 06:16:12.000000 pymodbus-3.7.0.dev0/test/test_utilities.py
```

### Comparing `pymodbus-3.6.8/AUTHORS.rst` & `pymodbus-3.7.0.dev0/AUTHORS.rst`

 * *Files 3% similar despite different names*

```diff
@@ -16,45 +16,40 @@
 - Alexander Lanin
 - Alexandre CUER
 - Alois Hockenschlohe
 - Arjan
 - André Srinivasan
 - banana-sun
 - Blaise Thompson
-- CapraTheBest
 - cgernert
 - corollaries
 - Chandler Riehm
 - Chris Hung
 - Christian Krause
 - dhoomakethu
 - doelki
 - DominicDataP
-- Dominique Martinet
 - Dries
 - duc996
 - Farzad Panahi
 - Fredo70
 - Gao Fang
 - Ghostkeeper
 - Hangyu Fan
 - Hayden Roche
 - Iktek
-- Ilkka Ollakka
 - Jakob Ruhe
 - Jakob Schlyter
 - James Braza
 - James Hilliard
 - jan iversen
 - Jerome Velociter
 - Joe Burmeister
-- John Miko
 - Jonathan Reichelt Gjertsen
 - julian
-- Justin Standring
 - Kenny Johansson
 - Matthias Straka
 - laund
 - Logan Gunthorpe
 - Marko Luther
 - Logan Gunthorpe
 - Marko Luther
```

### Comparing `pymodbus-3.6.8/CHANGELOG.rst` & `pymodbus-3.7.0.dev0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,59 +3,14 @@
 All these version would not be possible without a lot of work from volunteers!
 
 We, the maintainers, are greatful for each pull requests small or big, that
 helps make pymodbus a better product.
 
 :ref:`Authors`: contains a complete list of volunteers have contributed to each major version.
 
-Version 3.6.8
--------------
-* Allow socket exception response with wrong length
-
-
-Version 3.6.7
--------------
-* Add lock to async requests, correct logging and length calc. (FIX, not on dev)
-* test_simulator: use unused_tcp_port fixture (#2141)
-* streamline imports in Factory.py (#2140)
-* Secure testing is done with pymodbus in PR. (#2136)
-* Fix link to github in README (#2134)
-* Wildcard exception catch from pyserial. (#2125)
-* Problem with stale CI. (#2117)
-* Add connection exception to list of exceptions catpured in retries (#2113)
-* Move on_reconnect to client level (#2111)
-* Bump github stale. (#2110)
-* update package_test_tool (add 4 test scenarios) (#2107)
-* Bump dependencies. (#2108)
-* Cancel send if no connection. (#2103)
-
-
-Version 3.6.6
--------------
-* Solve transport close() as not inherited method. (#2098)
-* enable `mypy --check-untyped-defs` (#2096)
-* Add get_expected_response_length to transaction.
-* Remove control encode in framersRemove control encode in framers. (#2095)
-* Bump codeql in CI to v3. (#2093)
-* Improve server types (#2092)
-* Remove pointless try/except (#2091)
-* Improve transport types (#2090)
-* Use explicit ValueError when called with incorrect function code (#2089)
-* update message tests (incorporate all old tests). (#2088)
-* Improve simulator type hints (#2084)
-* Cleanup dead resetFrame code (#2082)
-* integrate message.encode() into framer.buildPacket. (#2062)
-* Repair client close() (intern= is needed for ModbusProtocol). (#2080)
-* Updated Message_Parser example (#2079)
-* Fix #2069 use released repl from pypi (#2077)
-* Fix field encoding of Read File Record Response (#2075)
-* Improve simulator types (#2076)
-* Bump actions. (#2071)
-
-
 Version 3.6.5
 -------------
 * Update framers to ease message integration (only decode/encode) (#2064)
 * Add negtive acknowledge to modbus exceptions (#2065)
 * add Message Socket/TLS and amend tests. (#2061)
 * Improve factory types (#2060)
 * ASCII. (#2054)
```

### Comparing `pymodbus-3.6.8/LICENSE` & `pymodbus-3.7.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/PKG-INFO` & `pymodbus-3.7.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodbus
-Version: 3.6.8
+Version: 3.7.0.dev0
 Summary: A fully featured modbus protocol stack in python
 Author: Galen Collins, Jan Iversen
 Maintainer: dhoomakethu, janiversen
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/pymodbus-dev/pymodbus/
 Project-URL: Source Code, https://github.com/pymodbus-dev/pymodbus
 Project-URL: Bug Reports, https://github.com/pymodbus-dev/pymodbus/issues
@@ -34,36 +34,36 @@
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 Provides-Extra: serial
 Requires-Dist: pyserial>=3.5; extra == "serial"
 Provides-Extra: repl
-Requires-Dist: pymodbus-repl>=2.0.3; extra == "repl"
+Requires-Dist: pymodbus-repl==2.0.3.dev0; extra == "repl"
 Provides-Extra: simulator
 Requires-Dist: aiohttp>=3.8.6; python_version < "3.12" and extra == "simulator"
 Requires-Dist: aiohttp>=3.9.0b0; python_version == "3.12" and extra == "simulator"
 Provides-Extra: documentation
 Requires-Dist: recommonmark>=0.7.1; extra == "documentation"
 Requires-Dist: Sphinx>=5.3.0; extra == "documentation"
 Requires-Dist: sphinx-rtd-theme>=1.1.1; extra == "documentation"
 Provides-Extra: development
-Requires-Dist: build>=1.1.1; extra == "development"
-Requires-Dist: codespell>=2.2.6; extra == "development"
-Requires-Dist: coverage>=7.4.3; extra == "development"
-Requires-Dist: mypy>=1.9.0; extra == "development"
-Requires-Dist: pylint>=3.1.0; extra == "development"
-Requires-Dist: pytest>=8.1.0; extra == "development"
-Requires-Dist: pytest-asyncio>=0.23.5.post1; extra == "development"
+Requires-Dist: build>=1.0.3; extra == "development"
+Requires-Dist: codespell>=2.2.2; extra == "development"
+Requires-Dist: coverage>=7.4.0; extra == "development"
+Requires-Dist: mypy>=1.6.0; extra == "development"
+Requires-Dist: pylint>=3.0.0; extra == "development"
+Requires-Dist: pytest>=7.3.1; extra == "development"
+Requires-Dist: pytest-asyncio>=0.20.3; extra == "development"
 Requires-Dist: pytest-cov>=4.1.0; extra == "development"
 Requires-Dist: pytest-profiling>=1.7.0; extra == "development"
-Requires-Dist: pytest-timeout>=2.3.1; extra == "development"
-Requires-Dist: pytest-xdist>=3.5.0; extra == "development"
-Requires-Dist: ruff>=0.3.3; extra == "development"
-Requires-Dist: twine>=5.0.0; extra == "development"
+Requires-Dist: pytest-timeout>=2.2.0; extra == "development"
+Requires-Dist: pytest-xdist>=3.3.1; extra == "development"
+Requires-Dist: ruff>=0.2.0; extra == "development"
+Requires-Dist: twine>=4.0.2; extra == "development"
 Requires-Dist: types-Pygments; extra == "development"
 Requires-Dist: types-pyserial; extra == "development"
 Provides-Extra: all
 Requires-Dist: pymodbus[development,documentation,repl,serial,simulator]; extra == "all"
 
 PyModbus - A Python Modbus Stack
 ================================
@@ -74,24 +74,24 @@
    :alt: Documentation Status
 .. image:: https://pepy.tech/badge/pymodbus
    :target: https://pepy.tech/project/pymodbus
    :alt: Downloads
 
 Pymodbus is a full Modbus protocol implementation offering client/server with synchronous/asynchronous API a well as simulators.
 
-Current release is `3.6.8 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.6.8>`_.
+Current release is `3.6.5 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.6.5>`_.
 
 Bleeding edge (not released) is `dev <https://github.com/pymodbus-dev/pymodbus/tree/dev>`_.
 
 All changes are described in `release notes <https://pymodbus.readthedocs.io/en/latest/source/changelog.html>`_
 and all API changes are `documented <https://pymodbus.readthedocs.io/en/latest/source/api_changes.html>`_
 
 A big thanks to all the `volunteers <https://pymodbus.readthedocs.io/en/latest/source/authors.html>`_ that helps make pymodbus a great project.
 
-Source code on `github <https://github.com/pymodbus-dev/pymodbus>`_
+Source code on `github <https://pymodbus.readthedocs.io/en/latest/source/authors.html>`_
 
 Pymodbus in a nutshell
 ----------------------
 Pymodbus consist of 5 parts:
 
 - **client**, connect to your favorite device(s)
 - **server**, simulate your favorite device(s)
```

### Comparing `pymodbus-3.6.8/README.rst` & `pymodbus-3.7.0.dev0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,24 @@
    :alt: Documentation Status
 .. image:: https://pepy.tech/badge/pymodbus
    :target: https://pepy.tech/project/pymodbus
    :alt: Downloads
 
 Pymodbus is a full Modbus protocol implementation offering client/server with synchronous/asynchronous API a well as simulators.
 
-Current release is `3.6.8 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.6.8>`_.
+Current release is `3.6.5 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.6.5>`_.
 
 Bleeding edge (not released) is `dev <https://github.com/pymodbus-dev/pymodbus/tree/dev>`_.
 
 All changes are described in `release notes <https://pymodbus.readthedocs.io/en/latest/source/changelog.html>`_
 and all API changes are `documented <https://pymodbus.readthedocs.io/en/latest/source/api_changes.html>`_
 
 A big thanks to all the `volunteers <https://pymodbus.readthedocs.io/en/latest/source/authors.html>`_ that helps make pymodbus a great project.
 
-Source code on `github <https://github.com/pymodbus-dev/pymodbus>`_
+Source code on `github <https://pymodbus.readthedocs.io/en/latest/source/authors.html>`_
 
 Pymodbus in a nutshell
 ----------------------
 Pymodbus consist of 5 parts:
 
 - **client**, connect to your favorite device(s)
 - **server**, simulate your favorite device(s)
```

### Comparing `pymodbus-3.6.8/pymodbus/bit_read_message.py` & `pymodbus-3.7.0.dev0/pymodbus/bit_read_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/bit_write_message.py` & `pymodbus-3.7.0.dev0/pymodbus/bit_write_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/client/__init__.py` & `pymodbus-3.7.0.dev0/pymodbus/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/client/base.py` & `pymodbus-3.7.0.dev0/pymodbus/client/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,14 @@
         self.transaction = ModbusTransactionManager(
             self, retries=retries, retry_on_empty=retry_on_empty, **kwargs
         )
         self.use_udp = False
         self.state = ModbusTransactionState.IDLE
         self.last_frame_end: float | None = 0
         self.silent_interval: float = 0
-        self._lock = asyncio.Lock()
 
     # ----------------------------------------------------------------------- #
     # Client external interface
     # ----------------------------------------------------------------------- #
     @property
     def connected(self) -> bool:
         """Return state of connection."""
@@ -121,15 +120,15 @@
         :raises MessageRegisterException: Check exception text.
 
         Use register() to add non-standard responses (like e.g. a login prompt) and
         have them interpreted automatically.
         """
         self.framer.decoder.register(custom_response_class)
 
-    def close(self, reconnect: bool = False) -> None:
+    def close(self, reconnect: bool = False) -> None:  # type: ignore[override] # pylint: disable=arguments-differ
         """Close connection."""
         if reconnect:
             self.connection_lost(asyncio.TimeoutError("Server not responding"))
         else:
             super().close()
 
     def idle_time(self) -> float:
@@ -159,45 +158,40 @@
     async def async_execute(self, request) -> ModbusResponse:
         """Execute requests asynchronously."""
         request.transaction_id = self.transaction.getNextTID()
         packet = self.framer.buildPacket(request)
 
         count = 0
         while count <= self.retries:
-            async with self._lock:
-                req = self.build_response(request.transaction_id)
-                if not count or not self.no_resend_on_retry:
-                    self.framer.resetFrame()
-                    self.send(packet)
-                if self.broadcast_enable and not request.slave_id:
-                    resp = None
-                    break
-                try:
-                    resp = await asyncio.wait_for(
-                        req, timeout=self.comm_params.timeout_connect
-                    )
-                    break
-                except asyncio.exceptions.TimeoutError:
-                    count += 1
+            req = self.build_response(request.transaction_id)
+            if not count or not self.no_resend_on_retry:
+                self.send(packet)
+            if self.broadcast_enable and not request.slave_id:
+                resp = None
+                break
+            try:
+                resp = await asyncio.wait_for(
+                    req, timeout=self.comm_params.timeout_connect
+                )
+                break
+            except asyncio.exceptions.TimeoutError:
+                count += 1
         if count > self.retries:
             self.close(reconnect=True)
             raise ModbusIOException(
                 f"ERROR: No response received after {self.retries} retries"
             )
 
         return resp  # type: ignore[return-value]
 
     def callback_new_connection(self):
         """Call when listener receive new connection request."""
 
     def callback_connected(self) -> None:
         """Call when connection is succcesfull."""
-        if self.on_reconnect_callback:
-            self.on_reconnect_callback()
-        self.framer.resetFrame()
 
     def callback_disconnected(self, exc: Exception | None) -> None:
         """Call when connection is lost."""
         Log.debug("callback_disconnected called: {}", exc)
 
     def callback_data(self, data: bytes, addr: tuple | None = None) -> int:
         """Handle received data.
@@ -313,14 +307,15 @@
         framer: Framer,
         timeout: float = 3,
         retries: int = 3,
         retry_on_empty: bool = False,
         broadcast_enable: bool = False,
         reconnect_delay: float = 0.1,
         reconnect_delay_max: float = 300.0,
+        on_reconnect_callback: Callable[[], None] | None = None,
         no_resend_on_retry: bool = False,
         **kwargs: Any,
     ) -> None:
         """Initialize a client instance."""
         ModbusClientMixin.__init__(self)  # type: ignore[arg-type]
         self.comm_params = CommParams(
             comm_type=kwargs.get("CommType"),
@@ -333,14 +328,15 @@
             port=kwargs.get("port", 0),
             sslctx=kwargs.get("sslctx", None),
             baudrate=kwargs.get("baudrate", None),
             bytesize=kwargs.get("bytesize", None),
             parity=kwargs.get("parity", None),
             stopbits=kwargs.get("stopbits", None),
             handle_local_echo=kwargs.get("handle_local_echo", False),
+            on_reconnect_callback=on_reconnect_callback,
         )
         self.params = self._params()
         self.params.retries = int(retries)
         self.params.retry_on_empty = bool(retry_on_empty)
         self.params.broadcast_enable = bool(broadcast_enable)
         self.retry_on_empty: int = 0
         self.no_resend_on_retry = no_resend_on_retry
```

### Comparing `pymodbus-3.6.8/pymodbus/client/mixin.py` & `pymodbus-3.7.0.dev0/pymodbus/client/mixin.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/client/serial.py` & `pymodbus-3.7.0.dev0/pymodbus/client/serial.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
     async def connect(self) -> bool:
         """Connect Async client."""
         self.reset_delay()
         Log.debug("Connecting to {}.", self.comm_params.host)
         return await self.base_connect()
 
-    def close(self, reconnect: bool = False) -> None:
+    def close(self, reconnect: bool = False) -> None:  # type: ignore[override]
         """Close connection."""
         super().close(reconnect=reconnect)
 
 
 class ModbusSerialClient(ModbusBaseSyncClient):
     """**ModbusSerialClient**.
 
@@ -214,17 +214,15 @@
                 baudrate=self.comm_params.baudrate,
                 parity=self.comm_params.parity,
                 exclusive=True,
             )
             if self.strict:
                 self.socket.inter_byte_timeout = self.inter_byte_timeout
             self.last_frame_end = None
-        # except serial.SerialException as msg:
-        # pyserial raises undocumented exceptions like termios
-        except Exception as msg:  # pylint: disable=broad-exception-caught
+        except serial.SerialException as msg:
             Log.error("{}", msg)
             self.close()
         return self.socket is not None
 
     def close(self):
         """Close the underlying socket connection."""
         if self.socket:
```

### Comparing `pymodbus-3.6.8/pymodbus/client/tcp.py` & `pymodbus-3.7.0.dev0/pymodbus/client/tcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         Log.debug(
             "Connecting to {}:{}.",
             self.comm_params.host,
             self.comm_params.port,
         )
         return await self.base_connect()
 
-    def close(self, reconnect: bool = False) -> None:
+    def close(self, reconnect: bool = False) -> None:  # type: ignore[override]
         """Close connection."""
         super().close(reconnect=reconnect)
 
 
 class ModbusTcpClient(ModbusBaseSyncClient):
     """**ModbusTcpClient**.
```

### Comparing `pymodbus-3.6.8/pymodbus/client/tls.py` & `pymodbus-3.7.0.dev0/pymodbus/client/tls.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/client/udp.py` & `pymodbus-3.7.0.dev0/pymodbus/client/udp.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/constants.py` & `pymodbus-3.7.0.dev0/pymodbus/constants.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/datastore/context.py` & `pymodbus-3.7.0.dev0/pymodbus/datastore/context.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/datastore/remote.py` & `pymodbus-3.7.0.dev0/pymodbus/datastore/remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,21 +46,20 @@
         func_fc = self.__get_callbacks[group_fx]
         self.result = func_fc(_address, _count)
         return self.__extract_result(self.decode(fc_as_hex), self.result)
 
     def setValues(self, fc_as_hex, address, values):
         """Set the datastore with the supplied values."""
         group_fx = self.decode(fc_as_hex)
-        if fc_as_hex not in self._write_fc:
-            raise ValueError(f"setValues() called with an non-write function code {fc_as_hex}")
-        func_fc = self.__set_callbacks[f"{group_fx}{fc_as_hex}"]
-        if fc_as_hex in {0x0F, 0x10}:  # Write Multiple Coils, Write Multiple Registers
-            self.result = func_fc(address, values)
-        else:
-            self.result = func_fc(address, values[0])
+        if fc_as_hex in self._write_fc:
+            func_fc = self.__set_callbacks[f"{group_fx}{fc_as_hex}"]
+            if fc_as_hex in {0x0F, 0x10}:
+                self.result = func_fc(address, values)
+            else:
+                self.result = func_fc(address, values[0])
         if self.result.isError():
             return self.result
         return None
 
     def __str__(self):
         """Return a string representation of the context.
```

### Comparing `pymodbus-3.6.8/pymodbus/datastore/simulator.py` & `pymodbus-3.7.0.dev0/pymodbus/datastore/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     :meta private:
     """
 
     def __init__(self, runtime):
         """Initialize."""
         self.runtime = runtime
         self.config = {}
-        self.config_types: dict[str, dict[str, Any]] = {
+        self.config_types = {
             Label.type_bits: {
                 Label.type: CellType.BITS,
                 Label.next: None,
                 Label.value: 0,
                 Label.action: None,
                 Label.method: self.handle_type_bits,
             },
@@ -744,20 +744,19 @@
             registers[inx].value = regs[0]
             registers[inx + 1].value = regs[1]
 
     # --------------------------------------------
     # Internal helper methods
     # --------------------------------------------
 
-    def validate_type(self, func_code, real_address, count) -> bool:
+    def validate_type(self, func_code, real_address, count):
         """Check if request is done against correct type.
 
         :meta private:
         """
-        check: tuple
         if func_code in self._bits_func_code:
             # Bit access
             check = (CellType.BITS, -1)
             reg_step = 1
         elif count % 2:
             # 16 bit access
             check = (CellType.UINT16, CellType.STRING)
```

### Comparing `pymodbus-3.6.8/pymodbus/datastore/store.py` & `pymodbus-3.7.0.dev0/pymodbus/datastore/store.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/device.py` & `pymodbus-3.7.0.dev0/pymodbus/device.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/diag_message.py` & `pymodbus-3.7.0.dev0/pymodbus/diag_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -378,15 +378,15 @@
     sub_function_code = 0x0003
 
     def execute(self, *args):
         """Execute the diagnostic request on the given device.
 
         :returns: The initialized response message
         """
-        char = (self.message & 0xFF00) >> 8  # type: ignore[operator]
+        char = (self.message & 0xFF00) >> 8
         _MCB._setDelimiter(char)  # pylint: disable=protected-access
         return ChangeAsciiInputDelimiterResponse(self.message)
 
 
 class ChangeAsciiInputDelimiterResponse(DiagnosticStatusSimpleResponse):
     """Change ascii input delimiter.
```

### Comparing `pymodbus-3.6.8/pymodbus/events.py` & `pymodbus-3.7.0.dev0/pymodbus/events.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/exceptions.py` & `pymodbus-3.7.0.dev0/pymodbus/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/factory.py` & `pymodbus-3.7.0.dev0/pymodbus/factory.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,76 +8,162 @@
 Regardless of how many functions are added to the lookup, O(1) behavior is
 kept as a result of a pre-computed lookup dictionary.
 """
 
 # pylint: disable=missing-type-doc
 from typing import Callable, Dict
 
-from pymodbus import bit_read_message as bit_r_msg
-from pymodbus import bit_write_message as bit_w_msg
-from pymodbus import diag_message as diag_msg
-from pymodbus import file_message as file_msg
-from pymodbus import mei_message as mei_msg
-from pymodbus import other_message as o_msg
-from pymodbus import pdu
-from pymodbus import register_read_message as reg_r_msg
-from pymodbus import register_write_message as reg_w_msg
+from pymodbus.bit_read_message import (
+    ReadCoilsRequest,
+    ReadCoilsResponse,
+    ReadDiscreteInputsRequest,
+    ReadDiscreteInputsResponse,
+)
+from pymodbus.bit_write_message import (
+    WriteMultipleCoilsRequest,
+    WriteMultipleCoilsResponse,
+    WriteSingleCoilRequest,
+    WriteSingleCoilResponse,
+)
+from pymodbus.diag_message import (
+    ChangeAsciiInputDelimiterRequest,
+    ChangeAsciiInputDelimiterResponse,
+    ClearCountersRequest,
+    ClearCountersResponse,
+    ClearOverrunCountRequest,
+    ClearOverrunCountResponse,
+    DiagnosticStatusRequest,
+    DiagnosticStatusResponse,
+    ForceListenOnlyModeRequest,
+    ForceListenOnlyModeResponse,
+    GetClearModbusPlusRequest,
+    GetClearModbusPlusResponse,
+    RestartCommunicationsOptionRequest,
+    RestartCommunicationsOptionResponse,
+    ReturnBusCommunicationErrorCountRequest,
+    ReturnBusCommunicationErrorCountResponse,
+    ReturnBusExceptionErrorCountRequest,
+    ReturnBusExceptionErrorCountResponse,
+    ReturnBusMessageCountRequest,
+    ReturnBusMessageCountResponse,
+    ReturnDiagnosticRegisterRequest,
+    ReturnDiagnosticRegisterResponse,
+    ReturnIopOverrunCountRequest,
+    ReturnIopOverrunCountResponse,
+    ReturnQueryDataRequest,
+    ReturnQueryDataResponse,
+    ReturnSlaveBusCharacterOverrunCountRequest,
+    ReturnSlaveBusCharacterOverrunCountResponse,
+    ReturnSlaveBusyCountRequest,
+    ReturnSlaveBusyCountResponse,
+    ReturnSlaveMessageCountRequest,
+    ReturnSlaveMessageCountResponse,
+    ReturnSlaveNAKCountRequest,
+    ReturnSlaveNAKCountResponse,
+    ReturnSlaveNoResponseCountRequest,
+    ReturnSlaveNoResponseCountResponse,
+)
 from pymodbus.exceptions import MessageRegisterException, ModbusException
+from pymodbus.file_message import (
+    ReadFifoQueueRequest,
+    ReadFifoQueueResponse,
+    ReadFileRecordRequest,
+    ReadFileRecordResponse,
+    WriteFileRecordRequest,
+    WriteFileRecordResponse,
+)
 from pymodbus.logging import Log
+from pymodbus.mei_message import (
+    ReadDeviceInformationRequest,
+    ReadDeviceInformationResponse,
+)
+from pymodbus.other_message import (
+    GetCommEventCounterRequest,
+    GetCommEventCounterResponse,
+    GetCommEventLogRequest,
+    GetCommEventLogResponse,
+    ReadExceptionStatusRequest,
+    ReadExceptionStatusResponse,
+    ReportSlaveIdRequest,
+    ReportSlaveIdResponse,
+)
+from pymodbus.pdu import (
+    ExceptionResponse,
+    IllegalFunctionRequest,
+    ModbusRequest,
+    ModbusResponse,
+)
+from pymodbus.pdu import ModbusExceptions as ecode
+from pymodbus.register_read_message import (
+    ReadHoldingRegistersRequest,
+    ReadHoldingRegistersResponse,
+    ReadInputRegistersRequest,
+    ReadInputRegistersResponse,
+    ReadWriteMultipleRegistersRequest,
+    ReadWriteMultipleRegistersResponse,
+)
+from pymodbus.register_write_message import (
+    MaskWriteRegisterRequest,
+    MaskWriteRegisterResponse,
+    WriteMultipleRegistersRequest,
+    WriteMultipleRegistersResponse,
+    WriteSingleRegisterRequest,
+    WriteSingleRegisterResponse,
+)
 
 
 # --------------------------------------------------------------------------- #
 # Server Decoder
 # --------------------------------------------------------------------------- #
 class ServerDecoder:
     """Request Message Factory (Server).
 
     To add more implemented functions, simply add them to the list
     """
 
     __function_table = [
-        reg_r_msg.ReadHoldingRegistersRequest,
-        bit_r_msg.ReadDiscreteInputsRequest,
-        reg_r_msg.ReadInputRegistersRequest,
-        bit_r_msg.ReadCoilsRequest,
-        bit_w_msg.WriteMultipleCoilsRequest,
-        reg_w_msg.WriteMultipleRegistersRequest,
-        reg_w_msg.WriteSingleRegisterRequest,
-        bit_w_msg.WriteSingleCoilRequest,
-        reg_r_msg.ReadWriteMultipleRegistersRequest,
-        diag_msg.DiagnosticStatusRequest,
-        o_msg.ReadExceptionStatusRequest,
-        o_msg.GetCommEventCounterRequest,
-        o_msg.GetCommEventLogRequest,
-        o_msg.ReportSlaveIdRequest,
-        file_msg.ReadFileRecordRequest,
-        file_msg.WriteFileRecordRequest,
-        reg_w_msg.MaskWriteRegisterRequest,
-        file_msg.ReadFifoQueueRequest,
-        mei_msg.ReadDeviceInformationRequest,
+        ReadHoldingRegistersRequest,
+        ReadDiscreteInputsRequest,
+        ReadInputRegistersRequest,
+        ReadCoilsRequest,
+        WriteMultipleCoilsRequest,
+        WriteMultipleRegistersRequest,
+        WriteSingleRegisterRequest,
+        WriteSingleCoilRequest,
+        ReadWriteMultipleRegistersRequest,
+        DiagnosticStatusRequest,
+        ReadExceptionStatusRequest,
+        GetCommEventCounterRequest,
+        GetCommEventLogRequest,
+        ReportSlaveIdRequest,
+        ReadFileRecordRequest,
+        WriteFileRecordRequest,
+        MaskWriteRegisterRequest,
+        ReadFifoQueueRequest,
+        ReadDeviceInformationRequest,
     ]
     __sub_function_table = [
-        diag_msg.ReturnQueryDataRequest,
-        diag_msg.RestartCommunicationsOptionRequest,
-        diag_msg.ReturnDiagnosticRegisterRequest,
-        diag_msg.ChangeAsciiInputDelimiterRequest,
-        diag_msg.ForceListenOnlyModeRequest,
-        diag_msg.ClearCountersRequest,
-        diag_msg.ReturnBusMessageCountRequest,
-        diag_msg.ReturnBusCommunicationErrorCountRequest,
-        diag_msg.ReturnBusExceptionErrorCountRequest,
-        diag_msg.ReturnSlaveMessageCountRequest,
-        diag_msg.ReturnSlaveNoResponseCountRequest,
-        diag_msg.ReturnSlaveNAKCountRequest,
-        diag_msg.ReturnSlaveBusyCountRequest,
-        diag_msg.ReturnSlaveBusCharacterOverrunCountRequest,
-        diag_msg.ReturnIopOverrunCountRequest,
-        diag_msg.ClearOverrunCountRequest,
-        diag_msg.GetClearModbusPlusRequest,
-        mei_msg.ReadDeviceInformationRequest,
+        ReturnQueryDataRequest,
+        RestartCommunicationsOptionRequest,
+        ReturnDiagnosticRegisterRequest,
+        ChangeAsciiInputDelimiterRequest,
+        ForceListenOnlyModeRequest,
+        ClearCountersRequest,
+        ReturnBusMessageCountRequest,
+        ReturnBusCommunicationErrorCountRequest,
+        ReturnBusExceptionErrorCountRequest,
+        ReturnSlaveMessageCountRequest,
+        ReturnSlaveNoResponseCountRequest,
+        ReturnSlaveNAKCountRequest,
+        ReturnSlaveBusyCountRequest,
+        ReturnSlaveBusCharacterOverrunCountRequest,
+        ReturnIopOverrunCountRequest,
+        ClearOverrunCountRequest,
+        GetClearModbusPlusRequest,
+        ReadDeviceInformationRequest,
     ]
 
     @classmethod
     def getFCdict(cls) -> Dict[int, Callable]:
         """Build function code - class list."""
         return {f.function_code: f for f in cls.__function_table}  # type: ignore[attr-defined]
 
@@ -103,28 +189,28 @@
 
     def lookupPduClass(self, function_code):
         """Use `function_code` to determine the class of the PDU.
 
         :param function_code: The function code specified in a frame.
         :returns: The class of the PDU that has a matching `function_code`.
         """
-        return self.lookup.get(function_code, pdu.ExceptionResponse)
+        return self.lookup.get(function_code, ExceptionResponse)
 
     def _helper(self, data: str):
         """Generate the correct request object from a valid request packet.
 
         This decodes from a list of the currently implemented request types.
 
         :param data: The request packet to decode
         :returns: The decoded request or illegal function request object
         """
         function_code = int(data[0])
         if not (request := self.lookup.get(function_code, lambda: None)()):
             Log.debug("Factory Request[{}]", function_code)
-            request = pdu.IllegalFunctionRequest(function_code)
+            request = IllegalFunctionRequest(function_code)
         else:
             fc_string = "{}: {}".format(  # pylint: disable=consider-using-f-string
                 str(self.lookup[function_code])  # pylint: disable=use-maxsplit-arg
                 .split(".")[-1]
                 .rstrip('">"'),
                 function_code,
             )
@@ -140,15 +226,15 @@
 
     def register(self, function):
         """Register a function and sub function class with the decoder.
 
         :param function: Custom function class to register
         :raises MessageRegisterException:
         """
-        if not issubclass(function, pdu.ModbusRequest):
+        if not issubclass(function, ModbusRequest):
             raise MessageRegisterException(
                 f'"{function.__class__.__name__}" is Not a valid Modbus Message'
                 ". Class needs to be derived from "
                 "`pymodbus.pdu.ModbusRequest` "
             )
         self.lookup[function.function_code] = function
         if hasattr(function, "sub_function_code"):
@@ -165,53 +251,53 @@
 class ClientDecoder:
     """Response Message Factory (Client).
 
     To add more implemented functions, simply add them to the list
     """
 
     function_table = [
-        reg_r_msg.ReadHoldingRegistersResponse,
-        bit_r_msg.ReadDiscreteInputsResponse,
-        reg_r_msg.ReadInputRegistersResponse,
-        bit_r_msg.ReadCoilsResponse,
-        bit_w_msg.WriteMultipleCoilsResponse,
-        reg_w_msg.WriteMultipleRegistersResponse,
-        reg_w_msg.WriteSingleRegisterResponse,
-        bit_w_msg.WriteSingleCoilResponse,
-        reg_r_msg.ReadWriteMultipleRegistersResponse,
-        diag_msg.DiagnosticStatusResponse,
-        o_msg.ReadExceptionStatusResponse,
-        o_msg.GetCommEventCounterResponse,
-        o_msg.GetCommEventLogResponse,
-        o_msg.ReportSlaveIdResponse,
-        file_msg.ReadFileRecordResponse,
-        file_msg.WriteFileRecordResponse,
-        reg_w_msg.MaskWriteRegisterResponse,
-        file_msg.ReadFifoQueueResponse,
-        mei_msg.ReadDeviceInformationResponse,
+        ReadHoldingRegistersResponse,
+        ReadDiscreteInputsResponse,
+        ReadInputRegistersResponse,
+        ReadCoilsResponse,
+        WriteMultipleCoilsResponse,
+        WriteMultipleRegistersResponse,
+        WriteSingleRegisterResponse,
+        WriteSingleCoilResponse,
+        ReadWriteMultipleRegistersResponse,
+        DiagnosticStatusResponse,
+        ReadExceptionStatusResponse,
+        GetCommEventCounterResponse,
+        GetCommEventLogResponse,
+        ReportSlaveIdResponse,
+        ReadFileRecordResponse,
+        WriteFileRecordResponse,
+        MaskWriteRegisterResponse,
+        ReadFifoQueueResponse,
+        ReadDeviceInformationResponse,
     ]
     __sub_function_table = [
-        diag_msg.ReturnQueryDataResponse,
-        diag_msg.RestartCommunicationsOptionResponse,
-        diag_msg.ReturnDiagnosticRegisterResponse,
-        diag_msg.ChangeAsciiInputDelimiterResponse,
-        diag_msg.ForceListenOnlyModeResponse,
-        diag_msg.ClearCountersResponse,
-        diag_msg.ReturnBusMessageCountResponse,
-        diag_msg.ReturnBusCommunicationErrorCountResponse,
-        diag_msg.ReturnBusExceptionErrorCountResponse,
-        diag_msg.ReturnSlaveMessageCountResponse,
-        diag_msg.ReturnSlaveNoResponseCountResponse,
-        diag_msg.ReturnSlaveNAKCountResponse,
-        diag_msg.ReturnSlaveBusyCountResponse,
-        diag_msg.ReturnSlaveBusCharacterOverrunCountResponse,
-        diag_msg.ReturnIopOverrunCountResponse,
-        diag_msg.ClearOverrunCountResponse,
-        diag_msg.GetClearModbusPlusResponse,
-        mei_msg.ReadDeviceInformationResponse,
+        ReturnQueryDataResponse,
+        RestartCommunicationsOptionResponse,
+        ReturnDiagnosticRegisterResponse,
+        ChangeAsciiInputDelimiterResponse,
+        ForceListenOnlyModeResponse,
+        ClearCountersResponse,
+        ReturnBusMessageCountResponse,
+        ReturnBusCommunicationErrorCountResponse,
+        ReturnBusExceptionErrorCountResponse,
+        ReturnSlaveMessageCountResponse,
+        ReturnSlaveNoResponseCountResponse,
+        ReturnSlaveNAKCountResponse,
+        ReturnSlaveBusyCountResponse,
+        ReturnSlaveBusCharacterOverrunCountResponse,
+        ReturnIopOverrunCountResponse,
+        ClearOverrunCountResponse,
+        GetClearModbusPlusResponse,
+        ReadDeviceInformationResponse,
     ]
 
     def __init__(self) -> None:
         """Initialize the client lookup tables."""
         functions = {f.function_code for f in self.function_table}  # type: ignore[attr-defined]
         self.lookup = {f.function_code: f for f in self.function_table}  # type: ignore[attr-defined]
         self.__sub_lookup: Dict[int, Dict[int, Callable]] = {f: {} for f in functions}
@@ -220,15 +306,15 @@
 
     def lookupPduClass(self, function_code):
         """Use `function_code` to determine the class of the PDU.
 
         :param function_code: The function code specified in a frame.
         :returns: The class of the PDU that has a matching `function_code`.
         """
-        return self.lookup.get(function_code, pdu.ExceptionResponse)
+        return self.lookup.get(function_code, ExceptionResponse)
 
     def decode(self, message):
         """Decode a response packet.
 
         :param message: The raw packet to decode
         :return: The decoded modbus message or None if error
         """
@@ -258,29 +344,29 @@
                 .rstrip('">"'),
                 function_code,
             )
         Log.debug("Factory Response[{}]", fc_string)
         response = self.lookup.get(function_code, lambda: None)()
         if function_code > 0x80:
             code = function_code & 0x7F  # strip error portion
-            response = pdu.ExceptionResponse(code, pdu.ModbusExceptions.IllegalFunction)
+            response = ExceptionResponse(code, ecode.IllegalFunction)
         if not response:
             raise ModbusException(f"Unknown response {function_code}")
         response.decode(data[1:])
 
         if hasattr(response, "sub_function_code"):
             lookup = self.__sub_lookup.get(response.function_code, {})
             if subtype := lookup.get(response.sub_function_code, None):
                 response.__class__ = subtype
 
         return response
 
     def register(self, function):
         """Register a function and sub function class with the decoder."""
-        if function and not issubclass(function, pdu.ModbusResponse):
+        if function and not issubclass(function, ModbusResponse):
             raise MessageRegisterException(
                 f'"{function.__class__.__name__}" is Not a valid Modbus Message'
                 ". Class needs to be derived from "
                 "`pymodbus.pdu.ModbusResponse` "
             )
         self.lookup[function.function_code] = function
         if hasattr(function, "sub_function_code"):
```

### Comparing `pymodbus-3.6.8/pymodbus/file_message.py` & `pymodbus-3.7.0.dev0/pymodbus/file_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         """Encode the response.
 
         :returns: The byte encoded message
         """
         total = sum(record.response_length + 1 for record in self.records)
         packet = struct.pack("B", total)
         for record in self.records:
-            packet += struct.pack(">BB", record.record_length, 0x06)
+            packet += struct.pack(">BB", 0x06, record.record_length)
             packet += record.record_data
         return packet
 
     def decode(self, data):
         """Decode the response.
 
         :param data: The packet data to decode
```

### Comparing `pymodbus-3.6.8/pymodbus/framer/__init__.py` & `pymodbus-3.7.0.dev0/pymodbus/framer/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/framer/ascii_framer.py` & `pymodbus-3.7.0.dev0/pymodbus/framer/ascii_framer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Ascii_framer."""
 # pylint: disable=missing-type-doc
-from binascii import a2b_hex
+import struct
+from binascii import a2b_hex, b2a_hex
 
 from pymodbus.exceptions import ModbusIOException
 from pymodbus.framer.base import BYTE_ORDER, FRAME_HEADER, ModbusFramer
 from pymodbus.logging import Log
 from pymodbus.message.ascii import MessageAscii
 
 
@@ -36,15 +37,14 @@
 
         :param decoder: The decoder implementation to use
         """
         super().__init__(decoder, client)
         self._hsize = 0x02
         self._start = b":"
         self._end = b"\r\n"
-        self.message_handler = MessageAscii([0], True)
 
     def decode_data(self, data):
         """Decode data."""
         if len(data) > 1:
             uid = int(data[1:3], 16)
             fcode = int(data[3:5], 16)
             return {"slave": uid, "fcode": fcode}
@@ -91,13 +91,28 @@
             self._buffer = self._buffer[self._header["len"] + 2 :]
             self._header = {"lrc": "0000", "len": 0, "uid": 0x00}
             callback(result)  # defer this
 
     def buildPacket(self, message):
         """Create a ready to send modbus packet.
 
+        Built off of a  modbus request/response
+
         :param message: The request/response to send
         :return: The encoded packet
         """
-        data = message.function_code.to_bytes(1,'big') + message.encode()
-        packet = self.message_handler.encode(data, message.slave_id, message.transaction_id)
-        return packet
+        encoded = message.encode()
+        buffer = struct.pack(
+            ASCII_FRAME_HEADER, message.slave_id, message.function_code
+        )
+        checksum = MessageAscii.compute_LRC(buffer + encoded)
+
+        packet = bytearray()
+        packet.extend(self._start)
+        packet.extend(f"{message.slave_id:02x}{message.function_code:02x}".encode())
+        packet.extend(b2a_hex(encoded))
+        packet.extend(f"{checksum:02x}".encode())
+        packet.extend(self._end)
+        return bytes(packet).upper()
+
+
+# __END__
```

### Comparing `pymodbus-3.6.8/pymodbus/framer/base.py` & `pymodbus-3.7.0.dev0/pymodbus/framer/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,16 +127,16 @@
         :param data: The new packet data
         :param callback: The function to send results to
         :param slave: Process if slave id matches, ignore otherwise (could be a
                list of slave ids (server) or single slave id(client/server))
         :param kwargs:
         :raises ModbusIOException:
         """
+        Log.debug("Processing: {}", data, ":hex")
         self._buffer += data
-        Log.debug("Processing: {}", self._buffer, ":hex")
         if not isinstance(slave, (list, tuple)):
             slave = [slave]
         single = kwargs.pop("single", False)
         self.frameProcessIncomingPacket(single, callback, slave, **kwargs)
 
     def frameProcessIncomingPacket(
         self, _single, _callback, _slave, _tid=None, **kwargs
```

### Comparing `pymodbus-3.6.8/pymodbus/framer/binary_framer.py` & `pymodbus-3.7.0.dev0/pymodbus/framer/binary_framer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Binary framer."""
 # pylint: disable=missing-type-doc
 import struct
 
 from pymodbus.exceptions import ModbusIOException
 from pymodbus.framer.base import BYTE_ORDER, FRAME_HEADER, ModbusFramer
 from pymodbus.logging import Log
-from pymodbus.message.rtu import MessageRTU
+from pymodbus.utilities import checkCRC, computeCRC
 
 
 BINARY_FRAME_HEADER = BYTE_ORDER + FRAME_HEADER
 
 # --------------------------------------------------------------------------- #
 # Modbus Binary Message
 # --------------------------------------------------------------------------- #
@@ -72,15 +72,15 @@
                 self._buffer = self._buffer[start:]
 
             if (end := self._buffer.find(self._end)) != -1:
                 self._header["len"] = end
                 self._header["uid"] = struct.unpack(">B", self._buffer[1:2])[0]
                 self._header["crc"] = struct.unpack(">H", self._buffer[end - 2 : end])[0]
                 data = self._buffer[1 : end - 2]
-                return MessageRTU.check_CRC(data, self._header["crc"])
+                return checkCRC(data, self._header["crc"])
             return False
 
         while len(self._buffer) > 1:
             if not check_frame(self):
                 Log.debug("Frame check failed, ignoring!!")
                 break
             if not self._validate_slave_id(slave, single):
@@ -109,15 +109,15 @@
         :returns: The encoded packet
         """
         data = self._preflight(message.encode())
         packet = (
             struct.pack(BINARY_FRAME_HEADER, message.slave_id, message.function_code)
             + data
         )
-        packet += struct.pack(">H", MessageRTU.compute_CRC(packet))
+        packet += struct.pack(">H", computeCRC(packet))
         packet = self._start + packet + self._end
         return packet
 
     def _preflight(self, data):
         """Do preflight buffer test.
 
         This basically scans the buffer for start and end
@@ -128,7 +128,10 @@
         """
         array = bytearray()
         for item in data:
             if item in self._repeat:
                 array.append(item)
             array.append(item)
         return bytes(array)
+
+
+# __END__
```

### Comparing `pymodbus-3.6.8/pymodbus/framer/rtu_framer.py` & `pymodbus-3.7.0.dev0/pymodbus/framer/rtu_framer.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import time
 
 from pymodbus.exceptions import (
     ModbusIOException,
 )
 from pymodbus.framer.base import BYTE_ORDER, FRAME_HEADER, ModbusFramer
 from pymodbus.logging import Log
-from pymodbus.message.rtu import MessageRTU
-from pymodbus.utilities import ModbusTransactionState
+from pymodbus.utilities import ModbusTransactionState, checkCRC, computeCRC
 
 
 RTU_FRAME_HEADER = BYTE_ORDER + FRAME_HEADER
 
 
 # --------------------------------------------------------------------------- #
 # Modbus RTU Message
@@ -59,15 +58,14 @@
         :param decoder: The decoder factory implementation to use
         """
         super().__init__(decoder, client)
         self._hsize = 0x01
         self._end = b"\x0d\x0a"
         self._min_frame_size = 4
         self.function_codes = decoder.lookup.keys() if decoder else {}
-        self.message_handler = MessageRTU([0], True)
 
     def decode_data(self, data):
         """Decode data."""
         if len(data) > self._hsize:
             uid = int(data[0])
             fcode = int(data[1])
             return {"slave": uid, "fcode": fcode}
@@ -129,15 +127,15 @@
                 if len(self._buffer) < size:
                     raise IndexError
                 self._header["crc"] = self._buffer[size - 2 : size]
                 frame_size = self._header["len"]
                 data = self._buffer[: frame_size - 2]
                 crc = self._header["crc"]
                 crc_val = (int(crc[0]) << 8) + int(crc[1])
-                return MessageRTU.check_CRC(data, crc_val)
+                return checkCRC(data, crc_val)
             except (IndexError, KeyError, struct.error):
                 return False
 
         broadcast = not slave[0]
         skip_cur_frame = False
         while get_frame_start(self, slave, broadcast, skip_cur_frame):
             self._header = {"uid": 0x00, "len": 0, "crc": b"\x00\x00"}
@@ -168,17 +166,20 @@
             callback(result)  # defer or push to a thread?
 
     def buildPacket(self, message):
         """Create a ready to send modbus packet.
 
         :param message: The populated request/response to send
         """
-        data = message.function_code.to_bytes(1, 'big') + message.encode()
-        packet = self.message_handler.encode(data, message.slave_id, message.transaction_id)
-
+        data = message.encode()
+        packet = (
+            struct.pack(RTU_FRAME_HEADER, message.slave_id, message.function_code)
+            + data
+        )
+        packet += struct.pack(">H", computeCRC(packet))
         # Ensure that transaction is actually the slave id for serial comms
         if message.slave_id:
             message.transaction_id = message.slave_id
         return packet
 
     def sendPacket(self, message):
         """Send packets on the bus with 3.5char delay between frames.
```

### Comparing `pymodbus-3.6.8/pymodbus/framer/socket_framer.py` & `pymodbus-3.7.0.dev0/pymodbus/framer/socket_framer.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import struct
 
 from pymodbus.exceptions import (
     ModbusIOException,
 )
 from pymodbus.framer.base import SOCKET_FRAME_HEADER, ModbusFramer
 from pymodbus.logging import Log
-from pymodbus.message.socket import MessageSocket
 
 
 # --------------------------------------------------------------------------- #
 # Modbus TCP Message
 # --------------------------------------------------------------------------- #
 
 
@@ -39,15 +38,14 @@
     def __init__(self, decoder, client=None):
         """Initialize a new instance of the framer.
 
         :param decoder: The decoder factory implementation to use
         """
         super().__init__(decoder, client)
         self._hsize = 0x07
-        self.message_handler = MessageSocket([0], True)
 
     def decode_data(self, data):
         """Decode data."""
         if len(data) > self._hsize:
             tid, pid, length, uid, fcode = struct.unpack(
                 SOCKET_FRAME_HEADER, data[0 : self._hsize + 1]
             )
@@ -56,49 +54,43 @@
                 "pid": pid,
                 "length": length,
                 "slave": uid,
                 "fcode": fcode,
             }
         return {}
 
-    def frameProcessIncomingPacket(self, single, callback, slave, tid=None, **kwargs):  # noqa: C901
+    def frameProcessIncomingPacket(self, single, callback, slave, tid=None, **kwargs):
         """Process new packet pattern.
 
         This takes in a new request packet, adds it to the current
         packet stream, and performs framing on it. That is, checks
         for complete messages, and once found, will process all that
         exist.  This handles the case when we read N + 1 or 1 // N
         messages at a time instead of 1.
 
         The processed and decoded messages are pushed to the callback
         function to process and send.
         """
         def check_frame(self):
             """Check and decode the next frame."""
-            if not self._buffer:
-                Log.debug("Frame check, no more data!")
-                return False
-            if not len(self._buffer) >= self._hsize +1:
-                Log.debug("Frame check failed, short frame {} >= {} !!", len(self._buffer), self._hsize+2)
+            if not len(self._buffer) > self._hsize:
                 return False
             (
                 self._header["tid"],
                 self._header["pid"],
                 self._header["len"],
                 self._header["uid"],
             ) = struct.unpack(">HHHB", self._buffer[0 : self._hsize])
-            if self._header["len"] == 2 and len(self._buffer) >= self._hsize + 2:
-                self._header["len"] = 3
             if self._header["len"] < 2:
                 length = self._hsize + self._header["len"] -1
                 self._buffer = self._buffer[length:]
                 self._header = {"tid": 0, "pid": 0, "len": 0, "uid": 0}
             elif len(self._buffer) - self._hsize + 1 >= self._header["len"]:
                 return True
-            Log.debug("Frame check failed, missing part of message len {}, MBAP len {} !!", len(self._buffer), self._header["len"])
+            Log.debug("Frame check failed, missing part of message!!")
             return False
 
         while True:
             if not check_frame(self):
                 return
             if not self._validate_slave_id(slave, single):
                 header_txt = self._header["uid"]
@@ -120,10 +112,18 @@
                 callback(result)  # defer or push to a thread?
 
     def buildPacket(self, message):
         """Create a ready to send modbus packet.
 
         :param message: The populated request/response to send
         """
-        data = message.function_code.to_bytes(1, 'big') + message.encode()
-        packet = self.message_handler.encode(data, message.slave_id, message.transaction_id)
+        data = message.encode()
+        packet = struct.pack(
+            SOCKET_FRAME_HEADER,
+            message.transaction_id,
+            message.protocol_id,
+            len(data) + 2,
+            message.slave_id,
+            message.function_code,
+        )
+        packet += data
         return packet
```

### Comparing `pymodbus-3.6.8/pymodbus/framer/tls_framer.py` & `pymodbus-3.7.0.dev0/pymodbus/framer/tls_framer.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import struct
 
 from pymodbus.exceptions import (
     ModbusIOException,
 )
 from pymodbus.framer.base import TLS_FRAME_HEADER, ModbusFramer
 from pymodbus.logging import Log
-from pymodbus.message.tls import MessageTLS
 
 
 # --------------------------------------------------------------------------- #
 # Modbus TLS Message
 # --------------------------------------------------------------------------- #
 
 
@@ -31,15 +30,14 @@
     def __init__(self, decoder, client=None):
         """Initialize a new instance of the framer.
 
         :param decoder: The decoder factory implementation to use
         """
         super().__init__(decoder, client)
         self._hsize = 0x0
-        self.message_encoder = MessageTLS([0], True)
 
     def decode_data(self, data):
         """Decode data."""
         if len(data) > self._hsize:
             (fcode,) = struct.unpack(TLS_FRAME_HEADER, data[0 : self._hsize + 1])
             return {"fcode": fcode}
         return {}
@@ -75,10 +73,14 @@
         callback(result)  # defer or push to a thread?
 
     def buildPacket(self, message):
         """Create a ready to send modbus packet.
 
         :param message: The populated request/response to send
         """
-        data = message.function_code.to_bytes(1,'big') + message.encode()
-        packet = self.message_encoder.encode(data, message.slave_id, message.transaction_id)
+        data = message.encode()
+        packet = struct.pack(TLS_FRAME_HEADER, message.function_code)
+        packet += data
         return packet
+
+
+# __END__
```

### Comparing `pymodbus-3.6.8/pymodbus/logging.py` & `pymodbus-3.7.0.dev0/pymodbus/logging.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/mei_message.py` & `pymodbus-3.7.0.dev0/pymodbus/mei_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/message/ascii.py` & `pymodbus-3.7.0.dev0/pymodbus/message/ascii.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/message/base.py` & `pymodbus-3.7.0.dev0/pymodbus/message/base.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/message/message.py` & `pymodbus-3.7.0.dev0/pymodbus/message/message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/message/raw.py` & `pymodbus-3.7.0.dev0/pymodbus/message/raw.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/message/socket.py` & `pymodbus-3.7.0.dev0/pymodbus/message/socket.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/message/tls.py` & `pymodbus-3.7.0.dev0/pymodbus/message/tls.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/other_message.py` & `pymodbus-3.7.0.dev0/pymodbus/other_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/payload.py` & `pymodbus-3.7.0.dev0/pymodbus/payload.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/pdu.py` & `pymodbus-3.7.0.dev0/pymodbus/pdu.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/register_read_message.py` & `pymodbus-3.7.0.dev0/pymodbus/register_read_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/register_write_message.py` & `pymodbus-3.7.0.dev0/pymodbus/register_write_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/server/__init__.py` & `pymodbus-3.7.0.dev0/pymodbus/server/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/server/async_io.py` & `pymodbus-3.7.0.dev0/pymodbus/server/async_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             timeout_connect=0.0,
             host=owner.comm_params.source_address[0],
             port=owner.comm_params.source_address[1],
         )
         super().__init__(params, False)
         self.server = owner
         self.running = False
-        self.receive_queue: asyncio.Queue = asyncio.Queue()
+        self.receive_queue = asyncio.Queue()
         self.handler_task = None  # coroutine to be run on asyncio loop
         self.framer: ModbusFramer
 
     def _log_exception(self):
         """Show log exception."""
         Log.debug(
             "Handler for stream [{}] has been canceled", self.comm_params.comm_name
@@ -108,15 +108,15 @@
         slaves = self.server.context.slaves()
         # this is an asyncio.Queue await, it will never fail
         data = await self._recv_()
         if isinstance(data, tuple):
             # addr is populated when talking over UDP
             data, *addr = data
         else:
-            addr = [None]
+            addr = (None,)  # empty tuple
 
         # if broadcast is enabled make sure to
         # process requests to address 0
         if self.server.broadcast_enable:
             if 0 not in slaves:
                 slaves.append(0)
 
@@ -126,47 +126,58 @@
         self.framer.processIncomingPacket(
             data=data,
             callback=lambda x: self.execute(x, *addr),
             slave=slaves,
             single=single,
         )
 
-    async def handle(self) -> None:
-        """Coroutine which represents a single master <=> slave conversation.
+    async def handle(self):
+        """Return Asyncio coroutine which represents a single conversation.
+
+        between the modbus slave and master
 
         Once the client connection is established, the data chunks will be
         fed to this coroutine via the asyncio.Queue object which is fed by
         the ModbusServerRequestHandler class's callback Future.
 
-        This callback future gets data from either asyncio.BaseProtocol.data_received
-        or asyncio.DatagramProtocol.datagram_received.
+        This callback future gets data from either
 
         This function will execute without blocking in the while-loop and
         yield to the asyncio event loop when the frame is exhausted.
         As a result, multiple clients can be interleaved without any
         interference between them.
         """
+        reset_frame = False
         while self.running:
             try:
                 await self.inner_handle()
             except asyncio.CancelledError:
                 # catch and ignore cancellation errors
                 if self.running:
                     self._log_exception()
                     self.running = False
             except Exception as exc:  # pylint: disable=broad-except
                 # force TCP socket termination as processIncomingPacket
                 # should handle application layer errors
-                Log.error(
-                    'Unknown exception "{}" on stream {} forcing disconnect',
-                    exc,
-                    self.comm_params.comm_name,
-                )
-                self.close()
-                self.callback_disconnected(exc)
+                # for UDP sockets, simply reset the frame
+                if isinstance(self, ModbusServerRequestHandler):
+                    Log.error(
+                        'Unknown exception "{}" on stream {} forcing disconnect',
+                        exc,
+                        self.comm_params.comm_name,
+                    )
+                    self.close()
+                    self.callback_disconnected(exc)
+                else:
+                    Log.error("Unknown error occurred {}", exc)
+                    reset_frame = True  # graceful recovery
+            finally:
+                if reset_frame:
+                    self.framer.resetFrame()
+                    reset_frame = False
 
     def execute(self, request, *addr):
         """Call with the resulting message.
 
         :param request: The decoded request message
         :param addr: the address
         """
@@ -560,29 +571,29 @@
 
     def __init__(self, server):
         """Register new server."""
         self.server = server
         self.loop = asyncio.get_event_loop()
 
     @classmethod
-    async def run(cls, server, custom_functions) -> None:
+    async def run(cls, server, custom_functions):
         """Help starting/stopping server."""
         for func in custom_functions:
             server.decoder.register(func)
-        cls.active_server = _serverList(server)  # type: ignore[assignment]
+        cls.active_server = _serverList(server)
         with suppress(asyncio.exceptions.CancelledError):
             await server.serve_forever()
 
     @classmethod
-    async def async_stop(cls) -> None:
+    async def async_stop(cls):
         """Wait for server stop."""
         if not cls.active_server:
             raise RuntimeError("ServerAsyncStop called without server task active.")
-        await cls.active_server.server.shutdown()  # type: ignore[union-attr]
-        cls.active_server = None  # type: ignore[assignment]
+        await cls.active_server.server.shutdown()
+        cls.active_server = None
 
     @classmethod
     def stop(cls):
         """Wait for server stop."""
         if not cls.active_server:
             Log.info("ServerStop called without server task active.")
             return
```

### Comparing `pymodbus-3.6.8/pymodbus/server/simulator/http_server.py` & `pymodbus-3.7.0.dev0/pymodbus/server/simulator/http_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,21 +176,21 @@
                 web.post("/api/{tail:[a-z]*}", self.handle_json),
                 web.get("/{tail:[a-z0-9.]*}", self.handle_html_static),
                 web.get("/", self.handle_html_static),
             ]
         )
         self.web_app.on_startup.append(self.start_modbus_server)
         self.web_app.on_shutdown.append(self.stop_modbus_server)
-        self.generator_html: dict[str, list] = {
+        self.generator_html = {
             "log": ["", self.build_html_log],
             "registers": ["", self.build_html_registers],
             "calls": ["", self.build_html_calls],
             "server": ["", self.build_html_server],
         }
-        self.generator_json: dict[str, list] = {
+        self.generator_json = {
             "log_json": [None, self.build_json_log],
             "registers_json": [None, self.build_json_registers],
             "calls_json": [None, self.build_json_calls],
             "server_json": [None, self.build_json_server],
         }
         self.submit = {
             "Clear": self.action_clear,
@@ -340,15 +340,15 @@
             .replace("<!--REGISTER_TYPES-->", register_types)
             .replace("<!--REGISTER_FOOT-->", foot)
             .replace("<!--REGISTER_ROWS-->", rows)
             .replace("<!--RESULT-->", result_txt)
         )
         return new_html
 
-    def build_html_calls(self, params: dict, html: str) -> str:
+    def build_html_calls(self, params, html):
         """Build html calls page."""
         result_txt, foot = self.helper_build_html_submit(params)
         if not foot:
             foot = "Montitoring active" if self.call_monitor.active else "not active"
         if not result_txt:
             result_txt = "ok"
 
@@ -376,29 +376,29 @@
             if self.call_monitor.range_stop != -1
             else ""
         )
         function_codes = ""
         for function in self.request_lookup.values():
             selected = (
                 "selected"
-                if function.function_code == self.call_monitor.function  #type: ignore[attr-defined]
+                if function.function_code == self.call_monitor.function
                 else ""
             )
-            function_codes += f"<option value={function.function_code} {selected}>{function.function_code_name}</option>"  #type: ignore[attr-defined]
+            function_codes += f"<option value={function.function_code} {selected}>{function.function_code_name}</option>"
         simulation_action = (
             "ACTIVE" if self.call_response.active != RESPONSE_INACTIVE else ""
         )
 
         max_len = MAX_FILTER if self.call_monitor.active else 0
         while len(self.call_list) > max_len:
             del self.call_list[0]
         call_rows = ""
         for entry in reversed(self.call_list):
             # req_obj = self.request_lookup[entry[1]]
-            call_rows += f"<tr><td>{entry.call} - {entry.fc}</td><td>{entry.address}</td><td>{entry.count}</td><td>{entry.data.decode()}</td></tr>"
+            call_rows += f"<tr><td>{entry.call} - {entry.fc}</td><td>{entry.address}</td><td>{entry.count}</td><td>{entry.data}</td></tr>"
             # line += req_obj.funcion_code_name
         new_html = (
             html.replace("<!--SIMULATION_ACTIVE-->", simulation_action)
             .replace("FUNCTION_RANGE_START", range_start_html)
             .replace("FUNCTION_RANGE_STOP", range_stop_html)
             .replace("<!--FUNCTION_CODES-->", function_codes)
             .replace(
```

### Comparing `pymodbus-3.6.8/pymodbus/server/simulator/main.py` & `pymodbus-3.7.0.dev0/pymodbus/server/simulator/main.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/server/simulator/setup.json` & `pymodbus-3.7.0.dev0/pymodbus/server/simulator/setup.json`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/server/simulator/web/apple120.png` & `pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/apple120.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/server/simulator/web/apple152.png` & `pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/apple152.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/server/simulator/web/apple60.png` & `pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/apple60.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/server/simulator/web/apple76.png` & `pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/apple76.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/server/simulator/web/favicon.ico` & `pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/server/simulator/web/generator/calls` & `pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/generator/calls`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/server/simulator/web/generator/log` & `pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/generator/log`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png` & `pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/server/simulator/web/generator/registers` & `pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/generator/registers`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/server/simulator/web/generator/server` & `pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/generator/server`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/server/simulator/web/index.html` & `pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/index.html`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/server/simulator/web/pymodbus.css` & `pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/pymodbus.css`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/server/simulator/web/welcome.html` & `pymodbus-3.7.0.dev0/pymodbus/server/simulator/web/welcome.html`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus/transaction.py` & `pymodbus-3.7.0.dev0/pymodbus/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import struct
 import time
 from contextlib import suppress
 from functools import partial
 from threading import RLock
 
 from pymodbus.exceptions import (
-    ConnectionException,
     InvalidMessageReceivedException,
     ModbusIOException,
 )
 from pymodbus.framer.ascii_framer import ModbusAsciiFramer
 from pymodbus.framer.binary_framer import ModbusBinaryFramer
 from pymodbus.framer.rtu_framer import ModbusRtuFramer
 from pymodbus.framer.socket_framer import ModbusSocketFramer
@@ -238,15 +237,15 @@
                             response = self.getTransaction(tid=0)
                         else:
                             last_exception = last_exception or (
                                 "No Response received from the remote slave"
                                 "/Unable to decode response"
                             )
                             response = ModbusIOException(
-                                last_exception, request.function_code  # type: ignore[assignment]
+                                last_exception, request.function_code
                             )
                         self.client.close()
                     if hasattr(self.client, "state"):
                         Log.debug(
                             "Changing transaction state from "
                             '"PROCESSING REPLY" to '
                             '"TRANSACTION_COMPLETE"'
@@ -322,15 +321,15 @@
                     'Changing transaction state from "SENDING" '
                     'to "WAITING FOR REPLY"'
                 )
                 self.client.state = ModbusTransactionState.WAITING_FOR_REPLY
             result = self._recv(response_length, full)
             # result2 = self._recv(response_length, full)
             Log.debug("RECV: {}", result, ":hex")
-        except (OSError, ModbusIOException, InvalidMessageReceivedException, ConnectionException) as msg:
+        except (OSError, ModbusIOException, InvalidMessageReceivedException) as msg:
             self.client.close()
             Log.debug("Transaction failed. ({}) ", msg)
             last_exception = msg
             result = b""
         return result, last_exception
 
     def _send(self, packet, _retrying=False):
@@ -383,15 +382,15 @@
                     elif expected_response_length is None and isinstance(
                         self.client.framer, ModbusRtuFramer
                     ):
                         with suppress(
                             IndexError  # response length indeterminate with available bytes
                         ):
                             expected_response_length = (
-                                self._get_expected_response_length(
+                                self.client.framer.get_expected_response_length(
                                     read_min
                                 )
                             )
                     if expected_response_length is not None:
                         expected_response_length -= min_size
                         total = expected_response_length + min_size
                 else:
@@ -421,25 +420,14 @@
             Log.debug(
                 "Changing transaction state from "
                 '"WAITING FOR REPLY" to "PROCESSING REPLY"'
             )
             self.client.state = ModbusTransactionState.PROCESSING_REPLY
         return result
 
-    def _get_expected_response_length(self, data):
-        """Get the expected response length.
-
-        :param data: Message data read so far
-        :raises IndexError: If not enough data to read byte count
-        :return: Total frame size
-        """
-        func_code = int(data[1])
-        pdu_class = self.client.framer.decoder.lookupPduClass(func_code)
-        return pdu_class.calculateRtuFrameSize(data)
-
     def addTransaction(self, request, tid=None):
         """Add a transaction to the handler.
 
         This holds the request in case it needs to be resent.
         After being sent, the request is removed.
 
         :param request: The request to hold on to
```

### Comparing `pymodbus-3.6.8/pymodbus/transport/serialtransport.py` & `pymodbus-3.7.0.dev0/pymodbus/transport/serialtransport.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,17 @@
         self.intern_protocol: asyncio.BaseProtocol = protocol
         self.sync_serial = serial.serial_for_url(*args, **kwargs)
         self.intern_write_buffer: list[bytes] = []
         self.poll_task: asyncio.Task | None = None
         self._poll_wait_time = 0.0005
         self.sync_serial.timeout = 0
         self.sync_serial.write_timeout = 0
+        self.future: asyncio.Task | None = None
 
-    def setup(self) -> None:
+    def setup(self):
         """Prepare to read/write."""
         if os.name == "nt" or self.force_poll:
             self.poll_task = asyncio.create_task(self.polling_task())
             self.poll_task.set_name("SerialTransport poll")
         else:
             self.async_loop.add_reader(self.sync_serial.fileno(), self.intern_read_ready)
         self.async_loop.call_soon(self.intern_protocol.connection_made, self)
@@ -39,14 +40,15 @@
     def close(self, exc: Exception | None = None) -> None:
         """Close the transport gracefully."""
         if not self.sync_serial:
             return
         self.flush()
         if self.poll_task:
             self.poll_task.cancel()
+            self.future = asyncio.ensure_future(self.poll_task)
             self.poll_task = None
         else:
             self.async_loop.remove_reader(self.sync_serial.fileno())
         self.sync_serial.close()
         self.sync_serial = None  # type: ignore[assignment]
         if exc:
             with contextlib.suppress(Exception):
@@ -114,47 +116,51 @@
 
     def abort(self) -> None:
         """Alias for closing the connection."""
         self.close()
 
     # ------------------------------------------------
 
-    def intern_read_ready(self) -> None:
+    def intern_read_ready(self):
         """Test if there are data waiting."""
         try:
             if data := self.sync_serial.read(1024):
-                self.intern_protocol.data_received(data)  # type: ignore[attr-defined]
+                self.intern_protocol.data_received(data)
         except serial.SerialException as exc:
             self.close(exc=exc)
 
-    def intern_write_ready(self) -> None:
+    def intern_write_ready(self):
         """Asynchronously write buffered data."""
         data = b"".join(self.intern_write_buffer)
         try:
-            if (nlen := self.sync_serial.write(data)) and nlen < len(data):
+            if (nlen := self.sync_serial.write(data)) < len(data):
                 self.intern_write_buffer = [data[nlen:]]
                 if not self.poll_task:
                     self.async_loop.add_writer(
                         self.sync_serial.fileno(), self.intern_write_ready
                     )
                 return
             self.flush()
         except (BlockingIOError, InterruptedError):
             return
         except serial.SerialException as exc:
             self.close(exc=exc)
 
     async def polling_task(self):
         """Poll and try to read/write."""
-        while self.sync_serial:
-            await asyncio.sleep(self._poll_wait_time)
-            while self.intern_write_buffer:
-                self.intern_write_ready()
-            if self.sync_serial.in_waiting:
-                self.intern_read_ready()
+        try:
+            while self.sync_serial:
+                await asyncio.sleep(self._poll_wait_time)
+                while self.intern_write_buffer:
+                    self.intern_write_ready()
+                if self.sync_serial.in_waiting:
+                    self.intern_read_ready()
+        except asyncio.CancelledError as exc:
+            self.close(exc)
+
 
 async def create_serial_connection(
     loop, protocol_factory, *args, **kwargs
 ) -> tuple[asyncio.Transport, asyncio.BaseProtocol]:
     """Create a connection to a new serial port instance."""
     protocol = protocol_factory()
     transport = SerialTransport(loop, protocol, *args, **kwargs)
```

### Comparing `pymodbus-3.6.8/pymodbus/transport/transport.py` & `pymodbus-3.7.0.dev0/pymodbus/transport/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     reconnect_delay: float | None = None
     reconnect_delay_max: float = 0.0
     timeout_connect: float | None = None
     host: str = "localhost" # On some machines this will now be ::1
     port: int = 0
     source_address: tuple[str, int] | None = None
     handle_local_echo: bool = False
+    on_reconnect_callback: Callable[[], None] | None = None
 
     # tls
     sslctx: ssl.SSLContext | None = None
 
     # serial
     baudrate: int = -1
     bytesize: int = -1
@@ -255,15 +256,15 @@
         self.is_closing = False
         try:
             self.transport = await self.call_create()
             if isinstance(self.transport, tuple):
                 self.transport = self.transport[0]
         except OSError as exc:
             Log.warning("Failed to start server {}", exc)
-            self.__close()
+            # self.close(intern=True)
             return False
         return True
 
     # --------------------------------------- #
     # ModbusProtocol asyncio standard methods #
     # --------------------------------------- #
     def connection_made(self, transport: asyncio.BaseTransport) -> None:
@@ -280,15 +281,15 @@
         """Call from asyncio, when the connection is lost or closed.
 
         :param reason: None or an exception object
         """
         if not self.transport or self.is_closing:
             return
         Log.debug("Connection lost {} due to {}", self.comm_params.comm_name, reason)
-        self.__close()
+        self.close(intern=True)
         if (
             not self.is_server
             and not self.listener
             and self.comm_params.reconnect_delay
         ):
             self.reconnect_task = asyncio.create_task(self.do_reconnect())
             self.reconnect_task.set_name("transport reconnect")
@@ -374,33 +375,35 @@
     # ----------------------------------- #
     def send(self, data: bytes, addr: tuple | None = None) -> None:
         """Send modbus message.
 
         :param data: non-empty bytes object with data to send.
         :param addr: optional addr, only used for UDP server.
         """
-        if not self.transport:
-            Log.error("Cancel send, because not connected!")
-            return
         Log.debug("send: {}", data, ":hex")
         if self.comm_params.handle_local_echo:
             self.sent_buffer += data
         if self.comm_params.comm_type == CommType.UDP:
             if addr:
                 self.transport.sendto(data, addr=addr)  # type: ignore[attr-defined]
             else:
                 self.transport.sendto(data)  # type: ignore[attr-defined]
         else:
             self.transport.write(data)  # type: ignore[attr-defined]
 
-    def __close(self, reconnect: bool = False) -> None:
-        """Close connection (internal).
+    def close(self, intern: bool = False, reconnect: bool = False) -> None:
+        """Close connection.
 
+        :param intern: (default false), True if called internally (temporary close)
         :param reconnect: (default false), try to reconnect
         """
+        if self.is_closing:
+            return
+        if not intern:
+            self.is_closing = True
         if self.transport:
             self.transport.close()
             self.transport = None  # type: ignore[assignment]
         self.recv_buffer = b""
         if self.is_server:
             for _key, value in self.active_connections.items():
                 value.listener = None
@@ -411,24 +414,14 @@
         if not reconnect and self.reconnect_task:
             self.reconnect_task.cancel()
             self.reconnect_task = None
             self.reconnect_delay_current = 0.0
         if self.listener:
             self.listener.active_connections.pop(self.unique_id)
 
-    def close(self, reconnect: bool = False) -> None:
-        """Close connection (external).
-
-        :param reconnect: (default false), try to reconnect
-        """
-        if self.is_closing:
-            return
-        self.is_closing = True
-        self.__close(reconnect=reconnect)
-
     def reset_delay(self) -> None:
         """Reset wait time before next reconnect to minimal period."""
         self.reconnect_delay_current = self.comm_params.reconnect_delay or 0.0
 
     def is_active(self) -> bool:
         """Return true if connected/listening."""
         return bool(self.transport)
@@ -466,14 +459,16 @@
             while True:
                 Log.debug(
                     "Wait {} {} ms before reconnecting.",
                     self.comm_params.comm_name,
                     self.reconnect_delay_current * 1000,
                 )
                 await asyncio.sleep(self.reconnect_delay_current)
+                if self.comm_params.on_reconnect_callback:
+                    self.comm_params.on_reconnect_callback()
                 if await self.connect():
                     break
                 self.reconnect_delay_current = min(
                     2 * self.reconnect_delay_current,
                     self.comm_params.reconnect_delay_max,
                 )
         except asyncio.CancelledError:
```

### Comparing `pymodbus-3.6.8/pymodbus/utilities.py` & `pymodbus-3.7.0.dev0/pymodbus/utilities.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from __future__ import annotations
 
 
 __all__ = [
     "pack_bitstring",
     "unpack_bitstring",
     "default",
+    "computeCRC",
+    "checkCRC",
     "rtuFrameSize",
 ]
 
 # pylint: disable=missing-type-doc
 import struct
 
 
@@ -146,14 +148,65 @@
 
 
 # --------------------------------------------------------------------------- #
 # Error Detection Functions
 # --------------------------------------------------------------------------- #
 
 
+def __generate_crc16_table():
+    """Generate a crc16 lookup table.
+
+    .. note:: This will only be generated once
+    """
+    result = []
+    for byte in range(256):
+        crc = 0x0000
+        for _ in range(8):
+            if (byte ^ crc) & 0x0001:
+                crc = (crc >> 1) ^ 0xA001
+            else:
+                crc >>= 1
+            byte >>= 1
+        result.append(crc)
+    return result
+
+
+__crc16_table = __generate_crc16_table()
+
+
+def computeCRC(data):  # pylint: disable=invalid-name
+    """Compute a crc16 on the passed in string.
+
+    For modbus, this is only used on the binary serial protocols (in this
+    case RTU).
+
+    The difference between modbus's crc16 and a normal crc16
+    is that modbus starts the crc value out at 0xffff.
+
+    :param data: The data to create a crc16 of
+    :returns: The calculated CRC
+    """
+    crc = 0xFFFF
+    for data_byte in data:
+        idx = __crc16_table[(crc ^ int(data_byte)) & 0xFF]
+        crc = ((crc >> 8) & 0xFF) ^ idx
+    swapped = ((crc << 8) & 0xFF00) | ((crc >> 8) & 0x00FF)
+    return swapped
+
+
+def checkCRC(data, check):  # pylint: disable=invalid-name
+    """Check if the data matches the passed in CRC.
+
+    :param data: The data to create a crc16 of
+    :param check: The CRC to validate
+    :returns: True if matched, False otherwise
+    """
+    return computeCRC(data) == check
+
+
 def rtuFrameSize(data, byte_count_pos):  # pylint: disable=invalid-name
     """Calculate the size of the frame based on the byte count.
 
     :param data: The buffer containing the frame.
     :param byte_count_pos: The index of the byte count in the buffer.
     :returns: The size of the frame.
```

### Comparing `pymodbus-3.6.8/pymodbus.egg-info/PKG-INFO` & `pymodbus-3.7.0.dev0/pymodbus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodbus
-Version: 3.6.8
+Version: 3.7.0.dev0
 Summary: A fully featured modbus protocol stack in python
 Author: Galen Collins, Jan Iversen
 Maintainer: dhoomakethu, janiversen
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/pymodbus-dev/pymodbus/
 Project-URL: Source Code, https://github.com/pymodbus-dev/pymodbus
 Project-URL: Bug Reports, https://github.com/pymodbus-dev/pymodbus/issues
@@ -34,36 +34,36 @@
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 Provides-Extra: serial
 Requires-Dist: pyserial>=3.5; extra == "serial"
 Provides-Extra: repl
-Requires-Dist: pymodbus-repl>=2.0.3; extra == "repl"
+Requires-Dist: pymodbus-repl==2.0.3.dev0; extra == "repl"
 Provides-Extra: simulator
 Requires-Dist: aiohttp>=3.8.6; python_version < "3.12" and extra == "simulator"
 Requires-Dist: aiohttp>=3.9.0b0; python_version == "3.12" and extra == "simulator"
 Provides-Extra: documentation
 Requires-Dist: recommonmark>=0.7.1; extra == "documentation"
 Requires-Dist: Sphinx>=5.3.0; extra == "documentation"
 Requires-Dist: sphinx-rtd-theme>=1.1.1; extra == "documentation"
 Provides-Extra: development
-Requires-Dist: build>=1.1.1; extra == "development"
-Requires-Dist: codespell>=2.2.6; extra == "development"
-Requires-Dist: coverage>=7.4.3; extra == "development"
-Requires-Dist: mypy>=1.9.0; extra == "development"
-Requires-Dist: pylint>=3.1.0; extra == "development"
-Requires-Dist: pytest>=8.1.0; extra == "development"
-Requires-Dist: pytest-asyncio>=0.23.5.post1; extra == "development"
+Requires-Dist: build>=1.0.3; extra == "development"
+Requires-Dist: codespell>=2.2.2; extra == "development"
+Requires-Dist: coverage>=7.4.0; extra == "development"
+Requires-Dist: mypy>=1.6.0; extra == "development"
+Requires-Dist: pylint>=3.0.0; extra == "development"
+Requires-Dist: pytest>=7.3.1; extra == "development"
+Requires-Dist: pytest-asyncio>=0.20.3; extra == "development"
 Requires-Dist: pytest-cov>=4.1.0; extra == "development"
 Requires-Dist: pytest-profiling>=1.7.0; extra == "development"
-Requires-Dist: pytest-timeout>=2.3.1; extra == "development"
-Requires-Dist: pytest-xdist>=3.5.0; extra == "development"
-Requires-Dist: ruff>=0.3.3; extra == "development"
-Requires-Dist: twine>=5.0.0; extra == "development"
+Requires-Dist: pytest-timeout>=2.2.0; extra == "development"
+Requires-Dist: pytest-xdist>=3.3.1; extra == "development"
+Requires-Dist: ruff>=0.2.0; extra == "development"
+Requires-Dist: twine>=4.0.2; extra == "development"
 Requires-Dist: types-Pygments; extra == "development"
 Requires-Dist: types-pyserial; extra == "development"
 Provides-Extra: all
 Requires-Dist: pymodbus[development,documentation,repl,serial,simulator]; extra == "all"
 
 PyModbus - A Python Modbus Stack
 ================================
@@ -74,24 +74,24 @@
    :alt: Documentation Status
 .. image:: https://pepy.tech/badge/pymodbus
    :target: https://pepy.tech/project/pymodbus
    :alt: Downloads
 
 Pymodbus is a full Modbus protocol implementation offering client/server with synchronous/asynchronous API a well as simulators.
 
-Current release is `3.6.8 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.6.8>`_.
+Current release is `3.6.5 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.6.5>`_.
 
 Bleeding edge (not released) is `dev <https://github.com/pymodbus-dev/pymodbus/tree/dev>`_.
 
 All changes are described in `release notes <https://pymodbus.readthedocs.io/en/latest/source/changelog.html>`_
 and all API changes are `documented <https://pymodbus.readthedocs.io/en/latest/source/api_changes.html>`_
 
 A big thanks to all the `volunteers <https://pymodbus.readthedocs.io/en/latest/source/authors.html>`_ that helps make pymodbus a great project.
 
-Source code on `github <https://github.com/pymodbus-dev/pymodbus>`_
+Source code on `github <https://pymodbus.readthedocs.io/en/latest/source/authors.html>`_
 
 Pymodbus in a nutshell
 ----------------------
 Pymodbus consist of 5 parts:
 
 - **client**, connect to your favorite device(s)
 - **server**, simulate your favorite device(s)
```

### Comparing `pymodbus-3.6.8/pymodbus.egg-info/SOURCES.txt` & `pymodbus-3.7.0.dev0/pymodbus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/pymodbus.egg-info/requires.txt` & `pymodbus-3.7.0.dev0/pymodbus.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 
 [all]
 pymodbus[development,documentation,repl,serial,simulator]
 
 [development]
-build>=1.1.1
-codespell>=2.2.6
-coverage>=7.4.3
-mypy>=1.9.0
-pylint>=3.1.0
-pytest>=8.1.0
-pytest-asyncio>=0.23.5.post1
+build>=1.0.3
+codespell>=2.2.2
+coverage>=7.4.0
+mypy>=1.6.0
+pylint>=3.0.0
+pytest>=7.3.1
+pytest-asyncio>=0.20.3
 pytest-cov>=4.1.0
 pytest-profiling>=1.7.0
-pytest-timeout>=2.3.1
-pytest-xdist>=3.5.0
-ruff>=0.3.3
-twine>=5.0.0
+pytest-timeout>=2.2.0
+pytest-xdist>=3.3.1
+ruff>=0.2.0
+twine>=4.0.2
 types-Pygments
 types-pyserial
 
 [documentation]
 recommonmark>=0.7.1
 Sphinx>=5.3.0
 sphinx-rtd-theme>=1.1.1
 
 [repl]
-pymodbus-repl>=2.0.3
+pymodbus-repl==2.0.3.dev0
 
 [serial]
 pyserial>=3.5
 
 [simulator]
 
 [simulator:python_version < "3.12"]
```

### Comparing `pymodbus-3.6.8/pyproject.toml` & `pymodbus-3.7.0.dev0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -43,40 +43,40 @@
 "pymodbus.simulator" = "pymodbus.server.simulator.main:main"
 
 [project.optional-dependencies]
 serial = [
     "pyserial>=3.5"
 ]
 repl = [
-   "pymodbus-repl>=2.0.3"
+   "pymodbus-repl==2.0.3.dev0"
 ]
 
 simulator = [
     "aiohttp>=3.8.6;python_version<'3.12'",
     "aiohttp>=3.9.0b0;python_version=='3.12'"
 ]
 documentation = [
     "recommonmark>=0.7.1",
     "Sphinx>=5.3.0",
     "sphinx-rtd-theme>=1.1.1"
 ]
 development = [
-    "build>=1.1.1",
-    "codespell>=2.2.6",
-    "coverage>=7.4.3",
-    "mypy>=1.9.0",
-    "pylint>=3.1.0",
-    "pytest>=8.1.0",
-    "pytest-asyncio>=0.23.5.post1",
+    "build>=1.0.3",
+    "codespell>=2.2.2",
+    "coverage>=7.4.0",
+    "mypy>=1.6.0",
+    "pylint>=3.0.0",
+    "pytest>=7.3.1",
+    "pytest-asyncio>=0.20.3",
     "pytest-cov>=4.1.0",
     "pytest-profiling>=1.7.0",
-    "pytest-timeout>=2.3.1",
-    "pytest-xdist>=3.5.0",
-    "ruff>=0.3.3",
-    "twine>=5.0.0",
+    "pytest-timeout>=2.2.0",
+    "pytest-xdist>=3.3.1",
+    "ruff>=0.2.0",
+    "twine>=4.0.2",
     "types-Pygments",
     "types-pyserial"
 ]
 all = [
     "pymodbus[serial, repl, simulator, documentation, development]"
 ]
 
@@ -194,15 +194,14 @@
 warn_unused_ignores = true
 enable_error_code = "ignore-without-code, redundant-self, truthy-iterable"
 disable_error_code = ["annotation-unchecked"]
 strict_concatenate = false
 disallow_subclassing_any = true
 disallow_untyped_decorators = true
 warn_unreachable = true
-check_untyped_defs = true
 
 [tool.distutils]
 bdist_wheel = {}
 
 [tool.distutils.egg_info]
 tag-svn-revision = false
 
@@ -222,19 +221,15 @@
 
 [tool.coverage.run]
 source = [
     "examples/",
     "pymodbus/",
     "test/",
 ]
-omit = [
-    "examples/contrib/",
-    "test/message/to_do*",
-    "test/message/generator.py",
-    ]
+omit = ["examples/contrib/"]
 branch = true
 
 [tool.coverage.report]
 exclude_also = [
     "except ImportError:",
     "_check_system_health",
     "if __name__ == .__main__.:",
```

### Comparing `pymodbus-3.6.8/test/test_device.py` & `pymodbus-3.7.0.dev0/test/test_device.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/test/test_events.py` & `pymodbus-3.7.0.dev0/test/test_events.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/test/test_exceptions.py` & `pymodbus-3.7.0.dev0/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/test/test_factory.py` & `pymodbus-3.7.0.dev0/test/test_factory.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/test/test_file_message.py` & `pymodbus-3.7.0.dev0/test/test_file_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,18 +157,18 @@
 
     # -----------------------------------------------------------------------#
     #  Read File Record Response
     # -----------------------------------------------------------------------#
 
     def test_read_file_record_response_encode(self):
         """Test basic bit message encoding/decoding."""
-        records = [FileRecord(record_data=b"\x00\x01\x02\x03\x04\x05")]
+        records = [FileRecord(record_data=b"\x00\x01\x02\x03")]
         handle = ReadFileRecordResponse(records)
         result = handle.encode()
-        assert result == b"\x08\x03\x06\x00\x01\x02\x03\x04\x05"
+        assert result == b"\x06\x06\x02\x00\x01\x02\x03"
 
     def test_read_file_record_response_decode(self):
         """Test basic bit message encoding/decoding."""
         record = FileRecord(
             file_number=0x00, record_number=0x00, record_data=b"\x0d\xfe\x00\x20"
         )
         request = b"\x0c\x05\x06\x0d\xfe\x00\x20\x05\x05\x06\x33\xcd\x00\x40"
```

### Comparing `pymodbus-3.6.8/test/test_framers.py` & `pymodbus-3.7.0.dev0/test/test_framers.py`

 * *Files 2% similar despite different names*

```diff
@@ -444,29 +444,14 @@
 
         message = bytearray(b"\x00\x01\x00\x00\x00\x0b\x01\x03\x08\x00\xb5\x12\x2f\x37\x21\x00\x03")
         response_ok = False
         framer = ModbusSocketFramer(ClientDecoder())
         framer.processIncomingPacket(message, _handle_response, slave=0)
         assert response_ok, "Response is valid, but not accepted"
 
-    def test_recv_socket_exception_faulty(self):
-        """Test receive packet."""
-        response_ok = False
-
-        def _handle_response(_reply):
-            """Handle response."""
-            nonlocal response_ok
-            response_ok = True
-
-        message = bytearray(b"\x00\x02\x00\x00\x00\x02\x01\x84\x02")
-        response_ok = False
-        framer = ModbusSocketFramer(ClientDecoder())
-        framer.processIncomingPacket(message, _handle_response, slave=0)
-        assert response_ok, "Response is valid, but not accepted"
-
     # ---- 100% coverage
     @pytest.mark.parametrize(
         ("framer", "message"),
         [
             (ModbusAsciiFramer, b':00010001000AF4\r\n',),
             (ModbusBinaryFramer, b'{\x00\x01\x00\x01\x00\n\xec\x1c}',),
             (ModbusRtuFramer, b"\x00\x01\x00\x01\x00\n\xec\x1c",),
```

### Comparing `pymodbus-3.6.8/test/test_logging.py` & `pymodbus-3.7.0.dev0/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/test/test_network.py` & `pymodbus-3.7.0.dev0/test/test_network.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,18 +76,18 @@
         assert await stub.start_run()
         assert await client.connect()
         test_data = b"Data got echoed."
         client.transport.write(test_data)
         client.close()
         stub.close()
 
-    async def test_parallel_requests(self, use_port, use_cls):
+    async def test_double_packet(self, use_port, use_cls):
         """Test double packet on network."""
         old_data = b''
-        client = AsyncModbusTcpClient(NULLMODEM_HOST, port=use_port, retries=0, timeout=30)
+        client = AsyncModbusTcpClient(NULLMODEM_HOST, port=use_port, retries=0)
 
         def local_handle_data(data: bytes) -> bytes | None:
             """Handle server side for this test case."""
             nonlocal old_data
 
             addr = int(data[9])
             response = data[0:5] + b'\x05\x00\x03\x02\x00' + (addr*10).to_bytes(1, 'big')
@@ -124,13 +124,10 @@
             assert reply.registers[0] == addr * 10, f"addr {addr} value"
 
         stub = ModbusProtocolStub(use_cls, True, handler=local_handle_data)
         stub.stub_handle_data = local_handle_data
         await stub.start_run()
 
         assert await client.connect()
-        try:
-            await asyncio.gather(*[local_call(1) for x in range(1, 10)])
-        except Exception as exc:  # pylint: disable=broad-exception-caught
-            pytest.fail(exc)
+        await asyncio.gather(*[local_call(x) for x in range(1, 10)])
         client.close()
         stub.close()
```

### Comparing `pymodbus-3.6.8/test/test_payload.py` & `pymodbus-3.7.0.dev0/test/test_payload.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/test/test_pdu.py` & `pymodbus-3.7.0.dev0/test/test_pdu.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/test/test_remote_datastore.py` & `pymodbus-3.7.0.dev0/test/test_remote_datastore.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/test/test_sparse_datastore.py` & `pymodbus-3.7.0.dev0/test/test_sparse_datastore.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.6.8/test/test_transaction.py` & `pymodbus-3.7.0.dev0/test/test_transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,18 +360,18 @@
 
     def test_tcp_framer_packet(self):
         """Test a tcp frame packet build."""
         old_encode = ModbusRequest.encode
         ModbusRequest.encode = lambda self: b""
         message = ModbusRequest()
         message.transaction_id = 0x0001
-        message.protocol_id = 0x0000
+        message.protocol_id = 0x1234
         message.slave_id = 0xFF
         message.function_code = 0x01
-        expected = b"\x00\x01\x00\x00\x00\x02\xff\x01"
+        expected = b"\x00\x01\x12\x34\x00\x02\xff\x01"
         actual = self._tcp.buildPacket(message)
         assert expected == actual
         ModbusRequest.encode = old_encode
 
     # ----------------------------------------------------------------------- #
     # TLS tests
     # ----------------------------------------------------------------------- #
```

### Comparing `pymodbus-3.6.8/test/test_utilities.py` & `pymodbus-3.7.0.dev0/test/test_utilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Test utilities."""
 import struct
 
 from pymodbus.utilities import (
+    checkCRC,
     default,
     dict_property,
     pack_bitstring,
     unpack_bitstring,
 )
 
 
@@ -86,7 +87,12 @@
         assert not default({1: 1})
         assert not default(True)
 
     def test_bit_packing(self):
         """Test all string <=> bit packing functions."""
         assert unpack_bitstring(b"\x55") == self.bits
         assert pack_bitstring(self.bits) == b"\x55"
+
+    def test_cyclic_redundancy_check(self):
+        """Test the cyclic redundancy check code."""
+        assert checkCRC(self.data, 0xE2DB)
+        assert checkCRC(self.string, 0x889E)
```


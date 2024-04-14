# Comparing `tmp/naludaq-0.26.0.tar.gz` & `tmp/naludaq-0.26.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naludaq-0.26.0.tar", last modified: Sat Apr  6 00:07:02 2024, max compression
+gzip compressed data, was "naludaq-0.26.1.tar", last modified: Sun Apr 14 21:21:30 2024, max compression
```

## Comparing `naludaq-0.26.0.tar` & `naludaq-0.26.1.tar`

### file list

```diff
@@ -1,266 +1,266 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.129927 naludaq-0.26.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-06 00:06:51.000000 naludaq-0.26.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16253 2024-04-06 00:07:02.125927 naludaq-0.26.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14876 2024-04-06 00:06:51.000000 naludaq-0.26.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-06 00:06:51.000000 naludaq-0.26.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 00:07:02.129927 naludaq-0.26.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-06 00:06:51.000000 naludaq-0.26.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.077927 naludaq-0.26.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.081927 naludaq-0.26.0/src/naludaq/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.085927 naludaq-0.26.0/src/naludaq/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/backend/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/backend/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/backend/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.085927 naludaq-0.26.0/src/naludaq/backend/managers/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/backend/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/backend/managers/acquisitions.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/backend/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/backend/managers/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/backend/managers/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/backend/managers/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.085927 naludaq-0.26.0/src/naludaq/backend/models/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/backend/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39254 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/backend/models/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/backend/models/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.085927 naludaq-0.26.0/src/naludaq/board/
--rw-r--r--   0 runner    (1001) docker     (127)    30544 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24036 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/board_inits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.089927 naludaq-0.26.0/src/naludaq/board/connections/
--rw-r--r--   0 runner    (1001) docker     (127)    19599 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/connections/_FTDI.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/connections/_MockUART.py
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/connections/_UART.py
--rw-r--r--   0 runner    (1001) docker     (127)    11460 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/connections/_USB.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/connections/base_ethernet.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/connections/base_serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/connections/connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/connections/tcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/connections/udp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.089927 naludaq-0.26.0/src/naludaq/board/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/initializers/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/initializers/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/initializers/asocv3s.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/initializers/init_aodsv2_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/initializers/init_hdsocv1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/initializers/init_udc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/initializers/init_upac96.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/initializers/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (127)    17749 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/board/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.093927 naludaq-0.26.0/src/naludaq/communication/
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10200 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/communication/_chip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/communication/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/communication/_fpga.py
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/communication/analog_registers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/communication/chip_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/communication/control_registers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/communication/digital_registers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/communication/i2c.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/communication/i2c_registers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20429 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/communication/registers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.093927 naludaq-0.26.0/src/naludaq/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/analog_debug_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.093927 naludaq-0.26.0/src/naludaq/controllers/biasing_mode/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/biasing_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/biasing_mode/udc16.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.097927 naludaq-0.26.0/src/naludaq/controllers/board/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/board/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/board/asocv3s.py
--rw-r--r--   0 runner    (1001) docker     (127)    15507 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/board/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/board/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/board/oleas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/board/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/board/udc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/board/upac.py
--rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/board/upac96.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.097927 naludaq-0.26.0/src/naludaq/controllers/connection/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21101 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/connection/connection_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/connection/upac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/connection/upac96.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.101927 naludaq-0.26.0/src/naludaq/controllers/external_dac/
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/external_dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/external_dac/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/external_dac/ad5671.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/external_dac/ad5675.py
--rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/external_dac/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/external_dac/dac7578.py
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/external_dac/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/external_dac/i2c_dac.py
--rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/external_dac/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/external_dac/upac32.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.101927 naludaq-0.26.0/src/naludaq/controllers/gainstages/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/gainstages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/gainstages/aodsv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/gainstages/oddsock_aods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.101927 naludaq-0.26.0/src/naludaq/controllers/peripherals/
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/peripherals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/peripherals/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/peripherals/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/peripherals/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/peripherals/peripherals_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/peripherals/upac.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/peripherals/upac96.py
--rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/project_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.101927 naludaq-0.26.0/src/naludaq/controllers/readout/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/readout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/readout/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/readout/asocv3.py
--rw-r--r--   0 runner    (1001) docker     (127)    14359 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/readout/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/readout/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/readout/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/si5341_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.105927 naludaq-0.26.0/src/naludaq/controllers/tia/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/tia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/tia/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/tia/hdsoc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.105927 naludaq-0.26.0/src/naludaq/controllers/trigger/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/trigger/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/trigger/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/trigger/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/trigger/siread.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/trigger/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/trigger/upac.py
--rw-r--r--   0 runner    (1001) docker     (127)    16581 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/controllers/trigger/upac96.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.105927 naludaq-0.26.0/src/naludaq/daq/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/daq/debugdaq.py
--rw-r--r--   0 runner    (1001) docker     (127)    20482 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/daq/lightdaq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/daq/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.105927 naludaq-0.26.0/src/naludaq/daq/workers/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/daq/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/daq/workers/answer_parser_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/daq/workers/csv_storage_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.109927 naludaq-0.26.0/src/naludaq/daq/workers/packager/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/daq/workers/packager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/daq/workers/packager/worker_packager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/daq/workers/packager/worker_packager_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/daq/workers/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/daq/workers/worker_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/daq/workers/worker_serial_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/daq/workers/worker_usb_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.109927 naludaq-0.26.0/src/naludaq/devices/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/devices/eeprom.py
--rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/devices/i2c_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/devices/ltc2990.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.109927 naludaq-0.26.0/src/naludaq/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/helpers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/helpers/fancyiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/helpers/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/helpers/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/helpers/register_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/helpers/semiton.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/helpers/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.113927 naludaq-0.26.0/src/naludaq/io/
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22338 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/io/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    35939 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/io/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/io/io_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.113927 naludaq-0.26.0/src/naludaq/models/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/models/acq_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/models/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (127)    16621 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/naludaq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.113927 naludaq-0.26.0/src/naludaq/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/parsers/aardvarcv3_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/parsers/answer_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/parsers/aodsoc_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/parsers/asocv3_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9243 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/parsers/asocv3s_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/parsers/hdsoc_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.117927 naludaq-0.26.0/src/naludaq/parsers/headers/
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/parsers/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/parsers/headers/asoc.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/parsers/headers/asocv2.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/parsers/headers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/parsers/headers/siread.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/parsers/headers/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/parsers/headers/upac32.py
--rw-r--r--   0 runner    (1001) docker     (127)    11956 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/parsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/parsers/trbhm_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/parsers/udc_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/parsers/upac96_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/parsers/upac_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.117927 naludaq-0.26.0/src/naludaq/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.117927 naludaq-0.26.0/src/naludaq/tools/adc2mv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/adc2mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/adc2mv/adc_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14397 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/adc2mv/adc_linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/adc2mv/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/adc2mv/pre_adc2mv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/autoaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.117927 naludaq-0.26.0/src/naludaq/tools/autotrigger/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/autotrigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/autotrigger/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/board_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.117927 naludaq-0.26.0/src/naludaq/tools/dac_sweep/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/dac_sweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/dac_sweep/dac_sweep_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.121927 naludaq-0.26.0/src/naludaq/tools/data_collector/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/data_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/data_collector/_daq_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    16831 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/data_collector/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/data_collector/udc16.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/ft60x.py
--rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/ftdi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.121927 naludaq-0.26.0/src/naludaq/tools/lookup_table/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/lookup_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/lookup_table/lookup_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/lookup_table/lookup_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.121927 naludaq-0.26.0/src/naludaq/tools/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/optimizers/bayesian_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.121927 naludaq-0.26.0/src/naludaq/tools/optimizers/conversion_ramp/
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/optimizers/conversion_ramp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/optimizers/conversion_ramp/channel_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    22275 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/optimizers/conversion_ramp/udc16.py
--rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/optimizers/gainstagetuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.121927 naludaq-0.26.0/src/naludaq/tools/pedestals/
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/pedestals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.125927 naludaq-0.26.0/src/naludaq/tools/pedestals/generators/
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/pedestals/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/pedestals/generators/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/pedestals/generators/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/pedestals/generators/udc16.py
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/pedestals/generators/upac96.py
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/pedestals/pedestals_correcter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/pedestals/pedestals_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/pedestals/upac32_pedestals_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.125927 naludaq-0.26.0/src/naludaq/tools/threshold_scan/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/threshold_scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/threshold_scan/threshold_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/threshold_scan/upac96_thresholdscan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.125927 naludaq-0.26.0/src/naludaq/tools/timing_cal/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/timing_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/timing_cal/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/timing_cal/correcter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.125927 naludaq-0.26.0/src/naludaq/tools/waiter/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/waiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-06 00:06:51.000000 naludaq-0.26.0/src/naludaq/tools/waiter/eventwaiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.125927 naludaq-0.26.0/src/naludaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16253 2024-04-06 00:07:02.000000 naludaq-0.26.0/src/naludaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-04-06 00:07:02.000000 naludaq-0.26.0/src/naludaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 00:07:02.000000 naludaq-0.26.0/src/naludaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-06 00:07:02.000000 naludaq-0.26.0/src/naludaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 00:07:02.000000 naludaq-0.26.0/src/naludaq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:07:02.125927 naludaq-0.26.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-06 00:06:52.000000 naludaq-0.26.0/tests/test_naludaq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.569848 naludaq-0.26.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-14 21:21:18.000000 naludaq-0.26.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16253 2024-04-14 21:21:30.565848 naludaq-0.26.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14876 2024-04-14 21:21:18.000000 naludaq-0.26.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-14 21:21:18.000000 naludaq-0.26.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 21:21:30.569848 naludaq-0.26.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-14 21:21:18.000000 naludaq-0.26.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.517848 naludaq-0.26.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.521848 naludaq-0.26.1/src/naludaq/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.525848 naludaq-0.26.1/src/naludaq/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/backend/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/backend/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/backend/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.525848 naludaq-0.26.1/src/naludaq/backend/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/backend/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/backend/managers/acquisitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/backend/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/backend/managers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/backend/managers/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/backend/managers/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.525848 naludaq-0.26.1/src/naludaq/backend/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/backend/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39569 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/backend/models/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/backend/models/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.525848 naludaq-0.26.1/src/naludaq/board/
+-rw-r--r--   0 runner    (1001) docker     (127)    30544 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24036 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/board_inits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.529848 naludaq-0.26.1/src/naludaq/board/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)    19599 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/connections/_FTDI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/connections/_MockUART.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/connections/_UART.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11460 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/connections/_USB.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/connections/base_ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/connections/base_serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/connections/connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/connections/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/connections/udp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.529848 naludaq-0.26.1/src/naludaq/board/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/initializers/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/initializers/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/initializers/asocv3s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/initializers/init_aodsv2_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/initializers/init_hdsocv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/initializers/init_udc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/initializers/init_upac96.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/initializers/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17749 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/board/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.533848 naludaq-0.26.1/src/naludaq/communication/
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10200 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/communication/_chip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/communication/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/communication/_fpga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/communication/analog_registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/communication/chip_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/communication/control_registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/communication/digital_registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/communication/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/communication/i2c_registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20429 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/communication/registers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.533848 naludaq-0.26.1/src/naludaq/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/analog_debug_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.533848 naludaq-0.26.1/src/naludaq/controllers/biasing_mode/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/biasing_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/biasing_mode/udc16.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.537848 naludaq-0.26.1/src/naludaq/controllers/board/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/board/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/board/asocv3s.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15507 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/board/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/board/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/board/oleas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/board/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/board/udc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/board/upac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/board/upac96.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.537848 naludaq-0.26.1/src/naludaq/controllers/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21101 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/connection/connection_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/connection/upac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/connection/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.537848 naludaq-0.26.1/src/naludaq/controllers/external_dac/
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/external_dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/external_dac/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/external_dac/ad5671.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/external_dac/ad5675.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/external_dac/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/external_dac/dac7578.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/external_dac/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/external_dac/i2c_dac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/external_dac/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/external_dac/upac32.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.541848 naludaq-0.26.1/src/naludaq/controllers/gainstages/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/gainstages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/gainstages/aodsv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/gainstages/oddsock_aods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.541848 naludaq-0.26.1/src/naludaq/controllers/peripherals/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/peripherals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/peripherals/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/peripherals/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/peripherals/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/peripherals/peripherals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/peripherals/upac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/peripherals/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/project_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.541848 naludaq-0.26.1/src/naludaq/controllers/readout/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/readout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/readout/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/readout/asocv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14359 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/readout/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/readout/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/readout/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/si5341_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.541848 naludaq-0.26.1/src/naludaq/controllers/tia/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/tia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/tia/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/tia/hdsoc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.545848 naludaq-0.26.1/src/naludaq/controllers/trigger/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/trigger/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/trigger/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/trigger/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/trigger/siread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/trigger/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/trigger/upac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16581 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/controllers/trigger/upac96.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.545848 naludaq-0.26.1/src/naludaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/daq/debugdaq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20482 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/daq/lightdaq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/daq/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.545848 naludaq-0.26.1/src/naludaq/daq/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/daq/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/daq/workers/answer_parser_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/daq/workers/csv_storage_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.549848 naludaq-0.26.1/src/naludaq/daq/workers/packager/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/daq/workers/packager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/daq/workers/packager/worker_packager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/daq/workers/packager/worker_packager_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/daq/workers/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/daq/workers/worker_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/daq/workers/worker_serial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/daq/workers/worker_usb_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.549848 naludaq-0.26.1/src/naludaq/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/devices/eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/devices/i2c_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/devices/ltc2990.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.549848 naludaq-0.26.1/src/naludaq/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/helpers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/helpers/fancyiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/helpers/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/helpers/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/helpers/register_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/helpers/semiton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/helpers/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.553848 naludaq-0.26.1/src/naludaq/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22338 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/io/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35939 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/io/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/io/io_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.553848 naludaq-0.26.1/src/naludaq/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/models/acq_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/models/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16621 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/naludaq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.553848 naludaq-0.26.1/src/naludaq/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/parsers/aardvarcv3_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/parsers/answer_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/parsers/aodsoc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/parsers/asocv3_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9243 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/parsers/asocv3s_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/parsers/hdsoc_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.557848 naludaq-0.26.1/src/naludaq/parsers/headers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/parsers/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/parsers/headers/asoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/parsers/headers/asocv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/parsers/headers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/parsers/headers/siread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/parsers/headers/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/parsers/headers/upac32.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11956 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/parsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/parsers/trbhm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/parsers/udc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/parsers/upac96_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/parsers/upac_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.557848 naludaq-0.26.1/src/naludaq/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.557848 naludaq-0.26.1/src/naludaq/tools/adc2mv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/adc2mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/adc2mv/adc_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14397 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/adc2mv/adc_linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/adc2mv/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/adc2mv/pre_adc2mv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/autoaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.557848 naludaq-0.26.1/src/naludaq/tools/autotrigger/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/autotrigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/autotrigger/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/board_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.557848 naludaq-0.26.1/src/naludaq/tools/dac_sweep/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/dac_sweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/dac_sweep/dac_sweep_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.561848 naludaq-0.26.1/src/naludaq/tools/data_collector/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/data_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/data_collector/_daq_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16831 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/data_collector/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/data_collector/udc16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/ft60x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/ftdi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.561848 naludaq-0.26.1/src/naludaq/tools/lookup_table/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/lookup_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/lookup_table/lookup_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/lookup_table/lookup_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.561848 naludaq-0.26.1/src/naludaq/tools/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/optimizers/bayesian_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.561848 naludaq-0.26.1/src/naludaq/tools/optimizers/conversion_ramp/
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/optimizers/conversion_ramp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/optimizers/conversion_ramp/channel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22275 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/optimizers/conversion_ramp/udc16.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/optimizers/gainstagetuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.561848 naludaq-0.26.1/src/naludaq/tools/pedestals/
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/pedestals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.565848 naludaq-0.26.1/src/naludaq/tools/pedestals/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/pedestals/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/pedestals/generators/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/pedestals/generators/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/pedestals/generators/udc16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/pedestals/generators/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/pedestals/pedestals_correcter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/pedestals/pedestals_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/pedestals/upac32_pedestals_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.565848 naludaq-0.26.1/src/naludaq/tools/threshold_scan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/threshold_scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/threshold_scan/threshold_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/threshold_scan/upac96_thresholdscan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.565848 naludaq-0.26.1/src/naludaq/tools/timing_cal/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/timing_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/timing_cal/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/timing_cal/correcter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.565848 naludaq-0.26.1/src/naludaq/tools/waiter/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/waiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-14 21:21:18.000000 naludaq-0.26.1/src/naludaq/tools/waiter/eventwaiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.565848 naludaq-0.26.1/src/naludaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16253 2024-04-14 21:21:30.000000 naludaq-0.26.1/src/naludaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-04-14 21:21:30.000000 naludaq-0.26.1/src/naludaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:21:30.000000 naludaq-0.26.1/src/naludaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-14 21:21:30.000000 naludaq-0.26.1/src/naludaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 21:21:30.000000 naludaq-0.26.1/src/naludaq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:21:30.565848 naludaq-0.26.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-14 21:21:19.000000 naludaq-0.26.1/tests/test_naludaq.py
```

### Comparing `naludaq-0.26.0/LICENSE.txt` & `naludaq-0.26.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/PKG-INFO` & `naludaq-0.26.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naludaq
-Version: 0.26.0
+Version: 0.26.1
 Summary: Backend package for Nalu Scientific hardware
 Home-page: 
 Author: Thomas Yang, Emily Lum, Terry Pham
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naludaq-0.26.0/README.md` & `naludaq-0.26.1/README.md`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/pyproject.toml` & `naludaq-0.26.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/setup.py` & `naludaq-0.26.1/setup.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/backend/__init__.py` & `naludaq-0.26.1/src/naludaq/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/backend/client.py` & `naludaq-0.26.1/src/naludaq/backend/client.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/backend/context.py` & `naludaq-0.26.1/src/naludaq/backend/context.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/backend/exceptions.py` & `naludaq-0.26.1/src/naludaq/backend/exceptions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/backend/managers/acquisitions.py` & `naludaq-0.26.1/src/naludaq/backend/managers/acquisitions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/backend/managers/config.py` & `naludaq-0.26.1/src/naludaq/backend/managers/config.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/backend/managers/connection.py` & `naludaq-0.26.1/src/naludaq/backend/managers/connection.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/backend/managers/io.py` & `naludaq-0.26.1/src/naludaq/backend/managers/io.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/backend/models/acquisition.py` & `naludaq-0.26.1/src/naludaq/backend/models/acquisition.py`

 * *Files 1% similar despite different names*

```diff
@@ -823,15 +823,15 @@
 
     def _raise_if_closed(self):
         if not self._open:
             raise IOError("Chunk is closed")
 
 
 class DiskAcquisition:
-    def __init__(self, path: Path):
+    def __init__(self, path: Path, parse: bool = True):
         """Utility for accessing acquisition directly from disk.
 
         The acquisition will be opened on instantiation. It is recommended to use
         this object as a context manager to ensure the acquisition is closed when
         it is no longer needed.
 
         Important: the acquisition should not be mutated while this object is alive.
@@ -844,18 +844,28 @@
             InvalidAcquisitionError: if the path is not a valid acquisition.
         """
         if not isinstance(path, (Path, str)):
             raise TypeError("Path must be a string or Path object")
         path = Path(path).resolve()
         if not DiskAcquisition._is_acquisition(path):
             raise AcquisitionError("Not a valid acquisition")
+        self.parse = parse
         self._root = path
         self._open = False
         self.open()
 
+    @property
+    def parse(self) -> bool:
+        """Whether to parse events when getting them"""
+        return self._parse
+
+    @parse.setter
+    def parse(self, value: bool):
+        self._parse = value
+
     def __len__(self) -> int:
         """Get the number of events in the acquisition"""
         return self._event_count
 
     def __del__(self):
         """Close the acquisition"""
         self.close()
@@ -877,21 +887,25 @@
 
         Raises:
             IndexError: if the index is out of bounds
             IOError: if the acquisition is closed
         """
         self._raise_if_closed()
         result = None
+        if self._parse:
+            fn = self.parsed_event
+        else:
+            fn = self.raw_event
         if isinstance(index, int):
             index = _resolve_index_or_raise(index, len(self))
-            result = self.parsed_event(index)
+            result = fn(index)
         elif isinstance(index, slice):
-            result = [self.parsed_event(i) for i in range(*index.indices(len(self)))]
+            result = [fn(i) for i in range(*index.indices(len(self)))]
         elif isinstance(index, list):
-            result = [self.parsed_event(i) for i in index]
+            result = [fn(i) for i in index]
         else:
             raise TypeError("Index must be an int or slice")
         return result
 
     def open(self):
         """Open the acquisition for reading.
```

### Comparing `naludaq-0.26.0/src/naludaq/backend/models/device.py` & `naludaq-0.26.1/src/naludaq/backend/models/device.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/board/__init__.py` & `naludaq-0.26.1/src/naludaq/board/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/board/board_inits.py` & `naludaq-0.26.1/src/naludaq/board/board_inits.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/board/connections/_FTDI.py` & `naludaq-0.26.1/src/naludaq/board/connections/_FTDI.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/board/connections/_MockUART.py` & `naludaq-0.26.1/src/naludaq/board/connections/_MockUART.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/board/connections/_UART.py` & `naludaq-0.26.1/src/naludaq/board/connections/_UART.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/board/connections/_USB.py` & `naludaq-0.26.1/src/naludaq/board/connections/_USB.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/board/connections/base_connection.py` & `naludaq-0.26.1/src/naludaq/board/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/board/connections/connection_factory.py` & `naludaq-0.26.1/src/naludaq/board/connections/connection_factory.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/board/connections/tcp.py` & `naludaq-0.26.1/src/naludaq/board/connections/tcp.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/board/connections/udp.py` & `naludaq-0.26.1/src/naludaq/board/connections/udp.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/board/initializers/__init__.py` & `naludaq-0.26.1/src/naludaq/board/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/board/initializers/aardvarcv3.py` & `naludaq-0.26.1/src/naludaq/board/initializers/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/board/initializers/aodsoc.py` & `naludaq-0.26.1/src/naludaq/board/initializers/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/board/initializers/asocv3s.py` & `naludaq-0.26.1/src/naludaq/board/initializers/asocv3s.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/board/initializers/init_aodsv2_eval.py` & `naludaq-0.26.1/src/naludaq/board/initializers/init_aodsv2_eval.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/board/initializers/init_hdsocv1.py` & `naludaq-0.26.1/src/naludaq/board/initializers/init_hdsocv1.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/board/initializers/init_udc.py` & `naludaq-0.26.1/src/naludaq/board/initializers/init_udc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/board/initializers/init_upac96.py` & `naludaq-0.26.1/src/naludaq/board/initializers/init_upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/board/initializers/trbhm.py` & `naludaq-0.26.1/src/naludaq/board/initializers/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/board/params.py` & `naludaq-0.26.1/src/naludaq/board/params.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/communication/__init__.py` & `naludaq-0.26.1/src/naludaq/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/communication/_chip.py` & `naludaq-0.26.1/src/naludaq/communication/_chip.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/communication/_common.py` & `naludaq-0.26.1/src/naludaq/communication/_common.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/communication/_fpga.py` & `naludaq-0.26.1/src/naludaq/communication/_fpga.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/communication/analog_registers.py` & `naludaq-0.26.1/src/naludaq/communication/analog_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/communication/chip_selection.py` & `naludaq-0.26.1/src/naludaq/communication/chip_selection.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/communication/control_registers.py` & `naludaq-0.26.1/src/naludaq/communication/control_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/communication/digital_registers.py` & `naludaq-0.26.1/src/naludaq/communication/digital_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/communication/i2c.py` & `naludaq-0.26.1/src/naludaq/communication/i2c.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/communication/i2c_registers.py` & `naludaq-0.26.1/src/naludaq/communication/i2c_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/communication/registers.py` & `naludaq-0.26.1/src/naludaq/communication/registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/__init__.py` & `naludaq-0.26.1/src/naludaq/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/analog_debug_controller.py` & `naludaq-0.26.1/src/naludaq/controllers/analog_debug_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/biasing_mode/__init__.py` & `naludaq-0.26.1/src/naludaq/controllers/biasing_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/biasing_mode/udc16.py` & `naludaq-0.26.1/src/naludaq/controllers/biasing_mode/udc16.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/board/__init__.py` & `naludaq-0.26.1/src/naludaq/controllers/board/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/board/aodsoc.py` & `naludaq-0.26.1/src/naludaq/controllers/board/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/board/asocv3s.py` & `naludaq-0.26.1/src/naludaq/controllers/board/asocv3s.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/board/default.py` & `naludaq-0.26.1/src/naludaq/controllers/board/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/board/hdsoc.py` & `naludaq-0.26.1/src/naludaq/controllers/board/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/board/oleas.py` & `naludaq-0.26.1/src/naludaq/controllers/board/oleas.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/board/trbhm.py` & `naludaq-0.26.1/src/naludaq/controllers/board/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/board/udc.py` & `naludaq-0.26.1/src/naludaq/controllers/board/udc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/board/upac.py` & `naludaq-0.26.1/src/naludaq/controllers/board/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/board/upac96.py` & `naludaq-0.26.1/src/naludaq/controllers/board/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/connection/__init__.py` & `naludaq-0.26.1/src/naludaq/controllers/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/connection/connection_controller.py` & `naludaq-0.26.1/src/naludaq/controllers/connection/connection_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/connection/upac.py` & `naludaq-0.26.1/src/naludaq/controllers/connection/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/connection/upac96.py` & `naludaq-0.26.1/src/naludaq/controllers/connection/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/external_dac/__init__.py` & `naludaq-0.26.1/src/naludaq/controllers/external_dac/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/external_dac/aardvarcv3.py` & `naludaq-0.26.1/src/naludaq/controllers/external_dac/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/external_dac/ad5671.py` & `naludaq-0.26.1/src/naludaq/controllers/external_dac/ad5671.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/external_dac/ad5675.py` & `naludaq-0.26.1/src/naludaq/controllers/external_dac/ad5675.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/external_dac/base.py` & `naludaq-0.26.1/src/naludaq/controllers/external_dac/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/external_dac/dac7578.py` & `naludaq-0.26.1/src/naludaq/controllers/external_dac/dac7578.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/external_dac/hdsoc.py` & `naludaq-0.26.1/src/naludaq/controllers/external_dac/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/external_dac/i2c_dac.py` & `naludaq-0.26.1/src/naludaq/controllers/external_dac/i2c_dac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/external_dac/trbhm.py` & `naludaq-0.26.1/src/naludaq/controllers/external_dac/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/external_dac/upac32.py` & `naludaq-0.26.1/src/naludaq/controllers/external_dac/upac32.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/gainstages/__init__.py` & `naludaq-0.26.1/src/naludaq/controllers/gainstages/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/gainstages/aodsv2.py` & `naludaq-0.26.1/src/naludaq/controllers/gainstages/aodsv2.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/gainstages/oddsock_aods.py` & `naludaq-0.26.1/src/naludaq/controllers/gainstages/oddsock_aods.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/peripherals/__init__.py` & `naludaq-0.26.1/src/naludaq/controllers/peripherals/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/peripherals/aardvarcv3.py` & `naludaq-0.26.1/src/naludaq/controllers/peripherals/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/peripherals/aodsoc.py` & `naludaq-0.26.1/src/naludaq/controllers/peripherals/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/peripherals/hdsoc.py` & `naludaq-0.26.1/src/naludaq/controllers/peripherals/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/peripherals/peripherals_controller.py` & `naludaq-0.26.1/src/naludaq/controllers/peripherals/peripherals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/peripherals/upac.py` & `naludaq-0.26.1/src/naludaq/controllers/peripherals/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/peripherals/upac96.py` & `naludaq-0.26.1/src/naludaq/controllers/peripherals/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/project_controller.py` & `naludaq-0.26.1/src/naludaq/controllers/project_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/readout/__init__.py` & `naludaq-0.26.1/src/naludaq/controllers/readout/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/readout/aardvarcv3.py` & `naludaq-0.26.1/src/naludaq/controllers/readout/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/readout/asocv3.py` & `naludaq-0.26.1/src/naludaq/controllers/readout/asocv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/readout/default.py` & `naludaq-0.26.1/src/naludaq/controllers/readout/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/readout/hdsoc.py` & `naludaq-0.26.1/src/naludaq/controllers/readout/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/readout/trbhm.py` & `naludaq-0.26.1/src/naludaq/controllers/readout/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/si5341_controller.py` & `naludaq-0.26.1/src/naludaq/controllers/si5341_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/tia/__init__.py` & `naludaq-0.26.1/src/naludaq/controllers/tia/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/tia/base.py` & `naludaq-0.26.1/src/naludaq/controllers/tia/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/tia/hdsoc.py` & `naludaq-0.26.1/src/naludaq/controllers/tia/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/trigger/__init__.py` & `naludaq-0.26.1/src/naludaq/controllers/trigger/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/trigger/aodsoc.py` & `naludaq-0.26.1/src/naludaq/controllers/trigger/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/trigger/default.py` & `naludaq-0.26.1/src/naludaq/controllers/trigger/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/trigger/hdsoc.py` & `naludaq-0.26.1/src/naludaq/controllers/trigger/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/trigger/trbhm.py` & `naludaq-0.26.1/src/naludaq/controllers/trigger/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/trigger/upac.py` & `naludaq-0.26.1/src/naludaq/controllers/trigger/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/controllers/trigger/upac96.py` & `naludaq-0.26.1/src/naludaq/controllers/trigger/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/daq/__init__.py` & `naludaq-0.26.1/src/naludaq/daq/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/daq/debugdaq.py` & `naludaq-0.26.1/src/naludaq/daq/debugdaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/daq/lightdaq.py` & `naludaq-0.26.1/src/naludaq/daq/lightdaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/daq/preprocess.py` & `naludaq-0.26.1/src/naludaq/daq/preprocess.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/daq/workers/__init__.py` & `naludaq-0.26.1/src/naludaq/daq/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/daq/workers/answer_parser_worker.py` & `naludaq-0.26.1/src/naludaq/daq/workers/answer_parser_worker.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/daq/workers/csv_storage_worker.py` & `naludaq-0.26.1/src/naludaq/daq/workers/csv_storage_worker.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/daq/workers/packager/__init__.py` & `naludaq-0.26.1/src/naludaq/daq/workers/packager/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/daq/workers/packager/worker_packager.py` & `naludaq-0.26.1/src/naludaq/daq/workers/packager/worker_packager.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/daq/workers/packager/worker_packager_debug.py` & `naludaq-0.26.1/src/naludaq/daq/workers/packager/worker_packager_debug.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py` & `naludaq-0.26.1/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/daq/workers/postprocessing.py` & `naludaq-0.26.1/src/naludaq/daq/workers/postprocessing.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/daq/workers/worker_parser.py` & `naludaq-0.26.1/src/naludaq/daq/workers/worker_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/daq/workers/worker_serial_reader.py` & `naludaq-0.26.1/src/naludaq/daq/workers/worker_serial_reader.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/daq/workers/worker_usb_reader.py` & `naludaq-0.26.1/src/naludaq/daq/workers/worker_usb_reader.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/devices/eeprom.py` & `naludaq-0.26.1/src/naludaq/devices/eeprom.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/devices/i2c_device.py` & `naludaq-0.26.1/src/naludaq/devices/i2c_device.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/devices/ltc2990.py` & `naludaq-0.26.1/src/naludaq/devices/ltc2990.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/helpers/decorators.py` & `naludaq-0.26.1/src/naludaq/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/helpers/exceptions.py` & `naludaq-0.26.1/src/naludaq/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/helpers/fancyiter.py` & `naludaq-0.26.1/src/naludaq/helpers/fancyiter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/helpers/helper_functions.py` & `naludaq-0.26.1/src/naludaq/helpers/helper_functions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/helpers/operations.py` & `naludaq-0.26.1/src/naludaq/helpers/operations.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/helpers/register_cache.py` & `naludaq-0.26.1/src/naludaq/helpers/register_cache.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/helpers/semiton.py` & `naludaq-0.26.1/src/naludaq/helpers/semiton.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/helpers/validations.py` & `naludaq-0.26.1/src/naludaq/helpers/validations.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/io/__init__.py` & `naludaq-0.26.1/src/naludaq/io/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/io/csv_writer.py` & `naludaq-0.26.1/src/naludaq/io/csv_writer.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/io/hdf5.py` & `naludaq-0.26.1/src/naludaq/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/io/io_manager.py` & `naludaq-0.26.1/src/naludaq/io/io_manager.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/models/acq_converters.py` & `naludaq-0.26.1/src/naludaq/models/acq_converters.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/models/acquisition.py` & `naludaq-0.26.1/src/naludaq/models/acquisition.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/naludaq.py` & `naludaq-0.26.1/src/naludaq/naludaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/parsers/__init__.py` & `naludaq-0.26.1/src/naludaq/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/parsers/aardvarcv3_parser.py` & `naludaq-0.26.1/src/naludaq/parsers/aardvarcv3_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/parsers/answer_parser.py` & `naludaq-0.26.1/src/naludaq/parsers/answer_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/parsers/aodsoc_parser.py` & `naludaq-0.26.1/src/naludaq/parsers/aodsoc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/parsers/asocv3_parser.py` & `naludaq-0.26.1/src/naludaq/parsers/asocv3_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/parsers/asocv3s_parser.py` & `naludaq-0.26.1/src/naludaq/parsers/asocv3s_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/parsers/hdsoc_parser.py` & `naludaq-0.26.1/src/naludaq/parsers/hdsoc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/parsers/headers/__init__.py` & `naludaq-0.26.1/src/naludaq/parsers/headers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/parsers/headers/asoc.py` & `naludaq-0.26.1/src/naludaq/parsers/headers/asoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/parsers/headers/asocv2.py` & `naludaq-0.26.1/src/naludaq/parsers/headers/asocv2.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/parsers/headers/base.py` & `naludaq-0.26.1/src/naludaq/parsers/headers/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/parsers/headers/siread.py` & `naludaq-0.26.1/src/naludaq/parsers/headers/siread.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/parsers/headers/trbhm.py` & `naludaq-0.26.1/src/naludaq/parsers/headers/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/parsers/headers/upac32.py` & `naludaq-0.26.1/src/naludaq/parsers/headers/upac32.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/parsers/parser.py` & `naludaq-0.26.1/src/naludaq/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/parsers/trbhm_parser.py` & `naludaq-0.26.1/src/naludaq/parsers/trbhm_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/parsers/udc_parser.py` & `naludaq-0.26.1/src/naludaq/parsers/udc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/parsers/upac96_parser.py` & `naludaq-0.26.1/src/naludaq/parsers/upac96_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/parsers/upac_parser.py` & `naludaq-0.26.1/src/naludaq/parsers/upac_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/adc2mv/adc_converter.py` & `naludaq-0.26.1/src/naludaq/tools/adc2mv/adc_converter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/adc2mv/adc_linear_regression.py` & `naludaq-0.26.1/src/naludaq/tools/adc2mv/adc_linear_regression.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/adc2mv/generate.py` & `naludaq-0.26.1/src/naludaq/tools/adc2mv/generate.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/adc2mv/pre_adc2mv.py` & `naludaq-0.26.1/src/naludaq/tools/adc2mv/pre_adc2mv.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/autoaction.py` & `naludaq-0.26.1/src/naludaq/tools/autoaction.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/autotrigger/default.py` & `naludaq-0.26.1/src/naludaq/tools/autotrigger/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/board_backup.py` & `naludaq-0.26.1/src/naludaq/tools/board_backup.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/dac_sweep/dac_sweep_controller.py` & `naludaq-0.26.1/src/naludaq/tools/dac_sweep/dac_sweep_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/data_collector/_daq_interface.py` & `naludaq-0.26.1/src/naludaq/tools/data_collector/_daq_interface.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/data_collector/default.py` & `naludaq-0.26.1/src/naludaq/tools/data_collector/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/data_collector/udc16.py` & `naludaq-0.26.1/src/naludaq/tools/data_collector/udc16.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/features.py` & `naludaq-0.26.1/src/naludaq/tools/features.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/ft60x.py` & `naludaq-0.26.1/src/naludaq/tools/ft60x.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/ftdi.py` & `naludaq-0.26.1/src/naludaq/tools/ftdi.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/lookup_table/lookup_table.py` & `naludaq-0.26.1/src/naludaq/tools/lookup_table/lookup_table.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/lookup_table/lookup_table_generator.py` & `naludaq-0.26.1/src/naludaq/tools/lookup_table/lookup_table_generator.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/metadata.py` & `naludaq-0.26.1/src/naludaq/tools/metadata.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/optimizers/bayesian_optimizer.py` & `naludaq-0.26.1/src/naludaq/tools/optimizers/bayesian_optimizer.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/optimizers/conversion_ramp/__init__.py` & `naludaq-0.26.1/src/naludaq/tools/optimizers/conversion_ramp/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/optimizers/conversion_ramp/channel_writer.py` & `naludaq-0.26.1/src/naludaq/tools/optimizers/conversion_ramp/channel_writer.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/optimizers/conversion_ramp/udc16.py` & `naludaq-0.26.1/src/naludaq/tools/optimizers/conversion_ramp/udc16.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/optimizers/gainstagetuner.py` & `naludaq-0.26.1/src/naludaq/tools/optimizers/gainstagetuner.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/pedestals/__init__.py` & `naludaq-0.26.1/src/naludaq/tools/pedestals/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/pedestals/generators/__init__.py` & `naludaq-0.26.1/src/naludaq/tools/pedestals/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/pedestals/generators/default.py` & `naludaq-0.26.1/src/naludaq/tools/pedestals/generators/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/pedestals/generators/hdsoc.py` & `naludaq-0.26.1/src/naludaq/tools/pedestals/generators/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/pedestals/generators/udc16.py` & `naludaq-0.26.1/src/naludaq/tools/pedestals/generators/udc16.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/pedestals/generators/upac96.py` & `naludaq-0.26.1/src/naludaq/tools/pedestals/generators/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/pedestals/pedestals_correcter.py` & `naludaq-0.26.1/src/naludaq/tools/pedestals/pedestals_correcter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/pedestals/pedestals_processor.py` & `naludaq-0.26.1/src/naludaq/tools/pedestals/pedestals_processor.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/pedestals/upac32_pedestals_controller.py` & `naludaq-0.26.1/src/naludaq/tools/pedestals/upac32_pedestals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/threshold_scan/__init__.py` & `naludaq-0.26.1/src/naludaq/tools/threshold_scan/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py` & `naludaq-0.26.1/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/threshold_scan/threshold_scan.py` & `naludaq-0.26.1/src/naludaq/tools/threshold_scan/threshold_scan.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/threshold_scan/upac96_thresholdscan.py` & `naludaq-0.26.1/src/naludaq/tools/threshold_scan/upac96_thresholdscan.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/timing_cal/__init__.py` & `naludaq-0.26.1/src/naludaq/tools/timing_cal/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/timing_cal/calibration.py` & `naludaq-0.26.1/src/naludaq/tools/timing_cal/calibration.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/timing_cal/correcter.py` & `naludaq-0.26.1/src/naludaq/tools/timing_cal/correcter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq/tools/waiter/eventwaiter.py` & `naludaq-0.26.1/src/naludaq/tools/waiter/eventwaiter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.0/src/naludaq.egg-info/PKG-INFO` & `naludaq-0.26.1/src/naludaq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naludaq
-Version: 0.26.0
+Version: 0.26.1
 Summary: Backend package for Nalu Scientific hardware
 Home-page: 
 Author: Thomas Yang, Emily Lum, Terry Pham
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naludaq-0.26.0/src/naludaq.egg-info/SOURCES.txt` & `naludaq-0.26.1/src/naludaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*


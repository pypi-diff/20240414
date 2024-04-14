# Comparing `tmp/iqrfpy-0.2.0.tar.gz` & `tmp/iqrfpy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iqrfpy-0.2.0.tar", last modified: Tue Apr  2 15:26:37 2024, max compression
+gzip compressed data, was "iqrfpy-0.2.1.tar", last modified: Sun Apr 14 16:20:58 2024, max compression
```

## Comparing `iqrfpy-0.2.0.tar` & `iqrfpy-0.2.1.tar`

### file list

```diff
@@ -1,303 +1,305 @@
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.307729 iqrfpy-0.2.0/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    11351 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/LICENSE
--rw-r--r--   0 khanak    (1000) khanak    (1000)     4862 2024-04-02 15:26:37.307729 iqrfpy-0.2.0/PKG-INFO
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3314 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/README.md
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.279728 iqrfpy-0.2.0/iqrfpy/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      235 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4377 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/async_response.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4162 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/confirmation.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.283728 iqrfpy-0.2.0/iqrfpy/enums/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      285 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/enums/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     8125 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/enums/commands.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5591 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/enums/message_types.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      691 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/enums/peripherals.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/enums/py.typed
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     7981 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/exceptions.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.283728 iqrfpy-0.2.0/iqrfpy/ext/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      281 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/ext/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/ext/py.typed
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    14585 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/irequest.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     6708 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/iresponse.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3391 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/itransport.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    12857 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/messages.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.283728 iqrfpy-0.2.0/iqrfpy/objects/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1421 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3119 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/binaryoutput_state.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2439 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/coordinator_authorize_bond_params.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      253 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/coordinator_dpa_param.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1316 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/exploration_per_enum_data.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      955 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/exploration_per_info_data.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1279 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/frc_params.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3135 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/io_triplet.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1249 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/node_read_data.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2327 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/node_validate_bonds_params.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5710 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/os_batch_data.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      224 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/os_indicate_param.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1295 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/os_load_code_flags.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1244 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/os_read_data.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      200 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/os_security_type_param.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3719 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/os_sleep_params.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4125 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/os_tr_conf_byte.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    29989 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/os_tr_conf_data.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1911 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/sensor_data.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2535 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/sensor_written_data.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.283728 iqrfpy-0.2.0/iqrfpy/peripherals/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      418 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.283728 iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      414 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.283728 iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      236 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2660 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/requests/enumerate.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4543 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/requests/set_output.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.283728 iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      197 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3516 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/responses/enumerate.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3616 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/responses/set_output.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.283728 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1623 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.287728 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1338 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2612 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/addr_info.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4522 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/authorize_bond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3655 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/backup.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5435 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/bond_node.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2647 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/bonded_devices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2650 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/clear_all_bonds.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2675 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/discovered_devices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5205 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/discovery.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3853 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/remove_bond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4203 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/restore.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4036 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/set_dpa_params.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5298 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/set_hops.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5116 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/set_mid.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     9428 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/smart_connect.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1046 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3677 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/addr_info.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3791 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/authorize_bond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3432 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/backup.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3725 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/bond_node.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3563 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/bonded_devices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2941 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/clear_all_bonds.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3647 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/discovered_devices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3429 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/discovery.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3441 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/remove_bond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2857 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/restore.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3588 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/set_dpa_params.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3783 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/set_hops.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2704 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/set_mid.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3776 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/smart_connect.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      299 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      160 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4978 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/requests/read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5136 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/requests/write.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      165 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3330 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/responses/read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2856 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/responses/write.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      298 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      159 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4934 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/requests/read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5132 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/requests/write.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      164 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3351 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/responses/read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2877 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/responses/write.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      733 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      376 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2870 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/requests/more_peripherals_information.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2730 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/requests/peripheral_enumeration.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3218 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/requests/peripheral_information.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      516 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4752 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/responses/more_peripherals_information.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4888 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/responses/peripheral_enumeration.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4183 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/responses/peripheral_information.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/frc/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      594 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/frc/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      392 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2604 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/requests/extra_result.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5101 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/requests/send.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     6786 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/requests/send_selective.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4064 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/requests/set_frc_params.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/frc/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      336 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3483 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/responses/extra_result.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3711 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/responses/send.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3833 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/responses/send_selective.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3485 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/responses/set_frc_params.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/generic/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      370 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/generic/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/generic/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      106 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/generic/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3268 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/generic/requests/generic.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/generic/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      109 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/generic/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3182 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/generic/responses/generic.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/io/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      435 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/io/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/io/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      275 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/io/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4126 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/io/requests/direction.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2553 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/io/requests/get.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4084 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/io/requests/set.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/io/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      217 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/io/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2873 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/io/responses/direction.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3298 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/io/responses/get.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2795 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/io/responses/set.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      499 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      278 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2583 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/requests/flashing.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2562 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/requests/pulse.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2574 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/requests/set_off.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2567 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/requests/set_on.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      287 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2696 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/responses/flashing.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2660 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/responses/pulse.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2677 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/responses/set_off.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2665 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/responses/set_on.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      499 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      278 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2583 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/requests/flashing.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2562 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/requests/pulse.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2574 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/requests/set_off.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2567 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/requests/set_on.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      287 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2696 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/responses/flashing.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2660 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/responses/pulse.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2677 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/responses/set_off.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2665 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/responses/set_on.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/node/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      719 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/node/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      419 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3606 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/requests/backup.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2557 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/requests/read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2604 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/requests/remove_bond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3938 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/requests/restore.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4425 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/requests/validate_bonds.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.299729 iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      448 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3430 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/backup.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3858 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2756 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/remove_bond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2861 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/restore.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2944 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/validate_bonds.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.299729 iqrfpy-0.2.0/iqrfpy/peripherals/os/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1860 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.299729 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1351 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3903 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/batch.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2625 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/factory_settings.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3203 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/indicate.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     7831 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/load_code.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2543 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2615 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/read_tr_conf.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2550 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/reset.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2564 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/restart.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2550 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/rfpgm.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5689 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/selective_batch.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5437 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/set_security.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3209 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/sleep.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5979 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/test_rf_signal.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4243 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/write_tr_conf.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4128 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/write_tr_conf_byte.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1149 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2711 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/batch.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2846 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/factory_settings.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2750 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/indicate.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4342 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/load_code.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4973 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4550 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/read_tr_conf.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2711 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/reset.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2737 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/restart.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2705 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/rfpgm.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2823 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/selective_batch.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2788 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/set_security.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2705 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/sleep.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4084 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/test_rf_signal.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2818 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/write_tr_conf.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2870 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/write_tr_conf_byte.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/py.typed
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/ram/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      396 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ram/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/ram/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      215 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ram/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4913 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ram/requests/read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4878 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ram/requests/read_any.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5108 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ram/requests/write.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/ram/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      222 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ram/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3349 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ram/responses/read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3272 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ram/responses/read_any.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2856 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ram/responses/write.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      587 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      381 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2592 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/requests/enumerate.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5088 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/requests/read_sensors.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5631 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/requests/read_sensors_with_types.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      366 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3721 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/responses/enumerate.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3239 2024-03-26 15:40:45.000000 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/responses/read_sensors.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3880 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/responses/read_sensors_with_types.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/thermometer/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      229 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/thermometer/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/thermometer/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      112 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/thermometer/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2606 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/thermometer/requests/read.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/thermometer/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      115 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/thermometer/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3693 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/thermometer/responses/read.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/uart/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      515 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/uart/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      303 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5734 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/requests/clear_write_read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2564 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/requests/close.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3778 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/requests/open.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5684 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/requests/write_read.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/uart/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      312 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3460 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/responses/clear_write_read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2690 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/responses/close.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2678 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/responses/open.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3395 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/responses/write_read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/py.typed
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    42518 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/response_factory.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.307729 iqrfpy-0.2.0/iqrfpy/utils/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      272 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/utils/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    27163 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/utils/common.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     8471 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/utils/dpa.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      563 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/utils/enums.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2175 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/utils/frc_parser.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/utils/py.typed
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    14876 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/utils/quantity_data.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2659 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/utils/sensor_constants.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    26301 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/utils/sensor_parser.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3397 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/utils/validators.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.307729 iqrfpy-0.2.0/iqrfpy.egg-info/
--rw-r--r--   0 khanak    (1000) khanak    (1000)     4862 2024-04-02 15:26:37.000000 iqrfpy-0.2.0/iqrfpy.egg-info/PKG-INFO
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    10578 2024-04-02 15:26:37.000000 iqrfpy-0.2.0/iqrfpy.egg-info/SOURCES.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        1 2024-04-02 15:26:37.000000 iqrfpy-0.2.0/iqrfpy.egg-info/dependency_links.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      114 2024-04-02 15:26:37.000000 iqrfpy-0.2.0/iqrfpy.egg-info/requires.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        7 2024-04-02 15:26:37.000000 iqrfpy-0.2.0/iqrfpy.egg-info/top_level.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      116 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/pyproject.toml
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1545 2024-04-02 15:26:37.307729 iqrfpy-0.2.0/setup.cfg
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.964932 iqrfpy-0.2.1/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    11351 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/LICENSE
+-rw-r--r--   0 khanak    (1000) khanak    (1000)     4862 2024-04-14 16:20:58.964932 iqrfpy-0.2.1/PKG-INFO
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3314 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/README.md
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.940931 iqrfpy-0.2.1/iqrfpy/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      235 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4379 2024-04-14 14:45:29.000000 iqrfpy-0.2.1/iqrfpy/async_response.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4163 2024-04-14 14:44:54.000000 iqrfpy-0.2.1/iqrfpy/confirmation.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.940931 iqrfpy-0.2.1/iqrfpy/enums/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      284 2024-04-14 15:45:45.000000 iqrfpy-0.2.1/iqrfpy/enums/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     8049 2024-04-12 14:09:30.000000 iqrfpy-0.2.1/iqrfpy/enums/commands.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5261 2024-04-12 14:09:30.000000 iqrfpy-0.2.1/iqrfpy/enums/message_types.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      615 2024-04-12 14:09:30.000000 iqrfpy-0.2.1/iqrfpy/enums/peripherals.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/enums/py.typed
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     7981 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/exceptions.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.940931 iqrfpy-0.2.1/iqrfpy/ext/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      376 2024-04-14 14:34:14.000000 iqrfpy-0.2.1/iqrfpy/ext/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/ext/py.typed
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    14602 2024-04-14 14:47:29.000000 iqrfpy-0.2.1/iqrfpy/irequest.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     6711 2024-04-14 14:45:57.000000 iqrfpy-0.2.1/iqrfpy/iresponse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3391 2024-04-14 14:47:42.000000 iqrfpy-0.2.1/iqrfpy/itransport.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    12857 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/messages.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.944932 iqrfpy-0.2.1/iqrfpy/objects/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1421 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/objects/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3119 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/objects/binaryoutput_state.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2441 2024-04-14 14:42:17.000000 iqrfpy-0.2.1/iqrfpy/objects/coordinator_authorize_bond_params.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      253 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/objects/coordinator_dpa_param.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1316 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/objects/exploration_per_enum_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      955 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/objects/exploration_per_info_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1279 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/objects/frc_params.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      900 2024-04-12 16:31:49.000000 iqrfpy-0.2.1/iqrfpy/objects/init_phy_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3138 2024-04-14 14:42:36.000000 iqrfpy-0.2.1/iqrfpy/objects/io_triplet.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1249 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/objects/node_read_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2329 2024-04-14 14:43:12.000000 iqrfpy-0.2.1/iqrfpy/objects/node_validate_bonds_params.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5713 2024-04-14 14:35:06.000000 iqrfpy-0.2.1/iqrfpy/objects/os_batch_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      224 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/objects/os_indicate_param.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1295 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/objects/os_load_code_flags.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1321 2024-04-12 16:24:06.000000 iqrfpy-0.2.1/iqrfpy/objects/os_read_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      200 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/objects/os_security_type_param.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3720 2024-04-14 14:42:47.000000 iqrfpy-0.2.1/iqrfpy/objects/os_sleep_params.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4430 2024-04-14 14:53:00.000000 iqrfpy-0.2.1/iqrfpy/objects/os_tr_conf_byte.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    30892 2024-04-14 14:50:47.000000 iqrfpy-0.2.1/iqrfpy/objects/os_tr_conf_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1911 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/objects/sensor_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2537 2024-04-14 14:42:44.000000 iqrfpy-0.2.1/iqrfpy/objects/sensor_written_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1122 2024-04-14 14:52:06.000000 iqrfpy-0.2.1/iqrfpy/objects/tr_mcu_type_data.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.944932 iqrfpy-0.2.1/iqrfpy/peripherals/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      418 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.944932 iqrfpy-0.2.1/iqrfpy/peripherals/binaryoutput/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      414 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/binaryoutput/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.944932 iqrfpy-0.2.1/iqrfpy/peripherals/binaryoutput/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      236 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/binaryoutput/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2660 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/binaryoutput/requests/enumerate.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4543 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/binaryoutput/requests/set_output.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.944932 iqrfpy-0.2.1/iqrfpy/peripherals/binaryoutput/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      197 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/binaryoutput/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3516 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/binaryoutput/responses/enumerate.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3616 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/binaryoutput/responses/set_output.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.944932 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1623 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.944932 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1338 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2612 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/addr_info.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4523 2024-04-14 14:03:12.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/authorize_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3656 2024-04-14 14:01:16.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/backup.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5438 2024-04-14 15:49:27.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/bond_node.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2647 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/bonded_devices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2650 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/clear_all_bonds.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2675 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/discovered_devices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5208 2024-04-14 14:48:14.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/discovery.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3854 2024-04-14 14:03:32.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/remove_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4204 2024-04-14 14:02:47.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/restore.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4037 2024-04-14 14:01:43.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/set_dpa_params.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5300 2024-04-14 14:02:41.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/set_hops.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5118 2024-04-14 14:01:30.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/set_mid.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     9433 2024-04-14 14:02:32.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/smart_connect.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.948932 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1046 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3679 2024-04-14 14:08:17.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/addr_info.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3793 2024-04-14 14:08:30.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/authorize_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3434 2024-04-14 14:07:56.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/backup.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3727 2024-04-14 14:04:30.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/bond_node.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3565 2024-04-14 14:04:15.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/bonded_devices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2943 2024-04-14 14:04:43.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/clear_all_bonds.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3649 2024-04-14 14:03:42.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/discovered_devices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3431 2024-04-14 14:08:50.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/discovery.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3443 2024-04-14 14:09:01.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/remove_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2859 2024-04-14 14:04:24.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/restore.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3590 2024-04-14 14:03:48.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/set_dpa_params.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3785 2024-04-14 14:04:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/set_hops.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2706 2024-04-14 14:08:07.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/set_mid.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3778 2024-04-14 14:03:55.000000 iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/smart_connect.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.948932 iqrfpy-0.2.1/iqrfpy/peripherals/eeeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      299 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/eeeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.948932 iqrfpy-0.2.1/iqrfpy/peripherals/eeeprom/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      160 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/eeeprom/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4980 2024-04-14 14:24:23.000000 iqrfpy-0.2.1/iqrfpy/peripherals/eeeprom/requests/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5137 2024-04-14 14:24:28.000000 iqrfpy-0.2.1/iqrfpy/peripherals/eeeprom/requests/write.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.948932 iqrfpy-0.2.1/iqrfpy/peripherals/eeeprom/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      165 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/eeeprom/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3332 2024-04-14 14:24:36.000000 iqrfpy-0.2.1/iqrfpy/peripherals/eeeprom/responses/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2858 2024-04-14 14:24:45.000000 iqrfpy-0.2.1/iqrfpy/peripherals/eeeprom/responses/write.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.948932 iqrfpy-0.2.1/iqrfpy/peripherals/eeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      298 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/eeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.948932 iqrfpy-0.2.1/iqrfpy/peripherals/eeprom/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      159 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/eeprom/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4936 2024-04-14 14:23:49.000000 iqrfpy-0.2.1/iqrfpy/peripherals/eeprom/requests/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5133 2024-04-14 14:23:52.000000 iqrfpy-0.2.1/iqrfpy/peripherals/eeprom/requests/write.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.948932 iqrfpy-0.2.1/iqrfpy/peripherals/eeprom/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      164 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/eeprom/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3353 2024-04-14 14:23:58.000000 iqrfpy-0.2.1/iqrfpy/peripherals/eeprom/responses/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2879 2024-04-14 14:24:11.000000 iqrfpy-0.2.1/iqrfpy/peripherals/eeprom/responses/write.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.948932 iqrfpy-0.2.1/iqrfpy/peripherals/exploration/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      733 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/exploration/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.948932 iqrfpy-0.2.1/iqrfpy/peripherals/exploration/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      376 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/exploration/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2934 2024-04-14 14:10:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/exploration/requests/more_peripherals_information.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2730 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/exploration/requests/peripheral_enumeration.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3218 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/exploration/requests/peripheral_information.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.948932 iqrfpy-0.2.1/iqrfpy/peripherals/exploration/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      516 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/exploration/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4754 2024-04-14 14:10:57.000000 iqrfpy-0.2.1/iqrfpy/peripherals/exploration/responses/more_peripherals_information.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4882 2024-04-14 14:11:02.000000 iqrfpy-0.2.1/iqrfpy/peripherals/exploration/responses/peripheral_enumeration.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4185 2024-04-14 14:10:52.000000 iqrfpy-0.2.1/iqrfpy/peripherals/exploration/responses/peripheral_information.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.948932 iqrfpy-0.2.1/iqrfpy/peripherals/frc/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      594 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/frc/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.948932 iqrfpy-0.2.1/iqrfpy/peripherals/frc/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      392 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/frc/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2604 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/frc/requests/extra_result.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5102 2024-04-14 14:15:18.000000 iqrfpy-0.2.1/iqrfpy/peripherals/frc/requests/send.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     6789 2024-04-14 14:19:27.000000 iqrfpy-0.2.1/iqrfpy/peripherals/frc/requests/send_selective.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4065 2024-04-14 14:15:24.000000 iqrfpy-0.2.1/iqrfpy/peripherals/frc/requests/set_frc_params.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.952932 iqrfpy-0.2.1/iqrfpy/peripherals/frc/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      336 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/frc/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3485 2024-04-14 14:17:50.000000 iqrfpy-0.2.1/iqrfpy/peripherals/frc/responses/extra_result.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3713 2024-04-14 14:16:40.000000 iqrfpy-0.2.1/iqrfpy/peripherals/frc/responses/send.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3835 2024-04-14 14:17:43.000000 iqrfpy-0.2.1/iqrfpy/peripherals/frc/responses/send_selective.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3557 2024-04-14 14:17:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/frc/responses/set_frc_params.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.952932 iqrfpy-0.2.1/iqrfpy/peripherals/generic/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      370 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/generic/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.952932 iqrfpy-0.2.1/iqrfpy/peripherals/generic/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      106 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/generic/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3268 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/generic/requests/generic.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.952932 iqrfpy-0.2.1/iqrfpy/peripherals/generic/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      109 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/generic/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3382 2024-04-14 14:16:16.000000 iqrfpy-0.2.1/iqrfpy/peripherals/generic/responses/generic.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.952932 iqrfpy-0.2.1/iqrfpy/peripherals/io/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      435 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/io/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.952932 iqrfpy-0.2.1/iqrfpy/peripherals/io/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      275 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/io/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4127 2024-04-14 14:20:30.000000 iqrfpy-0.2.1/iqrfpy/peripherals/io/requests/direction.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2553 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/io/requests/get.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4085 2024-04-14 14:28:05.000000 iqrfpy-0.2.1/iqrfpy/peripherals/io/requests/set.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.952932 iqrfpy-0.2.1/iqrfpy/peripherals/io/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      217 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/io/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2875 2024-04-14 14:20:36.000000 iqrfpy-0.2.1/iqrfpy/peripherals/io/responses/direction.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3300 2024-04-14 14:20:41.000000 iqrfpy-0.2.1/iqrfpy/peripherals/io/responses/get.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2797 2024-04-14 14:20:51.000000 iqrfpy-0.2.1/iqrfpy/peripherals/io/responses/set.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.952932 iqrfpy-0.2.1/iqrfpy/peripherals/ledg/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      499 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledg/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.952932 iqrfpy-0.2.1/iqrfpy/peripherals/ledg/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      278 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledg/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2583 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledg/requests/flashing.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2562 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledg/requests/pulse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2574 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledg/requests/set_off.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2567 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledg/requests/set_on.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.952932 iqrfpy-0.2.1/iqrfpy/peripherals/ledg/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      287 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledg/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2698 2024-04-14 14:24:51.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledg/responses/flashing.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2662 2024-04-14 14:25:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledg/responses/pulse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2679 2024-04-14 14:24:56.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledg/responses/set_off.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2667 2024-04-14 14:25:03.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledg/responses/set_on.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.952932 iqrfpy-0.2.1/iqrfpy/peripherals/ledr/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      499 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledr/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.952932 iqrfpy-0.2.1/iqrfpy/peripherals/ledr/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      278 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledr/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2583 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledr/requests/flashing.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2562 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledr/requests/pulse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2574 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledr/requests/set_off.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2567 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledr/requests/set_on.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.952932 iqrfpy-0.2.1/iqrfpy/peripherals/ledr/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      287 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledr/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2698 2024-04-14 14:23:12.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledr/responses/flashing.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2662 2024-04-14 14:23:34.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledr/responses/pulse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2679 2024-04-14 14:23:16.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledr/responses/set_off.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2667 2024-04-14 14:23:23.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ledr/responses/set_on.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.952932 iqrfpy-0.2.1/iqrfpy/peripherals/node/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      719 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/node/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.952932 iqrfpy-0.2.1/iqrfpy/peripherals/node/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      419 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/node/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3607 2024-04-14 14:13:30.000000 iqrfpy-0.2.1/iqrfpy/peripherals/node/requests/backup.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2557 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/node/requests/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2604 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/node/requests/remove_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3939 2024-04-14 14:19:01.000000 iqrfpy-0.2.1/iqrfpy/peripherals/node/requests/restore.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4426 2024-04-14 14:13:26.000000 iqrfpy-0.2.1/iqrfpy/peripherals/node/requests/validate_bonds.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.956932 iqrfpy-0.2.1/iqrfpy/peripherals/node/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      448 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/node/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3432 2024-04-14 14:14:06.000000 iqrfpy-0.2.1/iqrfpy/peripherals/node/responses/backup.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3860 2024-04-14 14:13:54.000000 iqrfpy-0.2.1/iqrfpy/peripherals/node/responses/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2758 2024-04-14 14:14:11.000000 iqrfpy-0.2.1/iqrfpy/peripherals/node/responses/remove_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2863 2024-04-14 14:13:46.000000 iqrfpy-0.2.1/iqrfpy/peripherals/node/responses/restore.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2946 2024-04-14 14:13:38.000000 iqrfpy-0.2.1/iqrfpy/peripherals/node/responses/validate_bonds.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.956932 iqrfpy-0.2.1/iqrfpy/peripherals/os/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1860 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.956932 iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1351 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3903 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/batch.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2625 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/factory_settings.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3203 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/indicate.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     7835 2024-04-14 14:21:12.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/load_code.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2543 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2615 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/read_tr_conf.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2550 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/reset.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2564 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/restart.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2550 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/rfpgm.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5690 2024-04-14 14:20:58.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/selective_batch.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5439 2024-04-14 14:21:26.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/set_security.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3209 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/sleep.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5979 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/test_rf_signal.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4243 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/write_tr_conf.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4128 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/write_tr_conf_byte.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.956932 iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1149 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2713 2024-04-14 14:22:16.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/batch.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2848 2024-04-14 14:21:54.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/factory_settings.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2752 2024-04-14 14:21:31.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/indicate.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4336 2024-04-14 14:21:44.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/load_code.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4967 2024-04-14 14:22:11.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4617 2024-04-14 14:22:28.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/read_tr_conf.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2713 2024-04-14 14:22:04.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/reset.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2739 2024-04-14 14:22:33.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/restart.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2707 2024-04-14 14:22:23.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/rfpgm.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2825 2024-04-14 14:21:37.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/selective_batch.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2790 2024-04-14 14:21:49.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/set_security.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2707 2024-04-14 14:22:40.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/sleep.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4084 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/test_rf_signal.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2820 2024-04-14 14:22:56.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/write_tr_conf.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2872 2024-04-14 14:22:47.000000 iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/write_tr_conf_byte.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/py.typed
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.956932 iqrfpy-0.2.1/iqrfpy/peripherals/ram/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      396 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ram/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.956932 iqrfpy-0.2.1/iqrfpy/peripherals/ram/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      215 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ram/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4915 2024-04-14 14:14:42.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ram/requests/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4881 2024-04-14 14:14:26.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ram/requests/read_any.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5109 2024-04-14 14:14:45.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ram/requests/write.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.960932 iqrfpy-0.2.1/iqrfpy/peripherals/ram/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      222 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ram/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3351 2024-04-14 14:19:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ram/responses/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3275 2024-04-14 14:15:01.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ram/responses/read_any.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2858 2024-04-14 14:15:12.000000 iqrfpy-0.2.1/iqrfpy/peripherals/ram/responses/write.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.960932 iqrfpy-0.2.1/iqrfpy/peripherals/sensor/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      587 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/sensor/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.960932 iqrfpy-0.2.1/iqrfpy/peripherals/sensor/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      381 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/sensor/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2592 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/sensor/requests/enumerate.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5087 2024-04-14 14:19:53.000000 iqrfpy-0.2.1/iqrfpy/peripherals/sensor/requests/read_sensors.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5629 2024-04-14 14:19:37.000000 iqrfpy-0.2.1/iqrfpy/peripherals/sensor/requests/read_sensors_with_types.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.960932 iqrfpy-0.2.1/iqrfpy/peripherals/sensor/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      366 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/sensor/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3723 2024-04-14 14:20:02.000000 iqrfpy-0.2.1/iqrfpy/peripherals/sensor/responses/enumerate.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3242 2024-04-14 14:20:21.000000 iqrfpy-0.2.1/iqrfpy/peripherals/sensor/responses/read_sensors.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3882 2024-04-14 14:20:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/sensor/responses/read_sensors_with_types.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.960932 iqrfpy-0.2.1/iqrfpy/peripherals/thermometer/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      229 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/thermometer/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.960932 iqrfpy-0.2.1/iqrfpy/peripherals/thermometer/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      112 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/thermometer/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2606 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/thermometer/requests/read.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.960932 iqrfpy-0.2.1/iqrfpy/peripherals/thermometer/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      115 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/thermometer/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3695 2024-04-14 14:11:10.000000 iqrfpy-0.2.1/iqrfpy/peripherals/thermometer/responses/read.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.960932 iqrfpy-0.2.1/iqrfpy/peripherals/uart/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      515 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/uart/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.960932 iqrfpy-0.2.1/iqrfpy/peripherals/uart/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      303 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/uart/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5736 2024-04-14 14:11:33.000000 iqrfpy-0.2.1/iqrfpy/peripherals/uart/requests/clear_write_read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2564 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/uart/requests/close.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3779 2024-04-14 14:11:19.000000 iqrfpy-0.2.1/iqrfpy/peripherals/uart/requests/open.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5686 2024-04-14 14:11:45.000000 iqrfpy-0.2.1/iqrfpy/peripherals/uart/requests/write_read.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.960932 iqrfpy-0.2.1/iqrfpy/peripherals/uart/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      312 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/uart/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3462 2024-04-14 14:12:00.000000 iqrfpy-0.2.1/iqrfpy/peripherals/uart/responses/clear_write_read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2692 2024-04-14 14:12:15.000000 iqrfpy-0.2.1/iqrfpy/peripherals/uart/responses/close.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2680 2024-04-14 14:11:54.000000 iqrfpy-0.2.1/iqrfpy/peripherals/uart/responses/open.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3397 2024-04-14 14:12:09.000000 iqrfpy-0.2.1/iqrfpy/peripherals/uart/responses/write_read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/py.typed
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    42515 2024-04-14 14:45:20.000000 iqrfpy-0.2.1/iqrfpy/response_factory.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.964932 iqrfpy-0.2.1/iqrfpy/utils/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      272 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/utils/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    30552 2024-04-14 15:02:10.000000 iqrfpy-0.2.1/iqrfpy/utils/common.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    11063 2024-04-14 14:32:00.000000 iqrfpy-0.2.1/iqrfpy/utils/dpa.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      755 2024-04-12 14:02:36.000000 iqrfpy-0.2.1/iqrfpy/utils/enums.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2175 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/utils/frc_parser.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/iqrfpy/utils/py.typed
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    14869 2024-04-14 14:27:42.000000 iqrfpy-0.2.1/iqrfpy/utils/quantity_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2661 2024-04-14 14:33:26.000000 iqrfpy-0.2.1/iqrfpy/utils/sensor_constants.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    26329 2024-04-14 14:32:11.000000 iqrfpy-0.2.1/iqrfpy/utils/sensor_parser.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3397 2024-03-18 17:43:19.000000 iqrfpy-0.2.1/iqrfpy/utils/validators.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-14 16:20:58.964932 iqrfpy-0.2.1/iqrfpy.egg-info/
+-rw-r--r--   0 khanak    (1000) khanak    (1000)     4862 2024-04-14 16:20:58.000000 iqrfpy-0.2.1/iqrfpy.egg-info/PKG-INFO
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    10645 2024-04-14 16:20:58.000000 iqrfpy-0.2.1/iqrfpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        1 2024-04-14 16:20:58.000000 iqrfpy-0.2.1/iqrfpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      114 2024-04-14 16:20:58.000000 iqrfpy-0.2.1/iqrfpy.egg-info/requires.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        7 2024-04-14 16:20:58.000000 iqrfpy-0.2.1/iqrfpy.egg-info/top_level.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      116 2024-04-02 13:56:09.000000 iqrfpy-0.2.1/pyproject.toml
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1545 2024-04-14 16:20:58.964932 iqrfpy-0.2.1/setup.cfg
```

### Comparing `iqrfpy-0.2.0/LICENSE` & `iqrfpy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/PKG-INFO` & `iqrfpy-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqrfpy
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python library for communication with IQRF Network
 Home-page: https://gitlab.iqrf.org/open-source/iqrf-sdk/iqrfpy/iqrfpy
 Author: Karel Hanák
 Author-email: karel.hanak@iqrf.org
 License: Apache-2.0
 Project-URL: Changelog, https://apidocs.iqrf.org/iqrfpy/latest/iqrfpy.html#changelog
 Project-URL: Documentation, https://apidocs.iqrf.org/iqrfpy/latest/iqrfpy.html
```

### Comparing `iqrfpy-0.2.0/README.md` & `iqrfpy-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/async_response.py` & `iqrfpy-0.2.1/iqrfpy/async_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     def from_dpa(cls, dpa: bytes) -> 'AsyncResponse':
         """Asynchronous response DPA factory method.
 
         Parses DPA data and constructs :obj:`AsyncResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`AsyncResponse`: Asynchronous response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr = dpa[ResponsePacketMembers.NADR]
         hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
         pnum = Common.pnum_from_dpa(dpa[ResponsePacketMembers.PNUM])
@@ -82,14 +83,15 @@
     def from_json(cls, json: dict) -> 'AsyncResponse':
         """Asynchronous response JSON factory method.
 
         Parses JSON API response and constructs :obj:`AsyncResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`AsyncResponse`: Asynchronous response message object.
         """
         msgid = Common.msgid_from_json(json)
         result = json['data']['rsp']
         packet = result['rData'].replace('.', '')
         pdata = bytes.fromhex(packet)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/confirmation.py` & `iqrfpy-0.2.1/iqrfpy/confirmation.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,14 +81,15 @@
     def from_dpa(cls, dpa: bytes) -> 'Confirmation':
         """Confirmation DPA factory method.
 
         Parses DPA confirmation message and constructs :obj:`Confirmation` object.
 
         Args:
             dpa (bytes): DPA confirmation bytes.
+
         Returns:
             :obj:`Confirmation`: Confirmation message object.
         """
         DpaValidator.confirmation_length(dpa=dpa)
         DpaValidator.confirmation_code(dpa=dpa)
         nadr = dpa[ResponsePacketMembers.NADR]
         pnum = Common.pnum_from_dpa(dpa[ResponsePacketMembers.PNUM])
```

### Comparing `iqrfpy-0.2.0/iqrfpy/enums/commands.py` & `iqrfpy-0.2.1/iqrfpy/enums/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Commands module.
 
 This module contains embed peripherals and standards command enums.
-These enums are extended with has_value() method for member identification.
 """
 
 from ..utils.enums import IntEnumMember
 from .peripherals import EmbedPeripherals
 
 __all__ = [
     'Command',
```

### Comparing `iqrfpy-0.2.0/iqrfpy/enums/message_types.py` & `iqrfpy-0.2.1/iqrfpy/enums/message_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Message types module.
 
 This module contains embed peripherals and standards message type enums.
-These enums are extended with has_value() method for member identification.
 """
 
 import enum
+from ..utils.enums import MetaEnum
 
 __all__ = [
     'MessageType',
     'GenericMessages',
     'ExplorationMessages',
     'CoordinatorMessages',
     'NodeMessages',
@@ -25,28 +25,17 @@
     'DALIMessages',
     'BinaryOutputMessages',
     'SensorMessages',
     'LightMessages'
 ]
 
 
-class MessageType(enum.Enum):
+class MessageType(enum.Enum, metaclass=MetaEnum):
     """JSON API message type base enum."""
 
-    @classmethod
-    def has_value(cls, value: str):
-        """Check if enum class has member value.
-
-        Args:
-            value (str): value to check
-        Returns:
-            :obj`bool`: True if value is a member of enum, False otherwise
-        """
-        return value in cls._value2member_map_
-
 
 class GenericMessages(MessageType):
     """Generic message types enum."""
 
     RAW = 'iqrfRaw'
     RAW_HDP = 'iqrfRawHdp'
```

### Comparing `iqrfpy-0.2.0/iqrfpy/enums/peripherals.py` & `iqrfpy-0.2.1/iqrfpy/enums/peripherals.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Peripherals module.
 
 This module contains embedded peripherals and standards enums.
-These enums are extended with has_value() method for member identification.
 """
 
 from ..utils.enums import IntEnumMember
 
 
 class Peripheral(IntEnumMember):
     """Base peripherals enum class."""
```

### Comparing `iqrfpy-0.2.0/iqrfpy/exceptions.py` & `iqrfpy-0.2.1/iqrfpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/irequest.py` & `iqrfpy-0.2.1/iqrfpy/irequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     RequestHwpidInvalidError, RequestParameterInvalidValueError
 
 __all__ = ['IRequest']
 
 
 class IRequest(ABC):
     """This abstract class serves as an interface for embedded peripherals and standards request messages.
+
     The class provides getters and setters for shared request properties in the form of the @property decorator.
     Shared properties such as device address, peripheral, peripheral command and hwpid are validated here.
     The class also provides generic DPA and JSON serialization methods for derived classes to amend.
     While the abstract class cannot be instantiated, it's methods can be called from a derived class using super.
 
     Network address (nadr) specifies target device: 0 (coordinator), 1-239 (node), 252 (local device),
     254 (temporary address) and 255 (broadcast), other values are reserved. Values in range 0-255.
@@ -227,14 +228,15 @@
 
     @staticmethod
     def _validate_dpa_rsp_time(dpa_rsp_time: Optional[float] = None):
         """Validates dpa timeout parameter.
 
         Args:
             dpa_rsp_time (float, optional): DPA timeout value in seconds. Defaults to None.
+
         Raises:
             RequestParameterInvalidValueError: If dpa_rsp_time is not None and is less than 0.
         """
         if dpa_rsp_time is None:
             return
         if dpa_rsp_time < 0:
             raise RequestParameterInvalidValueError('DPA response time should a positive integer.')
@@ -254,14 +256,15 @@
 
     @staticmethod
     def _validate_dev_process_time(dev_process_time: Optional[float] = None):
         """Validates device processing time parameter.
 
         Args:
             dev_process_time (float, optional): Device processing time value. Defaults to None.
+
         Raises:
             RequestParameterInvalidValueError: If dev_process_time is not None and is less than 0.
         """
         if dev_process_time is None:
             return
         if dev_process_time < 0:
             raise RequestParameterInvalidValueError('Device processing time should be a positive integer.')
@@ -289,15 +292,15 @@
 
     @msgid.setter
     def msgid(self, value: str):
         self._msgid = value
 
     @property
     def mtype(self) -> MessageType:
-        """:obj:`MessageType`
+        """:obj:`MessageType` Message type.
 
         Getter only.
         """
         return self._mtype
 
     @abstractmethod
     def to_dpa(self, mutable: bool = False) -> Union[bytes, bytearray]:
```

### Comparing `iqrfpy-0.2.0/iqrfpy/iresponse.py` & `iqrfpy-0.2.1/iqrfpy/iresponse.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from iqrfpy.utils.validators import DpaValidator
 
 __all__ = ['IResponse', 'IResponseGetterMixin']
 
 
 class IResponse(ABC):
     """This class serves as an interface for embedded peripherals and standards response messages.
+
     This class does not provide any deserialization logic in its factory methods as they simply serve as abstracts.
 
     Once a factory method is implemented, it should be used to parse responses and create response message objects.
     """
 
     ASYNC_MSGID = 'async'
 
@@ -246,22 +247,24 @@
 
     @classmethod
     def from_dpa(cls, dpa: bytes) -> IResponse:
         """Factory method. Parse DPA response into Response object.
 
         Args:
             dpa (bytes): DPA response.
+
         Raises:
             NotImplementedError: Factory method for mixin not implemented.
         """
         raise NotImplementedError('from_dpa() method not implemented.')
 
     @classmethod
     def from_json(cls, json: dict) -> IResponse:
         """Factory method. Parse JSON response into Response object.
 
         Args:
             json (dict): JSON API response.
+
         Raises:
             NotImplementedError: Factory method for mixin not implemented.
         """
         raise NotImplementedError('from_json() method not implemented.')
```

### Comparing `iqrfpy-0.2.0/iqrfpy/itransport.py` & `iqrfpy-0.2.1/iqrfpy/itransport.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,73 +23,80 @@
 
     @abstractmethod
     def terminate(self, force: bool = False) -> None:
         """Terminates transport.
 
         Args:
             force (bool): Force terminate transport.
+
         Raises:
             NotImplementedError: Abstract method not implemented.
         """
         raise NotImplementedError("Abstract method not implemented.")
 
     @abstractmethod
     def send(self, request: IRequest) -> None:
         """Serialize passed request to format acceptable by the communication channel and send request.
 
         Args:
             request (IRequest): Request message to send.
+
         Raises:
             NotImplementedError: Abstract method not implemented.
         """
         raise NotImplementedError("Abstract method not implemented.")
 
     @abstractmethod
     def send_and_receive(self, request: IRequest, timeout: Optional[float] = None) -> IResponse:
-        """Serialize request to format acceptable by the communication channel, send request and receive
-        response synchronously.
+        """Serialize request to format acceptable by the communication channel, send request and receive response synchronously.
 
         Args:
             request (IRequest): Request message to send.
             timeout (float, optional): Response timeout.
+
         Returns:
             :obj:`IResponse`: Response message object.
+
         Raises:
             NotImplementedError: Abstract method not implemented.
         """
         raise NotImplementedError("Abstract method not implemented.")
 
     @abstractmethod
     def receive(self, timeout: Optional[float] = None) -> IResponse:
         """Receive and return response synchronously.
 
         Args:
             timeout (float, optional): Response timeout.
+
         Returns:
             :obj:`IResponse`: Response message object.
+
         Raises:
             NotImplementedError: Abstract method not implemented.
         """
         raise NotImplementedError("Abstract method not implemented.")
 
     @abstractmethod
     def confirmation(self) -> Confirmation:
         """Receive and return confirmation synchronously.
 
         Returns:
             :obj:`Confirmation`: Confirmation message object.
+
         Raises:
             NotImplementedError: Abstract method not implemented.
         """
         raise NotImplementedError("Abstract method not implemented.")
 
     @abstractmethod
     def set_receive_callback(self, callback: Callable[[IResponse], None]) -> None:
         """Set callback to handle asynchronously received messages.
 
         Args:
             callback (Callable[[IResponse], None]): Function to call once a message has been received and successfully
                                                     deserialized.
+
         Raises:
             NotImplementedError: Abstract method not implemented.
         """
         raise NotImplementedError("Abstract method not implemented.")
```

### Comparing `iqrfpy-0.2.0/iqrfpy/messages.py` & `iqrfpy-0.2.1/iqrfpy/messages.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/objects/__init__.py` & `iqrfpy-0.2.1/iqrfpy/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/objects/binaryoutput_state.py` & `iqrfpy-0.2.1/iqrfpy/objects/binaryoutput_state.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/objects/coordinator_authorize_bond_params.py` & `iqrfpy-0.2.1/iqrfpy/objects/coordinator_authorize_bond_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
     @staticmethod
     def _validate_req_addr(req_addr: int):
         """Validates requested node address.
 
         Args:
             req_addr (int): Requested node address.
+
         Raises:
             RequestParameterInvalidValueError: If req_addr is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= req_addr <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Requested address value should be between 1 and 239.')
 
     @property
@@ -60,14 +61,15 @@
 
     @staticmethod
     def _validate_mid(mid: int):
         """Validates module ID.
 
         Args:
             mid (int): Module ID.
+
         Raises:
             RequestParameterInvalidValueError: If mid is less than 0 or greater than 4294967295.
         """
         if not dpa_constants.MID_MIN <= mid <= dpa_constants.MID_MAX:
             raise RequestParameterInvalidValueError('MID value should be an unsigned 32bit integer.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/objects/exploration_per_enum_data.py` & `iqrfpy-0.2.1/iqrfpy/objects/exploration_per_enum_data.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/objects/exploration_per_info_data.py` & `iqrfpy-0.2.1/iqrfpy/objects/exploration_per_info_data.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/objects/frc_params.py` & `iqrfpy-0.2.1/iqrfpy/objects/frc_params.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/objects/io_triplet.py` & `iqrfpy-0.2.1/iqrfpy/objects/io_triplet.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
     @staticmethod
     def _validate_port(port: Union[IoConstants, int]):
         """Validate port number.
 
         Args:
             port (Union[IoConstants, int]): Port number.
+
         Raises:
             RequestParameterInvalidValueError: If port is less than 0 or greater than 255.
         """
         if not BYTE_MIN <= port <= BYTE_MAX:
             raise RequestParameterInvalidValueError('Port should be between 0 and 255.')
 
     @property
@@ -61,14 +62,15 @@
 
     @staticmethod
     def _validate_mask(mask: int):
         """Validate port pin mask.
 
         Args:
             mask (int): Port pin mask.
+
         Raises:
             RequestParameterInvalidValueError: If mask is less than 0 or greater than 255.
         """
         if not BYTE_MIN <= mask <= BYTE_MAX:
             raise RequestParameterInvalidValueError('Mask should be between 0 and 255.')
 
     @property
@@ -86,14 +88,15 @@
 
     @staticmethod
     def _validate_value(value: int):
         """Validate value to write.
 
         Args:
             value (int): Value to write.
+
         Raises:
             RequestParameterInvalidValueError: If value is less than 0 or greater than 255.
         """
         if not BYTE_MIN <= value <= BYTE_MAX:
             raise RequestParameterInvalidValueError('Value should be between 0 and 255.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/objects/node_read_data.py` & `iqrfpy-0.2.1/iqrfpy/objects/node_read_data.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/objects/node_validate_bonds_params.py` & `iqrfpy-0.2.1/iqrfpy/objects/node_validate_bonds_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
     @staticmethod
     def _validate_bond_addr(bond_addr: int):
         """Validate node device address parameter.
 
         Args:
             bond_addr (int): Node device address.
+
         Raises:
             RequestParameterInvalidValueError: If bond_addr is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= bond_addr <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Bond address value should be between 0 and 255.')
 
     @property
@@ -56,14 +57,15 @@
 
     @staticmethod
     def _validate_mid(mid: int):
         """Validate module ID parameter.
 
         Args:
             mid (int): Node module ID.
+
         Raises:
             RequestParameterInvalidValueError: If mid is less than 0 or greater than 4294967295.
         """
         if not dpa_constants.MID_MIN <= mid <= dpa_constants.MID_MAX:
             raise RequestParameterInvalidValueError('MID value should be an unsigned 32bit integer.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/objects/os_batch_data.py` & `iqrfpy-0.2.1/iqrfpy/objects/os_batch_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
     @staticmethod
     def _validate_pnum(pnum: Union[Peripheral, int]):
         """Validate peripheral number parameter.
 
         Args:
             pnum (Union[Peripheral, int]): Peripheral number.
+
         Raises:
             RequestParameterInvalidValueError: If pnum is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= pnum <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('PNUM value should be between 0 and 255.')
 
     @property
@@ -70,14 +71,15 @@
 
     @staticmethod
     def _validate_pcmd(pcmd: Union[Command, int]):
         """Validate peripheral command parameter.
 
         Args:
             pcmd (Union[Command, int]): Peripheral command.
+
         Raises:
             RequestParameterInvalidValueError: If pcmd is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= pcmd <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('PCMD value should be between 0 and 255.')
 
     @property
@@ -95,14 +97,15 @@
 
     @staticmethod
     def _validate_hwpid(hwpid: int):
         """Validate hardware profile ID parameter.
 
         Args:
             hwpid (int): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
+
         Raises:
             RequestParameterInvalidValueError: If hwpid is less than 0 or greater than 65535.
         """
         if not dpa_constants.HWPID_MIN <= hwpid <= dpa_constants.HWPID_MAX:
             raise RequestParameterInvalidValueError('HWPID value should be between 0 and 65535.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/objects/os_load_code_flags.py` & `iqrfpy-0.2.1/iqrfpy/objects/os_load_code_flags.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/objects/os_read_data.py` & `iqrfpy-0.2.1/iqrfpy/objects/os_read_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """OS Read Data object."""
 from dataclasses import dataclass
 from .exploration_per_enum_data import ExplorationPerEnumData
+from .tr_mcu_type_data import TrMcuTypeData
 
 
 @dataclass
 class OsReadData:
     """OS Read Data class."""
 
-    __slots__ = 'mid', 'os_version', 'tr_type', 'os_build', 'rssi', 'supply_voltage', 'flags', 'slot_limits', 'ibk', \
+    __slots__ = 'mid', 'os_version', 'tr_mcu_type', 'os_build', 'rssi', 'supply_voltage', 'flags', 'slot_limits', 'ibk', \
         'per_enum'
 
     def __init__(self, data: dict):
         """Read Data constructor.
 
         Args:
             data (dict): OS Read data.
         """
         self.mid: int = data['mid']
         """Module ID."""
         self.os_version: int = data['osVersion']
         """OS version."""
-        self.tr_type: int = data['trMcuType']
+        self.tr_mcu_type: TrMcuTypeData = TrMcuTypeData(data['trMcuType'])
         """MCU type and TR series."""
         self.os_build: int = data['osBuild']
         """OS build."""
         self.rssi: int = data['rssi']
         """RSSI."""
         self.supply_voltage: int = data['supplyVoltage']
         """Supply voltage."""
```

### Comparing `iqrfpy-0.2.0/iqrfpy/objects/os_sleep_params.py` & `iqrfpy-0.2.1/iqrfpy/objects/os_sleep_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
     @staticmethod
     def _validate_time(time: int):
         """Validate sleep time parameter.
 
         Args:
             time (int): Sleep time.
+
         Raises:
             RequestParameterInvalidValueError: If time is less than 0 or greater than 255.
         """
         if not dpa_constants.WORD_MIN <= time <= dpa_constants.WORD_MAX:
             raise RequestParameterInvalidValueError('Time value should be between 0 and 65535.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/objects/os_tr_conf_byte.py` & `iqrfpy-0.2.1/iqrfpy/objects/os_tr_conf_byte.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,15 +18,23 @@
             mask (int): Bits of configuration byte to modify.
         """
         self._validate(address=address, value=value, mask=mask)
         self._address = address
         self._value = value
         self._mask = mask
 
-    def __eq__(self, other):
+    def __eq__(self, other: 'OsTrConfByte'):
+        """Rich comparison method, comparing this and another object to determine equality based on properties.
+
+        Args:
+            other (OsTrConfByte): Object to compare with.
+
+        Returns:
+            bool: True if the objects are equivalent, False otherwise.
+        """
         return self.address == other.address and \
             self.value == other.value and \
             self.mask == other.mask
 
     def _validate(self, address: int, value: int, mask: int):
         """Validate TR Configuration Byte parameters.
 
@@ -41,14 +49,15 @@
 
     @staticmethod
     def _validate_address(address: int):
         """Validate address parameter.
 
         Args:
             address (int): Configuration memory block address.
+
         Raises:
             RequestParameterInvalidValueError: If address is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= address <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Address value should be between 0 and 255.')
 
     @property
@@ -66,14 +75,15 @@
 
     @staticmethod
     def _validate_value(value: int):
         """Validate value parameter.
 
         Args:
             value (int): Value to set.
+
         Raises:
             RequestParameterInvalidValueError: If value is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= value <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Value should be between 0 and 255.')
 
     @property
@@ -91,14 +101,15 @@
 
     @staticmethod
     def _validate_mask(mask: int):
         """Validate mask parameter.
 
         Args:
             mask (int): Bits of configuration byte to modify.
+
         Raises:
             RequestParameterInvalidValueError: If mask is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= mask <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Mask value should be between 0 and 255.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/objects/os_tr_conf_data.py` & `iqrfpy-0.2.1/iqrfpy/objects/os_tr_conf_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,17 @@
             rf_signal_filter (int): RF signal filter.
             lp_rf_timeout (int): LP RF timeout.
             uart_baud_rate (Union[dpa_constants.BaudRates, int]): UART baud rate.
             alternative_dsm_channel (int): Alternative DSM channel.
             local_frc (bool): Local FRC reception enabled.
             rf_channel_a (int): RF Channel A.
             rf_channel_b (int): RF Channel B.
+            reserved_block_0 (List[int], optional): Reserved data block.
+            reserved_block_1 (List[int], optional): Reserved data block.
+            reserved_block_2 (List[int], optional): Reserved data block.
         """
         if embedded_peripherals is None:
             embedded_peripherals = []
         if reserved_block_0 is None:
             reserved_block_0 = [0] * 2
         if reserved_block_1 is None:
             reserved_block_1 = [0] * 3
@@ -75,14 +78,22 @@
         self._rf_channel_a = rf_channel_a
         self._rf_channel_b = rf_channel_b
         self._reserved_block_0 = reserved_block_0
         self._reserved_block_1 = reserved_block_1
         self._reserved_block_2 = reserved_block_2
 
     def __eq__(self, other: 'OsTrConfData'):
+        """Rich comparison method, comparing this and another object to determine equality based on properties.
+
+        Args:
+            other (OsTrConfData): Object to compare with.
+
+        Returns:
+            bool: True if the objects are equivalent, False otherwise.
+        """
         return self._embedded_peripherals == other._embedded_peripherals and \
             self._custom_dpa_handler == other._custom_dpa_handler and \
             self._dpa_peer_to_peer == other._dpa_peer_to_peer and \
             self._routing_off == other.routing_off and \
             self._io_setup == other._io_setup and \
             self._user_peer_to_peer == other._user_peer_to_peer and \
             self._stay_awake_when_not_bonded == other._stay_awake_when_not_bonded and \
@@ -136,42 +147,46 @@
         self._embedded_peripherals = value
 
     def enable_embedded_peripheral(self, peripheral: Union[EmbedPeripherals, int]) -> None:
         """Enables embedded peripheral.
 
         Args:
             peripheral (:obj:`EmbeddedPeripherals` or :obj:`int`): Embedded peripheral.
+
         Raises:
             ValueError: If peripheral value is less than 0 or greater than 31.
         """
         if not (0 <= peripheral <= 31):
             raise ValueError('Peripheral value should be between 0 and 31')
         if peripheral not in self._embedded_peripherals:
             self._embedded_peripherals.append(peripheral)
 
     def disable_embedded_peripheral(self, peripheral: Union[EmbedPeripherals, int]) -> None:
         """Disables embedded peripheral.
 
         Args:
             peripheral (:obj:`EmbeddedPeripherals` or :obj:`int`): Embedded peripheral.
+
         Raises:
             ValueError: If peripheral value is less than 0 or greater than 31.
         """
         if not (0 <= peripheral <= 31):
             raise ValueError('Peripheral value should be between 0 and 31')
         if peripheral in self._embedded_peripherals:
             self._embedded_peripherals.remove(peripheral)
 
     def get_embedded_peripheral_byte(self, peripheral: Union[EmbedPeripherals, int]) -> OsTrConfByte:
         """Returns embedded peripheral configuration byte.
 
         Args:
             peripheral (:obj:`EmbeddedPeripherals` or :obj:`int`): Embedded peripheral.
+
         Raises:
             ValueError: If peripheral value is less than 0 or greater than 31.
+
         Returns:
             :obj:`OsTrConfByte`: Embedded peripheral configuration byte.
         """
         if not (0 <= peripheral <= 31):
             raise ValueError('Peripheral value should be between 0 and 31')
         if 0 <= peripheral <= 7:
             address = 1
@@ -218,22 +233,22 @@
 
         Getter and setter.
         """
         return self._dpa_peer_to_peer
 
     @dpa_peer_to_peer.setter
     def dpa_peer_to_peer(self, value: bool):
-        """Returns DPA peer-to-peer configuration byte.
+        self._dpa_peer_to_peer = value
+
+    def get_dpa_peer_to_peer_byte(self) -> OsTrConfByte:
+        """Return DPA peer-to-peer configuration byte.
 
         Returns:
             :obj:`OsTrConfByte`: DPA peer-to-peer configuration byte.
         """
-        self._dpa_peer_to_peer = value
-
-    def get_dpa_peer_to_peer_byte(self) -> OsTrConfByte:
         return OsTrConfByte(
             address=TrConfByteAddrs.DPA_CONFIG_BITS_0,
             value=2 if self._dpa_peer_to_peer else 0,
             mask=TrConfBitMasks.DPA_PEER_TO_PEER
         )
 
     @property
@@ -358,14 +373,15 @@
 
     @staticmethod
     def _validate_rf_output_power(rf_output_power: int) -> None:
         """Validate rf output power parameter.
 
         Args:
             rf_output_power (int): RF output power.
+
         Raises:
             RequestParameterInvalidValueError: If rf_output_power is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= rf_output_power <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('RF output power value should be between 0 and 255.')
 
     @property
@@ -395,14 +411,15 @@
 
     @staticmethod
     def _validate_rf_signal_filter(rf_signal_filter: int) -> None:
         """Validate rf signal filter parameter.
 
         Args:
             rf_signal_filter (int): RF signal filter.
+
         Raises:
             RequestParameterInvalidValueError: If rf_signal_filter is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= rf_signal_filter <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('RF signal filter value should be between 0 and 255.')
 
     @property
@@ -432,14 +449,15 @@
 
     @staticmethod
     def _validate_lp_rf_timeout(lp_rf_timeout: int) -> None:
         """Validate lp rf timeout parameter.
 
         Args:
             lp_rf_timeout (int): LP RF timeout.
+
         Raises:
             RequestParameterInvalidValueError: If lp_rf_timeout is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= lp_rf_timeout <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('LP RF timeout value should be between 0 and 255.')
 
     @property
@@ -469,14 +487,15 @@
 
     @staticmethod
     def _validate_uart_baud_rate(uart_baud_rate: Union[dpa_constants.BaudRates, int]) -> None:
         """Validate uart baud rate parameter.
 
         Args:
             uart_baud_rate (Union[BaudRates, int]): UART Baud rate.
+
         Raises:
             RequestParameterInvalidValueError: If uart_baud_rate is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= uart_baud_rate <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('UART baud rate value should be between 0 and 255.')
 
     @property
@@ -506,14 +525,15 @@
 
     @staticmethod
     def _validate_alternative_dsm_channel(alternative_dsm_channels: int) -> None:
         """Validate alternative dsm channel parameters.
 
         Args:
             alternative_dsm_channels (int): Alternative DSM channel.
+
         Raises:
             RequestParameterInvalidValueError: If alternative_dsm_channels is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= alternative_dsm_channels <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Alternative DMS channel value should be between 0 and 255.')
 
     @property
@@ -567,14 +587,15 @@
 
     @staticmethod
     def _validate_rf_channel_a(rf_channel_a: int) -> None:
         """Validate RF Channel A Parameter.
 
         Args:
             rf_channel_a (int): RF Channel A.
+
         Raises:
             RequestParameterInvalidValueError: If rf_channel_a is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= rf_channel_a <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('RF channel A value should be between 0 and 255.')
 
     @property
@@ -604,14 +625,15 @@
 
     @staticmethod
     def _validate_rf_channel_b(rf_channel_b: int) -> None:
         """Validate RF Channel B Parameter.
 
         Args:
             rf_channel_b (int): RF Channel B.
+
         Raises:
             RequestParameterInvalidValueError: If rf_channel_b is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= rf_channel_b <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('RF channel B value should be between 0 and 255.')
 
     @property
@@ -641,14 +663,15 @@
 
     @staticmethod
     def _validate_reserved_block_0(data: List[int]) -> None:
         """Validate undocumented data bytes.
 
         Args:
             data (List[int]): Reserved data bytes.
+
         Raises:
             RequestParameterInvalidValueError: If data does not contain 2 values or if values are not
             in range from 0 to 255.
         """
         if len(data) != 2:
             raise RequestParameterInvalidValueError('Reserved block 0 should be 2B long.')
         if not Common.values_in_byte_range(data):
@@ -656,14 +679,15 @@
 
     @staticmethod
     def _validate_reserved_block_1(data: List[int]) -> None:
         """Validate undocumented data bytes.
 
         Args:
             data (List[int]): Reserved data bytes.
+
         Raises:
             RequestParameterInvalidValueError: If data does not contain 3 values or if values are not
             in range from 0 to 255.
         """
         if len(data) != 3:
             raise RequestParameterInvalidValueError('Reserved block 1 should be 3B long.')
         if not Common.values_in_byte_range(data):
@@ -671,14 +695,15 @@
 
     @staticmethod
     def _validate_reserved_block_2(data: List[int]) -> None:
         """Validate undocumented data bytes.
 
         Args:
             data (List[int]): Reserved data bytes.
+
         Raises:
             RequestParameterInvalidValueError: If data does not contain 13 values or if values are not
             in range from 0 to 255.
         """
         if len(data) != 13:
             raise RequestParameterInvalidValueError('Reserved block 2 should be 13B long.')
         if not Common.values_in_byte_range(data):
@@ -693,15 +718,15 @@
         """
         if isinstance(data, bytearray):
             data = list(data)
         embed_pers_data = data[0:4]
         embedded_pers = []
         for i in range(0, len(embed_pers_data * 8)):
             if embed_pers_data[int(i / 8)] & (1 << (i % 8)):
-                if EmbedPeripherals.has_value(i):
+                if i in EmbedPeripherals:
                     embedded_pers.append(EmbedPeripherals(i))
                 else:
                     embedded_pers.append(i)
         embedded_peripherals = embedded_pers
         custom_dpa_handler = bool(data[4] & 1)
         dpa_peer_to_peer = bool(data[4] & 2)
         routing_off = bool(data[4] & 8)
@@ -731,14 +756,15 @@
                    reserved_block_2=reserved_block_2)
 
     def to_pdata(self, to_bytes: bool = False) -> Union[List[int], bytearray]:
         """Serialize OS TR Configuration data object to DPA request pdata.
 
         Args:
             to_bytes (bool): Serialize into bytes.
+
         Returns:
             :obj:`list` of :obj:`int`: Serialized OS TR Configuration data.\n
             :obj:`bytearray`: Serialize OS TR Configuration data bytes if to_bytes is True.
         """
         embed_pers = Common.peripheral_list_to_bitmap(self.embedded_peripherals)
         conf_bits_0 = int(self.custom_dpa_handler) | int(self.dpa_peer_to_peer) << 1 | int(self.routing_off) << 3 | \
             int(self.io_setup) << 4 | int(self.user_peer_to_peer) << 5 | \
@@ -755,7 +781,22 @@
             [
                 self.rf_channel_a,
                 self.rf_channel_b
             ] + self._reserved_block_2
         if to_bytes:
             return bytearray(pdata)
         return pdata
+
+    @staticmethod
+    def calculate_checksum(data: List[int]) -> int:
+        """Calculates checksum from TR configuration data.
+
+        Args:
+            data (List[int]): List of integers representing TR configuration data.
+
+        Returns:
+            int: Checksum value.
+        """
+        checksum = 0x5F
+        for val in data:
+            checksum ^= val
+        return checksum
```

### Comparing `iqrfpy-0.2.0/iqrfpy/objects/sensor_data.py` & `iqrfpy-0.2.1/iqrfpy/objects/sensor_data.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/objects/sensor_written_data.py` & `iqrfpy-0.2.1/iqrfpy/objects/sensor_written_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
     @staticmethod
     def _validate_index(index: int):
         """Validate sensor index parameter.
 
         Args:
             index (int): Sensor index.
+
         Raises:
             RequestParameterInvalidValueError: If index is less than 0 or greater than 31.
         """
         if not dpa_constants.SENSOR_INDEX_MIN <= index <= dpa_constants.SENSOR_INDEX_MAX:
             raise RequestParameterInvalidValueError('Index value should be between 0 and 31.')
 
     @property
@@ -58,14 +59,15 @@
 
     @staticmethod
     def _validate_data(data: List[int]):
         """Validate data to write.
 
         Args:
             data (List[int]): Data to write.
+
         Raises:
             RequestParameterInvalidValueError: If data contains values not in range from 0 to 255.
         """
         if not Common.values_in_byte_range(data):
             raise RequestParameterInvalidValueError('Data values should be between 0 and 255.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/requests/enumerate.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/binaryoutput/requests/enumerate.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/requests/set_output.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/binaryoutput/requests/set_output.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/responses/enumerate.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/binaryoutput/responses/enumerate.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/responses/set_output.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/binaryoutput/responses/set_output.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/__init__.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/__init__.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/addr_info.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/addr_info.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/authorize_bond.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/authorize_bond.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
     @staticmethod
     def _validate_nodes(nodes: List[CoordinatorAuthorizeBondParams]) -> None:
         """Validates request parameters.
 
         Args:
             nodes (List[CoordinatorAuthorizeBondParams]): List of address-mid pairs.
+
         Raises:
             RequestParameterInvalidValueError: If length of nodes is 0 or greater than 11.
         """
         if len(nodes) == 0:
             raise RequestParameterInvalidValueError('At least one pair of requested address and MID is required.')
         if len(nodes) > 11:
             raise RequestParameterInvalidValueError('Request can carry at most 11 pairs of address and MID.')
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/backup.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/backup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 
     @staticmethod
     def _validate_index(index: int) -> None:
         """Validates index parameter.
 
         Args:
             index (int): Index of data block.
+
         Raises:
             RequestParameterInvalidValueError: If value is less than 0 or greater than 255.
         """
         if index < dpa_constants.BYTE_MIN or index > dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Index value should be between 0 and 255.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/bond_node.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/bond_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
     @staticmethod
     def _validate_req_addr(req_addr: int):
         """Validates requested address parameter.
 
         Args:
             req_addr (int): Requested node address.
+
         Raises:
             RequestParameterInvalidValueError: If req_addr is less than 0 or greater than 255.
         """
         if req_addr < dpa_constants.BYTE_MIN or req_addr > dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Address value should be between 0 and 255.')
 
     @property
@@ -78,18 +79,19 @@
     @req_addr.setter
     def req_addr(self, value: int):
         self._validate_req_addr(value)
         self._req_addr = value
 
     @staticmethod
     def _validate_bonding_test_retries(bonding_test_retries: int):
-        """Validates bonding test retries parameter
+        """Validates bonding test retries parameter.
 
         Args:
             bonding_test_retries (int): Maximum number of FRCs used to test whether node was bonded.
+
         Raises:
             RequestParameterInvalidValueError: If bonding_test_retries is less than 0 or greater than 255.
         """
         if bonding_test_retries < dpa_constants.BYTE_MIN or bonding_test_retries > dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Bonding test retries value should be between 0 and 255.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/bonded_devices.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/bonded_devices.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/clear_all_bonds.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/clear_all_bonds.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/discovered_devices.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/discovered_devices.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/discovery.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/discovery.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """Coordinator Discovery request class."""
 
     __slots__ = '_tx_power', '_max_addr'
 
     def __init__(self, tx_power: int, max_addr: int, hwpid: int = dpa_constants.HWPID_MAX,
                  dpa_rsp_time: Optional[float] = None, dev_process_time: Optional[float] = None,
                  msgid: Optional[str] = None):
-        """Discovery request constructor
+        """Discovery request constructor.
 
         Args:
             tx_power (int): TX power used for discovery.
             max_addr (int): Maximum node address to be included in the discovery process, 0 means all nodes.
             hwpid (int, optional): Hardware profile ID. Defaults to 65535 (Ignore HWPID check).
             dpa_rsp_time (float, optional): DPA request timeout in seconds. Defaults to None.
             dev_process_time (float, optional): Device processing time. Defaults to None.
@@ -57,14 +57,15 @@
 
     @staticmethod
     def _validate_tx_power(tx_power: int):
         """Validate TX power parameter.
 
         Args:
             tx_power (int): TX power used for discovery.
+
         Raises:
             RequestParameterInvalidValueError: If tx_power is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= tx_power <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('TX power value should be between 0 and 255.')
 
     @property
@@ -82,14 +83,15 @@
 
     @staticmethod
     def _validate_max_addr(max_addr: int):
         """Validate maximum node address parameter.
 
         Args:
             max_addr (int): Maximum node address to be included in the discovery process, 0 means all nodes.
+
         Raises:
             RequestParameterInvalidValueError: If max_addr is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= max_addr <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Max address value should be between 0 and 255.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/remove_bond.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/remove_bond.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 
     @staticmethod
     def _validate(bond_addr: int) -> None:
         """Validates removed node address parameter.
 
         Args:
             bond_addr (int): Address of node device to remove from list of bonded nodes.
+
         Raises:
             RequestParameterInvalidValueError: If bond_addr is less than 0 or greater than 255.
         """
         if bond_addr < dpa_constants.BYTE_MIN or bond_addr > dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Bond address value should be between 0 and 255.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/restore.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/restore.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
     @staticmethod
     def _validate_network_data(network_data: List[int]):
         """Validates network data parameter.
 
         Args:
             network_data (List[int]): Block of Coordinator network info data obtained by Backup request.
+
         Raises:
             RequestParameterInvalidValueError: If network_data is longer than 49 bytes (values)
                 or the values are not between 0 and 255.
         """
         if len(network_data) > dpa_constants.BACKUP_DATA_BLOCK_MAX_LEN:
             raise RequestParameterInvalidValueError('Network data should be at most 49 bytes long.')
         if not Common.values_in_byte_range(network_data):
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/set_dpa_params.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/set_dpa_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
     @staticmethod
     def _validate_dpa_param(dpa_param: Union[CoordinatorDpaParam, int]):
         """Validates DPA param parameter.
 
         Args:
             dpa_param (Union[CoordinatorDpaParam, int]): DPA param to set.
+
         Raises:
             RequestParameterInvalidValueError: If dpa_param is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= dpa_param <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('DPA param value should be between 0 and 255.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/set_hops.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/set_hops.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
     @staticmethod
     def _validate_request_hops(request_hops: int):
         """Validates request hops parameter.
 
         Args:
             request_hops (int): Number of hops to send DPA request.
+
         Raises:
             RequestParameterInvalidValueError: If request_hops is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= request_hops <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Request hops value should be between 0 and 255.')
 
     @property
@@ -82,14 +83,15 @@
 
     @staticmethod
     def _validate_response_hops(response_hops: int):
         """Validates response hops parameter.
 
         Args:
             response_hops (int): Number of hops to send DPA response.
+
         Raises:
             RequestParameterInvalidValueError: If response_hops is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= response_hops <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Response hops value should be between 0 and 255.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/set_mid.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/set_mid.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
     @staticmethod
     def _validate_bond_addr(bond_addr: int):
         """Validates node address parameter.
 
         Args:
             bond_addr (int): Address of node device.
+
         Raises:
             RequestParameterInvalidValueError: If bond_addr is less than 0 or greater than 255.
         """
         if bond_addr < dpa_constants.BYTE_MIN or bond_addr > dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Bond address value should be between 0 and 255.')
 
     @property
@@ -82,14 +83,15 @@
 
     @staticmethod
     def _validate_mid(mid: int):
         """Validates MID parameter.
 
         Args:
             mid (int): MID to assign to a node in Coordinator's DB.
+
         Raises:
             RequestParameterInvalidValueError: If MID is less than 0 or greater than 4294967295.
         """
         if mid < dpa_constants.MID_MIN or mid > dpa_constants.MID_MAX:
             raise RequestParameterInvalidValueError('MID value should be between 0 and 4294967295.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/smart_connect.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/requests/smart_connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 
     @staticmethod
     def _validate_req_addr(req_addr: int):
         """Validates requested address parameter.
 
         Args:
             req_addr (int): Requested node address.
+
         Raises:
             RequestParameterInvalidValueError: If req_addr is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= req_addr <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Requested address should be between 0 and 255.')
 
     @property
@@ -96,14 +97,15 @@
 
     @staticmethod
     def _validate_bonding_test_retries(bonding_test_retries: int):
         """Validates bonding test retries parameter.
 
         Args:
             bonding_test_retries (int): Maximum number of FRCs used to test whether node was bonded.
+
         Raises:
             RequestParameterInvalidValueError: If bonding_test_retries is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= bonding_test_retries <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Bonding test retries should be between 0 and 255.')
 
     @property
@@ -121,14 +123,15 @@
 
     @staticmethod
     def _validate_ibk(ibk: List[int]):
         """Validates individual bonding key parameter.
 
         Args:
             ibk (List[int]): Individual bonding key of node devices.
+
         Raises:
             RequestParameterInvalidValueError: If ibk is not 16 values long or if ibk values are not between 0 and 255.
         """
         if len(ibk) != dpa_constants.IBK_LEN:
             raise RequestParameterInvalidValueError('IBK should be list of 16 8bit unsigned integers.')
         if not Common.values_in_byte_range(ibk):
             raise RequestParameterInvalidValueError('IBK list should only contain values between 0 and 255.')
@@ -148,14 +151,15 @@
 
     @staticmethod
     def _validate_mid(mid: int):
         """Validates MID parameter.
 
         Args:
             mid (int): MID of node device.
+
         Raises:
             RequestParameterInvalidValueError: If MID is less than 0 or greater than 4294967295.
         """
         if not dpa_constants.MID_MIN <= mid <= dpa_constants.MID_MAX:
             raise RequestParameterInvalidValueError('MID value should be between 0 and 4294967295.')
 
     @property
@@ -173,14 +177,15 @@
 
     @staticmethod
     def _validate_virtual_device_address(virtual_device_address: int):
         """Validates virtual device address parameter.
 
         Args:
             virtual_device_address (int): Virtual device address.
+
         Raises:
             RequestParameterInvalidValueError: If virtual_device_address is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= virtual_device_address <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Virtual device address should be between 0 and 255.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/__init__.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/addr_info.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/addr_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     def from_dpa(cls, dpa: bytes) -> 'AddrInfoResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs AddrInfoResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             AddrInfoResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         _, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -87,13 +88,14 @@
     def from_json(cls, json: dict) -> 'AddrInfoResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs AddrInfoResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             AddrInfoResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, _, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/authorize_bond.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/authorize_bond.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     def from_dpa(cls, dpa: bytes) -> 'AuthorizeBondResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs AuthorizeBondResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             AuthorizeBondResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         _, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -87,13 +88,14 @@
     def from_json(cls, json: dict) -> 'AuthorizeBondResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs AuthorizeBondResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             AuthorizeBondResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, _, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/backup.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/backup.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     def from_dpa(cls, dpa: bytes) -> 'BackupResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs BackupResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             BackupResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         _, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -76,13 +77,14 @@
     def from_json(cls, json: dict) -> 'BackupResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs BackupResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             BackupResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, _, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/bond_node.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/bond_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     def from_dpa(cls, dpa: bytes) -> 'BondNodeResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs BondNodeResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             BondNodeResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         _, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -87,13 +88,14 @@
     def from_json(cls, json: dict) -> 'BondNodeResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs BondNodeResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             BondNodeResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, _, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/bonded_devices.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/bonded_devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     def from_dpa(cls, dpa: bytes) -> 'BondedDevicesResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs BondedDevicesResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             BondedDevicesResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         _, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -76,13 +77,14 @@
     def from_json(cls, json: dict) -> 'BondedDevicesResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs BondedDevicesResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             BondedDevicesResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, _, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/clear_all_bonds.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/clear_all_bonds.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     def from_dpa(cls, dpa: bytes) -> 'ClearAllBondsResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs ClearAllBondsResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             ClearAllBondsResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         _, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -60,13 +61,14 @@
     def from_json(cls, json: dict) -> 'ClearAllBondsResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs ClearAllBondsResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             ClearAllBondsResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, _, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/discovered_devices.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/discovered_devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     def from_dpa(cls, dpa: bytes) -> 'DiscoveredDevicesResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs DiscoveredDevicesResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             DiscoveredDevicesResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         _, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -76,13 +77,14 @@
     def from_json(cls, json: dict) -> 'DiscoveredDevicesResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs DiscoveredDevicesResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             DiscoveredDevicesResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, _, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/discovery.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     def from_dpa(cls, dpa: bytes) -> 'DiscoveryResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs DiscoveryResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             DiscoveryResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         _, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -76,13 +77,14 @@
     def from_json(cls, json: dict) -> 'DiscoveryResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs DiscoveryResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             DiscoveryResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, _, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/remove_bond.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/remove_bond.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     def from_dpa(cls, dpa: bytes) -> 'RemoveBondResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs RemoveBondResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             RemoveBondResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         _, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -76,13 +77,14 @@
     def from_json(cls, json: dict) -> 'RemoveBondResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs RemoveBondResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             RemoveBondResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, _, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/restore.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/restore.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     def from_dpa(cls, dpa: bytes) -> 'RestoreResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs RestoreResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             RestoreResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         _, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -60,13 +61,14 @@
     def from_json(cls, json: dict) -> 'RestoreResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs RestoreResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             RestoreResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, _, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/set_dpa_params.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/set_dpa_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     def from_dpa(cls, dpa: bytes) -> 'SetDpaParamsResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs SetDpaParamsResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             SetDpaParamsResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         _, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -77,13 +78,14 @@
     def from_json(cls, json: dict) -> 'SetDpaParamsResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs SetDpaParamsResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             SetDpaParamsResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, _, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/set_hops.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/set_hops.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     def from_dpa(cls, dpa: bytes) -> 'SetHopsResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs AddrInfoResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             AddrInfoResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         _, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -87,13 +88,14 @@
     def from_json(cls, json: dict) -> 'SetHopsResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs AddrInfoResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             AddrInfoResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, _, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/set_mid.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/set_mid.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     def from_dpa(cls, dpa: bytes) -> 'SetMidResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs SetMidResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             SetMidResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         _, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -58,13 +59,14 @@
     def from_json(cls, json: dict) -> 'SetMidResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs SetMidResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             SetMidResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, _, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/smart_connect.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/coordinator/responses/smart_connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     def from_dpa(cls, dpa: bytes) -> 'SmartConnectResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs SmartConnectResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             SmartConnectResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         _, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -87,13 +88,14 @@
     def from_json(cls, json: dict) -> 'SmartConnectResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs SmartConnectResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             SmartConnectResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, _, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/requests/read.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/eeeprom/requests/read.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 
     @staticmethod
     def _validate_address(address: int):
         """Validate memory address parameter.
 
         Args:
             address (int): Memory address to read from.
+
         Raises:
             RequestParameterInvalidValueError: If address is less than 0 or greater than 255.
         """
         if not dpa_constants.WORD_MIN <= address <= dpa_constants.WORD_MAX:
             raise RequestParameterInvalidValueError('Address should be between 0 and 65535.')
 
     @property
@@ -83,14 +84,15 @@
 
     @staticmethod
     def _validate_length(length: int):
         """Validate data length parameter.
 
         Args:
             length (int): Number of bytes to read from memory.
+
         Raises:
             RequestParameterInvalidValueError: If length is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= length <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Length should be between 0 and 255.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/requests/write.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/eeeprom/requests/write.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 
     @staticmethod
     def _validate_data(data: List[int]):
         """Validate data parameter.
 
         Args:
             data (List[int]): Data to write to memory.
+
         Raises:
             RequestParameterInvalidValueError: If data contains more than 54 values or data values are not
                 in range from 0 to 255.
         """
         if len(data) > dpa_constants.EEEPROM_WRITE_MAX_DATA_LEN:
             raise RequestParameterInvalidValueError('Data should contain at most 54 values.')
         if not Common.values_in_byte_range(data):
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/responses/read.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/eeeprom/responses/read.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     def from_dpa(cls, dpa: bytes) -> 'ReadResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs ReadResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             ReadResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -76,13 +77,14 @@
     def from_json(cls, json: dict) -> 'ReadResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs ReadResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             ReadResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/responses/write.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/eeeprom/responses/write.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     def from_dpa(cls, dpa: bytes) -> 'WriteResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs WriteResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             WriteResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -61,13 +62,14 @@
     def from_json(cls, json: dict) -> 'WriteResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs WriteResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             WriteResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/requests/read.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/eeprom/requests/read.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 
     @staticmethod
     def _validate_address(address: int):
         """Validates memory address parameter.
 
         Args:
             address (int): Memory address to read from.
+
         Raises:
             RequestParameterInvalidValueError: If address is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= address <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Address should be between 0 and 255')
 
     @property
@@ -83,14 +84,15 @@
 
     @staticmethod
     def _validate_length(length: int):
         """Validates data length parameter.
 
         Args:
             length (int): Number of bytes to read from memory.
+
         Raises:
             RequestParameterInvalidValueError: If length is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= length <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Length should be between 0 and 255.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/requests/write.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/eeprom/requests/write.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 
     @staticmethod
     def _validate_data(data: List[int]):
         """Validate data parameter.
 
         Args:
             data (List[int]): Data to write to memory.
+
         Raises:
             RequestParameterInvalidValueError: If data contains more than 55 values or data values are not
                 in range from 0 to 255.
         """
         if len(data) > dpa_constants.EEPROM_WRITE_MAX_DATA_LEN:
             raise RequestParameterInvalidValueError('Data should contain at most 55 values.')
         if not Common.values_in_byte_range(data):
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/responses/read.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/eeprom/responses/read.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     def from_dpa(cls, dpa: bytes) -> 'ReadResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`ReadResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`ReadResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -76,13 +77,14 @@
     def from_json(cls, json: dict) -> 'ReadResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`ReadResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`ReadResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/responses/write.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/eeprom/responses/write.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     def from_dpa(cls, dpa: bytes) -> 'WriteResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`WriteResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`WriteResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -61,13 +62,14 @@
     def from_json(cls, json: dict) -> 'WriteResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`WriteResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`WriteResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/exploration/__init__.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/exploration/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/exploration/requests/more_peripherals_information.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/exploration/requests/more_peripherals_information.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     def __init__(self, nadr: int, per: Union[Peripheral, int], hwpid: int = dpa_constants.HWPID_MAX,
                  dpa_rsp_time: Optional[float] = None, dev_process_time: Optional[float] = None,
                  msgid: Optional[str] = None):
         """More Peripherals Information request constructor.
 
         Args:
             nadr (int): Device address.
+            per (Union[Peripheral, int]): Requested peripheral.
             hwpid (int, optional): Hardware profile ID. Defaults to 65535 (Ignore HWPID check).
             dpa_rsp_time (float, optional): DPA request timeout in seconds. Defaults to None.
             dev_process_time (float, optional): Device processing time. Defaults to None.
             msgid (str, optional): JSON API message ID. Defaults to None. If the parameter is not specified, a random
                 UUIDv4 string is generated and used.
         """
         super().__init__(
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/exploration/requests/peripheral_enumeration.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/exploration/requests/peripheral_enumeration.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/exploration/requests/peripheral_information.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/exploration/requests/peripheral_information.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/exploration/responses/__init__.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/exploration/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/exploration/responses/more_peripherals_information.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/exploration/responses/more_peripherals_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     def from_dpa(cls, dpa: bytes) -> 'MorePeripheralsInformationResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs MorePeripheralsInformationResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             MorePeripheralsInformationResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         per = ExplorationResponsePeripheralCommand(dpa[ResponsePacketMembers.PCMD])
@@ -95,14 +96,15 @@
     def from_json(cls, json: dict) -> 'MorePeripheralsInformationResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs MorePeripheralsInformationResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             MorePeripheralsInformationResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         per = Common.pcmd_from_json(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         if rcode < 0:
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/exploration/responses/peripheral_enumeration.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/exploration/responses/peripheral_enumeration.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     def from_dpa(cls, dpa: bytes) -> 'PeripheralEnumerationResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs PeripheralEnumerationResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             PeripheralEnumerationResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -83,15 +84,15 @@
                 'hwpidVer': (dpa[18] << 8) + dpa[17],
                 'flags': dpa[19],
                 'userPer': [],
             }
             embed_pers_data = list(dpa[11:14])
             embedded_pers = []
             for i in range(0, len(embed_pers_data * 8)):
-                if embed_pers_data[int(i / 8)] & (1 << (i % 8)) and EmbedPeripherals.has_value(i):
+                if embed_pers_data[int(i / 8)] & (1 << (i % 8)) and i in EmbedPeripherals:
                     embedded_pers.append(i)
             result['embeddedPers'] = embedded_pers
             if result['perNr'] > 0:
                 user_per_data = list(dpa[20:])
                 user_pers = []
                 for i in range(0, len(user_per_data * 8)):
                     if user_per_data[int(i / 8)] & (1 << (i % 8)):
@@ -103,13 +104,14 @@
     def from_json(cls, json: dict) -> 'PeripheralEnumerationResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs PeripheralEnumerationResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             PeripheralEnumerationResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/exploration/responses/peripheral_information.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/exploration/responses/peripheral_information.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     def from_dpa(cls, dpa: bytes) -> 'PeripheralInformationResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs PeripheralInformationResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             PeripheralInformationResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, pnum, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -88,14 +89,15 @@
     def from_json(cls, json: dict) -> 'PeripheralInformationResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs PeripheralInformationResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             PeripheralInformationResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         pnum = Common.pnum_from_json(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         if rcode < 0:
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/frc/__init__.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/frc/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/frc/requests/extra_result.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/frc/requests/extra_result.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/frc/requests/send.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/frc/requests/send.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 
     @staticmethod
     def _validate_frc_command(frc_command: int):
         """Validate FRC command parameter.
 
         Args:
             frc_command (int): FRC command (data to collect).
+
         Raises:
             RequestParameterInvalidValueError: If frc_command is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= frc_command <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('FRC command value should be between 0 and 255.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/frc/requests/send_selective.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/frc/requests/send_selective.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 
     @staticmethod
     def _validate_frc_command(frc_command: int):
         """Validate FRC command parameter.
 
         Args:
             frc_command (int): FRC command (data to collect).
+
         Raises:
             RequestParameterInvalidValueError: If frc_command is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= frc_command <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('FRC command value should be between 0 and 255.')
 
     @property
@@ -87,14 +88,15 @@
 
     @staticmethod
     def _validate_selected_nodes(selected_nodes: List[int]):
         """Validate selected nodes parameter.
 
         Args:
             selected_nodes (List[int]): Selected nodes.
+
         Raises:
             RequestParameterInvalidValueError: If selected_nodes contains more than 240 values or values are not
             in range from 0 to 255.
         """
         if len(selected_nodes) > 240:
             raise RequestParameterInvalidValueError('Selected nodes should contain at most 240 values.')
         if min(selected_nodes) < 0 or max(selected_nodes) > 239:
@@ -115,14 +117,15 @@
 
     @staticmethod
     def _validate_user_data(user_data: List[int]):
         """Validate user data.
 
         Args:
             user_data (List[int]): User data (see FRC commands for details).
+
         Raises:
             RequestParameterInvalidValueError: If user_data contains more than 27 values or values are not
             in range from 0 to 255.
         """
         if len(user_data) > 27:
             raise RequestParameterInvalidValueError('User data should contain at most 27 values.')
         if not Common.values_in_byte_range(user_data):
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/frc/requests/set_frc_params.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/frc/requests/set_frc_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
     @staticmethod
     def _validate(frc_params: Union[FrcParams, int]):
         """Validate FRC params parameter.
 
         Args:
             frc_params (Union[FrcParams, int]): FRC parameters.
+
         Raises:
             RequestParameterInvalidValueError: If frc_params is less than 0 or greater than 255.
         """
         if isinstance(frc_params, int) and not dpa_constants.BYTE_MIN <= frc_params <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('FRC params value should be between 0 and 255.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/frc/responses/extra_result.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/frc/responses/extra_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     def from_dpa(cls, dpa: bytes) -> 'ExtraResultResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs ExtraResultResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             ExtraResultResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -77,13 +78,14 @@
     def from_json(cls, json: dict) -> 'ExtraResultResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs ExtraResultResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             ExtraResultResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(msgid=msgid, nadr=nadr, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/frc/responses/send.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/frc/responses/send.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     def from_dpa(cls, dpa: bytes) -> 'SendResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs SendResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             SendResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -88,13 +89,14 @@
     def from_json(cls, json: dict) -> 'SendResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs SendResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             SendResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(msgid=msgid, nadr=nadr, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/frc/responses/send_selective.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/frc/responses/send_selective.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     def from_dpa(cls, dpa: bytes) -> 'SendSelectiveResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs SendSelectiveResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             SendSelectiveResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -88,13 +89,14 @@
     def from_json(cls, json: dict) -> 'SendSelectiveResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs SendSelectiveResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             SendSelectiveResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(msgid=msgid, nadr=nadr, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/frc/responses/set_frc_params.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/frc/responses/set_frc_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
         Args:
             nadr (int): Device address.
             hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
             rcode (int, optional): Response code. Defaults to 128.
             dpa_value (int, optional): DPA value. Defaults to 0.
             msgid (str, optional): Message ID. Defaults to None.
+            pdata (List[int], optional): Raw PDATA. Defaults to None.
             result (dict, optional): JSON response data. Defaults to None.
         """
         super().__init__(
             nadr=nadr,
             pnum=EmbedPeripherals.FRC,
             pcmd=FrcResponseCommands.SET_PARAMS,
             m_type=FrcMessages.SET_PARAMS,
@@ -59,14 +60,15 @@
     def from_dpa(cls, dpa: bytes) -> 'SetFrcParamsResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs SetFrcParamsResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             SetFrcParamsResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -78,13 +80,14 @@
     def from_json(cls, json: dict) -> 'SetFrcParamsResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs SetFrcParamsResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             SetFrcParamsResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(msgid=msgid, nadr=nadr, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/generic/requests/generic.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/generic/requests/generic.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/generic/responses/generic.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/generic/responses/generic.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,20 @@
     def __init__(self, nadr: int, pnum: Union[Peripheral, int], pcmd: Union[Command, int],
                  hwpid: int = dpa_constants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  pdata: Optional[List[int]] = None, msgid: Optional[str] = None):
         """Generic response constructor.
 
         Args:
             nadr (int): Device address.
+            pnum (Union[Peripheral, int]): Peripheral number.
+            pcmd (pcmd: Union[Command, int]): Peripheral command.
             hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
             rcode (int, optional): Response code. Defaults to 128.
             dpa_value (int, optional): DPA value. Defaults to 0.
+            pdata (List[int], optional): Raw PDATA. Defaults to None.
             msgid (str, optional): Message ID. Defaults to None.
         """
         super().__init__(
             nadr=nadr,
             pnum=pnum,
             pcmd=pcmd,
             m_type=GenericMessages.RAW,
@@ -43,14 +46,15 @@
     def from_dpa(cls, dpa: bytes) -> 'GenericResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs GenericResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             GenericResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, pnum, pcmd, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, pnum=pnum, pcmd=pcmd, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, pdata=pdata)
 
@@ -58,14 +62,15 @@
     def from_json(cls, json: dict) -> 'GenericResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs GenericResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             GenericResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid = Common.msgid_from_json(json=json)
         raw = [int(x, 16) for x in Common.generic_rdata_from_json(json=json).split('.')]
         nadr = raw[ResponsePacketMembers.NADR]
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/io/requests/direction.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/io/requests/direction.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
     @staticmethod
     def _validate_triplets(triplets: List[IoTriplet]):
         """Validate IO subcommands triplets parameter.
 
         Args:
             triplets (List[IoTriplet]): List of port, mask and value subcommands triplets.
+
         Raises:
             RequestParameterInvalidValueError: If list contains more than 18 triplets.
         """
         if len(triplets) > 18:
             raise RequestParameterInvalidValueError('Request can carry at most 18 triplets.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/io/requests/get.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/io/requests/get.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/io/requests/set.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/io/requests/set.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
     @staticmethod
     def _validate_triplets(triplets: List[IoTriplet]):
         """Validate IO subcommands triplets parameter.
 
         Args:
             triplets (List[IoTriplet]): List of port, mask and value subcommands triplets.
+
         Raises:
             RequestParameterInvalidValueError: If list contains more than 18 triplets.
         """
         if len(triplets) > 18:
             raise RequestParameterInvalidValueError('Request can carry at most 18 triplets.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/io/responses/direction.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/io/responses/direction.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     def from_dpa(cls, dpa: bytes) -> 'DirectionResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs DirectionResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             DirectionResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -61,13 +62,14 @@
     def from_json(cls, json: dict) -> 'DirectionResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs DirectionResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             DirectionResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/io/responses/get.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/io/responses/get.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     def from_dpa(cls, dpa: bytes) -> 'GetResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs GetResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             GetResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -76,13 +77,14 @@
     def from_json(cls, json: dict) -> 'GetResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs GetResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             GetResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/io/responses/set.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/io/responses/set.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     def from_dpa(cls, dpa: bytes) -> 'SetResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs SetResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             SetResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -61,13 +62,14 @@
     def from_json(cls, json: dict) -> 'SetResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs SetResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             SetResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ledg/requests/flashing.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ledg/requests/flashing.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ledg/requests/pulse.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ledg/requests/pulse.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ledg/requests/set_off.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ledg/requests/set_off.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ledg/requests/set_on.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ledg/requests/set_on.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ledg/responses/flashing.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ledg/responses/flashing.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     def from_dpa(cls, dpa: bytes) -> 'FlashingResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs FlashingResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             FlashingResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -57,13 +58,14 @@
     def from_json(cls, json: dict) -> 'FlashingResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs FlashingResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             FlashingResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ledg/responses/pulse.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ledg/responses/pulse.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     def from_dpa(cls, dpa: bytes) -> 'PulseResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs PulseResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             PulseResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -57,13 +58,14 @@
     def from_json(cls, json: dict) -> 'PulseResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs PulseResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             PulseResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ledg/responses/set_off.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ledg/responses/set_off.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     def from_dpa(cls, dpa: bytes) -> 'SetOffResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs SetOffResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             SetOffResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -57,13 +58,14 @@
     def from_json(cls, json: dict) -> 'SetOffResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs SetOffResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             SetOffResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ledg/responses/set_on.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ledg/responses/set_on.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     def from_dpa(cls, dpa: bytes) -> 'SetOnResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs SetOnResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             SetOnResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -57,13 +58,14 @@
     def from_json(cls, json: dict) -> 'SetOnResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs SetOnResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             SetOnResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ledr/requests/flashing.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ledr/requests/flashing.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ledr/requests/pulse.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ledr/requests/pulse.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ledr/requests/set_off.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ledr/requests/set_off.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ledr/requests/set_on.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ledr/requests/set_on.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ledr/responses/flashing.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ledr/responses/flashing.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     def from_dpa(cls, dpa: bytes) -> 'FlashingResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs FlashingResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             FlashingResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -57,13 +58,14 @@
     def from_json(cls, json: dict) -> 'FlashingResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs FlashingResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             FlashingResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ledr/responses/pulse.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ledr/responses/pulse.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     def from_dpa(cls, dpa: bytes) -> 'PulseResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs PulseResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             PulseResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -57,13 +58,14 @@
     def from_json(cls, json: dict) -> 'PulseResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs PulseResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             PulseResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ledr/responses/set_off.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ledr/responses/set_off.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     def from_dpa(cls, dpa: bytes) -> 'SetOffResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs SetOffResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             SetOffResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -57,13 +58,14 @@
     def from_json(cls, json: dict) -> 'SetOffResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs SetOffResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             SetOffResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ledr/responses/set_on.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ledr/responses/set_on.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     def from_dpa(cls, dpa: bytes) -> 'SetOnResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs SetOnResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             SetOnResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -57,13 +58,14 @@
     def from_json(cls, json: dict) -> 'SetOnResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs SetOnResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             SetOnResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/node/__init__.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/node/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/node/requests/backup.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/node/requests/backup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
     @staticmethod
     def _validate(index: int) -> None:
         """Validate data block index parameter.
 
         Args:
             index (int): Data block index.
+
         Raises:
             RequestParameterInvalidValueError: If index is less than 0 or greater than 255.
         """
         if index < dpa_constants.BYTE_MIN or index > dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Index value should be between 0 and 255.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/node/requests/read.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/node/requests/read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/node/requests/remove_bond.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/node/requests/remove_bond.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/node/requests/restore.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/node/requests/restore.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
     @staticmethod
     def _validate(backup_data: List[int]):
         """Validate backup data.
 
         Args:
             backup_data (List[int]): Backup data.
+
         Raises:
             RequestParameterInvalidValueError: If backup_data is longer than 49 values or values are not
                 in range from 0 to 255.
         """
         if len(backup_data) > dpa_constants.BACKUP_DATA_BLOCK_MAX_LEN:
             raise RequestParameterInvalidValueError('Backup data should be at most 49 bytes long.')
         if not Common.values_in_byte_range(backup_data):
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/node/requests/validate_bonds.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/node/requests/validate_bonds.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
     @staticmethod
     def _validate(nodes: List[NodeValidateBondsParams]) -> None:
         """Validate nodes parameter.
 
         Args:
             nodes (List[NodeValidateBondsParams]): List of node and mid pairs.
+
         Raises:
             RequestParameterInvalidValueError: If length of nodes is 0 or greater than 11.
         """
         if len(nodes) == 0:
             raise RequestParameterInvalidValueError('At least one pair of address and MID is required.')
         if len(nodes) > 11:
             raise RequestParameterInvalidValueError('Request can carry at most 11 pairs of address and MID.')
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/backup.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/node/responses/backup.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     def from_dpa(cls, dpa: bytes) -> 'BackupResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs BackupResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             BackupResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -77,13 +78,14 @@
     def from_json(cls, json: dict) -> 'BackupResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs BackupResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             BackupResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/read.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/node/responses/read.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     def from_dpa(cls, dpa: bytes) -> 'ReadResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs ReadResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             ReadResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == 0:
@@ -92,13 +93,14 @@
     def from_json(cls, json: dict) -> 'ReadResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs ReadResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             ReadResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/remove_bond.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/node/responses/remove_bond.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     def from_dpa(cls, dpa: bytes) -> 'RemoveBondResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs RemoveBondResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             RemoveBondResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -59,13 +60,14 @@
     def from_json(cls, json: dict) -> 'RemoveBondResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs RemoveBondResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             RemoveBondResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/restore.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/node/responses/restore.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     def from_dpa(cls, dpa: bytes) -> 'RestoreResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs RestoreResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             RestoreResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -61,13 +62,14 @@
     def from_json(cls, json: dict) -> 'RestoreResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs RestoreResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             RestoreResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/validate_bonds.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/node/responses/validate_bonds.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     def from_dpa(cls, dpa: bytes) -> 'ValidateBondsResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs ValidateBondsResponse object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             ValidateBondsResponse: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -61,13 +62,14 @@
     def from_json(cls, json: dict) -> 'ValidateBondsResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs ValidateBondsResponse object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             ValidateBondsResponse: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/__init__.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/__init__.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/batch.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/batch.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/factory_settings.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/factory_settings.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/indicate.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/indicate.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/load_code.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/load_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 
     @staticmethod
     def _validate_flags(flags: Union[OsLoadCodeFlags, int]):
         """Validate flags parameter.
 
         Args:
             flags (Union[LoadCodeFlags, int]): Load code flags.
+
         Raises:
             RequestParameterInvalidValueError: If flags is less than 0 or greater than 255.
         """
         if isinstance(flags, OsLoadCodeFlags):
             return
         if not dpa_constants.BYTE_MIN <= flags <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Flags value should be between 0 and 255.')
@@ -97,14 +98,15 @@
 
     @staticmethod
     def _validate_address(address: int):
         """Validate address parameter.
 
         Args:
             address (int): EEEPROM address to load code from.
+
         Raises:
             RequestParameterInvalidValueError: If address is less than 0 or greater than 65535.
         """
         if not dpa_constants.WORD_MIN <= address <= dpa_constants.WORD_MAX:
             raise RequestParameterInvalidValueError('Address value should be between 0 and 65535.')
 
     @property
@@ -122,14 +124,15 @@
 
     @staticmethod
     def _validate_length(length: int):
         """Validate length parameter.
 
         Args:
             length (int): EEEPROM address to load code from.
+
         Raises:
             RequestParameterInvalidValueError: If length is less than 0 or greater than 65535.
         """
         if not dpa_constants.WORD_MIN <= length <= dpa_constants.WORD_MAX:
             raise RequestParameterInvalidValueError('Length value should be between 0 and 65535.')
 
     @property
@@ -147,14 +150,15 @@
 
     @staticmethod
     def _validate_checksum(checksum: int):
         """Validate address parameter.
 
         Args:
             checksum (int): Fletcher-16 checksum of the code to load.
+
         Raises:
             RequestParameterInvalidValueError: If checksum is less than 0 or greater than 65535.
         """
         if not dpa_constants.WORD_MIN <= checksum <= dpa_constants.WORD_MAX:
             raise RequestParameterInvalidValueError('Checksum value should be between 0 and 65535.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/read.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/read_tr_conf.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/read_tr_conf.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/reset.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/reset.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/restart.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/restart.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/rfpgm.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/rfpgm.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/selective_batch.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/selective_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 
     @staticmethod
     def _validate_selected_nodes(selected_nodes: List[int]):
         """Validate selected nodes parameter.
 
         Args:
             selected_nodes (List[int]): Selected nodes.
+
         Raises:
             RequestParameterInvalidValueError: If selected_nodes contains more than 240 values or values are not
             in range from 0 to 255.
         """
         if len(selected_nodes) > 240:
             raise RequestParameterInvalidValueError('Selected nodes should contain at most 240 values.')
         if min(selected_nodes) < 0 or max(selected_nodes) > 239:
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/set_security.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/set_security.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 
     @staticmethod
     def _validate_security_type(security_type: Union[OsSecurityTypeParam, int]):
         """Validate security type parameter.
 
         Args:
             security_type (Union[OsSecurityTypeParam, int]): Security type.
+
         Raises:
             RequestParameterInvalidValueError: If security_type is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= security_type <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Security type value should be between 0 and 255.')
 
     @property
@@ -87,14 +88,15 @@
 
     @staticmethod
     def _validate_data(data: List[int]):
         """Validate security data parameter.
 
         Args:
             data (List[int]): Security data.
+
         Raises:
             RequestParameterInvalidValueError: If data does not contain 16 values or if values are not
                 in range from 0 to 255.
         """
         if len(data) != 16:
             raise RequestParameterInvalidValueError('Data should be a list of 16 values.')
         if not Common.values_in_byte_range(data):
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/sleep.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/sleep.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/test_rf_signal.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/test_rf_signal.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/write_tr_conf.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/write_tr_conf.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/write_tr_conf_byte.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/requests/write_tr_conf_byte.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/__init__.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/batch.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     def from_dpa(cls, dpa: bytes) -> 'BatchResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`BatchResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`ResetResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -61,13 +62,14 @@
     def from_json(cls, json: dict) -> 'BatchResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`BatchResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`ResetResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/factory_settings.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/factory_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     def from_dpa(cls, dpa: bytes) -> 'FactorySettingsResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`FactorySettingsResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`FactorySettingsResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -61,13 +62,14 @@
     def from_json(cls, json: dict) -> 'FactorySettingsResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`FactorySettingsResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`FactorySettingsResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/indicate.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/indicate.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     def from_dpa(cls, dpa: bytes) -> 'IndicateResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`IndicateResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`IndicateResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -61,13 +62,14 @@
     def from_json(cls, json: dict) -> 'IndicateResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`IndicateResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`IndicateResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/load_code.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/load_code.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,26 +72,27 @@
 
         Returns:
             :obj:`OsLoadCodeErrors` or :obj:`None`: Load code error.
         """
         if self.get_load_result() is None:
             return None
         val = (self._load_result >> 1)
-        if OsLoadCodeErrors.has_value(val):
+        if val in OsLoadCodeErrors:
             return OsLoadCodeErrors(val)
         return OsLoadCodeErrors.RESERVED
 
     @classmethod
     def from_dpa(cls, dpa: bytes) -> 'LoadCodeResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`LoadCodeResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`LoadCodeResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -106,13 +107,14 @@
     def from_json(cls, json: dict) -> 'LoadCodeResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`LoadCodeResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`LoadCodeResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/read.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/read.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     def from_dpa(cls, dpa: bytes) -> 'ReadResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`ReadResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`ReadResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -92,15 +93,15 @@
                 'hwpidVer': (dpa[46] << 8) + dpa[45],
                 'flagsEnum': dpa[47],
                 'userPer': [],
             }
             embed_pers_data = list(dpa[39:43])
             embedded_pers = []
             for i in range(0, len(embed_pers_data * 8)):
-                if embed_pers_data[int(i / 8)] & (1 << (i % 8)) and EmbedPeripherals.has_value(i):
+                if embed_pers_data[int(i / 8)] & (1 << (i % 8)) and i in EmbedPeripherals:
                     embedded_pers.append(i)
             result['embeddedPers'] = embedded_pers
             if result['perNr'] > 0:
                 user_per_data = list(dpa[48:])
                 user_pers = []
                 for i in range(0, len(user_per_data * 8)):
                     if user_per_data[int(i / 8)] & (1 << (i % 8)):
@@ -112,13 +113,14 @@
     def from_json(cls, json: dict) -> 'ReadResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`ReadResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`ReadResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/read_tr_conf.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/read_tr_conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """OS Read TR Configuration response message."""
 
 from typing import List, Optional
 from iqrfpy.iresponse import IResponseGetterMixin
 from iqrfpy.enums.commands import OSResponseCommands
 from iqrfpy.enums.message_types import OSMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.objects.init_phy_data import InitPhyData
 from iqrfpy.objects.os_tr_conf_data import OsTrConfData
 from iqrfpy.utils import dpa as dpa_constants
 from iqrfpy.utils.dpa import ResponseCodes
 from iqrfpy.utils.common import Common
 from iqrfpy.utils.validators import DpaValidator, JsonValidator
 
 __all__ = [
@@ -48,15 +49,15 @@
             result=result
         )
         self._checksum = self._configuration = self._rfpgm = self._init_phy = None
         if rcode == ResponseCodes.OK:
             self._checksum = result['checksum']
             self._configuration = OsTrConfData.from_pdata(result['configuration'])
             self._rfpgm = result['rfpgm']
-            self._init_phy = result['initphy']
+            self._init_phy = InitPhyData(result['initphy'])
 
     @property
     def checksum(self) -> Optional[int]:
         """:obj:`int` :obj:`None`: Checksum.
 
         Getter only.
         """
@@ -75,29 +76,30 @@
         """:obj:`int` :obj:`None`: RFPGM parameters.
 
         Getter only.
         """
         return self._rfpgm
 
     @property
-    def init_phy(self) -> Optional[int]:
-        """:obj:`int` :obj:`None`: InitPHY.
+    def init_phy(self) -> InitPhyData:
+        """:obj:`InitPhyData`: InitPHY data.
 
         Getter only.
         """
         return self._init_phy
 
     @classmethod
     def from_dpa(cls, dpa: bytes) -> 'ReadTrConfResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`ReadTrConfResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`ReadTrConfResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -115,13 +117,14 @@
     def from_json(cls, json: dict) -> 'ReadTrConfResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`ReadTrConfResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`ReadTrConfResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/reset.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/reset.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     def from_dpa(cls, dpa: bytes) -> 'ResetResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`ResetResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`ResetResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -61,13 +62,14 @@
     def from_json(cls, json: dict) -> 'ResetResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`ResetResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`ResetResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/restart.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/restart.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     def from_dpa(cls, dpa: bytes) -> 'RestartResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`RestartResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`RestartResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -61,13 +62,14 @@
     def from_json(cls, json: dict) -> 'RestartResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`RestartResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`RestartResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/rfpgm.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/rfpgm.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     def from_dpa(cls, dpa: bytes) -> 'RfpgmResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`RfpgmResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`RfpgmResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -59,13 +60,14 @@
     def from_json(cls, json: dict) -> 'RfpgmResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`RfpgmResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`RfpgmResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/selective_batch.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/selective_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     def from_dpa(cls, dpa: bytes) -> 'SelectiveBatchResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`SelectiveBatchResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`SelectiveBatchResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -61,13 +62,14 @@
     def from_json(cls, json: dict) -> 'SelectiveBatchResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`SelectiveBatchResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`SelectiveBatchResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/set_security.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/set_security.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     def from_dpa(cls, dpa: bytes) -> 'SetSecurityResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`SetSecurityResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`SetSecurityResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -59,13 +60,14 @@
     def from_json(cls, json: dict) -> 'SetSecurityResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`SetSecurityResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`SetSecurityResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/sleep.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/sleep.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     def from_dpa(cls, dpa: bytes) -> 'SleepResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`SleepResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`SleepResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -59,13 +60,14 @@
     def from_json(cls, json: dict) -> 'SleepResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`SleepResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`SleepResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/test_rf_signal.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/test_rf_signal.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/write_tr_conf.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/write_tr_conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     def from_dpa(cls, dpa: bytes) -> 'WriteTrConfResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`WriteTrConfResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`WriteTrConfResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -61,13 +62,14 @@
     def from_json(cls, json: dict) -> 'WriteTrConfResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`WriteTrConfResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`WriteTrConfResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/write_tr_conf_byte.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/os/responses/write_tr_conf_byte.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     def from_dpa(cls, dpa: bytes) -> 'WriteTrConfByteResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`WriteTrConfByteResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`WriteTrConfByteResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -61,13 +62,14 @@
     def from_json(cls, json: dict) -> 'WriteTrConfByteResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`WriteTrConfByteResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`WriteTrConfByteResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ram/requests/read.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ram/requests/read.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 
     @staticmethod
     def _validate_address(address: int):
         """Validates memory address parameter.
 
         Args:
             address (int): Memory address to read from.
+
         Raises:
             RequestParameterInvalidValueError: If address is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= address <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Address should be between 0 and 255')
 
     @property
@@ -83,14 +84,15 @@
 
     @staticmethod
     def _validate_length(length: int):
         """Validates data length parameter.
 
         Args:
             length (int): Number of bytes to read from memory.
+
         Raises:
             RequestParameterInvalidValueError: If length is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= length <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Length should be between 0 and 255.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ram/requests/read_any.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ram/requests/read_any.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
     @staticmethod
     def _validate_address(address: int):
         """Validates memory address parameter.
 
         Args:
             address (int): Memory address to read from.
+
         Raises:
             RequestParameterInvalidValueError: If address is less than 0 or greater than 65535.
         """
         if not dpa_constants.WORD_MIN <= address <= dpa_constants.WORD_MAX:
             raise RequestParameterInvalidValueError('Address should be between 0 and 65535.')
 
     @property
@@ -82,14 +83,15 @@
 
     @staticmethod
     def _validate_length(length: int):
         """Validates data length parameter.
 
         Args:
             length (int): Number of bytes to read from memory.
+
         Raises:
             RequestParameterInvalidValueError: If length is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= length <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Length should be between 0 and 255.')
 
     @property
@@ -123,11 +125,12 @@
     def to_json(self) -> dict:
         """JSON API request serialization method.
 
         This method is not implemented as the message type is not supported by Daemon.
 
         Returns:
             :obj:`dict`: JSON API request object.
+
         Raises:
             NotImplementedError: ReadAny message type not implemented.
         """
         raise NotImplementedError('ReadAny JSON API request not implemented.')
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ram/requests/write.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ram/requests/write.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 
     @staticmethod
     def _validate_data(data: List[int]):
         """Validate data parameter.
 
         Args:
             data (List[int]): Data to write to memory.
+
         Raises:
             RequestParameterInvalidValueError: If data contains more than 48 values or data values are not
                 in range from 0 to 255.
         """
         if len(data) > dpa_constants.RAM_WRITE_MAX_DATA_LEN:
             raise RequestParameterInvalidValueError('Data should contain at most 55 values.')
         if not Common.values_in_byte_range(data):
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ram/responses/read.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ram/responses/read.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     def from_dpa(cls, dpa: bytes) -> 'ReadResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`ReadResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`ReadResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -76,14 +77,15 @@
     def from_json(cls, json: dict) -> 'ReadResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`ReadResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`ReadResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, pdata=pdata,
                    result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ram/responses/read_any.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ram/responses/read_any.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     def from_dpa(cls, dpa: bytes) -> 'ReadAnyResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`ReadAnyResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`ReadAnyResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -76,13 +77,15 @@
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`ReadAnyResponse` object.
         This method is not implemented as the message type is not supported by Daemon.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`ReadAnyResponse`: Response message object.
+
         Raises:
             NotImplementedError: ReadAny message type not implemented.
         """
         raise NotImplementedError('ReadAny JSON API request not implemented.')
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/ram/responses/write.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/ram/responses/write.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     def from_dpa(cls, dpa: bytes) -> 'WriteResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`WriteResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`WriteResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -61,13 +62,14 @@
     def from_json(cls, json: dict) -> 'WriteResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`WriteResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`WriteResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/sensor/__init__.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/sensor/requests/enumerate.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/sensor/requests/enumerate.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/sensor/requests/read_sensors.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/sensor/requests/read_sensors.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
     @staticmethod
     def _validate_sensors(sensors: Optional[List[int]] = None):
         """Validate sensors parameter.
 
         Args:
             sensors (List[int], optional): List of sensor indexes to read. If left empty, only the first sensor is read.
+
         Raises:
             RequestParameterInvalidValueError: If sensors contains more than 32 values or if values are not
                 in range from 0 to 31.
         """
         if sensors is not None:
             if len(sensors) == 0:
                 return
@@ -67,15 +68,16 @@
                 raise RequestParameterInvalidValueError('Sensors length should be at most 32 values.')
             if min(sensors) < 0 or max(sensors) > 31:
                 raise RequestParameterInvalidValueError('Sensors values should be between 0 and 31.')
 
     @property
     def sensors(self) -> Optional[List[int]]:
         """:obj:`list` of :obj:`int` or :obj:`None`: List of sensor indexes to read.
-            If left empty, only the first sensor is read.
+
+        If left empty, only the first sensor is read.
 
         Getter and setter.
         """
         return self._sensors
 
     @sensors.setter
     def sensors(self, value: Optional[List[int]] = None):
@@ -117,11 +119,12 @@
                                        pdata=self._pdata, mutable=mutable)
 
     def to_json(self) -> dict:
         """JSON API request serialization method.
 
         Returns:
             :obj:`dict`: JSON API request object.
+
         Raises:
             NotImplementedError: Message type not implemented.
         """
         raise NotImplementedError('JSON API request not implemented.')
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/sensor/requests/read_sensors_with_types.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/sensor/requests/read_sensors_with_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
     @staticmethod
     def _validate_sensors(sensors: Optional[List[int]] = None):
         """Validate sensors parameter.
 
         Args:
             sensors (List[int], optional): List of sensor indexes to read. If left empty, only the first sensor is read.
+
         Raises:
             RequestParameterInvalidValueError: If sensors contains more than 32 values or if values are not
                 in range from 0 to 31.
         """
         if sensors is not None:
             if len(sensors) == 0:
                 return
@@ -68,15 +69,16 @@
                 raise RequestParameterInvalidValueError('Sensors length should be at most 32 bytes.')
             if min(sensors) < 0 or max(sensors) > 31:
                 raise RequestParameterInvalidValueError('Sensors values should be between 0 and 31.')
 
     @property
     def sensors(self) -> Optional[List[int]]:
         """:obj:`list` of :obj:`int` or :obj:`None`: List of sensor indexes to read.
-            If left empty, only the first sensor is read.
+
+        If left empty, only the first sensor is read.
 
         Getter and setter.
         """
         return self._sensors
 
     @sensors.setter
     def sensors(self, value: Optional[List[int]] = None):
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/sensor/responses/enumerate.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/sensor/responses/enumerate.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     def from_dpa(cls, dpa: bytes) -> 'EnumerateResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`EnumerateResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`EnumerateResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -78,14 +79,15 @@
     def from_json(cls, json: dict) -> 'EnumerateResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`EnumerateResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`EnumerateResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         if rcode == ResponseCodes.OK:
             result = {'sensors': SensorParser.enumerate_from_json(result['sensors'])}
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/sensor/responses/read_sensors.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/sensor/responses/read_sensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     def from_dpa(cls, dpa: bytes) -> 'ReadSensorsResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`ReadSensorsResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`ReadSensorsResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -75,13 +76,15 @@
     def from_json(cls, json: dict) -> 'ReadSensorsResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`ReadSensorsResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`ReadSensorsResponse`: Response message object.
+
         Raises:
             NotImplementedError: Message type not implemented.
         """
         raise NotImplementedError('JSON API response not implemented.')
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/sensor/responses/read_sensors_with_types.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/sensor/responses/read_sensors_with_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     def from_dpa(cls, dpa: bytes) -> 'ReadSensorsWithTypesResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`ReadSensorsWithTypesResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`ReadSensorsWithTypesResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -80,14 +81,15 @@
     def from_json(cls, json: dict) -> 'ReadSensorsWithTypesResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`ReadSensorsWithTypesResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`ReadSensorsWithTypesResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         if rcode == ResponseCodes.OK:
             result = {'sensors': SensorParser.read_sensors_with_types_from_json(result['sensors'])}
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/thermometer/requests/read.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/thermometer/requests/read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/thermometer/responses/read.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/thermometer/responses/read.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     def from_dpa(cls, dpa: bytes) -> 'ReadResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`ReadResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`ReadResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -82,13 +83,14 @@
     def from_json(cls, json: dict) -> 'ReadResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`ReadResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`ReadResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/uart/__init__.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/uart/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/uart/requests/clear_write_read.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/uart/requests/clear_write_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 
     @staticmethod
     def _validate_read_timeout(read_timeout: int):
         """Validate read timeout parameter.
 
         Args:
             read_timeout (int): Timeout in 10ms unit to wait for data to be read. To read no data, use value 255.
+
         Raises:
             RequestParameterInvalidValueError: If read_timeout is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= read_timeout <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Read timeout value should be between 0 and 255.')
 
     @property
@@ -83,14 +84,15 @@
 
     @staticmethod
     def _validate_data(data: Optional[List[int]] = None):
         """Validate data parameter.
 
         Args:
             data (List[int], optional): Data to write to TX buffer.
+
         Raises:
             RequestParameterInvalidValueError: If data contains more than 57 values or if values are not
                 in range from 0 to 255.
         """
         if data is None:
             return
         if len(data) > 57:
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/uart/requests/close.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/uart/requests/close.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/uart/requests/open.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/uart/requests/open.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
     @staticmethod
     def _validate_baud_rate(baud_rate: Union[BaudRates, int]):
         """Validate baud rate parameter.
 
         Args:
             baud_rate (Union[BaudRates, int]): Baud rate.
+
         Raises:
             RequestParameterInvalidValueError: If baud_rate is less than 0 or greater than 255.
         """
         if not BYTE_MIN <= baud_rate <= BYTE_MAX:
             raise RequestParameterInvalidValueError('Baud rate value should be between 0 and 255.')
 
     @property
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/uart/requests/write_read.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/uart/requests/write_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 
     @staticmethod
     def _validate_read_timeout(read_timeout: int):
         """Validate read timeout parameter.
 
         Args:
             read_timeout (int): Timeout in 10ms unit to wait for data to be read. To read no data, use value 255.
+
         Raises:
             RequestParameterInvalidValueError: If read_timeout is less than 0 or greater than 255.
         """
         if not dpa_constants.BYTE_MIN <= read_timeout <= dpa_constants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Read timeout value should be between 0 and 255.')
 
     @property
@@ -83,14 +84,15 @@
 
     @staticmethod
     def _validate_data(data: Optional[List[int]] = None):
         """Validate data parameter.
 
         Args:
             data (List[int], optional): Data to write to TX buffer.
+
         Raises:
             RequestParameterInvalidValueError: If data contains more than 57 values or if values are not
                 in range from 0 to 255.
         """
         if data is None:
             return
         if len(data) > 57:
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/uart/responses/clear_write_read.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/uart/responses/clear_write_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     def from_dpa(cls, dpa: bytes) -> 'ClearWriteReadResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`ClearWriteReadResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`ClearWriteReadResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -74,13 +75,14 @@
     def from_json(cls, json: dict) -> 'ClearWriteReadResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`ClearWriteReadResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`ClearWriteReadResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/uart/responses/close.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/uart/responses/close.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     def from_dpa(cls, dpa: bytes) -> 'CloseResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`CloseResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`CloseResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -57,13 +58,14 @@
     def from_json(cls, json: dict) -> 'CloseResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`CloseResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`CloseResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/uart/responses/open.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/uart/responses/open.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     def from_dpa(cls, dpa: bytes) -> 'OpenResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`OpenResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`OpenResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         DpaValidator.response_length(dpa=dpa, expected_len=8)
         nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
         return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
@@ -57,13 +58,14 @@
     def from_json(cls, json: dict) -> 'OpenResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`OpenResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`OpenResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/peripherals/uart/responses/write_read.py` & `iqrfpy-0.2.1/iqrfpy/peripherals/uart/responses/write_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     def from_dpa(cls, dpa: bytes) -> 'WriteReadResponse':
         """DPA response factory method.
 
         Parses DPA data and constructs :obj:`WriteReadResponse` object.
 
         Args:
             dpa (bytes): DPA response bytes.
+
         Returns:
             :obj:`WriteReadResponse`: Response message object.
         """
         DpaValidator.base_response_length(dpa=dpa)
         nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
@@ -74,13 +75,14 @@
     def from_json(cls, json: dict) -> 'WriteReadResponse':
         """JSON response factory method.
 
         Parses JSON API response and constructs :obj:`WriteReadResponse` object.
 
         Args:
             json (dict): JSON API response.
+
         Returns:
             :obj:`WriteReadResponse`: Response message object.
         """
         JsonValidator.response_received(json=json)
         msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
         return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/response_factory.py` & `iqrfpy-0.2.1/iqrfpy/response_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1037,16 +1037,18 @@
                              allow_generic: bool = False) -> BaseFactory:
         """Find response factory by combination of pnum and pcmd.
 
         Args:
             pnum (Union[Peripheral int]): Peripheral number.
             pcmd (Union[Command, int]): Peripheral command.
             allow_generic (bool): Use generic response factory if a matching factory for pnum and pcmd does not exist.
+
         Returns:
             :obj:`BaseFactory`: Response factory.
+
         Raises:
             UnsupportedPeripheralError: If pnum does not exist in response factories and allow_generic is False.
             UnsupportedPeripheralCommandError: If pcmd does not exist in response factories and allow_generic is False.
         """
         if pnum in cls._dpa_factories:
             if pcmd in cls._dpa_factories[pnum]:
                 return cls._dpa_factories[pnum][pcmd]
@@ -1064,30 +1066,33 @@
     @classmethod
     def get_factory_from_mtype(cls, message_type: Union[MessageType, str], msgid: Optional[str] = None) -> BaseFactory:
         """Find response factory by message type.
 
         Args:
             message_type (Union[MessageType, str): Message type.
             msgid (str, optional): Message ID, used for error handling.
+
         Returns:
             :obj:`BaseFactory`: Response factory.
+
         Raises:
             UnsupportedMessageTypeError: If message type does not exist in response factories.
         """
         if message_type in cls._json_factories:
             return cls._json_factories[message_type]
         raise UnsupportedMessageTypeError(f'Unknown or unsupported message type: {message_type}', msgid)
 
     @classmethod
     def get_response_from_dpa(cls, dpa: bytes, allow_generic: bool = False) -> IResponse:
         """Process DPA response and return corresponding response message object.
 
         Args:
             dpa (bytes): DPA response.
             allow_generic (bool): Use generic response class if pnum or pcmd is unknown.
+
         Returns:
             :obj:`IResponse`: Response object.
         """
         IResponse.validate_dpa_response(dpa)
         pnum = dpa[ResponsePacketMembers.PNUM]
         pcmd = dpa[ResponsePacketMembers.PCMD]
         rcode = dpa[ResponsePacketMembers.RCODE]
@@ -1119,13 +1124,13 @@
             json (dict): JSON API response.
         Response:
             :obj:`IResponse`: Response object.
         """
         msgid = Common.msgid_from_json(json)
         mtype = Common.mtype_str_from_json(json)
         if msgid == IResponse.ASYNC_MSGID and \
-                GenericMessages.has_value(mtype) and GenericMessages(mtype) == GenericMessages.RAW:
+                mtype in GenericMessages and GenericMessages(mtype) == GenericMessages.RAW:
             factory = AsyncResponseFactory()
         else:
             message = Common.string_to_mtype(mtype)
             factory = cls.get_factory_from_mtype(message, msgid)
         return factory.create_from_json(json)
```

### Comparing `iqrfpy-0.2.0/iqrfpy/utils/common.py` & `iqrfpy-0.2.1/iqrfpy/utils/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
             nadr (int): Device address
             pnum (Union[Peripheral, int]): Peripheral.
             pcmd (Union[Command, int]): Peripheral command.
             hwpid (int): Hardware profile ID. Defaults to 65535
             pdata (List[int], optional): Request data.
             mutable (bool, optional): Serialize into mutable byte representation of DPA request packet.
                 Defaults to False.
+
         Returns:
             :obj:`bytes`: Immutable byte representation of DPA request packet.\n
             :obj:`bytearray`: Mutable byte representation of DPA request packet (if argument mutable is True).
         """
         dpa: List[int] = [nadr, 0, pnum, pcmd, hwpid & 0xFF, (hwpid >> 8) & 0xFF]
         if pdata is not None:
             dpa.extend(pdata)
@@ -76,17 +77,17 @@
         Raises:
             InvalidPeripheralValueError: Raised if pnum value is not between 0 and 255
             UnsupportedPeripheralError: Raised if pnum parameter value is not recognized as a member of any
                 peripheral enum
         """
         if pnum < 0 or pnum > 255:
             raise InvalidPeripheralValueError('Peripheral value out of range 0-255.')
-        if EmbedPeripherals.has_value(pnum):
+        if pnum in EmbedPeripherals:
             return EmbedPeripherals(pnum)
-        if Standards.has_value(pnum):
+        if pnum in Standards:
             return Standards(pnum)
         if dpa_constants.PNUM_USER_MIN <= pnum <= dpa_constants.PNUM_USER_MAX:
             return pnum
         raise UnsupportedPeripheralError('Unknown or unsupported peripheral.')
 
     @staticmethod
     def request_pcmd_from_dpa(pnum: Union[Peripheral, int], pcmd: int) -> Union[Command, int]:
@@ -144,15 +145,15 @@
             case Standards.SENSOR:
                 commands = SensorRequestCommands
             case Standards.LIGHT:
                 commands = LightRequestCommands
             case _:
                 raise UnsupportedPeripheralError('Unknown or unsupported peripheral.')
 
-        if commands is not None and commands.has_value(pcmd):
+        if commands is not None and pcmd in commands:
             return commands(pcmd)
         raise UnsupportedPeripheralCommandError('Unknown or unsupported peripheral command.')
 
     @staticmethod
     def response_pcmd_from_dpa(pnum: Union[Peripheral, int], pcmd: int) -> Union[Command, int]:
         """Return response command based on DPA peripheral and command data byte.
 
@@ -208,15 +209,15 @@
             case Standards.SENSOR:
                 commands = SensorResponseCommands
             case Standards.LIGHT:
                 commands = LightResponseCommands
             case _:
                 raise UnsupportedPeripheralError('Unknown or unsupported peripheral.')
 
-        if commands is not None and commands.has_value(pcmd):
+        if commands is not None and pcmd in commands:
             return commands(pcmd)
         raise UnsupportedPeripheralCommandError('Unknown or unsupported peripheral command.')
 
     @staticmethod
     def pdata_from_dpa(dpa: bytes) -> Union[List[int], None]:
         """Return PDATA from DPA response bytes.
 
@@ -231,14 +232,15 @@
 
     @staticmethod
     def parse_dpa_into_members(dpa: bytes):
         """Parse DPA response into response members.
 
         Args:
             dpa (bytes): DPA response.
+
         Returns:
             :obj:`(int, int, int, int, int, int, Optional[List[int]])`: Response members
         """
         nadr = dpa[dpa_constants.ResponsePacketMembers.NADR]
         pnum = dpa[dpa_constants.ResponsePacketMembers.PNUM]
         pcmd = dpa[dpa_constants.ResponsePacketMembers.PCMD]
         hwpid = Common.hwpid_from_dpa(
@@ -249,28 +251,30 @@
         dpa_value = dpa[dpa_constants.ResponsePacketMembers.DPA_VALUE]
         pdata = Common.pdata_from_dpa(dpa)
         return nadr, pnum, pcmd, hwpid, rcode, dpa_value, pdata
 
     # json
 
     @staticmethod
-    def serialize_to_json(mtype: MessageType, msgid: str, nadr: int, hwpid: int = 0xFFFF, params: dict = {},
+    def serialize_to_json(mtype: MessageType, msgid: str, nadr: int, hwpid: int = 0xFFFF, params: Optional[dict] = None,
                           dpa_rsp_time: Optional[float] = None):
         """Serialize request parameters into JSON API request object.
 
         Args:
             mtype (MessageType): Message type.
             msgid (str): Message ID.
             nadr (int): Device address.
             hwpid (int): Hardware profile ID. Defaults to 65535.
             params (dict, optional): Request parameters.
             dpa_rsp_time (float, optional): Request timeout.
+
         Returns:
             :obj:`dict`: JSON-serialized request
         """
+        params = params if params is not None else {}
         json: dict = {
             'mType': mtype.value,
             'data': {
                 'msgId': msgid,
                 'req': {
                     'nAdr': nadr,
                     'hwpId': hwpid,
@@ -517,15 +521,15 @@
         Raises:
             UnsupportedMessageTypeError: Raised if message type is not recognized as a member of any message type enum
         """
         messages = [GenericMessages, ExplorationMessages, CoordinatorMessages, NodeMessages, OSMessages, EEPROMMessages,
                     EEEPROMMessages, RAMMessages, LEDRMessages, LEDGMessages, IOMessages, ThermometerMessages,
                     UartMessages, FrcMessages, DALIMessages, BinaryOutputMessages, SensorMessages, LightMessages]
         for item in messages:
-            if item.has_value(string):
+            if string in item:
                 return item(string)
         raise UnsupportedMessageTypeError(f'Unknown or unsupported message type: {string}.')
 
     # general
 
     @staticmethod
     def bitmap_to_nodes(bitmap: List[int], coordinator_shift: bool = False) -> List[int]:
@@ -560,14 +564,15 @@
 
     @staticmethod
     def bitmap_4byte_to_indexes(bitmap: List[int]) -> List[int]:
         """Convert 4 byte bitmap to list of indexes.
 
         Args:
             bitmap (List[int]): Index bitmap.
+
         Returns:
             :obj:`List` of :obj:`int`: List of indexes.
         """
         indexes = [0] * 32
         for i in range(0, len(bitmap * 8)):
             if bitmap[int(i / 8)] & (1 << (i % 8)):
                 indexes[i] = 1
@@ -614,23 +619,27 @@
         if not len(string) % 2 == 0:
             raise ValueError('Argument should be even length.')
         if not Common.is_hex_string(string):
             raise ValueError('Argument is not a hexadecimal string.')
         return [int(string[i:i + 2], base=16) for i in range(0, len(string), 2)]
 
     @staticmethod
-    def list_to_hex_string(values: List[int]) -> str:
+    def list_to_hex_string(values: List[int], separator: str = '', uppercase: bool = False) -> str:
         """Convert list of unsigned integers to hexadecimal string.
 
         Args:
             values (List[int]): List of unsigned integers
+            separator (str, optional): Separator for byte string. Defaults to empty string.
+            uppercase (bool, optional): Output hex string uppercase. Defaults to False.
+
         Returns:
             :obj:`string`: Hexadecimal string representation of the list
         """
-        return ''.join(f'{value:02x}' for value in values)
+        hex_format = 'X' if uppercase else 'x'
+        return separator.join(f'{value:02{hex_format}}' for value in values)
 
     @staticmethod
     def peripheral_list_to_bitmap(values: List[int]) -> List[int]:
         """Convert list of peripheral numbers into a bitmap of peripherals.
 
         For example, the coordinator peripheral would be represented by the 1st bit in bitmap.
 
@@ -666,14 +675,16 @@
     def byte_complement(value: int):
         """Convert unsigned 1B value into a signed 1B value.
 
         Args:
             value (int): Input unsigned 1B value
         Returns:
             :obj:`int`: Signed 1B value
+        Raises:
+            ValueError: Raised when value is not in unsigned 8bit range.
         """
         if not 0 <= value <= 0xFF:
             raise ValueError('Not an unsigned 1B value.')
         if value < 0x80:
             return value
         return value - 0x100
 
@@ -681,13 +692,105 @@
     def word_complement(value: int) -> int:
         """Convert unsigned 2B value into a signed 2B value.
 
         Args:
             value (int): Input unsigned 2B value
         Returns:
             :obj:`int`: Signed 2B value
+        Raises:
+            ValueError: Raised when value is not in unsigned 16bit range.
         """
         if not 0 <= value <= 0xFFFF:
             raise ValueError('Not an unsigned 2B value.')
         if value < 0x8000:
             return value
         return value - 0x10000
+
+    @staticmethod
+    def bcd_to_decimal(byte: int) -> int:
+        """Convert a Binary-Coded Decimal (BCD) value to decimal integer.
+
+        Args:
+            byte (int): BCD value to convert.
+
+        Returns:
+            :obj:`int`: Decimal value encoded in BCD.
+
+        Raises:
+            ValueError: Raised when byte argument is not a valid BCD value.
+
+        Examples:
+            >>> Common.bcd_to_decimal(0x42)
+            42
+        """
+        high = (byte >> 4) & 0x0F
+        low = byte & 0x0F
+        if high > 9 or low > 9:
+            raise ValueError('Not a BCD value.')
+        return high * 10 + low
+
+    @staticmethod
+    def dpa_build_date_to_str(par1: int, par2: int) -> str:
+        """Convert DPA build date in BCD format to human-readable string.
+
+        Outputs date string in the following format: DD.MM.YYYY.
+
+        Args:
+            par1 (int): BCD-encoded day of DPA build date.
+            par2 (int): BCD-encoded month and year of DPA build date.
+
+        Returns:
+            str: Human-readable DPA build date string.
+        """
+        try:
+            day = Common.bcd_to_decimal(par1)
+            month = par2 & 0x0F
+            year = 2010 + ((par2 >> 4) & 0x0F)
+            return f'{day}.{month}.{year}'
+        except ValueError as e:
+            raise ValueError(f'Failed to convert DPA build date to string: {str(e)}') from e
+
+    @staticmethod
+    def dpa_version_to_str(dpa_version: int) -> str:
+        """Convert DPA version in BCD format to human-readable version string.
+
+        Args:
+            dpa_version (int): DPA version encoded in BCD format.
+
+        Returns:
+            str: Human-readable DPA version string.
+
+        Raises:
+            ValueError: Raised when dpa_version is not a valid BCD value.
+        """
+        try:
+            major = Common.bcd_to_decimal(int(dpa_version / 256))
+            minor = dpa_version & 0x00FF
+            return f'{major}.{minor:02X}'
+        except ValueError as e:
+            raise ValueError(f'Failed to convert version to string: {str(e)}') from e
+
+    @staticmethod
+    def fletcher_checksum(init: int, data: List[int]) -> int:
+        """Calculate one's complement Fletcher checksum from list of bytes.
+
+        See https://doc.iqrf.org/DpaTechGuide/pages/FletcherCSharp.html
+
+        Args:
+            init (int): Initial value.
+            data (List[int]): List of bytes to calculate checksum from.
+
+        Returns:
+            :obj:`int`: 16bit Fletcher checksum integer value.
+        """
+        checksum = init
+        for byte in data:
+            low = checksum & 0xFF
+            low += byte
+            if (low & 0x100) != 0:
+                low += 1
+            high = checksum >> 8
+            high += low & 0xFF
+            if (high & 0x100) != 0:
+                high += 1
+            checksum = ((low & 0xFF) | (high & 0xFF) << 8)
+        return checksum
```

### Comparing `iqrfpy-0.2.0/iqrfpy/utils/dpa.py` & `iqrfpy-0.2.1/iqrfpy/utils/dpa.py`

 * *Files 25% similar despite different names*

```diff
@@ -56,14 +56,18 @@
     'IoConstants',
     'TrConfByteAddrs',
     'TrConfBitMasks',
     'OsLoadCodeAction',
     'OsLoadCodeType',
     'OsLoadCodeErrors',
     'OsLoadCodeResult',
+    'McuTypes',
+    'TrDTypes',
+    'TrGTypes',
+    'RfBands',
 )
 
 
 class RequestPacketMembers(IntEnumMember):
     """Request packet member indices."""
 
     NADR = 0
@@ -171,34 +175,47 @@
     CONFIRMATION = 0xFF
 
     def __str__(self):
         """Convert self to representation of error code."""
         return self.to_string(self.value)
 
     @classmethod
+    def is_ok_response(cls, rcode: int) -> bool:
+        """Check if response code indicates OK response, including flags.
+
+        Args:
+            rcode (int): Response code to check.
+
+        Returns:
+            bool: True if response code indicates OK response, False otherwise.
+        """
+        return (rcode & ~cls.ASYNC_RESPONSE & ~cls.RESERVED_FLAG) == ResponseCodes.OK
+
+    @classmethod
     def to_string(cls, value: int):
         """Convert value to string representation of error code.
 
         Args:
             value (int): Value to convert
         Returns:
             :obj:`str`: String representation of error code
         """
         if not BYTE_MIN <= value <= BYTE_MAX:
             return 'Invalid DPA response code'
         if cls.ERROR_USER_FROM <= value <= cls.ERROR_USER_TO:
             return 'User error code'
         flags = []
-        if value & 0x40:
-            flags.append('reserved')
-            value -= 0x40
-        if value & 0x80:
-            flags.append('async')
-            value -= 0x80
-        if value not in cls._value2member_map_:
+        if value != cls.CONFIRMATION:
+            if value & 0x40:
+                flags.append('reserved')
+                value -= 0x40
+            if value & 0x80:
+                flags.append('async')
+                value -= 0x80
+        if value not in cls:
             return 'Unknown DPA response code'
         val = cls(value)
         str_val = None
         match val:
             case cls.OK:
                 str_val = 'No error'
             case cls.ERROR_FAIL:
@@ -359,7 +376,109 @@
     """OS Load Code error enum."""
 
     RESERVED = -1
     HEX_IQRF_CHECKSUM_MISMATCH = 0
     OLD_OS_MISSING = 3
     IQRF_OS_CHANGE_CHECKSUM_MISMATCH = 4
     UNSUPPORTED_IQRF_OS_VERSION = 7
+
+
+class McuTypes(IntEnumMember):
+    """TR module MCU types enum."""
+
+    PIC16LF1938 = 4
+    PIC16LF18877 = 5
+
+    def __str__(self):
+        """String representation of MCU type as module code.
+
+        PIC16LF1938 => D
+        PIC16LF18877 => G
+
+        Returns:
+            str: MCU type code.
+        """
+        match self.value:
+            case self.PIC16LF1938:
+                return 'D'
+            case self.PIC16LF18877:
+                return 'G'
+
+    @classmethod
+    def get_mcu_code(cls, item: int) -> str:
+        """Return MCU code associated with its type.
+
+        Returns:
+            str: MCU code associated with its type ('D' for PIC16LF1938, 'G' for PIC16LF18877, or '?' for unknown).
+        """
+        if item in cls:
+            return str(cls(item))
+        else:
+            return '?'
+
+
+class TrDTypes(IntEnumMember):
+    """TR module D types enum."""
+
+    TR_52D = 0
+    TR_58D_RJ = 1
+    TR_72D = 2
+    TR_53D = 3
+    TR_78D = 4
+    TR_54D = 8
+    TR_55D = 9
+    TR_56D = 10
+    TR_76D = 11
+    TR_77D = 12
+    TR_75D = 13
+
+    def __str__(self):
+        """String representation of TR D type.
+
+        TR_72D => TR-72D
+
+        Returns:
+           str: TR D type string.
+        """
+        return self.name.replace('_', '-')
+
+
+class TrGTypes(IntEnumMember):
+    """TR module G types enum."""
+
+    TR_82G = 0
+    TR_72G = 2
+    TR_85G = 9
+    TR_86G = 10
+    TR_76G = 11
+    TR_75G = 13
+
+    def __str__(self):
+        """String representation of TR G type.
+
+        TR_82G => TR-82G
+
+        Returns:
+            str: TR G type string.
+        """
+        return self.name.replace('_', '-')
+
+
+class RfBands(IntEnumMember):
+    """RF bands enum."""
+
+    RF_BAND_868 = 0
+    RF_BAND_916 = 1
+    RF_BAND_433 = 2
+    RF_BAND_RESERVED = 3
+
+    def __str__(self):
+        """Convert to human-readable string representation.
+
+        Example format 868 MHz.
+
+        Returns:
+            str: Human-readable RF Band string
+        """
+        if self.name == self.RF_BAND_RESERVED.name:
+            return 'Reserved'
+        return f'{self.name[8:]} MHz'
```

### Comparing `iqrfpy-0.2.0/iqrfpy/utils/frc_parser.py` & `iqrfpy-0.2.1/iqrfpy/utils/frc_parser.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy/utils/quantity_data.py` & `iqrfpy-0.2.1/iqrfpy/utils/quantity_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -723,18 +723,19 @@
 
 
 def get_sensor_class(sensor_type: Union[SensorTypes, int]):
     """Return quantity class corresponding to sensor type.
 
     Args:
         sensor_type (Union[SensorTypes, int]): Sensor type (represents a quantity)
+
     Returns:
         Quantity dataclass
     Raises:
         UnknownSensorTypeError: Raised if sensor type is passed as integer and the value is not recognized
         ValueError: Raised if sensor type is recognized, but corresponding quantity data is missing
     """
-    if not SensorTypes.has_value(sensor_type):
+    if sensor_type not in SensorTypes:
         raise UnknownSensorTypeError(f'Unknown or unsupported sensor type: {sensor_type}')
     if sensor_type not in _type_classes:
         raise ValueError(f'Quantity data not available for sensor type: {sensor_type}')
     return _type_classes[sensor_type]
```

### Comparing `iqrfpy-0.2.0/iqrfpy/utils/sensor_constants.py` & `iqrfpy-0.2.1/iqrfpy/utils/sensor_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,16 +90,18 @@
 
     @classmethod
     def from_int(cls, value: int) -> 'SensorFrcErrors':
         """Convert an integer value to SensorFrcError object.
 
         Args:
             value (int): Integer value to convert
+
         Returns:
             :obj:`SensorFrcErrors`: SensorFrcErrors enum member corresponding to the error code.
+
         Raises:
             ValueError: If value is not a SensorFrcError code.
         """
         match value:
             case 0:
                 return cls.NO_FRC_RESPONSE
             case 1:
```

### Comparing `iqrfpy-0.2.0/iqrfpy/utils/sensor_parser.py` & `iqrfpy-0.2.1/iqrfpy/utils/sensor_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Sensor parser module.
 
 Provides methods for parsing of sensor data collected by DPA and JSON API requests.
 """
 
 import math
 import struct
-from typing import List, Union
+from typing import List, Union, Optional
 from iqrfpy.exceptions import UnknownSensorTypeError
 from iqrfpy.objects.sensor_data import SensorData
 from iqrfpy.utils.sensor_constants import SensorDataSize, SensorTypes, SensorFrcCommands, SensorFrcErrors
 from iqrfpy.utils.common import Common
 from iqrfpy.utils.quantity_data import get_sensor_class
 
 
@@ -29,15 +29,15 @@
             :obj:`list` of :obj:`SensorData`: List of SensorData objects containing parsed data
         Raises:
             UnknownSensorTypeError: Raised if sensor type is passed as integer and the value is not recognized
         """
         sensor_data = []
         for i in range(len(dpa)):
             sensor_type_value = dpa[i]
-            if not SensorTypes.has_value(sensor_type_value):
+            if sensor_type_value not in SensorTypes:
                 raise UnknownSensorTypeError('Unsupported sensor type.')
             sensor_type = SensorTypes(sensor_type_value)
             sensor_class = get_sensor_class(sensor_type)
             sensor_data.append(
                 SensorData(
                     sensor_type=sensor_type,
                     index=len(sensor_data),
@@ -64,15 +64,15 @@
         Raises:
             UnknownSensorTypeError: Raised if sensor type is passed as integer and the value is not recognized
         """
         sensor_data = []
         for i in range(len(json_data)):
             data = json_data[i]
             sensor_type_value = data['type']
-            if not SensorTypes.has_value(sensor_type_value):
+            if sensor_type_value not in SensorTypes:
                 raise UnknownSensorTypeError('Unsupported sensor type.')
             sensor_type = SensorTypes(sensor_type_value)
             sensor_class = get_sensor_class(sensor_type)
             sensor_data.append(
                 SensorData(
                     sensor_type=sensor_type,
                     index=len(sensor_data),
@@ -104,15 +104,15 @@
         sensor_data = []
         data_index = 0
         sensor_index = 0
         while data_index < len(dpa):
             if sensor_index >= len(sensor_types):
                 raise ValueError('Too little sensor types provided for the amount of sensor data.')
             sensor_type_value = sensor_types[sensor_index]
-            if not SensorTypes.has_value(sensor_type_value):
+            if sensor_type_value not in SensorTypes:
                 raise UnknownSensorTypeError('Unsupported sensor type.')
             sensor_type = SensorTypes(sensor_type_value)
             if sensor_type == SensorTypes.DATA_BLOCK:
                 data_len = dpa[data_index] + 1
                 if data_index + data_len - 1 >= len(dpa):
                     raise ValueError('Data length longer than actual data.')
             else:
@@ -136,15 +136,15 @@
             UnknownSensorTypeError: Raised if sensor type is passed as integer and the value is not recognized
             ValueError: Raised if passed data is shorter than required to process all sensors
         """
         sensor_data = []
         index = 0
         while index < len(dpa):
             sensor_type_value = dpa[index]
-            if not SensorTypes.has_value(sensor_type_value):
+            if sensor_type_value not in SensorTypes:
                 raise UnknownSensorTypeError(f'Unsupported sensor type: {sensor_type_value}.')
             sensor_type = SensorTypes(sensor_type_value)
             if sensor_type == SensorTypes.DATA_BLOCK:
                 data_length = dpa[index + 1] + 1
                 if index + data_length >= len(dpa):
                     raise ValueError('Data length is less than expected to process all sensors.')
                 data = dpa[index + 2:index + 2 + data_length - 1]
@@ -180,15 +180,15 @@
         Raises:
             UnknownSensorTypeError: Raised if sensor type is passed as integer and the value is not recognized
         """
         sensor_data = []
         for i in range(len(json_data)):
             data = json_data[i]
             sensor_type_value = data['type']
-            if not SensorTypes.has_value(sensor_type_value):
+            if sensor_type_value not in SensorTypes:
                 raise UnknownSensorTypeError('Unsupported sensor type.')
             sensor_type = SensorTypes(sensor_type_value)
             sensor_class = get_sensor_class(sensor_type)
             sensor_data.append(
                 SensorData(
                     sensor_type=sensor_type,
                     index=len(sensor_data),
@@ -199,16 +199,17 @@
                     frc_commands=sensor_class.frc_commands,
                     value=data['value']
                 )
             )
         return sensor_data
 
     @classmethod
-    def frc_dpa(cls, sensor_type: Union[SensorTypes, int], sensor_index: int, frc_command: Union[SensorFrcCommands, int],
-                data: List[int], extra_result: List[int] = [], count: Union[int, None] = None) -> List[SensorData]:
+    def frc_dpa(cls, sensor_type: Union[SensorTypes, int], sensor_index: int,
+                frc_command: Union[SensorFrcCommands, int], data: List[int], extra_result: Optional[List[int]] = None,
+                count: Optional[int] = None) -> List[SensorData]:
         """Process data from DPA FRC response into a list of SensorData.
 
         SensorData object contains information about the measured quantity and converted value.
         The data argument expects only FRC data bytes, without the status byte.
         The extra_result argument can be omitted if the processed data fit into just the Send or SendSelective response.
 
         If count is specified, only that number of node data is processed.
@@ -231,15 +232,15 @@
             :obj:`list` of :obj:`SensorData`: List of SensorData objects containing parsed data
         Raises:
             UnknownSensorTypeError: Raised if sensor type is passed as integer and the value is not recognized
             ValueError: Raised if combined length of frc data and extra result does not match the required data
                         length to process nodes regardless of count argument value
         """
         if isinstance(sensor_type, int):
-            if not SensorTypes.has_value(sensor_type):
+            if sensor_type not in SensorTypes:
                 raise UnknownSensorTypeError('Unknown or unsupported sensor type.')
             sensor_type = SensorTypes(sensor_type)
         sensor_class = get_sensor_class(sensor_type)
         dpa = data
         if frc_command == SensorFrcCommands.FRC_1BYTE:
             dpa = data[1:]
         elif frc_command == SensorFrcCommands.FRC_2BYTES:
@@ -273,15 +274,16 @@
                     val |= 2
                 frc_values.append(val)
         elif data_len == 1:
             frc_values = dpa
         elif data_len == 2:
             frc_values = [(dpa[i + 1] << 8) + dpa[i] for i in range(0, len(dpa), 2)]
         else:
-            frc_values = [(dpa[i + 3] << 24) + (dpa[i + 2] << 16) + (dpa[i + 1] << 8) + dpa[i] for i in range(0, len(dpa), 4)]
+            frc_values = [(dpa[i + 3] << 24) + (dpa[i + 2] << 16) + (dpa[i + 1] << 8) + dpa[i] for i in
+                          range(0, len(dpa), 4)]
         sensor_data = []
         for frc_value in frc_values:
             sensor_data.append(
                 SensorData(
                     sensor_type=sensor_type,
                     index=sensor_index,
                     name=sensor_class.name,
@@ -390,15 +392,16 @@
             case SensorTypes.DATA_BLOCK:
                 length = values[0]
                 return values[1:1 + length]
             case _:
                 return None
 
     @staticmethod
-    def frc_convert(sensor_type: Union[SensorTypes, int], frc_command: int, frc_value: int) -> Union[int, float, SensorFrcErrors, None]:
+    def frc_convert(sensor_type: Union[SensorTypes, int], frc_command: int, frc_value: int) -> Union[
+            int, float, SensorFrcErrors, None]:
         """Convert data collected from FRC to a value within the range of quantity specified by sensor type.
 
         Args:
             sensor_type (Union[SensorTypes, int]): Sensor type (represents a quantity)
             frc_command (int): FRC command used when collecting data
             frc_value (int): Raw data to convert
 
@@ -480,16 +483,18 @@
 
 
 def _data_len_from_type(sensor_type: Union[SensorTypes, int]):
     """Return expected data length per node for sensor type.
 
     Args:
         sensor_type (Union[SensorTypes, int]): Sensor type (represents a quantity)
+
     Returns:
         :obj:`int`: Expected data length per node
+
     Raises:
         UnknownSensorTypeError: Raised if sensor_type value is an unknown or unsupported sensor type
     """
     if SensorDataSize.DATA_1BYTE_MIN <= sensor_type <= SensorDataSize.DATA_1BYTE_MAX:
         return 1
     if SensorDataSize.DATA_2BYTES_MIN <= sensor_type <= SensorDataSize.DATA_2BYTES_MAX:
         return 2
```

### Comparing `iqrfpy-0.2.0/iqrfpy/utils/validators.py` & `iqrfpy-0.2.1/iqrfpy/utils/validators.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.0/iqrfpy.egg-info/PKG-INFO` & `iqrfpy-0.2.1/iqrfpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqrfpy
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python library for communication with IQRF Network
 Home-page: https://gitlab.iqrf.org/open-source/iqrf-sdk/iqrfpy/iqrfpy
 Author: Karel Hanák
 Author-email: karel.hanak@iqrf.org
 License: Apache-2.0
 Project-URL: Changelog, https://apidocs.iqrf.org/iqrfpy/latest/iqrfpy.html#changelog
 Project-URL: Documentation, https://apidocs.iqrf.org/iqrfpy/latest/iqrfpy.html
```

### Comparing `iqrfpy-0.2.0/iqrfpy.egg-info/SOURCES.txt` & `iqrfpy-0.2.1/iqrfpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,27 +27,29 @@
 iqrfpy/objects/__init__.py
 iqrfpy/objects/binaryoutput_state.py
 iqrfpy/objects/coordinator_authorize_bond_params.py
 iqrfpy/objects/coordinator_dpa_param.py
 iqrfpy/objects/exploration_per_enum_data.py
 iqrfpy/objects/exploration_per_info_data.py
 iqrfpy/objects/frc_params.py
+iqrfpy/objects/init_phy_data.py
 iqrfpy/objects/io_triplet.py
 iqrfpy/objects/node_read_data.py
 iqrfpy/objects/node_validate_bonds_params.py
 iqrfpy/objects/os_batch_data.py
 iqrfpy/objects/os_indicate_param.py
 iqrfpy/objects/os_load_code_flags.py
 iqrfpy/objects/os_read_data.py
 iqrfpy/objects/os_security_type_param.py
 iqrfpy/objects/os_sleep_params.py
 iqrfpy/objects/os_tr_conf_byte.py
 iqrfpy/objects/os_tr_conf_data.py
 iqrfpy/objects/sensor_data.py
 iqrfpy/objects/sensor_written_data.py
+iqrfpy/objects/tr_mcu_type_data.py
 iqrfpy/peripherals/__init__.py
 iqrfpy/peripherals/py.typed
 iqrfpy/peripherals/binaryoutput/__init__.py
 iqrfpy/peripherals/binaryoutput/requests/__init__.py
 iqrfpy/peripherals/binaryoutput/requests/enumerate.py
 iqrfpy/peripherals/binaryoutput/requests/set_output.py
 iqrfpy/peripherals/binaryoutput/responses/__init__.py
```

### Comparing `iqrfpy-0.2.0/setup.cfg` & `iqrfpy-0.2.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iqrfpy
-version = 0.2.0
+version = 0.2.1
 url = https://gitlab.iqrf.org/open-source/iqrf-sdk/iqrfpy/iqrfpy
 author = Karel Hanák
 author_email = karel.hanak@iqrf.org
 description = A python library for communication with IQRF Network
 changelog = https://gitlab.iqrf.org/open-source/iqrf-sdk/iqrfpy/iqrfpy/-/blob/master/changelog.md
 long_description = file: README.md
 long_description_content_type = text/markdown
```


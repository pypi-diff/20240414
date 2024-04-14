# Comparing `tmp/cool-open-client-0.0.8.tar.gz` & `tmp/cool-open-client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cool-open-client-0.0.8.tar", last modified: Sun Oct 23 13:53:32 2022, max compression
+gzip compressed data, was "cool-open-client-0.0.9.tar", last modified: Sat Dec 24 19:28:57 2022, max compression
```

## Comparing `cool-open-client-0.0.8.tar` & `cool-open-client-0.0.9.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxrwx---   0 root         (0) pipx       (999)        0 2022-10-23 13:53:32.232597 cool-open-client-0.0.8/
--rwxrwx---   0 root         (0) pipx       (999)    35133 2022-07-08 19:46:09.000000 cool-open-client-0.0.8/LICENSE.md
--rwxrwx---   0 root         (0) pipx       (999)        1 2022-07-14 14:30:35.000000 cool-open-client-0.0.8/MANIFEST.in
--rwxrwx---   0 root         (0) pipx       (999)      648 2022-10-23 13:53:32.235704 cool-open-client-0.0.8/PKG-INFO
--rwxrwx---   0 root         (0) pipx       (999)      141 2022-07-08 12:59:11.000000 cool-open-client-0.0.8/README.md
-drwxrwx---   0 root         (0) pipx       (999)        0 2022-10-23 13:53:18.858668 cool-open-client-0.0.8/cool_open_client/
--rwxrwx---   0 root         (0) pipx       (999)        0 2022-07-29 10:54:48.000000 cool-open-client-0.0.8/cool_open_client/__init__.py
-drwxrwx---   0 root         (0) pipx       (999)        0 2022-10-23 13:53:19.905366 cool-open-client-0.0.8/cool_open_client/client/
--rwxrwx---   0 root         (0) pipx       (999)    10209 2022-10-23 13:52:07.000000 cool-open-client-0.0.8/cool_open_client/client/__init__.py
-drwxrwx---   0 root         (0) pipx       (999)        0 2022-10-23 13:53:23.752803 cool-open-client-0.0.8/cool_open_client/client/api/
--rwxrwx---   0 root         (0) pipx       (999)     2118 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/__init__.py
--rwxrwx---   0 root         (0) pipx       (999)     4520 2022-10-23 13:52:04.000000 cool-open-client-0.0.8/cool_open_client/client/api/admins_api.py
--rwxrwx---   0 root         (0) pipx       (999)     4511 2022-10-23 13:52:04.000000 cool-open-client-0.0.8/cool_open_client/client/api/authentication_api.py
--rwxrwx---   0 root         (0) pipx       (999)    19700 2022-10-23 13:52:04.000000 cool-open-client-0.0.8/cool_open_client/client/api/customer_api.py
--rwxrwx---   0 root         (0) pipx       (999)    10342 2022-10-23 13:52:04.000000 cool-open-client-0.0.8/cool_open_client/client/api/customer_sites_api.py
--rwxrwx---   0 root         (0) pipx       (999)    10318 2022-10-23 13:52:04.000000 cool-open-client-0.0.8/cool_open_client/client/api/customer_users_api.py
--rwxrwx---   0 root         (0) pipx       (999)     4528 2022-10-23 13:52:04.000000 cool-open-client-0.0.8/cool_open_client/client/api/customers_api.py
--rwxrwx---   0 root         (0) pipx       (999)    14244 2022-10-23 13:52:04.000000 cool-open-client-0.0.8/cool_open_client/client/api/device_api.py
--rwxrwx---   0 root         (0) pipx       (999)     5120 2022-10-23 13:52:04.000000 cool-open-client-0.0.8/cool_open_client/client/api/device_units_api.py
--rwxrwx---   0 root         (0) pipx       (999)     4424 2022-10-23 13:52:04.000000 cool-open-client-0.0.8/cool_open_client/client/api/devices_api.py
--rwxrwx---   0 root         (0) pipx       (999)     8013 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/me_api.py
--rwxrwx---   0 root         (0) pipx       (999)     4558 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/services_api.py
--rwxrwx---   0 root         (0) pipx       (999)    13988 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/site_api.py
--rwxrwx---   0 root         (0) pipx       (999)    10056 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/site_devices_api.py
--rwxrwx---   0 root         (0) pipx       (999)    10056 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/site_systems_api.py
--rwxrwx---   0 root         (0) pipx       (999)     9986 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/site_users_api.py
--rwxrwx---   0 root         (0) pipx       (999)     9986 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/site_zones_api.py
--rwxrwx---   0 root         (0) pipx       (999)     4390 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/sites_api.py
--rwxrwx---   0 root         (0) pipx       (999)    14244 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/system_api.py
--rwxrwx---   0 root         (0) pipx       (999)    11261 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/system_control_api.py
--rwxrwx---   0 root         (0) pipx       (999)    15066 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/system_units_api.py
--rwxrwx---   0 root         (0) pipx       (999)     4424 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/systems_api.py
--rwxrwx---   0 root         (0) pipx       (999)     9779 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/unit_api.py
--rwxrwx---   0 root         (0) pipx       (999)    26087 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/unit_control_api.py
--rwxrwx---   0 root         (0) pipx       (999)     4390 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/units_api.py
--rwxrwx---   0 root         (0) pipx       (999)    13988 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/user_api.py
--rwxrwx---   0 root         (0) pipx       (999)     4390 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/users_api.py
--rwxrwx---   0 root         (0) pipx       (999)     3635 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/websocket_api.py
--rwxrwx---   0 root         (0) pipx       (999)    14004 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/zone_api.py
--rwxrwx---   0 root         (0) pipx       (999)    21442 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/zone_control_api.py
--rwxrwx---   0 root         (0) pipx       (999)    14816 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/zone_units_api.py
--rwxrwx---   0 root         (0) pipx       (999)     4390 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api/zones_api.py
--rwxrwx---   0 root         (0) pipx       (999)    25086 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/api_client.py
--rwxrwx---   0 root         (0) pipx       (999)     7982 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/configuration.py
-drwxrwx---   0 root         (0) pipx       (999)        0 2022-10-23 13:53:31.558541 cool-open-client-0.0.8/cool_open_client/client/models/
--rwxrwx---   0 root         (0) pipx       (999)     8008 2022-10-23 13:52:07.000000 cool-open-client-0.0.8/cool_open_client/client/models/__init__.py
--rwxrwx---   0 root         (0) pipx       (999)     4028 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/authenticate_request_body.py
--rwxrwx---   0 root         (0) pipx       (999)     3895 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/bad_response401.py
--rwxrwx---   0 root         (0) pipx       (999)     3895 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/bad_response403.py
--rwxrwx---   0 root         (0) pipx       (999)     3895 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/bad_response404.py
--rwxrwx---   0 root         (0) pipx       (999)     3895 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/bad_response500.py
--rwxrwx---   0 root         (0) pipx       (999)     3843 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/control_tree_response.py
--rwxrwx---   0 root         (0) pipx       (999)     3260 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/control_tree_response_data.py
--rwxrwx---   0 root         (0) pipx       (999)     3402 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/control_tree_response_data_customers.py
--rwxrwx---   0 root         (0) pipx       (999)     5668 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/control_tree_response_data_customers_customer_id.py
--rwxrwx---   0 root         (0) pipx       (999)     3475 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/control_tree_response_data_customers_customer_id_sites.py
--rwxrwx---   0 root         (0) pipx       (999)     7702 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/control_tree_response_data_customers_customer_id_sites_site_id.py
--rwxrwx---   0 root         (0) pipx       (999)     4099 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/create_customer_request_body.py
--rwxrwx---   0 root         (0) pipx       (999)     4736 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/create_device_request_body.py
--rwxrwx---   0 root         (0) pipx       (999)     7946 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/create_site_request_body.py
--rwxrwx---   0 root         (0) pipx       (999)     4067 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/create_system_request_body.py
--rwxrwx---   0 root         (0) pipx       (999)     9244 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/create_user_request_body.py
--rwxrwx---   0 root         (0) pipx       (999)     4035 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/create_zone_request_body.py
--rwxrwx---   0 root         (0) pipx       (999)     3798 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/customer_response.py
--rwxrwx---   0 root         (0) pipx       (999)     6070 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/customer_response_data.py
--rwxrwx---   0 root         (0) pipx       (999)     3813 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/customers_response.py
--rwxrwx---   0 root         (0) pipx       (999)     3255 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/customers_response_data.py
--rwxrwx---   0 root         (0) pipx       (999)     3768 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/device_response.py
--rwxrwx---   0 root         (0) pipx       (999)     6787 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/device_response_data.py
--rwxrwx---   0 root         (0) pipx       (999)     3783 2022-10-23 13:52:05.000000 cool-open-client-0.0.8/cool_open_client/client/models/devices_response.py
--rwxrwx---   0 root         (0) pipx       (999)     2674 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/devices_response_data.py
--rwxrwx---   0 root         (0) pipx       (999)     3106 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/okresponse.py
--rwxrwx---   0 root         (0) pipx       (999)     3798 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/okresponse_with_id.py
--rwxrwx---   0 root         (0) pipx       (999)     3095 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/okresponse_with_id_data.py
--rwxrwx---   0 root         (0) pipx       (999)     3843 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/okresponse_with_token.py
--rwxrwx---   0 root         (0) pipx       (999)     3163 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/okresponse_with_token_data.py
--rwxrwx---   0 root         (0) pipx       (999)     3738 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/site_response.py
--rwxrwx---   0 root         (0) pipx       (999)    11979 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/site_response_data.py
--rwxrwx---   0 root         (0) pipx       (999)     3753 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/sites_response.py
--rwxrwx---   0 root         (0) pipx       (999)     3131 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/sites_response_data.py
--rwxrwx---   0 root         (0) pipx       (999)     3316 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/system_control_modes_body.py
--rwxrwx---   0 root         (0) pipx       (999)     3346 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/system_control_switches_body.py
--rwxrwx---   0 root         (0) pipx       (999)     3768 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/system_response.py
--rwxrwx---   0 root         (0) pipx       (999)     5856 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/system_response_data.py
--rwxrwx---   0 root         (0) pipx       (999)     3783 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/systems_response.py
--rwxrwx---   0 root         (0) pipx       (999)     3193 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/systems_response_data.py
--rwxrwx---   0 root         (0) pipx       (999)     3753 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/types_response.py
--rwxrwx---   0 root         (0) pipx       (999)    12251 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/types_response_data.py
--rwxrwx---   0 root         (0) pipx       (999)     2710 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_device_types.py
--rwxrwx---   0 root         (0) pipx       (999)     4141 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_device_types_type_object.py
--rwxrwx---   0 root         (0) pipx       (999)     2698 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_fan_modes.py
--rwxrwx---   0 root         (0) pipx       (999)     2470 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_hvac_brands.py
--rwxrwx---   0 root         (0) pipx       (999)     6556 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_hvac_brands_inner.py
--rwxrwx---   0 root         (0) pipx       (999)     2722 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_operation_modes.py
--rwxrwx---   0 root         (0) pipx       (999)     2734 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_operation_statuses.py
--rwxrwx---   0 root         (0) pipx       (999)     2710 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_permissions.py
--rwxrwx---   0 root         (0) pipx       (999)     2702 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_resources.py
--rwxrwx---   0 root         (0) pipx       (999)     2686 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_roles.py
--rwxrwx---   0 root         (0) pipx       (999)     2706 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_swing_modes.py
--rwxrwx---   0 root         (0) pipx       (999)     2730 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_temperature_scale.py
--rwxrwx---   0 root         (0) pipx       (999)     2702 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_unit_types.py
--rwxrwx---   0 root         (0) pipx       (999)     2698 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_week_days.py
--rwxrwx---   0 root         (0) pipx       (999)     3351 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/unit_control_fans_body.py
--rwxrwx---   0 root         (0) pipx       (999)     3509 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/unit_control_modes_body.py
--rwxrwx---   0 root         (0) pipx       (999)     3458 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/unit_control_setpoints_body.py
--rwxrwx---   0 root         (0) pipx       (999)     3427 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/unit_control_swings_body.py
--rwxrwx---   0 root         (0) pipx       (999)     3875 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/unit_control_switches_body.py
--rwxrwx---   0 root         (0) pipx       (999)     3738 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/unit_response.py
--rwxrwx---   0 root         (0) pipx       (999)    20563 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/unit_response_data.py
--rwxrwx---   0 root         (0) pipx       (999)     4406 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/unit_response_data_temperature_limits.py
--rwxrwx---   0 root         (0) pipx       (999)     3753 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/units_response.py
--rwxrwx---   0 root         (0) pipx       (999)     2666 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/units_response_data.py
--rwxrwx---   0 root         (0) pipx       (999)     4099 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/update_customer_request_body.py
--rwxrwx---   0 root         (0) pipx       (999)     3141 2022-10-23 13:52:06.000000 cool-open-client-0.0.8/cool_open_client/client/models/update_device_request_body.py
--rwxrwx---   0 root         (0) pipx       (999)     7776 2022-10-23 13:52:07.000000 cool-open-client-0.0.8/cool_open_client/client/models/update_site_request_body.py
--rwxrwx---   0 root         (0) pipx       (999)     3984 2022-10-23 13:52:07.000000 cool-open-client-0.0.8/cool_open_client/client/models/update_system_request_body.py
--rwxrwx---   0 root         (0) pipx       (999)     9418 2022-10-23 13:52:07.000000 cool-open-client-0.0.8/cool_open_client/client/models/update_unit_request_body.py
--rwxrwx---   0 root         (0) pipx       (999)     8119 2022-10-23 13:52:07.000000 cool-open-client-0.0.8/cool_open_client/client/models/update_user_request_body.py
--rwxrwx---   0 root         (0) pipx       (999)     3952 2022-10-23 13:52:07.000000 cool-open-client-0.0.8/cool_open_client/client/models/update_zone_request_body.py
--rwxrwx---   0 root         (0) pipx       (999)     3738 2022-10-23 13:52:07.000000 cool-open-client-0.0.8/cool_open_client/client/models/user_response.py
--rwxrwx---   0 root         (0) pipx       (999)     6690 2022-10-23 13:52:07.000000 cool-open-client-0.0.8/cool_open_client/client/models/user_response_data.py
--rwxrwx---   0 root         (0) pipx       (999)     3753 2022-10-23 13:52:07.000000 cool-open-client-0.0.8/cool_open_client/client/models/users_response.py
--rwxrwx---   0 root         (0) pipx       (999)     3131 2022-10-23 13:52:07.000000 cool-open-client-0.0.8/cool_open_client/client/models/users_response_data.py
--rwxrwx---   0 root         (0) pipx       (999)     3268 2022-10-23 13:52:07.000000 cool-open-client-0.0.8/cool_open_client/client/models/zone_control_fans_body.py
--rwxrwx---   0 root         (0) pipx       (999)     3300 2022-10-23 13:52:07.000000 cool-open-client-0.0.8/cool_open_client/client/models/zone_control_modes_body.py
--rwxrwx---   0 root         (0) pipx       (999)     3458 2022-10-23 13:52:07.000000 cool-open-client-0.0.8/cool_open_client/client/models/zone_control_setpoints_body.py
--rwxrwx---   0 root         (0) pipx       (999)     3330 2022-10-23 13:52:07.000000 cool-open-client-0.0.8/cool_open_client/client/models/zone_control_switches_body.py
--rwxrwx---   0 root         (0) pipx       (999)     3738 2022-10-23 13:52:07.000000 cool-open-client-0.0.8/cool_open_client/client/models/zone_response.py
--rwxrwx---   0 root         (0) pipx       (999)     5796 2022-10-23 13:52:07.000000 cool-open-client-0.0.8/cool_open_client/client/models/zone_response_data.py
--rwxrwx---   0 root         (0) pipx       (999)     3753 2022-10-23 13:52:07.000000 cool-open-client-0.0.8/cool_open_client/client/models/zones_response.py
--rwxrwx---   0 root         (0) pipx       (999)     3131 2022-10-23 13:52:07.000000 cool-open-client-0.0.8/cool_open_client/client/models/zones_response_data.py
--rwxrwx---   0 root         (0) pipx       (999)    10644 2022-10-23 13:52:07.000000 cool-open-client-0.0.8/cool_open_client/client/rest.py
--rwxrwx---   0 root         (0) pipx       (999)    18525 2022-10-23 13:34:56.000000 cool-open-client-0.0.8/cool_open_client/cool_automation_client.py
--rwxrwx---   0 root         (0) pipx       (999)     2293 2022-08-18 11:53:05.000000 cool-open-client-0.0.8/cool_open_client/hvac_units_factory.py
--rwxrwx---   0 root         (0) pipx       (999)     7134 2022-09-22 14:03:47.000000 cool-open-client-0.0.8/cool_open_client/unit.py
-drwxrwx---   0 root         (0) pipx       (999)        0 2022-10-23 13:53:31.938697 cool-open-client-0.0.8/cool_open_client/utils/
--rwxrwx---   0 root         (0) pipx       (999)        0 2022-07-09 18:33:19.000000 cool-open-client-0.0.8/cool_open_client/utils/__init__.py
--rwxrwx---   0 root         (0) pipx       (999)      583 2022-07-29 19:11:17.000000 cool-open-client-0.0.8/cool_open_client/utils/dict_to_model.py
--rwxrwx---   0 root         (0) pipx       (999)      913 2022-06-27 14:10:15.000000 cool-open-client-0.0.8/cool_open_client/utils/dictionaries.py
--rwxrwx---   0 root         (0) pipx       (999)      680 2022-09-17 20:52:54.000000 cool-open-client-0.0.8/cool_open_client/utils/singleton.py
--rwxrwx---   0 root         (0) pipx       (999)      208 2022-07-28 13:30:00.000000 cool-open-client-0.0.8/cool_open_client/utils/updatable.py
-drwxrwx---   0 root         (0) pipx       (999)        0 2022-10-23 13:53:19.413370 cool-open-client-0.0.8/cool_open_client.egg-info/
--rwxrwx---   0 root         (0) pipx       (999)      648 2022-10-23 13:53:14.000000 cool-open-client-0.0.8/cool_open_client.egg-info/PKG-INFO
--rwxrwx---   0 root         (0) pipx       (999)     7315 2022-10-23 13:53:17.000000 cool-open-client-0.0.8/cool_open_client.egg-info/SOURCES.txt
--rwxrwx---   0 root         (0) pipx       (999)        1 2022-10-23 13:53:14.000000 cool-open-client-0.0.8/cool_open_client.egg-info/dependency_links.txt
--rwxrwx---   0 root         (0) pipx       (999)      216 2022-10-23 13:53:14.000000 cool-open-client-0.0.8/cool_open_client.egg-info/requires.txt
--rwxrwx---   0 root         (0) pipx       (999)       23 2022-10-23 13:53:14.000000 cool-open-client-0.0.8/cool_open_client.egg-info/top_level.txt
--rwxrwx---   0 root         (0) pipx       (999)       99 2022-07-08 19:49:26.000000 cool-open-client-0.0.8/pyproject.toml
--rwxrwx---   0 root         (0) pipx       (999)       38 2022-10-23 13:53:32.270454 cool-open-client-0.0.8/setup.cfg
--rwxrwx---   0 root         (0) pipx       (999)     1336 2022-10-23 13:48:27.000000 cool-open-client-0.0.8/setup.py
-drwxrwx---   0 root         (0) pipx       (999)        0 2022-10-23 13:53:32.188490 cool-open-client-0.0.8/tests/
--rwxrwx---   0 root         (0) pipx       (999)        0 2022-07-26 12:32:25.000000 cool-open-client-0.0.8/tests/__init__.py
--rwxrwx---   0 root         (0) pipx       (999)     1491 2022-08-15 12:47:20.000000 cool-open-client-0.0.8/tests/test_cool_open_client.py
--rwxrwx---   0 root         (0) pipx       (999)      684 2022-08-09 08:02:33.000000 cool-open-client-0.0.8/tests/test_hvac_units_factory.py
--rwxrwx---   0 root         (0) pipx       (999)      766 2022-08-14 14:24:19.000000 cool-open-client-0.0.8/tests/test_websocket.py
+drwxrwx---   0 root         (0) pipx       (999)        0 2022-12-24 19:28:57.283170 cool-open-client-0.0.9/
+-rwxrwx---   0 root         (0) pipx       (999)    35133 2022-07-08 19:46:09.000000 cool-open-client-0.0.9/LICENSE.md
+-rwxrwx---   0 root         (0) pipx       (999)        1 2022-07-14 14:30:35.000000 cool-open-client-0.0.9/MANIFEST.in
+-rwxrwx---   0 root         (0) pipx       (999)      648 2022-12-24 19:28:57.284170 cool-open-client-0.0.9/PKG-INFO
+-rwxrwx---   0 root         (0) pipx       (999)      141 2022-07-08 12:59:11.000000 cool-open-client-0.0.9/README.md
+drwxrwx---   0 root         (0) pipx       (999)        0 2022-12-24 19:28:55.018197 cool-open-client-0.0.9/cool_open_client/
+-rwxrwx---   0 root         (0) pipx       (999)        0 2022-07-29 10:54:48.000000 cool-open-client-0.0.9/cool_open_client/__init__.py
+drwxrwx---   0 root         (0) pipx       (999)        0 2022-12-24 19:28:55.161043 cool-open-client-0.0.9/cool_open_client/client/
+-rwxrwx---   0 root         (0) pipx       (999)    10209 2022-10-23 13:52:07.000000 cool-open-client-0.0.9/cool_open_client/client/__init__.py
+drwxrwx---   0 root         (0) pipx       (999)        0 2022-12-24 19:28:55.723135 cool-open-client-0.0.9/cool_open_client/client/api/
+-rwxrwx---   0 root         (0) pipx       (999)     2118 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/__init__.py
+-rwxrwx---   0 root         (0) pipx       (999)     4520 2022-10-23 13:52:04.000000 cool-open-client-0.0.9/cool_open_client/client/api/admins_api.py
+-rwxrwx---   0 root         (0) pipx       (999)     4511 2022-10-23 13:52:04.000000 cool-open-client-0.0.9/cool_open_client/client/api/authentication_api.py
+-rwxrwx---   0 root         (0) pipx       (999)    19700 2022-10-23 13:52:04.000000 cool-open-client-0.0.9/cool_open_client/client/api/customer_api.py
+-rwxrwx---   0 root         (0) pipx       (999)    10342 2022-10-23 13:52:04.000000 cool-open-client-0.0.9/cool_open_client/client/api/customer_sites_api.py
+-rwxrwx---   0 root         (0) pipx       (999)    10318 2022-10-23 13:52:04.000000 cool-open-client-0.0.9/cool_open_client/client/api/customer_users_api.py
+-rwxrwx---   0 root         (0) pipx       (999)     4528 2022-10-23 13:52:04.000000 cool-open-client-0.0.9/cool_open_client/client/api/customers_api.py
+-rwxrwx---   0 root         (0) pipx       (999)    14244 2022-10-23 13:52:04.000000 cool-open-client-0.0.9/cool_open_client/client/api/device_api.py
+-rwxrwx---   0 root         (0) pipx       (999)     5120 2022-10-23 13:52:04.000000 cool-open-client-0.0.9/cool_open_client/client/api/device_units_api.py
+-rwxrwx---   0 root         (0) pipx       (999)     4424 2022-10-23 13:52:04.000000 cool-open-client-0.0.9/cool_open_client/client/api/devices_api.py
+-rwxrwx---   0 root         (0) pipx       (999)     8013 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/me_api.py
+-rwxrwx---   0 root         (0) pipx       (999)     4558 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/services_api.py
+-rwxrwx---   0 root         (0) pipx       (999)    13988 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/site_api.py
+-rwxrwx---   0 root         (0) pipx       (999)    10056 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/site_devices_api.py
+-rwxrwx---   0 root         (0) pipx       (999)    10056 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/site_systems_api.py
+-rwxrwx---   0 root         (0) pipx       (999)     9986 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/site_users_api.py
+-rwxrwx---   0 root         (0) pipx       (999)     9986 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/site_zones_api.py
+-rwxrwx---   0 root         (0) pipx       (999)     4390 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/sites_api.py
+-rwxrwx---   0 root         (0) pipx       (999)    14244 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/system_api.py
+-rwxrwx---   0 root         (0) pipx       (999)    11261 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/system_control_api.py
+-rwxrwx---   0 root         (0) pipx       (999)    15066 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/system_units_api.py
+-rwxrwx---   0 root         (0) pipx       (999)     4424 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/systems_api.py
+-rwxrwx---   0 root         (0) pipx       (999)     9779 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/unit_api.py
+-rwxrwx---   0 root         (0) pipx       (999)    26087 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/unit_control_api.py
+-rwxrwx---   0 root         (0) pipx       (999)     4390 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/units_api.py
+-rwxrwx---   0 root         (0) pipx       (999)    13988 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/user_api.py
+-rwxrwx---   0 root         (0) pipx       (999)     4390 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/users_api.py
+-rwxrwx---   0 root         (0) pipx       (999)     3635 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/websocket_api.py
+-rwxrwx---   0 root         (0) pipx       (999)    14004 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/zone_api.py
+-rwxrwx---   0 root         (0) pipx       (999)    21442 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/zone_control_api.py
+-rwxrwx---   0 root         (0) pipx       (999)    14816 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/zone_units_api.py
+-rwxrwx---   0 root         (0) pipx       (999)     4390 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api/zones_api.py
+-rwxrwx---   0 root         (0) pipx       (999)    25086 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/api_client.py
+-rwxrwx---   0 root         (0) pipx       (999)     7982 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/configuration.py
+drwxrwx---   0 root         (0) pipx       (999)        0 2022-12-24 19:28:57.149681 cool-open-client-0.0.9/cool_open_client/client/models/
+-rwxrwx---   0 root         (0) pipx       (999)     8008 2022-10-23 13:52:07.000000 cool-open-client-0.0.9/cool_open_client/client/models/__init__.py
+-rwxrwx---   0 root         (0) pipx       (999)     4028 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/authenticate_request_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     3895 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/bad_response401.py
+-rwxrwx---   0 root         (0) pipx       (999)     3895 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/bad_response403.py
+-rwxrwx---   0 root         (0) pipx       (999)     3895 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/bad_response404.py
+-rwxrwx---   0 root         (0) pipx       (999)     3895 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/bad_response500.py
+-rwxrwx---   0 root         (0) pipx       (999)     3843 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/control_tree_response.py
+-rwxrwx---   0 root         (0) pipx       (999)     3260 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/control_tree_response_data.py
+-rwxrwx---   0 root         (0) pipx       (999)     3402 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/control_tree_response_data_customers.py
+-rwxrwx---   0 root         (0) pipx       (999)     5668 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/control_tree_response_data_customers_customer_id.py
+-rwxrwx---   0 root         (0) pipx       (999)     3475 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/control_tree_response_data_customers_customer_id_sites.py
+-rwxrwx---   0 root         (0) pipx       (999)     7702 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/control_tree_response_data_customers_customer_id_sites_site_id.py
+-rwxrwx---   0 root         (0) pipx       (999)     4099 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/create_customer_request_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     4736 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/create_device_request_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     7946 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/create_site_request_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     4067 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/create_system_request_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     9244 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/create_user_request_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     4035 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/create_zone_request_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     3798 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/customer_response.py
+-rwxrwx---   0 root         (0) pipx       (999)     6070 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/customer_response_data.py
+-rwxrwx---   0 root         (0) pipx       (999)     3813 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/customers_response.py
+-rwxrwx---   0 root         (0) pipx       (999)     3255 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/customers_response_data.py
+-rwxrwx---   0 root         (0) pipx       (999)     3768 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/device_response.py
+-rwxrwx---   0 root         (0) pipx       (999)     6787 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/device_response_data.py
+-rwxrwx---   0 root         (0) pipx       (999)     3783 2022-10-23 13:52:05.000000 cool-open-client-0.0.9/cool_open_client/client/models/devices_response.py
+-rwxrwx---   0 root         (0) pipx       (999)     2674 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/devices_response_data.py
+-rwxrwx---   0 root         (0) pipx       (999)     3106 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/okresponse.py
+-rwxrwx---   0 root         (0) pipx       (999)     3798 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/okresponse_with_id.py
+-rwxrwx---   0 root         (0) pipx       (999)     3095 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/okresponse_with_id_data.py
+-rwxrwx---   0 root         (0) pipx       (999)     3843 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/okresponse_with_token.py
+-rwxrwx---   0 root         (0) pipx       (999)     3163 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/okresponse_with_token_data.py
+-rwxrwx---   0 root         (0) pipx       (999)     3738 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/site_response.py
+-rwxrwx---   0 root         (0) pipx       (999)    11979 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/site_response_data.py
+-rwxrwx---   0 root         (0) pipx       (999)     3753 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/sites_response.py
+-rwxrwx---   0 root         (0) pipx       (999)     3131 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/sites_response_data.py
+-rwxrwx---   0 root         (0) pipx       (999)     3316 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/system_control_modes_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     3346 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/system_control_switches_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     3768 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/system_response.py
+-rwxrwx---   0 root         (0) pipx       (999)     5856 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/system_response_data.py
+-rwxrwx---   0 root         (0) pipx       (999)     3783 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/systems_response.py
+-rwxrwx---   0 root         (0) pipx       (999)     3193 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/systems_response_data.py
+-rwxrwx---   0 root         (0) pipx       (999)     3753 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/types_response.py
+-rwxrwx---   0 root         (0) pipx       (999)    12251 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/types_response_data.py
+-rwxrwx---   0 root         (0) pipx       (999)     2710 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_device_types.py
+-rwxrwx---   0 root         (0) pipx       (999)     4141 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_device_types_type_object.py
+-rwxrwx---   0 root         (0) pipx       (999)     2698 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_fan_modes.py
+-rwxrwx---   0 root         (0) pipx       (999)     2470 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_hvac_brands.py
+-rwxrwx---   0 root         (0) pipx       (999)     6556 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_hvac_brands_inner.py
+-rwxrwx---   0 root         (0) pipx       (999)     2722 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_operation_modes.py
+-rwxrwx---   0 root         (0) pipx       (999)     2734 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_operation_statuses.py
+-rwxrwx---   0 root         (0) pipx       (999)     2710 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_permissions.py
+-rwxrwx---   0 root         (0) pipx       (999)     2702 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_resources.py
+-rwxrwx---   0 root         (0) pipx       (999)     2686 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_roles.py
+-rwxrwx---   0 root         (0) pipx       (999)     2706 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_swing_modes.py
+-rwxrwx---   0 root         (0) pipx       (999)     2730 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_temperature_scale.py
+-rwxrwx---   0 root         (0) pipx       (999)     2702 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_unit_types.py
+-rwxrwx---   0 root         (0) pipx       (999)     2698 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_week_days.py
+-rwxrwx---   0 root         (0) pipx       (999)     3351 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/unit_control_fans_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     3509 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/unit_control_modes_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     3458 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/unit_control_setpoints_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     3427 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/unit_control_swings_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     3875 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/unit_control_switches_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     3738 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/unit_response.py
+-rwxrwx---   0 root         (0) pipx       (999)    20563 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/unit_response_data.py
+-rwxrwx---   0 root         (0) pipx       (999)     4406 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/unit_response_data_temperature_limits.py
+-rwxrwx---   0 root         (0) pipx       (999)     3753 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/units_response.py
+-rwxrwx---   0 root         (0) pipx       (999)     2666 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/units_response_data.py
+-rwxrwx---   0 root         (0) pipx       (999)     4099 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/update_customer_request_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     3141 2022-10-23 13:52:06.000000 cool-open-client-0.0.9/cool_open_client/client/models/update_device_request_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     7776 2022-10-23 13:52:07.000000 cool-open-client-0.0.9/cool_open_client/client/models/update_site_request_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     3984 2022-10-23 13:52:07.000000 cool-open-client-0.0.9/cool_open_client/client/models/update_system_request_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     9418 2022-10-23 13:52:07.000000 cool-open-client-0.0.9/cool_open_client/client/models/update_unit_request_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     8119 2022-10-23 13:52:07.000000 cool-open-client-0.0.9/cool_open_client/client/models/update_user_request_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     3952 2022-10-23 13:52:07.000000 cool-open-client-0.0.9/cool_open_client/client/models/update_zone_request_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     3738 2022-10-23 13:52:07.000000 cool-open-client-0.0.9/cool_open_client/client/models/user_response.py
+-rwxrwx---   0 root         (0) pipx       (999)     6690 2022-10-23 13:52:07.000000 cool-open-client-0.0.9/cool_open_client/client/models/user_response_data.py
+-rwxrwx---   0 root         (0) pipx       (999)     3753 2022-10-23 13:52:07.000000 cool-open-client-0.0.9/cool_open_client/client/models/users_response.py
+-rwxrwx---   0 root         (0) pipx       (999)     3131 2022-10-23 13:52:07.000000 cool-open-client-0.0.9/cool_open_client/client/models/users_response_data.py
+-rwxrwx---   0 root         (0) pipx       (999)     3268 2022-10-23 13:52:07.000000 cool-open-client-0.0.9/cool_open_client/client/models/zone_control_fans_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     3300 2022-10-23 13:52:07.000000 cool-open-client-0.0.9/cool_open_client/client/models/zone_control_modes_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     3458 2022-10-23 13:52:07.000000 cool-open-client-0.0.9/cool_open_client/client/models/zone_control_setpoints_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     3330 2022-10-23 13:52:07.000000 cool-open-client-0.0.9/cool_open_client/client/models/zone_control_switches_body.py
+-rwxrwx---   0 root         (0) pipx       (999)     3738 2022-10-23 13:52:07.000000 cool-open-client-0.0.9/cool_open_client/client/models/zone_response.py
+-rwxrwx---   0 root         (0) pipx       (999)     5796 2022-10-23 13:52:07.000000 cool-open-client-0.0.9/cool_open_client/client/models/zone_response_data.py
+-rwxrwx---   0 root         (0) pipx       (999)     3753 2022-10-23 13:52:07.000000 cool-open-client-0.0.9/cool_open_client/client/models/zones_response.py
+-rwxrwx---   0 root         (0) pipx       (999)     3131 2022-10-23 13:52:07.000000 cool-open-client-0.0.9/cool_open_client/client/models/zones_response_data.py
+-rwxrwx---   0 root         (0) pipx       (999)    10644 2022-10-23 13:52:07.000000 cool-open-client-0.0.9/cool_open_client/client/rest.py
+-rwxrwx---   0 root         (0) pipx       (999)    18527 2022-12-24 19:21:10.000000 cool-open-client-0.0.9/cool_open_client/cool_automation_client.py
+-rwxrwx---   0 root         (0) pipx       (999)     2293 2022-08-18 11:53:05.000000 cool-open-client-0.0.9/cool_open_client/hvac_units_factory.py
+-rwxrwx---   0 root         (0) pipx       (999)     7134 2022-09-22 14:03:47.000000 cool-open-client-0.0.9/cool_open_client/unit.py
+drwxrwx---   0 root         (0) pipx       (999)        0 2022-12-24 19:28:57.213472 cool-open-client-0.0.9/cool_open_client/utils/
+-rwxrwx---   0 root         (0) pipx       (999)        0 2022-07-09 18:33:19.000000 cool-open-client-0.0.9/cool_open_client/utils/__init__.py
+-rwxrwx---   0 root         (0) pipx       (999)      583 2022-07-29 19:11:17.000000 cool-open-client-0.0.9/cool_open_client/utils/dict_to_model.py
+-rwxrwx---   0 root         (0) pipx       (999)      913 2022-06-27 14:10:15.000000 cool-open-client-0.0.9/cool_open_client/utils/dictionaries.py
+-rwxrwx---   0 root         (0) pipx       (999)      680 2022-09-17 20:52:54.000000 cool-open-client-0.0.9/cool_open_client/utils/singleton.py
+-rwxrwx---   0 root         (0) pipx       (999)      208 2022-07-28 13:30:00.000000 cool-open-client-0.0.9/cool_open_client/utils/updatable.py
+drwxrwx---   0 root         (0) pipx       (999)        0 2022-12-24 19:28:55.084235 cool-open-client-0.0.9/cool_open_client.egg-info/
+-rwxrwx---   0 root         (0) pipx       (999)      648 2022-12-24 19:28:54.000000 cool-open-client-0.0.9/cool_open_client.egg-info/PKG-INFO
+-rwxrwx---   0 root         (0) pipx       (999)     7315 2022-12-24 19:28:54.000000 cool-open-client-0.0.9/cool_open_client.egg-info/SOURCES.txt
+-rwxrwx---   0 root         (0) pipx       (999)        1 2022-12-24 19:28:54.000000 cool-open-client-0.0.9/cool_open_client.egg-info/dependency_links.txt
+-rwxrwx---   0 root         (0) pipx       (999)      216 2022-12-24 19:28:54.000000 cool-open-client-0.0.9/cool_open_client.egg-info/requires.txt
+-rwxrwx---   0 root         (0) pipx       (999)       23 2022-12-24 19:28:54.000000 cool-open-client-0.0.9/cool_open_client.egg-info/top_level.txt
+-rwxrwx---   0 root         (0) pipx       (999)       99 2022-07-08 19:49:26.000000 cool-open-client-0.0.9/pyproject.toml
+-rwxrwx---   0 root         (0) pipx       (999)       38 2022-12-24 19:28:57.289400 cool-open-client-0.0.9/setup.cfg
+-rwxrwx---   0 root         (0) pipx       (999)     1336 2022-12-24 19:26:08.000000 cool-open-client-0.0.9/setup.py
+drwxrwx---   0 root         (0) pipx       (999)        0 2022-12-24 19:28:57.270128 cool-open-client-0.0.9/tests/
+-rwxrwx---   0 root         (0) pipx       (999)        0 2022-07-26 12:32:25.000000 cool-open-client-0.0.9/tests/__init__.py
+-rwxrwx---   0 root         (0) pipx       (999)     1491 2022-08-15 12:47:20.000000 cool-open-client-0.0.9/tests/test_cool_open_client.py
+-rwxrwx---   0 root         (0) pipx       (999)      684 2022-08-09 08:02:33.000000 cool-open-client-0.0.9/tests/test_hvac_units_factory.py
+-rwxrwx---   0 root         (0) pipx       (999)      692 2022-12-24 19:21:44.000000 cool-open-client-0.0.9/tests/test_websocket.py
```

### Comparing `cool-open-client-0.0.8/LICENSE.md` & `cool-open-client-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/PKG-INFO` & `cool-open-client-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cool-open-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: This library will enable the use of the CoolAutomation API by third party projects
 Home-page: https://github.com/ShayGus/CoolControlOpenClient
 Author: Shay Gus
 Author-email: sgusin@gmail.com
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `cool-open-client-0.0.8/cool_open_client/client/__init__.py` & `cool-open-client-0.0.9/cool_open_client/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/__init__.py` & `cool-open-client-0.0.9/cool_open_client/client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/admins_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/admins_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/authentication_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/authentication_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/customer_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/customer_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/customer_sites_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/customer_sites_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/customer_users_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/customer_users_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/customers_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/customers_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/device_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/device_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/device_units_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/device_units_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/devices_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/devices_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/me_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/me_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/services_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/services_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/site_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/site_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/site_devices_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/site_devices_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/site_systems_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/site_systems_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/site_users_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/site_users_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/site_zones_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/site_zones_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/sites_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/sites_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/system_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/system_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/system_control_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/system_control_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/system_units_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/system_units_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/systems_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/systems_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/unit_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/unit_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/unit_control_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/unit_control_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/units_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/units_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/user_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/users_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/users_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/websocket_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/websocket_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/zone_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/zone_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/zone_control_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/zone_control_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/zone_units_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/zone_units_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api/zones_api.py` & `cool-open-client-0.0.9/cool_open_client/client/api/zones_api.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/api_client.py` & `cool-open-client-0.0.9/cool_open_client/client/api_client.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/configuration.py` & `cool-open-client-0.0.9/cool_open_client/client/configuration.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/__init__.py` & `cool-open-client-0.0.9/cool_open_client/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/authenticate_request_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/authenticate_request_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/bad_response401.py` & `cool-open-client-0.0.9/cool_open_client/client/models/bad_response401.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/bad_response403.py` & `cool-open-client-0.0.9/cool_open_client/client/models/bad_response403.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/bad_response404.py` & `cool-open-client-0.0.9/cool_open_client/client/models/bad_response404.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/bad_response500.py` & `cool-open-client-0.0.9/cool_open_client/client/models/bad_response500.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/control_tree_response.py` & `cool-open-client-0.0.9/cool_open_client/client/models/control_tree_response.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/control_tree_response_data.py` & `cool-open-client-0.0.9/cool_open_client/client/models/control_tree_response_data.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/control_tree_response_data_customers.py` & `cool-open-client-0.0.9/cool_open_client/client/models/control_tree_response_data_customers.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/control_tree_response_data_customers_customer_id.py` & `cool-open-client-0.0.9/cool_open_client/client/models/control_tree_response_data_customers_customer_id.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/control_tree_response_data_customers_customer_id_sites.py` & `cool-open-client-0.0.9/cool_open_client/client/models/control_tree_response_data_customers_customer_id_sites.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/control_tree_response_data_customers_customer_id_sites_site_id.py` & `cool-open-client-0.0.9/cool_open_client/client/models/control_tree_response_data_customers_customer_id_sites_site_id.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/create_customer_request_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/create_customer_request_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/create_device_request_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/create_device_request_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/create_site_request_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/create_site_request_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/create_system_request_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/create_system_request_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/create_user_request_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/create_user_request_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/create_zone_request_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/create_zone_request_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/customer_response.py` & `cool-open-client-0.0.9/cool_open_client/client/models/customer_response.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/customer_response_data.py` & `cool-open-client-0.0.9/cool_open_client/client/models/customer_response_data.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/customers_response.py` & `cool-open-client-0.0.9/cool_open_client/client/models/customers_response.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/customers_response_data.py` & `cool-open-client-0.0.9/cool_open_client/client/models/customers_response_data.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/device_response.py` & `cool-open-client-0.0.9/cool_open_client/client/models/device_response.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/device_response_data.py` & `cool-open-client-0.0.9/cool_open_client/client/models/device_response_data.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/devices_response.py` & `cool-open-client-0.0.9/cool_open_client/client/models/devices_response.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/devices_response_data.py` & `cool-open-client-0.0.9/cool_open_client/client/models/devices_response_data.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/okresponse.py` & `cool-open-client-0.0.9/cool_open_client/client/models/okresponse.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/okresponse_with_id.py` & `cool-open-client-0.0.9/cool_open_client/client/models/okresponse_with_id.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/okresponse_with_id_data.py` & `cool-open-client-0.0.9/cool_open_client/client/models/okresponse_with_id_data.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/okresponse_with_token.py` & `cool-open-client-0.0.9/cool_open_client/client/models/okresponse_with_token.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/okresponse_with_token_data.py` & `cool-open-client-0.0.9/cool_open_client/client/models/okresponse_with_token_data.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/site_response.py` & `cool-open-client-0.0.9/cool_open_client/client/models/site_response.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/site_response_data.py` & `cool-open-client-0.0.9/cool_open_client/client/models/site_response_data.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/sites_response.py` & `cool-open-client-0.0.9/cool_open_client/client/models/sites_response.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/sites_response_data.py` & `cool-open-client-0.0.9/cool_open_client/client/models/sites_response_data.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/system_control_modes_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/system_control_modes_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/system_control_switches_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/system_control_switches_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/system_response.py` & `cool-open-client-0.0.9/cool_open_client/client/models/system_response.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/system_response_data.py` & `cool-open-client-0.0.9/cool_open_client/client/models/system_response_data.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/systems_response.py` & `cool-open-client-0.0.9/cool_open_client/client/models/systems_response.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/systems_response_data.py` & `cool-open-client-0.0.9/cool_open_client/client/models/systems_response_data.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/types_response.py` & `cool-open-client-0.0.9/cool_open_client/client/models/types_response.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/types_response_data.py` & `cool-open-client-0.0.9/cool_open_client/client/models/types_response_data.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_device_types.py` & `cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_device_types.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_device_types_type_object.py` & `cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_device_types_type_object.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_fan_modes.py` & `cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_fan_modes.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_hvac_brands.py` & `cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_hvac_brands.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_hvac_brands_inner.py` & `cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_hvac_brands_inner.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_operation_modes.py` & `cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_operation_modes.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_operation_statuses.py` & `cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_operation_statuses.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_permissions.py` & `cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_permissions.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_resources.py` & `cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_resources.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_roles.py` & `cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_roles.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_swing_modes.py` & `cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_swing_modes.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_temperature_scale.py` & `cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_temperature_scale.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_unit_types.py` & `cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_unit_types.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/types_response_data_week_days.py` & `cool-open-client-0.0.9/cool_open_client/client/models/types_response_data_week_days.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/unit_control_fans_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/unit_control_fans_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/unit_control_modes_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/unit_control_modes_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/unit_control_setpoints_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/unit_control_setpoints_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/unit_control_swings_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/unit_control_swings_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/unit_control_switches_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/unit_control_switches_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/unit_response.py` & `cool-open-client-0.0.9/cool_open_client/client/models/unit_response.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/unit_response_data.py` & `cool-open-client-0.0.9/cool_open_client/client/models/unit_response_data.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/unit_response_data_temperature_limits.py` & `cool-open-client-0.0.9/cool_open_client/client/models/unit_response_data_temperature_limits.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/units_response.py` & `cool-open-client-0.0.9/cool_open_client/client/models/units_response.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/units_response_data.py` & `cool-open-client-0.0.9/cool_open_client/client/models/units_response_data.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/update_customer_request_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/update_customer_request_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/update_device_request_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/update_device_request_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/update_site_request_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/update_site_request_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/update_system_request_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/update_system_request_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/update_unit_request_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/update_unit_request_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/update_user_request_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/update_user_request_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/update_zone_request_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/update_zone_request_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/user_response.py` & `cool-open-client-0.0.9/cool_open_client/client/models/user_response.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/user_response_data.py` & `cool-open-client-0.0.9/cool_open_client/client/models/user_response_data.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/users_response.py` & `cool-open-client-0.0.9/cool_open_client/client/models/users_response.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/users_response_data.py` & `cool-open-client-0.0.9/cool_open_client/client/models/users_response_data.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/zone_control_fans_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/zone_control_fans_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/zone_control_modes_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/zone_control_modes_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/zone_control_setpoints_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/zone_control_setpoints_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/zone_control_switches_body.py` & `cool-open-client-0.0.9/cool_open_client/client/models/zone_control_switches_body.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/zone_response.py` & `cool-open-client-0.0.9/cool_open_client/client/models/zone_response.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/zone_response_data.py` & `cool-open-client-0.0.9/cool_open_client/client/models/zone_response_data.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/zones_response.py` & `cool-open-client-0.0.9/cool_open_client/client/models/zones_response.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/models/zones_response_data.py` & `cool-open-client-0.0.9/cool_open_client/client/models/zones_response_data.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/client/rest.py` & `cool-open-client-0.0.9/cool_open_client/client/rest.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/cool_automation_client.py` & `cool-open-client-0.0.9/cool_open_client/cool_automation_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 
 class CoolAutomationClient(Singleton):
     """
     The coolautomation_client for CoolAutomationCloud service
     """
 
     UNAUTHORIZES_ERROR_CODE = 401
-    SOCKET_URI = "wss://api.coolremote.net/api/v1/"
+    SOCKET_URI = "wss://api.coolremote.net:443/ws/v1"
 
     @classmethod
     async def create(cls, token, logger=None):
         self = cls(logger=logger)
         if token is None:
             raise ValueError("Toke cannot be None")
         self.token = token
```

### Comparing `cool-open-client-0.0.8/cool_open_client/hvac_units_factory.py` & `cool-open-client-0.0.9/cool_open_client/hvac_units_factory.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/unit.py` & `cool-open-client-0.0.9/cool_open_client/unit.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/utils/dict_to_model.py` & `cool-open-client-0.0.9/cool_open_client/utils/dict_to_model.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/utils/dictionaries.py` & `cool-open-client-0.0.9/cool_open_client/utils/dictionaries.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client/utils/singleton.py` & `cool-open-client-0.0.9/cool_open_client/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/cool_open_client.egg-info/PKG-INFO` & `cool-open-client-0.0.9/cool_open_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cool-open-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: This library will enable the use of the CoolAutomation API by third party projects
 Home-page: https://github.com/ShayGus/CoolControlOpenClient
 Author: Shay Gus
 Author-email: sgusin@gmail.com
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `cool-open-client-0.0.8/cool_open_client.egg-info/SOURCES.txt` & `cool-open-client-0.0.9/cool_open_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/setup.py` & `cool-open-client-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 from setuptools import setup, find_packages
 
 path_to_client = str(pathlib.Path(__file__).parent.absolute())
 
 setup(
     name="cool-open-client",
-    version="0.0.8",
+    version="0.0.9",
     author="Shay Gus",
     author_email="sgusin@gmail.com",
     description="This library will enable the use of the CoolAutomation API by third party projects",
     long_description="file:README.md",
     long_description_content_type="text/markdown",
     url="https://github.com/ShayGus/CoolControlOpenClient",
     license="GPLv3+",
```

### Comparing `cool-open-client-0.0.8/tests/test_cool_open_client.py` & `cool-open-client-0.0.9/tests/test_cool_open_client.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/tests/test_hvac_units_factory.py` & `cool-open-client-0.0.9/tests/test_hvac_units_factory.py`

 * *Files identical despite different names*

### Comparing `cool-open-client-0.0.8/tests/test_websocket.py` & `cool-open-client-0.0.9/tests/test_websocket.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-from asyncore import loop
 import unittest
-
+from time import sleep
 import asyncio
 from cool_open_client.cool_automation_client import CoolAutomationClient
 
 
 
 class TestWebSocket(unittest.TestCase):
     def setUp(self):
         self.token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYxZjhkYmFlYThhMzFjMTk2NmIxZWNlYyIsImlhdCI6MTY0OTc2MDQxNiwiZXhwIjoxNjgxMzE4MDE2fQ.RLwz3qiZgLBRwHYpPQGrYtPC3t34axQBh2C7pP_wdVU"
         self.loop = asyncio.get_event_loop()
 
     def test_websocket(self):
         client = self.loop.run_until_complete(CoolAutomationClient.create(self.token))
-        task = self.loop.create_task(client.open_socket())
-        # while not task.done:
-        #     asyncio.slee(10)
-        self.loop.run_until_complete(task)
+        client.open_socket()
+        # sleep(60)
+        # self.loop.run_until_complete(task)
 
 
 if __name__ == "__main__":
     unittest.main()
```

